# Comparing `tmp/cg-35.0.2.tar.gz` & `tmp/cg-36.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-35.0.2.tar", last modified: Thu Jun  8 15:18:09 2023, max compression
+gzip compressed data, was "dist/cg-36.0.1.tar", last modified: Mon Jun 12 13:46:25 2023, max compression
```

## Comparing `cg-35.0.2.tar` & `cg-36.0.1.tar`

### file list

```diff
@@ -1,1263 +1,1268 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-08 15:17:59.000000 cg-35.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-08 15:18:09.000000 cg-35.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-08 15:17:59.000000 cg-35.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 15:17:59.000000 cg-35.0.2/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/dragen_demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/db/models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sample_sheet/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/lims/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-08 15:17:59.000000 cg-35.0.2/cg/apps/tb/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/demultiplex/sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/set/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/upload/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/taxprofiler/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 15:17:59.000000 cg-35.0.2/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-08 15:17:59.000000 cg-35.0.2/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-08 15:17:59.000000 cg-35.0.2/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-08 15:17:59.000000 cg-35.0.2/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77815 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/templates/mip-dna_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    78381 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/report/templates/rnafusion_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/upload/upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-08 15:17:59.000000 cg-35.0.2/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/rnafusion/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/rnafusion/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/taxprofiler/taxprofiler_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 15:17:59.000000 cg-35.0.2/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-06-08 15:17:59.000000 cg-35.0.2/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 15:17:59.000000 cg-35.0.2/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-08 15:17:59.000000 cg-35.0.2/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-08 15:17:59.000000 cg-35.0.2/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    27531 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    30362 2023-06-08 15:17:59.000000 cg-35.0.2/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-08 15:17:59.000000 cg-35.0.2/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40097 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-08 15:18:09.000000 cg-35.0.2/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-08 15:17:59.000000 cg-35.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 15:17:59.000000 cg-35.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:18:09.000000 cg-35.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-08 15:17:59.000000 cg-35.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/demultiplex/test_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/lims/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/lims/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-08 15:17:59.000000 cg-35.0.2/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/test_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/upload/test_cli_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-08 15:17:59.000000 cg-35.0.2/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    74936 2023-06-08 15:17:59.000000 cg-35.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/copy_complete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/run_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/io/example_json.json
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/io/example_xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 15:17:59.000000 cg-35.0.2/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-08 15:17:59.000000 cg-35.0.2/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-08 15:17:59.000000 cg-35.0.2/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-08 15:17:59.000000 cg-35.0.2/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-08 15:17:59.000000 cg-35.0.2/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-08 15:17:59.000000 cg-35.0.2/tests/io/test_io_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-08 15:17:59.000000 cg-35.0.2/tests/io/test_io_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-08 15:17:59.000000 cg-35.0.2/tests/io/test_validate_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15701 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/demultiplex/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/demultiplex/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/demultiplex/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/test_report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/report/test_rnafusion_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/gisaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-08 15:17:59.000000 cg-35.0.2/tests/meta/workflow/test_rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 15:17:59.000000 cg-35.0.2/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-08 15:17:59.000000 cg-35.0.2/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-08 15:17:59.000000 cg-35.0.2/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 15:17:59.000000 cg-35.0.2/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-08 15:17:59.000000 cg-35.0.2/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-08 15:17:59.000000 cg-35.0.2/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27372 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-06-08 15:17:59.000000 cg-35.0.2/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-08 15:17:59.000000 cg-35.0.2/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:18:09.000000 cg-35.0.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:17:59.000000 cg-35.0.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-08 15:17:59.000000 cg-35.0.2/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-08 15:17:59.000000 cg-35.0.2/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-08 15:17:59.000000 cg-35.0.2/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-08 15:17:59.000000 cg-35.0.2/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-08 15:17:59.000000 cg-35.0.2/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-08 15:17:59.000000 cg-35.0.2/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-12 13:46:17.000000 cg-36.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-12 13:46:25.000000 cg-36.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-12 13:46:17.000000 cg-36.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 13:46:17.000000 cg-36.0.1/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/dragen_demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/db/models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sample_sheet/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-12 13:46:17.000000 cg-36.0.1/cg/apps/tb/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/demultiplex/sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/set/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/upload/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/taxprofiler/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 13:46:17.000000 cg-36.0.1/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 13:46:17.000000 cg-36.0.1/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-12 13:46:17.000000 cg-36.0.1/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 13:46:17.000000 cg-36.0.1/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77815 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/templates/mip-dna_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    78381 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/report/templates/rnafusion_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/upload/upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-12 13:46:17.000000 cg-36.0.1/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/rnafusion/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/rnafusion/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/taxprofiler/taxprofiler_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 13:46:17.000000 cg-36.0.1/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-06-12 13:46:17.000000 cg-36.0.1/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-12 13:46:17.000000 cg-36.0.1/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-12 13:46:17.000000 cg-36.0.1/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-12 13:46:17.000000 cg-36.0.1/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27531 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30362 2023-06-12 13:46:17.000000 cg-36.0.1/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-12 13:46:17.000000 cg-36.0.1/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40652 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-12 13:46:25.000000 cg-36.0.1/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 13:46:17.000000 cg-36.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-12 13:46:17.000000 cg-36.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:46:25.000000 cg-36.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-12 13:46:17.000000 cg-36.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/demultiplex/test_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/lims/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/lims/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-12 13:46:17.000000 cg-36.0.1/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/test_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/upload/test_cli_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-12 13:46:17.000000 cg-36.0.1/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75524 2023-06-12 13:46:17.000000 cg-36.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/copy_complete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/CopyComplete.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RTAComplete.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79276 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4459 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/run_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/io/example_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/io/example_xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-12 13:46:17.000000 cg-36.0.1/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-12 13:46:17.000000 cg-36.0.1/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-12 13:46:17.000000 cg-36.0.1/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-12 13:46:17.000000 cg-36.0.1/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-12 13:46:17.000000 cg-36.0.1/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-12 13:46:17.000000 cg-36.0.1/tests/io/test_io_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-12 13:46:17.000000 cg-36.0.1/tests/io/test_io_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-12 13:46:17.000000 cg-36.0.1/tests/io/test_validate_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15896 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/demultiplex/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/demultiplex/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/demultiplex/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/test_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/report/test_rnafusion_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/gisaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-12 13:46:17.000000 cg-36.0.1/tests/meta/workflow/test_rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-12 13:46:17.000000 cg-36.0.1/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-12 13:46:17.000000 cg-36.0.1/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-12 13:46:17.000000 cg-36.0.1/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 13:46:17.000000 cg-36.0.1/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-12 13:46:17.000000 cg-36.0.1/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-12 13:46:17.000000 cg-36.0.1/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27372 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-06-12 13:46:17.000000 cg-36.0.1/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-12 13:46:17.000000 cg-36.0.1/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:25.000000 cg-36.0.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:46:17.000000 cg-36.0.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 13:46:17.000000 cg-36.0.1/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-12 13:46:17.000000 cg-36.0.1/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 13:46:17.000000 cg-36.0.1/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-12 13:46:17.000000 cg-36.0.1/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-12 13:46:17.000000 cg-36.0.1/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-12 13:46:17.000000 cg-36.0.1/tests/utils/test_utils.py
```

### Comparing `cg-35.0.2/PKG-INFO` & `cg-36.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 35.0.2
+Version: 36.0.1
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-35.0.2/README.md` & `cg-36.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/crud/create.py` & `cg-36.0.1/cg/apps/cgstats/crud/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     Project,
     Supportparams,
     Sample,
     Unaligned,
 )
 from cg.apps.cgstats.stats import StatsAPI
 from cg.apps.demultiplex.sample_sheet.models import (
-    FlowCellSample,
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleDragen,
+    FlowCellSampleNovaSeq6000,
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
     SampleSheet,
 )
 from cg.constants.demultiplexing import DRAGEN_PASSED_FILTER_PCT, BclConverter
 from cg.constants.symbols import PERIOD
 from cg.models.demultiplex.demux_results import DemuxResults, LogfileParameters
 
 LOG = logging.getLogger(__name__)
@@ -207,15 +207,15 @@
             manager=manager, project_name=project_name
         )
         project_name_to_id[project_name] = project.project_id
     return project_name_to_id
 
 
 def get_or_create_sample(
-    manager: StatsAPI, sample: FlowCellSample, project_name_to_id: Dict[str, int]
+    manager: StatsAPI, sample: FlowCellSampleNovaSeq6000, project_name_to_id: Dict[str, int]
 ) -> Sample:
     """Create a new Sample object in the cgstats database if it doesn't already exist."""
 
     if sample.project == "indexcheck":
         LOG.debug("Skip adding indexcheck sample to database")
         return None
 
@@ -249,15 +249,15 @@
     tables in cgstats for samples demultiplexed with Dragen"""
 
     demux_samples: Dict[int, dict] = manager.find_handler.get_dragen_demux_samples(
         demux_results=demux_results,
         sample_sheet=sample_sheet,
     )
 
-    sample: FlowCellSampleDragen
+    sample: FlowCellSampleNovaSeq6000Dragen
     for sample in sample_sheet.samples:
         stats_sample: Sample = get_or_create_sample(
             manager=manager, sample=sample, project_name_to_id=project_name_to_id
         )
 
         if not stats_sample:
             continue
@@ -285,15 +285,15 @@
 
     demux_samples: Dict[int, Dict[str, DemuxSample]] = manager.find_handler.get_demux_samples(
         conversion_stats=demux_results.conversion_stats,
         demux_stats_path=demux_results.demux_stats_path,
         sample_sheet=sample_sheet,
     )
 
-    sample: FlowCellSampleBcl2Fastq
+    sample: FlowCellSampleNovaSeq6000Bcl2Fastq
     for sample in sample_sheet.samples:
         stats_sample: Sample = get_or_create_sample(
             manager=manager, sample=sample, project_name_to_id=project_name_to_id
         )
 
         if not stats_sample:
             continue
```

### Comparing `cg-35.0.2/cg/apps/cgstats/crud/delete.py` & `cg-36.0.1/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/crud/find.py` & `cg-36.0.1/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/base.py` & `cg-36.0.1/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/datasource.py` & `cg-36.0.1/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/demux.py` & `cg-36.0.1/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/demux_sample.py` & `cg-36.0.1/cg/apps/cgstats/db/models/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/dragen_demux_sample.py` & `cg-36.0.1/cg/apps/cgstats/db/models/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/sample.py` & `cg-36.0.1/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/support_params.py` & `cg-36.0.1/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/unaligned.py` & `cg-36.0.1/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/db/models/version.py` & `cg-36.0.1/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-36.0.1/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-36.0.1/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/parsers/demux_stats.py` & `cg-36.0.1/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-36.0.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-36.0.1/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/parsers/run_info.py` & `cg-36.0.1/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/cgstats/stats.py` & `cg-36.0.1/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/coverage/api.py` & `cg-36.0.1/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/crunchy/crunchy.py` & `cg-36.0.1/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/crunchy/files.py` & `cg-36.0.1/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/crunchy/sbatch.py` & `cg-36.0.1/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/demultiplex/demultiplex_api.py` & `cg-36.0.1/cg/apps/demultiplex/demultiplex_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cg.apps.demultiplex.sbatch import DEMULTIPLEX_COMMAND, DEMULTIPLEX_ERROR
 from cg.apps.slurm.slurm_api import SlurmAPI
 from cg.apps.tb import TrailblazerAPI
 from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles, BclConverter
 from cg.constants.priority import SlurmQos
 from cg.io.controller import WriteFile
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.models.demultiplex.sbatch import SbatchCommand, SbatchError
 from cg.models.slurm.sbatch import Sbatch, SbatchDragen
 from cgmodels.cg.constants import Pipeline
 
 LOG = logging.getLogger(__name__)
 
 
@@ -46,15 +46,15 @@
         """Set dry run."""
         LOG.debug(f"Set dry run to {dry_run}")
         self.dry_run = dry_run
         self.slurm_api.set_dry_run(dry_run=dry_run)
 
     @staticmethod
     def get_sbatch_error(
-        flow_cell: FlowCell,
+        flow_cell: FlowCellDirectoryData,
         email: str,
         demux_dir: Path,
     ) -> str:
         """Create the sbatch error string."""
         LOG.info("Creating the sbatch error string")
         error_parameters: SbatchError = SbatchError(
             flow_cell_id=flow_cell.id,
@@ -67,15 +67,15 @@
 
     @staticmethod
     def get_sbatch_command(
         run_dir: Path,
         unaligned_dir: Path,
         sample_sheet: Path,
         demux_completed: Path,
-        flow_cell: FlowCell,
+        flow_cell: FlowCellDirectoryData,
         environment: Literal["production", "stage"] = "stage",
     ) -> str:
         """Return sbatch command."""
         LOG.info("Creating the sbatch command string")
         command_parameters: SbatchCommand = SbatchCommand(
             run_dir=run_dir.as_posix(),
             demux_dir=unaligned_dir.parent.as_posix(),
@@ -83,71 +83,71 @@
             sample_sheet=sample_sheet.as_posix(),
             demux_completed_file=demux_completed.as_posix(),
             environment=environment,
         )
         return DEMULTIPLEX_COMMAND[flow_cell.bcl_converter].format(**command_parameters.dict())
 
     @staticmethod
-    def demultiplex_sbatch_path(flow_cell: FlowCell) -> Path:
+    def demultiplex_sbatch_path(flow_cell: FlowCellDirectoryData) -> Path:
         """Get the path to where sbatch script file should be kept."""
         return Path(flow_cell.path, "demux-novaseq.sh")
 
     @staticmethod
-    def get_run_name(flow_cell: FlowCell) -> str:
+    def get_run_name(flow_cell: FlowCellDirectoryData) -> str:
         """Create the run name for the sbatch job."""
         return f"{flow_cell.id}_demultiplex"
 
     @staticmethod
-    def get_stderr_logfile(flow_cell: FlowCell) -> Path:
+    def get_stderr_logfile(flow_cell: FlowCellDirectoryData) -> Path:
         """Create the path to the stderr logfile."""
         return Path(flow_cell.path, f"{DemultiplexingAPI.get_run_name(flow_cell)}.stderr")
 
     @staticmethod
-    def get_stdout_logfile(flow_cell: FlowCell) -> Path:
+    def get_stdout_logfile(flow_cell: FlowCellDirectoryData) -> Path:
         """Create the path to the stdout logfile."""
         return Path(flow_cell.path, f"{DemultiplexingAPI.get_run_name(flow_cell)}.stdout")
 
     def get_all_demultiplexed_flow_cell_dirs(self) -> List[Path]:
         """Return all demultiplex flow cell out directories."""
         demultiplex_flow_cells: List[Path] = []
         for flow_cell_dir in self.out_dir.iterdir():
             if flow_cell_dir.is_dir():
                 LOG.debug(f"Found directory {flow_cell_dir}")
                 demultiplex_flow_cells.append(flow_cell_dir)
         return demultiplex_flow_cells
 
-    def flow_cell_out_dir_path(self, flow_cell: FlowCell) -> Path:
+    def flow_cell_out_dir_path(self, flow_cell: FlowCellDirectoryData) -> Path:
         """Create the path to where the demuliplexed result should be produced."""
         return Path(self.out_dir, flow_cell.path.name)
 
-    def unaligned_dir_path(self, flow_cell: FlowCell) -> Path:
+    def unaligned_dir_path(self, flow_cell: FlowCellDirectoryData) -> Path:
         """Create the path to where the demuliplexed result should be produced."""
         return Path(
             self.flow_cell_out_dir_path(flow_cell), DemultiplexingDirsAndFiles.UNALIGNED_DIR_NAME
         )
 
-    def demultiplexing_completed_path(self, flow_cell: FlowCell) -> Path:
+    def demultiplexing_completed_path(self, flow_cell: FlowCellDirectoryData) -> Path:
         """Return the path to demultiplexing complete file."""
         LOG.info(
             Path(self.flow_cell_out_dir_path(flow_cell), DemultiplexingDirsAndFiles.DEMUX_COMPLETE)
         )
         return Path(
             self.flow_cell_out_dir_path(flow_cell), DemultiplexingDirsAndFiles.DEMUX_COMPLETE
         )
 
-    def is_demultiplexing_completed(self, flow_cell: FlowCell) -> bool:
+    def is_demultiplexing_completed(self, flow_cell: FlowCellDirectoryData) -> bool:
         """Check the path to where the demuliplexed result should be produced."""
         LOG.info(f"Check if demultiplexing is ready for {flow_cell.path}")
         logfile: Path = self.get_stderr_logfile(flow_cell)
         if not logfile.exists():
             LOG.warning("Could not find logfile!")
             return False
         return self.demultiplexing_completed_path(flow_cell).exists()
 
-    def is_demultiplexing_possible(self, flow_cell: FlowCell) -> bool:
+    def is_demultiplexing_possible(self, flow_cell: FlowCellDirectoryData) -> bool:
         """Check if it is possible to start demultiplexing.
 
         This means that
             - flow cell should be ready for demultiplexing (all files in place)
             - sample sheet needs to exist
             - demultiplexing should not be running
         """
@@ -187,15 +187,17 @@
     def write_trailblazer_config(content: dict, file_path: Path) -> None:
         """Write the content to a yaml file"""
         LOG.info(f"Writing yaml content {content} to {file_path}")
         WriteFile.write_file_from_content(
             content=content, file_format=FileFormat.YAML, file_path=file_path
         )
 
-    def add_to_trailblazer(self, tb_api: TrailblazerAPI, slurm_job_id: int, flow_cell: FlowCell):
+    def add_to_trailblazer(
+        self, tb_api: TrailblazerAPI, slurm_job_id: int, flow_cell: FlowCellDirectoryData
+    ):
         """Add demultiplexing entry to trailblazer."""
         if self.dry_run:
             return
         self.write_trailblazer_config(
             content=self.get_trailblazer_config(slurm_job_id=slurm_job_id),
             file_path=flow_cell.trailblazer_config_path,
         )
@@ -205,15 +207,15 @@
             config_path=flow_cell.trailblazer_config_path.as_posix(),
             out_dir=flow_cell.trailblazer_config_path.parent.as_posix(),
             slurm_quality_of_service=self.slurm_quality_of_service,
             email=self.mail,
             data_analysis=str(Pipeline.DEMULTIPLEX),
         )
 
-    def start_demultiplexing(self, flow_cell: FlowCell):
+    def start_demultiplexing(self, flow_cell: FlowCellDirectoryData):
         """Start demultiplexing for a flow cell."""
         self.create_demultiplexing_started_file(flow_cell.demultiplexing_started_path)
         demux_dir: Path = self.flow_cell_out_dir_path(flow_cell=flow_cell)
         unaligned_dir: Path = self.unaligned_dir_path(flow_cell=flow_cell)
         LOG.info(f"Demultiplexing to {unaligned_dir}")
         if not self.dry_run:
             LOG.info(f"Creating demux dir {unaligned_dir}")
```

### Comparing `cg-35.0.2/cg/apps/demultiplex/demux_report.py` & `cg-36.0.1/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/demultiplex/sample_sheet/create.py` & `cg-36.0.1/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from typing_extensions import Literal
 
 from cg.apps.demultiplex.sample_sheet.novaseq_sample_sheet import SampleSheetCreator
 from cg.apps.demultiplex.sample_sheet.models import FlowCellSample
 from cg.constants.sequencing import Sequencers
 from cg.constants.demultiplexing import BclConverter
 from cg.exc import FlowCellError
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 def create_sample_sheet(
     bcl_converter: Literal[BclConverter.BCL2FASTQ, BclConverter.DRAGEN],
-    flow_cell: FlowCell,
+    flow_cell: FlowCellDirectoryData,
     lims_samples: List[FlowCellSample],
     force: bool = False,
 ) -> List[List[str]]:
     """Create a sample sheet for a flow cell."""
     if flow_cell.sample_sheet_path.exists():
         message = f"Sample sheet {flow_cell.sample_sheet_path} already exists!"
         LOG.warning(message)
@@ -33,8 +33,11 @@
 
     sample_sheet_creator = SampleSheetCreator(
         bcl_converter=bcl_converter,
         flow_cell=flow_cell,
         lims_samples=lims_samples,
         force=force,
     )
+    LOG.info(
+        f"Constructing a {bcl_converter} sample sheet for the {flow_cell_sequencer} flow cell {flow_cell.id}"
+    )
     return sample_sheet_creator.construct_sample_sheet()
```

### Comparing `cg-35.0.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-36.0.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Functions that deals with dummy samples"""
 from cg.apps.demultiplex.sample_sheet.models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleDragen,
+    FlowCellSample,
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
 )
 from cg.constants.demultiplexing import BclConverter
-from typing import Union
+from typing import Type
 
 
 def dummy_sample_name(sample_name: str) -> str:
     """Convert a string to a dummy sample name replacing spaces and parentheses with dashes."""
     return sample_name.replace(" ", "-").replace("(", "-").replace(")", "-")
 
 
 def dummy_sample(
-    flow_cell_id: str, dummy_index: str, lane: int, name: str, bcl_converter: str
-) -> Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen]:
+    flow_cell_id: str, dummy_index: str, lane: int, name: str, sample_type: Type[FlowCellSample]
+) -> FlowCellSample:
     """Constructs and returns a dummy sample in Novaseq sample sheet format."""
-    flowcell_sample = {
-        BclConverter.BCL2FASTQ.value: FlowCellSampleBcl2Fastq,
-        BclConverter.DRAGEN.value: FlowCellSampleDragen,
-    }
-    return flowcell_sample[bcl_converter](
+    return sample_type(
         flowcell_id=flow_cell_id,
         lane=lane,
         sample_id=dummy_sample_name(sample_name=name),
         index=dummy_index,
         sample_name="indexcheck",
         project="indexcheck",
     )
```

### Comparing `cg-35.0.2/cg/apps/demultiplex/sample_sheet/index.py` & `cg-36.0.1/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-36.0.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """ Create a sample sheet for Novaseq flow cells."""
 
 import logging
-from typing import Dict, List, Set
+from typing import Dict, List, Set, Type
 
 from cg.apps.demultiplex.sample_sheet import index
 from cg.apps.demultiplex.sample_sheet.dummy_sample import dummy_sample
 from cg.apps.demultiplex.sample_sheet.index import Index
 from cg.apps.demultiplex.sample_sheet.validate import validate_sample_sheet
 from cg.apps.demultiplex.sample_sheet.models import FlowCellSample
 from cg.constants.demultiplexing import SampleSheetNovaSeq6000Sections
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.models.demultiplex.run_parameters import RunParameters
 
 LOG = logging.getLogger(__name__)
 
 
 class SampleSheetCreator:
     """Create a raw sample sheet for Novaseq flow cells."""
 
     def __init__(
         self,
         bcl_converter: str,
-        flow_cell: FlowCell,
+        flow_cell: FlowCellDirectoryData,
         lims_samples: List[FlowCellSample],
         force: bool = False,
     ):
         self.bcl_converter = bcl_converter
         self.flow_cell_id: str = flow_cell.id
         self.lims_samples: List[FlowCellSample] = lims_samples
         self.run_parameters: RunParameters = flow_cell.run_parameters
+        self.sample_type: Type[FlowCellSample] = flow_cell.sample_type
         self.force = force
 
     @property
     def valid_indexes(self) -> List[Index]:
         return index.get_valid_indexes(dual_indexes_only=True)
 
     def add_dummy_samples(self) -> None:
@@ -50,15 +51,15 @@
                     LOG.debug(f"Index {index_obj.sequence} already in use")
                     continue
                 dummy_flow_cell_sample: FlowCellSample = dummy_sample(
                     flow_cell_id=self.flow_cell_id,
                     dummy_index=index_obj.sequence,
                     lane=lane,
                     name=index_obj.name,
-                    bcl_converter=self.bcl_converter,
+                    sample_type=self.sample_type,
                 )
                 LOG.debug(f"Adding dummy sample {dummy_flow_cell_sample} to lane {lane}")
                 self.lims_samples.append(dummy_flow_cell_sample)
 
     def remove_unwanted_samples(self) -> None:
         """Filter out samples with indexes of unwanted length and single indexes."""
         LOG.info("Removing all samples without dual indexes")
@@ -70,21 +71,21 @@
                 continue
             samples_to_keep.append(sample)
         self.lims_samples = samples_to_keep
 
     @staticmethod
     def convert_sample_to_header_dict(
         sample: FlowCellSample,
-        sample_sheet_headers: List[str],
+        data_column_names: List[str],
     ) -> List[str]:
         """Convert a lims sample object to a dict with keys that corresponds to the sample sheet
         headers."""
-        LOG.debug(f"Use sample sheet header {sample_sheet_headers}")
+        LOG.debug(f"Use sample sheet header {data_column_names}")
         sample_dict = sample.dict(by_alias=True)
-        return [str(sample_dict[header]) for header in sample_sheet_headers]
+        return [str(sample_dict[column]) for column in data_column_names]
 
     def get_additional_sections_sample_sheet(self) -> List[List[str]]:
         """Build all sections of the sample sheet that is not the Data section."""
         return [
             [SampleSheetNovaSeq6000Sections.Settings.HEADER.value],
             SampleSheetNovaSeq6000Sections.Settings.BARCODE_MISMATCH_INDEX1.value,
             SampleSheetNovaSeq6000Sections.Settings.BARCODE_MISMATCH_INDEX2.value,
@@ -103,24 +104,21 @@
         sample_sheet_content: List[List[str]] = (
             self.get_additional_sections_sample_sheet() + self.get_data_section_header_and_columns()
         )
         for sample in self.lims_samples:
             sample_sheet_content.append(
                 self.convert_sample_to_header_dict(
                     sample=sample,
-                    sample_sheet_headers=SampleSheetNovaSeq6000Sections.Data.COLUMN_NAMES.value[
-                        self.bcl_converter
-                    ],
+                    data_column_names=self.get_data_section_header_and_columns()[1],
                 )
             )
         return sample_sheet_content
 
     def construct_sample_sheet(self) -> List[List[str]]:
         """Construct the sample sheet."""
-        LOG.info(f"Constructing sample sheet for {self.flow_cell_id}")
         # Create dummy samples for the indexes that is missing
         if self.run_parameters.requires_dummy_samples:
             self.add_dummy_samples()
         else:
             LOG.info("Skip adding dummy samples since run is not WGS")
         self.remove_unwanted_samples()
         index.adapt_indexes(
@@ -130,11 +128,11 @@
         sample_sheet_content: List[List[str]] = self.create_sample_sheet_content()
         if self.force:
             LOG.info("Skipping validation of sample sheet due to force flag")
             return sample_sheet_content
         LOG.info("Validating sample sheet")
         validate_sample_sheet(
             sample_sheet_content=sample_sheet_content,
-            bcl_converter=self.bcl_converter,
+            sample_type=self.sample_type,
         )
         LOG.info("Sample sheet passed validation")
         return sample_sheet_content
```

### Comparing `cg-35.0.2/cg/apps/demultiplex/sample_sheet/validate.py` & `cg-36.0.1/cg/apps/demultiplex/sample_sheet/validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import Dict, List, Type, Union
 from pydantic import parse_obj_as
 from typing_extensions import Literal
 
 from cg.apps.demultiplex.sample_sheet.models import (
     FlowCellSample,
     SampleSheet,
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleDragen,
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
 )
 from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import (
     BclConverter,
     SampleSheetNovaSeq6000Sections,
 )
 from cg.exc import SampleSheetError
@@ -29,15 +29,17 @@
         if sample_id in sample_ids:
             message: str = f"Sample {sample.sample_id} exists multiple times in sample sheet"
             LOG.warning(message)
             raise SampleSheetError(message)
         sample_ids.add(sample_id)
 
 
-def get_samples_by_lane(samples: List[FlowCellSample]) -> Dict[int, List[FlowCellSample]]:
+def get_samples_by_lane(
+    samples: List[FlowCellSample],
+) -> Dict[int, List[FlowCellSample]]:
     """Group and return samples by lane."""
     LOG.info("Order samples by lane")
     sample_by_lane: Dict[int, List[FlowCellSample]] = {}
     for sample in samples:
         if sample.lane not in sample_by_lane:
             sample_by_lane[sample.lane] = []
         sample_by_lane[sample.lane].append(sample)
@@ -77,35 +79,28 @@
         LOG.warning(message)
         raise SampleSheetError(message)
     return raw_samples
 
 
 def validate_sample_sheet(
     sample_sheet_content: List[List[str]],
-    bcl_converter: Literal[BclConverter.BCL2FASTQ, BclConverter.DRAGEN],
+    sample_type: Type[FlowCellSample],
 ) -> SampleSheet:
     """Return a validated sample sheet object."""
-    novaseq_sample: Dict[str, Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen]] = {
-        BclConverter.BCL2FASTQ.value: FlowCellSampleBcl2Fastq,
-        BclConverter.DRAGEN.value: FlowCellSampleDragen,
-    }
     raw_samples: List[Dict[str, str]] = get_raw_samples(sample_sheet_content=sample_sheet_content)
-    sample_type: Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen] = novaseq_sample[
-        bcl_converter
-    ]
     samples = parse_obj_as(List[sample_type], raw_samples)
     validate_samples_unique_per_lane(samples=samples)
     return SampleSheet(samples=samples)
 
 
 def get_sample_sheet_from_file(
     infile: Path,
-    bcl_converter: Literal[BclConverter.BCL2FASTQ, BclConverter.DRAGEN],
+    flow_cell_sample_type: Type[FlowCellSample],
 ) -> SampleSheet:
     """Parse and validate a sample sheet from file."""
     sample_sheet_content: List[List[str]] = ReadFile.get_content_from_file(
         file_format=FileFormat.CSV, file_path=infile
     )
     return validate_sample_sheet(
         sample_sheet_content=sample_sheet_content,
-        bcl_converter=bcl_converter,
+        sample_type=flow_cell_sample_type,
     )
```

### Comparing `cg-35.0.2/cg/apps/demultiplex/sbatch.py` & `cg-36.0.1/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/gens.py` & `cg-36.0.1/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/gt.py` & `cg-36.0.1/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/hermes/hermes_api.py` & `cg-36.0.1/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/hermes/models.py` & `cg-36.0.1/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/housekeeper/hk.py` & `cg-36.0.1/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/invoice/render.py` & `cg-36.0.1/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-36.0.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-36.0.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-36.0.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-36.0.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/lims/api.py` & `cg-36.0.1/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/lims/batch.py` & `cg-36.0.1/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/lims/order.py` & `cg-36.0.1/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/lims/sample_sheet.py` & `cg-36.0.1/cg/apps/lims/sample_sheet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Functions to get sample sheet information from Lims."""
 import logging
 import re
-from typing import Iterable, List, Optional, Union
+from typing import Iterable, List, Optional, Type
 
 from genologics.entities import Artifact, Container, Sample
 from genologics.lims import Lims
 
-from cg.apps.demultiplex.sample_sheet.models import FlowCellSampleBcl2Fastq, FlowCellSampleDragen
-from cg.constants.demultiplexing import BclConverter
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSample
 
 LOG = logging.getLogger(__name__)
 
 
 def get_placement_lane(lane: str) -> int:
     """Parse out the lane information from an artifact.placement."""
     return int(lane.split(":")[0])
@@ -62,36 +61,35 @@
     match = extract_sequence_in_parentheses(label=label)
     if match:
         assert match == sequence
 
     return sequence
 
 
-def flow_cell_samples(
-    lims: Lims, flowcell_id: str, bcl_converter: str
-) -> Iterable[Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen]]:
-    lims_flowcell_sample = {
-        BclConverter.BCL2FASTQ.value: FlowCellSampleBcl2Fastq,
-        BclConverter.DRAGEN.value: FlowCellSampleDragen,
-    }
-    LOG.info(f"Fetching samples from lims for flowcell {flowcell_id}")
-    containers: List[Container] = lims.get_containers(name=flowcell_id)
+def get_flow_cell_samples(
+    lims: Lims,
+    flow_cell_id: str,
+    flow_cell_sample_type: Type[FlowCellSample],
+) -> Iterable[FlowCellSample]:
+    """Return samples from LIMS for a given flow cell."""
+    LOG.info(f"Fetching samples from lims for flowcell {flow_cell_id}")
+    containers: List[Container] = lims.get_containers(name=flow_cell_id)
     if not containers:
         return []
     container: Container = containers[-1]  # only take the last one. See ÖA#217.
     raw_lanes: List[str] = sorted(container.placements.keys())
     for raw_lane in raw_lanes:
         lane: int = get_placement_lane(raw_lane)
         placement_artifact: Artifact = container.placements[raw_lane]
         non_pooled_artifacts: List[Artifact] = get_non_pooled_artifacts(placement_artifact)
         for artifact in non_pooled_artifacts:
             sample: Sample = artifact.samples[0]  # we are assured it only has one sample
             label: Optional[str] = get_reagent_label(artifact)
             index = get_index(lims=lims, label=label)
-            yield lims_flowcell_sample[bcl_converter](
-                flowcell_id=flowcell_id,
+            yield flow_cell_sample_type(
+                flowcell_id=flow_cell_id,
                 lane=lane,
                 sample_id=sample.id,
                 index=index,
                 sample_name=sample.name,
                 project=sample.project.name,
             )
```

### Comparing `cg-35.0.2/cg/apps/loqus.py` & `cg-36.0.1/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/madeline/api.py` & `cg-36.0.1/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/mip/confighandler.py` & `cg-36.0.1/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/mutacc_auto.py` & `cg-36.0.1/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/orderform/excel_orderform_parser.py` & `cg-36.0.1/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/orderform/json_orderform_parser.py` & `cg-36.0.1/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/orderform/orderform_parser.py` & `cg-36.0.1/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/osticket.py` & `cg-36.0.1/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/scout/scout_export.py` & `cg-36.0.1/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/scout/scoutapi.py` & `cg-36.0.1/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/api.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-36.0.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/slurm/sbatch.py` & `cg-36.0.1/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/slurm/slurm_api.py` & `cg-36.0.1/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/tb/api.py` & `cg-36.0.1/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/apps/tb/models.py` & `cg-36.0.1/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/add.py` & `cg-36.0.1/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/backup.py` & `cg-36.0.1/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/base.py` & `cg-36.0.1/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/clean.py` & `cg-36.0.1/cg/cli/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     rsync_past_run_dirs,
     microsalt_past_run_dirs,
 )
 from cg.constants import FlowCellStatus
 from cg.constants.constants import DRY_RUN, SKIP_CONFIRMATION
 from cg.constants.sequencing import Sequencers
 from cg.constants.housekeeper_tags import SequencingFileTag, ALIGNMENT_FILE_TAGS, ScoutTag
-from cg.models.demultiplex.flow_cell import FlowCell as DemultiplexFlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData as DemultiplexFlowCell
 from cg.utils.date import get_timedelta_from_date, get_date_days_ago
 from cg.exc import FlowCellError, HousekeeperBundleVersionMissingError
 from cg.meta.clean.api import CleanAPI
 from cg.meta.clean.demultiplexed_flow_cells import DemultiplexedRunsFlowCell
 from cg.meta.clean.flow_cell_run_directories import RunDirFlowCell
 from cg.models.cg_config import CGConfig
 from cg.store import Store
```

### Comparing `cg-35.0.2/cg/cli/compress/base.py` & `cg-36.0.1/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/compress/fastq.py` & `cg-36.0.1/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/compress/helpers.py` & `cg-36.0.1/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/delete/base.py` & `cg-36.0.1/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/delete/case.py` & `cg-36.0.1/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/delete/cases.py` & `cg-36.0.1/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/delete/observations.py` & `cg-36.0.1/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/deliver/base.py` & `cg-36.0.1/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/demultiplex/add.py` & `cg-36.0.1/cg/cli/demultiplex/add.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.constants.cgstats import STATS_HEADER
 from cg.constants.demultiplexing import OPTION_BCL_CONVERTER
 from cg.exc import FlowCellError
 from cg.meta.demultiplex.demux_post_processing import DemuxPostProcessingNovaseqAPI
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 @click.command(name="add")
 @OPTION_BCL_CONVERTER
 @click.argument("flow-cell-name")
@@ -35,15 +35,15 @@
         LOG.warning(f"Could not find flow cell path {flow_cell_run_path}")
         raise click.Abort
     demux_results_path: Path = Path(demultiplex_api.out_dir, flow_cell_name)
     if not demux_results_path.exists():
         LOG.warning(f"Could not find demultiplex result path {demux_results_path}")
         raise click.Abort
     try:
-        flow_cell: FlowCell = FlowCell(
+        flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
             flow_cell_path=flow_cell_run_path, bcl_converter=bcl_converter
         )
     except FlowCellError as error:
         raise click.Abort from error
     demux_results: DemuxResults = DemuxResults(
         demux_dir=demux_results_path, flow_cell=flow_cell, bcl_converter=bcl_converter
     )
```

### Comparing `cg-35.0.2/cg/cli/demultiplex/base.py` & `cg-36.0.1/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/demultiplex/demux.py` & `cg-36.0.1/cg/cli/demultiplex/demux.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.tb import TrailblazerAPI
 from cg.constants.demultiplexing import OPTION_BCL_CONVERTER
 from cg.exc import FlowCellError
 from cg.meta.demultiplex.delete_demultiplex_api import DeleteDemuxAPI
 from cg.models.cg_config import CGConfig
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 DRY_RUN = click.option("--dry-run", is_flag=True)
 
 
 @click.command(name="all")
@@ -35,15 +35,15 @@
     tb_api: TrailblazerAPI = context.trailblazer_api
     LOG.info(f"Search for flow cells ready to demultiplex in {flow_cells_directory}")
     for sub_dir in flow_cells_directory.iterdir():
         if not sub_dir.is_dir():
             continue
         LOG.info(f"Found directory {sub_dir}")
         try:
-            flow_cell = FlowCell(flow_cell_path=sub_dir, bcl_converter=bcl_converter)
+            flow_cell = FlowCellDirectoryData(flow_cell_path=sub_dir, bcl_converter=bcl_converter)
         except FlowCellError:
             continue
 
         if not demultiplex_api.is_demultiplexing_possible(flow_cell=flow_cell) and not dry_run:
             continue
 
         if not flow_cell.validate_sample_sheet():
@@ -95,15 +95,17 @@
 
     demultiplex_api: DemultiplexingAPI = context.demultiplex_api
     demultiplex_api.set_dry_run(dry_run=dry_run)
     LOG.info(f"setting flow cell id to {flow_cell_name}")
     LOG.info(f"setting out dir to {demultiplex_api.out_dir}")
 
     try:
-        flow_cell = FlowCell(flow_cell_path=flow_cell_directory, bcl_converter=bcl_converter)
+        flow_cell = FlowCellDirectoryData(
+            flow_cell_path=flow_cell_directory, bcl_converter=bcl_converter
+        )
     except FlowCellError as error:
         raise click.Abort from error
 
     delete_demux_api: DeleteDemuxAPI = DeleteDemuxAPI(
         config=context,
         demultiplex_base=demultiplex_api.out_dir,
         dry_run=dry_run,
```

### Comparing `cg-35.0.2/cg/cli/demultiplex/finish.py` & `cg-36.0.1/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/demultiplex/report.py` & `cg-36.0.1/cg/cli/demultiplex/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 import click
 from cg.apps.cgstats.parsers.conversion_stats import ConversionStats
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.demultiplex.demux_report import create_demux_report
 from cg.exc import FlowCellError
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 @click.command(name="report")
 @click.argument("flow-cell-name")
 @click.pass_obj
 def create_report_cmd(context: CGConfig, flow_cell_name: str):
     """Generate a demux report and print to stdout."""
     LOG.info(f"Check demuxed flowcell {flow_cell_name}")
     demux_api: DemultiplexingAPI = context.demultiplex_api
     try:
-        flow_cell: FlowCell = FlowCell(flow_cell_path=Path(demux_api.run_dir, flow_cell_name))
+        flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+            flow_cell_path=Path(demux_api.run_dir, flow_cell_name)
+        )
     except FlowCellError as error:
         raise click.Abort from error
     demux_results: DemuxResults = DemuxResults(
         demux_dir=Path(demux_api.out_dir, flow_cell_name, flow_cell=flow_cell)
     )
     conversion_stats: Path = demux_results.conversion_stats_path
     if not conversion_stats.exists():
```

### Comparing `cg-35.0.2/cg/cli/demultiplex/sample_sheet.py` & `cg-36.0.1/cg/cli/demultiplex/sample_sheet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 import logging
 from pathlib import Path
-from typing import List, Union
+from typing import List
 
 import click
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.demultiplex.sample_sheet.create import create_sample_sheet
-from cg.apps.demultiplex.sample_sheet.models import (
-    FlowCellSample,
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleDragen,
-)
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.validate import get_sample_sheet_from_file
-from cg.apps.lims.sample_sheet import flow_cell_samples
+from cg.apps.lims.sample_sheet import get_flow_cell_samples
 from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import OPTION_BCL_CONVERTER
 from cg.exc import FlowCellError
 from cg.io.controller import WriteFile, WriteStream
 from cg.models.cg_config import CGConfig
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from pydantic import ValidationError
 
 LOG = logging.getLogger(__name__)
 
 
 @click.group(name="samplesheet")
 def sample_sheet_commands():
     """Command group for the sample sheet commands."""
 
 
 @sample_sheet_commands.command(name="validate")
+@click.argument("flow-cell-name")
 @click.argument("sheet", type=click.Path(exists=True, dir_okay=False))
 @OPTION_BCL_CONVERTER
+@click.pass_obj
 def validate_sample_sheet(
+    context: CGConfig,
+    flow_cell_name: str,
     bcl_converter: str,
     sheet: click.Path,
 ):
-    """Validate a sample sheet."""
+    """Validate a sample sheet.
+    flow-cell-name is the flow cell run directory name, e.g. '201203_A00689_0200_AHVKJCDRXX'
+    """
+
+    flow_cell_path: Path = Path(context.demultiplex_api.run_dir, flow_cell_name)
+    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=flow_cell_path, bcl_converter=bcl_converter
+    )
     LOG.info(
-        f"Validating sample sheet {sheet}",
+        f"Validating {sheet} as a {flow_cell.sequencer_type} {bcl_converter} sample sheet",
     )
     sheet: Path = Path(str(sheet))
     try:
-        get_sample_sheet_from_file(infile=sheet, bcl_converter=bcl_converter)
+        get_sample_sheet_from_file(infile=sheet, flow_cell_sample_type=flow_cell.sample_type)
     except ValidationError as error:
         LOG.warning(error)
         raise click.Abort from error
     LOG.info("Sample sheet passed validation")
 
 
 @sample_sheet_commands.command(name="create")
@@ -59,29 +66,29 @@
 ):
     """Command to create a sample sheet.
     flow-cell-name is the flow cell run directory name, e.g. '201203_A00689_0200_AHVKJCDRXX'
 
     Search the flow cell in the directory specified in config.
     """
 
-    LOG.info(f"Creating sample sheet for flowcell {flow_cell_name}")
+    LOG.info(f"Creating sample sheet for flow cell {flow_cell_name}")
     demultiplex_api: DemultiplexingAPI = context.demultiplex_api
     flowcell_path: Path = Path(demultiplex_api.run_dir, flow_cell_name)
     if not flowcell_path.exists():
         LOG.warning(f"Could not find flow cell {flowcell_path}")
         raise click.Abort
     try:
-        flow_cell = FlowCell(flow_cell_path=flowcell_path, bcl_converter=bcl_converter)
+        flow_cell = FlowCellDirectoryData(flow_cell_path=flowcell_path, bcl_converter=bcl_converter)
     except FlowCellError as error:
         raise click.Abort from error
-    lims_samples: List[Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen]] = list(
-        flow_cell_samples(
+    lims_samples: List[FlowCellSample] = list(
+        get_flow_cell_samples(
             lims=context.lims_api,
-            flowcell_id=flow_cell.id,
-            bcl_converter=bcl_converter,
+            flow_cell_id=flow_cell.id,
+            flow_cell_sample_type=flow_cell.sample_type,
         )
     )
     if not lims_samples:
         LOG.warning(f"Could not find any samples in lims for {flow_cell.id}")
         raise click.Abort
     try:
         sample_sheet_content: List[List[str]] = create_sample_sheet(
@@ -118,26 +125,26 @@
     demux_api: DemultiplexingAPI = context.demultiplex_api
     flow_cells: Path = demux_api.run_dir
     for sub_dir in flow_cells.iterdir():
         if not sub_dir.is_dir():
             continue
         LOG.info(f"Found directory {sub_dir}")
         try:
-            flow_cell = FlowCell(flow_cell_path=sub_dir, bcl_converter=bcl_converter)
+            flow_cell = FlowCellDirectoryData(flow_cell_path=sub_dir, bcl_converter=bcl_converter)
         except FlowCellError:
             continue
         if flow_cell.sample_sheet_exists():
             LOG.info("Sample sheet already exists")
             continue
-        LOG.info(f"Creating sample sheet for flowcell {flow_cell.id}")
+        LOG.info(f"Creating sample sheet for flow cell {flow_cell.id}")
         lims_samples: List[FlowCellSample] = list(
-            flow_cell_samples(
+            get_flow_cell_samples(
                 lims=context.lims_api,
-                flowcell_id=flow_cell.id,
-                bcl_converter=bcl_converter,
+                flow_cell_id=flow_cell.id,
+                flow_cell_sample_type=flow_cell.sample_type,
             )
         )
         if not lims_samples:
             LOG.warning(f"Could not find any samples in lims for {flow_cell.id}")
             continue
 
         try:
```

### Comparing `cg-35.0.2/cg/cli/generate/report/base.py` & `cg-36.0.1/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/generate/report/options.py` & `cg-36.0.1/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/generate/report/utils.py` & `cg-36.0.1/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/get.py` & `cg-36.0.1/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/set/base.py` & `cg-36.0.1/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/set/case.py` & `cg-36.0.1/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/set/cases.py` & `cg-36.0.1/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/store/fastq.py` & `cg-36.0.1/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/store/store.py` & `cg-36.0.1/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/transfer.py` & `cg-36.0.1/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/base.py` & `cg-36.0.1/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/clinical_delivery.py` & `cg-36.0.1/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/coverage.py` & `cg-36.0.1/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/delivery_report.py` & `cg-36.0.1/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/fohm.py` & `cg-36.0.1/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/genotype.py` & `cg-36.0.1/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/gens.py` & `cg-36.0.1/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/gisaid.py` & `cg-36.0.1/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/mutacc.py` & `cg-36.0.1/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/nipt/base.py` & `cg-36.0.1/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/nipt/ftp.py` & `cg-36.0.1/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/nipt/statina.py` & `cg-36.0.1/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/observations/observations.py` & `cg-36.0.1/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/observations/utils.py` & `cg-36.0.1/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/scout.py` & `cg-36.0.1/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/utils.py` & `cg-36.0.1/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/upload/validate.py` & `cg-36.0.1/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/balsamic/base.py` & `cg-36.0.1/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/balsamic/options.py` & `cg-36.0.1/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/balsamic/pon.py` & `cg-36.0.1/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/balsamic/qc.py` & `cg-36.0.1/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/balsamic/umi.py` & `cg-36.0.1/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/base.py` & `cg-36.0.1/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/commands.py` & `cg-36.0.1/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/fastq/base.py` & `cg-36.0.1/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/fluffy/base.py` & `cg-36.0.1/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/microsalt/base.py` & `cg-36.0.1/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/mip/base.py` & `cg-36.0.1/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/mip/options.py` & `cg-36.0.1/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/mip_dna/base.py` & `cg-36.0.1/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/mip_rna/base.py` & `cg-36.0.1/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/mutant/base.py` & `cg-36.0.1/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/nextflow/options.py` & `cg-36.0.1/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/rnafusion/base.py` & `cg-36.0.1/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/rnafusion/options.py` & `cg-36.0.1/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/taxprofiler/base.py` & `cg-36.0.1/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/cli/workflow/taxprofiler/options.py` & `cg-36.0.1/cg/cli/workflow/taxprofiler/options.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/__init__.py` & `cg-36.0.1/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/bcl_convert_metrics.py` & `cg-36.0.1/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/compression.py` & `cg-36.0.1/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/constants.py` & `cg-36.0.1/cg/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import click
 
 from cg.utils.enums import StrEnum
 from cg.utils.date import get_date
 
 VALID_DATA_IN_PRODUCTION = get_date("2017-09-27")
 
+LENGTH_LONG_DATE: int = len("YYYYMMDD")
+
 MAX_ITEMS_TO_RETRIEVE = 50
 
 SCALE_TO_MILLION_READ_PAIRS = 2_000_000
 SCALE_TO_READ_PAIRS = 2
 
 ANALYSIS_TYPES = ["tumor_wgs", "tumor_normal_wgs", "tumor_panel", "tumor_normal_panel"]
```

### Comparing `cg-35.0.2/cg/constants/delivery.py` & `cg-36.0.1/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/demultiplexing.py` & `cg-36.0.1/cg/constants/demultiplexing.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,44 +66,49 @@
 
     class Data(Enum):
         HEADER: str = "[Data]"
         FLOW_CELL_ID: str = "FCID"
         LANE: str = "Lane"
         SAMPLE_INTERNAL_ID_BCL2FASTQ: str = "SampleID"
         SAMPLE_INTERNAL_ID_BCLCONVERT: str = "Sample_ID"
+        SAMPLE_REFERENCE: str = "SampleRef"
+        INDEX_1: str = "index"
+        INDEX_2: str = "index2"
         SAMPLE_NAME: str = "SampleName"
+        CONTROL: str = "Control"
+        RECIPE: str = "Recipe"
+        OPERATOR: str = "Operator"
         SAMPLE_PROJECT_BCL2FASTQ: str = "Project"
         SAMPLE_PROJECT_BCLCONVERT: str = "Sample_Project"
-        CONTROL: str = "Control"
 
         COLUMN_NAMES: Dict[str, List[str]] = {
-            "bcl2fastq": [
+            BclConverter.BCL2FASTQ.value: [
                 FLOW_CELL_ID,
                 LANE,
                 SAMPLE_INTERNAL_ID_BCL2FASTQ,
-                "SampleRef",
-                "index",
-                "index2",
+                SAMPLE_REFERENCE,
+                INDEX_1,
+                INDEX_2,
                 SAMPLE_NAME,
                 CONTROL,
-                "Recipe",
-                "Operator",
+                RECIPE,
+                OPERATOR,
                 SAMPLE_PROJECT_BCL2FASTQ,
             ],
-            "dragen": [
+            BclConverter.DRAGEN.value: [
                 FLOW_CELL_ID,
                 LANE,
                 SAMPLE_INTERNAL_ID_BCLCONVERT,
-                "SampleRef",
-                "index",
-                "index2",
+                SAMPLE_REFERENCE,
+                INDEX_1,
+                INDEX_2,
                 SAMPLE_NAME,
                 CONTROL,
-                "Recipe",
-                "Operator",
+                RECIPE,
+                OPERATOR,
                 SAMPLE_PROJECT_BCLCONVERT,
             ],
         }
 
 
 class SampleSheetNovaSeqXSections:
     """Class with all necessary constants for building a NovaSeqX sample sheet."""
@@ -125,23 +130,32 @@
     class Settings(Enum):
         HEADER: str = "[BCLConvert_Settings]"
         SOFTWARE_VERSION: List[str] = ["SoftwareVersion", "4.1.5"]
         FASTQ_COMPRESSION_FORMAT: List[str] = ["FastqCompressionFormat", "gzip"]
 
     class Data(Enum):
         HEADER: str = "[BCLConvert_Data]"
+        LANE: str = "Lane"
+        SAMPLE_INTERNAL_ID: str = "Sample_ID"
+        INDEX_1: str = "Index"
+        INDEX_2: str = "Index2"
+        ADAPTER_READ_1: str = "AdapterRead1"
+        ADAPTER_READ_2: str = "AdapterRead2"
+        BARCODE_MISMATCHES_1: str = "BarcodeMismatchesIndex1"
+        BARCODE_MISMATCHES_2: str = "BarcodeMismatchesIndex2"
+
         COLUMN_NAMES: List[str] = [
-            "Lane",
-            "Sample_ID",
-            "Index",
-            "Index2",
-            "AdapterRead1",
-            "AdapterRead2",
-            "BarcodeMismatchesIndex1",
-            "BarcodeMismatchesIndex2",
+            LANE,
+            SAMPLE_INTERNAL_ID,
+            INDEX_1,
+            INDEX_2,
+            ADAPTER_READ_1,
+            ADAPTER_READ_2,
+            BARCODE_MISMATCHES_1,
+            BARCODE_MISMATCHES_2,
         ]
 
 
 OPTION_BCL_CONVERTER = click.option(
     "-b",
     "--bcl-converter",
     type=click.Choice(["bcl2fastq", "dragen"]),
```

### Comparing `cg-35.0.2/cg/constants/encryption.py` & `cg-36.0.1/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/gene_panel.py` & `cg-36.0.1/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/housekeeper_tags.py` & `cg-36.0.1/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/lims.py` & `cg-36.0.1/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/nextflow.py` & `cg-36.0.1/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/observations.py` & `cg-36.0.1/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/orderforms.py` & `cg-36.0.1/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/priority.py` & `cg-36.0.1/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/report.py` & `cg-36.0.1/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/rnafusion.py` & `cg-36.0.1/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/scout_upload.py` & `cg-36.0.1/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/sequencing.py` & `cg-36.0.1/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/subject.py` & `cg-36.0.1/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/constants/taxprofiler.py` & `cg-36.0.1/cg/constants/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/exc.py` & `cg-36.0.1/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/io/api.py` & `cg-36.0.1/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/io/controller.py` & `cg-36.0.1/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/io/csv.py` & `cg-36.0.1/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/io/json.py` & `cg-36.0.1/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/io/validate_path.py` & `cg-36.0.1/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/io/xml.py` & `cg-36.0.1/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/io/yaml.py` & `cg-36.0.1/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/archive/ddn_dataflow.py` & `cg-36.0.1/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/backup/backup.py` & `cg-36.0.1/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/backup/pdc.py` & `cg-36.0.1/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/clean/api.py` & `cg-36.0.1/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-36.0.1/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/clean/flow_cell_run_directories.py` & `cg-36.0.1/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/compress/compress.py` & `cg-36.0.1/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/compress/files.py` & `cg-36.0.1/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/deliver.py` & `cg-36.0.1/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/deliver_ticket.py` & `cg-36.0.1/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-36.0.1/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/demultiplex/demux_post_processing.py` & `cg-36.0.1/cg/meta/demultiplex/demux_post_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Post-processing Demultiiplex API."""
+import datetime
 import logging
 import os
 import shutil
 import re
 from contextlib import redirect_stdout
 from pathlib import Path
 from typing import Iterable, List, Optional
@@ -12,22 +13,23 @@
 
 from cg.apps.cgstats.crud import create
 from cg.apps.cgstats.stats import StatsAPI
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.demultiplex.demux_report import create_demux_report
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants.cgstats import STATS_HEADER
+from cg.constants.constants import FlowCellStatus
 from cg.constants.demultiplexing import BclConverter, DemultiplexingDirsAndFiles
 from cg.exc import FlowCellError
 from cg.meta.demultiplex import files
 from cg.meta.transfer import TransferFlowCell
 from cg.models.cg_config import CGConfig
 from cg.models.cgstats.stats_sample import StatsSample
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.store import Store
 from cg.store.models import Flowcell, SampleLaneSequencingMetrics
 from cg.utils import Process
 
 LOG = logging.getLogger(__name__)
 
 
@@ -80,15 +82,15 @@
         self.status_db.session.add_all(sample_lane_sequencing_metrics)
         self.status_db.session.commit()
         LOG.info(f"Added sample lane sequencing metrics to status database for: {flow_cell_name}")
 
     def finish_flow_cell_temp(self, flow_cell_name: str) -> None:
         """
         1. Validate that the flow cell directory exists.
-        2. Validate that the demultiplexing data transfer is complete.
+        2. Validate that the demultiplexing is complete.
         3. Create flow cell.
         4. Store flow cell in status db.
         5. Store flow cell data in housekeeper.
         6. Create sequencing metrics.
         """
 
         LOG.info(f"Finish flow cell {flow_cell_name}")
@@ -103,31 +105,57 @@
 
         # 2. Validate that the demultiplexing is complete.
         if not Path(flow_cell_dir, DemultiplexingDirsAndFiles.DEMUX_COMPLETE).exists():
             LOG.warning(f"Demultiplexing is not complete for flow cell {flow_cell_name}")
             return
 
         # 3. Create flow cell.
-        try:
-            flow_cell: FlowCell = FlowCell(
-                flow_cell_path=flow_cell_dir, bcl_converter=bcl_converter
-            )
-        except FlowCellError:
-            LOG.error(f"Could not create flow cell for {flow_cell_name}")
+        parsed_flow_cell: Optional[
+            FlowCellDirectoryData
+        ] = self.parse_and_validate_flow_cell_directory_data(
+            flow_cell_directory=flow_cell_dir,
+            bcl_converter=bcl_converter,
+        )
+
+        if not parsed_flow_cell:
             return
 
+        flow_cell: Flowcell = self.create_flow_cell(parsed_flow_cell=parsed_flow_cell)
+
         # 4. Store flow cell in status db.
         self.status_db.session.add(flow_cell)
         self.status_db.session.commit()
 
-        # 5. Store flow cell data in housekeeper. TODO
+        # 5. Store flow cell data in housekeeper.
 
         # 6. Create sequencing metrics
         self.add_sample_lane_sequencing_metrics_for_flow_cell(flow_cell_name=flow_cell_name)
 
+    def create_flow_cell(self, parsed_flow_cell: FlowCellDirectoryData) -> Flowcell:
+        """Create flow cell from the parsed and validated flow cell data."""
+        return Flowcell(
+            name=parsed_flow_cell.id,
+            sequencer_type=parsed_flow_cell.sequencer_type,
+            sequencer_name=parsed_flow_cell.machine_name,
+            sequenced_at=parsed_flow_cell.run_date,
+        )
+
+    def parse_and_validate_flow_cell_directory_data(
+        self, flow_cell_directory: Path, bcl_converter: str
+    ) -> FlowCellDirectoryData:
+        """Parse flow cell data from the flow cell directory."""
+        try:
+            flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+                flow_cell_path=flow_cell_directory, bcl_converter=bcl_converter
+            )
+            return flow_cell
+
+        except FlowCellError:
+            LOG.error(f"Unable to parse flow cell data from {flow_cell_directory}")
+
     def get_bcl_converter(self, flow_cell_name: str) -> str:
         """Return type of BCL converter."""
         if self.is_bcl2fastq_demux_folder_structure(flow_cell_name=flow_cell_name):
             LOG.info("Flow cell was demultiplexed with bcl2fastq")
             return BclConverter.BCL2FASTQ
         LOG.info("Flow cell was demultiplexed with bcl_converter")
         return BclConverter.BCLCONVERT
@@ -228,15 +256,15 @@
 
     def finish_flow_cell(
         self, bcl_converter: str, flow_cell_name: str, flow_cell_path: Path
     ) -> None:
         """Post-processing flow cell."""
         LOG.info(f"Check demultiplexed flow cell {flow_cell_name}")
         try:
-            flow_cell: FlowCell = FlowCell(
+            flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
                 flow_cell_path=flow_cell_path, bcl_converter=bcl_converter
             )
         except FlowCellError:
             return
         demux_results: DemuxResults = DemuxResults(
             demux_dir=Path(self.demux_api.out_dir, flow_cell_name),
             flow_cell=flow_cell,
@@ -401,15 +429,15 @@
 
         Force is used to finish a flow cell even if the files are renamed already.
         """
         LOG.info(
             f"Check demuxed flow cell {flow_cell_name}",
         )
         try:
-            flow_cell: FlowCell = FlowCell(
+            flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
                 flow_cell_path=Path(self.demux_api.run_dir, flow_cell_name),
                 bcl_converter=bcl_converter,
             )
         except FlowCellError:
             return
         if not self.demux_api.is_demultiplexing_completed(flow_cell=flow_cell):
             LOG.warning("Demultiplex is not ready for %s", flow_cell_name)
```

### Comparing `cg-35.0.2/cg/meta/demultiplex/files.py` & `cg-36.0.1/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/encryption/encryption.py` & `cg-36.0.1/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/invoice.py` & `cg-36.0.1/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/meta.py` & `cg-36.0.1/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/observations/balsamic_observations_api.py` & `cg-36.0.1/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/observations/mip_dna_observations_api.py` & `cg-36.0.1/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/observations/observations_api.py` & `cg-36.0.1/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/api.py` & `cg-36.0.1/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/case_submitter.py` & `cg-36.0.1/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/fastq_submitter.py` & `cg-36.0.1/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/lims.py` & `cg-36.0.1/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/metagenome_submitter.py` & `cg-36.0.1/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/microbial_submitter.py` & `cg-36.0.1/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/pool_submitter.py` & `cg-36.0.1/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/sars_cov_2_submitter.py` & `cg-36.0.1/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/submitter.py` & `cg-36.0.1/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/orders/ticket_handler.py` & `cg-36.0.1/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/balsamic.py` & `cg-36.0.1/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/balsamic_umi.py` & `cg-36.0.1/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/field_validators.py` & `cg-36.0.1/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/mip_dna.py` & `cg-36.0.1/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/report_api.py` & `cg-36.0.1/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/rnafusion.py` & `cg-36.0.1/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/templates/balsamic_report.html` & `cg-36.0.1/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/templates/bootstrap.html` & `cg-36.0.1/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/templates/mip-dna_report.html` & `cg-36.0.1/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/report/templates/rnafusion_report.html` & `cg-36.0.1/cg/meta/report/templates/rnafusion_report.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/rsync/rsync_api.py` & `cg-36.0.1/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/tar/tar.py` & `cg-36.0.1/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/transfer/external_data.py` & `cg-36.0.1/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/transfer/flowcell.py` & `cg-36.0.1/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/transfer/lims.py` & `cg-36.0.1/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/balsamic/balsamic.py` & `cg-36.0.1/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/coverage.py` & `cg-36.0.1/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/fohm/fohm.py` & `cg-36.0.1/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/gisaid/constants.py` & `cg-36.0.1/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/gisaid/gisaid.py` & `cg-36.0.1/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/gisaid/models.py` & `cg-36.0.1/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/gt.py` & `cg-36.0.1/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/mip/mip_dna.py` & `cg-36.0.1/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/mip/mip_rna.py` & `cg-36.0.1/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/mutacc.py` & `cg-36.0.1/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/nipt/nipt.py` & `cg-36.0.1/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/rnafusion/rnafusion.py` & `cg-36.0.1/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-36.0.1/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-36.0.1/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/scout/hk_tags.py` & `cg-36.0.1/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/scout/mip_config_builder.py` & `cg-36.0.1/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-36.0.1/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/scout/scout_config_builder.py` & `cg-36.0.1/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/scout/uploadscoutapi.py` & `cg-36.0.1/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/upload/upload_api.py` & `cg-36.0.1/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/analysis.py` & `cg-36.0.1/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/balsamic.py` & `cg-36.0.1/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/balsamic_pon.py` & `cg-36.0.1/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/balsamic_qc.py` & `cg-36.0.1/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/balsamic_umi.py` & `cg-36.0.1/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/fastq.py` & `cg-36.0.1/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/fluffy.py` & `cg-36.0.1/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/microsalt.py` & `cg-36.0.1/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/mip.py` & `cg-36.0.1/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/mip_dna.py` & `cg-36.0.1/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/mip_rna.py` & `cg-36.0.1/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/mutant.py` & `cg-36.0.1/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/nextflow_common.py` & `cg-36.0.1/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/prepare_fastq.py` & `cg-36.0.1/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/rnafusion.py` & `cg-36.0.1/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/taxprofiler.py` & `cg-36.0.1/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/meta/workflow/tower_common.py` & `cg-36.0.1/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/balsamic/config.py` & `cg-36.0.1/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/balsamic/metrics.py` & `cg-36.0.1/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/cg_config.py` & `cg-36.0.1/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/cgstats/stats_sample.py` & `cg-36.0.1/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/compression_data.py` & `cg-36.0.1/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/deliverables/metric_deliverables.py` & `cg-36.0.1/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/demultiplex/demux_results.py` & `cg-36.0.1/cg/models/demultiplex/demux_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from cg.apps.cgstats.parsers.adapter_metrics import AdapterMetrics
 from cg.apps.cgstats.parsers.conversion_stats import ConversionStats
 from cg.apps.cgstats.parsers.quality_metrics import QualityMetrics
 from cg.apps.cgstats.parsers.dragen_demultiplexing_stats import DragenDemultiplexingStats
 from cg.apps.cgstats.parsers.run_info import RunInfo
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.constants.demultiplexing import DEMUX_STATS_PATH
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 class LogfileParameters(BaseModel):
     id_string: str  # This indicates software and version
     # This is the binary that was executed (atm only bcl2fastq)
@@ -26,18 +26,18 @@
     command_line: str
     time: datetime.datetime
 
 
 class DemuxResults:
     """Class to gather information from a demultiplex result."""
 
-    def __init__(self, demux_dir: Path, flow_cell: FlowCell, bcl_converter: str):
+    def __init__(self, demux_dir: Path, flow_cell: FlowCellDirectoryData, bcl_converter: str):
         LOG.info(f"Instantiating DemuxResults with path {demux_dir}")
         self.demux_dir: Path = demux_dir
-        self.flow_cell: FlowCell = flow_cell
+        self.flow_cell: FlowCellDirectoryData = flow_cell
         self.bcl_converter = bcl_converter
         self._conversion_stats: Optional[ConversionStats] = None
         self._demultiplexing_stats: Optional[DragenDemultiplexingStats] = None
         self._adapter_metrics: Optional[AdapterMetrics] = None
         self._quality_metrics: Optional[QualityMetrics] = None
         self._runinfo: Optional[RunInfo] = None
```

### Comparing `cg-35.0.2/cg/models/demultiplex/flow_cell.py` & `cg-36.0.1/cg/models/demultiplex/flow_cell.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Module for modeling flow cells."""
 import datetime
 import logging
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, Type, Union
 
 from pydantic import ValidationError
 from typing_extensions import Literal
 
-from cg.apps.demultiplex.sample_sheet.models import SampleSheet
+from cg.apps.demultiplex.sample_sheet.models import (
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
+    FlowCellSampleNovaSeqX,
+    SampleSheet,
+)
 from cg.apps.demultiplex.sample_sheet.validate import get_sample_sheet_from_file
+from cg.constants.constants import LENGTH_LONG_DATE
 from cg.constants.demultiplexing import (
+    BclConverter,
     DemultiplexingDirsAndFiles,
 )
 from cg.constants.sequencing import Sequencers, sequencer_types
 from cg.exc import FlowCellError, SampleSheetError
 from cg.models.demultiplex.run_parameters import (
     RunParameters,
     RunParametersNovaSeq6000,
     RunParametersNovaSeqX,
 )
 
 LOG = logging.getLogger(__name__)
 
 
-class FlowCell:
-    """Class to collect information about flow cell directories and there particular files."""
+class FlowCellDirectoryData:
+    """Class to collect information about flow cell directories and their particular files."""
 
     def __init__(self, flow_cell_path: Path, bcl_converter: Optional[str] = "bcl2fastq"):
-        LOG.debug(f"Instantiating FlowCell with path {flow_cell_path}")
+        LOG.debug(f"Instantiating FlowCellDirectoryData with path {flow_cell_path}")
         self.path: Path = flow_cell_path
         self.bcl_converter: Optional[str] = bcl_converter
         self._run_parameters: Optional[RunParameters] = None
         self.run_date: datetime.datetime = datetime.datetime.now()
         self.machine_name: str = ""
         self.machine_number: int = 0
         self.base_name: str = ""  # Base name is flow cell-id + flow cell position
@@ -44,15 +51,15 @@
 
         This will assume that the flow cell naming convention is used. If not we skip the flow cell.
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
         Example: '201203_A00689_0200_AHVKJCDRXX'.
         """
 
         self.validate_flow_cell_name()
-        self.run_date = datetime.datetime.strptime(self.split_flow_cell_name[0], "%y%m%d")
+        self.run_date = self._parse_date()
         self.machine_name = self.split_flow_cell_name[1]
         self.machine_number = int(self.split_flow_cell_name[2])
         base_name: str = self.split_flow_cell_name[-1]
         self.base_name = base_name
         LOG.debug(f"Set flow cell id to {base_name}")
         self.id = base_name[1:]
         self.position = base_name[0]
@@ -89,14 +96,29 @@
                 RunParametersNovaSeqX(run_parameters_path=self.run_parameters_path)
                 if self.sequencer_type == Sequencers.NOVASEQX
                 else RunParametersNovaSeq6000(run_parameters_path=self.run_parameters_path)
             )
         return self._run_parameters
 
     @property
+    def sample_type(
+        self,
+    ) -> Union[
+        Type[FlowCellSampleNovaSeq6000Bcl2Fastq],
+        Type[FlowCellSampleNovaSeq6000Dragen],
+        Type[FlowCellSampleNovaSeqX],
+    ]:
+        """Return the sample class used in the flow cell."""
+        if self.sequencer_type == Sequencers.NOVASEQX:
+            return FlowCellSampleNovaSeqX
+        if self.bcl_converter == BclConverter.DRAGEN:
+            return FlowCellSampleNovaSeq6000Dragen
+        return FlowCellSampleNovaSeq6000Bcl2Fastq
+
+    @property
     def sequencer_type(
         self,
     ) -> Literal[Sequencers.HISEQX, Sequencers.HISEQGA, Sequencers.NOVASEQ, Sequencers.NOVASEQX]:
         """Return the sequencer type."""
         return sequencer_types[self.machine_name]
 
     @property
@@ -130,14 +152,20 @@
         return Path(self.path, "slurm_job_ids.yaml")
 
     @property
     def hiseq_x_flow_cell(self) -> Path:
         """Return path to Hiseq X flow cell directory."""
         return Path(self.path, DemultiplexingDirsAndFiles.Hiseq_X_TILE_DIR)
 
+    def _parse_date(self):
+        """Return the parsed date in the correct format."""
+        if len(self.split_flow_cell_name[0]) == LENGTH_LONG_DATE:
+            return datetime.datetime.strptime(self.split_flow_cell_name[0], "%Y%m%d")
+        return datetime.datetime.strptime(self.split_flow_cell_name[0], "%y%m%d")
+
     def validate_flow_cell_name(self) -> None:
         """
         Validate on the following criteria:
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
         Example: '201203_A00689_0200_AHVKJCDRXX'.
         """
         if len(self.split_flow_cell_name) != 4:
@@ -155,27 +183,27 @@
         return self.sample_sheet_path.exists()
 
     def validate_sample_sheet(self) -> bool:
         """Validate if sample sheet is on correct format."""
         try:
             get_sample_sheet_from_file(
                 infile=self.sample_sheet_path,
-                bcl_converter=self.bcl_converter,
+                flow_cell_sample_type=self.sample_type,
             )
         except (SampleSheetError, ValidationError) as error:
             LOG.warning("Invalid sample sheet")
             LOG.warning(error)
             return False
         return True
 
     def get_sample_sheet(self) -> SampleSheet:
         """Return sample sheet object."""
         return get_sample_sheet_from_file(
             infile=self.sample_sheet_path,
-            bcl_converter=self.bcl_converter,
+            flow_cell_sample_type=self.sample_type,
         )
 
     def is_sequencing_done(self) -> bool:
         """Check if sequencing is done.
         This is indicated by that the file RTAComplete.txt exists.
         """
         LOG.info("Check if sequencing is done")
@@ -185,15 +213,15 @@
         """Check if copy of flow cell is done.
         This is indicated by that the file CopyComplete.txt exists.
         """
         LOG.info("Check if copy of data from sequence instrument is ready")
         return self.copy_complete_path.exists()
 
     def is_hiseq_x_copy_completed(self) -> bool:
-        """Check if copy of Hiiseq X flow cell is done."""
+        """Check if copy of Hiseq X flow cell is done."""
         LOG.info("Check if copy of data from Hiseq X sequence instrument is ready")
         return self.hiseq_x_copy_complete_path.exists()
 
     def is_hiseq_x_delivery_started(self) -> bool:
         """Check if delivery of Hiseq X flow cell is started."""
         LOG.info("Check if delivery of data from Hiseq X sequence instrument is ready")
         return self.hiseq_x_delivery_started_path.exists()
```

### Comparing `cg-35.0.2/cg/models/demultiplex/run_parameters.py` & `cg-36.0.1/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/demultiplex/sbatch.py` & `cg-36.0.1/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/file_data.py` & `cg-36.0.1/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/invoice/invoice.py` & `cg-36.0.1/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/lims/sample.py` & `cg-36.0.1/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/mip/mip_config.py` & `cg-36.0.1/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/mip/mip_metrics_deliverables.py` & `cg-36.0.1/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/mip/mip_sample_info.py` & `cg-36.0.1/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/nextflow/deliverables.py` & `cg-36.0.1/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/nextflow/sample.py` & `cg-36.0.1/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/observations/input_files.py` & `cg-36.0.1/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/orders/constants.py` & `cg-36.0.1/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/orders/excel_sample.py` & `cg-36.0.1/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/orders/json_sample.py` & `cg-36.0.1/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/orders/order.py` & `cg-36.0.1/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/orders/orderform_schema.py` & `cg-36.0.1/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/orders/sample_base.py` & `cg-36.0.1/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/orders/samples.py` & `cg-36.0.1/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/report/metadata.py` & `cg-36.0.1/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/report/report.py` & `cg-36.0.1/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/report/sample.py` & `cg-36.0.1/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/report/validators.py` & `cg-36.0.1/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/rnafusion/metrics.py` & `cg-36.0.1/cg/models/rnafusion/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/rnafusion/rnafusion_sample.py` & `cg-36.0.1/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/scout/scout_load_config.py` & `cg-36.0.1/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/slurm/sbatch.py` & `cg-36.0.1/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/models/workflow/mutant.py` & `cg-36.0.1/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/resources/20181012_Indices.csv` & `cg-36.0.1/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/resources/rnafusion_bundle_filenames.csv` & `cg-36.0.1/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/admin.py` & `cg-36.0.1/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/api.py` & `cg-36.0.1/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/app.py` & `cg-36.0.1/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/config.py` & `cg-36.0.1/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/ext.py` & `cg-36.0.1/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/invoices/templates/invoices/index.html` & `cg-36.0.1/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/invoices/templates/invoices/invoice.html` & `cg-36.0.1/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/invoices/templates/invoices/layout.html` & `cg-36.0.1/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/invoices/templates/invoices/new.html` & `cg-36.0.1/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/server/invoices/views.py` & `cg-36.0.1/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/api/add.py` & `cg-36.0.1/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/api/base.py` & `cg-36.0.1/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/api/core.py` & `cg-36.0.1/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/api/delete.py` & `cg-36.0.1/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/api/find_basic_data.py` & `cg-36.0.1/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/api/find_business_data.py` & `cg-36.0.1/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/api/status.py` & `cg-36.0.1/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_analysis_filters.py` & `cg-36.0.1/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_application_filters.py` & `cg-36.0.1/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_application_version_filters.py` & `cg-36.0.1/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_bed_filters.py` & `cg-36.0.1/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_bed_version_filters.py` & `cg-36.0.1/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_case_filters.py` & `cg-36.0.1/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_case_sample_filters.py` & `cg-36.0.1/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_collaboration_filters.py` & `cg-36.0.1/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_customer_filters.py` & `cg-36.0.1/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_flow_cell_filters.py` & `cg-36.0.1/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_invoice_filters.py` & `cg-36.0.1/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_organism_filters.py` & `cg-36.0.1/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_panel_filters.py` & `cg-36.0.1/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_pool_filters.py` & `cg-36.0.1/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_sample_filters.py` & `cg-36.0.1/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/filters/status_user_filters.py` & `cg-36.0.1/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/store/models.py` & `cg-36.0.1/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/checksum/checksum.py` & `cg-36.0.1/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/click/EnumChoice.py` & `cg-36.0.1/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/commands.py` & `cg-36.0.1/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/date.py` & `cg-36.0.1/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/dict.py` & `cg-36.0.1/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/dispatcher.py` & `cg-36.0.1/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/email.py` & `cg-36.0.1/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/flask/enum.py` & `cg-36.0.1/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg/utils/utils.py` & `cg-36.0.1/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/cg.egg-info/PKG-INFO` & `cg-36.0.1/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 35.0.2
+Version: 36.0.1
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-35.0.2/cg.egg-info/SOURCES.txt` & `cg-36.0.1/cg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -726,15 +726,20 @@
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/CopyComplete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RTAComplete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml
 tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
 tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
 tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
 tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
 tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
 tests/fixtures/apps/fluffy/SampleSheet.csv
 tests/fixtures/apps/fluffy/deliverables.yaml
 tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
```

### Comparing `cg-35.0.2/requirements.txt` & `cg-36.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/setup.py` & `cg-36.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="35.0.2",
+    version="36.0.1",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-35.0.2/tests/apps/cgstats/conftest.py` & `cg-36.0.1/tests/apps/cgstats/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 import pytest
 from pydantic import BaseModel
 
 from cg.apps.cgstats.crud import create
 from cg.apps.cgstats.db.models import Supportparams, Sample, Project, Datasource, Demux
 from cg.apps.cgstats.stats import StatsAPI
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from tests.models.demultiplexing.conftest import (
     fixture_demultiplexed_dragen_flow_cell,
     fixture_dragen_demux_results,
 )
 
 
 class MockDemuxResults:
     """Mock Demux Results"""
 
     def __init__(self, flow_cell_full_name: str, sample_sheet_path: Path):
         self.bcl_converter = "dragen"
         self.conversion_stats_path = Path("Demultiplex_Stats.csv")
         self.demux_host = "hasta"
-        self.flow_cell: FlowCell = self.mock_flowcell(flow_cell_full_name=flow_cell_full_name)
+        self.flow_cell: FlowCellDirectoryData = self.mock_flowcell(
+            flow_cell_full_name=flow_cell_full_name
+        )
         self.machine_name = "barbara"
         self.run_date = datetime.now()
         self.run_name = flow_cell_full_name
         self.results_dir = Path("results_dir/unaligned")
         self.sample_sheet_path = sample_sheet_path
         self.run_info = self.RunInfo()
 
@@ -40,16 +42,16 @@
     class RunInfo(BaseModel):
         basemask: str = "151,10,10,151"
 
     def get_logfile_parameters(self) -> LogfileParameters:
         return self.LogfileParameters()
 
     @staticmethod
-    def mock_flowcell(flow_cell_full_name: str) -> FlowCell:
-        return FlowCell(flow_cell_path=Path(flow_cell_full_name))
+    def mock_flowcell(flow_cell_full_name: str) -> FlowCellDirectoryData:
+        return FlowCellDirectoryData(flow_cell_path=Path(flow_cell_full_name))
 
 
 class MockDemuxSample(BaseModel):
     """Mock Demux Sample"""
 
     pass_filter_qscore: float = 0.85
     pass_filter_Q30: float = 0.90
@@ -100,15 +102,15 @@
         sample_sheet_path=novaseq_bcl2fastq_sample_sheet_path,
     )
 
     project_obj: Project = create.create_project(manager=nipt_stats_api, project_name=ticket_id)
     support_parameters_obj: Supportparams = create.create_support_parameters(
         manager=nipt_stats_api, demux_results=mock_demux_results
     )
-    flowcell_obj: FlowCell = create.create_flowcell(
+    flowcell_obj: FlowCellDirectoryData = create.create_flowcell(
         manager=nipt_stats_api, demux_results=mock_demux_results
     )
     datasource_obj: Datasource = create.create_datasource(
         manager=nipt_stats_api,
         demux_results=mock_demux_results,
         support_parameters_id=support_parameters_obj.supportparams_id,
     )
```

### Comparing `cg-35.0.2/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-36.0.1/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/cgstats/crud/test_delete.py` & `cg-36.0.1/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-36.0.1/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-36.0.1/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/cgstats/parsers/test_run_info.py` & `cg-36.0.1/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/cgstats/test_cgstats_create.py` & `cg-36.0.1/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/cgstats/test_stats.py` & `cg-36.0.1/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/conftest.py` & `cg-36.0.1/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/coverage/test_coverage.py` & `cg-36.0.1/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/crunchy/conftest.py` & `cg-36.0.1/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/crunchy/test_compress_fastq.py` & `cg-36.0.1/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/crunchy/test_config.py` & `cg-36.0.1/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/crunchy/test_crunchy.py` & `cg-36.0.1/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/crunchy/test_spring_decompression.py` & `cg-36.0.1/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/demultiplex/conftest.py` & `cg-36.0.1/tests/apps/demultiplex/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from pathlib import Path
 from typing import List
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.index import Index
 from cg.apps.demultiplex.sample_sheet.novaseq_sample_sheet import SampleSheetCreator
-from cg.apps.demultiplex.sample_sheet.models import FlowCellSampleBcl2Fastq, FlowCellSampleDragen
+from cg.apps.demultiplex.sample_sheet.models import (
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
+)
 from cg.constants.demultiplexing import SampleSheetNovaSeq6000Sections
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
 @pytest.fixture(name="output_dirs_bcl2fastq")
 def fixture_output_dirs_bcl2fastq(demultiplexed_runs: Path) -> Path:
     """Return the output path a dir with flow cells that have finished demultiplexing using
     bcl2fastq."""
     return Path(demultiplexed_runs, "bcl2fastq")
@@ -33,43 +36,43 @@
 def fixture_index_obj() -> Index:
     return Index(name="C07 - UDI0051", sequence="AACAGGTT-ATACCAAG")
 
 
 @pytest.fixture(name="lims_novaseq_bcl2fastq_samples")
 def fixture_lims_novaseq_bcl2fastq_samples(
     lims_novaseq_samples_raw: List[dict],
-) -> List[FlowCellSampleBcl2Fastq]:
+) -> List[FlowCellSampleNovaSeq6000Bcl2Fastq]:
     """Return a list of parsed flow cell samples"""
-    return [FlowCellSampleBcl2Fastq(**sample) for sample in lims_novaseq_samples_raw]
+    return [FlowCellSampleNovaSeq6000Bcl2Fastq(**sample) for sample in lims_novaseq_samples_raw]
 
 
 @pytest.fixture(name="lims_novaseq_dragen_samples")
 def fixture_lims_novaseq_dragen_samples(
     lims_novaseq_samples_raw: List[dict],
-) -> List[FlowCellSampleDragen]:
+) -> List[FlowCellSampleNovaSeq6000Dragen]:
     """Return a list of parsed flowcell samples"""
-    return [FlowCellSampleDragen(**sample) for sample in lims_novaseq_samples_raw]
+    return [FlowCellSampleNovaSeq6000Dragen(**sample) for sample in lims_novaseq_samples_raw]
 
 
 @pytest.fixture(name="novaseq_bcl2fastq_sample_sheet_object")
 def fixture_novaseq_bcl2fastq_sample_sheet_object(
-    bcl2fastq_flow_cell: FlowCell,
-    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleBcl2Fastq],
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
+    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleNovaSeq6000Bcl2Fastq],
 ) -> SampleSheetCreator:
     return SampleSheetCreator(
         flow_cell=bcl2fastq_flow_cell,
         lims_samples=lims_novaseq_bcl2fastq_samples,
         bcl_converter="bcl2fastq",
     )
 
 
 @pytest.fixture(name="novaseq_dragen_sample_sheet_object")
 def fixture_novaseq_dragen_sample_sheet_object(
-    dragen_flow_cell: FlowCell,
-    lims_novaseq_dragen_samples: List[FlowCellSampleDragen],
+    dragen_flow_cell: FlowCellDirectoryData,
+    lims_novaseq_dragen_samples: List[FlowCellSampleNovaSeq6000Dragen],
 ) -> SampleSheetCreator:
     return SampleSheetCreator(
         flow_cell=dragen_flow_cell,
         lims_samples=lims_novaseq_dragen_samples,
         bcl_converter="dragen",
     )
 
@@ -269,17 +272,17 @@
 @pytest.fixture(name="valid_sample_sheet_dragen_path")
 def fixture_valid_sample_sheet_dragen_path() -> Path:
     """Return the path to a NovaSeq S2 sample sheet, used in dragen demultiplexing."""
     return Path("tests", "fixtures", "apps", "demultiplexing", "SampleSheetS2_Dragen.csv")
 
 
 @pytest.fixture(name="novaseq_sample_1")
-def fixture_novaseq_sample_1() -> FlowCellSampleBcl2Fastq:
+def fixture_novaseq_sample_1() -> FlowCellSampleNovaSeq6000Bcl2Fastq:
     """Return a NovaSeq sample."""
-    return FlowCellSampleBcl2Fastq(
+    return FlowCellSampleNovaSeq6000Bcl2Fastq(
         FCID="HWHMWDMXX",
         Lane=1,
         SampleID="ACC7628A68",
         SampleRef="hg19",
         index="ATTCCACACT",
         index2="TGGTCTTGTT",
         SampleName="814206",
@@ -287,17 +290,17 @@
         Recipe="R1",
         Operator="script",
         Project="814206",
     )
 
 
 @pytest.fixture(name="novaseq_sample_2")
-def fixture_novaseq_sample_2() -> FlowCellSampleBcl2Fastq:
+def fixture_novaseq_sample_2() -> FlowCellSampleNovaSeq6000Bcl2Fastq:
     """Return a NovaSeq sample."""
-    return FlowCellSampleBcl2Fastq(
+    return FlowCellSampleNovaSeq6000Bcl2Fastq(
         FCID="HWHMWDMXX",
         Lane=2,
         SampleID="ACC7628A1",
         SampleRef="hg19",
         index="ATTCCACACT",
         index2="TGGTCTTGTT",
         SampleName="814206",
```

### Comparing `cg-35.0.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-36.0.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from pathlib import Path
 from typing import List
 from cg.apps.demultiplex.sample_sheet.novaseq_sample_sheet import SampleSheetCreator
-from cg.apps.demultiplex.sample_sheet.models import SampleSheet
+from cg.apps.demultiplex.sample_sheet.models import (
+    SampleSheet,
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
+)
 from cg.apps.demultiplex.sample_sheet.validate import validate_sample_sheet
 
 
 def test_convert_to_bcl2fastq_sheet(
     novaseq_bcl2fastq_sample_sheet_object: SampleSheetCreator, project_dir: Path
 ):
-    """Test that a created bcl2fastq sample sheet has samples."""
-    # GIVEN a sample sheet object populated with samples
+    """Test that a created Bcl2fastq sample sheet has samples."""
+    # GIVEN a sample sheet object populated with Bcl2fastq samples
     assert novaseq_bcl2fastq_sample_sheet_object.lims_samples
 
     # WHEN converting to a sample sheet
     sample_sheet: List[List[str]] = novaseq_bcl2fastq_sample_sheet_object.construct_sample_sheet()
 
     # THEN assert a correctly formatted sample sheet was created
     sample_sheet_object: SampleSheet = validate_sample_sheet(
         sample_sheet_content=sample_sheet,
-        bcl_converter=novaseq_bcl2fastq_sample_sheet_object.bcl_converter,
+        sample_type=FlowCellSampleNovaSeq6000Bcl2Fastq,
     )
     assert sample_sheet_object.samples
 
 
 def test_convert_to_dragen_sheet(
     novaseq_dragen_sample_sheet_object: SampleSheetCreator, project_dir: Path
 ):
-    """Test that a created bcl2fastq sample sheet has samples."""
-    # GIVEN a sample sheet object populated with samples
+    """Test that a created Dragen sample sheet has samples."""
+    # GIVEN a sample sheet object populated with Dragen samples
     assert novaseq_dragen_sample_sheet_object.lims_samples
 
     # WHEN converting to a sample sheet
     sample_sheet: List[List[str]] = novaseq_dragen_sample_sheet_object.construct_sample_sheet()
 
     # THEN assert a correctly formatted sample sheet was created
     sample_sheet_object: SampleSheet = validate_sample_sheet(
         sample_sheet_content=sample_sheet,
-        bcl_converter=novaseq_dragen_sample_sheet_object.bcl_converter,
+        sample_type=FlowCellSampleNovaSeq6000Dragen,
     )
     assert sample_sheet_object.samples
```

### Comparing `cg-35.0.2/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-36.0.1/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/demultiplex/test_sample_sheet.py` & `cg-36.0.1/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import List
 
 from cg.apps.demultiplex.sample_sheet import dummy_sample, index
 from cg.apps.demultiplex.sample_sheet.index import Index
-from cg.apps.demultiplex.sample_sheet.models import FlowCellSampleBcl2Fastq
+from cg.apps.demultiplex.sample_sheet.models import (
+    FlowCellSample,
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+)
 
 
 def test_get_valid_indexes():
     # GIVEN a sample sheet api
 
     # WHEN fetching the indexes
     indexes: List[Index] = index.get_valid_indexes()
@@ -27,17 +30,17 @@
     assert dummy_sample_name == "D10---D710-D504--TCCGCGAA-GGCTCTGA-"
 
 
 def test_get_dummy_sample(bcl2fastq_flow_cell_id: str, index_obj: Index):
     # GIVEN some dummy sample data
 
     # WHEN creating the dummy sample for a bcl2fastq sample sheet
-    dummy_flow_cell_sample: FlowCellSampleBcl2Fastq = dummy_sample.dummy_sample(
+    dummy_flow_cell_sample: FlowCellSample = dummy_sample.dummy_sample(
         flow_cell_id=bcl2fastq_flow_cell_id,
         dummy_index=index_obj.sequence,
         lane=1,
         name=index_obj.name,
-        bcl_converter="bcl2fastq",
+        sample_type=FlowCellSampleNovaSeq6000Bcl2Fastq,
     )
 
     # THEN assert the sample id was correct
     assert dummy_flow_cell_sample.sample_id == dummy_sample.dummy_sample_name(index_obj.name)
```

### Comparing `cg-35.0.2/tests/apps/demultiplex/test_validate_sample_sheet.py` & `cg-36.0.1/tests/apps/demultiplex/test_validate_sample_sheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import logging
 from typing import List, Dict
 
 import pytest
 
-from cg.apps.demultiplex.sample_sheet.models import SampleSheet, FlowCellSampleBcl2Fastq
+from cg.apps.demultiplex.sample_sheet.models import (
+    SampleSheet,
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
+)
 from cg.apps.demultiplex.sample_sheet.validate import (
+    get_samples_by_lane,
     get_raw_samples,
     validate_sample_sheet,
-    get_samples_by_lane,
     validate_samples_are_unique,
 )
 from cg.constants.demultiplexing import BclConverter
 from cg.exc import SampleSheetError
 
 
 def test_validate_samples_are_unique(
-    novaseq_sample_1: FlowCellSampleBcl2Fastq,
-    novaseq_sample_2: FlowCellSampleBcl2Fastq,
+    novaseq_sample_1: FlowCellSampleNovaSeq6000Bcl2Fastq,
+    novaseq_sample_2: FlowCellSampleNovaSeq6000Bcl2Fastq,
 ):
     """Test that validating two different samples finishes successfully."""
     # GIVEN two different NovaSeq samples
     assert novaseq_sample_1 != novaseq_sample_2
 
     # WHEN validating the samples
     validate_samples_are_unique(samples=[novaseq_sample_1, novaseq_sample_2])
 
     # THEN no error is raised
 
 
-def test_validate_samples_are_unique_not_unique(novaseq_sample_1: FlowCellSampleBcl2Fastq, caplog):
+def test_validate_samples_are_unique_when_not_unique(
+    novaseq_sample_1: FlowCellSampleNovaSeq6000Bcl2Fastq, caplog
+):
     """Test that validating two identical samples fails."""
     # GIVEN two identical NovaSeq samples
     caplog.set_level(logging.INFO)
 
     # WHEN validating the samples
     with pytest.raises(SampleSheetError):
         validate_samples_are_unique(samples=[novaseq_sample_1, novaseq_sample_1])
@@ -40,22 +46,22 @@
     # THEN a sample sheet error is raised due to the samples being identical
     assert (
         f"Sample {novaseq_sample_1.sample_id} exists multiple times in sample sheet" in caplog.text
     )
 
 
 def test_get_samples_by_lane(
-    novaseq_sample_1: FlowCellSampleBcl2Fastq,
-    novaseq_sample_2: FlowCellSampleBcl2Fastq,
+    novaseq_sample_1: FlowCellSampleNovaSeq6000Bcl2Fastq,
+    novaseq_sample_2: FlowCellSampleNovaSeq6000Bcl2Fastq,
 ):
     """Test that grouping two samples with different lanes returns two groups."""
     # GIVEN two samples on two different lanes
 
     # WHEN getting the samples per lane
-    samples_per_lane: Dict[int, List[FlowCellSampleBcl2Fastq]] = get_samples_by_lane(
+    samples_per_lane: Dict[int, List[FlowCellSampleNovaSeq6000Bcl2Fastq]] = get_samples_by_lane(
         samples=[novaseq_sample_1, novaseq_sample_2]
     )
 
     # THEN the returned value is a dictionary
     assert isinstance(samples_per_lane, Dict)
     # THEN the dictionary has two entries
     assert len(samples_per_lane) == 2
@@ -100,67 +106,67 @@
     with pytest.raises(SampleSheetError):
         get_raw_samples(sample_sheet_content=sample_sheet_bcl2fastq_data_header)
 
     # THEN an exception is raised because of the missing samples
     assert "Could not find any samples in sample sheet" in caplog.text
 
 
-def test_get_sample_sheet_s2_bcl2fastq_duplicate_same_lane(
+def test_get_sample_sheet_bcl2fastq_duplicate_same_lane(
     sample_sheet_bcl2fastq_duplicate_same_lane: List[List[str]],
 ):
     """Test that creating a Bcl2fastq sample sheet with duplicated samples in a lane fails."""
     # GIVEN a Bcl2fastq sample sheet with a sample duplicated in a lane
 
     # WHEN creating the sample sheet object
     with pytest.raises(SampleSheetError):
         # THEN a sample sheet error is raised
         validate_sample_sheet(
             sample_sheet_content=sample_sheet_bcl2fastq_duplicate_same_lane,
-            bcl_converter=BclConverter.BCL2FASTQ,
+            sample_type=FlowCellSampleNovaSeq6000Bcl2Fastq,
         )
 
 
-def test_get_sample_sheet_s2_dragen_duplicate_same_lane(
+def test_get_sample_sheet_dragen_duplicate_same_lane(
     sample_sheet_dragen_duplicate_same_lane: List[List[str]],
 ):
     """Test that creating a Dragen sample sheet with duplicated samples in a lane fails."""
     # GIVEN a Dragen sample sheet with a sample duplicated in a lane
 
     # WHEN creating the sample sheet object
     with pytest.raises(SampleSheetError):
         # THEN a sample sheet error is raised
         validate_sample_sheet(
             sample_sheet_content=sample_sheet_dragen_duplicate_same_lane,
-            bcl_converter=BclConverter.DRAGEN,
+            sample_type=FlowCellSampleNovaSeq6000Dragen,
         )
 
 
-def test_get_sample_sheet_s2_bcl2fastq_duplicate_different_lanes(
+def test_get_sample_sheet_bcl2fastq_duplicate_different_lanes(
     sample_sheet_bcl2fastq_duplicate_different_lane: List[List[str]],
 ):
     """Test that Bcl2fastq a sample sheet created with duplicated samples in different lanes has samples."""
     # GIVEN a Bcl2fastq sample sheet with same sample duplicated in different lanes
 
     # WHEN creating the sample sheet object
     sample_sheet: SampleSheet = validate_sample_sheet(
         sample_sheet_content=sample_sheet_bcl2fastq_duplicate_different_lane,
-        bcl_converter=BclConverter.BCL2FASTQ,
+        sample_type=FlowCellSampleNovaSeq6000Bcl2Fastq,
     )
 
     # THEN a sample sheet is returned with samples in it
     assert sample_sheet.samples
 
 
-def test_get_sample_sheet_s2_dragen_duplicate_different_lanes(
+def test_get_sample_sheet_dragen_duplicate_different_lanes(
     sample_sheet_dragen_duplicate_different_lane: List[List[str]],
 ):
     """Test that Dragen a sample sheet created with duplicated samples in different lanes has samples."""
     # GIVEN a Dragen sample sheet with same sample duplicated in different lanes
 
     # WHEN creating the sample sheet object
     sample_sheet: SampleSheet = validate_sample_sheet(
         sample_sheet_content=sample_sheet_dragen_duplicate_different_lane,
-        bcl_converter=BclConverter.DRAGEN,
+        sample_type=FlowCellSampleNovaSeq6000Dragen,
     )
 
     # THEN a sample sheet is returned with samples in it
     assert sample_sheet.samples
```

### Comparing `cg-35.0.2/tests/apps/gens/test_gens_api.py` & `cg-36.0.1/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/gt/conftest.py` & `cg-36.0.1/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/gt/test_gt_api.py` & `cg-36.0.1/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/hk/conftest.py` & `cg-36.0.1/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/hk/test__getattr__.py` & `cg-36.0.1/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/hk/test_add_file.py` & `cg-36.0.1/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/hk/test_bundles.py` & `cg-36.0.1/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/hk/test_core.py` & `cg-36.0.1/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/hk/test_file.py` & `cg-36.0.1/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/hk/test_version.py` & `cg-36.0.1/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/lims/conftest.py` & `cg-36.0.1/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/lims/test_api.py` & `cg-36.0.1/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/lims/test_sample_sheet.py` & `cg-36.0.1/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/loqus/conftest.py` & `cg-36.0.1/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/loqus/test_loqusdb_api.py` & `cg-36.0.1/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/madeline/conftest.py` & `cg-36.0.1/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/madeline/test_madeline.py` & `cg-36.0.1/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/mip/conftest.py` & `cg-36.0.1/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/mip/test_config_mip.py` & `cg-36.0.1/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/mutacc_auto/conftest.py` & `cg-36.0.1/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-36.0.1/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/orderform/conftest.py` & `cg-36.0.1/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-36.0.1/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/orderform/test_excel_sample_schema.py` & `cg-36.0.1/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/orderform/test_json_orderform_parser.py` & `cg-36.0.1/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/orderform/test_orderform_parser.py` & `cg-36.0.1/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/scout/conftest.py` & `cg-36.0.1/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/scout/test_get_causative_variants.py` & `cg-36.0.1/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/scout/test_get_scout_cases.py` & `cg-36.0.1/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/scout/test_scout_load_config.py` & `cg-36.0.1/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/scout/test_scout_models.py` & `cg-36.0.1/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-36.0.1/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-36.0.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-36.0.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/slurm/conftest.py` & `cg-36.0.1/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/slurm/test_slurm_api.py` & `cg-36.0.1/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/test_apps_environ.py` & `cg-36.0.1/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/apps/test_osticket.py` & `cg-36.0.1/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/add/test_cli_add.py` & `cg-36.0.1/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/add/test_cli_add_customer.py` & `cg-36.0.1/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/add/test_cli_add_family.py` & `cg-36.0.1/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/add/test_cli_add_relationship.py` & `cg-36.0.1/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/add/test_cli_add_sample.py` & `cg-36.0.1/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/backup/conftest.py` & `cg-36.0.1/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/backup/test_backup_command.py` & `cg-36.0.1/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/clean/conftest.py` & `cg-36.0.1/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/clean/test_balsamic_clean.py` & `cg-36.0.1/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-36.0.1/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/clean/test_hk_bundle_files.py` & `cg-36.0.1/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-36.0.1/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/clean/test_microbial_clean.py` & `cg-36.0.1/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-36.0.1/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/compress/conftest.py` & `cg-36.0.1/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/compress/test_cli_compress_fastq.py` & `cg-36.0.1/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/compress/test_cli_decompress_spring.py` & `cg-36.0.1/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/compress/test_compress_helpers.py` & `cg-36.0.1/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/compress/test_store_fastq.py` & `cg-36.0.1/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/conftest.py` & `cg-36.0.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/delete/test_cli_delete_case.py` & `cg-36.0.1/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/delete/test_cli_delete_cases.py` & `cg-36.0.1/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/deliver/conftest.py` & `cg-36.0.1/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/deliver/test_deliver_base.py` & `cg-36.0.1/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/deliver/test_rsync_base.py` & `cg-36.0.1/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-36.0.1/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/demultiplex/conftest.py` & `cg-36.0.1/tests/cli/demultiplex/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 
 from cg.apps.cgstats.stats import StatsAPI
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.apps.lims import LimsAPI
 from cg.models.cg_config import CGConfig
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.utils import Process
 from tests.apps.cgstats.conftest import fixture_populated_stats_api, fixture_stats_api
 from tests.apps.demultiplex.conftest import (
     fixture_lims_novaseq_bcl2fastq_samples,
     fixture_lims_novaseq_dragen_samples,
 )
 
@@ -96,16 +96,18 @@
 ) -> Path:
     """Return the path to a working directory that will be deleted after test is run.
 
     This is a path to a flow cell directory with the run parameters present.
     """
     working_dir: Path = Path(flow_cell_runs_working_directory, bcl2fastq_flow_cell_dir.name)
     working_dir.mkdir(parents=True)
-    existing_flow_cell: FlowCell = FlowCell(flow_cell_path=bcl2fastq_flow_cell_dir)
-    working_flow_cell: FlowCell = FlowCell(flow_cell_path=working_dir)
+    existing_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=bcl2fastq_flow_cell_dir
+    )
+    working_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(flow_cell_path=working_dir)
     shutil.copy(
         existing_flow_cell.run_parameters_path.as_posix(),
         working_flow_cell.run_parameters_path.as_posix(),
     )
     return working_dir
 
 
@@ -117,16 +119,18 @@
 
     This is a path to a flow cell directory with the run parameters present.
     """
     working_dir: Path = Path(
         flow_cell_runs_working_directory_bcl2fastq, bcl2fastq_flow_cell_dir.name
     )
     working_dir.mkdir(parents=True)
-    existing_flow_cell: FlowCell = FlowCell(flow_cell_path=bcl2fastq_flow_cell_dir)
-    working_flow_cell: FlowCell = FlowCell(flow_cell_path=working_dir)
+    existing_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=bcl2fastq_flow_cell_dir
+    )
+    working_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(flow_cell_path=working_dir)
     shutil.copy(
         existing_flow_cell.run_parameters_path.as_posix(),
         working_flow_cell.run_parameters_path.as_posix(),
     )
     return working_dir
 
 
@@ -136,16 +140,18 @@
 ) -> Path:
     """Return the path to a working directory that will be deleted after test is run.
 
     This is a path to a flow cell directory with the run parameters present.
     """
     working_dir: Path = Path(flow_cell_runs_working_directory_dragen, dragen_flow_cell_dir.name)
     working_dir.mkdir(parents=True)
-    existing_flow_cell: FlowCell = FlowCell(flow_cell_path=dragen_flow_cell_dir)
-    working_flow_cell: FlowCell = FlowCell(flow_cell_path=working_dir)
+    existing_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=dragen_flow_cell_dir
+    )
+    working_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(flow_cell_path=working_dir)
     shutil.copy(
         existing_flow_cell.run_parameters_path.as_posix(),
         working_flow_cell.run_parameters_path.as_posix(),
     )
     return working_dir
 
 
@@ -163,16 +169,20 @@
 def fixture_demultiplex_ready_flow_cell(
     flow_cell_working_directory: Path, bcl2fastq_flow_cell_dir: Path
 ) -> Path:
     """Return the path to a working directory that is ready for demultiplexing.
 
     This is a path to a flow cell directory with all the files necessary to start demultiplexing present.
     """
-    existing_flow_cell: FlowCell = FlowCell(flow_cell_path=bcl2fastq_flow_cell_dir)
-    working_flow_cell: FlowCell = FlowCell(flow_cell_path=flow_cell_working_directory)
+    existing_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=bcl2fastq_flow_cell_dir
+    )
+    working_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=flow_cell_working_directory
+    )
     shutil.copy(
         existing_flow_cell.sample_sheet_path.as_posix(),
         working_flow_cell.sample_sheet_path.as_posix(),
     )
     shutil.copy(
         str(DemultiplexingAPI.get_stderr_logfile(existing_flow_cell)),
         str(DemultiplexingAPI.get_stderr_logfile(working_flow_cell)),
@@ -186,16 +196,20 @@
 def fixture_demultiplex_ready_flow_cell_bcl2fastq(
     flow_cell_working_directory_bcl2fastq: Path, bcl2fastq_flow_cell_dir: Path
 ) -> Path:
     """Return the path to a working directory that is ready for demultiplexing.
 
     This is a path to a flow cell directory with all the files necessary to start demultiplexing present.
     """
-    existing_flow_cell: FlowCell = FlowCell(flow_cell_path=bcl2fastq_flow_cell_dir)
-    working_flow_cell: FlowCell = FlowCell(flow_cell_path=flow_cell_working_directory_bcl2fastq)
+    existing_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=bcl2fastq_flow_cell_dir
+    )
+    working_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=flow_cell_working_directory_bcl2fastq
+    )
     shutil.copy(
         existing_flow_cell.sample_sheet_path.as_posix(),
         working_flow_cell.sample_sheet_path.as_posix(),
     )
     shutil.copy(
         str(DemultiplexingAPI.get_stderr_logfile(existing_flow_cell)),
         str(DemultiplexingAPI.get_stderr_logfile(working_flow_cell)),
@@ -209,18 +223,18 @@
 def fixture_demultiplex_ready_flow_cell_dragen(
     flow_cell_working_directory_dragen: Path, dragen_flow_cell_dir: Path
 ) -> Path:
     """Return the path to a working directory that is ready for demultiplexing.
 
     This is a path to a flow cell directory with all the files necessary to start demultiplexing present.
     """
-    existing_flow_cell: FlowCell = FlowCell(
+    existing_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
         flow_cell_path=dragen_flow_cell_dir, bcl_converter="dragen"
     )
-    working_flow_cell: FlowCell = FlowCell(
+    working_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
         flow_cell_path=flow_cell_working_directory_dragen, bcl_converter="dragen"
     )
     shutil.copy(
         existing_flow_cell.sample_sheet_path.as_posix(),
         working_flow_cell.sample_sheet_path.as_posix(),
     )
     shutil.copy(
```

### Comparing `cg-35.0.2/tests/cli/demultiplex/test_add_flowcell.py` & `cg-36.0.1/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 
 from cg.cli.demultiplex.add import add_flow_cell_cmd
 from cg.models.cg_config import CGConfig
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from click.testing import CliRunner
 
 
 def test_add_flowcell_cmd(
     cli_runner: CliRunner,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     demultiplex_context: CGConfig,
     demultiplexed_flow_cell_finished_working_directory: Path,
     demultiplex_ready_flow_cell: Path,
 ):
     # GIVEN a cgstats api and a demultiplex api
     # GIVEN that there is a flowcell in the run dir
     assert demultiplex_ready_flow_cell.exists()
```

### Comparing `cg-35.0.2/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-36.0.1/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 from pathlib import Path
 from typing import List
 
 from click import testing
 
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.demultiplex.sample_sheet.models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleDragen,
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
 )
 from cg.cli.demultiplex.sample_sheet import create_sheet
 from cg.constants.demultiplexing import BclConverter
 from cg.constants.process import EXIT_SUCCESS
 from cg.models.cg_config import CGConfig
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
-FLOW_CELL_FUNCTION_NAME: str = "cg.cli.demultiplex.sample_sheet.flow_cell_samples"
+FLOW_CELL_FUNCTION_NAME: str = "cg.cli.demultiplex.sample_sheet.get_flow_cell_samples"
 
 
 def test_create_sample_sheet_no_run_parameters(
     cli_runner: testing.CliRunner,
     flow_cell_working_directory_no_run_parameters: Path,
     sample_sheet_context: CGConfig,
-    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleBcl2Fastq],
+    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleNovaSeq6000Bcl2Fastq],
     caplog,
     mocker,
 ):
     # GIVEN a folder with a non-existing sample sheet
-    flowcell_object: FlowCell = FlowCell(flow_cell_working_directory_no_run_parameters)
-    assert flowcell_object.run_parameters_path.exists() is False
+    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=flow_cell_working_directory_no_run_parameters
+    )
+    assert flow_cell.run_parameters_path.exists() is False
 
     # GIVEN flow cell samples
     mocker.patch(
         FLOW_CELL_FUNCTION_NAME,
         return_value=lims_novaseq_bcl2fastq_samples,
     )
 
     # GIVEN a demux API context
     demux_api: DemultiplexingAPI = sample_sheet_context.demultiplex_api
     demux_api.run_dir: Path = flow_cell_working_directory_no_run_parameters.parent
     sample_sheet_context.demultiplex_api_: DemultiplexingAPI = demux_api
 
     # WHEN running the create sample sheet command
     result: testing.Result = cli_runner.invoke(
-        create_sheet, [flowcell_object.full_name], obj=sample_sheet_context
+        create_sheet, [flow_cell.full_name], obj=sample_sheet_context
     )
 
     # THEN the process exits with a non-zero exit code
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN the correct information is communicated
     assert "Could not find run parameters file" in caplog.text
 
 
 def test_create_bcl2fastq_sample_sheet(
     cli_runner: testing.CliRunner,
     flow_cell_working_directory: Path,
     sample_sheet_context: CGConfig,
-    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleBcl2Fastq],
+    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleNovaSeq6000Bcl2Fastq],
     mocker,
 ):
     # GIVEN a flowcell directory with some run parameters
-    flowcell: FlowCell = FlowCell(flow_cell_working_directory)
+    flowcell: FlowCellDirectoryData = FlowCellDirectoryData(flow_cell_working_directory)
     assert flowcell.run_parameters_path.exists()
 
     # GIVEN that there is no sample sheet present
     assert not flowcell.sample_sheet_exists()
 
     # GIVEN flow cell samples
     mocker.patch(
@@ -88,19 +90,21 @@
     assert flowcell.validate_sample_sheet()
 
 
 def test_create_dragen_sample_sheet(
     cli_runner: testing.CliRunner,
     flow_cell_working_directory: Path,
     sample_sheet_context: CGConfig,
-    lims_novaseq_dragen_samples: List[FlowCellSampleDragen],
+    lims_novaseq_dragen_samples: List[FlowCellSampleNovaSeq6000Dragen],
     mocker,
 ):
     # GIVEN a flowcell directory with some run parameters
-    flowcell: FlowCell = FlowCell(flow_cell_working_directory, bcl_converter=BclConverter.DRAGEN)
+    flowcell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_working_directory, bcl_converter=BclConverter.DRAGEN
+    )
     assert flowcell.run_parameters_path.exists()
 
     # GIVEN that there is no sample sheet present
     assert not flowcell.sample_sheet_exists()
 
     # GIVEN flow cell samples
     mocker.patch(
```

### Comparing `cg-35.0.2/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-36.0.1/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from pathlib import Path
 
 from click import testing
 
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.cli.demultiplex.demux import demultiplex_all, demultiplex_flow_cell, delete_flow_cell
 from cg.models.cg_config import CGConfig
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
 def test_demultiplex_flow_cell_dry_run(
     cli_runner: testing.CliRunner,
     demultiplex_ready_flow_cell: Path,
     demultiplex_context: CGConfig,
     caplog,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN that all files are present for demultiplexing
-    flow_cell: FlowCell = FlowCell(demultiplex_ready_flow_cell)
+    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(demultiplex_ready_flow_cell)
 
     # GIVEN a out dir that does not exist
     demux_api: DemultiplexingAPI = demultiplex_context.demultiplex_api
     assert demux_api.is_demultiplexing_possible(flow_cell=flow_cell)
     demux_dir: Path = demux_api.flow_cell_out_dir_path(flow_cell)
     unaligned_dir: Path = demux_dir / "Unaligned"
     assert demux_dir.exists() is False
@@ -50,15 +50,15 @@
     demultiplex_context: CGConfig,
     caplog,
     mocker,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN that all files are present for demultiplexing
-    flow_cell: FlowCell = FlowCell(demultiplex_ready_flow_cell)
+    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(demultiplex_ready_flow_cell)
 
     # GIVEN a out dir that does not exist
     demux_api: DemultiplexingAPI = demultiplex_context.demultiplex_api
     demux_dir: Path = demux_api.flow_cell_out_dir_path(flow_cell)
     unaligned_dir: Path = demux_dir / "Unaligned"
     assert demux_api.is_demultiplexing_possible(flow_cell=flow_cell)
     assert demux_dir.exists() is False
@@ -89,15 +89,15 @@
     demultiplex_context: CGConfig,
     caplog,
     mocker,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN that all files are present for bcl2fastq demultiplexing
-    flow_cell: FlowCell = FlowCell(demultiplex_ready_flow_cell_bcl2fastq)
+    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(demultiplex_ready_flow_cell_bcl2fastq)
 
     # GIVEN a out dir that does not exist
     demux_api: DemultiplexingAPI = demultiplex_context.demultiplex_api
     demux_dir: Path = demux_api.flow_cell_out_dir_path(flow_cell)
     unaligned_dir: Path = demux_dir / "Unaligned"
     assert demux_api.is_demultiplexing_possible(flow_cell=flow_cell)
     assert demux_dir.exists() is False
@@ -129,15 +129,15 @@
     demultiplexed_flow_cells_working_directory: Path,
     caplog,
     mocker,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN that all files are present for dragen demultiplexing
-    flow_cell: FlowCell = FlowCell(
+    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
         flow_cell_path=demultiplex_ready_flow_cell_dragen, bcl_converter="dragen"
     )
 
     # GIVEN a out dir that does not exist
     demux_api: DemultiplexingAPI = demultiplex_context.demultiplex_api
     demux_dir: Path = demux_api.flow_cell_out_dir_path(flow_cell)
     unaligned_dir: Path = demux_dir / "Unaligned"
@@ -172,15 +172,17 @@
 ):
     """Test the demultiplex-all command on a directory with newly sequenced NovaSeq6000 flow cells."""
 
     caplog.set_level(logging.INFO)
 
     # GIVEN a context with the path to a directory where at least one flowcell is ready for demux
     demux_api: DemultiplexingAPI = demultiplex_context.demultiplex_api
-    flow_cell: FlowCell = FlowCell(flow_cell_path=demultiplex_ready_flow_cell)
+    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
+        flow_cell_path=demultiplex_ready_flow_cell
+    )
 
     assert demux_api.run_dir == demultiplex_ready_flow_cell.parent
 
     # WHEN running the demultiplex all command
     result: testing.Result = cli_runner.invoke(
         demultiplex_all, ["--dry-run"], obj=demultiplex_context
     )
@@ -196,15 +198,15 @@
 
 
 def test_start_demultiplex_flow_cell(
     caplog,
     cli_runner: testing.CliRunner,
     demultiplex_ready_flow_cell: Path,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     mocker,
 ):
     caplog.set_level(logging.DEBUG)
 
     # GIVEN that all files are present for demultiplexing
     demux_api: DemultiplexingAPI = demultiplex_context.demultiplex_api
```

### Comparing `cg-35.0.2/tests/cli/demultiplex/test_finish_demux.py` & `cg-36.0.1/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/demultiplex/test_stats_command.py` & `cg-36.0.1/tests/cli/demultiplex/test_stats_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from click.testing import CliRunner
 
 from cg.apps.cgstats.stats import StatsAPI
 from cg.cli.demultiplex.add import select_project_cmd
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
 def test_select_command(
     cli_runner: CliRunner,
     populated_stats_api: StatsAPI,
     demultiplexed_runs: Path,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     demultiplex_context: CGConfig,
 ):
     demultiplex_context.cg_stats_api_ = populated_stats_api
     # GIVEN a stats api with some information about a flowcell
     flowcell_id: str = bcl2fastq_flow_cell.id
     full_flow_cell_name: str = bcl2fastq_flow_cell.full_name
     assert populated_stats_api.find_handler.get_flow_cell_by_name(flow_cell_name=flowcell_id)
```

### Comparing `cg-35.0.2/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-36.0.1/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,120 @@
 from pathlib import Path
 
 from click.testing import CliRunner, Result
 
 from cg.apps.demultiplex.sample_sheet.validate import get_sample_sheet_from_file
+from cg.apps.demultiplex.sample_sheet.models import (
+    FlowCellSampleNovaSeq6000Bcl2Fastq,
+    FlowCellSampleNovaSeq6000Dragen,
+)
 from cg.cli.demultiplex.sample_sheet import validate_sample_sheet
 
 from cg.constants import EXIT_SUCCESS, FileExtensions
 from cg.constants.demultiplexing import BclConverter
 
 
-def test_validate_non_existing_sample_sheet(cli_runner: CliRunner, sample_sheet_context: dict):
+def test_validate_non_existing_sample_sheet(
+    cli_runner: CliRunner, sample_sheet_context: dict, bcl2fastq_flow_cell_full_name: str
+):
     """Test validate sample sheet when sample sheet does not exist."""
 
     # GIVEN a cli runner
     # GIVEN a sample sheet file that does not exist
     sample_sheet: Path = Path("a_sample_sheet_that_does_not_exist.csv")
     assert sample_sheet.exists() is False
 
     # WHEN validating the sample sheet
-    result = cli_runner.invoke(validate_sample_sheet, [str(sample_sheet)], obj=sample_sheet_context)
+    result = cli_runner.invoke(
+        validate_sample_sheet,
+        [bcl2fastq_flow_cell_full_name, str(sample_sheet)],
+        obj=sample_sheet_context,
+    )
 
     # THEN assert that it exits with a non-zero exit code
     assert result.exit_code != EXIT_SUCCESS
     # THEN assert the correct information was communicated
     assert f'Path "{sample_sheet.name}" does not exist' in result.output
 
 
 def test_validate_sample_sheet_wrong_file_type(
     cli_runner: CliRunner,
     sample_sheet_context: dict,
+    bcl2fastq_flow_cell_full_name: str,
     novaseq_6000_run_parameters_path: Path,
     caplog,
 ):
     """Test validate sample sheet when sample sheet is in wrong format."""
-    # GIVEN a existing file in the wrong file format
+    # GIVEN an existing file in the wrong file format
     sample_sheet: Path = novaseq_6000_run_parameters_path
     assert sample_sheet.exists()
     assert sample_sheet.suffix != FileExtensions.CSV
 
     # WHEN validating the sample sheet
     result: Result = cli_runner.invoke(
-        validate_sample_sheet, [str(sample_sheet)], obj=sample_sheet_context
+        validate_sample_sheet,
+        [bcl2fastq_flow_cell_full_name, str(sample_sheet)],
+        obj=sample_sheet_context,
     )
 
     # THEN assert it exits with a non-zero exit code
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN assert the correct information was communicated
     assert "seems to be in wrong format" in caplog.text
 
 
 def test_validate_correct_bcl2fastq_sample_sheet(
-    cli_runner: CliRunner, sample_sheet_context: dict, novaseq_bcl2fastq_sample_sheet_path: Path
+    cli_runner: CliRunner,
+    sample_sheet_context: dict,
+    bcl2fastq_flow_cell_full_name: str,
+    novaseq_bcl2fastq_sample_sheet_path: Path,
 ):
     """Test validate sample sheet when using a bcl2fastq sample sheet."""
 
     # GIVEN the path to a bcl2fastq sample sheet that exists
     sample_sheet: Path = novaseq_bcl2fastq_sample_sheet_path
     assert sample_sheet.exists()
 
     # GIVEN that the sample sheet is correct
     get_sample_sheet_from_file(
         infile=sample_sheet,
-        bcl_converter=BclConverter.BCL2FASTQ,
+        flow_cell_sample_type=FlowCellSampleNovaSeq6000Bcl2Fastq,
     )
 
     # WHEN validating the sample sheet
     result: Result = cli_runner.invoke(
-        validate_sample_sheet, [str(sample_sheet)], obj=sample_sheet_context
+        validate_sample_sheet,
+        [bcl2fastq_flow_cell_full_name, str(sample_sheet)],
+        obj=sample_sheet_context,
     )
 
     # THEN assert that it exits successfully
     assert result.exit_code == EXIT_SUCCESS
 
 
 def test_validate_correct_dragen_sample_sheet(
-    cli_runner: CliRunner, sample_sheet_context: dict, novaseq_dragen_sample_sheet_path: Path
+    cli_runner: CliRunner,
+    sample_sheet_context: dict,
+    dragen_flow_cell_full_name: str,
+    novaseq_dragen_sample_sheet_path: Path,
 ):
     """Test validate sample sheet when using a Dragen sample sheet."""
 
     # GIVEN the path to a bcl2fastq sample sheet that exists
     sample_sheet: Path = novaseq_dragen_sample_sheet_path
     assert sample_sheet.exists()
 
     # GIVEN that the sample sheet is correct
-    get_sample_sheet_from_file(infile=sample_sheet, bcl_converter=BclConverter.DRAGEN)
+    get_sample_sheet_from_file(
+        infile=sample_sheet, flow_cell_sample_type=FlowCellSampleNovaSeq6000Dragen
+    )
 
     # WHEN validating the sample sheet
     result: Result = cli_runner.invoke(
         validate_sample_sheet,
-        [str(sample_sheet), "-b", BclConverter.DRAGEN.value],
+        [dragen_flow_cell_full_name, str(sample_sheet), "-b", BclConverter.DRAGEN.value],
         obj=sample_sheet_context,
     )
 
     # THEN assert that it exits successfully
     assert result.exit_code == EXIT_SUCCESS
```

### Comparing `cg-35.0.2/tests/cli/generate/report/conftest.py` & `cg-36.0.1/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-36.0.1/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/generate/report/test_utils.py` & `cg-36.0.1/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/generate/test_cli_base.py` & `cg-36.0.1/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/get/test_cli_get.py` & `cg-36.0.1/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/get/test_cli_get_analysis.py` & `cg-36.0.1/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/get/test_cli_get_case.py` & `cg-36.0.1/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/get/test_cli_get_flow_cell.py` & `cg-36.0.1/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/get/test_cli_get_sample.py` & `cg-36.0.1/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/set/conftest.py` & `cg-36.0.1/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/set/test_cli_set_case.py` & `cg-36.0.1/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/set/test_cli_set_cases.py` & `cg-36.0.1/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/set/test_cli_set_flowcell.py` & `cg-36.0.1/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/set/test_cli_set_list_keys.py` & `cg-36.0.1/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/set/test_cli_set_sample.py` & `cg-36.0.1/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/set/test_cli_set_samples.py` & `cg-36.0.1/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/store/test_fastq.py` & `cg-36.0.1/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/test_base.py` & `cg-36.0.1/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/test_clean.py` & `cg-36.0.1/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/conftest.py` & `cg-36.0.1/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_scout.py` & `cg-36.0.1/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_auto.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_fastq.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_genotype.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_gens.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_nipt.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/upload/test_cli_upload_observations.py` & `cg-36.0.1/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/balsamic/conftest.py` & `cg-36.0.1/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-36.0.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-36.0.1/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/balsamic/test_link.py` & `cg-36.0.1/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-36.0.1/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/balsamic/test_run.py` & `cg-36.0.1/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-36.0.1/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/conftest.py` & `cg-36.0.1/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-36.0.1/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/fluffy/conftest.py` & `cg-36.0.1/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-36.0.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-36.0.1/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-36.0.1/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-36.0.1/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-36.0.1/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/microsalt/conftest.py` & `cg-36.0.1/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-36.0.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-36.0.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-36.0.1/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/conftest.py` & `cg-36.0.1/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-36.0.1/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-36.0.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/taxprofiler/conftest.py` & `cg-36.0.1/tests/cli/workflow/taxprofiler/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-36.0.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py` & `cg-36.0.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/test_cli_workflow.py` & `cg-36.0.1/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-36.0.1/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/conftest.py` & `cg-36.0.1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from cg.io.controller import ReadFile, WriteFile
 from cg.io.json import write_json, read_json
 from cg.meta.rsync import RsyncAPI
 from cg.meta.transfer.external_data import ExternalDataAPI
 from cg.models import CompressionData
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.models.demultiplex.run_parameters import RunParametersNovaSeq6000, RunParametersNovaSeqX
 from cg.store import Store
 from cg.store.models import Bed, BedVersion, Customer, Organism, Family, Sample
 from tests.mocks.crunchy import MockCrunchyAPI
 from tests.mocks.hk_mock import MockHousekeeperAPI
 from tests.mocks.limsmock import MockLimsAPI
 from tests.mocks.madeline import MockMadelineAPI
@@ -857,45 +857,57 @@
     novaseq_x_run_parameters_path: Path,
 ) -> RunParametersNovaSeqX:
     """Return a NovaSeqX run parameters object."""
     return RunParametersNovaSeqX(run_parameters_path=novaseq_x_run_parameters_path)
 
 
 @pytest.fixture(name="bcl2fastq_flow_cell", scope="session")
-def fixture_flow_cell(bcl2fastq_flow_cell_dir: Path) -> FlowCell:
+def fixture_flow_cell(bcl2fastq_flow_cell_dir: Path) -> FlowCellDirectoryData:
     """Create a flow cell object with flow cell that is demultiplexed."""
-    return FlowCell(flow_cell_path=bcl2fastq_flow_cell_dir)
+    return FlowCellDirectoryData(
+        flow_cell_path=bcl2fastq_flow_cell_dir, bcl_converter=BclConverter.BCL2FASTQ
+    )
 
 
 @pytest.fixture(name="dragen_flow_cell", scope="session")
-def fixture_dragen_flow_cell(dragen_flow_cell_dir: Path) -> FlowCell:
+def fixture_dragen_flow_cell(dragen_flow_cell_dir: Path) -> FlowCellDirectoryData:
     """Create a dragen flow cell object with flow cell that is demultiplexed."""
-    return FlowCell(flow_cell_path=dragen_flow_cell_dir)
+    return FlowCellDirectoryData(
+        flow_cell_path=dragen_flow_cell_dir, bcl_converter=BclConverter.DRAGEN
+    )
+
+
+@pytest.fixture(name="novaseq_x_flow_cell", scope="session")
+def fixture_novaseq_x_flow_cell(novaseq_x_flow_cell_dir: Path) -> FlowCellDirectoryData:
+    """Create a NovaSeqX flow cell object with flow cell that is demultiplexed."""
+    return FlowCellDirectoryData(
+        flow_cell_path=novaseq_x_flow_cell_dir, bcl_converter=BclConverter.DRAGEN
+    )
 
 
 @pytest.fixture(name="bcl2fastq_flow_cell_id", scope="session")
-def fixture_bcl2fast2_flow_cell_id(bcl2fastq_flow_cell: FlowCell) -> str:
+def fixture_bcl2fast2_flow_cell_id(bcl2fastq_flow_cell: FlowCellDirectoryData) -> str:
     """Return flow cell id from bcl2fastq flow cell object."""
     return bcl2fastq_flow_cell.id
 
 
 @pytest.fixture(name="dragen_flow_cell_id", scope="session")
-def fixture_dragen_flow_cell_id(dragen_flow_cell: FlowCell) -> str:
+def fixture_dragen_flow_cell_id(dragen_flow_cell: FlowCellDirectoryData) -> str:
     """Return flow cell id from dragen flow cell object."""
     return dragen_flow_cell.id
 
 
 @pytest.fixture(name="demultiplexing_delivery_file")
-def fixture_demultiplexing_delivery_file(bcl2fastq_flow_cell: FlowCell) -> Path:
+def fixture_demultiplexing_delivery_file(bcl2fastq_flow_cell: FlowCellDirectoryData) -> Path:
     """Return demultiplexing delivery started file."""
     return Path(bcl2fastq_flow_cell.path, DemultiplexingDirsAndFiles.DELIVERY)
 
 
 @pytest.fixture(name="hiseq_x_tile_dir")
-def fixture_hiseq_x_tile_dir(bcl2fastq_flow_cell: FlowCell) -> Path:
+def fixture_hiseq_x_tile_dir(bcl2fastq_flow_cell: FlowCellDirectoryData) -> Path:
     """Return Hiseq X tile dir."""
     return Path(bcl2fastq_flow_cell.path, DemultiplexingDirsAndFiles.Hiseq_X_TILE_DIR)
 
 
 @pytest.fixture(name="lims_novaseq_samples_file")
 def fixture_lims_novaseq_samples_file(raw_lims_sample_dir: Path) -> Path:
     """Return the path to a file with sample info in lims format."""
@@ -915,15 +927,15 @@
     demultiplexed_runs: Path, bcl2fastq_flow_cell_full_name: str
 ) -> Path:
     return Path(demultiplexed_runs, bcl2fastq_flow_cell_full_name)
 
 
 @pytest.fixture(name="bcl2fastq_demux_results")
 def fixture_bcl2fastq_demux_results(
-    demultiplexed_flow_cell: Path, bcl2fastq_flow_cell: FlowCell
+    demultiplexed_flow_cell: Path, bcl2fastq_flow_cell: FlowCellDirectoryData
 ) -> DemuxResults:
     return DemuxResults(
         demux_dir=demultiplexed_flow_cell,
         flow_cell=bcl2fastq_flow_cell,
         bcl_converter=BclConverter.BCL2FASTQ,
     )
```

### Comparing `cg-35.0.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-36.0.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-36.0.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-36.0.1/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/analysis/sample_coverage.bed` & `cg-36.0.1/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/balsamic/case/config.json` & `cg-36.0.1/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-36.0.1/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-36.0.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-36.0.1/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-36.0.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-36.0.1/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-36.0.1/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/madeline/madeline.xml` & `cg-36.0.1/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-36.0.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-36.0.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/scout/643594.config.yaml` & `cg-36.0.1/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/scout/case_export.json` & `cg-36.0.1/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/scout/export_causatives.json` & `cg-36.0.1/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/scout/none_case_export.json` & `cg-36.0.1/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/scout/other_sex_case.json` & `cg-36.0.1/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/scout/panel_export.bed` & `cg-36.0.1/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/scout/panel_export.csv` & `cg-36.0.1/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv` & `cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv` & `cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml` & `cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv` & `cg-36.0.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/balsamic.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/fastq.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/metagenome.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/microsalt.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/mip.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/rml.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-36.0.1/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/data/SampleSheet.csv` & `cg-36.0.1/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/data/cgfixture.db` & `cg-36.0.1/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/data/hkstore.db` & `cg-36.0.1/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/io/example_json.json` & `cg-36.0.1/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-36.0.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/NIPT-json.json` & `cg-36.0.1/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-36.0.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-36.0.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/report/case_data.json` & `cg-36.0.1/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/report/lims_exported_samples.json` & `cg-36.0.1/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/fixtures/report/lims_family.json` & `cg-36.0.1/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/io/conftest.py` & `cg-36.0.1/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/io/test_io_controller.py` & `cg-36.0.1/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/io/test_io_csv.py` & `cg-36.0.1/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/io/test_io_json.py` & `cg-36.0.1/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/io/test_io_xml.py` & `cg-36.0.1/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/io/test_io_yaml.py` & `cg-36.0.1/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/io/test_validate_path.py` & `cg-36.0.1/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/archive/conftest.py` & `cg-36.0.1/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/archive/test_archiving.py` & `cg-36.0.1/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/backup/conftest.py` & `cg-36.0.1/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/backup/test_meta_backup.py` & `cg-36.0.1/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/backup/test_meta_pdc.py` & `cg-36.0.1/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/clean/conftest.py` & `cg-36.0.1/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-36.0.1/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-36.0.1/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/compress/conftest.py` & `cg-36.0.1/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/compress/test_clean_fastq.py` & `cg-36.0.1/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/compress/test_compress_files.py` & `cg-36.0.1/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/compress/test_compress_meta_fastq.py` & `cg-36.0.1/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/compress/test_decompress_spring_meta.py` & `cg-36.0.1/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-36.0.1/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/conftest.py` & `cg-36.0.1/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/deliver/conftest.py` & `cg-36.0.1/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/deliver/test_deliver_ticket.py` & `cg-36.0.1/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/deliver/test_delivery_api.py` & `cg-36.0.1/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/demultiplex/conftest.py` & `cg-36.0.1/tests/meta/demultiplex/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List
 
 from cg.apps.cgstats.stats import StatsAPI
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.meta.demultiplex.delete_demultiplex_api import DeleteDemuxAPI
 from cg.models.cg_config import CGConfig
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.store.api import Store
 from cg.store.models import Sample, Family
 
 from tests.apps.cgstats.conftest import fixture_populated_stats_api
 from tests.cli.demultiplex.conftest import (
     fixture_demultiplex_configs,
     fixture_demultiplex_context,
@@ -69,15 +69,15 @@
     tmp_flow_cell_run_path.mkdir(exist_ok=True, parents=True)
 
     return tmp_flow_cell_run_path
 
 
 @pytest.fixture(name="cgstats_select_project_log_file")
 def fixture_cgstats_select_project_log_file(
-    bcl2fastq_flow_cell: FlowCell, flow_cell_project_id: int
+    bcl2fastq_flow_cell: FlowCellDirectoryData, flow_cell_project_id: int
 ) -> Path:
     """Return cgstats select project out file."""
     return Path(
         bcl2fastq_flow_cell.path,
         "-".join(["stats", str(flow_cell_project_id), bcl2fastq_flow_cell.id]) + ".txt",
     )
 
@@ -85,15 +85,15 @@
 @pytest.fixture(name="flow_cell_project_id")
 def fixture_flow_cell_project_id() -> int:
     """Return flow cell run project id."""
     return 174578
 
 
 @pytest.fixture(name="hiseq_x_copy_complete_file")
-def fixture_hiseq_x_copy_complete_file(bcl2fastq_flow_cell: FlowCell) -> Path:
+def fixture_hiseq_x_copy_complete_file(bcl2fastq_flow_cell: FlowCellDirectoryData) -> Path:
     """Return Hiseq X flow cell copy complete file."""
     return Path(bcl2fastq_flow_cell.path, DemultiplexingDirsAndFiles.Hiseq_X_COPY_COMPLETE)
 
 
 @pytest.fixture(name="populated_flow_cell_store")
 def fixture_populated_flow_cell_store(
     family_name: str,
```

### Comparing `cg-35.0.2/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-36.0.1/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-36.0.1/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cg.meta.demultiplex.demux_post_processing import (
     DemuxPostProcessingAPI,
     DemuxPostProcessingHiseqXAPI,
 )
 from cg.meta.transfer import TransferFlowCell
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.store import Store
 
 
 def test_set_dry_run(
     demultiplex_context: CGConfig,
 ):
     # GIVEN a demultiplex context
@@ -31,15 +31,15 @@
     # THEN dry run should be True
     assert post_demux_api.dry_run is True
 
 
 def test_add_to_cgstats_dry_run(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
     post_demux_api: DemuxPostProcessingHiseqXAPI = DemuxPostProcessingHiseqXAPI(
@@ -55,15 +55,15 @@
     # THEN we should just log and exit
     assert "Dry run will not add flow cell stats" in caplog.text
 
 
 def test_add_to_cgstats(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
     post_demux_api: DemuxPostProcessingHiseqXAPI = DemuxPostProcessingHiseqXAPI(
@@ -76,15 +76,15 @@
     # THEN we should run the command
     assert f"add --machine X -u Unaligned {bcl2fastq_flow_cell.path}" in caplog.text
 
 
 def test_cgstats_select_project_dry_run(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     flow_cell_project_id: int,
     cgstats_select_project_log_file: Path,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN a demultiplex context
 
@@ -109,15 +109,15 @@
     # THEN we should just log and exit
     assert "Dry run will not process selected project" in caplog.text
 
 
 def test_cgstats_select_project(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     flow_cell_project_id: int,
     cgstats_select_project_log_file: Path,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN a demultiplex context
 
@@ -145,15 +145,15 @@
     # THEN we should run the command
     assert f"select --project {flow_cell_project_id} {bcl2fastq_flow_cell.id}" in caplog.text
 
 
 def test_cgstats_lanestats_dry_run(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
     post_demux_api: DemuxPostProcessingHiseqXAPI = DemuxPostProcessingHiseqXAPI(
@@ -169,15 +169,15 @@
     # THEN we should run the command
     assert "Dry run will not add lane stats" in caplog.text
 
 
 def test_cgstats_lanestats(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
     post_demux_api: DemuxPostProcessingHiseqXAPI = DemuxPostProcessingHiseqXAPI(
@@ -190,15 +190,15 @@
     # THEN we should run the command
     assert f"lanestats {bcl2fastq_flow_cell.path}" in caplog.text
 
 
 def test_finish_flow_cell_copy_not_completed(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     hiseq_x_copy_complete_file: Path,
 ):
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
@@ -224,15 +224,15 @@
     assert f"{bcl2fastq_flow_cell.full_name} is not yet completely copied" in caplog.text
 
 
 def test_finish_flow_cell_delivery_started(
     caplog,
     demultiplexing_delivery_file: Path,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
 ):
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
     post_demux_api: DemuxPostProcessingHiseqXAPI = DemuxPostProcessingHiseqXAPI(
@@ -258,15 +258,15 @@
         in caplog.text
     )
 
 
 def test_finish_flow_cell_delivery_not_hiseq_x(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     hiseq_x_tile_dir: Path,
 ):
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
@@ -288,15 +288,15 @@
     # THEN we should log that this is not an Hiseq X flow cell
     assert f"{bcl2fastq_flow_cell.full_name} is not an Hiseq X flow cell" in caplog.text
 
 
 def test_finish_flow_cell_ready(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     flow_cell_project_id: int,
     demultiplexing_delivery_file: Path,
     hiseq_x_tile_dir: Path,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
 ):
     caplog.set_level(logging.INFO)
 
@@ -334,15 +334,15 @@
 
 
 def test_post_process_flow_cell_dry_run(
     bcl2fastq_demux_results: DemuxResults,
     caplog,
     demultiplexing_delivery_file: Path,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     flow_cell_project_id: int,
     flowcell_store: Store,
     hiseq_x_tile_dir: Path,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
 ):
     caplog.set_level(logging.DEBUG)
 
@@ -378,15 +378,15 @@
 
 def test_post_process_flow_cell(
     bcl2fastq_demux_results: DemuxResults,
     caplog,
     cgstats_select_project_log_file: Path,
     demultiplexing_delivery_file: Path,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     flow_cell_project_id: int,
     flowcell_store: Store,
     hiseq_x_tile_dir: Path,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
 ):
     caplog.set_level(logging.DEBUG)
 
@@ -420,15 +420,15 @@
     # THEN we should also transfer the flow cell
     assert f"Flow cell added: {bcl2fastq_flow_cell.id}" in caplog.text
 
 
 def test_finish_flow_cell(
     caplog,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     hiseq_x_copy_complete_file: Path,
 ):
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
@@ -453,15 +453,15 @@
     assert f"Check demultiplexed flow cell {bcl2fastq_flow_cell.full_name}" in caplog.text
 
 
 def test_finish_all_flowcells(
     caplog,
     demultiplexed_flow_cell_working_directory: Path,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
     hiseq_x_copy_complete_file: Path,
 ):
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a demultiplex context
 
     # GIVEN a Demultiplexing post process API
```

### Comparing `cg-35.0.2/tests/meta/demultiplex/test_rename_files.py` & `cg-36.0.1/tests/meta/demultiplex/test_rename_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 
 from cg.meta.demultiplex.demux_post_processing import DemuxPostProcessingNovaseqAPI
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
 def test_rename_demux_result(
     demultiplexed_flow_cell_working_directory: Path,
     demultiplex_context: CGConfig,
-    bcl2fastq_flow_cell: FlowCell,
+    bcl2fastq_flow_cell: FlowCellDirectoryData,
 ):
     # GIVEN that this is the location of the demultiplex api
     demultiplex_context.demultiplex_api_.out_dir = demultiplexed_flow_cell_working_directory
     post_demux_api: DemuxPostProcessingNovaseqAPI = DemuxPostProcessingNovaseqAPI(
         config=demultiplex_context
     )
     demux_dir: Path = demultiplexed_flow_cell_working_directory
```

### Comparing `cg-35.0.2/tests/meta/encryption/conftest.py` & `cg-36.0.1/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/encryption/test_encryption.py` & `cg-36.0.1/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/observations/conftest.py` & `cg-36.0.1/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/observations/test_meta_upload_observations.py` & `cg-36.0.1/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/conftest.py` & `cg-36.0.1/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-36.0.1/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-36.0.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-36.0.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-36.0.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_meta_orders_api.py` & `cg-36.0.1/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_meta_orders_lims.py` & `cg-36.0.1/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_meta_orders_status.py` & `cg-36.0.1/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/orders/test_ticket_handler.py` & `cg-36.0.1/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/report/conftest.py` & `cg-36.0.1/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/report/test_balsamic_api.py` & `cg-36.0.1/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/report/test_field_validators.py` & `cg-36.0.1/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/report/test_mip_dna_api.py` & `cg-36.0.1/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/report/test_report_api.py` & `cg-36.0.1/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/report/test_rnafusion_api.py` & `cg-36.0.1/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/rsync/conftest.py` & `cg-36.0.1/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/rsync/test_rsync.py` & `cg-36.0.1/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/test_invoice.py` & `cg-36.0.1/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/transfer/conftest.py` & `cg-36.0.1/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/transfer/test_external_data.py` & `cg-36.0.1/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-36.0.1/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-36.0.1/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/balsamic/test_balsamic.py` & `cg-36.0.1/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/conftest.py` & `cg-36.0.1/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-36.0.1/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/mutacc/conftest.py` & `cg-36.0.1/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-36.0.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/nipt/conftest.py` & `cg-36.0.1/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-36.0.1/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/scout/conftest.py` & `cg-36.0.1/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/scout/test_generate_load_config.py` & `cg-36.0.1/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-36.0.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-36.0.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-36.0.1/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/test_meta_upload_coverage.py` & `cg-36.0.1/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/test_upload_api.py` & `cg-36.0.1/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/upload/test_upload_genotypes_api.py` & `cg-36.0.1/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/workflow/conftest.py` & `cg-36.0.1/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/workflow/test_analysis.py` & `cg-36.0.1/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/workflow/test_balsamic.py` & `cg-36.0.1/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/workflow/test_microsalt.py` & `cg-36.0.1/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-36.0.1/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/meta/workflow/test_rnafusion.py` & `cg-36.0.1/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/balsamic_analysis_mock.py` & `cg-36.0.1/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/crunchy.py` & `cg-36.0.1/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/hk_mock.py` & `cg-36.0.1/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/limsmock.py` & `cg-36.0.1/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/madeline.py` & `cg-36.0.1/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/mip_analysis_mock.py` & `cg-36.0.1/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/osticket.py` & `cg-36.0.1/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/process_mock.py` & `cg-36.0.1/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/report.py` & `cg-36.0.1/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/scout.py` & `cg-36.0.1/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/store_model.py` & `cg-36.0.1/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/mocks/tb_mock.py` & `cg-36.0.1/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/balsamic/conftest.py` & `cg-36.0.1/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/balsamic/test_balsamic_analysis.py` & `cg-36.0.1/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/conftest.py` & `cg-36.0.1/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/demultiplexing/conftest.py` & `cg-36.0.1/tests/models/demultiplexing/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from pathlib import Path
 
 import pytest
 
 from cg.constants.demultiplexing import BclConverter
 from cg.models.demultiplex.demux_results import DemuxResults
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
 @pytest.fixture(name="demultiplexed_dragen_flow_cell")
 def fixture_demultiplexed_dragen_flow_cell(
     demultiplexed_runs: Path, dragen_flow_cell_full_name: str
 ) -> Path:
     return Path(demultiplexed_runs, dragen_flow_cell_full_name)
 
 
 @pytest.fixture(name="dragen_demux_results")
 def fixture_dragen_demux_results(
-    demultiplexed_dragen_flow_cell: Path, dragen_flow_cell: FlowCell
+    demultiplexed_dragen_flow_cell: Path, dragen_flow_cell: FlowCellDirectoryData
 ) -> DemuxResults:
     return DemuxResults(
         demux_dir=demultiplexed_dragen_flow_cell,
         flow_cell=dragen_flow_cell,
         bcl_converter=BclConverter.DRAGEN,
     )
```

### Comparing `cg-35.0.2/tests/models/demultiplexing/test_demux_results.py` & `cg-36.0.1/tests/models/demultiplexing/test_demux_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 
 from cg.models.demultiplex.demux_results import DemuxResults, LogfileParameters
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
-def test_demux_results_instance(demultiplexed_flow_cell: Path, bcl2fastq_flow_cell: FlowCell):
+def test_demux_results_instance(
+    demultiplexed_flow_cell: Path, bcl2fastq_flow_cell: FlowCellDirectoryData
+):
     # GIVEN the path to a demultiplexed flow cell and a flow cell object
 
     # WHEN instantiating a demux results object
     demux_results = DemuxResults(
         demux_dir=demultiplexed_flow_cell, flow_cell=bcl2fastq_flow_cell, bcl_converter="bcl2fastq"
     )
```

### Comparing `cg-35.0.2/tests/models/demultiplexing/test_run_parameters.py` & `cg-36.0.1/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/mip/conftest.py` & `cg-36.0.1/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/mip/test_mip_analysis.py` & `cg-36.0.1/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/mip/test_mip_config.py` & `cg-36.0.1/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-36.0.1/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/mip/test_mip_sample_info.py` & `cg-36.0.1/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/nextflow/conftest.py` & `cg-36.0.1/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/nextflow/test_nextflow_deliver.py` & `cg-36.0.1/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/observations/conftest.py` & `cg-36.0.1/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/observations/test_observations_input_files.py` & `cg-36.0.1/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/report/test_validators.py` & `cg-36.0.1/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/rnafusion/conftest.py` & `cg-36.0.1/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-36.0.1/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/test_cg_models.py` & `cg-36.0.1/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/test_compression_data.py` & `cg-36.0.1/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/test_file_data.py` & `cg-36.0.1/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/models/test_flowcell_class.py` & `cg-36.0.1/tests/models/test_flowcell_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Tests for the demultiplex flow cell class."""
 from pathlib import Path
 
 import pytest
-from cg.models.demultiplex.flow_cell import FlowCell
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
 def test_get_run_parameters_when_non_existing(fixtures_dir: Path):
     # GIVEN a flowcell object with a directory without run parameters
     flowcell_path: Path = (
         fixtures_dir
         / "apps"
         / "demultiplexing"
         / "demultiplexed-runs"
         / "201203_A00689_0200_AHVKJCDRXX"
     )
-    flow_cell = FlowCell(flow_cell_path=flowcell_path)
+    flow_cell = FlowCellDirectoryData(flow_cell_path=flowcell_path)
     assert flow_cell.run_parameters_path.exists() is False
 
     # WHEN fetching the run parameters object
     with pytest.raises(FileNotFoundError):
         # THEN assert that a FileNotFound error is raised
         flow_cell.run_parameters
```

### Comparing `cg-35.0.2/tests/server/conftest.py` & `cg-36.0.1/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/add/test_store_add_application_version.py` & `cg-36.0.1/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/add/test_store_add_base.py` & `cg-36.0.1/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/add/test_store_add_customer.py` & `cg-36.0.1/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/add/test_store_add_flow_celll.py` & `cg-36.0.1/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/conftest.py` & `cg-36.0.1/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/delete/test_store_api_delete.py` & `cg-36.0.1/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/find/test_find_basic_data.py` & `cg-36.0.1/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-36.0.1/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/find/test_find_business_data.py` & `cg-36.0.1/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/find/test_find_business_data_analysis.py` & `cg-36.0.1/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/find/test_find_business_data_case.py` & `cg-36.0.1/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/find/test_find_business_data_sample.py` & `cg-36.0.1/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_analyses_to_clean.py` & `cg-36.0.1/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-36.0.1/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_store_api_status.py` & `cg-36.0.1/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_store_api_status_analysis.py` & `cg-36.0.1/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_store_api_status_cases.py` & `cg-36.0.1/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_store_api_status_customer.py` & `cg-36.0.1/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_store_api_status_pool.py` & `cg-36.0.1/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/status/test_store_api_status_sample.py` & `cg-36.0.1/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/api/test_base.py` & `cg-36.0.1/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/conftest.py` & `cg-36.0.1/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_analyses_filters.py` & `cg-36.0.1/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_application_filters.py` & `cg-36.0.1/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_application_version_filters.py` & `cg-36.0.1/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_bed_filters.py` & `cg-36.0.1/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_bed_version_filters.py` & `cg-36.0.1/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_case_sample_filters.py` & `cg-36.0.1/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_cases_filters.py` & `cg-36.0.1/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_collaboration_filters.py` & `cg-36.0.1/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_customer_filters.py` & `cg-36.0.1/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_flow_cell_filters.py` & `cg-36.0.1/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_invoice_filters.py` & `cg-36.0.1/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_organism_filters.py` & `cg-36.0.1/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_panel_filters.py` & `cg-36.0.1/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_pool_filters.py` & `cg-36.0.1/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_samples_filters.py` & `cg-36.0.1/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/filters/test_status_user_filters.py` & `cg-36.0.1/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/test_delivery.py` & `cg-36.0.1/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store/test_store_models.py` & `cg-36.0.1/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/store_helpers.py` & `cg-36.0.1/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/test_store_helpers.py` & `cg-36.0.1/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/utils/conftest.py` & `cg-36.0.1/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/utils/test_commands.py` & `cg-36.0.1/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/utils/test_date.py` & `cg-36.0.1/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/utils/test_dict.py` & `cg-36.0.1/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/utils/test_dispatcher.py` & `cg-36.0.1/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-35.0.2/tests/utils/test_utils.py` & `cg-36.0.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

