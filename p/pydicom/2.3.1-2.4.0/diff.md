# Comparing `tmp/pydicom-2.3.1.tar.gz` & `tmp/pydicom-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicom-2.3.1.tar", last modified: Mon Nov 14 16:38:47 2022, max compression
+gzip compressed data, was "pydicom-2.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydicom-2.3.1.tar` & `pydicom-2.4.0.tar`

### file list

```diff
@@ -1,508 +1,440 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.384712 pydicom-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     9179 2022-11-14 16:38:39.000000 pydicom-2.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-11-14 16:38:39.000000 pydicom-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-11-14 16:38:39.000000 pydicom-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2022-11-14 16:38:47.384712 pydicom-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5469 2022-11-14 16:38:39.000000 pydicom-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     7153 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.320711 pydicom-2.3.1/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/_static/css/pydicom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/_templates/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.320711 pydicom-2.3.1/doc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/doc/assets/img/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/assets/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     5693 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/assets/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    33703 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/assets/img/pydicom_blue_light.png
--rw-r--r--   0 runner    (1001) docker     (121)    12643 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/assets/img/pydicom_blue_light.svg
--rw-r--r--   0 runner    (1001) docker     (121)    33283 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/assets/img/pydicom_flat_black.png
--rw-r--r--   0 runner    (1001) docker     (121)    12173 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/assets/img/pydicom_flat_black.svg
--rw-r--r--   0 runner    (1001) docker     (121)    29209 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/assets/img/pydicom_flat_black_alpha.png
--rw-r--r--   0 runner    (1001) docker     (121)    10525 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.332711 pydicom-2.3.1/doc/faq/
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/faq/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.332711 pydicom-2.3.1/doc/guides/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.332711 pydicom-2.3.1/doc/guides/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     5015 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/cli/cli_codify.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/cli/cli_dev.rst
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/cli/cli_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7729 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/cli/cli_intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5852 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/cli/cli_show.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11425 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/element_value_types.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.332711 pydicom-2.3.1/doc/guides/encoding/
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/encoding/encoder_plugin_options.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5137 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/encoding/encoder_plugins.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/encoding/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7283 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/encoding/rle_lossless.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/guides/writing_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.332711 pydicom-2.3.1/doc/old/
--rw-r--r--   0 runner    (1001) docker     (121)    11094 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/base_element.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/best_practices.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2854 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5612 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/image_data_compression.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/image_data_handlers.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5176 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/private_data_elements.rst
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/pydicom_user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/python2_support.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/ref_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/transition_to_pydicom1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/viewing_images.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/working_with_overlays.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8221 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/working_with_pixel_data.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/working_with_waveforms.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/old/writing_files.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.336711 pydicom-2.3.1/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/charset.rst
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/config.rst
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/data.rst
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/datadict.rst
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/dataset.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/dicomdir.rst
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/elem.dataelem.rst
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/elem.multival.rst
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/elem.rst
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/elem.sequence.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/elem.tag.rst
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/elem.valuerep.rst
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/elem.values.rst
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/encaps.rst
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/encoders.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/errors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/fileio.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/fileio.read.rst
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/fileio.rst
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/fileio.util.rst
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/fileio.write.rst
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/fileset.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/handlers.overlay_data.rst
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/handlers.pixel_data.rst
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/handlers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/handlers.waveform_data.rst
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7525 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/reference/uid.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.340711 pydicom-2.3.1/doc/release_notes/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.3.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.4.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.5.rst
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.6.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.7.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.8.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v0.9.9.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v1.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v1.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v1.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v1.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v1.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v1.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v2.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7542 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v2.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v2.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6511 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v2.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/release_notes/v2.3.0.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.340711 pydicom-2.3.1/doc/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10607 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/contributing_code.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9568 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/contributing_docs.rst
--rw-r--r--   0 runner    (1001) docker     (121)    22994 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/dataset_basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/dicom_json.rst
--rw-r--r--   0 runner    (1001) docker     (121)    19508 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/filesets.rst
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.340711 pydicom-2.3.1/doc/tutorials/pixel_data/
--rw-r--r--   0 runner    (1001) docker     (121)     7747 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/pixel_data/compressing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/sr_basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9581 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/virtualenvs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9196 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/waveforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.340711 pydicom-2.3.1/doc/tutorials/waveforms_assets/
--rw-r--r--   0 runner    (1001) docker     (121)   135332 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/waveforms_assets/waveforms_decode.png
--rw-r--r--   0 runner    (1001) docker     (121)    90122 2022-11-14 16:38:39.000000 pydicom-2.3.1/doc/tutorials/waveforms_assets/waveforms_encode.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.340711 pydicom-2.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/dicomtree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.340711 pydicom-2.3.1/examples/image_processing/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/image_processing/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/image_processing/plot_downsize_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/image_processing/plot_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/image_processing/reslice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.340711 pydicom-2.3.1/examples/input_output/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/input_output/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/input_output/plot_printing_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/input_output/plot_read_dicom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/input_output/plot_read_dicom_directory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4465 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/input_output/plot_read_fileset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/input_output/plot_read_rtplan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/input_output/plot_write_dicom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/memory_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.344711 pydicom-2.3.1/examples/metadata_processing/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/metadata_processing/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/metadata_processing/plot_add_dict_entries.py
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/metadata_processing/plot_anonymize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/metadata_processing/plot_sequences.py
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/plot_dicom_difference.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-11-14 16:38:39.000000 pydicom-2.3.1/examples/show_charset_name.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.348711 pydicom-2.3.1/pydicom/
--rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   494937 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/_dicom_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)   613172 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/_private_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/_storage_sopclass_uids.py
--rw-r--r--   0 runner    (1001) docker     (121)    63470 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/_uid_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.348711 pydicom-2.3.1/pydicom/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/benchmarks/bench_encaps.py
--rw-r--r--   0 runner    (1001) docker     (121)     7943 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/benchmarks/bench_handler_numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/benchmarks/bench_pixel_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/benchmarks/bench_rle_decode.py
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/benchmarks/bench_rle_encode.py
--rw-r--r--   0 runner    (1001) docker     (121)    31107 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/charset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.348711 pydicom-2.3.1/pydicom/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/cli/codify.py
--rw-r--r--   0 runner    (1001) docker     (121)     7281 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5323 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    18383 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.348711 pydicom-2.3.1/pydicom/data/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.352712 pydicom-2.3.1/pydicom/data/charset_files/
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/FileInfo.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrArab.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrFren.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrFrenMulti.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrGerm.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrGreek.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrH31.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrH32.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrHbrw.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrI2.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrJapMulti.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrKoreanMulti.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrRuss.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrSQEncoding.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrSQEncoding1.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrX1.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/charset_files/chrX2.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    11895 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     8190 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     6297 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/hashes.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.352712 pydicom-2.3.1/pydicom/data/palettes/
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/fall.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4754 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/hotiron.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4776 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/hotmetalblue.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/pet.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/pet20step.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/spring.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/summer.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/palettes/winter.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.360712 pydicom-2.3.1/pydicom/data/test_files/
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/693_J2KI.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    39206 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/CT_small.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    15412 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/ExplVR_BigEnd.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/ExplVR_BigEndNoMeta.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/ExplVR_LitEndNoMeta.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    30706 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm
--rw-r--r--   0 runner    (1001) docker     (121)   138518 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9844 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/JPEG-lossy.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/JPEG2000.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9844 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/JPGExtended.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9830 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small_RLE.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9708 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small_bigendian.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9846 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small_expb.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9702 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small_implicit.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     6008 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small_jp2klossless.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9958 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_small_padded.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9630 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/MR_truncated.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    15389 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4310 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4464 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4310 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm
--rw-r--r--   0 runner    (1001) docker     (121)   197506 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     5042 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_16bit.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3896 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2696 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_2frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_32bit.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     6246 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_small_odd.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    21686 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/UN_sequence.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     7618 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/badVR.dcm
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR1/
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR2/
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR3/
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293
--rw-r--r--   0 runner    (1001) docker     (121)     3908 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023
--rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.364712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.368712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678
--rw-r--r--   0 runner    (1001) docker     (121)    11116 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR
--rw-r--r--   0 runner    (1001) docker     (121)    11116 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-empty.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    11110 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit
--rw-r--r--   0 runner    (1001) docker     (121)    11092 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset
--rw-r--r--   0 runner    (1001) docker     (121)    11116 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient
--rw-r--r--   0 runner    (1001) docker     (121)    11116 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.368712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/
--rw-r--r--   0 runner    (1001) docker     (121)    13066 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.328711 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.372712 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/empty_charset_LEI.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4637 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/image_dfl.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    37084 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/liver_1frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    36532 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/liver_expb_1frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/meta_missing_tsyntax.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/nested_priv_SQ.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    38871 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/no_meta.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/no_meta_group_length.dcm
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/priv_SQ.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/reportsi.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     7568 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtdose.dcm
--rwxr-xr-x   0 runner    (1001) docker     (121)     1958 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtdose_1frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     7618 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtdose_expb.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtdose_expb_1frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     6816 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtdose_rle.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtdose_rle_1frame.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtplan.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    14474 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtplan.dump
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtplan_truncated.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtstruct.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     7935 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/rtstruct.dump
--rw-r--r--   0 runner    (1001) docker     (121)     6796 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/test-SR.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    20965 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/test1.json
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/test_PN.json
--rwxr-xr-x   0 runner    (1001) docker     (121)   291088 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/waveform_ecg.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     6958 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/test_files/zipMR.gz
--rw-r--r--   0 runner    (1001) docker     (121)     9463 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/data/urls.json
--rw-r--r--   0 runner    (1001) docker     (121)    18384 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/datadict.py
--rw-r--r--   0 runner    (1001) docker     (121)    31095 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/dataelem.py
--rw-r--r--   0 runner    (1001) docker     (121)   106270 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/dicomdir.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/dicomio.py
--rw-r--r--   0 runner    (1001) docker     (121)    26824 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/encaps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.372712 pydicom-2.3.1/pydicom/encoders/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36135 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5901 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/encoders/gdcm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/encoders/native.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/encoders/pylibjpeg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/env_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7794 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/filebase.py
--rw-r--r--   0 runner    (1001) docker     (121)    44269 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/filereader.py
--rw-r--r--   0 runner    (1001) docker     (121)   102357 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/fileset.py
--rw-r--r--   0 runner    (1001) docker     (121)    14625 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/fileutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    44257 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/filewriter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12252 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/jsonrep.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5140 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/multival.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.372712 pydicom-2.3.1/pydicom/overlay_data_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/overlay_data_handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.372712 pydicom-2.3.1/pydicom/overlays/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/overlays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9951 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/overlays/numpy_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.372712 pydicom-2.3.1/pydicom/pixel_data_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9761 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/gdcm_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/jpeg_ls_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    11644 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/numpy_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     8695 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/pillow_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    11053 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/pylibjpeg_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    16581 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/rle_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    54704 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/pixel_data_handlers/util.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5980 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.380712 pydicom-2.3.1/pydicom/sr/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/sr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   788696 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/sr/_cid_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)  2725654 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/sr/_concepts_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)   424514 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/sr/_snomed_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    11035 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/sr/codedict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/sr/coding.py
--rw-r--r--   0 runner    (1001) docker     (121)     8083 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.384712 pydicom-2.3.1/pydicom/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/_write_stds.py
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_JPEG_LS_transfer_syntax.py
--rw-r--r--   0 runner    (1001) docker     (121)    23452 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_charset.py
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    12639 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_codes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7289 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11331 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    37245 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_dataelem.py
--rw-r--r--   0 runner    (1001) docker     (121)    83588 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_dicomdir.py
--rw-r--r--   0 runner    (1001) docker     (121)     6640 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)    51853 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_encaps.py
--rw-r--r--   0 runner    (1001) docker     (121)    40830 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)     9907 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_encoders_gdcm.py
--rw-r--r--   0 runner    (1001) docker     (121)    16304 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_encoders_pydicom.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_env_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     9238 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_filebase.py
--rw-r--r--   0 runner    (1001) docker     (121)    64476 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_filereader.py
--rw-r--r--   0 runner    (1001) docker     (121)   103370 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_fileset.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_fileutil.py
--rw-r--r--   0 runner    (1001) docker     (121)   108880 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_filewriter.py
--rw-r--r--   0 runner    (1001) docker     (121)    22694 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_gdcm_pixel_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    91897 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_handler_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    10049 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_jpeg_ls_pixel_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    19207 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5701 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_multival.py
--rw-r--r--   0 runner    (1001) docker     (121)    51663 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_numpy_pixel_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    15710 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_overlay_np.py
--rw-r--r--   0 runner    (1001) docker     (121)    23921 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_pillow_pixel_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    30823 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_pylibjpeg.py
--rw-r--r--   0 runner    (1001) docker     (121)    23320 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_rawread.py
--rw-r--r--   0 runner    (1001) docker     (121)    44734 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_rle_pixel_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5323 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    15696 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)    16663 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_uid.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_unicode.py
--rw-r--r--   0 runner    (1001) docker     (121)    18477 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    59725 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_valuerep.py
--rw-r--r--   0 runner    (1001) docker     (121)     8633 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     5250 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/tests/test_waveform.py
--rw-r--r--   0 runner    (1001) docker     (121)    34984 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.384712 pydicom-2.3.1/pydicom/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15674 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/util/codify.py
--rw-r--r--   0 runner    (1001) docker     (121)     3956 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/util/dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/util/fixer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/util/hexutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/util/leanread.py
--rw-r--r--   0 runner    (1001) docker     (121)    66982 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/valuerep.py
--rw-r--r--   0 runner    (1001) docker     (121)    25894 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/values.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.384712 pydicom-2.3.1/pydicom/waveforms/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8584 2022-11-14 16:38:39.000000 pydicom-2.3.1/pydicom/waveforms/numpy_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:38:47.348711 pydicom-2.3.1/pydicom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2022-11-14 16:38:47.000000 pydicom-2.3.1/pydicom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18514 2022-11-14 16:38:47.000000 pydicom-2.3.1/pydicom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 16:38:47.000000 pydicom-2.3.1/pydicom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-14 16:38:47.000000 pydicom-2.3.1/pydicom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 16:38:47.000000 pydicom-2.3.1/pydicom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-14 16:38:47.000000 pydicom-2.3.1/pydicom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-14 16:38:47.000000 pydicom-2.3.1/pydicom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-14 16:38:47.388712 pydicom-2.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2761 2022-11-14 16:38:39.000000 pydicom-2.3.1/setup.py
+-rw-r--r--   0        0        0      588 2023-06-13 16:06:05.695394 pydicom-2.4.0/.circleci/config.yml
+-rw-r--r--   0        0        0      114 2023-06-13 16:06:05.695394 pydicom-2.4.0/.codespellrc
+-rw-r--r--   0        0        0       58 2023-06-13 16:06:05.695394 pydicom-2.4.0/.coveragerc
+-rw-r--r--   0        0        0       18 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      678 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      387 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      519 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      195 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/other_issues.md
+-rw-r--r--   0        0        0     1398 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/pixel_issue.md
+-rw-r--r--   0        0        0      626 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       19 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/codespell_ignore_words.txt
+-rw-r--r--   0        0        0     3351 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/merge-pytest.yml
+-rw-r--r--   0        0        0      743 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/merge-typing.yml
+-rw-r--r--   0        0        0     5501 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/pr-pytest.yml
+-rw-r--r--   0        0        0      360 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/pr-run-linters.yml
+-rw-r--r--   0        0        0      916 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/pr-type-spell.yml
+-rw-r--r--   0        0        0     1220 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/publish-pypi-deploy.yml
+-rw-r--r--   0        0        0      714 2023-06-13 16:06:05.695394 pydicom-2.4.0/.gitignore
+-rw-r--r--   0        0        0      197 2023-06-13 16:06:05.695394 pydicom-2.4.0/.lgtm.yml
+-rw-r--r--   0        0        0       62 2023-06-13 16:06:05.695394 pydicom-2.4.0/.pep8speaks.yml
+-rw-r--r--   0        0        0     9179 2023-06-13 16:06:05.695394 pydicom-2.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3196 2023-06-13 16:06:05.695394 pydicom-2.4.0/LICENSE
+-rw-r--r--   0        0        0      163 2023-06-13 16:06:05.695394 pydicom-2.4.0/MANIFEST.in
+-rw-r--r--   0        0        0      684 2023-06-13 16:06:05.695394 pydicom-2.4.0/Makefile
+-rw-r--r--   0        0        0     6055 2023-06-13 16:06:05.695394 pydicom-2.4.0/README.md
+-rw-r--r--   0        0        0     2488 2023-06-13 16:06:05.695394 pydicom-2.4.0/asv.conf.json
+-rw-r--r--   0        0        0        0 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_encaps.py
+-rw-r--r--   0        0        0     7943 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_handler_numpy.py
+-rw-r--r--   0        0        0     2989 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_nested_seq.py
+-rw-r--r--   0        0        0     2080 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_pixel_util.py
+-rw-r--r--   0        0        0     4160 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_rle_decode.py
+-rw-r--r--   0        0        0     3310 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_rle_encode.py
+-rwxr-xr-x   0        0        0     3049 2023-06-13 16:06:05.695394 pydicom-2.4.0/build_tools/circle/build_doc.sh
+-rwxr-xr-x   0        0        0     3520 2023-06-13 16:06:05.695394 pydicom-2.4.0/build_tools/circle/push_doc.sh
+-rw-r--r--   0        0        0     2811 2023-06-13 16:06:05.695394 pydicom-2.4.0/build_tools/sphinx/github_link.py
+-rw-r--r--   0        0        0      466 2023-06-13 16:06:05.695394 pydicom-2.4.0/dicom.py
+-rw-r--r--   0        0        0     7153 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/Makefile
+-rw-r--r--   0        0        0     1209 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/README.md
+-rw-r--r--   0        0        0     1751 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/_static/css/pydicom.css
+-rw-r--r--   0        0        0      290 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/_templates/class.rst
+-rw-r--r--   0        0        0      229 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/_templates/function.rst
+-rw-r--r--   0        0        0     1150 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/favicon.ico
+-rw-r--r--   0        0        0     5693 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/logo.png
+-rw-r--r--   0        0        0    33703 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/pydicom_blue_light.png
+-rw-r--r--   0        0        0    12643 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/pydicom_blue_light.svg
+-rw-r--r--   0        0        0    33283 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/assets/img/pydicom_flat_black.png
+-rw-r--r--   0        0        0    12173 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/assets/img/pydicom_flat_black.svg
+-rw-r--r--   0        0        0    29209 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/assets/img/pydicom_flat_black_alpha.png
+-rw-r--r--   0        0        0    10529 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/conf.py
+-rw-r--r--   0        0        0     3262 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/faq/index.rst
+-rw-r--r--   0        0        0     5015 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_codify.rst
+-rw-r--r--   0        0        0     2886 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_dev.rst
+-rw-r--r--   0        0        0      410 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_guide.rst
+-rw-r--r--   0        0        0     7729 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_intro.rst
+-rw-r--r--   0        0        0     5852 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_show.rst
+-rw-r--r--   0        0        0    11425 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/element_value_types.rst
+-rw-r--r--   0        0        0     1932 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/encoder_plugin_options.rst
+-rw-r--r--   0        0        0     5137 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/encoder_plugins.rst
+-rw-r--r--   0        0        0      270 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/index.rst
+-rw-r--r--   0        0        0     7283 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/rle_lossless.rst
+-rw-r--r--   0        0        0     5283 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/glossary.rst
+-rw-r--r--   0        0        0      245 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/index.rst
+-rw-r--r--   0        0        0     3998 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/writing_documentation.rst
+-rw-r--r--   0        0        0     1742 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/index.rst
+-rw-r--r--   0        0        0     3073 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/make.bat
+-rw-r--r--   0        0        0    11081 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/base_element.rst
+-rw-r--r--   0        0        0     4599 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/best_practices.rst
+-rw-r--r--   0        0        0     2854 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/getting_started.rst
+-rw-r--r--   0        0        0     5612 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/image_data_compression.rst
+-rw-r--r--   0        0        0     7357 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/image_data_handlers.rst
+-rw-r--r--   0        0        0     5176 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/private_data_elements.rst
+-rw-r--r--   0        0        0      337 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/pydicom_user_guide.rst
+-rw-r--r--   0        0        0      524 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/python2_support.rst
+-rw-r--r--   0        0        0     1090 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/ref_guide.rst
+-rw-r--r--   0        0        0     5049 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/transition_to_pydicom1.rst
+-rw-r--r--   0        0        0     2644 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/viewing_images.rst
+-rw-r--r--   0        0        0     3614 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/working_with_overlays.rst
+-rw-r--r--   0        0        0     8221 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/working_with_pixel_data.rst
+-rw-r--r--   0        0        0     3235 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/working_with_waveforms.rst
+-rw-r--r--   0        0        0     3779 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/writing_files.rst
+-rw-r--r--   0        0        0      327 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/charset.rst
+-rw-r--r--   0        0        0      774 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/config.rst
+-rw-r--r--   0        0        0      314 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/data.rst
+-rw-r--r--   0        0        0      802 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/datadict.rst
+-rw-r--r--   0        0        0      341 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/dataset.rst
+-rw-r--r--   0        0        0      233 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/dicomdir.rst
+-rw-r--r--   0        0        0      280 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.dataelem.rst
+-rw-r--r--   0        0        0      301 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.multival.rst
+-rw-r--r--   0        0        0      224 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.rst
+-rw-r--r--   0        0        0      335 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.sequence.rst
+-rw-r--r--   0        0        0      267 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.tag.rst
+-rw-r--r--   0        0        0      495 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.valuerep.rst
+-rw-r--r--   0        0        0      589 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.values.rst
+-rw-r--r--   0        0        0      723 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/encaps.rst
+-rw-r--r--   0        0        0      574 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/encoders.rst
+-rw-r--r--   0        0        0      186 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/errors.rst
+-rw-r--r--   0        0        0      275 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.base.rst
+-rw-r--r--   0        0        0      480 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.read.rst
+-rw-r--r--   0        0        0      221 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.rst
+-rw-r--r--   0        0        0      331 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.util.rst
+-rw-r--r--   0        0        0      632 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.write.rst
+-rw-r--r--   0        0        0      325 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileset.rst
+-rw-r--r--   0        0        0      285 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.overlay_data.rst
+-rw-r--r--   0        0        0      398 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.pixel_data.rst
+-rw-r--r--   0        0        0      615 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.rst
+-rw-r--r--   0        0        0      276 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.waveform_data.rst
+-rw-r--r--   0        0        0      399 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/index.rst
+-rw-r--r--   0        0        0      218 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/misc.rst
+-rw-r--r--   0        0        0     7525 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/uid.rst
+-rw-r--r--   0        0        0      523 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/index.rst
+-rw-r--r--   0        0        0     1959 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.2.rst
+-rw-r--r--   0        0        0     1625 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.3.rst
+-rw-r--r--   0        0        0     3132 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.4.rst
+-rw-r--r--   0        0        0     1320 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.5.rst
+-rw-r--r--   0        0        0      708 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.6.rst
+-rw-r--r--   0        0        0     2522 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.7.rst
+-rw-r--r--   0        0        0     1736 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.8.rst
+-rw-r--r--   0        0        0     1261 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.9.rst
+-rw-r--r--   0        0        0     3448 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.0.0.rst
+-rw-r--r--   0        0        0     2043 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.1.0.rst
+-rw-r--r--   0        0        0     3570 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.2.0.rst
+-rw-r--r--   0        0        0     3069 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.3.0.rst
+-rw-r--r--   0        0        0     4371 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.4.0.rst
+-rw-r--r--   0        0        0      358 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.4.1.rst
+-rw-r--r--   0        0        0     2806 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v2.0.0.rst
+-rw-r--r--   0        0        0     7542 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v2.1.0.rst
+-rw-r--r--   0        0        0      219 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v2.1.1.rst
+-rw-r--r--   0        0        0     6511 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/release_notes/v2.2.0.rst
+-rw-r--r--   0        0        0     2893 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/release_notes/v2.3.0.rst
+-rw-r--r--   0        0        0     2155 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/release_notes/v2.4.0.rst
+-rw-r--r--   0        0        0     1081 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/contributing.rst
+-rw-r--r--   0        0        0    10607 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/contributing_code.rst
+-rw-r--r--   0        0        0     9568 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/contributing_docs.rst
+-rw-r--r--   0        0        0    22994 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/dataset_basics.rst
+-rw-r--r--   0        0        0     4390 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/dicom_json.rst
+-rw-r--r--   0        0        0    19523 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/filesets.rst
+-rw-r--r--   0        0        0      311 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/index.rst
+-rw-r--r--   0        0        0     5487 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/installation.rst
+-rw-r--r--   0        0        0     7747 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/pixel_data/compressing.rst
+-rw-r--r--   0        0        0     2153 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/sr_basics.rst
+-rw-r--r--   0        0        0     9581 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/virtualenvs.rst
+-rw-r--r--   0        0        0     9195 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/waveforms.rst
+-rw-r--r--   0        0        0   135332 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_decode.png
+-rw-r--r--   0        0        0    90122 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_encode.png
+-rw-r--r--   0        0        0       77 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/README.txt
+-rw-r--r--   0        0        0     3481 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/dicomtree.py
+-rw-r--r--   0        0        0      173 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/README.txt
+-rw-r--r--   0        0        0     1377 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/plot_downsize_image.py
+-rw-r--r--   0        0        0     1541 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/plot_waveforms.py
+-rw-r--r--   0        0        0     2126 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/reslice.py
+-rw-r--r--   0        0        0      119 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/README.txt
+-rw-r--r--   0        0        0     1563 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_printing_dataset.py
+-rw-r--r--   0        0        0     1165 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_dicom.py
+-rw-r--r--   0        0        0     2794 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_dicom_directory.py
+-rw-r--r--   0        0        0     4465 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_fileset.py
+-rw-r--r--   0        0        0     1123 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_rtplan.py
+-rw-r--r--   0        0        0     2401 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_write_dicom.py
+-rw-r--r--   0        0        0     2392 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/memory_dataset.py
+-rw-r--r--   0        0        0      177 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/README.txt
+-rw-r--r--   0        0        0     1410 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/plot_add_dict_entries.py
+-rw-r--r--   0        0        0     2787 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/plot_anonymize.py
+-rw-r--r--   0        0        0     1071 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/plot_sequences.py
+-rw-r--r--   0        0        0     1033 2023-06-13 16:06:05.707394 pydicom-2.4.0/examples/plot_dicom_difference.py
+-rw-r--r--   0        0        0     1286 2023-06-13 16:06:05.707394 pydicom-2.4.0/examples/show_charset_name.py
+-rw-r--r--   0        0        0      330 2023-06-13 16:06:05.707394 pydicom-2.4.0/mypy.ini
+-rw-r--r--   0        0        0     1577 2023-06-13 16:06:05.707394 pydicom-2.4.0/pydicom/__init__.py
+-rw-r--r--   0        0        0   509435 2023-06-13 16:06:05.707394 pydicom-2.4.0/pydicom/_dicom_dict.py
+-rw-r--r--   0        0        0   613172 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_private_dict.py
+-rw-r--r--   0        0        0      130 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_storage_sopclass_uids.py
+-rw-r--r--   0        0        0    65890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_uid_dict.py
+-rw-r--r--   0        0        0      379 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_version.py
+-rw-r--r--   0        0        0    31107 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/charset.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/__init__.py
+-rw-r--r--   0        0        0     1001 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/codify.py
+-rw-r--r--   0        0        0     7670 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/main.py
+-rw-r--r--   0        0        0     5323 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/show.py
+-rw-r--r--   0        0        0      607 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/compat.py
+-rw-r--r--   0        0        0    18738 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/config.py
+-rw-r--r--   0        0        0      403 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/__init__.py
+-rw-r--r--   0        0        0     1896 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/FileInfo.txt
+-rw-r--r--   0        0        0     1892 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrArab.dcm
+-rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrFren.dcm
+-rw-r--r--   0        0        0     1938 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrFrenMulti.dcm
+-rw-r--r--   0        0        0     1894 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrGerm.dcm
+-rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrGreek.dcm
+-rw-r--r--   0        0        0     1950 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrH31.dcm
+-rw-r--r--   0        0        0     1960 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrH32.dcm
+-rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrHbrw.dcm
+-rw-r--r--   0        0        0     1934 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrI2.dcm
+-rw-r--r--   0        0        0     1918 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrJapMulti.dcm
+-rw-r--r--   0        0        0     1940 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm
+-rw-r--r--   0        0        0     1898 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrKoreanMulti.dcm
+-rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrRuss.dcm
+-rw-r--r--   0        0        0      520 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding.dcm
+-rw-r--r--   0        0        0      520 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding1.dcm
+-rw-r--r--   0        0        0     1910 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrX1.dcm
+-rw-r--r--   0        0        0     1904 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrX2.dcm
+-rw-r--r--   0        0        0    11895 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/data_manager.py
+-rw-r--r--   0        0        0     8205 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/download.py
+-rw-r--r--   0        0        0     6297 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/hashes.json
+-rw-r--r--   0        0        0     1725 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/README.md
+-rw-r--r--   0        0        0     4078 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/fall.dcm
+-rw-r--r--   0        0        0     4754 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/hotiron.dcm
+-rw-r--r--   0        0        0     4776 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/hotmetalblue.dcm
+-rw-r--r--   0        0        0     4732 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/pet.dcm
+-rw-r--r--   0        0        0     4790 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/pet20step.dcm
+-rw-r--r--   0        0        0     4104 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/palettes/spring.dcm
+-rw-r--r--   0        0        0     4100 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/palettes/summer.dcm
+-rw-r--r--   0        0        0     4112 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/palettes/winter.dcm
+-rw-r--r--   0        0        0     2057 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/retry.py
+-rw-r--r--   0        0        0     3590 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/693_J2KI.dcm
+-rw-r--r--   0        0        0    39206 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/CT_small.dcm
+-rw-r--r--   0        0        0    15412 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/ExplVR_BigEnd.dcm
+-rw-r--r--   0        0        0      434 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/ExplVR_BigEndNoMeta.dcm
+-rw-r--r--   0        0        0      434 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/ExplVR_LitEndNoMeta.dcm
+-rw-r--r--   0        0        0    30706 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm
+-rw-r--r--   0        0        0   138518 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm
+-rw-r--r--   0        0        0     9844 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPEG-lossy.dcm
+-rw-r--r--   0        0        0     3308 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm
+-rw-r--r--   0        0        0     3308 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPEG2000.dcm
+-rw-r--r--   0        0        0     9844 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPGExtended.dcm
+-rw-r--r--   0        0        0     9830 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small.dcm
+-rw-r--r--   0        0        0     7790 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_RLE.dcm
+-rw-r--r--   0        0        0     9708 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_bigendian.dcm
+-rw-r--r--   0        0        0     9846 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_expb.dcm
+-rw-r--r--   0        0        0     9702 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_implicit.dcm
+-rw-r--r--   0        0        0     6008 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_jp2klossless.dcm
+-rw-r--r--   0        0        0     6124 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm
+-rw-r--r--   0        0        0     9958 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_padded.dcm
+-rw-r--r--   0        0        0     9630 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_truncated.dcm
+-rw-r--r--   0        0        0    15439 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/README.txt
+-rw-r--r--   0        0        0     4316 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm
+-rw-r--r--   0        0        0     4310 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm
+-rw-r--r--   0        0        0     3626 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm
+-rw-r--r--   0        0        0     3136 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm
+-rw-r--r--   0        0        0     3090 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm
+-rw-r--r--   0        0        0     3140 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm
+-rw-r--r--   0        0        0     3094 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm
+-rw-r--r--   0        0        0     3420 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm
+-rw-r--r--   0        0        0     2998 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm
+-rw-r--r--   0        0        0     4464 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg.dcm
+-rw-r--r--   0        0        0     4310 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm
+-rw-r--r--   0        0        0   197506 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm
+-rw-r--r--   0        0        0     3424 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm
+-rw-r--r--   0        0        0     5204 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm
+-rw-r--r--   0        0        0     5042 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm
+-rw-r--r--   0        0        0     2006 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle.dcm
+-rw-r--r--   0        0        0     2606 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit.dcm
+-rw-r--r--   0        0        0     3896 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm
+-rw-r--r--   0        0        0     2696 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_2frame.dcm
+-rw-r--r--   0        0        0     3760 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit.dcm
+-rw-r--r--   0        0        0     6246 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm
+-rw-r--r--   0        0        0     1444 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd.dcm
+-rw-r--r--   0        0        0     1444 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd_big_endian.dcm
+-rw-r--r--   0        0        0     2044 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm
+-rw-r--r--   0        0        0    21686 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm
+-rw-r--r--   0        0        0      674 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/UN_sequence.dcm
+-rw-r--r--   0        0        0     7618 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/badVR.dcm
+-rw-r--r--   0        0        0     2300 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154
+-rw-r--r--   0        0        0     2298 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247
+-rw-r--r--   0        0        0     2298 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278
+-rw-r--r--   0        0        0     3810 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106
+-rw-r--r--   0        0        0     3812 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136
+-rw-r--r--   0        0        0     3812 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166
+-rw-r--r--   0        0        0     3812 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196
+-rw-r--r--   0        0        0     3920 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293
+-rw-r--r--   0        0        0     3908 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924
+-rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062
+-rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392
+-rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693
+-rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023
+-rw-r--r--   0        0        0     3938 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353
+-rw-r--r--   0        0        0     2336 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820
+-rw-r--r--   0        0        0     2336 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919
+-rw-r--r--   0        0        0     2330 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641
+-rw-r--r--   0        0        0     2336 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970
+-rw-r--r--   0        0        0     2356 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950
+-rw-r--r--   0        0        0     2354 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981
+-rw-r--r--   0        0        0     2354 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011
+-rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273
+-rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605
+-rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935
+-rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467
+-rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528
+-rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558
+-rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588
+-rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618
+-rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648
+-rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678
+-rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR
+-rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd
+-rw-r--r--   0        0        0      396 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-empty.dcm
+-rw-r--r--   0        0        0    11110 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit
+-rw-r--r--   0        0        0    11092 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset
+-rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient
+-rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered
+-rw-r--r--   0        0        0      719 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/README.txt
+-rw-r--r--   0        0        0    13066 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C
+-rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D
+-rw-r--r--   0        0        0     1206 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README
+-rw-r--r--   0        0        0      276 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/empty_charset_LEI.dcm
+-rw-r--r--   0        0        0     4637 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/image_dfl.dcm
+-rw-r--r--   0        0        0    37084 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/liver_1frame.dcm
+-rw-r--r--   0        0        0    36532 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/liver_expb_1frame.dcm
+-rw-r--r--   0        0        0      317 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/meta_missing_tsyntax.dcm
+-rw-r--r--   0        0        0      343 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/nested_priv_SQ.dcm
+-rw-r--r--   0        0        0    38871 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/no_meta.dcm
+-rw-r--r--   0        0        0      408 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/no_meta_group_length.dcm
+-rw-r--r--   0        0        0      546 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/priv_SQ.dcm
+-rw-r--r--   0        0        0     2968 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/reportsi.dcm
+-rw-r--r--   0        0        0     2700 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm
+-rw-r--r--   0        0        0     7568 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose.dcm
+-rwxr-xr-x   0        0        0     1958 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_1frame.dcm
+-rw-r--r--   0        0        0     7618 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_expb.dcm
+-rw-r--r--   0        0        0     2008 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_expb_1frame.dcm
+-rw-r--r--   0        0        0     6816 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_rle.dcm
+-rw-r--r--   0        0        0     2122 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_rle_1frame.dcm
+-rw-r--r--   0        0        0     2672 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtplan.dcm
+-rw-r--r--   0        0        0    14474 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtplan.dump
+-rw-r--r--   0        0        0     2129 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtplan_truncated.dcm
+-rw-r--r--   0        0        0     2534 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtstruct.dcm
+-rw-r--r--   0        0        0     7935 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtstruct.dump
+-rw-r--r--   0        0        0     6796 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/test-SR.dcm
+-rw-r--r--   0        0        0    20965 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/test1.json
+-rw-r--r--   0        0        0     1841 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/test_PN.json
+-rwxr-xr-x   0        0        0   291088 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/data/test_files/waveform_ecg.dcm
+-rw-r--r--   0        0        0     6958 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/data/test_files/zipMR.gz
+-rw-r--r--   0        0        0     9485 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/data/urls.json
+-rw-r--r--   0        0        0    18650 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/datadict.py
+-rw-r--r--   0        0        0    31098 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dataelem.py
+-rw-r--r--   0        0        0   109590 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dataset.py
+-rw-r--r--   0        0        0     5676 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dicomdir.py
+-rw-r--r--   0        0        0      403 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dicomio.py
+-rw-r--r--   0        0        0    26824 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encaps.py
+-rw-r--r--   0        0        0       66 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/__init__.py
+-rw-r--r--   0        0        0    36135 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/base.py
+-rw-r--r--   0        0        0     5901 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/gdcm.py
+-rw-r--r--   0        0        0     5374 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/native.py
+-rw-r--r--   0        0        0     1125 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/pylibjpeg.py
+-rw-r--r--   0        0        0     1714 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/env_info.py
+-rw-r--r--   0        0        0      771 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/errors.py
+-rw-r--r--   0        0        0     7794 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/filebase.py
+-rw-r--r--   0        0        0    44662 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/filereader.py
+-rw-r--r--   0        0        0   102357 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/fileset.py
+-rw-r--r--   0        0        0    14625 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/fileutil.py
+-rw-r--r--   0        0        0    44151 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/filewriter.py
+-rw-r--r--   0        0        0    12252 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/jsonrep.py
+-rw-r--r--   0        0        0     1644 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/misc.py
+-rw-r--r--   0        0        0     5140 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/multival.py
+-rw-r--r--   0        0        0      108 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/overlay_data_handlers/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/overlays/__init__.py
+-rw-r--r--   0        0        0     9951 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/overlays/numpy_handler.py
+-rw-r--r--   0        0        0      262 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/__init__.py
+-rw-r--r--   0        0        0     9761 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/gdcm_handler.py
+-rw-r--r--   0        0        0     3396 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/jpeg_ls_handler.py
+-rw-r--r--   0        0        0    12284 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/numpy_handler.py
+-rw-r--r--   0        0        0     8695 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/pillow_handler.py
+-rw-r--r--   0        0        0    11053 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/pylibjpeg_handler.py
+-rw-r--r--   0        0        0    16581 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/rle_handler.py
+-rw-r--r--   0        0        0    54722 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/util.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/py.typed
+-rw-r--r--   0        0        0     7573 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/sequence.py
+-rw-r--r--   0        0        0       38 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/sr/__init__.py
+-rw-r--r--   0        0        0   788696 2023-06-13 16:06:05.735394 pydicom-2.4.0/pydicom/sr/_cid_dict.py
+-rw-r--r--   0        0        0  2725654 2023-06-13 16:06:05.747394 pydicom-2.4.0/pydicom/sr/_concepts_dict.py
+-rw-r--r--   0        0        0   424515 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/sr/_snomed_dict.py
+-rw-r--r--   0        0        0    11035 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/sr/codedict.py
+-rw-r--r--   0        0        0     2026 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/sr/coding.py
+-rw-r--r--   0        0        0     8541 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/tag.py
+-rw-r--r--   0        0        0    34984 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/uid.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/__init__.py
+-rw-r--r--   0        0        0    17459 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/codify.py
+-rw-r--r--   0        0        0     3956 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/dump.py
+-rw-r--r--   0        0        0     4259 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/fixer.py
+-rw-r--r--   0        0        0     1576 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/hexutil.py
+-rw-r--r--   0        0        0     6465 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/leanread.py
+-rw-r--r--   0        0        0    73466 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/valuerep.py
+-rw-r--r--   0        0        0    26630 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/values.py
+-rw-r--r--   0        0        0       88 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/waveforms/__init__.py
+-rw-r--r--   0        0        0     8580 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/waveforms/numpy_handler.py
+-rw-r--r--   0        0        0     2829 2023-06-13 16:06:05.759395 pydicom-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-13 16:06:05.759395 pydicom-2.4.0/setup.cfg
+-rw-r--r--   0        0        0     2744 2023-06-13 16:06:05.759395 pydicom-2.4.0/setup.py
+-rwxr-xr-x   0        0        0    14008 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_cids/generate_concept_dicts.py
+-rwxr-xr-x   0        0        0    11894 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_dict/generate_dicom_dict.py
+-rwxr-xr-x   0        0        0     3769 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_dict/generate_private_dict.py
+-rwxr-xr-x   0        0        0     7710 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_dict/generate_uid_dict.py
+-rwxr-xr-x   0        0        0     2450 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_uids/generate_storage_sopclass_uids.py
+-rw-r--r--   0        0        0     1708 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/scripts/charlist.py
+-rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 pydicom-2.4.0/PKG-INFO
```

### Comparing `pydicom-2.3.1/CONTRIBUTING.md` & `pydicom-2.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/LICENSE` & `pydicom-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/PKG-INFO` & `pydicom-2.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,72 @@
 Metadata-Version: 2.1
 Name: pydicom
-Version: 2.3.1
+Version: 2.4.0
 Summary: A pure Python package for reading and writing DICOM data
-Home-page: https://github.com/pydicom/pydicom
-Download-URL: https://github.com/pydicom/pydicom/archive/master.zip
-Author: Darcy Mason and contributors
-Author-email: darcymason@gmail.com
-License: MIT
-Keywords: dicom python medical imaging
+Keywords: dicom, python, medical, imaging
+Author-email: Darcy Mason and contributors <darcymason@gmail.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6.1
-Description-Content-Type: text/markdown
+Requires-Dist: numpy ; extra == "docs"
+Requires-Dist: numpydoc ; extra == "docs"
+Requires-Dist: matplotlib ; extra == "docs"
+Requires-Dist: pillow ; extra == "docs"
+Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme ; extra == "docs"
+Requires-Dist: sphinx-gallery ; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon ; extra == "docs"
+Requires-Dist: sphinx-copybutton ; extra == "docs"
+Project-URL: documentation, https://pydicom.github.io/pydicom
+Project-URL: download, https://github.com/pydicom/pydicom/archive/master.zip
+Project-URL: homepage, https://github.com/pydicom/pydicom
+Project-URL: repository, https://github.com/pydicom/pydicom
 Provides-Extra: docs
-License-File: LICENSE
 
 [![unit-tests](https://github.com/pydicom/pydicom/workflows/unit-tests/badge.svg)](https://github.com/pydicom/pydicom/actions?query=workflow%3Aunit-tests)
 [![type-hints](https://github.com/pydicom/pydicom/workflows/type-hints/badge.svg)](https://github.com/pydicom/pydicom/actions?query=workflow%3Atype-hints)
 [![doc-build](https://circleci.com/gh/pydicom/pydicom/tree/master.svg?style=shield)](https://circleci.com/gh/pydicom/pydicom/tree/master)
 [![test-coverage](https://codecov.io/gh/pydicom/pydicom/branch/master/graph/badge.svg)](https://codecov.io/gh/pydicom/pydicom)
 [![Python version](https://img.shields.io/pypi/pyversions/pydicom.svg)](https://img.shields.io/pypi/pyversions/pydicom.svg)
 [![PyPI version](https://badge.fury.io/py/pydicom.svg)](https://badge.fury.io/py/pydicom)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6394735.svg)](https://doi.org/10.5281/zenodo.6394735)
-[![Gitter](https://badges.gitter.im/pydicom/Lobby.svg)](https://gitter.im/pydicom/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 # *pydicom*
 
-*pydicom* is a pure Python package for working with [DICOM](https://www.dicomstandard.org/) files. It lets you read, modify and write DICOM data in an easy "pythonic" way.
-
-As a pure Python package, *pydicom* can run anywhere Python runs without any other requirements, although if you're working with *Pixel Data* then we recommend you also install [NumPy](http://www.numpy.org).
+*pydicom* is a pure Python package for working with [DICOM](https://www.dicomstandard.org/) files.
+It lets you read, modify and write DICOM data in an easy "pythonic" way. As a pure Python package,
+*pydicom* can run anywhere Python runs without any other requirements, although if you're working 
+with *Pixel Data* then we recommend you also install [NumPy](http://www.numpy.org).
+
+Note that *pydicom* is a general-purpose DICOM framework concerned with 
+reading and writing DICOM datasets. In order to keep the 
+project manageable, it does not handle the specifics of individual SOP classes
+or other aspects of DICOM. Other libraries both inside and outside the
+[pydicom organization](https://github.com/pydicom) are based on *pydicom* 
+and provide support for other aspects of DICOM, and for more 
+specific applications.
+
+Examples are [pynetdicom](https://github.com/pydicom/pynetdicom), which 
+is a Python library for DICOM networking, and [deid](https://github.com/pydicom/deid),
+which supports the anonymization of DICOM files.
 
-If you're looking for a Python library for DICOM networking then you might be interested in another of our projects: [pynetdicom](https://github.com/pydicom/pynetdicom).
 
 ## Installation
 
 Using [pip](https://pip.pypa.io/en/stable/):
 ```
 pip install pydicom
 ```
@@ -137,11 +155,17 @@
 
 plt.imshow(arr, cmap="gray")
 plt.show()
 ```
 
 ## Contributing
 
-To contribute to *pydicom*, read our [contribution guide](https://github.com/pydicom/pydicom/blob/master/CONTRIBUTING.md).
-
-To contribute an example or extension of *pydicom* that doesn't belong with the core software, see our contribution repository:
+We are all volunteers working on *pydicom* in our free time. As our 
+resources are limited, we very much value your contributions, be it bug fixes, new 
+core features, or documentation improvements. For more information, please
+read our [contribution guide](https://github.com/pydicom/pydicom/blob/master/CONTRIBUTING.md).
+
+If you have examples or extensions of *pydicom* that don't belong with the 
+core software, but that you deem useful to others, you can add them to our 
+contribution repository:
 [contrib-pydicom](https://www.github.com/pydicom/contrib-pydicom).
+
```

### Comparing `pydicom-2.3.1/README.md` & `pydicom-2.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 [![unit-tests](https://github.com/pydicom/pydicom/workflows/unit-tests/badge.svg)](https://github.com/pydicom/pydicom/actions?query=workflow%3Aunit-tests)
 [![type-hints](https://github.com/pydicom/pydicom/workflows/type-hints/badge.svg)](https://github.com/pydicom/pydicom/actions?query=workflow%3Atype-hints)
 [![doc-build](https://circleci.com/gh/pydicom/pydicom/tree/master.svg?style=shield)](https://circleci.com/gh/pydicom/pydicom/tree/master)
 [![test-coverage](https://codecov.io/gh/pydicom/pydicom/branch/master/graph/badge.svg)](https://codecov.io/gh/pydicom/pydicom)
 [![Python version](https://img.shields.io/pypi/pyversions/pydicom.svg)](https://img.shields.io/pypi/pyversions/pydicom.svg)
 [![PyPI version](https://badge.fury.io/py/pydicom.svg)](https://badge.fury.io/py/pydicom)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6394735.svg)](https://doi.org/10.5281/zenodo.6394735)
-[![Gitter](https://badges.gitter.im/pydicom/Lobby.svg)](https://gitter.im/pydicom/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 # *pydicom*
 
-*pydicom* is a pure Python package for working with [DICOM](https://www.dicomstandard.org/) files. It lets you read, modify and write DICOM data in an easy "pythonic" way.
+*pydicom* is a pure Python package for working with [DICOM](https://www.dicomstandard.org/) files.
+It lets you read, modify and write DICOM data in an easy "pythonic" way. As a pure Python package,
+*pydicom* can run anywhere Python runs without any other requirements, although if you're working 
+with *Pixel Data* then we recommend you also install [NumPy](http://www.numpy.org).
+
+Note that *pydicom* is a general-purpose DICOM framework concerned with 
+reading and writing DICOM datasets. In order to keep the 
+project manageable, it does not handle the specifics of individual SOP classes
+or other aspects of DICOM. Other libraries both inside and outside the
+[pydicom organization](https://github.com/pydicom) are based on *pydicom* 
+and provide support for other aspects of DICOM, and for more 
+specific applications.
+
+Examples are [pynetdicom](https://github.com/pydicom/pynetdicom), which 
+is a Python library for DICOM networking, and [deid](https://github.com/pydicom/deid),
+which supports the anonymization of DICOM files.
 
-As a pure Python package, *pydicom* can run anywhere Python runs without any other requirements, although if you're working with *Pixel Data* then we recommend you also install [NumPy](http://www.numpy.org).
-
-If you're looking for a Python library for DICOM networking then you might be interested in another of our projects: [pynetdicom](https://github.com/pydicom/pynetdicom).
 
 ## Installation
 
 Using [pip](https://pip.pypa.io/en/stable/):
 ```
 pip install pydicom
 ```
@@ -106,11 +117,16 @@
 
 plt.imshow(arr, cmap="gray")
 plt.show()
 ```
 
 ## Contributing
 
-To contribute to *pydicom*, read our [contribution guide](https://github.com/pydicom/pydicom/blob/master/CONTRIBUTING.md).
-
-To contribute an example or extension of *pydicom* that doesn't belong with the core software, see our contribution repository:
+We are all volunteers working on *pydicom* in our free time. As our 
+resources are limited, we very much value your contributions, be it bug fixes, new 
+core features, or documentation improvements. For more information, please
+read our [contribution guide](https://github.com/pydicom/pydicom/blob/master/CONTRIBUTING.md).
+
+If you have examples or extensions of *pydicom* that don't belong with the 
+core software, but that you deem useful to others, you can add them to our 
+contribution repository:
 [contrib-pydicom](https://www.github.com/pydicom/contrib-pydicom).
```

### Comparing `pydicom-2.3.1/doc/Makefile` & `pydicom-2.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/README.md` & `pydicom-2.4.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/_static/css/pydicom.css` & `pydicom-2.4.0/doc/_static/css/pydicom.css`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/assets/img/favicon.ico` & `pydicom-2.4.0/doc/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/assets/img/logo.png` & `pydicom-2.4.0/doc/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/assets/img/pydicom_blue_light.png` & `pydicom-2.4.0/doc/assets/img/pydicom_blue_light.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/assets/img/pydicom_blue_light.svg` & `pydicom-2.4.0/doc/assets/img/pydicom_blue_light.svg`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/assets/img/pydicom_flat_black.png` & `pydicom-2.4.0/doc/assets/img/pydicom_flat_black.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/assets/img/pydicom_flat_black.svg` & `pydicom-2.4.0/doc/assets/img/pydicom_flat_black.svg`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/assets/img/pydicom_flat_black_alpha.png` & `pydicom-2.4.0/doc/assets/img/pydicom_flat_black_alpha.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/conf.py` & `pydicom-2.4.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         'http://dicom.nema.org/medical/dicom/current/output/chtml/%s',
         None
     ),
     'gh': (
         'https://github.com/pydicom/%s',
         None
     ),
-    "issue": ("https://github.com/pydicom/pydicom/issues/%s", "#"),
-    "pr": ("https://github.com/pydicom/pydicom/pull/%s", "#"),
+    "issue": ("https://github.com/pydicom/pydicom/issues/%s", "#%s"),
+    "pr": ("https://github.com/pydicom/pydicom/pull/%s", "#%s"),
 }
 
 # intersphinx configuration
 intersphinx_mapping = {
     'python': ('https://docs.python.org/{.major}'.format(
         sys.version_info), None),
     'numpy': ('https://docs.scipy.org/doc/numpy/', None),
```

### Comparing `pydicom-2.3.1/doc/faq/index.rst` & `pydicom-2.4.0/doc/faq/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -51,35 +51,37 @@
 libraries are required.
 
 .. _faq_install_version:
 
 What version of Python can I use?
 ---------------------------------
 
-+-----------------+------------------+--------------------------+
-| pydicom version |  Release date    | Python versions          |
-+=================+==================+==========================+
-| 1.0             | March 2018       | 2.7, 3.4, 3.5, 3.6       |
-+-----------------+------------------+--------------------------+
-| 1.1             | June 2018        | 2.7, 3.4, 3.5, 3.6       |
-+-----------------+------------------+--------------------------+
-| 1.2             | October 2018     | 2.7, 3.4, 3.5, 3.6       |
-+-----------------+------------------+--------------------------+
-| 1.3             | July 2019        | 2.7, 3.4, 3.5, 3.6       |
-+-----------------+------------------+--------------------------+
-| 1.4             | January 2020     | 2.7, 3.5, 3.6, 3.7, 3.8  |
-+-----------------+------------------+--------------------------+
-| 2.0             | May 2020         | 3.5, 3.6, 3.7, 3.8       |
-+-----------------+------------------+--------------------------+
-| 2.1             | November 2020    | 3.6, 3.7, 3.8, 3.9       |
-+-----------------+------------------+--------------------------+
-| 2.2             | August 2021      | 3.6, 3.7, 3.8, 3.9       |
-+-----------------+------------------+--------------------------+
-| 2.3             | ~February 2022   | 3.6, 3.7, 3.8, 3.9, 3.10 |
-+-----------------+------------------+--------------------------+
++-----------------+------------------+---------------------------+
+| pydicom version |  Release date    | Python versions           |
++=================+==================+===========================+
+| 1.0             | March 2018       | 2.7, 3.4, 3.5, 3.6        |
++-----------------+------------------+---------------------------+
+| 1.1             | June 2018        | 2.7, 3.4, 3.5, 3.6        |
++-----------------+------------------+---------------------------+
+| 1.2             | October 2018     | 2.7, 3.4, 3.5, 3.6        |
++-----------------+------------------+---------------------------+
+| 1.3             | July 2019        | 2.7, 3.4, 3.5, 3.6        |
++-----------------+------------------+---------------------------+
+| 1.4             | January 2020     | 2.7, 3.5, 3.6, 3.7, 3.8   |
++-----------------+------------------+---------------------------+
+| 2.0             | May 2020         | 3.5, 3.6, 3.7, 3.8        |
++-----------------+------------------+---------------------------+
+| 2.1             | November 2020    | 3.6, 3.7, 3.8, 3.9        |
++-----------------+------------------+---------------------------+
+| 2.2             | August 2021      | 3.6, 3.7, 3.8, 3.9        |
++-----------------+------------------+---------------------------+
+| 2.3             | March 2022       | 3.6, 3.7, 3.8, 3.9, 3.10  |
++-----------------+------------------+---------------------------+
+| 2.4             | ~September 2022  | 3.7, 3.8, 3.9, 3.10, 3.11 |
++-----------------+------------------+---------------------------+
 
 What about support for Python 2.7?
 ----------------------------------
 
 Python 2.7 reached `end of life <https://www.python.org/doc/sunset-python-2/>`_
 on 1st January, 2020 and is no longer supported by *pydicom*. More information
 is available :doc:`here</old/python2_support>`.
```

### Comparing `pydicom-2.3.1/doc/guides/cli/cli_codify.rst` & `pydicom-2.4.0/doc/guides/cli/cli_codify.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/cli/cli_dev.rst` & `pydicom-2.4.0/doc/guides/cli/cli_dev.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/cli/cli_intro.rst` & `pydicom-2.4.0/doc/guides/cli/cli_intro.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/cli/cli_show.rst` & `pydicom-2.4.0/doc/guides/cli/cli_show.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/element_value_types.rst` & `pydicom-2.4.0/doc/guides/element_value_types.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/encoding/encoder_plugin_options.rst` & `pydicom-2.4.0/doc/guides/encoding/encoder_plugin_options.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/encoding/encoder_plugins.rst` & `pydicom-2.4.0/doc/guides/encoding/encoder_plugins.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/encoding/rle_lossless.rst` & `pydicom-2.4.0/doc/guides/encoding/rle_lossless.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/glossary.rst` & `pydicom-2.4.0/doc/guides/glossary.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/guides/writing_documentation.rst` & `pydicom-2.4.0/doc/guides/writing_documentation.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/index.rst` & `pydicom-2.4.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/make.bat` & `pydicom-2.4.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/base_element.rst` & `pydicom-2.4.0/doc/old/base_element.rst`

 * *Files 0% similar despite different names*

```diff
@@ -174,21 +174,21 @@
   >>> elem.VR, elem.value
   ('PN', 'Last^First^mid^pre')
   >>> # an alternative is to use:
   >>> elem = ds[0x0010,0x0010]
   >>> elem.VR, elem.value
   ('PN', 'Last^First^mid^pre')
 
-To see whether the :class:`~dataset.Dataset` contains a particular element use
+To see whether the :class:`~dataset.Dataset` contains a particular element, use
 the ``in`` operator with the element's keyword or tag::
 
   >>> "PatientName" in ds  # or (0x0010,0x0010) in ds
   True
 
-To remove an element from the :class:`~dataset.Dataset`  use the ``del``
+To remove an element from the :class:`~dataset.Dataset`, use the ``del``
 operator::
 
   >>> del ds.SoftwareVersions  # or del ds[0x0018, 0x1020]
 
 To work with (7FE0,0010) *Pixel Data*, the raw :class:`bytes` are available
 through the `PixelData` keyword::
 
@@ -218,18 +218,18 @@
 
 The :class:`~dataelem.DataElement` class is not usually used directly in user
 code, but is used extensively by :class:`~dataset.Dataset`.
 :class:`~dataelem.DataElement` is a simple object which stores the following
 things:
 
   * :attr:`~dataelem.DataElement.tag` -- the element's tag (as a
-    :class:`~pydicom.tag.BaseTag` object)
+    :class:`~pydicom.tag.BaseTag` object).
   * :attr:`~dataelem.DataElement.VR` -- the element's Value Representation
     -- a two letter :class:`str` that describes to the format of the stored
-    value
+    value.
   * :attr:`~dataelem.DataElement.VM` -- the element's Value Multiplicity as
     an :class:`int`. This is automatically determined from the contents of
     the :attr:`~dataelem.DataElement.value`.
   * :attr:`~dataelem.DataElement.value` -- the element's actual value.
     A regular value like a number or string (or :class:`list` of them if the
     VM > 1), or a :class:`~sequence.Sequence`.
 
@@ -240,15 +240,15 @@
 :func:`BaseTags<tag.BaseTag>` are automatically created when you assign or read
 elements using their keywords as illustrated in sections above.
 
 The :class:`~tag.BaseTag` class is derived from :class:`int`,
 so in effect, it is just a number with some extra behavior:
 
   * :func:`~tag.Tag` is used to create instances of :class:`~tag.BaseTag` and
-    enforces that the DICOM tag fits in the expected 4-byte (group,element)
+    enforces the expected 4-byte (group,element) structure.
   * A :class:`~tag.BaseTag` instance can be created from an :class:`int` or a
     :class:`tuple` containing the (group,element), or from the DICOM keyword::
 
       >>> from pydicom.tag import Tag
       >>> t1 = Tag(0x00100010) # all of these are equivalent
       >>> t2 = Tag(0x10,0x10)
       >>> t3 = Tag((0x10, 0x10))
```

### Comparing `pydicom-2.3.1/doc/old/best_practices.rst` & `pydicom-2.4.0/doc/old/best_practices.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/getting_started.rst` & `pydicom-2.4.0/doc/old/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/image_data_compression.rst` & `pydicom-2.4.0/doc/old/image_data_compression.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/image_data_handlers.rst` & `pydicom-2.4.0/doc/old/image_data_handlers.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 The following packages can be used with *pydicom*:
 
 * `GDCM <http://gdcm.sourceforge.net/>`_ - this is the package that supports
   most compressed formats
 * `Pillow <http://pillow.readthedocs.io/en/latest/>`_, ideally with
   ``jpeg`` and ``jpeg2000`` plugins
-* `jpeg_ls <https://github.com/Who8MyLunch/CharPyLS>`_
+* `jpeg_ls <https://github.com/pydicom/pyjpegls>`_
 * :gh:`pylibjpeg <pylibjpeg>`, with the ``-libjpeg``, ``-openjpeg`` and
   ``-rle`` plugins
 
 Note that you always need the `NumPy <http://numpy.org/>`_ package to be able
 to handle pixel data.
 
 .. caution:: We rely on the data handling capacity of the mentioned
```

### Comparing `pydicom-2.3.1/doc/old/private_data_elements.rst` & `pydicom-2.4.0/doc/old/private_data_elements.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/python2_support.rst` & `pydicom-2.4.0/doc/old/python2_support.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/ref_guide.rst` & `pydicom-2.4.0/doc/old/ref_guide.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/transition_to_pydicom1.rst` & `pydicom-2.4.0/doc/old/transition_to_pydicom1.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/viewing_images.rst` & `pydicom-2.4.0/doc/old/viewing_images.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/working_with_overlays.rst` & `pydicom-2.4.0/doc/old/working_with_overlays.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/working_with_pixel_data.rst` & `pydicom-2.4.0/doc/old/working_with_pixel_data.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/working_with_waveforms.rst` & `pydicom-2.4.0/doc/old/working_with_waveforms.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/old/writing_files.rst` & `pydicom-2.4.0/doc/old/writing_files.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/config.rst` & `pydicom-2.4.0/doc/reference/config.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/datadict.rst` & `pydicom-2.4.0/doc/reference/datadict.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/elem.values.rst` & `pydicom-2.4.0/doc/reference/elem.values.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/encaps.rst` & `pydicom-2.4.0/doc/reference/encaps.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/encoders.rst` & `pydicom-2.4.0/doc/reference/encoders.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/fileio.write.rst` & `pydicom-2.4.0/doc/reference/fileio.write.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/handlers.rst` & `pydicom-2.4.0/doc/reference/handlers.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/reference/uid.rst` & `pydicom-2.4.0/doc/reference/uid.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.2.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.2.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.3.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.3.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.4.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.4.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.5.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.5.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.6.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.6.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.7.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.7.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.8.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.8.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v0.9.9.rst` & `pydicom-2.4.0/doc/release_notes/v0.9.9.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v1.0.0.rst` & `pydicom-2.4.0/doc/release_notes/v1.0.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v1.1.0.rst` & `pydicom-2.4.0/doc/release_notes/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v1.2.0.rst` & `pydicom-2.4.0/doc/release_notes/v1.2.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v1.3.0.rst` & `pydicom-2.4.0/doc/release_notes/v1.3.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v1.4.0.rst` & `pydicom-2.4.0/doc/release_notes/v1.4.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v2.0.0.rst` & `pydicom-2.4.0/doc/release_notes/v2.0.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v2.1.0.rst` & `pydicom-2.4.0/doc/release_notes/v2.1.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v2.2.0.rst` & `pydicom-2.4.0/doc/release_notes/v2.2.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/release_notes/v2.3.0.rst` & `pydicom-2.4.0/doc/release_notes/v2.3.0.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Version 2.3.1
-=================================
-
-Changes
--------
-* updated for Python 3.11 compatibility
-
-
 Version 2.3.0
 =================================
 
 Changes
 -------
 * :meth:`DataElement.description<pydicom.dataelem.DataElement.description>` is
   deprecated and will be removed in v3.0, use
```

### Comparing `pydicom-2.3.1/doc/tutorials/contributing.rst` & `pydicom-2.4.0/doc/tutorials/contributing.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/contributing_code.rst` & `pydicom-2.4.0/doc/tutorials/contributing_code.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/contributing_docs.rst` & `pydicom-2.4.0/doc/tutorials/contributing_docs.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/dataset_basics.rst` & `pydicom-2.4.0/doc/tutorials/dataset_basics.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/dicom_json.rst` & `pydicom-2.4.0/doc/tutorials/dicom_json.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/filesets.rst` & `pydicom-2.4.0/doc/tutorials/filesets.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ============================
 DICOM File-sets and DICOMDIR
 ============================
 
-This tutorial is about DICOM File-sets and covers
+This tutorial is about DICOM File-sets and covers:
 
 * An introduction to DICOM File-sets and the DICOMDIR file
 * Loading a File-set using the :class:`~pydicom.fileset.FileSet` class and
   accessing its managed SOP instances
 * Creating a new File-set and modifying existing ones
 
 It's assumed that you're already familiar with the :doc:`dataset basics
@@ -34,15 +34,15 @@
 The DICOMDIR file
 -----------------
 
 .. note::
 
     Despite its name, a DICOMDIR file is not a file system directory and
     can be read using :func:`~pydicom.filereader.dcmread` like any other DICOM
-    dataset
+    dataset.
 
 Every File-set must contain a single file with the filename ``DICOMDIR``, the
 location of which is dependent on the type of media used to store the File-set.
 For the most commonly used media (DVD, CD, USB, PC file system, etc), the
 DICOMDIR file will be in the root directory of the File-set. For other
 media types, :dcm:`Part 12 of the DICOM Standard<part12/ps3.12.html>`
 specifies where the DICOMDIR must be located.
@@ -50,15 +50,15 @@
 .. warning::
 
     It's **strongly recommended** that you avoid making changes to a DICOMDIR
     dataset directly unless you know what you're doing. Even minor changes may
     require recalculating the offsets for each directory record. Use the
     :class:`~pydicom.fileset.FileSet` methods (see below) instead.
 
-The DICOMDIR file is used to summarize the contents of the File-set, and is a
+The DICOMDIR file is used to summarize the contents of the File-set and is a
 *Media Storage Directory* instance that follows the
 :dcm:`Basic Directory IOD<part03/chapter_F.html>`.
 
 .. code-block:: python
 
     >>> from pydicom import dcmread
     >>> from pydicom.data import get_testdata_file
@@ -264,18 +264,18 @@
   <pydicom.fileset.FileSet.add>` or :meth:`FileSet.add_custom()
   <pydicom.fileset.FileSet.add_custom>` methods
 * Removing SOP instances with :meth:`FileSet.remove()
   <pydicom.fileset.FileSet.remove>`
 * Changing one of the following properties:
   :attr:`~pydicom.fileset.FileSet.ID`, :attr:`~pydicom.fileset.FileSet.UID`,
   :attr:`~pydicom.fileset.FileSet.descriptor_file_id` and
-  :attr:`~pydicom.fileset.FileSet.descriptor_character_set`.
+  :attr:`~pydicom.fileset.FileSet.descriptor_character_set`
 * When the :class:`~pydicom.fileset.FileSet` class determines it needs to move
   SOP instances from an existing File-set's directory structure to the
-  structure used by *pydicom*.
+  structure used by *pydicom*
 
 You can tell if changes are staged with the
 :attr:`~pydicom.fileset.FileSet.is_staged` property:
 
 .. code-block:: python
 
     >>> fs.is_staged
@@ -305,15 +305,15 @@
 The simplest way to add new SOP instances to the File-set is with the
 :meth:`~pydicom.fileset.FileSet.add` method, which takes the path to the
 instance or the instance itself as a :class:`~pydicom.dataset.Dataset` and
 returns the addition as a :class:`~pydicom.fileset.FileInstance`.
 
 To reduce memory usage, instances staged for addition are written to a
 temporary directory and only copied to the File-set itself when
-:meth:`~pydicom.fileset.FileSet.write` is called, however they can still be
+:meth:`~pydicom.fileset.FileSet.write` is called. However, they can still be
 accessed and loaded:
 
 .. code-block:: python
 
     >>> path = get_testdata_file("CT_small.dcm")
     >>> instance = fs.add(path)
     >>> instance.is_staged
@@ -328,15 +328,15 @@
 Alternatively, if you want more control over the directory records that will
 be added to the DICOMDIR file, or if you need to use PRIVATE records, you can
 use the :meth:`~pydicom.fileset.FileSet.add_custom` method.
 
 The :meth:`~pydicom.fileset.FileSet.add` method uses *pydicom's* default
 directory record creation functions to create the necessary records based on
 the SOP instance's attributes, such as *SOP Class UID* and *Modality*.
-Occasionally they may fail when an element required by these functions
+Occasionally, they may fail when an element required by these functions
 is empty or missing:
 
 .. code-block:: python
 
     >>> path = get_testdata_file("rtdose.dcm")
     >>> fs.add(path)
     Traceback (most recent call last):
@@ -354,23 +354,23 @@
       File "<stdin>", line 1, in <module>
       File ".../pydicom/fileset.py", line 1039, in add
         record = next(record_gen)
       File ".../pydicom/fileset.py", line 1860, in _recordify
         raise ValueError(
     ValueError: Unable to use the default 'RT DOSE' record creator as the instance is missing a required element or value. Either update the instance, define your own record creation function or use 'FileSet.add_custom()' instead
 
-When this occurs you have three choices:
+When this occurs, there are three options:
 
 * Update the instance to include the required element and/or value
 * Override the default record creation functions with your own by modifying
   :attr:`~pydicom.fileset.DIRECTORY_RECORDERS`
 * Use the :meth:`~pydicom.fileset.FileSet.add_custom` method
 
-From the exception message above we've got an empty *Instance Number*, so
-let's update the instance and try adding it again:
+According to the exception message above, the *Instance Number* element is empty.
+Let's update the instance and try adding it again:
 
 .. code-block:: python
 
     >>> ds = dcmread(path)
     >>> ds.InstanceNumber = "1"
     >>> fs.add(ds)
 
@@ -401,15 +401,15 @@
 
 .. code-block:: python
 
     >>> fs.add(get_testdata_file("CT_small.dcm"))
     >>> fs.add(get_testdata_file("MR_small.dcm"))
 
 To apply the changes we've made to the File-set we use
-:meth:`~pydicom.fileset.FileSet.write`. For new File-sets we have to supply the
+:meth:`~pydicom.fileset.FileSet.write`. For new File-sets, we have to supply the
 path where the File-set root directory will be located:
 
 .. code-block:: python
 
     >>> from pathlib import Path
     >>> from tempfile import TemporaryDirectory
     >>> t = TemporaryDirectory()
@@ -446,20 +446,20 @@
 
 For existing File-sets that don't use the same directory structure semantics
 as :class:`~pydicom.fileset.FileSet`, calling
 :meth:`~pydicom.fileset.FileSet.write` will move SOP instances over to the
 new structure. However, if the only modification you've made is to remove SOP
 instances or change :attr:`~pydicom.fileset.FileSet.ID`,
 :attr:`~pydicom.fileset.FileSet.UID`,
-:attr:`~pydicom.fileset.FileSet.descriptor_file_id` or
+:attr:`~pydicom.fileset.FileSet.descriptor_file_id`, or
 :attr:`~pydicom.fileset.FileSet.descriptor_character_set`, then you can pass
 the *use_existing* keyword parameter to keep the existing directory structure
 and update the DICOMDIR file.
 
-First we need to copy the existing example File-set to a temporary directory
+First, we need to copy the existing example File-set to a temporary directory
 so we don't accidentally modify it:
 
 .. code-block:: python
 
     >>> from shutil import copytree, copyfile
     >>> t = TemporaryDirectory()
     >>> dst = Path(t.name)
@@ -488,15 +488,15 @@
     /tmp/tmpu068kdwp/77654033/CR3/6278
     /tmp/tmpu068kdwp/77654033/CT2/17106
     /tmp/tmpu068kdwp/77654033/CT2/17136
     /tmp/tmpu068kdwp/77654033/CT2/17166
     /tmp/tmpu068kdwp/77654033/CT2/17196
 
 If you'd just called :meth:`~pydicom.fileset.FileSet.write` without
-*use_existing* then it would've moved the SOP instances to the new
+*use_existing*, then it would've moved the SOP instances to the new
 directory structure:
 
 .. code-block:: python
 
     >>> fs.write()
     >>> for path in sorted([p for p in dst.glob('**/*') if p.is_file()]):
     ...     print(path)
```

### Comparing `pydicom-2.3.1/doc/tutorials/installation.rst` & `pydicom-2.4.0/doc/tutorials/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -105,30 +105,30 @@
 
 Through conda::
 
   conda install -c conda-forge openjpeg jpeg
   conda install pillow
 
 
-Installing CharPyLS
+Installing pyjpegls
 -------------------
 
-`CharPyLS <https://github.com/Who8MyLunch/CharPyLS>`_ is a Python interface to
+`pyjpegls <https://github.com/pydicom/pyjpegls>`_ is a Python interface to
 the `CharLS <https://github.com/team-charls/charls>`_ C++ library and can
-decompress JPEG-LS images.
+decompress JPEG-LS images. It is a fork of `CharPyLS <https://github.com/Who8MyLunch/CharPyLS>`_
+created to provide compatibility with the latest Python versions.
 
 Using pip::
 
-  pip install cython
-  pip install git+https://github.com/Who8MyLunch/CharPyLS
+  pip install pyjpegls
 
 Through conda::
 
   conda install cython
-  pip install git+https://github.com/Who8MyLunch/CharPyLS
+  pip install git+https://github.com/pydicom/pyjpegls
 
 
 .. _tut_install_gdcm:
 
 Installing GDCM
 ---------------
```

### Comparing `pydicom-2.3.1/doc/tutorials/pixel_data/compressing.rst` & `pydicom-2.4.0/doc/tutorials/pixel_data/compressing.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/sr_basics.rst` & `pydicom-2.4.0/doc/tutorials/sr_basics.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/virtualenvs.rst` & `pydicom-2.4.0/doc/tutorials/virtualenvs.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/waveforms.rst` & `pydicom-2.4.0/doc/tutorials/waveforms.rst`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
     >>> raw = multiplex_array(ds, 0, as_raw=True)
     >>> raw[0, 0]
     80
 
 
 If (003A,0210) *Channel Sensitivity* is present within the multiplex's *Channel
 Definition Sequence* then the raw sample data needs to be corrected before it's
-in the quantity it represents. This correction is given by (sample + *Channel
-Baseline*) x *Channel Sensitivity* x *Channel Sensitivity Correction Factor*
+in the quantity it represents. This correction is given by sample x *Channel 
+Sensitivity* x *Channel Sensitivity Correction Factor* + *Channel Baseline*
 and will be applied when `as_raw` is ``False`` or when using the
 :meth:`Dataset.waveform_array()<pydicom.dataset.Dataset.waveform_array>`
 function:
 
     >>> arr = ds.waveform_array(0)
     >>> arr[0, 0]
     >>> 100.0
```

### Comparing `pydicom-2.3.1/doc/tutorials/waveforms_assets/waveforms_decode.png` & `pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_decode.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/doc/tutorials/waveforms_assets/waveforms_encode.png` & `pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_encode.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/dicomtree.py` & `pydicom-2.4.0/examples/dicomtree.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                   tree.hlist.yview_scroll(int(+1), "units"))
 
     show_file(filename, tree)
 
 
 def show_file(filename, tree):
     tree.hlist.add("root", text=filename)
-    ds = pydicom.dcmread(sys.argv[1])
+    ds = pydicom.dcmread(filename)
     ds.decode()  # change strings to unicode
     recurse_tree(tree, ds, "root", False)
     tree.autosetmode()
 
 
 def recurse_tree(tree, dataset, parent, hide=False):
     # order the dicom tags
```

### Comparing `pydicom-2.3.1/examples/image_processing/plot_downsize_image.py` & `pydicom-2.4.0/examples/image_processing/plot_downsize_image.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/image_processing/plot_waveforms.py` & `pydicom-2.4.0/examples/image_processing/plot_waveforms.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/image_processing/reslice.py` & `pydicom-2.4.0/examples/image_processing/reslice.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/input_output/plot_printing_dataset.py` & `pydicom-2.4.0/examples/input_output/plot_printing_dataset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/input_output/plot_read_dicom.py` & `pydicom-2.4.0/examples/input_output/plot_read_dicom.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 # Normal mode:
 print()
 print(f"File path........: {fpath}")
 print(f"SOP Class........: {ds.SOPClassUID} ({ds.SOPClassUID.name})")
 print()
 
 pat_name = ds.PatientName
-display_name = pat_name.family_name + ", " + pat_name.given_name
-print(f"Patient's Name...: {display_name}")
+print(f"Patient's Name...: {pat_name.family_comma_given()}")
 print(f"Patient ID.......: {ds.PatientID}")
 print(f"Modality.........: {ds.Modality}")
 print(f"Study Date.......: {ds.StudyDate}")
 print(f"Image size.......: {ds.Rows} x {ds.Columns}")
 print(f"Pixel Spacing....: {ds.PixelSpacing}")
 
 # use .get() if not sure the item exists, and want a default value if missing
```

### Comparing `pydicom-2.3.1/examples/input_output/plot_read_dicom_directory.py` & `pydicom-2.4.0/examples/input_output/plot_read_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/input_output/plot_read_fileset.py` & `pydicom-2.4.0/examples/input_output/plot_read_fileset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/input_output/plot_read_rtplan.py` & `pydicom-2.4.0/examples/input_output/plot_read_rtplan.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/input_output/plot_write_dicom.py` & `pydicom-2.4.0/examples/input_output/plot_write_dicom.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/memory_dataset.py` & `pydicom-2.4.0/examples/memory_dataset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/metadata_processing/plot_add_dict_entries.py` & `pydicom-2.4.0/examples/metadata_processing/plot_add_dict_entries.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/metadata_processing/plot_anonymize.py` & `pydicom-2.4.0/examples/metadata_processing/plot_anonymize.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/metadata_processing/plot_sequences.py` & `pydicom-2.4.0/examples/metadata_processing/plot_sequences.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/plot_dicom_difference.py` & `pydicom-2.4.0/examples/plot_dicom_difference.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/examples/show_charset_name.py` & `pydicom-2.4.0/examples/show_charset_name.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/__init__.py` & `pydicom-2.4.0/pydicom/__init__.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/_dicom_dict.py` & `pydicom-2.4.0/pydicom/_dicom_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,17 @@
     0x00080008: ('CS', '2-n', "Image Type", '', 'ImageType'),  # noqa
     0x00080010: ('SH', '1', "Recognition Code", 'Retired', 'RecognitionCode'),  # noqa
     0x00080012: ('DA', '1', "Instance Creation Date", '', 'InstanceCreationDate'),  # noqa
     0x00080013: ('TM', '1', "Instance Creation Time", '', 'InstanceCreationTime'),  # noqa
     0x00080014: ('UI', '1', "Instance Creator UID", '', 'InstanceCreatorUID'),  # noqa
     0x00080015: ('DT', '1', "Instance Coercion DateTime", '', 'InstanceCoercionDateTime'),  # noqa
     0x00080016: ('UI', '1', "SOP Class UID", '', 'SOPClassUID'),  # noqa
+    0x00080017: ('UI', '1', "Acquisition UID", '', 'AcquisitionUID'),  # noqa
     0x00080018: ('UI', '1', "SOP Instance UID", '', 'SOPInstanceUID'),  # noqa
+    0x00080019: ('UI', '1', "Pyramid UID", '', 'PyramidUID'),  # noqa
     0x0008001A: ('UI', '1-n', "Related General SOP Class UID", '', 'RelatedGeneralSOPClassUID'),  # noqa
     0x0008001B: ('UI', '1', "Original Specialized SOP Class UID", '', 'OriginalSpecializedSOPClassUID'),  # noqa
     0x00080020: ('DA', '1', "Study Date", '', 'StudyDate'),  # noqa
     0x00080021: ('DA', '1', "Series Date", '', 'SeriesDate'),  # noqa
     0x00080022: ('DA', '1', "Acquisition Date", '', 'AcquisitionDate'),  # noqa
     0x00080023: ('DA', '1', "Content Date", '', 'ContentDate'),  # noqa
     0x00080024: ('DA', '1', "Overlay Date", 'Retired', 'OverlayDate'),  # noqa
@@ -190,14 +192,56 @@
     0x0008030A: ('CS', '1', "Private Data Element Value Representation", '', 'PrivateDataElementValueRepresentation'),  # noqa
     0x0008030B: ('UL', '1-2', "Private Data Element Number of Items", '', 'PrivateDataElementNumberOfItems'),  # noqa
     0x0008030C: ('UC', '1', "Private Data Element Name", '', 'PrivateDataElementName'),  # noqa
     0x0008030D: ('UC', '1', "Private Data Element Keyword", '', 'PrivateDataElementKeyword'),  # noqa
     0x0008030E: ('UT', '1', "Private Data Element Description", '', 'PrivateDataElementDescription'),  # noqa
     0x0008030F: ('UT', '1', "Private Data Element Encoding", '', 'PrivateDataElementEncoding'),  # noqa
     0x00080310: ('SQ', '1', "Private Data Element Definition Sequence", '', 'PrivateDataElementDefinitionSequence'),  # noqa
+    0x00080400: ('SQ', '1', "Scope of Inventory Sequence", '', 'ScopeOfInventorySequence'),  # noqa
+    0x00080401: ('LT', '1', "Inventory Purpose", '', 'InventoryPurpose'),  # noqa
+    0x00080402: ('LT', '1', "Inventory Instance Description", '', 'InventoryInstanceDescription'),  # noqa
+    0x00080403: ('CS', '1', "Inventory Level", '', 'InventoryLevel'),  # noqa
+    0x00080404: ('DT', '1', "Item Inventory DateTime", '', 'ItemInventoryDateTime'),  # noqa
+    0x00080405: ('CS', '1', "Removed from Operational Use", '', 'RemovedFromOperationalUse'),  # noqa
+    0x00080406: ('SQ', '1', "Reason for Removal Code Sequence", '', 'ReasonForRemovalCodeSequence'),  # noqa
+    0x00080407: ('UR', '1', "Stored Instance Base URI", '', 'StoredInstanceBaseURI'),  # noqa
+    0x00080408: ('UR', '1', "Folder Access URI", '', 'FolderAccessURI'),  # noqa
+    0x00080409: ('UR', '1', "File Access URI", '', 'FileAccessURI'),  # noqa
+    0x0008040A: ('CS', '1', "Container File Type", '', 'ContainerFileType'),  # noqa
+    0x0008040B: ('UR', '1', "Filename in Container", '', 'FilenameInContainer'),  # noqa
+    0x0008040C: ('UV', '1', "File Offset in Container", '', 'FileOffsetInContainer'),  # noqa
+    0x0008040D: ('UV', '1', "File Length in Container", '', 'FileLengthInContainer'),  # noqa
+    0x0008040E: ('UI', '1', "Stored Instance Transfer Syntax UID", '', 'StoredInstanceTransferSyntaxUID'),  # noqa
+    0x0008040F: ('CS', '1-n', "Extended Matching Mechanisms", '', 'ExtendedMatchingMechanisms'),  # noqa
+    0x00080410: ('SQ', '1', "Range Matching Sequence", '', 'RangeMatchingSequence'),  # noqa
+    0x00080411: ('SQ', '1', "List of UID Matching Sequence", '', 'ListOfUIDMatchingSequence'),  # noqa
+    0x00080412: ('SQ', '1', "Empty Value Matching Sequence", '', 'EmptyValueMatchingSequence'),  # noqa
+    0x00080413: ('SQ', '1', "General Matching Sequence", '', 'GeneralMatchingSequence'),  # noqa
+    0x00080414: ('US', '1', "Requested Status Interval", '', 'RequestedStatusInterval'),  # noqa
+    0x00080415: ('CS', '1', "Retain Instances", '', 'RetainInstances'),  # noqa
+    0x00080416: ('DT', '1', "Expiration DateTime", '', 'ExpirationDateTime'),  # noqa
+    0x00080417: ('CS', '1', "Transaction Status", '', 'TransactionStatus'),  # noqa
+    0x00080418: ('LT', '1', "Transaction Status Comment", '', 'TransactionStatusComment'),  # noqa
+    0x00080419: ('SQ', '1', "File Set Access Sequence", '', 'FileSetAccessSequence'),  # noqa
+    0x0008041A: ('SQ', '1', "File Access Sequence", '', 'FileAccessSequence'),  # noqa
+    0x0008041B: ('OB', '1', "Record Key", '', 'RecordKey'),  # noqa
+    0x0008041C: ('OB', '1', "Prior Record Key", '', 'PriorRecordKey'),  # noqa
+    0x0008041D: ('SQ', '1', "Metadata Sequence", '', 'MetadataSequence'),  # noqa
+    0x0008041E: ('SQ', '1', "Updated Metadata Sequence", '', 'UpdatedMetadataSequence'),  # noqa
+    0x0008041F: ('DT', '1', "Study Update DateTime", '', 'StudyUpdateDateTime'),  # noqa
+    0x00080420: ('SQ', '1', "Inventory Access End Points Sequence", '', 'InventoryAccessEndPointsSequence'),  # noqa
+    0x00080421: ('SQ', '1', "Study Access End Points Sequence", '', 'StudyAccessEndPointsSequence'),  # noqa
+    0x00080422: ('SQ', '1', "Incorporated Inventory Instance Sequence", '', 'IncorporatedInventoryInstanceSequence'),  # noqa
+    0x00080423: ('SQ', '1', "Inventoried Studies Sequence", '', 'InventoriedStudiesSequence'),  # noqa
+    0x00080424: ('SQ', '1', "Inventoried Series Sequence", '', 'InventoriedSeriesSequence'),  # noqa
+    0x00080425: ('SQ', '1', "Inventoried Instances Sequence", '', 'InventoriedInstancesSequence'),  # noqa
+    0x00080426: ('CS', '1', "Inventory Completion Status", '', 'InventoryCompletionStatus'),  # noqa
+    0x00080427: ('UL', '1', "Number of Study Records in Instance", '', 'NumberOfStudyRecordsInInstance'),  # noqa
+    0x00080428: ('UV', '1', "Total Number of Study Records", '', 'TotalNumberOfStudyRecords'),  # noqa
+    0x00080429: ('UV', '1', "Maximum Number of Records", '', 'MaximumNumberOfRecords'),  # noqa
     0x00081000: ('AE', '1', "Network ID", 'Retired', 'NetworkID'),  # noqa
     0x00081010: ('SH', '1', "Station Name", '', 'StationName'),  # noqa
     0x00081030: ('LO', '1', "Study Description", '', 'StudyDescription'),  # noqa
     0x00081032: ('SQ', '1', "Procedure Code Sequence", '', 'ProcedureCodeSequence'),  # noqa
     0x0008103E: ('LO', '1', "Series Description", '', 'SeriesDescription'),  # noqa
     0x0008103F: ('SQ', '1', "Series Description Code Sequence", '', 'SeriesDescriptionCodeSequence'),  # noqa
     0x00081040: ('LO', '1', "Institutional Department Name", '', 'InstitutionalDepartmentName'),  # noqa
@@ -208,14 +252,15 @@
     0x00081052: ('SQ', '1', "Performing Physician Identification Sequence", '', 'PerformingPhysicianIdentificationSequence'),  # noqa
     0x00081060: ('PN', '1-n', "Name of Physician(s) Reading Study", '', 'NameOfPhysiciansReadingStudy'),  # noqa
     0x00081062: ('SQ', '1', "Physician(s) Reading Study Identification Sequence", '', 'PhysiciansReadingStudyIdentificationSequence'),  # noqa
     0x00081070: ('PN', '1-n', "Operators' Name", '', 'OperatorsName'),  # noqa
     0x00081072: ('SQ', '1', "Operator Identification Sequence", '', 'OperatorIdentificationSequence'),  # noqa
     0x00081080: ('LO', '1-n', "Admitting Diagnoses Description", '', 'AdmittingDiagnosesDescription'),  # noqa
     0x00081084: ('SQ', '1', "Admitting Diagnoses Code Sequence", '', 'AdmittingDiagnosesCodeSequence'),  # noqa
+    0x00081088: ('LO', '1', "Pyramid Description", '', 'PyramidDescription'),  # noqa
     0x00081090: ('LO', '1', "Manufacturer's Model Name", '', 'ManufacturerModelName'),  # noqa
     0x00081100: ('SQ', '1', "Referenced Results Sequence", 'Retired', 'ReferencedResultsSequence'),  # noqa
     0x00081110: ('SQ', '1', "Referenced Study Sequence", '', 'ReferencedStudySequence'),  # noqa
     0x00081111: ('SQ', '1', "Referenced Performed Procedure Step Sequence", '', 'ReferencedPerformedProcedureStepSequence'),  # noqa
     0x00081115: ('SQ', '1', "Referenced Series Sequence", '', 'ReferencedSeriesSequence'),  # noqa
     0x00081120: ('SQ', '1', "Referenced Patient Sequence", '', 'ReferencedPatientSequence'),  # noqa
     0x00081125: ('SQ', '1', "Referenced Visit Sequence", '', 'ReferencedVisitSequence'),  # noqa
@@ -286,15 +331,15 @@
     0x0008225C: ('SQ', '1', "On Axis Background Anatomic Structure Code Sequence (Trial)", 'Retired', 'OnAxisBackgroundAnatomicStructureCodeSequenceTrial'),  # noqa
     0x00083001: ('SQ', '1', "Alternate Representation Sequence", '', 'AlternateRepresentationSequence'),  # noqa
     0x00083002: ('UI', '1-n', "Available Transfer Syntax UID", '', 'AvailableTransferSyntaxUID'),  # noqa
     0x00083010: ('UI', '1-n', "Irradiation Event UID", '', 'IrradiationEventUID'),  # noqa
     0x00083011: ('SQ', '1', "Source Irradiation Event Sequence", '', 'SourceIrradiationEventSequence'),  # noqa
     0x00083012: ('UI', '1', "Radiopharmaceutical Administration Event UID", '', 'RadiopharmaceuticalAdministrationEventUID'),  # noqa
     0x00084000: ('LT', '1', "Identifying Comments", 'Retired', 'IdentifyingComments'),  # noqa
-    0x00089007: ('CS', '4', "Frame Type", '', 'FrameType'),  # noqa
+    0x00089007: ('CS', '4-5', "Frame Type", '', 'FrameType'),  # noqa
     0x00089092: ('SQ', '1', "Referenced Image Evidence Sequence", '', 'ReferencedImageEvidenceSequence'),  # noqa
     0x00089121: ('SQ', '1', "Referenced Raw Data Sequence", '', 'ReferencedRawDataSequence'),  # noqa
     0x00089123: ('UI', '1', "Creator-Version UID", '', 'CreatorVersionUID'),  # noqa
     0x00089124: ('SQ', '1', "Derivation Image Sequence", '', 'DerivationImageSequence'),  # noqa
     0x00089154: ('SQ', '1', "Source Image Evidence Sequence", '', 'SourceImageEvidenceSequence'),  # noqa
     0x00089205: ('CS', '1', "Pixel Presentation", '', 'PixelPresentation'),  # noqa
     0x00089206: ('CS', '1', "Volumetric Properties", '', 'VolumetricProperties'),  # noqa
@@ -390,14 +435,15 @@
     0x00120031: ('LO', '1', "Clinical Trial Site Name", '', 'ClinicalTrialSiteName'),  # noqa
     0x00120040: ('LO', '1', "Clinical Trial Subject ID", '', 'ClinicalTrialSubjectID'),  # noqa
     0x00120042: ('LO', '1', "Clinical Trial Subject Reading ID", '', 'ClinicalTrialSubjectReadingID'),  # noqa
     0x00120050: ('LO', '1', "Clinical Trial Time Point ID", '', 'ClinicalTrialTimePointID'),  # noqa
     0x00120051: ('ST', '1', "Clinical Trial Time Point Description", '', 'ClinicalTrialTimePointDescription'),  # noqa
     0x00120052: ('FD', '1', "Longitudinal Temporal Offset from Event", '', 'LongitudinalTemporalOffsetFromEvent'),  # noqa
     0x00120053: ('CS', '1', "Longitudinal Temporal Event Type", '', 'LongitudinalTemporalEventType'),  # noqa
+    0x00120054: ('SQ', '1', "Clinical Trial Time Point Type Code Sequence", '', 'ClinicalTrialTimePointTypeCodeSequence'),  # noqa
     0x00120060: ('LO', '1', "Clinical Trial Coordinating Center Name", '', 'ClinicalTrialCoordinatingCenterName'),  # noqa
     0x00120062: ('CS', '1', "Patient Identity Removed", '', 'PatientIdentityRemoved'),  # noqa
     0x00120063: ('LO', '1-n', "De-identification Method", '', 'DeidentificationMethod'),  # noqa
     0x00120064: ('SQ', '1', "De-identification Method Code Sequence", '', 'DeidentificationMethodCodeSequence'),  # noqa
     0x00120071: ('LO', '1', "Clinical Trial Series ID", '', 'ClinicalTrialSeriesID'),  # noqa
     0x00120072: ('LO', '1', "Clinical Trial Series Description", '', 'ClinicalTrialSeriesDescription'),  # noqa
     0x00120081: ('LO', '1', "Clinical Trial Protocol Ethics Committee Name", '', 'ClinicalTrialProtocolEthicsCommitteeName'),  # noqa
@@ -427,14 +473,22 @@
     0x00140102: ('DA', '1', "Secondary Review Date", '', 'SecondaryReviewDate'),  # noqa
     0x00140103: ('TM', '1', "Secondary Review Time", '', 'SecondaryReviewTime'),  # noqa
     0x00140104: ('PN', '1', "Secondary Reviewer Name", '', 'SecondaryReviewerName'),  # noqa
     0x00140105: ('ST', '1', "Repair ID", '', 'RepairID'),  # noqa
     0x00140106: ('SQ', '1', "Multiple Component Approval Sequence", '', 'MultipleComponentApprovalSequence'),  # noqa
     0x00140107: ('CS', '1-n', "Other Approval Status", '', 'OtherApprovalStatus'),  # noqa
     0x00140108: ('CS', '1-n', "Other Secondary Approval Status", '', 'OtherSecondaryApprovalStatus'),  # noqa
+    0x00140200: ('SQ', '1', "Data Element Label Sequence", '', 'DataElementLabelSequence'),  # noqa
+    0x00140201: ('SQ', '1', "Data Element Label Item Sequence", '', 'DataElementLabelItemSequence'),  # noqa
+    0x00140202: ('AT', '1', "Data Element", '', 'DataElement'),  # noqa
+    0x00140203: ('LO', '1', "Data Element Name", '', 'DataElementName'),  # noqa
+    0x00140204: ('LO', '1', "Data Element Description", '', 'DataElementDescription'),  # noqa
+    0x00140205: ('CS', '1', "Data Element Conditionality", '', 'DataElementConditionality'),  # noqa
+    0x00140206: ('IS', '1', "Data Element Minimum Characters", '', 'DataElementMinimumCharacters'),  # noqa
+    0x00140207: ('IS', '1', "Data Element Maximum Characters", '', 'DataElementMaximumCharacters'),  # noqa
     0x00141010: ('ST', '1', "Actual Environmental Conditions", '', 'ActualEnvironmentalConditions'),  # noqa
     0x00141020: ('DA', '1', "Expiry Date", '', 'ExpiryDate'),  # noqa
     0x00141040: ('ST', '1', "Environmental Conditions", '', 'EnvironmentalConditions'),  # noqa
     0x00142002: ('SQ', '1', "Evaluator Sequence", '', 'EvaluatorSequence'),  # noqa
     0x00142004: ('IS', '1', "Evaluator Number", '', 'EvaluatorNumber'),  # noqa
     0x00142006: ('PN', '1', "Evaluator Name", '', 'EvaluatorName'),  # noqa
     0x00142008: ('IS', '1', "Evaluation Attempt", '', 'EvaluationAttempt'),  # noqa
@@ -1597,14 +1651,15 @@
     0x00200017: ('IS', '1', "Time Slot Number", 'Retired', 'TimeSlotNumber'),  # noqa
     0x00200018: ('IS', '1', "Angle Number", 'Retired', 'AngleNumber'),  # noqa
     0x00200019: ('IS', '1', "Item Number", '', 'ItemNumber'),  # noqa
     0x00200020: ('CS', '2', "Patient Orientation", '', 'PatientOrientation'),  # noqa
     0x00200022: ('IS', '1', "Overlay Number", 'Retired', 'OverlayNumber'),  # noqa
     0x00200024: ('IS', '1', "Curve Number", 'Retired', 'CurveNumber'),  # noqa
     0x00200026: ('IS', '1', "LUT Number", 'Retired', 'LUTNumber'),  # noqa
+    0x00200027: ('LO', '1', "Pyramid Label", '', 'PyramidLabel'),  # noqa
     0x00200030: ('DS', '3', "Image Position", 'Retired', 'ImagePosition'),  # noqa
     0x00200032: ('DS', '3', "Image Position (Patient)", '', 'ImagePositionPatient'),  # noqa
     0x00200035: ('DS', '6', "Image Orientation", 'Retired', 'ImageOrientation'),  # noqa
     0x00200037: ('DS', '6', "Image Orientation (Patient)", '', 'ImageOrientationPatient'),  # noqa
     0x00200050: ('DS', '1', "Location", 'Retired', 'Location'),  # noqa
     0x00200052: ('UI', '1', "Frame of Reference UID", '', 'FrameOfReferenceUID'),  # noqa
     0x00200060: ('CS', '1', "Laterality", '', 'Laterality'),  # noqa
@@ -2117,14 +2172,15 @@
     0x00281410: ('CS', '1', "Alpha LUT Transfer Function", '', 'AlphaLUTTransferFunction'),  # noqa
     0x00282000: ('OB', '1', "ICC Profile", '', 'ICCProfile'),  # noqa
     0x00282002: ('CS', '1', "Color Space", '', 'ColorSpace'),  # noqa
     0x00282110: ('CS', '1', "Lossy Image Compression", '', 'LossyImageCompression'),  # noqa
     0x00282112: ('DS', '1-n', "Lossy Image Compression Ratio", '', 'LossyImageCompressionRatio'),  # noqa
     0x00282114: ('CS', '1-n', "Lossy Image Compression Method", '', 'LossyImageCompressionMethod'),  # noqa
     0x00283000: ('SQ', '1', "Modality LUT Sequence", '', 'ModalityLUTSequence'),  # noqa
+    0x00283001: ('SQ', '1', "Variable Modality LUT Sequence", '', 'VariableModalityLUTSequence'),  # noqa
     0x00283002: ('US or SS', '3', "LUT Descriptor", '', 'LUTDescriptor'),  # noqa
     0x00283003: ('LO', '1', "LUT Explanation", '', 'LUTExplanation'),  # noqa
     0x00283004: ('LO', '1', "Modality LUT Type", '', 'ModalityLUTType'),  # noqa
     0x00283006: ('US or OW', '1-n', "LUT Data", '', 'LUTData'),  # noqa
     0x00283010: ('SQ', '1', "VOI LUT Sequence", '', 'VOILUTSequence'),  # noqa
     0x00283110: ('SQ', '1', "Softcopy VOI LUT Sequence", '', 'SoftcopyVOILUTSequence'),  # noqa
     0x00284000: ('LT', '1', "Image Presentation Comments", 'Retired', 'ImagePresentationComments'),  # noqa
@@ -2332,14 +2388,32 @@
     0x003A0310: ('UI', '1', "Multiplex Group UID", '', 'MultiplexGroupUID'),  # noqa
     0x003A0311: ('DS', '1', "Powerline Frequency", '', 'PowerlineFrequency'),  # noqa
     0x003A0312: ('SQ', '1', "Channel Impedance Sequence", '', 'ChannelImpedanceSequence'),  # noqa
     0x003A0313: ('DS', '1', "Impedance Value", '', 'ImpedanceValue'),  # noqa
     0x003A0314: ('DT', '1', "Impedance Measurement DateTime", '', 'ImpedanceMeasurementDateTime'),  # noqa
     0x003A0315: ('DS', '1', "Impedance Measurement Frequency", '', 'ImpedanceMeasurementFrequency'),  # noqa
     0x003A0316: ('CS', '1', "Impedance Measurement Current Type", '', 'ImpedanceMeasurementCurrentType'),  # noqa
+    0x003A0317: ('CS', '1', "Waveform Amplifier Type", '', 'WaveformAmplifierType'),  # noqa
+    0x003A0318: ('SQ', '1', "Filter Low Frequency Characteristics Sequence", '', 'FilterLowFrequencyCharacteristicsSequence'),  # noqa
+    0x003A0319: ('SQ', '1', "Filter High Frequency Characteristics Sequence", '', 'FilterHighFrequencyCharacteristicsSequence'),  # noqa
+    0x003A0320: ('SQ', '1', "Summarized Filter Lookup Table Sequence", '', 'SummarizedFilterLookupTable'),  # noqa
+    0x003A0321: ('SQ', '1', "Notch Filter Characteristics Sequence", '', 'NotchFilterCharacteristicsSequence'),  # noqa
+    0x003A0322: ('CS', '1', "Waveform Filter Type", '', 'WaveformFilterType'),  # noqa
+    0x003A0323: ('SQ', '1', "Analog Filter Characteristics Sequence", '', 'AnalogFilterCharacteristicsSequence'),  # noqa
+    0x003A0324: ('DS', '1', "Analog Filter Roll Off", '', 'AnalogFilterRollOff'),  # noqa
+    0x003A0325: ('SQ', '1', "Analog Filter Type Code Sequence", '', 'AnalogFilterType'),  # noqa
+    0x003A0326: ('SQ', '1', "Digital Filter Characteristics Sequence", '', 'DigitalFilterCharacteristicsSequence'),  # noqa
+    0x003A0327: ('IS', '1', "Digital Filter Order", '', 'DigitalFilterOrder'),  # noqa
+    0x003A0328: ('SQ', '1', "Digital Filter Type Code Sequence", '', 'DigitalFilterTypeCodeSequence'),  # noqa
+    0x003A0329: ('ST', '1', "Waveform Filter Description", '', 'WaveformFilterDescription'),  # noqa
+    0x003A032A: ('SQ', '1', "Filter Lookup Table Sequence", '', 'FilterLookupTableSequence'),  # noqa
+    0x003A032B: ('ST', '1', "Filter Lookup Table Description", '', 'FilterLookupTableDescription'),  # noqa
+    0x003A032C: ('SQ', '1', "Frequency Encoding Code Sequence", '', 'FrequencyEncodingCodeSequence'),  # noqa
+    0x003A032D: ('SQ', '1', "Magnitude Encoding Code Sequence", '', 'MagnitudeEncodingCodeSequence'),  # noqa
+    0x003A032E: ('OD', '1', "Filter Lookup Table Data", '', 'FilterLookupTableData'),  # noqa
     0x00400001: ('AE', '1-n', "Scheduled Station AE Title", '', 'ScheduledStationAETitle'),  # noqa
     0x00400002: ('DA', '1', "Scheduled Procedure Step Start Date", '', 'ScheduledProcedureStepStartDate'),  # noqa
     0x00400003: ('TM', '1', "Scheduled Procedure Step Start Time", '', 'ScheduledProcedureStepStartTime'),  # noqa
     0x00400004: ('DA', '1', "Scheduled Procedure Step End Date", '', 'ScheduledProcedureStepEndDate'),  # noqa
     0x00400005: ('TM', '1', "Scheduled Procedure Step End Time", '', 'ScheduledProcedureStepEndTime'),  # noqa
     0x00400006: ('PN', '1', "Scheduled Performing Physician's Name", '', 'ScheduledPerformingPhysicianName'),  # noqa
     0x00400007: ('LO', '1', "Scheduled Procedure Step Description", '', 'ScheduledProcedureStepDescription'),  # noqa
@@ -3230,14 +3304,15 @@
     0x0070030C: ('CS', '1', "Frame of Reference Transformation Matrix Type", '', 'FrameOfReferenceTransformationMatrixType'),  # noqa
     0x0070030D: ('SQ', '1', "Registration Type Code Sequence", '', 'RegistrationTypeCodeSequence'),  # noqa
     0x0070030F: ('ST', '1', "Fiducial Description", '', 'FiducialDescription'),  # noqa
     0x00700310: ('SH', '1', "Fiducial Identifier", '', 'FiducialIdentifier'),  # noqa
     0x00700311: ('SQ', '1', "Fiducial Identifier Code Sequence", '', 'FiducialIdentifierCodeSequence'),  # noqa
     0x00700312: ('FD', '1', "Contour Uncertainty Radius", '', 'ContourUncertaintyRadius'),  # noqa
     0x00700314: ('SQ', '1', "Used Fiducials Sequence", '', 'UsedFiducialsSequence'),  # noqa
+    0x00700315: ('SQ', '1', "Used RT Structure Set ROI Sequence", '', 'UsedRTStructureSetROISequence'),  # noqa
     0x00700318: ('SQ', '1', "Graphic Coordinates Data Sequence", '', 'GraphicCoordinatesDataSequence'),  # noqa
     0x0070031A: ('UI', '1', "Fiducial UID", '', 'FiducialUID'),  # noqa
     0x0070031B: ('UI', '1', "Referenced Fiducial UID", '', 'ReferencedFiducialUID'),  # noqa
     0x0070031C: ('SQ', '1', "Fiducial Set Sequence", '', 'FiducialSetSequence'),  # noqa
     0x0070031E: ('SQ', '1', "Fiducial Sequence", '', 'FiducialSequence'),  # noqa
     0x0070031F: ('SQ', '1', "Fiducials Property Category Code Sequence", '', 'FiducialsPropertyCategoryCodeSequence'),  # noqa
     0x00700401: ('US', '3', "Graphic Layer Recommended Display CIELab Value", '', 'GraphicLayerRecommendedDisplayCIELabValue'),  # noqa
@@ -3733,16 +3808,16 @@
     0x21300010: ('SQ', '1', "Print Management Capabilities Sequence", 'Retired', 'PrintManagementCapabilitiesSequence'),  # noqa
     0x21300015: ('SQ', '1', "Printer Characteristics Sequence", 'Retired', 'PrinterCharacteristicsSequence'),  # noqa
     0x21300030: ('SQ', '1', "Film Box Content Sequence", 'Retired', 'FilmBoxContentSequence'),  # noqa
     0x21300040: ('SQ', '1', "Image Box Content Sequence", 'Retired', 'ImageBoxContentSequence'),  # noqa
     0x21300050: ('SQ', '1', "Annotation Content Sequence", 'Retired', 'AnnotationContentSequence'),  # noqa
     0x21300060: ('SQ', '1', "Image Overlay Box Content Sequence", 'Retired', 'ImageOverlayBoxContentSequence'),  # noqa
     0x21300080: ('SQ', '1', "Presentation LUT Content Sequence", 'Retired', 'PresentationLUTContentSequence'),  # noqa
-    0x213000A0: ('SQ', '1', "Proposed Study Sequence", 'Retired', 'ProposedStudySequence'),  # noqa
-    0x213000C0: ('SQ', '1', "Original Image Sequence", 'Retired', 'OriginalImageSequence'),  # noqa
+    0x213000A0: ('SQ', '1', "Proposed Study Sequence", '', 'ProposedStudySequence'),  # noqa
+    0x213000C0: ('SQ', '1', "Original Image Sequence", '', 'OriginalImageSequence'),  # noqa
     0x22000001: ('CS', '1', "Label Using Information Extracted From Instances", '', 'LabelUsingInformationExtractedFromInstances'),  # noqa
     0x22000002: ('UT', '1', "Label Text", '', 'LabelText'),  # noqa
     0x22000003: ('CS', '1', "Label Style Selection", '', 'LabelStyleSelection'),  # noqa
     0x22000004: ('LT', '1', "Media Disposition", '', 'MediaDisposition'),  # noqa
     0x22000005: ('LT', '1', "Barcode Value", '', 'BarcodeValue'),  # noqa
     0x22000006: ('CS', '1', "Barcode Symbology", '', 'BarcodeSymbology'),  # noqa
     0x22000007: ('CS', '1', "Allow Media Splitting", '', 'AllowMediaSplitting'),  # noqa
@@ -3776,25 +3851,79 @@
     0x30020034: ('DS', '4', "Diaphragm Position", '', 'DiaphragmPosition'),  # noqa
     0x30020040: ('SQ', '1', "Fluence Map Sequence", '', 'FluenceMapSequence'),  # noqa
     0x30020041: ('CS', '1', "Fluence Data Source", '', 'FluenceDataSource'),  # noqa
     0x30020042: ('DS', '1', "Fluence Data Scale", '', 'FluenceDataScale'),  # noqa
     0x30020050: ('SQ', '1', "Primary Fluence Mode Sequence", '', 'PrimaryFluenceModeSequence'),  # noqa
     0x30020051: ('CS', '1', "Fluence Mode", '', 'FluenceMode'),  # noqa
     0x30020052: ('SH', '1', "Fluence Mode ID", '', 'FluenceModeID'),  # noqa
+    0x30020100: ('IS', '1', "Selected Frame Number", '', 'SelectedFrameNumber'),  # noqa
+    0x30020101: ('SQ', '1', "Selected Frame Functional Groups Sequence", '', 'SelectedFrameFunctionalGroupsSequence'),  # noqa
+    0x30020102: ('SQ', '1', "RT Image Frame General Content Sequence", '', 'RTImageFrameGeneralContentSequence'),  # noqa
+    0x30020103: ('SQ', '1', "RT Image Frame Context Sequence", '', 'RTImageFrameContextSequence'),  # noqa
+    0x30020104: ('SQ', '1', "RT Image Scope Sequence", '', 'RTImageScopeSequence'),  # noqa
+    0x30020105: ('CS', '1', "Beam Modifier Coordinates Presence Flag", '', 'BeamModifierCoordinatesPresenceFlag'),  # noqa
+    0x30020106: ('FD', '1', "Start Cumulative Meterset", '', 'StartCumulativeMeterset'),  # noqa
+    0x30020107: ('FD', '1', "Stop Cumulative Meterset", '', 'StopCumulativeMeterset'),  # noqa
+    0x30020108: ('SQ', '1', "RT Acquisition Patient Position Sequence", '', 'RTAcquisitionPatientPositionSequence'),  # noqa
+    0x30020109: ('SQ', '1', "RT Image Frame Imaging Device Position Sequence", '', 'RTImageFrameImagingDevicePositionSequence'),  # noqa
+    0x3002010A: ('SQ', '1', "RT Image Frame kV Radiation Acquisition Sequence", '', 'RTImageFramekVRadiationAcquisitionSequence'),  # noqa
+    0x3002010B: ('SQ', '1', "RT Image Frame MV Radiation Acquisition Sequence", '', 'RTImageFrameMVRadiationAcquisitionSequence'),  # noqa
+    0x3002010C: ('SQ', '1', "RT Image Frame Radiation Acquisition Sequence", '', 'RTImageFrameRadiationAcquisitionSequence'),  # noqa
+    0x3002010D: ('SQ', '1', "Imaging Source Position Sequence", '', 'ImagingSourcePositionSequence'),  # noqa
+    0x3002010E: ('SQ', '1', "Image Receptor Position Sequence", '', 'ImageReceptorPositionSequence'),  # noqa
+    0x3002010F: ('FD', '16', "Device Position to Equipment Mapping Matrix", '', 'DevicePositionToEquipmentMappingMatrix'),  # noqa
+    0x30020110: ('SQ', '1', "Device Position Parameter Sequence", '', 'DevicePositionParameterSequence'),  # noqa
+    0x30020111: ('CS', '1', "Imaging Source Location Specification Type", '', 'ImagingSourceLocationSpecificationType'),  # noqa
+    0x30020112: ('SQ', '1', "Imaging Device Location Matrix Sequence", '', 'ImagingDeviceLocationMatrixSequence'),  # noqa
+    0x30020113: ('SQ', '1', "Imaging Device Location Parameter Sequence", '', 'ImagingDeviceLocationParameterSequence'),  # noqa
+    0x30020114: ('SQ', '1', "Imaging Aperture Sequence", '', 'ImagingApertureSequence'),  # noqa
+    0x30020115: ('CS', '1', "Imaging Aperture Specification Type", '', 'ImagingApertureSpecificationType'),  # noqa
+    0x30020116: ('US', '1', "Number of Acquisition Devices", '', 'NumberOfAcquisitionDevices'),  # noqa
+    0x30020117: ('SQ', '1', "Acquisition Device Sequence", '', 'AcquisitionDeviceSequence'),  # noqa
+    0x30020118: ('SQ', '1', "Acquisition Task Sequence", '', 'AcquisitionTaskSequence'),  # noqa
+    0x30020119: ('SQ', '1', "Acquisition Task Workitem Code Sequence", '', 'AcquisitionTaskWorkitemCodeSequence'),  # noqa
+    0x3002011A: ('SQ', '1', "Acquisition Subtask Sequence", '', 'AcquisitionSubtaskSequence'),  # noqa
+    0x3002011B: ('SQ', '1', "Subtask Workitem Code Sequence", '', 'SubtaskWorkitemCodeSequence'),  # noqa
+    0x3002011C: ('US', '1', "Acquisition Task Index", '', 'AcquisitionTaskIndex'),  # noqa
+    0x3002011D: ('US', '1', "Acquisition Subtask Index", '', 'AcquisitionSubtaskIndex'),  # noqa
+    0x3002011E: ('SQ', '1', "Referenced Baseline Parameters RT Radiation Instance Sequence", '', 'ReferencedBaselineParametersRTRadiationInstanceSequence'),  # noqa
+    0x3002011F: ('SQ', '1', "Position Acquisition Template Identification Sequence", '', 'PositionAcquisitionTemplateIdentificationSequence'),  # noqa
+    0x30020120: ('ST', '1', "Position Acquisition Template ID", '', 'PositionAcquisitionTemplateID'),  # noqa
+    0x30020121: ('LO', '1', "Position Acquisition Template Name", '', 'PositionAcquisitionTemplateName'),  # noqa
+    0x30020122: ('SQ', '1', "Position Acquisition Template Code Sequence", '', 'PositionAcquisitionTemplateCodeSequence'),  # noqa
+    0x30020123: ('LT', '1', "Position Acquisition Template Description", '', 'PositionAcquisitionTemplateDescription'),  # noqa
+    0x30020124: ('SQ', '1', "Acquisition Task Applicability Sequence", '', 'AcquisitionTaskApplicabilitySequence'),  # noqa
+    0x30020125: ('SQ', '1', "Projection Imaging Acquisition Parameter Sequence", '', 'ProjectionImagingAcquisitionParameterSequence'),  # noqa
+    0x30020126: ('SQ', '1', "CT Imaging Acquisition Parameter Sequence", '', 'CTImagingAcquisitionParameterSequence'),  # noqa
+    0x30020127: ('SQ', '1', "KV Imaging Generation Parameters Sequence", '', 'KVImagingGenerationParametersSequence'),  # noqa
+    0x30020128: ('SQ', '1', "MV Imaging Generation Parameters Sequence", '', 'MVImagingGenerationParametersSequence'),  # noqa
+    0x30020129: ('CS', '1', "Acquisition Signal Type", '', 'AcquisitionSignalType'),  # noqa
+    0x3002012A: ('CS', '1', "Acquisition Method", '', 'AcquisitionMethod'),  # noqa
+    0x3002012B: ('SQ', '1', "Scan Start Position Sequence", '', 'ScanStartPositionSequence'),  # noqa
+    0x3002012C: ('SQ', '1', "Scan Stop Position Sequence", '', 'ScanStopPositionSequence'),  # noqa
+    0x3002012D: ('FD', '1', "Imaging Source to Beam Modifier Definition Plane Distance", '', 'ImagingSourceToBeamModifierDefinitionPlaneDistance'),  # noqa
+    0x3002012E: ('CS', '1', "Scan Arc Type", '', 'ScanArcType'),  # noqa
+    0x3002012F: ('CS', '1', "Detector Positioning Type", '', 'DetectorPositioningType'),  # noqa
+    0x30020130: ('SQ', '1', "Additional RT Accessory Device Sequence", '', 'AdditionalRTAccessoryDeviceSequence'),  # noqa
+    0x30020131: ('SQ', '1', "Device-Specific Acquisition Parameter Sequence", '', 'DeviceSpecificAcquisitionParameterSequence'),  # noqa
+    0x30020132: ('SQ', '1', "Referenced Position Reference Instance Sequence", '', 'ReferencedPositionReferenceInstanceSequence'),  # noqa
+    0x30020133: ('SQ', '1', "Energy Derivation Code Sequence", '', 'EnergyDerivationCodeSequence'),  # noqa
+    0x30020134: ('FD', '1', "Maximum Cumulative Meterset Exposure", '', 'MaximumCumulativeMetersetExposure'),  # noqa
+    0x30020135: ('SQ', '1', "Acquisition Initiation Sequence", '', 'AcquisitionInitiationSequence'),  # noqa
     0x30040001: ('CS', '1', "DVH Type", '', 'DVHType'),  # noqa
     0x30040002: ('CS', '1', "Dose Units", '', 'DoseUnits'),  # noqa
     0x30040004: ('CS', '1', "Dose Type", '', 'DoseType'),  # noqa
     0x30040005: ('CS', '1', "Spatial Transform of Dose", '', 'SpatialTransformOfDose'),  # noqa
     0x30040006: ('LO', '1', "Dose Comment", '', 'DoseComment'),  # noqa
     0x30040008: ('DS', '3', "Normalization Point", '', 'NormalizationPoint'),  # noqa
     0x3004000A: ('CS', '1', "Dose Summation Type", '', 'DoseSummationType'),  # noqa
     0x3004000C: ('DS', '2-n', "Grid Frame Offset Vector", '', 'GridFrameOffsetVector'),  # noqa
     0x3004000E: ('DS', '1', "Dose Grid Scaling", '', 'DoseGridScaling'),  # noqa
-    0x30040010: ('SQ', '1', "RT Dose ROI Sequence", '', 'RTDoseROISequence'),  # noqa
-    0x30040012: ('DS', '1', "Dose Value", '', 'DoseValue'),  # noqa
+    0x30040010: ('SQ', '1', "RT Dose ROI Sequence", 'Retired', 'RTDoseROISequence'),  # noqa
+    0x30040012: ('DS', '1', "Dose Value", 'Retired', 'DoseValue'),  # noqa
     0x30040014: ('CS', '1-3', "Tissue Heterogeneity Correction", '', 'TissueHeterogeneityCorrection'),  # noqa
     0x30040040: ('DS', '3', "DVH Normalization Point", '', 'DVHNormalizationPoint'),  # noqa
     0x30040042: ('DS', '1', "DVH Normalization Dose Value", '', 'DVHNormalizationDoseValue'),  # noqa
     0x30040050: ('SQ', '1', "DVH Sequence", '', 'DVHSequence'),  # noqa
     0x30040052: ('DS', '1', "DVH Dose Scaling", '', 'DVHDoseScaling'),  # noqa
     0x30040054: ('CS', '1', "DVH Volume Units", '', 'DVHVolumeUnits'),  # noqa
     0x30040056: ('IS', '1', "DVH Number of Bins", '', 'DVHNumberOfBins'),  # noqa
@@ -3835,17 +3964,17 @@
     0x30060048: ('IS', '1', "Contour Number", '', 'ContourNumber'),  # noqa
     0x30060049: ('IS', '1-n', "Attached Contours", 'Retired', 'AttachedContours'),  # noqa
     0x3006004A: ('SQ', '1', "Source Pixel Planes Characteristics Sequence", '', 'SourcePixelPlanesCharacteristicsSequence'),  # noqa
     0x30060050: ('DS', '3-3n', "Contour Data", '', 'ContourData'),  # noqa
     0x30060080: ('SQ', '1', "RT ROI Observations Sequence", '', 'RTROIObservationsSequence'),  # noqa
     0x30060082: ('IS', '1', "Observation Number", '', 'ObservationNumber'),  # noqa
     0x30060084: ('IS', '1', "Referenced ROI Number", '', 'ReferencedROINumber'),  # noqa
-    0x30060085: ('SH', '1', "ROI Observation Label", '', 'ROIObservationLabel'),  # noqa
+    0x30060085: ('SH', '1', "ROI Observation Label", 'Retired', 'ROIObservationLabel'),  # noqa
     0x30060086: ('SQ', '1', "RT ROI Identification Code Sequence", '', 'RTROIIdentificationCodeSequence'),  # noqa
-    0x30060088: ('ST', '1', "ROI Observation Description", '', 'ROIObservationDescription'),  # noqa
+    0x30060088: ('ST', '1', "ROI Observation Description", 'Retired', 'ROIObservationDescription'),  # noqa
     0x300600A0: ('SQ', '1', "Related RT ROI Observations Sequence", '', 'RelatedRTROIObservationsSequence'),  # noqa
     0x300600A4: ('CS', '1', "RT ROI Interpreted Type", '', 'RTROIInterpretedType'),  # noqa
     0x300600A6: ('PN', '1', "ROI Interpreter", '', 'ROIInterpreter'),  # noqa
     0x300600B0: ('SQ', '1', "ROI Physical Properties Sequence", '', 'ROIPhysicalPropertiesSequence'),  # noqa
     0x300600B2: ('CS', '1', "ROI Physical Property", '', 'ROIPhysicalProperty'),  # noqa
     0x300600B4: ('DS', '1', "ROI Physical Property Value", '', 'ROIPhysicalPropertyValue'),  # noqa
     0x300600B6: ('SQ', '1', "ROI Elemental Composition Sequence", '', 'ROIElementalCompositionSequence'),  # noqa
@@ -3866,15 +3995,15 @@
     0x30080016: ('DS', '1', "Measured Dose Value", '', 'MeasuredDoseValue'),  # noqa
     0x30080020: ('SQ', '1', "Treatment Session Beam Sequence", '', 'TreatmentSessionBeamSequence'),  # noqa
     0x30080021: ('SQ', '1', "Treatment Session Ion Beam Sequence", '', 'TreatmentSessionIonBeamSequence'),  # noqa
     0x30080022: ('IS', '1', "Current Fraction Number", '', 'CurrentFractionNumber'),  # noqa
     0x30080024: ('DA', '1', "Treatment Control Point Date", '', 'TreatmentControlPointDate'),  # noqa
     0x30080025: ('TM', '1', "Treatment Control Point Time", '', 'TreatmentControlPointTime'),  # noqa
     0x3008002A: ('CS', '1', "Treatment Termination Status", '', 'TreatmentTerminationStatus'),  # noqa
-    0x3008002B: ('SH', '1', "Treatment Termination Code", '', 'TreatmentTerminationCode'),  # noqa
+    0x3008002B: ('SH', '1', "Treatment Termination Code", 'Retired', 'TreatmentTerminationCode'),  # noqa
     0x3008002C: ('CS', '1', "Treatment Verification Status", '', 'TreatmentVerificationStatus'),  # noqa
     0x30080030: ('SQ', '1', "Referenced Treatment Record Sequence", '', 'ReferencedTreatmentRecordSequence'),  # noqa
     0x30080032: ('DS', '1', "Specified Primary Meterset", '', 'SpecifiedPrimaryMeterset'),  # noqa
     0x30080033: ('DS', '1', "Specified Secondary Meterset", '', 'SpecifiedSecondaryMeterset'),  # noqa
     0x30080036: ('DS', '1', "Delivered Primary Meterset", '', 'DeliveredPrimaryMeterset'),  # noqa
     0x30080037: ('DS', '1', "Delivered Secondary Meterset", '', 'DeliveredSecondaryMeterset'),  # noqa
     0x3008003A: ('DS', '1', "Specified Treatment Time", '', 'SpecifiedTreatmentTime'),  # noqa
@@ -3909,14 +4038,18 @@
     0x30080078: ('DS', '1', "Start Meterset", '', 'StartMeterset'),  # noqa
     0x3008007A: ('DS', '1', "End Meterset", '', 'EndMeterset'),  # noqa
     0x30080080: ('SQ', '1', "Referenced Measured Dose Reference Sequence", '', 'ReferencedMeasuredDoseReferenceSequence'),  # noqa
     0x30080082: ('IS', '1', "Referenced Measured Dose Reference Number", '', 'ReferencedMeasuredDoseReferenceNumber'),  # noqa
     0x30080090: ('SQ', '1', "Referenced Calculated Dose Reference Sequence", '', 'ReferencedCalculatedDoseReferenceSequence'),  # noqa
     0x30080092: ('IS', '1', "Referenced Calculated Dose Reference Number", '', 'ReferencedCalculatedDoseReferenceNumber'),  # noqa
     0x300800A0: ('SQ', '1', "Beam Limiting Device Leaf Pairs Sequence", '', 'BeamLimitingDeviceLeafPairsSequence'),  # noqa
+    0x300800A1: ('SQ', '1', "Enhanced RT Beam Limiting Device Sequence", '', 'EnhancedRTBeamLimitingDeviceSequence'),  # noqa
+    0x300800A2: ('SQ', '1', "Enhanced RT Beam Limiting Opening Sequence", '', 'EnhancedRTBeamLimitingOpeningSequence'),  # noqa
+    0x300800A3: ('CS', '1', "Enhanced RT Beam Limiting Device Definition Flag", '', 'EnhancedRTBeamLimitingDeviceDefinitionFlag'),  # noqa
+    0x300800A4: ('FD', '2-2n', "Parallel RT Beam Delimiter Opening Extents", '', 'ParallelRTBeamDelimiterOpeningExtents'),  # noqa
     0x300800B0: ('SQ', '1', "Recorded Wedge Sequence", '', 'RecordedWedgeSequence'),  # noqa
     0x300800C0: ('SQ', '1', "Recorded Compensator Sequence", '', 'RecordedCompensatorSequence'),  # noqa
     0x300800D0: ('SQ', '1', "Recorded Block Sequence", '', 'RecordedBlockSequence'),  # noqa
     0x300800D1: ('SQ', '1', "Recorded Block Slab Sequence", '', 'RecordedBlockSlabSequence'),  # noqa
     0x300800E0: ('SQ', '1', "Treatment Summary Measured Dose Reference Sequence", '', 'TreatmentSummaryMeasuredDoseReferenceSequence'),  # noqa
     0x300800F0: ('SQ', '1', "Recorded Snout Sequence", '', 'RecordedSnoutSequence'),  # noqa
     0x300800F2: ('SQ', '1', "Recorded Range Shifter Sequence", '', 'RecordedRangeShifterSequence'),  # noqa
@@ -4751,25 +4884,26 @@
     0x30100083: ('CS', '1', "Fraction-Based Relationship Interval Anchor", '', 'FractionBasedRelationshipIntervalAnchor'),  # noqa
     0x30100084: ('FD', '1', "Minimum Hours between Fractions", '', 'MinimumHoursBetweenFractions'),  # noqa
     0x30100085: ('TM', '1-n', "Intended Fraction Start Time", '', 'IntendedFractionStartTime'),  # noqa
     0x30100086: ('LT', '1', "Intended Start Day of Week", '', 'IntendedStartDayOfWeek'),  # noqa
     0x30100087: ('SQ', '1', "Weekday Fraction Pattern Sequence", '', 'WeekdayFractionPatternSequence'),  # noqa
     0x30100088: ('SQ', '1', "Delivery Time Structure Code Sequence", '', 'DeliveryTimeStructureCodeSequence'),  # noqa
     0x30100089: ('SQ', '1', "Treatment Site Modifier Code Sequence", '', 'TreatmentSiteModifierCodeSequence'),  # noqa
-    0x30100090: ('CS', '1', "Robotic Base Location Indicator", '', 'RoboticBaseLocationIndicator'),  # noqa
+    0x30100090: ('CS', '1', "Robotic Base Location Indicator", 'Retired', 'RoboticBaseLocationIndicator'),  # noqa
     0x30100091: ('SQ', '1', "Robotic Path Node Set Code Sequence", '', 'RoboticPathNodeSetCodeSequence'),  # noqa
     0x30100092: ('UL', '1', "Robotic Node Identifier", '', 'RoboticNodeIdentifier'),  # noqa
     0x30100093: ('FD', '3', "RT Treatment Source Coordinates", '', 'RTTreatmentSourceCoordinates'),  # noqa
     0x30100094: ('FD', '1', "Radiation Source Coordinate SystemYaw Angle", '', 'RadiationSourceCoordinateSystemYawAngle'),  # noqa
     0x30100095: ('FD', '1', "Radiation Source Coordinate SystemRoll Angle", '', 'RadiationSourceCoordinateSystemRollAngle'),  # noqa
     0x30100096: ('FD', '1', "Radiation Source Coordinate System Pitch Angle", '', 'RadiationSourceCoordinateSystemPitchAngle'),  # noqa
     0x30100097: ('SQ', '1', "Robotic Path Control Point Sequence", '', 'RoboticPathControlPointSequence'),  # noqa
     0x30100098: ('SQ', '1', "Tomotherapeutic Control Point Sequence", '', 'TomotherapeuticControlPointSequence'),  # noqa
     0x30100099: ('FD', '1-n', "Tomotherapeutic Leaf Open Durations", '', 'TomotherapeuticLeafOpenDurations'),  # noqa
     0x3010009A: ('FD', '1-n', "Tomotherapeutic Leaf Initial Closed Durations", '', 'TomotherapeuticLeafInitialClosedDurations'),  # noqa
+    0x301000A0: ('SQ', '1', "Conceptual Volume Identification Sequence", '', 'ConceptualVolumeIdentificationSequence'),  # noqa
     0x40000010: ('LT', '1', "Arbitrary", 'Retired', 'Arbitrary'),  # noqa
     0x40004000: ('LT', '1', "Text Comments", 'Retired', 'TextComments'),  # noqa
     0x40080040: ('SH', '1', "Results ID", 'Retired', 'ResultsID'),  # noqa
     0x40080042: ('LO', '1', "Results ID Issuer", 'Retired', 'ResultsIDIssuer'),  # noqa
     0x40080050: ('SQ', '1', "Referenced Interpretation Sequence", 'Retired', 'ReferencedInterpretationSequence'),  # noqa
     0x400800FF: ('CS', '1', "Report Production Status (Trial)", 'Retired', 'ReportProductionStatusTrial'),  # noqa
     0x40080100: ('DA', '1', "Interpretation Recorded Date", 'Retired', 'InterpretationRecordedDate'),  # noqa
@@ -4892,14 +5026,15 @@
     0x54001006: ('CS', '1', "Waveform Sample Interpretation", '', 'WaveformSampleInterpretation'),  # noqa
     0x5400100A: ('OB or OW', '1', "Waveform Padding Value", '', 'WaveformPaddingValue'),  # noqa
     0x54001010: ('OB or OW', '1', "Waveform Data", '', 'WaveformData'),  # noqa
     0x56000010: ('OF', '1', "First Order Phase Correction Angle", '', 'FirstOrderPhaseCorrectionAngle'),  # noqa
     0x56000020: ('OF', '1', "Spectroscopy Data", '', 'SpectroscopyData'),  # noqa
     0x7FE00001: ('OV', '1', "Extended Offset Table", '', 'ExtendedOffsetTable'),  # noqa
     0x7FE00002: ('OV', '1', "Extended Offset Table Lengths", '', 'ExtendedOffsetTableLengths'),  # noqa
+    0x7FE00003: ('UV', '1', "Encapsulated Pixel Data Value Total Length", '', 'EncapsulatedPixelDataValueTotalLength'),  # noqa
     0x7FE00008: ('OF', '1', "Float Pixel Data", '', 'FloatPixelData'),  # noqa
     0x7FE00009: ('OD', '1', "Double Float Pixel Data", '', 'DoubleFloatPixelData'),  # noqa
     0x7FE00010: ('OB or OW', '1', "Pixel Data", '', 'PixelData'),  # noqa
     0x7FE00020: ('OW', '1', "Coefficients SDVN", 'Retired', 'CoefficientsSDVN'),  # noqa
     0x7FE00030: ('OW', '1', "Coefficients SDHN", 'Retired', 'CoefficientsSDHN'),  # noqa
     0x7FE00040: ('OW', '1', "Coefficients SDDN", 'Retired', 'CoefficientsSDDN'),  # noqa
     0xFFFAFFFA: ('SQ', '1', "Digital Signatures Sequence", '', 'DigitalSignaturesSequence'),  # noqa
```

### Comparing `pydicom-2.3.1/pydicom/_private_dict.py` & `pydicom-2.4.0/pydicom/_private_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/_uid_dict.py` & `pydicom-2.4.0/pydicom/_uid_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,27 @@
     '1.2.840.10008.1.2.4.90': ('JPEG 2000 Image Compression (Lossless Only)', 'Transfer Syntax', '', '', 'JPEG2000Lossless'),  # noqa
     '1.2.840.10008.1.2.4.91': ('JPEG 2000 Image Compression', 'Transfer Syntax', '', '', 'JPEG2000'),  # noqa
     '1.2.840.10008.1.2.4.92': ('JPEG 2000 Part 2 Multi-component Image Compression (Lossless Only)', 'Transfer Syntax', '', '', 'JPEG2000MCLossless'),  # noqa
     '1.2.840.10008.1.2.4.93': ('JPEG 2000 Part 2 Multi-component Image Compression', 'Transfer Syntax', '', '', 'JPEG2000MC'),  # noqa
     '1.2.840.10008.1.2.4.94': ('JPIP Referenced', 'Transfer Syntax', '', '', 'JPIPReferenced'),  # noqa
     '1.2.840.10008.1.2.4.95': ('JPIP Referenced Deflate', 'Transfer Syntax', '', '', 'JPIPReferencedDeflate'),  # noqa
     '1.2.840.10008.1.2.4.100': ('MPEG2 Main Profile / Main Level', 'Transfer Syntax', '', '', 'MPEG2MPML'),  # noqa
+    '1.2.840.10008.1.2.4.100.1': ('Fragmentable MPEG2 Main Profile / Main Level', 'Transfer Syntax', '', '', 'MPEG2MPMLF'),  # noqa
     '1.2.840.10008.1.2.4.101': ('MPEG2 Main Profile / High Level', 'Transfer Syntax', '', '', 'MPEG2MPHL'),  # noqa
+    '1.2.840.10008.1.2.4.101.1': ('Fragmentable MPEG2 Main Profile / High Level', 'Transfer Syntax', '', '', 'MPEG2MPHLF'),  # noqa
     '1.2.840.10008.1.2.4.102': ('MPEG-4 AVC/H.264 High Profile / Level 4.1', 'Transfer Syntax', '', '', 'MPEG4HP41'),  # noqa
+    '1.2.840.10008.1.2.4.102.1': ('Fragmentable MPEG-4 AVC/H.264 High Profile / Level 4.1', 'Transfer Syntax', '', '', 'MPEG4HP41F'),  # noqa
     '1.2.840.10008.1.2.4.103': ('MPEG-4 AVC/H.264 BD-compatible High Profile / Level 4.1', 'Transfer Syntax', '', '', 'MPEG4HP41BD'),  # noqa
+    '1.2.840.10008.1.2.4.103.1': ('Fragmentable MPEG-4 AVC/H.264 BD-compatible High Profile / Level 4.1', 'Transfer Syntax', '', '', 'MPEG4HP41BDF'),  # noqa
     '1.2.840.10008.1.2.4.104': ('MPEG-4 AVC/H.264 High Profile / Level 4.2 For 2D Video', 'Transfer Syntax', '', '', 'MPEG4HP422D'),  # noqa
+    '1.2.840.10008.1.2.4.104.1': ('Fragmentable MPEG-4 AVC/H.264 High Profile / Level 4.2 For 2D Video', 'Transfer Syntax', '', '', 'MPEG4HP422DF'),  # noqa
     '1.2.840.10008.1.2.4.105': ('MPEG-4 AVC/H.264 High Profile / Level 4.2 For 3D Video', 'Transfer Syntax', '', '', 'MPEG4HP423D'),  # noqa
+    '1.2.840.10008.1.2.4.105.1': ('Fragmentable MPEG-4 AVC/H.264 High Profile / Level 4.2 For 3D Video', 'Transfer Syntax', '', '', 'MPEG4HP423DF'),  # noqa
     '1.2.840.10008.1.2.4.106': ('MPEG-4 AVC/H.264 Stereo High Profile / Level 4.2', 'Transfer Syntax', '', '', 'MPEG4HP42STEREO'),  # noqa
+    '1.2.840.10008.1.2.4.106.1': ('Fragmentable MPEG-4 AVC/H.264 Stereo High Profile / Level 4.2', 'Transfer Syntax', '', '', 'MPEG4HP42STEREOF'),  # noqa
     '1.2.840.10008.1.2.4.107': ('HEVC/H.265 Main Profile / Level 5.1', 'Transfer Syntax', '', '', 'HEVCMP51'),  # noqa
     '1.2.840.10008.1.2.4.108': ('HEVC/H.265 Main 10 Profile / Level 5.1', 'Transfer Syntax', '', '', 'HEVCM10P51'),  # noqa
     '1.2.840.10008.1.2.5': ('RLE Lossless', 'Transfer Syntax', '', '', 'RLELossless'),  # noqa
     '1.2.840.10008.1.2.6.1': ('RFC 2557 MIME encapsulation', 'Transfer Syntax', '', 'Retired', 'RFC2557MIMEEncapsulation'),  # noqa
     '1.2.840.10008.1.2.6.2': ('XML Encoding', 'Transfer Syntax', '', 'Retired', 'XMLEncoding'),  # noqa
     '1.2.840.10008.1.2.7.1': ('SMPTE ST 2110-20 Uncompressed Progressive Active Video', 'Transfer Syntax', '', '', 'SMPTEST211020UncompressedProgressiveActiveVideo'),  # noqa
     '1.2.840.10008.1.2.7.2': ('SMPTE ST 2110-20 Uncompressed Interlaced Active Video', 'Transfer Syntax', '', '', 'SMPTEST211020UncompressedInterlacedActiveVideo'),  # noqa
@@ -104,23 +111,23 @@
     '1.2.840.10008.5.1.1.4.2': ('Referenced Image Box SOP Class', 'SOP Class', '', 'Retired', 'ReferencedImageBox'),  # noqa
     '1.2.840.10008.5.1.1.9': ('Basic Grayscale Print Management Meta SOP Class', 'Meta SOP Class', '', '', 'BasicGrayscalePrintManagementMeta'),  # noqa
     '1.2.840.10008.5.1.1.9.1': ('Referenced Grayscale Print Management Meta SOP Class', 'Meta SOP Class', '', 'Retired', 'ReferencedGrayscalePrintManagementMeta'),  # noqa
     '1.2.840.10008.5.1.1.14': ('Print Job SOP Class', 'SOP Class', '', '', 'PrintJob'),  # noqa
     '1.2.840.10008.5.1.1.15': ('Basic Annotation Box SOP Class', 'SOP Class', '', '', 'BasicAnnotationBox'),  # noqa
     '1.2.840.10008.5.1.1.16': ('Printer SOP Class', 'SOP Class', '', '', 'Printer'),  # noqa
     '1.2.840.10008.5.1.1.16.376': ('Printer Configuration Retrieval SOP Class', 'SOP Class', '', '', 'PrinterConfigurationRetrieval'),  # noqa
-    '1.2.840.10008.5.1.1.17': ('Printer SOP Instance', 'Well-known Printer SOP Instance', '', '', 'PrinterInstance'),  # noqa
-    '1.2.840.10008.5.1.1.17.376': ('Printer Configuration Retrieval SOP Instance', 'Well-known Printer SOP Instance', '', '', 'PrinterConfigurationRetrievalInstance'),  # noqa
+    '1.2.840.10008.5.1.1.17': ('Printer SOP Instance', 'Well-known SOP Instance', '', '', 'PrinterInstance'),  # noqa
+    '1.2.840.10008.5.1.1.17.376': ('Printer Configuration Retrieval SOP Instance', 'Well-known SOP Instance', '', '', 'PrinterConfigurationRetrievalInstance'),  # noqa
     '1.2.840.10008.5.1.1.18': ('Basic Color Print Management Meta SOP Class', 'Meta SOP Class', '', '', 'BasicColorPrintManagementMeta'),  # noqa
     '1.2.840.10008.5.1.1.18.1': ('Referenced Color Print Management Meta SOP Class', 'Meta SOP Class', '', 'Retired', 'ReferencedColorPrintManagementMeta'),  # noqa
     '1.2.840.10008.5.1.1.22': ('VOI LUT Box SOP Class', 'SOP Class', '', '', 'VOILUTBox'),  # noqa
     '1.2.840.10008.5.1.1.23': ('Presentation LUT SOP Class', 'SOP Class', '', '', 'PresentationLUT'),  # noqa
     '1.2.840.10008.5.1.1.24': ('Image Overlay Box SOP Class', 'SOP Class', '', 'Retired', 'ImageOverlayBox'),  # noqa
     '1.2.840.10008.5.1.1.24.1': ('Basic Print Image Overlay Box SOP Class', 'SOP Class', '', 'Retired', 'BasicPrintImageOverlayBox'),  # noqa
-    '1.2.840.10008.5.1.1.25': ('Print Queue SOP Instance', 'Well-known Print Queue SOP Instance', '', 'Retired', 'PrintQueue'),  # noqa
+    '1.2.840.10008.5.1.1.25': ('Print Queue SOP Instance', 'Well-known SOP Instance', '', 'Retired', 'PrintQueueInstance'),  # noqa
     '1.2.840.10008.5.1.1.26': ('Print Queue Management SOP Class', 'SOP Class', '', 'Retired', 'PrintQueueManagement'),  # noqa
     '1.2.840.10008.5.1.1.27': ('Stored Print Storage SOP Class', 'SOP Class', '', 'Retired', 'StoredPrintStorage'),  # noqa
     '1.2.840.10008.5.1.1.29': ('Hardcopy Grayscale Image Storage SOP Class', 'SOP Class', '', 'Retired', 'HardcopyGrayscaleImageStorage'),  # noqa
     '1.2.840.10008.5.1.1.30': ('Hardcopy Color Image Storage SOP Class', 'SOP Class', '', 'Retired', 'HardcopyColorImageStorage'),  # noqa
     '1.2.840.10008.5.1.1.31': ('Pull Print Request SOP Class', 'SOP Class', '', 'Retired', 'PullPrintRequest'),  # noqa
     '1.2.840.10008.5.1.1.32': ('Pull Stored Print Management Meta SOP Class', 'Meta SOP Class', '', 'Retired', 'PullStoredPrintManagementMeta'),  # noqa
     '1.2.840.10008.5.1.1.33': ('Media Creation Management SOP Class UID', 'SOP Class', '', '', 'MediaCreationManagement'),  # noqa
@@ -179,14 +186,15 @@
     '1.2.840.10008.5.1.4.1.1.11.5': ('XA/XRF Grayscale Softcopy Presentation State Storage', 'SOP Class', '', '', 'XAXRFGrayscaleSoftcopyPresentationStateStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.11.6': ('Grayscale Planar MPR Volumetric Presentation State Storage', 'SOP Class', '', '', 'GrayscalePlanarMPRVolumetricPresentationStateStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.11.7': ('Compositing Planar MPR Volumetric Presentation State Storage', 'SOP Class', '', '', 'CompositingPlanarMPRVolumetricPresentationStateStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.11.8': ('Advanced Blending Presentation State Storage', 'SOP Class', '', '', 'AdvancedBlendingPresentationStateStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.11.9': ('Volume Rendering Volumetric Presentation State Storage', 'SOP Class', '', '', 'VolumeRenderingVolumetricPresentationStateStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.11.10': ('Segmented Volume Rendering Volumetric Presentation State Storage', 'SOP Class', '', '', 'SegmentedVolumeRenderingVolumetricPresentationStateStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.11.11': ('Multiple Volume Rendering Volumetric Presentation State Storage', 'SOP Class', '', '', 'MultipleVolumeRenderingVolumetricPresentationStateStorage'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.11.12': ('Variable Modality LUT Softcopy Presentation State Storage', 'SOP Class', '', '', 'VariableModalityLUTPresentationStateStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.12.1': ('X-Ray Angiographic Image Storage', 'SOP Class', '', '', 'XRayAngiographicImageStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.12.1.1': ('Enhanced XA Image Storage', 'SOP Class', '', '', 'EnhancedXAImageStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.12.2': ('X-Ray Radiofluoroscopic Image Storage', 'SOP Class', '', '', 'XRayRadiofluoroscopicImageStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.12.2.1': ('Enhanced XRF Image Storage', 'SOP Class', '', '', 'EnhancedXRFImageStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.12.3': ('X-Ray Angiographic Bi-Plane Image Storage', 'SOP Class', '', 'Retired', 'XRayAngiographicBiPlaneImageStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.12.77': ('', 'SOP Class', '(2015c)', 'Retired', ''),  # noqa
     '1.2.840.10008.5.1.4.1.1.13.1.1': ('X-Ray 3D Angiographic Image Storage', 'SOP Class', '', '', 'XRay3DAngiographicImageStorage'),  # noqa
@@ -279,14 +287,21 @@
     '1.2.840.10008.5.1.4.1.1.200.2': ('CT Performed Procedure Protocol Storage', 'SOP Class', '', '', 'CTPerformedProcedureProtocolStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.200.3': ('Protocol Approval Storage', 'SOP Class', '', '', 'ProtocolApprovalStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.200.4': ('Protocol Approval Information Model - FIND', 'SOP Class', '', '', 'ProtocolApprovalInformationModelFind'),  # noqa
     '1.2.840.10008.5.1.4.1.1.200.5': ('Protocol Approval Information Model - MOVE', 'SOP Class', '', '', 'ProtocolApprovalInformationModelMove'),  # noqa
     '1.2.840.10008.5.1.4.1.1.200.6': ('Protocol Approval Information Model - GET', 'SOP Class', '', '', 'ProtocolApprovalInformationModelGet'),  # noqa
     '1.2.840.10008.5.1.4.1.1.200.7': ('XA Defined Procedure Protocol Storage', 'SOP Class', '', '', 'XADefinedProcedureProtocolStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.200.8': ('XA Performed Procedure Protocol Storage', 'SOP Class', '', '', 'XAPerformedProcedureProtocolStorage'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.201.1': ('Inventory Storage', 'SOP Class', '', '', 'InventoryStorage'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.201.2': ('Inventory - FIND', 'SOP Class', '', '', 'InventoryFind'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.201.3': ('Inventory - MOVE', 'SOP Class', '', '', 'InventoryMove'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.201.4': ('Inventory - GET', 'SOP Class', '', '', 'InventoryGet'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.201.5': ('Inventory Creation', 'SOP Class', '', '', 'InventoryCreation'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.201.6': ('Repository Query', 'SOP Class', '', '', 'RepositoryQuery'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.201.1.1': ('Storage Management SOP Instance', 'Well-known SOP Instance', '', '', 'StorageManagementInstance'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.1': ('RT Image Storage', 'SOP Class', '', '', 'RTImageStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.2': ('RT Dose Storage', 'SOP Class', '', '', 'RTDoseStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.3': ('RT Structure Set Storage', 'SOP Class', '', '', 'RTStructureSetStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.4': ('RT Beams Treatment Record Storage', 'SOP Class', '', '', 'RTBeamsTreatmentRecordStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.5': ('RT Plan Storage', 'SOP Class', '', '', 'RTPlanStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.6': ('RT Brachy Treatment Record Storage', 'SOP Class', '', '', 'RTBrachyTreatmentRecordStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.7': ('RT Treatment Summary Record Storage', 'SOP Class', '', '', 'RTTreatmentSummaryRecordStorage'),  # noqa
@@ -301,14 +316,17 @@
     '1.2.840.10008.5.1.4.1.1.481.16': ('RT Radiation Record Set Storage', 'SOP Class', '', '', 'RTRadiationRecordSetStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.17': ('RT Radiation Salvage Record Storage', 'SOP Class', '', '', 'RTRadiationSalvageRecordStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.18': ('Tomotherapeutic Radiation Record Storage', 'SOP Class', '', '', 'TomotherapeuticRadiationRecordStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.19': ('C-Arm Photon-Electron Radiation Record Storage', 'SOP Class', '', '', 'CArmPhotonElectronRadiationRecordStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.20': ('Robotic Radiation Record Storage', 'SOP Class', '', '', 'RoboticRadiationRecordStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.21': ('RT Radiation Set Delivery Instruction Storage', 'SOP Class', '', '', 'RTRadiationSetDeliveryInstructionStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.481.22': ('RT Treatment Preparation Storage', 'SOP Class', '', '', 'RTTreatmentPreparationStorage'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.481.23': ('Enhanced RT Image Storage', 'SOP Class', '', '', 'EnhancedRTImageStorage'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.481.24': ('Enhanced Continuous RT Image Storage', 'SOP Class', '', '', 'EnhancedContinuousRTImageStorage'),  # noqa
+    '1.2.840.10008.5.1.4.1.1.481.25': ('RT Patient Position Acquisition Instruction Storage', 'SOP Class', '', '', 'RTPatientPositionAcquisitionInstructionStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.501.1': ('DICOS CT Image Storage', 'SOP Class', 'DICOS', '', 'DICOSCTImageStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.501.2.1': ('DICOS Digital X-Ray Image Storage - For Presentation', 'SOP Class', 'DICOS', '', 'DICOSDigitalXRayImageStorageForPresentation'),  # noqa
     '1.2.840.10008.5.1.4.1.1.501.2.2': ('DICOS Digital X-Ray Image Storage - For Processing', 'SOP Class', 'DICOS', '', 'DICOSDigitalXRayImageStorageForProcessing'),  # noqa
     '1.2.840.10008.5.1.4.1.1.501.3': ('DICOS Threat Detection Report Storage', 'SOP Class', 'DICOS', '', 'DICOSThreatDetectionReportStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.501.4': ('DICOS 2D AIT Storage', 'SOP Class', 'DICOS', '', 'DICOS2DAITStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.501.5': ('DICOS 3D AIT Storage', 'SOP Class', 'DICOS', '', 'DICOS3DAITStorage'),  # noqa
     '1.2.840.10008.5.1.4.1.1.501.6': ('DICOS Quadrupole Resonance (QR) Storage', 'SOP Class', 'DICOS', '', 'DICOSQuadrupoleResonanceStorage'),  # noqa
```

### Comparing `pydicom-2.3.1/pydicom/benchmarks/bench_encaps.py` & `pydicom-2.4.0/benchmarks/bench_encaps.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/benchmarks/bench_handler_numpy.py` & `pydicom-2.4.0/benchmarks/bench_handler_numpy.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/benchmarks/bench_pixel_util.py` & `pydicom-2.4.0/benchmarks/bench_pixel_util.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/benchmarks/bench_rle_decode.py` & `pydicom-2.4.0/benchmarks/bench_rle_decode.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/benchmarks/bench_rle_encode.py` & `pydicom-2.4.0/benchmarks/bench_rle_encode.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/charset.py` & `pydicom-2.4.0/pydicom/charset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/cli/codify.py` & `pydicom-2.4.0/pydicom/cli/codify.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/cli/main.py` & `pydicom-2.4.0/pydicom/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 attributes, and calls set_defaults(func=callback_function)
 
 """
 
 import argparse
 import pkg_resources
 import re
+import sys
 from typing import Tuple, cast, List, Any, Dict, Optional, Callable
 
 from pydicom import dcmread
-from pydicom.data.data_manager import get_testdata_file
+from pydicom.data.data_manager import get_charset_files, get_testdata_file
 from pydicom.dataset import Dataset
 
 
 subparsers: Optional[argparse._SubParsersAction] = None
 
 
 # Restrict the allowed syntax tightly, since use Python `eval`
@@ -128,14 +129,22 @@
 
     # Get the pydicom test filename even without prefix, in case user forgot it
     try:
         pydicom_filename = cast(str, get_testdata_file(filename))
     except NotImplementedError:  # will get this if absolute path passed
         pydicom_filename = ""
 
+    # Check if filename is in charset files
+    if not pydicom_filename:
+        try:
+            char_filenames = get_charset_files(filename)
+            pydicom_filename = char_filenames[0]
+        except NotImplementedError:  # will get this if absolute path passed
+            pass
+
     if prefix == "pydicom":
         filename = pydicom_filename
 
     # Check element syntax first to avoid unnecessary load of file
     if element and not re_file_spec_object.match(element):
         raise argparse.ArgumentTypeError(
             f"Component '{element}' is not valid syntax for a "
@@ -197,16 +206,19 @@
     ----------
     args : List[str], optional
         Command-line arguments to parse.  If ``None``, then :attr:`sys.argv`
         is used.
     """
     global subparsers
 
+    py_version = sys.version.split()[0]
+
     parser = argparse.ArgumentParser(
-        prog="pydicom", description="pydicom command line utilities"
+        prog="pydicom",
+        description=f"pydicom command line utilities (Python {py_version})"
     )
     subparsers = parser.add_subparsers(help="subcommand help")
 
     help_parser = subparsers.add_parser(
         "help", help="display help for subcommands"
     )
     help_parser.add_argument(
```

### Comparing `pydicom-2.3.1/pydicom/cli/show.py` & `pydicom-2.4.0/pydicom/cli/show.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/compat.py` & `pydicom-2.4.0/pydicom/compat.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/config.py` & `pydicom-2.4.0/pydicom/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,14 +264,26 @@
         settings.writing_validation_mode = IGNORE
         yield
     finally:
         settings._reading_validation_mode = reading_mode
         settings._writing_validation_mode = writing_mode
 
 
+@contextmanager
+def strict_reading() -> Generator:
+    """Context manager to temporarily enably strict value validation
+    for reading."""
+    original_reading_mode = settings._reading_validation_mode
+    try:
+        settings.reading_validation_mode = RAISE
+        yield
+    finally:
+        settings._reading_validation_mode = original_reading_mode
+
+
 convert_wrong_length_to_UN = False
 """Convert a field VR to "UN" and return bytes if bytes length is invalid.
 Default ``False``.
 """
 
 datetime_conversion = False
 """Set to ``True`` to convert the value(s) of elements with a VR of DA, DT and
```

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/FileInfo.txt` & `pydicom-2.4.0/pydicom/data/charset_files/FileInfo.txt`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrArab.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrArab.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrFren.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrFren.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrFrenMulti.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrFrenMulti.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrGerm.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrGerm.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrGreek.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrGreek.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrH31.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrH31.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrH32.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrH32.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrHbrw.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrHbrw.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrI2.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrI2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrJapMulti.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrJapMulti.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrKoreanMulti.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrKoreanMulti.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrRuss.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrRuss.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrSQEncoding.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrSQEncoding1.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding1.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrX1.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrX1.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/charset_files/chrX2.dcm` & `pydicom-2.4.0/pydicom/data/charset_files/chrX2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/data_manager.py` & `pydicom-2.4.0/pydicom/data/data_manager.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/download.py` & `pydicom-2.4.0/pydicom/data/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     if HAVE_REQUESTS:
         if USE_PROGRESS_BAR:
             r = requests.get(url, stream=True)
             total_size_in_bytes = int(r.headers.get("content-length", 0))
             with open(fpath, "wb") as file:
                 for data in tqdm.tqdm(
-                    r.iter_content(), total=total_size_in_bytes,
+                    r.iter_content(chunk_size=4096), total=total_size_in_bytes,
                     unit="B", unit_scale=True, miniters=1,
                     desc=url.split("/")[-1]
                 ):
                     file.write(data)
         else:
             r = requests.get(url)
             with open(filename, "wb") as f:
```

### Comparing `pydicom-2.3.1/pydicom/data/hashes.json` & `pydicom-2.4.0/pydicom/data/hashes.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852941176470589%*

 * *Differences: {"'OBXXXX1A_expb.dcm'": "'0cf6b4b04a1f239755fe9aef2b093b3004a290c262ec2567f555212d6c679c83'",*

 * * "'OBXXXX1A_expb_2frame.dcm'": "'2ccd16a61d680e85ad82fe1d60c4c50496a91309aa2fd27157fc9660291d6ba5'"}*

```diff
@@ -8,16 +8,16 @@
     "MR-SIEMENS-DICOM-WithOverlays.dcm": "094faf56c63bff84c30567e29de0c67d7c5a8ae05cf880ac12175491b6b645d2",
     "MR2_J2KI.dcm": "8319846e6ad6dc70dbbaf61748b1987a6807fd02db3da24e7989fd5a5ce19e4e",
     "MR2_J2KR.dcm": "707f0a1b648b79f17b61e241af31fb9edea7fe596681a4bcab6cce890300a9a5",
     "MR2_UNCI.dcm": "7f79ac33e1ab32e1a8ca10ce62f18e5a2372e78c8a6684af17302b1a0171fc46",
     "MR2_UNCR.dcm": "c14c7f0c6e25bd4dfbb822fe264e540fc7142bf1c9d15d4c652ec8f5f97fa9e8",
     "OBXXXX1A.dcm": "164a460bebdc15fbe391ad4bfe4c84672eb2bad57adfe7dad372fd7367b0f63e",
     "OBXXXX1A_2frame.dcm": "6627f6e46dbf8c16292fb1eaff8807439bcd233dc68099c07f0b83c4093256b1",
-    "OBXXXX1A_expb.dcm": "668dc27f6db2c7d47d7384dbb86593cc8f681a44fca3bb93201913d5cd6463e2",
-    "OBXXXX1A_expb_2frame.dcm": "b27a5e056d005525d28fdabfebc061ef64cc3d652c835d062f4f5d31d2bf453b",
+    "OBXXXX1A_expb.dcm": "0cf6b4b04a1f239755fe9aef2b093b3004a290c262ec2567f555212d6c679c83",
+    "OBXXXX1A_expb_2frame.dcm": "2ccd16a61d680e85ad82fe1d60c4c50496a91309aa2fd27157fc9660291d6ba5",
     "OBXXXX1A_rle.dcm": "aaf57785817dbe35503c6175d677d2efa811f90e931fc5017611ba9ff4c7f92a",
     "OBXXXX1A_rle_2frame.dcm": "65bee869c507f535edea93a446a26e941fb9cbc3819e4d73395f11eef56d4687",
     "OT-PAL-8-face.dcm": "d5560470077f77ef6a0a52d22f9f61e803436d2b468a9550a4d12c5675ee0a97",
     "RG1_J2KI.dcm": "744d01372fdda4e21b507bb7f97329065de961f4f263342079b369b430064d65",
     "RG1_J2KR.dcm": "7fbfd29360af806770102fd7c4ffcb2a133075bd00920a4bb63460d516f67ac4",
     "RG1_UNCI.dcm": "3561020824868615a93a51078671b3ff73bb2578c966f76def99b4d982897e75",
     "RG1_UNCR.dcm": "946f28f48b9fbf360196a9b835c8fce83b0c654bf85a5107663c8a61df02e498",
```

### Comparing `pydicom-2.3.1/pydicom/data/palettes/README.md` & `pydicom-2.4.0/pydicom/data/palettes/README.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/fall.dcm` & `pydicom-2.4.0/pydicom/data/palettes/fall.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/hotiron.dcm` & `pydicom-2.4.0/pydicom/data/palettes/hotiron.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/hotmetalblue.dcm` & `pydicom-2.4.0/pydicom/data/palettes/hotmetalblue.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/pet.dcm` & `pydicom-2.4.0/pydicom/data/palettes/pet.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/pet20step.dcm` & `pydicom-2.4.0/pydicom/data/palettes/pet20step.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/spring.dcm` & `pydicom-2.4.0/pydicom/data/palettes/spring.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/summer.dcm` & `pydicom-2.4.0/pydicom/data/palettes/summer.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/palettes/winter.dcm` & `pydicom-2.4.0/pydicom/data/palettes/winter.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/retry.py` & `pydicom-2.4.0/pydicom/data/retry.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/693_J2KI.dcm` & `pydicom-2.4.0/pydicom/data/test_files/693_J2KI.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/CT_small.dcm` & `pydicom-2.4.0/pydicom/data/test_files/CT_small.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/ExplVR_BigEnd.dcm` & `pydicom-2.4.0/pydicom/data/test_files/ExplVR_BigEnd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm` & `pydicom-2.4.0/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm` & `pydicom-2.4.0/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/JPEG-lossy.dcm` & `pydicom-2.4.0/pydicom/data/test_files/JPEG-lossy.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm` & `pydicom-2.4.0/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/JPEG2000.dcm` & `pydicom-2.4.0/pydicom/data/test_files/JPEG2000.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/JPGExtended.dcm` & `pydicom-2.4.0/pydicom/data/test_files/JPGExtended.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small_RLE.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small_RLE.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small_bigendian.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small_bigendian.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small_expb.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small_expb.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small_implicit.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small_implicit.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small_jp2klossless.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small_jp2klossless.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_small_padded.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_small_padded.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/MR_truncated.dcm` & `pydicom-2.4.0/pydicom/data/test_files/MR_truncated.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/README.txt` & `pydicom-2.4.0/pydicom/data/test_files/README.txt`

 * *Files 1% similar despite different names*

```diff
@@ -179,16 +179,15 @@
   * minimal data elements kept from example files in issues 91, 97, 98
 
 OBXXXX1A.dcm
   * a file with a Photometric Interpretation of PALETTE COLOR
   * used to check if to pixel_array is interpreted correctly for such a case
   * taken from https://github.com/pydicom/pydicom/issues/205#issuecomment-103329677
   * supposedly from a Philips machine
-  * Explicit VR big endian version created using DCMTK's dcmconv and the
-    pixel data corrected using script for PR #714
+  * Explicit VR big endian version created using DCMTK's dcmconv
   * 2 frame version created using a script for PR #714
   * RLE encoded versions created using GDCM's gdcmconv for PR #708
 
 OT-PAL-8-face.dcm
   * a file with a Photometric Interpretation of PALETTE COLOR
   * used to check if to pixel_array is interpreted correctly for such a case
   * taken from http://www.barre.nom.fr/medical/samples/
@@ -199,20 +198,24 @@
   * From ftp://medical.nema.org/MEDICAL/Dicom/DataSets/WG04
 
 RG3_*.dcm
   * JPEG2000, JPEG2000Lossless and uncompressed versions
   * unsigned 16-bit/10-bit with windowing
   * From ftp://medical.nema.org/MEDICAL/Dicom/DataSets/WG04
 
-SC_rgb.dcm
+SC_rgb*.dcm
   * 16 and 32 bit versions created using a script for PR #714
   * Explicit VR big endian version created using DCMTK's dcmconv and the
     pixel data corrected using script for PR #714
   * 2 frame versions created using a script for PR #714
   * RLE encoded versions created using GDCM's gdcmconv for PR #708
+  
+SC_rgb_small_odd*.dcm
+  * 3x3 pixel version added for PR #601
+  * Big Endian version added for PR #1687
 
 SC_jpeg_no_color_transform.dcm
   * 8-bit baseline JPEG compressed in RGB color space without transformation
     into YCbCr color space
   * Individual tile of a TCGA whole slide image in Aperio SVS format obtained
     from TCIA
   * Created for PR #878 using DCMTK's img2cdm script with the value of the
```

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_16bit.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_2frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_2frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_32bit.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_small_odd.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm` & `pydicom-2.4.0/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/UN_sequence.dcm` & `pydicom-2.4.0/pydicom/data/test_files/UN_sequence.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/badVR.dcm` & `pydicom-2.4.0/pydicom/data/test_files/badVR.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/README.txt` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/README.txt`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README` & `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/image_dfl.dcm` & `pydicom-2.4.0/pydicom/data/test_files/image_dfl.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/liver_1frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/liver_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/liver_expb_1frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/liver_expb_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/no_meta.dcm` & `pydicom-2.4.0/pydicom/data/test_files/no_meta.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/priv_SQ.dcm` & `pydicom-2.4.0/pydicom/data/test_files/priv_SQ.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/reportsi.dcm` & `pydicom-2.4.0/pydicom/data/test_files/reportsi.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm` & `pydicom-2.4.0/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtdose.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtdose.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtdose_1frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtdose_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtdose_expb.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtdose_expb.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtdose_expb_1frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtdose_expb_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtdose_rle.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtdose_rle.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtdose_rle_1frame.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtdose_rle_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtplan.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtplan.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtplan.dump` & `pydicom-2.4.0/pydicom/data/test_files/rtplan.dump`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtplan_truncated.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtplan_truncated.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtstruct.dcm` & `pydicom-2.4.0/pydicom/data/test_files/rtstruct.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/rtstruct.dump` & `pydicom-2.4.0/pydicom/data/test_files/rtstruct.dump`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/test-SR.dcm` & `pydicom-2.4.0/pydicom/data/test_files/test-SR.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/test1.json` & `pydicom-2.4.0/pydicom/data/test_files/test1.json`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/test_PN.json` & `pydicom-2.4.0/pydicom/data/test_files/test_PN.json`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/waveform_ecg.dcm` & `pydicom-2.4.0/pydicom/data/test_files/waveform_ecg.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/test_files/zipMR.gz` & `pydicom-2.4.0/pydicom/data/test_files/zipMR.gz`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/data/urls.json` & `pydicom-2.4.0/pydicom/data/urls.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852941176470589%*

 * *Differences: {"'OBXXXX1A_expb.dcm'": "'https://github.com/pydicom/pydicom-data/raw/ce9de30a2c871f3949d5a90957753b30a29e7293/data_store/data/OBXXXX1A_expb.dcm'",*

 * * "'OBXXXX1A_expb_2frame.dcm'": "'https://github.com/pydicom/pydicom-data/raw/ce9de30a2c871f3949d5a90957753b30a29e7293/data_store/data/OBXXXX1A_expb_2frame.dcm'"}*

```diff
@@ -8,16 +8,16 @@
     "MR-SIEMENS-DICOM-WithOverlays.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/MR-SIEMENS-DICOM-WithOverlays.dcm",
     "MR2_J2KI.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/MR2_J2KI.dcm",
     "MR2_J2KR.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/MR2_J2KR.dcm",
     "MR2_UNCI.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/MR2_UNCI.dcm",
     "MR2_UNCR.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/MR2_UNCR.dcm",
     "OBXXXX1A.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/OBXXXX1A.dcm",
     "OBXXXX1A_2frame.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/OBXXXX1A_2frame.dcm",
-    "OBXXXX1A_expb.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/OBXXXX1A_expb.dcm",
-    "OBXXXX1A_expb_2frame.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/OBXXXX1A_expb_2frame.dcm",
+    "OBXXXX1A_expb.dcm": "https://github.com/pydicom/pydicom-data/raw/ce9de30a2c871f3949d5a90957753b30a29e7293/data_store/data/OBXXXX1A_expb.dcm",
+    "OBXXXX1A_expb_2frame.dcm": "https://github.com/pydicom/pydicom-data/raw/ce9de30a2c871f3949d5a90957753b30a29e7293/data_store/data/OBXXXX1A_expb_2frame.dcm",
     "OBXXXX1A_rle.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/OBXXXX1A_rle.dcm",
     "OBXXXX1A_rle_2frame.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/OBXXXX1A_rle_2frame.dcm",
     "OT-PAL-8-face.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/OT-PAL-8-face.dcm",
     "RG1_J2KI.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/RG1_J2KI.dcm",
     "RG1_J2KR.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/RG1_J2KR.dcm",
     "RG1_UNCI.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/RG1_UNCI.dcm",
     "RG1_UNCR.dcm": "https://github.com/pydicom/pydicom-data/raw/39a2eb31815eec435dc26c322c27aec5cfcbddb6/data/RG1_UNCR.dcm",
```

### Comparing `pydicom-2.3.1/pydicom/datadict.py` & `pydicom-2.4.0/pydicom/datadict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2008-2018 pydicom authors. See LICENSE file for details.
 # -*- coding: utf-8 -*-
 """Access dicom dictionary information"""
-
+import warnings
 from typing import Tuple, Optional, Dict
 
 from pydicom.config import logger
 from pydicom.tag import Tag, BaseTag, TagType
 
 # the actual dict of {tag: (VR, VM, name, is_retired, keyword), ...}
 from pydicom._dicom_dict import DicomDictionary
@@ -549,14 +549,19 @@
     try:
         private_dict = private_dictionaries[private_creator]
     except KeyError as exc:
         raise KeyError(
             f"Private creator '{private_creator}' not in the private "
             "dictionary"
         ) from exc
+    except TypeError as exc:
+        msg = (f"{tag.private_creator} '{private_creator}' "
+               f"is not a valid private creator")
+        warnings.warn(msg)
+        raise KeyError(msg) from exc
 
     # private elements are usually agnostic for
     # "block" (see PS3.5-2008 7.8.1 p44)
     # Some elements in _private_dict are explicit;
     # most have "xx" for high-byte of element
     #  so here put in the "xx" in the block position for key to look up
     group_str = f"{tag.group:04x}"
@@ -630,20 +635,21 @@
 
     Parameters
     ----------
     tag : int or str or Tuple[int, int]
         The tag for the element whose description is being retrieved, in any
         of the forms accepted by :func:`~pydicom.tag.Tag`.
     private_creator : str
-        The name of the private createor.
+        The name of the private creator.
 
     Returns
     -------
     str
         The description of the corresponding element.
 
     Raises
     ------
     KeyError
-        If the tag is not present in the private dictionary.
+        If the tag is not present in the private dictionary,
+        or if the private creator is not valid.
     """
     return get_private_entry(tag, private_creator)[2]
```

### Comparing `pydicom-2.3.1/pydicom/dataelem.py` & `pydicom-2.4.0/pydicom/dataelem.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,17 +646,17 @@
               in the format ``'[name]'``.
             * For unknown private elements this will be ``'Private tag data'``.
             * Otherwise returns an empty string ``''``.
         """
         if self.tag.is_private:
             if self.private_creator:
                 try:
-                    # If have name from private dictionary, use it, but
-                    #   but put in square brackets so is differentiated,
-                    #   and clear that cannot access it by name
+                    # If we have the name from the private dictionary, use it,
+                    # but put it in square brackets to make clear
+                    # that the tag cannot be accessed by that name
                     name = private_dictionary_description(
                         self.tag, self.private_creator
                     )
                     return f"[{name}]"
                 except KeyError:
                     pass
             elif self.tag.element >> 8 == 0:
```

### Comparing `pydicom-2.3.1/pydicom/dataset.py` & `pydicom-2.4.0/pydicom/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,28 @@
         * A single value, such as a number, string, etc. (i.e. VM = 1)
         * A list of numbers, strings, etc. (i.e. VM > 1)
         * A Sequence (list subclass), where each item is a Dataset which
             contains its own DataElements, and so on in a recursive manner.
 """
 import copy
 from bisect import bisect_left
+from contextlib import nullcontext
 import io
 from importlib.util import find_spec as have_package
 import inspect  # for __dir__
 from itertools import takewhile
 import json
 import os
 import os.path
 import re
 from types import TracebackType
 from typing import (
     Optional, Tuple, Union, List, Any, cast, Dict, ValuesView,
     Iterator, BinaryIO, AnyStr, Callable, TypeVar, Type, overload,
-    MutableSequence, MutableMapping, AbstractSet
+    MutableSequence, MutableMapping, AbstractSet, TYPE_CHECKING
 )
 import warnings
 import weakref
 
 from pydicom.filebase import DicomFileLike
 
 try:
@@ -59,14 +60,18 @@
     ExplicitVRLittleEndian, ImplicitVRLittleEndian, ExplicitVRBigEndian,
     RLELossless, PYDICOM_IMPLEMENTATION_UID, UID
 )
 from pydicom.valuerep import VR as VR_, AMBIGUOUS_VR
 from pydicom.waveforms import numpy_handler as wave_handler
 
 
+if TYPE_CHECKING:  # pragma: no cover
+    from pydicom.sequence import Sequence
+
+
 class PrivateBlock:
     """Helper class for a private block in the :class:`Dataset`.
 
     .. versionadded:: 1.3
 
     See the DICOM Standard, Part 5,
     :dcm:`Section 7.8.1<part05/sect_7.8.html#sect_7.8.1>` - Private Data
@@ -393,24 +398,92 @@
         self.is_little_endian: Optional[bool] = None
         self.is_implicit_VR: Optional[bool] = None
 
         # True if the dataset is a sequence item with undefined length
         self.is_undefined_length_sequence_item = False
 
         # the parent data set, if this dataset is a sequence item
-        self.parent: "Optional[weakref.ReferenceType[Dataset]]" = None
+        self._parent_seq: "Optional[weakref.ReferenceType[Sequence]]" = None
 
         # known private creator blocks
         self._private_blocks: Dict[Tuple[int, str], PrivateBlock] = {}
 
         self._pixel_array: Optional["numpy.ndarray"] = None
         self._pixel_id: Dict[str, int] = {}
 
         self.file_meta: FileMetaDataset
 
+    @property
+    def parent_seq(self) -> "Optional[weakref.ReferenceType[Sequence]]":
+        """Return a weak reference to the parent
+        :class:`~pydicom.sequence.Sequence`.
+
+        .. versionadded:: 2.4
+
+            Returned value is a weak reference to the parent ``Sequence``.
+        """
+        return self._parent_seq
+
+    @parent_seq.setter
+    def parent_seq(self, value: "Sequence") -> None:
+        """Set the parent :class:`~pydicom.sequence.Sequence`
+
+        .. versionadded:: 2.4
+        """
+        if value != self._parent_seq:
+            self._parent_seq = weakref.ref(value)
+
+    @property
+    def parent(self) -> "Optional[weakref.ReferenceType[Dataset]]":
+        """Return a weak reference to the parent Sequence's
+        parent Dataset.
+
+        .. deprecated:: 2.4
+        """
+        if config._use_future:
+            raise AttributeError("Future: Dataset.parent is removed in v3.x")
+        else:
+            warnings.warn(
+                "Dataset.parent will be removed in pydicom 3.0",
+                DeprecationWarning
+            )
+
+            parent_ref = self.parent_seq
+            if parent_ref is None:
+                return None
+
+            return cast("Sequence", parent_ref()).parent_dataset
+
+    @parent.setter
+    def parent(self, value: "Dataset") -> None:
+        """Set the parent :class:`~pydicom.sequence.Sequence`
+
+        .. deprecated:: 2.4
+        """
+        if config._use_future:
+            raise AttributeError("Future: Dataset.parent is removed in v3.x")
+        else:
+            warnings.warn(
+                "Dataset.parent will be removed in pydicom 3.0",
+                DeprecationWarning
+            )
+        self._parent = weakref.ref(value)
+
+    def __deepcopy__(self, memo: Optional[Dict[int, Any]]) -> "Dataset":
+        copied = Dataset()
+        if memo:
+            memo[id(self)] = copied   # add the new class to the memo
+        # Insert a deepcopy of all instance attributes
+        copied.__dict__.update(copy.deepcopy(self.__dict__, memo))
+        # Manually update the weakref to be correct
+        for elem in copied:  # DICOM elements
+            if elem.VR == VR_.SQ:
+                elem.value.parent_dataset = copied  # setter does weakref
+        return copied
+
     def __enter__(self) -> "Dataset":
         """Method invoked on entry to a with statement."""
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
@@ -817,17 +890,17 @@
         -------
         value
               If `name` matches a DICOM keyword, returns the corresponding
               element's value. Otherwise returns the class attribute's
               value (if present).
         """
         tag = tag_for_keyword(name)
-        if tag is not None:  # `name` isn't a DICOM element keyword
+        if tag is not None:  # None means `name` isn't a DICOM element keyword
             tag = Tag(tag)
-            if tag in self._dict:  # DICOM DataElement not in the Dataset
+            if tag in self._dict:
                 return self[tag].value
 
         # no tag or tag not contained in the dataset
         if name == '_dict':
             # special handling for contained dict, needed for pickle
             return {}
         # Try the base class attribute getter (fix for issue 332)
@@ -908,20 +981,14 @@
         else:
             try:
                 tag = Tag(key)
             except Exception as exc:
                 raise KeyError(f"'{key}'") from exc
 
         elem = self._dict[tag]
-        if isinstance(elem, DataElement):
-            if elem.VR == VR_.SQ and elem.value:
-                # let a sequence know its parent dataset, as sequence items
-                # may need parent dataset tags to resolve ambiguous tags
-                elem.value.parent = self
-            return elem
 
         if isinstance(elem, RawDataElement):
             # If a deferred read, then go get the value now
             if elem.value is None and elem.length != 0:
                 from pydicom.filereader import read_deferred_data_element
 
                 elem = read_deferred_data_element(
@@ -2115,14 +2182,24 @@
         name : str
             The keyword for the element you wish to add/change. If
             `name` is not a DICOM element keyword then this will be the
             name of the attribute to be added/changed.
         value
             The value for the attribute to be added/changed.
         """
+        # Save time for common Dataset attributes that are not DICOM keywords
+        # This check is fast if `name` is a DICOM keyword (first chr is upper)
+        # The startswith is needed for `is_implicit_VR`
+        if name.startswith("is_") or name.islower():
+            if name == "file_meta":
+                self._set_file_meta(value)
+            else:
+                object.__setattr__(self, name, value)
+            return
+
         tag = tag_for_keyword(name)
         if tag is not None:  # successfully mapped name to a tag
             if tag not in self:
                 # don't have this tag yet->create the data_element instance
                 vr = dictionary_VR(tag)
                 data_element = DataElement(tag, vr, value)
                 if vr == VR_.SQ:
@@ -2138,16 +2215,14 @@
             self[tag] = data_element
         elif repeater_has_keyword(name):
             # Check if `name` is repeaters element
             raise ValueError(
                 f"'{name}' is a DICOM repeating group element and must be "
                 "added using the add() or add_new() methods."
             )
-        elif name == "file_meta":
-            self._set_file_meta(value)
         else:
             # Warn if `name` is camel case but not a keyword
             if _RE_CAMEL_CASE.match(name):
                 msg = (
                     f"Camel case attribute '{name}' used which is not in the "
                     "element keyword data dictionary"
                 )
@@ -2234,14 +2309,22 @@
                     elem = DataElement_from_raw(
                         elem, self._character_set, self
                     )
                 elem.private_creator = self[private_creator_tag].value
 
         self._dict[elem_tag] = elem
 
+        if elem.VR == VR_.SQ and isinstance(elem, DataElement):
+            if not isinstance(elem.value, pydicom.Sequence):
+                elem.value = pydicom.Sequence(elem.value)  # type: ignore
+            if elem.value is not None:
+                # let a sequence know its parent dataset, as sequence items
+                # may need parent dataset tags to resolve ambiguous tags
+                elem.value.parent_dataset = self  # type:ignore
+
     def _slice_dataset(
         self,
         start: Optional[TagType],
         stop: Optional[TagType],
         step: Optional[int]
     ) -> List[BaseTag]:
         """Return the element tags in the Dataset that match the slice.
@@ -2486,26 +2569,31 @@
 
         Returns
         -------
         dict
             :class:`Dataset` representation based on the DICOM JSON Model.
         """
         json_dataset = {}
-        for key in self.keys():
-            json_key = '{:08X}'.format(key)
-            data_element = self[key]
-            try:
-                json_dataset[json_key] = data_element.to_json_dict(
-                    bulk_data_element_handler=bulk_data_element_handler,
-                    bulk_data_threshold=bulk_data_threshold
-                )
-            except Exception as exc:
-                logger.error(f"Error while processing tag {json_key}")
-                if not suppress_invalid_tags:
-                    raise exc
+        context = (
+            config.strict_reading() if suppress_invalid_tags
+            else nullcontext()
+        )
+        with context:
+            for key in self.keys():
+                json_key = '{:08X}'.format(key)
+                try:
+                    data_element = self[key]
+                    json_dataset[json_key] = data_element.to_json_dict(
+                        bulk_data_element_handler=bulk_data_element_handler,
+                        bulk_data_threshold=bulk_data_threshold
+                    )
+                except Exception as exc:
+                    logger.error(f"Error while processing tag {json_key}")
+                    if not suppress_invalid_tags:
+                        raise exc
 
         return json_dataset
 
     def to_json(
         self,
         bulk_data_threshold: int = 1024,
         bulk_data_element_handler: Optional[Callable[[DataElement], str]] = None,  # noqa
@@ -2564,25 +2652,30 @@
             self.to_json_dict(
                 bulk_data_threshold,
                 bulk_data_element_handler,
                 suppress_invalid_tags=suppress_invalid_tags
             )
         )
 
+    # For Pickle, need to make weakref a strong reference
+    # Adapted from https://stackoverflow.com/a/45588812/1987276
     def __getstate__(self) -> Dict[str, Any]:
-        # pickle cannot handle weakref - remove parent
-        d = self.__dict__.copy()
-        del d['parent']
-        return d
+        if self.parent_seq is not None:
+            s = self.__dict__.copy()
+            s['_parent_seq'] = s['_parent_seq']()
+            return s
+        return self.__dict__
 
+    # If recovering from a pickle, turn back into weak ref
     def __setstate__(self, state: Dict[str, Any]) -> None:
         self.__dict__.update(state)
-        # re-add parent - it will be set to the parent dataset on demand
-        # if the dataset is in a sequence
-        self.__dict__['parent'] = None
+        if self.__dict__['_parent_seq'] is not None:
+            self.__dict__['_parent_seq'] = weakref.ref(
+                self.__dict__['_parent_seq']
+            )
 
     __repr__ = __str__
 
 
 _FileDataset = TypeVar("_FileDataset", bound="FileDataset")
```

### Comparing `pydicom-2.3.1/pydicom/dicomdir.py` & `pydicom-2.4.0/pydicom/dicomdir.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/encaps.py` & `pydicom-2.4.0/pydicom/encaps.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/encoders/base.py` & `pydicom-2.4.0/pydicom/encoders/base.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/encoders/gdcm.py` & `pydicom-2.4.0/pydicom/encoders/gdcm.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/encoders/native.py` & `pydicom-2.4.0/pydicom/encoders/native.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/encoders/pylibjpeg.py` & `pydicom-2.4.0/pydicom/encoders/pylibjpeg.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/env_info.py` & `pydicom-2.4.0/pydicom/env_info.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/errors.py` & `pydicom-2.4.0/pydicom/errors.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/filebase.py` & `pydicom-2.4.0/pydicom/filebase.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/filereader.py` & `pydicom-2.4.0/pydicom/filereader.py`

 * *Files 2% similar despite different names*

```diff
@@ -865,21 +865,30 @@
     # Add the command set elements to the dataset (if any)
     dataset.update(command_set)
 
     # (0002, 0002) Media Storage SOP Class UID
     elem = file_meta.get(0x00020002, None)
     sop_class = elem.value.name if (elem and elem.VM == 1) else ""
     if sop_class == "Media Storage Directory Storage":
-        warnings.warn(
-            "The 'DicomDir' class is deprecated and will be removed in v3.0, "
-            "after which 'dcmread()' will return a normal 'FileDataset' "
-            "instance for 'Media Storage Directory' SOP Instances.",
-            DeprecationWarning
-        )
-        ds_class: Union[Type[FileDataset], Type[DicomDir]] = DicomDir
+        if "DirectoryRecordSequence" not in dataset:
+            warnings.warn(
+                "The SOP Class 'Media Storage Directory Storage' does"
+                "not match the contents of the dataset - handling it"
+                "as a regular dataset instead of a DICOMDIR."
+            )
+            ds_class: Union[Type[FileDataset], Type[DicomDir]] = FileDataset
+        else:
+            warnings.warn(
+                "The 'DicomDir' class is deprecated and will be removed in"
+                " v3.0, after which 'dcmread()' will return a normal "
+                "'FileDataset' instance for 'Media Storage Directory' "
+                "SOP Instances.",
+                DeprecationWarning
+            )
+            ds_class = DicomDir
     else:
         ds_class = FileDataset
 
     ds = ds_class(
         fileobj,
         dataset,
         preamble,
```

### Comparing `pydicom-2.3.1/pydicom/fileset.py` & `pydicom-2.4.0/pydicom/fileset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/fileutil.py` & `pydicom-2.4.0/pydicom/fileutil.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/filewriter.py` & `pydicom-2.4.0/pydicom/filewriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,18 +87,23 @@
             # so we default to OB for BitsAllocated 1 or 8
             elem.VR = VR.OW if cast(int, ds.BitsAllocated) > 8 else VR.OB
 
     # 'US or SS' and dependent on PixelRepresentation
     elif elem.tag in _us_ss_tags:
         # US if PixelRepresentation value is 0x0000, else SS
         #   For references, see the list at
-        #   https://github.com/darcymason/pydicom/pull/298
+        #   https://github.com/pydicom/pydicom/pull/298
         # PixelRepresentation is usually set in the root dataset
-        while 'PixelRepresentation' not in ds and ds.parent and ds.parent():
-            ds = cast(Dataset, ds.parent())
+        while (
+            'PixelRepresentation' not in ds
+            and ds.parent_seq is not None
+            and ds.parent_seq().parent_dataset()   # type: ignore
+        ):
+            # Make weakrefs into strong refs (locally here) by calling () them
+            ds = ds.parent_seq().parent_dataset()  # type: ignore
         # if no pixel data is present, none if these tags is used,
         # so we can just ignore a missing PixelRepresentation in this case
         if (
             'PixelRepresentation' not in ds
             and 'PixelData' not in ds
             or ds.PixelRepresentation == 0
         ):
@@ -255,16 +260,16 @@
     elem : dataelem.DataElement
         The element to encode.
     struct_format : str
         The character format as used by the struct module.
     """
     endianChar = '><'[fp.is_little_endian]
     value = elem.value
-    if value == "":
-        return  # don't need to write anything for empty string
+    if value is None or value == "":
+        return  # don't need to write anything for no or empty value
 
     format_string = endianChar + struct_format
     try:
         try:
             # works only if list, not if string or number
             value.append
         except AttributeError:  # is a single value - the usual case
@@ -346,43 +351,35 @@
 
         if isinstance(val, str):
             val = val.encode(default_encoding)  # type: ignore[assignment]
 
         fp.write(val)  # type: ignore[arg-type]
 
 
-def _encode_and_validate_string(vr: str, value: str,
-                                encodings: Sequence[str]) -> bytes:
-    encoded = encode_string(value, encodings)
-    validate_value(vr, encoded, config.settings.writing_validation_mode)
-    return encoded
-
-
 def write_text(
     fp: DicomIO, elem: DataElement, encodings: Optional[List[str]] = None
 ) -> None:
     """Write a single or multivalued text string."""
     encodings = encodings or [default_encoding]
     val = elem.value
     if val is not None:
         if _is_multi_value(val):
             val = cast(Union[Sequence[bytes], Sequence[str]], val)
             if isinstance(val[0], str):
                 val = cast(Sequence[str], val)
                 val = b'\\'.join(
-                    [_encode_and_validate_string(elem.VR, val, encodings)
-                     for val in val]
+                    [encode_string(val, encodings) for val in val]
                 )
             else:
                 val = cast(Sequence[bytes], val)
                 val = b'\\'.join([val for val in val])
         else:
             val = cast(Union[bytes, str], val)
             if isinstance(val, str):
-                val = _encode_and_validate_string(elem.VR, val, encodings)
+                val = encode_string(val, encodings)
 
         if len(val) % 2 != 0:
             val = val + b' '  # pad to even length
         fp.write(val)
 
 
 def write_number_string(fp: DicomIO, elem: DataElement) -> None:
```

### Comparing `pydicom-2.3.1/pydicom/jsonrep.py` & `pydicom-2.4.0/pydicom/jsonrep.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/misc.py` & `pydicom-2.4.0/pydicom/misc.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/multival.py` & `pydicom-2.4.0/pydicom/multival.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/overlays/numpy_handler.py` & `pydicom-2.4.0/pydicom/overlays/numpy_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/pixel_data_handlers/gdcm_handler.py` & `pydicom-2.4.0/pydicom/pixel_data_handlers/gdcm_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/pixel_data_handlers/jpeg_ls_handler.py` & `pydicom-2.4.0/pydicom/pixel_data_handlers/jpeg_ls_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2008-2018 pydicom authors. See LICENSE file for details.
 """
-Use the `jpeg_ls (CharPyLS) <https://github.com/Who8MyLunch/CharPyLS>`_ Python
+Use the `jpeg_ls (pyjpegls) <https://github.com/pydicom/pyjpegls>`_ Python
 package to decode *Pixel Data*.
 """
 from typing import TYPE_CHECKING, cast
 
 try:
     import numpy
     HAVE_NP = True
@@ -25,15 +25,15 @@
     from pydicom.dataset import Dataset
 
 
 HANDLER_NAME = 'JPEG-LS'
 
 DEPENDENCIES = {
     'numpy': ('http://www.numpy.org/', 'NumPy'),
-    'jpeg_ls': ('https://github.com/Who8MyLunch/CharPyLS', 'CharPyLS'),
+    'jpeg_ls': ('https://github.com/pydicom/pyjpegls', 'pyjpegls'),
 }
 
 SUPPORTED_TRANSFER_SYNTAXES = [
     pydicom.uid.JPEGLSLossless,
     pydicom.uid.JPEGLSNearLossless,
 ]
```

### Comparing `pydicom-2.3.1/pydicom/pixel_data_handlers/numpy_handler.py` & `pydicom-2.4.0/pydicom/pixel_data_handlers/numpy_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -254,16 +254,27 @@
         # Skip any trailing padding bits
         nr_pixels = get_expected_length(ds, unit='pixels')
         arr = cast(
             "np.ndarray", unpack_bits(pixel_data, as_array=True)[:nr_pixels]
         )
     else:
         # Skip the trailing padding byte(s) if present
-        dtype = pixel_dtype(ds, as_float=('Float' in px_keyword[0]))
-        arr = np.frombuffer(pixel_data[:expected_len], dtype=dtype)
+        dtype = pixel_dtype(ds, as_float=("Float" in px_keyword[0]))
+        if (not ds.is_little_endian and dtype.itemsize == 1 and
+                px_keyword[0] == "PixelData" and ds[0x7FE00010].VR == "OW"):
+            # handle the rare case that 1 byte pixels are encoded as OW
+            # in Big Endian transfer syntax
+            # Note: the host Endianness does not matter here; to be read
+            # correctly for a 1 byte type the bytes must always be ordered
+            # as Little Endian
+            dtype16 = dtype.name[:-1] + "16"
+            b = np.frombuffer(pixel_data, dtype=dtype16).byteswap().tobytes()
+            arr = np.frombuffer(b[:expected_len], dtype=dtype)
+        else:
+            arr = np.frombuffer(pixel_data[:expected_len], dtype=dtype)
         if ds.PhotometricInterpretation == 'YBR_FULL_422':
             # PS3.3 C.7.6.3.1.2: YBR_FULL_422 data needs to be resampled
             # Y1 Y2 B1 R1 -> Y1 B1 R1 Y2 B1 R1
             out = np.zeros(expected_len // 2 * 3, dtype=dtype)
             out[::6] = arr[::4]  # Y1
             out[3::6] = arr[1::4]  # Y2
             out[1::6], out[4::6] = arr[2::4], arr[2::4]  # B
```

### Comparing `pydicom-2.3.1/pydicom/pixel_data_handlers/pillow_handler.py` & `pydicom-2.4.0/pydicom/pixel_data_handlers/pillow_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/pixel_data_handlers/pylibjpeg_handler.py` & `pydicom-2.4.0/pydicom/pixel_data_handlers/pylibjpeg_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/pixel_data_handlers/rle_handler.py` & `pydicom-2.4.0/pydicom/pixel_data_handlers/rle_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/pixel_data_handlers/util.py` & `pydicom-2.4.0/pydicom/pixel_data_handlers/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2008-2018 pydicom authors. See LICENSE file for details.
 """Utility functions used in the pixel data handlers."""
 
-from struct import unpack
+from struct import unpack, unpack_from
 from sys import byteorder
 from typing import (
     Dict, Optional, Union, List, Tuple, TYPE_CHECKING, cast, Iterable,
     ByteString
 )
 import warnings
 
@@ -443,15 +443,15 @@
         )
 
     # Ambiguous VR, US or OW
     unc_data: Iterable[int]
     if item['LUTData'].VR == VR.OW:
         endianness = '<' if ds.is_little_endian else '>'
         unpack_fmt = f'{endianness}{nr_entries}H'
-        unc_data = unpack(unpack_fmt, cast(bytes, item.LUTData))
+        unc_data = unpack_from(unpack_fmt, cast(bytes, item.LUTData))
     else:
         unc_data = cast(List[int], item.LUTData)
 
     lut_data: "np.ndarray" = np.asarray(unc_data, dtype=dtype)
 
     # IVs < `first_map` get set to first LUT entry (i.e. index 0)
     clipped_iv = np.zeros(arr.shape, dtype=dtype)
```

### Comparing `pydicom-2.3.1/pydicom/sequence.py` & `pydicom-2.4.0/pydicom/sequence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Copyright 2008-2020 pydicom authors. See LICENSE file for details.
 """Define the Sequence class, which contains a sequence DataElement's items.
 
 Sequence is a list of pydicom Dataset objects.
 """
+from copy import deepcopy
 from typing import (
     Iterable, Optional, List, cast, Union, overload, MutableSequence,
     Dict, Any)
 import weakref
+import warnings
 
+from pydicom import config
 from pydicom.dataset import Dataset
 from pydicom.multival import MultiValue
 
 
 def validate_dataset(elem: object) -> Dataset:
     """Check that `elem` is a :class:`~pydicom.dataset.Dataset` instance."""
     if not isinstance(elem, Dataset):
@@ -46,83 +49,118 @@
         # Dataset IS iterable). This error, however, doesn't inform the user
         # that the actual issue is that their Dataset needs to be INSIDE an
         # iterable object
         if isinstance(iterable, Dataset):
             raise TypeError('The Sequence constructor requires an iterable')
 
         # the parent dataset
-        self._parent: "Optional[weakref.ReferenceType[Dataset]]" = None
+        self._parent_dataset: "Optional[weakref.ReferenceType[Dataset]]" = None
 
         # validate_dataset is used as a pseudo type_constructor
         self._list: List[Dataset] = []
         # If no inputs are provided, we create an empty Sequence
         super().__init__(validate_dataset, iterable or [])
-
+        for ds in self:
+            ds.parent_seq = self  # type: ignore
         self.is_undefined_length: bool
 
     def append(self, val: Dataset) -> None:  # type: ignore[override]
         """Append a :class:`~pydicom.dataset.Dataset` to the sequence."""
         super().append(val)
-        val.parent = self._parent
+        val.parent_seq = self  # type: ignore
 
     def extend(self, val: Iterable[Dataset]) -> None:  # type: ignore[override]
         """Extend the :class:`~pydicom.sequence.Sequence` using an iterable
         of :class:`~pydicom.dataset.Dataset` instances.
         """
         if isinstance(val, Dataset):
             raise TypeError("An iterable of 'Dataset' is required")
 
         super().extend(val)
         for ds in val:
-            ds.parent = self._parent
+            ds.parent_seq = self  # type: ignore
+
+    def __deepcopy__(self, memo: Optional[Dict[int, Any]]) -> "Sequence":
+        copied = Sequence()
+        if memo is not None:
+            memo[id(self)] = copied
+        copied.__dict__.update(deepcopy(self.__dict__, memo))
+        for ds in copied:
+            ds.parent_seq = copied  # type:ignore
+        return copied
 
     def __iadd__(    # type: ignore[override]
         self, other: Iterable[Dataset]
     ) -> MutableSequence[Dataset]:
         """Implement Sequence() += [Dataset()]."""
         if isinstance(other, Dataset):
             raise TypeError("An iterable of 'Dataset' is required")
 
         result = super().__iadd__(other)
         for ds in other:
-            ds.parent = self.parent
+            ds.parent_seq = self  # type: ignore
 
         return result
 
     def insert(    # type: ignore[override]
         self, position: int, val: Dataset
     ) -> None:
         """Insert a :class:`~pydicom.dataset.Dataset` into the sequence."""
         super().insert(position, val)
-        val.parent = self._parent
+        val.parent_seq = self  # type: ignore
 
     @property
-    def parent(self) -> "Optional[weakref.ReferenceType[Dataset]]":
+    def parent_dataset(self) -> "Optional[weakref.ReferenceType[Dataset]]":
         """Return a weak reference to the parent
         :class:`~pydicom.dataset.Dataset`.
 
-        .. versionadded:: 1.3
-
-        .. versionchanged:: 1.4
+        .. versionadded:: 2.4
 
             Returned value is a weak reference to the parent ``Dataset``.
         """
-        return self._parent
+        return self._parent_dataset
+
+    @parent_dataset.setter
+    def parent_dataset(self, value: Dataset) -> None:
+        """Set the parent :class:`~pydicom.dataset.Dataset`
+
+        .. versionadded:: 2.4
+        """
+        if value != self._parent_dataset:
+            self._parent_dataset = weakref.ref(value)
+
+    @property
+    def parent(self) -> "Optional[weakref.ReferenceType[Dataset]]":
+        """Return a weak reference to the parent Dataset
+
+        .. deprecated:: 2.4
+        """
+        if config._use_future:
+            raise AttributeError("Future: Sequence.parent is removed in v3.x")
+        else:
+            warnings.warn(
+                "Sequence.parent will be removed in pydicom 3.0",
+                DeprecationWarning
+            )
+            return self.parent_dataset
 
     @parent.setter
-    def parent(self, value: Dataset) -> None:
-        """Set the parent :class:`~pydicom.dataset.Dataset` and pass it to all
-        :class:`Sequence` items.
-
-        .. versionadded:: 1.3
-        """
-        if value != self._parent:
-            self._parent = weakref.ref(value)
-            for item in self._list:
-                item.parent = self._parent
+    def parent(self, value: "Dataset") -> None:
+        """Set the parent :class:`~pydicom.dataset.Dataset`
+
+        .. deprecated:: 2.4
+        """
+        if config._use_future:
+            raise AttributeError("Future: Sequence.parent is removed in v3.x")
+        else:
+            warnings.warn(
+                "Sequence.parent will be removed in pydicom 3.0",
+                DeprecationWarning
+            )
+            self.parent_dataset = value  # type:ignore
 
     @overload  # type: ignore[override]
     def __setitem__(self, idx: int, val: Dataset) -> None:
         pass  # pragma: no cover
 
     @overload
     def __setitem__(self, idx: slice, val: Iterable[Dataset]) -> None:
@@ -136,31 +174,35 @@
         """
         if isinstance(idx, slice):
             if isinstance(val, Dataset):
                 raise TypeError("Can only assign an iterable of 'Dataset'")
 
             super().__setitem__(idx, val)
             for ds in val:
-                ds.parent = self._parent
+                ds.parent_seq = self  # type: ignore
         else:
             val = cast(Dataset, val)
             super().__setitem__(idx, val)
-            val.parent = self._parent
+            val.parent_seq = self  # type: ignore
 
     def __str__(self) -> str:
         """String description of the Sequence."""
         return f"[{''.join([str(x) for x in self])}]"
 
     def __repr__(self) -> str:  # type: ignore[override]
         """String representation of the Sequence."""
         return f"<{self.__class__.__name__}, length {len(self)}>"
 
     def __getstate__(self) -> Dict[str, Any]:
-        # pickle cannot handle weakref - remove _parent
-        d = self.__dict__.copy()
-        del d['_parent']
-        return d
+        if self.parent_dataset is not None:
+            s = self.__dict__.copy()
+            s['_parent_dataset'] = s['_parent_dataset']()
+            return s
+        return self.__dict__
 
+    # If recovering from a pickle, turn back into weak ref
     def __setstate__(self, state: Dict[str, Any]) -> None:
         self.__dict__.update(state)
-        # re-add _parent - it will be set to the parent dataset on demand
-        self.__dict__['_parent'] = None
+        if self.__dict__['_parent_dataset'] is not None:
+            self.__dict__['_parent_dataset'] = weakref.ref(
+                self.__dict__['_parent_dataset']
+            )
```

### Comparing `pydicom-2.3.1/pydicom/sr/_cid_dict.py` & `pydicom-2.4.0/pydicom/sr/_cid_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/sr/_concepts_dict.py` & `pydicom-2.4.0/pydicom/sr/_concepts_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/sr/_snomed_dict.py` & `pydicom-2.4.0/pydicom/sr/_snomed_dict.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15072,8 +15072,8 @@
      'R0-00003': '716936005',
      'R0-00025': '716937001',
      'R-FFFC0': '716938006',
      'R-FFFDD': '716939003',
      'R-FFFEA': '716940001',
      'R0-0000B': '716941002',
      'R-FFFD9': '717027004',
-}
+}
```

### Comparing `pydicom-2.3.1/pydicom/sr/codedict.py` & `pydicom-2.4.0/pydicom/sr/codedict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/sr/coding.py` & `pydicom-2.4.0/pydicom/sr/coding.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/tag.py` & `pydicom-2.4.0/pydicom/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,19 @@
     def __str__(self) -> str:
         """Return the tag value as a hex string '(gggg, eeee)'."""
         return "({0:04x}, {1:04x})".format(self.group, self.element)
 
     __repr__ = __str__
 
     @property
+    def json_key(self) -> str:
+        """Return the tag value as a JSON key string 'GGGGEEEE'."""
+        return f"{self.group:04X}{self.element:04X}"
+
+    @property
     def group(self) -> int:
         """Return the tag's group number as :class:`int`."""
         return self >> 16
 
     @property
     def element(self) -> int:
         """Return the tag's element number as :class:`int`."""
@@ -222,14 +227,23 @@
     def is_private_creator(self) -> bool:
         """Return ``True`` if the tag is a private creator.
 
         .. versionadded:: 1.1
         """
         return self.is_private and 0x0010 <= self.element < 0x0100
 
+    @property
+    def private_creator(self) -> "BaseTag":
+        """Return the private creator tag for the given tag.
+        The result is meaningless if this is not a private tag.
+
+        .. versionadded:: 2.4
+        """
+        return BaseTag((self & 0xffff0000) | self.element >> 8)
+
 
 def TupleTag(group_elem: Tuple[int, int]) -> BaseTag:
     """Fast factory for :class:`BaseTag` object with known safe (group, elem)
     :class:`tuple`
     """
     long_value = group_elem[0] << 16 | group_elem[1]
     return BaseTag(long_value)
```

### Comparing `pydicom-2.3.1/pydicom/uid.py` & `pydicom-2.4.0/pydicom/uid.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/util/codify.py` & `pydicom-2.4.0/pydicom/util/codify.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # This can then be pasted into a python file and parameters edited as necessary
 # to create a DICOM file from scratch
 
 import argparse
 import os.path
 import re
 import sys
-from typing import Optional, List, Callable
+from typing import Optional, List, Callable, cast
+from collections import deque
 
 import pydicom
 from pydicom.datadict import dictionary_keyword
 from pydicom.dataelem import DataElement
 from pydicom.dataset import Dataset
 from pydicom.tag import BaseTag
 from pydicom.valuerep import BYTES_VR, AMBIGUOUS_VR, VR
@@ -76,15 +77,16 @@
     return line_term.join((line1, line2, line3))
 
 
 def code_dataelem(
     dataelem: DataElement,
     dataset_name: str = "ds",
     exclude_size: Optional[int] = None,
-    include_private: bool = False
+    include_private: bool = False,
+    var_names: Optional[deque] = None
 ) -> str:
     """Code lines for a single DICOM data element
 
     Parameters
     ----------
 
     dataelem : DataElement
@@ -92,36 +94,43 @@
     dataset_name : str
         The variable name of the Dataset containing `dataelem`
     exclude_size : Union[int, None]
         If specified, values longer than this (in bytes)
         will only have a commented string for a value,
         causing a syntax error when the code is run,
         and thus prompting the user to remove or fix that line.
-
+    var_names: Union[deque, None]
+        Used internally to ensure unique variable names in nested sequences.
     Returns
     -------
     str
         A string containing code to recreate the data element
         If the data element is a sequence, calls code_sequence
     """
 
     if dataelem.VR == VR.SQ:
         return code_sequence(
-            dataelem, dataset_name, exclude_size, include_private
+            dataelem, dataset_name, exclude_size, include_private,
+            var_names=var_names
         )
 
     # If in DICOM dictionary, set using the keyword
     # If not (e.g. is private element), set using add_new method
     have_keyword = True
     try:
         keyword = dictionary_keyword(dataelem.tag)
     except KeyError:
         have_keyword = False
 
-    valuerep = repr(dataelem.value)
+    # If the value representation of the data element is AT (Attribute Tag),
+    # then format it as a tag
+    if dataelem.VR == 'AT':
+        valuerep = tag_repr(dataelem.value)
+    else:
+        valuerep = repr(dataelem.value)
 
     if exclude_size:
         if (
             dataelem.VR in (BYTES_VR | AMBIGUOUS_VR) - {VR.US_SS}
             and not isinstance(dataelem.value, (int, float))
             and len(dataelem.value) > exclude_size
         ):
@@ -139,14 +148,15 @@
 
 def code_sequence(
     dataelem: DataElement,
     dataset_name: str = "ds",
     exclude_size: Optional[int] = None,
     include_private: bool = False,
     name_filter: Callable[[str], str] = default_name_filter,
+    var_names: Optional[deque] = None,
 ) -> str:
     """Code lines for recreating a Sequence data element
 
     Parameters
     ----------
     dataelem : DataElement
         The DataElement instance whose value is the Sequence
@@ -158,37 +168,51 @@
         run, and thus prompting the user to remove or fix that line.
     include_private: bool
         If ``False`` (default) private elements are skipped, otherwise private
         data elements will be coded.
     name_filter: Callable[[str], str]
         A callable taking a sequence name or sequence item name, and returning
         a shorter name for easier code reading
+    var_names: Union[deque, None]
+        Used internally to ensure unique variable names in nested sequences.
 
     Returns
     -------
     str
         A string containing code lines to recreate a DICOM sequence
     """
 
+    # Normally var_names is given from code_dataset, but for some tests need
+    #   to initialize it
+    if var_names is None:
+        var_names = deque()
+
+    def unique_name(name: str) -> str:
+        name_count = cast(deque, var_names).count(name) - 1
+        return name if name_count == 0 else name + f"_{name_count}"
+
     lines = []
     seq = dataelem.value
     seq_name = dataelem.name
     seq_item_name = seq_name.replace(" Sequence", "")
     try:
         seq_keyword = dictionary_keyword(dataelem.tag)
     except KeyError:
         seq_keyword = f"Tag{dataelem.tag:08x}"
 
     # Create comment line to document the start of Sequence
     lines.append("")
     lines.append("# " + seq_name)
 
     # Code line to create a new Sequence object
-    if name_filter:
-        seq_var = name_filter(seq_keyword)
+    seq_var = name_filter(seq_keyword)
+    var_names.append(seq_var)
+    orig_seq_var = seq_var
+    seq_var = unique_name(seq_var)
+
     lines.append(seq_var + " = Sequence()")
 
     # Code line to add the sequence to its parent
     lines.append(dataset_name + "." + seq_keyword + " = " + seq_var)
 
     # Code lines to add sequence items to the Sequence
     for i, ds in enumerate(seq):
@@ -204,33 +228,49 @@
             index_str = str(i + 1)
 
         # Code comment line to mark start of sequence item
         lines.append("")
         lines.append("# " + seq_name + ": " + seq_item_name + " " + index_str)
 
         # Determine the variable name to use for the sequence item (dataset)
-        ds_name = seq_var.replace("_sequence", "") + index_str
+        ds_name = orig_seq_var.replace("_sequence", "") + index_str
+
+        # Append "_#" if name already in use (in parent sequences)
+        var_names.append(ds_name)
+        ds_name = unique_name(ds_name)
+
+        # Code the sequence item dataset
+        code_item = code_dataset(
+            ds, ds_name, exclude_size, include_private, var_names=var_names
+        )
+
+        # Remove variable name from stored list, this dataset complete
+        var_names.pop()
 
-        # Code the sequence item
-        code_item = code_dataset(ds, ds_name, exclude_size, include_private)
-        lines.append(code_item)
+        # Code dataset creation and appending that to sequence, then the rest
+        # This keeps the logic close together, rather than after many items set
+        code_split = code_item.splitlines()
+        lines.append(code_split[0])  # "<ds_name> = Dataset()"
+        lines.append(f"{seq_var}.append({ds_name})")
+        lines.extend(code_split[1:])
 
-        # Code the line to append the item to its parent sequence
-        lines.append(seq_var + ".append(" + ds_name + ")")
+    # Remove sequence variable name we've used
+    var_names.pop()
 
     # Join the lines and return a single string
     return line_term.join(lines)
 
 
 def code_dataset(
     ds: Dataset,
     dataset_name: str = "ds",
     exclude_size: Optional[int] = None,
     include_private: bool = False,
     is_file_meta: bool = False,
+    var_names: Optional[deque] = None
 ) -> str:
     """Return Python code for creating `ds`.
 
     Parameters
     ----------
     ds : pydicom.dataset.Dataset
         The dataset to codify.
@@ -241,39 +281,47 @@
         commented string for a value, causing a syntax error when the code is
         run, and thus prompting the user to remove or fix that line.
     include_private : bool, optional
         If ``False`` (default) private elements are skipped, otherwise private
         data elements will be coded.
     is_file_meta : bool, optional
         ``True`` if `ds` contains file meta information elements.
+    var_names: deque, optional
+        Used internally to ensure unique variable names in nested sequences.
 
     Returns
     -------
     str
         The codified dataset.
     """
 
+    if var_names is None:
+        var_names = deque()
     lines = []
+
     ds_class = " = FileMetaDataset()" if is_file_meta else " = Dataset()"
+
     lines.append(dataset_name + ds_class)
     for dataelem in ds:
         # If a private data element and flag says so, skip it and go to next
         if not include_private and dataelem.tag.is_private:
             continue
         # Otherwise code the line and add it to the lines list
         code_line = code_dataelem(
-            dataelem, dataset_name, exclude_size, include_private
+            dataelem, dataset_name, exclude_size, include_private,
+            var_names=var_names
         )
         lines.append(code_line)
         # Add blank line if just coded a sequence
         if dataelem.VR == VR.SQ:
             lines.append("")
     # If sequence was end of this dataset, remove the extra blank line
     if len(lines) and lines[-1] == "":
         lines.pop()
+
     # Join all the code lines and return them
     return line_term.join(lines)
 
 
 def code_file(
     filename: str,
     exclude_size: Optional[int] = None,
@@ -309,16 +357,16 @@
     exclude_size: Optional[int] = None,
     include_private: bool = False
 ) -> str:
     """Write a complete source code file to recreate a DICOM file
 
     Parameters
     ----------
-    filename : str
-        Complete path and filename of a DICOM file to convert
+    ds : Dataset
+        A pydicom Dataset to convert
     exclude_size : Union[int,None]
         If not None, values longer than this (in bytes)
         will only have a commented string for a value,
         causing a syntax error when the code is run,
         and thus prompting the user to remove or fix that line.
     include_private : bool
         If ``False`` (default), private elements are skipped
@@ -332,14 +380,15 @@
     """
     lines = []
 
     # Code a nice header for the python file
     filename = ds.get("filename")
     identifier = f"DICOM file '{filename}'" if filename else "non-file dataset"
 
+    lines.append("# -*- coding: utf-8 -*-")
     lines.append(f"# Coded version of {identifier}")
     lines.append("# Produced by pydicom codify utility script")
 
     # Code the necessary imports
     lines.append(code_imports())
     lines.append("")
 
@@ -381,15 +430,15 @@
         "filespec",
         help=filespec_help,
         type=filespec_parser,
     )
     parser.add_argument(
         "outfile",
         nargs="?",
-        type=argparse.FileType("w"),
+        type=argparse.FileType("w", encoding="UTF-8"),
         help=(
             "Filename to write Python code to, if not specified then code is "
             "written to stdout"
         ),
         default=sys.stdout,
     )
     parser.add_argument(
```

### Comparing `pydicom-2.3.1/pydicom/util/dump.py` & `pydicom-2.4.0/pydicom/util/dump.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/util/fixer.py` & `pydicom-2.4.0/pydicom/util/fixer.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/util/hexutil.py` & `pydicom-2.4.0/pydicom/util/hexutil.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.3.1/pydicom/util/leanread.py` & `pydicom-2.4.0/pydicom/util/leanread.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType]
     ) -> Optional[bool]:
         self.fobj.close()
 
-        return None
+        return None  # noqa: PLR1711
 
     def __iter__(self) -> Iterator[_ElementType]:
         # Need the transfer_syntax later
         tsyntax: Optional[UID] = None
 
         # Yield the file meta info elements
         file_meta = data_element_generator(
```

### Comparing `pydicom-2.3.1/pydicom/valuerep.py` & `pydicom-2.4.0/pydicom/valuerep.py`

 * *Files 8% similar despite different names*

```diff
@@ -148,4040 +148,4445 @@
 00000930: 4259 5445 5f56 525f 5245 4745 5845 5320  BYTE_VR_REGEXES 
 00000940: 3d20 7b76 723a 2072 652e 636f 6d70 696c  = {vr: re.compil
 00000950: 6528 7265 6765 782e 656e 636f 6465 2829  e(regex.encode()
 00000960: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
 00000970: 2020 2020 2066 6f72 2028 7672 2c20 7265       for (vr, re
 00000980: 6765 7829 2069 6e20 5652 5f52 4547 4558  gex) in VR_REGEX
 00000990: 4553 2e69 7465 6d73 2829 7d0a 0a0a 6465  ES.items()}...de
-000009a0: 6620 7661 6c69 6461 7465 5f76 725f 6c65  f validate_vr_le
-000009b0: 6e67 7468 2876 723a 2073 7472 2c20 7661  ngth(vr: str, va
-000009c0: 6c75 653a 2055 6e69 6f6e 5b73 7472 2c20  lue: Union[str, 
-000009d0: 6279 7465 735d 2920 2d3e 2054 7570 6c65  bytes]) -> Tuple
-000009e0: 5b62 6f6f 6c2c 2073 7472 5d3a 0a20 2020  [bool, str]:.   
-000009f0: 2022 2222 5661 6c69 6461 7465 2074 6865   """Validate the
-00000a00: 2076 616c 7565 206c 656e 6774 6820 666f   value length fo
-00000a10: 7220 6120 6769 7665 6e20 5652 2e0a 0a20  r a given VR... 
-00000a20: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00000a30: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00000a40: 2076 7220 3a20 7374 720a 2020 2020 2020   vr : str.      
-00000a50: 2020 5468 6520 7661 6c75 6520 7265 7072    The value repr
-00000a60: 6573 656e 7461 7469 6f6e 2074 6f20 7661  esentation to va
-00000a70: 6c69 6461 7465 2061 6761 696e 7374 2e0a  lidate against..
-00000a80: 2020 2020 7661 6c75 6520 3a20 7374 7220      value : str 
-00000a90: 6f72 2062 7974 6573 0a20 2020 2020 2020  or bytes.       
-00000aa0: 2054 6865 2076 616c 7565 2074 6f20 7661   The value to va
-00000ab0: 6c69 6461 7465 2e0a 0a20 2020 2052 6574  lidate...    Ret
-00000ac0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00000ad0: 0a20 2020 2020 2020 2041 2074 7570 6c65  .        A tuple
-00000ae0: 206f 6620 6120 626f 6f6c 6561 6e20 7661   of a boolean va
-00000af0: 6c69 6461 7469 6f6e 2072 6573 756c 7420  lidation result 
-00000b00: 616e 6420 7468 6520 6572 726f 7220 6d65  and the error me
-00000b10: 7373 6167 652e 0a20 2020 2022 2222 0a20  ssage..    """. 
-00000b20: 2020 206d 6178 5f6c 656e 6774 6820 3d20     max_length = 
-00000b30: 4d41 585f 5641 4c55 455f 4c45 4e2e 6765  MAX_VALUE_LEN.ge
-00000b40: 7428 7672 2c20 3029 0a20 2020 2069 6620  t(vr, 0).    if 
-00000b50: 6d61 785f 6c65 6e67 7468 203e 2030 3a0a  max_length > 0:.
-00000b60: 2020 2020 2020 2020 7661 6c75 655f 6c65          value_le
-00000b70: 6e67 7468 203d 206c 656e 2876 616c 7565  ngth = len(value
-00000b80: 290a 2020 2020 2020 2020 6966 2076 616c  ).        if val
-00000b90: 7565 5f6c 656e 6774 6820 3e20 6d61 785f  ue_length > max_
-00000ba0: 6c65 6e67 7468 3a0a 2020 2020 2020 2020  length:.        
-00000bb0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00000bc0: 2c20 280a 2020 2020 2020 2020 2020 2020  , (.            
-00000bd0: 2020 2020 6622 5468 6520 7661 6c75 6520      f"The value 
-00000be0: 6c65 6e67 7468 2028 7b76 616c 7565 5f6c  length ({value_l
-00000bf0: 656e 6774 687d 2920 6578 6365 6564 7320  ength}) exceeds 
-00000c00: 7468 6520 220a 2020 2020 2020 2020 2020  the ".          
-00000c10: 2020 2020 2020 6622 6d61 7869 6d75 6d20        f"maximum 
-00000c20: 6c65 6e67 7468 206f 6620 7b6d 6178 5f6c  length of {max_l
-00000c30: 656e 6774 687d 2061 6c6c 6f77 6564 2066  ength} allowed f
-00000c40: 6f72 2056 5220 7b76 727d 2e22 0a20 2020  or VR {vr}.".   
-00000c50: 2020 2020 2020 2020 2029 0a20 2020 2072           ).    r
-00000c60: 6574 7572 6e20 5472 7565 2c20 2222 0a0a  eturn True, ""..
-00000c70: 0a64 6566 2076 616c 6964 6174 655f 7265  .def validate_re
-00000c80: 6765 7828 7672 3a20 7374 722c 2076 616c  gex(vr: str, val
-00000c90: 7565 3a20 556e 696f 6e5b 7374 722c 2062  ue: Union[str, b
-00000ca0: 7974 6573 5d29 202d 3e20 5475 706c 655b  ytes]) -> Tuple[
-00000cb0: 626f 6f6c 2c20 7374 725d 3a0a 2020 2020  bool, str]:.    
-00000cc0: 2222 2256 616c 6964 6174 6520 7468 6520  """Validate the 
-00000cd0: 7661 6c75 6520 666f 7220 6120 6769 7665  value for a give
-00000ce0: 6e20 5652 2066 6f72 2061 6c6c 6f77 6564  n VR for allowed
-00000cf0: 2063 6861 7261 6374 6572 730a 2020 2020   characters.    
-00000d00: 7573 696e 6720 6120 7265 6775 6c61 7220  using a regular 
-00000d10: 6578 7072 6573 7369 6f6e 2e0a 0a20 2020  expression...   
-00000d20: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00000d30: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2076  ----------.    v
-00000d40: 7220 3a20 7374 720a 2020 2020 2020 2020  r : str.        
-00000d50: 5468 6520 7661 6c75 6520 7265 7072 6573  The value repres
-00000d60: 656e 7461 7469 6f6e 2074 6f20 7661 6c69  entation to vali
-00000d70: 6461 7465 2061 6761 696e 7374 2e0a 2020  date against..  
-00000d80: 2020 7661 6c75 6520 3a20 7374 720a 2020    value : str.  
-00000d90: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
-00000da0: 746f 2076 616c 6964 6174 652e 0a0a 2020  to validate...  
-00000db0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00000dc0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4120  -----.        A 
-00000dd0: 7475 706c 6520 6f66 2061 2062 6f6f 6c65  tuple of a boole
-00000de0: 616e 2076 616c 6964 6174 696f 6e20 7265  an validation re
-00000df0: 7375 6c74 2061 6e64 2074 6865 2065 7272  sult and the err
-00000e00: 6f72 206d 6573 7361 6765 2e0a 2020 2020  or message..    
-00000e10: 2222 220a 2020 2020 6966 2076 616c 7565  """.    if value
-00000e20: 3a0a 2020 2020 2020 2020 7265 6765 783a  :.        regex:
-00000e30: 2041 6e79 0a20 2020 2020 2020 206e 6577   Any.        new
-00000e40: 6c69 6e65 3a20 556e 696f 6e5b 7374 722c  line: Union[str,
-00000e50: 2069 6e74 5d0a 2020 2020 2020 2020 6966   int].        if
-00000e60: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
-00000e70: 652c 2073 7472 293a 0a20 2020 2020 2020  e, str):.       
-00000e80: 2020 2020 2072 6567 6578 203d 2053 5452       regex = STR
-00000e90: 5f56 525f 5245 4745 5845 535b 7672 5d0a  _VR_REGEXES[vr].
-00000ea0: 2020 2020 2020 2020 2020 2020 6e65 776c              newl
-00000eb0: 696e 6520 3d20 225c 6e22 0a20 2020 2020  ine = "\n".     
-00000ec0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00000ed0: 2020 2020 2072 6567 6578 203d 2042 5954       regex = BYT
-00000ee0: 455f 5652 5f52 4547 4558 4553 5b76 725d  E_VR_REGEXES[vr]
-00000ef0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-00000f00: 6c69 6e65 203d 2031 3020 2023 206e 6577  line = 10  # new
-00000f10: 6c69 6e65 2063 6861 7261 6374 6572 0a20  line character. 
-00000f20: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
-00000f30: 2e6d 6174 6368 2872 6567 6578 2c20 7661  .match(regex, va
-00000f40: 6c75 6529 206f 7220 7661 6c75 6520 616e  lue) or value an
-00000f50: 6420 7661 6c75 655b 2d31 5d20 3d3d 206e  d value[-1] == n
-00000f60: 6577 6c69 6e65 3a0a 2020 2020 2020 2020  ewline:.        
-00000f70: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00000f80: 2c20 6622 496e 7661 6c69 6420 7661 6c75  , f"Invalid valu
-00000f90: 6520 666f 7220 5652 207b 7672 7d3a 207b  e for VR {vr}: {
-00000fa0: 7661 6c75 6521 727d 2e22 0a20 2020 2072  value!r}.".    r
-00000fb0: 6574 7572 6e20 5472 7565 2c20 2222 0a0a  eturn True, ""..
-00000fc0: 0a64 6566 2076 616c 6964 6174 655f 6c65  .def validate_le
-00000fd0: 6e67 7468 5f61 6e64 5f72 6567 6578 280a  ngth_and_regex(.
-00000fe0: 2020 2020 2020 2020 7672 3a20 7374 722c          vr: str,
-00000ff0: 2076 616c 7565 3a20 556e 696f 6e5b 7374   value: Union[st
-00001000: 722c 2062 7974 6573 5d29 202d 3e20 5475  r, bytes]) -> Tu
-00001010: 706c 655b 626f 6f6c 2c20 7374 725d 3a0a  ple[bool, str]:.
-00001020: 2020 2020 2222 2256 616c 6964 6174 6520      """Validate 
-00001030: 7468 6520 7661 6c75 6520 666f 7220 6120  the value for a 
-00001040: 6769 7665 6e20 5652 2062 6f74 6820 666f  given VR both fo
-00001050: 7220 6d61 7869 6d75 6d20 6c65 6e67 7468  r maximum length
-00001060: 2061 6e64 0a20 2020 2066 6f72 2061 6c6c   and.    for all
-00001070: 6f77 6564 2063 6861 7261 6374 6572 7320  owed characters 
-00001080: 7573 696e 6720 6120 7265 6775 6c61 7220  using a regular 
-00001090: 6578 7072 6573 7369 6f6e 2e0a 0a20 2020  expression...   
-000010a0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000010b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2076  ----------.    v
-000010c0: 7220 3a20 7374 720a 2020 2020 2020 2020  r : str.        
-000010d0: 5468 6520 7661 6c75 6520 7265 7072 6573  The value repres
-000010e0: 656e 7461 7469 6f6e 2074 6f20 7661 6c69  entation to vali
-000010f0: 6461 7465 2061 6761 696e 7374 2e0a 2020  date against..  
-00001100: 2020 7661 6c75 6520 3a20 7374 720a 2020    value : str.  
-00001110: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
-00001120: 746f 2076 616c 6964 6174 652e 0a0a 2020  to validate...  
-00001130: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00001140: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4120  -----.        A 
-00001150: 7475 706c 6520 6f66 2061 2062 6f6f 6c65  tuple of a boole
-00001160: 616e 2076 616c 6964 6174 696f 6e20 7265  an validation re
-00001170: 7375 6c74 2061 6e64 2074 6865 2065 7272  sult and the err
-00001180: 6f72 206d 6573 7361 6765 2e0a 2020 2020  or message..    
-00001190: 2222 220a 2020 2020 6973 5f76 616c 6964  """.    is_valid
-000011a0: 5f6c 656e 2c20 6d73 6731 203d 2076 616c  _len, msg1 = val
-000011b0: 6964 6174 655f 7672 5f6c 656e 6774 6828  idate_vr_length(
-000011c0: 7672 2c20 7661 6c75 6529 0a20 2020 2069  vr, value).    i
-000011d0: 735f 7661 6c69 645f 6578 7072 2c20 6d73  s_valid_expr, ms
-000011e0: 6732 203d 2076 616c 6964 6174 655f 7265  g2 = validate_re
-000011f0: 6765 7828 7672 2c20 7661 6c75 6529 0a20  gex(vr, value). 
-00001200: 2020 206d 7367 203d 2022 2022 2e6a 6f69     msg = " ".joi
-00001210: 6e28 5b6d 7367 312c 206d 7367 325d 292e  n([msg1, msg2]).
-00001220: 7374 7269 7028 290a 2020 2020 6966 206d  strip().    if m
-00001230: 7367 3a0a 2020 2020 2020 2020 6d73 6720  sg:.        msg 
-00001240: 2b3d 2028 0a20 2020 2020 2020 2020 2020  += (.           
-00001250: 2022 2050 6c65 6173 6520 7365 6520 3c68   " Please see <h
-00001260: 7474 7073 3a2f 2f64 6963 6f6d 2e6e 656d  ttps://dicom.nem
-00001270: 612e 6f72 672f 6d65 6469 6361 6c2f 6469  a.org/medical/di
-00001280: 636f 6d2f 6375 7272 656e 742f 6f75 7470  com/current/outp
-00001290: 7574 220a 2020 2020 2020 2020 2020 2020  ut".            
-000012a0: 222f 6874 6d6c 2f70 6172 7430 352e 6874  "/html/part05.ht
-000012b0: 6d6c 2374 6162 6c65 5f36 2e32 2d31 3e20  ml#table_6.2-1> 
-000012c0: 666f 7220 616c 6c6f 7765 6420 7661 6c75  for allowed valu
-000012d0: 6573 2066 6f72 2065 6163 6820 5652 2e22  es for each VR."
-000012e0: 0a20 2020 2020 2020 2029 0a20 2020 2072  .        ).    r
-000012f0: 6574 7572 6e20 6973 5f76 616c 6964 5f6c  eturn is_valid_l
-00001300: 656e 2061 6e64 2069 735f 7661 6c69 645f  en and is_valid_
-00001310: 6578 7072 2c20 6d73 670a 0a0a 6465 6620  expr, msg...def 
-00001320: 7661 6c69 6461 7465 5f70 6e5f 636f 6d70  validate_pn_comp
-00001330: 6f6e 656e 745f 6c65 6e67 7468 280a 2020  onent_length(.  
-00001340: 2020 2020 2020 7672 3a20 7374 722c 2076        vr: str, v
-00001350: 616c 7565 3a20 556e 696f 6e5b 7374 722c  alue: Union[str,
-00001360: 2062 7974 6573 5d29 202d 3e20 5475 706c   bytes]) -> Tupl
-00001370: 655b 626f 6f6c 2c20 7374 725d 3a0a 2020  e[bool, str]:.  
-00001380: 2020 2222 2256 616c 6964 6174 6520 7468    """Validate th
-00001390: 6520 504e 2063 6f6d 706f 6e65 6e74 2076  e PN component v
-000013a0: 616c 7565 2066 6f72 2074 6865 206d 6178  alue for the max
-000013b0: 696d 756d 206c 656e 6774 682e 0a0a 2020  imum length...  
-000013c0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000013d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000013e0: 7672 203a 2073 7472 0a20 2020 2020 2020  vr : str.       
-000013f0: 2049 676e 6f72 6564 2e0a 2020 2020 7661   Ignored..    va
-00001400: 6c75 6520 3a20 7374 720a 2020 2020 2020  lue : str.      
-00001410: 2020 5468 6520 7661 6c75 6520 746f 2076    The value to v
-00001420: 616c 6964 6174 652e 0a0a 2020 2020 5265  alidate...    Re
-00001430: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00001440: 2d0a 2020 2020 2020 2020 4120 7475 706c  -.        A tupl
-00001450: 6520 6f66 2061 2062 6f6f 6c65 616e 2076  e of a boolean v
-00001460: 616c 6964 6174 696f 6e20 7265 7375 6c74  alidation result
-00001470: 2061 6e64 2074 6865 2065 7272 6f72 206d   and the error m
-00001480: 6573 7361 6765 2e0a 2020 2020 2222 220a  essage..    """.
-00001490: 2020 2020 6966 206c 656e 2876 616c 7565      if len(value
-000014a0: 2920 3e20 3634 3a0a 2020 2020 2020 2020  ) > 64:.        
-000014b0: 7265 7475 726e 2046 616c 7365 2c20 280a  return False, (.
-000014c0: 2020 2020 2020 2020 2020 2020 6622 5468              f"Th
-000014d0: 6520 504e 2063 6f6d 706f 6e65 6e74 206c  e PN component l
-000014e0: 656e 6774 6820 287b 6c65 6e28 7661 6c75  ength ({len(valu
-000014f0: 6529 7d29 2065 7863 6565 6473 2074 6865  e)}) exceeds the
-00001500: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
-00001510: 226d 6178 696d 756d 2061 6c6c 6f77 6564  "maximum allowed
-00001520: 206c 656e 6774 6820 6f66 2036 342e 220a   length of 64.".
-00001530: 2020 2020 2020 2020 290a 2020 2020 7265          ).    re
-00001540: 7475 726e 2054 7275 652c 2022 220a 0a0a  turn True, ""...
-00001550: 6465 6620 7661 6c69 6461 7465 5f70 6e28  def validate_pn(
-00001560: 7672 3a20 7374 722c 2076 616c 7565 3a20  vr: str, value: 
-00001570: 556e 696f 6e5b 7374 722c 2062 7974 6573  Union[str, bytes
-00001580: 5d29 202d 3e20 5475 706c 655b 626f 6f6c  ]) -> Tuple[bool
-00001590: 2c20 7374 725d 3a0a 2020 2020 2222 2256  , str]:.    """V
-000015a0: 616c 6964 6174 6520 7468 6520 7661 6c75  alidate the valu
-000015b0: 6520 666f 7220 5652 2050 4e20 666f 7220  e for VR PN for 
-000015c0: 7468 6520 6d61 7869 6d75 6d20 6e75 6d62  the maximum numb
-000015d0: 6572 206f 6620 636f 6d70 6f6e 656e 7473  er of components
-000015e0: 0a20 2020 2061 6e64 2066 6f72 2074 6865  .    and for the
-000015f0: 206d 6178 696d 756d 206c 656e 6774 6820   maximum length 
-00001600: 6f66 2065 6163 6820 636f 6d70 6f6e 656e  of each componen
-00001610: 742e 0a0a 2020 2020 5061 7261 6d65 7465  t...    Paramete
-00001620: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00001630: 2d0a 2020 2020 7672 203a 2073 7472 0a20  -.    vr : str. 
-00001640: 2020 2020 2020 2049 676e 6f72 6564 2e0a         Ignored..
-00001650: 2020 2020 7661 6c75 6520 3a20 7374 720a      value : str.
-00001660: 2020 2020 2020 2020 5468 6520 7661 6c75          The valu
-00001670: 6520 746f 2076 616c 6964 6174 652e 0a0a  e to validate...
-00001680: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00001690: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000016a0: 4120 7475 706c 6520 6f66 2061 2062 6f6f  A tuple of a boo
-000016b0: 6c65 616e 2076 616c 6964 6174 696f 6e20  lean validation 
-000016c0: 7265 7375 6c74 2061 6e64 2074 6865 2065  result and the e
-000016d0: 7272 6f72 206d 6573 7361 6765 2e0a 2020  rror message..  
-000016e0: 2020 2222 220a 2020 2020 6966 206e 6f74    """.    if not
-000016f0: 2076 616c 7565 3a0a 2020 2020 2020 2020   value:.        
-00001700: 7265 7475 726e 2054 7275 652c 2022 220a  return True, "".
-00001710: 2020 2020 636f 6d70 6f6e 656e 7473 3a20      components: 
-00001720: 5365 7175 656e 6365 5b55 6e69 6f6e 5b73  Sequence[Union[s
-00001730: 7472 2c20 6279 7465 735d 5d0a 2020 2020  tr, bytes]].    
-00001740: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
-00001750: 6c75 652c 2062 7974 6573 293a 0a20 2020  lue, bytes):.   
-00001760: 2020 2020 2063 6f6d 706f 6e65 6e74 7320       components 
-00001770: 3d20 7661 6c75 652e 7370 6c69 7428 6222  = value.split(b"
-00001780: 3d22 290a 2020 2020 656c 7365 3a0a 2020  =").    else:.  
-00001790: 2020 2020 2020 636f 6d70 6f6e 656e 7473        components
-000017a0: 203d 2076 616c 7565 2e73 706c 6974 2822   = value.split("
-000017b0: 3d22 290a 2020 2020 6966 206c 656e 2863  =").    if len(c
-000017c0: 6f6d 706f 6e65 6e74 7329 203e 2033 3a0a  omponents) > 3:.
-000017d0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000017e0: 616c 7365 2c20 280a 2020 2020 2020 2020  alse, (.        
-000017f0: 2020 2020 6622 5468 6520 6e75 6d62 6572      f"The number
-00001800: 206f 6620 504e 2063 6f6d 706f 6e65 6e74   of PN component
-00001810: 7320 6c65 6e67 7468 2028 7b6c 656e 2863  s length ({len(c
-00001820: 6f6d 706f 6e65 6e74 7329 7d29 2065 7863  omponents)}) exc
-00001830: 6565 6473 2022 0a20 2020 2020 2020 2020  eeds ".         
-00001840: 2020 2066 2274 6865 206d 6178 696d 756d     f"the maximum
-00001850: 2061 6c6c 6f77 6564 206e 756d 6265 7220   allowed number 
-00001860: 6f66 2033 2e22 0a20 2020 2020 2020 2029  of 3.".        )
-00001870: 0a20 2020 2066 6f72 2063 6f6d 7020 696e  .    for comp in
-00001880: 2063 6f6d 706f 6e65 6e74 733a 0a20 2020   components:.   
-00001890: 2020 2020 2076 616c 6964 2c20 6d73 6720       valid, msg 
-000018a0: 3d20 7661 6c69 6461 7465 5f70 6e5f 636f  = validate_pn_co
-000018b0: 6d70 6f6e 656e 745f 6c65 6e67 7468 2822  mponent_length("
-000018c0: 504e 222c 2063 6f6d 7029 0a20 2020 2020  PN", comp).     
-000018d0: 2020 2069 6620 6e6f 7420 7661 6c69 643a     if not valid:
-000018e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000018f0: 7572 6e20 4661 6c73 652c 206d 7367 0a20  urn False, msg. 
-00001900: 2020 2072 6574 7572 6e20 5472 7565 2c20     return True, 
-00001910: 2222 0a0a 0a64 6566 2076 616c 6964 6174  ""...def validat
-00001920: 655f 706e 5f63 6f6d 706f 6e65 6e74 2876  e_pn_component(v
-00001930: 616c 7565 3a20 556e 696f 6e5b 7374 722c  alue: Union[str,
-00001940: 2062 7974 6573 5d29 202d 3e20 4e6f 6e65   bytes]) -> None
-00001950: 3a0a 2020 2020 2222 2256 616c 6964 6174  :.    """Validat
-00001960: 6520 7468 6520 7661 6c75 6520 6f66 2061  e the value of a
-00001970: 2073 696e 676c 6520 636f 6d70 6f6e 656e   single componen
-00001980: 7420 6f66 2056 5220 504e 2066 6f72 206d  t of VR PN for m
-00001990: 6178 696d 756d 206c 656e 6774 682e 0a0a  aximum length...
-000019a0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000019b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000019c0: 2020 7661 6c75 6520 3a20 7374 7220 6f72    value : str or
-000019d0: 2062 7974 6573 0a20 2020 2020 2020 2054   bytes.        T
-000019e0: 6865 2063 6f6d 706f 6e65 6e74 2076 616c  he component val
-000019f0: 7565 2074 6f20 7661 6c69 6461 7465 2e0a  ue to validate..
-00001a00: 0a20 2020 2052 6169 7365 730a 2020 2020  .    Raises.    
-00001a10: 2d2d 2d2d 2d2d 0a20 2020 2056 616c 7565  ------.    Value
-00001a20: 4572 726f 720a 2020 2020 2020 2020 4966  Error.        If
-00001a30: 2074 6865 2076 616c 6964 6174 696f 6e20   the validation 
-00001a40: 6661 696c 7320 616e 6420 7468 6520 7661  fails and the va
-00001a50: 6c69 6461 7469 6f6e 206d 6f64 6520 6973  lidation mode is
-00001a60: 2073 6574 2074 6f0a 2020 2020 2020 2020   set to.        
-00001a70: 6052 4149 5345 602e 0a20 2020 2022 2222  `RAISE`..    """
-00001a80: 0a20 2020 2076 616c 6964 6174 655f 7661  .    validate_va
-00001a90: 6c75 6528 2250 4e22 2c20 7661 6c75 652c  lue("PN", value,
-00001aa0: 2063 6f6e 6669 672e 7365 7474 696e 6773   config.settings
-00001ab0: 2e77 7269 7469 6e67 5f76 616c 6964 6174  .writing_validat
-00001ac0: 696f 6e5f 6d6f 6465 2c0a 2020 2020 2020  ion_mode,.      
-00001ad0: 2020 2020 2020 2020 2020 2020 2076 616c               val
-00001ae0: 6964 6174 655f 706e 5f63 6f6d 706f 6e65  idate_pn_compone
-00001af0: 6e74 5f6c 656e 6774 6829 0a0a 0a56 414c  nt_length)...VAL
-00001b00: 4944 4154 4f52 5320 3d20 7b0a 2020 2020  IDATORS = {.    
-00001b10: 2241 4522 3a20 7661 6c69 6461 7465 5f6c  "AE": validate_l
-00001b20: 656e 6774 685f 616e 645f 7265 6765 782c  ength_and_regex,
-00001b30: 0a20 2020 2022 4153 223a 2076 616c 6964  .    "AS": valid
-00001b40: 6174 655f 7265 6765 782c 0a20 2020 2022  ate_regex,.    "
-00001b50: 4353 223a 2076 616c 6964 6174 655f 6c65  CS": validate_le
-00001b60: 6e67 7468 5f61 6e64 5f72 6567 6578 2c0a  ngth_and_regex,.
-00001b70: 2020 2020 2244 4122 3a20 7661 6c69 6461      "DA": valida
-00001b80: 7465 5f72 6567 6578 2c0a 2020 2020 2244  te_regex,.    "D
-00001b90: 5322 3a20 7661 6c69 6461 7465 5f6c 656e  S": validate_len
-00001ba0: 6774 685f 616e 645f 7265 6765 782c 0a20  gth_and_regex,. 
-00001bb0: 2020 2022 4454 223a 2076 616c 6964 6174     "DT": validat
-00001bc0: 655f 7265 6765 782c 0a20 2020 2022 4953  e_regex,.    "IS
-00001bd0: 223a 2076 616c 6964 6174 655f 6c65 6e67  ": validate_leng
-00001be0: 7468 5f61 6e64 5f72 6567 6578 2c0a 2020  th_and_regex,.  
-00001bf0: 2020 224c 4f22 3a20 7661 6c69 6461 7465    "LO": validate
-00001c00: 5f76 725f 6c65 6e67 7468 2c0a 2020 2020  _vr_length,.    
-00001c10: 224c 5422 3a20 7661 6c69 6461 7465 5f76  "LT": validate_v
-00001c20: 725f 6c65 6e67 7468 2c0a 2020 2020 2250  r_length,.    "P
-00001c30: 4e22 3a20 7661 6c69 6461 7465 5f70 6e2c  N": validate_pn,
-00001c40: 0a20 2020 2022 5348 223a 2076 616c 6964  .    "SH": valid
-00001c50: 6174 655f 7672 5f6c 656e 6774 682c 0a20  ate_vr_length,. 
-00001c60: 2020 2022 5354 223a 2076 616c 6964 6174     "ST": validat
-00001c70: 655f 7672 5f6c 656e 6774 682c 0a20 2020  e_vr_length,.   
-00001c80: 2022 544d 223a 2076 616c 6964 6174 655f   "TM": validate_
-00001c90: 7265 6765 782c 0a20 2020 2022 5549 223a  regex,.    "UI":
-00001ca0: 2076 616c 6964 6174 655f 6c65 6e67 7468   validate_length
-00001cb0: 5f61 6e64 5f72 6567 6578 2c0a 2020 2020  _and_regex,.    
-00001cc0: 2255 5222 3a20 7661 6c69 6461 7465 5f72  "UR": validate_r
-00001cd0: 6567 6578 2c0a 7d0a 0a0a 6465 6620 7661  egex,.}...def va
-00001ce0: 6c69 6461 7465 5f76 616c 7565 2876 723a  lidate_value(vr:
-00001cf0: 2073 7472 2c20 7661 6c75 653a 2041 6e79   str, value: Any
-00001d00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001d10: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
-00001d20: 6d6f 6465 3a20 696e 742c 0a20 2020 2020  mode: int,.     
-00001d30: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00001d40: 6c69 6461 746f 723a 204f 7074 696f 6e61  lidator: Optiona
-00001d50: 6c5b 4361 6c6c 6162 6c65 5b5b 7374 722c  l[Callable[[str,
-00001d60: 2041 6e79 5d2c 0a20 2020 2020 2020 2020   Any],.         
-00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 2020 2020 2020 2020 2020 2020 2020 5475                Tu
-00001d90: 706c 655b 626f 6f6c 2c20 7374 725d 5d5d  ple[bool, str]]]
-00001da0: 203d 204e 6f6e 6529 202d 3e20 4e6f 6e65   = None) -> None
-00001db0: 3a0a 2020 2020 2222 2256 616c 6964 6174  :.    """Validat
-00001dc0: 6520 7468 6520 6769 7665 6e20 7661 6c75  e the given valu
-00001dd0: 6520 6167 6169 6e73 7420 7468 6520 4449  e against the DI
-00001de0: 434f 4d20 7374 616e 6461 7264 2e0a 0a20  COM standard... 
-00001df0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00001e00: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00001e10: 2076 7220 3a20 7374 720a 2020 2020 2020   vr : str.      
-00001e20: 2020 5468 6520 5652 206f 6620 7468 6520    The VR of the 
-00001e30: 7461 6720 7468 6520 7661 6c75 6520 6973  tag the value is
-00001e40: 2061 6464 6564 2074 6f2e 0a20 2020 2076   added to..    v
-00001e50: 616c 7565 203a 2041 6e79 0a20 2020 2020  alue : Any.     
-00001e60: 2020 2054 6865 2076 616c 7565 2074 6f20     The value to 
-00001e70: 6265 2076 616c 6964 6174 6564 2e0a 2020  be validated..  
-00001e80: 2020 7661 6c69 6461 7469 6f6e 5f6d 6f64    validation_mod
-00001e90: 6520 3a20 696e 740a 2020 2020 2020 2020  e : int.        
-00001ea0: 4465 6669 6e65 7320 6966 2076 616c 7565  Defines if value
-00001eb0: 7320 6172 6520 7661 6c69 6461 7465 6420  s are validated 
-00001ec0: 616e 6420 686f 7720 7661 6c69 6461 7469  and how validati
-00001ed0: 6f6e 2065 7272 6f72 7320 6172 650a 2020  on errors are.  
-00001ee0: 2020 2020 2020 6861 6e64 6c65 642e 0a20        handled.. 
-00001ef0: 2020 2076 616c 6964 6174 6f72 203a 2043     validator : C
-00001f00: 616c 6c61 626c 6520 6f72 204e 6f6e 650a  allable or None.
-00001f10: 2020 2020 2020 2020 4675 6e63 7469 6f6e          Function
-00001f20: 2074 6861 7420 646f 6573 2074 6865 2061   that does the a
-00001f30: 6374 7561 6c20 7661 6c69 6461 7469 6f6e  ctual validation
-00001f40: 2e20 4966 206e 6f74 2067 6976 656e 2c0a  . If not given,.
-00001f50: 2020 2020 2020 2020 7468 6520 7661 6c69          the vali
-00001f60: 6461 746f 7220 6973 2074 616b 656e 2066  dator is taken f
-00001f70: 726f 6d20 7468 6520 5652 2d73 7065 6369  rom the VR-speci
-00001f80: 6669 6320 7661 6c69 6461 746f 7220 7461  fic validator ta
-00001f90: 626c 6520 696e 7374 6561 642e 0a0a 2020  ble instead...  
-00001fa0: 2020 5261 6973 6573 0a20 2020 202d 2d2d    Raises.    ---
-00001fb0: 2d2d 2d0a 2020 2020 5661 6c75 6545 7272  ---.    ValueErr
-00001fc0: 6f72 0a20 2020 2020 2020 2049 6620 7468  or.        If th
-00001fd0: 6520 7661 6c69 6461 7469 6f6e 2066 6169  e validation fai
-00001fe0: 6c73 2061 6e64 2074 6865 2076 616c 6964  ls and the valid
-00001ff0: 6174 696f 6e20 6d6f 6465 2069 7320 7365  ation mode is se
-00002000: 7420 746f 0a20 2020 2020 2020 2060 5241  t to.        `RA
-00002010: 4953 4560 2e0a 2020 2020 2222 220a 2020  ISE`..    """.  
-00002020: 2020 6966 2076 616c 6964 6174 696f 6e5f    if validation_
-00002030: 6d6f 6465 203d 3d20 636f 6e66 6967 2e49  mode == config.I
-00002040: 474e 4f52 453a 0a20 2020 2020 2020 2072  GNORE:.        r
-00002050: 6574 7572 6e0a 0a20 2020 2069 6620 7661  eturn..    if va
-00002060: 6c75 6520 6973 206e 6f74 204e 6f6e 6520  lue is not None 
-00002070: 616e 6420 6973 696e 7374 616e 6365 2876  and isinstance(v
-00002080: 616c 7565 2c20 2873 7472 2c20 6279 7465  alue, (str, byte
-00002090: 7329 293a 0a20 2020 2020 2020 2076 616c  s)):.        val
-000020a0: 6964 6174 6f72 203d 2076 616c 6964 6174  idator = validat
-000020b0: 6f72 206f 7220 5641 4c49 4441 544f 5253  or or VALIDATORS
-000020c0: 2e67 6574 2876 7229 0a20 2020 2020 2020  .get(vr).       
-000020d0: 2069 6620 7661 6c69 6461 746f 7220 6973   if validator is
-000020e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000020f0: 2020 2020 2020 2069 735f 7661 6c69 642c         is_valid,
-00002100: 206d 7367 203d 2076 616c 6964 6174 6f72   msg = validator
-00002110: 2876 722c 2076 616c 7565 290a 2020 2020  (vr, value).    
-00002120: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00002130: 735f 7661 6c69 643a 0a20 2020 2020 2020  s_valid:.       
-00002140: 2020 2020 2020 2020 2069 6620 7661 6c69           if vali
-00002150: 6461 7469 6f6e 5f6d 6f64 6520 3d3d 2063  dation_mode == c
-00002160: 6f6e 6669 672e 5241 4953 453a 0a20 2020  onfig.RAISE:.   
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00002190: 7228 6d73 6729 0a20 2020 2020 2020 2020  r(msg).         
-000021a0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-000021b0: 7761 726e 286d 7367 290a 0a0a 4075 6e69  warn(msg)...@uni
-000021c0: 7175 650a 636c 6173 7320 5652 2873 7472  que.class VR(str
-000021d0: 2c20 456e 756d 293a 0a20 2020 2022 2222  , Enum):.    """
-000021e0: 4449 434f 4d20 4461 7461 2045 6c65 6d65  DICOM Data Eleme
-000021f0: 6e74 2773 2056 616c 7565 2052 6570 7265  nt's Value Repre
-00002200: 7365 6e74 6174 696f 6e20 2856 5229 2222  sentation (VR)""
-00002210: 220a 2020 2020 2320 5374 616e 6461 7264  ".    # Standard
-00002220: 2056 5273 2066 726f 6d20 5461 626c 6520   VRs from Table 
-00002230: 362e 322d 3120 696e 2050 6172 7420 350a  6.2-1 in Part 5.
-00002240: 2020 2020 4145 203d 2022 4145 220a 2020      AE = "AE".  
-00002250: 2020 4153 203d 2022 4153 220a 2020 2020    AS = "AS".    
-00002260: 4154 203d 2022 4154 220a 2020 2020 4353  AT = "AT".    CS
-00002270: 203d 2022 4353 220a 2020 2020 4441 203d   = "CS".    DA =
-00002280: 2022 4441 220a 2020 2020 4453 203d 2022   "DA".    DS = "
-00002290: 4453 220a 2020 2020 4454 203d 2022 4454  DS".    DT = "DT
-000022a0: 220a 2020 2020 4644 203d 2022 4644 220a  ".    FD = "FD".
-000022b0: 2020 2020 464c 203d 2022 464c 220a 2020      FL = "FL".  
-000022c0: 2020 4953 203d 2022 4953 220a 2020 2020    IS = "IS".    
-000022d0: 4c4f 203d 2022 4c4f 220a 2020 2020 4c54  LO = "LO".    LT
-000022e0: 203d 2022 4c54 220a 2020 2020 4f42 203d   = "LT".    OB =
-000022f0: 2022 4f42 220a 2020 2020 4f44 203d 2022   "OB".    OD = "
-00002300: 4f44 220a 2020 2020 4f46 203d 2022 4f46  OD".    OF = "OF
-00002310: 220a 2020 2020 4f4c 203d 2022 4f4c 220a  ".    OL = "OL".
-00002320: 2020 2020 4f57 203d 2022 4f57 220a 2020      OW = "OW".  
-00002330: 2020 4f56 203d 2022 4f56 220a 2020 2020    OV = "OV".    
-00002340: 504e 203d 2022 504e 220a 2020 2020 5348  PN = "PN".    SH
-00002350: 203d 2022 5348 220a 2020 2020 534c 203d   = "SH".    SL =
-00002360: 2022 534c 220a 2020 2020 5351 203d 2022   "SL".    SQ = "
-00002370: 5351 220a 2020 2020 5353 203d 2022 5353  SQ".    SS = "SS
-00002380: 220a 2020 2020 5354 203d 2022 5354 220a  ".    ST = "ST".
-00002390: 2020 2020 5356 203d 2022 5356 220a 2020      SV = "SV".  
-000023a0: 2020 544d 203d 2022 544d 220a 2020 2020    TM = "TM".    
-000023b0: 5543 203d 2022 5543 220a 2020 2020 5549  UC = "UC".    UI
-000023c0: 203d 2022 5549 220a 2020 2020 554c 203d   = "UI".    UL =
-000023d0: 2022 554c 220a 2020 2020 554e 203d 2022   "UL".    UN = "
-000023e0: 554e 220a 2020 2020 5552 203d 2022 5552  UN".    UR = "UR
-000023f0: 220a 2020 2020 5553 203d 2022 5553 220a  ".    US = "US".
-00002400: 2020 2020 5554 203d 2022 5554 220a 2020      UT = "UT".  
-00002410: 2020 5556 203d 2022 5556 220a 2020 2020    UV = "UV".    
-00002420: 2320 416d 6269 6775 6f75 7320 5652 7320  # Ambiguous VRs 
-00002430: 6672 6f6d 2054 6162 6c65 7320 362d 312c  from Tables 6-1,
-00002440: 2037 2d31 2061 6e64 2038 2d31 2069 6e20   7-1 and 8-1 in 
-00002450: 5061 7274 2036 0a20 2020 2055 535f 5353  Part 6.    US_SS
-00002460: 5f4f 5720 3d20 2255 5320 6f72 2053 5320  _OW = "US or SS 
-00002470: 6f72 204f 5722 0a20 2020 2055 535f 5353  or OW".    US_SS
-00002480: 203d 2022 5553 206f 7220 5353 220a 2020   = "US or SS".  
-00002490: 2020 5553 5f4f 5720 3d20 2255 5320 6f72    US_OW = "US or
-000024a0: 204f 5722 0a20 2020 204f 425f 4f57 203d   OW".    OB_OW =
-000024b0: 2022 4f42 206f 7220 4f57 220a 0a0a 2320   "OB or OW"...# 
-000024c0: 5374 616e 6461 7264 2056 5273 2066 726f  Standard VRs fro
-000024d0: 6d20 5461 626c 6520 362e 322d 3120 696e  m Table 6.2-1 in
-000024e0: 2050 6172 7420 350a 5354 414e 4441 5244   Part 5.STANDARD
-000024f0: 5f56 5220 3d20 7b0a 2020 2020 5652 2e41  _VR = {.    VR.A
-00002500: 452c 2056 522e 4153 2c20 5652 2e41 542c  E, VR.AS, VR.AT,
-00002510: 2056 522e 4353 2c20 5652 2e44 412c 2056   VR.CS, VR.DA, V
-00002520: 522e 4453 2c20 5652 2e44 542c 2056 522e  R.DS, VR.DT, VR.
-00002530: 4644 2c20 5652 2e46 4c2c 2056 522e 4953  FD, VR.FL, VR.IS
-00002540: 2c0a 2020 2020 5652 2e4c 4f2c 2056 522e  ,.    VR.LO, VR.
-00002550: 4c54 2c20 5652 2e4f 422c 2056 522e 4f44  LT, VR.OB, VR.OD
-00002560: 2c20 5652 2e4f 462c 2056 522e 4f4c 2c20  , VR.OF, VR.OL, 
-00002570: 5652 2e4f 572c 2056 522e 4f56 2c20 5652  VR.OW, VR.OV, VR
-00002580: 2e50 4e2c 2056 522e 5348 2c0a 2020 2020  .PN, VR.SH,.    
-00002590: 5652 2e53 4c2c 2056 522e 5351 2c20 5652  VR.SL, VR.SQ, VR
-000025a0: 2e53 532c 2056 522e 5354 2c20 5652 2e53  .SS, VR.ST, VR.S
-000025b0: 562c 2056 522e 544d 2c20 5652 2e55 432c  V, VR.TM, VR.UC,
-000025c0: 2056 522e 5549 2c20 5652 2e55 4c2c 2056   VR.UI, VR.UL, V
-000025d0: 522e 554e 2c0a 2020 2020 5652 2e55 522c  R.UN,.    VR.UR,
-000025e0: 2056 522e 5553 2c20 5652 2e55 542c 2056   VR.US, VR.UT, V
-000025f0: 522e 5556 2c0a 7d0a 2320 416d 6269 6775  R.UV,.}.# Ambigu
-00002600: 6f75 7320 5652 7320 6672 6f6d 2054 6162  ous VRs from Tab
-00002610: 6c65 7320 362d 312c 2037 2d31 2061 6e64  les 6-1, 7-1 and
-00002620: 2038 2d31 2069 6e20 5061 7274 2036 0a41   8-1 in Part 6.A
-00002630: 4d42 4947 554f 5553 5f56 5220 3d20 7b56  MBIGUOUS_VR = {V
-00002640: 522e 5553 5f53 535f 4f57 2c20 5652 2e55  R.US_SS_OW, VR.U
-00002650: 535f 5353 2c20 5652 2e55 535f 4f57 2c20  S_SS, VR.US_OW, 
-00002660: 5652 2e4f 425f 4f57 7d0a 0a23 2043 6861  VR.OB_OW}..# Cha
-00002670: 7261 6374 6572 2052 6570 6572 746f 6972  racter Repertoir
-00002680: 6520 666f 7220 5652 730a 2320 416c 6c6f  e for VRs.# Allo
-00002690: 7765 6420 6368 6172 6163 7465 7220 7265  wed character re
-000026a0: 7065 7274 6f69 7265 2066 6f72 2073 7472  pertoire for str
-000026b0: 2d6c 696b 6520 5652 732c 2062 6173 6564  -like VRs, based
-000026c0: 206f 6666 206f 6620 7468 6520 696e 666f   off of the info
-000026d0: 726d 6174 696f 6e0a 2320 2020 696e 2053  rmation.#   in S
-000026e0: 6563 7469 6f6e 2036 2e31 2e32 2061 6e64  ection 6.1.2 and
-000026f0: 2054 6162 6c65 2036 2e32 2d31 2069 6e20   Table 6.2-1 in 
-00002700: 5061 7274 2035 0a23 2042 6173 6963 2047  Part 5.# Basic G
-00002710: 3020 7365 7420 6f66 2049 534f 2036 3436  0 set of ISO 646
-00002720: 2028 4953 4f2d 4952 2036 2920 6f6e 6c79   (ISO-IR 6) only
-00002730: 0a44 4546 4155 4c54 5f43 4841 5253 4554  .DEFAULT_CHARSET
-00002740: 5f56 5220 3d20 7b0a 2020 2020 5652 2e41  _VR = {.    VR.A
-00002750: 452c 2056 522e 4153 2c20 5652 2e43 532c  E, VR.AS, VR.CS,
-00002760: 2056 522e 4441 2c20 5652 2e44 532c 2056   VR.DA, VR.DS, V
-00002770: 522e 4454 2c20 5652 2e49 532c 2056 522e  R.DT, VR.IS, VR.
-00002780: 544d 2c20 5652 2e55 492c 2056 522e 5552  TM, VR.UI, VR.UR
-00002790: 0a7d 0a23 2042 6173 6963 2047 3020 7365  .}.# Basic G0 se
-000027a0: 7420 6f66 2049 534f 2036 3436 206f 7220  t of ISO 646 or 
-000027b0: 6578 7465 6e73 6962 6c65 2f72 6570 6c61  extensible/repla
-000027c0: 6365 6162 6c65 2062 790a 2320 2020 2830  ceable by.#   (0
-000027d0: 3030 382c 3030 3035 2920 2a53 7065 6369  008,0005) *Speci
-000027e0: 6669 6320 4368 6172 6163 7465 7220 5365  fic Character Se
-000027f0: 742a 0a43 5553 544f 4d49 5a41 424c 455f  t*.CUSTOMIZABLE_
-00002800: 4348 4152 5345 545f 5652 203d 207b 5652  CHARSET_VR = {VR
-00002810: 2e4c 4f2c 2056 522e 4c54 2c20 5652 2e50  .LO, VR.LT, VR.P
-00002820: 4e2c 2056 522e 5348 2c20 5652 2e53 542c  N, VR.SH, VR.ST,
-00002830: 2056 522e 5543 2c20 5652 2e55 547d 0a0a   VR.UC, VR.UT}..
-00002840: 2320 436f 7272 6573 706f 6e64 696e 6720  # Corresponding 
-00002850: 5079 7468 6f6e 2062 7569 6c74 2d69 6e20  Python built-in 
-00002860: 666f 7220 6561 6368 2056 520a 2320 2020  for each VR.#   
-00002870: 466f 7220 736f 6d65 2056 5273 2074 6869  For some VRs thi
-00002880: 7320 6973 206d 6f72 6520 6120 2266 616c  s is more a "fal
-00002890: 6c62 6163 6b22 2063 6c61 7373 2d6c 696b  lback" class-lik
-000028a0: 6520 6265 6861 7669 6f75 7261 6c20 6465  e behavioural de
-000028b0: 6669 6e69 7469 6f6e 0a23 2020 2074 6861  finition.#   tha
-000028c0: 6e20 6163 7475 616c 2c20 616e 6420 6e6f  n actual, and no
-000028d0: 7465 2074 6861 7420 736f 6d65 2056 5273  te that some VRs
-000028e0: 2073 7563 6820 6173 2049 5320 616e 6420   such as IS and 
-000028f0: 4453 2061 7265 2070 7265 7365 6e74 2069  DS are present i
-00002900: 6e0a 2320 2020 6d75 6c74 6970 6c65 2073  n.#   multiple s
-00002910: 6574 730a 4259 5445 535f 5652 203d 207b  ets.BYTES_VR = {
-00002920: 5652 2e4f 422c 2056 522e 4f44 2c20 5652  VR.OB, VR.OD, VR
-00002930: 2e4f 462c 2056 522e 4f4c 2c20 5652 2e4f  .OF, VR.OL, VR.O
-00002940: 562c 2056 522e 4f57 2c20 5652 2e55 4e7d  V, VR.OW, VR.UN}
-00002950: 0a46 4c4f 4154 5f56 5220 3d20 7b56 522e  .FLOAT_VR = {VR.
-00002960: 4453 2c20 5652 2e46 442c 2056 522e 464c  DS, VR.FD, VR.FL
-00002970: 7d0a 494e 545f 5652 203d 207b 5652 2e41  }.INT_VR = {VR.A
-00002980: 542c 2056 522e 4953 2c20 5652 2e53 4c2c  T, VR.IS, VR.SL,
-00002990: 2056 522e 5353 2c20 5652 2e53 562c 2056   VR.SS, VR.SV, V
-000029a0: 522e 554c 2c20 5652 2e55 532c 2056 522e  R.UL, VR.US, VR.
-000029b0: 5556 7d0a 4c49 5354 5f56 5220 3d20 7b56  UV}.LIST_VR = {V
-000029c0: 522e 5351 7d0a 5354 525f 5652 203d 2044  R.SQ}.STR_VR = D
-000029d0: 4546 4155 4c54 5f43 4841 5253 4554 5f56  EFAULT_CHARSET_V
-000029e0: 5220 7c20 4355 5354 4f4d 495a 4142 4c45  R | CUSTOMIZABLE
-000029f0: 5f43 4841 5253 4554 5f56 520a 0a23 2054  _CHARSET_VR..# T
-00002a00: 6865 7365 2056 5273 206d 6179 2068 6176  hese VRs may hav
-00002a10: 6520 6261 636b 736c 6173 6820 6368 6172  e backslash char
-00002a20: 6163 7465 7273 206f 7220 656e 636f 6465  acters or encode
-00002a30: 6420 6261 636b 736c 6173 6865 7320 696e  d backslashes in
-00002a40: 2074 6865 0a23 2020 2076 616c 7565 2062   the.#   value b
-00002a50: 6173 6564 206f 6666 206f 6620 7468 6520  ased off of the 
-00002a60: 696e 666f 726d 6174 696f 6e20 696e 2054  information in T
-00002a70: 6162 6c65 2036 2e32 2d31 2069 6e20 5061  able 6.2-1 in Pa
-00002a80: 7274 2035 0a23 2044 6174 6145 6c65 6d65  rt 5.# DataEleme
-00002a90: 6e74 7320 7769 7468 2061 6d62 6967 756f  nts with ambiguo
-00002aa0: 7573 2056 5273 206d 6179 2075 7365 2060  us VRs may use `
-00002ab0: 6279 7465 7360 2076 616c 7565 7320 616e  bytes` values an
-00002ac0: 6420 736f 2061 7265 2061 6c6c 6f77 6564  d so are allowed
-00002ad0: 0a23 2020 2074 6f20 6861 7665 2062 6163  .#   to have bac
-00002ae0: 6b73 6c61 7368 6573 2028 6578 6365 7074  kslashes (except
-00002af0: 2027 5553 206f 7220 5353 2729 0a41 4c4c   'US or SS').ALL
-00002b00: 4f57 5f42 4143 4b53 4c41 5348 203d 2028  OW_BACKSLASH = (
-00002b10: 0a20 2020 207b 5652 2e4c 542c 2056 522e  .    {VR.LT, VR.
-00002b20: 5354 2c20 5652 2e55 542c 2056 522e 5553  ST, VR.UT, VR.US
-00002b30: 5f53 535f 4f57 2c20 5652 2e55 535f 4f57  _SS_OW, VR.US_OW
-00002b40: 2c20 5652 2e4f 425f 4f57 7d20 7c20 4259  , VR.OB_OW} | BY
-00002b50: 5445 535f 5652 0a29 0a0a 2320 5652 7320  TES_VR.)..# VRs 
-00002b60: 7768 6963 6820 6d61 7920 6861 7665 2061  which may have a
-00002b70: 2076 616c 7565 206d 6f72 6520 7468 616e   value more than
-00002b80: 2031 3032 3420 6279 7465 7320 6f72 2063   1024 bytes or c
-00002b90: 6861 7261 6374 6572 7320 6c6f 6e67 0a23  haracters long.#
-00002ba0: 2020 2055 7365 6420 746f 2066 6c61 6720     Used to flag 
-00002bb0: 7768 6963 6820 7661 6c75 6573 206d 6179  which values may
-00002bc0: 206e 6565 6420 7368 6f72 7465 6e69 6e67   need shortening
-00002bd0: 2064 7572 696e 6720 7072 696e 7469 6e67   during printing
-00002be0: 0a4c 4f4e 475f 5641 4c55 455f 5652 203d  .LONG_VALUE_VR =
-00002bf0: 207b 5652 2e4c 542c 2056 522e 5543 2c20   {VR.LT, VR.UC, 
-00002c00: 5652 2e55 547d 207c 2042 5954 4553 5f56  VR.UT} | BYTES_V
-00002c10: 5220 7c20 414d 4249 4755 4f55 535f 5652  R | AMBIGUOUS_VR
-00002c20: 0a0a 2320 5652 7320 7468 6174 2075 7365  ..# VRs that use
-00002c30: 2032 2062 7974 6520 6c65 6e67 7468 2066   2 byte length f
-00002c40: 6965 6c64 7320 666f 7220 4578 706c 6963  ields for Explic
-00002c50: 6974 2056 5220 6672 6f6d 2054 6162 6c65  it VR from Table
-00002c60: 2037 2e31 2d32 2069 6e20 5061 7274 2035   7.1-2 in Part 5
-00002c70: 0a23 2020 2041 6c6c 206f 7468 6572 2065  .#   All other e
-00002c80: 7870 6c69 6369 7420 5652 7320 616e 6420  xplicit VRs and 
-00002c90: 616c 6c20 696d 706c 6963 6974 2056 5273  all implicit VRs
-00002ca0: 2075 7365 2034 2062 7974 6520 6c65 6e67   use 4 byte leng
-00002cb0: 7468 2066 6965 6c64 730a 4558 504c 4943  th fields.EXPLIC
-00002cc0: 4954 5f56 525f 4c45 4e47 5448 5f31 3620  IT_VR_LENGTH_16 
-00002cd0: 3d20 7b0a 2020 2020 5652 2e41 452c 2056  = {.    VR.AE, V
-00002ce0: 522e 4153 2c20 5652 2e41 542c 2056 522e  R.AS, VR.AT, VR.
-00002cf0: 4353 2c20 5652 2e44 412c 2056 522e 4453  CS, VR.DA, VR.DS
-00002d00: 2c20 5652 2e44 542c 2056 522e 464c 2c20  , VR.DT, VR.FL, 
-00002d10: 5652 2e46 442c 2056 522e 4953 2c0a 2020  VR.FD, VR.IS,.  
-00002d20: 2020 5652 2e4c 4f2c 2056 522e 4c54 2c20    VR.LO, VR.LT, 
-00002d30: 5652 2e50 4e2c 2056 522e 5348 2c20 5652  VR.PN, VR.SH, VR
-00002d40: 2e53 4c2c 2056 522e 5353 2c20 5652 2e53  .SL, VR.SS, VR.S
-00002d50: 542c 2056 522e 544d 2c20 5652 2e55 492c  T, VR.TM, VR.UI,
-00002d60: 2056 522e 554c 2c0a 2020 2020 5652 2e55   VR.UL,.    VR.U
-00002d70: 532c 0a7d 0a45 5850 4c49 4349 545f 5652  S,.}.EXPLICIT_VR
-00002d80: 5f4c 454e 4754 485f 3332 203d 2053 5441  _LENGTH_32 = STA
-00002d90: 4e44 4152 445f 5652 202d 2045 5850 4c49  NDARD_VR - EXPLI
-00002da0: 4349 545f 5652 5f4c 454e 4754 485f 3136  CIT_VR_LENGTH_16
-00002db0: 0a0a 0a63 6c61 7373 205f 4461 7465 5469  ...class _DateTi
-00002dc0: 6d65 4261 7365 3a0a 2020 2020 2222 2242  meBase:.    """B
-00002dd0: 6173 6520 636c 6173 7320 666f 7220 4454  ase class for DT
-00002de0: 2c20 4441 2061 6e64 2054 4d20 656c 656d  , DA and TM elem
-00002df0: 656e 7420 7375 622d 636c 6173 7365 732e  ent sub-classes.
-00002e00: 2222 220a 2020 2020 6f72 6967 696e 616c  """.    original
-00002e10: 5f73 7472 696e 673a 2073 7472 0a0a 2020  _string: str..  
-00002e20: 2020 2320 4164 6420 7069 636b 6c69 6e67    # Add pickling
-00002e30: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
-00002e40: 206d 7574 6162 6c65 2061 6464 6974 696f   mutable additio
-00002e50: 6e73 0a20 2020 2064 6566 205f 5f67 6574  ns.    def __get
-00002e60: 7374 6174 655f 5f28 7365 6c66 2920 2d3e  state__(self) ->
-00002e70: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
-00002e80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002e90: 7365 6c66 2e5f 5f64 6963 745f 5f2e 636f  self.__dict__.co
-00002ea0: 7079 2829 0a0a 2020 2020 6465 6620 5f5f  py()..    def __
-00002eb0: 7365 7473 7461 7465 5f5f 2873 656c 662c  setstate__(self,
-00002ec0: 2073 7461 7465 3a20 4469 6374 5b73 7472   state: Dict[str
-00002ed0: 2c20 416e 795d 2920 2d3e 204e 6f6e 653a  , Any]) -> None:
-00002ee0: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-00002ef0: 6469 6374 5f5f 2e75 7064 6174 6528 7374  dict__.update(st
-00002f00: 6174 6529 0a0a 2020 2020 6465 6620 5f5f  ate)..    def __
-00002f10: 7265 6475 6365 5f65 785f 5f28 2020 2320  reduce_ex__(  # 
-00002f20: 7479 7065 3a20 6967 6e6f 7265 5b6f 7665  type: ignore[ove
-00002f30: 7272 6964 655d 0a20 2020 2020 2020 2073  rride].        s
-00002f40: 656c 662c 2070 726f 746f 636f 6c3a 2069  elf, protocol: i
-00002f50: 6e74 0a20 2020 2029 202d 3e20 5475 706c  nt.    ) -> Tupl
-00002f60: 655b 416e 792c 202e 2e2e 5d3a 0a20 2020  e[Any, ...]:.   
-00002f70: 2020 2020 2023 2050 7974 686f 6e20 332e       # Python 3.
-00002f80: 3820 2d20 7072 6f74 6f63 6f6c 3a20 5375  8 - protocol: Su
-00002f90: 7070 6f72 7473 496e 6465 7820 2861 6464  pportsIndex (add
-00002fa0: 6564 2069 6e20 332e 3829 0a20 2020 2020  ed in 3.8).     
-00002fb0: 2020 2023 2064 6174 6574 696d 652e 7469     # datetime.ti
-00002fc0: 6d65 2c20 616e 6420 6461 7465 7469 6d65  me, and datetime
-00002fd0: 2e64 6174 6574 696d 6520 7265 7475 726e  .datetime return
-00002fe0: 2054 7570 6c65 5b41 6e79 2c20 2e2e 2e5d   Tuple[Any, ...]
-00002ff0: 0a20 2020 2020 2020 2023 2064 6174 6574  .        # datet
-00003000: 696d 652e 6461 7465 2064 6f65 736e 2774  ime.date doesn't
-00003010: 2064 6566 696e 6520 5f5f 7265 6475 6365   define __reduce
-00003020: 5f65 785f 5f0a 2020 2020 2020 2020 7265  _ex__.        re
-00003030: 6475 6365 5f65 7820 3d20 6361 7374 2854  duce_ex = cast(T
-00003040: 7570 6c65 5b41 6e79 2c20 2e2e 2e5d 2c20  uple[Any, ...], 
-00003050: 7375 7065 7228 292e 5f5f 7265 6475 6365  super().__reduce
-00003060: 5f65 785f 5f28 7072 6f74 6f63 6f6c 2929  _ex__(protocol))
-00003070: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003080: 7265 6475 6365 5f65 7820 2b20 2873 656c  reduce_ex + (sel
-00003090: 662e 5f5f 6765 7473 7461 7465 5f5f 2829  f.__getstate__()
-000030a0: 2c29 0a0a 2020 2020 6465 6620 5f5f 7374  ,)..    def __st
-000030b0: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
-000030c0: 3a0a 2020 2020 2020 2020 6966 2068 6173  :.        if has
-000030d0: 6174 7472 2873 656c 662c 2027 6f72 6967  attr(self, 'orig
-000030e0: 696e 616c 5f73 7472 696e 6727 293a 0a20  inal_string'):. 
-000030f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003100: 6e20 7365 6c66 2e6f 7269 6769 6e61 6c5f  n self.original_
-00003110: 7374 7269 6e67 0a0a 2020 2020 2020 2020  string..        
-00003120: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
-00003130: 5f73 7472 5f5f 2829 0a0a 2020 2020 6465  _str__()..    de
-00003140: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-00003150: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00003160: 2072 6574 7572 6e20 6627 227b 7374 7228   return f'"{str(
-00003170: 7365 6c66 297d 2227 0a0a 0a63 6c61 7373  self)}"'...class
-00003180: 2044 4128 5f44 6174 6554 696d 6542 6173   DA(_DateTimeBas
-00003190: 652c 2064 6174 6574 696d 652e 6461 7465  e, datetime.date
-000031a0: 293a 0a20 2020 2022 2222 5374 6f72 6520  ):.    """Store 
-000031b0: 7661 6c75 6520 666f 7220 616e 2065 6c65  value for an ele
-000031c0: 6d65 6e74 2077 6974 6820 5652 202a 2a44  ment with VR **D
-000031d0: 412a 2a20 6173 203a 636c 6173 733a 6064  A** as :class:`d
-000031e0: 6174 6574 696d 652e 6461 7465 602e 0a0a  atetime.date`...
-000031f0: 2020 2020 4e6f 7465 2074 6861 7420 7468      Note that th
-00003200: 6520 3a63 6c61 7373 3a60 6461 7465 7469  e :class:`dateti
-00003210: 6d65 2e64 6174 6560 2062 6173 6520 636c  me.date` base cl
-00003220: 6173 7320 6973 2069 6d6d 7574 6162 6c65  ass is immutable
-00003230: 2e0a 2020 2020 2222 220a 2020 2020 6465  ..    """.    de
-00003240: 6620 5f5f 6e65 775f 5f28 2020 2320 7479  f __new__(  # ty
-00003250: 7065 3a20 6967 6e6f 7265 5b6d 6973 635d  pe: ignore[misc]
-00003260: 0a20 2020 2020 2020 2063 6c73 3a20 5479  .        cls: Ty
-00003270: 7065 5b22 4441 225d 2c20 2a61 7267 733a  pe["DA"], *args:
-00003280: 2041 6e79 2c20 2a2a 6b77 6172 6773 3a20   Any, **kwargs: 
-00003290: 416e 790a 2020 2020 2920 2d3e 204f 7074  Any.    ) -> Opt
-000032a0: 696f 6e61 6c5b 2244 4122 5d3a 0a20 2020  ional["DA"]:.   
-000032b0: 2020 2020 2022 2222 4372 6561 7465 2061       """Create a
-000032c0: 6e20 696e 7374 616e 6365 206f 6620 4441  n instance of DA
-000032d0: 206f 626a 6563 742e 0a0a 2020 2020 2020   object...      
-000032e0: 2020 5261 6973 6520 616e 2065 7863 6570    Raise an excep
-000032f0: 7469 6f6e 2069 6620 7468 6520 7374 7269  tion if the stri
-00003300: 6e67 2063 616e 6e6f 7420 6265 2070 6172  ng cannot be par
-00003310: 7365 6420 6f72 2074 6865 2061 7267 756d  sed or the argum
-00003320: 656e 740a 2020 2020 2020 2020 6973 206f  ent.        is o
-00003330: 7468 6572 7769 7365 2069 6e63 6f6d 7061  therwise incompa
-00003340: 7469 626c 652e 0a0a 2020 2020 2020 2020  tible...        
-00003350: 5468 6520 6172 6775 6d65 6e74 7320 2860  The arguments (`
-00003360: 602a 6172 6773 6060 2061 6e64 2060 602a  `*args`` and ``*
-00003370: 2a6b 7761 7267 7360 6029 2061 7265 2065  *kwargs``) are e
-00003380: 6974 6865 7220 7468 6520 6f6e 6573 0a20  ither the ones. 
-00003390: 2020 2020 2020 2069 6e68 6572 6974 6564         inherited
-000033a0: 2066 726f 6d20 3a63 6c61 7373 3a60 6461   from :class:`da
-000033b0: 7465 7469 6d65 2e64 6174 6560 2c20 6f72  tetime.date`, or
-000033c0: 2074 6865 2066 6972 7374 2061 7267 756d   the first argum
-000033d0: 656e 7420 6973 0a20 2020 2020 2020 2061  ent is.        a
-000033e0: 2073 7472 696e 6720 636f 6e66 6f72 6d61   string conforma
-000033f0: 6e74 2074 6f20 7468 6520 4441 2064 6566  nt to the DA def
-00003400: 696e 6974 696f 6e20 696e 2074 6865 2044  inition in the D
-00003410: 4943 4f4d 2053 7461 6e64 6172 642c 0a20  ICOM Standard,. 
-00003420: 2020 2020 2020 2050 6172 7420 352c 203a         Part 5, :
-00003430: 6463 6d3a 6054 6162 6c65 2036 2e32 2d31  dcm:`Table 6.2-1
-00003440: 3c70 6172 7430 352f 7365 6374 5f36 2e32  <part05/sect_6.2
-00003450: 2e68 746d 6c23 7461 626c 655f 362e 322d  .html#table_6.2-
-00003460: 313e 602c 0a20 2020 2020 2020 206f 7220  1>`,.        or 
-00003470: 6974 2069 7320 6120 3a63 6c61 7373 3a60  it is a :class:`
-00003480: 6461 7465 7469 6d65 2e64 6174 6560 206f  datetime.date` o
-00003490: 626a 6563 742c 206f 7220 616e 206f 626a  bject, or an obj
-000034a0: 6563 7420 6f66 2074 7970 650a 2020 2020  ect of type.    
-000034b0: 2020 2020 3a63 6c61 7373 3a60 7e70 7964      :class:`~pyd
-000034c0: 6963 6f6d 2e76 616c 7565 7265 702e 4441  icom.valuerep.DA
-000034d0: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
-000034e0: 2020 2020 2020 2069 6620 6e6f 7420 6172         if not ar
-000034f0: 6773 206f 7220 6172 6773 5b30 5d20 6973  gs or args[0] is
-00003500: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00003510: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00003520: 2020 2020 2020 2020 7661 6c20 3d20 6172          val = ar
-00003530: 6773 5b30 5d0a 2020 2020 2020 2020 6966  gs[0].        if
-00003540: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
-00003550: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00003560: 2020 2069 6620 7661 6c2e 7374 7269 7028     if val.strip(
-00003570: 2920 3d3d 2027 273a 0a20 2020 2020 2020  ) == '':.       
-00003580: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003590: 4e6f 6e65 2020 2320 656d 7074 7920 6461  None  # empty da
-000035a0: 7465 0a0a 2020 2020 2020 2020 2020 2020  te..            
-000035b0: 6966 206c 656e 2876 616c 2920 3d3d 2038  if len(val) == 8
-000035c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000035d0: 2020 7965 6172 203d 2069 6e74 2876 616c    year = int(val
-000035e0: 5b30 3a34 5d29 0a20 2020 2020 2020 2020  [0:4]).         
-000035f0: 2020 2020 2020 206d 6f6e 7468 203d 2069         month = i
-00003600: 6e74 2876 616c 5b34 3a36 5d29 0a20 2020  nt(val[4:6]).   
-00003610: 2020 2020 2020 2020 2020 2020 2064 6179               day
-00003620: 203d 2069 6e74 2876 616c 5b36 3a38 5d29   = int(val[6:8])
-00003630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003640: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00003650: 5f5f 6e65 775f 5f28 636c 732c 2079 6561  __new__(cls, yea
-00003660: 722c 206d 6f6e 7468 2c20 6461 7929 0a0a  r, month, day)..
-00003670: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00003680: 656e 2876 616c 2920 3d3d 2031 3020 616e  en(val) == 10 an
-00003690: 6420 7661 6c5b 345d 203d 3d20 272e 2720  d val[4] == '.' 
-000036a0: 616e 6420 7661 6c5b 375d 203d 3d20 272e  and val[7] == '.
-000036b0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-000036c0: 2020 2023 2041 4352 2d4e 454d 4120 5374     # ACR-NEMA St
-000036d0: 616e 6461 7264 2033 3030 2c20 7072 6564  andard 300, pred
-000036e0: 6563 6573 736f 7220 746f 2044 4943 4f4d  ecessor to DICOM
-000036f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003700: 2023 2066 6f72 2063 6f6d 7061 7469 6269   # for compatibi
-00003710: 6c69 7479 2077 6974 6820 6120 6665 7720  lity with a few 
-00003720: 6f6c 6420 7079 6469 636f 6d20 6578 616d  old pydicom exam
-00003730: 706c 6520 6669 6c65 730a 2020 2020 2020  ple files.      
-00003740: 2020 2020 2020 2020 2020 7965 6172 203d            year =
-00003750: 2069 6e74 2876 616c 5b30 3a34 5d29 0a20   int(val[0:4]). 
-00003760: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00003770: 6f6e 7468 203d 2069 6e74 2876 616c 5b35  onth = int(val[5
-00003780: 3a37 5d29 0a20 2020 2020 2020 2020 2020  :7]).           
-00003790: 2020 2020 2064 6179 203d 2069 6e74 2876       day = int(v
-000037a0: 616c 5b38 3a31 305d 290a 2020 2020 2020  al[8:10]).      
-000037b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000037c0: 2073 7570 6572 2829 2e5f 5f6e 6577 5f5f   super().__new__
-000037d0: 2863 6c73 2c20 7965 6172 2c20 6d6f 6e74  (cls, year, mont
-000037e0: 682c 2064 6179 290a 0a20 2020 2020 2020  h, day)..       
-000037f0: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
-00003800: 616c 2c20 6461 7465 7469 6d65 2e64 6174  al, datetime.dat
-00003810: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00003820: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
-00003830: 5f6e 6577 5f5f 2863 6c73 2c20 7661 6c2e  _new__(cls, val.
-00003840: 7965 6172 2c20 7661 6c2e 6d6f 6e74 682c  year, val.month,
-00003850: 2076 616c 2e64 6179 290a 0a20 2020 2020   val.day)..     
-00003860: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00003870: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-00003880: 2829 2e5f 5f6e 6577 5f5f 2863 6c73 2c20  ().__new__(cls, 
-00003890: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-000038a0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000038b0: 4578 6365 7074 696f 6e20 6173 2065 7863  Exception as exc
-000038c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000038d0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038f0: 6622 556e 6162 6c65 2074 6f20 636f 6e76  f"Unable to conv
-00003900: 6572 7420 277b 7661 6c7d 2720 746f 2027  ert '{val}' to '
-00003910: 4441 2720 6f62 6a65 6374 220a 2020 2020  DA' object".    
-00003920: 2020 2020 2020 2020 2920 6672 6f6d 2065          ) from e
-00003930: 7863 0a0a 2020 2020 6465 6620 5f5f 696e  xc..    def __in
-00003940: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
-00003950: 3a20 416e 792c 202a 2a6b 7761 7267 733a  : Any, **kwargs:
-00003960: 2041 6e79 2920 2d3e 204e 6f6e 653a 0a20   Any) -> None:. 
-00003970: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
-00003980: 2061 206e 6577 202a 2a44 412a 2a20 656c   a new **DA** el
-00003990: 656d 656e 7420 7661 6c75 652e 2222 220a  ement value.""".
-000039a0: 2020 2020 2020 2020 7661 6c20 3d20 6172          val = ar
-000039b0: 6773 5b30 5d0a 2020 2020 2020 2020 6966  gs[0].        if
-000039c0: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
-000039d0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-000039e0: 2020 2073 656c 662e 6f72 6967 696e 616c     self.original
-000039f0: 5f73 7472 696e 6720 3d20 7661 6c0a 2020  _string = val.  
-00003a00: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00003a10: 7461 6e63 6528 7661 6c2c 2044 4129 2061  tance(val, DA) a
-00003a20: 6e64 2068 6173 6174 7472 2876 616c 2c20  nd hasattr(val, 
-00003a30: 276f 7269 6769 6e61 6c5f 7374 7269 6e67  'original_string
-00003a40: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-00003a50: 7365 6c66 2e6f 7269 6769 6e61 6c5f 7374  self.original_st
-00003a60: 7269 6e67 203d 2076 616c 2e6f 7269 6769  ring = val.origi
-00003a70: 6e61 6c5f 7374 7269 6e67 0a20 2020 2020  nal_string.     
-00003a80: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00003a90: 6365 2876 616c 2c20 6461 7465 7469 6d65  ce(val, datetime
-00003aa0: 2e64 6174 6529 3a0a 2020 2020 2020 2020  .date):.        
-00003ab0: 2020 2020 7365 6c66 2e6f 7269 6769 6e61      self.origina
-00003ac0: 6c5f 7374 7269 6e67 203d 2066 227b 7661  l_string = f"{va
-00003ad0: 6c2e 7965 6172 7d7b 7661 6c2e 6d6f 6e74  l.year}{val.mont
-00003ae0: 683a 3032 7d7b 7661 6c2e 6461 793a 3032  h:02}{val.day:02
-00003af0: 7d22 0a0a 0a63 6c61 7373 2044 5428 5f44  }"...class DT(_D
-00003b00: 6174 6554 696d 6542 6173 652c 2064 6174  ateTimeBase, dat
-00003b10: 6574 696d 652e 6461 7465 7469 6d65 293a  etime.datetime):
-00003b20: 0a20 2020 2022 2222 5374 6f72 6520 7661  .    """Store va
-00003b30: 6c75 6520 666f 7220 616e 2065 6c65 6d65  lue for an eleme
-00003b40: 6e74 2077 6974 6820 5652 202a 2a44 542a  nt with VR **DT*
-00003b50: 2a20 6173 203a 636c 6173 733a 6064 6174  * as :class:`dat
-00003b60: 6574 696d 652e 6461 7465 7469 6d65 602e  etime.datetime`.
-00003b70: 0a0a 2020 2020 4e6f 7465 2074 6861 7420  ..    Note that 
-00003b80: 7468 6520 3a63 6c61 7373 3a60 6461 7465  the :class:`date
-00003b90: 7469 6d65 2e64 6174 6574 696d 6560 2062  time.datetime` b
-00003ba0: 6173 6520 636c 6173 7320 6973 2069 6d6d  ase class is imm
-00003bb0: 7574 6162 6c65 2e0a 2020 2020 2222 220a  utable..    """.
-00003bc0: 2020 2020 5f72 6567 6578 5f64 7420 3d20      _regex_dt = 
-00003bd0: 7265 2e63 6f6d 7069 6c65 2872 2228 285c  re.compile(r"((\
-00003be0: 647b 342c 3134 7d29 285c 2e28 5c64 7b31  d{4,14})(\.(\d{1
-00003bf0: 2c36 7d29 293f 2928 5b2b 2d5d 5c64 7b34  ,6}))?)([+-]\d{4
-00003c00: 7d29 3f22 290a 0a20 2020 2040 7374 6174  })?")..    @stat
-00003c10: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00003c20: 205f 7574 635f 6f66 6673 6574 2876 616c   _utc_offset(val
-00003c30: 7565 3a20 7374 7229 202d 3e20 6461 7465  ue: str) -> date
-00003c40: 7469 6d65 2e74 696d 657a 6f6e 653a 0a20  time.timezone:. 
-00003c50: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00003c60: 2074 6865 2055 5443 204f 6666 7365 7420   the UTC Offset 
-00003c70: 7375 6666 6978 2061 7320 6120 3a63 6c61  suffix as a :cla
-00003c80: 7373 3a60 6461 7465 7469 6d65 2e74 696d  ss:`datetime.tim
-00003c90: 657a 6f6e 6560 2e0a 0a20 2020 2020 2020  ezone`...       
-00003ca0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00003cb0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00003cc0: 2020 2020 2020 2076 616c 7565 203a 2073         value : s
-00003cd0: 7472 0a20 2020 2020 2020 2020 2020 2054  tr.            T
-00003ce0: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00003cf0: 5554 4320 6f66 6673 6574 2073 7566 6669  UTC offset suffi
-00003d00: 782c 2073 7563 6820 6173 2060 6027 2d31  x, such as ``'-1
-00003d10: 3030 3027 6060 206f 720a 2020 2020 2020  000'`` or.      
-00003d20: 2020 2020 2020 6060 272b 3032 3435 2760        ``'+0245'`
-00003d30: 602e 0a0a 2020 2020 2020 2020 5265 7475  `...        Retu
-00003d40: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00003d50: 2d2d 2d0a 2020 2020 2020 2020 6461 7465  ---.        date
-00003d60: 7469 6d65 2e74 696d 657a 6f6e 650a 2020  time.timezone.  
-00003d70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00003d80: 2020 2320 466f 726d 6174 2069 7320 265a    # Format is &Z
-00003d90: 5a58 582c 2026 203d 2027 2b27 206f 7220  ZXX, & = '+' or 
-00003da0: 272d 272c 205a 5a20 6973 2068 6f75 7273  '-', ZZ is hours
-00003db0: 2c20 5858 2069 7320 6d69 6e75 7465 730a  , XX is minutes.
-00003dc0: 2020 2020 2020 2020 686f 7572 203d 2069          hour = i
-00003dd0: 6e74 2876 616c 7565 5b31 3a33 5d29 202a  nt(value[1:3]) *
-00003de0: 2036 3020 2023 2043 6f6e 7665 7274 2068   60  # Convert h
-00003df0: 6f75 7273 2074 6f20 6d69 6e75 7465 730a  ours to minutes.
-00003e00: 2020 2020 2020 2020 6d69 6e75 7465 203d          minute =
-00003e10: 2069 6e74 2876 616c 7565 5b33 3a35 5d29   int(value[3:5])
-00003e20: 2020 2320 496e 206d 696e 7574 6573 0a20    # In minutes. 
-00003e30: 2020 2020 2020 206f 6666 7365 7420 3d20         offset = 
-00003e40: 2868 6f75 7220 2b20 6d69 6e75 7465 2920  (hour + minute) 
-00003e50: 2a20 3630 2020 2320 436f 6e76 6572 7420  * 60  # Convert 
-00003e60: 6d69 6e75 7465 7320 746f 2073 6563 6f6e  minutes to secon
-00003e70: 6473 0a20 2020 2020 2020 206f 6666 7365  ds.        offse
-00003e80: 7420 3d20 2d6f 6666 7365 7420 6966 2076  t = -offset if v
-00003e90: 616c 7565 5b30 5d20 3d3d 2027 2d27 2065  alue[0] == '-' e
-00003ea0: 6c73 6520 6f66 6673 6574 0a0a 2020 2020  lse offset..    
-00003eb0: 2020 2020 7265 7475 726e 2064 6174 6574      return datet
-00003ec0: 696d 652e 7469 6d65 7a6f 6e65 280a 2020  ime.timezone(.  
-00003ed0: 2020 2020 2020 2020 2020 6461 7465 7469            dateti
-00003ee0: 6d65 2e74 696d 6564 656c 7461 2873 6563  me.timedelta(sec
-00003ef0: 6f6e 6473 3d6f 6666 7365 7429 2c0a 2020  onds=offset),.  
-00003f00: 2020 2020 2020 2020 2020 6e61 6d65 3d76            name=v
-00003f10: 616c 7565 0a20 2020 2020 2020 2029 0a0a  alue.        )..
-00003f20: 2020 2020 6465 6620 5f5f 6e65 775f 5f28      def __new__(
-00003f30: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00003f40: 5b6d 6973 635d 0a20 2020 2020 2020 2063  [misc].        c
-00003f50: 6c73 3a20 5479 7065 5b22 4454 225d 2c20  ls: Type["DT"], 
-00003f60: 2a61 7267 733a 2041 6e79 2c20 2a2a 6b77  *args: Any, **kw
-00003f70: 6172 6773 3a20 416e 790a 2020 2020 2920  args: Any.    ) 
-00003f80: 2d3e 204f 7074 696f 6e61 6c5b 2244 5422  -> Optional["DT"
-00003f90: 5d3a 0a20 2020 2020 2020 2022 2222 4372  ]:.        """Cr
-00003fa0: 6561 7465 2061 6e20 696e 7374 616e 6365  eate an instance
-00003fb0: 206f 6620 4454 206f 626a 6563 742e 0a0a   of DT object...
-00003fc0: 2020 2020 2020 2020 5261 6973 6520 616e          Raise an
-00003fd0: 2065 7863 6570 7469 6f6e 2069 6620 7468   exception if th
-00003fe0: 6520 7374 7269 6e67 2063 616e 6e6f 7420  e string cannot 
-00003ff0: 6265 2070 6172 7365 6420 6f72 2074 6865  be parsed or the
-00004000: 2061 7267 756d 656e 740a 2020 2020 2020   argument.      
-00004010: 2020 6973 206f 7468 6572 7769 7365 2069    is otherwise i
-00004020: 6e63 6f6d 7061 7469 626c 652e 0a0a 2020  ncompatible...  
-00004030: 2020 2020 2020 5468 6520 6172 6775 6d65        The argume
-00004040: 6e74 7320 2860 602a 6172 6773 6060 2061  nts (``*args`` a
-00004050: 6e64 2060 602a 2a6b 7761 7267 7360 6029  nd ``**kwargs``)
-00004060: 2061 7265 2065 6974 6865 7220 7468 6520   are either the 
-00004070: 6f6e 6573 0a20 2020 2020 2020 2069 6e68  ones.        inh
-00004080: 6572 6974 6564 2066 726f 6d20 3a63 6c61  erited from :cla
-00004090: 7373 3a60 6461 7465 7469 6d65 2e64 6174  ss:`datetime.dat
-000040a0: 6574 696d 6560 2c20 6f72 2074 6865 2066  etime`, or the f
-000040b0: 6972 7374 2061 7267 756d 656e 7420 6973  irst argument is
-000040c0: 0a20 2020 2020 2020 2061 2073 7472 696e  .        a strin
-000040d0: 6720 636f 6e66 6f72 6d61 6e74 2074 6f20  g conformant to 
-000040e0: 7468 6520 4454 2064 6566 696e 6974 696f  the DT definitio
-000040f0: 6e20 696e 2074 6865 2044 4943 4f4d 2053  n in the DICOM S
-00004100: 7461 6e64 6172 642c 0a20 2020 2020 2020  tandard,.       
-00004110: 2050 6172 7420 352c 203a 6463 6d3a 6054   Part 5, :dcm:`T
-00004120: 6162 6c65 2036 2e32 2d31 3c70 6172 7430  able 6.2-1<part0
-00004130: 352f 7365 6374 5f36 2e32 2e68 746d 6c23  5/sect_6.2.html#
-00004140: 7461 626c 655f 362e 322d 313e 602c 0a20  table_6.2-1>`,. 
-00004150: 2020 2020 2020 206f 7220 6974 2069 7320         or it is 
-00004160: 6120 3a63 6c61 7373 3a60 6461 7465 7469  a :class:`dateti
-00004170: 6d65 2e64 6174 6574 696d 6560 206f 626a  me.datetime` obj
-00004180: 6563 742c 206f 7220 616e 206f 626a 6563  ect, or an objec
-00004190: 7420 6f66 2074 7970 650a 2020 2020 2020  t of type.      
-000041a0: 2020 3a63 6c61 7373 3a60 7e70 7964 6963    :class:`~pydic
-000041b0: 6f6d 2e76 616c 7565 7265 702e 4454 602e  om.valuerep.DT`.
-000041c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000041d0: 2020 2020 2069 6620 6e6f 7420 6172 6773       if not args
-000041e0: 206f 7220 6172 6773 5b30 5d20 6973 204e   or args[0] is N
-000041f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00004200: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00004210: 2020 2020 2020 7661 6c20 3d20 6172 6773        val = args
-00004220: 5b30 5d0a 2020 2020 2020 2020 6966 2069  [0].        if i
-00004230: 7369 6e73 7461 6e63 6528 7661 6c2c 2073  sinstance(val, s
-00004240: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00004250: 2069 6620 7661 6c2e 7374 7269 7028 2920   if val.strip() 
-00004260: 3d3d 2027 273a 0a20 2020 2020 2020 2020  == '':.         
-00004270: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00004280: 6e65 0a0a 2020 2020 2020 2020 2020 2020  ne..            
-00004290: 6d61 7463 6820 3d20 636c 732e 5f72 6567  match = cls._reg
-000042a0: 6578 5f64 742e 6d61 7463 6828 7661 6c29  ex_dt.match(val)
-000042b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000042c0: 6e6f 7420 6d61 7463 6820 6f72 206c 656e  not match or len
-000042d0: 2876 616c 2920 3e20 3236 3a0a 2020 2020  (val) > 26:.    
-000042e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000042f0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004310: 2020 6622 556e 6162 6c65 2074 6f20 636f    f"Unable to co
-00004320: 6e76 6572 7420 6e6f 6e2d 636f 6e66 6f72  nvert non-confor
-00004330: 6d61 6e74 2076 616c 7565 2027 7b76 616c  mant value '{val
-00004340: 7d27 2074 6f20 2744 5427 2022 0a20 2020  }' to 'DT' ".   
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004360: 2022 6f62 6a65 6374 220a 2020 2020 2020   "object".      
-00004370: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00004380: 2020 2020 2020 2020 2064 745f 6d61 7463           dt_matc
-00004390: 6820 3d20 6d61 7463 682e 6772 6f75 7028  h = match.group(
-000043a0: 3229 0a20 2020 2020 2020 2020 2020 2061  2).            a
-000043b0: 7267 7320 3d20 280a 2020 2020 2020 2020  rgs = (.        
-000043c0: 2020 2020 2020 2020 696e 7428 6474 5f6d          int(dt_m
-000043d0: 6174 6368 5b30 3a34 5d29 2c20 2023 2079  atch[0:4]),  # y
-000043e0: 6561 720a 2020 2020 2020 2020 2020 2020  ear.            
-000043f0: 2020 2020 3120 6966 206c 656e 2864 745f      1 if len(dt_
-00004400: 6d61 7463 6829 203c 2036 2065 6c73 6520  match) < 6 else 
-00004410: 696e 7428 6474 5f6d 6174 6368 5b34 3a36  int(dt_match[4:6
-00004420: 5d29 2c20 2023 206d 6f6e 7468 0a20 2020  ]),  # month.   
-00004430: 2020 2020 2020 2020 2020 2020 2031 2069               1 i
-00004440: 6620 6c65 6e28 6474 5f6d 6174 6368 2920  f len(dt_match) 
-00004450: 3c20 3820 656c 7365 2069 6e74 2864 745f  < 8 else int(dt_
-00004460: 6d61 7463 685b 363a 385d 292c 2020 2320  match[6:8]),  # 
-00004470: 6461 790a 2020 2020 2020 2020 2020 2020  day.            
-00004480: 290a 2020 2020 2020 2020 2020 2020 6b77  ).            kw
-00004490: 6172 6773 203d 207b 0a20 2020 2020 2020  args = {.       
-000044a0: 2020 2020 2020 2020 2027 686f 7572 273a           'hour':
-000044b0: 2030 2069 6620 6c65 6e28 6474 5f6d 6174   0 if len(dt_mat
-000044c0: 6368 2920 3c20 3130 2065 6c73 6520 696e  ch) < 10 else in
-000044d0: 7428 6474 5f6d 6174 6368 5b38 3a31 305d  t(dt_match[8:10]
-000044e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000044f0: 2020 2027 6d69 6e75 7465 273a 2030 2069     'minute': 0 i
-00004500: 6620 6c65 6e28 6474 5f6d 6174 6368 2920  f len(dt_match) 
-00004510: 3c20 3132 2065 6c73 6520 696e 7428 6474  < 12 else int(dt
-00004520: 5f6d 6174 6368 5b31 303a 3132 5d29 2c0a  _match[10:12]),.
-00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004540: 2773 6563 6f6e 6427 3a20 3020 6966 206c  'second': 0 if l
-00004550: 656e 2864 745f 6d61 7463 6829 203c 2031  en(dt_match) < 1
-00004560: 3420 656c 7365 2069 6e74 2864 745f 6d61  4 else int(dt_ma
-00004570: 7463 685b 3132 3a31 345d 292c 0a20 2020  tch[12:14]),.   
-00004580: 2020 2020 2020 2020 2020 2020 2027 6d69               'mi
-00004590: 6372 6f73 6563 6f6e 6427 3a20 300a 2020  crosecond': 0.  
-000045a0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000045b0: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
-000045c0: 745f 6d61 7463 6829 203e 3d20 3134 2061  t_match) >= 14 a
-000045d0: 6e64 206d 6174 6368 2e67 726f 7570 2834  nd match.group(4
-000045e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000045f0: 2020 206b 7761 7267 735b 276d 6963 726f     kwargs['micro
-00004600: 7365 636f 6e64 275d 203d 2069 6e74 280a  second'] = int(.
-00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004620: 2020 2020 6d61 7463 682e 6772 6f75 7028      match.group(
-00004630: 3429 2e72 7374 7269 7028 292e 6c6a 7573  4).rstrip().ljus
-00004640: 7428 362c 2027 3027 290a 2020 2020 2020  t(6, '0').      
-00004650: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00004660: 2020 2020 2020 2020 2023 2054 696d 657a           # Timez
-00004670: 6f6e 6520 6f66 6673 6574 0a20 2020 2020  one offset.     
-00004680: 2020 2020 2020 2074 7a5f 6d61 7463 6820         tz_match 
-00004690: 3d20 6d61 7463 682e 6772 6f75 7028 3529  = match.group(5)
-000046a0: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-000046b0: 7267 735b 2774 7a69 6e66 6f27 5d20 3d20  rgs['tzinfo'] = 
-000046c0: 636c 732e 5f75 7463 5f6f 6666 7365 7428  cls._utc_offset(
-000046d0: 747a 5f6d 6174 6368 2920 6966 2074 7a5f  tz_match) if tz_
-000046e0: 6d61 7463 6820 656c 7365 204e 6f6e 650a  match else None.
-000046f0: 0a20 2020 2020 2020 2020 2020 2023 2044  .            # D
-00004700: 5420 6d61 7920 696e 636c 7564 6520 6120  T may include a 
-00004710: 6c65 6170 2073 6563 6f6e 6420 7768 6963  leap second whic
-00004720: 6820 6973 6e27 7420 616c 6c6f 7765 6420  h isn't allowed 
-00004730: 6279 2064 6174 6574 696d 650a 2020 2020  by datetime.    
-00004740: 2020 2020 2020 2020 6966 206b 7761 7267          if kwarg
-00004750: 735b 2773 6563 6f6e 6427 5d20 3d3d 2036  s['second'] == 6
-00004760: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00004770: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-00004780: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004790: 2020 2020 2020 2227 6461 7465 7469 6d65        "'datetime
-000047a0: 2e64 6174 6574 696d 6527 2064 6f65 736e  .datetime' doesn
-000047b0: 2774 2061 6c6c 6f77 2061 2076 616c 7565  't allow a value
-000047c0: 206f 6620 2736 3027 2066 6f72 2022 0a20   of '60' for ". 
-000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 2020 2022 7468 6520 7365 636f 6e64 7320     "the seconds 
-000047f0: 636f 6d70 6f6e 656e 742c 2063 6861 6e67  component, chang
-00004800: 696e 6720 746f 2027 3539 2722 0a20 2020  ing to '59'".   
-00004810: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00004820: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00004830: 7761 7267 735b 2773 6563 6f6e 6427 5d20  wargs['second'] 
-00004840: 3d20 3539 0a0a 2020 2020 2020 2020 2020  = 59..          
-00004850: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00004860: 2e5f 5f6e 6577 5f5f 2863 6c73 2c20 2a61  .__new__(cls, *a
-00004870: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
-00004880: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00004890: 7461 6e63 6528 7661 6c2c 2064 6174 6574  tance(val, datet
-000048a0: 696d 652e 6461 7465 7469 6d65 293a 0a20  ime.datetime):. 
-000048b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000048c0: 6e20 7375 7065 7228 292e 5f5f 6e65 775f  n super().__new_
-000048d0: 5f28 0a20 2020 2020 2020 2020 2020 2020  _(.             
-000048e0: 2020 2063 6c73 2c20 2a76 616c 2e74 696d     cls, *val.tim
-000048f0: 6574 7570 6c65 2829 5b3a 365d 2c20 7661  etuple()[:6], va
-00004900: 6c2e 6d69 6372 6f73 6563 6f6e 642c 2076  l.microsecond, v
-00004910: 616c 2e74 7a69 6e66 6f0a 2020 2020 2020  al.tzinfo.      
-00004920: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00004930: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00004940: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00004950: 2e5f 5f6e 6577 5f5f 2863 6c73 2c20 2a61  .__new__(cls, *a
-00004960: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
-00004970: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00004980: 6365 7074 696f 6e20 6173 2065 7863 3a0a  ception as exc:.
-00004990: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000049a0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-000049b0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000049c0: 556e 6162 6c65 2074 6f20 636f 6e76 6572  Unable to conver
-000049d0: 7420 277b 7661 6c7d 2720 746f 2027 4454  t '{val}' to 'DT
-000049e0: 2720 6f62 6a65 6374 220a 2020 2020 2020  ' object".      
-000049f0: 2020 2020 2020 2920 6672 6f6d 2065 7863        ) from exc
-00004a00: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00004a10: 5f5f 2873 656c 662c 202a 6172 6773 3a20  __(self, *args: 
-00004a20: 416e 792c 202a 2a6b 7761 7267 733a 2041  Any, **kwargs: A
-00004a30: 6e79 2920 2d3e 204e 6f6e 653a 0a20 2020  ny) -> None:.   
-00004a40: 2020 2020 2022 2222 4372 6561 7465 2061       """Create a
-00004a50: 206e 6577 202a 2a44 542a 2a20 656c 656d   new **DT** elem
-00004a60: 656e 7420 7661 6c75 652e 2222 220a 2020  ent value.""".  
-00004a70: 2020 2020 2020 7661 6c20 3d20 6172 6773        val = args
-00004a80: 5b30 5d0a 2020 2020 2020 2020 6966 2069  [0].        if i
-00004a90: 7369 6e73 7461 6e63 6528 7661 6c2c 2073  sinstance(val, s
-00004aa0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00004ab0: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
-00004ac0: 7472 696e 6720 3d20 7661 6c0a 2020 2020  tring = val.    
-00004ad0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00004ae0: 6e63 6528 7661 6c2c 2044 5429 2061 6e64  nce(val, DT) and
-00004af0: 2068 6173 6174 7472 2876 616c 2c20 276f   hasattr(val, 'o
-00004b00: 7269 6769 6e61 6c5f 7374 7269 6e67 2729  riginal_string')
-00004b10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00004b20: 6c66 2e6f 7269 6769 6e61 6c5f 7374 7269  lf.original_stri
-00004b30: 6e67 203d 2076 616c 2e6f 7269 6769 6e61  ng = val.origina
-00004b40: 6c5f 7374 7269 6e67 0a20 2020 2020 2020  l_string.       
-00004b50: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00004b60: 2876 616c 2c20 6461 7465 7469 6d65 2e64  (val, datetime.d
-00004b70: 6174 6574 696d 6529 3a0a 2020 2020 2020  atetime):.      
-00004b80: 2020 2020 2020 7365 6c66 2e6f 7269 6769        self.origi
-00004b90: 6e61 6c5f 7374 7269 6e67 203d 2028 0a20  nal_string = (. 
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004bb0: 227b 7661 6c2e 7965 6172 3a30 347d 7b76  "{val.year:04}{v
-00004bc0: 616c 2e6d 6f6e 7468 3a30 327d 7b76 616c  al.month:02}{val
-00004bd0: 2e64 6179 3a30 327d 220a 2020 2020 2020  .day:02}".      
-00004be0: 2020 2020 2020 2020 2020 6622 7b76 616c            f"{val
-00004bf0: 2e68 6f75 723a 3032 7d7b 7661 6c2e 6d69  .hour:02}{val.mi
-00004c00: 6e75 7465 3a30 327d 7b76 616c 2e73 6563  nute:02}{val.sec
-00004c10: 6f6e 643a 3032 7d22 0a20 2020 2020 2020  ond:02}".       
-00004c20: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00004c30: 2020 2023 206d 696c 6c69 7365 636f 6e64     # millisecond
-00004c40: 7320 6172 6520 7365 6c64 6f6d 2075 7365  s are seldom use
-00004c50: 642c 2061 6464 2074 6865 6d20 6f6e 6c79  d, add them only
-00004c60: 2069 6620 6e65 6564 6564 0a20 2020 2020   if needed.     
-00004c70: 2020 2020 2020 2069 6620 7661 6c2e 6d69         if val.mi
-00004c80: 6372 6f73 6563 6f6e 6420 3e20 303a 0a20  crosecond > 0:. 
-00004c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004ca0: 656c 662e 6f72 6967 696e 616c 5f73 7472  elf.original_str
-00004cb0: 696e 6720 2b3d 2066 222e 7b76 616c 2e6d  ing += f".{val.m
-00004cc0: 6963 726f 7365 636f 6e64 3a30 367d 220a  icrosecond:06}".
-00004cd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004ce0: 7661 6c2e 747a 696e 666f 2069 7320 6e6f  val.tzinfo is no
-00004cf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00004d00: 2020 2020 2020 2020 2320 6f66 6673 6574          # offset
-00004d10: 3a20 4f70 7469 6f6e 616c 5b64 6174 6574  : Optional[datet
-00004d20: 696d 652e 7469 6d65 6465 6c74 615d 0a20  ime.timedelta]. 
-00004d30: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00004d40: 6666 7365 7420 3d20 7661 6c2e 747a 696e  ffset = val.tzin
-00004d50: 666f 2e75 7463 6f66 6673 6574 2876 616c  fo.utcoffset(val
-00004d60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004d70: 2020 6966 206f 6666 7365 7420 6973 206e    if offset is n
-00004d80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00004d90: 2020 2020 2020 2020 2020 2020 206f 6666               off
-00004da0: 7365 745f 6d69 6e20 3d20 6f66 6673 6574  set_min = offset
-00004db0: 2e64 6179 7320 2a20 3234 202a 2036 3020  .days * 24 * 60 
-00004dc0: 2b20 6f66 6673 6574 2e73 6563 6f6e 6473  + offset.seconds
-00004dd0: 202f 2f20 3630 0a20 2020 2020 2020 2020   // 60.         
-00004de0: 2020 2020 2020 2020 2020 2073 6967 6e20             sign 
-00004df0: 3d20 222b 2220 6966 206f 6666 7365 745f  = "+" if offset_
-00004e00: 6d69 6e20 3e3d 2030 2065 6c73 6520 222d  min >= 0 else "-
-00004e10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004e20: 2020 2020 2020 6f66 6673 6574 5f6d 696e        offset_min
-00004e30: 203d 2061 6273 286f 6666 7365 745f 6d69   = abs(offset_mi
-00004e40: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00004e50: 2020 2020 2020 2073 656c 662e 6f72 6967         self.orig
-00004e60: 696e 616c 5f73 7472 696e 6720 2b3d 2028  inal_string += (
-00004e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e80: 2020 2020 2020 2020 2066 227b 7369 676e           f"{sign
-00004e90: 7d7b 6f66 6673 6574 5f6d 696e 202f 2f20  }{offset_min // 
-00004ea0: 3630 3a30 327d 7b6f 6666 7365 745f 6d69  60:02}{offset_mi
-00004eb0: 6e20 2520 3630 3a30 327d 220a 2020 2020  n % 60:02}".    
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 290a 0a0a 636c 6173 7320 544d 285f 4461  )...class TM(_Da
-00004ee0: 7465 5469 6d65 4261 7365 2c20 6461 7465  teTimeBase, date
-00004ef0: 7469 6d65 2e74 696d 6529 3a0a 2020 2020  time.time):.    
-00004f00: 2222 2253 746f 7265 2076 616c 7565 2066  """Store value f
-00004f10: 6f72 2061 6e20 656c 656d 656e 7420 7769  or an element wi
-00004f20: 7468 2056 5220 2a2a 544d 2a2a 2061 7320  th VR **TM** as 
-00004f30: 3a63 6c61 7373 3a60 6461 7465 7469 6d65  :class:`datetime
-00004f40: 2e74 696d 6560 2e0a 0a20 2020 204e 6f74  .time`...    Not
-00004f50: 6520 7468 6174 2074 6865 203a 636c 6173  e that the :clas
-00004f60: 733a 6064 6174 6574 696d 652e 7469 6d65  s:`datetime.time
-00004f70: 6020 6261 7365 2063 6c61 7373 2069 7320  ` base class is 
-00004f80: 696d 6d75 7461 626c 652e 0a20 2020 2022  immutable..    "
-00004f90: 2222 0a20 2020 205f 5245 5f54 494d 4520  "".    _RE_TIME 
-00004fa0: 3d20 7265 2e63 6f6d 7069 6c65 280a 2020  = re.compile(.  
-00004fb0: 2020 2020 2020 7222 283f 503c 683e 5e28        r"(?P<h>^(
-00004fc0: 5b30 315d 5b30 2d39 5d7c 325b 302d 335d  [01][0-9]|2[0-3]
-00004fd0: 2929 220a 2020 2020 2020 2020 7222 2828  ))".        r"((
-00004fe0: 3f50 3c6d 3e28 5b30 2d35 5d5b 302d 395d  ?P<m>([0-5][0-9]
-00004ff0: 2929 220a 2020 2020 2020 2020 7222 2828  ))".        r"((
-00005000: 3f50 3c73 3e28 5b30 2d35 5d5b 302d 395d  ?P<s>([0-5][0-9]
-00005010: 7c36 3029 2922 0a20 2020 2020 2020 2072  |60))".        r
-00005020: 2228 5c2e 283f 503c 6d73 3e28 5b30 2d39  "(\.(?P<ms>([0-9
-00005030: 5d7b 312c 367d 293f 2929 3f29 3f29 3f24  ]{1,6})?))?)?)?$
-00005040: 220a 2020 2020 290a 0a20 2020 2064 6566  ".    )..    def
-00005050: 205f 5f6e 6577 5f5f 2820 2023 2074 7970   __new__(  # typ
-00005060: 653a 2069 676e 6f72 655b 6d69 7363 5d0a  e: ignore[misc].
-00005070: 2020 2020 2020 2020 636c 733a 2054 7970          cls: Typ
-00005080: 655b 2254 4d22 5d2c 202a 6172 6773 3a20  e["TM"], *args: 
-00005090: 416e 792c 202a 2a6b 7761 7267 733a 2041  Any, **kwargs: A
-000050a0: 6e79 0a20 2020 2029 202d 3e20 4f70 7469  ny.    ) -> Opti
-000050b0: 6f6e 616c 5b22 544d 225d 3a0a 2020 2020  onal["TM"]:.    
-000050c0: 2020 2020 2222 2243 7265 6174 6520 616e      """Create an
-000050d0: 2069 6e73 7461 6e63 6520 6f66 2054 4d20   instance of TM 
-000050e0: 6f62 6a65 6374 2066 726f 6d20 6120 7374  object from a st
-000050f0: 7269 6e67 2e0a 0a20 2020 2020 2020 2052  ring...        R
-00005100: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
-00005110: 6e20 6966 2074 6865 2073 7472 696e 6720  n if the string 
-00005120: 6361 6e6e 6f74 2062 6520 7061 7273 6564  cannot be parsed
-00005130: 206f 7220 7468 6520 6172 6775 6d65 6e74   or the argument
-00005140: 0a20 2020 2020 2020 2069 7320 6f74 6865  .        is othe
-00005150: 7277 6973 6520 696e 636f 6d70 6174 6962  rwise incompatib
-00005160: 6c65 2e0a 0a20 2020 2020 2020 2054 6865  le...        The
-00005170: 2061 7267 756d 656e 7473 2028 6060 2a61   arguments (``*a
-00005180: 7267 7360 6020 616e 6420 6060 2a2a 6b77  rgs`` and ``**kw
-00005190: 6172 6773 6060 2920 6172 6520 6569 7468  args``) are eith
-000051a0: 6572 2074 6865 206f 6e65 730a 2020 2020  er the ones.    
-000051b0: 2020 2020 696e 6865 7269 7465 6420 6672      inherited fr
-000051c0: 6f6d 203a 636c 6173 733a 6064 6174 6574  om :class:`datet
-000051d0: 696d 652e 7469 6d65 602c 206f 7220 7468  ime.time`, or th
-000051e0: 6520 6669 7273 7420 6172 6775 6d65 6e74  e first argument
-000051f0: 2069 730a 2020 2020 2020 2020 6120 7374   is.        a st
-00005200: 7269 6e67 2063 6f6e 666f 726d 616e 7420  ring conformant 
-00005210: 746f 2074 6865 2054 4d20 6465 6669 6e69  to the TM defini
-00005220: 7469 6f6e 2069 6e20 7468 6520 4449 434f  tion in the DICO
-00005230: 4d20 5374 616e 6461 7264 2c0a 2020 2020  M Standard,.    
-00005240: 2020 2020 5061 7274 2035 2c20 3a64 636d      Part 5, :dcm
-00005250: 3a60 5461 626c 6520 362e 322d 313c 7061  :`Table 6.2-1<pa
-00005260: 7274 3035 2f73 6563 745f 362e 322e 6874  rt05/sect_6.2.ht
-00005270: 6d6c 2374 6162 6c65 5f36 2e32 2d31 3e60  ml#table_6.2-1>`
-00005280: 2c0a 2020 2020 2020 2020 6f72 2069 7420  ,.        or it 
-00005290: 6973 2061 203a 636c 6173 733a 6064 6174  is a :class:`dat
-000052a0: 6574 696d 652e 7469 6d65 6020 6f62 6a65  etime.time` obje
-000052b0: 6374 2c20 6f72 2061 6e20 6f62 6a65 6374  ct, or an object
-000052c0: 206f 6620 7479 7065 0a20 2020 2020 2020   of type.       
-000052d0: 203a 636c 6173 733a 607e 7079 6469 636f   :class:`~pydico
-000052e0: 6d2e 7661 6c75 6572 6570 2e54 4d60 2e0a  m.valuerep.TM`..
-000052f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00005300: 2020 2020 6966 206e 6f74 2061 7267 7320      if not args 
-00005310: 6f72 2061 7267 735b 305d 2069 7320 4e6f  or args[0] is No
-00005320: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00005330: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00005340: 2020 2020 2076 616c 203d 2061 7267 735b       val = args[
-00005350: 305d 0a20 2020 2020 2020 2069 6620 6973  0].        if is
-00005360: 696e 7374 616e 6365 2876 616c 2c20 7374  instance(val, st
-00005370: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00005380: 6966 2076 616c 2e73 7472 6970 2829 203d  if val.strip() =
-00005390: 3d20 2727 3a0a 2020 2020 2020 2020 2020  = '':.          
-000053a0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000053b0: 6520 2023 2065 6d70 7479 2074 696d 650a  e  # empty time.
-000053c0: 0a20 2020 2020 2020 2020 2020 206d 6174  .            mat
-000053d0: 6368 203d 2063 6c73 2e5f 5245 5f54 494d  ch = cls._RE_TIM
-000053e0: 452e 6d61 7463 6828 7661 6c29 0a20 2020  E.match(val).   
-000053f0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00005400: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
-00005410: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00005420: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-00005430: 2020 2020 2020 2020 2020 2020 2066 2255               f"U
-00005440: 6e61 626c 6520 746f 2063 6f6e 7665 7274  nable to convert
-00005450: 206e 6f6e 2d63 6f6e 666f 726d 616e 7420   non-conformant 
-00005460: 7661 6c75 6520 277b 7661 6c7d 2720 746f  value '{val}' to
-00005470: 2027 544d 2720 220a 2020 2020 2020 2020   'TM' ".        
-00005480: 2020 2020 2020 2020 2020 2020 226f 626a              "obj
-00005490: 6563 7422 0a20 2020 2020 2020 2020 2020  ect".           
-000054a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000054b0: 2020 2020 686f 7572 203d 2069 6e74 286d      hour = int(m
-000054c0: 6174 6368 2e67 726f 7570 2827 6827 2929  atch.group('h'))
-000054d0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
-000054e0: 7574 6520 3d20 3020 6966 206d 6174 6368  ute = 0 if match
-000054f0: 2e67 726f 7570 2827 6d27 2920 6973 204e  .group('m') is N
-00005500: 6f6e 6520 656c 7365 2069 6e74 286d 6174  one else int(mat
-00005510: 6368 2e67 726f 7570 2827 6d27 2929 0a20  ch.group('m')). 
-00005520: 2020 2020 2020 2020 2020 2073 6563 6f6e             secon
-00005530: 6420 3d20 3020 6966 206d 6174 6368 2e67  d = 0 if match.g
-00005540: 726f 7570 2827 7327 2920 6973 204e 6f6e  roup('s') is Non
-00005550: 6520 656c 7365 2069 6e74 286d 6174 6368  e else int(match
-00005560: 2e67 726f 7570 2827 7327 2929 0a0a 2020  .group('s'))..  
-00005570: 2020 2020 2020 2020 2020 6966 2073 6563            if sec
-00005580: 6f6e 6420 3d3d 2036 303a 0a20 2020 2020  ond == 60:.     
-00005590: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-000055a0: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-000055c0: 6461 7465 7469 6d65 2e74 696d 6527 2064  datetime.time' d
-000055d0: 6f65 736e 2774 2061 6c6c 6f77 2061 2076  oesn't allow a v
-000055e0: 616c 7565 206f 6620 2736 3027 2066 6f72  alue of '60' for
-000055f0: 2074 6865 2022 0a20 2020 2020 2020 2020   the ".         
-00005600: 2020 2020 2020 2020 2020 2022 7365 636f             "seco
-00005610: 6e64 7320 636f 6d70 6f6e 656e 742c 2063  nds component, c
-00005620: 6861 6e67 696e 6720 746f 2027 3539 2722  hanging to '59'"
-00005630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005640: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00005650: 2020 2073 6563 6f6e 6420 3d20 3539 0a0a     second = 59..
-00005660: 2020 2020 2020 2020 2020 2020 6d69 6372              micr
-00005670: 6f73 6563 6f6e 6420 3d20 300a 2020 2020  osecond = 0.    
-00005680: 2020 2020 2020 2020 6966 206d 6174 6368          if match
-00005690: 2e67 726f 7570 2827 6d73 2729 3a0a 2020  .group('ms'):.  
-000056a0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000056b0: 6372 6f73 6563 6f6e 6420 3d20 696e 7428  crosecond = int(
-000056c0: 6d61 7463 682e 6772 6f75 7028 276d 7327  match.group('ms'
-000056d0: 292e 7273 7472 6970 2829 2e6c 6a75 7374  ).rstrip().ljust
-000056e0: 2836 2c20 2730 2729 290a 0a20 2020 2020  (6, '0'))..     
-000056f0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00005700: 7065 7228 292e 5f5f 6e65 775f 5f28 0a20  per().__new__(. 
-00005710: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00005720: 6c73 2c20 686f 7572 2c20 6d69 6e75 7465  ls, hour, minute
-00005730: 2c20 7365 636f 6e64 2c20 6d69 6372 6f73  , second, micros
-00005740: 6563 6f6e 640a 2020 2020 2020 2020 2020  econd.          
-00005750: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
-00005760: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
-00005770: 6461 7465 7469 6d65 2e74 696d 6529 3a0a  datetime.time):.
-00005780: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005790: 726e 2073 7570 6572 2829 2e5f 5f6e 6577  rn super().__new
-000057a0: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
-000057b0: 2020 2020 636c 732c 2076 616c 2e68 6f75      cls, val.hou
-000057c0: 722c 2076 616c 2e6d 696e 7574 652c 2076  r, val.minute, v
-000057d0: 616c 2e73 6563 6f6e 642c 2076 616c 2e6d  al.second, val.m
-000057e0: 6963 726f 7365 636f 6e64 0a20 2020 2020  icrosecond.     
-000057f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00005800: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00005810: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
-00005820: 292e 5f5f 6e65 775f 5f28 0a20 2020 2020  ).__new__(.     
-00005830: 2020 2020 2020 2020 2020 2063 6c73 2c20             cls, 
-00005840: 2a61 7267 732c 202a 2a6b 7761 7267 730a  *args, **kwargs.
-00005850: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00005860: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00005870: 6570 7469 6f6e 2061 7320 6578 633a 0a20  eption as exc:. 
-00005880: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00005890: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-000058a0: 2020 2020 2020 2020 2020 2020 2066 2255               f"U
-000058b0: 6e61 626c 6520 746f 2063 6f6e 7665 7274  nable to convert
-000058c0: 2027 7b76 616c 7d27 2074 6f20 2754 4d27   '{val}' to 'TM'
-000058d0: 206f 626a 6563 7422 0a20 2020 2020 2020   object".       
-000058e0: 2020 2020 2029 2066 726f 6d20 6578 630a       ) from exc.
-000058f0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00005900: 5f28 7365 6c66 2c20 2a61 7267 733a 2041  _(self, *args: A
-00005910: 6e79 2c20 2a2a 6b77 6172 6773 3a20 416e  ny, **kwargs: An
-00005920: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
-00005930: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00005940: 6974 5f5f 2829 0a20 2020 2020 2020 2076  it__().        v
-00005950: 616c 203d 2061 7267 735b 305d 0a20 2020  al = args[0].   
-00005960: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00005970: 6365 2876 616c 2c20 7374 7229 3a0a 2020  ce(val, str):.  
-00005980: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00005990: 7269 6769 6e61 6c5f 7374 7269 6e67 203d  riginal_string =
-000059a0: 2076 616c 0a20 2020 2020 2020 2065 6c69   val.        eli
-000059b0: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-000059c0: 2c20 544d 2920 616e 6420 6861 7361 7474  , TM) and hasatt
-000059d0: 7228 7661 6c2c 2027 6f72 6967 696e 616c  r(val, 'original
-000059e0: 5f73 7472 696e 6727 293a 0a20 2020 2020  _string'):.     
-000059f0: 2020 2020 2020 2073 656c 662e 6f72 6967         self.orig
-00005a00: 696e 616c 5f73 7472 696e 6720 3d20 7661  inal_string = va
-00005a10: 6c2e 6f72 6967 696e 616c 5f73 7472 696e  l.original_strin
-00005a20: 670a 2020 2020 2020 2020 656c 6966 2069  g.        elif i
-00005a30: 7369 6e73 7461 6e63 6528 7661 6c2c 2064  sinstance(val, d
-00005a40: 6174 6574 696d 652e 7469 6d65 293a 0a20  atetime.time):. 
-00005a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005a60: 6f72 6967 696e 616c 5f73 7472 696e 6720  original_string 
-00005a70: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00005a80: 2020 2020 6622 7b76 616c 2e68 6f75 723a      f"{val.hour:
-00005a90: 3032 7d7b 7661 6c2e 6d69 6e75 7465 3a30  02}{val.minute:0
-00005aa0: 327d 7b76 616c 2e73 6563 6f6e 643a 3032  2}{val.second:02
-00005ab0: 7d22 0a20 2020 2020 2020 2020 2020 2029  }".            )
-00005ac0: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
-00005ad0: 696c 6c69 7365 636f 6e64 7320 6172 6520  illiseconds are 
-00005ae0: 7365 6c64 6f6d 2075 7365 642c 2061 6464  seldom used, add
-00005af0: 2074 6865 6d20 6f6e 6c79 2069 6620 6e65   them only if ne
-00005b00: 6564 6564 0a20 2020 2020 2020 2020 2020  eded.           
-00005b10: 2069 6620 7661 6c2e 6d69 6372 6f73 6563   if val.microsec
-00005b20: 6f6e 6420 3e20 303a 0a20 2020 2020 2020  ond > 0:.       
-00005b30: 2020 2020 2020 2020 2073 656c 662e 6f72           self.or
-00005b40: 6967 696e 616c 5f73 7472 696e 6720 2b3d  iginal_string +=
-00005b50: 2066 222e 7b76 616c 2e6d 6963 726f 7365   f".{val.microse
-00005b60: 636f 6e64 3a30 367d 220a 0a0a 6465 6620  cond:06}"...def 
-00005b70: 6973 5f76 616c 6964 5f64 7328 733a 2073  is_valid_ds(s: s
-00005b80: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
-00005b90: 2022 2222 4368 6563 6b20 7768 6574 6865   """Check whethe
-00005ba0: 7220 7468 6973 2073 7472 696e 6720 6973  r this string is
-00005bb0: 2061 2076 616c 6964 2064 6563 696d 616c   a valid decimal
-00005bc0: 2073 7472 696e 672e 0a0a 2020 2020 5661   string...    Va
-00005bd0: 6c69 6420 6465 6369 6d61 6c20 7374 7269  lid decimal stri
-00005be0: 6e67 7320 6d75 7374 2062 6520 3136 2063  ngs must be 16 c
-00005bf0: 6861 7261 6374 6572 7320 6f72 2066 6577  haracters or few
-00005c00: 6572 2c20 616e 6420 636f 6e74 6169 6e20  er, and contain 
-00005c10: 6f6e 6c79 0a20 2020 2063 6861 7261 6374  only.    charact
-00005c20: 6572 7320 6672 6f6d 2061 206c 696d 6974  ers from a limit
-00005c30: 6564 2073 6574 2e0a 0a20 2020 2050 6172  ed set...    Par
-00005c40: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00005c50: 2d2d 2d2d 2d2d 0a20 2020 2073 3a20 7374  ------.    s: st
-00005c60: 720a 2020 2020 2020 2020 5374 7269 6e67  r.        String
-00005c70: 2074 6f20 7465 7374 2e0a 0a20 2020 2052   to test...    R
-00005c80: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00005c90: 2d2d 0a20 2020 2062 6f6f 6c0a 2020 2020  --.    bool.    
-00005ca0: 2020 2020 5472 7565 2069 6620 7468 6520      True if the 
-00005cb0: 7374 7269 6e67 2069 7320 6120 7661 6c69  string is a vali
-00005cc0: 6420 6465 6369 6d61 6c20 7374 7269 6e67  d decimal string
-00005cd0: 2e20 4f74 6865 7277 6973 6520 4661 6c73  . Otherwise Fals
-00005ce0: 652e 0a20 2020 2022 2222 0a20 2020 2072  e..    """.    r
-00005cf0: 6574 7572 6e20 7661 6c69 6461 7465 5f6c  eturn validate_l
-00005d00: 656e 6774 685f 616e 645f 7265 6765 7828  ength_and_regex(
-00005d10: 2244 5322 2c20 7329 5b30 5d0a 0a0a 6465  "DS", s)[0]...de
-00005d20: 6620 666f 726d 6174 5f6e 756d 6265 725f  f format_number_
-00005d30: 6173 5f64 7328 7661 6c3a 2055 6e69 6f6e  as_ds(val: Union
-00005d40: 5b66 6c6f 6174 2c20 4465 6369 6d61 6c5d  [float, Decimal]
-00005d50: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-00005d60: 2254 7275 6e63 6174 6520 6120 666c 6f61  "Truncate a floa
-00005d70: 7427 7320 7265 7072 6573 656e 7461 7469  t's representati
-00005d80: 6f6e 2074 6f20 6769 7665 2061 2076 616c  on to give a val
-00005d90: 6964 2044 6563 696d 616c 2053 7472 696e  id Decimal Strin
-00005da0: 6720 2844 5329 2e0a 0a20 2020 2044 4943  g (DS)...    DIC
-00005db0: 4f4d 2773 2064 6563 696d 616c 2073 7472  OM's decimal str
-00005dc0: 696e 6720 2844 5329 2072 6570 7265 7365  ing (DS) represe
-00005dd0: 6e74 6174 696f 6e20 6973 206c 696d 6974  ntation is limit
-00005de0: 6564 2074 6f20 7374 7269 6e67 7320 7769  ed to strings wi
-00005df0: 7468 2031 360a 2020 2020 6368 6172 6163  th 16.    charac
-00005e00: 7465 7273 2061 6e64 2061 206c 696d 6974  ters and a limit
-00005e10: 6564 2073 6574 206f 6620 6368 6172 6163  ed set of charac
-00005e20: 7465 7273 2e20 5468 6973 2066 756e 6374  ters. This funct
-00005e30: 696f 6e20 7265 7072 6573 656e 7473 2061  ion represents a
-00005e40: 0a20 2020 2066 6c6f 6174 2074 6861 7420  .    float that 
-00005e50: 7361 7469 7366 6965 7320 7468 6573 6520  satisfies these 
-00005e60: 636f 6e73 7472 6169 6e74 7320 7768 696c  constraints whil
-00005e70: 6520 7265 7461 696e 696e 6720 6173 206d  e retaining as m
-00005e80: 7563 680a 2020 2020 7072 6563 6973 696f  uch.    precisio
-00005e90: 6e20 6173 2070 6f73 7369 626c 652e 2053  n as possible. S
-00005ea0: 6f6d 6520 666c 6f61 7473 2061 7265 2072  ome floats are r
-00005eb0: 6570 7265 7365 6e74 6564 2075 7369 6e67  epresented using
-00005ec0: 2073 6369 656e 7469 6669 630a 2020 2020   scientific.    
-00005ed0: 6e6f 7461 7469 6f6e 2074 6f20 6d61 6b65  notation to make
-00005ee0: 206d 6f72 6520 6566 6669 6369 656e 7420   more efficient 
-00005ef0: 7573 6520 6f66 2074 6865 206c 696d 6974  use of the limit
-00005f00: 6564 206e 756d 6265 7220 6f66 2063 6861  ed number of cha
-00005f10: 7261 6374 6572 732e 0a0a 2020 2020 4e6f  racters...    No
-00005f20: 7465 2074 6861 7420 7468 6973 2077 696c  te that this wil
-00005f30: 6c20 696e 6375 7220 6120 6c6f 7373 206f  l incur a loss o
-00005f40: 6620 7072 6563 6973 696f 6e20 6966 2074  f precision if t
-00005f50: 6865 206e 756d 6265 7220 6361 6e6e 6f74  he number cannot
-00005f60: 2062 650a 2020 2020 7265 7072 6573 656e   be.    represen
-00005f70: 7465 6420 7769 7468 2031 3620 6368 6172  ted with 16 char
-00005f80: 6163 7465 7273 2e20 4675 7274 6865 726d  acters. Furtherm
-00005f90: 6f72 652c 206e 6f6e 2d66 696e 6974 6520  ore, non-finite 
-00005fa0: 666c 6f61 7473 2028 696e 6673 2061 6e64  floats (infs and
-00005fb0: 0a20 2020 206e 616e 7329 2063 616e 6e6f  .    nans) canno
-00005fc0: 7420 6265 2072 6570 7265 7365 6e74 6564  t be represented
-00005fd0: 2061 7320 6465 6369 6d61 6c20 7374 7269   as decimal stri
-00005fe0: 6e67 7320 616e 6420 7769 6c6c 2063 6175  ngs and will cau
-00005ff0: 7365 2061 6e20 6572 726f 7220 746f 0a20  se an error to. 
-00006000: 2020 2062 6520 7261 6973 6564 2e0a 0a20     be raised... 
-00006010: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00006020: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00006030: 2076 616c 3a20 556e 696f 6e5b 666c 6f61   val: Union[floa
-00006040: 742c 2044 6563 696d 616c 5d0a 2020 2020  t, Decimal].    
-00006050: 2020 2020 5468 6520 666c 6f61 7469 6e67      The floating
-00006060: 2070 6f69 6e74 2076 616c 7565 2077 686f   point value who
-00006070: 7365 2072 6570 7265 7365 6e74 6174 696f  se representatio
-00006080: 6e20 6973 2072 6571 7569 7265 642e 0a0a  n is required...
-00006090: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000060a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7374 720a  -------.    str.
-000060b0: 2020 2020 2020 2020 5374 7269 6e67 2072          String r
-000060c0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-000060d0: 2074 6865 2066 6c6f 6174 2073 6174 6973   the float satis
-000060e0: 6679 696e 6720 7468 6520 636f 6e73 7472  fying the constr
-000060f0: 6169 6e74 7320 6f66 2074 6865 0a20 2020  aints of the.   
-00006100: 2020 2020 2064 6563 696d 616c 2073 7472       decimal str
-00006110: 696e 6720 7265 7072 6573 656e 7461 7469  ing representati
-00006120: 6f6e 2e0a 0a20 2020 2052 6169 7365 730a  on...    Raises.
-00006130: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2056      ------.    V
-00006140: 616c 7565 4572 726f 720a 2020 2020 2020  alueError.      
-00006150: 2020 4966 2076 616c 2064 6f65 7320 6e6f    If val does no
-00006160: 7420 7265 7072 6573 656e 7420 6120 6669  t represent a fi
-00006170: 6e69 7465 2076 616c 7565 0a0a 2020 2020  nite value..    
-00006180: 2222 220a 2020 2020 6966 206e 6f74 2069  """.    if not i
-00006190: 7369 6e73 7461 6e63 6528 7661 6c2c 2028  sinstance(val, (
-000061a0: 666c 6f61 742c 2044 6563 696d 616c 2929  float, Decimal))
-000061b0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-000061c0: 5479 7065 4572 726f 7228 2227 7661 6c27  TypeError("'val'
-000061d0: 206d 7573 7420 6265 206f 6620 7479 7065   must be of type
-000061e0: 2066 6c6f 6174 206f 7220 6465 6369 6d61   float or decima
-000061f0: 6c2e 4465 6369 6d61 6c22 290a 2020 2020  l.Decimal").    
-00006200: 6966 206e 6f74 2069 7366 696e 6974 6528  if not isfinite(
-00006210: 7661 6c29 3a0a 2020 2020 2020 2020 7261  val):.        ra
-00006220: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-00006230: 2020 2020 2020 2020 2020 2020 2243 616e              "Can
-00006240: 6e6f 7420 656e 636f 6465 206e 6f6e 2d66  not encode non-f
-00006250: 696e 6974 6520 666c 6f61 7473 2061 7320  inite floats as 
-00006260: 4449 434f 4d20 6465 6369 6d61 6c20 7374  DICOM decimal st
-00006270: 7269 6e67 732e 2022 0a20 2020 2020 2020  rings. ".       
-00006280: 2020 2020 2066 2247 6f74 2027 7b76 616c       f"Got '{val
-00006290: 7d27 220a 2020 2020 2020 2020 290a 0a20  }'".        ).. 
-000062a0: 2020 2076 616c 7374 7220 3d20 7374 7228     valstr = str(
-000062b0: 7661 6c29 0a0a 2020 2020 2320 496e 2074  val)..    # In t
-000062c0: 6865 2073 696d 706c 6520 6361 7365 2c20  he simple case, 
-000062d0: 7468 6520 6465 6661 756c 7420 7079 7468  the default pyth
-000062e0: 6f6e 2073 7472 696e 6720 7265 7072 6573  on string repres
-000062f0: 656e 7461 7469 6f6e 0a20 2020 2023 2077  entation.    # w
-00006300: 696c 6c20 646f 0a20 2020 2069 6620 6c65  ill do.    if le
-00006310: 6e28 7661 6c73 7472 2920 3c3d 2031 363a  n(valstr) <= 16:
-00006320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006330: 7661 6c73 7472 0a0a 2020 2020 2320 4465  valstr..    # De
-00006340: 6369 6465 2077 6865 7468 6572 2074 6f20  cide whether to 
-00006350: 7573 6520 7363 6965 6e74 6966 6963 206e  use scientific n
-00006360: 6f74 6174 696f 6e0a 2020 2020 6c6f 6776  otation.    logv
-00006370: 616c 203d 206c 6f67 3130 2863 6173 7428  al = log10(cast(
-00006380: 556e 696f 6e5b 666c 6f61 742c 2044 6563  Union[float, Dec
-00006390: 696d 616c 5d2c 2061 6273 2876 616c 2929  imal], abs(val))
-000063a0: 290a 0a20 2020 2023 2043 6861 7261 6374  )..    # Charact
-000063b0: 6572 7320 6e65 6564 6564 2066 6f72 2027  ers needed for '
-000063c0: 2d27 2061 7420 7374 6172 740a 2020 2020  -' at start.    
-000063d0: 7369 676e 5f63 6861 7273 203d 2031 2069  sign_chars = 1 i
-000063e0: 6620 7661 6c20 3c20 302e 3020 656c 7365  f val < 0.0 else
-000063f0: 2030 0a0a 2020 2020 2320 4e75 6d62 6572   0..    # Number
-00006400: 7320 6c61 7267 6572 2074 6861 6e20 3165  s larger than 1e
-00006410: 3134 2063 616e 6e6f 7420 6265 2063 6f72  14 cannot be cor
-00006420: 7265 6374 6c79 2072 6570 7265 7365 6e74  rectly represent
-00006430: 6564 2062 7920 7472 756e 6361 7469 6e67  ed by truncating
-00006440: 0a20 2020 2023 2074 6865 6972 2073 7472  .    # their str
-00006450: 696e 6720 7265 7072 6573 656e 7461 7469  ing representati
-00006460: 6f6e 7320 746f 2031 3620 6368 6172 732c  ons to 16 chars,
-00006470: 2065 2e67 2070 6920 2a20 3130 5e31 3320   e.g pi * 10^13 
-00006480: 776f 756c 6420 6265 636f 6d65 0a20 2020  would become.   
-00006490: 2023 2027 3331 3431 3539 3236 3533 3538   # '314159265358
-000064a0: 3937 392e 272c 2077 6869 6368 206d 6179  979.', which may
-000064b0: 206e 6f74 2062 6520 756e 6976 6572 7361   not be universa
-000064c0: 6c6c 7920 756e 6465 7273 746f 6f64 2e20  lly understood. 
-000064d0: 5468 6973 206c 696d 6974 0a20 2020 2023  This limit.    #
-000064e0: 2069 7320 3165 3133 2066 6f72 206e 6567   is 1e13 for neg
-000064f0: 6174 6976 6520 6e75 6d62 6572 7320 6265  ative numbers be
-00006500: 6361 7573 6520 6f66 2074 6865 206d 696e  cause of the min
-00006510: 7573 2073 6967 6e2e 0a20 2020 2023 2046  us sign..    # F
-00006520: 6f72 206e 6567 6174 6976 6520 6578 706f  or negative expo
-00006530: 6e65 6e74 732c 2074 6865 2070 6f69 6e74  nents, the point
-00006540: 206f 6620 6571 7561 6c20 7072 6563 6973   of equal precis
-00006550: 696f 6e20 6265 7477 6565 6e20 7363 6965  ion between scie
-00006560: 6e74 6966 6963 0a20 2020 2023 2061 6e64  ntific.    # and
-00006570: 2073 7461 6e64 6172 6420 6e6f 7461 7469   standard notati
-00006580: 6f6e 2069 7320 3165 2d34 2065 2e67 2e20  on is 1e-4 e.g. 
-00006590: 2730 2e30 3030 3331 3431 3539 3236 3533  '0.0003141592653
-000065a0: 3527 2061 6e64 0a20 2020 2023 2027 332e  5' and.    # '3.
-000065b0: 3134 3135 3932 3635 3335 652d 3034 2720  1415926535e-04' 
-000065c0: 6172 6520 626f 7468 2031 3620 6368 6172  are both 16 char
-000065d0: 730a 2020 2020 7573 655f 7363 6965 6e74  s.    use_scient
-000065e0: 6966 6963 203d 206c 6f67 7661 6c20 3c20  ific = logval < 
-000065f0: 2d34 206f 7220 6c6f 6776 616c 203e 3d20  -4 or logval >= 
-00006600: 2831 3420 2d20 7369 676e 5f63 6861 7273  (14 - sign_chars
-00006610: 290a 0a20 2020 2069 6620 7573 655f 7363  )..    if use_sc
-00006620: 6965 6e74 6966 6963 3a0a 2020 2020 2020  ientific:.      
-00006630: 2020 2320 496e 2070 7269 6e63 6970 6c65    # In principle
-00006640: 2c20 7765 2063 6f75 6c64 2068 6176 6520  , we could have 
-00006650: 6120 6e75 6d62 6572 2077 6865 7265 2074  a number where t
-00006660: 6865 2065 7870 6f6e 656e 740a 2020 2020  he exponent.    
-00006670: 2020 2020 2320 6e65 6564 7320 7468 7265      # needs thre
-00006680: 6520 6469 6769 7473 2074 6f20 6265 2072  e digits to be r
-00006690: 6570 7265 7365 6e74 6564 2028 6269 6767  epresented (bigg
-000066a0: 6572 2074 6861 6e20 7468 6973 2063 616e  er than this can
-000066b0: 6e6f 7420 6265 0a20 2020 2020 2020 2023  not be.        #
-000066c0: 2072 6570 7265 7365 6e74 6564 2062 7920   represented by 
-000066d0: 666c 6f61 7473 292e 2044 7565 2074 6f20  floats). Due to 
-000066e0: 666c 6f61 7469 6e67 2070 6f69 6e74 206c  floating point l
-000066f0: 696d 6974 6174 696f 6e73 0a20 2020 2020  imitations.     
-00006700: 2020 2023 2074 6869 7320 6973 2062 6573     # this is bes
-00006710: 7420 6368 6563 6b65 6420 666f 7220 6279  t checked for by
-00006720: 2064 6f69 6e67 2074 6865 2073 7472 696e   doing the strin
-00006730: 6720 636f 6e76 6572 7369 6f6e 0a20 2020  g conversion.   
-00006740: 2020 2020 2072 656d 6169 6e69 6e67 5f63       remaining_c
-00006750: 6861 7273 203d 2031 3020 2d20 7369 676e  hars = 10 - sign
-00006760: 5f63 6861 7273 0a20 2020 2020 2020 2074  _chars.        t
-00006770: 7275 6e63 5f73 7472 203d 2066 277b 7661  runc_str = f'{va
-00006780: 6c3a 2e7b 7265 6d61 696e 696e 675f 6368  l:.{remaining_ch
-00006790: 6172 737d 657d 270a 2020 2020 2020 2020  ars}e}'.        
-000067a0: 6966 206c 656e 2874 7275 6e63 5f73 7472  if len(trunc_str
-000067b0: 2920 3e20 3136 3a0a 2020 2020 2020 2020  ) > 16:.        
-000067c0: 2020 2020 7472 756e 635f 7374 7220 3d20      trunc_str = 
-000067d0: 6627 7b76 616c 3a2e 7b72 656d 6169 6e69  f'{val:.{remaini
-000067e0: 6e67 5f63 6861 7273 202d 2031 7d65 7d27  ng_chars - 1}e}'
-000067f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006800: 7472 756e 635f 7374 720a 2020 2020 656c  trunc_str.    el
-00006810: 7365 3a0a 2020 2020 2020 2020 6966 206c  se:.        if l
-00006820: 6f67 7661 6c20 3e3d 2031 2e30 3a0a 2020  ogval >= 1.0:.  
-00006830: 2020 2020 2020 2020 2020 2320 6368 6172            # char
-00006840: 7320 7265 6d61 696e 696e 6720 666f 7220  s remaining for 
-00006850: 6469 6769 7473 2061 6674 6572 2073 6967  digits after sig
-00006860: 6e2c 2064 6967 6974 7320 6c65 6674 206f  n, digits left o
-00006870: 6620 272e 2720 616e 6420 272e 270a 2020  f '.' and '.'.  
-00006880: 2020 2020 2020 2020 2020 7265 6d61 696e            remain
-00006890: 696e 675f 6368 6172 7320 3d20 3134 202d  ing_chars = 14 -
-000068a0: 2073 6967 6e5f 6368 6172 7320 2d20 696e   sign_chars - in
-000068b0: 7428 666c 6f6f 7228 6c6f 6776 616c 2929  t(floor(logval))
-000068c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000068d0: 2020 2020 2020 2020 2020 2072 656d 6169             remai
-000068e0: 6e69 6e67 5f63 6861 7273 203d 2031 3420  ning_chars = 14 
-000068f0: 2d20 7369 676e 5f63 6861 7273 0a20 2020  - sign_chars.   
-00006900: 2020 2020 2072 6574 7572 6e20 6627 7b76       return f'{v
-00006910: 616c 3a2e 7b72 656d 6169 6e69 6e67 5f63  al:.{remaining_c
-00006920: 6861 7273 7d66 7d27 0a0a 0a63 6c61 7373  hars}f}'...class
-00006930: 2044 5366 6c6f 6174 2866 6c6f 6174 293a   DSfloat(float):
-00006940: 0a20 2020 2022 2222 5374 6f72 6520 7661  .    """Store va
-00006950: 6c75 6520 666f 7220 616e 2065 6c65 6d65  lue for an eleme
-00006960: 6e74 2077 6974 6820 5652 202a 2a44 532a  nt with VR **DS*
-00006970: 2a20 6173 203a 636c 6173 733a 6066 6c6f  * as :class:`flo
-00006980: 6174 602e 0a0a 2020 2020 4966 2063 6f6e  at`...    If con
-00006990: 7374 7275 6374 6564 2066 726f 6d20 616e  structed from an
-000069a0: 2065 6d70 7479 2073 7472 696e 672c 2072   empty string, r
-000069b0: 6574 7572 6e20 7468 6520 656d 7074 7920  eturn the empty 
-000069c0: 7374 7269 6e67 2c0a 2020 2020 6e6f 7420  string,.    not 
-000069d0: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
-000069e0: 6869 7320 636c 6173 732e 0a0a 2020 2020  his class...    
-000069f0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00006a00: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7661  ---------.    va
-00006a10: 6c3a 2055 6e69 6f6e 5b73 7472 2c20 696e  l: Union[str, in
-00006a20: 742c 2066 6c6f 6174 2c20 4465 6369 6d61  t, float, Decima
-00006a30: 6c5d 0a20 2020 2020 2020 2056 616c 7565  l].        Value
-00006a40: 2074 6f20 7374 6f72 6520 6173 2061 2044   to store as a D
-00006a50: 532e 0a20 2020 2061 7574 6f5f 666f 726d  S..    auto_form
-00006a60: 6174 3a20 626f 6f6c 0a20 2020 2020 2020  at: bool.       
-00006a70: 2049 6620 5472 7565 2c20 6175 746f 6d61   If True, automa
-00006a80: 7469 6361 6c6c 7920 666f 726d 6174 2074  tically format t
-00006a90: 6865 2073 7472 696e 6720 7265 7072 6573  he string repres
-00006aa0: 656e 7461 7469 6f6e 206f 6620 7468 6973  entation of this
-00006ab0: 0a20 2020 2020 2020 206e 756d 6265 7220  .        number 
-00006ac0: 746f 2065 6e73 7572 6520 6974 2073 6174  to ensure it sat
-00006ad0: 6973 6669 6573 2074 6865 2063 6f6e 7374  isfies the const
-00006ae0: 7261 696e 7473 2069 6e20 7468 6520 4449  raints in the DI
-00006af0: 434f 4d20 7374 616e 6461 7264 2e0a 2020  COM standard..  
-00006b00: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
-00006b10: 7468 6973 2077 696c 6c20 6c65 6164 2074  this will lead t
-00006b20: 6f20 6c6f 7373 206f 6620 7072 6563 6973  o loss of precis
-00006b30: 696f 6e20 666f 7220 736f 6d65 206e 756d  ion for some num
-00006b40: 6265 7273 2e0a 0a20 2020 2022 2222 0a20  bers...    """. 
-00006b50: 2020 2061 7574 6f5f 666f 726d 6174 3a20     auto_format: 
-00006b60: 626f 6f6c 0a0a 2020 2020 6465 6620 5f5f  bool..    def __
-00006b70: 6e65 775f 5f28 2020 2320 7479 7065 3a20  new__(  # type: 
-00006b80: 6967 6e6f 7265 5b6d 6973 635d 0a20 2020  ignore[misc].   
-00006b90: 2020 2020 2063 6c73 3a20 5479 7065 5b22       cls: Type["
-00006ba0: 4453 666c 6f61 7422 5d2c 0a20 2020 2020  DSfloat"],.     
-00006bb0: 2020 2076 616c 3a20 556e 696f 6e5b 4e6f     val: Union[No
-00006bc0: 6e65 2c20 7374 722c 2069 6e74 2c20 666c  ne, str, int, fl
-00006bd0: 6f61 742c 2044 6563 696d 616c 5d2c 0a20  oat, Decimal],. 
-00006be0: 2020 2020 2020 2061 7574 6f5f 666f 726d         auto_form
-00006bf0: 6174 3a20 626f 6f6c 203d 2046 616c 7365  at: bool = False
-00006c00: 2c0a 2020 2020 2020 2020 7661 6c69 6461  ,.        valida
-00006c10: 7469 6f6e 5f6d 6f64 653a 2069 6e74 203d  tion_mode: int =
-00006c20: 204e 6f6e 650a 2020 2020 2920 2d3e 204f   None.    ) -> O
-00006c30: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
-00006c40: 722c 2022 4453 666c 6f61 7422 5d5d 3a0a  r, "DSfloat"]]:.
-00006c50: 2020 2020 2020 2020 6966 2076 616c 2069          if val i
-00006c60: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00006c70: 2020 2020 7265 7475 726e 2076 616c 0a0a      return val..
-00006c80: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00006c90: 7461 6e63 6528 7661 6c2c 2073 7472 2920  tance(val, str) 
-00006ca0: 616e 6420 7661 6c2e 7374 7269 7028 2920  and val.strip() 
-00006cb0: 3d3d 2027 273a 0a20 2020 2020 2020 2020  == '':.         
-00006cc0: 2020 2072 6574 7572 6e20 7661 6c0a 0a20     return val.. 
-00006cd0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00006ce0: 7065 7228 292e 5f5f 6e65 775f 5f28 636c  per().__new__(cl
-00006cf0: 732c 2076 616c 290a 0a20 2020 2064 6566  s, val)..    def
-00006d00: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00006d10: 2020 2073 656c 662c 2076 616c 3a20 556e     self, val: Un
-00006d20: 696f 6e5b 7374 722c 2069 6e74 2c20 666c  ion[str, int, fl
-00006d30: 6f61 742c 2044 6563 696d 616c 5d2c 0a20  oat, Decimal],. 
-00006d40: 2020 2020 2020 2061 7574 6f5f 666f 726d         auto_form
-00006d50: 6174 3a20 626f 6f6c 203d 2046 616c 7365  at: bool = False
-00006d60: 2c0a 2020 2020 2020 2020 7661 6c69 6461  ,.        valida
-00006d70: 7469 6f6e 5f6d 6f64 653a 2069 6e74 203d  tion_mode: int =
-00006d80: 204e 6f6e 650a 2020 2020 2920 2d3e 204e   None.    ) -> N
-00006d90: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00006da0: 5374 6f72 6520 7468 6520 6f72 6967 696e  Store the origin
-00006db0: 616c 2073 7472 696e 6720 6966 206f 6e65  al string if one
-00006dc0: 2067 6976 656e 2c20 666f 7220 6578 6163   given, for exac
-00006dd0: 7420 7772 6974 652d 6f75 7420 6f66 2073  t write-out of s
-00006de0: 616d 650a 2020 2020 2020 2020 7661 6c75  ame.        valu
-00006df0: 6520 6c61 7465 722e 0a20 2020 2020 2020  e later..       
-00006e00: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00006e10: 7661 6c69 6461 7469 6f6e 5f6d 6f64 6520  validation_mode 
-00006e20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00006e30: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
-00006e40: 6d6f 6465 203d 2063 6f6e 6669 672e 7365  mode = config.se
-00006e50: 7474 696e 6773 2e72 6561 6469 6e67 5f76  ttings.reading_v
-00006e60: 616c 6964 6174 696f 6e5f 6d6f 6465 0a0a  alidation_mode..
-00006e70: 2020 2020 2020 2020 2320 2e2e 2e20 616c          # ... al
-00006e80: 736f 2069 6620 7573 6572 2063 6861 6e67  so if user chang
-00006e90: 6573 2061 2064 6174 6120 656c 656d 656e  es a data elemen
-00006ea0: 7420 7661 6c75 652c 2074 6865 6e20 7769  t value, then wi
-00006eb0: 6c6c 2067 6574 0a20 2020 2020 2020 2023  ll get.        #
-00006ec0: 2061 2064 6966 6665 7265 6e74 206f 626a   a different obj
-00006ed0: 6563 742c 2062 6563 6175 7365 2066 6c6f  ect, because flo
-00006ee0: 6174 2069 7320 696d 6d75 7461 626c 652e  at is immutable.
-00006ef0: 0a20 2020 2020 2020 2068 6173 5f61 7474  .        has_att
-00006f00: 7269 6275 7465 203d 2068 6173 6174 7472  ribute = hasattr
-00006f10: 2876 616c 2c20 276f 7269 6769 6e61 6c5f  (val, 'original_
-00006f20: 7374 7269 6e67 2729 0a20 2020 2020 2020  string').       
-00006f30: 2070 7265 5f63 6865 636b 6564 203d 2046   pre_checked = F
-00006f40: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
-00006f50: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
-00006f60: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00006f70: 2020 7365 6c66 2e6f 7269 6769 6e61 6c5f    self.original_
-00006f80: 7374 7269 6e67 203d 2076 616c 2e73 7472  string = val.str
-00006f90: 6970 2829 0a20 2020 2020 2020 2065 6c69  ip().        eli
-00006fa0: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-00006fb0: 2c20 2844 5366 6c6f 6174 2c20 4453 6465  , (DSfloat, DSde
-00006fc0: 6369 6d61 6c29 293a 0a20 2020 2020 2020  cimal)):.       
-00006fd0: 2020 2020 2069 6620 7661 6c2e 6175 746f       if val.auto
-00006fe0: 5f66 6f72 6d61 743a 0a20 2020 2020 2020  _format:.       
-00006ff0: 2020 2020 2020 2020 2061 7574 6f5f 666f           auto_fo
-00007000: 726d 6174 203d 2054 7275 6520 2023 206f  rmat = True  # o
-00007010: 7665 7272 6964 6520 696e 7075 7420 7061  verride input pa
-00007020: 7261 6d65 7465 720a 2020 2020 2020 2020  rameter.        
-00007030: 2020 2020 2020 2020 7072 655f 6368 6563          pre_chec
-00007040: 6b65 6420 3d20 5472 7565 0a20 2020 2020  ked = True.     
-00007050: 2020 2020 2020 2069 6620 6861 735f 6174         if has_at
-00007060: 7472 6962 7574 653a 0a20 2020 2020 2020  tribute:.       
-00007070: 2020 2020 2020 2020 2073 656c 662e 6f72           self.or
-00007080: 6967 696e 616c 5f73 7472 696e 6720 3d20  iginal_string = 
-00007090: 7661 6c2e 6f72 6967 696e 616c 5f73 7472  val.original_str
-000070a0: 696e 670a 0a20 2020 2020 2020 2073 656c  ing..        sel
-000070b0: 662e 6175 746f 5f66 6f72 6d61 7420 3d20  f.auto_format = 
-000070c0: 6175 746f 5f66 6f72 6d61 740a 2020 2020  auto_format.    
-000070d0: 2020 2020 6966 2073 656c 662e 6175 746f      if self.auto
-000070e0: 5f66 6f72 6d61 7420 616e 6420 6e6f 7420  _format and not 
-000070f0: 7072 655f 6368 6563 6b65 643a 0a20 2020  pre_checked:.   
-00007100: 2020 2020 2020 2020 2023 2049 6620 6175           # If au
-00007110: 746f 5f66 6f72 6d61 7420 6973 2054 7275  to_format is Tru
-00007120: 652c 206b 6565 7020 7468 6520 666c 6f61  e, keep the floa
-00007130: 7420 7661 6c75 6520 7468 6520 7361 6d65  t value the same
-00007140: 2c20 6275 7420 6368 616e 6765 0a20 2020  , but change.   
-00007150: 2020 2020 2020 2020 2023 2074 6865 2073           # the s
-00007160: 7472 696e 6720 7265 7072 6573 656e 7461  tring representa
-00007170: 7469 6f6e 2073 746f 7265 6420 696e 206f  tion stored in o
-00007180: 7269 6769 6e61 6c5f 7374 7269 6e67 2069  riginal_string i
-00007190: 6620 6e65 6365 7373 6172 790a 2020 2020  f necessary.    
-000071a0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
-000071b0: 7472 2873 656c 662c 2027 6f72 6967 696e  tr(self, 'origin
-000071c0: 616c 5f73 7472 696e 6727 293a 0a20 2020  al_string'):.   
-000071d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000071e0: 6e6f 7420 6973 5f76 616c 6964 5f64 7328  not is_valid_ds(
-000071f0: 7365 6c66 2e6f 7269 6769 6e61 6c5f 7374  self.original_st
-00007200: 7269 6e67 293a 0a20 2020 2020 2020 2020  ring):.         
-00007210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007220: 6f72 6967 696e 616c 5f73 7472 696e 6720  original_string 
-00007230: 3d20 666f 726d 6174 5f6e 756d 6265 725f  = format_number_
-00007240: 6173 5f64 7328 0a20 2020 2020 2020 2020  as_ds(.         
-00007250: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00007260: 6c6f 6174 2873 656c 662e 6f72 6967 696e  loat(self.origin
-00007270: 616c 5f73 7472 696e 6729 0a20 2020 2020  al_string).     
-00007280: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00007290: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000072a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000072b0: 2020 2073 656c 662e 6f72 6967 696e 616c     self.original
-000072c0: 5f73 7472 696e 6720 3d20 666f 726d 6174  _string = format
-000072d0: 5f6e 756d 6265 725f 6173 5f64 7328 7365  _number_as_ds(se
-000072e0: 6c66 290a 0a20 2020 2020 2020 2069 6620  lf)..        if 
-000072f0: 2876 616c 6964 6174 696f 6e5f 6d6f 6465  (validation_mode
-00007300: 203d 3d20 636f 6e66 6967 2e52 4149 5345   == config.RAISE
-00007310: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00007320: 2020 2020 206e 6f74 2073 656c 662e 6175       not self.au
-00007330: 746f 5f66 6f72 6d61 7429 3a0a 2020 2020  to_format):.    
-00007340: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00007350: 6570 7228 7365 6c66 295b 313a 2d31 5d29  epr(self)[1:-1])
-00007360: 203e 2031 363a 0a20 2020 2020 2020 2020   > 16:.         
-00007370: 2020 2020 2020 2072 6169 7365 204f 7665         raise Ove
-00007380: 7266 6c6f 7745 7272 6f72 280a 2020 2020  rflowError(.    
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2256 616c 7565 7320 666f 7220 656c 656d  "Values for elem
-000073b0: 656e 7473 2077 6974 6820 6120 5652 206f  ents with a VR o
-000073c0: 6620 2744 5327 206d 7573 7420 6265 203c  f 'DS' must be <
-000073d0: 3d20 3136 2022 0a20 2020 2020 2020 2020  = 16 ".         
-000073e0: 2020 2020 2020 2020 2020 2022 6368 6172             "char
-000073f0: 6163 7465 7273 206c 6f6e 672c 2062 7574  acters long, but
-00007400: 2074 6865 2066 6c6f 6174 2070 726f 7669   the float provi
-00007410: 6465 6420 7265 7175 6972 6573 203e 2031  ded requires > 1
-00007420: 3620 220a 2020 2020 2020 2020 2020 2020  6 ".            
-00007430: 2020 2020 2020 2020 2263 6861 7261 6374          "charact
-00007440: 6572 7320 746f 2062 6520 6163 6375 7261  ers to be accura
-00007450: 7465 6c79 2072 6570 7265 7365 6e74 6564  tely represented
-00007460: 2e20 5573 6520 6120 736d 616c 6c65 7220  . Use a smaller 
-00007470: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00007480: 2020 2020 2020 2273 7472 696e 672c 2073        "string, s
-00007490: 6574 2027 636f 6e66 6967 2e73 6574 7469  et 'config.setti
-000074a0: 6e67 732e 7265 6164 696e 675f 7661 6c69  ngs.reading_vali
-000074b0: 6461 7469 6f6e 5f6d 6f64 6527 2074 6f20  dation_mode' to 
-000074c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000074d0: 2020 2020 2020 2227 5741 524e 2720 746f        "'WARN' to
-000074e0: 206f 7665 7272 6964 6520 7468 6520 6c65   override the le
-000074f0: 6e67 7468 2063 6865 636b 2c20 6f72 2022  ngth check, or "
-00007500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007510: 2020 2020 2022 6578 706c 6963 6974 6c79       "explicitly
-00007520: 2063 6f6e 7374 7275 6374 2061 2044 5320   construct a DS 
-00007530: 6f62 6a65 6374 2077 6974 6820 2761 7574  object with 'aut
-00007540: 6f5f 666f 726d 6174 2720 220a 2020 2020  o_format' ".    
-00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2273 6574 2074 6f20 5472 7565 220a 2020  "set to True".  
-00007570: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00007580: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00007590: 6f74 2069 735f 7661 6c69 645f 6473 2872  ot is_valid_ds(r
-000075a0: 6570 7228 7365 6c66 295b 313a 2d31 5d29  epr(self)[1:-1])
-000075b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000075c0: 2020 2320 5468 6973 2077 696c 6c20 6361    # This will ca
-000075d0: 7463 6820 6e61 6e20 616e 6420 696e 660a  tch nan and inf.
-000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00007600: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00007610: 2020 2020 2020 6627 5661 6c75 6520 227b        f'Value "{
-00007620: 7374 7228 7365 6c66 297d 2220 6973 206e  str(self)}" is n
-00007630: 6f74 2076 616c 6964 2066 6f72 2065 6c65  ot valid for ele
-00007640: 6d65 6e74 7320 7769 7468 2061 2056 5220  ments with a VR 
-00007650: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00007660: 2020 2020 2020 276f 6620 4453 270a 2020        'of DS'.  
-00007670: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00007680: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
-00007690: 7365 6c66 2c20 6f74 6865 723a 2041 6e79  self, other: Any
-000076a0: 2920 2d3e 2041 6e79 3a0a 2020 2020 2020  ) -> Any:.      
-000076b0: 2020 2222 224f 7665 7272 6964 6520 746f    """Override to
-000076c0: 2061 6c6c 6f77 2073 7472 696e 6720 6571   allow string eq
-000076d0: 7561 6c69 7479 2063 6f6d 7061 7269 736f  uality compariso
-000076e0: 6e73 2e22 2222 0a20 2020 2020 2020 2069  ns.""".        i
-000076f0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-00007700: 6572 2c20 7374 7229 3a0a 2020 2020 2020  er, str):.      
-00007710: 2020 2020 2020 7265 7475 726e 2073 7472        return str
-00007720: 2873 656c 6629 203d 3d20 6f74 6865 720a  (self) == other.
-00007730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007740: 7375 7065 7228 292e 5f5f 6571 5f5f 286f  super().__eq__(o
-00007750: 7468 6572 290a 0a20 2020 2064 6566 205f  ther)..    def _
-00007760: 5f68 6173 685f 5f28 7365 6c66 2920 2d3e  _hash__(self) ->
-00007770: 2069 6e74 3a0a 2020 2020 2020 2020 7265   int:.        re
-00007780: 7475 726e 2073 7570 6572 2829 2e5f 5f68  turn super().__h
-00007790: 6173 685f 5f28 290a 0a20 2020 2064 6566  ash__()..    def
-000077a0: 205f 5f6e 655f 5f28 7365 6c66 2c20 6f74   __ne__(self, ot
-000077b0: 6865 723a 2041 6e79 2920 2d3e 2041 6e79  her: Any) -> Any
-000077c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000077d0: 206e 6f74 2073 656c 6620 3d3d 206f 7468   not self == oth
-000077e0: 6572 0a0a 2020 2020 6465 6620 5f5f 7374  er..    def __st
-000077f0: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
-00007800: 3a0a 2020 2020 2020 2020 6966 2068 6173  :.        if has
-00007810: 6174 7472 2873 656c 662c 2027 6f72 6967  attr(self, 'orig
-00007820: 696e 616c 5f73 7472 696e 6727 2920 616e  inal_string') an
-00007830: 6420 6e6f 7420 7365 6c66 2e61 7574 6f5f  d not self.auto_
-00007840: 666f 726d 6174 3a0a 2020 2020 2020 2020  format:.        
-00007850: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00007860: 6f72 6967 696e 616c 5f73 7472 696e 670a  original_string.
-00007870: 0a20 2020 2020 2020 2023 2049 7373 7565  .        # Issue
-00007880: 2023 3933 3720 2850 7974 686f 6e20 332e   #937 (Python 3.
-00007890: 3820 636f 6d70 6174 6962 696c 6974 7929  8 compatibility)
-000078a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000078b0: 7265 7072 2873 656c 6629 5b31 3a2d 315d  repr(self)[1:-1]
-000078c0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-000078d0: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
-000078e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000078f0: 2e61 7574 6f5f 666f 726d 6174 2061 6e64  .auto_format and
-00007900: 2068 6173 6174 7472 2873 656c 662c 2027   hasattr(self, '
-00007910: 6f72 6967 696e 616c 5f73 7472 696e 6727  original_string'
-00007920: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00007930: 6574 7572 6e20 6622 277b 7365 6c66 2e6f  eturn f"'{self.o
-00007940: 7269 6769 6e61 6c5f 7374 7269 6e67 7d27  riginal_string}'
-00007950: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00007960: 6e20 6622 277b 7375 7065 7228 292e 5f5f  n f"'{super().__
-00007970: 7265 7072 5f5f 2829 7d27 220a 0a0a 636c  repr__()}'"...cl
-00007980: 6173 7320 4453 6465 6369 6d61 6c28 4465  ass DSdecimal(De
-00007990: 6369 6d61 6c29 3a0a 2020 2020 2222 2253  cimal):.    """S
-000079a0: 746f 7265 2076 616c 7565 2066 6f72 2061  tore value for a
-000079b0: 6e20 656c 656d 656e 7420 7769 7468 2056  n element with V
-000079c0: 5220 2a2a 4453 2a2a 2061 7320 3a63 6c61  R **DS** as :cla
-000079d0: 7373 3a60 6465 6369 6d61 6c2e 4465 6369  ss:`decimal.Deci
-000079e0: 6d61 6c60 2e0a 0a20 2020 2050 6172 616d  mal`...    Param
-000079f0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00007a00: 2d2d 2d2d 0a20 2020 2076 616c 3a20 556e  ----.    val: Un
-00007a10: 696f 6e5b 7374 722c 2069 6e74 2c20 666c  ion[str, int, fl
-00007a20: 6f61 742c 2044 6563 696d 616c 5d0a 2020  oat, Decimal].  
-00007a30: 2020 2020 2020 5661 6c75 6520 746f 2073        Value to s
-00007a40: 746f 7265 2061 7320 6120 4453 2e0a 2020  tore as a DS..  
-00007a50: 2020 6175 746f 5f66 6f72 6d61 743a 2062    auto_format: b
-00007a60: 6f6f 6c0a 2020 2020 2020 2020 4966 2054  ool.        If T
-00007a70: 7275 652c 2061 7574 6f6d 6174 6963 616c  rue, automatical
-00007a80: 6c79 2066 6f72 6d61 7420 7468 6520 7374  ly format the st
-00007a90: 7269 6e67 2072 6570 7265 7365 6e74 6174  ring representat
-00007aa0: 696f 6e20 6f66 2074 6869 730a 2020 2020  ion of this.    
-00007ab0: 2020 2020 6e75 6d62 6572 2074 6f20 656e      number to en
-00007ac0: 7375 7265 2069 7420 7361 7469 7366 6965  sure it satisfie
-00007ad0: 7320 7468 6520 636f 6e73 7472 6169 6e74  s the constraint
-00007ae0: 7320 696e 2074 6865 2044 4943 4f4d 2073  s in the DICOM s
-00007af0: 7461 6e64 6172 642e 0a20 2020 2020 2020  tandard..       
-00007b00: 204e 6f74 6520 7468 6174 2074 6869 7320   Note that this 
-00007b10: 7769 6c6c 206c 6561 6420 746f 206c 6f73  will lead to los
-00007b20: 7320 6f66 2070 7265 6369 7369 6f6e 2066  s of precision f
-00007b30: 6f72 2073 6f6d 6520 6e75 6d62 6572 732e  or some numbers.
-00007b40: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
-00007b50: 2d2d 2d2d 2d0a 2020 2020 4966 2063 6f6e  -----.    If con
-00007b60: 7374 7275 6374 6564 2066 726f 6d20 616e  structed from an
-00007b70: 2065 6d70 7479 2073 7472 696e 672c 2072   empty string, r
-00007b80: 6574 7572 6e73 2074 6865 2065 6d70 7479  eturns the empty
-00007b90: 2073 7472 696e 672c 206e 6f74 2061 6e0a   string, not an.
-00007ba0: 2020 2020 696e 7374 616e 6365 206f 6620      instance of 
-00007bb0: 7468 6973 2063 6c61 7373 2e0a 0a20 2020  this class...   
-00007bc0: 2022 2222 0a20 2020 2061 7574 6f5f 666f   """.    auto_fo
-00007bd0: 726d 6174 3a20 626f 6f6c 0a0a 2020 2020  rmat: bool..    
-00007be0: 6465 6620 5f5f 6e65 775f 5f28 2020 2320  def __new__(  # 
-00007bf0: 7479 7065 3a20 6967 6e6f 7265 5b6d 6973  type: ignore[mis
-00007c00: 635d 0a20 2020 2020 2020 2063 6c73 3a20  c].        cls: 
-00007c10: 5479 7065 5b22 4453 6465 6369 6d61 6c22  Type["DSdecimal"
-00007c20: 5d2c 0a20 2020 2020 2020 2076 616c 3a20  ],.        val: 
-00007c30: 556e 696f 6e5b 4e6f 6e65 2c20 7374 722c  Union[None, str,
-00007c40: 2069 6e74 2c20 666c 6f61 742c 2044 6563   int, float, Dec
-00007c50: 696d 616c 5d2c 0a20 2020 2020 2020 2061  imal],.        a
-00007c60: 7574 6f5f 666f 726d 6174 3a20 626f 6f6c  uto_format: bool
-00007c70: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00007c80: 2020 7661 6c69 6461 7469 6f6e 5f6d 6f64    validation_mod
-00007c90: 653a 2069 6e74 203d 204e 6f6e 650a 2020  e: int = None.  
-00007ca0: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
-00007cb0: 556e 696f 6e5b 7374 722c 2022 4453 6465  Union[str, "DSde
-00007cc0: 6369 6d61 6c22 5d5d 3a0a 2020 2020 2020  cimal"]]:.      
-00007cd0: 2020 2222 2243 7265 6174 6520 616e 2069    """Create an i
-00007ce0: 6e73 7461 6e63 6520 6f66 2044 5320 6f62  nstance of DS ob
-00007cf0: 6a65 6374 2c20 6f72 2072 6574 7572 6e20  ject, or return 
-00007d00: 6120 626c 616e 6b20 7374 7269 6e67 2069  a blank string i
-00007d10: 6620 6f6e 6520 6973 0a20 2020 2020 2020  f one is.       
-00007d20: 2070 6173 7365 6420 696e 2c20 652e 672e   passed in, e.g.
-00007d30: 2066 726f 6d20 6120 7479 7065 2032 2044   from a type 2 D
-00007d40: 4943 4f4d 2062 6c61 6e6b 2076 616c 7565  ICOM blank value
-00007d50: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00007d60: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00007d70: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00007d80: 2076 616c 203a 2073 7472 206f 7220 6e75   val : str or nu
-00007d90: 6d65 7269 630a 2020 2020 2020 2020 2020  meric.          
-00007da0: 2020 4120 7374 7269 6e67 206f 7220 6120    A string or a 
-00007db0: 6e75 6d62 6572 2074 7970 6520 7768 6963  number type whic
-00007dc0: 6820 6361 6e20 6265 2063 6f6e 7665 7274  h can be convert
-00007dd0: 6564 2074 6f20 6120 6465 6369 6d61 6c2e  ed to a decimal.
-00007de0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007df0: 2020 2020 2069 6620 7661 6c20 6973 204e       if val is N
-00007e00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00007e10: 2072 6574 7572 6e20 7661 6c0a 0a20 2020   return val..   
-00007e20: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00007e30: 6365 2876 616c 2c20 7374 7229 2061 6e64  ce(val, str) and
-00007e40: 2076 616c 2e73 7472 6970 2829 203d 3d20   val.strip() == 
-00007e50: 2727 3a0a 2020 2020 2020 2020 2020 2020  '':.            
-00007e60: 7265 7475 726e 2076 616c 0a0a 2020 2020  return val..    
-00007e70: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00007e80: 6528 7661 6c2c 2066 6c6f 6174 2920 616e  e(val, float) an
-00007e90: 6420 6e6f 7420 636f 6e66 6967 2e61 6c6c  d not config.all
-00007ea0: 6f77 5f44 535f 666c 6f61 743a 0a20 2020  ow_DS_float:.   
-00007eb0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00007ec0: 7970 6545 7272 6f72 280a 2020 2020 2020  ypeError(.      
-00007ed0: 2020 2020 2020 2020 2020 2227 4453 2720            "'DS' 
-00007ee0: 6361 6e6e 6f74 2062 6520 696e 7374 616e  cannot be instan
-00007ef0: 7469 6174 6564 2077 6974 6820 6120 666c  tiated with a fl
-00007f00: 6f61 7420 7661 6c75 6520 756e 6c65 7373  oat value unless
-00007f10: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00007f20: 2020 2022 2763 6f6e 6669 672e 616c 6c6f     "'config.allo
-00007f30: 775f 4453 5f66 6c6f 6174 2720 6973 2073  w_DS_float' is s
-00007f40: 6574 2074 6f20 5472 7565 2e20 596f 7520  et to True. You 
-00007f50: 7368 6f75 6c64 2063 6f6e 7665 7274 2022  should convert "
-00007f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007f70: 2022 7468 6520 7661 6c75 6520 746f 2061   "the value to a
-00007f80: 2073 7472 696e 6720 7769 7468 2074 6865   string with the
-00007f90: 2064 6573 6972 6564 206e 756d 6265 7220   desired number 
-00007fa0: 6f66 2064 6967 6974 732c 2022 0a20 2020  of digits, ".   
-00007fb0: 2020 2020 2020 2020 2020 2020 2022 6f72               "or
-00007fc0: 2075 7365 2027 4465 6369 6d61 6c2e 7175   use 'Decimal.qu
-00007fd0: 616e 7469 7a65 2829 2720 616e 6420 7061  antize()' and pa
-00007fe0: 7373 2061 2027 4465 6369 6d61 6c27 2069  ss a 'Decimal' i
-00007ff0: 6e73 7461 6e63 652e 220a 2020 2020 2020  nstance.".      
-00008000: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00008010: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00008020: 5f5f 6e65 775f 5f28 636c 732c 2076 616c  __new__(cls, val
-00008030: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
-00008040: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00008050: 662c 0a20 2020 2020 2020 2076 616c 3a20  f,.        val: 
-00008060: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
-00008070: 666c 6f61 742c 2044 6563 696d 616c 5d2c  float, Decimal],
-00008080: 0a20 2020 2020 2020 2061 7574 6f5f 666f  .        auto_fo
-00008090: 726d 6174 3a20 626f 6f6c 203d 2046 616c  rmat: bool = Fal
-000080a0: 7365 2c0a 2020 2020 2020 2020 7661 6c69  se,.        vali
-000080b0: 6461 7469 6f6e 5f6d 6f64 653a 2069 6e74  dation_mode: int
-000080c0: 203d 204e 6f6e 650a 2020 2020 2920 2d3e   = None.    ) ->
-000080d0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000080e0: 2222 5374 6f72 6520 7468 6520 6f72 6967  ""Store the orig
-000080f0: 696e 616c 2073 7472 696e 6720 6966 206f  inal string if o
-00008100: 6e65 2067 6976 656e 2c20 666f 7220 6578  ne given, for ex
-00008110: 6163 7420 7772 6974 652d 6f75 7420 6f66  act write-out of
-00008120: 2073 616d 650a 2020 2020 2020 2020 7661   same.        va
-00008130: 6c75 6520 6c61 7465 722e 2045 2e67 2e20  lue later. E.g. 
-00008140: 6966 2073 6574 2060 6027 312e 3233 6532  if set ``'1.23e2
-00008150: 2760 602c 203a 636c 6173 733a 607e 6465  '``, :class:`~de
-00008160: 6369 6d61 6c2e 4465 6369 6d61 6c60 2077  cimal.Decimal` w
-00008170: 6f75 6c64 0a20 2020 2020 2020 2077 7269  ould.        wri
-00008180: 7465 2060 6027 3132 3327 6060 2c20 6275  te ``'123'``, bu
-00008190: 7420 3a63 6c61 7373 3a60 4453 6020 7769  t :class:`DS` wi
-000081a0: 6c6c 2075 7365 2074 6865 206f 7269 6769  ll use the origi
-000081b0: 6e61 6c2e 0a20 2020 2020 2020 2022 2222  nal..        """
-000081c0: 0a20 2020 2020 2020 2069 6620 7661 6c69  .        if vali
-000081d0: 6461 7469 6f6e 5f6d 6f64 6520 6973 204e  dation_mode is N
-000081e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000081f0: 2076 616c 6964 6174 696f 6e5f 6d6f 6465   validation_mode
-00008200: 203d 2063 6f6e 6669 672e 7365 7474 696e   = config.settin
-00008210: 6773 2e72 6561 6469 6e67 5f76 616c 6964  gs.reading_valid
-00008220: 6174 696f 6e5f 6d6f 6465 0a0a 2020 2020  ation_mode..    
-00008230: 2020 2020 2320 2e2e 2e20 616c 736f 2069      # ... also i
-00008240: 6620 7573 6572 2063 6861 6e67 6573 2061  f user changes a
-00008250: 2064 6174 6120 656c 656d 656e 7420 7661   data element va
-00008260: 6c75 652c 2074 6865 6e20 7769 6c6c 2067  lue, then will g
-00008270: 6574 0a20 2020 2020 2020 2023 2061 2064  et.        # a d
-00008280: 6966 6665 7265 6e74 2044 6563 696d 616c  ifferent Decimal
-00008290: 2c20 6173 2044 6563 696d 616c 2069 7320  , as Decimal is 
-000082a0: 696d 6d75 7461 626c 652e 0a20 2020 2020  immutable..     
-000082b0: 2020 2070 7265 5f63 6865 636b 6564 203d     pre_checked =
-000082c0: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
-000082d0: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-000082e0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-000082f0: 2020 2020 7365 6c66 2e6f 7269 6769 6e61      self.origina
-00008300: 6c5f 7374 7269 6e67 203d 2076 616c 2e73  l_string = val.s
-00008310: 7472 6970 2829 0a20 2020 2020 2020 2065  trip().        e
-00008320: 6c69 6620 6973 696e 7374 616e 6365 2876  lif isinstance(v
-00008330: 616c 2c20 2844 5366 6c6f 6174 2c20 4453  al, (DSfloat, DS
-00008340: 6465 6369 6d61 6c29 293a 0a20 2020 2020  decimal)):.     
-00008350: 2020 2020 2020 2069 6620 7661 6c2e 6175         if val.au
-00008360: 746f 5f66 6f72 6d61 743a 0a20 2020 2020  to_format:.     
-00008370: 2020 2020 2020 2020 2020 2061 7574 6f5f             auto_
-00008380: 666f 726d 6174 203d 2054 7275 6520 2023  format = True  #
-00008390: 206f 7665 7272 6964 6520 696e 7075 7420   override input 
-000083a0: 7061 7261 6d65 7465 720a 2020 2020 2020  parameter.      
-000083b0: 2020 2020 2020 2020 2020 7072 655f 6368            pre_ch
-000083c0: 6563 6b65 6420 3d20 5472 7565 0a0a 2020  ecked = True..  
-000083d0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-000083e0: 6174 7472 2876 616c 2c20 276f 7269 6769  attr(val, 'origi
-000083f0: 6e61 6c5f 7374 7269 6e67 2729 3a0a 2020  nal_string'):.  
-00008400: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008410: 6c66 2e6f 7269 6769 6e61 6c5f 7374 7269  lf.original_stri
-00008420: 6e67 203d 2076 616c 2e6f 7269 6769 6e61  ng = val.origina
-00008430: 6c5f 7374 7269 6e67 0a0a 2020 2020 2020  l_string..      
-00008440: 2020 7365 6c66 2e61 7574 6f5f 666f 726d    self.auto_form
-00008450: 6174 203d 2061 7574 6f5f 666f 726d 6174  at = auto_format
-00008460: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00008470: 2e61 7574 6f5f 666f 726d 6174 2061 6e64  .auto_format and
-00008480: 206e 6f74 2070 7265 5f63 6865 636b 6564   not pre_checked
-00008490: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000084a0: 4966 2061 7574 6f5f 666f 726d 6174 2069  If auto_format i
-000084b0: 7320 5472 7565 2c20 6b65 6570 2074 6865  s True, keep the
-000084c0: 2066 6c6f 6174 2076 616c 7565 2074 6865   float value the
-000084d0: 2073 616d 652c 2062 7574 2063 6861 6e67   same, but chang
-000084e0: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
-000084f0: 7468 6520 7374 7269 6e67 2072 6570 7265  the string repre
-00008500: 7365 6e74 6174 696f 6e20 7374 6f72 6564  sentation stored
-00008510: 2069 6e20 6f72 6967 696e 616c 5f73 7472   in original_str
-00008520: 696e 6720 6966 206e 6563 6573 7361 7279  ing if necessary
-00008530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00008540: 6861 7361 7474 7228 7365 6c66 2c20 276f  hasattr(self, 'o
-00008550: 7269 6769 6e61 6c5f 7374 7269 6e67 2729  riginal_string')
-00008560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008570: 2020 6966 206e 6f74 2069 735f 7661 6c69    if not is_vali
-00008580: 645f 6473 2873 656c 662e 6f72 6967 696e  d_ds(self.origin
-00008590: 616c 5f73 7472 696e 6729 3a0a 2020 2020  al_string):.    
-000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085b0: 7365 6c66 2e6f 7269 6769 6e61 6c5f 7374  self.original_st
-000085c0: 7269 6e67 203d 2066 6f72 6d61 745f 6e75  ring = format_nu
-000085d0: 6d62 6572 5f61 735f 6473 280a 2020 2020  mber_as_ds(.    
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 2020 2020 666c 6f61 7428 7365 6c66 2e6f      float(self.o
-00008600: 7269 6769 6e61 6c5f 7374 7269 6e67 290a  riginal_string).
-00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008620: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00008630: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008640: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
-00008650: 6769 6e61 6c5f 7374 7269 6e67 203d 2066  ginal_string = f
-00008660: 6f72 6d61 745f 6e75 6d62 6572 5f61 735f  ormat_number_as_
-00008670: 6473 2873 656c 6629 0a0a 2020 2020 2020  ds(self)..      
-00008680: 2020 6966 2076 616c 6964 6174 696f 6e5f    if validation_
-00008690: 6d6f 6465 2021 3d20 636f 6e66 6967 2e49  mode != config.I
-000086a0: 474e 4f52 453a 0a20 2020 2020 2020 2020  GNORE:.         
-000086b0: 2020 2069 6620 6c65 6e28 7265 7072 2873     if len(repr(s
-000086c0: 656c 6629 2e73 7472 6970 2822 2722 2929  elf).strip("'"))
-000086d0: 203e 2031 363a 0a20 2020 2020 2020 2020   > 16:.         
-000086e0: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
-000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008700: 2020 2022 5661 6c75 6573 2066 6f72 2065     "Values for e
-00008710: 6c65 6d65 6e74 7320 7769 7468 2061 2056  lements with a V
-00008720: 5220 6f66 2027 4453 2720 7661 6c75 6573  R of 'DS' values
-00008730: 206d 7573 7420 6265 2022 0a20 2020 2020   must be ".     
-00008740: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008750: 3c3d 2031 3620 6368 6172 6163 7465 7273  <= 16 characters
-00008760: 206c 6f6e 672e 2055 7365 2061 2073 6d61   long. Use a sma
-00008770: 6c6c 6572 2073 7472 696e 672c 2073 6574  ller string, set
-00008780: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00008790: 2020 2020 2020 2022 2763 6f6e 6669 672e         "'config.
-000087a0: 7365 7474 696e 6773 2e72 6561 6469 6e67  settings.reading
-000087b0: 5f76 616c 6964 6174 696f 6e5f 6d6f 6465  _validation_mode
-000087c0: 2720 746f 2022 0a20 2020 2020 2020 2020  ' to ".         
-000087d0: 2020 2020 2020 2020 2020 2022 2757 4152             "'WAR
-000087e0: 4e27 2074 6f20 6f76 6572 7269 6465 2074  N' to override t
-000087f0: 6865 206c 656e 6774 6820 6368 6563 6b2c  he length check,
-00008800: 2075 7365 2022 0a20 2020 2020 2020 2020   use ".         
-00008810: 2020 2020 2020 2020 2020 2022 2744 6563             "'Dec
-00008820: 696d 616c 2e71 7561 6e74 697a 6528 2927  imal.quantize()'
-00008830: 2061 6e64 2069 6e69 7469 616c 697a 6520   and initialize 
-00008840: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00008850: 2020 2020 2020 2277 6974 6820 6120 2744        "with a 'D
-00008860: 6563 696d 616c 2720 696e 7374 616e 6365  ecimal' instance
-00008870: 2c20 6f72 2065 7870 6c69 6369 746c 7920  , or explicitly 
-00008880: 636f 6e73 7472 7563 7420 6120 4453 2022  construct a DS "
-00008890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088a0: 2020 2020 2022 696e 7374 616e 6365 2077       "instance w
-000088b0: 6974 6820 2761 7574 6f5f 666f 726d 6174  ith 'auto_format
-000088c0: 2720 7365 7420 746f 2054 7275 6522 0a20  ' set to True". 
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000088e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088f0: 2069 6620 7661 6c69 6461 7469 6f6e 5f6d   if validation_m
-00008900: 6f64 6520 3d3d 2063 6f6e 6669 672e 5241  ode == config.RA
-00008910: 4953 453a 0a20 2020 2020 2020 2020 2020  ISE:.           
-00008920: 2020 2020 2020 2020 2072 6169 7365 204f           raise O
-00008930: 7665 7266 6c6f 7745 7272 6f72 286d 7367  verflowError(msg
-00008940: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008950: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00008960: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
-00008970: 2069 6620 6e6f 7420 6973 5f76 616c 6964   if not is_valid
-00008980: 5f64 7328 7265 7072 2873 656c 6629 2e73  _ds(repr(self).s
-00008990: 7472 6970 2822 2722 2929 3a0a 2020 2020  trip("'")):.    
-000089a0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-000089b0: 6973 2077 696c 6c20 6361 7463 6820 6e61  is will catch na
-000089c0: 6e20 616e 6420 696e 660a 2020 2020 2020  n and inf.      
-000089d0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-000089e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000089f0: 2020 2020 2020 6627 5661 6c75 6520 227b        f'Value "{
-00008a00: 7374 7228 7365 6c66 297d 2220 6973 206e  str(self)}" is n
-00008a10: 6f74 2076 616c 6964 2066 6f72 2065 6c65  ot valid for ele
-00008a20: 6d65 6e74 7320 7769 7468 2061 2056 5220  ments with a VR 
-00008a30: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00008a40: 2020 2020 2020 276f 6620 4453 270a 2020        'of DS'.  
-00008a50: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 6966 2076 616c 6964 6174 696f 6e5f 6d6f  if validation_mo
-00008a80: 6465 203d 3d20 636f 6e66 6967 2e52 4149  de == config.RAI
-00008a90: 5345 3a0a 2020 2020 2020 2020 2020 2020  SE:.            
-00008aa0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00008ab0: 6c75 6545 7272 6f72 286d 7367 290a 2020  lueError(msg).  
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-00008ad0: 726e 696e 6773 2e77 6172 6e28 6d73 6729  rnings.warn(msg)
-00008ae0: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
-00008af0: 2873 656c 662c 206f 7468 6572 3a20 416e  (self, other: An
-00008b00: 7929 202d 3e20 416e 793a 0a20 2020 2020  y) -> Any:.     
-00008b10: 2020 2022 2222 4f76 6572 7269 6465 2074     """Override t
-00008b20: 6f20 616c 6c6f 7720 7374 7269 6e67 2065  o allow string e
-00008b30: 7175 616c 6974 7920 636f 6d70 6172 6973  quality comparis
-00008b40: 6f6e 732e 2222 220a 2020 2020 2020 2020  ons.""".        
-00008b50: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
-00008b60: 6865 722c 2073 7472 293a 0a20 2020 2020  her, str):.     
-00008b70: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00008b80: 7228 7365 6c66 2920 3d3d 206f 7468 6572  r(self) == other
-00008b90: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00008ba0: 2073 7570 6572 2829 2e5f 5f65 715f 5f28   super().__eq__(
-00008bb0: 6f74 6865 7229 0a0a 2020 2020 6465 6620  other)..    def 
-00008bc0: 5f5f 6861 7368 5f5f 2873 656c 6629 202d  __hash__(self) -
-00008bd0: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
-00008be0: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
-00008bf0: 6861 7368 5f5f 2829 0a0a 2020 2020 6465  hash__()..    de
-00008c00: 6620 5f5f 6e65 5f5f 2873 656c 662c 206f  f __ne__(self, o
-00008c10: 7468 6572 3a20 416e 7929 202d 3e20 416e  ther: Any) -> An
-00008c20: 793a 0a20 2020 2020 2020 2072 6574 7572  y:.        retur
-00008c30: 6e20 6e6f 7420 7365 6c66 203d 3d20 6f74  n not self == ot
-00008c40: 6865 720a 0a20 2020 2064 6566 205f 5f73  her..    def __s
-00008c50: 7472 5f5f 2873 656c 6629 202d 3e20 7374  tr__(self) -> st
-00008c60: 723a 0a20 2020 2020 2020 2068 6173 5f73  r:.        has_s
-00008c70: 7472 203d 2068 6173 6174 7472 2873 656c  tr = hasattr(sel
-00008c80: 662c 2027 6f72 6967 696e 616c 5f73 7472  f, 'original_str
-00008c90: 696e 6727 290a 2020 2020 2020 2020 6966  ing').        if
-00008ca0: 2068 6173 5f73 7472 2061 6e64 206c 656e   has_str and len
-00008cb0: 2873 656c 662e 6f72 6967 696e 616c 5f73  (self.original_s
-00008cc0: 7472 696e 6729 203c 3d20 3136 3a0a 2020  tring) <= 16:.  
-00008cd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008ce0: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
-00008cf0: 7472 696e 670a 0a20 2020 2020 2020 2072  tring..        r
-00008d00: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
-00008d10: 7374 725f 5f28 290a 0a20 2020 2064 6566  str__()..    def
-00008d20: 205f 5f72 6570 725f 5f28 7365 6c66 2920   __repr__(self) 
-00008d30: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-00008d40: 6966 2073 656c 662e 6175 746f 5f66 6f72  if self.auto_for
-00008d50: 6d61 7420 616e 6420 6861 7361 7474 7228  mat and hasattr(
-00008d60: 7365 6c66 2c20 276f 7269 6769 6e61 6c5f  self, 'original_
-00008d70: 7374 7269 6e67 2729 3a0a 2020 2020 2020  string'):.      
-00008d80: 2020 2020 2020 7265 7475 726e 2066 2227        return f"'
-00008d90: 7b73 656c 662e 6f72 6967 696e 616c 5f73  {self.original_s
-00008da0: 7472 696e 677d 2722 0a20 2020 2020 2020  tring}'".       
-00008db0: 2072 6574 7572 6e20 6622 277b 7374 7228   return f"'{str(
-00008dc0: 7365 6c66 297d 2722 0a0a 0a23 2043 484f  self)}'"...# CHO
-00008dd0: 4f53 4520 5459 5045 204f 4620 4453 0a44  OSE TYPE OF DS.D
-00008de0: 5363 6c61 7373 3a20 416e 790a 6966 2063  Sclass: Any.if c
-00008df0: 6f6e 6669 672e 7573 655f 4453 5f64 6563  onfig.use_DS_dec
-00008e00: 696d 616c 3a0a 2020 2020 4453 636c 6173  imal:.    DSclas
-00008e10: 7320 3d20 4453 6465 6369 6d61 6c0a 656c  s = DSdecimal.el
-00008e20: 7365 3a0a 2020 2020 4453 636c 6173 7320  se:.    DSclass 
-00008e30: 3d20 4453 666c 6f61 740a 0a0a 6465 6620  = DSfloat...def 
-00008e40: 4453 280a 2020 2020 7661 6c3a 2055 6e69  DS(.    val: Uni
-00008e50: 6f6e 5b4e 6f6e 652c 2073 7472 2c20 696e  on[None, str, in
-00008e60: 742c 2066 6c6f 6174 2c20 4465 6369 6d61  t, float, Decima
-00008e70: 6c5d 2c20 6175 746f 5f66 6f72 6d61 743a  l], auto_format:
-00008e80: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00008e90: 2020 2076 616c 6964 6174 696f 6e5f 6d6f     validation_mo
-00008ea0: 6465 3a20 696e 7420 3d20 4e6f 6e65 0a29  de: int = None.)
-00008eb0: 202d 3e20 556e 696f 6e5b 4e6f 6e65 2c20   -> Union[None, 
-00008ec0: 7374 722c 2044 5366 6c6f 6174 2c20 4453  str, DSfloat, DS
-00008ed0: 6465 6369 6d61 6c5d 3a0a 2020 2020 2222  decimal]:.    ""
-00008ee0: 2246 6163 746f 7279 2066 756e 6374 696f  "Factory functio
-00008ef0: 6e20 666f 7220 6372 6561 7469 6e67 2044  n for creating D
-00008f00: 5320 636c 6173 7320 696e 7374 616e 6365  S class instance
-00008f10: 732e 0a0a 2020 2020 4368 6563 6b73 2066  s...    Checks f
-00008f20: 6f72 2062 6c61 6e6b 2073 7472 696e 673b  or blank string;
-00008f30: 2069 6620 736f 2c20 7265 7475 726e 7320   if so, returns 
-00008f40: 7468 6174 2c20 656c 7365 2063 616c 6c73  that, else calls
-00008f50: 203a 636c 6173 733a 6044 5366 6c6f 6174   :class:`DSfloat
-00008f60: 600a 2020 2020 6f72 203a 636c 6173 733a  `.    or :class:
-00008f70: 6044 5364 6563 696d 616c 6020 746f 2063  `DSdecimal` to c
-00008f80: 7265 6174 6520 7468 6520 636c 6173 7320  reate the class 
-00008f90: 696e 7374 616e 6365 2e20 5468 6973 2061  instance. This a
-00008fa0: 766f 6964 7320 6f76 6572 7269 6469 6e67  voids overriding
-00008fb0: 0a20 2020 2060 6044 5366 6c6f 6174 2e5f  .    ``DSfloat._
-00008fc0: 5f6e 6577 5f5f 2829 6060 2028 7768 6963  _new__()`` (whic
-00008fd0: 6820 6361 7272 6965 7320 6120 7469 6d65  h carries a time
-00008fe0: 2070 656e 616c 7479 2066 6f72 206c 6172   penalty for lar
-00008ff0: 6765 2061 7272 6179 7320 6f66 0a20 2020  ge arrays of.   
-00009000: 2044 5329 2e0a 0a20 2020 2053 696d 696c   DS)...    Simil
-00009010: 6172 6c79 2074 6865 2073 7472 696e 6720  arly the string 
-00009020: 636c 6561 6e20 616e 6420 6368 6563 6b20  clean and check 
-00009030: 6361 6e20 6265 2061 766f 6964 6564 2061  can be avoided a
-00009040: 6e64 203a 636c 6173 733a 6044 5366 6c6f  nd :class:`DSflo
-00009050: 6174 600a 2020 2020 6361 6c6c 6564 2064  at`.    called d
-00009060: 6972 6563 746c 7920 6966 2061 2073 7472  irectly if a str
-00009070: 696e 6720 6861 7320 616c 7265 6164 7920  ing has already 
-00009080: 6265 656e 2070 726f 6365 7373 6564 2e0a  been processed..
-00009090: 2020 2020 2222 220a 2020 2020 6966 2076      """.    if v
-000090a0: 616c 2069 7320 4e6f 6e65 3a0a 2020 2020  al is None:.    
-000090b0: 2020 2020 7265 7475 726e 2076 616c 0a0a      return val..
-000090c0: 2020 2020 6966 2076 616c 6964 6174 696f      if validatio
-000090d0: 6e5f 6d6f 6465 2069 7320 4e6f 6e65 3a0a  n_mode is None:.
-000090e0: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
-000090f0: 6f6e 5f6d 6f64 6520 3d20 636f 6e66 6967  on_mode = config
-00009100: 2e73 6574 7469 6e67 732e 7265 6164 696e  .settings.readin
-00009110: 675f 7661 6c69 6461 7469 6f6e 5f6d 6f64  g_validation_mod
-00009120: 650a 0a20 2020 2069 6620 6973 696e 7374  e..    if isinst
-00009130: 616e 6365 2876 616c 2c20 7374 7229 3a0a  ance(val, str):.
-00009140: 2020 2020 2020 2020 6966 2076 616c 2e73          if val.s
-00009150: 7472 6970 2829 203d 3d20 2727 3a0a 2020  trip() == '':.  
-00009160: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009170: 2076 616c 0a20 2020 2020 2020 2076 616c   val.        val
-00009180: 6964 6174 655f 7661 6c75 6528 2244 5322  idate_value("DS"
-00009190: 2c20 7661 6c2c 2076 616c 6964 6174 696f  , val, validatio
-000091a0: 6e5f 6d6f 6465 290a 0a20 2020 2069 6620  n_mode)..    if 
-000091b0: 636f 6e66 6967 2e75 7365 5f44 535f 6465  config.use_DS_de
-000091c0: 6369 6d61 6c3a 0a20 2020 2020 2020 2072  cimal:.        r
-000091d0: 6574 7572 6e20 4453 6465 6369 6d61 6c28  eturn DSdecimal(
-000091e0: 7661 6c2c 2061 7574 6f5f 666f 726d 6174  val, auto_format
-000091f0: 2c20 7661 6c69 6461 7469 6f6e 5f6d 6f64  , validation_mod
-00009200: 6529 0a0a 2020 2020 7265 7475 726e 2044  e)..    return D
-00009210: 5366 6c6f 6174 2876 616c 2c20 6175 746f  Sfloat(val, auto
-00009220: 5f66 6f72 6d61 742c 2076 616c 6964 6174  _format, validat
-00009230: 696f 6e5f 6d6f 6465 290a 0a0a 636c 6173  ion_mode)...clas
-00009240: 7320 4953 2869 6e74 293a 0a20 2020 2022  s IS(int):.    "
-00009250: 2222 5374 6f72 6520 7661 6c75 6520 666f  ""Store value fo
-00009260: 7220 616e 2065 6c65 6d65 6e74 2077 6974  r an element wit
-00009270: 6820 5652 202a 2a49 532a 2a20 6173 203a  h VR **IS** as :
-00009280: 636c 6173 733a 6069 6e74 602e 0a0a 2020  class:`int`...  
-00009290: 2020 5374 6f72 6573 206f 7269 6769 6e61    Stores origina
-000092a0: 6c20 696e 7465 6765 7220 7374 7269 6e67  l integer string
-000092b0: 2066 6f72 2065 7861 6374 2072 6577 7269   for exact rewri
-000092c0: 7469 6e67 206f 6620 7468 6520 7374 7269  ting of the stri
-000092d0: 6e67 0a20 2020 206f 7269 6769 6e61 6c6c  ng.    originall
-000092e0: 7920 7265 6164 206f 7220 7374 6f72 6564  y read or stored
-000092f0: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00009300: 6566 205f 5f6e 6577 5f5f 2820 2023 2074  ef __new__(  # t
-00009310: 7970 653a 2069 676e 6f72 655b 6d69 7363  ype: ignore[misc
-00009320: 5d0a 2020 2020 2020 2020 2020 2020 636c  ].            cl
-00009330: 733a 2054 7970 655b 2249 5322 5d2c 2076  s: Type["IS"], v
-00009340: 616c 3a20 556e 696f 6e5b 4e6f 6e65 2c20  al: Union[None, 
-00009350: 7374 722c 2069 6e74 2c20 666c 6f61 742c  str, int, float,
-00009360: 2044 6563 696d 616c 5d2c 0a20 2020 2020   Decimal],.     
-00009370: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
-00009380: 6e5f 6d6f 6465 3a20 696e 7420 3d20 4e6f  n_mode: int = No
-00009390: 6e65 0a20 2020 2029 202d 3e20 4f70 7469  ne.    ) -> Opti
-000093a0: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
-000093b0: 2249 5322 5d5d 3a0a 2020 2020 2020 2020  "IS"]]:.        
-000093c0: 2222 2243 7265 6174 6520 696e 7374 616e  """Create instan
-000093d0: 6365 2069 6620 6e65 7720 696e 7465 6765  ce if new intege
-000093e0: 7220 7374 7269 6e67 2222 220a 2020 2020  r string""".    
-000093f0: 2020 2020 6966 2076 616c 2069 7320 4e6f      if val is No
-00009400: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00009410: 7265 7475 726e 2076 616c 0a0a 2020 2020  return val..    
-00009420: 2020 2020 6966 2076 616c 6964 6174 696f      if validatio
-00009430: 6e5f 6d6f 6465 2069 7320 4e6f 6e65 3a0a  n_mode is None:.
-00009440: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
-00009450: 6461 7469 6f6e 5f6d 6f64 6520 3d20 636f  dation_mode = co
-00009460: 6e66 6967 2e73 6574 7469 6e67 732e 7265  nfig.settings.re
-00009470: 6164 696e 675f 7661 6c69 6461 7469 6f6e  ading_validation
-00009480: 5f6d 6f64 650a 0a20 2020 2020 2020 2069  _mode..        i
-00009490: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-000094a0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-000094b0: 2020 2020 6966 2076 616c 2e73 7472 6970      if val.strip
-000094c0: 2829 203d 3d20 2727 3a0a 2020 2020 2020  () == '':.      
-000094d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000094e0: 2076 616c 0a20 2020 2020 2020 2020 2020   val.           
-000094f0: 2076 616c 6964 6174 655f 7661 6c75 6528   validate_value(
-00009500: 2249 5322 2c20 7661 6c2c 2076 616c 6964  "IS", val, valid
-00009510: 6174 696f 6e5f 6d6f 6465 290a 0a20 2020  ation_mode)..   
-00009520: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00009530: 2020 2020 2020 6e65 7776 616c 203d 2073        newval = s
-00009540: 7570 6572 2829 2e5f 5f6e 6577 5f5f 2863  uper().__new__(c
-00009550: 6c73 2c20 7661 6c29 0a20 2020 2020 2020  ls, val).       
-00009560: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00009570: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00009580: 2320 6163 6365 7074 2066 6c6f 6174 2073  # accept float s
-00009590: 7472 696e 6773 2077 6865 6e20 6e6f 2069  trings when no i
-000095a0: 6e74 6567 6572 206c 6f73 732c 2065 2e67  nteger loss, e.g
-000095b0: 2e20 2231 2e30 220a 2020 2020 2020 2020  . "1.0".        
-000095c0: 2020 2020 6e65 7776 616c 203d 2073 7570      newval = sup
-000095d0: 6572 2829 2e5f 5f6e 6577 5f5f 2863 6c73  er().__new__(cls
-000095e0: 2c20 666c 6f61 7428 7661 6c29 290a 0a20  , float(val)).. 
-000095f0: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-00009600: 6620 6120 666c 6f61 7420 6f72 2044 6563  f a float or Dec
-00009610: 696d 616c 2070 6173 7365 6420 696e 2c20  imal passed in, 
-00009620: 7468 656e 2063 6f75 6c64 2068 6176 6520  then could have 
-00009630: 6c6f 7374 2069 6e66 6f2c 0a20 2020 2020  lost info,.     
-00009640: 2020 2023 2061 6e64 2077 696c 6c20 7261     # and will ra
-00009650: 6973 6520 6572 726f 722e 2045 2e67 2e20  ise error. E.g. 
-00009660: 4953 2844 6563 696d 616c 2827 3127 2929  IS(Decimal('1'))
-00009670: 2069 7320 6f6b 2c20 6275 7420 6e6f 7420   is ok, but not 
-00009680: 4953 2831 2e32 3329 0a20 2020 2020 2020  IS(1.23).       
-00009690: 2023 2020 2049 5328 2731 2e32 3327 2920   #   IS('1.23') 
-000096a0: 7769 6c6c 2072 6169 7365 2056 616c 7565  will raise Value
-000096b0: 4572 726f 720a 2020 2020 2020 2020 6966  Error.        if
-000096c0: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
-000096d0: 2028 666c 6f61 742c 2044 6563 696d 616c   (float, Decimal
-000096e0: 2c20 7374 7229 2920 616e 6420 6e65 7776  , str)) and newv
-000096f0: 616c 2021 3d20 666c 6f61 7428 7661 6c29  al != float(val)
-00009700: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00009710: 6973 6520 5479 7065 4572 726f 7228 2243  ise TypeError("C
-00009720: 6f75 6c64 206e 6f74 2063 6f6e 7665 7274  ould not convert
-00009730: 2076 616c 7565 2074 6f20 696e 7465 6765   value to intege
-00009740: 7220 7769 7468 6f75 7420 6c6f 7373 2229  r without loss")
-00009750: 0a0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
-00009760: 6b73 2069 6e20 6361 7365 2075 6e64 6572  ks in case under
-00009770: 6c79 696e 6720 696e 7420 6973 203e 3332  lying int is >32
-00009780: 2062 6974 732c 2044 4943 4f4d 2064 6f65   bits, DICOM doe
-00009790: 7320 6e6f 7420 616c 6c6f 7720 7468 6973  s not allow this
-000097a0: 0a20 2020 2020 2020 2069 6620 286e 6f74  .        if (not
-000097b0: 202d 322a 2a33 3120 3c3d 206e 6577 7661   -2**31 <= newva
-000097c0: 6c20 3c20 322a 2a33 3120 616e 640a 2020  l < 2**31 and.  
-000097d0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-000097e0: 6c69 6461 7469 6f6e 5f6d 6f64 6520 3d3d  lidation_mode ==
-000097f0: 2063 6f6e 6669 672e 5241 4953 4529 3a0a   config.RAISE):.
-00009800: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009810: 6520 4f76 6572 666c 6f77 4572 726f 7228  e OverflowError(
-00009820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009830: 2022 456c 656d 656e 7473 2077 6974 6820   "Elements with 
-00009840: 6120 5652 206f 6620 4953 206d 7573 7420  a VR of IS must 
-00009850: 6861 7665 2061 2076 616c 7565 2062 6574  have a value bet
-00009860: 7765 656e 202d 322a 2a33 3120 220a 2020  ween -2**31 ".  
-00009870: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00009880: 6e64 2028 322a 2a33 3120 2d20 3129 2e20  nd (2**31 - 1). 
-00009890: 5365 7420 220a 2020 2020 2020 2020 2020  Set ".          
-000098a0: 2020 2020 2020 2227 636f 6e66 6967 2e73        "'config.s
-000098b0: 6574 7469 6e67 732e 7265 6164 696e 675f  ettings.reading_
-000098c0: 7661 6c69 6461 7469 6f6e 5f6d 6f64 6527  validation_mode'
-000098d0: 2074 6f20 220a 2020 2020 2020 2020 2020   to ".          
-000098e0: 2020 2020 2020 2227 5741 524e 2720 746f        "'WARN' to
-000098f0: 206f 7665 7272 6964 6520 7468 6520 7661   override the va
-00009900: 6c75 6520 6368 6563 6b22 0a20 2020 2020  lue check".     
-00009910: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00009920: 2020 7265 7475 726e 206e 6577 7661 6c0a    return newval.
-00009930: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00009940: 5f28 7365 6c66 2c20 7661 6c3a 2055 6e69  _(self, val: Uni
-00009950: 6f6e 5b73 7472 2c20 696e 742c 2066 6c6f  on[str, int, flo
-00009960: 6174 2c20 4465 6369 6d61 6c5d 2c0a 2020  at, Decimal],.  
-00009970: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00009980: 616c 6964 6174 696f 6e5f 6d6f 6465 3a20  alidation_mode: 
-00009990: 696e 7420 3d20 4e6f 6e65 2920 2d3e 204e  int = None) -> N
-000099a0: 6f6e 653a 0a20 2020 2020 2020 2023 2049  one:.        # I
-000099b0: 6620 6120 7374 7269 6e67 2070 6173 7365  f a string passe
-000099c0: 642c 2074 6865 6e20 7374 6f72 6520 6974  d, then store it
-000099d0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-000099e0: 7374 616e 6365 2876 616c 2c20 7374 7229  stance(val, str)
-000099f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00009a00: 6c66 2e6f 7269 6769 6e61 6c5f 7374 7269  lf.original_stri
-00009a10: 6e67 203d 2076 616c 2e73 7472 6970 2829  ng = val.strip()
-00009a20: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-00009a30: 696e 7374 616e 6365 2876 616c 2c20 4953  instance(val, IS
-00009a40: 2920 616e 6420 6861 7361 7474 7228 7661  ) and hasattr(va
-00009a50: 6c2c 2027 6f72 6967 696e 616c 5f73 7472  l, 'original_str
-00009a60: 696e 6727 293a 0a20 2020 2020 2020 2020  ing'):.         
-00009a70: 2020 2073 656c 662e 6f72 6967 696e 616c     self.original
-00009a80: 5f73 7472 696e 6720 3d20 7661 6c2e 6f72  _string = val.or
-00009a90: 6967 696e 616c 5f73 7472 696e 670a 0a20  iginal_string.. 
-00009aa0: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
-00009ab0: 6c66 2c20 6f74 6865 723a 2041 6e79 2920  lf, other: Any) 
-00009ac0: 2d3e 2041 6e79 3a0a 2020 2020 2020 2020  -> Any:.        
-00009ad0: 2222 224f 7665 7272 6964 6520 746f 2061  """Override to a
-00009ae0: 6c6c 6f77 2073 7472 696e 6720 6571 7561  llow string equa
-00009af0: 6c69 7479 2063 6f6d 7061 7269 736f 6e73  lity comparisons
-00009b00: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
-00009b10: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
-00009b20: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00009b30: 2020 2020 7265 7475 726e 2073 7472 2873      return str(s
-00009b40: 656c 6629 203d 3d20 6f74 6865 720a 0a20  elf) == other.. 
-00009b50: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00009b60: 7065 7228 292e 5f5f 6571 5f5f 286f 7468  per().__eq__(oth
-00009b70: 6572 290a 0a20 2020 2064 6566 205f 5f68  er)..    def __h
-00009b80: 6173 685f 5f28 7365 6c66 2920 2d3e 2069  ash__(self) -> i
-00009b90: 6e74 3a0a 2020 2020 2020 2020 7265 7475  nt:.        retu
-00009ba0: 726e 2073 7570 6572 2829 2e5f 5f68 6173  rn super().__has
-00009bb0: 685f 5f28 290a 0a20 2020 2064 6566 205f  h__()..    def _
-00009bc0: 5f6e 655f 5f28 7365 6c66 2c20 6f74 6865  _ne__(self, othe
-00009bd0: 723a 2041 6e79 2920 2d3e 2041 6e79 3a0a  r: Any) -> Any:.
-00009be0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00009bf0: 6f74 2073 656c 6620 3d3d 206f 7468 6572  ot self == other
-00009c00: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
-00009c10: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0a  _(self) -> str:.
-00009c20: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
-00009c30: 7472 2873 656c 662c 2027 6f72 6967 696e  tr(self, 'origin
-00009c40: 616c 5f73 7472 696e 6727 293a 0a20 2020  al_string'):.   
-00009c50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00009c60: 7365 6c66 2e6f 7269 6769 6e61 6c5f 7374  self.original_st
-00009c70: 7269 6e67 0a0a 2020 2020 2020 2020 2320  ring..        # 
-00009c80: 4973 7375 6520 2339 3337 2028 5079 7468  Issue #937 (Pyth
-00009c90: 6f6e 2033 2e38 2063 6f6d 7061 7469 6269  on 3.8 compatibi
-00009ca0: 6c69 7479 290a 2020 2020 2020 2020 7265  lity).        re
-00009cb0: 7475 726e 2072 6570 7228 7365 6c66 295b  turn repr(self)[
-00009cc0: 313a 2d31 5d0a 0a20 2020 2064 6566 205f  1:-1]..    def _
-00009cd0: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
-00009ce0: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
-00009cf0: 7475 726e 2066 2227 7b73 7570 6572 2829  turn f"'{super()
-00009d00: 2e5f 5f72 6570 725f 5f28 297d 2722 0a0a  .__repr__()}'"..
-00009d10: 0a5f 5420 3d20 5479 7065 5661 7228 275f  ._T = TypeVar('_
-00009d20: 5427 290a 0a0a 6465 6620 4d75 6c74 6953  T')...def MultiS
-00009d30: 7472 696e 6728 0a20 2020 2020 2020 2076  tring(.        v
-00009d40: 616c 3a20 7374 722c 2076 616c 7479 7065  al: str, valtype
-00009d50: 3a20 4f70 7469 6f6e 616c 5b43 616c 6c61  : Optional[Calla
-00009d60: 626c 655b 5b73 7472 5d2c 205f 545d 5d20  ble[[str], _T]] 
-00009d70: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00009d80: 7661 6c69 6461 7469 6f6e 5f6d 6f64 653a  validation_mode:
-00009d90: 2069 6e74 203d 204e 6f6e 650a 2920 2d3e   int = None.) ->
-00009da0: 2055 6e69 6f6e 5b5f 542c 204d 7574 6162   Union[_T, Mutab
-00009db0: 6c65 5365 7175 656e 6365 5b5f 545d 5d3a  leSequence[_T]]:
-00009dc0: 0a20 2020 2022 2222 5370 6c69 7420 6120  .    """Split a 
-00009dd0: 7374 7269 6e67 2062 7920 6465 6c69 6d69  string by delimi
-00009de0: 7465 7273 2069 6620 7468 6572 6520 6172  ters if there ar
-00009df0: 6520 616e 790a 0a20 2020 2050 6172 616d  e any..    Param
-00009e00: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00009e10: 2d2d 2d2d 0a20 2020 2076 616c 203a 2073  ----.    val : s
-00009e20: 7472 0a20 2020 2020 2020 2054 6865 2073  tr.        The s
-00009e30: 7472 696e 6720 746f 2073 706c 6974 2075  tring to split u
-00009e40: 702e 0a20 2020 2076 616c 7479 7065 203a  p..    valtype :
-00009e50: 2074 7970 6520 6f72 2063 616c 6c61 626c   type or callabl
-00009e60: 652c 206f 7074 696f 6e61 6c0a 2020 2020  e, optional.    
-00009e70: 2020 2020 4465 6661 756c 7420 3a63 6c61      Default :cla
-00009e80: 7373 3a60 7374 7260 2c20 6275 7420 6361  ss:`str`, but ca
-00009e90: 6e20 6265 2065 2e67 2e20 3a63 6c61 7373  n be e.g. :class
-00009ea0: 3a60 7e70 7964 6963 6f6d 2e75 6964 2e55  :`~pydicom.uid.U
-00009eb0: 4944 6020 746f 0a20 2020 2020 2020 206f  ID` to.        o
-00009ec0: 7665 7277 7269 7465 2074 6f20 6120 7370  verwrite to a sp
-00009ed0: 6563 6966 6963 2074 7970 652e 0a20 2020  ecific type..   
-00009ee0: 2076 616c 6964 6174 696f 6e5f 6d6f 6465   validation_mode
-00009ef0: 203a 2069 6e74 0a20 2020 2020 2020 2044   : int.        D
-00009f00: 6566 696e 6573 2069 6620 7661 6c75 6573  efines if values
-00009f10: 2061 7265 2076 616c 6964 6174 6564 2061   are validated a
-00009f20: 6e64 2068 6f77 2076 616c 6964 6174 696f  nd how validatio
-00009f30: 6e20 6572 726f 7273 2061 7265 0a20 2020  n errors are.   
-00009f40: 2020 2020 2068 616e 646c 6564 2e0a 0a20       handled... 
-00009f50: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00009f60: 2d2d 2d2d 2d2d 0a20 2020 2076 616c 7479  ------.    valty
-00009f70: 7065 206f 7220 4d75 6c74 6956 616c 7565  pe or MultiValue
-00009f80: 206f 6620 7661 6c74 7970 650a 2020 2020   of valtype.    
-00009f90: 2020 2020 5468 6520 7370 6c69 7420 7661      The split va
-00009fa0: 6c75 6520 6173 2060 7661 6c74 7970 6560  lue as `valtype`
-00009fb0: 206f 7220 6120 3a63 6c61 7373 3a60 6c69   or a :class:`li
-00009fc0: 7374 6020 6f66 2060 7661 6c74 7970 6560  st` of `valtype`
-00009fd0: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
-00009fe0: 2076 616c 7479 7065 2069 7320 4e6f 6e65   valtype is None
-00009ff0: 3a0a 2020 2020 2020 2020 7661 6c74 7970  :.        valtyp
-0000a000: 6520 3d20 6361 7374 2843 616c 6c61 626c  e = cast(Callabl
-0000a010: 655b 5b73 7472 5d2c 205f 545d 2c20 7374  e[[str], _T], st
-0000a020: 7229 0a0a 2020 2020 2320 5265 6d6f 7665  r)..    # Remove
-0000a030: 2074 7261 696c 696e 6720 626c 616e 6b20   trailing blank 
-0000a040: 7573 6564 2074 6f20 7061 6420 746f 2065  used to pad to e
-0000a050: 7665 6e20 6c65 6e67 7468 0a20 2020 2023  ven length.    #
-0000a060: 2032 3030 352e 3035 2e32 353a 2061 6c73   2005.05.25: als
-0000a070: 6f20 6368 6563 6b20 666f 7220 7472 6169  o check for trai
-0000a080: 6c69 6e67 2030 2c20 6572 726f 7220 6d61  ling 0, error ma
-0000a090: 6465 0a20 2020 2023 2069 6e20 5045 5420  de.    # in PET 
-0000a0a0: 6669 6c65 7320 7765 2061 7265 2063 6f6e  files we are con
-0000a0b0: 7665 7274 696e 670a 2020 2020 7768 696c  verting.    whil
-0000a0c0: 6520 7661 6c20 616e 6420 7661 6c2e 656e  e val and val.en
-0000a0d0: 6473 7769 7468 2828 2720 272c 2027 5c78  dswith((' ', '\x
-0000a0e0: 3030 2729 293a 0a20 2020 2020 2020 2076  00')):.        v
-0000a0f0: 616c 203d 2076 616c 5b3a 2d31 5d0a 0a20  al = val[:-1].. 
-0000a100: 2020 2073 706c 6974 7570 3a20 4c69 7374     splitup: List
-0000a110: 5b73 7472 5d20 3d20 7661 6c2e 7370 6c69  [str] = val.spli
-0000a120: 7428 225c 5c22 290a 2020 2020 6966 206c  t("\\").    if l
-0000a130: 656e 2873 706c 6974 7570 2920 3d3d 2031  en(splitup) == 1
-0000a140: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0000a150: 2076 616c 7479 7065 2873 706c 6974 7570   valtype(splitup
-0000a160: 5b30 5d29 0a0a 2020 2020 7265 7475 726e  [0])..    return
-0000a170: 204d 756c 7469 5661 6c75 6528 7661 6c74   MultiValue(valt
-0000a180: 7970 652c 2073 706c 6974 7570 2c20 7661  ype, splitup, va
-0000a190: 6c69 6461 7469 6f6e 5f6d 6f64 6529 0a0a  lidation_mode)..
-0000a1a0: 0a64 6566 205f 7665 7269 6679 5f65 6e63  .def _verify_enc
-0000a1b0: 6f64 696e 6773 280a 2020 2020 656e 636f  odings(.    enco
-0000a1c0: 6469 6e67 733a 204f 7074 696f 6e61 6c5b  dings: Optional[
-0000a1d0: 556e 696f 6e5b 7374 722c 2053 6571 7565  Union[str, Seque
-0000a1e0: 6e63 655b 7374 725d 5d5d 0a29 202d 3e20  nce[str]]].) -> 
-0000a1f0: 4f70 7469 6f6e 616c 5b54 7570 6c65 5b73  Optional[Tuple[s
-0000a200: 7472 2c20 2e2e 2e5d 5d3a 0a20 2020 2022  tr, ...]]:.    "
-0000a210: 2222 4368 6563 6b73 2074 6865 2065 6e63  ""Checks the enc
-0000a220: 6f64 696e 6720 746f 2065 6e73 7572 6520  oding to ensure 
-0000a230: 7072 6f70 6572 2066 6f72 6d61 7422 2222  proper format"""
-0000a240: 0a20 2020 2069 6620 656e 636f 6469 6e67  .    if encoding
-0000a250: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-0000a260: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-0000a270: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0000a280: 6528 656e 636f 6469 6e67 732c 2073 7472  e(encodings, str
-0000a290: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0000a2a0: 6e20 2865 6e63 6f64 696e 6773 2c29 0a0a  n (encodings,)..
-0000a2b0: 2020 2020 7265 7475 726e 2074 7570 6c65      return tuple
-0000a2c0: 2865 6e63 6f64 696e 6773 290a 0a0a 6465  (encodings)...de
-0000a2d0: 6620 5f64 6563 6f64 655f 7065 7273 6f6e  f _decode_person
-0000a2e0: 6e61 6d65 280a 2020 2020 636f 6d70 6f6e  name(.    compon
-0000a2f0: 656e 7473 3a20 5365 7175 656e 6365 5b62  ents: Sequence[b
-0000a300: 7974 6573 5d2c 2065 6e63 6f64 696e 6773  ytes], encodings
-0000a310: 3a20 5365 7175 656e 6365 5b73 7472 5d0a  : Sequence[str].
-0000a320: 2920 2d3e 2054 7570 6c65 5b73 7472 2c20  ) -> Tuple[str, 
-0000a330: 2e2e 2e5d 3a0a 2020 2020 2222 2252 6574  ...]:.    """Ret
-0000a340: 7572 6e20 6120 6c69 7374 206f 6620 6465  urn a list of de
-0000a350: 636f 6465 6420 7065 7273 6f6e 206e 616d  coded person nam
-0000a360: 6520 636f 6d70 6f6e 656e 7473 2e0a 0a20  e components... 
-0000a370: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000a380: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000a390: 2063 6f6d 706f 6e65 6e74 7320 3a20 6c69   components : li
-0000a3a0: 7374 206f 6620 6279 7465 730a 2020 2020  st of bytes.    
-0000a3b0: 2020 2020 5468 6520 6c69 7374 206f 6620      The list of 
-0000a3c0: 7468 6520 7570 2074 6f20 7468 7265 6520  the up to three 
-0000a3d0: 656e 636f 6465 6420 7065 7273 6f6e 206e  encoded person n
-0000a3e0: 616d 6520 636f 6d70 6f6e 656e 7473 0a20  ame components. 
-0000a3f0: 2020 2065 6e63 6f64 696e 6773 203a 206c     encodings : l
-0000a400: 6973 7420 6f66 2073 7472 0a20 2020 2020  ist of str.     
-0000a410: 2020 2054 6865 2050 7974 686f 6e20 656e     The Python en
-0000a420: 636f 6469 6e67 7320 7573 6573 2074 6f20  codings uses to 
-0000a430: 6465 636f 6465 2060 636f 6d70 6f6e 656e  decode `componen
-0000a440: 7473 602e 0a0a 2020 2020 5265 7475 726e  ts`...    Return
-0000a450: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-0000a460: 2020 7465 7874 2074 7970 650a 2020 2020    text type.    
-0000a470: 2020 2020 5468 6520 756e 6963 6f64 6520      The unicode 
-0000a480: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-0000a490: 696e 6720 7468 6520 7065 7273 6f6e 206e  ing the person n
-0000a4a0: 616d 652e 0a20 2020 2020 2020 2049 6620  ame..        If 
-0000a4b0: 7468 6520 6465 636f 6469 6e67 206f 6620  the decoding of 
-0000a4c0: 736f 6d65 2063 6f6d 706f 6e65 6e74 2070  some component p
-0000a4d0: 6172 7473 2069 7320 6e6f 7420 706f 7373  arts is not poss
-0000a4e0: 6962 6c65 2075 7369 6e67 2074 6865 0a20  ible using the. 
-0000a4f0: 2020 2020 2020 2067 6976 656e 2065 6e63         given enc
-0000a500: 6f64 696e 6773 2c20 7468 6579 2061 7265  odings, they are
-0000a510: 2064 6563 6f64 6564 2077 6974 6820 7468   decoded with th
-0000a520: 6520 6669 7273 7420 656e 636f 6469 6e67  e first encoding
-0000a530: 2075 7369 6e67 0a20 2020 2020 2020 2072   using.        r
-0000a540: 6570 6c61 6365 6d65 6e74 2063 6861 7261  eplacement chara
-0000a550: 6374 6572 7320 666f 7220 6279 7465 7320  cters for bytes 
-0000a560: 7468 6174 2063 616e 6e6f 7420 6265 2064  that cannot be d
-0000a570: 6563 6f64 6564 2e0a 2020 2020 2222 220a  ecoded..    """.
-0000a580: 2020 2020 6672 6f6d 2070 7964 6963 6f6d      from pydicom
-0000a590: 2e63 6861 7273 6574 2069 6d70 6f72 7420  .charset import 
-0000a5a0: 6465 636f 6465 5f62 7974 6573 0a0a 2020  decode_bytes..  
-0000a5b0: 2020 636f 6d70 7320 3d20 5b64 6563 6f64    comps = [decod
-0000a5c0: 655f 6279 7465 7328 632c 2065 6e63 6f64  e_bytes(c, encod
-0000a5d0: 696e 6773 2c20 504e 5f44 454c 494d 5329  ings, PN_DELIMS)
-0000a5e0: 2066 6f72 2063 2069 6e20 636f 6d70 6f6e   for c in compon
-0000a5f0: 656e 7473 5d0a 0a20 2020 2023 2052 656d  ents]..    # Rem
-0000a600: 6f76 6520 656d 7074 7920 656c 656d 656e  ove empty elemen
-0000a610: 7473 2066 726f 6d20 7468 6520 656e 6420  ts from the end 
-0000a620: 746f 2061 766f 6964 2074 7261 696c 696e  to avoid trailin
-0000a630: 6720 273d 270a 2020 2020 7768 696c 6520  g '='.    while 
-0000a640: 6c65 6e28 636f 6d70 7329 2061 6e64 206e  len(comps) and n
-0000a650: 6f74 2063 6f6d 7073 5b2d 315d 3a0a 2020  ot comps[-1]:.  
-0000a660: 2020 2020 2020 636f 6d70 732e 706f 7028        comps.pop(
-0000a670: 290a 0a20 2020 2072 6574 7572 6e20 7475  )..    return tu
-0000a680: 706c 6528 636f 6d70 7329 0a0a 0a64 6566  ple(comps)...def
-0000a690: 205f 656e 636f 6465 5f70 6572 736f 6e6e   _encode_personn
-0000a6a0: 616d 6528 0a20 2020 2063 6f6d 706f 6e65  ame(.    compone
-0000a6b0: 6e74 733a 2053 6571 7565 6e63 655b 7374  nts: Sequence[st
-0000a6c0: 725d 2c20 656e 636f 6469 6e67 733a 2053  r], encodings: S
-0000a6d0: 6571 7565 6e63 655b 7374 725d 0a29 202d  equence[str].) -
-0000a6e0: 3e20 6279 7465 733a 0a20 2020 2022 2222  > bytes:.    """
-0000a6f0: 456e 636f 6465 2061 206c 6973 7420 6f66  Encode a list of
-0000a700: 2074 6578 7420 7374 7269 6e67 2070 6572   text string per
-0000a710: 736f 6e20 6e61 6d65 2063 6f6d 706f 6e65  son name compone
-0000a720: 6e74 732e 0a0a 2020 2020 5061 7261 6d65  nts...    Parame
-0000a730: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0000a740: 2d2d 2d0a 2020 2020 636f 6d70 6f6e 656e  ---.    componen
-0000a750: 7473 203a 206c 6973 7420 6f66 2073 7472  ts : list of str
-0000a760: 0a20 2020 2020 2020 2054 6865 206c 6973  .        The lis
-0000a770: 7420 6f66 2074 6865 2075 7020 746f 2074  t of the up to t
-0000a780: 6872 6565 2075 6e69 636f 6465 2070 6572  hree unicode per
-0000a790: 736f 6e20 6e61 6d65 2063 6f6d 706f 6e65  son name compone
-0000a7a0: 6e74 730a 2020 2020 656e 636f 6469 6e67  nts.    encoding
-0000a7b0: 7320 3a20 6c69 7374 206f 6620 7374 720a  s : list of str.
-0000a7c0: 2020 2020 2020 2020 5468 6520 5079 7468          The Pyth
-0000a7d0: 6f6e 2065 6e63 6f64 696e 6773 2075 7365  on encodings use
-0000a7e0: 7320 746f 2065 6e63 6f64 6520 6063 6f6d  s to encode `com
-0000a7f0: 706f 6e65 6e74 7360 2e0a 0a20 2020 2052  ponents`...    R
-0000a800: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0000a810: 2d2d 0a20 2020 2062 7974 6520 7374 7269  --.    byte stri
-0000a820: 6e67 0a20 2020 2020 2020 2054 6865 2062  ng.        The b
-0000a830: 7974 6520 7374 7269 6e67 2074 6861 7420  yte string that 
-0000a840: 6361 6e20 6265 2077 7269 7474 656e 2061  can be written a
-0000a850: 7320 6120 504e 2044 4943 4f4d 2074 6167  s a PN DICOM tag
-0000a860: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
-0000a870: 4966 2074 6865 2065 6e63 6f64 696e 6720  If the encoding 
-0000a880: 6f66 2073 6f6d 6520 636f 6d70 6f6e 656e  of some componen
-0000a890: 7420 7061 7274 7320 6973 206e 6f74 2070  t parts is not p
-0000a8a0: 6f73 7369 626c 6520 7573 696e 6720 7468  ossible using th
-0000a8b0: 650a 2020 2020 2020 2020 6769 7665 6e20  e.        given 
-0000a8c0: 656e 636f 6469 6e67 732c 2074 6865 7920  encodings, they 
-0000a8d0: 6172 6520 656e 636f 6465 6420 7769 7468  are encoded with
-0000a8e0: 2074 6865 2066 6972 7374 2065 6e63 6f64   the first encod
-0000a8f0: 696e 6720 7573 696e 670a 2020 2020 2020  ing using.      
-0000a900: 2020 7265 706c 6163 656d 656e 7420 6279    replacement by
-0000a910: 7465 7320 666f 7220 6368 6172 6163 7465  tes for characte
-0000a920: 7273 2074 6861 7420 6361 6e6e 6f74 2062  rs that cannot b
-0000a930: 6520 656e 636f 6465 642e 0a20 2020 2022  e encoded..    "
-0000a940: 2222 0a20 2020 2066 726f 6d20 7079 6469  "".    from pydi
-0000a950: 636f 6d2e 6368 6172 7365 7420 696d 706f  com.charset impo
-0000a960: 7274 2065 6e63 6f64 655f 7374 7269 6e67  rt encode_string
-0000a970: 0a0a 2020 2020 656e 636f 6465 645f 636f  ..    encoded_co
-0000a980: 6d70 7320 3d20 5b5d 0a20 2020 2066 6f72  mps = [].    for
-0000a990: 2063 6f6d 7020 696e 2063 6f6d 706f 6e65   comp in compone
-0000a9a0: 6e74 733a 0a20 2020 2020 2020 2067 726f  nts:.        gro
-0000a9b0: 7570 7320 3d20 5b0a 2020 2020 2020 2020  ups = [.        
-0000a9c0: 2020 2020 656e 636f 6465 5f73 7472 696e      encode_strin
-0000a9d0: 6728 6772 6f75 702c 2065 6e63 6f64 696e  g(group, encodin
-0000a9e0: 6773 2920 666f 7220 6772 6f75 7020 696e  gs) for group in
-0000a9f0: 2063 6f6d 702e 7370 6c69 7428 275e 2729   comp.split('^')
-0000aa00: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-0000aa10: 2020 2065 6e63 6f64 6564 5f63 6f6d 7020     encoded_comp 
-0000aa20: 3d20 6227 5e27 2e6a 6f69 6e28 6772 6f75  = b'^'.join(grou
-0000aa30: 7073 290a 2020 2020 2020 2020 7661 6c69  ps).        vali
-0000aa40: 6461 7465 5f70 6e5f 636f 6d70 6f6e 656e  date_pn_componen
-0000aa50: 7428 656e 636f 6465 645f 636f 6d70 290a  t(encoded_comp).
-0000aa60: 2020 2020 2020 2020 656e 636f 6465 645f          encoded_
-0000aa70: 636f 6d70 732e 6170 7065 6e64 2865 6e63  comps.append(enc
-0000aa80: 6f64 6564 5f63 6f6d 7029 0a0a 2020 2020  oded_comp)..    
-0000aa90: 2320 5265 6d6f 7665 2065 6d70 7479 2065  # Remove empty e
-0000aaa0: 6c65 6d65 6e74 7320 6672 6f6d 2074 6865  lements from the
-0000aab0: 2065 6e64 0a20 2020 2077 6869 6c65 206c   end.    while l
-0000aac0: 656e 2865 6e63 6f64 6564 5f63 6f6d 7073  en(encoded_comps
-0000aad0: 2920 616e 6420 6e6f 7420 656e 636f 6465  ) and not encode
-0000aae0: 645f 636f 6d70 735b 2d31 5d3a 0a20 2020  d_comps[-1]:.   
-0000aaf0: 2020 2020 2065 6e63 6f64 6564 5f63 6f6d       encoded_com
-0000ab00: 7073 2e70 6f70 2829 0a20 2020 2072 6574  ps.pop().    ret
-0000ab10: 7572 6e20 6227 3d27 2e6a 6f69 6e28 656e  urn b'='.join(en
-0000ab20: 636f 6465 645f 636f 6d70 7329 0a0a 0a63  coded_comps)...c
-0000ab30: 6c61 7373 2050 6572 736f 6e4e 616d 653a  lass PersonName:
-0000ab40: 0a20 2020 2022 2222 5265 7072 6573 656e  .    """Represen
-0000ab50: 7461 7469 6f6e 206f 6620 7468 6520 7661  tation of the va
-0000ab60: 6c75 6520 666f 7220 616e 2065 6c65 6d65  lue for an eleme
-0000ab70: 6e74 2077 6974 6820 5652 202a 2a50 4e2a  nt with VR **PN*
-0000ab80: 2a2e 2222 220a 2020 2020 6465 6620 5f5f  *.""".    def __
-0000ab90: 6e65 775f 5f28 2020 2320 7479 7065 3a20  new__(  # type: 
-0000aba0: 6967 6e6f 7265 5b6d 6973 635d 0a20 2020  ignore[misc].   
-0000abb0: 2020 2020 2063 6c73 3a20 5479 7065 5b22       cls: Type["
-0000abc0: 5065 7273 6f6e 4e61 6d65 225d 2c20 2a61  PersonName"], *a
-0000abd0: 7267 733a 2041 6e79 2c20 2a2a 6b77 6172  rgs: Any, **kwar
-0000abe0: 6773 3a20 416e 790a 2020 2020 2920 2d3e  gs: Any.    ) ->
-0000abf0: 204f 7074 696f 6e61 6c5b 2250 6572 736f   Optional["Perso
-0000ac00: 6e4e 616d 6522 5d3a 0a20 2020 2020 2020  nName"]:.       
-0000ac10: 2069 6620 6c65 6e28 6172 6773 2920 616e   if len(args) an
-0000ac20: 6420 6172 6773 5b30 5d20 6973 204e 6f6e  d args[0] is Non
-0000ac30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000ac40: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-0000ac50: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-0000ac60: 2829 2e5f 5f6e 6577 5f5f 2863 6c73 290a  ().__new__(cls).
-0000ac70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000ac80: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0000ac90: 0a20 2020 2020 2020 2076 616c 3a20 556e  .        val: Un
-0000aca0: 696f 6e5b 6279 7465 732c 2073 7472 2c20  ion[bytes, str, 
-0000acb0: 2250 6572 736f 6e4e 616d 6522 5d2c 0a20  "PersonName"],. 
-0000acc0: 2020 2020 2020 2065 6e63 6f64 696e 6773         encodings
-0000acd0: 3a20 4f70 7469 6f6e 616c 5b53 6571 7565  : Optional[Seque
-0000ace0: 6e63 655b 7374 725d 5d20 3d20 4e6f 6e65  nce[str]] = None
-0000acf0: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
-0000ad00: 616c 5f73 7472 696e 673a 204f 7074 696f  al_string: Optio
-0000ad10: 6e61 6c5b 6279 7465 735d 203d 204e 6f6e  nal[bytes] = Non
-0000ad20: 652c 0a20 2020 2020 2020 2076 616c 6964  e,.        valid
-0000ad30: 6174 696f 6e5f 6d6f 6465 3a20 696e 7420  ation_mode: int 
-0000ad40: 3d20 4e6f 6e65 0a20 2020 2029 202d 3e20  = None.    ) -> 
-0000ad50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000ad60: 2243 7265 6174 6520 6120 6e65 7720 6060  "Create a new ``
-0000ad70: 5065 7273 6f6e 4e61 6d65 6060 2e0a 0a20  PersonName``... 
-0000ad80: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000ad90: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000ada0: 2d2d 2d2d 0a20 2020 2020 2020 2076 616c  ----.        val
-0000adb0: 3a20 7374 722c 2062 7974 6573 2c20 5065  : str, bytes, Pe
-0000adc0: 7273 6f6e 4e61 6d65 0a20 2020 2020 2020  rsonName.       
-0000add0: 2020 2020 2054 6865 2076 616c 7565 2074       The value t
-0000ade0: 6f20 7573 6520 666f 7220 7468 6520 2a2a  o use for the **
-0000adf0: 504e 2a2a 2065 6c65 6d65 6e74 2e0a 2020  PN** element..  
-0000ae00: 2020 2020 2020 656e 636f 6469 6e67 733a        encodings:
-0000ae10: 206c 6973 7420 6f66 2073 7472 2c20 6f70   list of str, op
-0000ae20: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0000ae30: 2020 2041 206c 6973 7420 6f66 2074 6865     A list of the
-0000ae40: 2065 6e63 6f64 696e 6773 2075 7365 6420   encodings used 
-0000ae50: 666f 7220 7468 6520 7661 6c75 652e 0a20  for the value.. 
-0000ae60: 2020 2020 2020 206f 7269 6769 6e61 6c5f         original_
-0000ae70: 7374 7269 6e67 3a20 6279 7465 732c 206f  string: bytes, o
-0000ae80: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000ae90: 2020 2020 5768 656e 2063 7265 6174 696e      When creatin
-0000aea0: 6720 6120 6060 5065 7273 6f6e 4e61 6d65  g a ``PersonName
-0000aeb0: 6060 2075 7369 6e67 2061 2064 6563 6f64  `` using a decod
-0000aec0: 6564 2073 7472 696e 672c 2074 6869 7320  ed string, this 
-0000aed0: 6973 2074 6865 0a20 2020 2020 2020 2020  is the.         
-0000aee0: 2020 206f 7269 6769 6e61 6c20 656e 636f     original enco
-0000aef0: 6465 6420 7661 6c75 652e 0a0a 2020 2020  ded value...    
-0000af00: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
-0000af10: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
-0000af20: 4120 3a63 6c61 7373 3a60 5065 7273 6f6e  A :class:`Person
-0000af30: 4e61 6d65 6020 6d61 7920 616c 736f 2062  Name` may also b
-0000af40: 6520 636f 6e73 7472 7563 7465 6420 6279  e constructed by
-0000af50: 2073 7065 6369 6679 696e 6720 696e 6469   specifying indi
-0000af60: 7669 6475 616c 0a20 2020 2020 2020 2063  vidual.        c
-0000af70: 6f6d 706f 6e65 6e74 7320 7573 696e 6720  omponents using 
-0000af80: 7468 6520 3a6d 6574 683a 6066 726f 6d5f  the :meth:`from_
-0000af90: 6e61 6d65 645f 636f 6d70 6f6e 656e 7473  named_components
-0000afa0: 6020 616e 640a 2020 2020 2020 2020 3a6d  ` and.        :m
-0000afb0: 6574 683a 6066 726f 6d5f 6e61 6d65 645f  eth:`from_named_
-0000afc0: 636f 6d70 6f6e 656e 7473 5f76 6574 6572  components_veter
-0000afd0: 696e 6172 7960 2063 6c61 7373 206d 6574  inary` class met
-0000afe0: 686f 6473 2e0a 2020 2020 2020 2020 2222  hods..        ""
-0000aff0: 220a 2020 2020 2020 2020 7365 6c66 2e6f  ".        self.o
-0000b000: 7269 6769 6e61 6c5f 7374 7269 6e67 3a20  riginal_string: 
-0000b010: 6279 7465 730a 2020 2020 2020 2020 7365  bytes.        se
-0000b020: 6c66 2e5f 636f 6d70 6f6e 656e 7473 3a20  lf._components: 
-0000b030: 4f70 7469 6f6e 616c 5b54 7570 6c65 5b73  Optional[Tuple[s
-0000b040: 7472 2c20 2e2e 2e5d 5d20 3d20 4e6f 6e65  tr, ...]] = None
-0000b050: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-0000b060: 636f 6469 6e67 733a 204f 7074 696f 6e61  codings: Optiona
-0000b070: 6c5b 5475 706c 655b 7374 722c 202e 2e2e  l[Tuple[str, ...
-0000b080: 5d5d 0a20 2020 2020 2020 2069 6620 7661  ]].        if va
-0000b090: 6c69 6461 7469 6f6e 5f6d 6f64 6520 6973  lidation_mode is
-0000b0a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b0b0: 2020 2076 616c 6964 6174 696f 6e5f 6d6f     validation_mo
-0000b0c0: 6465 203d 2063 6f6e 6669 672e 7365 7474  de = config.sett
-0000b0d0: 696e 6773 2e72 6561 6469 6e67 5f76 616c  ings.reading_val
-0000b0e0: 6964 6174 696f 6e5f 6d6f 6465 0a20 2020  idation_mode.   
-0000b0f0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0000b100: 7469 6f6e 5f6d 6f64 6520 3d20 7661 6c69  tion_mode = vali
-0000b110: 6461 7469 6f6e 5f6d 6f64 650a 0a20 2020  dation_mode..   
-0000b120: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000b130: 6365 2876 616c 2c20 5065 7273 6f6e 4e61  ce(val, PersonNa
-0000b140: 6d65 293a 0a20 2020 2020 2020 2020 2020  me):.           
-0000b150: 2065 6e63 6f64 696e 6773 203d 2076 616c   encodings = val
-0000b160: 2e65 6e63 6f64 696e 6773 0a20 2020 2020  .encodings.     
-0000b170: 2020 2020 2020 2073 656c 662e 6f72 6967         self.orig
-0000b180: 696e 616c 5f73 7472 696e 6720 3d20 7661  inal_string = va
-0000b190: 6c2e 6f72 6967 696e 616c 5f73 7472 696e  l.original_strin
-0000b1a0: 670a 2020 2020 2020 2020 2020 2020 7365  g.            se
-0000b1b0: 6c66 2e5f 636f 6d70 6f6e 656e 7473 203d  lf._components =
-0000b1c0: 2074 7570 6c65 2873 7472 2876 616c 292e   tuple(str(val).
-0000b1d0: 7370 6c69 7428 273d 2729 290a 2020 2020  split('=')).    
-0000b1e0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-0000b1f0: 6e63 6528 7661 6c2c 2062 7974 6573 293a  nce(val, bytes):
-0000b200: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
-0000b210: 6869 7320 6973 2074 6865 2072 6177 2062  his is the raw b
-0000b220: 7974 6520 7374 7269 6e67 202d 2064 6563  yte string - dec
-0000b230: 6f64 6520 6974 206f 6e20 6465 6d61 6e64  ode it on demand
-0000b240: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b250: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
-0000b260: 6720 3d20 7661 6c0a 2020 2020 2020 2020  g = val.        
-0000b270: 2020 2020 7661 6c69 6461 7465 5f76 616c      validate_val
-0000b280: 7565 2822 504e 222c 2076 616c 2c20 7661  ue("PN", val, va
-0000b290: 6c69 6461 7469 6f6e 5f6d 6f64 6529 0a20  lidation_mode). 
-0000b2a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b2b0: 5f63 6f6d 706f 6e65 6e74 7320 3d20 4e6f  _components = No
-0000b2c0: 6e65 0a20 2020 2020 2020 2065 6c73 653a  ne.        else:
-0000b2d0: 0a20 2020 2020 2020 2020 2020 2023 2076  .            # v
-0000b2e0: 616c 3a20 7374 720a 2020 2020 2020 2020  al: str.        
-0000b2f0: 2020 2020 2320 6076 616c 6020 6973 2074      # `val` is t
-0000b300: 6865 2064 6563 6f64 6564 2070 6572 736f  he decoded perso
-0000b310: 6e20 6e61 6d65 2076 616c 7565 0a20 2020  n name value.   
-0000b320: 2020 2020 2020 2020 2023 2060 6f72 6967           # `orig
-0000b330: 696e 616c 5f73 7472 696e 6760 2073 686f  inal_string` sho
-0000b340: 756c 6420 6265 2074 6865 206f 7269 6769  uld be the origi
-0000b350: 6e61 6c20 656e 636f 6465 6420 7661 6c75  nal encoded valu
-0000b360: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-0000b370: 6c66 2e6f 7269 6769 6e61 6c5f 7374 7269  lf.original_stri
-0000b380: 6e67 203d 2063 6173 7428 6279 7465 732c  ng = cast(bytes,
-0000b390: 206f 7269 6769 6e61 6c5f 7374 7269 6e67   original_string
-0000b3a0: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0000b3b0: 6966 2077 6520 646f 6e27 7420 6861 7665  if we don't have
-0000b3c0: 2074 6865 2062 7974 6520 7374 7269 6e67   the byte string
-0000b3d0: 2061 7420 7468 6973 2070 6f69 6e74 2c20   at this point, 
-0000b3e0: 7765 2061 7420 6c65 6173 740a 2020 2020  we at least.    
-0000b3f0: 2020 2020 2020 2020 2320 7661 6c69 6461          # valida
-0000b400: 7465 2074 6865 206c 656e 6774 6820 6f66  te the length of
-0000b410: 2074 6865 2073 7472 696e 6720 636f 6d70   the string comp
-0000b420: 6f6e 656e 7473 0a20 2020 2020 2020 2020  onents.         
-0000b430: 2020 2076 616c 6964 6174 655f 7661 6c75     validate_valu
-0000b440: 6528 2250 4e22 2c20 6f72 6967 696e 616c  e("PN", original
-0000b450: 5f73 7472 696e 6720 6966 206f 7269 6769  _string if origi
-0000b460: 6e61 6c5f 7374 7269 6e67 2065 6c73 6520  nal_string else 
-0000b470: 7661 6c2c 0a20 2020 2020 2020 2020 2020  val,.           
-0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b490: 7661 6c69 6461 7469 6f6e 5f6d 6f64 6529  validation_mode)
-0000b4a0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
-0000b4b0: 706f 6e65 6e74 7320 3d20 7661 6c2e 7370  ponents = val.sp
-0000b4c0: 6c69 7428 273d 2729 0a20 2020 2020 2020  lit('=').       
-0000b4d0: 2020 2020 2023 2052 656d 6f76 6520 656d       # Remove em
-0000b4e0: 7074 7920 656c 656d 656e 7473 2066 726f  pty elements fro
-0000b4f0: 6d20 7468 6520 656e 6420 746f 2061 766f  m the end to avo
-0000b500: 6964 2074 7261 696c 696e 6720 273d 270a  id trailing '='.
-0000b510: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-0000b520: 6520 6c65 6e28 636f 6d70 6f6e 656e 7473  e len(components
-0000b530: 2920 616e 6420 6e6f 7420 636f 6d70 6f6e  ) and not compon
-0000b540: 656e 7473 5b2d 315d 3a0a 2020 2020 2020  ents[-1]:.      
-0000b550: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
-0000b560: 656e 7473 2e70 6f70 2829 0a20 2020 2020  ents.pop().     
-0000b570: 2020 2020 2020 2073 656c 662e 5f63 6f6d         self._com
-0000b580: 706f 6e65 6e74 7320 3d20 7475 706c 6528  ponents = tuple(
-0000b590: 636f 6d70 6f6e 656e 7473 290a 0a20 2020  components)..   
-0000b5a0: 2020 2020 2020 2020 2023 2069 6620 7468           # if th
-0000b5b0: 6520 656e 636f 6469 6e67 2069 7320 6e6f  e encoding is no
-0000b5c0: 7420 6769 7665 6e2c 206c 6561 7665 2069  t given, leave i
-0000b5d0: 7420 6173 2075 6e64 6566 696e 6564 2028  t as undefined (
-0000b5e0: 4e6f 6e65 290a 2020 2020 2020 2020 7365  None).        se
-0000b5f0: 6c66 2e65 6e63 6f64 696e 6773 203d 205f  lf.encodings = _
-0000b600: 7665 7269 6679 5f65 6e63 6f64 696e 6773  verify_encodings
-0000b610: 2865 6e63 6f64 696e 6773 290a 0a20 2020  (encodings)..   
-0000b620: 2064 6566 205f 6372 6561 7465 5f64 6963   def _create_dic
-0000b630: 7428 7365 6c66 2920 2d3e 2044 6963 745b  t(self) -> Dict[
-0000b640: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
-0000b650: 2020 2022 2222 4372 6561 7465 7320 6120     """Creates a 
-0000b660: 6469 6374 696f 6e61 7279 206f 6620 7065  dictionary of pe
-0000b670: 7273 6f6e 206e 616d 6520 6772 6f75 7020  rson name group 
-0000b680: 616e 6420 636f 6d70 6f6e 656e 7420 6e61  and component na
-0000b690: 6d65 732e 0a0a 2020 2020 2020 2020 5573  mes...        Us
-0000b6a0: 6564 2065 7863 6c75 7369 7665 6c79 2066  ed exclusively f
-0000b6b0: 6f72 2060 666f 726d 6174 7465 6460 2066  or `formatted` f
-0000b6c0: 6f72 2062 6163 6b77 6172 6473 2063 6f6d  or backwards com
-0000b6d0: 7061 7469 6269 6c69 7479 2e0a 2020 2020  patibility..    
-0000b6e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000b6f0: 7061 7274 7320 3d20 5b0a 2020 2020 2020  parts = [.      
-0000b700: 2020 2020 2020 2766 616d 696c 795f 6e61        'family_na
-0000b710: 6d65 272c 2027 6769 7665 6e5f 6e61 6d65  me', 'given_name
-0000b720: 272c 2027 6d69 6464 6c65 5f6e 616d 6527  ', 'middle_name'
-0000b730: 2c20 276e 616d 655f 7072 6566 6978 272c  , 'name_prefix',
-0000b740: 0a20 2020 2020 2020 2020 2020 2027 6e61  .            'na
-0000b750: 6d65 5f73 7566 6669 7827 2c20 2769 6465  me_suffix', 'ide
-0000b760: 6f67 7261 7068 6963 272c 2027 7068 6f6e  ographic', 'phon
-0000b770: 6574 6963 270a 2020 2020 2020 2020 5d0a  etic'.        ].
-0000b780: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-0000b790: 633a 2067 6574 6174 7472 2873 656c 662c  c: getattr(self,
-0000b7a0: 2063 2c20 2727 2920 666f 7220 6320 696e   c, '') for c in
-0000b7b0: 2070 6172 7473 7d0a 0a20 2020 2040 7072   parts}..    @pr
-0000b7c0: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
-0000b7d0: 6f6d 706f 6e65 6e74 7328 7365 6c66 2920  omponents(self) 
-0000b7e0: 2d3e 2054 7570 6c65 5b73 7472 2c20 2e2e  -> Tuple[str, ..
-0000b7f0: 2e5d 3a0a 2020 2020 2020 2020 2222 2252  .]:.        """R
-0000b800: 6574 7572 6e73 2075 7020 746f 2074 6872  eturns up to thr
-0000b810: 6565 2064 6563 6f64 6564 2070 6572 736f  ee decoded perso
-0000b820: 6e20 6e61 6d65 2063 6f6d 706f 6e65 6e74  n name component
-0000b830: 7320 6173 2061 0a20 2020 2020 2020 203a  s as a.        :
-0000b840: 636c 6173 733a 6074 7570 6c65 6020 6f66  class:`tuple` of
-0000b850: 203a 636c 6173 733a 6073 7472 602e 0a0a   :class:`str`...
-0000b860: 2020 2020 2020 2020 2e2e 2076 6572 7369          .. versi
-0000b870: 6f6e 6164 6465 643a 3a20 312e 320a 0a20  onadded:: 1.2.. 
-0000b880: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-0000b890: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-0000b8a0: 2020 2020 2020 2054 7570 6c65 5b73 7472         Tuple[str
-0000b8b0: 2c20 2e2e 2e5d 0a20 2020 2020 2020 2020  , ...].         
-0000b8c0: 2020 2054 6865 2028 616c 7068 6162 6574     The (alphabet
-0000b8d0: 6963 2c20 6964 656f 6772 6170 6869 632c  ic, ideographic,
-0000b8e0: 2070 686f 6e65 7469 6329 2063 6f6d 706f   phonetic) compo
-0000b8f0: 6e65 6e74 7320 6f66 2074 6865 0a20 2020  nents of the.   
-0000b900: 2020 2020 2020 2020 2064 6563 6f64 6564           decoded
-0000b910: 2070 6572 736f 6e20 6e61 6d65 2e20 416e   person name. An
-0000b920: 7920 6f66 2074 6865 2063 6f6d 706f 6e65  y of the compone
-0000b930: 6e74 7320 6d61 7920 6265 2061 6273 656e  nts may be absen
-0000b940: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
-0000b950: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000b960: 636f 6d70 6f6e 656e 7473 2069 7320 4e6f  components is No
-0000b970: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b980: 6772 6f75 7073 203d 2073 656c 662e 6f72  groups = self.or
-0000b990: 6967 696e 616c 5f73 7472 696e 672e 7370  iginal_string.sp
-0000b9a0: 6c69 7428 6227 3d27 290a 2020 2020 2020  lit(b'=').      
-0000b9b0: 2020 2020 2020 656e 636f 6469 6e67 7320        encodings 
-0000b9c0: 3d20 7365 6c66 2e65 6e63 6f64 696e 6773  = self.encodings
-0000b9d0: 206f 7220 5b64 6566 6175 6c74 5f65 6e63   or [default_enc
-0000b9e0: 6f64 696e 675d 0a20 2020 2020 2020 2020  oding].         
-0000b9f0: 2020 2073 656c 662e 5f63 6f6d 706f 6e65     self._compone
-0000ba00: 6e74 7320 3d20 5f64 6563 6f64 655f 7065  nts = _decode_pe
-0000ba10: 7273 6f6e 6e61 6d65 2867 726f 7570 732c  rsonname(groups,
-0000ba20: 2065 6e63 6f64 696e 6773 290a 0a20 2020   encodings)..   
-0000ba30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000ba40: 2e5f 636f 6d70 6f6e 656e 7473 0a0a 2020  ._components..  
-0000ba50: 2020 6465 6620 5f6e 616d 655f 7061 7274    def _name_part
-0000ba60: 2873 656c 662c 2069 3a20 696e 7429 202d  (self, i: int) -
-0000ba70: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
-0000ba80: 2222 5265 7475 726e 2074 6865 2060 6960  ""Return the `i`
-0000ba90: 7468 2070 6172 7420 6f66 2074 6865 206e  th part of the n
-0000baa0: 616d 652e 2222 220a 2020 2020 2020 2020  ame.""".        
-0000bab0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000bac0: 2072 6574 7572 6e20 7365 6c66 2e63 6f6d   return self.com
-0000bad0: 706f 6e65 6e74 735b 305d 2e73 706c 6974  ponents[0].split
-0000bae0: 2827 5e27 295b 695d 0a20 2020 2020 2020  ('^')[i].       
-0000baf0: 2065 7863 6570 7420 496e 6465 7845 7272   except IndexErr
-0000bb00: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0000bb10: 7265 7475 726e 2027 270a 0a20 2020 2040  return ''..    @
-0000bb20: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000bb30: 2066 616d 696c 795f 6e61 6d65 2873 656c   family_name(sel
-0000bb40: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-0000bb50: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
-0000bb60: 2066 6972 7374 2028 6661 6d69 6c79 206e   first (family n
-0000bb70: 616d 6529 2067 726f 7570 206f 6620 7468  ame) group of th
-0000bb80: 6520 616c 7068 6162 6574 6963 2070 6572  e alphabetic per
-0000bb90: 736f 6e20 6e61 6d65 0a20 2020 2020 2020  son name.       
-0000bba0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-0000bbb0: 6173 2061 2075 6e69 636f 6465 2073 7472  as a unicode str
-0000bbc0: 696e 670a 0a20 2020 2020 2020 202e 2e20  ing..        .. 
-0000bbd0: 7665 7273 696f 6e61 6464 6564 3a3a 2031  versionadded:: 1
-0000bbe0: 2e32 0a20 2020 2020 2020 2022 2222 0a20  .2.        """. 
-0000bbf0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000bc00: 6c66 2e5f 6e61 6d65 5f70 6172 7428 3029  lf._name_part(0)
-0000bc10: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000bc20: 2020 2020 6465 6620 6769 7665 6e5f 6e61      def given_na
-0000bc30: 6d65 2873 656c 6629 202d 3e20 7374 723a  me(self) -> str:
-0000bc40: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000bc50: 726e 2074 6865 2073 6563 6f6e 6420 2867  rn the second (g
-0000bc60: 6976 656e 206e 616d 6529 2067 726f 7570  iven name) group
-0000bc70: 206f 6620 7468 6520 616c 7068 6162 6574   of the alphabet
-0000bc80: 6963 2070 6572 736f 6e20 6e61 6d65 0a20  ic person name. 
-0000bc90: 2020 2020 2020 2072 6570 7265 7365 6e74         represent
-0000bca0: 6174 696f 6e20 6173 2061 2075 6e69 636f  ation as a unico
-0000bcb0: 6465 2073 7472 696e 670a 0a20 2020 2020  de string..     
-0000bcc0: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
-0000bcd0: 6564 3a3a 2031 2e32 0a20 2020 2020 2020  ed:: 1.2.       
-0000bce0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000bcf0: 7572 6e20 7365 6c66 2e5f 6e61 6d65 5f70  urn self._name_p
-0000bd00: 6172 7428 3129 0a0a 2020 2020 4070 726f  art(1)..    @pro
-0000bd10: 7065 7274 790a 2020 2020 6465 6620 6d69  perty.    def mi
-0000bd20: 6464 6c65 5f6e 616d 6528 7365 6c66 2920  ddle_name(self) 
-0000bd30: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0000bd40: 2222 2252 6574 7572 6e20 7468 6520 7468  """Return the th
-0000bd50: 6972 6420 286d 6964 646c 6520 6e61 6d65  ird (middle name
-0000bd60: 2920 6772 6f75 7020 6f66 2074 6865 2061  ) group of the a
-0000bd70: 6c70 6861 6265 7469 6320 7065 7273 6f6e  lphabetic person
-0000bd80: 206e 616d 650a 2020 2020 2020 2020 7265   name.        re
-0000bd90: 7072 6573 656e 7461 7469 6f6e 2061 7320  presentation as 
-0000bda0: 6120 756e 6963 6f64 6520 7374 7269 6e67  a unicode string
-0000bdb0: 0a0a 2020 2020 2020 2020 2e2e 2076 6572  ..        .. ver
-0000bdc0: 7369 6f6e 6164 6465 643a 3a20 312e 320a  sionadded:: 1.2.
-0000bdd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000bde0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000bdf0: 5f6e 616d 655f 7061 7274 2832 290a 0a20  _name_part(2).. 
-0000be00: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000be10: 2064 6566 206e 616d 655f 7072 6566 6978   def name_prefix
-0000be20: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-0000be30: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-0000be40: 2074 6865 2066 6f75 7274 6820 286e 616d   the fourth (nam
-0000be50: 6520 7072 6566 6978 2920 6772 6f75 7020  e prefix) group 
-0000be60: 6f66 2074 6865 2061 6c70 6861 6265 7469  of the alphabeti
-0000be70: 6320 7065 7273 6f6e 206e 616d 650a 2020  c person name.  
-0000be80: 2020 2020 2020 7265 7072 6573 656e 7461        representa
-0000be90: 7469 6f6e 2061 7320 6120 756e 6963 6f64  tion as a unicod
-0000bea0: 6520 7374 7269 6e67 0a0a 2020 2020 2020  e string..      
-0000beb0: 2020 2e2e 2076 6572 7369 6f6e 6164 6465    .. versionadde
-0000bec0: 643a 3a20 312e 320a 2020 2020 2020 2020  d:: 1.2.        
-0000bed0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-0000bee0: 726e 2073 656c 662e 5f6e 616d 655f 7061  rn self._name_pa
-0000bef0: 7274 2833 290a 0a20 2020 2040 7072 6f70  rt(3)..    @prop
-0000bf00: 6572 7479 0a20 2020 2064 6566 206e 616d  erty.    def nam
-0000bf10: 655f 7375 6666 6978 2873 656c 6629 202d  e_suffix(self) -
-0000bf20: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
-0000bf30: 2222 5265 7475 726e 2074 6865 2066 6966  ""Return the fif
-0000bf40: 7468 2028 6e61 6d65 2073 7566 6669 7829  th (name suffix)
-0000bf50: 2067 726f 7570 206f 6620 7468 6520 616c   group of the al
-0000bf60: 7068 6162 6574 6963 2070 6572 736f 6e20  phabetic person 
-0000bf70: 6e61 6d65 0a20 2020 2020 2020 2072 6570  name.        rep
-0000bf80: 7265 7365 6e74 6174 696f 6e20 6173 2061  resentation as a
-0000bf90: 2075 6e69 636f 6465 2073 7472 696e 670a   unicode string.
-0000bfa0: 0a20 2020 2020 2020 202e 2e20 7665 7273  .        .. vers
-0000bfb0: 696f 6e61 6464 6564 3a3a 2031 2e32 0a20  ionadded:: 1.2. 
-0000bfc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000bfd0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000bfe0: 6e61 6d65 5f70 6172 7428 3429 0a0a 2020  name_part(4)..  
-0000bff0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000c000: 6465 6620 6964 656f 6772 6170 6869 6328  def ideographic(
-0000c010: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
-0000c020: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-0000c030: 7468 6520 7365 636f 6e64 2028 6964 656f  the second (ideo
-0000c040: 6772 6170 6869 6329 2070 6572 736f 6e20  graphic) person 
-0000c050: 6e61 6d65 2063 6f6d 706f 6e65 6e74 2061  name component a
-0000c060: 7320 610a 2020 2020 2020 2020 756e 6963  s a.        unic
-0000c070: 6f64 6520 7374 7269 6e67 0a0a 2020 2020  ode string..    
-0000c080: 2020 2020 2e2e 2076 6572 7369 6f6e 6164      .. versionad
-0000c090: 6465 643a 3a20 312e 320a 2020 2020 2020  ded:: 1.2.      
-0000c0a0: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-0000c0b0: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
-0000c0c0: 6574 7572 6e20 7365 6c66 2e63 6f6d 706f  eturn self.compo
-0000c0d0: 6e65 6e74 735b 315d 0a20 2020 2020 2020  nents[1].       
-0000c0e0: 2065 7863 6570 7420 496e 6465 7845 7272   except IndexErr
-0000c0f0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0000c100: 7265 7475 726e 2027 270a 0a20 2020 2040  return ''..    @
-0000c110: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000c120: 2070 686f 6e65 7469 6328 7365 6c66 2920   phonetic(self) 
-0000c130: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0000c140: 2222 2252 6574 7572 6e20 7468 6520 7468  """Return the th
-0000c150: 6972 6420 2870 686f 6e65 7469 6329 2070  ird (phonetic) p
-0000c160: 6572 736f 6e20 6e61 6d65 2063 6f6d 706f  erson name compo
-0000c170: 6e65 6e74 2061 7320 610a 2020 2020 2020  nent as a.      
-0000c180: 2020 756e 6963 6f64 6520 7374 7269 6e67    unicode string
-0000c190: 0a0a 2020 2020 2020 2020 2e2e 2076 6572  ..        .. ver
-0000c1a0: 7369 6f6e 6164 6465 643a 3a20 312e 320a  sionadded:: 1.2.
-0000c1b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c1c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000c1d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c1e0: 2e63 6f6d 706f 6e65 6e74 735b 325d 0a20  .components[2]. 
-0000c1f0: 2020 2020 2020 2065 7863 6570 7420 496e         except In
-0000c200: 6465 7845 7272 6f72 3a0a 2020 2020 2020  dexError:.      
-0000c210: 2020 2020 2020 7265 7475 726e 2027 270a        return ''.
-0000c220: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
-0000c230: 7365 6c66 2c20 6f74 6865 723a 2041 6e79  self, other: Any
-0000c240: 2920 2d3e 2041 6e79 3a0a 2020 2020 2020  ) -> Any:.      
-0000c250: 2020 2222 2252 6574 7572 6e20 6060 5472    """Return ``Tr
-0000c260: 7565 6060 2069 6620 606f 7468 6572 6020  ue`` if `other` 
-0000c270: 6571 7561 6c73 2074 6865 2063 7572 7265  equals the curre
-0000c280: 6e74 206e 616d 652e 2222 220a 2020 2020  nt name.""".    
-0000c290: 2020 2020 7265 7475 726e 2073 7472 2873      return str(s
-0000c2a0: 656c 6629 203d 3d20 6f74 6865 720a 0a20  elf) == other.. 
-0000c2b0: 2020 2064 6566 205f 5f6e 655f 5f28 7365     def __ne__(se
-0000c2c0: 6c66 2c20 6f74 6865 723a 2041 6e79 2920  lf, other: Any) 
-0000c2d0: 2d3e 2041 6e79 3a0a 2020 2020 2020 2020  -> Any:.        
-0000c2e0: 2222 2252 6574 7572 6e20 6060 5472 7565  """Return ``True
-0000c2f0: 6060 2069 6620 606f 7468 6572 6020 646f  `` if `other` do
-0000c300: 6573 6e27 7420 6571 7561 6c20 7468 6520  esn't equal the 
-0000c310: 6375 7272 656e 7420 6e61 6d65 2e22 2222  current name."""
-0000c320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c330: 6e6f 7420 7365 6c66 203d 3d20 6f74 6865  not self == othe
-0000c340: 720a 0a20 2020 2064 6566 205f 5f73 7472  r..    def __str
-0000c350: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
-0000c360: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000c370: 726e 2061 2073 7472 696e 6720 7265 7072  rn a string repr
-0000c380: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-0000c390: 6520 6e61 6d65 2e22 2222 0a20 2020 2020  e name.""".     
-0000c3a0: 2020 2072 6574 7572 6e20 273d 272e 6a6f     return '='.jo
-0000c3b0: 696e 2873 656c 662e 636f 6d70 6f6e 656e  in(self.componen
-0000c3c0: 7473 292e 5f5f 7374 725f 5f28 290a 0a20  ts).__str__().. 
-0000c3d0: 2020 2064 6566 205f 5f69 7465 725f 5f28     def __iter__(
-0000c3e0: 7365 6c66 2920 2d3e 2049 7465 7261 746f  self) -> Iterato
-0000c3f0: 725b 7374 725d 3a0a 2020 2020 2020 2020  r[str]:.        
-0000c400: 2222 2249 7465 7261 7465 2074 6872 6f75  """Iterate throu
-0000c410: 6768 2074 6865 206e 616d 652e 2222 220a  gh the name.""".
-0000c420: 2020 2020 2020 2020 7969 656c 6420 6672          yield fr
-0000c430: 6f6d 2073 656c 662e 5f5f 7374 725f 5f28  om self.__str__(
-0000c440: 290a 0a20 2020 2064 6566 205f 5f6c 656e  )..    def __len
-0000c450: 5f5f 2873 656c 6629 202d 3e20 696e 743a  __(self) -> int:
-0000c460: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000c470: 726e 2074 6865 206c 656e 6774 6820 6f66  rn the length of
-0000c480: 2074 6865 2070 6572 736f 6e20 6e61 6d65   the person name
-0000c490: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
-0000c4a0: 7572 6e20 6c65 6e28 7365 6c66 2e5f 5f73  urn len(self.__s
-0000c4b0: 7472 5f5f 2829 290a 0a20 2020 2064 6566  tr__())..    def
-0000c4c0: 205f 5f63 6f6e 7461 696e 735f 5f28 7365   __contains__(se
-0000c4d0: 6c66 2c20 783a 2041 6e79 2920 2d3e 2062  lf, x: Any) -> b
-0000c4e0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-0000c4f0: 5265 7475 726e 2060 6054 7275 6560 6020  Return ``True`` 
-0000c500: 6966 2060 7860 2069 7320 696e 2074 6865  if `x` is in the
-0000c510: 206e 616d 652e 2222 220a 2020 2020 2020   name.""".      
-0000c520: 2020 7265 7475 726e 2078 2069 6e20 7365    return x in se
-0000c530: 6c66 2e5f 5f73 7472 5f5f 2829 0a0a 2020  lf.__str__()..  
-0000c540: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-0000c550: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-0000c560: 2020 2020 2022 2222 5265 7475 726e 2061       """Return a
-0000c570: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-0000c580: 6f66 2074 6865 206e 616d 652e 2222 220a  of the name.""".
-0000c590: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-0000c5a0: 3d27 2e6a 6f69 6e28 7365 6c66 2e63 6f6d  ='.join(self.com
-0000c5b0: 706f 6e65 6e74 7329 2e5f 5f72 6570 725f  ponents).__repr_
-0000c5c0: 5f28 290a 0a20 2020 2064 6566 205f 5f68  _()..    def __h
-0000c5d0: 6173 685f 5f28 7365 6c66 2920 2d3e 2069  ash__(self) -> i
-0000c5e0: 6e74 3a0a 2020 2020 2020 2020 2222 2252  nt:.        """R
-0000c5f0: 6574 7572 6e20 6120 6861 7368 206f 6620  eturn a hash of 
-0000c600: 7468 6520 6e61 6d65 2e22 2222 0a20 2020  the name.""".   
-0000c610: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
-0000c620: 2873 656c 662e 636f 6d70 6f6e 656e 7473  (self.components
-0000c630: 290a 0a20 2020 2064 6566 2064 6563 6f64  )..    def decod
-0000c640: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
-0000c650: 2065 6e63 6f64 696e 6773 3a20 4f70 7469   encodings: Opti
-0000c660: 6f6e 616c 5b53 6571 7565 6e63 655b 7374  onal[Sequence[st
-0000c670: 725d 5d20 3d20 4e6f 6e65 0a20 2020 2029  r]] = None.    )
-0000c680: 202d 3e20 2250 6572 736f 6e4e 616d 6522   -> "PersonName"
-0000c690: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-0000c6a0: 7572 6e20 7468 6520 7061 7469 656e 7420  urn the patient 
-0000c6b0: 6e61 6d65 2064 6563 6f64 6564 2062 7920  name decoded by 
-0000c6c0: 7468 6520 6769 7665 6e20 6065 6e63 6f64  the given `encod
-0000c6d0: 696e 6773 602e 0a0a 2020 2020 2020 2020  ings`...        
-0000c6e0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000c6f0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000c700: 2020 2020 2020 656e 636f 6469 6e67 7320        encodings 
-0000c710: 3a20 6c69 7374 206f 6620 7374 722c 206f  : list of str, o
-0000c720: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000c730: 2020 2020 5468 6520 6c69 7374 206f 6620      The list of 
-0000c740: 656e 636f 6469 6e67 7320 7573 6564 2066  encodings used f
-0000c750: 6f72 2064 6563 6f64 696e 6720 7468 6520  or decoding the 
-0000c760: 6279 7465 2073 7472 696e 672e 2049 6620  byte string. If 
-0000c770: 6e6f 740a 2020 2020 2020 2020 2020 2020  not.            
-0000c780: 6769 7665 6e2c 2074 6865 2069 6e69 7469  given, the initi
-0000c790: 616c 2065 6e63 6f64 696e 6773 2073 6574  al encodings set
-0000c7a0: 2069 6e20 7468 6520 6f62 6a65 6374 2061   in the object a
-0000c7b0: 7265 2075 7365 642e 0a0a 2020 2020 2020  re used...      
-0000c7c0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0000c7d0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0000c7e0: 2020 7661 6c75 6572 6570 2e50 6572 736f    valuerep.Perso
-0000c7f0: 6e4e 616d 650a 2020 2020 2020 2020 2020  nName.          
-0000c800: 2020 4120 7065 7273 6f6e 206e 616d 6520    A person name 
-0000c810: 6f62 6a65 6374 2074 6861 7420 7769 6c6c  object that will
-0000c820: 2072 6574 7572 6e20 7468 6520 6465 636f   return the deco
-0000c830: 6465 6420 7374 7269 6e67 2077 6974 680a  ded string with.
-0000c840: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-0000c850: 6769 7665 6e20 656e 636f 6469 6e67 7320  given encodings 
-0000c860: 6f6e 2064 656d 616e 642e 2049 6620 7468  on demand. If th
-0000c870: 6520 656e 636f 6469 6e67 7320 6172 6520  e encodings are 
-0000c880: 6e6f 7420 6769 7665 6e2c 0a20 2020 2020  not given,.     
-0000c890: 2020 2020 2020 2074 6865 2063 7572 7265         the curre
-0000c8a0: 6e74 206f 626a 6563 7420 6973 2072 6574  nt object is ret
-0000c8b0: 7572 6e65 642e 0a20 2020 2020 2020 2022  urned..        "
-0000c8c0: 2222 0a20 2020 2020 2020 2023 2069 6e20  "".        # in 
-0000c8d0: 7468 6520 636f 6d6d 6f6e 2063 6173 6520  the common case 
-0000c8e0: 2865 6e63 6f64 696e 6720 6469 6420 6e6f  (encoding did no
-0000c8f0: 7420 6368 616e 6765 2920 7765 2064 6563  t change) we dec
-0000c900: 6f64 6520 6f6e 2064 656d 616e 640a 2020  ode on demand.  
-0000c910: 2020 2020 2020 6966 2065 6e63 6f64 696e        if encodin
-0000c920: 6773 2069 7320 4e6f 6e65 206f 7220 656e  gs is None or en
-0000c930: 636f 6469 6e67 7320 3d3d 2073 656c 662e  codings == self.
-0000c940: 656e 636f 6469 6e67 733a 0a20 2020 2020  encodings:.     
-0000c950: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000c960: 6c66 0a0a 2020 2020 2020 2020 2320 7468  lf..        # th
-0000c970: 6520 656e 636f 6469 6e67 2077 6173 2075  e encoding was u
-0000c980: 6e6b 6e6f 776e 206f 7220 696e 636f 7272  nknown or incorr
-0000c990: 6563 7420 2d20 6372 6561 7465 2061 206e  ect - create a n
-0000c9a0: 6577 0a20 2020 2020 2020 2023 2050 6572  ew.        # Per
-0000c9b0: 736f 6e4e 616d 6520 6f62 6a65 6374 2077  sonName object w
-0000c9c0: 6974 6820 7468 6520 6368 616e 6765 6420  ith the changed 
-0000c9d0: 656e 636f 6469 6e67 0a20 2020 2020 2020  encoding.       
-0000c9e0: 2065 6e63 6f64 696e 6773 203d 205f 7665   encodings = _ve
-0000c9f0: 7269 6679 5f65 6e63 6f64 696e 6773 2865  rify_encodings(e
-0000ca00: 6e63 6f64 696e 6773 290a 2020 2020 2020  ncodings).      
-0000ca10: 2020 6966 2073 656c 662e 6f72 6967 696e    if self.origin
-0000ca20: 616c 5f73 7472 696e 6720 6973 204e 6f6e  al_string is Non
-0000ca30: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000ca40: 2069 6620 7468 6520 6f72 6967 696e 616c   if the original
-0000ca50: 2065 6e63 6f64 696e 6720 7761 7320 6e6f   encoding was no
-0000ca60: 7420 7365 742c 2077 6520 7365 7420 6974  t set, we set it
-0000ca70: 206e 6f77 0a20 2020 2020 2020 2020 2020   now.           
-0000ca80: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
-0000ca90: 7472 696e 6720 3d20 5f65 6e63 6f64 655f  tring = _encode_
-0000caa0: 7065 7273 6f6e 6e61 6d65 280a 2020 2020  personname(.    
-0000cab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cac0: 2e63 6f6d 706f 6e65 6e74 732c 2073 656c  .components, sel
-0000cad0: 662e 656e 636f 6469 6e67 7320 6f72 205b  f.encodings or [
-0000cae0: 6465 6661 756c 745f 656e 636f 6469 6e67  default_encoding
-0000caf0: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-0000cb00: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
-0000cb10: 7720 7468 6174 2077 6520 6861 7665 2074  w that we have t
-0000cb20: 6865 2062 7974 6520 6c65 6e67 7468 2c20  he byte length, 
-0000cb30: 7765 2072 652d 7661 6c69 6461 7465 2074  we re-validate t
-0000cb40: 6865 2076 616c 7565 0a20 2020 2020 2020  he value.       
-0000cb50: 2020 2020 2076 616c 6964 6174 655f 7661       validate_va
-0000cb60: 6c75 6528 2250 4e22 2c20 7365 6c66 2e6f  lue("PN", self.o
-0000cb70: 7269 6769 6e61 6c5f 7374 7269 6e67 2c20  riginal_string, 
-0000cb80: 7365 6c66 2e76 616c 6964 6174 696f 6e5f  self.validation_
-0000cb90: 6d6f 6465 290a 0a20 2020 2020 2020 2072  mode)..        r
-0000cba0: 6574 7572 6e20 5065 7273 6f6e 4e61 6d65  eturn PersonName
-0000cbb0: 2873 656c 662e 6f72 6967 696e 616c 5f73  (self.original_s
-0000cbc0: 7472 696e 672c 2065 6e63 6f64 696e 6773  tring, encodings
-0000cbd0: 290a 0a20 2020 2064 6566 2065 6e63 6f64  )..    def encod
-0000cbe0: 6528 7365 6c66 2c20 656e 636f 6469 6e67  e(self, encoding
-0000cbf0: 733a 204f 7074 696f 6e61 6c5b 5365 7175  s: Optional[Sequ
-0000cc00: 656e 6365 5b73 7472 5d5d 203d 204e 6f6e  ence[str]] = Non
-0000cc10: 6529 202d 3e20 6279 7465 733a 0a20 2020  e) -> bytes:.   
-0000cc20: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-0000cc30: 6865 2070 6174 6965 6e74 206e 616d 6520  he patient name 
-0000cc40: 6465 636f 6465 6420 6279 2074 6865 2067  decoded by the g
-0000cc50: 6976 656e 2060 656e 636f 6469 6e67 7360  iven `encodings`
-0000cc60: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0000cc70: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0000cc80: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000cc90: 2065 6e63 6f64 696e 6773 203a 206c 6973   encodings : lis
-0000cca0: 7420 6f66 2073 7472 2c20 6f70 7469 6f6e  t of str, option
-0000ccb0: 616c 0a20 2020 2020 2020 2020 2020 2054  al.            T
-0000ccc0: 6865 206c 6973 7420 6f66 2065 6e63 6f64  he list of encod
-0000ccd0: 696e 6773 2075 7365 6420 666f 7220 656e  ings used for en
-0000cce0: 636f 6469 6e67 2074 6865 2075 6e69 636f  coding the unico
-0000ccf0: 6465 2073 7472 696e 672e 2049 660a 2020  de string. If.  
-0000cd00: 2020 2020 2020 2020 2020 6e6f 7420 6769            not gi
-0000cd10: 7665 6e2c 2074 6865 2069 6e69 7469 616c  ven, the initial
-0000cd20: 2065 6e63 6f64 696e 6773 2073 6574 2069   encodings set i
-0000cd30: 6e20 7468 6520 6f62 6a65 6374 2061 7265  n the object are
-0000cd40: 2075 7365 642e 0a0a 2020 2020 2020 2020   used...        
-0000cd50: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-0000cd60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000cd70: 6279 7465 730a 2020 2020 2020 2020 2020  bytes.          
-0000cd80: 2020 5468 6520 7065 7273 6f6e 206e 616d    The person nam
-0000cd90: 6520 656e 636f 6465 6420 7769 7468 2074  e encoded with t
-0000cda0: 6865 2067 6976 656e 2065 6e63 6f64 696e  he given encodin
-0000cdb0: 6773 2061 7320 6120 6279 7465 2073 7472  gs as a byte str
-0000cdc0: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-0000cdd0: 2049 6620 6e6f 2065 6e63 6f64 696e 6720   If no encoding 
-0000cde0: 6973 2067 6976 656e 2c20 7468 6520 6f72  is given, the or
-0000cdf0: 6967 696e 616c 2062 7974 6520 7374 7269  iginal byte stri
-0000ce00: 6e67 2069 7320 7265 7475 726e 6564 2c20  ng is returned, 
-0000ce10: 6966 0a20 2020 2020 2020 2020 2020 2061  if.            a
-0000ce20: 7661 696c 6162 6c65 2c20 6f74 6865 7277  vailable, otherw
-0000ce30: 6973 6520 6561 6368 2067 726f 7570 206f  ise each group o
-0000ce40: 6620 7468 6520 7061 7469 656e 7420 6e61  f the patient na
-0000ce50: 6d65 2069 7320 656e 636f 6465 640a 2020  me is encoded.  
-0000ce60: 2020 2020 2020 2020 2020 7769 7468 2074            with t
-0000ce70: 6865 2066 6972 7374 206d 6174 6368 696e  he first matchin
-0000ce80: 6720 6f66 2074 6865 2067 6976 656e 2065  g of the given e
-0000ce90: 6e63 6f64 696e 6773 2e0a 2020 2020 2020  ncodings..      
-0000cea0: 2020 2222 220a 2020 2020 2020 2020 656e    """.        en
-0000ceb0: 636f 6469 6e67 7320 3d20 5f76 6572 6966  codings = _verif
-0000cec0: 795f 656e 636f 6469 6e67 7328 656e 636f  y_encodings(enco
-0000ced0: 6469 6e67 7329 206f 7220 7365 6c66 2e65  dings) or self.e
-0000cee0: 6e63 6f64 696e 6773 0a0a 2020 2020 2020  ncodings..      
-0000cef0: 2020 2320 6966 2074 6865 2065 6e63 6f64    # if the encod
-0000cf00: 696e 6720 6973 206e 6f74 2074 6865 206f  ing is not the o
-0000cf10: 7269 6769 6e61 6c20 656e 636f 6469 6e67  riginal encoding
-0000cf20: 2c20 7765 2068 6176 6520 746f 2072 6574  , we have to ret
-0000cf30: 7572 6e0a 2020 2020 2020 2020 2320 6120  urn.        # a 
-0000cf40: 7265 2d65 6e63 6f64 6564 2073 7472 696e  re-encoded strin
-0000cf50: 6720 2877 6974 686f 7574 2075 7064 6174  g (without updat
-0000cf60: 696e 6720 7468 6520 6f72 6967 696e 616c  ing the original
-0000cf70: 2073 7472 696e 6729 0a20 2020 2020 2020   string).       
-0000cf80: 2069 6620 656e 636f 6469 6e67 7320 213d   if encodings !=
-0000cf90: 2073 656c 662e 656e 636f 6469 6e67 7320   self.encodings 
-0000cfa0: 616e 6420 7365 6c66 2e65 6e63 6f64 696e  and self.encodin
-0000cfb0: 6773 2069 7320 6e6f 7420 4e6f 6e65 3a0a  gs is not None:.
-0000cfc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000cfd0: 726e 205f 656e 636f 6465 5f70 6572 736f  rn _encode_perso
-0000cfe0: 6e6e 616d 6528 0a20 2020 2020 2020 2020  nname(.         
-0000cff0: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
-0000d000: 6f6e 656e 7473 2c20 6361 7374 2853 6571  onents, cast(Seq
-0000d010: 7565 6e63 655b 7374 725d 2c20 656e 636f  uence[str], enco
-0000d020: 6469 6e67 7329 0a20 2020 2020 2020 2020  dings).         
-0000d030: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-0000d040: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
-0000d050: 7472 696e 6720 6973 204e 6f6e 653a 0a20  tring is None:. 
-0000d060: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-0000d070: 7468 6520 6f72 6967 696e 616c 2065 6e63  the original enc
-0000d080: 6f64 696e 6720 7761 7320 6e6f 7420 7365  oding was not se
-0000d090: 742c 2077 6520 7365 7420 6974 206e 6f77  t, we set it now
-0000d0a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d0b0: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
-0000d0c0: 6720 3d20 5f65 6e63 6f64 655f 7065 7273  g = _encode_pers
-0000d0d0: 6f6e 6e61 6d65 280a 2020 2020 2020 2020  onname(.        
-0000d0e0: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-0000d0f0: 706f 6e65 6e74 732c 2065 6e63 6f64 696e  ponents, encodin
-0000d100: 6773 206f 7220 5b64 6566 6175 6c74 5f65  gs or [default_e
-0000d110: 6e63 6f64 696e 675d 0a20 2020 2020 2020  ncoding].       
-0000d120: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000d130: 7265 7475 726e 2073 656c 662e 6f72 6967  return self.orig
-0000d140: 696e 616c 5f73 7472 696e 670a 0a20 2020  inal_string..   
-0000d150: 2064 6566 2066 616d 696c 795f 636f 6d6d   def family_comm
-0000d160: 615f 6769 7665 6e28 7365 6c66 2920 2d3e  a_given(self) ->
-0000d170: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-0000d180: 2252 6574 7572 6e20 7468 6520 6e61 6d65  "Return the name
-0000d190: 2061 7320 2246 616d 696c 792c 2047 6976   as "Family, Giv
-0000d1a0: 656e 222e 2222 220a 2020 2020 2020 2020  en".""".        
-0000d1b0: 7265 7475 726e 2066 227b 7365 6c66 2e66  return f"{self.f
-0000d1c0: 616d 696c 795f 6e61 6d65 7d2c 207b 7365  amily_name}, {se
-0000d1d0: 6c66 2e67 6976 656e 5f6e 616d 657d 220a  lf.given_name}".
-0000d1e0: 0a20 2020 2064 6566 2066 6f72 6d61 7474  .    def formatt
-0000d1f0: 6564 2873 656c 662c 2066 6f72 6d61 745f  ed(self, format_
-0000d200: 7374 723a 2073 7472 2920 2d3e 2073 7472  str: str) -> str
-0000d210: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-0000d220: 7572 6e20 7468 6520 6e61 6d65 2061 7320  urn the name as 
-0000d230: 6120 3a63 6c61 7373 3a60 7374 7260 2066  a :class:`str` f
-0000d240: 6f72 6d61 7474 6564 2075 7369 6e67 2060  ormatted using `
-0000d250: 666f 726d 6174 5f73 7472 602e 2222 220a  format_str`.""".
-0000d260: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-0000d270: 6f72 6d61 745f 7374 7220 2520 7365 6c66  ormat_str % self
-0000d280: 2e5f 6372 6561 7465 5f64 6963 7428 290a  ._create_dict().
-0000d290: 0a20 2020 2064 6566 205f 5f62 6f6f 6c5f  .    def __bool_
-0000d2a0: 5f28 7365 6c66 2920 2d3e 2062 6f6f 6c3a  _(self) -> bool:
-0000d2b0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000d2c0: 726e 2060 6054 7275 6560 6020 6966 2074  rn ``True`` if t
-0000d2d0: 6865 206e 616d 6520 6973 206e 6f74 2065  he name is not e
-0000d2e0: 6d70 7479 2e22 2222 0a20 2020 2020 2020  mpty.""".       
-0000d2f0: 2069 6620 6e6f 7420 7365 6c66 2e6f 7269   if not self.ori
-0000d300: 6769 6e61 6c5f 7374 7269 6e67 3a0a 2020  ginal_string:.  
-0000d310: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d320: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0000d330: 2020 2062 6f6f 6c28 7365 6c66 2e63 6f6d     bool(self.com
-0000d340: 706f 6e65 6e74 7329 0a20 2020 2020 2020  ponents).       
-0000d350: 2020 2020 2020 2020 2061 6e64 2028 6c65           and (le
-0000d360: 6e28 7365 6c66 2e63 6f6d 706f 6e65 6e74  n(self.component
-0000d370: 7329 203e 2031 206f 7220 626f 6f6c 2873  s) > 1 or bool(s
-0000d380: 656c 662e 636f 6d70 6f6e 656e 7473 5b30  elf.components[0
-0000d390: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-0000d3a0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0000d3b0: 6e20 626f 6f6c 2873 656c 662e 6f72 6967  n bool(self.orig
-0000d3c0: 696e 616c 5f73 7472 696e 6729 0a0a 2020  inal_string)..  
-0000d3d0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-0000d3e0: 2020 2020 6465 6620 5f65 6e63 6f64 655f      def _encode_
-0000d3f0: 636f 6d70 6f6e 656e 745f 6772 6f75 7073  component_groups
-0000d400: 280a 2020 2020 2020 2020 616c 7068 6162  (.        alphab
-0000d410: 6574 6963 5f67 726f 7570 3a20 5365 7175  etic_group: Sequ
-0000d420: 656e 6365 5b55 6e69 6f6e 5b73 7472 2c20  ence[Union[str, 
-0000d430: 6279 7465 735d 5d2c 0a20 2020 2020 2020  bytes]],.       
-0000d440: 2069 6465 6f67 7261 7068 6963 5f67 726f   ideographic_gro
-0000d450: 7570 3a20 5365 7175 656e 6365 5b55 6e69  up: Sequence[Uni
-0000d460: 6f6e 5b73 7472 2c20 6279 7465 735d 5d2c  on[str, bytes]],
-0000d470: 0a20 2020 2020 2020 2070 686f 6e65 7469  .        phoneti
-0000d480: 635f 6772 6f75 703a 2053 6571 7565 6e63  c_group: Sequenc
-0000d490: 655b 556e 696f 6e5b 7374 722c 2062 7974  e[Union[str, byt
-0000d4a0: 6573 5d5d 2c0a 2020 2020 2020 2020 656e  es]],.        en
-0000d4b0: 636f 6469 6e67 733a 204f 7074 696f 6e61  codings: Optiona
-0000d4c0: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
-0000d4d0: 6f6e 652c 0a20 2020 2029 202d 3e20 6279  one,.    ) -> by
-0000d4e0: 7465 733a 0a20 2020 2020 2020 2022 2222  tes:.        """
-0000d4f0: 4372 6561 7465 7320 6120 6279 7465 2073  Creates a byte s
-0000d500: 7472 696e 6720 666f 7220 6120 7065 7273  tring for a pers
-0000d510: 6f6e 206e 616d 6520 6672 6f6d 206c 6973  on name from lis
-0000d520: 7473 206f 6620 7061 7274 732e 0a0a 2020  ts of parts...  
-0000d530: 2020 2020 2020 4561 6368 206f 6620 7468        Each of th
-0000d540: 6520 7468 7265 6520 636f 6d70 6f6e 656e  e three componen
-0000d550: 7420 6772 6f75 7073 2028 616c 7068 6162  t groups (alphab
-0000d560: 6574 6963 2c20 6964 656f 6772 6170 6869  etic, ideographi
-0000d570: 632c 2070 686f 6e65 7469 6329 0a20 2020  c, phonetic).   
-0000d580: 2020 2020 2061 7265 2073 7570 706c 6965       are supplie
-0000d590: 6420 6173 2061 206c 6973 7420 6f66 2063  d as a list of c
-0000d5a0: 6f6d 706f 6e65 6e74 732e 0a0a 2020 2020  omponents...    
-0000d5b0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000d5c0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000d5d0: 2d0a 2020 2020 2020 2020 616c 7068 6162  -.        alphab
-0000d5e0: 6574 6963 5f67 726f 7570 3a20 5365 7175  etic_group: Sequ
-0000d5f0: 656e 6365 5b55 6e69 6f6e 5b73 7472 2c20  ence[Union[str, 
-0000d600: 6279 7465 735d 5d0a 2020 2020 2020 2020  bytes]].        
-0000d610: 2020 2020 4c69 7374 206f 6620 636f 6d70      List of comp
-0000d620: 6f6e 656e 7473 2066 6f72 2074 6865 2061  onents for the a
-0000d630: 6c70 6861 6265 7469 6320 6772 6f75 702e  lphabetic group.
-0000d640: 0a20 2020 2020 2020 2069 6465 6f67 7261  .        ideogra
-0000d650: 7068 6963 5f67 726f 7570 3a20 5365 7175  phic_group: Sequ
-0000d660: 656e 6365 5b55 6e69 6f6e 5b73 7472 2c20  ence[Union[str, 
-0000d670: 6279 7465 735d 5d0a 2020 2020 2020 2020  bytes]].        
-0000d680: 2020 2020 4c69 7374 206f 6620 636f 6d70      List of comp
-0000d690: 6f6e 656e 7473 2066 6f72 2074 6865 2069  onents for the i
-0000d6a0: 6465 6f67 7261 7068 6963 2067 726f 7570  deographic group
-0000d6b0: 2e0a 2020 2020 2020 2020 7068 6f6e 6574  ..        phonet
-0000d6c0: 6963 5f67 726f 7570 3a20 5365 7175 656e  ic_group: Sequen
-0000d6d0: 6365 5b55 6e69 6f6e 5b73 7472 2c20 6279  ce[Union[str, by
-0000d6e0: 7465 735d 5d0a 2020 2020 2020 2020 2020  tes]].          
-0000d6f0: 2020 4c69 7374 206f 6620 636f 6d70 6f6e    List of compon
-0000d700: 656e 7473 2066 6f72 2074 6865 2070 686f  ents for the pho
-0000d710: 6e65 7469 6320 6772 6f75 702e 0a20 2020  netic group..   
-0000d720: 2020 2020 2065 6e63 6f64 696e 6773 3a20       encodings: 
-0000d730: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-0000d740: 725d 5d0a 2020 2020 2020 2020 2020 2020  r]].            
-0000d750: 4120 6c69 7374 206f 6620 656e 636f 6469  A list of encodi
-0000d760: 6e67 7320 7573 6564 2066 6f72 2074 6865  ngs used for the
-0000d770: 206f 7468 6572 2069 6e70 7574 2070 6172   other input par
-0000d780: 616d 6574 6572 732e 0a0a 2020 2020 2020  ameters...      
-0000d790: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0000d7a0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0000d7b0: 2020 6279 7465 733a 0a20 2020 2020 2020    bytes:.       
-0000d7c0: 2020 2020 2042 7974 6573 2073 7472 696e       Bytes strin
-0000d7d0: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
-0000d7e0: 206f 6620 7468 6520 7065 7273 6f6e 206e   of the person n
-0000d7f0: 616d 652e 0a0a 2020 2020 2020 2020 5261  ame...        Ra
-0000d800: 6973 6573 0a20 2020 2020 2020 202d 2d2d  ises.        ---
-0000d810: 2d2d 2d0a 2020 2020 2020 2020 5661 6c75  ---.        Valu
-0000d820: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-0000d830: 2020 2020 4966 2061 6e79 206f 6620 7468      If any of th
-0000d840: 6520 696e 7075 7420 7374 7269 6e67 7320  e input strings 
-0000d850: 636f 6e74 6169 6e20 6469 7361 6c6c 6f77  contain disallow
-0000d860: 6564 2063 6861 7261 6374 6572 733a 0a20  ed characters:. 
-0000d870: 2020 2020 2020 2020 2020 2027 5c5c 2720             '\\' 
-0000d880: 2873 696e 676c 6520 6261 636b 736c 6173  (single backslas
-0000d890: 6829 2c20 275e 272c 2027 3d27 2e0a 2020  h), '^', '='..  
-0000d8a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d8b0: 2020 6672 6f6d 2070 7964 6963 6f6d 2e63    from pydicom.c
-0000d8c0: 6861 7273 6574 2069 6d70 6f72 7420 656e  harset import en
-0000d8d0: 636f 6465 5f73 7472 696e 672c 2064 6563  code_string, dec
-0000d8e0: 6f64 655f 6279 7465 730a 0a20 2020 2020  ode_bytes..     
-0000d8f0: 2020 2064 6566 2065 6e63 2873 3a20 7374     def enc(s: st
-0000d900: 7229 202d 3e20 6279 7465 733a 0a20 2020  r) -> bytes:.   
-0000d910: 2020 2020 2020 2020 2062 203d 2065 6e63           b = enc
-0000d920: 6f64 655f 7374 7269 6e67 2873 2c20 656e  ode_string(s, en
-0000d930: 636f 6469 6e67 7320 6f72 205b 6465 6661  codings or [defa
-0000d940: 756c 745f 656e 636f 6469 6e67 5d29 0a20  ult_encoding]). 
-0000d950: 2020 2020 2020 2020 2020 2076 616c 6964             valid
-0000d960: 6174 655f 7661 6c75 6528 2250 4e22 2c20  ate_value("PN", 
-0000d970: 622c 2063 6f6e 6669 672e 7365 7474 696e  b, config.settin
-0000d980: 6773 2e77 7269 7469 6e67 5f76 616c 6964  gs.writing_valid
-0000d990: 6174 696f 6e5f 6d6f 6465 2c0a 2020 2020  ation_mode,.    
-0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9b0: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
-0000d9c0: 706e 5f63 6f6d 706f 6e65 6e74 5f6c 656e  pn_component_len
-0000d9d0: 6774 6829 0a20 2020 2020 2020 2020 2020  gth).           
-0000d9e0: 2072 6574 7572 6e20 620a 0a20 2020 2020   return b..     
-0000d9f0: 2020 2064 6566 2064 6563 2873 3a20 6279     def dec(s: by
-0000da00: 7465 7329 202d 3e20 7374 723a 0a20 2020  tes) -> str:.   
-0000da10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000da20: 6465 636f 6465 5f62 7974 6573 2873 2c20  decode_bytes(s, 
-0000da30: 656e 636f 6469 6e67 7320 6f72 205b 6465  encodings or [de
-0000da40: 6661 756c 745f 656e 636f 6469 6e67 5d2c  fault_encoding],
-0000da50: 2073 6574 2829 290a 0a20 2020 2020 2020   set())..       
-0000da60: 2065 6e63 6f64 6564 5f63 6f6d 706f 6e65   encoded_compone
-0000da70: 6e74 5f73 6570 203d 2065 6e63 2827 5e27  nt_sep = enc('^'
-0000da80: 290a 2020 2020 2020 2020 656e 636f 6465  ).        encode
-0000da90: 645f 6772 6f75 705f 7365 7020 3d20 656e  d_group_sep = en
-0000daa0: 6328 273d 2729 0a0a 2020 2020 2020 2020  c('=')..        
-0000dab0: 6469 7361 6c6c 6f77 6564 5f63 6861 7273  disallowed_chars
-0000dac0: 203d 205b 275c 5c27 2c20 273d 272c 2027   = ['\\', '=', '
-0000dad0: 5e27 5d0a 0a20 2020 2020 2020 2064 6566  ^']..        def
-0000dae0: 2073 7461 6e64 6172 6469 7a65 5f65 6e63   standardize_enc
-0000daf0: 6f64 696e 6728 7661 6c3a 2055 6e69 6f6e  oding(val: Union
-0000db00: 5b73 7472 2c20 6279 7465 735d 2920 2d3e  [str, bytes]) ->
-0000db10: 2062 7974 6573 3a0a 2020 2020 2020 2020   bytes:.        
-0000db20: 2020 2020 2320 5265 7475 726e 2061 2062      # Return a b
-0000db30: 7974 6520 656e 636f 6465 6420 7374 7269  yte encoded stri
-0000db40: 6e67 2072 6567 6172 646c 6573 7320 6f66  ng regardless of
-0000db50: 2074 6865 2069 6e70 7574 2074 7970 650a   the input type.
-0000db60: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-0000db70: 6973 2061 6c6c 6f77 7320 7468 6520 7573  is allows the us
-0000db80: 6572 2074 6f20 7375 7070 6c79 2061 206d  er to supply a m
-0000db90: 6978 7475 7265 206f 6620 7374 7220 616e  ixture of str an
-0000dba0: 6420 6279 7465 730a 2020 2020 2020 2020  d bytes.        
-0000dbb0: 2020 2020 2320 666f 7220 6469 6666 6572      # for differ
-0000dbc0: 656e 7420 7061 7274 7320 6f66 2074 6865  ent parts of the
-0000dbd0: 2069 6e70 7574 0a20 2020 2020 2020 2020   input.         
-0000dbe0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000dbf0: 2876 616c 2c20 6279 7465 7329 3a0a 2020  (val, bytes):.  
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000dc10: 6c5f 656e 6320 3d20 7661 6c0a 2020 2020  l_enc = val.    
-0000dc20: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
-0000dc30: 6465 6320 3d20 6465 6328 7661 6c29 0a20  dec = dec(val). 
-0000dc40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000dc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc60: 2076 616c 5f65 6e63 203d 2065 6e63 2876   val_enc = enc(v
-0000dc70: 616c 290a 2020 2020 2020 2020 2020 2020  al).            
-0000dc80: 2020 2020 7661 6c5f 6465 6320 3d20 7661      val_dec = va
-0000dc90: 6c0a 0a20 2020 2020 2020 2020 2020 2023  l..            #
-0000dca0: 2043 6865 636b 2066 6f72 2064 6973 616c   Check for disal
-0000dcb0: 6c6f 7765 6420 6368 6172 7320 696e 2074  lowed chars in t
-0000dcc0: 6865 2064 6563 6f64 6564 2073 7472 696e  he decoded strin
-0000dcd0: 670a 2020 2020 2020 2020 2020 2020 666f  g.            fo
-0000dce0: 7220 6320 696e 2064 6973 616c 6c6f 7765  r c in disallowe
-0000dcf0: 645f 6368 6172 733a 0a20 2020 2020 2020  d_chars:.       
-0000dd00: 2020 2020 2020 2020 2069 6620 6320 696e           if c in
-0000dd10: 2076 616c 5f64 6563 3a0a 2020 2020 2020   val_dec:.      
-0000dd20: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000dd30: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 2020 2020 2020 2020 6627 5374 7269 6e67          f'String
-0000dd60: 7320 6d61 7920 6e6f 7420 636f 6e74 6169  s may not contai
-0000dd70: 6e20 7468 6520 7b63 7d20 6368 6172 6163  n the {c} charac
-0000dd80: 7465 7227 0a20 2020 2020 2020 2020 2020  ter'.           
-0000dd90: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000dda0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-0000ddb0: 2074 6865 2065 6e63 6f64 6564 2073 7472   the encoded str
-0000ddc0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-0000ddd0: 7265 7475 726e 2076 616c 5f65 6e63 0a0a  return val_enc..
-0000dde0: 2020 2020 2020 2020 6465 6620 6d61 6b65          def make
-0000ddf0: 5f63 6f6d 706f 6e65 6e74 5f67 726f 7570  _component_group
-0000de00: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
-0000de10: 6d70 6f6e 656e 7473 3a20 5365 7175 656e  mponents: Sequen
-0000de20: 6365 5b55 6e69 6f6e 5b73 7472 2c20 6279  ce[Union[str, by
-0000de30: 7465 735d 5d0a 2020 2020 2020 2020 2920  tes]].        ) 
-0000de40: 2d3e 2062 7974 6573 3a0a 2020 2020 2020  -> bytes:.      
-0000de50: 2020 2020 2020 656e 636f 6465 645f 636f        encoded_co
-0000de60: 6d70 6f6e 656e 7473 203d 205b 7374 616e  mponents = [stan
-0000de70: 6461 7264 697a 655f 656e 636f 6469 6e67  dardize_encoding
-0000de80: 2863 2920 666f 7220 6320 696e 2063 6f6d  (c) for c in com
-0000de90: 706f 6e65 6e74 735d 0a20 2020 2020 2020  ponents].       
-0000dea0: 2020 2020 206a 6f69 6e65 645f 636f 6d70       joined_comp
-0000deb0: 6f6e 656e 7473 203d 2065 6e63 6f64 6564  onents = encoded
-0000dec0: 5f63 6f6d 706f 6e65 6e74 5f73 6570 2e6a  _component_sep.j
-0000ded0: 6f69 6e28 656e 636f 6465 645f 636f 6d70  oin(encoded_comp
-0000dee0: 6f6e 656e 7473 290a 2020 2020 2020 2020  onents).        
-0000def0: 2020 2020 7265 7475 726e 206a 6f69 6e65      return joine
-0000df00: 645f 636f 6d70 6f6e 656e 7473 2e72 7374  d_components.rst
-0000df10: 7269 7028 656e 636f 6465 645f 636f 6d70  rip(encoded_comp
-0000df20: 6f6e 656e 745f 7365 7029 0a0a 2020 2020  onent_sep)..    
-0000df30: 2020 2020 636f 6d70 6f6e 656e 745f 6772      component_gr
-0000df40: 6f75 7073 3a20 4c69 7374 5b62 7974 6573  oups: List[bytes
-0000df50: 5d20 3d20 5b0a 2020 2020 2020 2020 2020  ] = [.          
-0000df60: 2020 6d61 6b65 5f63 6f6d 706f 6e65 6e74    make_component
-0000df70: 5f67 726f 7570 2861 6c70 6861 6265 7469  _group(alphabeti
-0000df80: 635f 6772 6f75 7029 2c0a 2020 2020 2020  c_group),.      
-0000df90: 2020 2020 2020 6d61 6b65 5f63 6f6d 706f        make_compo
-0000dfa0: 6e65 6e74 5f67 726f 7570 2869 6465 6f67  nent_group(ideog
-0000dfb0: 7261 7068 6963 5f67 726f 7570 292c 0a20  raphic_group),. 
-0000dfc0: 2020 2020 2020 2020 2020 206d 616b 655f             make_
-0000dfd0: 636f 6d70 6f6e 656e 745f 6772 6f75 7028  component_group(
-0000dfe0: 7068 6f6e 6574 6963 5f67 726f 7570 290a  phonetic_group).
-0000dff0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0000e000: 2020 6a6f 696e 6564 5f67 726f 7570 733a    joined_groups:
-0000e010: 2062 7974 6573 203d 2065 6e63 6f64 6564   bytes = encoded
-0000e020: 5f67 726f 7570 5f73 6570 2e6a 6f69 6e28  _group_sep.join(
-0000e030: 636f 6d70 6f6e 656e 745f 6772 6f75 7073  component_groups
-0000e040: 290a 2020 2020 2020 2020 6a6f 696e 6564  ).        joined
-0000e050: 5f67 726f 7570 7320 3d20 6a6f 696e 6564  _groups = joined
-0000e060: 5f67 726f 7570 732e 7273 7472 6970 2865  _groups.rstrip(e
-0000e070: 6e63 6f64 6564 5f67 726f 7570 5f73 6570  ncoded_group_sep
-0000e080: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000e090: 206a 6f69 6e65 645f 6772 6f75 7073 0a0a   joined_groups..
-0000e0a0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-0000e0b0: 0a20 2020 2064 6566 2066 726f 6d5f 6e61  .    def from_na
-0000e0c0: 6d65 645f 636f 6d70 6f6e 656e 7473 280a  med_components(.
-0000e0d0: 2020 2020 2020 2020 636c 732c 0a20 2020          cls,.   
-0000e0e0: 2020 2020 2066 616d 696c 795f 6e61 6d65       family_name
-0000e0f0: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
-0000e100: 6573 5d20 3d20 2727 2c0a 2020 2020 2020  es] = '',.      
-0000e110: 2020 6769 7665 6e5f 6e61 6d65 3a20 556e    given_name: Un
-0000e120: 696f 6e5b 7374 722c 2062 7974 6573 5d20  ion[str, bytes] 
-0000e130: 3d20 2727 2c0a 2020 2020 2020 2020 6d69  = '',.        mi
-0000e140: 6464 6c65 5f6e 616d 653a 2055 6e69 6f6e  ddle_name: Union
-0000e150: 5b73 7472 2c20 6279 7465 735d 203d 2027  [str, bytes] = '
-0000e160: 272c 0a20 2020 2020 2020 206e 616d 655f  ',.        name_
-0000e170: 7072 6566 6978 3a20 556e 696f 6e5b 7374  prefix: Union[st
-0000e180: 722c 2062 7974 6573 5d20 3d20 2727 2c0a  r, bytes] = '',.
-0000e190: 2020 2020 2020 2020 6e61 6d65 5f73 7566          name_suf
-0000e1a0: 6669 783a 2055 6e69 6f6e 5b73 7472 2c20  fix: Union[str, 
-0000e1b0: 6279 7465 735d 203d 2027 272c 0a20 2020  bytes] = '',.   
-0000e1c0: 2020 2020 2066 616d 696c 795f 6e61 6d65       family_name
-0000e1d0: 5f69 6465 6f67 7261 7068 6963 3a20 556e  _ideographic: Un
-0000e1e0: 696f 6e5b 7374 722c 2062 7974 6573 5d20  ion[str, bytes] 
-0000e1f0: 3d20 2727 2c0a 2020 2020 2020 2020 6769  = '',.        gi
-0000e200: 7665 6e5f 6e61 6d65 5f69 6465 6f67 7261  ven_name_ideogra
-0000e210: 7068 6963 3a20 556e 696f 6e5b 7374 722c  phic: Union[str,
-0000e220: 2062 7974 6573 5d20 3d20 2727 2c0a 2020   bytes] = '',.  
-0000e230: 2020 2020 2020 6d69 6464 6c65 5f6e 616d        middle_nam
-0000e240: 655f 6964 656f 6772 6170 6869 633a 2055  e_ideographic: U
-0000e250: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
-0000e260: 203d 2027 272c 0a20 2020 2020 2020 206e   = '',.        n
-0000e270: 616d 655f 7072 6566 6978 5f69 6465 6f67  ame_prefix_ideog
-0000e280: 7261 7068 6963 3a20 556e 696f 6e5b 7374  raphic: Union[st
-0000e290: 722c 2062 7974 6573 5d20 3d20 2727 2c0a  r, bytes] = '',.
-0000e2a0: 2020 2020 2020 2020 6e61 6d65 5f73 7566          name_suf
-0000e2b0: 6669 785f 6964 656f 6772 6170 6869 633a  fix_ideographic:
-0000e2c0: 2055 6e69 6f6e 5b73 7472 2c20 6279 7465   Union[str, byte
-0000e2d0: 735d 203d 2027 272c 0a20 2020 2020 2020  s] = '',.       
-0000e2e0: 2066 616d 696c 795f 6e61 6d65 5f70 686f   family_name_pho
-0000e2f0: 6e65 7469 633a 2055 6e69 6f6e 5b73 7472  netic: Union[str
-0000e300: 2c20 6279 7465 735d 203d 2027 272c 0a20  , bytes] = '',. 
-0000e310: 2020 2020 2020 2067 6976 656e 5f6e 616d         given_nam
-0000e320: 655f 7068 6f6e 6574 6963 3a20 556e 696f  e_phonetic: Unio
-0000e330: 6e5b 7374 722c 2062 7974 6573 5d20 3d20  n[str, bytes] = 
-0000e340: 2727 2c0a 2020 2020 2020 2020 6d69 6464  '',.        midd
-0000e350: 6c65 5f6e 616d 655f 7068 6f6e 6574 6963  le_name_phonetic
-0000e360: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
-0000e370: 6573 5d20 3d20 2727 2c0a 2020 2020 2020  es] = '',.      
-0000e380: 2020 6e61 6d65 5f70 7265 6669 785f 7068    name_prefix_ph
-0000e390: 6f6e 6574 6963 3a20 556e 696f 6e5b 7374  onetic: Union[st
-0000e3a0: 722c 2062 7974 6573 5d20 3d20 2727 2c0a  r, bytes] = '',.
-0000e3b0: 2020 2020 2020 2020 6e61 6d65 5f73 7566          name_suf
-0000e3c0: 6669 785f 7068 6f6e 6574 6963 3a20 556e  fix_phonetic: Un
-0000e3d0: 696f 6e5b 7374 722c 2062 7974 6573 5d20  ion[str, bytes] 
-0000e3e0: 3d20 2727 2c0a 2020 2020 2020 2020 656e  = '',.        en
-0000e3f0: 636f 6469 6e67 733a 204f 7074 696f 6e61  codings: Optiona
-0000e400: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
-0000e410: 6f6e 652c 0a20 2020 2029 202d 3e20 2750  one,.    ) -> 'P
-0000e420: 6572 736f 6e4e 616d 6527 3a0a 2020 2020  ersonName':.    
-0000e430: 2020 2020 2222 2243 6f6e 7374 7275 6374      """Construct
-0000e440: 2061 2050 6572 736f 6e4e 616d 6520 6672   a PersonName fr
-0000e450: 6f6d 2065 7870 6c69 6369 7420 6e61 6d65  om explicit name
-0000e460: 6420 636f 6d70 6f6e 656e 7473 2e0a 0a20  d components... 
-0000e470: 2020 2020 2020 2054 6865 2044 4943 4f4d         The DICOM
-0000e480: 2073 7461 6e64 6172 6420 6465 7363 7269   standard descri
-0000e490: 6265 7320 6875 6d61 6e20 6e61 6d65 7320  bes human names 
-0000e4a0: 7573 696e 6720 6669 7665 2063 6f6d 706f  using five compo
-0000e4b0: 6e65 6e74 733a 0a20 2020 2020 2020 2066  nents:.        f
-0000e4c0: 616d 696c 7920 6e61 6d65 2c20 6769 7665  amily name, give
-0000e4d0: 6e20 6e61 6d65 2c20 6d69 6464 6c65 206e  n name, middle n
-0000e4e0: 616d 652c 206e 616d 6520 7072 6566 6978  ame, name prefix
-0000e4f0: 2c20 616e 6420 6e61 6d65 2073 7566 6669  , and name suffi
-0000e500: 782e 0a20 2020 2020 2020 2041 6e79 2063  x..        Any c
-0000e510: 6f6d 706f 6e65 6e74 206d 6179 2062 6520  omponent may be 
-0000e520: 616e 2065 6d70 7479 2073 7472 696e 6720  an empty string 
-0000e530: 2874 6865 2064 6566 6175 6c74 2920 6966  (the default) if
-0000e540: 206e 6f74 2075 7365 642e 0a20 2020 2020   not used..     
-0000e550: 2020 2041 2063 6f6d 706f 6e65 6e74 206d     A component m
-0000e560: 6179 2063 6f6e 7461 696e 206d 756c 7469  ay contain multi
-0000e570: 706c 6520 7370 6163 652d 7365 7061 7261  ple space-separa
-0000e580: 7465 6420 776f 7264 7320 6966 2074 6865  ted words if the
-0000e590: 7265 0a20 2020 2020 2020 2061 7265 2c20  re.        are, 
-0000e5a0: 666f 7220 6578 616d 706c 652c 206d 756c  for example, mul
-0000e5b0: 7469 706c 6520 6769 7665 6e20 6e61 6d65  tiple given name
-0000e5c0: 732c 206d 6964 646c 6520 6e61 6d65 732c  s, middle names,
-0000e5d0: 206f 7220 7469 746c 6573 2e0a 0a20 2020   or titles...   
-0000e5e0: 2020 2020 2041 6464 6974 696f 6e61 6c6c       Additionall
-0000e5f0: 792c 2065 6163 6820 636f 6d70 6f6e 656e  y, each componen
-0000e600: 7420 6d61 7920 6265 2072 6570 7265 7365  t may be represe
-0000e610: 6e74 6564 2069 6e20 6964 656f 6772 6170  nted in ideograp
-0000e620: 6869 6320 6f72 0a20 2020 2020 2020 2070  hic or.        p
-0000e630: 686f 6e65 7469 6320 666f 726d 2069 6e20  honetic form in 
-0000e640: 6164 6469 7469 6f6e 2074 6f20 286f 7220  addition to (or 
-0000e650: 696e 7374 6561 6420 6f66 2920 616c 7068  instead of) alph
-0000e660: 6162 6574 6963 2066 6f72 6d2e 0a0a 2020  abetic form...  
-0000e670: 2020 2020 2020 466f 7220 6d6f 7265 2069        For more i
-0000e680: 6e66 6f72 6d61 7469 6f6e 2073 6565 2074  nformation see t
-0000e690: 6865 2066 6f6c 6c6f 7769 6e67 2070 6172  he following par
-0000e6a0: 7473 206f 6620 7468 6520 4449 434f 4d20  ts of the DICOM 
-0000e6b0: 7374 616e 6461 7264 3a0a 2020 2020 2020  standard:.      
-0000e6c0: 2020 2d20 3a64 636d 3a60 5661 6c75 6520    - :dcm:`Value 
-0000e6d0: 5265 7072 6573 656e 7461 7469 6f6e 7320  Representations 
-0000e6e0: 3c70 6172 7430 352f 7365 6374 5f36 2e32  <part05/sect_6.2
-0000e6f0: 2e68 746d 6c3e 600a 2020 2020 2020 2020  .html>`.        
-0000e700: 2d20 3a64 636d 3a60 504e 2045 7861 6d70  - :dcm:`PN Examp
-0000e710: 6c65 7320 3c70 6172 7430 352f 7365 6374  les <part05/sect
-0000e720: 5f36 2e32 2e68 746d 6c23 7365 6374 5f36  _6.2.html#sect_6
-0000e730: 2e32 2e31 2e31 3e60 0a20 2020 2020 2020  .2.1.1>`.       
-0000e740: 202d 203a 6463 6d3a 6050 4e20 5072 6563   - :dcm:`PN Prec
-0000e750: 6973 6520 7365 6d61 6e74 6963 7320 3c70  ise semantics <p
-0000e760: 6172 7430 352f 7365 6374 5f36 2e32 2e68  art05/sect_6.2.h
-0000e770: 746d 6c23 7365 6374 5f36 2e32 2e31 2e32  tml#sect_6.2.1.2
-0000e780: 3e60 0a0a 2020 2020 2020 2020 4578 616d  >`..        Exam
-0000e790: 706c 650a 2020 2020 2020 2020 2d2d 2d2d  ple.        ----
-0000e7a0: 2d2d 2d0a 2020 2020 2020 2020 4120 6361  ---.        A ca
-0000e7b0: 7365 2077 6974 6820 6d75 6c74 6970 6c65  se with multiple
-0000e7c0: 2067 6976 656e 206e 616d 6573 2061 6e64   given names and
-0000e7d0: 2073 7566 6669 7865 7320 2844 4943 4f4d   suffixes (DICOM
-0000e7e0: 2073 7461 6e64 6172 642c 0a20 2020 2020   standard,.     
-0000e7f0: 2020 2070 6172 7420 352c 2073 6563 7420     part 5, sect 
-0000e800: 362e 322e 312e 3129 3a0a 0a20 2020 2020  6.2.1.1):..     
-0000e810: 2020 203e 3e3e 2070 6e20 3d20 5065 7273     >>> pn = Pers
-0000e820: 6f6e 4e61 6d65 2e66 726f 6d5f 6e61 6d65  onName.from_name
-0000e830: 645f 636f 6d70 6f6e 656e 7473 280a 2020  d_components(.  
-0000e840: 2020 2020 2020 2020 2020 2020 2020 6661                fa
-0000e850: 6d69 6c79 5f6e 616d 653d 2741 6461 6d73  mily_name='Adams
-0000e860: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0000e870: 2020 2067 6976 656e 5f6e 616d 653d 274a     given_name='J
-0000e880: 6f68 6e20 526f 6265 7274 2051 7569 6e63  ohn Robert Quinc
-0000e890: 7927 2c0a 2020 2020 2020 2020 2020 2020  y',.            
-0000e8a0: 2020 2020 6e61 6d65 5f70 7265 6669 783d      name_prefix=
-0000e8b0: 2752 6576 2e27 2c0a 2020 2020 2020 2020  'Rev.',.        
-0000e8c0: 2020 2020 2020 2020 6e61 6d65 5f73 7566          name_suf
-0000e8d0: 6669 783d 2742 2e41 2e20 4d2e 4469 762e  fix='B.A. M.Div.
-0000e8e0: 270a 2020 2020 2020 2020 2020 2020 290a  '.            ).
-0000e8f0: 0a20 2020 2020 2020 2041 204b 6f72 6561  .        A Korea
-0000e900: 6e20 6361 7365 2077 6974 6820 7068 6f6e  n case with phon
-0000e910: 6574 6963 2061 6e64 2069 6465 6f67 7261  etic and ideogra
-0000e920: 7068 6963 2072 6570 7265 7365 6e74 6174  phic representat
-0000e930: 696f 6e73 2028 5053 332e 352d 3230 3038  ions (PS3.5-2008
-0000e940: 0a20 2020 2020 2020 2073 6563 7469 6f6e  .        section
-0000e950: 2049 2e32 2070 2e20 3130 3829 3a0a 0a20   I.2 p. 108):.. 
-0000e960: 2020 2020 2020 203e 3e3e 2070 6e20 3d20         >>> pn = 
-0000e970: 5065 7273 6f6e 4e61 6d65 2e66 726f 6d5f  PersonName.from_
-0000e980: 6e61 6d65 645f 636f 6d70 6f6e 656e 7473  named_components
-0000e990: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000e9a0: 2020 6661 6d69 6c79 5f6e 616d 653d 2748    family_name='H
-0000e9b0: 6f6e 6727 2c0a 2020 2020 2020 2020 2020  ong',.          
-0000e9c0: 2020 2020 2020 6769 7665 6e5f 6e61 6d65        given_name
-0000e9d0: 3d27 4769 6c64 6f6e 6727 2c0a 2020 2020  ='Gildong',.    
-0000e9e0: 2020 2020 2020 2020 2020 2020 6661 6d69              fami
-0000e9f0: 6c79 5f6e 616d 655f 6964 656f 6772 6170  ly_name_ideograp
-0000ea00: 6869 633d 27e6 b4aa 272c 0a20 2020 2020  hic='...',.     
-0000ea10: 2020 2020 2020 2020 2020 2067 6976 656e             given
-0000ea20: 5f6e 616d 655f 6964 656f 6772 6170 6869  _name_ideographi
-0000ea30: 633d 27e5 9089 e6b4 9e27 2c0a 2020 2020  c='......',.    
-0000ea40: 2020 2020 2020 2020 2020 2020 6661 6d69              fami
-0000ea50: 6c79 5f6e 616d 655f 7068 6f6e 6574 6963  ly_name_phonetic
-0000ea60: 3d27 ed99 8d27 2c0a 2020 2020 2020 2020  ='...',.        
-0000ea70: 2020 2020 2020 2020 6769 7665 6e5f 6e61          given_na
-0000ea80: 6d65 5f70 686f 6e65 7469 633d 27ea b8b8  me_phonetic='...
-0000ea90: eb8f 9927 2c0a 2020 2020 2020 2020 2020  ...',.          
-0000eaa0: 2020 2020 2020 656e 636f 6469 6e67 733d        encodings=
-0000eab0: 5b64 6566 6175 6c74 5f65 6e63 6f64 696e  [default_encodin
-0000eac0: 672c 2027 6575 635f 6b72 275d 0a20 2020  g, 'euc_kr'].   
-0000ead0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000eae0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000eaf0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000eb00: 2d0a 2020 2020 2020 2020 6661 6d69 6c79  -.        family
-0000eb10: 5f6e 616d 653a 2055 6e69 6f6e 5b73 7472  _name: Union[str
-0000eb20: 2c20 6279 7465 735d 0a20 2020 2020 2020  , bytes].       
-0000eb30: 2020 2020 2046 616d 696c 7920 6e61 6d65       Family name
-0000eb40: 2069 6e20 616c 7068 6162 6574 6963 2066   in alphabetic f
-0000eb50: 6f72 6d2e 0a20 2020 2020 2020 2067 6976  orm..        giv
-0000eb60: 656e 5f6e 616d 653a 2055 6e69 6f6e 5b73  en_name: Union[s
-0000eb70: 7472 2c20 6279 7465 735d 0a20 2020 2020  tr, bytes].     
-0000eb80: 2020 2020 2020 2047 6976 656e 206e 616d         Given nam
-0000eb90: 6520 696e 2061 6c70 6861 6265 7469 6320  e in alphabetic 
-0000eba0: 666f 726d 2e0a 2020 2020 2020 2020 6d69  form..        mi
-0000ebb0: 6464 6c65 5f6e 616d 653a 2055 6e69 6f6e  ddle_name: Union
-0000ebc0: 5b73 7472 2c20 6279 7465 735d 0a20 2020  [str, bytes].   
-0000ebd0: 2020 2020 2020 2020 204d 6964 646c 6520           Middle 
-0000ebe0: 6e61 6d65 2069 6e20 616c 7068 6162 6574  name in alphabet
-0000ebf0: 6963 2066 6f72 6d2e 0a20 2020 2020 2020  ic form..       
-0000ec00: 206e 616d 655f 7072 6566 6978 3a20 556e   name_prefix: Un
-0000ec10: 696f 6e5b 7374 722c 2062 7974 6573 5d0a  ion[str, bytes].
-0000ec20: 2020 2020 2020 2020 2020 2020 4e61 6d65              Name
-0000ec30: 2070 7265 6669 7820 696e 2061 6c70 6861   prefix in alpha
-0000ec40: 6265 7469 6320 666f 726d 2c20 652e 672e  betic form, e.g.
-0000ec50: 2027 4d72 732e 272c 2027 4472 2e27 2c20   'Mrs.', 'Dr.', 
-0000ec60: 2753 722e 272c 2027 5265 762e 272e 0a20  'Sr.', 'Rev.'.. 
-0000ec70: 2020 2020 2020 206e 616d 655f 7375 6666         name_suff
-0000ec80: 6978 3a20 556e 696f 6e5b 7374 722c 2062  ix: Union[str, b
-0000ec90: 7974 6573 5d0a 2020 2020 2020 2020 2020  ytes].          
-0000eca0: 2020 4e61 6d65 2070 7265 6669 7820 696e    Name prefix in
-0000ecb0: 2061 6c70 6861 6265 7469 6320 666f 726d   alphabetic form
-0000ecc0: 2c20 652e 672e 2027 4d2e 442e 272c 2027  , e.g. 'M.D.', '
-0000ecd0: 422e 412e 2c20 4d2e 4469 762e 272c 0a20  B.A., M.Div.',. 
-0000ece0: 2020 2020 2020 2020 2020 2027 4368 6965             'Chie
-0000ecf0: 6620 4578 6563 7574 6976 6520 4f66 6669  f Executive Offi
-0000ed00: 6365 7227 2e0a 2020 2020 2020 2020 6661  cer'..        fa
-0000ed10: 6d69 6c79 5f6e 616d 655f 6964 656f 6772  mily_name_ideogr
-0000ed20: 6170 6869 633a 2055 6e69 6f6e 5b73 7472  aphic: Union[str
-0000ed30: 2c20 6279 7465 735d 0a20 2020 2020 2020  , bytes].       
-0000ed40: 2020 2020 2046 616d 696c 7920 6e61 6d65       Family name
-0000ed50: 2069 6e20 6964 656f 6772 6170 6869 6320   in ideographic 
-0000ed60: 666f 726d 2e0a 2020 2020 2020 2020 6769  form..        gi
-0000ed70: 7665 6e5f 6e61 6d65 5f69 6465 6f67 7261  ven_name_ideogra
-0000ed80: 7068 6963 3a20 556e 696f 6e5b 7374 722c  phic: Union[str,
-0000ed90: 2062 7974 6573 5d0a 2020 2020 2020 2020   bytes].        
-0000eda0: 2020 2020 4769 7665 6e20 6e61 6d65 2069      Given name i
-0000edb0: 6e20 6964 656f 6772 6170 6869 6320 666f  n ideographic fo
-0000edc0: 726d 2e0a 2020 2020 2020 2020 6d69 6464  rm..        midd
-0000edd0: 6c65 5f6e 616d 655f 6964 656f 6772 6170  le_name_ideograp
-0000ede0: 6869 633a 2055 6e69 6f6e 5b73 7472 2c20  hic: Union[str, 
-0000edf0: 6279 7465 735d 0a20 2020 2020 2020 2020  bytes].         
-0000ee00: 2020 204d 6964 646c 6520 6e61 6d65 2069     Middle name i
-0000ee10: 6e20 6964 656f 6772 6170 6869 6320 666f  n ideographic fo
-0000ee20: 726d 2e0a 2020 2020 2020 2020 6e61 6d65  rm..        name
-0000ee30: 5f70 7265 6669 785f 6964 656f 6772 6170  _prefix_ideograp
-0000ee40: 6869 633a 2055 6e69 6f6e 5b73 7472 2c20  hic: Union[str, 
-0000ee50: 6279 7465 735d 0a20 2020 2020 2020 2020  bytes].         
-0000ee60: 2020 204e 616d 6520 7072 6566 6978 2069     Name prefix i
-0000ee70: 6e20 6964 656f 6772 6170 6869 6320 666f  n ideographic fo
-0000ee80: 726d 2e0a 2020 2020 2020 2020 6e61 6d65  rm..        name
-0000ee90: 5f73 7566 6669 785f 6964 656f 6772 6170  _suffix_ideograp
-0000eea0: 6869 633a 2055 6e69 6f6e 5b73 7472 2c20  hic: Union[str, 
-0000eeb0: 6279 7465 735d 0a20 2020 2020 2020 2020  bytes].         
-0000eec0: 2020 204e 616d 6520 7375 6666 6978 2069     Name suffix i
-0000eed0: 6e20 6964 656f 6772 6170 6869 6320 666f  n ideographic fo
-0000eee0: 726d 2e0a 2020 2020 2020 2020 6661 6d69  rm..        fami
-0000eef0: 6c79 5f6e 616d 655f 7068 6f6e 6574 6963  ly_name_phonetic
-0000ef00: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
-0000ef10: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
-0000ef20: 4661 6d69 6c79 206e 616d 6520 696e 2070  Family name in p
-0000ef30: 686f 6e65 7469 6320 666f 726d 2e0a 2020  honetic form..  
-0000ef40: 2020 2020 2020 6769 7665 6e5f 6e61 6d65        given_name
-0000ef50: 5f70 686f 6e65 7469 633a 2055 6e69 6f6e  _phonetic: Union
-0000ef60: 5b73 7472 2c20 6279 7465 735d 0a20 2020  [str, bytes].   
-0000ef70: 2020 2020 2020 2020 2047 6976 656e 206e           Given n
-0000ef80: 616d 6520 696e 2070 686f 6e65 7469 6320  ame in phonetic 
-0000ef90: 666f 726d 2e0a 2020 2020 2020 2020 6d69  form..        mi
-0000efa0: 6464 6c65 5f6e 616d 655f 7068 6f6e 6574  ddle_name_phonet
-0000efb0: 6963 3a20 556e 696f 6e5b 7374 722c 2062  ic: Union[str, b
-0000efc0: 7974 6573 5d0a 2020 2020 2020 2020 2020  ytes].          
-0000efd0: 2020 4d69 6464 6c65 206e 616d 6520 696e    Middle name in
-0000efe0: 2070 686f 6e65 7469 6320 666f 726d 2e0a   phonetic form..
-0000eff0: 2020 2020 2020 2020 6e61 6d65 5f70 7265          name_pre
-0000f000: 6669 785f 7068 6f6e 6574 6963 3a20 556e  fix_phonetic: Un
-0000f010: 696f 6e5b 7374 722c 2062 7974 6573 5d0a  ion[str, bytes].
-0000f020: 2020 2020 2020 2020 2020 2020 4e61 6d65              Name
-0000f030: 2070 7265 6669 7820 696e 2070 686f 6e65   prefix in phone
-0000f040: 7469 6320 666f 726d 2e0a 2020 2020 2020  tic form..      
-0000f050: 2020 6e61 6d65 5f73 7566 6669 785f 7068    name_suffix_ph
-0000f060: 6f6e 6574 6963 3a20 556e 696f 6e5b 7374  onetic: Union[st
-0000f070: 722c 2062 7974 6573 5d0a 2020 2020 2020  r, bytes].      
-0000f080: 2020 2020 2020 4e61 6d65 2073 7566 6669        Name suffi
-0000f090: 7820 696e 2070 686f 6e65 7469 6320 666f  x in phonetic fo
-0000f0a0: 726d 2e0a 2020 2020 2020 2020 656e 636f  rm..        enco
-0000f0b0: 6469 6e67 733a 204f 7074 696f 6e61 6c5b  dings: Optional[
-0000f0c0: 4c69 7374 5b73 7472 5d5d 0a20 2020 2020  List[str]].     
-0000f0d0: 2020 2020 2020 2041 206c 6973 7420 6f66         A list of
-0000f0e0: 2065 6e63 6f64 696e 6773 2075 7365 6420   encodings used 
-0000f0f0: 666f 7220 7468 6520 6f74 6865 7220 696e  for the other in
-0000f100: 7075 7420 7061 7261 6d65 7465 7273 2e0a  put parameters..
-0000f110: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000f120: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000f130: 0a20 2020 2020 2020 2050 6572 736f 6e4e  .        PersonN
-0000f140: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-0000f150: 2050 6572 736f 6e4e 616d 6520 636f 6e73   PersonName cons
-0000f160: 7472 7563 7465 6420 6672 6f6d 2074 6865  tructed from the
-0000f170: 2073 7570 706c 6965 6420 636f 6d70 6f6e   supplied compon
-0000f180: 656e 7473 2e0a 0a20 2020 2020 2020 204e  ents...        N
-0000f190: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
-0000f1a0: 2d2d 0a20 2020 2020 2020 2053 7472 696e  --.        Strin
-0000f1b0: 6773 206d 6179 206e 6f74 2063 6f6e 7461  gs may not conta
-0000f1c0: 696e 2074 6865 2066 6f6c 6c6f 7769 6e67  in the following
-0000f1d0: 2063 6861 7261 6374 6572 733a 2027 5e27   characters: '^'
-0000f1e0: 2c20 273d 272c 0a20 2020 2020 2020 206f  , '=',.        o
-0000f1f0: 7220 7468 6520 6261 636b 736c 6173 6820  r the backslash 
-0000f200: 6368 6172 6163 7465 722e 0a20 2020 2020  character..     
-0000f210: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
-0000f220: 6c70 6861 6265 7469 635f 6772 6f75 703a  lphabetic_group:
-0000f230: 204c 6973 745b 556e 696f 6e5b 7374 722c   List[Union[str,
-0000f240: 2062 7974 6573 5d5d 203d 205b 0a20 2020   bytes]] = [.   
-0000f250: 2020 2020 2020 2020 2066 616d 696c 795f           family_
-0000f260: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0000f270: 2020 6769 7665 6e5f 6e61 6d65 2c0a 2020    given_name,.  
-0000f280: 2020 2020 2020 2020 2020 6d69 6464 6c65            middle
-0000f290: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-0000f2a0: 2020 206e 616d 655f 7072 6566 6978 2c0a     name_prefix,.
-0000f2b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000f2c0: 5f73 7566 6669 782c 0a20 2020 2020 2020  _suffix,.       
-0000f2d0: 205d 0a0a 2020 2020 2020 2020 2320 4964   ]..        # Id
-0000f2e0: 656f 6772 6170 6869 6320 636f 6d70 6f6e  eographic compon
-0000f2f0: 656e 7420 6772 6f75 700a 2020 2020 2020  ent group.      
-0000f300: 2020 6964 656f 6772 6170 6869 635f 6772    ideographic_gr
-0000f310: 6f75 703a 204c 6973 745b 556e 696f 6e5b  oup: List[Union[
-0000f320: 7374 722c 2062 7974 6573 5d5d 203d 205b  str, bytes]] = [
-0000f330: 0a20 2020 2020 2020 2020 2020 2066 616d  .            fam
-0000f340: 696c 795f 6e61 6d65 5f69 6465 6f67 7261  ily_name_ideogra
-0000f350: 7068 6963 2c0a 2020 2020 2020 2020 2020  phic,.          
-0000f360: 2020 6769 7665 6e5f 6e61 6d65 5f69 6465    given_name_ide
-0000f370: 6f67 7261 7068 6963 2c0a 2020 2020 2020  ographic,.      
-0000f380: 2020 2020 2020 6d69 6464 6c65 5f6e 616d        middle_nam
-0000f390: 655f 6964 656f 6772 6170 6869 632c 0a20  e_ideographic,. 
-0000f3a0: 2020 2020 2020 2020 2020 206e 616d 655f             name_
-0000f3b0: 7072 6566 6978 5f69 6465 6f67 7261 7068  prefix_ideograph
-0000f3c0: 6963 2c0a 2020 2020 2020 2020 2020 2020  ic,.            
-0000f3d0: 6e61 6d65 5f73 7566 6669 785f 6964 656f  name_suffix_ideo
-0000f3e0: 6772 6170 6869 632c 0a20 2020 2020 2020  graphic,.       
-0000f3f0: 205d 0a0a 2020 2020 2020 2020 2320 5068   ]..        # Ph
-0000f400: 6f6e 6574 6963 2063 6f6d 706f 6e65 6e74  onetic component
-0000f410: 2067 726f 7570 0a20 2020 2020 2020 2070   group.        p
-0000f420: 686f 6e65 7469 635f 6772 6f75 703a 204c  honetic_group: L
-0000f430: 6973 745b 556e 696f 6e5b 7374 722c 2062  ist[Union[str, b
-0000f440: 7974 6573 5d5d 203d 205b 0a20 2020 2020  ytes]] = [.     
-0000f450: 2020 2020 2020 2066 616d 696c 795f 6e61         family_na
-0000f460: 6d65 5f70 686f 6e65 7469 632c 0a20 2020  me_phonetic,.   
-0000f470: 2020 2020 2020 2020 2067 6976 656e 5f6e           given_n
-0000f480: 616d 655f 7068 6f6e 6574 6963 2c0a 2020  ame_phonetic,.  
-0000f490: 2020 2020 2020 2020 2020 6d69 6464 6c65            middle
-0000f4a0: 5f6e 616d 655f 7068 6f6e 6574 6963 2c0a  _name_phonetic,.
-0000f4b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000f4c0: 5f70 7265 6669 785f 7068 6f6e 6574 6963  _prefix_phonetic
-0000f4d0: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
-0000f4e0: 6d65 5f73 7566 6669 785f 7068 6f6e 6574  me_suffix_phonet
-0000f4f0: 6963 2c0a 2020 2020 2020 2020 5d0a 0a20  ic,.        ].. 
-0000f500: 2020 2020 2020 2065 6e63 6f64 6564 5f76         encoded_v
-0000f510: 616c 7565 3a20 6279 7465 7320 3d20 636c  alue: bytes = cl
-0000f520: 732e 5f65 6e63 6f64 655f 636f 6d70 6f6e  s._encode_compon
-0000f530: 656e 745f 6772 6f75 7073 280a 2020 2020  ent_groups(.    
-0000f540: 2020 2020 2020 2020 616c 7068 6162 6574          alphabet
-0000f550: 6963 5f67 726f 7570 2c0a 2020 2020 2020  ic_group,.      
-0000f560: 2020 2020 2020 6964 656f 6772 6170 6869        ideographi
-0000f570: 635f 6772 6f75 702c 0a20 2020 2020 2020  c_group,.       
-0000f580: 2020 2020 2070 686f 6e65 7469 635f 6772       phonetic_gr
-0000f590: 6f75 702c 0a20 2020 2020 2020 2020 2020  oup,.           
-0000f5a0: 2065 6e63 6f64 696e 6773 2c0a 2020 2020   encodings,.    
-0000f5b0: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
-0000f5c0: 6574 7572 6e20 636c 7328 656e 636f 6465  eturn cls(encode
-0000f5d0: 645f 7661 6c75 652c 2065 6e63 6f64 696e  d_value, encodin
-0000f5e0: 6773 3d65 6e63 6f64 696e 6773 290a 0a20  gs=encodings).. 
-0000f5f0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-0000f600: 2020 2020 6465 6620 6672 6f6d 5f6e 616d      def from_nam
-0000f610: 6564 5f63 6f6d 706f 6e65 6e74 735f 7665  ed_components_ve
-0000f620: 7465 7269 6e61 7279 280a 2020 2020 2020  terinary(.      
-0000f630: 2020 636c 732c 0a20 2020 2020 2020 2072    cls,.        r
-0000f640: 6573 706f 6e73 6962 6c65 5f70 6172 7479  esponsible_party
-0000f650: 5f6e 616d 653a 2055 6e69 6f6e 5b73 7472  _name: Union[str
-0000f660: 2c20 6279 7465 735d 203d 2027 272c 0a20  , bytes] = '',. 
-0000f670: 2020 2020 2020 2070 6174 6965 6e74 5f6e         patient_n
-0000f680: 616d 653a 2055 6e69 6f6e 5b73 7472 2c20  ame: Union[str, 
-0000f690: 6279 7465 735d 203d 2027 272c 0a20 2020  bytes] = '',.   
-0000f6a0: 2020 2020 2072 6573 706f 6e73 6962 6c65       responsible
-0000f6b0: 5f70 6172 7479 5f6e 616d 655f 6964 656f  _party_name_ideo
-0000f6c0: 6772 6170 6869 633a 2055 6e69 6f6e 5b73  graphic: Union[s
-0000f6d0: 7472 2c20 6279 7465 735d 203d 2027 272c  tr, bytes] = '',
-0000f6e0: 0a20 2020 2020 2020 2070 6174 6965 6e74  .        patient
-0000f6f0: 5f6e 616d 655f 6964 656f 6772 6170 6869  _name_ideographi
-0000f700: 633a 2055 6e69 6f6e 5b73 7472 2c20 6279  c: Union[str, by
-0000f710: 7465 735d 203d 2027 272c 0a20 2020 2020  tes] = '',.     
-0000f720: 2020 2072 6573 706f 6e73 6962 6c65 5f70     responsible_p
-0000f730: 6172 7479 5f6e 616d 655f 7068 6f6e 6574  arty_name_phonet
-0000f740: 6963 3a20 556e 696f 6e5b 7374 722c 2062  ic: Union[str, b
-0000f750: 7974 6573 5d20 3d20 2727 2c0a 2020 2020  ytes] = '',.    
-0000f760: 2020 2020 7061 7469 656e 745f 6e61 6d65      patient_name
-0000f770: 5f70 686f 6e65 7469 633a 2055 6e69 6f6e  _phonetic: Union
-0000f780: 5b73 7472 2c20 6279 7465 735d 203d 2027  [str, bytes] = '
-0000f790: 272c 0a20 2020 2020 2020 2065 6e63 6f64  ',.        encod
-0000f7a0: 696e 6773 3a20 4f70 7469 6f6e 616c 5b4c  ings: Optional[L
-0000f7b0: 6973 745b 7374 725d 5d20 3d20 4e6f 6e65  ist[str]] = None
-0000f7c0: 2c0a 2020 2020 2920 2d3e 2027 5065 7273  ,.    ) -> 'Pers
-0000f7d0: 6f6e 4e61 6d65 273a 0a20 2020 2020 2020  onName':.       
-0000f7e0: 2022 2222 436f 6e73 7472 7563 7420 6120   """Construct a 
-0000f7f0: 5065 7273 6f6e 4e61 6d65 2066 726f 6d20  PersonName from 
-0000f800: 6578 706c 6963 6974 206e 616d 6564 2063  explicit named c
-0000f810: 6f6d 706f 6e65 6e74 7320 666f 6c6c 6f77  omponents follow
-0000f820: 696e 6720 7468 650a 2020 2020 2020 2020  ing the.        
-0000f830: 7665 7465 7269 6e61 7279 2075 7361 6765  veterinary usage
-0000f840: 2063 6f6e 7665 6e74 696f 6e2e 0a0a 2020   convention...  
-0000f850: 2020 2020 2020 5468 6520 4449 434f 4d20        The DICOM 
-0000f860: 7374 616e 6461 7264 2064 6573 6372 6962  standard describ
-0000f870: 6573 206e 616d 6573 2066 6f72 2076 6574  es names for vet
-0000f880: 6572 696e 6172 7920 7573 6520 7769 7468  erinary use with
-0000f890: 2074 776f 2063 6f6d 706f 6e65 6e74 733a   two components:
-0000f8a0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-0000f8b0: 6962 6c65 2070 6172 7479 2066 616d 696c  ible party famil
-0000f8c0: 7920 6e61 6d65 204f 5220 7265 7370 6f6e  y name OR respon
-0000f8d0: 7369 626c 6520 7061 7274 7920 6f72 6761  sible party orga
-0000f8e0: 6e69 7a61 7469 6f6e 206e 616d 652c 0a20  nization name,. 
-0000f8f0: 2020 2020 2020 2061 6e64 2070 6174 6965         and patie
-0000f900: 6e74 206e 616d 652e 0a20 2020 2020 2020  nt name..       
-0000f910: 2041 6e79 2063 6f6d 706f 6e65 6e74 206d   Any component m
-0000f920: 6179 2062 6520 616e 2065 6d70 7479 2073  ay be an empty s
-0000f930: 7472 696e 6720 2874 6865 2064 6566 6175  tring (the defau
-0000f940: 6c74 2920 6966 206e 6f74 2075 7365 642e  lt) if not used.
-0000f950: 0a20 2020 2020 2020 2041 2063 6f6d 706f  .        A compo
-0000f960: 6e65 6e74 206d 6179 2063 6f6e 7461 696e  nent may contain
-0000f970: 206d 756c 7469 706c 6520 7370 6163 652d   multiple space-
-0000f980: 7365 7061 7261 7465 6420 776f 7264 7320  separated words 
-0000f990: 6966 206e 6563 6573 7361 7279 2e0a 0a20  if necessary... 
-0000f9a0: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
-0000f9b0: 6c6c 792c 2065 6163 6820 636f 6d70 6f6e  lly, each compon
-0000f9c0: 656e 7420 6d61 7920 6265 2072 6570 7265  ent may be repre
-0000f9d0: 7365 6e74 6564 2069 6e20 6964 656f 6772  sented in ideogr
-0000f9e0: 6170 6869 6320 6f72 0a20 2020 2020 2020  aphic or.       
-0000f9f0: 2070 686f 6e65 7469 6320 666f 726d 2069   phonetic form i
-0000fa00: 6e20 6164 6469 7469 6f6e 2074 6f20 286f  n addition to (o
-0000fa10: 7220 696e 7374 6561 6420 6f66 2920 616c  r instead of) al
-0000fa20: 7068 6162 6574 6963 2066 6f72 6d2e 0a0a  phabetic form...
-0000fa30: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
-0000fa40: 2069 6e66 6f72 6d61 7469 6f6e 2073 6565   information see
-0000fa50: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-0000fa60: 6172 7473 206f 6620 7468 6520 4449 434f  arts of the DICO
-0000fa70: 4d20 7374 616e 6461 7264 3a0a 2020 2020  M standard:.    
-0000fa80: 2020 2020 2d20 3a64 636d 3a60 5661 6c75      - :dcm:`Valu
-0000fa90: 6520 5265 7072 6573 656e 7461 7469 6f6e  e Representation
-0000faa0: 7320 3c70 6172 7430 352f 7365 6374 5f36  s <part05/sect_6
-0000fab0: 2e32 2e68 746d 6c3e 600a 2020 2020 2020  .2.html>`.      
-0000fac0: 2020 2d20 3a64 636d 3a60 504e 2045 7861    - :dcm:`PN Exa
-0000fad0: 6d70 6c65 7320 3c70 6172 7430 352f 7365  mples <part05/se
-0000fae0: 6374 5f36 2e32 2e68 746d 6c23 7365 6374  ct_6.2.html#sect
-0000faf0: 5f36 2e32 2e31 2e31 3e60 0a20 2020 2020  _6.2.1.1>`.     
-0000fb00: 2020 202d 203a 6463 6d3a 6050 4e20 5072     - :dcm:`PN Pr
-0000fb10: 6563 6973 6520 7365 6d61 6e74 6963 7320  ecise semantics 
-0000fb20: 3c70 6172 7430 352f 7365 6374 5f36 2e32  <part05/sect_6.2
-0000fb30: 2e68 746d 6c23 7365 6374 5f36 2e32 2e31  .html#sect_6.2.1
-0000fb40: 2e31 3e60 0a0a 2020 2020 2020 2020 4578  .1>`..        Ex
-0000fb50: 616d 706c 650a 2020 2020 2020 2020 2d2d  ample.        --
-0000fb60: 2d2d 2d2d 2d0a 0a20 2020 2020 2020 2041  -----..        A
-0000fb70: 2068 6f72 7365 2077 686f 7365 2072 6573   horse whose res
-0000fb80: 706f 6e73 6962 6c65 206f 7267 616e 697a  ponsible organiz
-0000fb90: 6174 696f 6e20 6973 206e 616d 6564 2022  ation is named "
-0000fba0: 4142 4320 4661 726d 7322 2c20 616e 6420  ABC Farms", and 
-0000fbb0: 7768 6f73 650a 2020 2020 2020 2020 6e61  whose.        na
-0000fbc0: 6d65 2069 7320 2252 756e 6e69 6e67 204f  me is "Running O
-0000fbd0: 6e20 5761 7465 7222 0a0a 2020 2020 2020  n Water"..      
-0000fbe0: 2020 3e3e 3e20 706e 203d 2050 6572 736f    >>> pn = Perso
-0000fbf0: 6e4e 616d 652e 6672 6f6d 5f6e 616d 6564  nName.from_named
-0000fc00: 5f63 6f6d 706f 6e65 6e74 735f 7665 7465  _components_vete
-0000fc10: 7269 6e61 7279 280a 2020 2020 2020 2020  rinary(.        
-0000fc20: 2020 2020 2020 2020 7265 7370 6f6e 7369          responsi
-0000fc30: 626c 655f 7061 7274 795f 6e61 6d65 3d27  ble_party_name='
-0000fc40: 4142 4320 4661 726d 7327 2c0a 2020 2020  ABC Farms',.    
-0000fc50: 2020 2020 2020 2020 2020 2020 7061 7469              pati
-0000fc60: 656e 745f 6e61 6d65 3d27 5275 6e6e 696e  ent_name='Runnin
-0000fc70: 6720 6f6e 2057 6174 6572 270a 2020 2020  g on Water'.    
-0000fc80: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000fc90: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000fca0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000fcb0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-0000fcc0: 6962 6c65 5f70 6172 7479 5f6e 616d 653a  ible_party_name:
-0000fcd0: 2055 6e69 6f6e 5b73 7472 2c20 6279 7465   Union[str, byte
-0000fce0: 735d 0a20 2020 2020 2020 2020 2020 204e  s].            N
-0000fcf0: 616d 6520 6f66 2074 6865 2072 6573 706f  ame of the respo
-0000fd00: 6e73 6962 6c65 2070 6172 7479 2069 6e20  nsible party in 
-0000fd10: 616c 7068 6162 6574 6963 2066 6f72 6d2e  alphabetic form.
-0000fd20: 2054 6869 7320 6d61 7920 6265 0a20 2020   This may be.   
-0000fd30: 2020 2020 2020 2020 2065 6974 6865 7220           either 
-0000fd40: 7468 6520 6661 6d69 6c79 206e 616d 6520  the family name 
-0000fd50: 6f66 2074 6865 2072 6573 706f 6e73 6962  of the responsib
-0000fd60: 6c65 2070 6172 7479 2c20 6f72 2074 6865  le party, or the
-0000fd70: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0000fd80: 6520 6f66 2074 6865 2072 6573 706f 6e73  e of the respons
-0000fd90: 6962 6c65 206f 7267 616e 697a 6174 696f  ible organizatio
-0000fda0: 6e2e 0a20 2020 2020 2020 2070 6174 6965  n..        patie
-0000fdb0: 6e74 5f6e 616d 653a 2055 6e69 6f6e 5b73  nt_name: Union[s
-0000fdc0: 7472 2c20 6279 7465 735d 0a20 2020 2020  tr, bytes].     
-0000fdd0: 2020 2020 2020 2050 6174 6965 6e74 206e         Patient n
-0000fde0: 616d 6520 696e 2061 6c70 6861 6265 7469  ame in alphabeti
-0000fdf0: 6320 666f 726d 2e0a 2020 2020 2020 2020  c form..        
-0000fe00: 7265 7370 6f6e 7369 626c 655f 7061 7274  responsible_part
-0000fe10: 795f 6e61 6d65 5f69 6465 6f67 7261 7068  y_name_ideograph
-0000fe20: 6963 3a20 556e 696f 6e5b 7374 722c 2062  ic: Union[str, b
-0000fe30: 7974 6573 5d0a 2020 2020 2020 2020 2020  ytes].          
-0000fe40: 2020 4e61 6d65 206f 6620 7468 6520 7265    Name of the re
-0000fe50: 7370 6f6e 7369 626c 6520 7061 7274 7920  sponsible party 
-0000fe60: 696e 2069 6465 6f67 7261 7068 6963 2066  in ideographic f
-0000fe70: 6f72 6d2e 0a20 2020 2020 2020 2070 6174  orm..        pat
-0000fe80: 6965 6e74 5f6e 616d 655f 6964 656f 6772  ient_name_ideogr
-0000fe90: 6170 6869 633a 2055 6e69 6f6e 5b73 7472  aphic: Union[str
-0000fea0: 2c20 6279 7465 735d 0a20 2020 2020 2020  , bytes].       
-0000feb0: 2020 2020 2050 6174 6965 6e74 206e 616d       Patient nam
-0000fec0: 6520 696e 2069 6465 6f67 7261 7068 6963  e in ideographic
-0000fed0: 2066 6f72 6d2e 0a20 2020 2020 2020 2072   form..        r
-0000fee0: 6573 706f 6e73 6962 6c65 5f70 6172 7479  esponsible_party
-0000fef0: 5f6e 616d 655f 7068 6f6e 6574 6963 3a20  _name_phonetic: 
-0000ff00: 556e 696f 6e5b 7374 722c 2062 7974 6573  Union[str, bytes
-0000ff10: 5d0a 2020 2020 2020 2020 2020 2020 4e61  ].            Na
-0000ff20: 6d65 206f 6620 7468 6520 7265 7370 6f6e  me of the respon
-0000ff30: 7369 626c 6520 7061 7274 7920 696e 2070  sible party in p
-0000ff40: 686f 6e65 7469 6320 666f 726d 2e0a 2020  honetic form..  
-0000ff50: 2020 2020 2020 7061 7469 656e 745f 6e61        patient_na
-0000ff60: 6d65 5f70 686f 6e65 7469 633a 2055 6e69  me_phonetic: Uni
-0000ff70: 6f6e 5b73 7472 2c20 6279 7465 735d 0a20  on[str, bytes]. 
-0000ff80: 2020 2020 2020 2020 2020 2050 6174 6965             Patie
-0000ff90: 6e74 206e 616d 6520 696e 2070 686f 6e65  nt name in phone
-0000ffa0: 7469 6320 666f 726d 2e0a 2020 2020 2020  tic form..      
-0000ffb0: 2020 656e 636f 6469 6e67 733a 204f 7074    encodings: Opt
-0000ffc0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-0000ffd0: 0a20 2020 2020 2020 2020 2020 2041 206c  .            A l
-0000ffe0: 6973 7420 6f66 2065 6e63 6f64 696e 6773  ist of encodings
-0000fff0: 2075 7365 6420 666f 7220 7468 6520 6f74   used for the ot
-00010000: 6865 7220 696e 7075 7420 7061 7261 6d65  her input parame
-00010010: 7465 7273 0a0a 2020 2020 2020 2020 5265  ters..        Re
-00010020: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00010030: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5065  -----.        Pe
-00010040: 7273 6f6e 4e61 6d65 3a0a 2020 2020 2020  rsonName:.      
-00010050: 2020 2020 2020 5065 7273 6f6e 4e61 6d65        PersonName
-00010060: 2063 6f6e 7374 7275 6374 6564 2066 726f   constructed fro
-00010070: 6d20 7468 6520 7375 7070 6c69 6564 2063  m the supplied c
-00010080: 6f6d 706f 6e65 6e74 730a 0a20 2020 2020  omponents..     
-00010090: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
-000100a0: 202d 2d2d 2d2d 0a20 2020 2020 2020 2053   -----.        S
-000100b0: 7472 696e 6773 206d 6179 206e 6f74 2063  trings may not c
-000100c0: 6f6e 7461 696e 2074 6865 2066 6f6c 6c6f  ontain the follo
-000100d0: 7769 6e67 2063 6861 7261 6374 6572 733a  wing characters:
-000100e0: 2027 5e27 2c20 273d 272c 0a20 2020 2020   '^', '=',.     
-000100f0: 2020 206f 7220 7468 6520 6261 636b 736c     or the backsl
-00010100: 6173 6820 6368 6172 6163 7465 722e 0a20  ash character.. 
-00010110: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010120: 2020 2061 6c70 6861 6265 7469 635f 6772     alphabetic_gr
-00010130: 6f75 703a 204c 6973 745b 556e 696f 6e5b  oup: List[Union[
-00010140: 7374 722c 2062 7974 6573 5d5d 203d 205b  str, bytes]] = [
-00010150: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00010160: 706f 6e73 6962 6c65 5f70 6172 7479 5f6e  ponsible_party_n
-00010170: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00010180: 2070 6174 6965 6e74 5f6e 616d 652c 0a20   patient_name,. 
-00010190: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-000101a0: 2020 6964 656f 6772 6170 6869 635f 6772    ideographic_gr
-000101b0: 6f75 703a 204c 6973 745b 556e 696f 6e5b  oup: List[Union[
-000101c0: 7374 722c 2062 7974 6573 5d5d 203d 205b  str, bytes]] = [
-000101d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000101e0: 706f 6e73 6962 6c65 5f70 6172 7479 5f6e  ponsible_party_n
-000101f0: 616d 655f 6964 656f 6772 6170 6869 632c  ame_ideographic,
-00010200: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-00010210: 6965 6e74 5f6e 616d 655f 6964 656f 6772  ient_name_ideogr
-00010220: 6170 6869 632c 0a20 2020 2020 2020 205d  aphic,.        ]
-00010230: 0a0a 2020 2020 2020 2020 7068 6f6e 6574  ..        phonet
-00010240: 6963 5f67 726f 7570 3a20 4c69 7374 5b55  ic_group: List[U
-00010250: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
-00010260: 5d20 3d20 5b0a 2020 2020 2020 2020 2020  ] = [.          
-00010270: 2020 7265 7370 6f6e 7369 626c 655f 7061    responsible_pa
-00010280: 7274 795f 6e61 6d65 5f70 686f 6e65 7469  rty_name_phoneti
-00010290: 632c 0a20 2020 2020 2020 2020 2020 2070  c,.            p
-000102a0: 6174 6965 6e74 5f6e 616d 655f 7068 6f6e  atient_name_phon
-000102b0: 6574 6963 2c0a 2020 2020 2020 2020 5d0a  etic,.        ].
-000102c0: 0a20 2020 2020 2020 2065 6e63 6f64 6564  .        encoded
-000102d0: 5f76 616c 7565 3a20 6279 7465 7320 3d20  _value: bytes = 
-000102e0: 636c 732e 5f65 6e63 6f64 655f 636f 6d70  cls._encode_comp
-000102f0: 6f6e 656e 745f 6772 6f75 7073 280a 2020  onent_groups(.  
-00010300: 2020 2020 2020 2020 2020 616c 7068 6162            alphab
-00010310: 6574 6963 5f67 726f 7570 2c0a 2020 2020  etic_group,.    
-00010320: 2020 2020 2020 2020 6964 656f 6772 6170          ideograp
-00010330: 6869 635f 6772 6f75 702c 0a20 2020 2020  hic_group,.     
-00010340: 2020 2020 2020 2070 686f 6e65 7469 635f         phonetic_
-00010350: 6772 6f75 702c 0a20 2020 2020 2020 2020  group,.         
-00010360: 2020 2065 6e63 6f64 696e 6773 0a20 2020     encodings.   
-00010370: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00010380: 7265 7475 726e 2063 6c73 2865 6e63 6f64  return cls(encod
-00010390: 6564 5f76 616c 7565 2c20 656e 636f 6469  ed_value, encodi
-000103a0: 6e67 733d 656e 636f 6469 6e67 7329 0a0a  ngs=encodings)..
-000103b0: 0a23 2041 6c69 6173 206f 6c64 2063 6c61  .# Alias old cla
-000103c0: 7373 206e 616d 6573 2066 6f72 2062 6163  ss names for bac
-000103d0: 6b77 6172 6473 2063 6f6d 7061 7420 696e  kwards compat in
-000103e0: 2075 7365 7220 636f 6465 0a64 6566 205f   user code.def _
-000103f0: 5f67 6574 6174 7472 5f5f 286e 616d 653a  _getattr__(name:
-00010400: 2073 7472 2920 2d3e 2041 6e79 3a0a 2020   str) -> Any:.  
-00010410: 2020 6966 206e 616d 6520 3d3d 2022 5065    if name == "Pe
-00010420: 7273 6f6e 4e61 6d65 556e 6963 6f64 6522  rsonNameUnicode"
-00010430: 3a0a 2020 2020 2020 2020 7761 726e 696e  :.        warnin
-00010440: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
-00010450: 2020 2020 2022 2750 6572 736f 6e4e 616d       "'PersonNam
-00010460: 6555 6e69 636f 6465 2720 6973 2064 6570  eUnicode' is dep
-00010470: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
-00010480: 2062 6520 7265 6d6f 7665 6420 696e 2022   be removed in "
-00010490: 0a20 2020 2020 2020 2020 2020 2022 7079  .            "py
-000104a0: 6469 636f 6d20 7633 2e30 2c20 7573 6520  dicom v3.0, use 
-000104b0: 2750 6572 736f 6e4e 616d 6527 2069 6e73  'PersonName' ins
-000104c0: 7465 6164 222c 0a20 2020 2020 2020 2020  tead",.         
-000104d0: 2020 2044 6570 7265 6361 7469 6f6e 5761     DeprecationWa
-000104e0: 726e 696e 670a 2020 2020 2020 2020 290a  rning.        ).
-000104f0: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-00010500: 6c6f 6261 6c73 2829 5b27 5065 7273 6f6e  lobals()['Person
-00010510: 4e61 6d65 275d 0a0a 2020 2020 7261 6973  Name']..    rais
-00010520: 6520 4174 7472 6962 7574 6545 7272 6f72  e AttributeError
-00010530: 2866 226d 6f64 756c 6520 7b5f 5f6e 616d  (f"module {__nam
-00010540: 655f 5f7d 2068 6173 206e 6f20 6174 7472  e__} has no attr
-00010550: 6962 7574 6520 7b6e 616d 657d 2229 0a0a  ibute {name}")..
-00010560: 0a69 6620 7379 732e 7665 7273 696f 6e5f  .if sys.version_
-00010570: 696e 666f 5b3a 325d 203c 2028 332c 2037  info[:2] < (3, 7
-00010580: 293a 0a20 2020 2050 6572 736f 6e4e 616d  ):.    PersonNam
-00010590: 6555 6e69 636f 6465 203d 2050 6572 736f  eUnicode = Perso
-000105a0: 6e4e 616d 650a                           nName.
+000009a0: 6620 7661 6c69 6461 7465 5f74 7970 6528  f validate_type(
+000009b0: 7672 3a20 7374 722c 2076 616c 7565 3a20  vr: str, value: 
+000009c0: 416e 792c 0a20 2020 2020 2020 2020 2020  Any,.           
+000009d0: 2020 2020 2020 2074 7970 6573 3a20 556e         types: Un
+000009e0: 696f 6e5b 5479 7065 2c20 5475 706c 655b  ion[Type, Tuple[
+000009f0: 5479 7065 2c20 5479 7065 5d5d 2920 2d3e  Type, Type]]) ->
+00000a00: 2054 7570 6c65 5b62 6f6f 6c2c 2073 7472   Tuple[bool, str
+00000a10: 5d3a 0a20 2020 2022 2222 4368 6563 6b73  ]:.    """Checks
+00000a20: 2066 6f72 2076 616c 6964 2074 7970 6573   for valid types
+00000a30: 2066 6f72 2061 2067 6976 656e 2056 522e   for a given VR.
+00000a40: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00000a50: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00000a60: 2020 2020 7672 203a 2073 7472 0a20 2020      vr : str.   
+00000a70: 2020 2020 2054 6865 2076 616c 7565 2072       The value r
+00000a80: 6570 7265 7365 6e74 6174 696f 6e20 746f  epresentation to
+00000a90: 2076 616c 6964 6174 6520 6167 6169 6e73   validate agains
+00000aa0: 742e 0a20 2020 2076 616c 7565 203a 2041  t..    value : A
+00000ab0: 6e79 0a20 2020 2020 2020 2054 6865 2076  ny.        The v
+00000ac0: 616c 7565 2074 6f20 7661 6c69 6461 7465  alue to validate
+00000ad0: 2e0a 2020 2020 7479 7065 733a 2054 7970  ..    types: Typ
+00000ae0: 6520 6f72 2054 7570 6c65 5b54 7970 655d  e or Tuple[Type]
+00000af0: 0a20 2020 2020 2020 2054 6865 2074 7970  .        The typ
+00000b00: 6520 6f72 2074 7570 6c65 206f 6620 7479  e or tuple of ty
+00000b10: 7065 7320 7375 7070 6f72 7465 6420 666f  pes supported fo
+00000b20: 7220 7468 6520 6769 7665 6e20 5652 2e0a  r the given VR..
+00000b30: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00000b40: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00000b50: 2041 2074 7570 6c65 206f 6620 6120 626f   A tuple of a bo
+00000b60: 6f6c 6561 6e20 7661 6c69 6461 7469 6f6e  olean validation
+00000b70: 2072 6573 756c 7420 616e 6420 7468 6520   result and the 
+00000b80: 6572 726f 7220 6d65 7373 6167 652e 0a20  error message.. 
+00000b90: 2020 2022 2222 0a20 2020 2069 6620 7661     """.    if va
+00000ba0: 6c75 6520 6973 206e 6f74 204e 6f6e 6520  lue is not None 
+00000bb0: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
+00000bc0: 6365 2876 616c 7565 2c20 7479 7065 7329  ce(value, types)
+00000bd0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00000be0: 2046 616c 7365 2c20 280a 2020 2020 2020   False, (.      
+00000bf0: 2020 2020 2020 6622 4120 7661 6c75 6520        f"A value 
+00000c00: 6f66 2074 7970 6520 277b 7479 7065 2876  of type '{type(v
+00000c10: 616c 7565 292e 5f5f 6e61 6d65 5f5f 7d27  alue).__name__}'
+00000c20: 2063 616e 6e6f 7420 6265 2022 0a20 2020   cannot be ".   
+00000c30: 2020 2020 2020 2020 2066 2261 7373 6967           f"assig
+00000c40: 6e65 6420 746f 2061 2074 6167 2077 6974  ned to a tag wit
+00000c50: 6820 5652 207b 7672 7d2e 220a 2020 2020  h VR {vr}.".    
+00000c60: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
+00000c70: 2054 7275 652c 2022 220a 0a0a 6465 6620   True, ""...def 
+00000c80: 7661 6c69 6461 7465 5f76 725f 6c65 6e67  validate_vr_leng
+00000c90: 7468 2876 723a 2073 7472 2c20 7661 6c75  th(vr: str, valu
+00000ca0: 653a 2041 6e79 2920 2d3e 2054 7570 6c65  e: Any) -> Tuple
+00000cb0: 5b62 6f6f 6c2c 2073 7472 5d3a 0a20 2020  [bool, str]:.   
+00000cc0: 2022 2222 5661 6c69 6461 7465 2074 6865   """Validate the
+00000cd0: 2076 616c 7565 206c 656e 6774 6820 666f   value length fo
+00000ce0: 7220 6120 6769 7665 6e20 5652 2e0a 0a20  r a given VR... 
+00000cf0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00000d00: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00000d10: 2076 7220 3a20 7374 720a 2020 2020 2020   vr : str.      
+00000d20: 2020 5468 6520 7661 6c75 6520 7265 7072    The value repr
+00000d30: 6573 656e 7461 7469 6f6e 2074 6f20 7661  esentation to va
+00000d40: 6c69 6461 7465 2061 6761 696e 7374 2e0a  lidate against..
+00000d50: 2020 2020 7661 6c75 6520 3a20 416e 790a      value : Any.
+00000d60: 2020 2020 2020 2020 5468 6520 7661 6c75          The valu
+00000d70: 6520 746f 2076 616c 6964 6174 652e 0a0a  e to validate...
+00000d80: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00000d90: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00000da0: 4120 7475 706c 6520 6f66 2061 2062 6f6f  A tuple of a boo
+00000db0: 6c65 616e 2076 616c 6964 6174 696f 6e20  lean validation 
+00000dc0: 7265 7375 6c74 2061 6e64 2074 6865 2065  result and the e
+00000dd0: 7272 6f72 206d 6573 7361 6765 2e0a 2020  rror message..  
+00000de0: 2020 2222 220a 2020 2020 6d61 785f 6c65    """.    max_le
+00000df0: 6e67 7468 203d 204d 4158 5f56 414c 5545  ngth = MAX_VALUE
+00000e00: 5f4c 454e 2e67 6574 2876 722c 2030 290a  _LEN.get(vr, 0).
+00000e10: 2020 2020 6966 206d 6178 5f6c 656e 6774      if max_lengt
+00000e20: 6820 3e20 303a 0a20 2020 2020 2020 2076  h > 0:.        v
+00000e30: 616c 7565 5f6c 656e 6774 6820 3d20 6c65  alue_length = le
+00000e40: 6e28 7661 6c75 6529 0a20 2020 2020 2020  n(value).       
+00000e50: 2069 6620 7661 6c75 655f 6c65 6e67 7468   if value_length
+00000e60: 203e 206d 6178 5f6c 656e 6774 683a 0a20   > max_length:. 
+00000e70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000e80: 6e20 4661 6c73 652c 2028 0a20 2020 2020  n False, (.     
+00000e90: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
+00000ea0: 2076 616c 7565 206c 656e 6774 6820 287b   value length ({
+00000eb0: 7661 6c75 655f 6c65 6e67 7468 7d29 2065  value_length}) e
+00000ec0: 7863 6565 6473 2074 6865 2022 0a20 2020  xceeds the ".   
+00000ed0: 2020 2020 2020 2020 2020 2020 2066 226d               f"m
+00000ee0: 6178 696d 756d 206c 656e 6774 6820 6f66  aximum length of
+00000ef0: 207b 6d61 785f 6c65 6e67 7468 7d20 616c   {max_length} al
+00000f00: 6c6f 7765 6420 666f 7220 5652 207b 7672  lowed for VR {vr
+00000f10: 7d2e 220a 2020 2020 2020 2020 2020 2020  }.".            
+00000f20: 290a 2020 2020 7265 7475 726e 2054 7275  ).    return Tru
+00000f30: 652c 2022 220a 0a0a 6465 6620 7661 6c69  e, ""...def vali
+00000f40: 6461 7465 5f74 7970 655f 616e 645f 6c65  date_type_and_le
+00000f50: 6e67 7468 2876 723a 2073 7472 2c20 7661  ngth(vr: str, va
+00000f60: 6c75 653a 2041 6e79 2920 2d3e 2054 7570  lue: Any) -> Tup
+00000f70: 6c65 5b62 6f6f 6c2c 2073 7472 5d3a 0a20  le[bool, str]:. 
+00000f80: 2020 2022 2222 5661 6c69 6461 7465 2074     """Validate t
+00000f90: 6865 2063 6f72 7265 6374 2074 7970 6520  he correct type 
+00000fa0: 616e 6420 7468 6520 7661 6c75 6520 6c65  and the value le
+00000fb0: 6e67 7468 2066 6f72 2061 2067 6976 656e  ngth for a given
+00000fc0: 2056 522e 0a0a 2020 2020 5061 7261 6d65   VR...    Parame
+00000fd0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00000fe0: 2d2d 2d0a 2020 2020 7672 203a 2073 7472  ---.    vr : str
+00000ff0: 0a20 2020 2020 2020 2054 6865 2076 616c  .        The val
+00001000: 7565 2072 6570 7265 7365 6e74 6174 696f  ue representatio
+00001010: 6e20 746f 2076 616c 6964 6174 6520 6167  n to validate ag
+00001020: 6169 6e73 742e 0a20 2020 2076 616c 7565  ainst..    value
+00001030: 203a 2041 6e79 0a20 2020 2020 2020 2054   : Any.        T
+00001040: 6865 2076 616c 7565 2074 6f20 7661 6c69  he value to vali
+00001050: 6461 7465 2e0a 0a20 2020 2052 6574 7572  date...    Retur
+00001060: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00001070: 2020 2020 2020 2041 2074 7570 6c65 206f         A tuple o
+00001080: 6620 6120 626f 6f6c 6561 6e20 7661 6c69  f a boolean vali
+00001090: 6461 7469 6f6e 2072 6573 756c 7420 616e  dation result an
+000010a0: 6420 7468 6520 6572 726f 7220 6d65 7373  d the error mess
+000010b0: 6167 652e 0a20 2020 2022 2222 0a20 2020  age..    """.   
+000010c0: 2076 616c 6964 2c20 6d73 6720 3d20 7661   valid, msg = va
+000010d0: 6c69 6461 7465 5f74 7970 6528 7672 2c20  lidate_type(vr, 
+000010e0: 7661 6c75 652c 2028 7374 722c 2062 7974  value, (str, byt
+000010f0: 6573 2929 0a20 2020 2069 6620 6e6f 7420  es)).    if not 
+00001100: 7661 6c69 643a 0a20 2020 2020 2020 2072  valid:.        r
+00001110: 6574 7572 6e20 7661 6c69 642c 206d 7367  eturn valid, msg
+00001120: 0a20 2020 2072 6574 7572 6e20 7661 6c69  .    return vali
+00001130: 6461 7465 5f76 725f 6c65 6e67 7468 2876  date_vr_length(v
+00001140: 722c 2076 616c 7565 290a 0a0a 6465 6620  r, value)...def 
+00001150: 7661 6c69 6461 7465 5f72 6567 6578 2876  validate_regex(v
+00001160: 723a 2073 7472 2c20 7661 6c75 653a 2041  r: str, value: A
+00001170: 6e79 2920 2d3e 2054 7570 6c65 5b62 6f6f  ny) -> Tuple[boo
+00001180: 6c2c 2073 7472 5d3a 0a20 2020 2022 2222  l, str]:.    """
+00001190: 5661 6c69 6461 7465 2074 6865 2076 616c  Validate the val
+000011a0: 7565 2066 6f72 2061 2067 6976 656e 2056  ue for a given V
+000011b0: 5220 666f 7220 616c 6c6f 7765 6420 6368  R for allowed ch
+000011c0: 6172 6163 7465 7273 0a20 2020 2075 7369  aracters.    usi
+000011d0: 6e67 2061 2072 6567 756c 6172 2065 7870  ng a regular exp
+000011e0: 7265 7373 696f 6e2e 0a0a 2020 2020 5061  ression...    Pa
+000011f0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00001200: 2d2d 2d2d 2d2d 2d0a 2020 2020 7672 203a  -------.    vr :
+00001210: 2073 7472 0a20 2020 2020 2020 2054 6865   str.        The
+00001220: 2076 616c 7565 2072 6570 7265 7365 6e74   value represent
+00001230: 6174 696f 6e20 746f 2076 616c 6964 6174  ation to validat
+00001240: 6520 6167 6169 6e73 742e 0a20 2020 2076  e against..    v
+00001250: 616c 7565 203a 2041 6e79 0a20 2020 2020  alue : Any.     
+00001260: 2020 2054 6865 2076 616c 7565 2074 6f20     The value to 
+00001270: 7661 6c69 6461 7465 2e0a 0a20 2020 2052  validate...    R
+00001280: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00001290: 2d2d 0a20 2020 2020 2020 2041 2074 7570  --.        A tup
+000012a0: 6c65 206f 6620 6120 626f 6f6c 6561 6e20  le of a boolean 
+000012b0: 7661 6c69 6461 7469 6f6e 2072 6573 756c  validation resul
+000012c0: 7420 616e 6420 7468 6520 6572 726f 7220  t and the error 
+000012d0: 6d65 7373 6167 652e 0a20 2020 2022 2222  message..    """
+000012e0: 0a20 2020 2069 6620 7661 6c75 653a 0a20  .    if value:. 
+000012f0: 2020 2020 2020 2072 6567 6578 3a20 416e         regex: An
+00001300: 790a 2020 2020 2020 2020 6e65 776c 696e  y.        newlin
+00001310: 653a 2055 6e69 6f6e 5b73 7472 2c20 696e  e: Union[str, in
+00001320: 745d 0a20 2020 2020 2020 2069 6620 6973  t].        if is
+00001330: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
+00001340: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00001350: 2020 7265 6765 7820 3d20 5354 525f 5652    regex = STR_VR
+00001360: 5f52 4547 4558 4553 5b76 725d 0a20 2020  _REGEXES[vr].   
+00001370: 2020 2020 2020 2020 206e 6577 6c69 6e65           newline
+00001380: 203d 2022 5c6e 220a 2020 2020 2020 2020   = "\n".        
+00001390: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000013a0: 2020 7265 6765 7820 3d20 4259 5445 5f56    regex = BYTE_V
+000013b0: 525f 5245 4745 5845 535b 7672 5d0a 2020  R_REGEXES[vr].  
+000013c0: 2020 2020 2020 2020 2020 6e65 776c 696e            newlin
+000013d0: 6520 3d20 3130 2020 2320 6e65 776c 696e  e = 10  # newlin
+000013e0: 6520 6368 6172 6163 7465 720a 2020 2020  e character.    
+000013f0: 2020 2020 6966 206e 6f74 2072 652e 6d61      if not re.ma
+00001400: 7463 6828 7265 6765 782c 2076 616c 7565  tch(regex, value
+00001410: 2920 6f72 2076 616c 7565 2061 6e64 2076  ) or value and v
+00001420: 616c 7565 5b2d 315d 203d 3d20 6e65 776c  alue[-1] == newl
+00001430: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
+00001440: 2072 6574 7572 6e20 4661 6c73 652c 2066   return False, f
+00001450: 2249 6e76 616c 6964 2076 616c 7565 2066  "Invalid value f
+00001460: 6f72 2056 5220 7b76 727d 3a20 7b76 616c  or VR {vr}: {val
+00001470: 7565 2172 7d2e 220a 2020 2020 7265 7475  ue!r}.".    retu
+00001480: 726e 2054 7275 652c 2022 220a 0a0a 6465  rn True, ""...de
+00001490: 6620 7661 6c69 6461 7465 5f74 7970 655f  f validate_type_
+000014a0: 616e 645f 7265 6765 7828 7672 3a20 7374  and_regex(vr: st
+000014b0: 722c 2076 616c 7565 3a20 416e 7929 202d  r, value: Any) -
+000014c0: 3e20 5475 706c 655b 626f 6f6c 2c20 7374  > Tuple[bool, st
+000014d0: 725d 3a0a 2020 2020 2222 2256 616c 6964  r]:.    """Valid
+000014e0: 6174 6520 7468 6174 2074 6865 2076 616c  ate that the val
+000014f0: 7565 2069 7320 6f66 2074 7970 6520 3a63  ue is of type :c
+00001500: 6c61 7373 3a60 7374 7260 206f 7220 3a63  lass:`str` or :c
+00001510: 6c61 7373 3a60 6279 7465 7360 0a20 2020  lass:`bytes`.   
+00001520: 2061 6e64 2074 6861 7420 7468 6520 7661   and that the va
+00001530: 6c75 6520 6d61 7463 6865 7320 7468 6520  lue matches the 
+00001540: 5652 2d73 7065 6369 6669 6320 7265 6775  VR-specific regu
+00001550: 6c61 7220 6578 7072 6573 7369 6f6e 2e0a  lar expression..
+00001560: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00001570: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00001580: 2020 2076 7220 3a20 7374 720a 2020 2020     vr : str.    
+00001590: 2020 2020 5468 6520 7661 6c75 6520 7265      The value re
+000015a0: 7072 6573 656e 7461 7469 6f6e 2074 6f20  presentation to 
+000015b0: 7661 6c69 6461 7465 2061 6761 696e 7374  validate against
+000015c0: 2e0a 2020 2020 7661 6c75 6520 3a20 416e  ..    value : An
+000015d0: 790a 2020 2020 2020 2020 5468 6520 7661  y.        The va
+000015e0: 6c75 6520 746f 2076 616c 6964 6174 652e  lue to validate.
+000015f0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00001600: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00001610: 2020 4120 7475 706c 6520 6f66 2061 2062    A tuple of a b
+00001620: 6f6f 6c65 616e 2076 616c 6964 6174 696f  oolean validatio
+00001630: 6e20 7265 7375 6c74 2061 6e64 2074 6865  n result and the
+00001640: 2065 7272 6f72 206d 6573 7361 6765 2e0a   error message..
+00001650: 2020 2020 2222 220a 2020 2020 7661 6c69      """.    vali
+00001660: 642c 206d 7367 203d 2076 616c 6964 6174  d, msg = validat
+00001670: 655f 7479 7065 2876 722c 2076 616c 7565  e_type(vr, value
+00001680: 2c20 2873 7472 2c20 6279 7465 7329 290a  , (str, bytes)).
+00001690: 2020 2020 6966 206e 6f74 2076 616c 6964      if not valid
+000016a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000016b0: 2076 616c 6964 2c20 6d73 670a 2020 2020   valid, msg.    
+000016c0: 7265 7475 726e 2076 616c 6964 6174 655f  return validate_
+000016d0: 7265 6765 7828 7672 2c20 7661 6c75 6529  regex(vr, value)
+000016e0: 0a0a 0a64 6566 2076 616c 6964 6174 655f  ...def validate_
+000016f0: 6461 7465 5f74 696d 6528 0a20 2020 2020  date_time(.     
+00001700: 2020 2076 723a 2073 7472 2c20 7661 6c75     vr: str, valu
+00001710: 653a 2041 6e79 2c20 6461 7465 5f74 696d  e: Any, date_tim
+00001720: 655f 7479 7065 3a20 5479 7065 2920 2d3e  e_type: Type) ->
+00001730: 2054 7570 6c65 5b62 6f6f 6c2c 2073 7472   Tuple[bool, str
+00001740: 5d3a 0a20 2020 2022 2222 4368 6563 6b73  ]:.    """Checks
+00001750: 2066 6f72 2076 616c 6964 2076 616c 7565   for valid value
+00001760: 7320 666f 7220 6461 7465 2f74 696d 6520  s for date/time 
+00001770: 7265 6c61 7465 6420 5652 732e 0a0a 2020  related VRs...  
+00001780: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00001790: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000017a0: 7672 203a 2073 7472 0a20 2020 2020 2020  vr : str.       
+000017b0: 2054 6865 2076 616c 7565 2072 6570 7265   The value repre
+000017c0: 7365 6e74 6174 696f 6e20 746f 2076 616c  sentation to val
+000017d0: 6964 6174 6520 6167 6169 6e73 742e 0a20  idate against.. 
+000017e0: 2020 2076 616c 7565 203a 2041 6e79 0a20     value : Any. 
+000017f0: 2020 2020 2020 2054 6865 2076 616c 7565         The value
+00001800: 2074 6f20 7661 6c69 6461 7465 2e0a 2020   to validate..  
+00001810: 2020 6461 7465 5f74 696d 655f 7479 7065    date_time_type
+00001820: 3a20 7479 7065 0a20 2020 2020 2020 2054  : type.        T
+00001830: 6865 2073 7065 6369 6669 6320 7479 7065  he specific type
+00001840: 2073 7570 706f 7274 6564 2066 6f72 2074   supported for t
+00001850: 6865 2067 6976 656e 2056 5220 2861 6464  he given VR (add
+00001860: 6974 696f 6e61 6c20 746f 2073 7472 2f62  itional to str/b
+00001870: 7974 6573 292e 0a0a 2020 2020 5265 7475  ytes)...    Retu
+00001880: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00001890: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
+000018a0: 6f66 2061 2062 6f6f 6c65 616e 2076 616c  of a boolean val
+000018b0: 6964 6174 696f 6e20 7265 7375 6c74 2061  idation result a
+000018c0: 6e64 2074 6865 2065 7272 6f72 206d 6573  nd the error mes
+000018d0: 7361 6765 2e0a 2020 2020 2222 220a 0a20  sage..    """.. 
+000018e0: 2020 2069 6620 7661 6c75 6520 616e 6420     if value and 
+000018f0: 6973 696e 7374 616e 6365 2876 616c 7565  isinstance(value
+00001900: 2c20 6461 7465 5f74 696d 655f 7479 7065  , date_time_type
+00001910: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00001920: 6e20 5472 7565 2c20 2222 0a20 2020 2072  n True, "".    r
+00001930: 6574 7572 6e20 7661 6c69 6461 7465 5f74  eturn validate_t
+00001940: 7970 655f 616e 645f 7265 6765 7828 7672  ype_and_regex(vr
+00001950: 2c20 7661 6c75 6529 0a0a 0a64 6566 2076  , value)...def v
+00001960: 616c 6964 6174 655f 6c65 6e67 7468 5f61  alidate_length_a
+00001970: 6e64 5f74 7970 655f 616e 645f 7265 6765  nd_type_and_rege
+00001980: 7828 0a20 2020 2020 2020 2076 723a 2073  x(.        vr: s
+00001990: 7472 2c20 7661 6c75 653a 2041 6e79 2920  tr, value: Any) 
+000019a0: 2d3e 2054 7570 6c65 5b62 6f6f 6c2c 2073  -> Tuple[bool, s
+000019b0: 7472 5d3a 0a20 2020 2022 2222 5661 6c69  tr]:.    """Vali
+000019c0: 6461 7465 2074 6865 2076 616c 7565 2066  date the value f
+000019d0: 6f72 2061 2067 6976 656e 2056 5220 666f  or a given VR fo
+000019e0: 7220 6d61 7869 6d75 6d20 6c65 6e67 7468  r maximum length
+000019f0: 2c20 666f 7220 7468 6520 636f 7272 6563  , for the correc
+00001a00: 740a 2020 2020 7661 6c75 6520 7479 7065  t.    value type
+00001a10: 2c20 616e 6420 666f 7220 616c 6c6f 7765  , and for allowe
+00001a20: 6420 6368 6172 6163 7465 7273 2075 7369  d characters usi
+00001a30: 6e67 2061 2072 6567 756c 6172 2065 7870  ng a regular exp
+00001a40: 7265 7373 696f 6e2e 0a0a 2020 2020 5061  ression...    Pa
+00001a50: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00001a60: 2d2d 2d2d 2d2d 2d0a 2020 2020 7672 203a  -------.    vr :
+00001a70: 2073 7472 0a20 2020 2020 2020 2054 6865   str.        The
+00001a80: 2076 616c 7565 2072 6570 7265 7365 6e74   value represent
+00001a90: 6174 696f 6e20 746f 2076 616c 6964 6174  ation to validat
+00001aa0: 6520 6167 6169 6e73 742e 0a20 2020 2076  e against..    v
+00001ab0: 616c 7565 203a 2041 6e79 0a20 2020 2020  alue : Any.     
+00001ac0: 2020 2054 6865 2076 616c 7565 2074 6f20     The value to 
+00001ad0: 7661 6c69 6461 7465 2e0a 0a20 2020 2052  validate...    R
+00001ae0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00001af0: 2d2d 0a20 2020 2020 2020 2041 2074 7570  --.        A tup
+00001b00: 6c65 206f 6620 6120 626f 6f6c 6561 6e20  le of a boolean 
+00001b10: 7661 6c69 6461 7469 6f6e 2072 6573 756c  validation resul
+00001b20: 7420 616e 6420 7468 6520 6572 726f 7220  t and the error 
+00001b30: 6d65 7373 6167 652e 0a20 2020 2022 2222  message..    """
+00001b40: 0a20 2020 2076 616c 6964 2c20 6d73 6720  .    valid, msg 
+00001b50: 3d20 7661 6c69 6461 7465 5f74 7970 6528  = validate_type(
+00001b60: 7672 2c20 7661 6c75 652c 2028 7374 722c  vr, value, (str,
+00001b70: 2062 7974 6573 2929 0a20 2020 2069 6620   bytes)).    if 
+00001b80: 6e6f 7420 7661 6c69 643a 0a20 2020 2020  not valid:.     
+00001b90: 2020 2072 6574 7572 6e20 7661 6c69 642c     return valid,
+00001ba0: 206d 7367 0a20 2020 2069 735f 7661 6c69   msg.    is_vali
+00001bb0: 645f 6c65 6e2c 206d 7367 3120 3d20 7661  d_len, msg1 = va
+00001bc0: 6c69 6461 7465 5f76 725f 6c65 6e67 7468  lidate_vr_length
+00001bd0: 2876 722c 2076 616c 7565 290a 2020 2020  (vr, value).    
+00001be0: 6973 5f76 616c 6964 5f65 7870 722c 206d  is_valid_expr, m
+00001bf0: 7367 3220 3d20 7661 6c69 6461 7465 5f72  sg2 = validate_r
+00001c00: 6567 6578 2876 722c 2076 616c 7565 290a  egex(vr, value).
+00001c10: 2020 2020 6d73 6720 3d20 2220 222e 6a6f      msg = " ".jo
+00001c20: 696e 285b 6d73 6731 2c20 6d73 6732 5d29  in([msg1, msg2])
+00001c30: 2e73 7472 6970 2829 0a20 2020 2069 6620  .strip().    if 
+00001c40: 6d73 673a 0a20 2020 2020 2020 206d 7367  msg:.        msg
+00001c50: 202b 3d20 280a 2020 2020 2020 2020 2020   += (.          
+00001c60: 2020 2220 506c 6561 7365 2073 6565 203c    " Please see <
+00001c70: 6874 7470 733a 2f2f 6469 636f 6d2e 6e65  https://dicom.ne
+00001c80: 6d61 2e6f 7267 2f6d 6564 6963 616c 2f64  ma.org/medical/d
+00001c90: 6963 6f6d 2f63 7572 7265 6e74 2f6f 7574  icom/current/out
+00001ca0: 7075 7422 0a20 2020 2020 2020 2020 2020  put".           
+00001cb0: 2022 2f68 746d 6c2f 7061 7274 3035 2e68   "/html/part05.h
+00001cc0: 746d 6c23 7461 626c 655f 362e 322d 313e  tml#table_6.2-1>
+00001cd0: 2066 6f72 2061 6c6c 6f77 6564 2076 616c   for allowed val
+00001ce0: 7565 7320 666f 7220 6561 6368 2056 522e  ues for each VR.
+00001cf0: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
+00001d00: 7265 7475 726e 2069 735f 7661 6c69 645f  return is_valid_
+00001d10: 6c65 6e20 616e 6420 6973 5f76 616c 6964  len and is_valid
+00001d20: 5f65 7870 722c 206d 7367 0a0a 0a64 6566  _expr, msg...def
+00001d30: 2076 616c 6964 6174 655f 706e 5f63 6f6d   validate_pn_com
+00001d40: 706f 6e65 6e74 5f6c 656e 6774 6828 7672  ponent_length(vr
+00001d50: 3a20 7374 722c 2076 616c 7565 3a20 416e  : str, value: An
+00001d60: 7929 202d 3e20 5475 706c 655b 626f 6f6c  y) -> Tuple[bool
+00001d70: 2c20 7374 725d 3a0a 2020 2020 2222 2256  , str]:.    """V
+00001d80: 616c 6964 6174 6520 7468 6520 504e 2063  alidate the PN c
+00001d90: 6f6d 706f 6e65 6e74 2076 616c 7565 2066  omponent value f
+00001da0: 6f72 2074 6865 206d 6178 696d 756d 206c  or the maximum l
+00001db0: 656e 6774 682e 0a0a 2020 2020 5061 7261  ength...    Para
+00001dc0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00001dd0: 2d2d 2d2d 2d0a 2020 2020 7672 203a 2073  -----.    vr : s
+00001de0: 7472 0a20 2020 2020 2020 2049 676e 6f72  tr.        Ignor
+00001df0: 6564 2e0a 2020 2020 7661 6c75 6520 3a20  ed..    value : 
+00001e00: 7374 720a 2020 2020 2020 2020 5468 6520  str.        The 
+00001e10: 7661 6c75 6520 746f 2076 616c 6964 6174  value to validat
+00001e20: 652e 0a0a 2020 2020 5265 7475 726e 730a  e...    Returns.
+00001e30: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00001e40: 2020 2020 4120 7475 706c 6520 6f66 2061      A tuple of a
+00001e50: 2062 6f6f 6c65 616e 2076 616c 6964 6174   boolean validat
+00001e60: 696f 6e20 7265 7375 6c74 2061 6e64 2074  ion result and t
+00001e70: 6865 2065 7272 6f72 206d 6573 7361 6765  he error message
+00001e80: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
+00001e90: 206c 656e 2876 616c 7565 2920 3e20 3634   len(value) > 64
+00001ea0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001eb0: 2046 616c 7365 2c20 280a 2020 2020 2020   False, (.      
+00001ec0: 2020 2020 2020 6622 5468 6520 504e 2063        f"The PN c
+00001ed0: 6f6d 706f 6e65 6e74 206c 656e 6774 6820  omponent length 
+00001ee0: 287b 6c65 6e28 7661 6c75 6529 7d29 2065  ({len(value)}) e
+00001ef0: 7863 6565 6473 2074 6865 2022 0a20 2020  xceeds the ".   
+00001f00: 2020 2020 2020 2020 2066 226d 6178 696d           f"maxim
+00001f10: 756d 2061 6c6c 6f77 6564 206c 656e 6774  um allowed lengt
+00001f20: 6820 6f66 2036 342e 220a 2020 2020 2020  h of 64.".      
+00001f30: 2020 290a 2020 2020 7265 7475 726e 2054    ).    return T
+00001f40: 7275 652c 2022 220a 0a0a 6465 6620 7661  rue, ""...def va
+00001f50: 6c69 6461 7465 5f70 6e28 7672 3a20 7374  lidate_pn(vr: st
+00001f60: 722c 2076 616c 7565 3a20 416e 7929 202d  r, value: Any) -
+00001f70: 3e20 5475 706c 655b 626f 6f6c 2c20 7374  > Tuple[bool, st
+00001f80: 725d 3a0a 2020 2020 2222 2256 616c 6964  r]:.    """Valid
+00001f90: 6174 6520 7468 6520 7661 6c75 6520 666f  ate the value fo
+00001fa0: 7220 5652 2050 4e20 666f 7220 7468 6520  r VR PN for the 
+00001fb0: 6d61 7869 6d75 6d20 6e75 6d62 6572 206f  maximum number o
+00001fc0: 6620 636f 6d70 6f6e 656e 7473 0a20 2020  f components.   
+00001fd0: 2061 6e64 2066 6f72 2074 6865 206d 6178   and for the max
+00001fe0: 696d 756d 206c 656e 6774 6820 6f66 2065  imum length of e
+00001ff0: 6163 6820 636f 6d70 6f6e 656e 742e 0a0a  ach component...
+00002000: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00002010: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00002020: 2020 7672 203a 2073 7472 0a20 2020 2020    vr : str.     
+00002030: 2020 2049 676e 6f72 6564 2e0a 2020 2020     Ignored..    
+00002040: 7661 6c75 6520 3a20 7374 720a 2020 2020  value : str.    
+00002050: 2020 2020 5468 6520 7661 6c75 6520 746f      The value to
+00002060: 2076 616c 6964 6174 652e 0a0a 2020 2020   validate...    
+00002070: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00002080: 2d2d 2d0a 2020 2020 2020 2020 4120 7475  ---.        A tu
+00002090: 706c 6520 6f66 2061 2062 6f6f 6c65 616e  ple of a boolean
+000020a0: 2076 616c 6964 6174 696f 6e20 7265 7375   validation resu
+000020b0: 6c74 2061 6e64 2074 6865 2065 7272 6f72  lt and the error
+000020c0: 206d 6573 7361 6765 2e0a 2020 2020 2222   message..    ""
+000020d0: 220a 2020 2020 6966 206e 6f74 2076 616c  ".    if not val
+000020e0: 7565 206f 7220 6973 696e 7374 616e 6365  ue or isinstance
+000020f0: 2876 616c 7565 2c20 5065 7273 6f6e 4e61  (value, PersonNa
+00002100: 6d65 293a 0a20 2020 2020 2020 2072 6574  me):.        ret
+00002110: 7572 6e20 5472 7565 2c20 2222 0a20 2020  urn True, "".   
+00002120: 2076 616c 6964 2c20 6d73 6720 3d20 7661   valid, msg = va
+00002130: 6c69 6461 7465 5f74 7970 6528 7672 2c20  lidate_type(vr, 
+00002140: 7661 6c75 652c 2028 7374 722c 2062 7974  value, (str, byt
+00002150: 6573 2929 0a20 2020 2069 6620 6e6f 7420  es)).    if not 
+00002160: 7661 6c69 643a 0a20 2020 2020 2020 2072  valid:.        r
+00002170: 6574 7572 6e20 7661 6c69 642c 206d 7367  eturn valid, msg
+00002180: 0a20 2020 2063 6f6d 706f 6e65 6e74 733a  .    components:
+00002190: 2053 6571 7565 6e63 655b 556e 696f 6e5b   Sequence[Union[
+000021a0: 7374 722c 2062 7974 6573 5d5d 0a20 2020  str, bytes]].   
+000021b0: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
+000021c0: 616c 7565 2c20 6279 7465 7329 3a0a 2020  alue, bytes):.  
+000021d0: 2020 2020 2020 636f 6d70 6f6e 656e 7473        components
+000021e0: 203d 2076 616c 7565 2e73 706c 6974 2862   = value.split(b
+000021f0: 223d 2229 0a20 2020 2065 6c73 653a 0a20  "=").    else:. 
+00002200: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+00002210: 7320 3d20 7661 6c75 652e 7370 6c69 7428  s = value.split(
+00002220: 223d 2229 0a20 2020 2069 6620 6c65 6e28  "=").    if len(
+00002230: 636f 6d70 6f6e 656e 7473 2920 3e20 333a  components) > 3:
+00002240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002250: 4661 6c73 652c 2028 0a20 2020 2020 2020  False, (.       
+00002260: 2020 2020 2066 2254 6865 206e 756d 6265       f"The numbe
+00002270: 7220 6f66 2050 4e20 636f 6d70 6f6e 656e  r of PN componen
+00002280: 7473 206c 656e 6774 6820 287b 6c65 6e28  ts length ({len(
+00002290: 636f 6d70 6f6e 656e 7473 297d 2920 6578  components)}) ex
+000022a0: 6365 6564 7320 220a 2020 2020 2020 2020  ceeds ".        
+000022b0: 2020 2020 6622 7468 6520 6d61 7869 6d75      f"the maximu
+000022c0: 6d20 616c 6c6f 7765 6420 6e75 6d62 6572  m allowed number
+000022d0: 206f 6620 332e 220a 2020 2020 2020 2020   of 3.".        
+000022e0: 290a 2020 2020 666f 7220 636f 6d70 2069  ).    for comp i
+000022f0: 6e20 636f 6d70 6f6e 656e 7473 3a0a 2020  n components:.  
+00002300: 2020 2020 2020 7661 6c69 642c 206d 7367        valid, msg
+00002310: 203d 2076 616c 6964 6174 655f 706e 5f63   = validate_pn_c
+00002320: 6f6d 706f 6e65 6e74 5f6c 656e 6774 6828  omponent_length(
+00002330: 2250 4e22 2c20 636f 6d70 290a 2020 2020  "PN", comp).    
+00002340: 2020 2020 6966 206e 6f74 2076 616c 6964      if not valid
+00002350: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00002360: 7475 726e 2046 616c 7365 2c20 6d73 670a  turn False, msg.
+00002370: 2020 2020 7265 7475 726e 2054 7275 652c      return True,
+00002380: 2022 220a 0a0a 6465 6620 7661 6c69 6461   ""...def valida
+00002390: 7465 5f70 6e5f 636f 6d70 6f6e 656e 7428  te_pn_component(
+000023a0: 7661 6c75 653a 2055 6e69 6f6e 5b73 7472  value: Union[str
+000023b0: 2c20 6279 7465 735d 2920 2d3e 204e 6f6e  , bytes]) -> Non
+000023c0: 653a 0a20 2020 2022 2222 5661 6c69 6461  e:.    """Valida
+000023d0: 7465 2074 6865 2076 616c 7565 206f 6620  te the value of 
+000023e0: 6120 7369 6e67 6c65 2063 6f6d 706f 6e65  a single compone
+000023f0: 6e74 206f 6620 5652 2050 4e20 666f 7220  nt of VR PN for 
+00002400: 6d61 7869 6d75 6d20 6c65 6e67 7468 2e0a  maximum length..
+00002410: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00002420: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00002430: 2020 2076 616c 7565 203a 2073 7472 206f     value : str o
+00002440: 7220 6279 7465 730a 2020 2020 2020 2020  r bytes.        
+00002450: 5468 6520 636f 6d70 6f6e 656e 7420 7661  The component va
+00002460: 6c75 6520 746f 2076 616c 6964 6174 652e  lue to validate.
+00002470: 0a0a 2020 2020 5261 6973 6573 0a20 2020  ..    Raises.   
+00002480: 202d 2d2d 2d2d 2d0a 2020 2020 5661 6c75   ------.    Valu
+00002490: 6545 7272 6f72 0a20 2020 2020 2020 2049  eError.        I
+000024a0: 6620 7468 6520 7661 6c69 6461 7469 6f6e  f the validation
+000024b0: 2066 6169 6c73 2061 6e64 2074 6865 2076   fails and the v
+000024c0: 616c 6964 6174 696f 6e20 6d6f 6465 2069  alidation mode i
+000024d0: 7320 7365 7420 746f 0a20 2020 2020 2020  s set to.       
+000024e0: 2060 5241 4953 4560 2e0a 2020 2020 2222   `RAISE`..    ""
+000024f0: 220a 2020 2020 7661 6c69 6461 7465 5f76  ".    validate_v
+00002500: 616c 7565 2822 504e 222c 2076 616c 7565  alue("PN", value
+00002510: 2c20 636f 6e66 6967 2e73 6574 7469 6e67  , config.setting
+00002520: 732e 7772 6974 696e 675f 7661 6c69 6461  s.writing_valida
+00002530: 7469 6f6e 5f6d 6f64 652c 0a20 2020 2020  tion_mode,.     
+00002540: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00002550: 6c69 6461 7465 5f70 6e5f 636f 6d70 6f6e  lidate_pn_compon
+00002560: 656e 745f 6c65 6e67 7468 290a 0a0a 5641  ent_length)...VA
+00002570: 4c55 455f 4c45 4e47 5448 203d 207b 0a20  LUE_LENGTH = {. 
+00002580: 2020 2022 5553 223a 2032 2c0a 2020 2020     "US": 2,.    
+00002590: 2253 5322 3a20 322c 0a20 2020 2022 554c  "SS": 2,.    "UL
+000025a0: 223a 2034 2c0a 2020 2020 2253 4c22 3a20  ": 4,.    "SL": 
+000025b0: 342c 0a20 2020 2022 5556 223a 2038 2c0a  4,.    "UV": 8,.
+000025c0: 2020 2020 2253 5622 3a20 382c 0a20 2020      "SV": 8,.   
+000025d0: 2022 464c 223a 2034 2c0a 2020 2020 2246   "FL": 4,.    "F
+000025e0: 4422 3a20 380a 7d0a 0a0a 6465 6620 7661  D": 8.}...def va
+000025f0: 6c69 6461 7465 5f6e 756d 6265 7228 0a20  lidate_number(. 
+00002600: 2020 2020 2020 2076 723a 2073 7472 2c20         vr: str, 
+00002610: 7661 6c75 653a 2041 6e79 2c20 6d69 6e5f  value: Any, min_
+00002620: 7661 6c75 653a 2069 6e74 2c20 6d61 785f  value: int, max_
+00002630: 7661 6c75 653a 2069 6e74 0a29 202d 3e20  value: int.) -> 
+00002640: 5475 706c 655b 626f 6f6c 2c20 7374 725d  Tuple[bool, str]
+00002650: 3a0a 2020 2020 2222 2256 616c 6964 6174  :.    """Validat
+00002660: 6520 7468 6520 7661 6c75 6520 666f 7220  e the value for 
+00002670: 6120 6e75 6d65 7269 6361 6c20 5652 2066  a numerical VR f
+00002680: 6f72 2074 7970 6520 616e 6420 616c 6c6f  or type and allo
+00002690: 7765 6420 7261 6e67 652e 0a0a 2020 2020  wed range...    
+000026a0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000026b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7672  ---------.    vr
+000026c0: 203a 2073 7472 0a20 2020 2020 2020 2054   : str.        T
+000026d0: 6865 2076 616c 7565 2072 6570 7265 7365  he value represe
+000026e0: 6e74 6174 696f 6e20 746f 2076 616c 6964  ntation to valid
+000026f0: 6174 6520 6167 6169 6e73 742e 0a20 2020  ate against..   
+00002700: 2076 616c 7565 203a 2041 6e79 0a20 2020   value : Any.   
+00002710: 2020 2020 2054 6865 2076 616c 7565 2074       The value t
+00002720: 6f20 7661 6c69 6461 7465 2e0a 2020 2020  o validate..    
+00002730: 6d69 6e5f 7661 6c75 6520 3a20 696e 740a  min_value : int.
+00002740: 2020 2020 2020 2020 5468 6520 6d69 6e69          The mini
+00002750: 6d75 6d20 616c 6c6f 7765 6420 7661 6c75  mum allowed valu
+00002760: 652e 0a20 2020 206d 6178 5f76 616c 7565  e..    max_value
+00002770: 203a 2069 6e74 0a20 2020 2020 2020 2054   : int.        T
+00002780: 6865 206d 6178 696d 756d 2061 6c6c 6f77  he maximum allow
+00002790: 6564 2076 616c 7565 2e0a 0a20 2020 2052  ed value...    R
+000027a0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+000027b0: 2d2d 0a20 2020 2020 2020 2041 2074 7570  --.        A tup
+000027c0: 6c65 206f 6620 6120 626f 6f6c 6561 6e20  le of a boolean 
+000027d0: 7661 6c69 6461 7469 6f6e 2072 6573 756c  validation resul
+000027e0: 7420 616e 6420 7468 6520 6572 726f 7220  t and the error 
+000027f0: 6d65 7373 6167 652e 0a20 2020 2022 2222  message..    """
+00002800: 0a20 2020 2076 616c 6964 2c20 6d73 6720  .    valid, msg 
+00002810: 3d20 7661 6c69 6461 7465 5f74 7970 6528  = validate_type(
+00002820: 7672 2c20 7661 6c75 652c 2028 696e 742c  vr, value, (int,
+00002830: 2062 7974 6573 2929 0a20 2020 2069 6620   bytes)).    if 
+00002840: 6e6f 7420 7661 6c69 643a 0a20 2020 2020  not valid:.     
+00002850: 2020 2072 6574 7572 6e20 7661 6c69 642c     return valid,
+00002860: 206d 7367 0a20 2020 2069 6620 6973 696e   msg.    if isin
+00002870: 7374 616e 6365 2876 616c 7565 2c20 696e  stance(value, in
+00002880: 7429 3a0a 2020 2020 2020 2020 6966 2076  t):.        if v
+00002890: 616c 7565 203c 206d 696e 5f76 616c 7565  alue < min_value
+000028a0: 206f 7220 7661 6c75 6520 3e20 6d61 785f   or value > max_
+000028b0: 7661 6c75 653a 0a20 2020 2020 2020 2020  value:.         
+000028c0: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
+000028d0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+000028e0: 2020 2066 2249 6e76 616c 6964 2076 616c     f"Invalid val
+000028f0: 7565 3a20 6120 7661 6c75 6520 666f 7220  ue: a value for 
+00002900: 6120 7461 6720 7769 7468 2056 5220 7b76  a tag with VR {v
+00002910: 727d 206d 7573 7420 6265 2022 0a20 2020  r} must be ".   
+00002920: 2020 2020 2020 2020 2020 2020 2066 2262               f"b
+00002930: 6574 7765 656e 207b 6d69 6e5f 7661 6c75  etween {min_valu
+00002940: 657d 2061 6e64 207b 6d61 785f 7661 6c75  e} and {max_valu
+00002950: 657d 2e22 0a20 2020 2020 2020 2020 2020  e}.".           
+00002960: 2029 0a20 2020 2065 6c69 6620 6c65 6e28   ).    elif len(
+00002970: 7661 6c75 6529 2025 2056 414c 5545 5f4c  value) % VALUE_L
+00002980: 454e 4754 485b 7672 5d3a 0a20 2020 2020  ENGTH[vr]:.     
+00002990: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
+000029a0: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+000029b0: 2249 6e76 616c 6964 2076 616c 7565 206c  "Invalid value l
+000029c0: 656e 6774 6820 7b6c 656e 2876 616c 7565  ength {len(value
+000029d0: 297d 3a20 7468 6520 7661 6c75 6520 6c65  )}: the value le
+000029e0: 6e67 7468 2066 6f72 2061 2074 6167 2022  ngth for a tag "
+000029f0: 0a20 2020 2020 2020 2020 2020 2066 2277  .            f"w
+00002a00: 6974 6820 5652 207b 7672 7d20 6d75 7374  ith VR {vr} must
+00002a10: 2062 6520 6120 6d75 6c74 6970 6c65 206f   be a multiple o
+00002a20: 6620 7b56 414c 5545 5f4c 454e 4754 485b  f {VALUE_LENGTH[
+00002a30: 7672 5d7d 2e22 0a20 2020 2020 2020 2029  vr]}.".        )
+00002a40: 0a20 2020 2072 6574 7572 6e20 5472 7565  .    return True
+00002a50: 2c20 2222 0a0a 0a56 414c 4944 4154 4f52  , ""...VALIDATOR
+00002a60: 5320 3d20 7b0a 2020 2020 2241 4522 3a20  S = {.    "AE": 
+00002a70: 7661 6c69 6461 7465 5f6c 656e 6774 685f  validate_length_
+00002a80: 616e 645f 7479 7065 5f61 6e64 5f72 6567  and_type_and_reg
+00002a90: 6578 2c0a 2020 2020 2241 5322 3a20 7661  ex,.    "AS": va
+00002aa0: 6c69 6461 7465 5f74 7970 655f 616e 645f  lidate_type_and_
+00002ab0: 7265 6765 782c 0a20 2020 2022 4353 223a  regex,.    "CS":
+00002ac0: 2076 616c 6964 6174 655f 6c65 6e67 7468   validate_length
+00002ad0: 5f61 6e64 5f74 7970 655f 616e 645f 7265  _and_type_and_re
+00002ae0: 6765 782c 0a20 2020 2022 4441 223a 206c  gex,.    "DA": l
+00002af0: 616d 6264 6120 7672 2c20 7661 6c75 653a  ambda vr, value:
+00002b00: 2076 616c 6964 6174 655f 6461 7465 5f74   validate_date_t
+00002b10: 696d 6528 7672 2c20 7661 6c75 652c 2064  ime(vr, value, d
+00002b20: 6174 6574 696d 652e 6461 7465 292c 0a20  atetime.date),. 
+00002b30: 2020 2022 4453 223a 2076 616c 6964 6174     "DS": validat
+00002b40: 655f 6c65 6e67 7468 5f61 6e64 5f74 7970  e_length_and_typ
+00002b50: 655f 616e 645f 7265 6765 782c 0a20 2020  e_and_regex,.   
+00002b60: 2022 4454 223a 206c 616d 6264 6120 7672   "DT": lambda vr
+00002b70: 2c20 7661 6c75 653a 2076 616c 6964 6174  , value: validat
+00002b80: 655f 6461 7465 5f74 696d 6528 7672 2c20  e_date_time(vr, 
+00002b90: 7661 6c75 652c 2064 6174 6574 696d 652e  value, datetime.
+00002ba0: 6461 7465 7469 6d65 292c 0a20 2020 2022  datetime),.    "
+00002bb0: 4644 223a 206c 616d 6264 6120 7672 2c20  FD": lambda vr, 
+00002bc0: 7661 6c75 653a 2076 616c 6964 6174 655f  value: validate_
+00002bd0: 7479 7065 2876 722c 2076 616c 7565 2c20  type(vr, value, 
+00002be0: 2866 6c6f 6174 2c20 696e 7429 292c 0a20  (float, int)),. 
+00002bf0: 2020 2022 464c 223a 206c 616d 6264 6120     "FL": lambda 
+00002c00: 7672 2c20 7661 6c75 653a 2076 616c 6964  vr, value: valid
+00002c10: 6174 655f 7479 7065 2876 722c 2076 616c  ate_type(vr, val
+00002c20: 7565 2c20 2866 6c6f 6174 2c20 696e 7429  ue, (float, int)
+00002c30: 292c 0a20 2020 2022 4953 223a 2076 616c  ),.    "IS": val
+00002c40: 6964 6174 655f 6c65 6e67 7468 5f61 6e64  idate_length_and
+00002c50: 5f74 7970 655f 616e 645f 7265 6765 782c  _type_and_regex,
+00002c60: 0a20 2020 2022 4c4f 223a 2076 616c 6964  .    "LO": valid
+00002c70: 6174 655f 7479 7065 5f61 6e64 5f6c 656e  ate_type_and_len
+00002c80: 6774 682c 0a20 2020 2022 4c54 223a 2076  gth,.    "LT": v
+00002c90: 616c 6964 6174 655f 7479 7065 5f61 6e64  alidate_type_and
+00002ca0: 5f6c 656e 6774 682c 0a20 2020 2022 504e  _length,.    "PN
+00002cb0: 223a 2076 616c 6964 6174 655f 706e 2c0a  ": validate_pn,.
+00002cc0: 2020 2020 2253 4822 3a20 7661 6c69 6461      "SH": valida
+00002cd0: 7465 5f74 7970 655f 616e 645f 6c65 6e67  te_type_and_leng
+00002ce0: 7468 2c0a 2020 2020 2253 4c22 3a20 6c61  th,.    "SL": la
+00002cf0: 6d62 6461 2076 722c 2076 616c 7565 3a20  mbda vr, value: 
+00002d00: 7661 6c69 6461 7465 5f6e 756d 6265 7228  validate_number(
+00002d10: 0a20 2020 2020 2020 2076 722c 2076 616c  .        vr, val
+00002d20: 7565 2c20 2d30 7838 3030 3030 3030 302c  ue, -0x80000000,
+00002d30: 2030 7837 6666 6666 6666 6629 2c0a 2020   0x7fffffff),.  
+00002d40: 2020 2253 5322 3a20 6c61 6d62 6461 2076    "SS": lambda v
+00002d50: 722c 2076 616c 7565 3a20 7661 6c69 6461  r, value: valida
+00002d60: 7465 5f6e 756d 6265 7228 7672 2c20 7661  te_number(vr, va
+00002d70: 6c75 652c 202d 3078 3830 3030 2c20 3078  lue, -0x8000, 0x
+00002d80: 3766 6666 292c 0a20 2020 2022 5354 223a  7fff),.    "ST":
+00002d90: 2076 616c 6964 6174 655f 7479 7065 5f61   validate_type_a
+00002da0: 6e64 5f6c 656e 6774 682c 0a20 2020 2022  nd_length,.    "
+00002db0: 5356 223a 206c 616d 6264 6120 7672 2c20  SV": lambda vr, 
+00002dc0: 7661 6c75 653a 2076 616c 6964 6174 655f  value: validate_
+00002dd0: 6e75 6d62 6572 280a 2020 2020 2020 2020  number(.        
+00002de0: 7672 2c20 7661 6c75 652c 202d 3078 3830  vr, value, -0x80
+00002df0: 3030 3030 3030 3030 3030 3030 3030 2c20  00000000000000, 
+00002e00: 3078 3766 6666 6666 6666 6666 6666 6666  0x7fffffffffffff
+00002e10: 6666 292c 0a20 2020 2022 544d 223a 206c  ff),.    "TM": l
+00002e20: 616d 6264 6120 7672 2c20 7661 6c75 653a  ambda vr, value:
+00002e30: 2076 616c 6964 6174 655f 6461 7465 5f74   validate_date_t
+00002e40: 696d 6528 7672 2c20 7661 6c75 652c 2064  ime(vr, value, d
+00002e50: 6174 6574 696d 652e 7469 6d65 292c 0a20  atetime.time),. 
+00002e60: 2020 2022 5549 223a 2076 616c 6964 6174     "UI": validat
+00002e70: 655f 6c65 6e67 7468 5f61 6e64 5f74 7970  e_length_and_typ
+00002e80: 655f 616e 645f 7265 6765 782c 0a20 2020  e_and_regex,.   
+00002e90: 2022 554c 223a 206c 616d 6264 6120 7672   "UL": lambda vr
+00002ea0: 2c20 7661 6c75 653a 2076 616c 6964 6174  , value: validat
+00002eb0: 655f 6e75 6d62 6572 2876 722c 2076 616c  e_number(vr, val
+00002ec0: 7565 2c20 302c 2030 7866 6666 6666 6666  ue, 0, 0xfffffff
+00002ed0: 6629 2c0a 2020 2020 2255 5322 3a20 6c61  f),.    "US": la
+00002ee0: 6d62 6461 2076 722c 2076 616c 7565 3a20  mbda vr, value: 
+00002ef0: 7661 6c69 6461 7465 5f6e 756d 6265 7228  validate_number(
+00002f00: 7672 2c20 7661 6c75 652c 2030 2c20 3078  vr, value, 0, 0x
+00002f10: 6666 6666 292c 0a20 2020 2022 5552 223a  ffff),.    "UR":
+00002f20: 2076 616c 6964 6174 655f 7479 7065 5f61   validate_type_a
+00002f30: 6e64 5f72 6567 6578 2c0a 2020 2020 2255  nd_regex,.    "U
+00002f40: 5622 3a20 6c61 6d62 6461 2076 722c 2076  V": lambda vr, v
+00002f50: 616c 7565 3a20 7661 6c69 6461 7465 5f6e  alue: validate_n
+00002f60: 756d 6265 7228 7672 2c20 7661 6c75 652c  umber(vr, value,
+00002f70: 2030 2c20 3078 6666 6666 6666 6666 6666   0, 0xffffffffff
+00002f80: 6666 6666 6666 292c 0a7d 0a0a 0a64 6566  ffffff),.}...def
+00002f90: 2076 616c 6964 6174 655f 7661 6c75 6528   validate_value(
+00002fa0: 7672 3a20 7374 722c 2076 616c 7565 3a20  vr: str, value: 
+00002fb0: 416e 792c 0a20 2020 2020 2020 2020 2020  Any,.           
+00002fc0: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
+00002fd0: 6f6e 5f6d 6f64 653a 2069 6e74 2c0a 2020  on_mode: int,.  
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ff0: 2076 616c 6964 6174 6f72 3a20 4f70 7469   validator: Opti
+00003000: 6f6e 616c 5b43 616c 6c61 626c 655b 5b73  onal[Callable[[s
+00003010: 7472 2c20 416e 795d 2c0a 2020 2020 2020  tr, Any],.      
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 2054 7570 6c65 5b62 6f6f 6c2c 2073 7472   Tuple[bool, str
+00003050: 5d5d 5d20 3d20 4e6f 6e65 2920 2d3e 204e  ]]] = None) -> N
+00003060: 6f6e 653a 0a20 2020 2022 2222 5661 6c69  one:.    """Vali
+00003070: 6461 7465 2074 6865 2067 6976 656e 2076  date the given v
+00003080: 616c 7565 2061 6761 696e 7374 2074 6865  alue against the
+00003090: 2044 4943 4f4d 2073 7461 6e64 6172 642e   DICOM standard.
+000030a0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+000030b0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000030c0: 2020 2020 7672 203a 2073 7472 0a20 2020      vr : str.   
+000030d0: 2020 2020 2054 6865 2056 5220 6f66 2074       The VR of t
+000030e0: 6865 2074 6167 2074 6865 2076 616c 7565  he tag the value
+000030f0: 2069 7320 6164 6465 6420 746f 2e0a 2020   is added to..  
+00003100: 2020 7661 6c75 6520 3a20 416e 790a 2020    value : Any.  
+00003110: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
+00003120: 746f 2062 6520 7661 6c69 6461 7465 642e  to be validated.
+00003130: 0a20 2020 2076 616c 6964 6174 696f 6e5f  .    validation_
+00003140: 6d6f 6465 203a 2069 6e74 0a20 2020 2020  mode : int.     
+00003150: 2020 2044 6566 696e 6573 2069 6620 7661     Defines if va
+00003160: 6c75 6573 2061 7265 2076 616c 6964 6174  lues are validat
+00003170: 6564 2061 6e64 2068 6f77 2076 616c 6964  ed and how valid
+00003180: 6174 696f 6e20 6572 726f 7273 2061 7265  ation errors are
+00003190: 0a20 2020 2020 2020 2068 616e 646c 6564  .        handled
+000031a0: 2e0a 2020 2020 7661 6c69 6461 746f 7220  ..    validator 
+000031b0: 3a20 4361 6c6c 6162 6c65 206f 7220 4e6f  : Callable or No
+000031c0: 6e65 0a20 2020 2020 2020 2046 756e 6374  ne.        Funct
+000031d0: 696f 6e20 7468 6174 2064 6f65 7320 7468  ion that does th
+000031e0: 6520 6163 7475 616c 2076 616c 6964 6174  e actual validat
+000031f0: 696f 6e2e 2049 6620 6e6f 7420 6769 7665  ion. If not give
+00003200: 6e2c 0a20 2020 2020 2020 2074 6865 2076  n,.        the v
+00003210: 616c 6964 6174 6f72 2069 7320 7461 6b65  alidator is take
+00003220: 6e20 6672 6f6d 2074 6865 2056 522d 7370  n from the VR-sp
+00003230: 6563 6966 6963 2076 616c 6964 6174 6f72  ecific validator
+00003240: 2074 6162 6c65 2069 6e73 7465 6164 2e0a   table instead..
+00003250: 0a20 2020 2052 6169 7365 730a 2020 2020  .    Raises.    
+00003260: 2d2d 2d2d 2d2d 0a20 2020 2056 616c 7565  ------.    Value
+00003270: 4572 726f 720a 2020 2020 2020 2020 4966  Error.        If
+00003280: 2074 6865 2076 616c 6964 6174 696f 6e20   the validation 
+00003290: 6661 696c 7320 616e 6420 7468 6520 7661  fails and the va
+000032a0: 6c69 6461 7469 6f6e 206d 6f64 6520 6973  lidation mode is
+000032b0: 2073 6574 2074 6f0a 2020 2020 2020 2020   set to.        
+000032c0: 6052 4149 5345 602e 0a20 2020 2022 2222  `RAISE`..    """
+000032d0: 0a20 2020 2069 6620 7661 6c69 6461 7469  .    if validati
+000032e0: 6f6e 5f6d 6f64 6520 3d3d 2063 6f6e 6669  on_mode == confi
+000032f0: 672e 4947 4e4f 5245 3a0a 2020 2020 2020  g.IGNORE:.      
+00003300: 2020 7265 7475 726e 0a0a 2020 2020 6966    return..    if
+00003310: 2076 616c 7565 2069 7320 6e6f 7420 4e6f   value is not No
+00003320: 6e65 3a0a 2020 2020 2020 2020 7661 6c69  ne:.        vali
+00003330: 6461 746f 7220 3d20 7661 6c69 6461 746f  dator = validato
+00003340: 7220 6f72 2056 414c 4944 4154 4f52 532e  r or VALIDATORS.
+00003350: 6765 7428 7672 290a 2020 2020 2020 2020  get(vr).        
+00003360: 6966 2076 616c 6964 6174 6f72 2069 7320  if validator is 
+00003370: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003380: 2020 2020 2020 6973 5f76 616c 6964 2c20        is_valid, 
+00003390: 6d73 6720 3d20 7661 6c69 6461 746f 7228  msg = validator(
+000033a0: 7672 2c20 7661 6c75 6529 0a20 2020 2020  vr, value).     
+000033b0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+000033c0: 5f76 616c 6964 3a0a 2020 2020 2020 2020  _valid:.        
+000033d0: 2020 2020 2020 2020 6966 2076 616c 6964          if valid
+000033e0: 6174 696f 6e5f 6d6f 6465 203d 3d20 636f  ation_mode == co
+000033f0: 6e66 6967 2e52 4149 5345 3a0a 2020 2020  nfig.RAISE:.    
+00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003410: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00003420: 286d 7367 290a 2020 2020 2020 2020 2020  (msg).          
+00003430: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00003440: 6172 6e28 6d73 6729 0a0a 0a40 756e 6971  arn(msg)...@uniq
+00003450: 7565 0a63 6c61 7373 2056 5228 7374 722c  ue.class VR(str,
+00003460: 2045 6e75 6d29 3a0a 2020 2020 2222 2244   Enum):.    """D
+00003470: 4943 4f4d 2044 6174 6120 456c 656d 656e  ICOM Data Elemen
+00003480: 7427 7320 5661 6c75 6520 5265 7072 6573  t's Value Repres
+00003490: 656e 7461 7469 6f6e 2028 5652 2922 2222  entation (VR)"""
+000034a0: 0a20 2020 2023 2053 7461 6e64 6172 6420  .    # Standard 
+000034b0: 5652 7320 6672 6f6d 2054 6162 6c65 2036  VRs from Table 6
+000034c0: 2e32 2d31 2069 6e20 5061 7274 2035 0a20  .2-1 in Part 5. 
+000034d0: 2020 2041 4520 3d20 2241 4522 0a20 2020     AE = "AE".   
+000034e0: 2041 5320 3d20 2241 5322 0a20 2020 2041   AS = "AS".    A
+000034f0: 5420 3d20 2241 5422 0a20 2020 2043 5320  T = "AT".    CS 
+00003500: 3d20 2243 5322 0a20 2020 2044 4120 3d20  = "CS".    DA = 
+00003510: 2244 4122 0a20 2020 2044 5320 3d20 2244  "DA".    DS = "D
+00003520: 5322 0a20 2020 2044 5420 3d20 2244 5422  S".    DT = "DT"
+00003530: 0a20 2020 2046 4420 3d20 2246 4422 0a20  .    FD = "FD". 
+00003540: 2020 2046 4c20 3d20 2246 4c22 0a20 2020     FL = "FL".   
+00003550: 2049 5320 3d20 2249 5322 0a20 2020 204c   IS = "IS".    L
+00003560: 4f20 3d20 224c 4f22 0a20 2020 204c 5420  O = "LO".    LT 
+00003570: 3d20 224c 5422 0a20 2020 204f 4220 3d20  = "LT".    OB = 
+00003580: 224f 4222 0a20 2020 204f 4420 3d20 224f  "OB".    OD = "O
+00003590: 4422 0a20 2020 204f 4620 3d20 224f 4622  D".    OF = "OF"
+000035a0: 0a20 2020 204f 4c20 3d20 224f 4c22 0a20  .    OL = "OL". 
+000035b0: 2020 204f 5720 3d20 224f 5722 0a20 2020     OW = "OW".   
+000035c0: 204f 5620 3d20 224f 5622 0a20 2020 2050   OV = "OV".    P
+000035d0: 4e20 3d20 2250 4e22 0a20 2020 2053 4820  N = "PN".    SH 
+000035e0: 3d20 2253 4822 0a20 2020 2053 4c20 3d20  = "SH".    SL = 
+000035f0: 2253 4c22 0a20 2020 2053 5120 3d20 2253  "SL".    SQ = "S
+00003600: 5122 0a20 2020 2053 5320 3d20 2253 5322  Q".    SS = "SS"
+00003610: 0a20 2020 2053 5420 3d20 2253 5422 0a20  .    ST = "ST". 
+00003620: 2020 2053 5620 3d20 2253 5622 0a20 2020     SV = "SV".   
+00003630: 2054 4d20 3d20 2254 4d22 0a20 2020 2055   TM = "TM".    U
+00003640: 4320 3d20 2255 4322 0a20 2020 2055 4920  C = "UC".    UI 
+00003650: 3d20 2255 4922 0a20 2020 2055 4c20 3d20  = "UI".    UL = 
+00003660: 2255 4c22 0a20 2020 2055 4e20 3d20 2255  "UL".    UN = "U
+00003670: 4e22 0a20 2020 2055 5220 3d20 2255 5222  N".    UR = "UR"
+00003680: 0a20 2020 2055 5320 3d20 2255 5322 0a20  .    US = "US". 
+00003690: 2020 2055 5420 3d20 2255 5422 0a20 2020     UT = "UT".   
+000036a0: 2055 5620 3d20 2255 5622 0a20 2020 2023   UV = "UV".    #
+000036b0: 2041 6d62 6967 756f 7573 2056 5273 2066   Ambiguous VRs f
+000036c0: 726f 6d20 5461 626c 6573 2036 2d31 2c20  rom Tables 6-1, 
+000036d0: 372d 3120 616e 6420 382d 3120 696e 2050  7-1 and 8-1 in P
+000036e0: 6172 7420 360a 2020 2020 5553 5f53 535f  art 6.    US_SS_
+000036f0: 4f57 203d 2022 5553 206f 7220 5353 206f  OW = "US or SS o
+00003700: 7220 4f57 220a 2020 2020 5553 5f53 5320  r OW".    US_SS 
+00003710: 3d20 2255 5320 6f72 2053 5322 0a20 2020  = "US or SS".   
+00003720: 2055 535f 4f57 203d 2022 5553 206f 7220   US_OW = "US or 
+00003730: 4f57 220a 2020 2020 4f42 5f4f 5720 3d20  OW".    OB_OW = 
+00003740: 224f 4220 6f72 204f 5722 0a0a 0a23 2053  "OB or OW"...# S
+00003750: 7461 6e64 6172 6420 5652 7320 6672 6f6d  tandard VRs from
+00003760: 2054 6162 6c65 2036 2e32 2d31 2069 6e20   Table 6.2-1 in 
+00003770: 5061 7274 2035 0a53 5441 4e44 4152 445f  Part 5.STANDARD_
+00003780: 5652 203d 207b 0a20 2020 2056 522e 4145  VR = {.    VR.AE
+00003790: 2c20 5652 2e41 532c 2056 522e 4154 2c20  , VR.AS, VR.AT, 
+000037a0: 5652 2e43 532c 2056 522e 4441 2c20 5652  VR.CS, VR.DA, VR
+000037b0: 2e44 532c 2056 522e 4454 2c20 5652 2e46  .DS, VR.DT, VR.F
+000037c0: 442c 2056 522e 464c 2c20 5652 2e49 532c  D, VR.FL, VR.IS,
+000037d0: 0a20 2020 2056 522e 4c4f 2c20 5652 2e4c  .    VR.LO, VR.L
+000037e0: 542c 2056 522e 4f42 2c20 5652 2e4f 442c  T, VR.OB, VR.OD,
+000037f0: 2056 522e 4f46 2c20 5652 2e4f 4c2c 2056   VR.OF, VR.OL, V
+00003800: 522e 4f57 2c20 5652 2e4f 562c 2056 522e  R.OW, VR.OV, VR.
+00003810: 504e 2c20 5652 2e53 482c 0a20 2020 2056  PN, VR.SH,.    V
+00003820: 522e 534c 2c20 5652 2e53 512c 2056 522e  R.SL, VR.SQ, VR.
+00003830: 5353 2c20 5652 2e53 542c 2056 522e 5356  SS, VR.ST, VR.SV
+00003840: 2c20 5652 2e54 4d2c 2056 522e 5543 2c20  , VR.TM, VR.UC, 
+00003850: 5652 2e55 492c 2056 522e 554c 2c20 5652  VR.UI, VR.UL, VR
+00003860: 2e55 4e2c 0a20 2020 2056 522e 5552 2c20  .UN,.    VR.UR, 
+00003870: 5652 2e55 532c 2056 522e 5554 2c20 5652  VR.US, VR.UT, VR
+00003880: 2e55 562c 0a7d 0a23 2041 6d62 6967 756f  .UV,.}.# Ambiguo
+00003890: 7573 2056 5273 2066 726f 6d20 5461 626c  us VRs from Tabl
+000038a0: 6573 2036 2d31 2c20 372d 3120 616e 6420  es 6-1, 7-1 and 
+000038b0: 382d 3120 696e 2050 6172 7420 360a 414d  8-1 in Part 6.AM
+000038c0: 4249 4755 4f55 535f 5652 203d 207b 5652  BIGUOUS_VR = {VR
+000038d0: 2e55 535f 5353 5f4f 572c 2056 522e 5553  .US_SS_OW, VR.US
+000038e0: 5f53 532c 2056 522e 5553 5f4f 572c 2056  _SS, VR.US_OW, V
+000038f0: 522e 4f42 5f4f 577d 0a0a 2320 4368 6172  R.OB_OW}..# Char
+00003900: 6163 7465 7220 5265 7065 7274 6f69 7265  acter Repertoire
+00003910: 2066 6f72 2056 5273 0a23 2041 6c6c 6f77   for VRs.# Allow
+00003920: 6564 2063 6861 7261 6374 6572 2072 6570  ed character rep
+00003930: 6572 746f 6972 6520 666f 7220 7374 722d  ertoire for str-
+00003940: 6c69 6b65 2056 5273 2c20 6261 7365 6420  like VRs, based 
+00003950: 6f66 6620 6f66 2074 6865 2069 6e66 6f72  off of the infor
+00003960: 6d61 7469 6f6e 0a23 2020 2069 6e20 5365  mation.#   in Se
+00003970: 6374 696f 6e20 362e 312e 3220 616e 6420  ction 6.1.2 and 
+00003980: 5461 626c 6520 362e 322d 3120 696e 2050  Table 6.2-1 in P
+00003990: 6172 7420 350a 2320 4261 7369 6320 4730  art 5.# Basic G0
+000039a0: 2073 6574 206f 6620 4953 4f20 3634 3620   set of ISO 646 
+000039b0: 2849 534f 2d49 5220 3629 206f 6e6c 790a  (ISO-IR 6) only.
+000039c0: 4445 4641 554c 545f 4348 4152 5345 545f  DEFAULT_CHARSET_
+000039d0: 5652 203d 207b 0a20 2020 2056 522e 4145  VR = {.    VR.AE
+000039e0: 2c20 5652 2e41 532c 2056 522e 4353 2c20  , VR.AS, VR.CS, 
+000039f0: 5652 2e44 412c 2056 522e 4453 2c20 5652  VR.DA, VR.DS, VR
+00003a00: 2e44 542c 2056 522e 4953 2c20 5652 2e54  .DT, VR.IS, VR.T
+00003a10: 4d2c 2056 522e 5549 2c20 5652 2e55 520a  M, VR.UI, VR.UR.
+00003a20: 7d0a 2320 4261 7369 6320 4730 2073 6574  }.# Basic G0 set
+00003a30: 206f 6620 4953 4f20 3634 3620 6f72 2065   of ISO 646 or e
+00003a40: 7874 656e 7369 626c 652f 7265 706c 6163  xtensible/replac
+00003a50: 6561 626c 6520 6279 0a23 2020 2028 3030  eable by.#   (00
+00003a60: 3038 2c30 3030 3529 202a 5370 6563 6966  08,0005) *Specif
+00003a70: 6963 2043 6861 7261 6374 6572 2053 6574  ic Character Set
+00003a80: 2a0a 4355 5354 4f4d 495a 4142 4c45 5f43  *.CUSTOMIZABLE_C
+00003a90: 4841 5253 4554 5f56 5220 3d20 7b56 522e  HARSET_VR = {VR.
+00003aa0: 4c4f 2c20 5652 2e4c 542c 2056 522e 504e  LO, VR.LT, VR.PN
+00003ab0: 2c20 5652 2e53 482c 2056 522e 5354 2c20  , VR.SH, VR.ST, 
+00003ac0: 5652 2e55 432c 2056 522e 5554 7d0a 0a23  VR.UC, VR.UT}..#
+00003ad0: 2043 6f72 7265 7370 6f6e 6469 6e67 2050   Corresponding P
+00003ae0: 7974 686f 6e20 6275 696c 742d 696e 2066  ython built-in f
+00003af0: 6f72 2065 6163 6820 5652 0a23 2020 2046  or each VR.#   F
+00003b00: 6f72 2073 6f6d 6520 5652 7320 7468 6973  or some VRs this
+00003b10: 2069 7320 6d6f 7265 2061 2022 6661 6c6c   is more a "fall
+00003b20: 6261 636b 2220 636c 6173 732d 6c69 6b65  back" class-like
+00003b30: 2062 6568 6176 696f 7572 616c 2064 6566   behavioural def
+00003b40: 696e 6974 696f 6e0a 2320 2020 7468 616e  inition.#   than
+00003b50: 2061 6374 7561 6c2c 2061 6e64 206e 6f74   actual, and not
+00003b60: 6520 7468 6174 2073 6f6d 6520 5652 7320  e that some VRs 
+00003b70: 7375 6368 2061 7320 4953 2061 6e64 2044  such as IS and D
+00003b80: 5320 6172 6520 7072 6573 656e 7420 696e  S are present in
+00003b90: 0a23 2020 206d 756c 7469 706c 6520 7365  .#   multiple se
+00003ba0: 7473 0a42 5954 4553 5f56 5220 3d20 7b56  ts.BYTES_VR = {V
+00003bb0: 522e 4f42 2c20 5652 2e4f 442c 2056 522e  R.OB, VR.OD, VR.
+00003bc0: 4f46 2c20 5652 2e4f 4c2c 2056 522e 4f56  OF, VR.OL, VR.OV
+00003bd0: 2c20 5652 2e4f 572c 2056 522e 554e 7d0a  , VR.OW, VR.UN}.
+00003be0: 464c 4f41 545f 5652 203d 207b 5652 2e44  FLOAT_VR = {VR.D
+00003bf0: 532c 2056 522e 4644 2c20 5652 2e46 4c7d  S, VR.FD, VR.FL}
+00003c00: 0a49 4e54 5f56 5220 3d20 7b56 522e 4154  .INT_VR = {VR.AT
+00003c10: 2c20 5652 2e49 532c 2056 522e 534c 2c20  , VR.IS, VR.SL, 
+00003c20: 5652 2e53 532c 2056 522e 5356 2c20 5652  VR.SS, VR.SV, VR
+00003c30: 2e55 4c2c 2056 522e 5553 2c20 5652 2e55  .UL, VR.US, VR.U
+00003c40: 567d 0a4c 4953 545f 5652 203d 207b 5652  V}.LIST_VR = {VR
+00003c50: 2e53 517d 0a53 5452 5f56 5220 3d20 4445  .SQ}.STR_VR = DE
+00003c60: 4641 554c 545f 4348 4152 5345 545f 5652  FAULT_CHARSET_VR
+00003c70: 207c 2043 5553 544f 4d49 5a41 424c 455f   | CUSTOMIZABLE_
+00003c80: 4348 4152 5345 545f 5652 0a0a 2320 5468  CHARSET_VR..# Th
+00003c90: 6573 6520 5652 7320 6d61 7920 6861 7665  ese VRs may have
+00003ca0: 2062 6163 6b73 6c61 7368 2063 6861 7261   backslash chara
+00003cb0: 6374 6572 7320 6f72 2065 6e63 6f64 6564  cters or encoded
+00003cc0: 2062 6163 6b73 6c61 7368 6573 2069 6e20   backslashes in 
+00003cd0: 7468 650a 2320 2020 7661 6c75 6520 6261  the.#   value ba
+00003ce0: 7365 6420 6f66 6620 6f66 2074 6865 2069  sed off of the i
+00003cf0: 6e66 6f72 6d61 7469 6f6e 2069 6e20 5461  nformation in Ta
+00003d00: 626c 6520 362e 322d 3120 696e 2050 6172  ble 6.2-1 in Par
+00003d10: 7420 350a 2320 4461 7461 456c 656d 656e  t 5.# DataElemen
+00003d20: 7473 2077 6974 6820 616d 6269 6775 6f75  ts with ambiguou
+00003d30: 7320 5652 7320 6d61 7920 7573 6520 6062  s VRs may use `b
+00003d40: 7974 6573 6020 7661 6c75 6573 2061 6e64  ytes` values and
+00003d50: 2073 6f20 6172 6520 616c 6c6f 7765 640a   so are allowed.
+00003d60: 2320 2020 746f 2068 6176 6520 6261 636b  #   to have back
+00003d70: 736c 6173 6865 7320 2865 7863 6570 7420  slashes (except 
+00003d80: 2755 5320 6f72 2053 5327 290a 414c 4c4f  'US or SS').ALLO
+00003d90: 575f 4241 434b 534c 4153 4820 3d20 280a  W_BACKSLASH = (.
+00003da0: 2020 2020 7b56 522e 4c54 2c20 5652 2e53      {VR.LT, VR.S
+00003db0: 542c 2056 522e 5554 2c20 5652 2e55 535f  T, VR.UT, VR.US_
+00003dc0: 5353 5f4f 572c 2056 522e 5553 5f4f 572c  SS_OW, VR.US_OW,
+00003dd0: 2056 522e 4f42 5f4f 577d 207c 2042 5954   VR.OB_OW} | BYT
+00003de0: 4553 5f56 520a 290a 0a23 2056 5273 2077  ES_VR.)..# VRs w
+00003df0: 6869 6368 206d 6179 2068 6176 6520 6120  hich may have a 
+00003e00: 7661 6c75 6520 6d6f 7265 2074 6861 6e20  value more than 
+00003e10: 3130 3234 2062 7974 6573 206f 7220 6368  1024 bytes or ch
+00003e20: 6172 6163 7465 7273 206c 6f6e 670a 2320  aracters long.# 
+00003e30: 2020 5573 6564 2074 6f20 666c 6167 2077    Used to flag w
+00003e40: 6869 6368 2076 616c 7565 7320 6d61 7920  hich values may 
+00003e50: 6e65 6564 2073 686f 7274 656e 696e 6720  need shortening 
+00003e60: 6475 7269 6e67 2070 7269 6e74 696e 670a  during printing.
+00003e70: 4c4f 4e47 5f56 414c 5545 5f56 5220 3d20  LONG_VALUE_VR = 
+00003e80: 7b56 522e 4c54 2c20 5652 2e55 432c 2056  {VR.LT, VR.UC, V
+00003e90: 522e 5554 7d20 7c20 4259 5445 535f 5652  R.UT} | BYTES_VR
+00003ea0: 207c 2041 4d42 4947 554f 5553 5f56 520a   | AMBIGUOUS_VR.
+00003eb0: 0a23 2056 5273 2074 6861 7420 7573 6520  .# VRs that use 
+00003ec0: 3220 6279 7465 206c 656e 6774 6820 6669  2 byte length fi
+00003ed0: 656c 6473 2066 6f72 2045 7870 6c69 6369  elds for Explici
+00003ee0: 7420 5652 2066 726f 6d20 5461 626c 6520  t VR from Table 
+00003ef0: 372e 312d 3220 696e 2050 6172 7420 350a  7.1-2 in Part 5.
+00003f00: 2320 2020 416c 6c20 6f74 6865 7220 6578  #   All other ex
+00003f10: 706c 6963 6974 2056 5273 2061 6e64 2061  plicit VRs and a
+00003f20: 6c6c 2069 6d70 6c69 6369 7420 5652 7320  ll implicit VRs 
+00003f30: 7573 6520 3420 6279 7465 206c 656e 6774  use 4 byte lengt
+00003f40: 6820 6669 656c 6473 0a45 5850 4c49 4349  h fields.EXPLICI
+00003f50: 545f 5652 5f4c 454e 4754 485f 3136 203d  T_VR_LENGTH_16 =
+00003f60: 207b 0a20 2020 2056 522e 4145 2c20 5652   {.    VR.AE, VR
+00003f70: 2e41 532c 2056 522e 4154 2c20 5652 2e43  .AS, VR.AT, VR.C
+00003f80: 532c 2056 522e 4441 2c20 5652 2e44 532c  S, VR.DA, VR.DS,
+00003f90: 2056 522e 4454 2c20 5652 2e46 4c2c 2056   VR.DT, VR.FL, V
+00003fa0: 522e 4644 2c20 5652 2e49 532c 0a20 2020  R.FD, VR.IS,.   
+00003fb0: 2056 522e 4c4f 2c20 5652 2e4c 542c 2056   VR.LO, VR.LT, V
+00003fc0: 522e 504e 2c20 5652 2e53 482c 2056 522e  R.PN, VR.SH, VR.
+00003fd0: 534c 2c20 5652 2e53 532c 2056 522e 5354  SL, VR.SS, VR.ST
+00003fe0: 2c20 5652 2e54 4d2c 2056 522e 5549 2c20  , VR.TM, VR.UI, 
+00003ff0: 5652 2e55 4c2c 0a20 2020 2056 522e 5553  VR.UL,.    VR.US
+00004000: 2c0a 7d0a 4558 504c 4943 4954 5f56 525f  ,.}.EXPLICIT_VR_
+00004010: 4c45 4e47 5448 5f33 3220 3d20 5354 414e  LENGTH_32 = STAN
+00004020: 4441 5244 5f56 5220 2d20 4558 504c 4943  DARD_VR - EXPLIC
+00004030: 4954 5f56 525f 4c45 4e47 5448 5f31 360a  IT_VR_LENGTH_16.
+00004040: 0a0a 636c 6173 7320 5f44 6174 6554 696d  ..class _DateTim
+00004050: 6542 6173 653a 0a20 2020 2022 2222 4261  eBase:.    """Ba
+00004060: 7365 2063 6c61 7373 2066 6f72 2044 542c  se class for DT,
+00004070: 2044 4120 616e 6420 544d 2065 6c65 6d65   DA and TM eleme
+00004080: 6e74 2073 7562 2d63 6c61 7373 6573 2e22  nt sub-classes."
+00004090: 2222 0a20 2020 206f 7269 6769 6e61 6c5f  "".    original_
+000040a0: 7374 7269 6e67 3a20 7374 720a 0a20 2020  string: str..   
+000040b0: 2023 2041 6464 2070 6963 6b6c 696e 6720   # Add pickling 
+000040c0: 7375 7070 6f72 7420 666f 7220 7468 6520  support for the 
+000040d0: 6d75 7461 626c 6520 6164 6469 7469 6f6e  mutable addition
+000040e0: 730a 2020 2020 6465 6620 5f5f 6765 7473  s.    def __gets
+000040f0: 7461 7465 5f5f 2873 656c 6629 202d 3e20  tate__(self) -> 
+00004100: 4469 6374 5b73 7472 2c20 416e 795d 3a0a  Dict[str, Any]:.
+00004110: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00004120: 656c 662e 5f5f 6469 6374 5f5f 2e63 6f70  elf.__dict__.cop
+00004130: 7928 290a 0a20 2020 2064 6566 205f 5f73  y()..    def __s
+00004140: 6574 7374 6174 655f 5f28 7365 6c66 2c20  etstate__(self, 
+00004150: 7374 6174 653a 2044 6963 745b 7374 722c  state: Dict[str,
+00004160: 2041 6e79 5d29 202d 3e20 4e6f 6e65 3a0a   Any]) -> None:.
+00004170: 2020 2020 2020 2020 7365 6c66 2e5f 5f64          self.__d
+00004180: 6963 745f 5f2e 7570 6461 7465 2873 7461  ict__.update(sta
+00004190: 7465 290a 0a20 2020 2064 6566 205f 5f72  te)..    def __r
+000041a0: 6564 7563 655f 6578 5f5f 2820 2023 2074  educe_ex__(  # t
+000041b0: 7970 653a 2069 676e 6f72 655b 6f76 6572  ype: ignore[over
+000041c0: 7269 6465 5d0a 2020 2020 2020 2020 7365  ride].        se
+000041d0: 6c66 2c20 7072 6f74 6f63 6f6c 3a20 696e  lf, protocol: in
+000041e0: 740a 2020 2020 2920 2d3e 2054 7570 6c65  t.    ) -> Tuple
+000041f0: 5b41 6e79 2c20 2e2e 2e5d 3a0a 2020 2020  [Any, ...]:.    
+00004200: 2020 2020 2320 5079 7468 6f6e 2033 2e38      # Python 3.8
+00004210: 202d 2070 726f 746f 636f 6c3a 2053 7570   - protocol: Sup
+00004220: 706f 7274 7349 6e64 6578 2028 6164 6465  portsIndex (adde
+00004230: 6420 696e 2033 2e38 290a 2020 2020 2020  d in 3.8).      
+00004240: 2020 2320 6461 7465 7469 6d65 2e74 696d    # datetime.tim
+00004250: 652c 2061 6e64 2064 6174 6574 696d 652e  e, and datetime.
+00004260: 6461 7465 7469 6d65 2072 6574 7572 6e20  datetime return 
+00004270: 5475 706c 655b 416e 792c 202e 2e2e 5d0a  Tuple[Any, ...].
+00004280: 2020 2020 2020 2020 2320 6461 7465 7469          # dateti
+00004290: 6d65 2e64 6174 6520 646f 6573 6e27 7420  me.date doesn't 
+000042a0: 6465 6669 6e65 205f 5f72 6564 7563 655f  define __reduce_
+000042b0: 6578 5f5f 0a20 2020 2020 2020 2072 6564  ex__.        red
+000042c0: 7563 655f 6578 203d 2063 6173 7428 5475  uce_ex = cast(Tu
+000042d0: 706c 655b 416e 792c 202e 2e2e 5d2c 2073  ple[Any, ...], s
+000042e0: 7570 6572 2829 2e5f 5f72 6564 7563 655f  uper().__reduce_
+000042f0: 6578 5f5f 2870 726f 746f 636f 6c29 290a  ex__(protocol)).
+00004300: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00004310: 6564 7563 655f 6578 202b 2028 7365 6c66  educe_ex + (self
+00004320: 2e5f 5f67 6574 7374 6174 655f 5f28 292c  .__getstate__(),
+00004330: 290a 0a20 2020 2064 6566 205f 5f73 7472  )..    def __str
+00004340: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
+00004350: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
+00004360: 7474 7228 7365 6c66 2c20 276f 7269 6769  ttr(self, 'origi
+00004370: 6e61 6c5f 7374 7269 6e67 2729 3a0a 2020  nal_string'):.  
+00004380: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00004390: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
+000043a0: 7472 696e 670a 0a20 2020 2020 2020 2072  tring..        r
+000043b0: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
+000043c0: 7374 725f 5f28 290a 0a20 2020 2064 6566  str__()..    def
+000043d0: 205f 5f72 6570 725f 5f28 7365 6c66 2920   __repr__(self) 
+000043e0: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+000043f0: 7265 7475 726e 2066 2722 7b73 7472 2873  return f'"{str(s
+00004400: 656c 6629 7d22 270a 0a0a 636c 6173 7320  elf)}"'...class 
+00004410: 4441 285f 4461 7465 5469 6d65 4261 7365  DA(_DateTimeBase
+00004420: 2c20 6461 7465 7469 6d65 2e64 6174 6529  , datetime.date)
+00004430: 3a0a 2020 2020 2222 2253 746f 7265 2076  :.    """Store v
+00004440: 616c 7565 2066 6f72 2061 6e20 656c 656d  alue for an elem
+00004450: 656e 7420 7769 7468 2056 5220 2a2a 4441  ent with VR **DA
+00004460: 2a2a 2061 7320 3a63 6c61 7373 3a60 6461  ** as :class:`da
+00004470: 7465 7469 6d65 2e64 6174 6560 2e0a 0a20  tetime.date`... 
+00004480: 2020 204e 6f74 6520 7468 6174 2074 6865     Note that the
+00004490: 203a 636c 6173 733a 6064 6174 6574 696d   :class:`datetim
+000044a0: 652e 6461 7465 6020 6261 7365 2063 6c61  e.date` base cla
+000044b0: 7373 2069 7320 696d 6d75 7461 626c 652e  ss is immutable.
+000044c0: 0a20 2020 2022 2222 0a20 2020 2064 6566  .    """.    def
+000044d0: 205f 5f6e 6577 5f5f 2820 2023 2074 7970   __new__(  # typ
+000044e0: 653a 2069 676e 6f72 655b 6d69 7363 5d0a  e: ignore[misc].
+000044f0: 2020 2020 2020 2020 636c 733a 2054 7970          cls: Typ
+00004500: 655b 2244 4122 5d2c 202a 6172 6773 3a20  e["DA"], *args: 
+00004510: 416e 792c 202a 2a6b 7761 7267 733a 2041  Any, **kwargs: A
+00004520: 6e79 0a20 2020 2029 202d 3e20 4f70 7469  ny.    ) -> Opti
+00004530: 6f6e 616c 5b22 4441 225d 3a0a 2020 2020  onal["DA"]:.    
+00004540: 2020 2020 2222 2243 7265 6174 6520 616e      """Create an
+00004550: 2069 6e73 7461 6e63 6520 6f66 2044 4120   instance of DA 
+00004560: 6f62 6a65 6374 2e0a 0a20 2020 2020 2020  object...       
+00004570: 2052 6169 7365 2061 6e20 6578 6365 7074   Raise an except
+00004580: 696f 6e20 6966 2074 6865 2073 7472 696e  ion if the strin
+00004590: 6720 6361 6e6e 6f74 2062 6520 7061 7273  g cannot be pars
+000045a0: 6564 206f 7220 7468 6520 6172 6775 6d65  ed or the argume
+000045b0: 6e74 0a20 2020 2020 2020 2069 7320 6f74  nt.        is ot
+000045c0: 6865 7277 6973 6520 696e 636f 6d70 6174  herwise incompat
+000045d0: 6962 6c65 2e0a 0a20 2020 2020 2020 2054  ible...        T
+000045e0: 6865 2061 7267 756d 656e 7473 2028 6060  he arguments (``
+000045f0: 2a61 7267 7360 6020 616e 6420 6060 2a2a  *args`` and ``**
+00004600: 6b77 6172 6773 6060 2920 6172 6520 6569  kwargs``) are ei
+00004610: 7468 6572 2074 6865 206f 6e65 730a 2020  ther the ones.  
+00004620: 2020 2020 2020 696e 6865 7269 7465 6420        inherited 
+00004630: 6672 6f6d 203a 636c 6173 733a 6064 6174  from :class:`dat
+00004640: 6574 696d 652e 6461 7465 602c 206f 7220  etime.date`, or 
+00004650: 7468 6520 6669 7273 7420 6172 6775 6d65  the first argume
+00004660: 6e74 2069 730a 2020 2020 2020 2020 6120  nt is.        a 
+00004670: 7374 7269 6e67 2063 6f6e 666f 726d 616e  string conforman
+00004680: 7420 746f 2074 6865 2044 4120 6465 6669  t to the DA defi
+00004690: 6e69 7469 6f6e 2069 6e20 7468 6520 4449  nition in the DI
+000046a0: 434f 4d20 5374 616e 6461 7264 2c0a 2020  COM Standard,.  
+000046b0: 2020 2020 2020 5061 7274 2035 2c20 3a64        Part 5, :d
+000046c0: 636d 3a60 5461 626c 6520 362e 322d 313c  cm:`Table 6.2-1<
+000046d0: 7061 7274 3035 2f73 6563 745f 362e 322e  part05/sect_6.2.
+000046e0: 6874 6d6c 2374 6162 6c65 5f36 2e32 2d31  html#table_6.2-1
+000046f0: 3e60 2c0a 2020 2020 2020 2020 6f72 2069  >`,.        or i
+00004700: 7420 6973 2061 203a 636c 6173 733a 6064  t is a :class:`d
+00004710: 6174 6574 696d 652e 6461 7465 6020 6f62  atetime.date` ob
+00004720: 6a65 6374 2c20 6f72 2061 6e20 6f62 6a65  ject, or an obje
+00004730: 6374 206f 6620 7479 7065 0a20 2020 2020  ct of type.     
+00004740: 2020 203a 636c 6173 733a 607e 7079 6469     :class:`~pydi
+00004750: 636f 6d2e 7661 6c75 6572 6570 2e44 4160  com.valuerep.DA`
+00004760: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00004770: 2020 2020 2020 6966 206e 6f74 2061 7267        if not arg
+00004780: 7320 6f72 2061 7267 735b 305d 2069 7320  s or args[0] is 
+00004790: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000047a0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+000047b0: 2020 2020 2020 2076 616c 203d 2061 7267         val = arg
+000047c0: 735b 305d 0a20 2020 2020 2020 2069 6620  s[0].        if 
+000047d0: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
+000047e0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+000047f0: 2020 6966 2076 616c 2e73 7472 6970 2829    if val.strip()
+00004800: 203d 3d20 2727 3a0a 2020 2020 2020 2020   == '':.        
+00004810: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00004820: 6f6e 6520 2023 2065 6d70 7479 2064 6174  one  # empty dat
+00004830: 650a 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00004840: 6620 6c65 6e28 7661 6c29 203d 3d20 383a  f len(val) == 8:
+00004850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004860: 2079 6561 7220 3d20 696e 7428 7661 6c5b   year = int(val[
+00004870: 303a 345d 290a 2020 2020 2020 2020 2020  0:4]).          
+00004880: 2020 2020 2020 6d6f 6e74 6820 3d20 696e        month = in
+00004890: 7428 7661 6c5b 343a 365d 290a 2020 2020  t(val[4:6]).    
+000048a0: 2020 2020 2020 2020 2020 2020 6461 7920              day 
+000048b0: 3d20 696e 7428 7661 6c5b 363a 385d 290a  = int(val[6:8]).
+000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048d0: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
+000048e0: 5f6e 6577 5f5f 2863 6c73 2c20 7965 6172  _new__(cls, year
+000048f0: 2c20 6d6f 6e74 682c 2064 6179 290a 0a20  , month, day).. 
+00004900: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00004910: 6e28 7661 6c29 203d 3d20 3130 2061 6e64  n(val) == 10 and
+00004920: 2076 616c 5b34 5d20 3d3d 2027 2e27 2061   val[4] == '.' a
+00004930: 6e64 2076 616c 5b37 5d20 3d3d 2027 2e27  nd val[7] == '.'
+00004940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004950: 2020 2320 4143 522d 4e45 4d41 2053 7461    # ACR-NEMA Sta
+00004960: 6e64 6172 6420 3330 302c 2070 7265 6465  ndard 300, prede
+00004970: 6365 7373 6f72 2074 6f20 4449 434f 4d0a  cessor to DICOM.
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2320 666f 7220 636f 6d70 6174 6962 696c  # for compatibil
+000049a0: 6974 7920 7769 7468 2061 2066 6577 206f  ity with a few o
+000049b0: 6c64 2070 7964 6963 6f6d 2065 7861 6d70  ld pydicom examp
+000049c0: 6c65 2066 696c 6573 0a20 2020 2020 2020  le files.       
+000049d0: 2020 2020 2020 2020 2079 6561 7220 3d20           year = 
+000049e0: 696e 7428 7661 6c5b 303a 345d 290a 2020  int(val[0:4]).  
+000049f0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00004a00: 6e74 6820 3d20 696e 7428 7661 6c5b 353a  nth = int(val[5:
+00004a10: 375d 290a 2020 2020 2020 2020 2020 2020  7]).            
+00004a20: 2020 2020 6461 7920 3d20 696e 7428 7661      day = int(va
+00004a30: 6c5b 383a 3130 5d29 0a20 2020 2020 2020  l[8:10]).       
+00004a40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004a50: 7375 7065 7228 292e 5f5f 6e65 775f 5f28  super().__new__(
+00004a60: 636c 732c 2079 6561 722c 206d 6f6e 7468  cls, year, month
+00004a70: 2c20 6461 7929 0a0a 2020 2020 2020 2020  , day)..        
+00004a80: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
+00004a90: 6c2c 2064 6174 6574 696d 652e 6461 7465  l, datetime.date
+00004aa0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00004ab0: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
+00004ac0: 6e65 775f 5f28 636c 732c 2076 616c 2e79  new__(cls, val.y
+00004ad0: 6561 722c 2076 616c 2e6d 6f6e 7468 2c20  ear, val.month, 
+00004ae0: 7661 6c2e 6461 7929 0a0a 2020 2020 2020  val.day)..      
+00004af0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00004b00: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00004b10: 292e 5f5f 6e65 775f 5f28 636c 732c 202a  ).__new__(cls, *
+00004b20: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+00004b30: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00004b40: 7863 6570 7469 6f6e 2061 7320 6578 633a  xception as exc:
+00004b50: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00004b60: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004b80: 2255 6e61 626c 6520 746f 2063 6f6e 7665  "Unable to conve
+00004b90: 7274 2027 7b76 616c 7d27 2074 6f20 2744  rt '{val}' to 'D
+00004ba0: 4127 206f 626a 6563 7422 0a20 2020 2020  A' object".     
+00004bb0: 2020 2020 2020 2029 2066 726f 6d20 6578         ) from ex
+00004bc0: 630a 0a20 2020 2064 6566 205f 5f69 6e69  c..    def __ini
+00004bd0: 745f 5f28 7365 6c66 2c20 2a61 7267 733a  t__(self, *args:
+00004be0: 2041 6e79 2c20 2a2a 6b77 6172 6773 3a20   Any, **kwargs: 
+00004bf0: 416e 7929 202d 3e20 4e6f 6e65 3a0a 2020  Any) -> None:.  
+00004c00: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
+00004c10: 6120 6e65 7720 2a2a 4441 2a2a 2065 6c65  a new **DA** ele
+00004c20: 6d65 6e74 2076 616c 7565 2e22 2222 0a20  ment value.""". 
+00004c30: 2020 2020 2020 2076 616c 203d 2061 7267         val = arg
+00004c40: 735b 305d 0a20 2020 2020 2020 2069 6620  s[0].        if 
+00004c50: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
+00004c60: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00004c70: 2020 7365 6c66 2e6f 7269 6769 6e61 6c5f    self.original_
+00004c80: 7374 7269 6e67 203d 2076 616c 0a20 2020  string = val.   
+00004c90: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00004ca0: 616e 6365 2876 616c 2c20 4441 2920 616e  ance(val, DA) an
+00004cb0: 6420 6861 7361 7474 7228 7661 6c2c 2027  d hasattr(val, '
+00004cc0: 6f72 6967 696e 616c 5f73 7472 696e 6727  original_string'
+00004cd0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00004ce0: 656c 662e 6f72 6967 696e 616c 5f73 7472  elf.original_str
+00004cf0: 696e 6720 3d20 7661 6c2e 6f72 6967 696e  ing = val.origin
+00004d00: 616c 5f73 7472 696e 670a 2020 2020 2020  al_string.      
+00004d10: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00004d20: 6528 7661 6c2c 2064 6174 6574 696d 652e  e(val, datetime.
+00004d30: 6461 7465 293a 0a20 2020 2020 2020 2020  date):.         
+00004d40: 2020 2073 656c 662e 6f72 6967 696e 616c     self.original
+00004d50: 5f73 7472 696e 6720 3d20 6622 7b76 616c  _string = f"{val
+00004d60: 2e79 6561 727d 7b76 616c 2e6d 6f6e 7468  .year}{val.month
+00004d70: 3a30 327d 7b76 616c 2e64 6179 3a30 327d  :02}{val.day:02}
+00004d80: 220a 0a0a 636c 6173 7320 4454 285f 4461  "...class DT(_Da
+00004d90: 7465 5469 6d65 4261 7365 2c20 6461 7465  teTimeBase, date
+00004da0: 7469 6d65 2e64 6174 6574 696d 6529 3a0a  time.datetime):.
+00004db0: 2020 2020 2222 2253 746f 7265 2076 616c      """Store val
+00004dc0: 7565 2066 6f72 2061 6e20 656c 656d 656e  ue for an elemen
+00004dd0: 7420 7769 7468 2056 5220 2a2a 4454 2a2a  t with VR **DT**
+00004de0: 2061 7320 3a63 6c61 7373 3a60 6461 7465   as :class:`date
+00004df0: 7469 6d65 2e64 6174 6574 696d 6560 2e0a  time.datetime`..
+00004e00: 0a20 2020 204e 6f74 6520 7468 6174 2074  .    Note that t
+00004e10: 6865 203a 636c 6173 733a 6064 6174 6574  he :class:`datet
+00004e20: 696d 652e 6461 7465 7469 6d65 6020 6261  ime.datetime` ba
+00004e30: 7365 2063 6c61 7373 2069 7320 696d 6d75  se class is immu
+00004e40: 7461 626c 652e 0a20 2020 2022 2222 0a20  table..    """. 
+00004e50: 2020 205f 7265 6765 785f 6474 203d 2072     _regex_dt = r
+00004e60: 652e 636f 6d70 696c 6528 7222 2828 5c64  e.compile(r"((\d
+00004e70: 7b34 2c31 347d 2928 5c2e 285c 647b 312c  {4,14})(\.(\d{1,
+00004e80: 367d 2929 3f29 285b 2b2d 5d5c 647b 347d  6}))?)([+-]\d{4}
+00004e90: 293f 2229 0a0a 2020 2020 4073 7461 7469  )?")..    @stati
+00004ea0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00004eb0: 5f75 7463 5f6f 6666 7365 7428 7661 6c75  _utc_offset(valu
+00004ec0: 653a 2073 7472 2920 2d3e 2064 6174 6574  e: str) -> datet
+00004ed0: 696d 652e 7469 6d65 7a6f 6e65 3a0a 2020  ime.timezone:.  
+00004ee0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00004ef0: 7468 6520 5554 4320 4f66 6673 6574 2073  the UTC Offset s
+00004f00: 7566 6669 7820 6173 2061 203a 636c 6173  uffix as a :clas
+00004f10: 733a 6064 6174 6574 696d 652e 7469 6d65  s:`datetime.time
+00004f20: 7a6f 6e65 602e 0a0a 2020 2020 2020 2020  zone`...        
+00004f30: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00004f40: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00004f50: 2020 2020 2020 7661 6c75 6520 3a20 7374        value : st
+00004f60: 720a 2020 2020 2020 2020 2020 2020 5468  r.            Th
+00004f70: 6520 7661 6c75 6520 6f66 2074 6865 2055  e value of the U
+00004f80: 5443 206f 6666 7365 7420 7375 6666 6978  TC offset suffix
+00004f90: 2c20 7375 6368 2061 7320 6060 272d 3130  , such as ``'-10
+00004fa0: 3030 2760 6020 6f72 0a20 2020 2020 2020  00'`` or.       
+00004fb0: 2020 2020 2060 6027 2b30 3234 3527 6060       ``'+0245'``
+00004fc0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00004fd0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00004fe0: 2d2d 0a20 2020 2020 2020 2064 6174 6574  --.        datet
+00004ff0: 696d 652e 7469 6d65 7a6f 6e65 0a20 2020  ime.timezone.   
+00005000: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005010: 2023 2046 6f72 6d61 7420 6973 2026 5a5a   # Format is &ZZ
+00005020: 5858 2c20 2620 3d20 272b 2720 6f72 2027  XX, & = '+' or '
+00005030: 2d27 2c20 5a5a 2069 7320 686f 7572 732c  -', ZZ is hours,
+00005040: 2058 5820 6973 206d 696e 7574 6573 0a20   XX is minutes. 
+00005050: 2020 2020 2020 2068 6f75 7220 3d20 696e         hour = in
+00005060: 7428 7661 6c75 655b 313a 335d 2920 2a20  t(value[1:3]) * 
+00005070: 3630 2020 2320 436f 6e76 6572 7420 686f  60  # Convert ho
+00005080: 7572 7320 746f 206d 696e 7574 6573 0a20  urs to minutes. 
+00005090: 2020 2020 2020 206d 696e 7574 6520 3d20         minute = 
+000050a0: 696e 7428 7661 6c75 655b 333a 355d 2920  int(value[3:5]) 
+000050b0: 2023 2049 6e20 6d69 6e75 7465 730a 2020   # In minutes.  
+000050c0: 2020 2020 2020 6f66 6673 6574 203d 2028        offset = (
+000050d0: 686f 7572 202b 206d 696e 7574 6529 202a  hour + minute) *
+000050e0: 2036 3020 2023 2043 6f6e 7665 7274 206d   60  # Convert m
+000050f0: 696e 7574 6573 2074 6f20 7365 636f 6e64  inutes to second
+00005100: 730a 2020 2020 2020 2020 6f66 6673 6574  s.        offset
+00005110: 203d 202d 6f66 6673 6574 2069 6620 7661   = -offset if va
+00005120: 6c75 655b 305d 203d 3d20 272d 2720 656c  lue[0] == '-' el
+00005130: 7365 206f 6666 7365 740a 0a20 2020 2020  se offset..     
+00005140: 2020 2072 6574 7572 6e20 6461 7465 7469     return dateti
+00005150: 6d65 2e74 696d 657a 6f6e 6528 0a20 2020  me.timezone(.   
+00005160: 2020 2020 2020 2020 2064 6174 6574 696d           datetim
+00005170: 652e 7469 6d65 6465 6c74 6128 7365 636f  e.timedelta(seco
+00005180: 6e64 733d 6f66 6673 6574 292c 0a20 2020  nds=offset),.   
+00005190: 2020 2020 2020 2020 206e 616d 653d 7661           name=va
+000051a0: 6c75 650a 2020 2020 2020 2020 290a 0a20  lue.        ).. 
+000051b0: 2020 2064 6566 205f 5f6e 6577 5f5f 2820     def __new__( 
+000051c0: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+000051d0: 6d69 7363 5d0a 2020 2020 2020 2020 636c  misc].        cl
+000051e0: 733a 2054 7970 655b 2244 5422 5d2c 202a  s: Type["DT"], *
+000051f0: 6172 6773 3a20 416e 792c 202a 2a6b 7761  args: Any, **kwa
+00005200: 7267 733a 2041 6e79 0a20 2020 2029 202d  rgs: Any.    ) -
+00005210: 3e20 4f70 7469 6f6e 616c 5b22 4454 225d  > Optional["DT"]
+00005220: 3a0a 2020 2020 2020 2020 2222 2243 7265  :.        """Cre
+00005230: 6174 6520 616e 2069 6e73 7461 6e63 6520  ate an instance 
+00005240: 6f66 2044 5420 6f62 6a65 6374 2e0a 0a20  of DT object... 
+00005250: 2020 2020 2020 2052 6169 7365 2061 6e20         Raise an 
+00005260: 6578 6365 7074 696f 6e20 6966 2074 6865  exception if the
+00005270: 2073 7472 696e 6720 6361 6e6e 6f74 2062   string cannot b
+00005280: 6520 7061 7273 6564 206f 7220 7468 6520  e parsed or the 
+00005290: 6172 6775 6d65 6e74 0a20 2020 2020 2020  argument.       
+000052a0: 2069 7320 6f74 6865 7277 6973 6520 696e   is otherwise in
+000052b0: 636f 6d70 6174 6962 6c65 2e0a 0a20 2020  compatible...   
+000052c0: 2020 2020 2054 6865 2061 7267 756d 656e       The argumen
+000052d0: 7473 2028 6060 2a61 7267 7360 6020 616e  ts (``*args`` an
+000052e0: 6420 6060 2a2a 6b77 6172 6773 6060 2920  d ``**kwargs``) 
+000052f0: 6172 6520 6569 7468 6572 2074 6865 206f  are either the o
+00005300: 6e65 730a 2020 2020 2020 2020 696e 6865  nes.        inhe
+00005310: 7269 7465 6420 6672 6f6d 203a 636c 6173  rited from :clas
+00005320: 733a 6064 6174 6574 696d 652e 6461 7465  s:`datetime.date
+00005330: 7469 6d65 602c 206f 7220 7468 6520 6669  time`, or the fi
+00005340: 7273 7420 6172 6775 6d65 6e74 2069 730a  rst argument is.
+00005350: 2020 2020 2020 2020 6120 7374 7269 6e67          a string
+00005360: 2063 6f6e 666f 726d 616e 7420 746f 2074   conformant to t
+00005370: 6865 2044 5420 6465 6669 6e69 7469 6f6e  he DT definition
+00005380: 2069 6e20 7468 6520 4449 434f 4d20 5374   in the DICOM St
+00005390: 616e 6461 7264 2c0a 2020 2020 2020 2020  andard,.        
+000053a0: 5061 7274 2035 2c20 3a64 636d 3a60 5461  Part 5, :dcm:`Ta
+000053b0: 626c 6520 362e 322d 313c 7061 7274 3035  ble 6.2-1<part05
+000053c0: 2f73 6563 745f 362e 322e 6874 6d6c 2374  /sect_6.2.html#t
+000053d0: 6162 6c65 5f36 2e32 2d31 3e60 2c0a 2020  able_6.2-1>`,.  
+000053e0: 2020 2020 2020 6f72 2069 7420 6973 2061        or it is a
+000053f0: 203a 636c 6173 733a 6064 6174 6574 696d   :class:`datetim
+00005400: 652e 6461 7465 7469 6d65 6020 6f62 6a65  e.datetime` obje
+00005410: 6374 2c20 6f72 2061 6e20 6f62 6a65 6374  ct, or an object
+00005420: 206f 6620 7479 7065 0a20 2020 2020 2020   of type.       
+00005430: 203a 636c 6173 733a 607e 7079 6469 636f   :class:`~pydico
+00005440: 6d2e 7661 6c75 6572 6570 2e44 5460 2e0a  m.valuerep.DT`..
+00005450: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005460: 2020 2020 6966 206e 6f74 2061 7267 7320      if not args 
+00005470: 6f72 2061 7267 735b 305d 2069 7320 4e6f  or args[0] is No
+00005480: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00005490: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+000054a0: 2020 2020 2076 616c 203d 2061 7267 735b       val = args[
+000054b0: 305d 0a20 2020 2020 2020 2069 6620 6973  0].        if is
+000054c0: 696e 7374 616e 6365 2876 616c 2c20 7374  instance(val, st
+000054d0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000054e0: 6966 2076 616c 2e73 7472 6970 2829 203d  if val.strip() =
+000054f0: 3d20 2727 3a0a 2020 2020 2020 2020 2020  = '':.          
+00005500: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00005510: 650a 0a20 2020 2020 2020 2020 2020 206d  e..            m
+00005520: 6174 6368 203d 2063 6c73 2e5f 7265 6765  atch = cls._rege
+00005530: 785f 6474 2e6d 6174 6368 2876 616c 290a  x_dt.match(val).
+00005540: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00005550: 6f74 206d 6174 6368 206f 7220 6c65 6e28  ot match or len(
+00005560: 7661 6c29 203e 2032 363a 0a20 2020 2020  val) > 26:.     
+00005570: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00005580: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055a0: 2066 2255 6e61 626c 6520 746f 2063 6f6e   f"Unable to con
+000055b0: 7665 7274 206e 6f6e 2d63 6f6e 666f 726d  vert non-conform
+000055c0: 616e 7420 7661 6c75 6520 277b 7661 6c7d  ant value '{val}
+000055d0: 2720 746f 2027 4454 2720 220a 2020 2020  ' to 'DT' ".    
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 226f 626a 6563 7422 0a20 2020 2020 2020  "object".       
+00005600: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00005610: 2020 2020 2020 2020 6474 5f6d 6174 6368          dt_match
+00005620: 203d 206d 6174 6368 2e67 726f 7570 2832   = match.group(2
+00005630: 290a 2020 2020 2020 2020 2020 2020 6172  ).            ar
+00005640: 6773 203d 2028 0a20 2020 2020 2020 2020  gs = (.         
+00005650: 2020 2020 2020 2069 6e74 2864 745f 6d61         int(dt_ma
+00005660: 7463 685b 303a 345d 292c 2020 2320 7965  tch[0:4]),  # ye
+00005670: 6172 0a20 2020 2020 2020 2020 2020 2020  ar.             
+00005680: 2020 2031 2069 6620 6c65 6e28 6474 5f6d     1 if len(dt_m
+00005690: 6174 6368 2920 3c20 3620 656c 7365 2069  atch) < 6 else i
+000056a0: 6e74 2864 745f 6d61 7463 685b 343a 365d  nt(dt_match[4:6]
+000056b0: 292c 2020 2320 6d6f 6e74 680a 2020 2020  ),  # month.    
+000056c0: 2020 2020 2020 2020 2020 2020 3120 6966              1 if
+000056d0: 206c 656e 2864 745f 6d61 7463 6829 203c   len(dt_match) <
+000056e0: 2038 2065 6c73 6520 696e 7428 6474 5f6d   8 else int(dt_m
+000056f0: 6174 6368 5b36 3a38 5d29 2c20 2023 2064  atch[6:8]),  # d
+00005700: 6179 0a20 2020 2020 2020 2020 2020 2029  ay.            )
+00005710: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00005720: 7267 7320 3d20 7b0a 2020 2020 2020 2020  rgs = {.        
+00005730: 2020 2020 2020 2020 2768 6f75 7227 3a20          'hour': 
+00005740: 3020 6966 206c 656e 2864 745f 6d61 7463  0 if len(dt_matc
+00005750: 6829 203c 2031 3020 656c 7365 2069 6e74  h) < 10 else int
+00005760: 2864 745f 6d61 7463 685b 383a 3130 5d29  (dt_match[8:10])
+00005770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005780: 2020 276d 696e 7574 6527 3a20 3020 6966    'minute': 0 if
+00005790: 206c 656e 2864 745f 6d61 7463 6829 203c   len(dt_match) <
+000057a0: 2031 3220 656c 7365 2069 6e74 2864 745f   12 else int(dt_
+000057b0: 6d61 7463 685b 3130 3a31 325d 292c 0a20  match[10:12]),. 
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000057d0: 7365 636f 6e64 273a 2030 2069 6620 6c65  second': 0 if le
+000057e0: 6e28 6474 5f6d 6174 6368 2920 3c20 3134  n(dt_match) < 14
+000057f0: 2065 6c73 6520 696e 7428 6474 5f6d 6174   else int(dt_mat
+00005800: 6368 5b31 323a 3134 5d29 2c0a 2020 2020  ch[12:14]),.    
+00005810: 2020 2020 2020 2020 2020 2020 276d 6963              'mic
+00005820: 726f 7365 636f 6e64 273a 2030 0a20 2020  rosecond': 0.   
+00005830: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00005840: 2020 2020 2020 2069 6620 6c65 6e28 6474         if len(dt
+00005850: 5f6d 6174 6368 2920 3e3d 2031 3420 616e  _match) >= 14 an
+00005860: 6420 6d61 7463 682e 6772 6f75 7028 3429  d match.group(4)
+00005870: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005880: 2020 6b77 6172 6773 5b27 6d69 6372 6f73    kwargs['micros
+00005890: 6563 6f6e 6427 5d20 3d20 696e 7428 0a20  econd'] = int(. 
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 2020 206d 6174 6368 2e67 726f 7570 2834     match.group(4
+000058c0: 292e 7273 7472 6970 2829 2e6c 6a75 7374  ).rstrip().ljust
+000058d0: 2836 2c20 2730 2729 0a20 2020 2020 2020  (6, '0').       
+000058e0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000058f0: 2020 2020 2020 2020 2320 5469 6d65 7a6f          # Timezo
+00005900: 6e65 206f 6666 7365 740a 2020 2020 2020  ne offset.      
+00005910: 2020 2020 2020 747a 5f6d 6174 6368 203d        tz_match =
+00005920: 206d 6174 6368 2e67 726f 7570 2835 290a   match.group(5).
+00005930: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+00005940: 6773 5b27 747a 696e 666f 275d 203d 2063  gs['tzinfo'] = c
+00005950: 6c73 2e5f 7574 635f 6f66 6673 6574 2874  ls._utc_offset(t
+00005960: 7a5f 6d61 7463 6829 2069 6620 747a 5f6d  z_match) if tz_m
+00005970: 6174 6368 2065 6c73 6520 4e6f 6e65 0a0a  atch else None..
+00005980: 2020 2020 2020 2020 2020 2020 2320 4454              # DT
+00005990: 206d 6179 2069 6e63 6c75 6465 2061 206c   may include a l
+000059a0: 6561 7020 7365 636f 6e64 2077 6869 6368  eap second which
+000059b0: 2069 736e 2774 2061 6c6c 6f77 6564 2062   isn't allowed b
+000059c0: 7920 6461 7465 7469 6d65 0a20 2020 2020  y datetime.     
+000059d0: 2020 2020 2020 2069 6620 6b77 6172 6773         if kwargs
+000059e0: 5b27 7365 636f 6e64 275d 203d 3d20 3630  ['second'] == 60
+000059f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005a00: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00005a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a20: 2020 2020 2022 2764 6174 6574 696d 652e       "'datetime.
+00005a30: 6461 7465 7469 6d65 2720 646f 6573 6e27  datetime' doesn'
+00005a40: 7420 616c 6c6f 7720 6120 7661 6c75 6520  t allow a value 
+00005a50: 6f66 2027 3630 2720 666f 7220 220a 2020  of '60' for ".  
+00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a70: 2020 2274 6865 2073 6563 6f6e 6473 2063    "the seconds c
+00005a80: 6f6d 706f 6e65 6e74 2c20 6368 616e 6769  omponent, changi
+00005a90: 6e67 2074 6f20 2735 3927 220a 2020 2020  ng to '59'".    
+00005aa0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 6b77                kw
+00005ac0: 6172 6773 5b27 7365 636f 6e64 275d 203d  args['second'] =
+00005ad0: 2035 390a 0a20 2020 2020 2020 2020 2020   59..           
+00005ae0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00005af0: 5f5f 6e65 775f 5f28 636c 732c 202a 6172  __new__(cls, *ar
+00005b00: 6773 2c20 2a2a 6b77 6172 6773 290a 0a20  gs, **kwargs).. 
+00005b10: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00005b20: 616e 6365 2876 616c 2c20 6461 7465 7469  ance(val, dateti
+00005b30: 6d65 2e64 6174 6574 696d 6529 3a0a 2020  me.datetime):.  
+00005b40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00005b50: 2073 7570 6572 2829 2e5f 5f6e 6577 5f5f   super().__new__
+00005b60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005b70: 2020 636c 732c 202a 7661 6c2e 7469 6d65    cls, *val.time
+00005b80: 7475 706c 6528 295b 3a36 5d2c 2076 616c  tuple()[:6], val
+00005b90: 2e6d 6963 726f 7365 636f 6e64 2c20 7661  .microsecond, va
+00005ba0: 6c2e 747a 696e 666f 0a20 2020 2020 2020  l.tzinfo.       
+00005bb0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00005bc0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00005bd0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00005be0: 5f5f 6e65 775f 5f28 636c 732c 202a 6172  __new__(cls, *ar
+00005bf0: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+00005c00: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00005c10: 6570 7469 6f6e 2061 7320 6578 633a 0a20  eption as exc:. 
+00005c20: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00005c30: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00005c40: 2020 2020 2020 2020 2020 2020 2066 2255               f"U
+00005c50: 6e61 626c 6520 746f 2063 6f6e 7665 7274  nable to convert
+00005c60: 2027 7b76 616c 7d27 2074 6f20 2744 5427   '{val}' to 'DT'
+00005c70: 206f 626a 6563 7422 0a20 2020 2020 2020   object".       
+00005c80: 2020 2020 2029 2066 726f 6d20 6578 630a       ) from exc.
+00005c90: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00005ca0: 5f28 7365 6c66 2c20 2a61 7267 733a 2041  _(self, *args: A
+00005cb0: 6e79 2c20 2a2a 6b77 6172 6773 3a20 416e  ny, **kwargs: An
+00005cc0: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
+00005cd0: 2020 2020 2222 2243 7265 6174 6520 6120      """Create a 
+00005ce0: 6e65 7720 2a2a 4454 2a2a 2065 6c65 6d65  new **DT** eleme
+00005cf0: 6e74 2076 616c 7565 2e22 2222 0a20 2020  nt value.""".   
+00005d00: 2020 2020 2076 616c 203d 2061 7267 735b       val = args[
+00005d10: 305d 0a20 2020 2020 2020 2069 6620 6973  0].        if is
+00005d20: 696e 7374 616e 6365 2876 616c 2c20 7374  instance(val, st
+00005d30: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00005d40: 7365 6c66 2e6f 7269 6769 6e61 6c5f 7374  self.original_st
+00005d50: 7269 6e67 203d 2076 616c 0a20 2020 2020  ring = val.     
+00005d60: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00005d70: 6365 2876 616c 2c20 4454 2920 616e 6420  ce(val, DT) and 
+00005d80: 6861 7361 7474 7228 7661 6c2c 2027 6f72  hasattr(val, 'or
+00005d90: 6967 696e 616c 5f73 7472 696e 6727 293a  iginal_string'):
+00005da0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005db0: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
+00005dc0: 6720 3d20 7661 6c2e 6f72 6967 696e 616c  g = val.original
+00005dd0: 5f73 7472 696e 670a 2020 2020 2020 2020  _string.        
+00005de0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00005df0: 7661 6c2c 2064 6174 6574 696d 652e 6461  val, datetime.da
+00005e00: 7465 7469 6d65 293a 0a20 2020 2020 2020  tetime):.       
+00005e10: 2020 2020 2073 656c 662e 6f72 6967 696e       self.origin
+00005e20: 616c 5f73 7472 696e 6720 3d20 280a 2020  al_string = (.  
+00005e30: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00005e40: 7b76 616c 2e79 6561 723a 3034 7d7b 7661  {val.year:04}{va
+00005e50: 6c2e 6d6f 6e74 683a 3032 7d7b 7661 6c2e  l.month:02}{val.
+00005e60: 6461 793a 3032 7d22 0a20 2020 2020 2020  day:02}".       
+00005e70: 2020 2020 2020 2020 2066 227b 7661 6c2e           f"{val.
+00005e80: 686f 7572 3a30 327d 7b76 616c 2e6d 696e  hour:02}{val.min
+00005e90: 7574 653a 3032 7d7b 7661 6c2e 7365 636f  ute:02}{val.seco
+00005ea0: 6e64 3a30 327d 220a 2020 2020 2020 2020  nd:02}".        
+00005eb0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00005ec0: 2020 2320 6d69 6c6c 6973 6563 6f6e 6473    # milliseconds
+00005ed0: 2061 7265 2073 656c 646f 6d20 7573 6564   are seldom used
+00005ee0: 2c20 6164 6420 7468 656d 206f 6e6c 7920  , add them only 
+00005ef0: 6966 206e 6565 6465 640a 2020 2020 2020  if needed.      
+00005f00: 2020 2020 2020 6966 2076 616c 2e6d 6963        if val.mic
+00005f10: 726f 7365 636f 6e64 203e 2030 3a0a 2020  rosecond > 0:.  
+00005f20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005f30: 6c66 2e6f 7269 6769 6e61 6c5f 7374 7269  lf.original_stri
+00005f40: 6e67 202b 3d20 6622 2e7b 7661 6c2e 6d69  ng += f".{val.mi
+00005f50: 6372 6f73 6563 6f6e 643a 3036 7d22 0a0a  crosecond:06}"..
+00005f60: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00005f70: 616c 2e74 7a69 6e66 6f20 6973 206e 6f74  al.tzinfo is not
+00005f80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005f90: 2020 2020 2020 2023 206f 6666 7365 743a         # offset:
+00005fa0: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
+00005fb0: 6d65 2e74 696d 6564 656c 7461 5d0a 2020  me.timedelta].  
+00005fc0: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+00005fd0: 6673 6574 203d 2076 616c 2e74 7a69 6e66  fset = val.tzinf
+00005fe0: 6f2e 7574 636f 6666 7365 7428 7661 6c29  o.utcoffset(val)
+00005ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006000: 2069 6620 6f66 6673 6574 2069 7320 6e6f   if offset is no
+00006010: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00006020: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
+00006030: 6574 5f6d 696e 203d 206f 6666 7365 742e  et_min = offset.
+00006040: 6461 7973 202a 2032 3420 2a20 3630 202b  days * 24 * 60 +
+00006050: 206f 6666 7365 742e 7365 636f 6e64 7320   offset.seconds 
+00006060: 2f2f 2036 300a 2020 2020 2020 2020 2020  // 60.          
+00006070: 2020 2020 2020 2020 2020 7369 676e 203d            sign =
+00006080: 2022 2b22 2069 6620 6f66 6673 6574 5f6d   "+" if offset_m
+00006090: 696e 203e 3d20 3020 656c 7365 2022 2d22  in >= 0 else "-"
+000060a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060b0: 2020 2020 206f 6666 7365 745f 6d69 6e20       offset_min 
+000060c0: 3d20 6162 7328 6f66 6673 6574 5f6d 696e  = abs(offset_min
+000060d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000060e0: 2020 2020 2020 7365 6c66 2e6f 7269 6769        self.origi
+000060f0: 6e61 6c5f 7374 7269 6e67 202b 3d20 280a  nal_string += (.
+00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006110: 2020 2020 2020 2020 6622 7b73 6967 6e7d          f"{sign}
+00006120: 7b6f 6666 7365 745f 6d69 6e20 2f2f 2036  {offset_min // 6
+00006130: 303a 3032 7d7b 6f66 6673 6574 5f6d 696e  0:02}{offset_min
+00006140: 2025 2036 303a 3032 7d22 0a20 2020 2020   % 60:02}".     
+00006150: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00006160: 0a0a 0a63 6c61 7373 2054 4d28 5f44 6174  ...class TM(_Dat
+00006170: 6554 696d 6542 6173 652c 2064 6174 6574  eTimeBase, datet
+00006180: 696d 652e 7469 6d65 293a 0a20 2020 2022  ime.time):.    "
+00006190: 2222 5374 6f72 6520 7661 6c75 6520 666f  ""Store value fo
+000061a0: 7220 616e 2065 6c65 6d65 6e74 2077 6974  r an element wit
+000061b0: 6820 5652 202a 2a54 4d2a 2a20 6173 203a  h VR **TM** as :
+000061c0: 636c 6173 733a 6064 6174 6574 696d 652e  class:`datetime.
+000061d0: 7469 6d65 602e 0a0a 2020 2020 4e6f 7465  time`...    Note
+000061e0: 2074 6861 7420 7468 6520 3a63 6c61 7373   that the :class
+000061f0: 3a60 6461 7465 7469 6d65 2e74 696d 6560  :`datetime.time`
+00006200: 2062 6173 6520 636c 6173 7320 6973 2069   base class is i
+00006210: 6d6d 7574 6162 6c65 2e0a 2020 2020 2222  mmutable..    ""
+00006220: 220a 2020 2020 5f52 455f 5449 4d45 203d  ".    _RE_TIME =
+00006230: 2072 652e 636f 6d70 696c 6528 0a20 2020   re.compile(.   
+00006240: 2020 2020 2072 2228 3f50 3c68 3e5e 285b       r"(?P<h>^([
+00006250: 3031 5d5b 302d 395d 7c32 5b30 2d33 5d29  01][0-9]|2[0-3])
+00006260: 2922 0a20 2020 2020 2020 2072 2228 283f  )".        r"((?
+00006270: 503c 6d3e 285b 302d 355d 5b30 2d39 5d29  P<m>([0-5][0-9])
+00006280: 2922 0a20 2020 2020 2020 2072 2228 283f  )".        r"((?
+00006290: 503c 733e 285b 302d 355d 5b30 2d39 5d7c  P<s>([0-5][0-9]|
+000062a0: 3630 2929 220a 2020 2020 2020 2020 7222  60))".        r"
+000062b0: 285c 2e28 3f50 3c6d 733e 285b 302d 395d  (\.(?P<ms>([0-9]
+000062c0: 7b31 2c36 7d29 3f29 293f 293f 293f 2422  {1,6})?))?)?)?$"
+000062d0: 0a20 2020 2029 0a0a 2020 2020 6465 6620  .    )..    def 
+000062e0: 5f5f 6e65 775f 5f28 2020 2320 7479 7065  __new__(  # type
+000062f0: 3a20 6967 6e6f 7265 5b6d 6973 635d 0a20  : ignore[misc]. 
+00006300: 2020 2020 2020 2063 6c73 3a20 5479 7065         cls: Type
+00006310: 5b22 544d 225d 2c20 2a61 7267 733a 2041  ["TM"], *args: A
+00006320: 6e79 2c20 2a2a 6b77 6172 6773 3a20 416e  ny, **kwargs: An
+00006330: 790a 2020 2020 2920 2d3e 204f 7074 696f  y.    ) -> Optio
+00006340: 6e61 6c5b 2254 4d22 5d3a 0a20 2020 2020  nal["TM"]:.     
+00006350: 2020 2022 2222 4372 6561 7465 2061 6e20     """Create an 
+00006360: 696e 7374 616e 6365 206f 6620 544d 206f  instance of TM o
+00006370: 626a 6563 7420 6672 6f6d 2061 2073 7472  bject from a str
+00006380: 696e 672e 0a0a 2020 2020 2020 2020 5261  ing...        Ra
+00006390: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
+000063a0: 2069 6620 7468 6520 7374 7269 6e67 2063   if the string c
+000063b0: 616e 6e6f 7420 6265 2070 6172 7365 6420  annot be parsed 
+000063c0: 6f72 2074 6865 2061 7267 756d 656e 740a  or the argument.
+000063d0: 2020 2020 2020 2020 6973 206f 7468 6572          is other
+000063e0: 7769 7365 2069 6e63 6f6d 7061 7469 626c  wise incompatibl
+000063f0: 652e 0a0a 2020 2020 2020 2020 5468 6520  e...        The 
+00006400: 6172 6775 6d65 6e74 7320 2860 602a 6172  arguments (``*ar
+00006410: 6773 6060 2061 6e64 2060 602a 2a6b 7761  gs`` and ``**kwa
+00006420: 7267 7360 6029 2061 7265 2065 6974 6865  rgs``) are eithe
+00006430: 7220 7468 6520 6f6e 6573 0a20 2020 2020  r the ones.     
+00006440: 2020 2069 6e68 6572 6974 6564 2066 726f     inherited fro
+00006450: 6d20 3a63 6c61 7373 3a60 6461 7465 7469  m :class:`dateti
+00006460: 6d65 2e74 696d 6560 2c20 6f72 2074 6865  me.time`, or the
+00006470: 2066 6972 7374 2061 7267 756d 656e 7420   first argument 
+00006480: 6973 0a20 2020 2020 2020 2061 2073 7472  is.        a str
+00006490: 696e 6720 636f 6e66 6f72 6d61 6e74 2074  ing conformant t
+000064a0: 6f20 7468 6520 544d 2064 6566 696e 6974  o the TM definit
+000064b0: 696f 6e20 696e 2074 6865 2044 4943 4f4d  ion in the DICOM
+000064c0: 2053 7461 6e64 6172 642c 0a20 2020 2020   Standard,.     
+000064d0: 2020 2050 6172 7420 352c 203a 6463 6d3a     Part 5, :dcm:
+000064e0: 6054 6162 6c65 2036 2e32 2d31 3c70 6172  `Table 6.2-1<par
+000064f0: 7430 352f 7365 6374 5f36 2e32 2e68 746d  t05/sect_6.2.htm
+00006500: 6c23 7461 626c 655f 362e 322d 313e 602c  l#table_6.2-1>`,
+00006510: 0a20 2020 2020 2020 206f 7220 6974 2069  .        or it i
+00006520: 7320 6120 3a63 6c61 7373 3a60 6461 7465  s a :class:`date
+00006530: 7469 6d65 2e74 696d 6560 206f 626a 6563  time.time` objec
+00006540: 742c 206f 7220 616e 206f 626a 6563 7420  t, or an object 
+00006550: 6f66 2074 7970 650a 2020 2020 2020 2020  of type.        
+00006560: 3a63 6c61 7373 3a60 7e70 7964 6963 6f6d  :class:`~pydicom
+00006570: 2e76 616c 7565 7265 702e 544d 602e 0a20  .valuerep.TM`.. 
+00006580: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006590: 2020 2069 6620 6e6f 7420 6172 6773 206f     if not args o
+000065a0: 7220 6172 6773 5b30 5d20 6973 204e 6f6e  r args[0] is Non
+000065b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000065c0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+000065d0: 2020 2020 7661 6c20 3d20 6172 6773 5b30      val = args[0
+000065e0: 5d0a 2020 2020 2020 2020 6966 2069 7369  ].        if isi
+000065f0: 6e73 7461 6e63 6528 7661 6c2c 2073 7472  nstance(val, str
+00006600: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00006610: 6620 7661 6c2e 7374 7269 7028 2920 3d3d  f val.strip() ==
+00006620: 2027 273a 0a20 2020 2020 2020 2020 2020   '':.           
+00006630: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00006640: 2020 2320 656d 7074 7920 7469 6d65 0a0a    # empty time..
+00006650: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+00006660: 6820 3d20 636c 732e 5f52 455f 5449 4d45  h = cls._RE_TIME
+00006670: 2e6d 6174 6368 2876 616c 290a 2020 2020  .match(val).    
+00006680: 2020 2020 2020 2020 6966 206e 6f74 206d          if not m
+00006690: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+000066a0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000066b0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+000066c0: 2020 2020 2020 2020 2020 2020 6622 556e              f"Un
+000066d0: 6162 6c65 2074 6f20 636f 6e76 6572 7420  able to convert 
+000066e0: 6e6f 6e2d 636f 6e66 6f72 6d61 6e74 2076  non-conformant v
+000066f0: 616c 7565 2027 7b76 616c 7d27 2074 6f20  alue '{val}' to 
+00006700: 2754 4d27 2022 0a20 2020 2020 2020 2020  'TM' ".         
+00006710: 2020 2020 2020 2020 2020 2022 6f62 6a65             "obje
+00006720: 6374 220a 2020 2020 2020 2020 2020 2020  ct".            
+00006730: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00006740: 2020 2068 6f75 7220 3d20 696e 7428 6d61     hour = int(ma
+00006750: 7463 682e 6772 6f75 7028 2768 2729 290a  tch.group('h')).
+00006760: 2020 2020 2020 2020 2020 2020 6d69 6e75              minu
+00006770: 7465 203d 2030 2069 6620 6d61 7463 682e  te = 0 if match.
+00006780: 6772 6f75 7028 276d 2729 2069 7320 4e6f  group('m') is No
+00006790: 6e65 2065 6c73 6520 696e 7428 6d61 7463  ne else int(matc
+000067a0: 682e 6772 6f75 7028 276d 2729 290a 2020  h.group('m')).  
+000067b0: 2020 2020 2020 2020 2020 7365 636f 6e64            second
+000067c0: 203d 2030 2069 6620 6d61 7463 682e 6772   = 0 if match.gr
+000067d0: 6f75 7028 2773 2729 2069 7320 4e6f 6e65  oup('s') is None
+000067e0: 2065 6c73 6520 696e 7428 6d61 7463 682e   else int(match.
+000067f0: 6772 6f75 7028 2773 2729 290a 0a20 2020  group('s'))..   
+00006800: 2020 2020 2020 2020 2069 6620 7365 636f           if seco
+00006810: 6e64 203d 3d20 3630 3a0a 2020 2020 2020  nd == 60:.      
+00006820: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+00006830: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
+00006840: 2020 2020 2020 2020 2020 2020 2022 2764               "'d
+00006850: 6174 6574 696d 652e 7469 6d65 2720 646f  atetime.time' do
+00006860: 6573 6e27 7420 616c 6c6f 7720 6120 7661  esn't allow a va
+00006870: 6c75 6520 6f66 2027 3630 2720 666f 7220  lue of '60' for 
+00006880: 7468 6520 220a 2020 2020 2020 2020 2020  the ".          
+00006890: 2020 2020 2020 2020 2020 2273 6563 6f6e            "secon
+000068a0: 6473 2063 6f6d 706f 6e65 6e74 2c20 6368  ds component, ch
+000068b0: 616e 6769 6e67 2074 6f20 2735 3927 220a  anging to '59'".
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000068e0: 2020 7365 636f 6e64 203d 2035 390a 0a20    second = 59.. 
+000068f0: 2020 2020 2020 2020 2020 206d 6963 726f             micro
+00006900: 7365 636f 6e64 203d 2030 0a20 2020 2020  second = 0.     
+00006910: 2020 2020 2020 2069 6620 6d61 7463 682e         if match.
+00006920: 6772 6f75 7028 276d 7327 293a 0a20 2020  group('ms'):.   
+00006930: 2020 2020 2020 2020 2020 2020 206d 6963               mic
+00006940: 726f 7365 636f 6e64 203d 2069 6e74 286d  rosecond = int(m
+00006950: 6174 6368 2e67 726f 7570 2827 6d73 2729  atch.group('ms')
+00006960: 2e72 7374 7269 7028 292e 6c6a 7573 7428  .rstrip().ljust(
+00006970: 362c 2027 3027 2929 0a0a 2020 2020 2020  6, '0'))..      
+00006980: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
+00006990: 6572 2829 2e5f 5f6e 6577 5f5f 280a 2020  er().__new__(.  
+000069a0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+000069b0: 732c 2068 6f75 722c 206d 696e 7574 652c  s, hour, minute,
+000069c0: 2073 6563 6f6e 642c 206d 6963 726f 7365   second, microse
+000069d0: 636f 6e64 0a20 2020 2020 2020 2020 2020  cond.           
+000069e0: 2029 0a0a 2020 2020 2020 2020 6966 2069   )..        if i
+000069f0: 7369 6e73 7461 6e63 6528 7661 6c2c 2064  sinstance(val, d
+00006a00: 6174 6574 696d 652e 7469 6d65 293a 0a20  atetime.time):. 
+00006a10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006a20: 6e20 7375 7065 7228 292e 5f5f 6e65 775f  n super().__new_
+00006a30: 5f28 0a20 2020 2020 2020 2020 2020 2020  _(.             
+00006a40: 2020 2063 6c73 2c20 7661 6c2e 686f 7572     cls, val.hour
+00006a50: 2c20 7661 6c2e 6d69 6e75 7465 2c20 7661  , val.minute, va
+00006a60: 6c2e 7365 636f 6e64 2c20 7661 6c2e 6d69  l.second, val.mi
+00006a70: 6372 6f73 6563 6f6e 640a 2020 2020 2020  crosecond.      
+00006a80: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00006a90: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00006aa0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+00006ab0: 2e5f 5f6e 6577 5f5f 280a 2020 2020 2020  .__new__(.      
+00006ac0: 2020 2020 2020 2020 2020 636c 732c 202a            cls, *
+00006ad0: 6172 6773 2c20 2a2a 6b77 6172 6773 0a20  args, **kwargs. 
+00006ae0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006af0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+00006b00: 7074 696f 6e20 6173 2065 7863 3a0a 2020  ption as exc:.  
+00006b10: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00006b20: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00006b30: 2020 2020 2020 2020 2020 2020 6622 556e              f"Un
+00006b40: 6162 6c65 2074 6f20 636f 6e76 6572 7420  able to convert 
+00006b50: 277b 7661 6c7d 2720 746f 2027 544d 2720  '{val}' to 'TM' 
+00006b60: 6f62 6a65 6374 220a 2020 2020 2020 2020  object".        
+00006b70: 2020 2020 2920 6672 6f6d 2065 7863 0a0a      ) from exc..
+00006b80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00006b90: 2873 656c 662c 202a 6172 6773 3a20 416e  (self, *args: An
+00006ba0: 792c 202a 2a6b 7761 7267 733a 2041 6e79  y, **kwargs: Any
+00006bb0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00006bc0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00006bd0: 745f 5f28 290a 2020 2020 2020 2020 7661  t__().        va
+00006be0: 6c20 3d20 6172 6773 5b30 5d0a 2020 2020  l = args[0].    
+00006bf0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00006c00: 6528 7661 6c2c 2073 7472 293a 0a20 2020  e(val, str):.   
+00006c10: 2020 2020 2020 2020 2073 656c 662e 6f72           self.or
+00006c20: 6967 696e 616c 5f73 7472 696e 6720 3d20  iginal_string = 
+00006c30: 7661 6c0a 2020 2020 2020 2020 656c 6966  val.        elif
+00006c40: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
+00006c50: 2054 4d29 2061 6e64 2068 6173 6174 7472   TM) and hasattr
+00006c60: 2876 616c 2c20 276f 7269 6769 6e61 6c5f  (val, 'original_
+00006c70: 7374 7269 6e67 2729 3a0a 2020 2020 2020  string'):.      
+00006c80: 2020 2020 2020 7365 6c66 2e6f 7269 6769        self.origi
+00006c90: 6e61 6c5f 7374 7269 6e67 203d 2076 616c  nal_string = val
+00006ca0: 2e6f 7269 6769 6e61 6c5f 7374 7269 6e67  .original_string
+00006cb0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00006cc0: 696e 7374 616e 6365 2876 616c 2c20 6461  instance(val, da
+00006cd0: 7465 7469 6d65 2e74 696d 6529 3a0a 2020  tetime.time):.  
+00006ce0: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+00006cf0: 7269 6769 6e61 6c5f 7374 7269 6e67 203d  riginal_string =
+00006d00: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00006d10: 2020 2066 227b 7661 6c2e 686f 7572 3a30     f"{val.hour:0
+00006d20: 327d 7b76 616c 2e6d 696e 7574 653a 3032  2}{val.minute:02
+00006d30: 7d7b 7661 6c2e 7365 636f 6e64 3a30 327d  }{val.second:02}
+00006d40: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+00006d50: 2020 2020 2020 2020 2020 2020 2320 6d69              # mi
+00006d60: 6c6c 6973 6563 6f6e 6473 2061 7265 2073  lliseconds are s
+00006d70: 656c 646f 6d20 7573 6564 2c20 6164 6420  eldom used, add 
+00006d80: 7468 656d 206f 6e6c 7920 6966 206e 6565  them only if nee
+00006d90: 6465 640a 2020 2020 2020 2020 2020 2020  ded.            
+00006da0: 6966 2076 616c 2e6d 6963 726f 7365 636f  if val.microseco
+00006db0: 6e64 203e 2030 3a0a 2020 2020 2020 2020  nd > 0:.        
+00006dc0: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
+00006dd0: 6769 6e61 6c5f 7374 7269 6e67 202b 3d20  ginal_string += 
+00006de0: 6622 2e7b 7661 6c2e 6d69 6372 6f73 6563  f".{val.microsec
+00006df0: 6f6e 643a 3036 7d22 0a0a 0a64 6566 2069  ond:06}"...def i
+00006e00: 735f 7661 6c69 645f 6473 2873 3a20 7374  s_valid_ds(s: st
+00006e10: 7229 202d 3e20 626f 6f6c 3a0a 2020 2020  r) -> bool:.    
+00006e20: 2222 2243 6865 636b 2077 6865 7468 6572  """Check whether
+00006e30: 2074 6869 7320 7374 7269 6e67 2069 7320   this string is 
+00006e40: 6120 7661 6c69 6420 6465 6369 6d61 6c20  a valid decimal 
+00006e50: 7374 7269 6e67 2e0a 0a20 2020 2056 616c  string...    Val
+00006e60: 6964 2064 6563 696d 616c 2073 7472 696e  id decimal strin
+00006e70: 6773 206d 7573 7420 6265 2031 3620 6368  gs must be 16 ch
+00006e80: 6172 6163 7465 7273 206f 7220 6665 7765  aracters or fewe
+00006e90: 722c 2061 6e64 2063 6f6e 7461 696e 206f  r, and contain o
+00006ea0: 6e6c 790a 2020 2020 6368 6172 6163 7465  nly.    characte
+00006eb0: 7273 2066 726f 6d20 6120 6c69 6d69 7465  rs from a limite
+00006ec0: 6420 7365 742e 0a0a 2020 2020 5061 7261  d set...    Para
+00006ed0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00006ee0: 2d2d 2d2d 2d0a 2020 2020 733a 2073 7472  -----.    s: str
+00006ef0: 0a20 2020 2020 2020 2053 7472 696e 6720  .        String 
+00006f00: 746f 2074 6573 742e 0a0a 2020 2020 5265  to test...    Re
+00006f10: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00006f20: 2d0a 2020 2020 626f 6f6c 0a20 2020 2020  -.    bool.     
+00006f30: 2020 2054 7275 6520 6966 2074 6865 2073     True if the s
+00006f40: 7472 696e 6720 6973 2061 2076 616c 6964  tring is a valid
+00006f50: 2064 6563 696d 616c 2073 7472 696e 672e   decimal string.
+00006f60: 204f 7468 6572 7769 7365 2046 616c 7365   Otherwise False
+00006f70: 2e0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
+00006f80: 7475 726e 2076 616c 6964 6174 655f 6c65  turn validate_le
+00006f90: 6e67 7468 5f61 6e64 5f74 7970 655f 616e  ngth_and_type_an
+00006fa0: 645f 7265 6765 7828 2244 5322 2c20 7329  d_regex("DS", s)
+00006fb0: 5b30 5d0a 0a0a 6465 6620 666f 726d 6174  [0]...def format
+00006fc0: 5f6e 756d 6265 725f 6173 5f64 7328 7661  _number_as_ds(va
+00006fd0: 6c3a 2055 6e69 6f6e 5b66 6c6f 6174 2c20  l: Union[float, 
+00006fe0: 4465 6369 6d61 6c5d 2920 2d3e 2073 7472  Decimal]) -> str
+00006ff0: 3a0a 2020 2020 2222 2254 7275 6e63 6174  :.    """Truncat
+00007000: 6520 6120 666c 6f61 7427 7320 7265 7072  e a float's repr
+00007010: 6573 656e 7461 7469 6f6e 2074 6f20 6769  esentation to gi
+00007020: 7665 2061 2076 616c 6964 2044 6563 696d  ve a valid Decim
+00007030: 616c 2053 7472 696e 6720 2844 5329 2e0a  al String (DS)..
+00007040: 0a20 2020 2044 4943 4f4d 2773 2064 6563  .    DICOM's dec
+00007050: 696d 616c 2073 7472 696e 6720 2844 5329  imal string (DS)
+00007060: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00007070: 6973 206c 696d 6974 6564 2074 6f20 7374  is limited to st
+00007080: 7269 6e67 7320 7769 7468 2031 360a 2020  rings with 16.  
+00007090: 2020 6368 6172 6163 7465 7273 2061 6e64    characters and
+000070a0: 2061 206c 696d 6974 6564 2073 6574 206f   a limited set o
+000070b0: 6620 6368 6172 6163 7465 7273 2e20 5468  f characters. Th
+000070c0: 6973 2066 756e 6374 696f 6e20 7265 7072  is function repr
+000070d0: 6573 656e 7473 2061 0a20 2020 2066 6c6f  esents a.    flo
+000070e0: 6174 2074 6861 7420 7361 7469 7366 6965  at that satisfie
+000070f0: 7320 7468 6573 6520 636f 6e73 7472 6169  s these constrai
+00007100: 6e74 7320 7768 696c 6520 7265 7461 696e  nts while retain
+00007110: 696e 6720 6173 206d 7563 680a 2020 2020  ing as much.    
+00007120: 7072 6563 6973 696f 6e20 6173 2070 6f73  precision as pos
+00007130: 7369 626c 652e 2053 6f6d 6520 666c 6f61  sible. Some floa
+00007140: 7473 2061 7265 2072 6570 7265 7365 6e74  ts are represent
+00007150: 6564 2075 7369 6e67 2073 6369 656e 7469  ed using scienti
+00007160: 6669 630a 2020 2020 6e6f 7461 7469 6f6e  fic.    notation
+00007170: 2074 6f20 6d61 6b65 206d 6f72 6520 6566   to make more ef
+00007180: 6669 6369 656e 7420 7573 6520 6f66 2074  ficient use of t
+00007190: 6865 206c 696d 6974 6564 206e 756d 6265  he limited numbe
+000071a0: 7220 6f66 2063 6861 7261 6374 6572 732e  r of characters.
+000071b0: 0a0a 2020 2020 4e6f 7465 2074 6861 7420  ..    Note that 
+000071c0: 7468 6973 2077 696c 6c20 696e 6375 7220  this will incur 
+000071d0: 6120 6c6f 7373 206f 6620 7072 6563 6973  a loss of precis
+000071e0: 696f 6e20 6966 2074 6865 206e 756d 6265  ion if the numbe
+000071f0: 7220 6361 6e6e 6f74 2062 650a 2020 2020  r cannot be.    
+00007200: 7265 7072 6573 656e 7465 6420 7769 7468  represented with
+00007210: 2031 3620 6368 6172 6163 7465 7273 2e20   16 characters. 
+00007220: 4675 7274 6865 726d 6f72 652c 206e 6f6e  Furthermore, non
+00007230: 2d66 696e 6974 6520 666c 6f61 7473 2028  -finite floats (
+00007240: 696e 6673 2061 6e64 0a20 2020 206e 616e  infs and.    nan
+00007250: 7329 2063 616e 6e6f 7420 6265 2072 6570  s) cannot be rep
+00007260: 7265 7365 6e74 6564 2061 7320 6465 6369  resented as deci
+00007270: 6d61 6c20 7374 7269 6e67 7320 616e 6420  mal strings and 
+00007280: 7769 6c6c 2063 6175 7365 2061 6e20 6572  will cause an er
+00007290: 726f 7220 746f 0a20 2020 2062 6520 7261  ror to.    be ra
+000072a0: 6973 6564 2e0a 0a20 2020 2050 6172 616d  ised...    Param
+000072b0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000072c0: 2d2d 2d2d 0a20 2020 2076 616c 3a20 556e  ----.    val: Un
+000072d0: 696f 6e5b 666c 6f61 742c 2044 6563 696d  ion[float, Decim
+000072e0: 616c 5d0a 2020 2020 2020 2020 5468 6520  al].        The 
+000072f0: 666c 6f61 7469 6e67 2070 6f69 6e74 2076  floating point v
+00007300: 616c 7565 2077 686f 7365 2072 6570 7265  alue whose repre
+00007310: 7365 6e74 6174 696f 6e20 6973 2072 6571  sentation is req
+00007320: 7569 7265 642e 0a0a 2020 2020 5265 7475  uired...    Retu
+00007330: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00007340: 2020 2020 7374 720a 2020 2020 2020 2020      str.        
+00007350: 5374 7269 6e67 2072 6570 7265 7365 6e74  String represent
+00007360: 6174 696f 6e20 6f66 2074 6865 2066 6c6f  ation of the flo
+00007370: 6174 2073 6174 6973 6679 696e 6720 7468  at satisfying th
+00007380: 6520 636f 6e73 7472 6169 6e74 7320 6f66  e constraints of
+00007390: 2074 6865 0a20 2020 2020 2020 2064 6563   the.        dec
+000073a0: 696d 616c 2073 7472 696e 6720 7265 7072  imal string repr
+000073b0: 6573 656e 7461 7469 6f6e 2e0a 0a20 2020  esentation...   
+000073c0: 2052 6169 7365 730a 2020 2020 2d2d 2d2d   Raises.    ----
+000073d0: 2d2d 0a20 2020 2056 616c 7565 4572 726f  --.    ValueErro
+000073e0: 720a 2020 2020 2020 2020 4966 2076 616c  r.        If val
+000073f0: 2064 6f65 7320 6e6f 7420 7265 7072 6573   does not repres
+00007400: 656e 7420 6120 6669 6e69 7465 2076 616c  ent a finite val
+00007410: 7565 0a0a 2020 2020 2222 220a 2020 2020  ue..    """.    
+00007420: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00007430: 6528 7661 6c2c 2028 666c 6f61 742c 2044  e(val, (float, D
+00007440: 6563 696d 616c 2929 3a0a 2020 2020 2020  ecimal)):.      
+00007450: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+00007460: 7228 2227 7661 6c27 206d 7573 7420 6265  r("'val' must be
+00007470: 206f 6620 7479 7065 2066 6c6f 6174 206f   of type float o
+00007480: 7220 6465 6369 6d61 6c2e 4465 6369 6d61  r decimal.Decima
+00007490: 6c22 290a 2020 2020 6966 206e 6f74 2069  l").    if not i
+000074a0: 7366 696e 6974 6528 7661 6c29 3a0a 2020  sfinite(val):.  
+000074b0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000074c0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+000074d0: 2020 2020 2243 616e 6e6f 7420 656e 636f      "Cannot enco
+000074e0: 6465 206e 6f6e 2d66 696e 6974 6520 666c  de non-finite fl
+000074f0: 6f61 7473 2061 7320 4449 434f 4d20 6465  oats as DICOM de
+00007500: 6369 6d61 6c20 7374 7269 6e67 732e 2022  cimal strings. "
+00007510: 0a20 2020 2020 2020 2020 2020 2066 2247  .            f"G
+00007520: 6f74 2027 7b76 616c 7d27 220a 2020 2020  ot '{val}'".    
+00007530: 2020 2020 290a 0a20 2020 2076 616c 7374      )..    valst
+00007540: 7220 3d20 7374 7228 7661 6c29 0a0a 2020  r = str(val)..  
+00007550: 2020 2320 496e 2074 6865 2073 696d 706c    # In the simpl
+00007560: 6520 6361 7365 2c20 7468 6520 6465 6661  e case, the defa
+00007570: 756c 7420 7079 7468 6f6e 2073 7472 696e  ult python strin
+00007580: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
+00007590: 0a20 2020 2023 2077 696c 6c20 646f 0a20  .    # will do. 
+000075a0: 2020 2069 6620 6c65 6e28 7661 6c73 7472     if len(valstr
+000075b0: 2920 3c3d 2031 363a 0a20 2020 2020 2020  ) <= 16:.       
+000075c0: 2072 6574 7572 6e20 7661 6c73 7472 0a0a   return valstr..
+000075d0: 2020 2020 2320 4465 6369 6465 2077 6865      # Decide whe
+000075e0: 7468 6572 2074 6f20 7573 6520 7363 6965  ther to use scie
+000075f0: 6e74 6966 6963 206e 6f74 6174 696f 6e0a  ntific notation.
+00007600: 2020 2020 6c6f 6776 616c 203d 206c 6f67      logval = log
+00007610: 3130 2863 6173 7428 556e 696f 6e5b 666c  10(cast(Union[fl
+00007620: 6f61 742c 2044 6563 696d 616c 5d2c 2061  oat, Decimal], a
+00007630: 6273 2876 616c 2929 290a 0a20 2020 2023  bs(val)))..    #
+00007640: 2043 6861 7261 6374 6572 7320 6e65 6564   Characters need
+00007650: 6564 2066 6f72 2027 2d27 2061 7420 7374  ed for '-' at st
+00007660: 6172 740a 2020 2020 7369 676e 5f63 6861  art.    sign_cha
+00007670: 7273 203d 2031 2069 6620 7661 6c20 3c20  rs = 1 if val < 
+00007680: 302e 3020 656c 7365 2030 0a0a 2020 2020  0.0 else 0..    
+00007690: 2320 4e75 6d62 6572 7320 6c61 7267 6572  # Numbers larger
+000076a0: 2074 6861 6e20 3165 3134 2063 616e 6e6f   than 1e14 canno
+000076b0: 7420 6265 2063 6f72 7265 6374 6c79 2072  t be correctly r
+000076c0: 6570 7265 7365 6e74 6564 2062 7920 7472  epresented by tr
+000076d0: 756e 6361 7469 6e67 0a20 2020 2023 2074  uncating.    # t
+000076e0: 6865 6972 2073 7472 696e 6720 7265 7072  heir string repr
+000076f0: 6573 656e 7461 7469 6f6e 7320 746f 2031  esentations to 1
+00007700: 3620 6368 6172 732c 2065 2e67 2070 6920  6 chars, e.g pi 
+00007710: 2a20 3130 5e31 3320 776f 756c 6420 6265  * 10^13 would be
+00007720: 636f 6d65 0a20 2020 2023 2027 3331 3431  come.    # '3141
+00007730: 3539 3236 3533 3538 3937 392e 272c 2077  59265358979.', w
+00007740: 6869 6368 206d 6179 206e 6f74 2062 6520  hich may not be 
+00007750: 756e 6976 6572 7361 6c6c 7920 756e 6465  universally unde
+00007760: 7273 746f 6f64 2e20 5468 6973 206c 696d  rstood. This lim
+00007770: 6974 0a20 2020 2023 2069 7320 3165 3133  it.    # is 1e13
+00007780: 2066 6f72 206e 6567 6174 6976 6520 6e75   for negative nu
+00007790: 6d62 6572 7320 6265 6361 7573 6520 6f66  mbers because of
+000077a0: 2074 6865 206d 696e 7573 2073 6967 6e2e   the minus sign.
+000077b0: 0a20 2020 2023 2046 6f72 206e 6567 6174  .    # For negat
+000077c0: 6976 6520 6578 706f 6e65 6e74 732c 2074  ive exponents, t
+000077d0: 6865 2070 6f69 6e74 206f 6620 6571 7561  he point of equa
+000077e0: 6c20 7072 6563 6973 696f 6e20 6265 7477  l precision betw
+000077f0: 6565 6e20 7363 6965 6e74 6966 6963 0a20  een scientific. 
+00007800: 2020 2023 2061 6e64 2073 7461 6e64 6172     # and standar
+00007810: 6420 6e6f 7461 7469 6f6e 2069 7320 3165  d notation is 1e
+00007820: 2d34 2065 2e67 2e20 2730 2e30 3030 3331  -4 e.g. '0.00031
+00007830: 3431 3539 3236 3533 3527 2061 6e64 0a20  415926535' and. 
+00007840: 2020 2023 2027 332e 3134 3135 3932 3635     # '3.14159265
+00007850: 3335 652d 3034 2720 6172 6520 626f 7468  35e-04' are both
+00007860: 2031 3620 6368 6172 730a 2020 2020 7573   16 chars.    us
+00007870: 655f 7363 6965 6e74 6966 6963 203d 206c  e_scientific = l
+00007880: 6f67 7661 6c20 3c20 2d34 206f 7220 6c6f  ogval < -4 or lo
+00007890: 6776 616c 203e 3d20 2831 3420 2d20 7369  gval >= (14 - si
+000078a0: 676e 5f63 6861 7273 290a 0a20 2020 2069  gn_chars)..    i
+000078b0: 6620 7573 655f 7363 6965 6e74 6966 6963  f use_scientific
+000078c0: 3a0a 2020 2020 2020 2020 2320 496e 2070  :.        # In p
+000078d0: 7269 6e63 6970 6c65 2c20 7765 2063 6f75  rinciple, we cou
+000078e0: 6c64 2068 6176 6520 6120 6e75 6d62 6572  ld have a number
+000078f0: 2077 6865 7265 2074 6865 2065 7870 6f6e   where the expon
+00007900: 656e 740a 2020 2020 2020 2020 2320 6e65  ent.        # ne
+00007910: 6564 7320 7468 7265 6520 6469 6769 7473  eds three digits
+00007920: 2074 6f20 6265 2072 6570 7265 7365 6e74   to be represent
+00007930: 6564 2028 6269 6767 6572 2074 6861 6e20  ed (bigger than 
+00007940: 7468 6973 2063 616e 6e6f 7420 6265 0a20  this cannot be. 
+00007950: 2020 2020 2020 2023 2072 6570 7265 7365         # represe
+00007960: 6e74 6564 2062 7920 666c 6f61 7473 292e  nted by floats).
+00007970: 2044 7565 2074 6f20 666c 6f61 7469 6e67   Due to floating
+00007980: 2070 6f69 6e74 206c 696d 6974 6174 696f   point limitatio
+00007990: 6e73 0a20 2020 2020 2020 2023 2074 6869  ns.        # thi
+000079a0: 7320 6973 2062 6573 7420 6368 6563 6b65  s is best checke
+000079b0: 6420 666f 7220 6279 2064 6f69 6e67 2074  d for by doing t
+000079c0: 6865 2073 7472 696e 6720 636f 6e76 6572  he string conver
+000079d0: 7369 6f6e 0a20 2020 2020 2020 2072 656d  sion.        rem
+000079e0: 6169 6e69 6e67 5f63 6861 7273 203d 2031  aining_chars = 1
+000079f0: 3020 2d20 7369 676e 5f63 6861 7273 0a20  0 - sign_chars. 
+00007a00: 2020 2020 2020 2074 7275 6e63 5f73 7472         trunc_str
+00007a10: 203d 2066 277b 7661 6c3a 2e7b 7265 6d61   = f'{val:.{rema
+00007a20: 696e 696e 675f 6368 6172 737d 657d 270a  ining_chars}e}'.
+00007a30: 2020 2020 2020 2020 6966 206c 656e 2874          if len(t
+00007a40: 7275 6e63 5f73 7472 2920 3e20 3136 3a0a  runc_str) > 16:.
+00007a50: 2020 2020 2020 2020 2020 2020 7472 756e              trun
+00007a60: 635f 7374 7220 3d20 6627 7b76 616c 3a2e  c_str = f'{val:.
+00007a70: 7b72 656d 6169 6e69 6e67 5f63 6861 7273  {remaining_chars
+00007a80: 202d 2031 7d65 7d27 0a20 2020 2020 2020   - 1}e}'.       
+00007a90: 2072 6574 7572 6e20 7472 756e 635f 7374   return trunc_st
+00007aa0: 720a 2020 2020 656c 7365 3a0a 2020 2020  r.    else:.    
+00007ab0: 2020 2020 6966 206c 6f67 7661 6c20 3e3d      if logval >=
+00007ac0: 2031 2e30 3a0a 2020 2020 2020 2020 2020   1.0:.          
+00007ad0: 2020 2320 6368 6172 7320 7265 6d61 696e    # chars remain
+00007ae0: 696e 6720 666f 7220 6469 6769 7473 2061  ing for digits a
+00007af0: 6674 6572 2073 6967 6e2c 2064 6967 6974  fter sign, digit
+00007b00: 7320 6c65 6674 206f 6620 272e 2720 616e  s left of '.' an
+00007b10: 6420 272e 270a 2020 2020 2020 2020 2020  d '.'.          
+00007b20: 2020 7265 6d61 696e 696e 675f 6368 6172    remaining_char
+00007b30: 7320 3d20 3134 202d 2073 6967 6e5f 6368  s = 14 - sign_ch
+00007b40: 6172 7320 2d20 696e 7428 666c 6f6f 7228  ars - int(floor(
+00007b50: 6c6f 6776 616c 2929 0a20 2020 2020 2020  logval)).       
+00007b60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007b70: 2020 2072 656d 6169 6e69 6e67 5f63 6861     remaining_cha
+00007b80: 7273 203d 2031 3420 2d20 7369 676e 5f63  rs = 14 - sign_c
+00007b90: 6861 7273 0a20 2020 2020 2020 2072 6574  hars.        ret
+00007ba0: 7572 6e20 6627 7b76 616c 3a2e 7b72 656d  urn f'{val:.{rem
+00007bb0: 6169 6e69 6e67 5f63 6861 7273 7d66 7d27  aining_chars}f}'
+00007bc0: 0a0a 0a63 6c61 7373 2044 5366 6c6f 6174  ...class DSfloat
+00007bd0: 2866 6c6f 6174 293a 0a20 2020 2022 2222  (float):.    """
+00007be0: 5374 6f72 6520 7661 6c75 6520 666f 7220  Store value for 
+00007bf0: 616e 2065 6c65 6d65 6e74 2077 6974 6820  an element with 
+00007c00: 5652 202a 2a44 532a 2a20 6173 203a 636c  VR **DS** as :cl
+00007c10: 6173 733a 6066 6c6f 6174 602e 0a0a 2020  ass:`float`...  
+00007c20: 2020 4966 2063 6f6e 7374 7275 6374 6564    If constructed
+00007c30: 2066 726f 6d20 616e 2065 6d70 7479 2073   from an empty s
+00007c40: 7472 696e 672c 2072 6574 7572 6e20 7468  tring, return th
+00007c50: 6520 656d 7074 7920 7374 7269 6e67 2c0a  e empty string,.
+00007c60: 2020 2020 6e6f 7420 616e 2069 6e73 7461      not an insta
+00007c70: 6e63 6520 6f66 2074 6869 7320 636c 6173  nce of this clas
+00007c80: 732e 0a0a 2020 2020 5061 7261 6d65 7465  s...    Paramete
+00007c90: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00007ca0: 2d0a 2020 2020 7661 6c3a 2055 6e69 6f6e  -.    val: Union
+00007cb0: 5b73 7472 2c20 696e 742c 2066 6c6f 6174  [str, int, float
+00007cc0: 2c20 4465 6369 6d61 6c5d 0a20 2020 2020  , Decimal].     
+00007cd0: 2020 2056 616c 7565 2074 6f20 7374 6f72     Value to stor
+00007ce0: 6520 6173 2061 2044 532e 0a20 2020 2061  e as a DS..    a
+00007cf0: 7574 6f5f 666f 726d 6174 3a20 626f 6f6c  uto_format: bool
+00007d00: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00007d10: 2c20 6175 746f 6d61 7469 6361 6c6c 7920  , automatically 
+00007d20: 666f 726d 6174 2074 6865 2073 7472 696e  format the strin
+00007d30: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
+00007d40: 206f 6620 7468 6973 0a20 2020 2020 2020   of this.       
+00007d50: 206e 756d 6265 7220 746f 2065 6e73 7572   number to ensur
+00007d60: 6520 6974 2073 6174 6973 6669 6573 2074  e it satisfies t
+00007d70: 6865 2063 6f6e 7374 7261 696e 7473 2069  he constraints i
+00007d80: 6e20 7468 6520 4449 434f 4d20 7374 616e  n the DICOM stan
+00007d90: 6461 7264 2e0a 2020 2020 2020 2020 4e6f  dard..        No
+00007da0: 7465 2074 6861 7420 7468 6973 2077 696c  te that this wil
+00007db0: 6c20 6c65 6164 2074 6f20 6c6f 7373 206f  l lead to loss o
+00007dc0: 6620 7072 6563 6973 696f 6e20 666f 7220  f precision for 
+00007dd0: 736f 6d65 206e 756d 6265 7273 2e0a 0a20  some numbers... 
+00007de0: 2020 2022 2222 0a20 2020 2061 7574 6f5f     """.    auto_
+00007df0: 666f 726d 6174 3a20 626f 6f6c 0a0a 2020  format: bool..  
+00007e00: 2020 6465 6620 5f5f 6e65 775f 5f28 2020    def __new__(  
+00007e10: 2320 7479 7065 3a20 6967 6e6f 7265 5b6d  # type: ignore[m
+00007e20: 6973 635d 0a20 2020 2020 2020 2063 6c73  isc].        cls
+00007e30: 3a20 5479 7065 5b22 4453 666c 6f61 7422  : Type["DSfloat"
+00007e40: 5d2c 0a20 2020 2020 2020 2076 616c 3a20  ],.        val: 
+00007e50: 556e 696f 6e5b 4e6f 6e65 2c20 7374 722c  Union[None, str,
+00007e60: 2069 6e74 2c20 666c 6f61 742c 2044 6563   int, float, Dec
+00007e70: 696d 616c 5d2c 0a20 2020 2020 2020 2061  imal],.        a
+00007e80: 7574 6f5f 666f 726d 6174 3a20 626f 6f6c  uto_format: bool
+00007e90: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+00007ea0: 2020 7661 6c69 6461 7469 6f6e 5f6d 6f64    validation_mod
+00007eb0: 653a 2069 6e74 203d 204e 6f6e 650a 2020  e: int = None.  
+00007ec0: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+00007ed0: 556e 696f 6e5b 7374 722c 2022 4453 666c  Union[str, "DSfl
+00007ee0: 6f61 7422 5d5d 3a0a 2020 2020 2020 2020  oat"]]:.        
+00007ef0: 6966 2076 616c 2069 7320 4e6f 6e65 3a0a  if val is None:.
+00007f00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00007f10: 726e 2076 616c 0a0a 2020 2020 2020 2020  rn val..        
+00007f20: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
+00007f30: 6c2c 2073 7472 2920 616e 6420 7661 6c2e  l, str) and val.
+00007f40: 7374 7269 7028 2920 3d3d 2027 273a 0a20  strip() == '':. 
+00007f50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007f60: 6e20 7661 6c0a 0a20 2020 2020 2020 2072  n val..        r
+00007f70: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
+00007f80: 6e65 775f 5f28 636c 732c 2076 616c 290a  new__(cls, val).
+00007f90: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00007fa0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00007fb0: 2076 616c 3a20 556e 696f 6e5b 7374 722c   val: Union[str,
+00007fc0: 2069 6e74 2c20 666c 6f61 742c 2044 6563   int, float, Dec
+00007fd0: 696d 616c 5d2c 0a20 2020 2020 2020 2061  imal],.        a
+00007fe0: 7574 6f5f 666f 726d 6174 3a20 626f 6f6c  uto_format: bool
+00007ff0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+00008000: 2020 7661 6c69 6461 7469 6f6e 5f6d 6f64    validation_mod
+00008010: 653a 2069 6e74 203d 204e 6f6e 650a 2020  e: int = None.  
+00008020: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+00008030: 2020 2020 2022 2222 5374 6f72 6520 7468       """Store th
+00008040: 6520 6f72 6967 696e 616c 2073 7472 696e  e original strin
+00008050: 6720 6966 206f 6e65 2067 6976 656e 2c20  g if one given, 
+00008060: 666f 7220 6578 6163 7420 7772 6974 652d  for exact write-
+00008070: 6f75 7420 6f66 2073 616d 650a 2020 2020  out of same.    
+00008080: 2020 2020 7661 6c75 6520 6c61 7465 722e      value later.
+00008090: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000080a0: 2020 2020 2069 6620 7661 6c69 6461 7469       if validati
+000080b0: 6f6e 5f6d 6f64 6520 6973 204e 6f6e 653a  on_mode is None:
+000080c0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+000080d0: 6964 6174 696f 6e5f 6d6f 6465 203d 2063  idation_mode = c
+000080e0: 6f6e 6669 672e 7365 7474 696e 6773 2e72  onfig.settings.r
+000080f0: 6561 6469 6e67 5f76 616c 6964 6174 696f  eading_validatio
+00008100: 6e5f 6d6f 6465 0a0a 2020 2020 2020 2020  n_mode..        
+00008110: 2320 2e2e 2e20 616c 736f 2069 6620 7573  # ... also if us
+00008120: 6572 2063 6861 6e67 6573 2061 2064 6174  er changes a dat
+00008130: 6120 656c 656d 656e 7420 7661 6c75 652c  a element value,
+00008140: 2074 6865 6e20 7769 6c6c 2067 6574 0a20   then will get. 
+00008150: 2020 2020 2020 2023 2061 2064 6966 6665         # a diffe
+00008160: 7265 6e74 206f 626a 6563 742c 2062 6563  rent object, bec
+00008170: 6175 7365 2066 6c6f 6174 2069 7320 696d  ause float is im
+00008180: 6d75 7461 626c 652e 0a20 2020 2020 2020  mutable..       
+00008190: 2068 6173 5f61 7474 7269 6275 7465 203d   has_attribute =
+000081a0: 2068 6173 6174 7472 2876 616c 2c20 276f   hasattr(val, 'o
+000081b0: 7269 6769 6e61 6c5f 7374 7269 6e67 2729  riginal_string')
+000081c0: 0a20 2020 2020 2020 2070 7265 5f63 6865  .        pre_che
+000081d0: 636b 6564 203d 2046 616c 7365 0a20 2020  cked = False.   
+000081e0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000081f0: 6365 2876 616c 2c20 7374 7229 3a0a 2020  ce(val, str):.  
+00008200: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+00008210: 7269 6769 6e61 6c5f 7374 7269 6e67 203d  riginal_string =
+00008220: 2076 616c 2e73 7472 6970 2829 0a20 2020   val.strip().   
+00008230: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00008240: 616e 6365 2876 616c 2c20 2844 5366 6c6f  ance(val, (DSflo
+00008250: 6174 2c20 4453 6465 6369 6d61 6c29 293a  at, DSdecimal)):
+00008260: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008270: 7661 6c2e 6175 746f 5f66 6f72 6d61 743a  val.auto_format:
+00008280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008290: 2061 7574 6f5f 666f 726d 6174 203d 2054   auto_format = T
+000082a0: 7275 6520 2023 206f 7665 7272 6964 6520  rue  # override 
+000082b0: 696e 7075 7420 7061 7261 6d65 7465 720a  input parameter.
+000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082d0: 7072 655f 6368 6563 6b65 6420 3d20 5472  pre_checked = Tr
+000082e0: 7565 0a20 2020 2020 2020 2020 2020 2069  ue.            i
+000082f0: 6620 6861 735f 6174 7472 6962 7574 653a  f has_attribute:
+00008300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008310: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
+00008320: 7472 696e 6720 3d20 7661 6c2e 6f72 6967  tring = val.orig
+00008330: 696e 616c 5f73 7472 696e 670a 0a20 2020  inal_string..   
+00008340: 2020 2020 2073 656c 662e 6175 746f 5f66       self.auto_f
+00008350: 6f72 6d61 7420 3d20 6175 746f 5f66 6f72  ormat = auto_for
+00008360: 6d61 740a 2020 2020 2020 2020 6966 2073  mat.        if s
+00008370: 656c 662e 6175 746f 5f66 6f72 6d61 7420  elf.auto_format 
+00008380: 616e 6420 6e6f 7420 7072 655f 6368 6563  and not pre_chec
+00008390: 6b65 643a 0a20 2020 2020 2020 2020 2020  ked:.           
+000083a0: 2023 2049 6620 6175 746f 5f66 6f72 6d61   # If auto_forma
+000083b0: 7420 6973 2054 7275 652c 206b 6565 7020  t is True, keep 
+000083c0: 7468 6520 666c 6f61 7420 7661 6c75 6520  the float value 
+000083d0: 7468 6520 7361 6d65 2c20 6275 7420 6368  the same, but ch
+000083e0: 616e 6765 0a20 2020 2020 2020 2020 2020  ange.           
+000083f0: 2023 2074 6865 2073 7472 696e 6720 7265   # the string re
+00008400: 7072 6573 656e 7461 7469 6f6e 2073 746f  presentation sto
+00008410: 7265 6420 696e 206f 7269 6769 6e61 6c5f  red in original_
+00008420: 7374 7269 6e67 2069 6620 6e65 6365 7373  string if necess
+00008430: 6172 790a 2020 2020 2020 2020 2020 2020  ary.            
+00008440: 6966 2068 6173 6174 7472 2873 656c 662c  if hasattr(self,
+00008450: 2027 6f72 6967 696e 616c 5f73 7472 696e   'original_strin
+00008460: 6727 293a 0a20 2020 2020 2020 2020 2020  g'):.           
+00008470: 2020 2020 2069 6620 6e6f 7420 6973 5f76       if not is_v
+00008480: 616c 6964 5f64 7328 7365 6c66 2e6f 7269  alid_ds(self.ori
+00008490: 6769 6e61 6c5f 7374 7269 6e67 293a 0a20  ginal_string):. 
+000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084b0: 2020 2073 656c 662e 6f72 6967 696e 616c     self.original
+000084c0: 5f73 7472 696e 6720 3d20 666f 726d 6174  _string = format
+000084d0: 5f6e 756d 6265 725f 6173 5f64 7328 0a20  _number_as_ds(. 
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
+00008500: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
+00008510: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00008520: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008530: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008550: 6f72 6967 696e 616c 5f73 7472 696e 6720  original_string 
+00008560: 3d20 666f 726d 6174 5f6e 756d 6265 725f  = format_number_
+00008570: 6173 5f64 7328 7365 6c66 290a 0a20 2020  as_ds(self)..   
+00008580: 2020 2020 2069 6620 2876 616c 6964 6174       if (validat
+00008590: 696f 6e5f 6d6f 6465 203d 3d20 636f 6e66  ion_mode == conf
+000085a0: 6967 2e52 4149 5345 2061 6e64 0a20 2020  ig.RAISE and.   
+000085b0: 2020 2020 2020 2020 2020 2020 206e 6f74               not
+000085c0: 2073 656c 662e 6175 746f 5f66 6f72 6d61   self.auto_forma
+000085d0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000085e0: 6966 206c 656e 2873 7472 2873 656c 6629  if len(str(self)
+000085f0: 2920 3e20 3136 3a0a 2020 2020 2020 2020  ) > 16:.        
+00008600: 2020 2020 2020 2020 7261 6973 6520 4f76          raise Ov
+00008610: 6572 666c 6f77 4572 726f 7228 0a20 2020  erflowError(.   
+00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008630: 2022 5661 6c75 6573 2066 6f72 2065 6c65   "Values for ele
+00008640: 6d65 6e74 7320 7769 7468 2061 2056 5220  ments with a VR 
+00008650: 6f66 2027 4453 2720 6d75 7374 2062 6520  of 'DS' must be 
+00008660: 3c3d 2031 3620 220a 2020 2020 2020 2020  <= 16 ".        
+00008670: 2020 2020 2020 2020 2020 2020 2263 6861              "cha
+00008680: 7261 6374 6572 7320 6c6f 6e67 2c20 6275  racters long, bu
+00008690: 7420 7468 6520 666c 6f61 7420 7072 6f76  t the float prov
+000086a0: 6964 6564 2072 6571 7569 7265 7320 3e20  ided requires > 
+000086b0: 3136 2022 0a20 2020 2020 2020 2020 2020  16 ".           
+000086c0: 2020 2020 2020 2020 2022 6368 6172 6163           "charac
+000086d0: 7465 7273 2074 6f20 6265 2061 6363 7572  ters to be accur
+000086e0: 6174 656c 7920 7265 7072 6573 656e 7465  ately represente
+000086f0: 642e 2055 7365 2061 2073 6d61 6c6c 6572  d. Use a smaller
+00008700: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00008710: 2020 2020 2020 2022 7374 7269 6e67 2c20         "string, 
+00008720: 7365 7420 2763 6f6e 6669 672e 7365 7474  set 'config.sett
+00008730: 696e 6773 2e72 6561 6469 6e67 5f76 616c  ings.reading_val
+00008740: 6964 6174 696f 6e5f 6d6f 6465 2720 746f  idation_mode' to
+00008750: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00008760: 2020 2020 2020 2022 2757 4152 4e27 2074         "'WARN' t
+00008770: 6f20 6f76 6572 7269 6465 2074 6865 206c  o override the l
+00008780: 656e 6774 6820 6368 6563 6b2c 206f 7220  ength check, or 
+00008790: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000087a0: 2020 2020 2020 2265 7870 6c69 6369 746c        "explicitl
+000087b0: 7920 636f 6e73 7472 7563 7420 6120 4453  y construct a DS
+000087c0: 206f 626a 6563 7420 7769 7468 2027 6175   object with 'au
+000087d0: 746f 5f66 6f72 6d61 7427 2022 0a20 2020  to_format' ".   
+000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087f0: 2022 7365 7420 746f 2054 7275 6522 0a20   "set to True". 
+00008800: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00008810: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008820: 6e6f 7420 6973 5f76 616c 6964 5f64 7328  not is_valid_ds(
+00008830: 7374 7228 7365 6c66 2929 3a0a 2020 2020  str(self)):.    
+00008840: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+00008850: 6973 2077 696c 6c20 6361 7463 6820 6e61  is will catch na
+00008860: 6e20 616e 6420 696e 660a 2020 2020 2020  n and inf.      
+00008870: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00008880: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088a0: 6627 5661 6c75 6520 227b 7374 7228 7365  f'Value "{str(se
+000088b0: 6c66 297d 2220 6973 206e 6f74 2076 616c  lf)}" is not val
+000088c0: 6964 2066 6f72 2065 6c65 6d65 6e74 7320  id for elements 
+000088d0: 7769 7468 2061 2056 5220 270a 2020 2020  with a VR '.    
+000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088f0: 276f 6620 4453 270a 2020 2020 2020 2020  'of DS'.        
+00008900: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00008910: 6566 205f 5f65 715f 5f28 7365 6c66 2c20  ef __eq__(self, 
+00008920: 6f74 6865 723a 2041 6e79 2920 2d3e 2041  other: Any) -> A
+00008930: 6e79 3a0a 2020 2020 2020 2020 2222 224f  ny:.        """O
+00008940: 7665 7272 6964 6520 746f 2061 6c6c 6f77  verride to allow
+00008950: 2073 7472 696e 6720 6571 7561 6c69 7479   string equality
+00008960: 2063 6f6d 7061 7269 736f 6e73 2e22 2222   comparisons."""
+00008970: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00008980: 7374 616e 6365 286f 7468 6572 2c20 7374  stance(other, st
+00008990: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000089a0: 7265 7475 726e 2073 7472 2873 656c 6629  return str(self)
+000089b0: 203d 3d20 6f74 6865 720a 0a20 2020 2020   == other..     
+000089c0: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+000089d0: 292e 5f5f 6571 5f5f 286f 7468 6572 290a  ).__eq__(other).
+000089e0: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
+000089f0: 5f28 7365 6c66 2920 2d3e 2069 6e74 3a0a  _(self) -> int:.
+00008a00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00008a10: 7570 6572 2829 2e5f 5f68 6173 685f 5f28  uper().__hash__(
+00008a20: 290a 0a20 2020 2064 6566 205f 5f6e 655f  )..    def __ne_
+00008a30: 5f28 7365 6c66 2c20 6f74 6865 723a 2041  _(self, other: A
+00008a40: 6e79 2920 2d3e 2041 6e79 3a0a 2020 2020  ny) -> Any:.    
+00008a50: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+00008a60: 656c 6620 3d3d 206f 7468 6572 0a0a 2020  elf == other..  
+00008a70: 2020 6465 6620 5f5f 7374 725f 5f28 7365    def __str__(se
+00008a80: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+00008a90: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
+00008aa0: 656c 662c 2027 6f72 6967 696e 616c 5f73  elf, 'original_s
+00008ab0: 7472 696e 6727 2920 616e 6420 6e6f 7420  tring') and not 
+00008ac0: 7365 6c66 2e61 7574 6f5f 666f 726d 6174  self.auto_format
+00008ad0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00008ae0: 7475 726e 2073 656c 662e 6f72 6967 696e  turn self.origin
+00008af0: 616c 5f73 7472 696e 670a 0a20 2020 2020  al_string..     
+00008b00: 2020 2023 2049 7373 7565 2023 3933 3720     # Issue #937 
+00008b10: 2850 7974 686f 6e20 332e 3820 636f 6d70  (Python 3.8 comp
+00008b20: 6174 6962 696c 6974 7929 0a20 2020 2020  atibility).     
+00008b30: 2020 2072 6574 7572 6e20 7265 7072 2873     return repr(s
+00008b40: 656c 6629 5b31 3a2d 315d 0a0a 2020 2020  elf)[1:-1]..    
+00008b50: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+00008b60: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+00008b70: 2020 2069 6620 7365 6c66 2e61 7574 6f5f     if self.auto_
+00008b80: 666f 726d 6174 2061 6e64 2068 6173 6174  format and hasat
+00008b90: 7472 2873 656c 662c 2027 6f72 6967 696e  tr(self, 'origin
+00008ba0: 616c 5f73 7472 696e 6727 293a 0a20 2020  al_string'):.   
+00008bb0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008bc0: 6622 277b 7365 6c66 2e6f 7269 6769 6e61  f"'{self.origina
+00008bd0: 6c5f 7374 7269 6e67 7d27 220a 0a20 2020  l_string}'"..   
+00008be0: 2020 2020 2072 6574 7572 6e20 6622 277b       return f"'{
+00008bf0: 7375 7065 7228 292e 5f5f 7265 7072 5f5f  super().__repr__
+00008c00: 2829 7d27 220a 0a0a 636c 6173 7320 4453  ()}'"...class DS
+00008c10: 6465 6369 6d61 6c28 4465 6369 6d61 6c29  decimal(Decimal)
+00008c20: 3a0a 2020 2020 2222 2253 746f 7265 2076  :.    """Store v
+00008c30: 616c 7565 2066 6f72 2061 6e20 656c 656d  alue for an elem
+00008c40: 656e 7420 7769 7468 2056 5220 2a2a 4453  ent with VR **DS
+00008c50: 2a2a 2061 7320 3a63 6c61 7373 3a60 6465  ** as :class:`de
+00008c60: 6369 6d61 6c2e 4465 6369 6d61 6c60 2e0a  cimal.Decimal`..
+00008c70: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00008c80: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00008c90: 2020 2076 616c 3a20 556e 696f 6e5b 7374     val: Union[st
+00008ca0: 722c 2069 6e74 2c20 666c 6f61 742c 2044  r, int, float, D
+00008cb0: 6563 696d 616c 5d0a 2020 2020 2020 2020  ecimal].        
+00008cc0: 5661 6c75 6520 746f 2073 746f 7265 2061  Value to store a
+00008cd0: 7320 6120 4453 2e0a 2020 2020 6175 746f  s a DS..    auto
+00008ce0: 5f66 6f72 6d61 743a 2062 6f6f 6c0a 2020  _format: bool.  
+00008cf0: 2020 2020 2020 4966 2054 7275 652c 2061        If True, a
+00008d00: 7574 6f6d 6174 6963 616c 6c79 2066 6f72  utomatically for
+00008d10: 6d61 7420 7468 6520 7374 7269 6e67 2072  mat the string r
+00008d20: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00008d30: 2074 6869 730a 2020 2020 2020 2020 6e75   this.        nu
+00008d40: 6d62 6572 2074 6f20 656e 7375 7265 2069  mber to ensure i
+00008d50: 7420 7361 7469 7366 6965 7320 7468 6520  t satisfies the 
+00008d60: 636f 6e73 7472 6169 6e74 7320 696e 2074  constraints in t
+00008d70: 6865 2044 4943 4f4d 2073 7461 6e64 6172  he DICOM standar
+00008d80: 642e 0a20 2020 2020 2020 204e 6f74 6520  d..        Note 
+00008d90: 7468 6174 2074 6869 7320 7769 6c6c 206c  that this will l
+00008da0: 6561 6420 746f 206c 6f73 7320 6f66 2070  ead to loss of p
+00008db0: 7265 6369 7369 6f6e 2066 6f72 2073 6f6d  recision for som
+00008dc0: 6520 6e75 6d62 6572 732e 0a0a 2020 2020  e numbers...    
+00008dd0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+00008de0: 2020 2020 4966 2063 6f6e 7374 7275 6374      If construct
+00008df0: 6564 2066 726f 6d20 616e 2065 6d70 7479  ed from an empty
+00008e00: 2073 7472 696e 672c 2072 6574 7572 6e73   string, returns
+00008e10: 2074 6865 2065 6d70 7479 2073 7472 696e   the empty strin
+00008e20: 672c 206e 6f74 2061 6e0a 2020 2020 696e  g, not an.    in
+00008e30: 7374 616e 6365 206f 6620 7468 6973 2063  stance of this c
+00008e40: 6c61 7373 2e0a 0a20 2020 2022 2222 0a20  lass...    """. 
+00008e50: 2020 2061 7574 6f5f 666f 726d 6174 3a20     auto_format: 
+00008e60: 626f 6f6c 0a0a 2020 2020 6465 6620 5f5f  bool..    def __
+00008e70: 6e65 775f 5f28 2020 2320 7479 7065 3a20  new__(  # type: 
+00008e80: 6967 6e6f 7265 5b6d 6973 635d 0a20 2020  ignore[misc].   
+00008e90: 2020 2020 2063 6c73 3a20 5479 7065 5b22       cls: Type["
+00008ea0: 4453 6465 6369 6d61 6c22 5d2c 0a20 2020  DSdecimal"],.   
+00008eb0: 2020 2020 2076 616c 3a20 556e 696f 6e5b       val: Union[
+00008ec0: 4e6f 6e65 2c20 7374 722c 2069 6e74 2c20  None, str, int, 
+00008ed0: 666c 6f61 742c 2044 6563 696d 616c 5d2c  float, Decimal],
+00008ee0: 0a20 2020 2020 2020 2061 7574 6f5f 666f  .        auto_fo
+00008ef0: 726d 6174 3a20 626f 6f6c 203d 2046 616c  rmat: bool = Fal
+00008f00: 7365 2c0a 2020 2020 2020 2020 7661 6c69  se,.        vali
+00008f10: 6461 7469 6f6e 5f6d 6f64 653a 2069 6e74  dation_mode: int
+00008f20: 203d 204e 6f6e 650a 2020 2020 2920 2d3e   = None.    ) ->
+00008f30: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+00008f40: 7374 722c 2022 4453 6465 6369 6d61 6c22  str, "DSdecimal"
+00008f50: 5d5d 3a0a 2020 2020 2020 2020 2222 2243  ]]:.        """C
+00008f60: 7265 6174 6520 616e 2069 6e73 7461 6e63  reate an instanc
+00008f70: 6520 6f66 2044 5320 6f62 6a65 6374 2c20  e of DS object, 
+00008f80: 6f72 2072 6574 7572 6e20 6120 626c 616e  or return a blan
+00008f90: 6b20 7374 7269 6e67 2069 6620 6f6e 6520  k string if one 
+00008fa0: 6973 0a20 2020 2020 2020 2070 6173 7365  is.        passe
+00008fb0: 6420 696e 2c20 652e 672e 2066 726f 6d20  d in, e.g. from 
+00008fc0: 6120 7479 7065 2032 2044 4943 4f4d 2062  a type 2 DICOM b
+00008fd0: 6c61 6e6b 2076 616c 7565 2e0a 0a20 2020  lank value...   
+00008fe0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00008ff0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00009000: 2d2d 0a20 2020 2020 2020 2076 616c 203a  --.        val :
+00009010: 2073 7472 206f 7220 6e75 6d65 7269 630a   str or numeric.
+00009020: 2020 2020 2020 2020 2020 2020 4120 7374              A st
+00009030: 7269 6e67 206f 7220 6120 6e75 6d62 6572  ring or a number
+00009040: 2074 7970 6520 7768 6963 6820 6361 6e20   type which can 
+00009050: 6265 2063 6f6e 7665 7274 6564 2074 6f20  be converted to 
+00009060: 6120 6465 6369 6d61 6c2e 0a20 2020 2020  a decimal..     
+00009070: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00009080: 6620 7661 6c20 6973 204e 6f6e 653a 0a20  f val is None:. 
+00009090: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000090a0: 6e20 7661 6c0a 0a20 2020 2020 2020 2069  n val..        i
+000090b0: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
+000090c0: 2c20 7374 7229 2061 6e64 2076 616c 2e73  , str) and val.s
+000090d0: 7472 6970 2829 203d 3d20 2727 3a0a 2020  trip() == '':.  
+000090e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000090f0: 2076 616c 0a0a 2020 2020 2020 2020 6966   val..        if
+00009100: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
+00009110: 2066 6c6f 6174 2920 616e 6420 6e6f 7420   float) and not 
+00009120: 636f 6e66 6967 2e61 6c6c 6f77 5f44 535f  config.allow_DS_
+00009130: 666c 6f61 743a 0a20 2020 2020 2020 2020  float:.         
+00009140: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00009150: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00009160: 2020 2020 2227 4453 2720 6361 6e6e 6f74      "'DS' cannot
+00009170: 2062 6520 696e 7374 616e 7469 6174 6564   be instantiated
+00009180: 2077 6974 6820 6120 666c 6f61 7420 7661   with a float va
+00009190: 6c75 6520 756e 6c65 7373 2022 0a20 2020  lue unless ".   
+000091a0: 2020 2020 2020 2020 2020 2020 2022 2763               "'c
+000091b0: 6f6e 6669 672e 616c 6c6f 775f 4453 5f66  onfig.allow_DS_f
+000091c0: 6c6f 6174 2720 6973 2073 6574 2074 6f20  loat' is set to 
+000091d0: 5472 7565 2e20 596f 7520 7368 6f75 6c64  True. You should
+000091e0: 2063 6f6e 7665 7274 2022 0a20 2020 2020   convert ".     
+000091f0: 2020 2020 2020 2020 2020 2022 7468 6520             "the 
+00009200: 7661 6c75 6520 746f 2061 2073 7472 696e  value to a strin
+00009210: 6720 7769 7468 2074 6865 2064 6573 6972  g with the desir
+00009220: 6564 206e 756d 6265 7220 6f66 2064 6967  ed number of dig
+00009230: 6974 732c 2022 0a20 2020 2020 2020 2020  its, ".         
+00009240: 2020 2020 2020 2022 6f72 2075 7365 2027         "or use '
+00009250: 4465 6369 6d61 6c2e 7175 616e 7469 7a65  Decimal.quantize
+00009260: 2829 2720 616e 6420 7061 7373 2061 2027  ()' and pass a '
+00009270: 4465 6369 6d61 6c27 2069 6e73 7461 6e63  Decimal' instanc
+00009280: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
+00009290: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000092a0: 6e20 7375 7065 7228 292e 5f5f 6e65 775f  n super().__new_
+000092b0: 5f28 636c 732c 2076 616c 290a 0a20 2020  _(cls, val)..   
+000092c0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000092d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000092e0: 2020 2020 2076 616c 3a20 556e 696f 6e5b       val: Union[
+000092f0: 7374 722c 2069 6e74 2c20 666c 6f61 742c  str, int, float,
+00009300: 2044 6563 696d 616c 5d2c 0a20 2020 2020   Decimal],.     
+00009310: 2020 2061 7574 6f5f 666f 726d 6174 3a20     auto_format: 
+00009320: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00009330: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00009340: 5f6d 6f64 653a 2069 6e74 203d 204e 6f6e  _mode: int = Non
+00009350: 650a 2020 2020 2920 2d3e 204e 6f6e 653a  e.    ) -> None:
+00009360: 0a20 2020 2020 2020 2022 2222 5374 6f72  .        """Stor
+00009370: 6520 7468 6520 6f72 6967 696e 616c 2073  e the original s
+00009380: 7472 696e 6720 6966 206f 6e65 2067 6976  tring if one giv
+00009390: 656e 2c20 666f 7220 6578 6163 7420 7772  en, for exact wr
+000093a0: 6974 652d 6f75 7420 6f66 2073 616d 650a  ite-out of same.
+000093b0: 2020 2020 2020 2020 7661 6c75 6520 6c61          value la
+000093c0: 7465 722e 2045 2e67 2e20 6966 2073 6574  ter. E.g. if set
+000093d0: 2060 6027 312e 3233 6532 2760 602c 203a   ``'1.23e2'``, :
+000093e0: 636c 6173 733a 607e 6465 6369 6d61 6c2e  class:`~decimal.
+000093f0: 4465 6369 6d61 6c60 2077 6f75 6c64 0a20  Decimal` would. 
+00009400: 2020 2020 2020 2077 7269 7465 2060 6027         write ``'
+00009410: 3132 3327 6060 2c20 6275 7420 3a63 6c61  123'``, but :cla
+00009420: 7373 3a60 4453 6020 7769 6c6c 2075 7365  ss:`DS` will use
+00009430: 2074 6865 206f 7269 6769 6e61 6c2e 0a20   the original.. 
+00009440: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00009450: 2020 2069 6620 7661 6c69 6461 7469 6f6e     if validation
+00009460: 5f6d 6f64 6520 6973 204e 6f6e 653a 0a20  _mode is None:. 
+00009470: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+00009480: 6174 696f 6e5f 6d6f 6465 203d 2063 6f6e  ation_mode = con
+00009490: 6669 672e 7365 7474 696e 6773 2e72 6561  fig.settings.rea
+000094a0: 6469 6e67 5f76 616c 6964 6174 696f 6e5f  ding_validation_
+000094b0: 6d6f 6465 0a0a 2020 2020 2020 2020 2320  mode..        # 
+000094c0: 2e2e 2e20 616c 736f 2069 6620 7573 6572  ... also if user
+000094d0: 2063 6861 6e67 6573 2061 2064 6174 6120   changes a data 
+000094e0: 656c 656d 656e 7420 7661 6c75 652c 2074  element value, t
+000094f0: 6865 6e20 7769 6c6c 2067 6574 0a20 2020  hen will get.   
+00009500: 2020 2020 2023 2061 2064 6966 6665 7265       # a differe
+00009510: 6e74 2044 6563 696d 616c 2c20 6173 2044  nt Decimal, as D
+00009520: 6563 696d 616c 2069 7320 696d 6d75 7461  ecimal is immuta
+00009530: 626c 652e 0a20 2020 2020 2020 2070 7265  ble..        pre
+00009540: 5f63 6865 636b 6564 203d 2046 616c 7365  _checked = False
+00009550: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00009560: 7374 616e 6365 2876 616c 2c20 7374 7229  stance(val, str)
+00009570: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009580: 6c66 2e6f 7269 6769 6e61 6c5f 7374 7269  lf.original_stri
+00009590: 6e67 203d 2076 616c 2e73 7472 6970 2829  ng = val.strip()
+000095a0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+000095b0: 696e 7374 616e 6365 2876 616c 2c20 2844  instance(val, (D
+000095c0: 5366 6c6f 6174 2c20 4453 6465 6369 6d61  Sfloat, DSdecima
+000095d0: 6c29 293a 0a20 2020 2020 2020 2020 2020  l)):.           
+000095e0: 2069 6620 7661 6c2e 6175 746f 5f66 6f72   if val.auto_for
+000095f0: 6d61 743a 0a20 2020 2020 2020 2020 2020  mat:.           
+00009600: 2020 2020 2061 7574 6f5f 666f 726d 6174       auto_format
+00009610: 203d 2054 7275 6520 2023 206f 7665 7272   = True  # overr
+00009620: 6964 6520 696e 7075 7420 7061 7261 6d65  ide input parame
+00009630: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
+00009640: 2020 2020 7072 655f 6368 6563 6b65 6420      pre_checked 
+00009650: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
+00009660: 2020 2020 6966 2068 6173 6174 7472 2876      if hasattr(v
+00009670: 616c 2c20 276f 7269 6769 6e61 6c5f 7374  al, 'original_st
+00009680: 7269 6e67 2729 3a0a 2020 2020 2020 2020  ring'):.        
+00009690: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
+000096a0: 6769 6e61 6c5f 7374 7269 6e67 203d 2076  ginal_string = v
+000096b0: 616c 2e6f 7269 6769 6e61 6c5f 7374 7269  al.original_stri
+000096c0: 6e67 0a0a 2020 2020 2020 2020 7365 6c66  ng..        self
+000096d0: 2e61 7574 6f5f 666f 726d 6174 203d 2061  .auto_format = a
+000096e0: 7574 6f5f 666f 726d 6174 0a20 2020 2020  uto_format.     
+000096f0: 2020 2069 6620 7365 6c66 2e61 7574 6f5f     if self.auto_
+00009700: 666f 726d 6174 2061 6e64 206e 6f74 2070  format and not p
+00009710: 7265 5f63 6865 636b 6564 3a0a 2020 2020  re_checked:.    
+00009720: 2020 2020 2020 2020 2320 4966 2061 7574          # If aut
+00009730: 6f5f 666f 726d 6174 2069 7320 5472 7565  o_format is True
+00009740: 2c20 6b65 6570 2074 6865 2066 6c6f 6174  , keep the float
+00009750: 2076 616c 7565 2074 6865 2073 616d 652c   value the same,
+00009760: 2062 7574 2063 6861 6e67 650a 2020 2020   but change.    
+00009770: 2020 2020 2020 2020 2320 7468 6520 7374          # the st
+00009780: 7269 6e67 2072 6570 7265 7365 6e74 6174  ring representat
+00009790: 696f 6e20 7374 6f72 6564 2069 6e20 6f72  ion stored in or
+000097a0: 6967 696e 616c 5f73 7472 696e 6720 6966  iginal_string if
+000097b0: 206e 6563 6573 7361 7279 0a20 2020 2020   necessary.     
+000097c0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+000097d0: 7228 7365 6c66 2c20 276f 7269 6769 6e61  r(self, 'origina
+000097e0: 6c5f 7374 7269 6e67 2729 3a0a 2020 2020  l_string'):.    
+000097f0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00009800: 6f74 2069 735f 7661 6c69 645f 6473 2873  ot is_valid_ds(s
+00009810: 656c 662e 6f72 6967 696e 616c 5f73 7472  elf.original_str
+00009820: 696e 6729 3a0a 2020 2020 2020 2020 2020  ing):.          
+00009830: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+00009840: 7269 6769 6e61 6c5f 7374 7269 6e67 203d  riginal_string =
+00009850: 2066 6f72 6d61 745f 6e75 6d62 6572 5f61   format_number_a
+00009860: 735f 6473 280a 2020 2020 2020 2020 2020  s_ds(.          
+00009870: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00009880: 6f61 7428 7365 6c66 2e6f 7269 6769 6e61  oat(self.origina
+00009890: 6c5f 7374 7269 6e67 290a 2020 2020 2020  l_string).      
+000098a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000098b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000098c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000098d0: 2020 7365 6c66 2e6f 7269 6769 6e61 6c5f    self.original_
+000098e0: 7374 7269 6e67 203d 2066 6f72 6d61 745f  string = format_
+000098f0: 6e75 6d62 6572 5f61 735f 6473 2873 656c  number_as_ds(sel
+00009900: 6629 0a0a 2020 2020 2020 2020 6966 2076  f)..        if v
+00009910: 616c 6964 6174 696f 6e5f 6d6f 6465 2021  alidation_mode !
+00009920: 3d20 636f 6e66 6967 2e49 474e 4f52 453a  = config.IGNORE:
+00009930: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009940: 6c65 6e28 7265 7072 2873 656c 6629 2e73  len(repr(self).s
+00009950: 7472 6970 2822 2722 2929 203e 2031 363a  trip("'")) > 16:
+00009960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009970: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
+00009980: 2020 2020 2020 2020 2020 2020 2022 5661               "Va
+00009990: 6c75 6573 2066 6f72 2065 6c65 6d65 6e74  lues for element
+000099a0: 7320 7769 7468 2061 2056 5220 6f66 2027  s with a VR of '
+000099b0: 4453 2720 7661 6c75 6573 206d 7573 7420  DS' values must 
+000099c0: 6265 2022 0a20 2020 2020 2020 2020 2020  be ".           
+000099d0: 2020 2020 2020 2020 2022 3c3d 2031 3620           "<= 16 
+000099e0: 6368 6172 6163 7465 7273 206c 6f6e 672e  characters long.
+000099f0: 2055 7365 2061 2073 6d61 6c6c 6572 2073   Use a smaller s
+00009a00: 7472 696e 672c 2073 6574 2022 0a20 2020  tring, set ".   
+00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a20: 2022 2763 6f6e 6669 672e 7365 7474 696e   "'config.settin
+00009a30: 6773 2e72 6561 6469 6e67 5f76 616c 6964  gs.reading_valid
+00009a40: 6174 696f 6e5f 6d6f 6465 2720 746f 2022  ation_mode' to "
+00009a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a60: 2020 2020 2022 2757 4152 4e27 2074 6f20       "'WARN' to 
+00009a70: 6f76 6572 7269 6465 2074 6865 206c 656e  override the len
+00009a80: 6774 6820 6368 6563 6b2c 2075 7365 2022  gth check, use "
+00009a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009aa0: 2020 2020 2022 2744 6563 696d 616c 2e71       "'Decimal.q
+00009ab0: 7561 6e74 697a 6528 2927 2061 6e64 2069  uantize()' and i
+00009ac0: 6e69 7469 616c 697a 6520 220a 2020 2020  nitialize ".    
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ae0: 2277 6974 6820 6120 2744 6563 696d 616c  "with a 'Decimal
+00009af0: 2720 696e 7374 616e 6365 2c20 6f72 2065  ' instance, or e
+00009b00: 7870 6c69 6369 746c 7920 636f 6e73 7472  xplicitly constr
+00009b10: 7563 7420 6120 4453 2022 0a20 2020 2020  uct a DS ".     
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00009b30: 696e 7374 616e 6365 2077 6974 6820 2761  instance with 'a
+00009b40: 7574 6f5f 666f 726d 6174 2720 7365 7420  uto_format' set 
+00009b50: 746f 2054 7275 6522 0a20 2020 2020 2020  to True".       
+00009b60: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00009b70: 2020 2020 2020 2020 2020 2069 6620 7661             if va
+00009b80: 6c69 6461 7469 6f6e 5f6d 6f64 6520 3d3d  lidation_mode ==
+00009b90: 2063 6f6e 6669 672e 5241 4953 453a 0a20   config.RAISE:. 
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 2020 2072 6169 7365 204f 7665 7266 6c6f     raise Overflo
+00009bc0: 7745 7272 6f72 286d 7367 290a 2020 2020  wError(msg).    
+00009bd0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
+00009be0: 696e 6773 2e77 6172 6e28 6d73 6729 0a20  ings.warn(msg). 
+00009bf0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00009c00: 7420 6973 5f76 616c 6964 5f64 7328 7265  t is_valid_ds(re
+00009c10: 7072 2873 656c 6629 2e73 7472 6970 2822  pr(self).strip("
+00009c20: 2722 2929 3a0a 2020 2020 2020 2020 2020  '")):.          
+00009c30: 2020 2020 2020 2320 5468 6973 2077 696c        # This wil
+00009c40: 6c20 6361 7463 6820 6e61 6e20 616e 6420  l catch nan and 
+00009c50: 696e 660a 2020 2020 2020 2020 2020 2020  inf.            
+00009c60: 2020 2020 6d73 6720 3d20 280a 2020 2020      msg = (.    
+00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c80: 6627 5661 6c75 6520 227b 7374 7228 7365  f'Value "{str(se
+00009c90: 6c66 297d 2220 6973 206e 6f74 2076 616c  lf)}" is not val
+00009ca0: 6964 2066 6f72 2065 6c65 6d65 6e74 7320  id for elements 
+00009cb0: 7769 7468 2061 2056 5220 270a 2020 2020  with a VR '.    
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 276f 6620 4453 270a 2020 2020 2020 2020  'of DS'.        
+00009ce0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009cf0: 2020 2020 2020 2020 2020 6966 2076 616c            if val
+00009d00: 6964 6174 696f 6e5f 6d6f 6465 203d 3d20  idation_mode == 
+00009d10: 636f 6e66 6967 2e52 4149 5345 3a0a 2020  config.RAISE:.  
+00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d30: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00009d40: 6f72 286d 7367 290a 2020 2020 2020 2020  or(msg).        
+00009d50: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+00009d60: 2e77 6172 6e28 6d73 6729 0a0a 2020 2020  .warn(msg)..    
+00009d70: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
+00009d80: 206f 7468 6572 3a20 416e 7929 202d 3e20   other: Any) -> 
+00009d90: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
+00009da0: 4f76 6572 7269 6465 2074 6f20 616c 6c6f  Override to allo
+00009db0: 7720 7374 7269 6e67 2065 7175 616c 6974  w string equalit
+00009dc0: 7920 636f 6d70 6172 6973 6f6e 732e 2222  y comparisons.""
+00009dd0: 220a 2020 2020 2020 2020 6966 2069 7369  ".        if isi
+00009de0: 6e73 7461 6e63 6528 6f74 6865 722c 2073  nstance(other, s
+00009df0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00009e00: 2072 6574 7572 6e20 7374 7228 7365 6c66   return str(self
+00009e10: 2920 3d3d 206f 7468 6572 0a0a 2020 2020  ) == other..    
+00009e20: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00009e30: 2829 2e5f 5f65 715f 5f28 6f74 6865 7229  ().__eq__(other)
+00009e40: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
+00009e50: 5f5f 2873 656c 6629 202d 3e20 696e 743a  __(self) -> int:
+00009e60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009e70: 7375 7065 7228 292e 5f5f 6861 7368 5f5f  super().__hash__
+00009e80: 2829 0a0a 2020 2020 6465 6620 5f5f 6e65  ()..    def __ne
+00009e90: 5f5f 2873 656c 662c 206f 7468 6572 3a20  __(self, other: 
+00009ea0: 416e 7929 202d 3e20 416e 793a 0a20 2020  Any) -> Any:.   
+00009eb0: 2020 2020 2072 6574 7572 6e20 6e6f 7420       return not 
+00009ec0: 7365 6c66 203d 3d20 6f74 6865 720a 0a20  self == other.. 
+00009ed0: 2020 2064 6566 205f 5f73 7472 5f5f 2873     def __str__(s
+00009ee0: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+00009ef0: 2020 2020 2068 6173 5f73 7472 203d 2068       has_str = h
+00009f00: 6173 6174 7472 2873 656c 662c 2027 6f72  asattr(self, 'or
+00009f10: 6967 696e 616c 5f73 7472 696e 6727 290a  iginal_string').
+00009f20: 2020 2020 2020 2020 6966 2068 6173 5f73          if has_s
+00009f30: 7472 2061 6e64 206c 656e 2873 656c 662e  tr and len(self.
+00009f40: 6f72 6967 696e 616c 5f73 7472 696e 6729  original_string)
+00009f50: 203c 3d20 3136 3a0a 2020 2020 2020 2020   <= 16:.        
+00009f60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00009f70: 6f72 6967 696e 616c 5f73 7472 696e 670a  original_string.
+00009f80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009f90: 7375 7065 7228 292e 5f5f 7374 725f 5f28  super().__str__(
+00009fa0: 290a 0a20 2020 2064 6566 205f 5f72 6570  )..    def __rep
+00009fb0: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
+00009fc0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00009fd0: 662e 6175 746f 5f66 6f72 6d61 7420 616e  f.auto_format an
+00009fe0: 6420 6861 7361 7474 7228 7365 6c66 2c20  d hasattr(self, 
+00009ff0: 276f 7269 6769 6e61 6c5f 7374 7269 6e67  'original_string
+0000a000: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000a010: 7265 7475 726e 2066 2227 7b73 656c 662e  return f"'{self.
+0000a020: 6f72 6967 696e 616c 5f73 7472 696e 677d  original_string}
+0000a030: 2722 0a20 2020 2020 2020 2072 6574 7572  '".        retur
+0000a040: 6e20 6622 277b 7374 7228 7365 6c66 297d  n f"'{str(self)}
+0000a050: 2722 0a0a 0a23 2043 484f 4f53 4520 5459  '"...# CHOOSE TY
+0000a060: 5045 204f 4620 4453 0a44 5363 6c61 7373  PE OF DS.DSclass
+0000a070: 3a20 416e 790a 6966 2063 6f6e 6669 672e  : Any.if config.
+0000a080: 7573 655f 4453 5f64 6563 696d 616c 3a0a  use_DS_decimal:.
+0000a090: 2020 2020 4453 636c 6173 7320 3d20 4453      DSclass = DS
+0000a0a0: 6465 6369 6d61 6c0a 656c 7365 3a0a 2020  decimal.else:.  
+0000a0b0: 2020 4453 636c 6173 7320 3d20 4453 666c    DSclass = DSfl
+0000a0c0: 6f61 740a 0a0a 6465 6620 4453 280a 2020  oat...def DS(.  
+0000a0d0: 2020 7661 6c3a 2055 6e69 6f6e 5b4e 6f6e    val: Union[Non
+0000a0e0: 652c 2073 7472 2c20 696e 742c 2066 6c6f  e, str, int, flo
+0000a0f0: 6174 2c20 4465 6369 6d61 6c5d 2c20 6175  at, Decimal], au
+0000a100: 746f 5f66 6f72 6d61 743a 2062 6f6f 6c20  to_format: bool 
+0000a110: 3d20 4661 6c73 652c 0a20 2020 2076 616c  = False,.    val
+0000a120: 6964 6174 696f 6e5f 6d6f 6465 3a20 696e  idation_mode: in
+0000a130: 7420 3d20 4e6f 6e65 0a29 202d 3e20 556e  t = None.) -> Un
+0000a140: 696f 6e5b 4e6f 6e65 2c20 7374 722c 2044  ion[None, str, D
+0000a150: 5366 6c6f 6174 2c20 4453 6465 6369 6d61  Sfloat, DSdecima
+0000a160: 6c5d 3a0a 2020 2020 2222 2246 6163 746f  l]:.    """Facto
+0000a170: 7279 2066 756e 6374 696f 6e20 666f 7220  ry function for 
+0000a180: 6372 6561 7469 6e67 2044 5320 636c 6173  creating DS clas
+0000a190: 7320 696e 7374 616e 6365 732e 0a0a 2020  s instances...  
+0000a1a0: 2020 4368 6563 6b73 2066 6f72 2062 6c61    Checks for bla
+0000a1b0: 6e6b 2073 7472 696e 673b 2069 6620 736f  nk string; if so
+0000a1c0: 2c20 7265 7475 726e 7320 7468 6174 2c20  , returns that, 
+0000a1d0: 656c 7365 2063 616c 6c73 203a 636c 6173  else calls :clas
+0000a1e0: 733a 6044 5366 6c6f 6174 600a 2020 2020  s:`DSfloat`.    
+0000a1f0: 6f72 203a 636c 6173 733a 6044 5364 6563  or :class:`DSdec
+0000a200: 696d 616c 6020 746f 2063 7265 6174 6520  imal` to create 
+0000a210: 7468 6520 636c 6173 7320 696e 7374 616e  the class instan
+0000a220: 6365 2e20 5468 6973 2061 766f 6964 7320  ce. This avoids 
+0000a230: 6f76 6572 7269 6469 6e67 0a20 2020 2060  overriding.    `
+0000a240: 6044 5366 6c6f 6174 2e5f 5f6e 6577 5f5f  `DSfloat.__new__
+0000a250: 2829 6060 2028 7768 6963 6820 6361 7272  ()`` (which carr
+0000a260: 6965 7320 6120 7469 6d65 2070 656e 616c  ies a time penal
+0000a270: 7479 2066 6f72 206c 6172 6765 2061 7272  ty for large arr
+0000a280: 6179 7320 6f66 0a20 2020 2044 5329 2e0a  ays of.    DS)..
+0000a290: 0a20 2020 2053 696d 696c 6172 6c79 2074  .    Similarly t
+0000a2a0: 6865 2073 7472 696e 6720 636c 6561 6e20  he string clean 
+0000a2b0: 616e 6420 6368 6563 6b20 6361 6e20 6265  and check can be
+0000a2c0: 2061 766f 6964 6564 2061 6e64 203a 636c   avoided and :cl
+0000a2d0: 6173 733a 6044 5366 6c6f 6174 600a 2020  ass:`DSfloat`.  
+0000a2e0: 2020 6361 6c6c 6564 2064 6972 6563 746c    called directl
+0000a2f0: 7920 6966 2061 2073 7472 696e 6720 6861  y if a string ha
+0000a300: 7320 616c 7265 6164 7920 6265 656e 2070  s already been p
+0000a310: 726f 6365 7373 6564 2e0a 2020 2020 2222  rocessed..    ""
+0000a320: 220a 2020 2020 6966 2076 616c 2069 7320  ".    if val is 
+0000a330: 4e6f 6e65 3a0a 2020 2020 2020 2020 7265  None:.        re
+0000a340: 7475 726e 2076 616c 0a0a 2020 2020 6966  turn val..    if
+0000a350: 2076 616c 6964 6174 696f 6e5f 6d6f 6465   validation_mode
+0000a360: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000a370: 2020 7661 6c69 6461 7469 6f6e 5f6d 6f64    validation_mod
+0000a380: 6520 3d20 636f 6e66 6967 2e73 6574 7469  e = config.setti
+0000a390: 6e67 732e 7265 6164 696e 675f 7661 6c69  ngs.reading_vali
+0000a3a0: 6461 7469 6f6e 5f6d 6f64 650a 0a20 2020  dation_mode..   
+0000a3b0: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
+0000a3c0: 616c 2c20 7374 7229 3a0a 2020 2020 2020  al, str):.      
+0000a3d0: 2020 6966 2076 616c 2e73 7472 6970 2829    if val.strip()
+0000a3e0: 203d 3d20 2727 3a0a 2020 2020 2020 2020   == '':.        
+0000a3f0: 2020 2020 7265 7475 726e 2076 616c 0a20      return val. 
+0000a400: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
+0000a410: 7661 6c75 6528 2244 5322 2c20 7661 6c2c  value("DS", val,
+0000a420: 2076 616c 6964 6174 696f 6e5f 6d6f 6465   validation_mode
+0000a430: 290a 0a20 2020 2069 6620 636f 6e66 6967  )..    if config
+0000a440: 2e75 7365 5f44 535f 6465 6369 6d61 6c3a  .use_DS_decimal:
+0000a450: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000a460: 4453 6465 6369 6d61 6c28 7661 6c2c 2061  DSdecimal(val, a
+0000a470: 7574 6f5f 666f 726d 6174 2c20 7661 6c69  uto_format, vali
+0000a480: 6461 7469 6f6e 5f6d 6f64 6529 0a0a 2020  dation_mode)..  
+0000a490: 2020 7265 7475 726e 2044 5366 6c6f 6174    return DSfloat
+0000a4a0: 2876 616c 2c20 6175 746f 5f66 6f72 6d61  (val, auto_forma
+0000a4b0: 742c 2076 616c 6964 6174 696f 6e5f 6d6f  t, validation_mo
+0000a4c0: 6465 290a 0a0a 636c 6173 7320 4953 666c  de)...class ISfl
+0000a4d0: 6f61 7428 666c 6f61 7429 3a0a 2020 2020  oat(float):.    
+0000a4e0: 2222 2253 746f 7265 2076 616c 7565 2066  """Store value f
+0000a4f0: 6f72 2061 6e20 656c 656d 656e 7420 7769  or an element wi
+0000a500: 7468 2056 5220 2a2a 4953 2a2a 2061 7320  th VR **IS** as 
+0000a510: 3a63 6c61 7373 3a60 666c 6f61 7460 2e0a  :class:`float`..
+0000a520: 0a20 2020 2053 746f 7265 7320 6f72 6967  .    Stores orig
+0000a530: 696e 616c 2069 6e74 6567 6572 2073 7472  inal integer str
+0000a540: 696e 6720 666f 7220 6578 6163 7420 7265  ing for exact re
+0000a550: 7772 6974 696e 6720 6f66 2074 6865 2073  writing of the s
+0000a560: 7472 696e 670a 2020 2020 6f72 6967 696e  tring.    origin
+0000a570: 616c 6c79 2072 6561 6420 6f72 2073 746f  ally read or sto
+0000a580: 7265 642e 0a0a 2020 2020 4e6f 7465 3a20  red...    Note: 
+0000a590: 4279 2074 6865 2044 4943 4f4d 2073 7461  By the DICOM sta
+0000a5a0: 6e64 6172 642c 2049 5320 6361 6e20 6f6e  ndard, IS can on
+0000a5b0: 6c79 2062 6520 616e 203a 636c 6173 733a  ly be an :class:
+0000a5c0: 6069 6e74 602c 0a20 2020 2068 6f77 6576  `int`,.    howev
+0000a5d0: 6572 2c20 6974 2069 7320 6e6f 7420 756e  er, it is not un
+0000a5e0: 636f 6d6d 6f6e 2074 6f20 7365 6520 666c  common to see fl
+0000a5f0: 6f61 7420 4953 2076 616c 7565 732e 2020  oat IS values.  
+0000a600: 5468 6973 2063 6c61 7373 0a20 2020 2069  This class.    i
+0000a610: 7320 7573 6564 2069 6620 7468 6520 636f  s used if the co
+0000a620: 6e66 6967 2073 6574 7469 6e67 7320 616c  nfig settings al
+0000a630: 6c6f 7720 6e6f 6e2d 7374 7269 6374 2072  low non-strict r
+0000a640: 6561 6469 6e67 2e0a 0a20 2020 2047 656e  eading...    Gen
+0000a650: 6572 616c 6c79 2c20 7573 6520 3a63 6c61  erally, use :cla
+0000a660: 7373 3a60 7e70 7964 6963 6f6d 2e76 616c  ss:`~pydicom.val
+0000a670: 7565 7265 702e 4953 6020 746f 2063 7265  uerep.IS` to cre
+0000a680: 6174 6520 4953 2076 616c 7565 732c 0a20  ate IS values,. 
+0000a690: 2020 2074 6869 7320 6973 2072 6574 7572     this is retur
+0000a6a0: 6e65 6420 696e 7374 6561 6420 6966 2074  ned instead if t
+0000a6b0: 6865 2076 616c 7565 2063 616e 6e6f 7420  he value cannot 
+0000a6c0: 6265 2072 6570 7265 7365 6e74 6564 2061  be represented a
+0000a6d0: 7320 616e 0a20 2020 203a 636c 6173 733a  s an.    :class:
+0000a6e0: 6069 6e74 602e 2020 5365 6520 3a63 6c61  `int`.  See :cla
+0000a6f0: 7373 3a60 7e70 7964 6963 6f6d 2e76 616c  ss:`~pydicom.val
+0000a700: 7565 7265 702e 4953 6020 666f 7220 6465  uerep.IS` for de
+0000a710: 7461 696c 7320 6f66 2074 6865 0a20 2020  tails of the.   
+0000a720: 2070 6172 616d 6574 6572 7320 616e 6420   parameters and 
+0000a730: 7265 7475 726e 2076 616c 7565 732e 0a20  return values.. 
+0000a740: 2020 2022 2222 0a20 2020 2064 6566 205f     """.    def _
+0000a750: 5f6e 6577 5f5f 2820 2023 2074 7970 653a  _new__(  # type:
+0000a760: 2069 676e 6f72 655b 6d69 7363 5d0a 2020   ignore[misc].  
+0000a770: 2020 2020 2020 2020 2020 636c 733a 2054            cls: T
+0000a780: 7970 655b 2249 5366 6c6f 6174 225d 2c20  ype["ISfloat"], 
+0000a790: 7661 6c3a 2055 6e69 6f6e 5b73 7472 2c20  val: Union[str, 
+0000a7a0: 666c 6f61 742c 2044 6563 696d 616c 5d2c  float, Decimal],
+0000a7b0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+0000a7c0: 6964 6174 696f 6e5f 6d6f 6465 3a20 696e  idation_mode: in
+0000a7d0: 7420 3d20 4e6f 6e65 0a20 2020 2029 202d  t = None.    ) -
+0000a7e0: 3e20 666c 6f61 743a 0a20 2020 2020 2020  > float:.       
+0000a7f0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+0000a800: 5f5f 6e65 775f 5f28 636c 732c 2076 616c  __new__(cls, val
+0000a810: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
+0000a820: 745f 5f28 7365 6c66 2c20 7661 6c3a 2055  t__(self, val: U
+0000a830: 6e69 6f6e 5b73 7472 2c20 666c 6f61 742c  nion[str, float,
+0000a840: 2044 6563 696d 616c 5d2c 0a20 2020 2020   Decimal],.     
+0000a850: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+0000a860: 6461 7469 6f6e 5f6d 6f64 653a 2069 6e74  dation_mode: int
+0000a870: 203d 204e 6f6e 6529 202d 3e20 4e6f 6e65   = None) -> None
+0000a880: 3a0a 2020 2020 2020 2020 2320 4966 2061  :.        # If a
+0000a890: 2073 7472 696e 6720 7061 7373 6564 2c20   string passed, 
+0000a8a0: 7468 656e 2073 746f 7265 2069 740a 2020  then store it.  
+0000a8b0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000a8c0: 6e63 6528 7661 6c2c 2073 7472 293a 0a20  nce(val, str):. 
+0000a8d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a8e0: 6f72 6967 696e 616c 5f73 7472 696e 6720  original_string 
+0000a8f0: 3d20 7661 6c2e 7374 7269 7028 290a 2020  = val.strip().  
+0000a900: 2020 2020 2020 656c 6966 2028 6973 696e        elif (isin
+0000a910: 7374 616e 6365 2876 616c 2c20 2849 532c  stance(val, (IS,
+0000a920: 2049 5366 6c6f 6174 2929 0a20 2020 2020   ISfloat)).     
+0000a930: 2020 2020 2020 2020 2020 2061 6e64 2068             and h
+0000a940: 6173 6174 7472 2876 616c 2c20 276f 7269  asattr(val, 'ori
+0000a950: 6769 6e61 6c5f 7374 7269 6e67 2729 293a  ginal_string')):
+0000a960: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000a970: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
+0000a980: 6720 3d20 7661 6c2e 6f72 6967 696e 616c  g = val.original
+0000a990: 5f73 7472 696e 670a 2020 2020 2020 2020  _string.        
+0000a9a0: 6966 2076 616c 6964 6174 696f 6e5f 6d6f  if validation_mo
+0000a9b0: 6465 3a0a 2020 2020 2020 2020 2020 2020  de:.            
+0000a9c0: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
+0000a9d0: 2020 2020 2020 2020 6627 5661 6c75 6520          f'Value 
+0000a9e0: 227b 7374 7228 7365 6c66 297d 2220 6973  "{str(self)}" is
+0000a9f0: 206e 6f74 2076 616c 6964 2066 6f72 2065   not valid for e
+0000aa00: 6c65 6d65 6e74 7320 7769 7468 2061 2056  lements with a V
+0000aa10: 5220 270a 2020 2020 2020 2020 2020 2020  R '.            
+0000aa20: 2020 2020 276f 6620 4953 270a 2020 2020      'of IS'.    
+0000aa30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000aa40: 2020 2020 2020 6966 2076 616c 6964 6174        if validat
+0000aa50: 696f 6e5f 6d6f 6465 203d 3d20 636f 6e66  ion_mode == conf
+0000aa60: 6967 2e57 4152 4e3a 0a20 2020 2020 2020  ig.WARN:.       
+0000aa70: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0000aa80: 732e 7761 726e 286d 7367 290a 2020 2020  s.warn(msg).    
+0000aa90: 2020 2020 2020 2020 656c 6966 2076 616c          elif val
+0000aaa0: 6964 6174 696f 6e5f 6d6f 6465 203d 3d20  idation_mode == 
+0000aab0: 636f 6e66 6967 2e52 4149 5345 3a0a 2020  config.RAISE:.  
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
+0000aad0: 6720 2b3d 2028 0a20 2020 2020 2020 2020  g += (.         
+0000aae0: 2020 2020 2020 2020 2020 2022 5c6e 5365             "\nSe
+0000aaf0: 7420 7265 6164 696e 675f 7661 6c69 6461  t reading_valida
+0000ab00: 7469 6f6e 5f6d 6f64 6520 746f 2057 4152  tion_mode to WAR
+0000ab10: 4e20 6f72 2049 474e 4f52 4520 746f 2062  N or IGNORE to b
+0000ab20: 7970 6173 7322 0a20 2020 2020 2020 2020  ypass".         
+0000ab30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000ab40: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+0000ab50: 7970 6545 7272 6f72 286d 7367 290a 0a0a  ypeError(msg)...
+0000ab60: 636c 6173 7320 4953 2869 6e74 293a 0a20  class IS(int):. 
+0000ab70: 2020 2022 2222 5374 6f72 6520 7661 6c75     """Store valu
+0000ab80: 6520 666f 7220 616e 2065 6c65 6d65 6e74  e for an element
+0000ab90: 2077 6974 6820 5652 202a 2a49 532a 2a20   with VR **IS** 
+0000aba0: 6173 203a 636c 6173 733a 6069 6e74 602e  as :class:`int`.
+0000abb0: 0a0a 2020 2020 5374 6f72 6573 206f 7269  ..    Stores ori
+0000abc0: 6769 6e61 6c20 696e 7465 6765 7220 7374  ginal integer st
+0000abd0: 7269 6e67 2066 6f72 2065 7861 6374 2072  ring for exact r
+0000abe0: 6577 7269 7469 6e67 206f 6620 7468 6520  ewriting of the 
+0000abf0: 7374 7269 6e67 0a20 2020 206f 7269 6769  string.    origi
+0000ac00: 6e61 6c6c 7920 7265 6164 206f 7220 7374  nally read or st
+0000ac10: 6f72 6564 2e0a 2020 2020 2222 220a 0a20  ored..    """.. 
+0000ac20: 2020 2064 6566 205f 5f6e 6577 5f5f 2820     def __new__( 
+0000ac30: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+0000ac40: 6d69 7363 5d0a 2020 2020 2020 2020 2020  misc].          
+0000ac50: 2020 636c 733a 2054 7970 655b 2249 5322    cls: Type["IS"
+0000ac60: 5d2c 2076 616c 3a20 556e 696f 6e5b 4e6f  ], val: Union[No
+0000ac70: 6e65 2c20 7374 722c 2069 6e74 2c20 666c  ne, str, int, fl
+0000ac80: 6f61 742c 2044 6563 696d 616c 5d2c 0a20  oat, Decimal],. 
+0000ac90: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+0000aca0: 6174 696f 6e5f 6d6f 6465 3a20 696e 7420  ation_mode: int 
+0000acb0: 3d20 4e6f 6e65 0a20 2020 2029 202d 3e20  = None.    ) -> 
+0000acc0: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
+0000acd0: 7472 2c20 2249 5322 2c20 2249 5366 6c6f  tr, "IS", "ISflo
+0000ace0: 6174 225d 5d3a 0a20 2020 2020 2020 2022  at"]]:.        "
+0000acf0: 2222 4372 6561 7465 2069 6e73 7461 6e63  ""Create instanc
+0000ad00: 6520 6966 206e 6577 2069 6e74 6567 6572  e if new integer
+0000ad10: 2073 7472 696e 6722 2222 0a20 2020 2020   string""".     
+0000ad20: 2020 2069 6620 7661 6c20 6973 204e 6f6e     if val is Non
+0000ad30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000ad40: 6574 7572 6e20 7661 6c0a 0a20 2020 2020  eturn val..     
+0000ad50: 2020 2069 6620 7661 6c69 6461 7469 6f6e     if validation
+0000ad60: 5f6d 6f64 6520 6973 204e 6f6e 653a 0a20  _mode is None:. 
+0000ad70: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+0000ad80: 6174 696f 6e5f 6d6f 6465 203d 2063 6f6e  ation_mode = con
+0000ad90: 6669 672e 7365 7474 696e 6773 2e72 6561  fig.settings.rea
+0000ada0: 6469 6e67 5f76 616c 6964 6174 696f 6e5f  ding_validation_
+0000adb0: 6d6f 6465 0a0a 2020 2020 2020 2020 6966  mode..        if
+0000adc0: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
+0000add0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+0000ade0: 2020 2069 6620 7661 6c2e 7374 7269 7028     if val.strip(
+0000adf0: 2920 3d3d 2027 273a 0a20 2020 2020 2020  ) == '':.       
+0000ae00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000ae10: 7661 6c0a 2020 2020 2020 2020 2020 2020  val.            
+0000ae20: 7661 6c69 6461 7465 5f76 616c 7565 2822  validate_value("
+0000ae30: 4953 222c 2076 616c 2c20 7661 6c69 6461  IS", val, valida
+0000ae40: 7469 6f6e 5f6d 6f64 6529 0a0a 2020 2020  tion_mode)..    
+0000ae50: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000ae60: 2020 2020 206e 6577 7661 6c3a 2055 6e69       newval: Uni
+0000ae70: 6f6e 5b49 532c 2049 5366 6c6f 6174 5d20  on[IS, ISfloat] 
+0000ae80: 3d20 7375 7065 7228 292e 5f5f 6e65 775f  = super().__new_
+0000ae90: 5f28 636c 732c 2076 616c 290a 2020 2020  _(cls, val).    
+0000aea0: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+0000aeb0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+0000aec0: 2020 2023 2061 6363 6570 7420 666c 6f61     # accept floa
+0000aed0: 7420 7374 7269 6e67 7320 7768 656e 206e  t strings when n
+0000aee0: 6f20 696e 7465 6765 7220 6c6f 7373 2c20  o integer loss, 
+0000aef0: 652e 672e 2022 312e 3022 0a20 2020 2020  e.g. "1.0".     
+0000af00: 2020 2020 2020 206e 6577 7661 6c20 3d20         newval = 
+0000af10: 7375 7065 7228 292e 5f5f 6e65 775f 5f28  super().__new__(
+0000af20: 636c 732c 2066 6c6f 6174 2876 616c 2929  cls, float(val))
+0000af30: 0a0a 2020 2020 2020 2020 2320 4966 2061  ..        # If a
+0000af40: 2066 6c6f 6174 206f 7220 4465 6369 6d61   float or Decima
+0000af50: 6c20 7761 7320 7061 7373 6564 2069 6e2c  l was passed in,
+0000af60: 2063 6865 636b 2066 6f72 206e 6f6e 2d69   check for non-i
+0000af70: 6e74 6567 6572 2c0a 2020 2020 2020 2020  nteger,.        
+0000af80: 2320 692e 652e 2063 6f75 6c64 206c 6f73  # i.e. could los
+0000af90: 6520 696e 666f 2069 6620 636f 6e76 6572  e info if conver
+0000afa0: 7465 6420 746f 2069 6e74 0a20 2020 2020  ted to int.     
+0000afb0: 2020 2023 2049 6620 736f 2c20 6372 6561     # If so, crea
+0000afc0: 7465 2061 6e20 4953 666c 6f61 7420 696e  te an ISfloat in
+0000afd0: 7374 6561 6420 2869 6620 616c 6c6f 7765  stead (if allowe
+0000afe0: 6420 6279 2073 6574 7469 6e67 7329 0a20  d by settings). 
+0000aff0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000b000: 616e 6365 2876 616c 2c20 2866 6c6f 6174  ance(val, (float
+0000b010: 2c20 4465 6369 6d61 6c2c 2073 7472 2929  , Decimal, str))
+0000b020: 2061 6e64 206e 6577 7661 6c20 213d 2066   and newval != f
+0000b030: 6c6f 6174 2876 616c 293a 0a20 2020 2020  loat(val):.     
+0000b040: 2020 2020 2020 206e 6577 7661 6c20 3d20         newval = 
+0000b050: 4953 666c 6f61 7428 7661 6c2c 2076 616c  ISfloat(val, val
+0000b060: 6964 6174 696f 6e5f 6d6f 6465 290a 0a20  idation_mode).. 
+0000b070: 2020 2020 2020 2023 2043 6865 636b 7320         # Checks 
+0000b080: 696e 2063 6173 6520 756e 6465 726c 7969  in case underlyi
+0000b090: 6e67 2069 6e74 2069 7320 3e33 3220 6269  ng int is >32 bi
+0000b0a0: 7473 2c20 4449 434f 4d20 646f 6573 206e  ts, DICOM does n
+0000b0b0: 6f74 2061 6c6c 6f77 2074 6869 730a 2020  ot allow this.  
+0000b0c0: 2020 2020 2020 6966 2028 6e6f 7420 2d32        if (not -2
+0000b0d0: 2a2a 3331 203c 3d20 6e65 7776 616c 203c  **31 <= newval <
+0000b0e0: 2032 2a2a 3331 2061 6e64 0a20 2020 2020   2**31 and.     
+0000b0f0: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+0000b100: 6174 696f 6e5f 6d6f 6465 203d 3d20 636f  ation_mode == co
+0000b110: 6e66 6967 2e52 4149 5345 293a 0a20 2020  nfig.RAISE):.   
+0000b120: 2020 2020 2020 2020 2072 6169 7365 204f           raise O
+0000b130: 7665 7266 6c6f 7745 7272 6f72 280a 2020  verflowError(.  
+0000b140: 2020 2020 2020 2020 2020 2020 2020 2245                "E
+0000b150: 6c65 6d65 6e74 7320 7769 7468 2061 2056  lements with a V
+0000b160: 5220 6f66 2049 5320 6d75 7374 2068 6176  R of IS must hav
+0000b170: 6520 6120 7661 6c75 6520 6265 7477 6565  e a value betwee
+0000b180: 6e20 2d32 2a2a 3331 2022 0a20 2020 2020  n -2**31 ".     
+0000b190: 2020 2020 2020 2020 2020 2022 616e 6420             "and 
+0000b1a0: 2832 2a2a 3331 202d 2031 292e 2053 6574  (2**31 - 1). Set
+0000b1b0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000b1c0: 2020 2022 2763 6f6e 6669 672e 7365 7474     "'config.sett
+0000b1d0: 696e 6773 2e72 6561 6469 6e67 5f76 616c  ings.reading_val
+0000b1e0: 6964 6174 696f 6e5f 6d6f 6465 2720 746f  idation_mode' to
+0000b1f0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000b200: 2020 2022 2757 4152 4e27 2074 6f20 6f76     "'WARN' to ov
+0000b210: 6572 7269 6465 2074 6865 2076 616c 7565  erride the value
+0000b220: 2063 6865 636b 220a 2020 2020 2020 2020   check".        
+0000b230: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
+0000b240: 6574 7572 6e20 6e65 7776 616c 0a0a 2020  eturn newval..  
+0000b250: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000b260: 656c 662c 2076 616c 3a20 556e 696f 6e5b  elf, val: Union[
+0000b270: 7374 722c 2069 6e74 2c20 666c 6f61 742c  str, int, float,
+0000b280: 2044 6563 696d 616c 5d2c 0a20 2020 2020   Decimal],.     
+0000b290: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+0000b2a0: 6461 7469 6f6e 5f6d 6f64 653a 2069 6e74  dation_mode: int
+0000b2b0: 203d 204e 6f6e 6529 202d 3e20 4e6f 6e65   = None) -> None
+0000b2c0: 3a0a 2020 2020 2020 2020 2320 4966 2061  :.        # If a
+0000b2d0: 2073 7472 696e 6720 7061 7373 6564 2c20   string passed, 
+0000b2e0: 7468 656e 2073 746f 7265 2069 740a 2020  then store it.  
+0000b2f0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000b300: 6e63 6528 7661 6c2c 2073 7472 293a 0a20  nce(val, str):. 
+0000b310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b320: 6f72 6967 696e 616c 5f73 7472 696e 6720  original_string 
+0000b330: 3d20 7661 6c2e 7374 7269 7028 290a 2020  = val.strip().  
+0000b340: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+0000b350: 7461 6e63 6528 7661 6c2c 2049 5329 2061  tance(val, IS) a
+0000b360: 6e64 2068 6173 6174 7472 2876 616c 2c20  nd hasattr(val, 
+0000b370: 276f 7269 6769 6e61 6c5f 7374 7269 6e67  'original_string
+0000b380: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000b390: 7365 6c66 2e6f 7269 6769 6e61 6c5f 7374  self.original_st
+0000b3a0: 7269 6e67 203d 2076 616c 2e6f 7269 6769  ring = val.origi
+0000b3b0: 6e61 6c5f 7374 7269 6e67 0a0a 2020 2020  nal_string..    
+0000b3c0: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
+0000b3d0: 206f 7468 6572 3a20 416e 7929 202d 3e20   other: Any) -> 
+0000b3e0: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
+0000b3f0: 4f76 6572 7269 6465 2074 6f20 616c 6c6f  Override to allo
+0000b400: 7720 7374 7269 6e67 2065 7175 616c 6974  w string equalit
+0000b410: 7920 636f 6d70 6172 6973 6f6e 732e 2222  y comparisons.""
+0000b420: 220a 2020 2020 2020 2020 6966 2069 7369  ".        if isi
+0000b430: 6e73 7461 6e63 6528 6f74 6865 722c 2073  nstance(other, s
+0000b440: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+0000b450: 2072 6574 7572 6e20 7374 7228 7365 6c66   return str(self
+0000b460: 2920 3d3d 206f 7468 6572 0a0a 2020 2020  ) == other..    
+0000b470: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+0000b480: 2829 2e5f 5f65 715f 5f28 6f74 6865 7229  ().__eq__(other)
+0000b490: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
+0000b4a0: 5f5f 2873 656c 6629 202d 3e20 696e 743a  __(self) -> int:
+0000b4b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b4c0: 7375 7065 7228 292e 5f5f 6861 7368 5f5f  super().__hash__
+0000b4d0: 2829 0a0a 2020 2020 6465 6620 5f5f 6e65  ()..    def __ne
+0000b4e0: 5f5f 2873 656c 662c 206f 7468 6572 3a20  __(self, other: 
+0000b4f0: 416e 7929 202d 3e20 416e 793a 0a20 2020  Any) -> Any:.   
+0000b500: 2020 2020 2072 6574 7572 6e20 6e6f 7420       return not 
+0000b510: 7365 6c66 203d 3d20 6f74 6865 720a 0a20  self == other.. 
+0000b520: 2020 2064 6566 205f 5f73 7472 5f5f 2873     def __str__(s
+0000b530: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+0000b540: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+0000b550: 7365 6c66 2c20 276f 7269 6769 6e61 6c5f  self, 'original_
+0000b560: 7374 7269 6e67 2729 3a0a 2020 2020 2020  string'):.      
+0000b570: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000b580: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
+0000b590: 670a 0a20 2020 2020 2020 2023 2049 7373  g..        # Iss
+0000b5a0: 7565 2023 3933 3720 2850 7974 686f 6e20  ue #937 (Python 
+0000b5b0: 332e 3820 636f 6d70 6174 6962 696c 6974  3.8 compatibilit
+0000b5c0: 7929 0a20 2020 2020 2020 2072 6574 7572  y).        retur
+0000b5d0: 6e20 7265 7072 2873 656c 6629 5b31 3a2d  n repr(self)[1:-
+0000b5e0: 315d 0a0a 2020 2020 6465 6620 5f5f 7265  1]..    def __re
+0000b5f0: 7072 5f5f 2873 656c 6629 202d 3e20 7374  pr__(self) -> st
+0000b600: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+0000b610: 6e20 6622 277b 7375 7065 7228 292e 5f5f  n f"'{super().__
+0000b620: 7265 7072 5f5f 2829 7d27 220a 0a0a 5f54  repr__()}'"..._T
+0000b630: 203d 2054 7970 6556 6172 2827 5f54 2729   = TypeVar('_T')
+0000b640: 0a0a 0a64 6566 204d 756c 7469 5374 7269  ...def MultiStri
+0000b650: 6e67 280a 2020 2020 2020 2020 7661 6c3a  ng(.        val:
+0000b660: 2073 7472 2c20 7661 6c74 7970 653a 204f   str, valtype: O
+0000b670: 7074 696f 6e61 6c5b 4361 6c6c 6162 6c65  ptional[Callable
+0000b680: 5b5b 7374 725d 2c20 5f54 5d5d 203d 204e  [[str], _T]] = N
+0000b690: 6f6e 652c 0a20 2020 2020 2020 2076 616c  one,.        val
+0000b6a0: 6964 6174 696f 6e5f 6d6f 6465 3a20 696e  idation_mode: in
+0000b6b0: 7420 3d20 4e6f 6e65 0a29 202d 3e20 556e  t = None.) -> Un
+0000b6c0: 696f 6e5b 5f54 2c20 4d75 7461 626c 6553  ion[_T, MutableS
+0000b6d0: 6571 7565 6e63 655b 5f54 5d5d 3a0a 2020  equence[_T]]:.  
+0000b6e0: 2020 2222 2253 706c 6974 2061 2073 7472    """Split a str
+0000b6f0: 696e 6720 6279 2064 656c 696d 6974 6572  ing by delimiter
+0000b700: 7320 6966 2074 6865 7265 2061 7265 2061  s if there are a
+0000b710: 6e79 0a0a 2020 2020 5061 7261 6d65 7465  ny..    Paramete
+0000b720: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+0000b730: 2d0a 2020 2020 7661 6c20 3a20 7374 720a  -.    val : str.
+0000b740: 2020 2020 2020 2020 5468 6520 7374 7269          The stri
+0000b750: 6e67 2074 6f20 7370 6c69 7420 7570 2e0a  ng to split up..
+0000b760: 2020 2020 7661 6c74 7970 6520 3a20 7479      valtype : ty
+0000b770: 7065 206f 7220 6361 6c6c 6162 6c65 2c20  pe or callable, 
+0000b780: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000b790: 2044 6566 6175 6c74 203a 636c 6173 733a   Default :class:
+0000b7a0: 6073 7472 602c 2062 7574 2063 616e 2062  `str`, but can b
+0000b7b0: 6520 652e 672e 203a 636c 6173 733a 607e  e e.g. :class:`~
+0000b7c0: 7079 6469 636f 6d2e 7569 642e 5549 4460  pydicom.uid.UID`
+0000b7d0: 2074 6f0a 2020 2020 2020 2020 6f76 6572   to.        over
+0000b7e0: 7772 6974 6520 746f 2061 2073 7065 6369  write to a speci
+0000b7f0: 6669 6320 7479 7065 2e0a 2020 2020 7661  fic type..    va
+0000b800: 6c69 6461 7469 6f6e 5f6d 6f64 6520 3a20  lidation_mode : 
+0000b810: 696e 740a 2020 2020 2020 2020 4465 6669  int.        Defi
+0000b820: 6e65 7320 6966 2076 616c 7565 7320 6172  nes if values ar
+0000b830: 6520 7661 6c69 6461 7465 6420 616e 6420  e validated and 
+0000b840: 686f 7720 7661 6c69 6461 7469 6f6e 2065  how validation e
+0000b850: 7272 6f72 7320 6172 650a 2020 2020 2020  rrors are.      
+0000b860: 2020 6861 6e64 6c65 642e 0a0a 2020 2020    handled...    
+0000b870: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+0000b880: 2d2d 2d0a 2020 2020 7661 6c74 7970 6520  ---.    valtype 
+0000b890: 6f72 204d 756c 7469 5661 6c75 6520 6f66  or MultiValue of
+0000b8a0: 2076 616c 7479 7065 0a20 2020 2020 2020   valtype.       
+0000b8b0: 2054 6865 2073 706c 6974 2076 616c 7565   The split value
+0000b8c0: 2061 7320 6076 616c 7479 7065 6020 6f72   as `valtype` or
+0000b8d0: 2061 203a 636c 6173 733a 606c 6973 7460   a :class:`list`
+0000b8e0: 206f 6620 6076 616c 7479 7065 602e 0a20   of `valtype`.. 
+0000b8f0: 2020 2022 2222 0a20 2020 2069 6620 7661     """.    if va
+0000b900: 6c74 7970 6520 6973 204e 6f6e 653a 0a20  ltype is None:. 
+0000b910: 2020 2020 2020 2076 616c 7479 7065 203d         valtype =
+0000b920: 2063 6173 7428 4361 6c6c 6162 6c65 5b5b   cast(Callable[[
+0000b930: 7374 725d 2c20 5f54 5d2c 2073 7472 290a  str], _T], str).
+0000b940: 0a20 2020 2023 2052 656d 6f76 6520 7472  .    # Remove tr
+0000b950: 6169 6c69 6e67 2062 6c61 6e6b 2075 7365  ailing blank use
+0000b960: 6420 746f 2070 6164 2074 6f20 6576 656e  d to pad to even
+0000b970: 206c 656e 6774 680a 2020 2020 2320 3230   length.    # 20
+0000b980: 3035 2e30 352e 3235 3a20 616c 736f 2063  05.05.25: also c
+0000b990: 6865 636b 2066 6f72 2074 7261 696c 696e  heck for trailin
+0000b9a0: 6720 302c 2065 7272 6f72 206d 6164 650a  g 0, error made.
+0000b9b0: 2020 2020 2320 696e 2050 4554 2066 696c      # in PET fil
+0000b9c0: 6573 2077 6520 6172 6520 636f 6e76 6572  es we are conver
+0000b9d0: 7469 6e67 0a20 2020 2077 6869 6c65 2076  ting.    while v
+0000b9e0: 616c 2061 6e64 2076 616c 2e65 6e64 7377  al and val.endsw
+0000b9f0: 6974 6828 2827 2027 2c20 275c 7830 3027  ith((' ', '\x00'
+0000ba00: 2929 3a0a 2020 2020 2020 2020 7661 6c20  )):.        val 
+0000ba10: 3d20 7661 6c5b 3a2d 315d 0a0a 2020 2020  = val[:-1]..    
+0000ba20: 7370 6c69 7475 703a 204c 6973 745b 7374  splitup: List[st
+0000ba30: 725d 203d 2076 616c 2e73 706c 6974 2822  r] = val.split("
+0000ba40: 5c5c 2229 0a20 2020 2069 6620 6c65 6e28  \\").    if len(
+0000ba50: 7370 6c69 7475 7029 203d 3d20 313a 0a20  splitup) == 1:. 
+0000ba60: 2020 2020 2020 2072 6574 7572 6e20 7661         return va
+0000ba70: 6c74 7970 6528 7370 6c69 7475 705b 305d  ltype(splitup[0]
+0000ba80: 290a 0a20 2020 2072 6574 7572 6e20 4d75  )..    return Mu
+0000ba90: 6c74 6956 616c 7565 2876 616c 7479 7065  ltiValue(valtype
+0000baa0: 2c20 7370 6c69 7475 702c 2076 616c 6964  , splitup, valid
+0000bab0: 6174 696f 6e5f 6d6f 6465 290a 0a0a 6465  ation_mode)...de
+0000bac0: 6620 5f76 6572 6966 795f 656e 636f 6469  f _verify_encodi
+0000bad0: 6e67 7328 0a20 2020 2065 6e63 6f64 696e  ngs(.    encodin
+0000bae0: 6773 3a20 4f70 7469 6f6e 616c 5b55 6e69  gs: Optional[Uni
+0000baf0: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
+0000bb00: 5b73 7472 5d5d 5d0a 2920 2d3e 204f 7074  [str]]].) -> Opt
+0000bb10: 696f 6e61 6c5b 5475 706c 655b 7374 722c  ional[Tuple[str,
+0000bb20: 202e 2e2e 5d5d 3a0a 2020 2020 2222 2243   ...]]:.    """C
+0000bb30: 6865 636b 7320 7468 6520 656e 636f 6469  hecks the encodi
+0000bb40: 6e67 2074 6f20 656e 7375 7265 2070 726f  ng to ensure pro
+0000bb50: 7065 7220 666f 726d 6174 2222 220a 2020  per format""".  
+0000bb60: 2020 6966 2065 6e63 6f64 696e 6773 2069    if encodings i
+0000bb70: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000bb80: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+0000bb90: 2069 6620 6973 696e 7374 616e 6365 2865   if isinstance(e
+0000bba0: 6e63 6f64 696e 6773 2c20 7374 7229 3a0a  ncodings, str):.
+0000bbb0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+0000bbc0: 656e 636f 6469 6e67 732c 290a 0a20 2020  encodings,)..   
+0000bbd0: 2072 6574 7572 6e20 7475 706c 6528 656e   return tuple(en
+0000bbe0: 636f 6469 6e67 7329 0a0a 0a64 6566 205f  codings)...def _
+0000bbf0: 6465 636f 6465 5f70 6572 736f 6e6e 616d  decode_personnam
+0000bc00: 6528 0a20 2020 2063 6f6d 706f 6e65 6e74  e(.    component
+0000bc10: 733a 2053 6571 7565 6e63 655b 6279 7465  s: Sequence[byte
+0000bc20: 735d 2c20 656e 636f 6469 6e67 733a 2053  s], encodings: S
+0000bc30: 6571 7565 6e63 655b 7374 725d 0a29 202d  equence[str].) -
+0000bc40: 3e20 5475 706c 655b 7374 722c 202e 2e2e  > Tuple[str, ...
+0000bc50: 5d3a 0a20 2020 2022 2222 5265 7475 726e  ]:.    """Return
+0000bc60: 2061 206c 6973 7420 6f66 2064 6563 6f64   a list of decod
+0000bc70: 6564 2070 6572 736f 6e20 6e61 6d65 2063  ed person name c
+0000bc80: 6f6d 706f 6e65 6e74 732e 0a0a 2020 2020  omponents...    
+0000bc90: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000bca0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 636f  ---------.    co
+0000bcb0: 6d70 6f6e 656e 7473 203a 206c 6973 7420  mponents : list 
+0000bcc0: 6f66 2062 7974 6573 0a20 2020 2020 2020  of bytes.       
+0000bcd0: 2054 6865 206c 6973 7420 6f66 2074 6865   The list of the
+0000bce0: 2075 7020 746f 2074 6872 6565 2065 6e63   up to three enc
+0000bcf0: 6f64 6564 2070 6572 736f 6e20 6e61 6d65  oded person name
+0000bd00: 2063 6f6d 706f 6e65 6e74 730a 2020 2020   components.    
+0000bd10: 656e 636f 6469 6e67 7320 3a20 6c69 7374  encodings : list
+0000bd20: 206f 6620 7374 720a 2020 2020 2020 2020   of str.        
+0000bd30: 5468 6520 5079 7468 6f6e 2065 6e63 6f64  The Python encod
+0000bd40: 696e 6773 2075 7365 7320 746f 2064 6563  ings uses to dec
+0000bd50: 6f64 6520 6063 6f6d 706f 6e65 6e74 7360  ode `components`
+0000bd60: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0000bd70: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2074     -------.    t
+0000bd80: 6578 7420 7479 7065 0a20 2020 2020 2020  ext type.       
+0000bd90: 2054 6865 2075 6e69 636f 6465 2073 7472   The unicode str
+0000bda0: 696e 6720 7265 7072 6573 656e 7469 6e67  ing representing
+0000bdb0: 2074 6865 2070 6572 736f 6e20 6e61 6d65   the person name
+0000bdc0: 2e0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
+0000bdd0: 2064 6563 6f64 696e 6720 6f66 2073 6f6d   decoding of som
+0000bde0: 6520 636f 6d70 6f6e 656e 7420 7061 7274  e component part
+0000bdf0: 7320 6973 206e 6f74 2070 6f73 7369 626c  s is not possibl
+0000be00: 6520 7573 696e 6720 7468 650a 2020 2020  e using the.    
+0000be10: 2020 2020 6769 7665 6e20 656e 636f 6469      given encodi
+0000be20: 6e67 732c 2074 6865 7920 6172 6520 6465  ngs, they are de
+0000be30: 636f 6465 6420 7769 7468 2074 6865 2066  coded with the f
+0000be40: 6972 7374 2065 6e63 6f64 696e 6720 7573  irst encoding us
+0000be50: 696e 670a 2020 2020 2020 2020 7265 706c  ing.        repl
+0000be60: 6163 656d 656e 7420 6368 6172 6163 7465  acement characte
+0000be70: 7273 2066 6f72 2062 7974 6573 2074 6861  rs for bytes tha
+0000be80: 7420 6361 6e6e 6f74 2062 6520 6465 636f  t cannot be deco
+0000be90: 6465 642e 0a20 2020 2022 2222 0a20 2020  ded..    """.   
+0000bea0: 2066 726f 6d20 7079 6469 636f 6d2e 6368   from pydicom.ch
+0000beb0: 6172 7365 7420 696d 706f 7274 2064 6563  arset import dec
+0000bec0: 6f64 655f 6279 7465 730a 0a20 2020 2063  ode_bytes..    c
+0000bed0: 6f6d 7073 203d 205b 6465 636f 6465 5f62  omps = [decode_b
+0000bee0: 7974 6573 2863 2c20 656e 636f 6469 6e67  ytes(c, encoding
+0000bef0: 732c 2050 4e5f 4445 4c49 4d53 2920 666f  s, PN_DELIMS) fo
+0000bf00: 7220 6320 696e 2063 6f6d 706f 6e65 6e74  r c in component
+0000bf10: 735d 0a0a 2020 2020 2320 5265 6d6f 7665  s]..    # Remove
+0000bf20: 2065 6d70 7479 2065 6c65 6d65 6e74 7320   empty elements 
+0000bf30: 6672 6f6d 2074 6865 2065 6e64 2074 6f20  from the end to 
+0000bf40: 6176 6f69 6420 7472 6169 6c69 6e67 2027  avoid trailing '
+0000bf50: 3d27 0a20 2020 2077 6869 6c65 206c 656e  ='.    while len
+0000bf60: 2863 6f6d 7073 2920 616e 6420 6e6f 7420  (comps) and not 
+0000bf70: 636f 6d70 735b 2d31 5d3a 0a20 2020 2020  comps[-1]:.     
+0000bf80: 2020 2063 6f6d 7073 2e70 6f70 2829 0a0a     comps.pop()..
+0000bf90: 2020 2020 7265 7475 726e 2074 7570 6c65      return tuple
+0000bfa0: 2863 6f6d 7073 290a 0a0a 6465 6620 5f65  (comps)...def _e
+0000bfb0: 6e63 6f64 655f 7065 7273 6f6e 6e61 6d65  ncode_personname
+0000bfc0: 280a 2020 2020 636f 6d70 6f6e 656e 7473  (.    components
+0000bfd0: 3a20 5365 7175 656e 6365 5b73 7472 5d2c  : Sequence[str],
+0000bfe0: 2065 6e63 6f64 696e 6773 3a20 5365 7175   encodings: Sequ
+0000bff0: 656e 6365 5b73 7472 5d0a 2920 2d3e 2062  ence[str].) -> b
+0000c000: 7974 6573 3a0a 2020 2020 2222 2245 6e63  ytes:.    """Enc
+0000c010: 6f64 6520 6120 6c69 7374 206f 6620 7465  ode a list of te
+0000c020: 7874 2073 7472 696e 6720 7065 7273 6f6e  xt string person
+0000c030: 206e 616d 6520 636f 6d70 6f6e 656e 7473   name components
+0000c040: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+0000c050: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0000c060: 0a20 2020 2063 6f6d 706f 6e65 6e74 7320  .    components 
+0000c070: 3a20 6c69 7374 206f 6620 7374 720a 2020  : list of str.  
+0000c080: 2020 2020 2020 5468 6520 6c69 7374 206f        The list o
+0000c090: 6620 7468 6520 7570 2074 6f20 7468 7265  f the up to thre
+0000c0a0: 6520 756e 6963 6f64 6520 7065 7273 6f6e  e unicode person
+0000c0b0: 206e 616d 6520 636f 6d70 6f6e 656e 7473   name components
+0000c0c0: 0a20 2020 2065 6e63 6f64 696e 6773 203a  .    encodings :
+0000c0d0: 206c 6973 7420 6f66 2073 7472 0a20 2020   list of str.   
+0000c0e0: 2020 2020 2054 6865 2050 7974 686f 6e20       The Python 
+0000c0f0: 656e 636f 6469 6e67 7320 7573 6573 2074  encodings uses t
+0000c100: 6f20 656e 636f 6465 2060 636f 6d70 6f6e  o encode `compon
+0000c110: 656e 7473 602e 0a0a 2020 2020 5265 7475  ents`...    Retu
+0000c120: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0000c130: 2020 2020 6279 7465 2073 7472 696e 670a      byte string.
+0000c140: 2020 2020 2020 2020 5468 6520 6279 7465          The byte
+0000c150: 2073 7472 696e 6720 7468 6174 2063 616e   string that can
+0000c160: 2062 6520 7772 6974 7465 6e20 6173 2061   be written as a
+0000c170: 2050 4e20 4449 434f 4d20 7461 6720 7661   PN DICOM tag va
+0000c180: 6c75 652e 0a20 2020 2020 2020 2049 6620  lue..        If 
+0000c190: 7468 6520 656e 636f 6469 6e67 206f 6620  the encoding of 
+0000c1a0: 736f 6d65 2063 6f6d 706f 6e65 6e74 2070  some component p
+0000c1b0: 6172 7473 2069 7320 6e6f 7420 706f 7373  arts is not poss
+0000c1c0: 6962 6c65 2075 7369 6e67 2074 6865 0a20  ible using the. 
+0000c1d0: 2020 2020 2020 2067 6976 656e 2065 6e63         given enc
+0000c1e0: 6f64 696e 6773 2c20 7468 6579 2061 7265  odings, they are
+0000c1f0: 2065 6e63 6f64 6564 2077 6974 6820 7468   encoded with th
+0000c200: 6520 6669 7273 7420 656e 636f 6469 6e67  e first encoding
+0000c210: 2075 7369 6e67 0a20 2020 2020 2020 2072   using.        r
+0000c220: 6570 6c61 6365 6d65 6e74 2062 7974 6573  eplacement bytes
+0000c230: 2066 6f72 2063 6861 7261 6374 6572 7320   for characters 
+0000c240: 7468 6174 2063 616e 6e6f 7420 6265 2065  that cannot be e
+0000c250: 6e63 6f64 6564 2e0a 2020 2020 2222 220a  ncoded..    """.
+0000c260: 2020 2020 6672 6f6d 2070 7964 6963 6f6d      from pydicom
+0000c270: 2e63 6861 7273 6574 2069 6d70 6f72 7420  .charset import 
+0000c280: 656e 636f 6465 5f73 7472 696e 670a 0a20  encode_string.. 
+0000c290: 2020 2065 6e63 6f64 6564 5f63 6f6d 7073     encoded_comps
+0000c2a0: 203d 205b 5d0a 2020 2020 666f 7220 636f   = [].    for co
+0000c2b0: 6d70 2069 6e20 636f 6d70 6f6e 656e 7473  mp in components
+0000c2c0: 3a0a 2020 2020 2020 2020 6772 6f75 7073  :.        groups
+0000c2d0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+0000c2e0: 2065 6e63 6f64 655f 7374 7269 6e67 2867   encode_string(g
+0000c2f0: 726f 7570 2c20 656e 636f 6469 6e67 7329  roup, encodings)
+0000c300: 2066 6f72 2067 726f 7570 2069 6e20 636f   for group in co
+0000c310: 6d70 2e73 706c 6974 2827 5e27 290a 2020  mp.split('^').  
+0000c320: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0000c330: 656e 636f 6465 645f 636f 6d70 203d 2062  encoded_comp = b
+0000c340: 275e 272e 6a6f 696e 2867 726f 7570 7329  '^'.join(groups)
+0000c350: 0a20 2020 2020 2020 2065 6e63 6f64 6564  .        encoded
+0000c360: 5f63 6f6d 7073 2e61 7070 656e 6428 656e  _comps.append(en
+0000c370: 636f 6465 645f 636f 6d70 290a 0a20 2020  coded_comp)..   
+0000c380: 2023 2052 656d 6f76 6520 656d 7074 7920   # Remove empty 
+0000c390: 656c 656d 656e 7473 2066 726f 6d20 7468  elements from th
+0000c3a0: 6520 656e 640a 2020 2020 7768 696c 6520  e end.    while 
+0000c3b0: 6c65 6e28 656e 636f 6465 645f 636f 6d70  len(encoded_comp
+0000c3c0: 7329 2061 6e64 206e 6f74 2065 6e63 6f64  s) and not encod
+0000c3d0: 6564 5f63 6f6d 7073 5b2d 315d 3a0a 2020  ed_comps[-1]:.  
+0000c3e0: 2020 2020 2020 656e 636f 6465 645f 636f        encoded_co
+0000c3f0: 6d70 732e 706f 7028 290a 2020 2020 7265  mps.pop().    re
+0000c400: 7475 726e 2062 273d 272e 6a6f 696e 2865  turn b'='.join(e
+0000c410: 6e63 6f64 6564 5f63 6f6d 7073 290a 0a0a  ncoded_comps)...
+0000c420: 636c 6173 7320 5065 7273 6f6e 4e61 6d65  class PersonName
+0000c430: 3a0a 2020 2020 2222 2252 6570 7265 7365  :.    """Represe
+0000c440: 6e74 6174 696f 6e20 6f66 2074 6865 2076  ntation of the v
+0000c450: 616c 7565 2066 6f72 2061 6e20 656c 656d  alue for an elem
+0000c460: 656e 7420 7769 7468 2056 5220 2a2a 504e  ent with VR **PN
+0000c470: 2a2a 2e22 2222 0a20 2020 2064 6566 205f  **.""".    def _
+0000c480: 5f6e 6577 5f5f 2820 2023 2074 7970 653a  _new__(  # type:
+0000c490: 2069 676e 6f72 655b 6d69 7363 5d0a 2020   ignore[misc].  
+0000c4a0: 2020 2020 2020 636c 733a 2054 7970 655b        cls: Type[
+0000c4b0: 2250 6572 736f 6e4e 616d 6522 5d2c 202a  "PersonName"], *
+0000c4c0: 6172 6773 3a20 416e 792c 202a 2a6b 7761  args: Any, **kwa
+0000c4d0: 7267 733a 2041 6e79 0a20 2020 2029 202d  rgs: Any.    ) -
+0000c4e0: 3e20 4f70 7469 6f6e 616c 5b22 5065 7273  > Optional["Pers
+0000c4f0: 6f6e 4e61 6d65 225d 3a0a 2020 2020 2020  onName"]:.      
+0000c500: 2020 6966 206c 656e 2861 7267 7329 2061    if len(args) a
+0000c510: 6e64 2061 7267 735b 305d 2069 7320 4e6f  nd args[0] is No
+0000c520: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000c530: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+0000c540: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+0000c550: 7228 292e 5f5f 6e65 775f 5f28 636c 7329  r().__new__(cls)
+0000c560: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+0000c570: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0000c580: 2c0a 2020 2020 2020 2020 7661 6c3a 2055  ,.        val: U
+0000c590: 6e69 6f6e 5b62 7974 6573 2c20 7374 722c  nion[bytes, str,
+0000c5a0: 2022 5065 7273 6f6e 4e61 6d65 225d 2c0a   "PersonName"],.
+0000c5b0: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
+0000c5c0: 733a 204f 7074 696f 6e61 6c5b 5365 7175  s: Optional[Sequ
+0000c5d0: 656e 6365 5b73 7472 5d5d 203d 204e 6f6e  ence[str]] = Non
+0000c5e0: 652c 0a20 2020 2020 2020 206f 7269 6769  e,.        origi
+0000c5f0: 6e61 6c5f 7374 7269 6e67 3a20 4f70 7469  nal_string: Opti
+0000c600: 6f6e 616c 5b62 7974 6573 5d20 3d20 4e6f  onal[bytes] = No
+0000c610: 6e65 2c0a 2020 2020 2020 2020 7661 6c69  ne,.        vali
+0000c620: 6461 7469 6f6e 5f6d 6f64 653a 2069 6e74  dation_mode: int
+0000c630: 203d 204e 6f6e 650a 2020 2020 2920 2d3e   = None.    ) ->
+0000c640: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000c650: 2222 4372 6561 7465 2061 206e 6577 2060  ""Create a new `
+0000c660: 6050 6572 736f 6e4e 616d 6560 602e 0a0a  `PersonName``...
+0000c670: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000c680: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0000c690: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
+0000c6a0: 6c3a 2073 7472 2c20 6279 7465 732c 2050  l: str, bytes, P
+0000c6b0: 6572 736f 6e4e 616d 650a 2020 2020 2020  ersonName.      
+0000c6c0: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
+0000c6d0: 746f 2075 7365 2066 6f72 2074 6865 202a  to use for the *
+0000c6e0: 2a50 4e2a 2a20 656c 656d 656e 742e 0a20  *PN** element.. 
+0000c6f0: 2020 2020 2020 2065 6e63 6f64 696e 6773         encodings
+0000c700: 3a20 6c69 7374 206f 6620 7374 722c 206f  : list of str, o
+0000c710: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000c720: 2020 2020 4120 6c69 7374 206f 6620 7468      A list of th
+0000c730: 6520 656e 636f 6469 6e67 7320 7573 6564  e encodings used
+0000c740: 2066 6f72 2074 6865 2076 616c 7565 2e0a   for the value..
+0000c750: 2020 2020 2020 2020 6f72 6967 696e 616c          original
+0000c760: 5f73 7472 696e 673a 2062 7974 6573 2c20  _string: bytes, 
+0000c770: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000c780: 2020 2020 2057 6865 6e20 6372 6561 7469       When creati
+0000c790: 6e67 2061 2060 6050 6572 736f 6e4e 616d  ng a ``PersonNam
+0000c7a0: 6560 6020 7573 696e 6720 6120 6465 636f  e`` using a deco
+0000c7b0: 6465 6420 7374 7269 6e67 2c20 7468 6973  ded string, this
+0000c7c0: 2069 7320 7468 650a 2020 2020 2020 2020   is the.        
+0000c7d0: 2020 2020 6f72 6967 696e 616c 2065 6e63      original enc
+0000c7e0: 6f64 6564 2076 616c 7565 2e0a 0a20 2020  oded value...   
+0000c7f0: 2020 2020 204e 6f74 6573 0a20 2020 2020       Notes.     
+0000c800: 2020 202d 2d2d 2d2d 0a20 2020 2020 2020     -----.       
+0000c810: 2041 203a 636c 6173 733a 6050 6572 736f   A :class:`Perso
+0000c820: 6e4e 616d 6560 206d 6179 2061 6c73 6f20  nName` may also 
+0000c830: 6265 2063 6f6e 7374 7275 6374 6564 2062  be constructed b
+0000c840: 7920 7370 6563 6966 7969 6e67 2069 6e64  y specifying ind
+0000c850: 6976 6964 7561 6c0a 2020 2020 2020 2020  ividual.        
+0000c860: 636f 6d70 6f6e 656e 7473 2075 7369 6e67  components using
+0000c870: 2074 6865 203a 6d65 7468 3a60 6672 6f6d   the :meth:`from
+0000c880: 5f6e 616d 6564 5f63 6f6d 706f 6e65 6e74  _named_component
+0000c890: 7360 2061 6e64 0a20 2020 2020 2020 203a  s` and.        :
+0000c8a0: 6d65 7468 3a60 6672 6f6d 5f6e 616d 6564  meth:`from_named
+0000c8b0: 5f63 6f6d 706f 6e65 6e74 735f 7665 7465  _components_vete
+0000c8c0: 7269 6e61 7279 6020 636c 6173 7320 6d65  rinary` class me
+0000c8d0: 7468 6f64 732e 0a20 2020 2020 2020 2022  thods..        "
+0000c8e0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+0000c8f0: 6f72 6967 696e 616c 5f73 7472 696e 673a  original_string:
+0000c900: 2062 7974 6573 0a20 2020 2020 2020 2073   bytes.        s
+0000c910: 656c 662e 5f63 6f6d 706f 6e65 6e74 733a  elf._components:
+0000c920: 204f 7074 696f 6e61 6c5b 5475 706c 655b   Optional[Tuple[
+0000c930: 7374 722c 202e 2e2e 5d5d 203d 204e 6f6e  str, ...]] = Non
+0000c940: 650a 2020 2020 2020 2020 7365 6c66 2e65  e.        self.e
+0000c950: 6e63 6f64 696e 6773 3a20 4f70 7469 6f6e  ncodings: Option
+0000c960: 616c 5b54 7570 6c65 5b73 7472 2c20 2e2e  al[Tuple[str, ..
+0000c970: 2e5d 5d0a 2020 2020 2020 2020 6966 2076  .]].        if v
+0000c980: 616c 6964 6174 696f 6e5f 6d6f 6465 2069  alidation_mode i
+0000c990: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000c9a0: 2020 2020 7661 6c69 6461 7469 6f6e 5f6d      validation_m
+0000c9b0: 6f64 6520 3d20 636f 6e66 6967 2e73 6574  ode = config.set
+0000c9c0: 7469 6e67 732e 7265 6164 696e 675f 7661  tings.reading_va
+0000c9d0: 6c69 6461 7469 6f6e 5f6d 6f64 650a 2020  lidation_mode.  
+0000c9e0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0000c9f0: 6174 696f 6e5f 6d6f 6465 203d 2076 616c  ation_mode = val
+0000ca00: 6964 6174 696f 6e5f 6d6f 6465 0a0a 2020  idation_mode..  
+0000ca10: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000ca20: 6e63 6528 7661 6c2c 2050 6572 736f 6e4e  nce(val, PersonN
+0000ca30: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
+0000ca40: 2020 656e 636f 6469 6e67 7320 3d20 7661    encodings = va
+0000ca50: 6c2e 656e 636f 6469 6e67 730a 2020 2020  l.encodings.    
+0000ca60: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
+0000ca70: 6769 6e61 6c5f 7374 7269 6e67 203d 2076  ginal_string = v
+0000ca80: 616c 2e6f 7269 6769 6e61 6c5f 7374 7269  al.original_stri
+0000ca90: 6e67 0a20 2020 2020 2020 2020 2020 2073  ng.            s
+0000caa0: 656c 662e 5f63 6f6d 706f 6e65 6e74 7320  elf._components 
+0000cab0: 3d20 7475 706c 6528 7374 7228 7661 6c29  = tuple(str(val)
+0000cac0: 2e73 706c 6974 2827 3d27 2929 0a20 2020  .split('=')).   
+0000cad0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+0000cae0: 616e 6365 2876 616c 2c20 6279 7465 7329  ance(val, bytes)
+0000caf0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000cb00: 7468 6973 2069 7320 7468 6520 7261 7720  this is the raw 
+0000cb10: 6279 7465 2073 7472 696e 6720 2d20 6465  byte string - de
+0000cb20: 636f 6465 2069 7420 6f6e 2064 656d 616e  code it on deman
+0000cb30: 640a 2020 2020 2020 2020 2020 2020 7365  d.            se
+0000cb40: 6c66 2e6f 7269 6769 6e61 6c5f 7374 7269  lf.original_stri
+0000cb50: 6e67 203d 2076 616c 0a20 2020 2020 2020  ng = val.       
+0000cb60: 2020 2020 2076 616c 6964 6174 655f 7661       validate_va
+0000cb70: 6c75 6528 2250 4e22 2c20 7661 6c2c 2076  lue("PN", val, v
+0000cb80: 616c 6964 6174 696f 6e5f 6d6f 6465 290a  alidation_mode).
+0000cb90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cba0: 2e5f 636f 6d70 6f6e 656e 7473 203d 204e  ._components = N
+0000cbb0: 6f6e 650a 2020 2020 2020 2020 656c 7365  one.        else
+0000cbc0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000cbd0: 7661 6c3a 2073 7472 0a20 2020 2020 2020  val: str.       
+0000cbe0: 2020 2020 2023 2060 7661 6c60 2069 7320       # `val` is 
+0000cbf0: 7468 6520 6465 636f 6465 6420 7065 7273  the decoded pers
+0000cc00: 6f6e 206e 616d 6520 7661 6c75 650a 2020  on name value.  
+0000cc10: 2020 2020 2020 2020 2020 2320 606f 7269            # `ori
+0000cc20: 6769 6e61 6c5f 7374 7269 6e67 6020 7368  ginal_string` sh
+0000cc30: 6f75 6c64 2062 6520 7468 6520 6f72 6967  ould be the orig
+0000cc40: 696e 616c 2065 6e63 6f64 6564 2076 616c  inal encoded val
+0000cc50: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
+0000cc60: 656c 662e 6f72 6967 696e 616c 5f73 7472  elf.original_str
+0000cc70: 696e 6720 3d20 6361 7374 2862 7974 6573  ing = cast(bytes
+0000cc80: 2c20 6f72 6967 696e 616c 5f73 7472 696e  , original_strin
+0000cc90: 6729 0a20 2020 2020 2020 2020 2020 2023  g).            #
+0000cca0: 2069 6620 7765 2064 6f6e 2774 2068 6176   if we don't hav
+0000ccb0: 6520 7468 6520 6279 7465 2073 7472 696e  e the byte strin
+0000ccc0: 6720 6174 2074 6869 7320 706f 696e 742c  g at this point,
+0000ccd0: 2077 6520 6174 206c 6561 7374 0a20 2020   we at least.   
+0000cce0: 2020 2020 2020 2020 2023 2076 616c 6964           # valid
+0000ccf0: 6174 6520 7468 6520 6c65 6e67 7468 206f  ate the length o
+0000cd00: 6620 7468 6520 7374 7269 6e67 2063 6f6d  f the string com
+0000cd10: 706f 6e65 6e74 730a 2020 2020 2020 2020  ponents.        
+0000cd20: 2020 2020 7661 6c69 6461 7465 5f76 616c      validate_val
+0000cd30: 7565 2822 504e 222c 206f 7269 6769 6e61  ue("PN", origina
+0000cd40: 6c5f 7374 7269 6e67 2069 6620 6f72 6967  l_string if orig
+0000cd50: 696e 616c 5f73 7472 696e 6720 656c 7365  inal_string else
+0000cd60: 2076 616c 2c0a 2020 2020 2020 2020 2020   val,.          
+0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd80: 2076 616c 6964 6174 696f 6e5f 6d6f 6465   validation_mode
+0000cd90: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+0000cda0: 6d70 6f6e 656e 7473 203d 2076 616c 2e73  mponents = val.s
+0000cdb0: 706c 6974 2827 3d27 290a 2020 2020 2020  plit('=').      
+0000cdc0: 2020 2020 2020 2320 5265 6d6f 7665 2065        # Remove e
+0000cdd0: 6d70 7479 2065 6c65 6d65 6e74 7320 6672  mpty elements fr
+0000cde0: 6f6d 2074 6865 2065 6e64 2074 6f20 6176  om the end to av
+0000cdf0: 6f69 6420 7472 6169 6c69 6e67 2027 3d27  oid trailing '='
+0000ce00: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+0000ce10: 6c65 206c 656e 2863 6f6d 706f 6e65 6e74  le len(component
+0000ce20: 7329 2061 6e64 206e 6f74 2063 6f6d 706f  s) and not compo
+0000ce30: 6e65 6e74 735b 2d31 5d3a 0a20 2020 2020  nents[-1]:.     
+0000ce40: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
+0000ce50: 6e65 6e74 732e 706f 7028 290a 2020 2020  nents.pop().    
+0000ce60: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+0000ce70: 6d70 6f6e 656e 7473 203d 2074 7570 6c65  mponents = tuple
+0000ce80: 2863 6f6d 706f 6e65 6e74 7329 0a0a 2020  (components)..  
+0000ce90: 2020 2020 2020 2020 2020 2320 6966 2074            # if t
+0000cea0: 6865 2065 6e63 6f64 696e 6720 6973 206e  he encoding is n
+0000ceb0: 6f74 2067 6976 656e 2c20 6c65 6176 6520  ot given, leave 
+0000cec0: 6974 2061 7320 756e 6465 6669 6e65 6420  it as undefined 
+0000ced0: 284e 6f6e 6529 0a20 2020 2020 2020 2073  (None).        s
+0000cee0: 656c 662e 656e 636f 6469 6e67 7320 3d20  elf.encodings = 
+0000cef0: 5f76 6572 6966 795f 656e 636f 6469 6e67  _verify_encoding
+0000cf00: 7328 656e 636f 6469 6e67 7329 0a0a 2020  s(encodings)..  
+0000cf10: 2020 6465 6620 5f63 7265 6174 655f 6469    def _create_di
+0000cf20: 6374 2873 656c 6629 202d 3e20 4469 6374  ct(self) -> Dict
+0000cf30: 5b73 7472 2c20 7374 725d 3a0a 2020 2020  [str, str]:.    
+0000cf40: 2020 2020 2222 2243 7265 6174 6573 2061      """Creates a
+0000cf50: 2064 6963 7469 6f6e 6172 7920 6f66 2070   dictionary of p
+0000cf60: 6572 736f 6e20 6e61 6d65 2067 726f 7570  erson name group
+0000cf70: 2061 6e64 2063 6f6d 706f 6e65 6e74 206e   and component n
+0000cf80: 616d 6573 2e0a 0a20 2020 2020 2020 2055  ames...        U
+0000cf90: 7365 6420 6578 636c 7573 6976 656c 7920  sed exclusively 
+0000cfa0: 666f 7220 6066 6f72 6d61 7474 6564 6020  for `formatted` 
+0000cfb0: 666f 7220 6261 636b 7761 7264 7320 636f  for backwards co
+0000cfc0: 6d70 6174 6962 696c 6974 792e 0a20 2020  mpatibility..   
+0000cfd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000cfe0: 2070 6172 7473 203d 205b 0a20 2020 2020   parts = [.     
+0000cff0: 2020 2020 2020 2027 6661 6d69 6c79 5f6e         'family_n
+0000d000: 616d 6527 2c20 2767 6976 656e 5f6e 616d  ame', 'given_nam
+0000d010: 6527 2c20 276d 6964 646c 655f 6e61 6d65  e', 'middle_name
+0000d020: 272c 2027 6e61 6d65 5f70 7265 6669 7827  ', 'name_prefix'
+0000d030: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
+0000d040: 616d 655f 7375 6666 6978 272c 2027 6964  ame_suffix', 'id
+0000d050: 656f 6772 6170 6869 6327 2c20 2770 686f  eographic', 'pho
+0000d060: 6e65 7469 6327 0a20 2020 2020 2020 205d  netic'.        ]
+0000d070: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d080: 7b63 3a20 6765 7461 7474 7228 7365 6c66  {c: getattr(self
+0000d090: 2c20 632c 2027 2729 2066 6f72 2063 2069  , c, '') for c i
+0000d0a0: 6e20 7061 7274 737d 0a0a 2020 2020 4070  n parts}..    @p
+0000d0b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000d0c0: 636f 6d70 6f6e 656e 7473 2873 656c 6629  components(self)
+0000d0d0: 202d 3e20 5475 706c 655b 7374 722c 202e   -> Tuple[str, .
+0000d0e0: 2e2e 5d3a 0a20 2020 2020 2020 2022 2222  ..]:.        """
+0000d0f0: 5265 7475 726e 7320 7570 2074 6f20 7468  Returns up to th
+0000d100: 7265 6520 6465 636f 6465 6420 7065 7273  ree decoded pers
+0000d110: 6f6e 206e 616d 6520 636f 6d70 6f6e 656e  on name componen
+0000d120: 7473 2061 7320 610a 2020 2020 2020 2020  ts as a.        
+0000d130: 3a63 6c61 7373 3a60 7475 706c 6560 206f  :class:`tuple` o
+0000d140: 6620 3a63 6c61 7373 3a60 7374 7260 2e0a  f :class:`str`..
+0000d150: 0a20 2020 2020 2020 202e 2e20 7665 7273  .        .. vers
+0000d160: 696f 6e61 6464 6564 3a3a 2031 2e32 0a0a  ionadded:: 1.2..
+0000d170: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000d180: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000d190: 2020 2020 2020 2020 5475 706c 655b 7374          Tuple[st
+0000d1a0: 722c 202e 2e2e 5d0a 2020 2020 2020 2020  r, ...].        
+0000d1b0: 2020 2020 5468 6520 2861 6c70 6861 6265      The (alphabe
+0000d1c0: 7469 632c 2069 6465 6f67 7261 7068 6963  tic, ideographic
+0000d1d0: 2c20 7068 6f6e 6574 6963 2920 636f 6d70  , phonetic) comp
+0000d1e0: 6f6e 656e 7473 206f 6620 7468 650a 2020  onents of the.  
+0000d1f0: 2020 2020 2020 2020 2020 6465 636f 6465            decode
+0000d200: 6420 7065 7273 6f6e 206e 616d 652e 2041  d person name. A
+0000d210: 6e79 206f 6620 7468 6520 636f 6d70 6f6e  ny of the compon
+0000d220: 656e 7473 206d 6179 2062 6520 6162 7365  ents may be abse
+0000d230: 6e74 2e0a 2020 2020 2020 2020 2222 220a  nt..        """.
+0000d240: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d250: 5f63 6f6d 706f 6e65 6e74 7320 6973 204e  _components is N
+0000d260: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d270: 2067 726f 7570 7320 3d20 7365 6c66 2e6f   groups = self.o
+0000d280: 7269 6769 6e61 6c5f 7374 7269 6e67 2e73  riginal_string.s
+0000d290: 706c 6974 2862 273d 2729 0a20 2020 2020  plit(b'=').     
+0000d2a0: 2020 2020 2020 2065 6e63 6f64 696e 6773         encodings
+0000d2b0: 203d 2073 656c 662e 656e 636f 6469 6e67   = self.encoding
+0000d2c0: 7320 6f72 205b 6465 6661 756c 745f 656e  s or [default_en
+0000d2d0: 636f 6469 6e67 5d0a 2020 2020 2020 2020  coding].        
+0000d2e0: 2020 2020 7365 6c66 2e5f 636f 6d70 6f6e      self._compon
+0000d2f0: 656e 7473 203d 205f 6465 636f 6465 5f70  ents = _decode_p
+0000d300: 6572 736f 6e6e 616d 6528 6772 6f75 7073  ersonname(groups
+0000d310: 2c20 656e 636f 6469 6e67 7329 0a0a 2020  , encodings)..  
+0000d320: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000d330: 662e 5f63 6f6d 706f 6e65 6e74 730a 0a20  f._components.. 
+0000d340: 2020 2064 6566 205f 6e61 6d65 5f70 6172     def _name_par
+0000d350: 7428 7365 6c66 2c20 693a 2069 6e74 2920  t(self, i: int) 
+0000d360: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+0000d370: 2222 2252 6574 7572 6e20 7468 6520 6069  """Return the `i
+0000d380: 6074 6820 7061 7274 206f 6620 7468 6520  `th part of the 
+0000d390: 6e61 6d65 2e22 2222 0a20 2020 2020 2020  name.""".       
+0000d3a0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000d3b0: 2020 7265 7475 726e 2073 656c 662e 636f    return self.co
+0000d3c0: 6d70 6f6e 656e 7473 5b30 5d2e 7370 6c69  mponents[0].spli
+0000d3d0: 7428 275e 2729 5b69 5d0a 2020 2020 2020  t('^')[i].      
+0000d3e0: 2020 6578 6365 7074 2049 6e64 6578 4572    except IndexEr
+0000d3f0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+0000d400: 2072 6574 7572 6e20 2727 0a0a 2020 2020   return ''..    
+0000d410: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000d420: 6620 6661 6d69 6c79 5f6e 616d 6528 7365  f family_name(se
+0000d430: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+0000d440: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+0000d450: 6520 6669 7273 7420 2866 616d 696c 7920  e first (family 
+0000d460: 6e61 6d65 2920 6772 6f75 7020 6f66 2074  name) group of t
+0000d470: 6865 2061 6c70 6861 6265 7469 6320 7065  he alphabetic pe
+0000d480: 7273 6f6e 206e 616d 650a 2020 2020 2020  rson name.      
+0000d490: 2020 7265 7072 6573 656e 7461 7469 6f6e    representation
+0000d4a0: 2061 7320 6120 756e 6963 6f64 6520 7374   as a unicode st
+0000d4b0: 7269 6e67 0a0a 2020 2020 2020 2020 2e2e  ring..        ..
+0000d4c0: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
+0000d4d0: 312e 320a 2020 2020 2020 2020 2222 220a  1.2.        """.
+0000d4e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000d4f0: 656c 662e 5f6e 616d 655f 7061 7274 2830  elf._name_part(0
+0000d500: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000d510: 0a20 2020 2064 6566 2067 6976 656e 5f6e  .    def given_n
+0000d520: 616d 6528 7365 6c66 2920 2d3e 2073 7472  ame(self) -> str
+0000d530: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+0000d540: 7572 6e20 7468 6520 7365 636f 6e64 2028  urn the second (
+0000d550: 6769 7665 6e20 6e61 6d65 2920 6772 6f75  given name) grou
+0000d560: 7020 6f66 2074 6865 2061 6c70 6861 6265  p of the alphabe
+0000d570: 7469 6320 7065 7273 6f6e 206e 616d 650a  tic person name.
+0000d580: 2020 2020 2020 2020 7265 7072 6573 656e          represen
+0000d590: 7461 7469 6f6e 2061 7320 6120 756e 6963  tation as a unic
+0000d5a0: 6f64 6520 7374 7269 6e67 0a0a 2020 2020  ode string..    
+0000d5b0: 2020 2020 2e2e 2076 6572 7369 6f6e 6164      .. versionad
+0000d5c0: 6465 643a 3a20 312e 320a 2020 2020 2020  ded:: 1.2.      
+0000d5d0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000d5e0: 7475 726e 2073 656c 662e 5f6e 616d 655f  turn self._name_
+0000d5f0: 7061 7274 2831 290a 0a20 2020 2040 7072  part(1)..    @pr
+0000d600: 6f70 6572 7479 0a20 2020 2064 6566 206d  operty.    def m
+0000d610: 6964 646c 655f 6e61 6d65 2873 656c 6629  iddle_name(self)
+0000d620: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0000d630: 2022 2222 5265 7475 726e 2074 6865 2074   """Return the t
+0000d640: 6869 7264 2028 6d69 6464 6c65 206e 616d  hird (middle nam
+0000d650: 6529 2067 726f 7570 206f 6620 7468 6520  e) group of the 
+0000d660: 616c 7068 6162 6574 6963 2070 6572 736f  alphabetic perso
+0000d670: 6e20 6e61 6d65 0a20 2020 2020 2020 2072  n name.        r
+0000d680: 6570 7265 7365 6e74 6174 696f 6e20 6173  epresentation as
+0000d690: 2061 2075 6e69 636f 6465 2073 7472 696e   a unicode strin
+0000d6a0: 670a 0a20 2020 2020 2020 202e 2e20 7665  g..        .. ve
+0000d6b0: 7273 696f 6e61 6464 6564 3a3a 2031 2e32  rsionadded:: 1.2
+0000d6c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d6d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000d6e0: 2e5f 6e61 6d65 5f70 6172 7428 3229 0a0a  ._name_part(2)..
+0000d6f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000d700: 2020 6465 6620 6e61 6d65 5f70 7265 6669    def name_prefi
+0000d710: 7828 7365 6c66 2920 2d3e 2073 7472 3a0a  x(self) -> str:.
+0000d720: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+0000d730: 6e20 7468 6520 666f 7572 7468 2028 6e61  n the fourth (na
+0000d740: 6d65 2070 7265 6669 7829 2067 726f 7570  me prefix) group
+0000d750: 206f 6620 7468 6520 616c 7068 6162 6574   of the alphabet
+0000d760: 6963 2070 6572 736f 6e20 6e61 6d65 0a20  ic person name. 
+0000d770: 2020 2020 2020 2072 6570 7265 7365 6e74         represent
+0000d780: 6174 696f 6e20 6173 2061 2075 6e69 636f  ation as a unico
+0000d790: 6465 2073 7472 696e 670a 0a20 2020 2020  de string..     
+0000d7a0: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
+0000d7b0: 6564 3a3a 2031 2e32 0a20 2020 2020 2020  ed:: 1.2.       
+0000d7c0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+0000d7d0: 7572 6e20 7365 6c66 2e5f 6e61 6d65 5f70  urn self._name_p
+0000d7e0: 6172 7428 3329 0a0a 2020 2020 4070 726f  art(3)..    @pro
+0000d7f0: 7065 7274 790a 2020 2020 6465 6620 6e61  perty.    def na
+0000d800: 6d65 5f73 7566 6669 7828 7365 6c66 2920  me_suffix(self) 
+0000d810: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+0000d820: 2222 2252 6574 7572 6e20 7468 6520 6669  """Return the fi
+0000d830: 6674 6820 286e 616d 6520 7375 6666 6978  fth (name suffix
+0000d840: 2920 6772 6f75 7020 6f66 2074 6865 2061  ) group of the a
+0000d850: 6c70 6861 6265 7469 6320 7065 7273 6f6e  lphabetic person
+0000d860: 206e 616d 650a 2020 2020 2020 2020 7265   name.        re
+0000d870: 7072 6573 656e 7461 7469 6f6e 2061 7320  presentation as 
+0000d880: 6120 756e 6963 6f64 6520 7374 7269 6e67  a unicode string
+0000d890: 0a0a 2020 2020 2020 2020 2e2e 2076 6572  ..        .. ver
+0000d8a0: 7369 6f6e 6164 6465 643a 3a20 312e 320a  sionadded:: 1.2.
+0000d8b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d8c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000d8d0: 5f6e 616d 655f 7061 7274 2834 290a 0a20  _name_part(4).. 
+0000d8e0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000d8f0: 2064 6566 2061 6c70 6861 6265 7469 6328   def alphabetic(
+0000d900: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+0000d910: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+0000d920: 7468 6520 6669 7273 7420 2861 6c70 6861  the first (alpha
+0000d930: 6265 7469 6329 2070 6572 736f 6e20 6e61  betic) person na
+0000d940: 6d65 2063 6f6d 706f 6e65 6e74 2061 7320  me component as 
+0000d950: 610a 2020 2020 2020 2020 756e 6963 6f64  a.        unicod
+0000d960: 6520 7374 7269 6e67 0a20 2020 2020 2020  e string.       
+0000d970: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
+0000d980: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000d990: 7475 726e 2073 656c 662e 636f 6d70 6f6e  turn self.compon
+0000d9a0: 656e 7473 5b30 5d0a 2020 2020 2020 2020  ents[0].        
+0000d9b0: 6578 6365 7074 2049 6e64 6578 4572 726f  except IndexErro
+0000d9c0: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+0000d9d0: 6574 7572 6e20 2727 0a0a 2020 2020 4070  eturn ''..    @p
+0000d9e0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000d9f0: 6964 656f 6772 6170 6869 6328 7365 6c66  ideographic(self
+0000da00: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+0000da10: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
+0000da20: 7365 636f 6e64 2028 6964 656f 6772 6170  second (ideograp
+0000da30: 6869 6329 2070 6572 736f 6e20 6e61 6d65  hic) person name
+0000da40: 2063 6f6d 706f 6e65 6e74 2061 7320 610a   component as a.
+0000da50: 2020 2020 2020 2020 756e 6963 6f64 6520          unicode 
+0000da60: 7374 7269 6e67 0a0a 2020 2020 2020 2020  string..        
+0000da70: 2e2e 2076 6572 7369 6f6e 6164 6465 643a  .. versionadded:
+0000da80: 3a20 312e 320a 2020 2020 2020 2020 2222  : 1.2.        ""
+0000da90: 220a 2020 2020 2020 2020 7472 793a 0a20  ".        try:. 
+0000daa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000dab0: 6e20 7365 6c66 2e63 6f6d 706f 6e65 6e74  n self.component
+0000dac0: 735b 315d 0a20 2020 2020 2020 2065 7863  s[1].        exc
+0000dad0: 6570 7420 496e 6465 7845 7272 6f72 3a0a  ept IndexError:.
+0000dae0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000daf0: 726e 2027 270a 0a20 2020 2040 7072 6f70  rn ''..    @prop
+0000db00: 6572 7479 0a20 2020 2064 6566 2070 686f  erty.    def pho
+0000db10: 6e65 7469 6328 7365 6c66 2920 2d3e 2073  netic(self) -> s
+0000db20: 7472 3a0a 2020 2020 2020 2020 2222 2252  tr:.        """R
+0000db30: 6574 7572 6e20 7468 6520 7468 6972 6420  eturn the third 
+0000db40: 2870 686f 6e65 7469 6329 2070 6572 736f  (phonetic) perso
+0000db50: 6e20 6e61 6d65 2063 6f6d 706f 6e65 6e74  n name component
+0000db60: 2061 7320 610a 2020 2020 2020 2020 756e   as a.        un
+0000db70: 6963 6f64 6520 7374 7269 6e67 0a0a 2020  icode string..  
+0000db80: 2020 2020 2020 2e2e 2076 6572 7369 6f6e        .. version
+0000db90: 6164 6465 643a 3a20 312e 320a 2020 2020  added:: 1.2.    
+0000dba0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000dbb0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000dbc0: 2072 6574 7572 6e20 7365 6c66 2e63 6f6d   return self.com
+0000dbd0: 706f 6e65 6e74 735b 325d 0a20 2020 2020  ponents[2].     
+0000dbe0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
+0000dbf0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+0000dc00: 2020 7265 7475 726e 2027 270a 0a20 2020    return ''..   
+0000dc10: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
+0000dc20: 2c20 6f74 6865 723a 2041 6e79 2920 2d3e  , other: Any) ->
+0000dc30: 2041 6e79 3a0a 2020 2020 2020 2020 2222   Any:.        ""
+0000dc40: 2252 6574 7572 6e20 6060 5472 7565 6060  "Return ``True``
+0000dc50: 2069 6620 606f 7468 6572 6020 6571 7561   if `other` equa
+0000dc60: 6c73 2074 6865 2063 7572 7265 6e74 206e  ls the current n
+0000dc70: 616d 652e 2222 220a 2020 2020 2020 2020  ame.""".        
+0000dc80: 7265 7475 726e 2073 7472 2873 656c 6629  return str(self)
+0000dc90: 203d 3d20 6f74 6865 720a 0a20 2020 2064   == other..    d
+0000dca0: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
+0000dcb0: 6f74 6865 723a 2041 6e79 2920 2d3e 2041  other: Any) -> A
+0000dcc0: 6e79 3a0a 2020 2020 2020 2020 2222 2252  ny:.        """R
+0000dcd0: 6574 7572 6e20 6060 5472 7565 6060 2069  eturn ``True`` i
+0000dce0: 6620 606f 7468 6572 6020 646f 6573 6e27  f `other` doesn'
+0000dcf0: 7420 6571 7561 6c20 7468 6520 6375 7272  t equal the curr
+0000dd00: 656e 7420 6e61 6d65 2e22 2222 0a20 2020  ent name.""".   
+0000dd10: 2020 2020 2072 6574 7572 6e20 6e6f 7420       return not 
+0000dd20: 7365 6c66 203d 3d20 6f74 6865 720a 0a20  self == other.. 
+0000dd30: 2020 2064 6566 205f 5f73 7472 5f5f 2873     def __str__(s
+0000dd40: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+0000dd50: 2020 2020 2022 2222 5265 7475 726e 2061       """Return a
+0000dd60: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
+0000dd70: 7461 7469 6f6e 206f 6620 7468 6520 6e61  tation of the na
+0000dd80: 6d65 2e22 2222 0a20 2020 2020 2020 2072  me.""".        r
+0000dd90: 6574 7572 6e20 273d 272e 6a6f 696e 2873  eturn '='.join(s
+0000dda0: 656c 662e 636f 6d70 6f6e 656e 7473 292e  elf.components).
+0000ddb0: 5f5f 7374 725f 5f28 290a 0a20 2020 2064  __str__()..    d
+0000ddc0: 6566 205f 5f69 7465 725f 5f28 7365 6c66  ef __iter__(self
+0000ddd0: 2920 2d3e 2049 7465 7261 746f 725b 7374  ) -> Iterator[st
+0000dde0: 725d 3a0a 2020 2020 2020 2020 2222 2249  r]:.        """I
+0000ddf0: 7465 7261 7465 2074 6872 6f75 6768 2074  terate through t
+0000de00: 6865 206e 616d 652e 2222 220a 2020 2020  he name.""".    
+0000de10: 2020 2020 7969 656c 6420 6672 6f6d 2073      yield from s
+0000de20: 656c 662e 5f5f 7374 725f 5f28 290a 0a20  elf.__str__().. 
+0000de30: 2020 2064 6566 205f 5f6c 656e 5f5f 2873     def __len__(s
+0000de40: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+0000de50: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
+0000de60: 6865 206c 656e 6774 6820 6f66 2074 6865  he length of the
+0000de70: 2070 6572 736f 6e20 6e61 6d65 2e22 2222   person name."""
+0000de80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000de90: 6c65 6e28 7365 6c66 2e5f 5f73 7472 5f5f  len(self.__str__
+0000dea0: 2829 290a 0a20 2020 2064 6566 205f 5f63  ())..    def __c
+0000deb0: 6f6e 7461 696e 735f 5f28 7365 6c66 2c20  ontains__(self, 
+0000dec0: 783a 2041 6e79 2920 2d3e 2062 6f6f 6c3a  x: Any) -> bool:
+0000ded0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+0000dee0: 726e 2060 6054 7275 6560 6020 6966 2060  rn ``True`` if `
+0000def0: 7860 2069 7320 696e 2074 6865 206e 616d  x` is in the nam
+0000df00: 652e 2222 220a 2020 2020 2020 2020 7265  e.""".        re
+0000df10: 7475 726e 2078 2069 6e20 7365 6c66 2e5f  turn x in self._
+0000df20: 5f73 7472 5f5f 2829 0a0a 2020 2020 6465  _str__()..    de
+0000df30: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
+0000df40: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0000df50: 2022 2222 5265 7475 726e 2061 2072 6570   """Return a rep
+0000df60: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
+0000df70: 6865 206e 616d 652e 2222 220a 2020 2020  he name.""".    
+0000df80: 2020 2020 7265 7475 726e 2027 3d27 2e6a      return '='.j
+0000df90: 6f69 6e28 7365 6c66 2e63 6f6d 706f 6e65  oin(self.compone
+0000dfa0: 6e74 7329 2e5f 5f72 6570 725f 5f28 290a  nts).__repr__().
+0000dfb0: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
+0000dfc0: 5f28 7365 6c66 2920 2d3e 2069 6e74 3a0a  _(self) -> int:.
+0000dfd0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+0000dfe0: 6e20 6120 6861 7368 206f 6620 7468 6520  n a hash of the 
+0000dff0: 6e61 6d65 2e22 2222 0a20 2020 2020 2020  name.""".       
+0000e000: 2072 6574 7572 6e20 6861 7368 2873 656c   return hash(sel
+0000e010: 662e 636f 6d70 6f6e 656e 7473 290a 0a20  f.components).. 
+0000e020: 2020 2064 6566 2064 6563 6f64 6528 0a20     def decode(. 
+0000e030: 2020 2020 2020 2073 656c 662c 2065 6e63         self, enc
+0000e040: 6f64 696e 6773 3a20 4f70 7469 6f6e 616c  odings: Optional
+0000e050: 5b53 6571 7565 6e63 655b 7374 725d 5d20  [Sequence[str]] 
+0000e060: 3d20 4e6f 6e65 0a20 2020 2029 202d 3e20  = None.    ) -> 
+0000e070: 2250 6572 736f 6e4e 616d 6522 3a0a 2020  "PersonName":.  
+0000e080: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+0000e090: 7468 6520 7061 7469 656e 7420 6e61 6d65  the patient name
+0000e0a0: 2064 6563 6f64 6564 2062 7920 7468 6520   decoded by the 
+0000e0b0: 6769 7665 6e20 6065 6e63 6f64 696e 6773  given `encodings
+0000e0c0: 602e 0a0a 2020 2020 2020 2020 5061 7261  `...        Para
+0000e0d0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0000e0e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000e0f0: 2020 656e 636f 6469 6e67 7320 3a20 6c69    encodings : li
+0000e100: 7374 206f 6620 7374 722c 206f 7074 696f  st of str, optio
+0000e110: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+0000e120: 5468 6520 6c69 7374 206f 6620 656e 636f  The list of enco
+0000e130: 6469 6e67 7320 7573 6564 2066 6f72 2064  dings used for d
+0000e140: 6563 6f64 696e 6720 7468 6520 6279 7465  ecoding the byte
+0000e150: 2073 7472 696e 672e 2049 6620 6e6f 740a   string. If not.
+0000e160: 2020 2020 2020 2020 2020 2020 6769 7665              give
+0000e170: 6e2c 2074 6865 2069 6e69 7469 616c 2065  n, the initial e
+0000e180: 6e63 6f64 696e 6773 2073 6574 2069 6e20  ncodings set in 
+0000e190: 7468 6520 6f62 6a65 6374 2061 7265 2075  the object are u
+0000e1a0: 7365 642e 0a0a 2020 2020 2020 2020 5265  sed...        Re
+0000e1b0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+0000e1c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
+0000e1d0: 6c75 6572 6570 2e50 6572 736f 6e4e 616d  luerep.PersonNam
+0000e1e0: 650a 2020 2020 2020 2020 2020 2020 4120  e.            A 
+0000e1f0: 7065 7273 6f6e 206e 616d 6520 6f62 6a65  person name obje
+0000e200: 6374 2074 6861 7420 7769 6c6c 2072 6574  ct that will ret
+0000e210: 7572 6e20 7468 6520 6465 636f 6465 6420  urn the decoded 
+0000e220: 7374 7269 6e67 2077 6974 680a 2020 2020  string with.    
+0000e230: 2020 2020 2020 2020 7468 6520 6769 7665          the give
+0000e240: 6e20 656e 636f 6469 6e67 7320 6f6e 2064  n encodings on d
+0000e250: 656d 616e 642e 2049 6620 7468 6520 656e  emand. If the en
+0000e260: 636f 6469 6e67 7320 6172 6520 6e6f 7420  codings are not 
+0000e270: 6769 7665 6e2c 0a20 2020 2020 2020 2020  given,.         
+0000e280: 2020 2074 6865 2063 7572 7265 6e74 206f     the current o
+0000e290: 626a 6563 7420 6973 2072 6574 7572 6e65  bject is returne
+0000e2a0: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
+0000e2b0: 2020 2020 2020 2023 2069 6e20 7468 6520         # in the 
+0000e2c0: 636f 6d6d 6f6e 2063 6173 6520 2865 6e63  common case (enc
+0000e2d0: 6f64 696e 6720 6469 6420 6e6f 7420 6368  oding did not ch
+0000e2e0: 616e 6765 2920 7765 2064 6563 6f64 6520  ange) we decode 
+0000e2f0: 6f6e 2064 656d 616e 640a 2020 2020 2020  on demand.      
+0000e300: 2020 6966 2065 6e63 6f64 696e 6773 2069    if encodings i
+0000e310: 7320 4e6f 6e65 206f 7220 656e 636f 6469  s None or encodi
+0000e320: 6e67 7320 3d3d 2073 656c 662e 656e 636f  ngs == self.enco
+0000e330: 6469 6e67 733a 0a20 2020 2020 2020 2020  dings:.         
+0000e340: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0000e350: 2020 2020 2020 2020 2320 7468 6520 656e          # the en
+0000e360: 636f 6469 6e67 2077 6173 2075 6e6b 6e6f  coding was unkno
+0000e370: 776e 206f 7220 696e 636f 7272 6563 7420  wn or incorrect 
+0000e380: 2d20 6372 6561 7465 2061 206e 6577 0a20  - create a new. 
+0000e390: 2020 2020 2020 2023 2050 6572 736f 6e4e         # PersonN
+0000e3a0: 616d 6520 6f62 6a65 6374 2077 6974 6820  ame object with 
+0000e3b0: 7468 6520 6368 616e 6765 6420 656e 636f  the changed enco
+0000e3c0: 6469 6e67 0a20 2020 2020 2020 2065 6e63  ding.        enc
+0000e3d0: 6f64 696e 6773 203d 205f 7665 7269 6679  odings = _verify
+0000e3e0: 5f65 6e63 6f64 696e 6773 2865 6e63 6f64  _encodings(encod
+0000e3f0: 696e 6773 290a 2020 2020 2020 2020 6966  ings).        if
+0000e400: 2073 656c 662e 6f72 6967 696e 616c 5f73   self.original_s
+0000e410: 7472 696e 6720 6973 204e 6f6e 653a 0a20  tring is None:. 
+0000e420: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+0000e430: 7468 6520 6f72 6967 696e 616c 2065 6e63  the original enc
+0000e440: 6f64 696e 6720 7761 7320 6e6f 7420 7365  oding was not se
+0000e450: 742c 2077 6520 7365 7420 6974 206e 6f77  t, we set it now
+0000e460: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e470: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
+0000e480: 6720 3d20 5f65 6e63 6f64 655f 7065 7273  g = _encode_pers
+0000e490: 6f6e 6e61 6d65 280a 2020 2020 2020 2020  onname(.        
+0000e4a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+0000e4b0: 706f 6e65 6e74 732c 2073 656c 662e 656e  ponents, self.en
+0000e4c0: 636f 6469 6e67 7320 6f72 205b 6465 6661  codings or [defa
+0000e4d0: 756c 745f 656e 636f 6469 6e67 5d0a 2020  ult_encoding].  
+0000e4e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000e4f0: 2020 2020 2020 2020 2320 6e6f 7720 7468          # now th
+0000e500: 6174 2077 6520 6861 7665 2074 6865 2062  at we have the b
+0000e510: 7974 6520 6c65 6e67 7468 2c20 7765 2072  yte length, we r
+0000e520: 652d 7661 6c69 6461 7465 2074 6865 2076  e-validate the v
+0000e530: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
+0000e540: 2076 616c 6964 6174 655f 7661 6c75 6528   validate_value(
+0000e550: 2250 4e22 2c20 7365 6c66 2e6f 7269 6769  "PN", self.origi
+0000e560: 6e61 6c5f 7374 7269 6e67 2c20 7365 6c66  nal_string, self
+0000e570: 2e76 616c 6964 6174 696f 6e5f 6d6f 6465  .validation_mode
+0000e580: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0000e590: 6e20 5065 7273 6f6e 4e61 6d65 2873 656c  n PersonName(sel
+0000e5a0: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
+0000e5b0: 672c 2065 6e63 6f64 696e 6773 290a 0a20  g, encodings).. 
+0000e5c0: 2020 2064 6566 2065 6e63 6f64 6528 7365     def encode(se
+0000e5d0: 6c66 2c20 656e 636f 6469 6e67 733a 204f  lf, encodings: O
+0000e5e0: 7074 696f 6e61 6c5b 5365 7175 656e 6365  ptional[Sequence
+0000e5f0: 5b73 7472 5d5d 203d 204e 6f6e 6529 202d  [str]] = None) -
+0000e600: 3e20 6279 7465 733a 0a20 2020 2020 2020  > bytes:.       
+0000e610: 2022 2222 5265 7475 726e 2074 6865 2070   """Return the p
+0000e620: 6174 6965 6e74 206e 616d 6520 6465 636f  atient name deco
+0000e630: 6465 6420 6279 2074 6865 2067 6976 656e  ded by the given
+0000e640: 2060 656e 636f 6469 6e67 7360 2e0a 0a20   `encodings`... 
+0000e650: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000e660: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000e670: 2d2d 2d2d 0a20 2020 2020 2020 2065 6e63  ----.        enc
+0000e680: 6f64 696e 6773 203a 206c 6973 7420 6f66  odings : list of
+0000e690: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
+0000e6a0: 2020 2020 2020 2020 2020 2054 6865 206c             The l
+0000e6b0: 6973 7420 6f66 2065 6e63 6f64 696e 6773  ist of encodings
+0000e6c0: 2075 7365 6420 666f 7220 656e 636f 6469   used for encodi
+0000e6d0: 6e67 2074 6865 2075 6e69 636f 6465 2073  ng the unicode s
+0000e6e0: 7472 696e 672e 2049 660a 2020 2020 2020  tring. If.      
+0000e6f0: 2020 2020 2020 6e6f 7420 6769 7665 6e2c        not given,
+0000e700: 2074 6865 2069 6e69 7469 616c 2065 6e63   the initial enc
+0000e710: 6f64 696e 6773 2073 6574 2069 6e20 7468  odings set in th
+0000e720: 6520 6f62 6a65 6374 2061 7265 2075 7365  e object are use
+0000e730: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
+0000e740: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000e750: 2d2d 2d0a 2020 2020 2020 2020 6279 7465  ---.        byte
+0000e760: 730a 2020 2020 2020 2020 2020 2020 5468  s.            Th
+0000e770: 6520 7065 7273 6f6e 206e 616d 6520 656e  e person name en
+0000e780: 636f 6465 6420 7769 7468 2074 6865 2067  coded with the g
+0000e790: 6976 656e 2065 6e63 6f64 696e 6773 2061  iven encodings a
+0000e7a0: 7320 6120 6279 7465 2073 7472 696e 672e  s a byte string.
+0000e7b0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+0000e7c0: 6e6f 2065 6e63 6f64 696e 6720 6973 2067  no encoding is g
+0000e7d0: 6976 656e 2c20 7468 6520 6f72 6967 696e  iven, the origin
+0000e7e0: 616c 2062 7974 6520 7374 7269 6e67 2069  al byte string i
+0000e7f0: 7320 7265 7475 726e 6564 2c20 6966 0a20  s returned, if. 
+0000e800: 2020 2020 2020 2020 2020 2061 7661 696c             avail
+0000e810: 6162 6c65 2c20 6f74 6865 7277 6973 6520  able, otherwise 
+0000e820: 6561 6368 2067 726f 7570 206f 6620 7468  each group of th
+0000e830: 6520 7061 7469 656e 7420 6e61 6d65 2069  e patient name i
+0000e840: 7320 656e 636f 6465 640a 2020 2020 2020  s encoded.      
+0000e850: 2020 2020 2020 7769 7468 2074 6865 2066        with the f
+0000e860: 6972 7374 206d 6174 6368 696e 6720 6f66  irst matching of
+0000e870: 2074 6865 2067 6976 656e 2065 6e63 6f64   the given encod
+0000e880: 696e 6773 2e0a 2020 2020 2020 2020 2222  ings..        ""
+0000e890: 220a 2020 2020 2020 2020 656e 636f 6469  ".        encodi
+0000e8a0: 6e67 7320 3d20 5f76 6572 6966 795f 656e  ngs = _verify_en
+0000e8b0: 636f 6469 6e67 7328 656e 636f 6469 6e67  codings(encoding
+0000e8c0: 7329 206f 7220 7365 6c66 2e65 6e63 6f64  s) or self.encod
+0000e8d0: 696e 6773 0a0a 2020 2020 2020 2020 2320  ings..        # 
+0000e8e0: 6966 2074 6865 2065 6e63 6f64 696e 6720  if the encoding 
+0000e8f0: 6973 206e 6f74 2074 6865 206f 7269 6769  is not the origi
+0000e900: 6e61 6c20 656e 636f 6469 6e67 2c20 7765  nal encoding, we
+0000e910: 2068 6176 6520 746f 2072 6574 7572 6e0a   have to return.
+0000e920: 2020 2020 2020 2020 2320 6120 7265 2d65          # a re-e
+0000e930: 6e63 6f64 6564 2073 7472 696e 6720 2877  ncoded string (w
+0000e940: 6974 686f 7574 2075 7064 6174 696e 6720  ithout updating 
+0000e950: 7468 6520 6f72 6967 696e 616c 2073 7472  the original str
+0000e960: 696e 6729 0a20 2020 2020 2020 2069 6620  ing).        if 
+0000e970: 656e 636f 6469 6e67 7320 213d 2073 656c  encodings != sel
+0000e980: 662e 656e 636f 6469 6e67 7320 616e 6420  f.encodings and 
+0000e990: 7365 6c66 2e65 6e63 6f64 696e 6773 2069  self.encodings i
+0000e9a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000e9b0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000e9c0: 656e 636f 6465 5f70 6572 736f 6e6e 616d  encode_personnam
+0000e9d0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+0000e9e0: 2020 2073 656c 662e 636f 6d70 6f6e 656e     self.componen
+0000e9f0: 7473 2c20 6361 7374 2853 6571 7565 6e63  ts, cast(Sequenc
+0000ea00: 655b 7374 725d 2c20 656e 636f 6469 6e67  e[str], encoding
+0000ea10: 7329 0a20 2020 2020 2020 2020 2020 2029  s).            )
+0000ea20: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000ea30: 662e 6f72 6967 696e 616c 5f73 7472 696e  f.original_strin
+0000ea40: 6720 6973 204e 6f6e 653a 0a20 2020 2020  g is None:.     
+0000ea50: 2020 2020 2020 2023 2069 6620 7468 6520         # if the 
+0000ea60: 6f72 6967 696e 616c 2065 6e63 6f64 696e  original encodin
+0000ea70: 6720 7761 7320 6e6f 7420 7365 742c 2077  g was not set, w
+0000ea80: 6520 7365 7420 6974 206e 6f77 0a20 2020  e set it now.   
+0000ea90: 2020 2020 2020 2020 2073 656c 662e 6f72           self.or
+0000eaa0: 6967 696e 616c 5f73 7472 696e 6720 3d20  iginal_string = 
+0000eab0: 5f65 6e63 6f64 655f 7065 7273 6f6e 6e61  _encode_personna
+0000eac0: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+0000ead0: 2020 2020 7365 6c66 2e63 6f6d 706f 6e65      self.compone
+0000eae0: 6e74 732c 2065 6e63 6f64 696e 6773 206f  nts, encodings o
+0000eaf0: 7220 5b64 6566 6175 6c74 5f65 6e63 6f64  r [default_encod
+0000eb00: 696e 675d 0a20 2020 2020 2020 2020 2020  ing].           
+0000eb10: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+0000eb20: 726e 2073 656c 662e 6f72 6967 696e 616c  rn self.original
+0000eb30: 5f73 7472 696e 670a 0a20 2020 2064 6566  _string..    def
+0000eb40: 2066 616d 696c 795f 636f 6d6d 615f 6769   family_comma_gi
+0000eb50: 7665 6e28 7365 6c66 2920 2d3e 2073 7472  ven(self) -> str
+0000eb60: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+0000eb70: 7572 6e20 7468 6520 6e61 6d65 2061 7320  urn the name as 
+0000eb80: 2246 616d 696c 792c 2047 6976 656e 222e  "Family, Given".
+0000eb90: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000eba0: 726e 2066 227b 7365 6c66 2e66 616d 696c  rn f"{self.famil
+0000ebb0: 795f 6e61 6d65 7d2c 207b 7365 6c66 2e67  y_name}, {self.g
+0000ebc0: 6976 656e 5f6e 616d 657d 220a 0a20 2020  iven_name}"..   
+0000ebd0: 2064 6566 2066 6f72 6d61 7474 6564 2873   def formatted(s
+0000ebe0: 656c 662c 2066 6f72 6d61 745f 7374 723a  elf, format_str:
+0000ebf0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
+0000ec00: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+0000ec10: 7468 6520 6e61 6d65 2061 7320 6120 3a63  the name as a :c
+0000ec20: 6c61 7373 3a60 7374 7260 2066 6f72 6d61  lass:`str` forma
+0000ec30: 7474 6564 2075 7369 6e67 2060 666f 726d  tted using `form
+0000ec40: 6174 5f73 7472 602e 2222 220a 2020 2020  at_str`.""".    
+0000ec50: 2020 2020 7265 7475 726e 2066 6f72 6d61      return forma
+0000ec60: 745f 7374 7220 2520 7365 6c66 2e5f 6372  t_str % self._cr
+0000ec70: 6561 7465 5f64 6963 7428 290a 0a20 2020  eate_dict()..   
+0000ec80: 2064 6566 205f 5f62 6f6f 6c5f 5f28 7365   def __bool__(se
+0000ec90: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+0000eca0: 2020 2020 2022 2222 5265 7475 726e 2060       """Return `
+0000ecb0: 6054 7275 6560 6020 6966 2074 6865 206e  `True`` if the n
+0000ecc0: 616d 6520 6973 206e 6f74 2065 6d70 7479  ame is not empty
+0000ecd0: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+0000ece0: 6e6f 7420 7365 6c66 2e6f 7269 6769 6e61  not self.origina
+0000ecf0: 6c5f 7374 7269 6e67 3a0a 2020 2020 2020  l_string:.      
+0000ed00: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
+0000ed10: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000ed20: 6f6f 6c28 7365 6c66 2e63 6f6d 706f 6e65  ool(self.compone
+0000ed30: 6e74 7329 0a20 2020 2020 2020 2020 2020  nts).           
+0000ed40: 2020 2020 2061 6e64 2028 6c65 6e28 7365       and (len(se
+0000ed50: 6c66 2e63 6f6d 706f 6e65 6e74 7329 203e  lf.components) >
+0000ed60: 2031 206f 7220 626f 6f6c 2873 656c 662e   1 or bool(self.
+0000ed70: 636f 6d70 6f6e 656e 7473 5b30 5d29 290a  components[0])).
+0000ed80: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000ed90: 2020 2020 2020 2072 6574 7572 6e20 626f         return bo
+0000eda0: 6f6c 2873 656c 662e 6f72 6967 696e 616c  ol(self.original
+0000edb0: 5f73 7472 696e 6729 0a0a 2020 2020 4073  _string)..    @s
+0000edc0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+0000edd0: 6465 6620 5f65 6e63 6f64 655f 636f 6d70  def _encode_comp
+0000ede0: 6f6e 656e 745f 6772 6f75 7073 280a 2020  onent_groups(.  
+0000edf0: 2020 2020 2020 616c 7068 6162 6574 6963        alphabetic
+0000ee00: 5f67 726f 7570 3a20 5365 7175 656e 6365  _group: Sequence
+0000ee10: 5b55 6e69 6f6e 5b73 7472 2c20 6279 7465  [Union[str, byte
+0000ee20: 735d 5d2c 0a20 2020 2020 2020 2069 6465  s]],.        ide
+0000ee30: 6f67 7261 7068 6963 5f67 726f 7570 3a20  ographic_group: 
+0000ee40: 5365 7175 656e 6365 5b55 6e69 6f6e 5b73  Sequence[Union[s
+0000ee50: 7472 2c20 6279 7465 735d 5d2c 0a20 2020  tr, bytes]],.   
+0000ee60: 2020 2020 2070 686f 6e65 7469 635f 6772       phonetic_gr
+0000ee70: 6f75 703a 2053 6571 7565 6e63 655b 556e  oup: Sequence[Un
+0000ee80: 696f 6e5b 7374 722c 2062 7974 6573 5d5d  ion[str, bytes]]
+0000ee90: 2c0a 2020 2020 2020 2020 656e 636f 6469  ,.        encodi
+0000eea0: 6e67 733a 204f 7074 696f 6e61 6c5b 4c69  ngs: Optional[Li
+0000eeb0: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
+0000eec0: 0a20 2020 2029 202d 3e20 6279 7465 733a  .    ) -> bytes:
+0000eed0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+0000eee0: 7465 7320 6120 6279 7465 2073 7472 696e  tes a byte strin
+0000eef0: 6720 666f 7220 6120 7065 7273 6f6e 206e  g for a person n
+0000ef00: 616d 6520 6672 6f6d 206c 6973 7473 206f  ame from lists o
+0000ef10: 6620 7061 7274 732e 0a0a 2020 2020 2020  f parts...      
+0000ef20: 2020 4561 6368 206f 6620 7468 6520 7468    Each of the th
+0000ef30: 7265 6520 636f 6d70 6f6e 656e 7420 6772  ree component gr
+0000ef40: 6f75 7073 2028 616c 7068 6162 6574 6963  oups (alphabetic
+0000ef50: 2c20 6964 656f 6772 6170 6869 632c 2070  , ideographic, p
+0000ef60: 686f 6e65 7469 6329 0a20 2020 2020 2020  honetic).       
+0000ef70: 2061 7265 2073 7570 706c 6965 6420 6173   are supplied as
+0000ef80: 2061 206c 6973 7420 6f66 2063 6f6d 706f   a list of compo
+0000ef90: 6e65 6e74 732e 0a0a 2020 2020 2020 2020  nents...        
+0000efa0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0000efb0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000efc0: 2020 2020 2020 616c 7068 6162 6574 6963        alphabetic
+0000efd0: 5f67 726f 7570 3a20 5365 7175 656e 6365  _group: Sequence
+0000efe0: 5b55 6e69 6f6e 5b73 7472 2c20 6279 7465  [Union[str, byte
+0000eff0: 735d 5d0a 2020 2020 2020 2020 2020 2020  s]].            
+0000f000: 4c69 7374 206f 6620 636f 6d70 6f6e 656e  List of componen
+0000f010: 7473 2066 6f72 2074 6865 2061 6c70 6861  ts for the alpha
+0000f020: 6265 7469 6320 6772 6f75 702e 0a20 2020  betic group..   
+0000f030: 2020 2020 2069 6465 6f67 7261 7068 6963       ideographic
+0000f040: 5f67 726f 7570 3a20 5365 7175 656e 6365  _group: Sequence
+0000f050: 5b55 6e69 6f6e 5b73 7472 2c20 6279 7465  [Union[str, byte
+0000f060: 735d 5d0a 2020 2020 2020 2020 2020 2020  s]].            
+0000f070: 4c69 7374 206f 6620 636f 6d70 6f6e 656e  List of componen
+0000f080: 7473 2066 6f72 2074 6865 2069 6465 6f67  ts for the ideog
+0000f090: 7261 7068 6963 2067 726f 7570 2e0a 2020  raphic group..  
+0000f0a0: 2020 2020 2020 7068 6f6e 6574 6963 5f67        phonetic_g
+0000f0b0: 726f 7570 3a20 5365 7175 656e 6365 5b55  roup: Sequence[U
+0000f0c0: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+0000f0d0: 5d0a 2020 2020 2020 2020 2020 2020 4c69  ].            Li
+0000f0e0: 7374 206f 6620 636f 6d70 6f6e 656e 7473  st of components
+0000f0f0: 2066 6f72 2074 6865 2070 686f 6e65 7469   for the phoneti
+0000f100: 6320 6772 6f75 702e 0a20 2020 2020 2020  c group..       
+0000f110: 2065 6e63 6f64 696e 6773 3a20 4f70 7469   encodings: Opti
+0000f120: 6f6e 616c 5b4c 6973 745b 7374 725d 5d0a  onal[List[str]].
+0000f130: 2020 2020 2020 2020 2020 2020 4120 6c69              A li
+0000f140: 7374 206f 6620 656e 636f 6469 6e67 7320  st of encodings 
+0000f150: 7573 6564 2066 6f72 2074 6865 206f 7468  used for the oth
+0000f160: 6572 2069 6e70 7574 2070 6172 616d 6574  er input paramet
+0000f170: 6572 732e 0a0a 2020 2020 2020 2020 5265  ers...        Re
+0000f180: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+0000f190: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6279  -----.        by
+0000f1a0: 7465 733a 0a20 2020 2020 2020 2020 2020  tes:.           
+0000f1b0: 2042 7974 6573 2073 7472 696e 6720 7265   Bytes string re
+0000f1c0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+0000f1d0: 7468 6520 7065 7273 6f6e 206e 616d 652e  the person name.
+0000f1e0: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+0000f1f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d0a  .        ------.
+0000f200: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+0000f210: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0000f220: 4966 2061 6e79 206f 6620 7468 6520 696e  If any of the in
+0000f230: 7075 7420 7374 7269 6e67 7320 636f 6e74  put strings cont
+0000f240: 6169 6e20 6469 7361 6c6c 6f77 6564 2063  ain disallowed c
+0000f250: 6861 7261 6374 6572 733a 0a20 2020 2020  haracters:.     
+0000f260: 2020 2020 2020 2027 5c5c 2720 2873 696e         '\\' (sin
+0000f270: 676c 6520 6261 636b 736c 6173 6829 2c20  gle backslash), 
+0000f280: 275e 272c 2027 3d27 2e0a 2020 2020 2020  '^', '='..      
+0000f290: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
+0000f2a0: 6f6d 2070 7964 6963 6f6d 2e63 6861 7273  om pydicom.chars
+0000f2b0: 6574 2069 6d70 6f72 7420 656e 636f 6465  et import encode
+0000f2c0: 5f73 7472 696e 672c 2064 6563 6f64 655f  _string, decode_
+0000f2d0: 6279 7465 730a 0a20 2020 2020 2020 2064  bytes..        d
+0000f2e0: 6566 2065 6e63 2873 3a20 7374 7229 202d  ef enc(s: str) -
+0000f2f0: 3e20 6279 7465 733a 0a20 2020 2020 2020  > bytes:.       
+0000f300: 2020 2020 2072 6574 7572 6e20 656e 636f       return enco
+0000f310: 6465 5f73 7472 696e 6728 732c 2065 6e63  de_string(s, enc
+0000f320: 6f64 696e 6773 206f 7220 5b64 6566 6175  odings or [defau
+0000f330: 6c74 5f65 6e63 6f64 696e 675d 290a 0a20  lt_encoding]).. 
+0000f340: 2020 2020 2020 2064 6566 2064 6563 2873         def dec(s
+0000f350: 3a20 6279 7465 7329 202d 3e20 7374 723a  : bytes) -> str:
+0000f360: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000f370: 7572 6e20 6465 636f 6465 5f62 7974 6573  urn decode_bytes
+0000f380: 2873 2c20 656e 636f 6469 6e67 7320 6f72  (s, encodings or
+0000f390: 205b 6465 6661 756c 745f 656e 636f 6469   [default_encodi
+0000f3a0: 6e67 5d2c 2073 6574 2829 290a 0a20 2020  ng], set())..   
+0000f3b0: 2020 2020 2065 6e63 6f64 6564 5f63 6f6d       encoded_com
+0000f3c0: 706f 6e65 6e74 5f73 6570 203d 2065 6e63  ponent_sep = enc
+0000f3d0: 2827 5e27 290a 2020 2020 2020 2020 656e  ('^').        en
+0000f3e0: 636f 6465 645f 6772 6f75 705f 7365 7020  coded_group_sep 
+0000f3f0: 3d20 656e 6328 273d 2729 0a0a 2020 2020  = enc('=')..    
+0000f400: 2020 2020 6469 7361 6c6c 6f77 6564 5f63      disallowed_c
+0000f410: 6861 7273 203d 205b 275c 5c27 2c20 273d  hars = ['\\', '=
+0000f420: 272c 2027 5e27 5d0a 0a20 2020 2020 2020  ', '^']..       
+0000f430: 2064 6566 2073 7461 6e64 6172 6469 7a65   def standardize
+0000f440: 5f65 6e63 6f64 696e 6728 7661 6c3a 2055  _encoding(val: U
+0000f450: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+0000f460: 2920 2d3e 2062 7974 6573 3a0a 2020 2020  ) -> bytes:.    
+0000f470: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+0000f480: 2061 2062 7974 6520 656e 636f 6465 6420   a byte encoded 
+0000f490: 7374 7269 6e67 2072 6567 6172 646c 6573  string regardles
+0000f4a0: 7320 6f66 2074 6865 2069 6e70 7574 2074  s of the input t
+0000f4b0: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
+0000f4c0: 2320 5468 6973 2061 6c6c 6f77 7320 7468  # This allows th
+0000f4d0: 6520 7573 6572 2074 6f20 7375 7070 6c79  e user to supply
+0000f4e0: 2061 206d 6978 7475 7265 206f 6620 7374   a mixture of st
+0000f4f0: 7220 616e 6420 6279 7465 730a 2020 2020  r and bytes.    
+0000f500: 2020 2020 2020 2020 2320 666f 7220 6469          # for di
+0000f510: 6666 6572 656e 7420 7061 7274 7320 6f66  fferent parts of
+0000f520: 2074 6865 2069 6e70 7574 0a20 2020 2020   the input.     
+0000f530: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000f540: 616e 6365 2876 616c 2c20 6279 7465 7329  ance(val, bytes)
+0000f550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f560: 2020 7661 6c5f 656e 6320 3d20 7661 6c0a    val_enc = val.
+0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f580: 7661 6c5f 6465 6320 3d20 6465 6328 7661  val_dec = dec(va
+0000f590: 6c29 0a20 2020 2020 2020 2020 2020 2065  l).            e
+0000f5a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000f5b0: 2020 2020 2076 616c 5f65 6e63 203d 2065       val_enc = e
+0000f5c0: 6e63 2876 616c 290a 2020 2020 2020 2020  nc(val).        
+0000f5d0: 2020 2020 2020 2020 7661 6c5f 6465 6320          val_dec 
+0000f5e0: 3d20 7661 6c0a 0a20 2020 2020 2020 2020  = val..         
+0000f5f0: 2020 2023 2043 6865 636b 2066 6f72 2064     # Check for d
+0000f600: 6973 616c 6c6f 7765 6420 6368 6172 7320  isallowed chars 
+0000f610: 696e 2074 6865 2064 6563 6f64 6564 2073  in the decoded s
+0000f620: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0000f630: 2020 666f 7220 6320 696e 2064 6973 616c    for c in disal
+0000f640: 6c6f 7765 645f 6368 6172 733a 0a20 2020  lowed_chars:.   
+0000f650: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000f660: 6320 696e 2076 616c 5f64 6563 3a0a 2020  c in val_dec:.  
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000f690: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000f6a0: 2020 2020 2020 2020 2020 2020 6627 5374              f'St
+0000f6b0: 7269 6e67 7320 6d61 7920 6e6f 7420 636f  rings may not co
+0000f6c0: 6e74 6169 6e20 7468 6520 7b63 7d20 6368  ntain the {c} ch
+0000f6d0: 6172 6163 7465 7227 0a20 2020 2020 2020  aracter'.       
+0000f6e0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+0000f6f0: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
+0000f700: 7475 726e 2074 6865 2065 6e63 6f64 6564  turn the encoded
+0000f710: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0000f720: 2020 2020 7265 7475 726e 2076 616c 5f65      return val_e
+0000f730: 6e63 0a0a 2020 2020 2020 2020 6465 6620  nc..        def 
+0000f740: 6d61 6b65 5f63 6f6d 706f 6e65 6e74 5f67  make_component_g
+0000f750: 726f 7570 280a 2020 2020 2020 2020 2020  roup(.          
+0000f760: 2020 636f 6d70 6f6e 656e 7473 3a20 5365    components: Se
+0000f770: 7175 656e 6365 5b55 6e69 6f6e 5b73 7472  quence[Union[str
+0000f780: 2c20 6279 7465 735d 5d0a 2020 2020 2020  , bytes]].      
+0000f790: 2020 2920 2d3e 2062 7974 6573 3a0a 2020    ) -> bytes:.  
+0000f7a0: 2020 2020 2020 2020 2020 656e 636f 6465            encode
+0000f7b0: 645f 636f 6d70 6f6e 656e 7473 203d 205b  d_components = [
+0000f7c0: 7374 616e 6461 7264 697a 655f 656e 636f  standardize_enco
+0000f7d0: 6469 6e67 2863 2920 666f 7220 6320 696e  ding(c) for c in
+0000f7e0: 2063 6f6d 706f 6e65 6e74 735d 0a20 2020   components].   
+0000f7f0: 2020 2020 2020 2020 206a 6f69 6e65 645f           joined_
+0000f800: 636f 6d70 6f6e 656e 7473 203d 2065 6e63  components = enc
+0000f810: 6f64 6564 5f63 6f6d 706f 6e65 6e74 5f73  oded_component_s
+0000f820: 6570 2e6a 6f69 6e28 656e 636f 6465 645f  ep.join(encoded_
+0000f830: 636f 6d70 6f6e 656e 7473 290a 2020 2020  components).    
+0000f840: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+0000f850: 6f69 6e65 645f 636f 6d70 6f6e 656e 7473  oined_components
+0000f860: 2e72 7374 7269 7028 656e 636f 6465 645f  .rstrip(encoded_
+0000f870: 636f 6d70 6f6e 656e 745f 7365 7029 0a0a  component_sep)..
+0000f880: 2020 2020 2020 2020 636f 6d70 6f6e 656e          componen
+0000f890: 745f 6772 6f75 7073 3a20 4c69 7374 5b62  t_groups: List[b
+0000f8a0: 7974 6573 5d20 3d20 5b0a 2020 2020 2020  ytes] = [.      
+0000f8b0: 2020 2020 2020 6d61 6b65 5f63 6f6d 706f        make_compo
+0000f8c0: 6e65 6e74 5f67 726f 7570 2861 6c70 6861  nent_group(alpha
+0000f8d0: 6265 7469 635f 6772 6f75 7029 2c0a 2020  betic_group),.  
+0000f8e0: 2020 2020 2020 2020 2020 6d61 6b65 5f63            make_c
+0000f8f0: 6f6d 706f 6e65 6e74 5f67 726f 7570 2869  omponent_group(i
+0000f900: 6465 6f67 7261 7068 6963 5f67 726f 7570  deographic_group
+0000f910: 292c 0a20 2020 2020 2020 2020 2020 206d  ),.            m
+0000f920: 616b 655f 636f 6d70 6f6e 656e 745f 6772  ake_component_gr
+0000f930: 6f75 7028 7068 6f6e 6574 6963 5f67 726f  oup(phonetic_gro
+0000f940: 7570 290a 2020 2020 2020 2020 5d0a 2020  up).        ].  
+0000f950: 2020 2020 2020 6a6f 696e 6564 5f67 726f        joined_gro
+0000f960: 7570 733a 2062 7974 6573 203d 2065 6e63  ups: bytes = enc
+0000f970: 6f64 6564 5f67 726f 7570 5f73 6570 2e6a  oded_group_sep.j
+0000f980: 6f69 6e28 636f 6d70 6f6e 656e 745f 6772  oin(component_gr
+0000f990: 6f75 7073 290a 2020 2020 2020 2020 6a6f  oups).        jo
+0000f9a0: 696e 6564 5f67 726f 7570 7320 3d20 6a6f  ined_groups = jo
+0000f9b0: 696e 6564 5f67 726f 7570 732e 7273 7472  ined_groups.rstr
+0000f9c0: 6970 2865 6e63 6f64 6564 5f67 726f 7570  ip(encoded_group
+0000f9d0: 5f73 6570 290a 2020 2020 2020 2020 7265  _sep).        re
+0000f9e0: 7475 726e 206a 6f69 6e65 645f 6772 6f75  turn joined_grou
+0000f9f0: 7073 0a0a 2020 2020 4063 6c61 7373 6d65  ps..    @classme
+0000fa00: 7468 6f64 0a20 2020 2064 6566 2066 726f  thod.    def fro
+0000fa10: 6d5f 6e61 6d65 645f 636f 6d70 6f6e 656e  m_named_componen
+0000fa20: 7473 280a 2020 2020 2020 2020 636c 732c  ts(.        cls,
+0000fa30: 0a20 2020 2020 2020 2066 616d 696c 795f  .        family_
+0000fa40: 6e61 6d65 3a20 556e 696f 6e5b 7374 722c  name: Union[str,
+0000fa50: 2062 7974 6573 5d20 3d20 2727 2c0a 2020   bytes] = '',.  
+0000fa60: 2020 2020 2020 6769 7665 6e5f 6e61 6d65        given_name
+0000fa70: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
+0000fa80: 6573 5d20 3d20 2727 2c0a 2020 2020 2020  es] = '',.      
+0000fa90: 2020 6d69 6464 6c65 5f6e 616d 653a 2055    middle_name: U
+0000faa0: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+0000fab0: 203d 2027 272c 0a20 2020 2020 2020 206e   = '',.        n
+0000fac0: 616d 655f 7072 6566 6978 3a20 556e 696f  ame_prefix: Unio
+0000fad0: 6e5b 7374 722c 2062 7974 6573 5d20 3d20  n[str, bytes] = 
+0000fae0: 2727 2c0a 2020 2020 2020 2020 6e61 6d65  '',.        name
+0000faf0: 5f73 7566 6669 783a 2055 6e69 6f6e 5b73  _suffix: Union[s
+0000fb00: 7472 2c20 6279 7465 735d 203d 2027 272c  tr, bytes] = '',
+0000fb10: 0a20 2020 2020 2020 2066 616d 696c 795f  .        family_
+0000fb20: 6e61 6d65 5f69 6465 6f67 7261 7068 6963  name_ideographic
+0000fb30: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
+0000fb40: 6573 5d20 3d20 2727 2c0a 2020 2020 2020  es] = '',.      
+0000fb50: 2020 6769 7665 6e5f 6e61 6d65 5f69 6465    given_name_ide
+0000fb60: 6f67 7261 7068 6963 3a20 556e 696f 6e5b  ographic: Union[
+0000fb70: 7374 722c 2062 7974 6573 5d20 3d20 2727  str, bytes] = ''
+0000fb80: 2c0a 2020 2020 2020 2020 6d69 6464 6c65  ,.        middle
+0000fb90: 5f6e 616d 655f 6964 656f 6772 6170 6869  _name_ideographi
+0000fba0: 633a 2055 6e69 6f6e 5b73 7472 2c20 6279  c: Union[str, by
+0000fbb0: 7465 735d 203d 2027 272c 0a20 2020 2020  tes] = '',.     
+0000fbc0: 2020 206e 616d 655f 7072 6566 6978 5f69     name_prefix_i
+0000fbd0: 6465 6f67 7261 7068 6963 3a20 556e 696f  deographic: Unio
+0000fbe0: 6e5b 7374 722c 2062 7974 6573 5d20 3d20  n[str, bytes] = 
+0000fbf0: 2727 2c0a 2020 2020 2020 2020 6e61 6d65  '',.        name
+0000fc00: 5f73 7566 6669 785f 6964 656f 6772 6170  _suffix_ideograp
+0000fc10: 6869 633a 2055 6e69 6f6e 5b73 7472 2c20  hic: Union[str, 
+0000fc20: 6279 7465 735d 203d 2027 272c 0a20 2020  bytes] = '',.   
+0000fc30: 2020 2020 2066 616d 696c 795f 6e61 6d65       family_name
+0000fc40: 5f70 686f 6e65 7469 633a 2055 6e69 6f6e  _phonetic: Union
+0000fc50: 5b73 7472 2c20 6279 7465 735d 203d 2027  [str, bytes] = '
+0000fc60: 272c 0a20 2020 2020 2020 2067 6976 656e  ',.        given
+0000fc70: 5f6e 616d 655f 7068 6f6e 6574 6963 3a20  _name_phonetic: 
+0000fc80: 556e 696f 6e5b 7374 722c 2062 7974 6573  Union[str, bytes
+0000fc90: 5d20 3d20 2727 2c0a 2020 2020 2020 2020  ] = '',.        
+0000fca0: 6d69 6464 6c65 5f6e 616d 655f 7068 6f6e  middle_name_phon
+0000fcb0: 6574 6963 3a20 556e 696f 6e5b 7374 722c  etic: Union[str,
+0000fcc0: 2062 7974 6573 5d20 3d20 2727 2c0a 2020   bytes] = '',.  
+0000fcd0: 2020 2020 2020 6e61 6d65 5f70 7265 6669        name_prefi
+0000fce0: 785f 7068 6f6e 6574 6963 3a20 556e 696f  x_phonetic: Unio
+0000fcf0: 6e5b 7374 722c 2062 7974 6573 5d20 3d20  n[str, bytes] = 
+0000fd00: 2727 2c0a 2020 2020 2020 2020 6e61 6d65  '',.        name
+0000fd10: 5f73 7566 6669 785f 7068 6f6e 6574 6963  _suffix_phonetic
+0000fd20: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
+0000fd30: 6573 5d20 3d20 2727 2c0a 2020 2020 2020  es] = '',.      
+0000fd40: 2020 656e 636f 6469 6e67 733a 204f 7074    encodings: Opt
+0000fd50: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+0000fd60: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
+0000fd70: 3e20 2750 6572 736f 6e4e 616d 6527 3a0a  > 'PersonName':.
+0000fd80: 2020 2020 2020 2020 2222 2243 6f6e 7374          """Const
+0000fd90: 7275 6374 2061 2050 6572 736f 6e4e 616d  ruct a PersonNam
+0000fda0: 6520 6672 6f6d 2065 7870 6c69 6369 7420  e from explicit 
+0000fdb0: 6e61 6d65 6420 636f 6d70 6f6e 656e 7473  named components
+0000fdc0: 2e0a 0a20 2020 2020 2020 2054 6865 2044  ...        The D
+0000fdd0: 4943 4f4d 2073 7461 6e64 6172 6420 6465  ICOM standard de
+0000fde0: 7363 7269 6265 7320 6875 6d61 6e20 6e61  scribes human na
+0000fdf0: 6d65 7320 7573 696e 6720 6669 7665 2063  mes using five c
+0000fe00: 6f6d 706f 6e65 6e74 733a 0a20 2020 2020  omponents:.     
+0000fe10: 2020 2066 616d 696c 7920 6e61 6d65 2c20     family name, 
+0000fe20: 6769 7665 6e20 6e61 6d65 2c20 6d69 6464  given name, midd
+0000fe30: 6c65 206e 616d 652c 206e 616d 6520 7072  le name, name pr
+0000fe40: 6566 6978 2c20 616e 6420 6e61 6d65 2073  efix, and name s
+0000fe50: 7566 6669 782e 0a20 2020 2020 2020 2041  uffix..        A
+0000fe60: 6e79 2063 6f6d 706f 6e65 6e74 206d 6179  ny component may
+0000fe70: 2062 6520 616e 2065 6d70 7479 2073 7472   be an empty str
+0000fe80: 696e 6720 2874 6865 2064 6566 6175 6c74  ing (the default
+0000fe90: 2920 6966 206e 6f74 2075 7365 642e 0a20  ) if not used.. 
+0000fea0: 2020 2020 2020 2041 2063 6f6d 706f 6e65         A compone
+0000feb0: 6e74 206d 6179 2063 6f6e 7461 696e 206d  nt may contain m
+0000fec0: 756c 7469 706c 6520 7370 6163 652d 7365  ultiple space-se
+0000fed0: 7061 7261 7465 6420 776f 7264 7320 6966  parated words if
+0000fee0: 2074 6865 7265 0a20 2020 2020 2020 2061   there.        a
+0000fef0: 7265 2c20 666f 7220 6578 616d 706c 652c  re, for example,
+0000ff00: 206d 756c 7469 706c 6520 6769 7665 6e20   multiple given 
+0000ff10: 6e61 6d65 732c 206d 6964 646c 6520 6e61  names, middle na
+0000ff20: 6d65 732c 206f 7220 7469 746c 6573 2e0a  mes, or titles..
+0000ff30: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
+0000ff40: 6e61 6c6c 792c 2065 6163 6820 636f 6d70  nally, each comp
+0000ff50: 6f6e 656e 7420 6d61 7920 6265 2072 6570  onent may be rep
+0000ff60: 7265 7365 6e74 6564 2069 6e20 6964 656f  resented in ideo
+0000ff70: 6772 6170 6869 6320 6f72 0a20 2020 2020  graphic or.     
+0000ff80: 2020 2070 686f 6e65 7469 6320 666f 726d     phonetic form
+0000ff90: 2069 6e20 6164 6469 7469 6f6e 2074 6f20   in addition to 
+0000ffa0: 286f 7220 696e 7374 6561 6420 6f66 2920  (or instead of) 
+0000ffb0: 616c 7068 6162 6574 6963 2066 6f72 6d2e  alphabetic form.
+0000ffc0: 0a0a 2020 2020 2020 2020 466f 7220 6d6f  ..        For mo
+0000ffd0: 7265 2069 6e66 6f72 6d61 7469 6f6e 2073  re information s
+0000ffe0: 6565 2074 6865 2066 6f6c 6c6f 7769 6e67  ee the following
+0000fff0: 2070 6172 7473 206f 6620 7468 6520 4449   parts of the DI
+00010000: 434f 4d20 7374 616e 6461 7264 3a0a 2020  COM standard:.  
+00010010: 2020 2020 2020 2d20 3a64 636d 3a60 5661        - :dcm:`Va
+00010020: 6c75 6520 5265 7072 6573 656e 7461 7469  lue Representati
+00010030: 6f6e 7320 3c70 6172 7430 352f 7365 6374  ons <part05/sect
+00010040: 5f36 2e32 2e68 746d 6c3e 600a 2020 2020  _6.2.html>`.    
+00010050: 2020 2020 2d20 3a64 636d 3a60 504e 2045      - :dcm:`PN E
+00010060: 7861 6d70 6c65 7320 3c70 6172 7430 352f  xamples <part05/
+00010070: 7365 6374 5f36 2e32 2e68 746d 6c23 7365  sect_6.2.html#se
+00010080: 6374 5f36 2e32 2e31 2e31 3e60 0a20 2020  ct_6.2.1.1>`.   
+00010090: 2020 2020 202d 203a 6463 6d3a 6050 4e20       - :dcm:`PN 
+000100a0: 5072 6563 6973 6520 7365 6d61 6e74 6963  Precise semantic
+000100b0: 7320 3c70 6172 7430 352f 7365 6374 5f36  s <part05/sect_6
+000100c0: 2e32 2e68 746d 6c23 7365 6374 5f36 2e32  .2.html#sect_6.2
+000100d0: 2e31 2e32 3e60 0a0a 2020 2020 2020 2020  .1.2>`..        
+000100e0: 4578 616d 706c 650a 2020 2020 2020 2020  Example.        
+000100f0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00010100: 4120 6361 7365 2077 6974 6820 6d75 6c74  A case with mult
+00010110: 6970 6c65 2067 6976 656e 206e 616d 6573  iple given names
+00010120: 2061 6e64 2073 7566 6669 7865 7320 2844   and suffixes (D
+00010130: 4943 4f4d 2073 7461 6e64 6172 642c 0a20  ICOM standard,. 
+00010140: 2020 2020 2020 2070 6172 7420 352c 2073         part 5, s
+00010150: 6563 7420 362e 322e 312e 3129 3a0a 0a20  ect 6.2.1.1):.. 
+00010160: 2020 2020 2020 203e 3e3e 2070 6e20 3d20         >>> pn = 
+00010170: 5065 7273 6f6e 4e61 6d65 2e66 726f 6d5f  PersonName.from_
+00010180: 6e61 6d65 645f 636f 6d70 6f6e 656e 7473  named_components
+00010190: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000101a0: 2020 6661 6d69 6c79 5f6e 616d 653d 2741    family_name='A
+000101b0: 6461 6d73 272c 0a20 2020 2020 2020 2020  dams',.         
+000101c0: 2020 2020 2020 2067 6976 656e 5f6e 616d         given_nam
+000101d0: 653d 274a 6f68 6e20 526f 6265 7274 2051  e='John Robert Q
+000101e0: 7569 6e63 7927 2c0a 2020 2020 2020 2020  uincy',.        
+000101f0: 2020 2020 2020 2020 6e61 6d65 5f70 7265          name_pre
+00010200: 6669 783d 2752 6576 2e27 2c0a 2020 2020  fix='Rev.',.    
+00010210: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00010220: 5f73 7566 6669 783d 2742 2e41 2e20 4d2e  _suffix='B.A. M.
+00010230: 4469 762e 270a 2020 2020 2020 2020 2020  Div.'.          
+00010240: 2020 290a 0a20 2020 2020 2020 2041 204b    )..        A K
+00010250: 6f72 6561 6e20 6361 7365 2077 6974 6820  orean case with 
+00010260: 7068 6f6e 6574 6963 2061 6e64 2069 6465  phonetic and ide
+00010270: 6f67 7261 7068 6963 2072 6570 7265 7365  ographic represe
+00010280: 6e74 6174 696f 6e73 2028 5053 332e 352d  ntations (PS3.5-
+00010290: 3230 3038 0a20 2020 2020 2020 2073 6563  2008.        sec
+000102a0: 7469 6f6e 2049 2e32 2070 2e20 3130 3829  tion I.2 p. 108)
+000102b0: 3a0a 0a20 2020 2020 2020 203e 3e3e 2070  :..        >>> p
+000102c0: 6e20 3d20 5065 7273 6f6e 4e61 6d65 2e66  n = PersonName.f
+000102d0: 726f 6d5f 6e61 6d65 645f 636f 6d70 6f6e  rom_named_compon
+000102e0: 656e 7473 280a 2020 2020 2020 2020 2020  ents(.          
+000102f0: 2020 2020 2020 6661 6d69 6c79 5f6e 616d        family_nam
+00010300: 653d 2748 6f6e 6727 2c0a 2020 2020 2020  e='Hong',.      
+00010310: 2020 2020 2020 2020 2020 6769 7665 6e5f            given_
+00010320: 6e61 6d65 3d27 4769 6c64 6f6e 6727 2c0a  name='Gildong',.
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 6661 6d69 6c79 5f6e 616d 655f 6964 656f  family_name_ideo
+00010350: 6772 6170 6869 633d 27e6 b4aa 272c 0a20  graphic='...',. 
+00010360: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00010370: 6976 656e 5f6e 616d 655f 6964 656f 6772  iven_name_ideogr
+00010380: 6170 6869 633d 27e5 9089 e6b4 9e27 2c0a  aphic='......',.
+00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 6661 6d69 6c79 5f6e 616d 655f 7068 6f6e  family_name_phon
+000103b0: 6574 6963 3d27 ed99 8d27 2c0a 2020 2020  etic='...',.    
+000103c0: 2020 2020 2020 2020 2020 2020 6769 7665              give
+000103d0: 6e5f 6e61 6d65 5f70 686f 6e65 7469 633d  n_name_phonetic=
+000103e0: 27ea b8b8 eb8f 9927 2c0a 2020 2020 2020  '......',.      
+000103f0: 2020 2020 2020 2020 2020 656e 636f 6469            encodi
+00010400: 6e67 733d 5b64 6566 6175 6c74 5f65 6e63  ngs=[default_enc
+00010410: 6f64 696e 672c 2027 6575 635f 6b72 275d  oding, 'euc_kr']
+00010420: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00010430: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00010440: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00010450: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6661  -----.        fa
+00010460: 6d69 6c79 5f6e 616d 653a 2055 6e69 6f6e  mily_name: Union
+00010470: 5b73 7472 2c20 6279 7465 735d 0a20 2020  [str, bytes].   
+00010480: 2020 2020 2020 2020 2046 616d 696c 7920           Family 
+00010490: 6e61 6d65 2069 6e20 616c 7068 6162 6574  name in alphabet
+000104a0: 6963 2066 6f72 6d2e 0a20 2020 2020 2020  ic form..       
+000104b0: 2067 6976 656e 5f6e 616d 653a 2055 6e69   given_name: Uni
+000104c0: 6f6e 5b73 7472 2c20 6279 7465 735d 0a20  on[str, bytes]. 
+000104d0: 2020 2020 2020 2020 2020 2047 6976 656e             Given
+000104e0: 206e 616d 6520 696e 2061 6c70 6861 6265   name in alphabe
+000104f0: 7469 6320 666f 726d 2e0a 2020 2020 2020  tic form..      
+00010500: 2020 6d69 6464 6c65 5f6e 616d 653a 2055    middle_name: U
+00010510: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+00010520: 0a20 2020 2020 2020 2020 2020 204d 6964  .            Mid
+00010530: 646c 6520 6e61 6d65 2069 6e20 616c 7068  dle name in alph
+00010540: 6162 6574 6963 2066 6f72 6d2e 0a20 2020  abetic form..   
+00010550: 2020 2020 206e 616d 655f 7072 6566 6978       name_prefix
+00010560: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
+00010570: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
+00010580: 4e61 6d65 2070 7265 6669 7820 696e 2061  Name prefix in a
+00010590: 6c70 6861 6265 7469 6320 666f 726d 2c20  lphabetic form, 
+000105a0: 652e 672e 2027 4d72 732e 272c 2027 4472  e.g. 'Mrs.', 'Dr
+000105b0: 2e27 2c20 2753 722e 272c 2027 5265 762e  .', 'Sr.', 'Rev.
+000105c0: 272e 0a20 2020 2020 2020 206e 616d 655f  '..        name_
+000105d0: 7375 6666 6978 3a20 556e 696f 6e5b 7374  suffix: Union[st
+000105e0: 722c 2062 7974 6573 5d0a 2020 2020 2020  r, bytes].      
+000105f0: 2020 2020 2020 4e61 6d65 2070 7265 6669        Name prefi
+00010600: 7820 696e 2061 6c70 6861 6265 7469 6320  x in alphabetic 
+00010610: 666f 726d 2c20 652e 672e 2027 4d2e 442e  form, e.g. 'M.D.
+00010620: 272c 2027 422e 412e 2c20 4d2e 4469 762e  ', 'B.A., M.Div.
+00010630: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00010640: 4368 6965 6620 4578 6563 7574 6976 6520  Chief Executive 
+00010650: 4f66 6669 6365 7227 2e0a 2020 2020 2020  Officer'..      
+00010660: 2020 6661 6d69 6c79 5f6e 616d 655f 6964    family_name_id
+00010670: 656f 6772 6170 6869 633a 2055 6e69 6f6e  eographic: Union
+00010680: 5b73 7472 2c20 6279 7465 735d 0a20 2020  [str, bytes].   
+00010690: 2020 2020 2020 2020 2046 616d 696c 7920           Family 
+000106a0: 6e61 6d65 2069 6e20 6964 656f 6772 6170  name in ideograp
+000106b0: 6869 6320 666f 726d 2e0a 2020 2020 2020  hic form..      
+000106c0: 2020 6769 7665 6e5f 6e61 6d65 5f69 6465    given_name_ide
+000106d0: 6f67 7261 7068 6963 3a20 556e 696f 6e5b  ographic: Union[
+000106e0: 7374 722c 2062 7974 6573 5d0a 2020 2020  str, bytes].    
+000106f0: 2020 2020 2020 2020 4769 7665 6e20 6e61          Given na
+00010700: 6d65 2069 6e20 6964 656f 6772 6170 6869  me in ideographi
+00010710: 6320 666f 726d 2e0a 2020 2020 2020 2020  c form..        
+00010720: 6d69 6464 6c65 5f6e 616d 655f 6964 656f  middle_name_ideo
+00010730: 6772 6170 6869 633a 2055 6e69 6f6e 5b73  graphic: Union[s
+00010740: 7472 2c20 6279 7465 735d 0a20 2020 2020  tr, bytes].     
+00010750: 2020 2020 2020 204d 6964 646c 6520 6e61         Middle na
+00010760: 6d65 2069 6e20 6964 656f 6772 6170 6869  me in ideographi
+00010770: 6320 666f 726d 2e0a 2020 2020 2020 2020  c form..        
+00010780: 6e61 6d65 5f70 7265 6669 785f 6964 656f  name_prefix_ideo
+00010790: 6772 6170 6869 633a 2055 6e69 6f6e 5b73  graphic: Union[s
+000107a0: 7472 2c20 6279 7465 735d 0a20 2020 2020  tr, bytes].     
+000107b0: 2020 2020 2020 204e 616d 6520 7072 6566         Name pref
+000107c0: 6978 2069 6e20 6964 656f 6772 6170 6869  ix in ideographi
+000107d0: 6320 666f 726d 2e0a 2020 2020 2020 2020  c form..        
+000107e0: 6e61 6d65 5f73 7566 6669 785f 6964 656f  name_suffix_ideo
+000107f0: 6772 6170 6869 633a 2055 6e69 6f6e 5b73  graphic: Union[s
+00010800: 7472 2c20 6279 7465 735d 0a20 2020 2020  tr, bytes].     
+00010810: 2020 2020 2020 204e 616d 6520 7375 6666         Name suff
+00010820: 6978 2069 6e20 6964 656f 6772 6170 6869  ix in ideographi
+00010830: 6320 666f 726d 2e0a 2020 2020 2020 2020  c form..        
+00010840: 6661 6d69 6c79 5f6e 616d 655f 7068 6f6e  family_name_phon
+00010850: 6574 6963 3a20 556e 696f 6e5b 7374 722c  etic: Union[str,
+00010860: 2062 7974 6573 5d0a 2020 2020 2020 2020   bytes].        
+00010870: 2020 2020 4661 6d69 6c79 206e 616d 6520      Family name 
+00010880: 696e 2070 686f 6e65 7469 6320 666f 726d  in phonetic form
+00010890: 2e0a 2020 2020 2020 2020 6769 7665 6e5f  ..        given_
+000108a0: 6e61 6d65 5f70 686f 6e65 7469 633a 2055  name_phonetic: U
+000108b0: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+000108c0: 0a20 2020 2020 2020 2020 2020 2047 6976  .            Giv
+000108d0: 656e 206e 616d 6520 696e 2070 686f 6e65  en name in phone
+000108e0: 7469 6320 666f 726d 2e0a 2020 2020 2020  tic form..      
+000108f0: 2020 6d69 6464 6c65 5f6e 616d 655f 7068    middle_name_ph
+00010900: 6f6e 6574 6963 3a20 556e 696f 6e5b 7374  onetic: Union[st
+00010910: 722c 2062 7974 6573 5d0a 2020 2020 2020  r, bytes].      
+00010920: 2020 2020 2020 4d69 6464 6c65 206e 616d        Middle nam
+00010930: 6520 696e 2070 686f 6e65 7469 6320 666f  e in phonetic fo
+00010940: 726d 2e0a 2020 2020 2020 2020 6e61 6d65  rm..        name
+00010950: 5f70 7265 6669 785f 7068 6f6e 6574 6963  _prefix_phonetic
+00010960: 3a20 556e 696f 6e5b 7374 722c 2062 7974  : Union[str, byt
+00010970: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
+00010980: 4e61 6d65 2070 7265 6669 7820 696e 2070  Name prefix in p
+00010990: 686f 6e65 7469 6320 666f 726d 2e0a 2020  honetic form..  
+000109a0: 2020 2020 2020 6e61 6d65 5f73 7566 6669        name_suffi
+000109b0: 785f 7068 6f6e 6574 6963 3a20 556e 696f  x_phonetic: Unio
+000109c0: 6e5b 7374 722c 2062 7974 6573 5d0a 2020  n[str, bytes].  
+000109d0: 2020 2020 2020 2020 2020 4e61 6d65 2073            Name s
+000109e0: 7566 6669 7820 696e 2070 686f 6e65 7469  uffix in phoneti
+000109f0: 6320 666f 726d 2e0a 2020 2020 2020 2020  c form..        
+00010a00: 656e 636f 6469 6e67 733a 204f 7074 696f  encodings: Optio
+00010a10: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0a20  nal[List[str]]. 
+00010a20: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
+00010a30: 7420 6f66 2065 6e63 6f64 696e 6773 2075  t of encodings u
+00010a40: 7365 6420 666f 7220 7468 6520 6f74 6865  sed for the othe
+00010a50: 7220 696e 7075 7420 7061 7261 6d65 7465  r input paramete
+00010a60: 7273 2e0a 0a20 2020 2020 2020 2052 6574  rs...        Ret
+00010a70: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00010a80: 2d2d 2d2d 0a20 2020 2020 2020 2050 6572  ----.        Per
+00010a90: 736f 6e4e 616d 653a 0a20 2020 2020 2020  sonName:.       
+00010aa0: 2020 2020 2050 6572 736f 6e4e 616d 6520       PersonName 
+00010ab0: 636f 6e73 7472 7563 7465 6420 6672 6f6d  constructed from
+00010ac0: 2074 6865 2073 7570 706c 6965 6420 636f   the supplied co
+00010ad0: 6d70 6f6e 656e 7473 2e0a 0a20 2020 2020  mponents...     
+00010ae0: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
+00010af0: 202d 2d2d 2d2d 0a20 2020 2020 2020 2053   -----.        S
+00010b00: 7472 696e 6773 206d 6179 206e 6f74 2063  trings may not c
+00010b10: 6f6e 7461 696e 2074 6865 2066 6f6c 6c6f  ontain the follo
+00010b20: 7769 6e67 2063 6861 7261 6374 6572 733a  wing characters:
+00010b30: 2027 5e27 2c20 273d 272c 0a20 2020 2020   '^', '=',.     
+00010b40: 2020 206f 7220 7468 6520 6261 636b 736c     or the backsl
+00010b50: 6173 6820 6368 6172 6163 7465 722e 0a20  ash character.. 
+00010b60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010b70: 2020 2061 6c70 6861 6265 7469 635f 6772     alphabetic_gr
+00010b80: 6f75 703a 204c 6973 745b 556e 696f 6e5b  oup: List[Union[
+00010b90: 7374 722c 2062 7974 6573 5d5d 203d 205b  str, bytes]] = [
+00010ba0: 0a20 2020 2020 2020 2020 2020 2066 616d  .            fam
+00010bb0: 696c 795f 6e61 6d65 2c0a 2020 2020 2020  ily_name,.      
+00010bc0: 2020 2020 2020 6769 7665 6e5f 6e61 6d65        given_name
+00010bd0: 2c0a 2020 2020 2020 2020 2020 2020 6d69  ,.            mi
+00010be0: 6464 6c65 5f6e 616d 652c 0a20 2020 2020  ddle_name,.     
+00010bf0: 2020 2020 2020 206e 616d 655f 7072 6566         name_pref
+00010c00: 6978 2c0a 2020 2020 2020 2020 2020 2020  ix,.            
+00010c10: 6e61 6d65 5f73 7566 6669 782c 0a20 2020  name_suffix,.   
+00010c20: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+00010c30: 2320 4964 656f 6772 6170 6869 6320 636f  # Ideographic co
+00010c40: 6d70 6f6e 656e 7420 6772 6f75 700a 2020  mponent group.  
+00010c50: 2020 2020 2020 6964 656f 6772 6170 6869        ideographi
+00010c60: 635f 6772 6f75 703a 204c 6973 745b 556e  c_group: List[Un
+00010c70: 696f 6e5b 7374 722c 2062 7974 6573 5d5d  ion[str, bytes]]
+00010c80: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00010c90: 2066 616d 696c 795f 6e61 6d65 5f69 6465   family_name_ide
+00010ca0: 6f67 7261 7068 6963 2c0a 2020 2020 2020  ographic,.      
+00010cb0: 2020 2020 2020 6769 7665 6e5f 6e61 6d65        given_name
+00010cc0: 5f69 6465 6f67 7261 7068 6963 2c0a 2020  _ideographic,.  
+00010cd0: 2020 2020 2020 2020 2020 6d69 6464 6c65            middle
+00010ce0: 5f6e 616d 655f 6964 656f 6772 6170 6869  _name_ideographi
+00010cf0: 632c 0a20 2020 2020 2020 2020 2020 206e  c,.            n
+00010d00: 616d 655f 7072 6566 6978 5f69 6465 6f67  ame_prefix_ideog
+00010d10: 7261 7068 6963 2c0a 2020 2020 2020 2020  raphic,.        
+00010d20: 2020 2020 6e61 6d65 5f73 7566 6669 785f      name_suffix_
+00010d30: 6964 656f 6772 6170 6869 632c 0a20 2020  ideographic,.   
+00010d40: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+00010d50: 2320 5068 6f6e 6574 6963 2063 6f6d 706f  # Phonetic compo
+00010d60: 6e65 6e74 2067 726f 7570 0a20 2020 2020  nent group.     
+00010d70: 2020 2070 686f 6e65 7469 635f 6772 6f75     phonetic_grou
+00010d80: 703a 204c 6973 745b 556e 696f 6e5b 7374  p: List[Union[st
+00010d90: 722c 2062 7974 6573 5d5d 203d 205b 0a20  r, bytes]] = [. 
+00010da0: 2020 2020 2020 2020 2020 2066 616d 696c             famil
+00010db0: 795f 6e61 6d65 5f70 686f 6e65 7469 632c  y_name_phonetic,
+00010dc0: 0a20 2020 2020 2020 2020 2020 2067 6976  .            giv
+00010dd0: 656e 5f6e 616d 655f 7068 6f6e 6574 6963  en_name_phonetic
+00010de0: 2c0a 2020 2020 2020 2020 2020 2020 6d69  ,.            mi
+00010df0: 6464 6c65 5f6e 616d 655f 7068 6f6e 6574  ddle_name_phonet
+00010e00: 6963 2c0a 2020 2020 2020 2020 2020 2020  ic,.            
+00010e10: 6e61 6d65 5f70 7265 6669 785f 7068 6f6e  name_prefix_phon
+00010e20: 6574 6963 2c0a 2020 2020 2020 2020 2020  etic,.          
+00010e30: 2020 6e61 6d65 5f73 7566 6669 785f 7068    name_suffix_ph
+00010e40: 6f6e 6574 6963 2c0a 2020 2020 2020 2020  onetic,.        
+00010e50: 5d0a 0a20 2020 2020 2020 2065 6e63 6f64  ]..        encod
+00010e60: 6564 5f76 616c 7565 3a20 6279 7465 7320  ed_value: bytes 
+00010e70: 3d20 636c 732e 5f65 6e63 6f64 655f 636f  = cls._encode_co
+00010e80: 6d70 6f6e 656e 745f 6772 6f75 7073 280a  mponent_groups(.
+00010e90: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+00010ea0: 6162 6574 6963 5f67 726f 7570 2c0a 2020  abetic_group,.  
+00010eb0: 2020 2020 2020 2020 2020 6964 656f 6772            ideogr
+00010ec0: 6170 6869 635f 6772 6f75 702c 0a20 2020  aphic_group,.   
+00010ed0: 2020 2020 2020 2020 2070 686f 6e65 7469           phoneti
+00010ee0: 635f 6772 6f75 702c 0a20 2020 2020 2020  c_group,.       
+00010ef0: 2020 2020 2065 6e63 6f64 696e 6773 2c0a       encodings,.
+00010f00: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00010f10: 2020 2072 6574 7572 6e20 636c 7328 656e     return cls(en
+00010f20: 636f 6465 645f 7661 6c75 652c 2065 6e63  coded_value, enc
+00010f30: 6f64 696e 6773 3d65 6e63 6f64 696e 6773  odings=encodings
+00010f40: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
+00010f50: 686f 640a 2020 2020 6465 6620 6672 6f6d  hod.    def from
+00010f60: 5f6e 616d 6564 5f63 6f6d 706f 6e65 6e74  _named_component
+00010f70: 735f 7665 7465 7269 6e61 7279 280a 2020  s_veterinary(.  
+00010f80: 2020 2020 2020 636c 732c 0a20 2020 2020        cls,.     
+00010f90: 2020 2072 6573 706f 6e73 6962 6c65 5f70     responsible_p
+00010fa0: 6172 7479 5f6e 616d 653a 2055 6e69 6f6e  arty_name: Union
+00010fb0: 5b73 7472 2c20 6279 7465 735d 203d 2027  [str, bytes] = '
+00010fc0: 272c 0a20 2020 2020 2020 2070 6174 6965  ',.        patie
+00010fd0: 6e74 5f6e 616d 653a 2055 6e69 6f6e 5b73  nt_name: Union[s
+00010fe0: 7472 2c20 6279 7465 735d 203d 2027 272c  tr, bytes] = '',
+00010ff0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00011000: 6962 6c65 5f70 6172 7479 5f6e 616d 655f  ible_party_name_
+00011010: 6964 656f 6772 6170 6869 633a 2055 6e69  ideographic: Uni
+00011020: 6f6e 5b73 7472 2c20 6279 7465 735d 203d  on[str, bytes] =
+00011030: 2027 272c 0a20 2020 2020 2020 2070 6174   '',.        pat
+00011040: 6965 6e74 5f6e 616d 655f 6964 656f 6772  ient_name_ideogr
+00011050: 6170 6869 633a 2055 6e69 6f6e 5b73 7472  aphic: Union[str
+00011060: 2c20 6279 7465 735d 203d 2027 272c 0a20  , bytes] = '',. 
+00011070: 2020 2020 2020 2072 6573 706f 6e73 6962         responsib
+00011080: 6c65 5f70 6172 7479 5f6e 616d 655f 7068  le_party_name_ph
+00011090: 6f6e 6574 6963 3a20 556e 696f 6e5b 7374  onetic: Union[st
+000110a0: 722c 2062 7974 6573 5d20 3d20 2727 2c0a  r, bytes] = '',.
+000110b0: 2020 2020 2020 2020 7061 7469 656e 745f          patient_
+000110c0: 6e61 6d65 5f70 686f 6e65 7469 633a 2055  name_phonetic: U
+000110d0: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+000110e0: 203d 2027 272c 0a20 2020 2020 2020 2065   = '',.        e
+000110f0: 6e63 6f64 696e 6773 3a20 4f70 7469 6f6e  ncodings: Option
+00011100: 616c 5b4c 6973 745b 7374 725d 5d20 3d20  al[List[str]] = 
+00011110: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2027  None,.    ) -> '
+00011120: 5065 7273 6f6e 4e61 6d65 273a 0a20 2020  PersonName':.   
+00011130: 2020 2020 2022 2222 436f 6e73 7472 7563       """Construc
+00011140: 7420 6120 5065 7273 6f6e 4e61 6d65 2066  t a PersonName f
+00011150: 726f 6d20 6578 706c 6963 6974 206e 616d  rom explicit nam
+00011160: 6564 2063 6f6d 706f 6e65 6e74 7320 666f  ed components fo
+00011170: 6c6c 6f77 696e 6720 7468 650a 2020 2020  llowing the.    
+00011180: 2020 2020 7665 7465 7269 6e61 7279 2075      veterinary u
+00011190: 7361 6765 2063 6f6e 7665 6e74 696f 6e2e  sage convention.
+000111a0: 0a0a 2020 2020 2020 2020 5468 6520 4449  ..        The DI
+000111b0: 434f 4d20 7374 616e 6461 7264 2064 6573  COM standard des
+000111c0: 6372 6962 6573 206e 616d 6573 2066 6f72  cribes names for
+000111d0: 2076 6574 6572 696e 6172 7920 7573 6520   veterinary use 
+000111e0: 7769 7468 2074 776f 2063 6f6d 706f 6e65  with two compone
+000111f0: 6e74 733a 0a20 2020 2020 2020 2072 6573  nts:.        res
+00011200: 706f 6e73 6962 6c65 2070 6172 7479 2066  ponsible party f
+00011210: 616d 696c 7920 6e61 6d65 204f 5220 7265  amily name OR re
+00011220: 7370 6f6e 7369 626c 6520 7061 7274 7920  sponsible party 
+00011230: 6f72 6761 6e69 7a61 7469 6f6e 206e 616d  organization nam
+00011240: 652c 0a20 2020 2020 2020 2061 6e64 2070  e,.        and p
+00011250: 6174 6965 6e74 206e 616d 652e 0a20 2020  atient name..   
+00011260: 2020 2020 2041 6e79 2063 6f6d 706f 6e65       Any compone
+00011270: 6e74 206d 6179 2062 6520 616e 2065 6d70  nt may be an emp
+00011280: 7479 2073 7472 696e 6720 2874 6865 2064  ty string (the d
+00011290: 6566 6175 6c74 2920 6966 206e 6f74 2075  efault) if not u
+000112a0: 7365 642e 0a20 2020 2020 2020 2041 2063  sed..        A c
+000112b0: 6f6d 706f 6e65 6e74 206d 6179 2063 6f6e  omponent may con
+000112c0: 7461 696e 206d 756c 7469 706c 6520 7370  tain multiple sp
+000112d0: 6163 652d 7365 7061 7261 7465 6420 776f  ace-separated wo
+000112e0: 7264 7320 6966 206e 6563 6573 7361 7279  rds if necessary
+000112f0: 2e0a 0a20 2020 2020 2020 2041 6464 6974  ...        Addit
+00011300: 696f 6e61 6c6c 792c 2065 6163 6820 636f  ionally, each co
+00011310: 6d70 6f6e 656e 7420 6d61 7920 6265 2072  mponent may be r
+00011320: 6570 7265 7365 6e74 6564 2069 6e20 6964  epresented in id
+00011330: 656f 6772 6170 6869 6320 6f72 0a20 2020  eographic or.   
+00011340: 2020 2020 2070 686f 6e65 7469 6320 666f       phonetic fo
+00011350: 726d 2069 6e20 6164 6469 7469 6f6e 2074  rm in addition t
+00011360: 6f20 286f 7220 696e 7374 6561 6420 6f66  o (or instead of
+00011370: 2920 616c 7068 6162 6574 6963 2066 6f72  ) alphabetic for
+00011380: 6d2e 0a0a 2020 2020 2020 2020 466f 7220  m...        For 
+00011390: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+000113a0: 2073 6565 2074 6865 2066 6f6c 6c6f 7769   see the followi
+000113b0: 6e67 2070 6172 7473 206f 6620 7468 6520  ng parts of the 
+000113c0: 4449 434f 4d20 7374 616e 6461 7264 3a0a  DICOM standard:.
+000113d0: 2020 2020 2020 2020 2d20 3a64 636d 3a60          - :dcm:`
+000113e0: 5661 6c75 6520 5265 7072 6573 656e 7461  Value Representa
+000113f0: 7469 6f6e 7320 3c70 6172 7430 352f 7365  tions <part05/se
+00011400: 6374 5f36 2e32 2e68 746d 6c3e 600a 2020  ct_6.2.html>`.  
+00011410: 2020 2020 2020 2d20 3a64 636d 3a60 504e        - :dcm:`PN
+00011420: 2045 7861 6d70 6c65 7320 3c70 6172 7430   Examples <part0
+00011430: 352f 7365 6374 5f36 2e32 2e68 746d 6c23  5/sect_6.2.html#
+00011440: 7365 6374 5f36 2e32 2e31 2e31 3e60 0a20  sect_6.2.1.1>`. 
+00011450: 2020 2020 2020 202d 203a 6463 6d3a 6050         - :dcm:`P
+00011460: 4e20 5072 6563 6973 6520 7365 6d61 6e74  N Precise semant
+00011470: 6963 7320 3c70 6172 7430 352f 7365 6374  ics <part05/sect
+00011480: 5f36 2e32 2e68 746d 6c23 7365 6374 5f36  _6.2.html#sect_6
+00011490: 2e32 2e31 2e31 3e60 0a0a 2020 2020 2020  .2.1.1>`..      
+000114a0: 2020 4578 616d 706c 650a 2020 2020 2020    Example.      
+000114b0: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2020    -------..     
+000114c0: 2020 2041 2068 6f72 7365 2077 686f 7365     A horse whose
+000114d0: 2072 6573 706f 6e73 6962 6c65 206f 7267   responsible org
+000114e0: 616e 697a 6174 696f 6e20 6973 206e 616d  anization is nam
+000114f0: 6564 2022 4142 4320 4661 726d 7322 2c20  ed "ABC Farms", 
+00011500: 616e 6420 7768 6f73 650a 2020 2020 2020  and whose.      
+00011510: 2020 6e61 6d65 2069 7320 2252 756e 6e69    name is "Runni
+00011520: 6e67 204f 6e20 5761 7465 7222 0a0a 2020  ng On Water"..  
+00011530: 2020 2020 2020 3e3e 3e20 706e 203d 2050        >>> pn = P
+00011540: 6572 736f 6e4e 616d 652e 6672 6f6d 5f6e  ersonName.from_n
+00011550: 616d 6564 5f63 6f6d 706f 6e65 6e74 735f  amed_components_
+00011560: 7665 7465 7269 6e61 7279 280a 2020 2020  veterinary(.    
+00011570: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+00011580: 6f6e 7369 626c 655f 7061 7274 795f 6e61  onsible_party_na
+00011590: 6d65 3d27 4142 4320 4661 726d 7327 2c0a  me='ABC Farms',.
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115b0: 7061 7469 656e 745f 6e61 6d65 3d27 5275  patient_name='Ru
+000115c0: 6e6e 696e 6720 6f6e 2057 6174 6572 270a  nning on Water'.
+000115d0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000115e0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000115f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00011600: 2d2d 2d2d 0a20 2020 2020 2020 2072 6573  ----.        res
+00011610: 706f 6e73 6962 6c65 5f70 6172 7479 5f6e  ponsible_party_n
+00011620: 616d 653a 2055 6e69 6f6e 5b73 7472 2c20  ame: Union[str, 
+00011630: 6279 7465 735d 0a20 2020 2020 2020 2020  bytes].         
+00011640: 2020 204e 616d 6520 6f66 2074 6865 2072     Name of the r
+00011650: 6573 706f 6e73 6962 6c65 2070 6172 7479  esponsible party
+00011660: 2069 6e20 616c 7068 6162 6574 6963 2066   in alphabetic f
+00011670: 6f72 6d2e 2054 6869 7320 6d61 7920 6265  orm. This may be
+00011680: 0a20 2020 2020 2020 2020 2020 2065 6974  .            eit
+00011690: 6865 7220 7468 6520 6661 6d69 6c79 206e  her the family n
+000116a0: 616d 6520 6f66 2074 6865 2072 6573 706f  ame of the respo
+000116b0: 6e73 6962 6c65 2070 6172 7479 2c20 6f72  nsible party, or
+000116c0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+000116d0: 206e 616d 6520 6f66 2074 6865 2072 6573   name of the res
+000116e0: 706f 6e73 6962 6c65 206f 7267 616e 697a  ponsible organiz
+000116f0: 6174 696f 6e2e 0a20 2020 2020 2020 2070  ation..        p
+00011700: 6174 6965 6e74 5f6e 616d 653a 2055 6e69  atient_name: Uni
+00011710: 6f6e 5b73 7472 2c20 6279 7465 735d 0a20  on[str, bytes]. 
+00011720: 2020 2020 2020 2020 2020 2050 6174 6965             Patie
+00011730: 6e74 206e 616d 6520 696e 2061 6c70 6861  nt name in alpha
+00011740: 6265 7469 6320 666f 726d 2e0a 2020 2020  betic form..    
+00011750: 2020 2020 7265 7370 6f6e 7369 626c 655f      responsible_
+00011760: 7061 7274 795f 6e61 6d65 5f69 6465 6f67  party_name_ideog
+00011770: 7261 7068 6963 3a20 556e 696f 6e5b 7374  raphic: Union[st
+00011780: 722c 2062 7974 6573 5d0a 2020 2020 2020  r, bytes].      
+00011790: 2020 2020 2020 4e61 6d65 206f 6620 7468        Name of th
+000117a0: 6520 7265 7370 6f6e 7369 626c 6520 7061  e responsible pa
+000117b0: 7274 7920 696e 2069 6465 6f67 7261 7068  rty in ideograph
+000117c0: 6963 2066 6f72 6d2e 0a20 2020 2020 2020  ic form..       
+000117d0: 2070 6174 6965 6e74 5f6e 616d 655f 6964   patient_name_id
+000117e0: 656f 6772 6170 6869 633a 2055 6e69 6f6e  eographic: Union
+000117f0: 5b73 7472 2c20 6279 7465 735d 0a20 2020  [str, bytes].   
+00011800: 2020 2020 2020 2020 2050 6174 6965 6e74           Patient
+00011810: 206e 616d 6520 696e 2069 6465 6f67 7261   name in ideogra
+00011820: 7068 6963 2066 6f72 6d2e 0a20 2020 2020  phic form..     
+00011830: 2020 2072 6573 706f 6e73 6962 6c65 5f70     responsible_p
+00011840: 6172 7479 5f6e 616d 655f 7068 6f6e 6574  arty_name_phonet
+00011850: 6963 3a20 556e 696f 6e5b 7374 722c 2062  ic: Union[str, b
+00011860: 7974 6573 5d0a 2020 2020 2020 2020 2020  ytes].          
+00011870: 2020 4e61 6d65 206f 6620 7468 6520 7265    Name of the re
+00011880: 7370 6f6e 7369 626c 6520 7061 7274 7920  sponsible party 
+00011890: 696e 2070 686f 6e65 7469 6320 666f 726d  in phonetic form
+000118a0: 2e0a 2020 2020 2020 2020 7061 7469 656e  ..        patien
+000118b0: 745f 6e61 6d65 5f70 686f 6e65 7469 633a  t_name_phonetic:
+000118c0: 2055 6e69 6f6e 5b73 7472 2c20 6279 7465   Union[str, byte
+000118d0: 735d 0a20 2020 2020 2020 2020 2020 2050  s].            P
+000118e0: 6174 6965 6e74 206e 616d 6520 696e 2070  atient name in p
+000118f0: 686f 6e65 7469 6320 666f 726d 2e0a 2020  honetic form..  
+00011900: 2020 2020 2020 656e 636f 6469 6e67 733a        encodings:
+00011910: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00011920: 7472 5d5d 0a20 2020 2020 2020 2020 2020  tr]].           
+00011930: 2041 206c 6973 7420 6f66 2065 6e63 6f64   A list of encod
+00011940: 696e 6773 2075 7365 6420 666f 7220 7468  ings used for th
+00011950: 6520 6f74 6865 7220 696e 7075 7420 7061  e other input pa
+00011960: 7261 6d65 7465 7273 0a0a 2020 2020 2020  rameters..      
+00011970: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00011980: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00011990: 2020 5065 7273 6f6e 4e61 6d65 3a0a 2020    PersonName:.  
+000119a0: 2020 2020 2020 2020 2020 5065 7273 6f6e            Person
+000119b0: 4e61 6d65 2063 6f6e 7374 7275 6374 6564  Name constructed
+000119c0: 2066 726f 6d20 7468 6520 7375 7070 6c69   from the suppli
+000119d0: 6564 2063 6f6d 706f 6e65 6e74 730a 0a20  ed components.. 
+000119e0: 2020 2020 2020 204e 6f74 6573 0a20 2020         Notes.   
+000119f0: 2020 2020 202d 2d2d 2d2d 0a20 2020 2020       -----.     
+00011a00: 2020 2053 7472 696e 6773 206d 6179 206e     Strings may n
+00011a10: 6f74 2063 6f6e 7461 696e 2074 6865 2066  ot contain the f
+00011a20: 6f6c 6c6f 7769 6e67 2063 6861 7261 6374  ollowing charact
+00011a30: 6572 733a 2027 5e27 2c20 273d 272c 0a20  ers: '^', '=',. 
+00011a40: 2020 2020 2020 206f 7220 7468 6520 6261         or the ba
+00011a50: 636b 736c 6173 6820 6368 6172 6163 7465  ckslash characte
+00011a60: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+00011a70: 2020 2020 2020 2061 6c70 6861 6265 7469         alphabeti
+00011a80: 635f 6772 6f75 703a 204c 6973 745b 556e  c_group: List[Un
+00011a90: 696f 6e5b 7374 722c 2062 7974 6573 5d5d  ion[str, bytes]]
+00011aa0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00011ab0: 2072 6573 706f 6e73 6962 6c65 5f70 6172   responsible_par
+00011ac0: 7479 5f6e 616d 652c 0a20 2020 2020 2020  ty_name,.       
+00011ad0: 2020 2020 2070 6174 6965 6e74 5f6e 616d       patient_nam
+00011ae0: 652c 0a20 2020 2020 2020 205d 0a0a 2020  e,.        ]..  
+00011af0: 2020 2020 2020 6964 656f 6772 6170 6869        ideographi
+00011b00: 635f 6772 6f75 703a 204c 6973 745b 556e  c_group: List[Un
+00011b10: 696f 6e5b 7374 722c 2062 7974 6573 5d5d  ion[str, bytes]]
+00011b20: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00011b30: 2072 6573 706f 6e73 6962 6c65 5f70 6172   responsible_par
+00011b40: 7479 5f6e 616d 655f 6964 656f 6772 6170  ty_name_ideograp
+00011b50: 6869 632c 0a20 2020 2020 2020 2020 2020  hic,.           
+00011b60: 2070 6174 6965 6e74 5f6e 616d 655f 6964   patient_name_id
+00011b70: 656f 6772 6170 6869 632c 0a20 2020 2020  eographic,.     
+00011b80: 2020 205d 0a0a 2020 2020 2020 2020 7068     ]..        ph
+00011b90: 6f6e 6574 6963 5f67 726f 7570 3a20 4c69  onetic_group: Li
+00011ba0: 7374 5b55 6e69 6f6e 5b73 7472 2c20 6279  st[Union[str, by
+00011bb0: 7465 735d 5d20 3d20 5b0a 2020 2020 2020  tes]] = [.      
+00011bc0: 2020 2020 2020 7265 7370 6f6e 7369 626c        responsibl
+00011bd0: 655f 7061 7274 795f 6e61 6d65 5f70 686f  e_party_name_pho
+00011be0: 6e65 7469 632c 0a20 2020 2020 2020 2020  netic,.         
+00011bf0: 2020 2070 6174 6965 6e74 5f6e 616d 655f     patient_name_
+00011c00: 7068 6f6e 6574 6963 2c0a 2020 2020 2020  phonetic,.      
+00011c10: 2020 5d0a 0a20 2020 2020 2020 2065 6e63    ]..        enc
+00011c20: 6f64 6564 5f76 616c 7565 3a20 6279 7465  oded_value: byte
+00011c30: 7320 3d20 636c 732e 5f65 6e63 6f64 655f  s = cls._encode_
+00011c40: 636f 6d70 6f6e 656e 745f 6772 6f75 7073  component_groups
+00011c50: 280a 2020 2020 2020 2020 2020 2020 616c  (.            al
+00011c60: 7068 6162 6574 6963 5f67 726f 7570 2c0a  phabetic_group,.
+00011c70: 2020 2020 2020 2020 2020 2020 6964 656f              ideo
+00011c80: 6772 6170 6869 635f 6772 6f75 702c 0a20  graphic_group,. 
+00011c90: 2020 2020 2020 2020 2020 2070 686f 6e65             phone
+00011ca0: 7469 635f 6772 6f75 702c 0a20 2020 2020  tic_group,.     
+00011cb0: 2020 2020 2020 2065 6e63 6f64 696e 6773         encodings
+00011cc0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00011cd0: 2020 2020 7265 7475 726e 2063 6c73 2865      return cls(e
+00011ce0: 6e63 6f64 6564 5f76 616c 7565 2c20 656e  ncoded_value, en
+00011cf0: 636f 6469 6e67 733d 656e 636f 6469 6e67  codings=encoding
+00011d00: 7329 0a0a 0a23 2041 6c69 6173 206f 6c64  s)...# Alias old
+00011d10: 2063 6c61 7373 206e 616d 6573 2066 6f72   class names for
+00011d20: 2062 6163 6b77 6172 6473 2063 6f6d 7061   backwards compa
+00011d30: 7420 696e 2075 7365 7220 636f 6465 0a64  t in user code.d
+00011d40: 6566 205f 5f67 6574 6174 7472 5f5f 286e  ef __getattr__(n
+00011d50: 616d 653a 2073 7472 2920 2d3e 2041 6e79  ame: str) -> Any
+00011d60: 3a0a 2020 2020 6966 206e 616d 6520 3d3d  :.    if name ==
+00011d70: 2022 5065 7273 6f6e 4e61 6d65 556e 6963   "PersonNameUnic
+00011d80: 6f64 6522 3a0a 2020 2020 2020 2020 7761  ode":.        wa
+00011d90: 726e 696e 6773 2e77 6172 6e28 0a20 2020  rnings.warn(.   
+00011da0: 2020 2020 2020 2020 2022 2750 6572 736f           "'Perso
+00011db0: 6e4e 616d 6555 6e69 636f 6465 2720 6973  nNameUnicode' is
+00011dc0: 2064 6570 7265 6361 7465 6420 616e 6420   deprecated and 
+00011dd0: 7769 6c6c 2062 6520 7265 6d6f 7665 6420  will be removed 
+00011de0: 696e 2022 0a20 2020 2020 2020 2020 2020  in ".           
+00011df0: 2022 7079 6469 636f 6d20 7633 2e30 2c20   "pydicom v3.0, 
+00011e00: 7573 6520 2750 6572 736f 6e4e 616d 6527  use 'PersonName'
+00011e10: 2069 6e73 7465 6164 222c 0a20 2020 2020   instead",.     
+00011e20: 2020 2020 2020 2044 6570 7265 6361 7469         Deprecati
+00011e30: 6f6e 5761 726e 696e 670a 2020 2020 2020  onWarning.      
+00011e40: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+00011e50: 726e 2067 6c6f 6261 6c73 2829 5b27 5065  rn globals()['Pe
+00011e60: 7273 6f6e 4e61 6d65 275d 0a0a 2020 2020  rsonName']..    
+00011e70: 7261 6973 6520 4174 7472 6962 7574 6545  raise AttributeE
+00011e80: 7272 6f72 2866 226d 6f64 756c 6520 7b5f  rror(f"module {_
+00011e90: 5f6e 616d 655f 5f7d 2068 6173 206e 6f20  _name__} has no 
+00011ea0: 6174 7472 6962 7574 6520 7b6e 616d 657d  attribute {name}
+00011eb0: 2229 0a0a 0a69 6620 7379 732e 7665 7273  ")...if sys.vers
+00011ec0: 696f 6e5f 696e 666f 5b3a 325d 203c 2028  ion_info[:2] < (
+00011ed0: 332c 2037 293a 0a20 2020 2050 6572 736f  3, 7):.    Perso
+00011ee0: 6e4e 616d 6555 6e69 636f 6465 203d 2050  nNameUnicode = P
+00011ef0: 6572 736f 6e4e 616d 650a                 ersonName.
```

### Comparing `pydicom-2.3.1/pydicom/values.py` & `pydicom-2.4.0/pydicom/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,17 @@
     # "=" means use 'standard' size, needed on 64-bit systems.
     bytes_per_value = calcsize("=" + struct_format)
     length = len(byte_string)
 
     if length % bytes_per_value != 0:
         raise BytesLengthException(
             "Expected total bytes to be an even multiple of bytes per value. "
-            f"Instead received {byte_string!r} with length {length} and "
+            f"Instead received "
+            f"{repr(byte_string) if len(byte_string) <= 256 else 'bytes'} "
+            f"with length {length} and "
             f"struct format '{struct_format}' which corresponds to bytes per "
             f"value of {bytes_per_value}."
         )
 
     format_string = f"{endianChar}{length // bytes_per_value}{struct_format}"
     value: Union[Tuple[int, ...], Tuple[float, ...]] = (
         unpack(format_string, byte_string)
@@ -460,22 +462,30 @@
         A list of the character encoding schemes used to encode the 'PN' value.
 
     Returns
     -------
     valuerep.PersonName or MultiValue of PersonName
         The decoded 'PN' value(s).
     """
-    def get_valtype(x: bytes) -> PersonName:
-        return PersonName(x, encodings).decode()
 
-    b_split = byte_string.rstrip(b'\x00 ').split(b'\\')
-    if len(b_split) == 1:
-        return get_valtype(b_split[0])
+    encodings = encodings or [default_encoding]
 
-    return MultiValue(get_valtype, b_split)
+    def get_valtype(x: str) -> PersonName:
+        person_name = PersonName(x, encodings)
+        # Using an already decoded string in PersonName constructor leaves
+        # the original string as undefined, let's set it through encode
+        person_name.encode()
+        return person_name.decode()
+
+    stripped_string = byte_string.rstrip(b'\x00 ')
+    decoded_value = decode_bytes(stripped_string, encodings, TEXT_VR_DELIMS)
+    value_splitted = decoded_value.split('\\')
+    if len(value_splitted) == 1:
+        return get_valtype(value_splitted[0])
+    return MultiValue(get_valtype, value_splitted)
 
 
 def convert_string(
     byte_string: bytes,
     is_little_endian: bool,
     struct_format: Optional[str] = None
 ) -> Union[str, MutableSequence[str]]:
@@ -519,20 +529,26 @@
         The value representation of the element. Needed for validation.
 
     Returns
     -------
     str or list of str
         The decoded value(s).
     """
-    values = byte_string.split(b'\\')
-    as_strings = [convert_single_string(value, encodings, vr)
-                  for value in values]
+    def handle_value(v: str) -> str:
+        if vr is not None:
+            validate_value(
+                vr, v, config.settings.reading_validation_mode)
+        return v.rstrip('\0 ')
+
+    encodings = encodings or [default_encoding]
+    decoded_string = decode_bytes(byte_string, encodings, TEXT_VR_DELIMS)
+    values = decoded_string.split("\\")
+    as_strings = [handle_value(value) for value in values]
     if len(as_strings) == 1:
         return as_strings[0]
-
     return MultiValue(str, as_strings,
                       validation_mode=config.settings.reading_validation_mode)
 
 
 def convert_single_string(
     byte_string: bytes, encodings: Optional[List[str]] = None,
     vr: str = None,
@@ -549,19 +565,19 @@
         The value representation of the element. Needed for validation.
 
     Returns
     -------
     str
         The decoded text.
     """
-    if vr is not None:
-        validate_value(
-            vr, byte_string, config.settings.reading_validation_mode)
     encodings = encodings or [default_encoding]
     value = decode_bytes(byte_string, encodings, TEXT_VR_DELIMS)
+    if vr is not None:
+        validate_value(
+            vr, value, config.settings.reading_validation_mode)
     return value.rstrip('\0 ')
 
 
 def convert_SQ(
     byte_string: bytes,
     is_implicit_VR: bool,
     is_little_endian: bool,
```

### Comparing `pydicom-2.3.1/pydicom/waveforms/numpy_handler.py` & `pydicom-2.4.0/pydicom/waveforms/numpy_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             arr = arr.astype('float')
             seq = cast(List["Dataset"], item.ChannelDefinitionSequence)
             for jj, ch in enumerate(seq):
                 baseline = ch.get("ChannelBaseline", 0.0)
                 sensitivity = ch.get("ChannelSensitivity", 1.0)
                 correction = ch.get("ChannelSensitivityCorrectionFactor", 1.0)
                 arr[..., jj] = (
-                    (arr[..., jj] + baseline) * sensitivity * correction
+                    arr[..., jj] * sensitivity * correction + baseline
                 )
 
         yield arr
 
 
 def multiplex_array(
     ds: "Dataset", index: int, as_raw: bool = True
@@ -210,11 +210,11 @@
         arr = arr.astype('float')
         seq = cast(List["Dataset"], item.ChannelDefinitionSequence)
         for jj, ch in enumerate(seq):
             baseline = ch.get("ChannelBaseline", 0.0)
             sensitivity = ch.get("ChannelSensitivity", 1.0)
             correction = ch.get("ChannelSensitivityCorrectionFactor", 1.0)
             arr[..., jj] = (
-                (arr[..., jj] + baseline) * sensitivity * correction
+                arr[..., jj] * sensitivity * correction + baseline
             )
 
     return cast("np.ndarray", arr)
```

### Comparing `pydicom-2.3.1/setup.py` & `pydicom-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Remove setup.py in pydicom v3.0
 import os
 from pathlib import Path
 from setuptools import setup, find_packages
 
 try:
     import dicom
     HAVE_DICOM = True
@@ -42,15 +43,14 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Healthcare Industry",
         "Intended Audience :: Science/Research",
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
@@ -60,15 +60,15 @@
     packages=find_packages(),
     py_modules=[] if not HAVE_DICOM else ["dicom"],
     package_data={
         'pydicom': data_files_inventory() + ['py.typed'],
     },
     include_package_data=True,
     zip_safe=False,
-    python_requires='>=3.6.1',
+    python_requires='>=3.7',
     install_requires=[],
     extras_require={
         "docs": [
             "numpy",
             "numpydoc",
             "matplotlib",
             "pillow",
```

