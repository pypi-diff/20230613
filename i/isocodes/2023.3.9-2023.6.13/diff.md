# Comparing `tmp/isocodes-2023.3.9.tar.gz` & `tmp/isocodes-2023.6.13.tar.gz`

## Comparing `isocodes-2023.3.9.tar` & `isocodes-2023.6.13.tar`

### file list

```diff
@@ -1,1154 +1,1163 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.flake8
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.gitmodules
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 isocodes-2023.3.9/tox.ini
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 isocodes-2023.3.9/update.sh
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.github/workflows/publish-test.yaml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.github/workflows/upgrade-dependencies.yml
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/__init__.py
--rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_15924.json
--rw-r--r--   0        0        0    43284 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_3166-1.json
--rw-r--r--   0        0        0   501099 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_3166-2.json
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_3166-3.json
--rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_4217.json
--rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_639-2.json
--rw-r--r--   0        0        0   874782 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_639-3.json
--rw-r--r--   0        0        0     8486 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_639-5.json
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-15924.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-3166-1.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-3166-2.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-3166-3.json
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-4217.json
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-639-2.json
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-639-3.json
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-639-5.json
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ace/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ach/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    22487 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ak/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/an/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    28339 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    31617 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22752 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22649 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   311331 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ay/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ba/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    29950 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   201179 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    27908 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    18766 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    28906 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    15126 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    15015 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35751 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    96597 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    35713 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    32879 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    22283 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23830 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23424 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    25765 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ce/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ch/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/chr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21581 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    20258 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   256161 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24009 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24860 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14412 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/csb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23328 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   135392 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23454 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   219517 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23574 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   395472 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/dv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    40229 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/dz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ee/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    57390 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    91227 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/en/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8524 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    47595 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22133 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    48656 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10493 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    15692 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23281 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9689 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23059 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22375 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    30637 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23811 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    21800 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    20888 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ff/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    21391 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23844 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24141 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   166186 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23058 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   407281 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/frp/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    23756 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    22913 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/fy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    23528 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    14446 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22783 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   306888 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35101 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32619 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    44025 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/gv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ha/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/haw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    35310 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23488 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    26178 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    52545 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ht/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    69162 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    30567 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/hy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ia/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23003 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   165253 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23311 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   292415 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/io/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23986 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   149997 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23660 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   163383 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   369645 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/iu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24942 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   100171 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23644 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    16790 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/jam/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    36655 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   109788 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ki/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35806 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/km/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    29606 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32465 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   390349 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24204 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24693 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kok/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kok/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9310 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/kw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    29069 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ky/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ky/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23186 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    75936 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22164 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    31678 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22888 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mai/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    27425 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    34752 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    34245 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35144 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32230 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   425099 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/my/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/na/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nah/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23349 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ne/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23417 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   196696 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23302 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    85951 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/nv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23463 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    34110 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32596 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   217560 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    31594 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   410401 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    14875 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pap/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23647 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   188055 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23814 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   121821 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23926 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23190 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    15062 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23166 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22866 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    27706 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23251 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   112174 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    11510 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    29137 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    18412 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    21974 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    15826 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   104509 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23525 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sd/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    31931 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/si/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23531 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24319 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22611 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    79740 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/son/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23866 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   145300 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    29938 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    17095 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   122426 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23553 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   164336 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   398696 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/sw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    31984 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    33169 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   438383 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    35338 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32092 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    28527 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    33663 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    83632 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    18029 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23676 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    77264 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24213 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   343245 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    21810 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    29812 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ug/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   265202 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    12535 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    29090 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   511201 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/uz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24644 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   135733 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    27170 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    16925 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    22427 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wal/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21638 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/wo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/yo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23425 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   117078 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23076 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23030 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23183 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24205 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    32698 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/pkgconfig/iso-codes.pc
--rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_15924.xml
--rw-r--r--   0        0        0    40003 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_3166-1.xml
--rw-r--r--   0        0        0   334692 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_3166-2.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_3166-3.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_3166.xml -> iso_3166-1.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_3166_2.xml -> iso_3166-2.xml
--rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_4217.xml
--rw-r--r--   0        0        0    48857 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639-2.xml
--rw-r--r--   0        0        0  1016601 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639-3.xml
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639-5.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639.xml -> iso_639-2.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639_3.xml -> iso_639-3.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639_5.xml -> iso_639-5.xml
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 isocodes-2023.3.9/requirements/build-requirements.txt
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 isocodes-2023.3.9/requirements/dev-requirements.txt
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 isocodes-2023.3.9/requirements/doc-requirements.txt
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 isocodes-2023.3.9/requirements/requirements.txt
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 isocodes-2023.3.9/requirements/test-requirements.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 isocodes-2023.3.9/tests/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isocodes-2023.3.9/tests/test_general.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 isocodes-2023.3.9/.gitignore
--rw-r--r--   0        0        0    24477 2020-02-02 00:00:00.000000 isocodes-2023.3.9/LICENSE
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 isocodes-2023.3.9/README.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 isocodes-2023.3.9/pyproject.toml
--rw-r--r--   0        0        0    32328 2020-02-02 00:00:00.000000 isocodes-2023.3.9/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.gitmodules
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 isocodes-2023.6.13/tox.ini
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 isocodes-2023.6.13/update.sh
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/dependabot.yml
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/publish-test.yaml
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/__init__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/py.typed
+-rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_15924.json
+-rw-r--r--   0        0        0    43284 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-1.json
+-rw-r--r--   0        0        0   501099 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-2.json
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-3.json
+-rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_4217.json
+-rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-2.json
+-rw-r--r--   0        0        0   874782 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-3.json
+-rw-r--r--   0        0        0     8486 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-5.json
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-15924.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-1.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-2.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-3.json
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-4217.json
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-2.json
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-3.json
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-5.json
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ace/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ach/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    22487 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ak/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/an/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    28339 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    31617 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22752 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22649 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   311331 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ay/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ba/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    30045 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   201179 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    27908 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    18766 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    28945 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    15126 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35751 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    96597 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    35713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    32879 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    22283 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23927 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23424 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    25765 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ce/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ch/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/chr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21581 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    20258 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   256161 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24094 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24860 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14412 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/csb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    35290 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    15797 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14506 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23328 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   135392 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23454 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   219517 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23574 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   395556 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    40229 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ee/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    57390 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    91227 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/en/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8524 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    47595 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22133 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    48656 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10493 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    15724 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9689 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23059 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22375 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    30637 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23811 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    21800 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    20888 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ff/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    21391 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23844 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24141 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   166186 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23058 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   407281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/frp/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    23756 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    22913 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    23528 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    14446 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22867 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   306888 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35101 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32619 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    44025 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ha/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    35310 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23488 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    26178 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    52545 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ht/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    69162 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    30567 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23086 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   165253 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23311 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   292415 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/io/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24295 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23986 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   149997 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23660 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   163383 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   369645 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/iu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24942 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   100171 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23644 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    16790 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/jam/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    36655 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   109788 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ki/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35806 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    29606 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32465 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   390349 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24204 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9310 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    29069 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23186 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    75936 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22164 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    31678 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22888 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mai/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    27425 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    34752 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    34245 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35144 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32230 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   425099 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/my/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/na/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nah/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23349 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   213685 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23302 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    86365 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23749 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    34110 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32596 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   217560 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    31594 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   410401 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    14875 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pap/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23849 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   188055 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23814 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   121821 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23926 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23190 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    15062 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23166 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22866 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    27706 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23251 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   112174 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    11510 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    29137 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    18412 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    21974 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    15826 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24430 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   104509 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23525 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sd/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    31931 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23531 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24319 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22611 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    79740 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/son/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23866 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   145300 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    29938 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    17095 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   122426 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23553 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   164336 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   398696 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    31984 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    33169 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   438383 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    35338 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32092 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    28527 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    33663 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    83632 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    18029 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23676 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    77264 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24213 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   343245 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    21810 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    29812 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   265202 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    12535 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    29090 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   511201 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24644 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   135733 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    27170 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    16925 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    22427 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21638 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/yo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23425 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   117078 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23388 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24126 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23390 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24253 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    32698 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/pkgconfig/iso-codes.pc
+-rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_15924.xml
+-rw-r--r--   0        0        0    40003 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-1.xml
+-rw-r--r--   0        0        0   334692 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-2.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-3.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166.xml -> iso_3166-1.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166_2.xml -> iso_3166-2.xml
+-rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_4217.xml
+-rw-r--r--   0        0        0    48857 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-2.xml
+-rw-r--r--   0        0        0  1016601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-3.xml
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-5.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639.xml -> iso_639-2.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639_3.xml -> iso_639-3.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639_5.xml -> iso_639-5.xml
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/build-requirements.txt
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/dev-requirements.txt
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/doc-requirements.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/requirements.txt
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/test-requirements.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 isocodes-2023.6.13/tests/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isocodes-2023.6.13/tests/test_general.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.gitignore
+-rw-r--r--   0        0        0    24477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/LICENSE
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 isocodes-2023.6.13/README.md
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 isocodes-2023.6.13/pyproject.toml
+-rw-r--r--   0        0        0    32330 2020-02-02 00:00:00.000000 isocodes-2023.6.13/PKG-INFO
```

### Comparing `isocodes-2023.3.9/.pre-commit-config.yaml` & `isocodes-2023.6.13/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/.github/workflows/codeql.yml` & `isocodes-2023.6.13/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/.github/workflows/publish-test.yaml` & `isocodes-2023.6.13/.github/workflows/publish-test.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 on:
   push:
     branches:        
       - main
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to TestPyPI
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     steps:
       - name: Checkout
         uses: actions/checkout@v3.2.0
-      - name: Set up Python 3.7
+      - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: 3.9
       - name: Install build dependencies
         run: pip install -r requirements/build-requirements.txt
       - name: Build package
         run: hatch build
       - name: Publish distribution 📦 to Test PyPI
         uses: pypa/gh-action-pypi-publish@v1.6.4
         with:
```

### Comparing `isocodes-2023.3.9/.github/workflows/publish.yaml` & `isocodes-2023.6.13/.github/workflows/publish.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 on:
   push:
     tags:        
       - '*'
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     steps:
       - name: Checkout
         uses: actions/checkout@v3.2.0
-      - name: Set up Python 3.7
+      - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: 3.9
       - name: Install dependencies
         run: pip install -r requirements/build-requirements.txt
       - name: Build package
         run: hatch build
       - name: Publish distribution 📦 to PyPI
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@v1.6.4
```

### Comparing `isocodes-2023.3.9/.github/workflows/test.yaml` & `isocodes-2023.6.13/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Test iso-codes
 on: [pull_request]
 jobs:
   pytest:
     name: Run tests
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
         python: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: Checkout
         uses: actions/checkout@v3.2.0
       - name: Set up Python
```

### Comparing `isocodes-2023.3.9/isocodes/__init__.py` & `isocodes-2023.6.13/isocodes/__init__.py`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_15924.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_15924.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_3166-1.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-1.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_3166-2.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_3166-3.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_4217.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_4217.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_639-2.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_639-3.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/iso_639-5.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-5.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-15924.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-15924.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-3166-1.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-1.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-3166-2.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-3166-3.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-4217.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-4217.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-639-2.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-639-3.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/iso-codes/json/schema-639-5.json` & `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-5.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-10-17 00:54+0000\n"
+"PO-Revision-Date: 2023-03-11 04:51+0000\n"
 "Last-Translator: Viktar Vauchkevich <victorenator@gmail.com>\n"
 "Language-Team: Belarusian <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/be/>\n"
 "Language: be\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "Afghanistan"
 msgstr "Афганістан"
 
 msgid "Albania"
 msgstr "Албанія"
 
@@ -410,14 +410,17 @@
 
 msgid "India"
 msgstr "Індыя"
 
 msgid "Indonesia"
 msgstr "Інданезія"
 
+msgid "Iran"
+msgstr "Іран"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Іран, Ісламская Рэспубліка"
 
 msgid "Iraq"
 msgstr "Ірак"
 
 msgid "Ireland"
@@ -527,14 +530,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Кыргызстан"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Лаоская Народна-Дэмакратычная Рэспубліка"
 
+msgid "Laos"
+msgstr "Лаос"
+
 msgid "Latvia"
 msgstr "Латвія"
 
 msgid "Lebanese Republic"
 msgstr "Ліванская Рэспубліка"
 
 msgid "Lebanon"
@@ -1136,14 +1142,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Швейцарская Канфедэрацыя"
 
 msgid "Switzerland"
 msgstr "Швейцарыя"
 
+msgid "Syria"
+msgstr "Сірыя"
+
 msgid "Syrian Arab Republic"
 msgstr "Сірыйская Арабская Рэспубліка"
 
 msgid "Taiwan"
 msgstr "Тайвань"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2015-06-19 15:59+0300\n"
-"Last-Translator: Viktar Siarheichyk <vics@fsfe.org>\n"
-"Language-Team: Debian l10n team for Belarusian <debian-l10n-belarusian@lists."
-"debian.org>\n"
+"PO-Revision-Date: 2023-03-11 04:51+0000\n"
+"Last-Translator: Viktar Vauchkevich <victorenator@gmail.com>\n"
+"Language-Team: Belarusian <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-3/be/>\n"
 "Language: be\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Virtaal 0.7.1\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "British Antarctic Territory"
 msgstr "Брытанскія тэрыторыі ў Антарктыдзе"
 
 msgid "Burma, Socialist Republic of the Union of"
 msgstr "Бірма, Сацыялістычная Рэспубліка Бірманскага Саюза"
 
@@ -96,9 +98,12 @@
 
 msgid "Wake Island"
 msgstr "Востраў Уэйк"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
 msgstr "Емен, Народная Дэмакратычная Рэспубліка"
 
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Югаславія, Сацыялістычная Федэратыўная Рэспубліка"
+
 msgid "Zaire, Republic of"
 msgstr "Заір, Рэспубліка"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-12-10 18:48+0000\n"
-"Last-Translator: Chris Leonard <cjlhomeaddress@gmail.com>\n"
-"Language-Team: Bulgarian <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-1/bg/>\n"
+"PO-Revision-Date: 2023-04-06 19:14+0300\n"
+"Last-Translator: Damyan Ivanov <dmn@debian.org>\n"
+"Language-Team: Bulgarian <dict@ludost.net>\n"
 "Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"X-Generator: Gtranslator 42.0\n"
 
 msgid "Afghanistan"
 msgstr "Афганистан"
 
 msgid "Albania"
 msgstr "Албания"
 
@@ -409,14 +408,17 @@
 
 msgid "India"
 msgstr "Индия"
 
 msgid "Indonesia"
 msgstr "Индонезия"
 
+msgid "Iran"
+msgstr "Иран"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Иран, Ислямска република"
 
 msgid "Iraq"
 msgstr "Ирак"
 
 msgid "Ireland"
@@ -526,14 +528,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Киргизстан"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Демократична република на народа на Лао"
 
+msgid "Laos"
+msgstr "Лаос"
+
 msgid "Latvia"
 msgstr "Латвия"
 
 msgid "Lebanese Republic"
 msgstr "Лебанска република"
 
 msgid "Lebanon"
@@ -1135,14 +1140,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Швейцарска конфедерация"
 
 msgid "Switzerland"
 msgstr "Швейцария"
 
+msgid "Syria"
+msgstr "Сирия"
+
 msgid "Syrian Arab Republic"
 msgstr "Сирийска арабска република"
 
 msgid "Taiwan"
 msgstr "Тайван"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,104 +1,103 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2016-01-03 17:54+0200\n"
-"Last-Translator: Damyan Ivanov <dmn@debian.org>\n"
-"Language-Team: Bulgarian <dict@ludost.net>\n"
-"Language: bg\n"
+"PO-Revision-Date: 2011-06-20 11:05+0100\n"
+"Last-Translator: Arangel Angov <arangel@linux.net.mk>\n"
+"Language-Team: Macedonian <ossm-members@hedona.on.net.mk>\n"
+"Language: mk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Gtranslator 2.91.7\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"X-Generator: KBabel 1.11.4\n"
 
 msgid "British Antarctic Territory"
-msgstr "Британски антарктически територии"
+msgstr "Британска антартичка територија"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Бурма, Социалистическа република на обединението"
+msgstr "Социјалистичка република на сојузот на Бурма"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Белоруска ССР"
+msgstr "Беолоруска ССР Советска социјалистичка република"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Острови Кантон и Ендербъри"
+msgstr "Кантон и Ендербури"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Чехословакия, Чехословашка социалистическа република"
+msgstr "Чехословачка, Чехословачка социјалистичка Република"
 
 msgid "Dahomey"
-msgstr "Дахоми"
+msgstr "Дахомеј"
 
 msgid "Dronning Maud Land"
-msgstr "Земя на кралица Мод"
+msgstr "Dronning Maud Land"
 
 msgid "East Timor"
-msgstr "Източен Тимор"
+msgstr "Источен Тимор"
 
 msgid "France, Metropolitan"
-msgstr "Франция, метрополитен"
+msgstr "Франција, Метрополијан"
 
 msgid "French Afars and Issas"
-msgstr "Френски Афари и Исаи"
+msgstr "Француски Афарс и Исас"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Френски южни и антарктически територии"
+msgstr "Јужни француски територии и антартички територии"
 
 msgid "German Democratic Republic"
-msgstr "Германска Демократична Република"
+msgstr "Демократска република Германија"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Острови Гилберт и Елис"
+msgstr "Островите Гилберт и Елис"
 
 msgid "Johnston Island"
-msgstr "Остров Джонсън"
+msgstr "Островот на Џонстон"
 
 msgid "Midway Islands"
-msgstr "Острови Мидуей"
+msgstr "Острови Мидвеј"
 
 msgid "Netherlands Antilles"
-msgstr "Холандски Антили"
+msgstr "Холандски антили"
 
 msgid "Neutral Zone"
 msgstr "Неутрална зона"
 
 msgid "New Hebrides"
-msgstr "Нови Хебриди"
+msgstr "Нов Хебридес"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Тихоокеански острови"
+msgstr "Пацифички острови (сигурна територија)"
 
 msgid "Panama Canal Zone"
-msgstr "Панама централна зона"
+msgstr "Панамски канал"
 
 msgid "Serbia and Montenegro"
-msgstr "Сърбия и Черна гора"
+msgstr "Србија и Црна Гора"
 
 msgid "Sikkim"
 msgstr "Сиким"
 
 msgid "Southern Rhodesia"
-msgstr "Южна Родезия"
+msgstr "Јужна Родезија"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "САЩ - тихоокеански острови"
+msgstr "Разни острови на САД во пацификот"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "СССР, Съюз на съветските социалистически републики"
+msgstr "УССР, Унија на советски социјалистички републики"
 
 msgid "Upper Volta, Republic of"
-msgstr "Горна Волта, Република"
+msgstr "Република горна Волта"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Виетнам, Демократична република"
+msgstr "Демократска република Виетнам"
 
 msgid "Wake Island"
-msgstr "Остров Уейк"
+msgstr "Островот Вејк"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr "Йемен, Демократична, Народна демократична република"
+msgstr "Демократска република Јемен"
 
 msgid "Zaire, Republic of"
-msgstr "Заир, Република"
+msgstr "Република Заир"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_639-2\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2014-08-21 23:24+0300\n"
-"Last-Translator: Roumen Petrov <transl@roumenpetrov.info>\n"
+"PO-Revision-Date: 2023-04-06 19:18+0300\n"
+"Last-Translator: Damyan Ivanov <dmn@debian.org>\n"
 "Language-Team: Bulgarian <dict@ludost.net>\n"
 "Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"X-Generator: Gtranslator 42.0\n"
 
 msgid "Abkhazian"
 msgstr "Абхазки"
 
 msgid "Achinese"
 msgstr "Ачински"
 
@@ -679,14 +680,17 @@
 
 msgid "Somali"
 msgstr "Сомалийски"
 
 msgid "Sorbian languages"
 msgstr "Лужишки езици"
 
+msgid "South American Indian (Other)"
+msgstr "южноамерикански индиански (други)"
+
 msgid "Southern Altai"
 msgstr "Южно-алтайски"
 
 msgid "Southern Sami"
 msgstr "Южносаамски"
 
 msgid "Spanish; Castilian"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-12-24 22:57+0100\n"
-"Last-Translator: Sergi Almacellas Abellana <sergi@koolpi.com>\n"
+"PO-Revision-Date: 2023-03-29 20:40+0000\n"
+"Last-Translator: Chris Leonard <cjlhomeaddress@gmail.com>\n"
 "Language-Team: Catalan <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/ca/>\n"
 "Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Poedit 2.4.2\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albània"
 
@@ -59,15 +59,15 @@
 msgid "Australia"
 msgstr "Austràlia"
 
 msgid "Austria"
 msgstr "Àustria"
 
 msgid "Azerbaijan"
-msgstr "Azerbaitjan"
+msgstr "Azerbaidjan"
 
 msgid "Bahamas"
 msgstr "Bahames"
 
 msgid "Bahrain"
 msgstr "Bahrain"
 
@@ -86,15 +86,15 @@
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
 msgstr "Benín"
 
 msgid "Bermuda"
-msgstr "Bermuda"
+msgstr "Bermudes"
 
 msgid "Bhutan"
 msgstr "Bhutan"
 
 msgid "Bolivarian Republic of Venezuela"
 msgstr "República Bolívariana de Veneçuela"
 
@@ -409,14 +409,17 @@
 
 msgid "India"
 msgstr "Índia"
 
 msgid "Indonesia"
 msgstr "Indonèsia"
 
+msgid "Iran"
+msgstr "Iran"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Iran"
 
 msgid "Iraq"
 msgstr "Iraq"
 
 msgid "Ireland"
@@ -526,14 +529,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Kirguizistan"
 
 msgid "Lao People's Democratic Republic"
 msgstr "República Democràtica Popular de Laos"
 
+msgid "Laos"
+msgstr "Laos"
+
 msgid "Latvia"
 msgstr "Letònia"
 
 msgid "Lebanese Republic"
 msgstr "República Libanesa"
 
 msgid "Lebanon"
@@ -665,15 +671,15 @@
 msgid "North Korea"
 msgstr "Corea del Nord"
 
 msgid "North Macedonia"
 msgstr "Macedònia del Nord"
 
 msgid "Northern Mariana Islands"
-msgstr "Illes Marianes del Nord"
+msgstr "Illes Mariannes Septentrionals"
 
 msgid "Norway"
 msgstr "Noruega"
 
 msgid "Oman"
 msgstr "Oman"
 
@@ -1010,21 +1016,21 @@
 msgid "Romania"
 msgstr "Romania"
 
 msgid "Russian Federation"
 msgstr "Federació Russa"
 
 msgid "Rwanda"
-msgstr "Rwanda"
+msgstr "Ruanda"
 
 msgid "Rwandese Republic"
 msgstr "República Rwandesa"
 
 msgid "Réunion"
-msgstr "Reunió"
+msgstr "Illa de la Reunió"
 
 msgid "Saint Barthélemy"
 msgstr "Saint Barthélemy"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
 msgstr "Saint Helena, Ascension i Tristan da Cunha"
 
@@ -1088,15 +1094,15 @@
 msgid "Solomon Islands"
 msgstr "Illes Salomó"
 
 msgid "Somalia"
 msgstr "Somàlia"
 
 msgid "South Africa"
-msgstr "Sudàfrica"
+msgstr "Sud-àfrica"
 
 msgid "South Georgia and the South Sandwich Islands"
 msgstr "Illes Geòrgia del Sud i Sandwich del Sud"
 
 msgid "South Korea"
 msgstr "Corea del Sud"
 
@@ -1135,14 +1141,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Confederació Suïssa"
 
 msgid "Switzerland"
 msgstr "Suïssa"
 
+msgid "Syria"
+msgstr "Síria"
+
 msgid "Syrian Arab Republic"
 msgstr "República Àrab Síria"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan, Province of China"
@@ -1199,15 +1208,15 @@
 msgid "Ukraine"
 msgstr "Ucraïna"
 
 msgid "Union of the Comoros"
 msgstr "Unió de les Comores"
 
 msgid "United Arab Emirates"
-msgstr "Unió dels Emirats Àrabs"
+msgstr "Emirats Àrabs Units"
 
 msgid "United Kingdom"
 msgstr "Regne Unit"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
 msgstr "Regne Unit de la Gran Bretanya i Irlanda del Nord"
 
@@ -1265,15 +1274,15 @@
 msgid "Yemen"
 msgstr "Iemen"
 
 msgid "Zambia"
 msgstr "Zàmbia"
 
 msgid "Zimbabwe"
-msgstr "Zimbabwe"
+msgstr "Zimbàbue"
 
 msgid "the State of Eritrea"
 msgstr "Estat d'Eritrea"
 
 msgid "the State of Palestine"
 msgstr "Estat de Palestina"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2012-03-05 22:45+0200\n"
-"Last-Translator: Toni Hermoso Pulido <toniher@softcatala.org>\n"
-"Language-Team: Catalan <ca@dodds.net>\n"
+"PO-Revision-Date: 2023-03-29 20:40+0000\n"
+"Last-Translator: d <dmanye@gmail.com>\n"
+"Language-Team: Catalan <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-3/ca/>\n"
 "Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Pootle 2.1.6\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "British Antarctic Territory"
 msgstr "Territori Britànic Antàrtic"
 
 msgid "Burma, Socialist Republic of the Union of"
 msgstr "Burma, República Socialista de la Unió de"
 
@@ -96,9 +97,12 @@
 
 msgid "Wake Island"
 msgstr "Illes Wake"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
 msgstr "Iemen, Democràtic, República democràtica popular del"
 
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Iugoslàvia, República Federal Socialista de"
+
 msgid "Zaire, Republic of"
 msgstr "Zaire, República del"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,511 +1,511 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_4217\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-06-21 08:20+0000\n"
-"Last-Translator: Sergi Almacellas Abellana <sergi@koolpi.com>\n"
-"Language-Team: Catalan <https://hosted.weblate.org/projects/iso-codes/"
-"iso-4217/ca/>\n"
-"Language: ca\n"
+"PO-Revision-Date: 2021-05-24 20:32+0000\n"
+"Last-Translator: Adolfo Jayme Barrientos <fitojb@ubuntu.com>\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/iso-codes/"
+"iso-4217/es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.13.1-dev\n"
-"X-Bugs: Report translation errors to the Language-Team address.\n"
+"X-Generator: Weblate 4.7-dev\n"
+
+msgid "ADB Unit of Account"
+msgstr "Unidad de cuenta del ADB"
 
 msgid "Afghani"
-msgstr "Afgani"
+msgstr "Afganí"
 
 msgid "Algerian Dinar"
-msgstr "Dinar algerià"
+msgstr "Dinar argelino"
 
 msgid "Argentine Peso"
-msgstr "Peso argentí"
+msgstr "Peso argentino"
 
 msgid "Armenian Dram"
-msgstr "Dram armeni"
+msgstr "Dram armenio"
 
 msgid "Aruban Florin"
-msgstr "Florí d'Aruba"
+msgstr "Florín arubeño"
 
 msgid "Australian Dollar"
-msgstr "Dòlar australià"
+msgstr "Dólar australiano"
 
 msgid "Bahamian Dollar"
-msgstr "Dòlar de les Bahames"
+msgstr "Dólar bahameño"
 
 msgid "Bahraini Dinar"
-msgstr "Dinar de Bahrain"
+msgstr "Dinar bareiní"
 
 msgid "Baht"
 msgstr "Baht"
 
 msgid "Balboa"
 msgstr "Balboa"
 
 msgid "Barbados Dollar"
-msgstr "Dòlar de Barbados"
+msgstr "Dólar barbadense"
 
 msgid "Belarusian Ruble"
-msgstr "Ruble bielorús"
+msgstr "Rublo bielorruso"
 
 msgid "Belize Dollar"
-msgstr "Dòlar de Belize"
+msgstr "Dólar beliceño"
 
 msgid "Bermudian Dollar"
-msgstr "Dòlar de les Bermudes"
+msgstr "Dólar bermudeño"
 
 msgid "Boliviano"
 msgstr "Boliviano"
 
-msgid "Bolívar Soberano"
-msgstr "Bolívar Sobirà"
-
 msgid "Bond Markets Unit European Composite Unit (EURCO)"
-msgstr "Unitat composta europea per al mercat d'obligacions (EURCO)"
+msgstr "Unidad de Mercados de Bonos Unidad Europea Compuesta (EURCO)"
 
 msgid "Bond Markets Unit European Monetary Unit (E.M.U.-6)"
-msgstr "Unitat monetària europea per al mercat d'obligacions (EMU-6)"
+msgstr "Unidad de Mercados de Bonos Unidad Monetaria Europea (E.U.M.-6)"
+
+msgid "Bond Markets Unit European Unit of Account 17 (E.U.A.-17)"
+msgstr "Unidad de Mercados de Bonos Unidad de cuenta europea 17 (E.U.A.-17)"
+
+msgid "Bond Markets Unit European Unit of Account 9 (E.U.A.-9)"
+msgstr "Unidad de Mercados de Bonos Unidad de cuenta europea 9 (E.U.A.-9)"
 
 msgid "Brazilian Real"
-msgstr "Real brasiler"
+msgstr "Real brasileño"
 
 msgid "Brunei Dollar"
-msgstr "Dòlar de Brunei"
+msgstr "Dólar bruneano"
 
 msgid "Bulgarian Lev"
-msgstr "Lev búlgar"
+msgstr "Lev búlgaro"
 
 msgid "Burundi Franc"
-msgstr "Franc de Burundi"
+msgstr "Franco burundés"
 
 msgid "CFA Franc BCEAO"
-msgstr "Franc CFA de la BCEAO"
+msgstr "franco CFA BCEAO"
 
 msgid "CFA Franc BEAC"
-msgstr "Franc CFA de la BEAC"
+msgstr "franco CFA BEAC"
 
 msgid "CFP Franc"
-msgstr "Franc CFP"
+msgstr "Franco CFP"
 
 msgid "Cabo Verde Escudo"
-msgstr "Escut de Cap Verd"
+msgstr "Escudo caboverdiano"
 
 msgid "Canadian Dollar"
-msgstr "Dòlar canadenc"
+msgstr "Dólar canadiense"
 
 msgid "Cayman Islands Dollar"
-msgstr "Dòlar de les Illes Caiman"
+msgstr "Dólar caimanés"
 
 msgid "Chilean Peso"
-msgstr "Peso xilè"
+msgstr "Peso chileno"
 
 msgid "Codes specifically reserved for testing purposes"
-msgstr "Codis específicament reservats per proves"
+msgstr "Códigos reservados específicamente para pruebas"
 
 msgid "Colombian Peso"
-msgstr "Peso colombià"
-
-msgid "Comorian Franc"
-msgstr "Franc de les Comores"
+msgstr "Peso colombiano"
 
 msgid "Congolese Franc"
-msgstr "Franc congolès"
+msgstr "Franco congoleño"
 
 msgid "Convertible Mark"
-msgstr "Marc convertible"
+msgstr "Marco convertible"
 
 msgid "Cordoba Oro"
-msgstr "Córdoba or"
+msgstr "Córdoba"
 
 msgid "Costa Rican Colon"
-msgstr "Colon costa-riqueny"
+msgstr "Colón costarricense"
 
 msgid "Cuban Peso"
-msgstr "Peso cubà"
+msgstr "Peso cubano"
 
 msgid "Czech Koruna"
-msgstr "Corona txeca"
+msgstr "Corona checa"
 
 msgid "Dalasi"
 msgstr "Dalasi"
 
 msgid "Danish Krone"
 msgstr "Corona danesa"
 
 msgid "Denar"
 msgstr "Denar"
 
 msgid "Djibouti Franc"
-msgstr "Franc de Djibouti"
+msgstr "Franco yibutiano"
 
 msgid "Dobra"
 msgstr "Dobra"
 
 msgid "Dominican Peso"
-msgstr "Peso dominicà"
+msgstr "Peso dominicano"
 
 msgid "Dong"
 msgstr "Dong"
 
 msgid "East Caribbean Dollar"
-msgstr "Dòlar del Carib Oriental"
+msgstr "Dólar del Caribe oriental"
 
 msgid "Egyptian Pound"
-msgstr "Lliura egípcia"
+msgstr "Libra egipcia"
 
 msgid "El Salvador Colon"
-msgstr "Colon salvadorenc"
+msgstr "Colón salvadoreño"
 
 msgid "Ethiopian Birr"
-msgstr "Birr etíop"
+msgstr "Birr etíope"
 
 msgid "Euro"
 msgstr "Euro"
 
 msgid "Falkland Islands Pound"
-msgstr "Lliura de les Malvines"
+msgstr "Libra malvinense"
 
 msgid "Fiji Dollar"
-msgstr "Dòlar de Fiji"
+msgstr "Dólar fiyiano"
 
 msgid "Forint"
-msgstr "Fòrint"
+msgstr "Forint húngaro"
 
 msgid "Ghana Cedi"
-msgstr "Cedi de Ghana"
+msgstr "Cedi ghanés"
 
 msgid "Gibraltar Pound"
-msgstr "Lliura de Gibraltar"
+msgstr "Libra gibraltareña"
 
 msgid "Gold"
-msgstr "Or"
+msgstr "Oro"
 
 msgid "Gourde"
-msgstr "Gourde"
+msgstr "Gourde haitiano"
 
 msgid "Guarani"
 msgstr "Guaraní"
 
-msgid "Guinean Franc"
-msgstr "Franc de Guinea"
-
 msgid "Guyana Dollar"
-msgstr "Dòlar de Guyana"
+msgstr "Dólar guayanés"
 
 msgid "Hong Kong Dollar"
-msgstr "Dòlar de Hong Kong"
+msgstr "Dólar hongkonés"
 
 msgid "Hryvnia"
-msgstr "Hrívnia"
+msgstr "Grivnia"
 
 msgid "Iceland Krona"
 msgstr "Corona islandesa"
 
 msgid "Indian Rupee"
-msgstr "Rupia índia"
+msgstr "Rupia india"
 
 msgid "Iranian Rial"
-msgstr "Rial iranià"
+msgstr "Rial iraní"
 
 msgid "Iraqi Dinar"
-msgstr "Dinar iraquià"
+msgstr "Dinar iraquí"
 
 msgid "Jamaican Dollar"
-msgstr "Dòlar jamaicà"
+msgstr "Dólar jamaiqueño"
 
 msgid "Jordanian Dinar"
-msgstr "Dinar jordà"
+msgstr "Dinar jordano"
 
 msgid "Kenyan Shilling"
-msgstr "Xíling kenyà"
+msgstr "Chelín keniata"
 
 msgid "Kina"
 msgstr "Kina"
 
 msgid "Kuna"
 msgstr "Kuna"
 
 msgid "Kuwaiti Dinar"
-msgstr "Dinar kuwaitià"
+msgstr "Dinar kuwaití"
 
 msgid "Kwanza"
 msgstr "Kwanza"
 
 msgid "Kyat"
 msgstr "Kyat"
 
 msgid "Lari"
 msgstr "Lari"
 
 msgid "Lebanese Pound"
-msgstr "Lliura libanesa"
+msgstr "Libra libanesa"
 
 msgid "Lek"
 msgstr "Lek"
 
 msgid "Lempira"
 msgstr "Lempira"
 
 msgid "Leone"
 msgstr "Leone"
 
 msgid "Liberian Dollar"
-msgstr "Dòlar liberià"
+msgstr "Dólar liberiano"
 
 msgid "Libyan Dinar"
-msgstr "Dinar libi"
+msgstr "Dinar libio"
 
 msgid "Lilangeni"
-msgstr "Lilangeni"
+msgstr "Lilangeni suazi"
 
 msgid "Loti"
 msgstr "Loti"
 
 msgid "Malagasy Ariary"
-msgstr "Ariary malgaix"
+msgstr "Ariary malgache"
 
 msgid "Malawi Kwacha"
-msgstr "Kwacha malawià"
+msgstr "Kwacha malauí"
 
 msgid "Malaysian Ringgit"
-msgstr "Ringgit de Malàisia"
+msgstr "Ringgit malasio"
 
 msgid "Mauritius Rupee"
 msgstr "Rupia mauriciana"
 
 msgid "Mexican Peso"
-msgstr "Peso mexicà"
+msgstr "Peso mexicano"
 
 msgid "Moldovan Leu"
-msgstr "Leu moldau"
+msgstr "Leu moldavo"
 
 msgid "Moroccan Dirham"
 msgstr "Dírham marroquí"
 
 msgid "Mozambique Metical"
-msgstr "Metical de Moçambic"
+msgstr "Metical mozambiqueño"
 
 msgid "Naira"
 msgstr "Naira"
 
 msgid "Nakfa"
 msgstr "Nakfa"
 
 msgid "Namibia Dollar"
-msgstr "Dòlar namibià"
+msgstr "Dólar namibio"
 
 msgid "Nepalese Rupee"
 msgstr "Rupia nepalesa"
 
 msgid "Netherlands Antillean Guilder"
-msgstr "Florí de les Antilles Neerlandeses"
+msgstr "Florín antillano neerlandés"
 
 msgid "New Israeli Sheqel"
-msgstr "Nou xéquel israelià"
+msgstr "Nuevo séquel israelí"
 
 msgid "New Taiwan Dollar"
-msgstr "Nou dòlar de Taiwan"
+msgstr "Nuevo dólar taiwanés"
 
 msgid "New Zealand Dollar"
-msgstr "Dòlar neozelandès"
+msgstr "Dólar neozelandés"
 
 msgid "Ngultrum"
 msgstr "Ngultrum"
 
 msgid "North Korean Won"
-msgstr "Won nord-coreà"
+msgstr "Won norcoreano"
 
 msgid "Norwegian Krone"
 msgstr "Corona noruega"
 
 msgid "Ouguiya"
-msgstr "Ouguiya"
+msgstr "Uquiya"
 
 msgid "Pakistan Rupee"
-msgstr "Rupia pakistanesa"
+msgstr "Rupia pakistaní"
 
 msgid "Palladium"
-msgstr "Pal·ladi"
+msgstr "Paladio"
 
 msgid "Pataca"
 msgstr "Pataca"
 
 msgid "Pa’anga"
-msgstr "Pa'anga"
+msgstr "Paʻanga"
 
 msgid "Peso Convertible"
 msgstr "Peso convertible"
 
 msgid "Peso Uruguayo"
-msgstr "Peso uruguaià"
+msgstr "Peso uruguayo"
 
 msgid "Philippine Peso"
-msgstr "Peso filipí"
+msgstr "Peso filipino"
 
 msgid "Platinum"
-msgstr "Platí"
+msgstr "Platino"
 
 msgid "Pound Sterling"
-msgstr "Lliura esterlina"
+msgstr "Libra esterlina"
 
 msgid "Pula"
 msgstr "Pula"
 
 msgid "Qatari Rial"
-msgstr "Rial de Qatar"
+msgstr "Rial catarí"
 
 msgid "Quetzal"
 msgstr "Quetzal"
 
 msgid "Rand"
 msgstr "Rand"
 
 msgid "Rial Omani"
-msgstr "Rial omanita"
+msgstr "Rial omaní"
 
 msgid "Riel"
-msgstr "Riel"
+msgstr "Riel camboyano"
 
 msgid "Romanian Leu"
-msgstr "Leu romanès"
+msgstr "Leu rumano"
 
 msgid "Rufiyaa"
 msgstr "Rufiyaa"
 
 msgid "Rupiah"
-msgstr "Rupia"
+msgstr "Rupia indonesia"
 
 msgid "Russian Ruble"
-msgstr "Ruble rus"
+msgstr "Rublo ruso"
 
 msgid "Rwanda Franc"
-msgstr "Franc de Ruanda"
+msgstr "Franco ruandés"
 
 msgid "SDR (Special Drawing Right)"
-msgstr "DEG (drets especials de gir)"
+msgstr "DEG (Derecho especial de giro)"
 
 msgid "Saint Helena Pound"
-msgstr "Lliura de Santa Helena"
+msgstr "Libra santaeleniana"
 
 msgid "Saudi Riyal"
-msgstr "Rial saudita"
+msgstr "Rial saudí"
 
 msgid "Serbian Dinar"
-msgstr "Dinar serbi"
+msgstr "Dinar serbio"
 
 msgid "Seychelles Rupee"
-msgstr "Rupia de les Seychelles"
+msgstr "Rupia seychellense"
 
 msgid "Silver"
 msgstr "Plata"
 
 msgid "Singapore Dollar"
-msgstr "Dòlar de Singapur"
+msgstr "Dólar singapurense"
 
 msgid "Sol"
 msgstr "Sol"
 
 msgid "Solomon Islands Dollar"
-msgstr "Dòlar de les Illes Salomó"
+msgstr "Dólar salomonense"
 
 msgid "Som"
 msgstr "Som"
 
 msgid "Somali Shilling"
-msgstr "Xíling somali"
+msgstr "Chelín somalí"
 
 msgid "Somoni"
 msgstr "Somoni"
 
 msgid "South Sudanese Pound"
-msgstr "Lliura sud-sudanesa"
+msgstr "Libra sursudanesa"
 
 msgid "Sri Lanka Rupee"
-msgstr "Rupia de Sri Lanka"
+msgstr "Rupia esrilanquesa"
 
 msgid "Sucre"
 msgstr "Sucre"
 
 msgid "Sudanese Pound"
-msgstr "Lliura sudanesa"
+msgstr "Libra sudanesa"
 
 msgid "Surinam Dollar"
-msgstr "Dòlar de Singapur"
+msgstr "Dólar surinamés"
 
 msgid "Swedish Krona"
 msgstr "Corona sueca"
 
 msgid "Swiss Franc"
-msgstr "Franc suís"
+msgstr "Franco suizo"
 
 msgid "Syrian Pound"
-msgstr "Lliura siriana"
+msgstr "Libra siria"
 
 msgid "Taka"
 msgstr "Taka"
 
 msgid "Tala"
 msgstr "Tala"
 
 msgid "Tanzanian Shilling"
-msgstr "Xíling tanzà"
+msgstr "Chelín tanzano"
 
 msgid "Tenge"
 msgstr "Tenge"
 
 msgid "The codes assigned for transactions where no currency is involved"
-msgstr "Els codis assignats per a transaccions on no hi ha moneda involucrada"
+msgstr ""
+"Los códigos asignados para transacciones donde no hay moneda involucrada"
 
 msgid "Trinidad and Tobago Dollar"
-msgstr "Dòlar de Trinitat i Tobago"
+msgstr "Dólar trinitense"
 
 msgid "Tugrik"
 msgstr "Tugrik"
 
 msgid "Tunisian Dinar"
-msgstr "Dinar tunisià"
+msgstr "Dinar tunecino"
 
 msgid "Turkish Lira"
 msgstr "Lira turca"
 
 msgid "Turkmenistan New Manat"
-msgstr "Manat turcman"
+msgstr "Nuevo manat turcomano"
 
 msgid "UAE Dirham"
-msgstr "Dírham dels EAU"
+msgstr "Dírham emiratí"
 
 msgid "US Dollar"
-msgstr "Dòlar dels Estats Units"
+msgstr "Dólar estadounidense"
 
 msgid "Uganda Shilling"
-msgstr "Xíling ugandès"
+msgstr "Chelín ugandés"
 
 msgid "Uzbekistan Sum"
-msgstr "Som d'Uzbekistan"
+msgstr "Som uzbeco"
 
 msgid "Vatu"
 msgstr "Vatu"
 
 msgid "Won"
-msgstr "Won"
+msgstr "Won surcoreano"
 
 msgid "Yemeni Rial"
-msgstr "Rial iemenita"
+msgstr "Rial yemení"
 
 msgid "Yen"
-msgstr "Ien"
+msgstr "Yen"
 
 msgid "Yuan Renminbi"
-msgstr "Iuan renminbi"
+msgstr "Yuan renminbi"
 
 msgid "Zambian Kwacha"
-msgstr "Kwacha zambià"
+msgstr "Kwacha zambiano"
 
 msgid "Zimbabwe Dollar"
-msgstr "Dòlar de Zimbàbue"
+msgstr "Dólar zimbabuense"
 
 msgid "Zloty"
 msgstr "Zloty"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,29 +1,32 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_15924\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2019-03-03 09:18+0000\n"
-"Last-Translator: Lorem Ipsum <aditoo@seznam.cz>\n"
+"PO-Revision-Date: 2023-03-21 13:41+0000\n"
+"Last-Translator: Miroslav Kure <kurem@upcase.inf.upol.cz>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/iso-codes/"
 "iso-15924/cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 3.5-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "Afaka"
 msgstr "Afaka"
 
 msgid "Arabic"
 msgstr "Arabské"
 
+msgid "Arabic (Nastaliq variant)"
+msgstr "Arabské (varianta nastaliq)"
+
 msgid "Armenian"
 msgstr "Arménské"
 
 msgid "Avestan"
 msgstr "Avestické"
 
 msgid "Balinese"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-12-10 18:48+0000\n"
+"PO-Revision-Date: 2023-03-21 13:41+0000\n"
 "Last-Translator: Miroslav Kure <kurem@upcase.inf.upol.cz>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n>1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "Afghanistan"
 msgstr "Afghánistán"
 
 msgid "Albania"
 msgstr "Albánie"
 
@@ -409,14 +409,17 @@
 
 msgid "India"
 msgstr "Indie"
 
 msgid "Indonesia"
 msgstr "Indonésie"
 
+msgid "Iran"
+msgstr "Írán"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Írán, islámská republika"
 
 msgid "Iraq"
 msgstr "Irák"
 
 msgid "Ireland"
@@ -526,14 +529,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Kyrgyzstán"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Laoská lidově demokratická republika"
 
+msgid "Laos"
+msgstr "Laos"
+
 msgid "Latvia"
 msgstr "Lotyšsko"
 
 msgid "Lebanese Republic"
 msgstr "Libanonská republika"
 
 msgid "Lebanon"
@@ -1135,14 +1141,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Švýcarská konfederace"
 
 msgid "Switzerland"
 msgstr "Švýcarsko"
 
+msgid "Syria"
+msgstr "Sýrie"
+
 msgid "Syrian Arab Republic"
 msgstr "Syrská arabská republika"
 
 msgid "Taiwan"
 msgstr "Tchaj-wan"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2014-01-28 20:08+0100\n"
-"Last-Translator: Miroslav Kure <kurem@debian.cz>\n"
-"Language-Team: Czech <debian-l10n-czech@lists.debian.org>\n"
+"PO-Revision-Date: 2023-03-21 13:41+0000\n"
+"Last-Translator: Miroslav Kure <kurem@upcase.inf.upol.cz>\n"
+"Language-Team: Czech <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-3/cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: KBabel 1.3.1\n"
 "Plural-Forms: nplurals=2; plural=n>1;\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "British Antarctic Territory"
 msgstr "Britské teritorium v Antarktidě"
 
 msgid "Burma, Socialist Republic of the Union of"
 msgstr "Barma, socialistická republika svazu"
 
@@ -96,9 +97,12 @@
 
 msgid "Wake Island"
 msgstr "Ostrov Wake"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
 msgstr "Jemen, lidově demokratická republika"
 
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Jugoslávie, (socialistická) federativní republika"
+
 msgid "Zaire, Republic of"
 msgstr "Zair, republika"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,50 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2019-04-19 13:34+0000\n"
-"Last-Translator: Aled Powell <aled@aledpowell.cymru>\n"
+"PO-Revision-Date: 2023-04-23 17:51+0000\n"
+"Last-Translator: dreigiau <sterilgrimed23@gmail.com>\n"
 "Language-Team: Welsh <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/cy/>\n"
 "Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=(n==0) ? 0 : (n==1) ? 1 : (n==2) ? 2 : "
 "(n==3) ? 3 :(n==6) ? 4 : 5;\n"
-"X-Generator: Weblate 3.6-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid "Afghanistan"
 msgstr "Afghanistan"
 
 msgid "Albania"
 msgstr "Albania"
 
 msgid "Algeria"
 msgstr "Algeria"
 
 msgid "American Samoa"
-msgstr "American Samoa"
+msgstr "Samoa America"
 
 msgid "Andorra"
 msgstr "Andorra"
 
 msgid "Angola"
 msgstr "Angola"
 
 msgid "Anguilla"
 msgstr "Anguilla"
 
 msgid "Antarctica"
 msgstr "Antarctica"
 
 msgid "Antigua and Barbuda"
-msgstr "Antigua ac Barbuda"
+msgstr "Antigua a Barbuda"
 
 msgid "Arab Republic of Egypt"
 msgstr "Gweriniaeth Arabaidd yr Aifft"
 
 msgid "Argentina"
 msgstr "Yr Ariannin"
 
@@ -105,63 +105,63 @@
 msgid "Bolivia, Plurinational State of"
 msgstr "Bolifia, Gwladwriaeth Amlgenedlaethol"
 
 msgid "Bonaire, Sint Eustatius and Saba"
 msgstr "Bonaire, Sint Eustatius a Saba"
 
 msgid "Bosnia and Herzegovina"
-msgstr "Bosnia a Herzegovina"
+msgstr "Bosnia a Hercegovina"
 
 msgid "Botswana"
 msgstr "Botswana"
 
 msgid "Bouvet Island"
 msgstr "Ynys Bouvet"
 
 msgid "Brazil"
 msgstr "Brasil"
 
 msgid "British Indian Ocean Territory"
-msgstr "British Indian Ocean Territory"
+msgstr "Tiriogaeth Brydeinig Cefnfor India"
 
 msgid "British Virgin Islands"
-msgstr "Ynysoedd Virgin Prydain"
+msgstr "Ynysoedd Prydeinig y Wyryf"
 
 msgid "Brunei Darussalam"
 msgstr "Brunei Darussalam"
 
 msgid "Bulgaria"
 msgstr "Bwlgaria"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
 msgid "Burundi"
-msgstr "Burundi"
+msgstr "Bwrwndi"
 
 msgid "Cabo Verde"
 msgstr "Penrhyn Verde"
 
 msgid "Cambodia"
 msgstr "Cambodia"
 
 msgid "Cameroon"
-msgstr "Cameroon"
+msgstr "Camerŵn"
 
 msgid "Canada"
 msgstr "Canada"
 
 msgid "Cayman Islands"
-msgstr "Ynysoedd y Cayman"
+msgstr "Ynysoedd Cayman"
 
 msgid "Central African Republic"
-msgstr "Gweriniaeth Canol Affrica"
+msgstr "Gweriniaeth Canolbarth Affrica"
 
 msgid "Chad"
-msgstr "Chad"
+msgstr "Tchad"
 
 msgid "Chile"
 msgstr "Chile"
 
 msgid "China"
 msgstr "Tsieina"
 
@@ -207,15 +207,15 @@
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
 msgstr "Cyprus"
 
 msgid "Czech Republic"
-msgstr "Y Weriniaeth Tsiec"
+msgstr "Gweriniaeth Tsiec"
 
 msgid "Czechia"
 msgstr "Tsiecia"
 
 msgid "Côte d'Ivoire"
 msgstr "Côte d'Ivoire"
 
@@ -252,15 +252,15 @@
 msgid "Egypt"
 msgstr "Yr Aifft"
 
 msgid "El Salvador"
 msgstr "El Salvador"
 
 msgid "Equatorial Guinea"
-msgstr "Guinea Cyhydeddol"
+msgstr "Guinea Gyhydeddol"
 
 msgid "Eritrea"
 msgstr "Eritrea"
 
 msgid "Estonia"
 msgstr "Estonia"
 
@@ -270,15 +270,15 @@
 msgid "Ethiopia"
 msgstr "Ethiopia"
 
 msgid "Falkland Islands (Malvinas)"
 msgstr "Ynysoedd y Falklands (Malvinas)"
 
 msgid "Faroe Islands"
-msgstr "Ynysoedd y Ffaro"
+msgstr "Ynysoedd Ffaro"
 
 msgid "Federal Democratic Republic of Ethiopia"
 msgstr "Gweriniaeth Democratic Ffederal Ethiopia"
 
 msgid "Federal Democratic Republic of Nepal"
 msgstr "Gweriniaeth Ddemocrataidd Ffederal Nepal"
 
@@ -306,15 +306,15 @@
 msgid "France"
 msgstr "Ffrainc"
 
 msgid "French Guiana"
 msgstr "Guiana Ffrangeg"
 
 msgid "French Polynesia"
-msgstr "Polynesia Ffrangeg"
+msgstr "Polynesia Ffrengig"
 
 msgid "French Republic"
 msgstr "Gweriniaeth Ffrainc"
 
 msgid "French Southern Territories"
 msgstr "French Southern Territories"
 
@@ -342,30 +342,30 @@
 msgid "Grand Duchy of Luxembourg"
 msgstr "Archddugiaeth Lwcsembwrg"
 
 msgid "Greece"
 msgstr "Groeg"
 
 msgid "Greenland"
-msgstr "Greenland"
+msgstr "Yr Ynys Las"
 
 msgid "Grenada"
 msgstr "Grenada"
 
 msgid "Guadeloupe"
 msgstr "Guadeloupe"
 
 msgid "Guam"
 msgstr "Guam"
 
 msgid "Guatemala"
 msgstr "Gwatemala"
 
 msgid "Guernsey"
-msgstr "Guernsey"
+msgstr "Ynys y Garn"
 
 msgid "Guinea"
 msgstr "Guinea"
 
 msgid "Guinea-Bissau"
 msgstr "Guinea-Bissau"
 
@@ -375,15 +375,15 @@
 msgid "Haiti"
 msgstr "Haiti"
 
 msgid "Hashemite Kingdom of Jordan"
 msgstr "Gweriniaeth Hashemeit yr Iorddonen"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Ynys Heard ac Ynysoedd McDonald"
+msgstr "Ynysoedd Heard a McDonald"
 
 msgid "Hellenic Republic"
 msgstr "Gweriniaeth Groeg"
 
 msgid "Holy See (Vatican City State)"
 msgstr "Yr Esgobaeth Sanctaidd (Talaith Dinas y Fatican)"
 
@@ -410,14 +410,17 @@
 
 msgid "India"
 msgstr "India"
 
 msgid "Indonesia"
 msgstr "Indonesia"
 
+msgid "Iran"
+msgstr "Iran"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Iran, Gweriniaeth Islamaidd"
 
 msgid "Iraq"
 msgstr "Irac"
 
 msgid "Ireland"
@@ -453,18 +456,18 @@
 msgid "Japan"
 msgstr "Japan"
 
 msgid "Jersey"
 msgstr "Jersey"
 
 msgid "Jordan"
-msgstr "Gwlad Yr Iorddonen"
+msgstr "Gwlad Iorddonen"
 
 msgid "Kazakhstan"
-msgstr "Kazakhstan"
+msgstr "Kazakstan"
 
 msgid "Kenya"
 msgstr "Kenya"
 
 msgid "Kingdom of Bahrain"
 msgstr "Teyrnas Bahrain"
 
@@ -527,22 +530,25 @@
 
 msgid "Kyrgyzstan"
 msgstr "Kyrgyzstan"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Gweriniaeth Ddemocrataidd y Bobl Lao"
 
+msgid "Laos"
+msgstr "Laos"
+
 msgid "Latvia"
 msgstr "Latfia"
 
 msgid "Lebanese Republic"
 msgstr "Gweriniaeth Lebanon"
 
 msgid "Lebanon"
-msgstr "Lebanon"
+msgstr "Libanus"
 
 msgid "Lesotho"
 msgstr "Lesotho"
 
 msgid "Liberia"
 msgstr "Liberia"
 
@@ -621,15 +627,15 @@
 msgid "Montserrat"
 msgstr "Montserrat"
 
 msgid "Morocco"
 msgstr "Moroco"
 
 msgid "Mozambique"
-msgstr "Mozambique"
+msgstr "Mosambic"
 
 msgid "Myanmar"
 msgstr "Myanmar"
 
 msgid "Namibia"
 msgstr "Namibia"
 
@@ -659,19 +665,22 @@
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
 msgstr "Ynys Norfolk"
 
+msgid "North Korea"
+msgstr "Gogledd Corea"
+
 msgid "North Macedonia"
 msgstr "Gogledd Macedonia"
 
 msgid "Northern Mariana Islands"
-msgstr "Ynysoedd Northern Mariana"
+msgstr "Ynysoedd Gogledd Mariana"
 
 msgid "Norway"
 msgstr "Norwy"
 
 msgid "Oman"
 msgstr "Oman"
 
@@ -696,21 +705,21 @@
 msgid "People's Democratic Republic of Algeria"
 msgstr "Gweriniaeth Democratic Pobl Algeria"
 
 msgid "People's Republic of Bangladesh"
 msgstr "Gweriniaeth Pobl Bangladesh"
 
 msgid "People's Republic of China"
-msgstr "Gweriniaeth Pobl Tseina"
+msgstr "Gweriniaeth Pobl Tsieina"
 
 msgid "Peru"
 msgstr "Periw"
 
 msgid "Philippines"
-msgstr "Pilipinas"
+msgstr "Y Philipinau"
 
 msgid "Pitcairn"
 msgstr "Pitcairn"
 
 msgid "Plurinational State of Bolivia"
 msgstr "Gwladwriaeth Amlgenedlaethol Bolifia"
 
@@ -962,14 +971,17 @@
 
 msgid "Republic of Trinidad and Tobago"
 msgstr "Gweriniaeth Trinidad a Tobago"
 
 msgid "Republic of Tunisia"
 msgstr "Gweriniaeth Twnisia"
 
+msgid "Republic of Türkiye"
+msgstr "Gweriniaeth Twrci"
+
 msgid "Republic of Uganda"
 msgstr "Gweriniaeth Uganda"
 
 msgid "Republic of Uzbekistan"
 msgstr "Gweriniaeth Wsbecistan"
 
 msgid "Republic of Vanuatu"
@@ -1086,15 +1098,18 @@
 msgid "Somalia"
 msgstr "Somalia"
 
 msgid "South Africa"
 msgstr "De Affrica"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "De Georgia ac Ynysoedd De Sandwich"
+msgstr "De Georgia ac Ynysoedd Sandwich y De"
+
+msgid "South Korea"
+msgstr "De Corea"
 
 msgid "South Sudan"
 msgstr "De Swdan"
 
 msgid "Spain"
 msgstr "Sbaen"
 
@@ -1127,14 +1142,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Y Conffederasiwn Swisaidd"
 
 msgid "Switzerland"
 msgstr "Y Swistir"
 
+msgid "Syria"
+msgstr "Syria"
+
 msgid "Syrian Arab Republic"
 msgstr "Gweriniaeth Arabaidd Syria"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan, Province of China"
@@ -1173,30 +1191,33 @@
 msgid "Tunisia"
 msgstr "Twnisia"
 
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
-msgstr "Ynysoedd y Turks a Caicos"
+msgstr "Ynysoedd Turks a Caicos"
 
 msgid "Tuvalu"
-msgstr "Tuvalu"
+msgstr "Twfalw"
+
+msgid "Türkiye"
+msgstr "Twrci"
 
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Wcrain"
 
 msgid "Union of the Comoros"
 msgstr "Undeb y Comoros"
 
 msgid "United Arab Emirates"
-msgstr "Emiriaethau Arabaidd Unedig"
+msgstr "Yr Emiradau Arabaidd Unedig"
 
 msgid "United Kingdom"
 msgstr "Y Deyrnas Unedig"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
 msgstr "Teyrnas Unedig Prydain Fawr a Gogledd Iwerddon"
 
@@ -1206,30 +1227,30 @@
 msgid "United Republic of Tanzania"
 msgstr "Gweriniaeth Unedig Tanzania"
 
 msgid "United States"
 msgstr "Yr Unol Daleithiau"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Mân Ynysoedd Pellenig yr Unol Daleithiau"
+msgstr "Ynysoedd Pellennig Bychain yr Unol Daleithiau"
 
 msgid "United States of America"
 msgstr "Unol Daleithiau America"
 
 msgid "Uruguay"
 msgstr "Uruguay"
 
 msgid "Uzbekistan"
 msgstr "Wsbecistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
-msgstr "Venezuela"
+msgstr "Feneswela"
 
 msgid "Venezuela, Bolivarian Republic of"
 msgstr "Venezuela, Gweriniaeth Bolifaraidd"
 
 msgid "Viet Nam"
 msgstr "Fietnam"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2013-03-04 10:54-0000\n"
-"Last-Translator: Dafydd Tomos <l10n@da.fydd.org>\n"
-"Language-Team: Welsh\n"
+"PO-Revision-Date: 2023-04-15 14:50+0000\n"
+"Last-Translator: dreigiau <sterilgrimed23@gmail.com>\n"
+"Language-Team: Welsh <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-3/cy/>\n"
 "Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 1.5.4\n"
+"Plural-Forms: nplurals=6; plural=(n==0) ? 0 : (n==1) ? 1 : (n==2) ? 2 : "
+"(n==3) ? 3 :(n==6) ? 4 : 5;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "British Antarctic Territory"
 msgstr "Tiriogaeth Antarctig Prydain"
 
 msgid "Burma, Socialist Republic of the Union of"
 msgstr "Burma, Gweriniaeth Sosialaidd Undeb"
 
@@ -95,9 +98,12 @@
 
 msgid "Wake Island"
 msgstr "Ynys Wake"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
 msgstr "Yemen, Democrataidd, Gweriniaeth Democrataidd Pobl"
 
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Iwgoslafia, Gweriniaeth Ffederal (Sosialaidd)"
+
 msgid "Zaire, Republic of"
 msgstr "Zaire, Gweriniaeth"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/cy/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,361 +1,414 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: iso_639-2\n"
+"Project-Id-Version: iso_639-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2018-03-19 21:51+0000\n"
-"Last-Translator: Huw Waters <huwwaters@gmail.com>\n"
-"Language-Team: Welsh <https://hosted.weblate.org/projects/iso-codes/"
-"iso-639-2/cy/>\n"
-"Language: cy\n"
+"PO-Revision-Date: 2018-09-19 06:30+0000\n"
+"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
+"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/iso-"
+"codes/iso-639-3/nb/>\n"
+"Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=(n==0) ? 0 : (n==1) ? 1 : (n==2) ? 2 : "
-"(n==3) ? 3 :(n==6) ? 4 : 5;\n"
-"X-Generator: Weblate 2.20-dev\n"
-
-msgid "Abkhazian"
-msgstr "Abchaseg"
-
-msgid "Achinese"
-msgstr "Atsienëeg"
-
-msgid "Acoli"
-msgstr "Acholeg"
-
-msgid "Adangme"
-msgstr "Adangmëeg"
-
-msgid "Adyghe; Adygei"
-msgstr "Adygëeg"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 3.2-dev\n"
 
 msgid "Afar"
-msgstr "Affareg"
+msgstr "afar"
 
 msgid "Afrikaans"
-msgstr "Affricaneg"
-
-msgid "Albanian"
-msgstr "Albaneg"
-
-msgid "Amharic"
-msgstr "Amhareg"
+msgstr "Afrikansk"
 
 msgid "Arabic"
-msgstr "Arabeg"
+msgstr "Arabisk"
+
+msgid "Aragonese"
+msgstr "aragonsk"
 
 msgid "Armenian"
-msgstr "Armeneg"
+msgstr "armensk"
 
 msgid "Assamese"
-msgstr "Asameg"
+msgstr "assamisk"
+
+msgid "Avestan"
+msgstr "avestisk"
 
 msgid "Aymara"
-msgstr "Aimareg"
+msgstr "aymara"
 
 msgid "Azerbaijani"
-msgstr "Aserbaijani"
+msgstr "Aserbadjansk"
+
+msgid "Balinese"
+msgstr "balinesisk"
+
+msgid "Bambara"
+msgstr "bambara"
+
+msgid "Bashkir"
+msgstr "basjkirsk"
 
 msgid "Basque"
-msgstr "Basgeg"
+msgstr "Baskisk"
 
-msgid "Belarusian"
-msgstr "Belarwseg"
+msgid "Batak"
+msgstr "batak"
 
 msgid "Bengali"
-msgstr "Bengaleg"
+msgstr "bengali"
 
 msgid "Bislama"
-msgstr "Bislama"
+msgstr "bislama"
+
+msgid "Blissymbols"
+msgstr "blissymbol"
 
 msgid "Breton"
-msgstr "Llydaweg"
+msgstr "Breton"
+
+msgid "Buginese"
+msgstr "buginesisk"
+
+msgid "Buhid"
+msgstr "buhid"
 
 msgid "Bulgarian"
-msgstr "Bwlgareg"
+msgstr "Bulgarsk"
 
 msgid "Burmese"
-msgstr "Byrmaneg"
+msgstr "burmesisk"
 
-msgid "Chinese"
-msgstr "Tsieinëeg"
+msgid "Catalan"
+msgstr "Katalan"
+
+msgid "Chamorro"
+msgstr "chamorro"
+
+msgid "Cherokee"
+msgstr "cherokee"
 
-msgid "Cornish"
-msgstr "Cernyweg"
+msgid "Chinese"
+msgstr "Kinesisk"
 
-msgid "Corsican"
-msgstr "Corseg"
+msgid "Chuvash"
+msgstr "tsjuvansk"
 
 msgid "Croatian"
-msgstr "Croateg"
+msgstr "Kroatsisk"
 
 msgid "Czech"
-msgstr "Tsieceg"
+msgstr "Tjekkisk"
 
 msgid "Danish"
-msgstr "Daneg"
+msgstr "Dansk"
+
+msgid "Dong"
+msgstr "Vietnamesiske dồng"
+
+msgid "Dutch"
+msgstr "Nederlandsk"
 
-msgid "English"
-msgstr "Saesneg"
+msgid "Dzongkha"
+msgstr "dzongkha"
 
 msgid "Esperanto"
 msgstr "Esperanto"
 
 msgid "Estonian"
-msgstr "Estoneg"
+msgstr "Estonsk"
+
+msgid "Ewe"
+msgstr "ewe"
 
 msgid "Faroese"
-msgstr "Ffaröeg"
+msgstr "færøysk"
 
 msgid "Fijian"
-msgstr "Ffijïeg"
+msgstr "fijiansk"
 
 msgid "Finnish"
-msgstr "Ffinneg"
+msgstr "Finsk"
 
 msgid "French"
-msgstr "Ffrangeg"
+msgstr "Fransk"
 
-msgid "Galician"
-msgstr "Galiseg"
+msgid "Fulah"
+msgstr "fulani"
 
-msgid "Georgian"
-msgstr "Georgeg"
+msgid "Ganda"
+msgstr "ganda"
 
 msgid "German"
-msgstr "Almaeneg"
-
-msgid "Guarani"
-msgstr "Gwarani"
+msgstr "Tysk"
 
 msgid "Gujarati"
-msgstr "Gwjwrati"
+msgstr "gujarati"
 
-msgid "Hausa"
-msgstr "Hawsa"
+msgid "Hawaiian"
+msgstr "hawaiisk"
 
 msgid "Hebrew"
-msgstr "Hebraeg"
+msgstr "Hebraisk"
 
 msgid "Hindi"
-msgstr "Hindi"
+msgstr "hindi"
 
 msgid "Hungarian"
-msgstr "Hwngareg"
+msgstr "Ungarsk"
 
 msgid "Icelandic"
-msgstr "Islandeg"
+msgstr "Islandsk"
+
+msgid "Ido"
+msgstr "ido"
 
-msgid "Indonesian"
-msgstr "Indoneseg"
+msgid "Igbo"
+msgstr "ibo"
+
+msgid "Interlingue"
+msgstr "interlingue"
 
 msgid "Inuktitut"
-msgstr "Inwctitwt"
+msgstr "inuktitut"
 
 msgid "Inupiaq"
-msgstr "Inwpiac"
+msgstr "unupiak"
 
 msgid "Irish"
-msgstr "Gwyddeleg"
+msgstr "Irsk"
 
 msgid "Italian"
-msgstr "Eidaleg"
+msgstr "Italiensk"
 
 msgid "Japanese"
-msgstr "Siapaneg"
-
-msgid "Javanese"
-msgstr "Jafaneg"
+msgstr "Japansk"
 
 msgid "Kannada"
-msgstr "Canareg"
+msgstr "kannada"
 
 msgid "Kashmiri"
-msgstr "Cashmireg"
+msgstr "kasjmiri"
 
 msgid "Kazakh"
-msgstr "Cazacheg"
+msgstr "kasakhisk"
+
+msgid "Kikuyu"
+msgstr "kikuyu"
 
 msgid "Kinyarwanda"
-msgstr "Ciniarwanda"
+msgstr "kinjarwanda"
+
+msgid "Kirghiz"
+msgstr "kirgisisk"
+
+msgid "Komi"
+msgstr "komi"
+
+msgid "Kongo"
+msgstr "kikongo"
 
 msgid "Korean"
-msgstr "Corëeg"
+msgstr "Koreansk"
 
-msgid "Kurdish"
-msgstr "Cwrdeg"
+msgid "Kuanyama"
+msgstr "kuanyama"
 
 msgid "Lao"
-msgstr "Laoeg"
+msgstr "laotisk"
 
-msgid "Latin"
-msgstr "Lladin"
+msgid "Lari"
+msgstr "Georgiske lari"
 
 msgid "Latvian"
-msgstr "Latfieg"
+msgstr "Latvisk"
 
 msgid "Lingala"
-msgstr "Lingala"
+msgstr "lingala"
 
 msgid "Lithuanian"
-msgstr "Lithwaneg"
+msgstr "Lituaisk"
+
+msgid "Luba-Katanga"
+msgstr "luba-katanga"
 
 msgid "Macedonian"
-msgstr "Macedoneg"
+msgstr "Makedonsk"
 
 msgid "Malagasy"
-msgstr "Malagasi"
-
-msgid "Malay"
-msgstr "Malaieg"
+msgstr "madagassisk"
 
 msgid "Malayalam"
-msgstr "Malaialameg"
+msgstr "malayalam"
+
+msgid "Mali"
+msgstr "Mali"
 
 msgid "Maltese"
-msgstr "Malteg"
+msgstr "Maltisk"
 
 msgid "Manx"
-msgstr "Manaweg"
+msgstr "manx"
 
 msgid "Maori"
 msgstr "Maori"
 
-msgid "Marathi"
-msgstr "Marati"
-
-msgid "Mongolian"
-msgstr "Mongoleg"
-
 msgid "Nauru"
-msgstr "Nawrŵeg"
+msgstr "nauru"
 
-msgid "Nepali"
-msgstr "Nepaleg"
+msgid "Ndebele, North"
+msgstr "ndebele (nord)"
 
-msgid "Norwegian"
-msgstr "Norwyeg"
+msgid "Ndebele, South"
+msgstr "ndebele, sør"
 
-msgid "Oriya"
-msgstr "Orïa"
+msgid "Ojibwa"
+msgstr "ojibwa"
 
 msgid "Oromo"
-msgstr "Oromo"
+msgstr "oromo"
 
 msgid "Polish"
-msgstr "Pwyleg"
+msgstr "Polsk"
 
 msgid "Portuguese"
-msgstr "Portiwgaleg"
+msgstr "Portugisisk"
 
 msgid "Quechua"
-msgstr "Cetshwa"
+msgstr "quechua"
+
+msgid "Romanian"
+msgstr "Rumensk"
 
 msgid "Rundi"
-msgstr "Rwndi"
+msgstr "rundi"
 
 msgid "Russian"
-msgstr "Rwsieg"
+msgstr "Russisk"
 
 msgid "Samoan"
-msgstr "Samöeg"
+msgstr "samoansk"
 
 msgid "Sango"
-msgstr "Sango"
+msgstr "sango"
 
 msgid "Sanskrit"
-msgstr "Sansgrit"
+msgstr "sanskrit"
 
 msgid "Serbian"
-msgstr "Serbeg"
+msgstr "Serbisk"
 
-msgid "Shona"
-msgstr "Shona"
+msgid "Sidamo"
+msgstr "sidamo"
 
 msgid "Sindhi"
-msgstr "Sindhi"
+msgstr "sindhi"
 
 msgid "Slovak"
-msgstr "Slofaceg"
+msgstr "Slovakisk"
 
 msgid "Slovenian"
-msgstr "Slofeneg"
+msgstr "Slovensk"
 
 msgid "Somali"
-msgstr "Somalieg"
+msgstr "somalisk"
 
-msgid "Sundanese"
-msgstr "Swndaneg"
+msgid "Sotho, Southern"
+msgstr "Sotho, (sørlig)"
+
+msgid "Southern Sotho"
+msgstr "Sørsotho"
+
+msgid "Spanish"
+msgstr "Spansk"
 
-msgid "Swahili"
-msgstr "Swahili"
+msgid "Sundanese"
+msgstr "sundanesisk"
 
 msgid "Swati"
-msgstr "Swati"
+msgstr "swati"
 
 msgid "Swedish"
-msgstr "Swedeg"
+msgstr "Svensk"
 
 msgid "Tagalog"
-msgstr "Tagalog"
+msgstr "tagalog"
 
-msgid "Tajik"
-msgstr "Tajiceg"
+msgid "Tala"
+msgstr "Samoanske tala"
 
 msgid "Tamil"
-msgstr "Tamileg"
+msgstr "Tamilsk"
 
 msgid "Tatar"
-msgstr "Tatareg"
+msgstr "tatarisk"
 
 msgid "Telugu"
-msgstr "Telwgw"
+msgstr "telugu"
 
 msgid "Thai"
-msgstr "Tai"
+msgstr "Thai"
 
 msgid "Tibetan"
-msgstr "Tibeteg"
+msgstr "tibetansk"
+
+msgid "Tokelau"
+msgstr "Tokelau"
+
+msgid "Tonga (Tonga Islands)"
+msgstr "tonga (Tonga-øyene)"
 
 msgid "Tsonga"
-msgstr "Tsongeg"
+msgstr "tsonga"
 
 msgid "Tswana"
-msgstr "Tswana"
+msgstr "tswana"
 
 msgid "Turkish"
-msgstr "Tyrceg"
+msgstr "Tyrkisk"
 
 msgid "Turkmen"
-msgstr "Tyrcmeneg"
+msgstr "turkmensk"
+
+msgid "Tuvalu"
+msgstr "Tuvalu"
 
 msgid "Twi"
-msgstr "Twi"
+msgstr "twi"
+
+msgid "Uighur"
+msgstr "uigurisk"
 
 msgid "Urdu"
-msgstr "Wrdw"
+msgstr "urdu"
 
 msgid "Uzbek"
-msgstr "Wsbeceg"
+msgstr "usbekisk"
+
+msgid "Vai"
+msgstr "vai"
+
+msgid "Venda"
+msgstr "venda"
 
 msgid "Vietnamese"
-msgstr "Fietnameg"
+msgstr "Vietnamesisk"
+
+msgid "Walloon"
+msgstr "Vietnamesisk"
 
 msgid "Welsh"
-msgstr "Cymraeg"
+msgstr "Walisisk"
 
 msgid "Wolof"
-msgstr "Woloff"
+msgstr "wolof"
 
 msgid "Xhosa"
 msgstr "Xhosa"
 
 msgid "Yiddish"
-msgstr "Iddew-Almaeneg"
+msgstr "jiddisk"
 
 msgid "Yoruba"
-msgstr "Iorwba"
-
-msgid "Zulu"
-msgstr "Zwlw"
+msgstr "joruba"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_639-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2023-02-24 21:01+0000\n"
-"Last-Translator: \"Dr. Tobias Quathamer\" <toddy@debian.org>\n"
+"PO-Revision-Date: 2023-04-24 20:51+0000\n"
+"Last-Translator: Ettore Atalan <atalanttore@googlemail.com>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/iso-codes/"
 "iso-639-3/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid "'Are'are"
 msgstr "'Are'are"
 
 msgid "'Auhelawa"
 msgstr "'Auhelawa"
 
@@ -592,14 +592,17 @@
 
 msgid "Aleut, Mednyj"
 msgstr "Alëutisch, Mednyj"
 
 msgid "Algerian Arabic"
 msgstr "Algerisch-Arabisch"
 
+msgid "Algerian Jewish Sign Language"
+msgstr "Algerisch-Jüdische Gebärdensprache"
+
 msgid "Algerian Saharan Arabic"
 msgstr "Algerisches Sahara-Arabisch"
 
 msgid "Algerian Sign Language"
 msgstr "Algerische Gebärdensprache"
 
 msgid "Algonquian, Carolina"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -370,14 +370,17 @@
 
 msgid "Georgia"
 msgstr "Georgia"
 
 msgid "Gipuzkoa"
 msgstr "Guipúzcoa"
 
+msgid "Granada"
+msgstr "Granada"
+
 msgid "Granma"
 msgstr "Granma"
 
 msgid "Guadalajara"
 msgstr "Guadalajara"
 
 msgid "Guadeloupe"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,511 +1,514 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_4217\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2021-05-24 20:32+0000\n"
-"Last-Translator: Adolfo Jayme Barrientos <fitojb@ubuntu.com>\n"
-"Language-Team: Spanish <https://hosted.weblate.org/projects/iso-codes/"
-"iso-4217/es/>\n"
-"Language: es\n"
+"PO-Revision-Date: 2019-04-27 17:48+0000\n"
+"Last-Translator: Rui Mendes <xz9@protonmail.com>\n"
+"Language-Team: Portuguese <https://hosted.weblate.org/projects/iso-codes/"
+"iso-4217/pt/>\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.7-dev\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 3.6.1\n"
 
 msgid "ADB Unit of Account"
-msgstr "Unidad de cuenta del ADB"
+msgstr "Unidade de conta ADB"
 
 msgid "Afghani"
-msgstr "Afganí"
+msgstr "Afegâni"
 
 msgid "Algerian Dinar"
 msgstr "Dinar argelino"
 
 msgid "Argentine Peso"
 msgstr "Peso argentino"
 
 msgid "Armenian Dram"
-msgstr "Dram armenio"
+msgstr "Dram da Arménia"
 
 msgid "Aruban Florin"
-msgstr "Florín arubeño"
+msgstr "Florim arubano"
 
 msgid "Australian Dollar"
 msgstr "Dólar australiano"
 
 msgid "Bahamian Dollar"
-msgstr "Dólar bahameño"
+msgstr "Dólar das Bahamas"
 
 msgid "Bahraini Dinar"
-msgstr "Dinar bareiní"
+msgstr "Dinar baremita"
 
 msgid "Baht"
 msgstr "Baht"
 
 msgid "Balboa"
 msgstr "Balboa"
 
 msgid "Barbados Dollar"
-msgstr "Dólar barbadense"
+msgstr "Dólar dos Barbados"
 
 msgid "Belarusian Ruble"
-msgstr "Rublo bielorruso"
+msgstr "Rublo bielorrusso"
 
 msgid "Belize Dollar"
-msgstr "Dólar beliceño"
+msgstr "Dólar de Belize"
 
 msgid "Bermudian Dollar"
-msgstr "Dólar bermudeño"
+msgstr "Dólar das Bermudas"
 
 msgid "Boliviano"
 msgstr "Boliviano"
 
 msgid "Bond Markets Unit European Composite Unit (EURCO)"
-msgstr "Unidad de Mercados de Bonos Unidad Europea Compuesta (EURCO)"
+msgstr "Unidade Composta Europeia de Mercados de Obrigações (EURCO)"
 
 msgid "Bond Markets Unit European Monetary Unit (E.M.U.-6)"
-msgstr "Unidad de Mercados de Bonos Unidad Monetaria Europea (E.U.M.-6)"
+msgstr ""
+"Unidade Monetária Europeia (E.M.U.-6) (unidade de mercado de obrigações)"
 
 msgid "Bond Markets Unit European Unit of Account 17 (E.U.A.-17)"
-msgstr "Unidad de Mercados de Bonos Unidad de cuenta europea 17 (E.U.A.-17)"
+msgstr ""
+"Unidade Europeia de Conta 17 (E.U.A.-17) (unidade de mercado de obrigações)"
 
 msgid "Bond Markets Unit European Unit of Account 9 (E.U.A.-9)"
-msgstr "Unidad de Mercados de Bonos Unidad de cuenta europea 9 (E.U.A.-9)"
+msgstr ""
+"Unidade Europeia de Conta 9 (E.U.A.-9) (unidade de mercado de obrigações)"
 
 msgid "Brazilian Real"
-msgstr "Real brasileño"
+msgstr "Real brasileiro"
 
 msgid "Brunei Dollar"
-msgstr "Dólar bruneano"
+msgstr "Dólar do Brunei"
 
 msgid "Bulgarian Lev"
 msgstr "Lev búlgaro"
 
 msgid "Burundi Franc"
-msgstr "Franco burundés"
+msgstr "Franco do Burundi"
 
 msgid "CFA Franc BCEAO"
-msgstr "franco CFA BCEAO"
+msgstr "Franco CFA da África Ocidental"
 
 msgid "CFA Franc BEAC"
-msgstr "franco CFA BEAC"
+msgstr "Franco CFA da África Central"
 
 msgid "CFP Franc"
 msgstr "Franco CFP"
 
 msgid "Cabo Verde Escudo"
-msgstr "Escudo caboverdiano"
+msgstr "Escudo cabo-verdiano"
 
 msgid "Canadian Dollar"
-msgstr "Dólar canadiense"
+msgstr "Dólar canadiano"
 
 msgid "Cayman Islands Dollar"
-msgstr "Dólar caimanés"
+msgstr "Dólar das Ilhas Caimão"
 
 msgid "Chilean Peso"
 msgstr "Peso chileno"
 
 msgid "Codes specifically reserved for testing purposes"
-msgstr "Códigos reservados específicamente para pruebas"
+msgstr "Código reservado especificamente para testes"
 
 msgid "Colombian Peso"
 msgstr "Peso colombiano"
 
 msgid "Congolese Franc"
-msgstr "Franco congoleño"
+msgstr "Franco congolês"
 
 msgid "Convertible Mark"
-msgstr "Marco convertible"
+msgstr "Marco conversível"
 
 msgid "Cordoba Oro"
-msgstr "Córdoba"
+msgstr "Córdoba ouro"
 
 msgid "Costa Rican Colon"
-msgstr "Colón costarricense"
+msgstr "Colón costa-riquenho"
 
 msgid "Cuban Peso"
 msgstr "Peso cubano"
 
 msgid "Czech Koruna"
-msgstr "Corona checa"
+msgstr "Coroa checa"
 
 msgid "Dalasi"
 msgstr "Dalasi"
 
 msgid "Danish Krone"
-msgstr "Corona danesa"
+msgstr "Coroa dinamarquesa"
 
 msgid "Denar"
-msgstr "Denar"
+msgstr "Dinar macedónio"
 
 msgid "Djibouti Franc"
-msgstr "Franco yibutiano"
+msgstr "Franco jibutiano"
 
 msgid "Dobra"
 msgstr "Dobra"
 
 msgid "Dominican Peso"
 msgstr "Peso dominicano"
 
 msgid "Dong"
-msgstr "Dong"
+msgstr "Dongue"
 
 msgid "East Caribbean Dollar"
-msgstr "Dólar del Caribe oriental"
+msgstr "Dólar das Caraíbas Orientais"
 
 msgid "Egyptian Pound"
-msgstr "Libra egipcia"
+msgstr "Libra egípcia"
 
 msgid "El Salvador Colon"
-msgstr "Colón salvadoreño"
+msgstr "Colón salvadorenho"
 
 msgid "Ethiopian Birr"
 msgstr "Birr etíope"
 
 msgid "Euro"
 msgstr "Euro"
 
 msgid "Falkland Islands Pound"
-msgstr "Libra malvinense"
+msgstr "Libra das Ilhas Malvinas"
 
 msgid "Fiji Dollar"
-msgstr "Dólar fiyiano"
+msgstr "Dólar fijiano"
 
 msgid "Forint"
-msgstr "Forint húngaro"
+msgstr "Florim húngaro"
 
 msgid "Ghana Cedi"
-msgstr "Cedi ghanés"
+msgstr "Cedi do Gana"
 
 msgid "Gibraltar Pound"
-msgstr "Libra gibraltareña"
+msgstr "Libra de Gibraltar"
 
 msgid "Gold"
-msgstr "Oro"
+msgstr "Ouro"
 
 msgid "Gourde"
-msgstr "Gourde haitiano"
+msgstr "Gurde"
 
 msgid "Guarani"
-msgstr "Guaraní"
+msgstr "Guarani"
 
 msgid "Guyana Dollar"
-msgstr "Dólar guayanés"
+msgstr "Dólar da Guiana"
 
 msgid "Hong Kong Dollar"
-msgstr "Dólar hongkonés"
+msgstr "Dólar de Hong Kong"
 
 msgid "Hryvnia"
-msgstr "Grivnia"
+msgstr "Grívnia"
 
 msgid "Iceland Krona"
-msgstr "Corona islandesa"
+msgstr "Coroa islandesa"
 
 msgid "Indian Rupee"
-msgstr "Rupia india"
+msgstr "Rupia indiana"
 
 msgid "Iranian Rial"
-msgstr "Rial iraní"
+msgstr "Rial iraniano"
 
 msgid "Iraqi Dinar"
-msgstr "Dinar iraquí"
+msgstr "Dinar iraquiano"
 
 msgid "Jamaican Dollar"
-msgstr "Dólar jamaiqueño"
+msgstr "Dólar jamaicano"
 
 msgid "Jordanian Dinar"
 msgstr "Dinar jordano"
 
 msgid "Kenyan Shilling"
-msgstr "Chelín keniata"
+msgstr "Xelim queniano"
 
 msgid "Kina"
-msgstr "Kina"
+msgstr "Quina"
 
 msgid "Kuna"
 msgstr "Kuna"
 
 msgid "Kuwaiti Dinar"
-msgstr "Dinar kuwaití"
+msgstr "Dinar kuwaitiano"
 
 msgid "Kwanza"
 msgstr "Kwanza"
 
 msgid "Kyat"
-msgstr "Kyat"
+msgstr "Quiate"
 
 msgid "Lari"
 msgstr "Lari"
 
 msgid "Lebanese Pound"
 msgstr "Libra libanesa"
 
 msgid "Lek"
-msgstr "Lek"
+msgstr "Leque da Albânia"
 
 msgid "Lempira"
 msgstr "Lempira"
 
 msgid "Leone"
 msgstr "Leone"
 
 msgid "Liberian Dollar"
 msgstr "Dólar liberiano"
 
 msgid "Libyan Dinar"
-msgstr "Dinar libio"
+msgstr "Dinar líbio"
 
 msgid "Lilangeni"
-msgstr "Lilangeni suazi"
+msgstr "Lilanguéni suázi"
 
 msgid "Loti"
 msgstr "Loti"
 
 msgid "Malagasy Ariary"
-msgstr "Ariary malgache"
+msgstr "Ariari malgaxe"
 
 msgid "Malawi Kwacha"
-msgstr "Kwacha malauí"
+msgstr "Kwacha do Maláui"
 
 msgid "Malaysian Ringgit"
-msgstr "Ringgit malasio"
+msgstr "Ringgit malaio"
 
 msgid "Mauritius Rupee"
 msgstr "Rupia mauriciana"
 
 msgid "Mexican Peso"
 msgstr "Peso mexicano"
 
 msgid "Moldovan Leu"
 msgstr "Leu moldavo"
 
 msgid "Moroccan Dirham"
-msgstr "Dírham marroquí"
+msgstr "Dirame marroquino"
 
 msgid "Mozambique Metical"
-msgstr "Metical mozambiqueño"
+msgstr "Metical moçambicano"
 
 msgid "Naira"
 msgstr "Naira"
 
 msgid "Nakfa"
 msgstr "Nakfa"
 
 msgid "Namibia Dollar"
-msgstr "Dólar namibio"
+msgstr "Dólar namibiano"
 
 msgid "Nepalese Rupee"
 msgstr "Rupia nepalesa"
 
 msgid "Netherlands Antillean Guilder"
-msgstr "Florín antillano neerlandés"
+msgstr "Florim das Antilhas Neerlandesas"
 
 msgid "New Israeli Sheqel"
-msgstr "Nuevo séquel israelí"
+msgstr "Novo shekel israelita"
 
 msgid "New Taiwan Dollar"
-msgstr "Nuevo dólar taiwanés"
+msgstr "Novo dólar taiwanês"
 
 msgid "New Zealand Dollar"
-msgstr "Dólar neozelandés"
+msgstr "Dólar neozelandês"
 
 msgid "Ngultrum"
 msgstr "Ngultrum"
 
 msgid "North Korean Won"
-msgstr "Won norcoreano"
+msgstr "Won norte-coreano"
 
 msgid "Norwegian Krone"
-msgstr "Corona noruega"
+msgstr "Coroa norueguesa"
 
 msgid "Ouguiya"
-msgstr "Uquiya"
+msgstr "Uguia"
 
 msgid "Pakistan Rupee"
-msgstr "Rupia pakistaní"
+msgstr "Rupia paquistanesa"
 
 msgid "Palladium"
-msgstr "Paladio"
+msgstr "Paládio"
 
 msgid "Pataca"
-msgstr "Pataca"
+msgstr "Pataca macaense"
 
 msgid "Pa’anga"
-msgstr "Paʻanga"
+msgstr "Paanga"
 
 msgid "Peso Convertible"
-msgstr "Peso convertible"
+msgstr "Peso convertível"
 
 msgid "Peso Uruguayo"
-msgstr "Peso uruguayo"
+msgstr "Peso uruguaio"
 
 msgid "Philippine Peso"
 msgstr "Peso filipino"
 
 msgid "Platinum"
-msgstr "Platino"
+msgstr "Platina"
 
 msgid "Pound Sterling"
 msgstr "Libra esterlina"
 
 msgid "Pula"
 msgstr "Pula"
 
 msgid "Qatari Rial"
-msgstr "Rial catarí"
+msgstr "Rial catariano"
 
 msgid "Quetzal"
 msgstr "Quetzal"
 
 msgid "Rand"
-msgstr "Rand"
+msgstr "Rande"
 
 msgid "Rial Omani"
-msgstr "Rial omaní"
+msgstr "Rial omanense"
 
 msgid "Riel"
-msgstr "Riel camboyano"
+msgstr "Riel"
 
 msgid "Romanian Leu"
-msgstr "Leu rumano"
+msgstr "Leu romeno"
 
 msgid "Rufiyaa"
-msgstr "Rufiyaa"
+msgstr "Rupia maldiva"
 
 msgid "Rupiah"
-msgstr "Rupia indonesia"
+msgstr "Rupia indonésia"
 
 msgid "Russian Ruble"
-msgstr "Rublo ruso"
+msgstr "Rublo russo"
 
 msgid "Rwanda Franc"
-msgstr "Franco ruandés"
+msgstr "Franco ruandês"
 
 msgid "SDR (Special Drawing Right)"
-msgstr "DEG (Derecho especial de giro)"
+msgstr "SDR (direitos especiais de saque)"
 
 msgid "Saint Helena Pound"
-msgstr "Libra santaeleniana"
+msgstr "Libra de Santa Helena"
 
 msgid "Saudi Riyal"
-msgstr "Rial saudí"
+msgstr "Rial saudita"
 
 msgid "Serbian Dinar"
-msgstr "Dinar serbio"
+msgstr "Dinar sérvio"
 
 msgid "Seychelles Rupee"
-msgstr "Rupia seychellense"
+msgstr "Rupia das Seicheles"
 
 msgid "Silver"
-msgstr "Plata"
+msgstr "Prata"
 
 msgid "Singapore Dollar"
-msgstr "Dólar singapurense"
+msgstr "Dólar de Singapura"
 
 msgid "Sol"
-msgstr "Sol"
+msgstr "Novo sol"
 
 msgid "Solomon Islands Dollar"
-msgstr "Dólar salomonense"
+msgstr "Dólar das Ilhas Salomão"
 
 msgid "Som"
 msgstr "Som"
 
 msgid "Somali Shilling"
-msgstr "Chelín somalí"
+msgstr "Xelim somaliano"
 
 msgid "Somoni"
 msgstr "Somoni"
 
 msgid "South Sudanese Pound"
-msgstr "Libra sursudanesa"
+msgstr "Libra sul-sudanesa"
 
 msgid "Sri Lanka Rupee"
-msgstr "Rupia esrilanquesa"
+msgstr "Rupia do Sri Lanka"
 
 msgid "Sucre"
-msgstr "Sucre"
+msgstr "SUCRE"
 
 msgid "Sudanese Pound"
 msgstr "Libra sudanesa"
 
 msgid "Surinam Dollar"
-msgstr "Dólar surinamés"
+msgstr "Dólar do Suriname"
 
 msgid "Swedish Krona"
-msgstr "Corona sueca"
+msgstr "Coroa sueca"
 
 msgid "Swiss Franc"
-msgstr "Franco suizo"
+msgstr "Franco suíço"
 
 msgid "Syrian Pound"
-msgstr "Libra siria"
+msgstr "Libra síria"
 
 msgid "Taka"
 msgstr "Taka"
 
 msgid "Tala"
 msgstr "Tala"
 
 msgid "Tanzanian Shilling"
-msgstr "Chelín tanzano"
+msgstr "Xelim tanzaniano"
 
 msgid "Tenge"
 msgstr "Tenge"
 
 msgid "The codes assigned for transactions where no currency is involved"
 msgstr ""
-"Los códigos asignados para transacciones donde no hay moneda involucrada"
+"Os códigos atribuídos para transações nas quais nenhuma moeda está envolvida"
 
 msgid "Trinidad and Tobago Dollar"
-msgstr "Dólar trinitense"
+msgstr "Dólar de Trindade e Tobago"
 
 msgid "Tugrik"
-msgstr "Tugrik"
+msgstr "Tugrique"
 
 msgid "Tunisian Dinar"
-msgstr "Dinar tunecino"
+msgstr "Dinar tunisino"
 
 msgid "Turkish Lira"
 msgstr "Lira turca"
 
 msgid "Turkmenistan New Manat"
-msgstr "Nuevo manat turcomano"
+msgstr "Manat turcomeno"
 
 msgid "UAE Dirham"
-msgstr "Dírham emiratí"
+msgstr "Dirham dos Emirados Árabes"
 
 msgid "US Dollar"
-msgstr "Dólar estadounidense"
+msgstr "Dólar americano"
 
 msgid "Uganda Shilling"
-msgstr "Chelín ugandés"
+msgstr "Xelim ugandês"
 
 msgid "Uzbekistan Sum"
-msgstr "Som uzbeco"
+msgstr "Som usbeque"
 
 msgid "Vatu"
 msgstr "Vatu"
 
 msgid "Won"
-msgstr "Won surcoreano"
+msgstr "Won sul-coreano"
 
 msgid "Yemeni Rial"
-msgstr "Rial yemení"
+msgstr "Rial iemenita"
 
 msgid "Yen"
-msgstr "Yen"
+msgstr "Iene"
 
 msgid "Yuan Renminbi"
-msgstr "Yuan renminbi"
+msgstr "Renminbi chinês"
 
 msgid "Zambian Kwacha"
 msgstr "Kwacha zambiano"
 
 msgid "Zimbabwe Dollar"
 msgstr "Dólar zimbabuense"
 
 msgid "Zloty"
-msgstr "Zloty"
+msgstr "Zlóti"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_639-2\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2010-10-02 07:52+0200\n"
-"Last-Translator: Fran Diéguez <frandieguez@ubuntu.com>\n"
-"Language-Team: Galician <proxecto@trasno.net>\n"
+"PO-Revision-Date: 2023-03-24 14:39+0000\n"
+"Last-Translator: Juan Comesaña Fernández <xan.comesana@gmail.com>\n"
+"Language-Team: Galician <https://hosted.weblate.org/projects/iso-codes/"
+"iso-639-2/gl/>\n"
 "Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "Abkhazian"
 msgstr "Abxaziano"
 
 msgid "Achinese"
 msgstr "Achinés"
 
@@ -664,15 +666,15 @@
 msgid "Karelian"
 msgstr "Careliano"
 
 msgid "Karen languages"
 msgstr "Idiomas Karen"
 
 msgid "Kashmiri"
-msgstr "Cachemir"
+msgstr "Caxemirés"
 
 msgid "Kashubian"
 msgstr "Caxubio; Casubio"
 
 msgid "Kawi"
 msgstr "Kawi"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-12-10 18:48+0000\n"
+"PO-Revision-Date: 2023-03-03 15:38+0000\n"
 "Last-Translator: Andika Triwidada <andika@gmail.com>\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 "X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albania"
@@ -410,14 +410,17 @@
 
 msgid "India"
 msgstr "India"
 
 msgid "Indonesia"
 msgstr "Indonesia"
 
+msgid "Iran"
+msgstr "Iran"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Iran, Republik Islam"
 
 msgid "Iraq"
 msgstr "Irak"
 
 msgid "Ireland"
@@ -527,14 +530,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Kirgizstan"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Republik Demokrat Rakyat Laos"
 
+msgid "Laos"
+msgstr "Laos"
+
 msgid "Latvia"
 msgstr "Latvia"
 
 msgid "Lebanese Republic"
 msgstr "Republik Libanon"
 
 msgid "Lebanon"
@@ -1136,14 +1142,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Konfederasi Swiss"
 
 msgid "Switzerland"
 msgstr "Swiss"
 
+msgid "Syria"
+msgstr "Suriah"
+
 msgid "Syrian Arab Republic"
 msgstr "Republik Arab Syria"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,105 +1,104 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: iso_3166-3\n"
+"Project-Id-Version: nn\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2018-03-05 19:47+0000\n"
-"Last-Translator: Andika Triwidada <andika@gmail.com>\n"
-"Language-Team: Indonesian <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-3/id/>\n"
-"Language: id\n"
+"PO-Revision-Date: 2013-02-12 13:17+0100\n"
+"Last-Translator: Haavard Korsvoll\n"
+"Language-Team: Norwegian Nynorsk <i18n-nn@lister.ping.uio.no>\n"
+"Language: nn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 2.20-dev\n"
+"X-Generator: Lokalize 1.4\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "British Antarctic Territory"
-msgstr "Wilayah Antartika Inggris"
+msgstr "Britisk antarktis"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Republik Sosialis Persatuan Birma"
+msgstr "Unionen Myanmar"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Republik Sosialis Soviet Belarusia"
+msgstr "Den sovjetiske sosialistiske republikk kviterussland"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Kepulauan Canton dan Enderbury"
+msgstr "Kanton og Endebury øyane"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Republik Sosialis Chekoslovakia"
+msgstr "Tsjekkoslovakia, tsjekkoslovakisk sosialistisk republikk"
 
 msgid "Dahomey"
 msgstr "Dahomey"
 
 msgid "Dronning Maud Land"
-msgstr "Dataran Maud"
+msgstr "Dronning Maud Land"
 
 msgid "East Timor"
-msgstr "Timor Timur"
+msgstr "Aust-Timor"
 
 msgid "France, Metropolitan"
-msgstr "Prancis, Metropolitan"
+msgstr "Metropolitan-Frankrike"
 
 msgid "French Afars and Issas"
-msgstr "Prancis Afars dan Issas"
+msgstr "Fransk Afars og Issas"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Perancis, Wilayah Bagian Selatan dan Antartika"
+msgstr "Franske sørlege og antarktiske territorium"
 
 msgid "German Democratic Republic"
-msgstr "Republik Demokrat Jerman"
+msgstr "Den tyske demokratiske republikken"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Kepulauan Gilbert dan Ellice"
+msgstr "Gilbert og Ellice-øyane"
 
 msgid "Johnston Island"
-msgstr "Kepulauan Johnston"
+msgstr "Johnstonøyane"
 
 msgid "Midway Islands"
-msgstr "Kepulauan Midway"
+msgstr "Midwayøyane"
 
 msgid "Netherlands Antilles"
-msgstr "Antilles Belanda"
+msgstr "Dei nederlandske Antillane"
 
 msgid "Neutral Zone"
-msgstr "Zona Netral"
+msgstr "Nøytral sone"
 
 msgid "New Hebrides"
-msgstr "Hebrida Baru"
+msgstr "Nye hebridane"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Kepulauan Pasifik (Wilayah Kepercayaan)"
+msgstr "Stillehavsøyane (trust territory)"
 
 msgid "Panama Canal Zone"
-msgstr "Zona Terusan Panama"
+msgstr "Panama kanalsone"
 
 msgid "Serbia and Montenegro"
-msgstr "Serbia dan Montenegro"
+msgstr "Serbia og Montenegro"
 
 msgid "Sikkim"
 msgstr "Sikkim"
 
 msgid "Southern Rhodesia"
-msgstr "Rhodesia Selatan"
+msgstr "Sør-Rhodesia"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "Kepualau Pasifik Amerika"
+msgstr "US ymse stillehavsøyar"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "Republik Sosialis Soviet Serikat"
+msgstr "SSSR, Sambandet av Sosialistiske Sovjet-Republikkar"
 
 msgid "Upper Volta, Republic of"
-msgstr "Republik Volta"
+msgstr "Republikken Øvre Volta"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Republik Demokrat Viet-Nam"
+msgstr "Den demokratiske republikken Vietnam"
 
 msgid "Wake Island"
-msgstr "Pulau Wake"
+msgstr "Wake Island"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr "Republik Demokratik Rakyat Yaman"
+msgstr "Den demokratiske folkerepublikken Jemen"
 
 msgid "Zaire, Republic of"
-msgstr "Republik Zaire"
+msgstr "Republikken Zaire"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_639-5\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-12-10 18:48+0000\n"
+"PO-Revision-Date: 2023-03-03 15:38+0000\n"
 "Last-Translator: Andika Triwidada <andika@gmail.com>\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/iso-codes/"
 "iso-639-5/id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "Afro-Asiatic languages"
 msgstr "Bahasa Afro-Asiatik"
 
 msgid "Alacalufan languages"
 msgstr "Bahasa Alacalufan"
 
@@ -178,14 +178,17 @@
 
 msgid "Karen languages"
 msgstr "Bahasa-bahasa Karen"
 
 msgid "Khoisan languages"
 msgstr "Bahasa-bahasa Khoisa"
 
+msgid "Kordofanian languages"
+msgstr "Bahasa-bahasa Kordofania"
+
 msgid "Kru languages"
 msgstr "Bahasa-bahasa Kru"
 
 msgid "Land Dayak languages"
 msgstr "Bahasa Dayak Darat"
 
 msgid "Mande languages"
@@ -220,14 +223,20 @@
 
 msgid "North Germanic languages"
 msgstr "Bahasa Jermanik Utara"
 
 msgid "Nubian languages"
 msgstr "Bahasa-bahasa Nubia"
 
+msgid "Omotic languages"
+msgstr "Bahasa-bahasa Omotik"
+
+msgid "Oto-Manguean languages"
+msgstr "Bahasa-bahasa Oto-Manguea"
+
 msgid "Otomian languages"
 msgstr "Bahasa-bahasa Otomia"
 
 msgid "Papuan languages"
 msgstr "Bahasa-bahasa Papua"
 
 msgid "Philippine languages"
@@ -265,14 +274,17 @@
 
 msgid "South Caucasian languages"
 msgstr "Bahasa Kaukasia Selatan"
 
 msgid "Tai languages"
 msgstr "Bahasa-bahasa Tai"
 
+msgid "Trans-New Guinea languages"
+msgstr "Bahasa-bahasa Trans-Nugini"
+
 msgid "Tupi languages"
 msgstr "Bahasa-bahasa Tupi"
 
 msgid "Uto-Aztecan languages"
 msgstr "Bahasa Uto-Aztec"
 
 msgid "Wakashan languages"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-09-02 09:40+0000\n"
+"PO-Revision-Date: 2023-03-20 09:23+0000\n"
 "Last-Translator: Sveinn í Felli <sv1@fellsnet.is>\n"
 "Language-Team: Icelandic <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/is/>\n"
 "Language: is\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n % 10 != 1 || n % 100 == 11;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 "X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albanía"
@@ -410,14 +410,17 @@
 
 msgid "India"
 msgstr "Indland"
 
 msgid "Indonesia"
 msgstr "Indónesía"
 
+msgid "Iran"
+msgstr "Íran"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Íran, íslamska lýðveldið"
 
 msgid "Iraq"
 msgstr "Írak"
 
 msgid "Ireland"
@@ -527,14 +530,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Kirgisistan"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Alþýðulýðveldið Laó"
 
+msgid "Laos"
+msgstr "Laós"
+
 msgid "Latvia"
 msgstr "Lettland"
 
 msgid "Lebanese Republic"
 msgstr "Lýðveldið Líbanon"
 
 msgid "Lebanon"
@@ -1136,14 +1142,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Svissneska ríkjasambandið"
 
 msgid "Switzerland"
 msgstr "Sviss"
 
+msgid "Syria"
+msgstr "Sýrland"
+
 msgid "Syrian Arab Republic"
 msgstr "Sýrlenska arabalýðveldið"
 
 msgid "Taiwan"
 msgstr "Tævan"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2017-10-23 16:07+0000\n"
+"PO-Revision-Date: 2023-03-20 09:23+0000\n"
 "Last-Translator: Sveinn í Felli <sv1@fellsnet.is>\n"
-"Language-Team: Icelandic <translation-team-is@lists.sourceforge.net>\n"
+"Language-Team: Icelandic <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-3/is/>\n"
 "Language: is\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Bugs: Report translation errors to the Language-Team address.\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Lokalize 1.5\n"
+"X-Generator: Weblate 4.16.2-dev\n"
+"X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "British Antarctic Territory"
 msgstr "Breska suðurskautslandssvæðið"
 
 msgid "Burma, Socialist Republic of the Union of"
 msgstr "Búrma, sambandsríki sósíalistalýðveldisins"
 
@@ -97,9 +98,12 @@
 
 msgid "Wake Island"
 msgstr "Wake-eyja"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
 msgstr "Jemen, sambandslýðveldi, alþýðulýðveldi"
 
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Júgóslavía, (sósíalíska) sambandslýðveldið"
+
 msgid "Zaire, Republic of"
 msgstr "Lýðveldið Saír"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,103 +1,107 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2011-06-20 11:05+0100\n"
-"Last-Translator: Arangel Angov <arangel@linux.net.mk>\n"
-"Language-Team: Macedonian <ossm-members@hedona.on.net.mk>\n"
-"Language: mk\n"
+"PO-Revision-Date: 2023-04-06 19:15+0300\n"
+"Last-Translator: Damyan Ivanov <dmn@debian.org>\n"
+"Language-Team: Bulgarian <dict@ludost.net>\n"
+"Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: KBabel 1.11.4\n"
+"X-Generator: Gtranslator 42.0\n"
+"Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 msgid "British Antarctic Territory"
-msgstr "Британска антартичка територија"
+msgstr "Британски антарктически територии"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Социјалистичка република на сојузот на Бурма"
+msgstr "Бурма, Социалистическа република на обединението"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Беолоруска ССР Советска социјалистичка република"
+msgstr "Белоруска ССР"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Кантон и Ендербури"
+msgstr "Острови Кантон и Ендербъри"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Чехословачка, Чехословачка социјалистичка Република"
+msgstr "Чехословакия, Чехословашка социалистическа република"
 
 msgid "Dahomey"
-msgstr "Дахомеј"
+msgstr "Дахоми"
 
 msgid "Dronning Maud Land"
-msgstr "Dronning Maud Land"
+msgstr "Земя на кралица Мод"
 
 msgid "East Timor"
-msgstr "Источен Тимор"
+msgstr "Източен Тимор"
 
 msgid "France, Metropolitan"
-msgstr "Франција, Метрополијан"
+msgstr "Франция, метрополитен"
 
 msgid "French Afars and Issas"
-msgstr "Француски Афарс и Исас"
+msgstr "Френски Афари и Исаи"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Јужни француски територии и антартички територии"
+msgstr "Френски южни и антарктически територии"
 
 msgid "German Democratic Republic"
-msgstr "Демократска република Германија"
+msgstr "Германска Демократична Република"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Островите Гилберт и Елис"
+msgstr "Острови Гилберт и Елис"
 
 msgid "Johnston Island"
-msgstr "Островот на Џонстон"
+msgstr "Остров Джонсън"
 
 msgid "Midway Islands"
-msgstr "Острови Мидвеј"
+msgstr "Острови Мидуей"
 
 msgid "Netherlands Antilles"
-msgstr "Холандски антили"
+msgstr "Холандски Антили"
 
 msgid "Neutral Zone"
 msgstr "Неутрална зона"
 
 msgid "New Hebrides"
-msgstr "Нов Хебридес"
+msgstr "Нови Хебриди"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Пацифички острови (сигурна територија)"
+msgstr "Тихоокеански острови"
 
 msgid "Panama Canal Zone"
-msgstr "Панамски канал"
+msgstr "Панама централна зона"
 
 msgid "Serbia and Montenegro"
-msgstr "Србија и Црна Гора"
+msgstr "Сърбия и Черна гора"
 
 msgid "Sikkim"
 msgstr "Сиким"
 
 msgid "Southern Rhodesia"
-msgstr "Јужна Родезија"
+msgstr "Южна Родезия"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "Разни острови на САД во пацификот"
+msgstr "САЩ - тихоокеански острови"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "УССР, Унија на советски социјалистички републики"
+msgstr "СССР, Съюз на съветските социалистически републики"
 
 msgid "Upper Volta, Republic of"
-msgstr "Република горна Волта"
+msgstr "Горна Волта, Република"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Демократска република Виетнам"
+msgstr "Виетнам, Демократична република"
 
 msgid "Wake Island"
-msgstr "Островот Вејк"
+msgstr "Остров Уейк"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr "Демократска република Јемен"
+msgstr "Йемен, Демократична, Народна демократична република"
+
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Югославия, (Социалистическа) федеративна република"
 
 msgid "Zaire, Republic of"
-msgstr "Република Заир"
+msgstr "Заир, Република"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,34 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2017-12-29 14:24+0000\n"
-"Last-Translator: Chris Leonard <cjlhomeaddress@gmail.com>\n"
-"Language-Team: Moldovan <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-1/mo/>\n"
+"PO-Revision-Date: 2023-03-07 17:40+0000\n"
+"Last-Translator: Vlad Nenea <diskette144@hotmail.com>\n"
+"Language-Team: Moldavian <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-1/ro_MD/>\n"
 "Language: mo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 2.19-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "Afghanistan"
 msgstr "Афганистан"
 
 msgid "Armenia"
 msgstr "Армения"
 
 msgid "Austria"
 msgstr "Аустрия"
 
 msgid "Azerbaijan"
-msgstr "Азербаиӂан"
+msgstr "Азербайӂан"
 
 msgid "Belarus"
 msgstr "Беларус"
 
 msgid "Bulgaria"
 msgstr "Булгария"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-1.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,414 +1,402 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: iso_639-3\n"
+"Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2018-09-19 06:30+0000\n"
-"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
-"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/iso-"
-"codes/iso-639-3/nb/>\n"
-"Language: nb\n"
+"PO-Revision-Date: 2022-02-03 00:54+0000\n"
+"Last-Translator: Chris Leonard <cjlhomeaddress@gmail.com>\n"
+"Language-Team: Zulu <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-1/zu/>\n"
+"Language: zu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.2-dev\n"
+"X-Generator: Weblate 4.11-dev\n"
 
-msgid "Afar"
-msgstr "afar"
+msgid "Afghanistan"
+msgstr "I-Afganistani"
 
-msgid "Afrikaans"
-msgstr "Afrikansk"
+msgid "Albania"
+msgstr "I-Albaniya"
 
-msgid "Arabic"
-msgstr "Arabisk"
+msgid "Algeria"
+msgstr "IAljiriya"
 
-msgid "Aragonese"
-msgstr "aragonsk"
+msgid "Andorra"
+msgstr "I-Andora"
 
-msgid "Armenian"
-msgstr "armensk"
+msgid "Angola"
+msgstr "I-Angola"
 
-msgid "Assamese"
-msgstr "assamisk"
+msgid "Antigua and Barbuda"
+msgstr "Antigua no Barbuda"
 
-msgid "Avestan"
-msgstr "avestisk"
+msgid "Argentina"
+msgstr "I-Argentina"
 
-msgid "Aymara"
-msgstr "aymara"
+msgid "Australia"
+msgstr "I-Ostreliya"
 
-msgid "Azerbaijani"
-msgstr "Aserbadjansk"
+msgid "Austria"
+msgstr "I-Ostriya"
 
-msgid "Balinese"
-msgstr "balinesisk"
+msgid "Azerbaijan"
+msgstr "I-Azerbayijani"
 
-msgid "Bambara"
-msgstr "bambara"
+msgid "Bangladesh"
+msgstr "Isi-Bhangladeshi"
 
-msgid "Bashkir"
-msgstr "basjkirsk"
+msgid "Barbados"
+msgstr "I-Barbados"
 
-msgid "Basque"
-msgstr "Baskisk"
+msgid "Belarus"
+msgstr "IBelarusi"
 
-msgid "Batak"
-msgstr "batak"
+msgid "Belgium"
+msgstr "Isi-Bhelijiyamu"
 
-msgid "Bengali"
-msgstr "bengali"
+msgid "Belize"
+msgstr "Belize"
 
-msgid "Bislama"
-msgstr "bislama"
+msgid "Benin"
+msgstr "IBenini"
 
-msgid "Blissymbols"
-msgstr "blissymbol"
+msgid "Bolivia"
+msgstr "I Boliviya"
 
-msgid "Breton"
-msgstr "Breton"
+msgid "Bosnia and Herzegovina"
+msgstr "IBhosniya neHerzegovina"
 
-msgid "Buginese"
-msgstr "buginesisk"
+msgid "Botswana"
+msgstr "IButswana"
 
-msgid "Buhid"
-msgstr "buhid"
+msgid "Brazil"
+msgstr "IBrazili"
 
-msgid "Bulgarian"
-msgstr "Bulgarsk"
+msgid "Bulgaria"
+msgstr "IBulgariya"
 
-msgid "Burmese"
-msgstr "burmesisk"
+msgid "Burkina Faso"
+msgstr "IBukhina Faso"
 
-msgid "Catalan"
-msgstr "Katalan"
+msgid "Burundi"
+msgstr "IBurundi"
 
-msgid "Chamorro"
-msgstr "chamorro"
+msgid "Cameroon"
+msgstr "IKamerooni"
 
-msgid "Cherokee"
-msgstr "cherokee"
+msgid "Canada"
+msgstr "I Khanada"
 
-msgid "Chinese"
-msgstr "Kinesisk"
+msgid "Chad"
+msgstr "ITshedi"
 
-msgid "Chuvash"
-msgstr "tsjuvansk"
+msgid "Chile"
+msgstr "I-Chile"
 
-msgid "Croatian"
-msgstr "Kroatsisk"
+msgid "China"
+msgstr "Isi-Shayina"
 
-msgid "Czech"
-msgstr "Tjekkisk"
+msgid "Colombia"
+msgstr "IKolombiya"
 
-msgid "Danish"
-msgstr "Dansk"
+msgid "Comoros"
+msgstr "IsiKhomorosi"
 
-msgid "Dong"
-msgstr "Vietnamesiske dồng"
+msgid "Croatia"
+msgstr "IKrowati"
 
-msgid "Dutch"
-msgstr "Nederlandsk"
+msgid "Denmark"
+msgstr "IDenimaki"
 
-msgid "Dzongkha"
-msgstr "dzongkha"
+msgid "Djibouti"
+msgstr "IJibuthi"
 
-msgid "Esperanto"
-msgstr "Esperanto"
+msgid "Dominican Republic"
+msgstr "Ulawulo lokuziphatha kwe Dominikhani"
 
-msgid "Estonian"
-msgstr "Estonsk"
+msgid "Egypt"
+msgstr "IGibhithe"
 
-msgid "Ewe"
-msgstr "ewe"
+msgid "El Salvador"
+msgstr "El Salvador"
 
-msgid "Faroese"
-msgstr "færøysk"
+msgid "Equatorial Guinea"
+msgstr "IGini Enkabazwe"
 
-msgid "Fijian"
-msgstr "fijiansk"
+msgid "Eritrea"
+msgstr "I-Eritrea"
 
-msgid "Finnish"
-msgstr "Finsk"
+msgid "Estonia"
+msgstr "I-Estoniya"
 
-msgid "French"
-msgstr "Fransk"
+msgid "Ethiopia"
+msgstr "I-Ithiopia"
 
-msgid "Fulah"
-msgstr "fulani"
+msgid "Fiji"
+msgstr "IFiji"
 
-msgid "Ganda"
-msgstr "ganda"
+msgid "Finland"
+msgstr "IFinlandi"
 
-msgid "German"
-msgstr "Tysk"
+msgid "France"
+msgstr "IFulansi"
 
-msgid "Gujarati"
-msgstr "gujarati"
+msgid "Gabon"
+msgstr "IGaboni"
 
-msgid "Hawaiian"
-msgstr "hawaiisk"
+msgid "Germany"
+msgstr "IJalimani"
 
-msgid "Hebrew"
-msgstr "Hebraisk"
+msgid "Ghana"
+msgstr "IGana"
 
-msgid "Hindi"
-msgstr "hindi"
+msgid "Greece"
+msgstr "IGreki"
 
-msgid "Hungarian"
-msgstr "Ungarsk"
+msgid "Grenada"
+msgstr "I-Grenada"
 
-msgid "Icelandic"
-msgstr "Islandsk"
+msgid "Guatemala"
+msgstr "I-Guwathemala"
 
-msgid "Ido"
-msgstr "ido"
+msgid "Guinea"
+msgstr "IGini"
 
-msgid "Igbo"
-msgstr "ibo"
+msgid "Guinea-Bissau"
+msgstr "IGini Bisawu"
 
-msgid "Interlingue"
-msgstr "interlingue"
+msgid "Honduras"
+msgstr "I-Hondurasi"
 
-msgid "Inuktitut"
-msgstr "inuktitut"
+msgid "Hong Kong"
+msgstr "Hong Kong"
 
-msgid "Inupiaq"
-msgstr "unupiak"
+msgid "Hungary"
+msgstr "I-Hungariya"
 
-msgid "Irish"
-msgstr "Irsk"
+msgid "Iceland"
+msgstr "I-Ayisilandi"
 
-msgid "Italian"
-msgstr "Italiensk"
+msgid "Indonesia"
+msgstr "I-Indonesia"
 
-msgid "Japanese"
-msgstr "Japansk"
+msgid "Iraq"
+msgstr "I-Iraki"
 
-msgid "Kannada"
-msgstr "kannada"
+msgid "Ireland"
+msgstr "I-Ayilendi"
 
-msgid "Kashmiri"
-msgstr "kasjmiri"
+msgid "Israel"
+msgstr "Isreyili"
 
-msgid "Kazakh"
-msgstr "kasakhisk"
+msgid "Italy"
+msgstr "ITaliya"
 
-msgid "Kikuyu"
-msgstr "kikuyu"
+msgid "Japan"
+msgstr "IJaphani"
 
-msgid "Kinyarwanda"
-msgstr "kinjarwanda"
+msgid "Kenya"
+msgstr "IKenya"
 
-msgid "Kirghiz"
-msgstr "kirgisisk"
+msgid "Latvia"
+msgstr "ILatviya"
 
-msgid "Komi"
-msgstr "komi"
+msgid "Lesotho"
+msgstr "OSotho"
 
-msgid "Kongo"
-msgstr "kikongo"
+msgid "Liberia"
+msgstr "ILiberia"
 
-msgid "Korean"
-msgstr "Koreansk"
+msgid "Libya"
+msgstr "ILibiya"
 
-msgid "Kuanyama"
-msgstr "kuanyama"
+msgid "Lithuania"
+msgstr "ILithuwaniya"
 
-msgid "Lao"
-msgstr "laotisk"
+msgid "Luxembourg"
+msgstr "I-Luxembourg"
 
-msgid "Lari"
-msgstr "Georgiske lari"
+msgid "Madagascar"
+msgstr "IMadagasika"
 
-msgid "Latvian"
-msgstr "Latvisk"
+msgid "Malawi"
+msgstr "IMalawi"
 
-msgid "Lingala"
-msgstr "lingala"
-
-msgid "Lithuanian"
-msgstr "Lituaisk"
-
-msgid "Luba-Katanga"
-msgstr "luba-katanga"
-
-msgid "Macedonian"
-msgstr "Makedonsk"
-
-msgid "Malagasy"
-msgstr "madagassisk"
+msgid "Mali"
+msgstr "IMali"
 
-msgid "Malayalam"
-msgstr "malayalam"
+msgid "Malta"
+msgstr "IMalta"
 
-msgid "Mali"
-msgstr "Mali"
+msgid "Mauritania"
+msgstr "IMoritaniya"
 
-msgid "Maltese"
-msgstr "Maltisk"
+msgid "Mauritius"
+msgstr "IMorishisi"
 
-msgid "Manx"
-msgstr "manx"
+msgid "Mayotte"
+msgstr "IMayotte"
 
-msgid "Maori"
-msgstr "Maori"
+msgid "Mexico"
+msgstr "IMekisiko"
 
-msgid "Nauru"
-msgstr "nauru"
+msgid "Montenegro"
+msgstr "IMontenegro"
 
-msgid "Ndebele, North"
-msgstr "ndebele (nord)"
+msgid "Morocco"
+msgstr "IMorokho"
 
-msgid "Ndebele, South"
-msgstr "ndebele, sør"
+msgid "Mozambique"
+msgstr "IMozambiki"
 
-msgid "Ojibwa"
-msgstr "ojibwa"
+msgid "Namibia"
+msgstr "INamibhiya"
 
-msgid "Oromo"
-msgstr "oromo"
+msgid "Nepal"
+msgstr "Nepal"
 
-msgid "Polish"
-msgstr "Polsk"
+msgid "Netherlands"
+msgstr "I-Netherlands"
 
-msgid "Portuguese"
-msgstr "Portugisisk"
+msgid "New Zealand"
+msgstr "INyuzilandi"
 
-msgid "Quechua"
-msgstr "quechua"
+msgid "Nicaragua"
+msgstr "Nicaragua"
 
-msgid "Romanian"
-msgstr "Rumensk"
+msgid "Niger"
+msgstr "INayighe"
 
-msgid "Rundi"
-msgstr "rundi"
+msgid "Nigeria"
+msgstr "INigeria"
 
-msgid "Russian"
-msgstr "Russisk"
+msgid "Norway"
+msgstr "INoki"
 
-msgid "Samoan"
-msgstr "samoansk"
+msgid "Pakistan"
+msgstr "IPakistani"
 
-msgid "Sango"
-msgstr "sango"
+msgid "Panama"
+msgstr "Panama"
 
-msgid "Sanskrit"
-msgstr "sanskrit"
+msgid "Paraguay"
+msgstr "I-Paraguwayi"
 
-msgid "Serbian"
-msgstr "Serbisk"
+msgid "Peru"
+msgstr "I-Peru"
 
-msgid "Sidamo"
-msgstr "sidamo"
+msgid "Poland"
+msgstr "IPolandi"
 
-msgid "Sindhi"
-msgstr "sindhi"
+msgid "Portugal"
+msgstr "IPhothugali"
 
-msgid "Slovak"
-msgstr "Slovakisk"
+msgid "Republic of the Congo"
+msgstr "IKongo"
 
-msgid "Slovenian"
-msgstr "Slovensk"
+msgid "Romania"
+msgstr "I-Romaniya"
 
-msgid "Somali"
-msgstr "somalisk"
+msgid "Rwanda"
+msgstr "IRuwanda"
 
-msgid "Sotho, Southern"
-msgstr "Sotho, (sørlig)"
+msgid "Réunion"
+msgstr "IRiyunion"
 
-msgid "Southern Sotho"
-msgstr "Sørsotho"
+msgid "San Marino"
+msgstr "USanti Marino"
 
-msgid "Spanish"
-msgstr "Spansk"
+msgid "Sao Tome and Principe"
+msgstr "ISawu Tome noPhrinitshipeyi"
 
-msgid "Sundanese"
-msgstr "sundanesisk"
+msgid "Senegal"
+msgstr "ISenegal"
 
-msgid "Swati"
-msgstr "swati"
+msgid "Serbia"
+msgstr "ISerbiya"
 
-msgid "Swedish"
-msgstr "Svensk"
+msgid "Seychelles"
+msgstr "IsiSeyisheli"
 
-msgid "Tagalog"
-msgstr "tagalog"
+msgid "Sierra Leone"
+msgstr "ISiera Liyoni"
 
-msgid "Tala"
-msgstr "Samoanske tala"
+msgid "Slovakia"
+msgstr "ISlovaki"
 
-msgid "Tamil"
-msgstr "Tamilsk"
+msgid "Slovenia"
+msgstr "ISloveniya"
 
-msgid "Tatar"
-msgstr "tatarisk"
+msgid "Somalia"
+msgstr "ISomalia"
 
-msgid "Telugu"
-msgstr "telugu"
+msgid "South Africa"
+msgstr "IRiphabliki yaseNingizimu Afrika"
 
-msgid "Thai"
-msgstr "Thai"
+msgid "South Sudan"
+msgstr "ISudan yaseNingizimu"
 
-msgid "Tibetan"
-msgstr "tibetansk"
+msgid "Spain"
+msgstr "ISpeyini"
 
-msgid "Tokelau"
-msgstr "Tokelau"
+msgid "Sri Lanka"
+msgstr "Sri Lanka"
 
-msgid "Tonga (Tonga Islands)"
-msgstr "tonga (Tonga-øyene)"
+msgid "Sudan"
+msgstr "ISudan"
 
-msgid "Tsonga"
-msgstr "tsonga"
+msgid "Sweden"
+msgstr "ISwidi"
 
-msgid "Tswana"
-msgstr "tswana"
+msgid "Switzerland"
+msgstr "I-Switzerland"
 
-msgid "Turkish"
-msgstr "Tyrkisk"
+msgid "Taiwan"
+msgstr "I-Tayiwani"
 
-msgid "Turkmen"
-msgstr "turkmensk"
+msgid "Tanzania"
+msgstr "ITanzania"
 
-msgid "Tuvalu"
-msgstr "Tuvalu"
+msgid "Thailand"
+msgstr "I-Thayilandi"
 
-msgid "Twi"
-msgstr "twi"
+msgid "Togo"
+msgstr "ITogo"
 
-msgid "Uighur"
-msgstr "uigurisk"
+msgid "Trinidad and Tobago"
+msgstr "I-Trinidad ne Tobago"
 
-msgid "Urdu"
-msgstr "urdu"
+msgid "Tunisia"
+msgstr "ITunisia"
 
-msgid "Uzbek"
-msgstr "usbekisk"
+msgid "Uganda"
+msgstr "IYuganda"
 
-msgid "Vai"
-msgstr "vai"
+msgid "Ukraine"
+msgstr "I-Yukreyini"
 
-msgid "Venda"
-msgstr "venda"
+msgid "United Kingdom"
+msgstr "Umbuso Ohlangeneyo"
 
-msgid "Vietnamese"
-msgstr "Vietnamesisk"
+msgid "United States of America"
+msgstr "IMelika"
 
-msgid "Walloon"
-msgstr "Vietnamesisk"
+msgid "Uruguay"
+msgstr "I-Uruguwayi"
 
-msgid "Welsh"
-msgstr "Walisisk"
+msgid "Venezuela"
+msgstr "I-Venezuwela"
 
-msgid "Wolof"
-msgstr "wolof"
+msgid "Vietnam"
+msgstr "IViyetnami"
 
-msgid "Xhosa"
-msgstr "Xhosa"
+msgid "Yemen"
+msgstr "IYemen"
 
-msgid "Yiddish"
-msgstr "jiddisk"
+msgid "Zambia"
+msgstr "IZambiya"
 
-msgid "Yoruba"
-msgstr "joruba"
+msgid "Zimbabwe"
+msgstr "IZimbabwe"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-11-28 16:08+0000\n"
-"Last-Translator: Pander <pander@users.sourceforge.net>\n"
+"PO-Revision-Date: 2023-03-18 21:41+0000\n"
+"Last-Translator: Frans Spiesschaert <frans.spiesschaert@gmail.com>\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 "X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "Afghanistan"
 msgstr "Afghanistan"
 
 msgid "Albania"
 msgstr "Albanië"
@@ -410,14 +410,17 @@
 
 msgid "India"
 msgstr "India"
 
 msgid "Indonesia"
 msgstr "Indonesië"
 
+msgid "Iran"
+msgstr "Iran"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Iran"
 
 msgid "Iraq"
 msgstr "Irak"
 
 msgid "Ireland"
@@ -527,14 +530,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Kirgizië"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Laos Democratische Volksrepubliek"
 
+msgid "Laos"
+msgstr "Laos"
+
 msgid "Latvia"
 msgstr "Letland"
 
 msgid "Lebanese Republic"
 msgstr "Republiek Libanon"
 
 msgid "Lebanon"
@@ -1136,14 +1142,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Zwitserse Bondsstaat"
 
 msgid "Switzerland"
 msgstr "Zwitserland"
 
+msgid "Syria"
+msgstr "Syrië"
+
 msgid "Syrian Arab Republic"
 msgstr "Syrië"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-2\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-09-17 12:22+0000\n"
+"PO-Revision-Date: 2023-04-22 14:41+0000\n"
 "Last-Translator: Pander <pander@users.sourceforge.net>\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-2/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "'Eua"
 msgstr "'Eua"
 
 msgid "//Karas"
 msgstr "//Karas"
@@ -53,14 +53,17 @@
 
 msgid "Abra"
 msgstr "Abra"
 
 msgid "Abruzzo"
 msgstr "Abruzzen"
 
+msgid "Abuja Federal Capital Territory"
+msgstr "Federaal Hoofdstedelijk Territorium"
+
 msgid "Abyan"
 msgstr "Abyan"
 
 msgid "Abşeron"
 msgstr "Abseron"
 
 msgid "Abū Z̧aby"
@@ -77,14 +80,20 @@
 
 msgid "Acre"
 msgstr "Acre"
 
 msgid "Ad Daqahlīyah"
 msgstr "Ad Daqahlyah"
 
+msgid "Ad Dawḩah"
+msgstr "Doha"
+
+msgid "Ad Dākhilīyah"
+msgstr "Ad Dachiliyah"
+
 msgid "Adamaoua"
 msgstr "Adamaoua"
 
 msgid "Adamawa"
 msgstr "Adamawa"
 
 msgid "Adana"
@@ -104,14 +113,17 @@
 
 msgid "Adygeja, Respublika"
 msgstr "Adygeya, Republiek"
 
 msgid "Adıyaman"
 msgstr "Adıyaman"
 
+msgid "Aerodrom †"
+msgstr "Aerodrom †"
+
 msgid "Afar"
 msgstr "Afar"
 
 msgid "Afyonkarahisar"
 msgstr "Afyonkarahisar"
 
 msgid "Agadez"
@@ -209,35 +221,56 @@
 
 msgid "Akmolinskaja oblast'"
 msgstr "Aqmola, Provincie"
 
 msgid "Aknīstes novads"
 msgstr "Aknīste"
 
+msgid "Akrahreppur"
+msgstr "Akrahreppur"
+
+msgid "Akraneskaupstaður"
+msgstr "Akranes"
+
 msgid "Aksaray"
 msgstr "Aksaray"
 
 msgid "Aktjubinskaja oblast'"
 msgstr "Aqtöbe, Provincie"
 
+msgid "Akureyrarbær"
+msgstr "Akureyri"
+
 msgid "Akwa Ibom"
 msgstr "Akwa Ibom"
 
+msgid "Al Anbār"
+msgstr "Al-Anbar"
+
 msgid "Al Awsaţ"
 msgstr "Maekel"
 
 msgid "Al Aḩmadī"
 msgstr "Ahmadi"
 
+msgid "Al Balqā’"
+msgstr "Balka"
+
+msgid "Al Başrah"
+msgstr "Al-Basrah"
+
 msgid "Al Baţḩā’"
 msgstr "Batha"
 
 msgid "Al Baḩr al Aḩmar"
 msgstr "Al-Bahr-al-Ahmar"
 
+msgid "Al Biqā‘"
+msgstr "Bekavallei"
+
 msgid "Al Buraymī"
 msgstr "Al Buraymī"
 
 msgid "Al Buţnān"
 msgstr "Al Butnan"
 
 msgid "Al Buḩayrah"
@@ -260,23 +293,32 @@
 
 msgid "Al Hoceïma"
 msgstr "Al Hoceïma"
 
 msgid "Al Iskandarīyah"
 msgstr "Alexandrië"
 
+msgid "Al Ismā'īlīyah"
+msgstr "Ismaïlia"
+
 msgid "Al Jabal al Akhḑar"
 msgstr "Al Jabal al Akhdar"
 
 msgid "Al Jabal al Gharbī"
 msgstr "Al Jabal al Gharbī"
 
+msgid "Al Jafārah"
+msgstr "Al Jfara"
+
 msgid "Al Jahrā’"
 msgstr "Jahra"
 
+msgid "Al Janūb"
+msgstr "Zuid-Libanon"
+
 msgid "Al Janūbī"
 msgstr "Debub"
 
 msgid "Al Janūbīyah"
 msgstr "Al Janblyah"
 
 msgid "Al Jawf"
@@ -317,26 +359,35 @@
 
 msgid "Al Minyā"
 msgstr "Minya"
 
 msgid "Al Minūfīyah"
 msgstr "Al Minufiyah"
 
+msgid "Al Muthanná"
+msgstr "Al-Muthanna"
+
 msgid "Al Muḩarraq"
 msgstr "Al Muharraq"
 
 msgid "Al Qalyūbīyah"
 msgstr "Al Qalyubiyah"
 
 msgid "Al Qaşīm"
 msgstr "Al Qasim"
 
+msgid "Al Quds"
+msgstr "Al-Quds"
+
 msgid "Al Qunayţirah"
 msgstr "Quneitra;Al Quneitra"
 
+msgid "Al Qādisīyah"
+msgstr "Al-Qadisiyah"
+
 msgid "Al Qāhirah"
 msgstr "Caïro"
 
 msgid "Al Uqşur"
 msgstr "Luxor"
 
 msgid "Al Wakrah"
@@ -344,23 +395,29 @@
 
 msgid "Al Wusţá"
 msgstr "Al Wusta"
 
 msgid "Al Wādī al Jadīd"
 msgstr "Al Wadi al Jadid"
 
+msgid "Al Wāḩāt"
+msgstr "Al Wahat"
+
 msgid "Al Ḩasakah"
 msgstr "Al-Hasakah"
 
 msgid "Al Ḩudaydah"
 msgstr "Al Hudaydah"
 
 msgid "Al ‘Aqabah"
 msgstr "Akaba"
 
+msgid "Al ‘A̅şimah"
+msgstr "Amman"
+
 msgid "Al ‘Āşimah"
 msgstr "Al-Asimah"
 
 msgid "Alabama"
 msgstr "Alabama"
 
 msgid "Alacant*"
@@ -461,14 +518,17 @@
 
 msgid "Amambay"
 msgstr "Amambay"
 
 msgid "Amapá"
 msgstr "Amapá"
 
+msgid "Amara"
+msgstr "Amhara"
+
 msgid "Amarumayu"
 msgstr "Amazonas"
 
 msgid "Amasya"
 msgstr "Amasya"
 
 msgid "Amatas novads"
@@ -503,14 +563,23 @@
 
 msgid "Amānat al ‘Āşimah [city]"
 msgstr "Amanat al-Asimah (stad Sanaa)"
 
 msgid "An Giang"
 msgstr "An Giang"
 
+msgid "An Nabaţīyah"
+msgstr "Nabatiye"
+
+msgid "An Najaf"
+msgstr "An-Najaf"
+
+msgid "An Nuqāţ al Khams"
+msgstr "An Nuqat al Khams"
+
 msgid "Anabar"
 msgstr "Anabar"
 
 msgid "Anambra"
 msgstr "Anambra"
 
 msgid "Anatolikí Makedonía kai Thráki"
@@ -572,14 +641,17 @@
 
 msgid "Ankara"
 msgstr "Ankara"
 
 msgid "Annaba"
 msgstr "Annaba"
 
+msgid "Annobon"
+msgstr "Annobón"
+
 msgid "Ansabā"
 msgstr "Anseba"
 
 msgid "Anse Boileau"
 msgstr "Anse Boileau"
 
 msgid "Anse Etoile"
@@ -587,14 +659,17 @@
 
 msgid "Anse Royale"
 msgstr "Anse Royale"
 
 msgid "Anse aux Pins"
 msgstr "Anse aux Pins"
 
+msgid "Anse la Raye"
+msgstr "Anse-la-Raye"
+
 msgid "Antalya"
 msgstr "Antalya"
 
 msgid "Antananarivo"
 msgstr "Antananarivo"
 
 msgid "Antioquia"
@@ -614,14 +689,20 @@
 
 msgid "Antsla"
 msgstr "Antsla"
 
 msgid "Antwerpen"
 msgstr "Antwerpen"
 
+msgid "Anuradhapura"
+msgstr "Anuradhapura"
+
+msgid "Anykščiai"
+msgstr "Anykščiai"
+
 msgid "Anzoátegui"
 msgstr "Anzoátegui"
 
 msgid "Aomori"
 msgstr "Aomori"
 
 msgid "Aousserd (EH)"
@@ -650,14 +731,17 @@
 
 msgid "Apurimaq"
 msgstr "Apurímac"
 
 msgid "Ar Raqqah"
 msgstr "Ar-Raqqah"
 
+msgid "Ar Rayyān"
+msgstr "Ar Rayyan"
+
 msgid "Araba*"
 msgstr "Álava"
 
 msgid "Arad"
 msgstr "Arad"
 
 msgid "Aragac̣otn"
@@ -674,14 +758,17 @@
 
 msgid "Arauca"
 msgstr "Arauca"
 
 msgid "Aračinovo"
 msgstr "Aračinovo"
 
+msgid "Arbīl"
+msgstr "Erbil"
+
 msgid "Ardabīl"
 msgstr "Ardebil"
 
 msgid "Ardahan"
 msgstr "Ardahan"
 
 msgid "Ardennes"
@@ -755,38 +842,56 @@
 
 msgid "Arua"
 msgstr "Arua"
 
 msgid "Aruba"
 msgstr "Aruba"
 
+msgid "Arunāchal Pradesh"
+msgstr "Arunachal Pradesh"
+
 msgid "Arusha"
 msgstr "Arusha"
 
+msgid "As Sulaymānīyah"
+msgstr "Suleimaniya"
+
 msgid "As Suwaydā'"
 msgstr "As-Suwayda"
 
 msgid "As Suways"
 msgstr "As Suways"
 
 msgid "Ascension"
 msgstr "Ascension"
 
 msgid "Ascoli Piceno"
 msgstr "Ascoli Piceno"
 
+msgid "Ash Shamāl"
+msgstr "Ash Shamal"
+
+msgid "Ash Shamālī"
+msgstr "Ash Shamālī"
+
 msgid "Ash Shamālīyah"
 msgstr "Ash Shamallyah"
 
 msgid "Ash Sharqīyah"
 msgstr "Ash Sharqiyah"
 
+msgid "Ash Shimāl"
+msgstr "Noord-Libanon"
+
 msgid "Ash Shāriqah"
 msgstr "Sharjah"
 
+msgid "Ash Shīḩānīyah"
+msgstr "Al-Shahaniya"
+
 msgid "Ashanti"
 msgstr "Ashanti"
 
 msgid "Assa-Zag (EH-partial)"
 msgstr "Assa-Zag (EH-gedeeltelijk)"
 
 msgid "Assaba"
@@ -812,14 +917,17 @@
 
 msgid "Asunción"
 msgstr "Asunción"
 
 msgid "Aswān"
 msgstr "Aswan"
 
+msgid "Asyūţ"
+msgstr "Assioet"
+
 msgid "Atacama"
 msgstr "Atacama"
 
 msgid "Atacora"
 msgstr "Atacora"
 
 msgid "Atlantique"
@@ -902,17 +1010,23 @@
 
 msgid "Aydın"
 msgstr "Aydin"
 
 msgid "Ayeyarwady"
 msgstr "Ayeyarwady"
 
+msgid "Az Zarqā’"
+msgstr "Zarka"
+
 msgid "Az Zāwiyah"
 msgstr "Az Zawiyah"
 
+msgid "Azad Jammu and Kashmir"
+msgstr "Azad-staat van Jammu en Kasjmir"
+
 msgid "Azilal"
 msgstr "Azilal"
 
 msgid "Azua"
 msgstr "Azua"
 
 msgid "Azuay"
@@ -956,14 +1070,17 @@
 
 msgid "Ba"
 msgstr "Ba"
 
 msgid "Baalbek-Hermel"
 msgstr "Baalbek-Hermel"
 
+msgid "Baat Dambang"
+msgstr "Battambang"
+
 msgid "Babītes novads"
 msgstr "Babīte"
 
 msgid "Babək"
 msgstr "Babak"
 
 msgid "Bacău"
@@ -986,14 +1103,17 @@
 
 msgid "Bafatá"
 msgstr "Bafatá"
 
 msgid "Bagerhat"
 msgstr "Bagerhat"
 
+msgid "Baghdād"
+msgstr "Bagdad"
+
 msgid "Baghlān"
 msgstr "Baghlan"
 
 msgid "Bagmati"
 msgstr "Bagmati"
 
 msgid "Bago"
@@ -1007,14 +1127,17 @@
 
 msgid "Baie Lazare"
 msgstr "Baie Lazare"
 
 msgid "Baie Sainte Anne"
 msgstr "Baie Sainte Anne"
 
+msgid "Baitsi"
+msgstr "Baiti"
+
 msgid "Baja California"
 msgstr "Baja California; Neder-Californië"
 
 msgid "Baja California Sur"
 msgstr "Baja California Sur; Zuid-Neder-Californië"
 
 msgid "Baja Verapaz"
@@ -1091,14 +1214,17 @@
 
 msgid "Banjul"
 msgstr "Banjul"
 
 msgid "Banskobystrický kraj"
 msgstr "Banská Bystrica, Regio"
 
+msgid "Banteay Mean Choăy"
+msgstr "Banteay Mean Cheay"
+
 msgid "Banten"
 msgstr "Banten"
 
 msgid "Banwa"
 msgstr "Banwa"
 
 msgid "Banī Suwayf"
@@ -1181,14 +1307,17 @@
 
 msgid "Basilicata"
 msgstr "Basilicata"
 
 msgid "Basse-Kotto"
 msgstr "Basse-Kotto"
 
+msgid "Bataan"
+msgstr "Bataan"
+
 msgid "Batanes"
 msgstr "Batanes"
 
 msgid "Batangas"
 msgstr "Batangas"
 
 msgid "Bath and North East Somerset"
@@ -1199,14 +1328,17 @@
 
 msgid "Batman"
 msgstr "Batman"
 
 msgid "Batna"
 msgstr "Batna"
 
+msgid "Batticaloa"
+msgstr "Batticaloa"
+
 msgid "Batys Qazaqstan oblysy"
 msgstr "Batıs Qazaqstan, Provincie"
 
 msgid "Baucau"
 msgstr "Baucau"
 
 msgid "Bauchi"
@@ -1262,14 +1394,17 @@
 
 msgid "Belait"
 msgstr "Belait"
 
 msgid "Belfast City"
 msgstr "Belfast"
 
+msgid "Belgorodskaja oblast'"
+msgstr "Belgorod, Oblast"
+
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Belluno"
 msgstr "Belluno"
 
 msgid "Beltinci"
@@ -1298,14 +1433,17 @@
 
 msgid "Benguela"
 msgstr "Benguela"
 
 msgid "Benguet"
 msgstr "Benguet"
 
+msgid "Benshangul-Gumaz"
+msgstr "Benishangul-Gumuz"
+
 msgid "Benslimane"
 msgstr "Benslimane"
 
 msgid "Benue"
 msgstr "Benue"
 
 msgid "Beograd"
@@ -1397,29 +1535,41 @@
 
 msgid "Bingöl"
 msgstr "Bingol"
 
 msgid "Biobío"
 msgstr "Biobío"
 
+msgid "Bioko Nord"
+msgstr "Bioko Norte"
+
+msgid "Bioko Sud"
+msgstr "Bioko Sur"
+
 msgid "Biombo"
 msgstr "Biombo"
 
 msgid "Birgu"
 msgstr "Birgu"
 
 msgid "Birkirkara"
 msgstr "Birkirkara"
 
 msgid "Birmingham"
 msgstr "Birmingham"
 
+msgid "Birštono"
+msgstr "Birštonas"
+
 msgid "Birżebbuġa"
 msgstr "Birżebbuġa"
 
+msgid "Biržai"
+msgstr "Biržai"
+
 msgid "Bishkek Shaary"
 msgstr "Bisjkek"
 
 msgid "Biskra"
 msgstr "Biskra"
 
 msgid "Bissau"
@@ -1484,14 +1634,20 @@
 
 msgid "Bloke"
 msgstr "Bloke"
 
 msgid "Blue Nile"
 msgstr "Blauwe Nijl"
 
+msgid "Bláskógabyggð"
+msgstr "Bláskógabyggð"
+
+msgid "Blönduósbær"
+msgstr "Blönduós"
+
 msgid "Boa Vista"
 msgstr "Boa Vista"
 
 msgid "Boaco"
 msgstr "Boaco"
 
 msgid "Bobonaro"
@@ -1538,14 +1694,17 @@
 
 msgid "Bolton"
 msgstr "Bolton"
 
 msgid "Bolu"
 msgstr "Bolu"
 
+msgid "Bolungarvíkurkaupstaður"
+msgstr "Bolungarvík"
+
 msgid "Bolzano"
 msgstr "Bolzano"
 
 msgid "Bolívar"
 msgstr "Bolívar"
 
 msgid "Bomet"
@@ -1568,14 +1727,20 @@
 
 msgid "Boquerón"
 msgstr "Boquerón"
 
 msgid "Bordj Bou Arréridj"
 msgstr "Bordj Bou Arréridj"
 
+msgid "Borgarbyggð"
+msgstr "Borgarbyggð"
+
+msgid "Borgarfjarðarhreppur"
+msgstr "Borgarfjarðarhreppur"
+
 msgid "Borgo Maggiore"
 msgstr "Borgo Maggiore"
 
 msgid "Borgou"
 msgstr "Borgou"
 
 msgid "Borkou"
@@ -1595,14 +1760,17 @@
 
 msgid "Borsod-Abaúj-Zemplén"
 msgstr "Borsod-Abaúj-Zemplén"
 
 msgid "Bosilovo"
 msgstr "Bosilovo"
 
+msgid "Botha-Bothe"
+msgstr "Butha-Buthe"
+
 msgid "Botoșani"
 msgstr "Botoșani"
 
 msgid "Bouches-du-Rhône"
 msgstr "Oevers van de Rhône"
 
 msgid "Boucle du Mouhoun"
@@ -1727,14 +1895,17 @@
 
 msgid "Bristol, City of"
 msgstr "Bristol, City of"
 
 msgid "British Columbia"
 msgstr "Brits-Columbia"
 
+msgid "Brjanskaja oblast'"
+msgstr "Brjansk, Oblast"
+
 msgid "Brno-město"
 msgstr "Brno-město"
 
 msgid "Brno-venkov"
 msgstr "Brno-venkov"
 
 msgid "Brocēnu novads"
@@ -1844,14 +2015,17 @@
 
 msgid "Burgos"
 msgstr "Burgos"
 
 msgid "Buri Ram"
 msgstr "Buri Ram"
 
+msgid "Burjatija, Respublika"
+msgstr "Boerjatië, Republiek"
+
 msgid "Bursa"
 msgstr "Bursa"
 
 msgid "Burtnieku novads"
 msgstr "Burtnieki"
 
 msgid "Bururi"
@@ -1868,14 +2042,17 @@
 
 msgid "Busia"
 msgstr "Busia"
 
 msgid "Butaleja"
 msgstr "Butaleja"
 
+msgid "Butel †"
+msgstr "Butel †"
+
 msgid "Buxoro"
 msgstr "Buchara"
 
 msgid "Buzău"
 msgstr "Buzău"
 
 msgid "Bács-Kiskun"
@@ -1910,26 +2087,35 @@
 
 msgid "Bình Thuận"
 msgstr "Binh Thuan"
 
 msgid "Bình Định"
 msgstr "Binh Dinh"
 
+msgid "Bābil"
+msgstr "Babil"
+
 msgid "Bādghīs"
 msgstr "Badghis"
 
+msgid "Bāgmatī"
+msgstr "Bagmati"
+
 msgid "Bāmyān"
 msgstr "Bamyan"
 
 msgid "Bălți"
 msgstr "Bălți"
 
 msgid "Břeclav"
 msgstr "Břeclav"
 
+msgid "Būr Sa‘īd"
+msgstr "Port Said"
+
 msgid "Būshehr"
 msgstr "Bushehr"
 
 msgid "Bərdə"
 msgstr "Barda"
 
 msgid "Bạc Liêu"
@@ -2033,14 +2219,17 @@
 
 msgid "Campobasso"
 msgstr "Campobasso"
 
 msgid "Canarias"
 msgstr "Canarische Eilanden"
 
+msgid "Canaries"
+msgstr "Canaries"
+
 msgid "Canelones"
 msgstr "Canelones"
 
 msgid "Canillo"
 msgstr "Canillo"
 
 msgid "Canindeyú"
@@ -2195,14 +2384,17 @@
 
 msgid "Celje"
 msgstr "Celje"
 
 msgid "Centar Župa"
 msgstr "Centar Župa"
 
+msgid "Centar †"
+msgstr "Centar †"
+
 msgid "Central"
 msgstr "Central"
 
 msgid "Central Abaco"
 msgstr "Central Abaco"
 
 msgid "Central Andros"
@@ -2219,14 +2411,17 @@
 
 msgid "Central Equatoria"
 msgstr "Centraal-Equatoria"
 
 msgid "Central Luzon (Region III)"
 msgstr "Central Luzon (Regio III)"
 
+msgid "Central Province"
+msgstr "Centrale Provincie"
+
 msgid "Central Region"
 msgstr "Centrale Regio"
 
 msgid "Central River"
 msgstr "Central River"
 
 msgid "Central Singapore"
@@ -2249,14 +2444,17 @@
 
 msgid "Centre-Sud"
 msgstr "Centre-Sud"
 
 msgid "Centre-Val de Loire"
 msgstr "Centre-Val de Loire"
 
+msgid "Centro Sud"
+msgstr "Centro Sur"
+
 msgid "Ceredigion [Sir Ceredigion]"
 msgstr "Ceredigion"
 
 msgid "Cerklje na Gorenjskem"
 msgstr "Cerklje na Gorenjskem"
 
 msgid "Cerknica"
@@ -2291,14 +2489,17 @@
 
 msgid "Chagang-do"
 msgstr "Chagang-do"
 
 msgid "Chaguanas"
 msgstr "Chaguanas"
 
+msgid "Chahār Maḩāl va Bakhtīārī"
+msgstr "Chahar Mahaal en Bakhtiari"
+
 msgid "Chai Nat"
 msgstr "Chai Nat"
 
 msgid "Chaiyaphum"
 msgstr "Chaiyaphum"
 
 msgid "Chalatenango"
@@ -2306,14 +2507,17 @@
 
 msgid "Champasak"
 msgstr "Champassak"
 
 msgid "Chandpur"
 msgstr "Chandpur"
 
+msgid "Chandīgarh"
+msgstr "Chandigarh"
+
 msgid "Changhua"
 msgstr "Changhua"
 
 msgid "Chanthaburi"
 msgstr "Chanthaburi"
 
 msgid "Chapai Nawabganj"
@@ -2363,14 +2567,17 @@
 
 msgid "Cheshire East"
 msgstr "Oost-Cheshire"
 
 msgid "Cheshire West and Chester"
 msgstr "West-Cheshire en Chester"
 
+msgid "Chhattīsgarh"
+msgstr "Chhattisgarh"
+
 msgid "Chhukha"
 msgstr "Chhukha"
 
 msgid "Chiang Mai"
 msgstr "Chiang Mai"
 
 msgid "Chiang Rai"
@@ -2579,14 +2786,17 @@
 
 msgid "Colima"
 msgstr "Colima"
 
 msgid "Collines"
 msgstr "Collines"
 
+msgid "Colombo"
+msgstr "Colombo"
+
 msgid "Colonia"
 msgstr "Colonia"
 
 msgid "Colorado"
 msgstr "Colorado"
 
 msgid "Colón"
@@ -2666,14 +2876,20 @@
 
 msgid "Cortés"
 msgstr "Cortés"
 
 msgid "Cosenza"
 msgstr "Cosenza"
 
+msgid "Costa Caribe Norte"
+msgstr "Región Autónoma de la Costa Caribe Norte"
+
+msgid "Costa Caribe Sur"
+msgstr "Región Autónoma de la Costa Caribe Sur"
+
 msgid "Cotabato"
 msgstr "Cotabato"
 
 msgid "Cotopaxi"
 msgstr "Cotopaxi"
 
 msgid "Couffo"
@@ -2819,14 +3035,17 @@
 
 msgid "Dagdas novads"
 msgstr "Dagda"
 
 msgid "Dagestan, Respublika"
 msgstr "Dagestan, Republiek"
 
+msgid "Dahūk"
+msgstr "Duhok"
+
 msgid "Dajabón"
 msgstr "Dajabón"
 
 msgid "Dakar"
 msgstr "Dakar"
 
 msgid "Dakhla-Oued Ed-Dahab (EH)"
@@ -2834,17 +3053,23 @@
 
 msgid "Dakhlet Nouâdhibou"
 msgstr "Dakhlet Nouadhibou"
 
 msgid "Dalaba"
 msgstr "Dalaba"
 
+msgid "Dalabyggð"
+msgstr "Dalabyggð"
+
 msgid "Dalarnas län [SE-20]"
 msgstr "Dalarnas län"
 
+msgid "Dalvíkurbyggð"
+msgstr "Dalvíkurbyggð"
+
 msgid "Danilovgrad"
 msgstr "Danilovgrad"
 
 msgid "Dar es Salaam"
 msgstr "Dar es Salaam"
 
 msgid "Dar'ā"
@@ -2894,14 +3119,17 @@
 
 msgid "Daşoguz"
 msgstr "Daşoguz"
 
 msgid "Debar"
 msgstr "Debar"
 
+msgid "Debrca"
+msgstr "Debarca"
+
 msgid "Debrecen"
 msgstr "Debrecen"
 
 msgid "Debubawi K’eyyĭḥ Baḥri"
 msgstr "Debubawi Keyih Bahri"
 
 msgid "Dedza"
@@ -2942,14 +3170,17 @@
 
 msgid "Denigomodu"
 msgstr "Denigomodu"
 
 msgid "Denizli"
 msgstr "Denizli"
 
+msgid "Dennery"
+msgstr "Dennery"
+
 msgid "Dependencias Federales"
 msgstr "Federale Afhankelijkheden"
 
 msgid "Derby"
 msgstr "Derby"
 
 msgid "Derbyshire"
@@ -2972,14 +3203,17 @@
 
 msgid "Dhamār"
 msgstr "Dhamar"
 
 msgid "Dhawalagiri"
 msgstr "Dhawalagiri"
 
+msgid "Dhī Qār"
+msgstr "Dhi Qar"
+
 msgid "Dibër"
 msgstr "Dibër"
 
 msgid "Diego Martin"
 msgstr "Diego Martin"
 
 msgid "Diekirch"
@@ -3029,20 +3263,29 @@
 
 msgid "Divača"
 msgstr "Divaca"
 
 msgid "Diyarbakır"
 msgstr "Diyarbakır"
 
+msgid "Diyālá"
+msgstr "Diyala"
+
 msgid "Djelfa"
 msgstr "Djelfa"
 
+msgid "Djibloho"
+msgstr "Djibloho"
+
 msgid "Djibouti"
 msgstr "Djibouti"
 
+msgid "Djúpavogshreppur"
+msgstr "Djúpivogur"
+
 msgid "Dnipropetrovska oblast"
 msgstr "Dnjepropetrovsk, Provincie"
 
 msgid "Dobeles novads"
 msgstr "Dobele"
 
 msgid "Dobje"
@@ -3113,14 +3356,17 @@
 
 msgid "Dornava"
 msgstr "Dornava"
 
 msgid "Dornod"
 msgstr "Dornod"
 
+msgid "Dornogovĭ"
+msgstr "Dornogovĭ"
+
 msgid "Dorset"
 msgstr "Dorset"
 
 msgid "Dosso"
 msgstr "Dosso"
 
 msgid "Doubs"
@@ -3170,23 +3416,29 @@
 
 msgid "Dudley"
 msgstr "Dudley"
 
 msgid "Dumfries and Galloway"
 msgstr "Dumfries en Galloway"
 
+msgid "Dumyāţ"
+msgstr "Damietta"
+
 msgid "Dunaújváros"
 msgstr "Dunaújváros"
 
 msgid "Dundagas novads"
 msgstr "Dundaga"
 
 msgid "Dundee City"
 msgstr "Dundee"
 
+msgid "Dundgovĭ"
+msgstr "Dundgovĭ"
+
 msgid "Duplek"
 msgstr "Duplek"
 
 msgid "Durango"
 msgstr "Durango"
 
 msgid "Durazno"
@@ -3221,14 +3473,17 @@
 
 msgid "Díli"
 msgstr "Dili"
 
 msgid "Düzce"
 msgstr "Düzce"
 
+msgid "Dādra and Nagar Haveli and Damān and Diu"
+msgstr "Dadra en Nagar Haveli en Daman en Diu"
+
 msgid "Dāykundī"
 msgstr "Daikondi"
 
 msgid "Děčín"
 msgstr "Děčín"
 
 msgid "Ealing"
@@ -3278,14 +3533,17 @@
 
 msgid "Eastern Equatoria"
 msgstr "Oost-Equatoria"
 
 msgid "Eastern Highlands"
 msgstr "Eastern Highlands"
 
+msgid "Eastern Province"
+msgstr "Oostelijke Provincie"
+
 msgid "Eastern Samar"
 msgstr "Eastern Samar"
 
 msgid "Eastern Visayas (Region VIII)"
 msgstr "Eastern Visayas (Regio VIII)"
 
 msgid "Ebon"
@@ -3506,23 +3764,32 @@
 
 msgid "Eure-et-Loir"
 msgstr "Eure en Loir"
 
 msgid "Euskal Herria"
 msgstr "Baskenland"
 
+msgid "Evrejskaja avtonomnaja oblast'"
+msgstr "Joodse Autonome Oblast"
+
 msgid "Ewa"
 msgstr "Ewa"
 
 msgid "Extremadura"
 msgstr "Extremadura"
 
 msgid "Exuma"
 msgstr "Exuma"
 
+msgid "Eyja- og Miklaholtshreppur"
+msgstr "Eyja- og Miklaholtshreppur"
+
+msgid "Eyjafjarðarsveit"
+msgstr "Eyjafjarðarsveit"
+
 msgid "Eşfahān"
 msgstr "Isfahan"
 
 msgid "Fa'asaleleaga"
 msgstr "Fa'asaleleaga"
 
 msgid "Faadhippolhu"
@@ -3539,14 +3806,17 @@
 
 msgid "Falkirk"
 msgstr "Falkirk"
 
 msgid "Far North"
 msgstr "Verre Noorden"
 
+msgid "Far Western"
+msgstr "Ver-Westers"
+
 msgid "Faranah"
 msgstr "Faranah"
 
 msgid "Faridpur"
 msgstr "Faridpur"
 
 msgid "Faro"
@@ -3599,35 +3869,50 @@
 
 msgid "Fiorentino"
 msgstr "Fiorentino"
 
 msgid "Firenze"
 msgstr "Florence"
 
+msgid "Fjallabyggð"
+msgstr "Fjallabyggð"
+
+msgid "Fjarðabyggð"
+msgstr "Fjarðabyggð"
+
 msgid "Flacq"
 msgstr "Flacq"
 
 msgid "Flevoland"
 msgstr "Flevoland"
 
 msgid "Flintshire [Sir y Fflint GB-FFL]"
 msgstr "Flintshire"
 
+msgid "Fljótsdalshreppur"
+msgstr "Fljótsdalshreppur"
+
+msgid "Fljótsdalshérað"
+msgstr "Fljótsdalshérað"
+
 msgid "Flores"
 msgstr "Flores"
 
 msgid "Florești"
 msgstr "Florești"
 
 msgid "Floriana"
 msgstr "Floriana"
 
 msgid "Florida"
 msgstr "Florida"
 
+msgid "Flóahreppur"
+msgstr "Flóahreppur"
+
 msgid "Foggia"
 msgstr "Foggia"
 
 msgid "Fontana"
 msgstr "Fontana"
 
 msgid "Fontvieille"
@@ -3656,14 +3941,17 @@
 
 msgid "Freiburg"
 msgstr "Fribourg"
 
 msgid "Fria"
 msgstr "Fria"
 
+msgid "Friuli Venezia Giulia"
+msgstr "Friuli-Venezia Giulia"
+
 msgid "Frosinone"
 msgstr "Frosinone"
 
 msgid "Fryslân"
 msgstr "Friesland"
 
 msgid "Frýdek-Místek"
@@ -3734,14 +4022,17 @@
 
 msgid "Galguduud"
 msgstr "Galguduud"
 
 msgid "Galicia [Galicia]"
 msgstr "Galicia"
 
+msgid "Galle"
+msgstr "Galle"
+
 msgid "Galway"
 msgstr "Galway"
 
 msgid "Galápagos"
 msgstr "Galápagos"
 
 msgid "Gambela Peoples"
@@ -3776,14 +4067,17 @@
 
 msgid "Garissa"
 msgstr "Garissa"
 
 msgid "Garkalnes novads"
 msgstr "Garkalne"
 
+msgid "Garðabær"
+msgstr "Garðabær"
+
 msgid "Gasa"
 msgstr "Gasa"
 
 msgid "Gash-Barka"
 msgstr "Gash-Barka"
 
 msgid "Gateshead"
@@ -3791,14 +4085,17 @@
 
 msgid "Gauteng"
 msgstr "Gauteng"
 
 msgid "Gaza"
 msgstr "Gaza"
 
+msgid "Gazi Baba †"
+msgstr "Gazi Baba †"
+
 msgid "Gaziantep"
 msgstr "Gaziantep"
 
 msgid "Gazipur"
 msgstr "Gazipur"
 
 msgid "Gbarpolu"
@@ -3887,14 +4184,17 @@
 
 msgid "Giurgiu"
 msgstr "Giurgiu"
 
 msgid "Gjirokastër"
 msgstr "Gjirokastër"
 
+msgid "Gjorče Petrov †"
+msgstr "Gorče Petrov †"
+
 msgid "Glacis"
 msgstr "Glacis"
 
 msgid "Glarus"
 msgstr "Glarus"
 
 msgid "Glasgow City"
@@ -3971,14 +4271,20 @@
 
 msgid "Gotlands län [SE-09]"
 msgstr "Gotlands län"
 
 msgid "Gourma"
 msgstr "Gourma"
 
+msgid "Govĭ-Altay"
+msgstr "Govĭ-Altaj"
+
+msgid "Govĭ-Sümber"
+msgstr "Govĭsümber"
+
 msgid "Gracias a Dios"
 msgstr "Gracias a Dios"
 
 msgid "Grad"
 msgstr "Grad"
 
 msgid "Grad Zagreb"
@@ -4037,29 +4343,44 @@
 
 msgid "Grevenmacher"
 msgstr "Grevenmacher"
 
 msgid "Gribingui"
 msgstr "Gribingui"
 
+msgid "Grindavíkurbær"
+msgstr "Grindavík"
+
 msgid "Grobiņas novads"
 msgstr "Grobiņa"
 
 msgid "Grodnenskaja oblast'"
 msgstr "Grodno, Provincie"
 
 msgid "Groningen"
 msgstr "Groningen"
 
+msgid "Gros Islet"
+msgstr "Gros Islet"
+
 msgid "Grosseto"
 msgstr "Grosseto"
 
 msgid "Grosuplje"
 msgstr "Grosuplje"
 
+msgid "Grundarfjarðarbær"
+msgstr "Grundarfjörður"
+
+msgid "Grímsnes- og Grafningshreppur"
+msgstr "Grímsnes- og Grafningshreppur"
+
+msgid "Grýtubakkahreppur"
+msgstr "Grýtubakkahreppur"
+
 msgid "Guadalajara"
 msgstr "Guadalajara"
 
 msgid "Guadalcanal"
 msgstr "Guadalcanal"
 
 msgid "Guadeloupe"
@@ -4124,23 +4445,29 @@
 
 msgid "Guimaras"
 msgstr "Guimaras"
 
 msgid "Guizhou Sheng"
 msgstr "Guizhou, Provincie"
 
+msgid "Gujarāt"
+msgstr "Gujarat"
+
 msgid "Gulbenes novads"
 msgstr "Gulbene"
 
 msgid "Gulf"
 msgstr "Gulf"
 
 msgid "Gulu"
 msgstr "Gulu"
 
+msgid "Guna Yala"
+msgstr "Guna Yala"
+
 msgid "Gunma"
 msgstr "Gunma"
 
 msgid "Guria"
 msgstr "Guria"
 
 msgid "Gusinje"
@@ -4229,26 +4556,32 @@
 
 msgid "Haa"
 msgstr "Haa"
 
 msgid "Haapsalu"
 msgstr "Haapsalu"
 
+msgid "Habarovskij kraj"
+msgstr "Chabarovsk, Kraj"
+
 msgid "Habiganj"
 msgstr "Habiganj"
 
 msgid "Hackney"
 msgstr "Hackney"
 
 msgid "Hacıqabul"
 msgstr "Haciqabul"
 
 msgid "Hadjer Lamis"
 msgstr "Hadjer-Lamis"
 
+msgid "Hafnarfjarðarkaupstaður"
+msgstr "Hafnarfjörður"
+
 msgid "Hahdhunmathi"
 msgstr "Haddhunmathi-atol"
 
 msgid "Hainan Sheng"
 msgstr "Hainan, Provincie"
 
 msgid "Hainaut"
@@ -4256,14 +4589,17 @@
 
 msgid "Hajdina"
 msgstr "Hajdina"
 
 msgid "Hajdú-Bihar"
 msgstr "Hajdú-Bihar"
 
+msgid "Hakasija, Respublika"
+msgstr "Chakassië, Republiek"
+
 msgid "Hakkâri"
 msgstr "Hakkâri"
 
 msgid "Haljala"
 msgstr "Haljala"
 
 msgid "Hallands län [SE-13]"
@@ -4271,17 +4607,26 @@
 
 msgid "Halton"
 msgstr "Halton"
 
 msgid "Hamadān"
 msgstr "Hamadan"
 
+msgid "Hambantota"
+msgstr "Hambantota"
+
 msgid "Hamburg"
 msgstr "Hamburg"
 
+msgid "Hamgyǒng-bukto"
+msgstr "Hamgyŏng-pukto"
+
+msgid "Hamgyǒng-namdo"
+msgstr "Hamgyŏng-namdo"
+
 msgid "Hammersmith and Fulham"
 msgstr "Hammersmith en Fulham"
 
 msgid "Hampshire"
 msgstr "Hampshire"
 
 msgid "Hanover"
@@ -4289,14 +4634,17 @@
 
 msgid "Hanty-Mansijskij avtonomnyj okrug"
 msgstr "Chanto-Mansië, Autonoom District"
 
 msgid "Harare"
 msgstr "Harare"
 
+msgid "Harari People"
+msgstr "Harari"
+
 msgid "Harbour Island"
 msgstr "Harbour Island"
 
 msgid "Hardap"
 msgstr "Hardap"
 
 msgid "Harghita"
@@ -4313,35 +4661,47 @@
 
 msgid "Harrow"
 msgstr "Harrow"
 
 msgid "Hartlepool"
 msgstr "Hartlepool"
 
+msgid "Haryāna"
+msgstr "Haryana"
+
 msgid "Haskovo"
 msgstr "Chaskovo"
 
 msgid "Hatay"
 msgstr "Hatay"
 
 msgid "Hato Mayor"
 msgstr "Hato Mayor"
 
+msgid "Hatohobei"
+msgstr "Hatohobei"
+
 msgid "Haut-Katanga"
 msgstr "Haut-Katanga"
 
+msgid "Haut-Lomami"
+msgstr "Opper-Lomami"
+
 msgid "Haut-Mbomou"
 msgstr "Haut-Mbomou"
 
 msgid "Haut-Ogooué"
 msgstr "Haut-Ogooué"
 
 msgid "Haut-Rhin"
 msgstr "Hoog-Rijn"
 
+msgid "Haut-Uélé"
+msgstr "Opper-Uele"
+
 msgid "Haute-Corse"
 msgstr "Hoog-Corsica"
 
 msgid "Haute-Garonne"
 msgstr "Hoog-Garonne"
 
 msgid "Haute-Kotto"
@@ -4400,14 +4760,17 @@
 
 msgid "Heilongjiang Sheng"
 msgstr "Heilongjiang, Provincie"
 
 msgid "Hela"
 msgstr "Hela"
 
+msgid "Helgafellssveit"
+msgstr "Helgafellssveit"
+
 msgid "Helmand"
 msgstr "Helmand"
 
 msgid "Henan Sheng"
 msgstr "Henan, Provincie"
 
 msgid "Hentiy"
@@ -4457,14 +4820,17 @@
 
 msgid "Hiiumaa"
 msgstr "Hiiumaa"
 
 msgid "Hillingdon"
 msgstr "Hillingdon"
 
+msgid "Himāchal Pradesh"
+msgstr "Himachal Pradesh"
+
 msgid "Hiroshima"
 msgstr "Hiroshima"
 
 msgid "Hodh ech Chargui"
 msgstr "Hodh ech Chargui"
 
 msgid "Hodh el Gharbi"
@@ -4526,14 +4892,17 @@
 
 msgid "Hrastnik"
 msgstr "Hrastnik"
 
 msgid "Hrpelje-Kozina"
 msgstr "Hrpelje-Kozina"
 
+msgid "Hrunamannahreppur"
+msgstr "Hrunamannahreppur"
+
 msgid "Hsinchu"
 msgstr "Hsinchu"
 
 msgid "Hualien"
 msgstr "Hualien"
 
 msgid "Huambo"
@@ -4568,14 +4937,20 @@
 
 msgid "Huánuco"
 msgstr "Huánuco"
 
 msgid "Huíla"
 msgstr "Huíla"
 
+msgid "Hvalfjarðarsveit"
+msgstr "Hvalfjarðarsveit"
+
+msgid "Hveragerðisbær"
+msgstr "Hveragerðisbær"
+
 msgid "Hwanghae-bukto"
 msgstr "Hwanghae-bukto"
 
 msgid "Hwanghae-namdo"
 msgstr "Hwanghae-namdo"
 
 msgid "Hyogo"
@@ -4601,17 +4976,26 @@
 
 msgid "Hódmezővásárhely"
 msgstr "Hódmezővásárhely"
 
 msgid "Höfuðborgarsvæði"
 msgstr "Hoofdstedelijke Regio"
 
+msgid "Hörgársveit"
+msgstr "Hörgársveit"
+
 msgid "Hövsgöl"
 msgstr "Hövsgöl"
 
+msgid "Húnavatnshreppur"
+msgstr "Húnavatnshreppur"
+
+msgid "Húnaþing vestra"
+msgstr "Húnaþing vestra"
+
 msgid "Hưng Yên"
 msgstr "Hung Yen"
 
 msgid "H̱efa"
 msgstr "Haifa"
 
 msgid "Hải Phòng"
@@ -4796,14 +5180,17 @@
 
 msgid "Irbid"
 msgstr "Irbid"
 
 msgid "Iringa"
 msgstr "Iringa"
 
+msgid "Irkutskaja oblast'"
+msgstr "Irkoetsk, Oblast"
+
 msgid "Isabel"
 msgstr "Isabel"
 
 msgid "Isabela"
 msgstr "Isabela"
 
 msgid "Isernia"
@@ -4853,17 +5240,23 @@
 
 msgid "Isère"
 msgstr "Isère"
 
 msgid "Itapúa"
 msgstr "Itapúa"
 
+msgid "Ituri"
+msgstr "Ituri"
+
 msgid "Ivano-Frankivska oblast"
 msgstr "Ivano-Frankivsk, Provincie"
 
+msgid "Ivanovskaja oblast'"
+msgstr "Ivanovo, Oblast"
+
 msgid "Ivančna Gorica"
 msgstr "Ivancna Gorica"
 
 msgid "Iwate"
 msgstr "Iwate"
 
 msgid "Izabal"
@@ -4907,23 +5300,32 @@
 
 msgid "Jamalpur"
 msgstr "Jamalpur"
 
 msgid "Jambi"
 msgstr "Jambi"
 
+msgid "Jammu and Kashmīr"
+msgstr "Jammu en Kasjmir"
+
 msgid "Jan Mayen (Arctic Region)"
 msgstr "Jan Mayen (Arctische regio)"
 
 msgid "Janakpur"
 msgstr "Janakpur"
 
 msgid "Janūb Sīnā'"
 msgstr "Zuidelijke Sinaï"
 
+msgid "Janūb al Bāţinah"
+msgstr "Gouvernement Zuid Al Batinah"
+
+msgid "Janūb ash Sharqīyah"
+msgstr "Gouvernement Zuid Ash Sharqiyah"
+
 msgid "Jarash"
 msgstr "Jerash"
 
 msgid "Jardin Exotique"
 msgstr "Jardin Exotique"
 
 msgid "Jaroslavskaja oblast'"
@@ -4982,14 +5384,17 @@
 
 msgid "Jeollanam-do"
 msgstr "Jeollanam-do; Zuid-Jeolla"
 
 msgid "Jerada"
 msgstr "Jerada"
 
+msgid "Jericho and Al Aghwar"
+msgstr "Jericho - Al Aghwar"
+
 msgid "Jerusalem"
 msgstr "Jeruzalem"
 
 msgid "Jesenice"
 msgstr "Jesenice"
 
 msgid "Jeseník"
@@ -5000,14 +5405,17 @@
 
 msgid "Jhalakathi"
 msgstr "Jhalokati"
 
 msgid "Jhenaidah"
 msgstr "Jhenaidah"
 
+msgid "Jhārkhand"
+msgstr "Jharkhand"
+
 msgid "Jiangsu Sheng"
 msgstr "Jiangsu, Provincie"
 
 msgid "Jiangxi Sheng"
 msgstr "Jiangxi, Provincie"
 
 msgid "Jigawa"
@@ -5054,14 +5462,17 @@
 
 msgid "Jonava"
 msgstr "Jonava"
 
 msgid "Jonglei"
 msgstr "Jonquali"
 
+msgid "Joniškis"
+msgstr "Joniškis"
+
 msgid "Jowzjān"
 msgstr "Jowzjan"
 
 msgid "Joypurhat"
 msgstr "Jaipurhat"
 
 msgid "Jubbada Dhexe"
@@ -5138,14 +5549,17 @@
 
 msgid "Kaabong"
 msgstr "Kaabong"
 
 msgid "Kabale"
 msgstr "Kabale"
 
+msgid "Kabardino-Balkarskaja Respublika"
+msgstr "Kabardië-Balkarië, Republiek"
+
 msgid "Kabarole"
 msgstr "Kabarole"
 
 msgid "Kaberamaido"
 msgstr "Kaberamaido"
 
 msgid "Kachin"
@@ -5186,26 +5600,32 @@
 
 msgid "Kainuu"
 msgstr "Kainuu"
 
 msgid "Kairouan"
 msgstr "Kairouan"
 
+msgid "Kaišiadorys"
+msgstr "Kaišiadorys"
+
 msgid "Kajiado"
 msgstr "Kajiado"
 
 msgid "Kakamega"
 msgstr "Kakamega"
 
 msgid "Kalangala"
 msgstr "Kalangala"
 
 msgid "Kalasin"
 msgstr "Kalasin"
 
+msgid "Kaldrananeshreppur"
+msgstr "Kaldrananeshreppur"
+
 msgid "Kalimantan"
 msgstr "Kalimantan"
 
 msgid "Kalimantan Barat"
 msgstr "West-Kalimantan"
 
 msgid "Kalimantan Selatan"
@@ -5216,26 +5636,41 @@
 
 msgid "Kalimantan Timur"
 msgstr "Oost-Kalimantan"
 
 msgid "Kalimantan Utara"
 msgstr "Noord-Kalimantan"
 
+msgid "Kalinga"
+msgstr "Kalinga"
+
+msgid "Kaliningradskaja oblast'"
+msgstr "Kaliningrad, Oblast"
+
 msgid "Kaliro"
 msgstr "Kaliro"
 
 msgid "Kalkara"
 msgstr "Kalkara"
 
 msgid "Kalmar län [SE-08]"
 msgstr "Kalmar län"
 
+msgid "Kalmykija, Respublika"
+msgstr "Kalmukkië, Republiek"
+
+msgid "Kalutara"
+msgstr "Kalutara"
+
 msgid "Kaluzhskaya oblast'"
 msgstr "Kaloega, Oblast"
 
+msgid "Kalvarijos"
+msgstr "Kalvarija"
+
 msgid "Kambja"
 msgstr "Kambja"
 
 msgid "Kamchatskiy kray"
 msgstr "Kamtsjatka, Kraj"
 
 msgid "Kamnik"
@@ -5243,17 +5678,26 @@
 
 msgid "Kampala"
 msgstr "Kampala"
 
 msgid "Kamphaeng Phet"
 msgstr "Kamphaeng Phet"
 
+msgid "Kampong Chaam"
+msgstr "Kampong Cham"
+
 msgid "Kampong Chhnang"
 msgstr "Kampong Chhnang"
 
+msgid "Kampong Spueu"
+msgstr "Kampong Spoe"
+
+msgid "Kampong Thum"
+msgstr "Kampong Thum"
+
 msgid "Kampot"
 msgstr "Kampot"
 
 msgid "Kamuli"
 msgstr "Kamuli"
 
 msgid "Kamwenge"
@@ -5264,26 +5708,35 @@
 
 msgid "Kanal"
 msgstr "Kanal"
 
 msgid "Kanchanaburi"
 msgstr "Kanchanaburi"
 
+msgid "Kandaal"
+msgstr "Kandal"
+
 msgid "Kandahār"
 msgstr "Kandahar"
 
 msgid "Kandavas novads"
 msgstr "Kandava"
 
+msgid "Kandy"
+msgstr "Kandy"
+
 msgid "Kanem"
 msgstr "Kanem"
 
 msgid "Kanepi"
 msgstr "Kanepi"
 
+msgid "Kangweonto"
+msgstr "Kangwŏn-do"
+
 msgid "Kankan"
 msgstr "Kankan"
 
 msgid "Kano"
 msgstr "Kano"
 
 msgid "Kansas"
@@ -5291,14 +5744,17 @@
 
 msgid "Kanta-Häme"
 msgstr "Kanta-Häme"
 
 msgid "Kanungu"
 msgstr "Kanungu"
 
+msgid "Kaoh Kong"
+msgstr "Koh Kong"
+
 msgid "Kaohsiung"
 msgstr "Kaohsiung"
 
 msgid "Kaolack"
 msgstr "Kaolack"
 
 msgid "Kapchorwa"
@@ -5315,47 +5771,65 @@
 
 msgid "Karagandinskaja oblast'"
 msgstr "Karaganda, Provincie"
 
 msgid "Karaman"
 msgstr "Karaman"
 
+msgid "Karbalā’"
+msgstr "Karbala"
+
 msgid "Karbinci"
 msgstr "Karbinci"
 
 msgid "Kardzhali"
 msgstr "Kardzjali"
 
+msgid "Karelija, Respublika"
+msgstr "Karelië, Republiek"
+
 msgid "Karlovarský kraj"
 msgstr "Karlsbad, Regio"
 
 msgid "Karlovačka županija"
 msgstr "Karlovac, Provincie"
 
 msgid "Karlovy Vary"
 msgstr "Karlsbad"
 
 msgid "Karnali"
 msgstr "Karnali"
 
+msgid "Karnātaka"
+msgstr "Karnataka"
+
 msgid "Karonga"
 msgstr "Karonga"
 
+msgid "Karpoš †"
+msgstr "Karpoš †"
+
 msgid "Kars"
 msgstr "Kars"
 
 msgid "Karuzi"
 msgstr "Karuzi"
 
 msgid "Karviná"
 msgstr "Karviná"
 
 msgid "Kasaï"
 msgstr "Kasaï"
 
+msgid "Kasaï Central"
+msgstr "Centraal-Kasaï"
+
+msgid "Kasaï Oriental"
+msgstr "Oost-Kasaï"
+
 msgid "Kasese"
 msgstr "Kasese"
 
 msgid "Kassala"
 msgstr "Kassala"
 
 msgid "Kasserine"
@@ -5387,14 +5861,20 @@
 
 msgid "Kauno miestas"
 msgstr "Kauno miestas"
 
 msgid "Kavadarci"
 msgstr "Kavadarci"
 
+msgid "Kavango East"
+msgstr "Kavango-Oost"
+
+msgid "Kavango West"
+msgstr "Kavango-West"
+
 msgid "Kayah"
 msgstr "Kayah"
 
 msgid "Kayangel"
 msgstr "Kayangel"
 
 msgid "Kayanza"
@@ -5408,38 +5888,47 @@
 
 msgid "Kayseri"
 msgstr "Kayseri"
 
 msgid "Kayunga"
 msgstr "Kayunga"
 
+msgid "Kazlų Rūdos"
+msgstr "Kazlų Rūda"
+
 msgid "Kebbi"
 msgstr "Kebbi"
 
 msgid "Kecskemét"
 msgstr "Kecskemét"
 
 msgid "Kedah"
 msgstr "Kedah"
 
 msgid "Keelung"
 msgstr "Keelung"
 
+msgid "Kegalla"
+msgstr "Kegalle"
+
 msgid "Kehtna"
 msgstr "Kehtna"
 
 msgid "Keila"
 msgstr "Keila"
 
 msgid "Kelantan"
 msgstr "Kelantan"
 
 msgid "Kelmė"
 msgstr "Kelmė"
 
+msgid "Kemerovskaja oblast'"
+msgstr "Kemerovo, Oblast"
+
 msgid "Kemö-Gïrïbïngï"
 msgstr "Kémo"
 
 msgid "Kensington and Chelsea"
 msgstr "Kensington en Chelsea"
 
 msgid "Kent"
@@ -5516,26 +6005,41 @@
 
 msgid "Khomas"
 msgstr "Khomas"
 
 msgid "Khon Kaen"
 msgstr "Khon Kaen"
 
+msgid "Khorāsān-e Jonūbī"
+msgstr "Zuid-Khorasan"
+
+msgid "Khorāsān-e Raẕavī"
+msgstr "Razavi-Khorasan"
+
+msgid "Khorāsān-e Shomālī"
+msgstr "Noord-Khorasan"
+
 msgid "Khouribga"
 msgstr "Khouribga"
 
 msgid "Khulna"
 msgstr "Khulna"
 
 msgid "Khyber Pakhtunkhwa"
 msgstr "Khyber Pakhtunkhwa"
 
 msgid "Khánh Hòa"
 msgstr "Khanh Hoa"
 
+msgid "Khémisset"
+msgstr "Khémisset"
+
+msgid "Khénifra"
+msgstr "Khénifra"
+
 msgid "Khōst"
 msgstr "Khost"
 
 msgid "Khūzestān"
 msgstr "Khoezistan"
 
 msgid "Kiambu"
@@ -5567,14 +6071,17 @@
 
 msgid "Kilifi"
 msgstr "Kilifi"
 
 msgid "Kilimanjaro"
 msgstr "Kilimanjaro"
 
+msgid "Kilinochchi"
+msgstr "Kilinochchi"
+
 msgid "Kilis"
 msgstr "Kilis"
 
 msgid "Kilkenny"
 msgstr "Kilkenny"
 
 msgid "Kindia"
@@ -5603,23 +6110,32 @@
 
 msgid "Kirklees"
 msgstr "Kirklees"
 
 msgid "Kirkop"
 msgstr "Kirkop"
 
+msgid "Kirkūk"
+msgstr "Kirkuk"
+
 msgid "Kirovohradska oblast"
 msgstr "Kirovohrad, Provincie"
 
+msgid "Kirovskaja oblast'"
+msgstr "Kirov, Oblast"
+
 msgid "Kiruhura"
 msgstr "Kiruhura"
 
 msgid "Kirundo"
 msgstr "Kirundo"
 
+msgid "Kisela Voda †"
+msgstr "Kisela Voda †"
+
 msgid "Kishoreganj"
 msgstr "Kishoreganj"
 
 msgid "Kisii"
 msgstr "Kisii"
 
 msgid "Kisoro"
@@ -5639,20 +6155,29 @@
 
 msgid "Kié-Ntem"
 msgstr "Kié-Ntem"
 
 msgid "Kičevo"
 msgstr "Kičevo"
 
+msgid "Kjósarhreppur"
+msgstr "Kjósarhreppur"
+
 msgid "Kladno"
 msgstr "Kladno"
 
 msgid "Klaipėda"
 msgstr "Klaipėda"
 
+msgid "Klaipėdos apskritis"
+msgstr "Klaipėda"
+
+msgid "Klaipėdos miestas"
+msgstr "Klaipėda"
+
 msgid "Klatovy"
 msgstr "Klatovy"
 
 msgid "Knowsley"
 msgstr "Knowsley"
 
 msgid "Kobarid"
@@ -5672,14 +6197,17 @@
 
 msgid "Kocēnu novads"
 msgstr "Kocēnu novads"
 
 msgid "Kogi"
 msgstr "Kogi"
 
+msgid "Kohgīlūyeh va Bowyer Aḩmad"
+msgstr "Kohgiluyeh en Boyer Ahmad"
+
 msgid "Kohila"
 msgstr "Kohila"
 
 msgid "Kohtla-Järve"
 msgstr "Kohtla-Järve"
 
 msgid "Kokneses novads"
@@ -5783,14 +6311,17 @@
 
 msgid "Kostanajskaja oblast'"
 msgstr "Qostanay, Provincie"
 
 msgid "Kostel"
 msgstr "Kostel"
 
+msgid "Kostromskaja oblast'"
+msgstr "Kostroma, Oblast"
+
 msgid "Kotayk'"
 msgstr "Kotayk'"
 
 msgid "Kotido"
 msgstr "Kotido"
 
 msgid "Kotor"
@@ -5831,26 +6362,32 @@
 
 msgid "Košický kraj"
 msgstr "Košice, Regio"
 
 msgid "Krabi"
 msgstr "Krabi"
 
+msgid "Kracheh"
+msgstr "Kracheh"
+
 msgid "Kraj Vysočina"
 msgstr "Vysočina, Regio"
 
 msgid "Kranj"
 msgstr "Kranj"
 
 msgid "Kranjska Gora"
 msgstr "Kranjska Gora"
 
 msgid "Krapinsko-zagorska županija"
 msgstr "Krapina-Zagorje, Provincie"
 
+msgid "Krasnodarskij kraj"
+msgstr "Krasnodar, Kraj"
+
 msgid "Krasnojarskij kraj"
 msgstr "Krasnojarsk, Kraj"
 
 msgid "Kratovo"
 msgstr "Kratovo"
 
 msgid "Kretinga"
@@ -5918,35 +6455,53 @@
 
 msgid "Kunene"
 msgstr "Kunene"
 
 msgid "Kungota"
 msgstr "Kungota"
 
+msgid "Kupiškis"
+msgstr "Kupiškis"
+
+msgid "Kurganskaja oblast'"
+msgstr "Koergan, Oblast"
+
 msgid "Kurigram"
 msgstr "Kurigram"
 
+msgid "Kurskaja oblast'"
+msgstr "Koersk, Oblast"
+
+msgid "Kurunegala"
+msgstr "Kurunegala"
+
 msgid "Kushtia"
 msgstr "Kushtia"
 
 msgid "Kutná Hora"
 msgstr "Kutná Hora"
 
 msgid "Kuusalu"
 msgstr "Kuusalu"
 
 msgid "Kuzma"
 msgstr "Kuzma"
 
+msgid "Kvemo Kartli"
+msgstr "Kvemo Kartli"
+
 msgid "Kwajalein"
 msgstr "Kwajalein"
 
 msgid "Kwale"
 msgstr "Kwale"
 
+msgid "Kwango"
+msgstr "Kwango"
+
 msgid "Kwara"
 msgstr "Kwara"
 
 msgid "Kwazulu-Natal"
 msgstr "Kwazulu-Natal"
 
 msgid "Kweneng"
@@ -5987,14 +6542,17 @@
 
 msgid "Kénédougou"
 msgstr "Kénédougou"
 
 msgid "Kérouané"
 msgstr "Kérouané"
 
+msgid "Kópavogsbær"
+msgstr "Kópavogur"
+
 msgid "Kürdəmir"
 msgstr "Kurdamir"
 
 msgid "Kütahya"
 msgstr "Kütahya"
 
 msgid "Kābul"
@@ -6092,14 +6650,17 @@
 
 msgid "La Unión"
 msgstr "La Unión"
 
 msgid "La Vega"
 msgstr "La Vega"
 
+msgid "Laborie"
+msgstr "Laborie"
+
 msgid "Labé"
 msgstr "Labé"
 
 msgid "Lacs"
 msgstr "Lacs"
 
 msgid "Ladākh"
@@ -6167,14 +6728,17 @@
 
 msgid "Lancashire"
 msgstr "Lancashire"
 
 msgid "Landes"
 msgstr "Landes"
 
+msgid "Langanesbyggð"
+msgstr "Langanesbyggð"
+
 msgid "Laois"
 msgstr "Laois"
 
 msgid "Lappi"
 msgstr "Lapland"
 
 msgid "Lara"
@@ -6272,14 +6836,17 @@
 
 msgid "Lenart"
 msgstr "Lenart"
 
 msgid "Lendava"
 msgstr "Lendava"
 
+msgid "Leningradskaja oblast'"
+msgstr "Leningrad, Oblast"
+
 msgid "Leova"
 msgstr "Leova"
 
 msgid "Leribe"
 msgstr "Leribe"
 
 msgid "Lerik"
@@ -6377,14 +6944,17 @@
 
 msgid "Lindi"
 msgstr "Lindi"
 
 msgid "Line Islands"
 msgstr "Line-eilanden"
 
+msgid "Lipeckaja oblast'"
+msgstr "Lipetsk, Oblast"
+
 msgid "Lipkovo"
 msgstr "Lipkovo"
 
 msgid "Lira"
 msgstr "Lira"
 
 msgid "Lisboa"
@@ -6566,14 +7136,17 @@
 
 msgid "Loški Potok"
 msgstr "Loski Potok"
 
 msgid "Loṙi"
 msgstr "Lori"
 
+msgid "Lualaba"
+msgstr "Lualaba"
+
 msgid "Luanda"
 msgstr "Luanda"
 
 msgid "Luapula"
 msgstr "Luapula"
 
 msgid "Lubelskie"
@@ -6746,14 +7319,17 @@
 
 msgid "Mae Hong Son"
 msgstr "Mae Hong Son"
 
 msgid "Mafeteng"
 msgstr "Mafeteng"
 
+msgid "Magadanskaja oblast'"
+msgstr "Magadan, Oblast"
+
 msgid "Magallanes"
 msgstr "Magallanes"
 
 msgid "Magdalena"
 msgstr "Magdalena"
 
 msgid "Maguindanao"
@@ -6779,14 +7355,17 @@
 
 msgid "Mahdia"
 msgstr "Mahdia"
 
 msgid "Mahilioŭskaja voblasć"
 msgstr "Mahiljow, Provincie"
 
+msgid "Mahārāshtra"
+msgstr "Maharashtra"
+
 msgid "Mai-Ndombe"
 msgstr "Mai-Ndombe"
 
 msgid "Maine"
 msgstr "Maine"
 
 msgid "Maine-et-Loire"
@@ -6917,14 +7496,17 @@
 
 msgid "Manisa"
 msgstr "Manisa"
 
 msgid "Manitoba"
 msgstr "Manitoba"
 
+msgid "Mannar"
+msgstr "Mannar"
+
 msgid "Mantova"
 msgstr "Mantova"
 
 msgid "Manufahi"
 msgstr "Manufahi"
 
 msgid "Manus"
@@ -6962,14 +7544,20 @@
 
 msgid "Margibi"
 msgstr "Margibi"
 
 msgid "Maribor"
 msgstr "Maribor"
 
+msgid "Marij Èl, Respublika"
+msgstr "Mari El, Republiek"
+
+msgid "Marijampolė"
+msgstr "Marijampolė"
+
 msgid "Marijampolės apskritis"
 msgstr "Marijampolė (district)"
 
 msgid "Marinduque"
 msgstr "Marinduque"
 
 msgid "Markazī"
@@ -7064,20 +7652,26 @@
 
 msgid "Matabeleland South"
 msgstr "Matabeleland Zuid"
 
 msgid "Matagalpa"
 msgstr "Matagalpa"
 
+msgid "Matale"
+msgstr "Matale"
+
 msgid "Matam"
 msgstr "Matam"
 
 msgid "Matanzas"
 msgstr "Matanzas"
 
+msgid "Matara"
+msgstr "Matara"
+
 msgid "Matera"
 msgstr "Matera"
 
 msgid "Mato Grosso"
 msgstr "Mato Grosso"
 
 msgid "Mato Grosso do Sul"
@@ -7085,14 +7679,17 @@
 
 msgid "Maule"
 msgstr "Maule"
 
 msgid "Mauren"
 msgstr "Mauren"
 
+msgid "Mavrovo i Rostuše"
+msgstr "Mavrovo en Rostuša"
+
 msgid "Mayabeque"
 msgstr "Mayabeque"
 
 msgid "Mayaguana"
 msgstr "Mayaguana"
 
 msgid "Mayaro-Rio Claro"
@@ -7109,14 +7706,17 @@
 
 msgid "Mayo-Kebbi-Ouest"
 msgstr "Mayo-Kebbi Ouest"
 
 msgid "Mayotte"
 msgstr "Mayotte"
 
+msgid "Maysān"
+msgstr "Maysan"
+
 msgid "Mayuge"
 msgstr "Mayuge"
 
 msgid "Mazowieckie"
 msgstr "Masovië"
 
 msgid "Mazsalacas novads"
@@ -7127,14 +7727,17 @@
 
 msgid "Małopolskie"
 msgstr "Klein-Polen"
 
 msgid "Maţrūḩ"
 msgstr "Matruh"
 
+msgid "Mažeikiai"
+msgstr "Mažeikiai"
+
 msgid "Ma‘ān"
 msgstr "Ma'an"
 
 msgid "Ma’rib"
 msgstr "Ma'rib"
 
 msgid "Mbale"
@@ -7166,14 +7769,17 @@
 
 msgid "Medvode"
 msgstr "Medvode"
 
 msgid "Medway"
 msgstr "Medway"
 
+msgid "Meghālaya"
+msgstr "Meghalaya"
+
 msgid "Mehedinți"
 msgstr "Mehedinți"
 
 msgid "Meherpur"
 msgstr "Meherpur"
 
 msgid "Mejit"
@@ -7247,14 +7853,17 @@
 
 msgid "Michoacán de Ocampo"
 msgstr "Michoacán de Ocampo"
 
 msgid "Micoud"
 msgstr "Micoud"
 
+msgid "Mid Western"
+msgstr "Mid-Westers"
+
 msgid "Mid and East Antrim"
 msgstr "Mid and East Antrim"
 
 msgid "Mid-Ulster"
 msgstr "Mid Ulster"
 
 msgid "Middlesbrough"
@@ -7412,23 +8021,29 @@
 
 msgid "Monagas"
 msgstr "Monagas"
 
 msgid "Monaghan"
 msgstr "Monaghan"
 
+msgid "Monaragala"
+msgstr "Moneragala"
+
 msgid "Monastir"
 msgstr "Monastir"
 
 msgid "Mondol Kiri"
 msgstr "Mondol Kiri"
 
 msgid "Moneghetti"
 msgstr "Moneghetti"
 
+msgid "Mongala"
+msgstr "Mongala"
+
 msgid "Monggar"
 msgstr "Monggar"
 
 msgid "Monmouthshire [Sir Fynwy GB-FYN]"
 msgstr "Monmouthshire"
 
 msgid "Mono"
@@ -7496,14 +8111,17 @@
 
 msgid "Morazán"
 msgstr "Morazán"
 
 msgid "Morbihan"
 msgstr "Morbihan"
 
+msgid "Mordovija, Respublika"
+msgstr "Mordovië, Republiek"
+
 msgid "Morelos"
 msgstr "Morelos"
 
 msgid "Morobe"
 msgstr "Morobe"
 
 msgid "Morogoro"
@@ -7514,14 +8132,20 @@
 
 msgid "Moroto"
 msgstr "Moroto"
 
 msgid "Moselle"
 msgstr "Moezel"
 
+msgid "Mosfellsbær"
+msgstr "Mosfellsbær"
+
+msgid "Moskovskaja oblast'"
+msgstr "Moskou, Oblast"
+
 msgid "Moskva"
 msgstr "Moskou"
 
 msgid "Most"
 msgstr "Most"
 
 msgid "Mosta"
@@ -7574,14 +8198,17 @@
 
 msgid "Msida"
 msgstr "Msida"
 
 msgid "Mtarfa"
 msgstr "Mtarfa"
 
+msgid "Mtskheta-Mtianeti"
+msgstr "Mtscheta-Mtianeti"
+
 msgid "Mtwara"
 msgstr "Mtwara"
 
 msgid "Mubende"
 msgstr "Mubende"
 
 msgid "Mubārak al Kabīr"
@@ -7631,14 +8258,17 @@
 
 msgid "Murcia, Región de"
 msgstr "Murcia, Regio"
 
 msgid "Mureș"
 msgstr "Mureș"
 
+msgid "Murmanskaja oblast'"
+msgstr "Moermansk, Oblast"
+
 msgid "Murska Sobota"
 msgstr "Murska Sobota"
 
 msgid "Murzuq"
 msgstr "Murzuq"
 
 msgid "Musandam"
@@ -7697,14 +8327,17 @@
 
 msgid "México"
 msgstr "Mexico"
 
 msgid "Møre og Romsdal"
 msgstr "Møre og Romsdal"
 
+msgid "Mýrdalshreppur"
+msgstr "Mýrdalshreppur"
+
 msgid "Mādabā"
 msgstr "Madaba"
 
 msgid "Mālpils novads"
 msgstr "Mālpils"
 
 msgid "Mārupes novads"
@@ -7820,14 +8453,17 @@
 
 msgid "Namibe"
 msgstr "Namibe"
 
 msgid "Namosi"
 msgstr "Namosi"
 
+msgid "Nampho"
+msgstr "Namp'o"
+
 msgid "Nampula"
 msgstr "Nampula"
 
 msgid "Namu"
 msgstr "Namu"
 
 msgid "Namur"
@@ -7892,14 +8528,17 @@
 
 msgid "Narva-Jõesuu"
 msgstr "Narva-Jõesuu"
 
 msgid "Naryn"
 msgstr "Naryn, Provincie"
 
+msgid "Nasarawa"
+msgstr "Nassarawa"
+
 msgid "National Capital District (Port Moresby)"
 msgstr "National Capital District (Port Moresby)"
 
 msgid "National Capital Region"
 msgstr "Nationale Hoofstadregio"
 
 msgid "Natore"
@@ -7958,14 +8597,17 @@
 
 msgid "Negros Oriental"
 msgstr "Negros Oriental"
 
 msgid "Nei Mongol Zizhiqu"
 msgstr "Binnen-Mongolië, Autonome Regio"
 
+msgid "Nelson"
+msgstr "Nelson"
+
 msgid "Neneckij avtonomnyj okrug"
 msgstr "Nenetsië, Autonoom District"
 
 msgid "Neno"
 msgstr "Neno"
 
 msgid "Neretas novads"
@@ -8225,14 +8867,17 @@
 
 msgid "North Bank"
 msgstr "North Bank"
 
 msgid "North Carolina"
 msgstr "Noord-Carolina"
 
+msgid "North Central Province"
+msgstr "Noordelijke Centrale Provincie"
+
 msgid "North Dakota"
 msgstr "Noord-Dakota"
 
 msgid "North Darfur"
 msgstr "Noord-Darfoer"
 
 msgid "North East"
@@ -8276,14 +8921,17 @@
 
 msgid "North Tyneside"
 msgstr "Noord-Tyneside"
 
 msgid "North West"
 msgstr "Noord-West"
 
+msgid "North Western Province"
+msgstr "Noordwestelijke Provincie"
+
 msgid "North Yorkshire"
 msgstr "North Yorkshire"
 
 msgid "North-West"
 msgstr "Noord-West"
 
 msgid "North-Western"
@@ -8306,14 +8954,17 @@
 
 msgid "Northern Mariana Islands"
 msgstr "Noordelijke Marianen"
 
 msgid "Northern Mindanao (Region X)"
 msgstr "Northern Mindanao (Regio X)"
 
+msgid "Northern Province"
+msgstr "Noordelijke Provincie"
+
 msgid "Northern Region"
 msgstr "Noordelijke Regio"
 
 msgid "Northern Samar"
 msgstr "Northern Samar"
 
 msgid "Northern Territory"
@@ -8330,14 +8981,17 @@
 
 msgid "Norðurland eystra"
 msgstr "Noordland oost"
 
 msgid "Norðurland vestra"
 msgstr "Noordland west"
 
+msgid "Norðurþing"
+msgstr "Norðurþing"
+
 msgid "Nottingham"
 msgstr "Nottingham"
 
 msgid "Nottinghamshire"
 msgstr "Nottinghamshire"
 
 msgid "Nouaceur"
@@ -8369,20 +9023,26 @@
 
 msgid "Novaci"
 msgstr "Novaci"
 
 msgid "Novara"
 msgstr "Novara"
 
+msgid "Novgorodskaja oblast'"
+msgstr "Novgorod, Oblast"
+
 msgid "Novo Mesto"
 msgstr "Novo mesto"
 
 msgid "Novo Selo"
 msgstr "Novo Selo"
 
+msgid "Novosibirskaja oblast'"
+msgstr "Novosibirsk, Oblast"
+
 msgid "Nový Jičín"
 msgstr "Nový Jičín"
 
 msgid "Nsanje"
 msgstr "Nsanje"
 
 msgid "Ntcheu"
@@ -8435,14 +9095,17 @@
 
 msgid "Nusa Tenggara Barat"
 msgstr "West-Nusa Tenggara"
 
 msgid "Nusa Tenggara Timur"
 msgstr "Oost-Nusa Tenggara"
 
+msgid "Nuwara Eliya"
+msgstr "Nuwara Eliya"
+
 msgid "Nyamira"
 msgstr "Nyamira"
 
 msgid "Nyandarua"
 msgstr "Nyandarua"
 
 msgid "Nyanga"
@@ -8468,23 +9131,29 @@
 
 msgid "Nótio Aigaío"
 msgstr "Zuid-Egeïsche Eilanden"
 
 msgid "Nõo"
 msgstr "Nõo"
 
+msgid "Nāgāland"
+msgstr "Nagaland"
+
 msgid "Nālūt"
 msgstr "Nalut"
 
 msgid "Nīcas novads"
 msgstr "Nīca"
 
 msgid "Nīmrōz"
 msgstr "Nimroz"
 
+msgid "Nīnawá"
+msgstr "Ninawa"
+
 msgid "Nūristān"
 msgstr "Nooristan"
 
 msgid "Oaxaca"
 msgstr "Oaxaca"
 
 msgid "Oberösterreich"
@@ -8579,14 +9248,17 @@
 
 msgid "Omaheke"
 msgstr "Omaheke"
 
 msgid "Ombella-Mpoko"
 msgstr "Ombella-Mpoko"
 
+msgid "Omskaja oblast'"
+msgstr "Omsk, Oblast"
+
 msgid "Omusati"
 msgstr "Omusati"
 
 msgid "Ondo"
 msgstr "Ondo"
 
 msgid "Ontario"
@@ -8621,32 +9293,41 @@
 
 msgid "Oregon"
 msgstr "Oregon"
 
 msgid "Orellana"
 msgstr "Orellana"
 
+msgid "Orenburgskaja oblast'"
+msgstr "Orenburg, Oblast"
+
 msgid "Orhei"
 msgstr "Orhei"
 
 msgid "Orhon"
 msgstr "Orhon"
 
 msgid "Oristano"
 msgstr "Oristano"
 
 msgid "Orkney Islands"
 msgstr "Orkney-eilanden"
 
+msgid "Orlovskaja oblast'"
+msgstr "Orjol, Oblast"
+
 msgid "Ormož"
 msgstr "Ormoz"
 
 msgid "Orne"
 msgstr "Orne"
 
+msgid "Oromia"
+msgstr "Oromia"
+
 msgid "Oruro"
 msgstr "Oruro"
 
 msgid "Osaka"
 msgstr "Osaka"
 
 msgid "Osh"
@@ -8753,14 +9434,23 @@
 
 msgid "Ozolnieku novads"
 msgstr "Ozolnieki"
 
 msgid "Oğuz"
 msgstr "Oguz"
 
+msgid "P'yǒngan-bukto"
+msgstr "P'yŏngan-pukto"
+
+msgid "P'yǒngan-namdo"
+msgstr "P'yŏngan-namdo"
+
+msgid "P'yǒngyang"
+msgstr "Pyongyang"
+
 msgid "Pabna"
 msgstr "Pabna"
 
 msgid "Pader"
 msgstr "Pader"
 
 msgid "Padova"
@@ -8813,23 +9503,32 @@
 
 msgid "Pamplemousses"
 msgstr "Pamplemousses"
 
 msgid "Panamá"
 msgstr "Panama"
 
+msgid "Panamá Oeste"
+msgstr "Panama"
+
 msgid "Panchagarh"
 msgstr "Panchagarh"
 
 msgid "Pando"
 msgstr "Pando"
 
 msgid "Panevėžio apskritis"
 msgstr "Panevėžys (district)"
 
+msgid "Panevėžio miestas"
+msgstr "Panevėžys"
+
+msgid "Panevėžys"
+msgstr "Panevėžys"
+
 msgid "Pangasinan"
 msgstr "Pangasinaans"
 
 msgid "Panjshayr"
 msgstr "Panjshir"
 
 msgid "Paola"
@@ -8957,23 +9656,29 @@
 
 msgid "Penghu"
 msgstr "Penghu"
 
 msgid "Pennsylvania"
 msgstr "Pennsylvania"
 
+msgid "Penzenskaja oblast'"
+msgstr "Penza, Oblast"
+
 msgid "Perak"
 msgstr "Perak"
 
 msgid "Peravia"
 msgstr "Peravia"
 
 msgid "Perlis"
 msgstr "Perlis"
 
+msgid "Permskij kraj"
+msgstr "Perm, Kraj"
+
 msgid "Pernambuco"
 msgstr "Pernambuco"
 
 msgid "Pernik"
 msgstr "Pernik"
 
 msgid "Perth and Kinross"
@@ -9356,14 +10061,17 @@
 
 msgid "Prienai"
 msgstr "Prienai"
 
 msgid "Prilep"
 msgstr "Prilep"
 
+msgid "Primorskij kraj"
+msgstr "Primorje, Kraj"
+
 msgid "Primorsko-goranska županija"
 msgstr "Primorje-Gorski, Provincie"
 
 msgid "Prince Edward Island"
 msgstr "Prins Edwardeiland"
 
 msgid "Princes Town"
@@ -9377,14 +10085,23 @@
 
 msgid "Prostějov"
 msgstr "Prostějov"
 
 msgid "Provence-Alpes-Côte-d’Azur"
 msgstr "Provence-Alpes-Côte-d'Azur"
 
+msgid "Province 1"
+msgstr "Provincie 1"
+
+msgid "Province 2"
+msgstr "Provincie 2"
+
+msgid "Province 5"
+msgstr "Provincie 5"
+
 msgid "Príncipe"
 msgstr "Principe"
 
 msgid "Pskovskaja oblast'"
 msgstr "Pskov, Oblast"
 
 msgid "Ptuj"
@@ -9419,14 +10136,17 @@
 
 msgid "Puno"
 msgstr "Puno"
 
 msgid "Puntarenas"
 msgstr "Puntarenas"
 
+msgid "Puttalam"
+msgstr "Puttalam"
+
 msgid "Putumayo"
 msgstr "Putumayo"
 
 msgid "Puy-de-Dôme"
 msgstr "Puy-de-Dôme"
 
 msgid "Pyrénées-Atlantiques"
@@ -9593,20 +10313,26 @@
 
 msgid "Raasiku"
 msgstr "Raasiku"
 
 msgid "Rabat"
 msgstr "Rabat"
 
+msgid "Rabat Gozo"
+msgstr "Victoria"
+
 msgid "Rabat Malta"
 msgstr "Rabat Malta"
 
 msgid "Rabat-Salé-Kénitra"
 msgstr "Rabat-Salé-Kénitra"
 
+msgid "Rach'a-Lechkhumi-Kvemo Svaneti"
+msgstr "Ratsja-Letsjchoemi en Kvemo Svaneti"
+
 msgid "Radenci"
 msgstr "Radenci"
 
 msgid "Radeče"
 msgstr "Radece"
 
 msgid "Radlje ob Dravi"
@@ -9614,14 +10340,17 @@
 
 msgid "Radoviš"
 msgstr "Radoviš"
 
 msgid "Radovljica"
 msgstr "Radovljica"
 
+msgid "Radviliškis"
+msgstr "Radviliškis"
+
 msgid "Rae"
 msgstr "Rae"
 
 msgid "Rafah"
 msgstr "Rafah"
 
 msgid "Ragged Island"
@@ -9656,14 +10385,20 @@
 
 msgid "Rangamati"
 msgstr "Rangamati"
 
 msgid "Rangpur"
 msgstr "Rangpur"
 
+msgid "Rangárþing eystra"
+msgstr "Rangárþing eystra"
+
+msgid "Rangárþing ytra"
+msgstr "Rangárþing ytra"
+
 msgid "Rankovce"
 msgstr "Rankovce"
 
 msgid "Ranong"
 msgstr "Ranong"
 
 msgid "Rapla"
@@ -9752,14 +10487,17 @@
 
 msgid "Região Autónoma dos Açores"
 msgstr "Autonome Regio Azoren"
 
 msgid "Região Continental"
 msgstr "Continentale Regio"
 
+msgid "Região Insular"
+msgstr "Eilandenregio"
+
 msgid "Región Metropolitana de Santiago"
 msgstr "Santiago, Hoofdstedelijke Regio van"
 
 msgid "Rehamna"
 msgstr "Rehamna"
 
 msgid "Relizane"
@@ -9785,14 +10523,23 @@
 
 msgid "Retalhuleu"
 msgstr "Retalhuleu"
 
 msgid "Rewa"
 msgstr "Rewa"
 
+msgid "Reykhólahreppur"
+msgstr "Reykhólahreppur"
+
+msgid "Reykjanesbær"
+msgstr "Reykjanesbær"
+
+msgid "Reykjavíkurborg"
+msgstr "Reykjavik"
+
 msgid "Rezina"
 msgstr "Rezina"
 
 msgid "Rečica ob Savinji"
 msgstr "Rečica ob Savinji"
 
 msgid "Rheinland-Pfalz"
@@ -9851,14 +10598,20 @@
 
 msgid "Risaralda"
 msgstr "Risaralda"
 
 msgid "Rivas"
 msgstr "Rivas"
 
+msgid "River Cess"
+msgstr "River Cess"
+
+msgid "River Gee"
+msgstr "River Gee"
+
 msgid "River Nile"
 msgstr "Nijl"
 
 msgid "Rivera"
 msgstr "Rivera"
 
 msgid "Rivers"
@@ -9905,14 +10658,17 @@
 
 msgid "Roi Et"
 msgstr "Roi Et"
 
 msgid "Rojas novads"
 msgstr "Roja"
 
+msgid "Rokiškis"
+msgstr "Rokiškis"
+
 msgid "Rokycany"
 msgstr "Rokycany"
 
 msgid "Roma"
 msgstr "Rome"
 
 msgid "Romblon"
@@ -10001,14 +10757,17 @@
 
 msgid "Ruyigi"
 msgstr "Ruyigi"
 
 msgid "Ruše"
 msgstr "Ruse"
 
+msgid "Ryanggang-do"
+msgstr "Ryanggang-do"
+
 msgid "Rychnov nad Kněžnou"
 msgstr "Rychnov nad Kněžnou"
 
 msgid "Räpina"
 msgstr "Räpina"
 
 msgid "Río Negro"
@@ -10019,14 +10778,17 @@
 
 msgid "Rîșcani"
 msgstr "Rîșcani"
 
 msgid "Rõuge"
 msgstr "Rõuge"
 
+msgid "Rājasthān"
+msgstr "Rajasthan"
+
 msgid "Rēzekne"
 msgstr "Rēzekne (stad)"
 
 msgid "Rēzeknes novads"
 msgstr "Rēzekne"
 
 msgid "Rīf Dimashq"
@@ -10142,20 +10904,29 @@
 
 msgid "Saint John Figtree"
 msgstr "Saint John Figtree"
 
 msgid "Saint Joseph"
 msgstr "Saint Joseph"
 
+msgid "Saint Julian's"
+msgstr "San Ġiljan"
+
 msgid "Saint Kitts"
 msgstr "Saint Kitts"
 
+msgid "Saint Lawrence"
+msgstr "San Lawrenz"
+
 msgid "Saint Louis"
 msgstr "Saint Louis"
 
+msgid "Saint Lucia's"
+msgstr "Santa Luċija"
+
 msgid "Saint Lucy"
 msgstr "Saint Lucy"
 
 msgid "Saint Luke"
 msgstr "Saint Luke"
 
 msgid "Saint Mark"
@@ -10178,14 +10949,17 @@
 
 msgid "Saint Paul Capisterre"
 msgstr "Saint Paul Capisterre"
 
 msgid "Saint Paul Charlestown"
 msgstr "Saint Paul Charlestown"
 
+msgid "Saint Paul's Bay"
+msgstr "San Pawl il-Baħar"
+
 msgid "Saint Peter"
 msgstr "Saint Peter"
 
 msgid "Saint Peter Basseterre"
 msgstr "Saint Peter Basseterre"
 
 msgid "Saint Philip"
@@ -10286,32 +11060,41 @@
 
 msgid "Samangān"
 msgstr "Samangan"
 
 msgid "Samaná"
 msgstr "Samaná"
 
+msgid "Samar"
+msgstr "Samar"
+
 msgid "Samarqand"
 msgstr "Samarkand"
 
 msgid "Samarskaja oblast'"
 msgstr "Samara, Oblast"
 
 msgid "Samburu"
 msgstr "Samburu"
 
 msgid "Samdrup Jongkhar"
 msgstr "Samdrup Jongkhar"
 
+msgid "Samegrelo-Zemo Svaneti"
+msgstr "Samegrelo-Zemo Svaneti"
+
 msgid "Samsun"
 msgstr "Samsun"
 
 msgid "Samtse"
 msgstr "Samtse"
 
+msgid "Samtskhe-Javakheti"
+msgstr "Samtsche-Dzjavacheti"
+
 msgid "Samut Prakan"
 msgstr "Samut Prakan"
 
 msgid "Samut Sakhon"
 msgstr "Samut Sakhon"
 
 msgid "Samut Songkhram"
@@ -10388,14 +11171,17 @@
 
 msgid "Sankt Gallen"
 msgstr "Sankt Gallen"
 
 msgid "Sankt-Peterburg"
 msgstr "Sint-Petersburg"
 
+msgid "Sankuru"
+msgstr "Sankuru"
+
 msgid "Sanma"
 msgstr "Sanma"
 
 msgid "Sanmatenga"
 msgstr "Sanmatenga"
 
 msgid "Sannat"
@@ -10460,14 +11246,17 @@
 
 msgid "Sar-e Pul"
 msgstr "Sar-e Pol"
 
 msgid "Saraburi"
 msgstr "Saraburi"
 
+msgid "Saraj †"
+msgstr "Saraj †"
+
 msgid "Saramacca"
 msgstr "Saramacca"
 
 msgid "Sarangani"
 msgstr "Sarangani"
 
 msgid "Saratovskaja oblast'"
@@ -10589,14 +11378,17 @@
 
 msgid "Selibe Phikwe"
 msgstr "Selibe Phikwe"
 
 msgid "Selnica ob Dravi"
 msgstr "Selnica ob Dravi"
 
+msgid "Seltjarnarnesbær"
+msgstr "Seltjarnarnesbær"
+
 msgid "Sembabule"
 msgstr "Sembabule"
 
 msgid "Semienawi K’eyyĭḥ Baḥri"
 msgstr "Semenawi Keyih Bahri"
 
 msgid "Semily"
@@ -10652,14 +11444,17 @@
 
 msgid "Sevilla"
 msgstr "Sevilla"
 
 msgid "Sevnica"
 msgstr "Sevnica"
 
+msgid "Seyðisfjarðarkaupstaður"
+msgstr "Seyðisfjarðarkaupstaður"
+
 msgid "Sežana"
 msgstr "Sezana"
 
 msgid "Sfax"
 msgstr "Sfax"
 
 msgid "Shaanxi Sheng"
@@ -10670,14 +11465,23 @@
 
 msgid "Shabeellaha Hoose"
 msgstr "Neder-Shabelle"
 
 msgid "Shabwah"
 msgstr "Shabwah"
 
+msgid "Shamāl Sīnā'"
+msgstr "Noord-Sinaï"
+
+msgid "Shamāl al Bāţinah"
+msgstr "Gouvernement Noord Al Batinah"
+
+msgid "Shamāl ash Sharqīyah"
+msgstr "Gouvernement Noord Ash Sharqiyah"
+
 msgid "Shan"
 msgstr "Shan"
 
 msgid "Shandong Sheng"
 msgstr "Shandong, Provincie"
 
 msgid "Shanghai Shi"
@@ -10694,14 +11498,17 @@
 
 msgid "Sherpur"
 msgstr "Sherpur"
 
 msgid "Shetland Islands"
 msgstr "Shetland-eilanden"
 
+msgid "Shida Kartli"
+msgstr "Sjida Kartli"
+
 msgid "Shiga"
 msgstr "Shiga"
 
 msgid "Shimane"
 msgstr "Shimane"
 
 msgid "Shinyanga"
@@ -10868,32 +11675,47 @@
 
 msgid "Siġġiewi"
 msgstr "Siġġiewi"
 
 msgid "Sjælland"
 msgstr "Seeland"
 
+msgid "Skaftárhreppur"
+msgstr "Skaftárhreppur"
+
+msgid "Skagabyggð"
+msgstr "Skagabyggð"
+
+msgid "Skeiða- og Gnúpverjahreppur"
+msgstr "Skeiða- og Gnúpverjahreppur"
+
 msgid "Skhirate-Témara"
 msgstr "Skhirate-Témara"
 
 msgid "Skikda"
 msgstr "Skikda"
 
+msgid "Skorradalshreppur"
+msgstr "Skorradalshreppur"
+
 msgid "Skrundas novads"
 msgstr "Skrunda"
 
 msgid "Skrīveru novads"
 msgstr "Skrīveri"
 
 msgid "Skuodas"
 msgstr "Skuodas"
 
 msgid "Skåne län [SE-12]"
 msgstr "Skåne län"
 
+msgid "Skútustaðahreppur"
+msgstr "Skútustaðahreppur"
+
 msgid "Sliema"
 msgstr "Sliema"
 
 msgid "Sligo"
 msgstr "Sligo"
 
 msgid "Sliven"
@@ -10916,14 +11738,17 @@
 
 msgid "Smolenskaja oblast'"
 msgstr "Smolensk, Oblast"
 
 msgid "Smolyan"
 msgstr "Smoljan"
 
+msgid "Snæfellsbær"
+msgstr "Snæfellsbær"
+
 msgid "Soccsksargen (Region XII)"
 msgstr "Soccsksargen (Regio XII)"
 
 msgid "Sodražica"
 msgstr "Sodrazica"
 
 msgid "Sofala"
@@ -11111,14 +11936,17 @@
 
 msgid "Southern Leyte"
 msgstr "Southern Leyte"
 
 msgid "Southern Nations, Nationalities and Peoples"
 msgstr "Yedebub Biheroch Bihereseboch na Hizboch"
 
+msgid "Southern Province"
+msgstr "Zuidelijke Provincie"
+
 msgid "Southern Region"
 msgstr "Zuidelijke Regio"
 
 msgid "Southland"
 msgstr "Zuidland"
 
 msgid "Southwark"
@@ -11183,17 +12011,23 @@
 
 msgid "Stoke-on-Trent"
 msgstr "Stoke aan Trent"
 
 msgid "Stopiņu novads"
 msgstr "Stopiņi"
 
+msgid "Stoĕng Trêng"
+msgstr "Stoeng Treng"
+
 msgid "Strakonice"
 msgstr "Strakonice"
 
+msgid "Strandabyggð"
+msgstr "Strandabyggð"
+
 msgid "Straža"
 msgstr "Straža"
 
 msgid "Strenču novads"
 msgstr "Strenči"
 
 msgid "Struga"
@@ -11204,14 +12038,17 @@
 
 msgid "Strășeni"
 msgstr "Strășeni"
 
 msgid "Studeničani"
 msgstr "Studeničani"
 
+msgid "Stykkishólmsbær"
+msgstr "Stykkishólmsbær"
+
 msgid "Stînga Nistrului, unitatea teritorială din"
 msgstr "Transnistrië, Territoriale Eenheid"
 
 msgid "Středočeský kraj"
 msgstr "Midden-Bohemen, Regio"
 
 msgid "Suceava"
@@ -11234,14 +12071,17 @@
 
 msgid "Sud-Ouest"
 msgstr "Sud-Ouest"
 
 msgid "Sud-Ubangi"
 msgstr "Zuid-Ubangi"
 
+msgid "Sudūr Pashchim"
+msgstr "Sudurpashchim"
+
 msgid "Suffolk"
 msgstr "Suffolk"
 
 msgid "Sughd"
 msgstr "Sughd"
 
 msgid "Sukhothai"
@@ -11327,20 +12167,47 @@
 
 msgid "Suðurland"
 msgstr "Zuidland"
 
 msgid "Suðurnes"
 msgstr "Zuidelijk schiereiland"
 
+msgid "Suðurnesjabær"
+msgstr "Suðurnesjabær"
+
 msgid "Svaay Rieng"
 msgstr "Svay Rieng"
 
 msgid "Svalbard (Arctic Region)"
 msgstr "Spitsbergen (Arctische regio); Svalbard (Arctische regio)"
 
+msgid "Svalbarðshreppur"
+msgstr "Svalbarðshreppur"
+
+msgid "Svalbarðsstrandarhreppur"
+msgstr "Svalbarðsstrandarhreppur"
+
+msgid "Sveitarfélagið Hornafjörður"
+msgstr "Hornafjörður"
+
+msgid "Sveitarfélagið Skagafjörður"
+msgstr "Skagafjörður"
+
+msgid "Sveitarfélagið Skagaströnd"
+msgstr "Skagaströnd"
+
+msgid "Sveitarfélagið Vogar"
+msgstr "Sveitarfélagið Vogar"
+
+msgid "Sveitarfélagið Árborg"
+msgstr "Árborg"
+
+msgid "Sveitarfélagið Ölfus"
+msgstr "Ölfus"
+
 msgid "Sverdlovskaja oblast'"
 msgstr "Sverdlovsk, Oblast"
 
 msgid "Sveta Ana"
 msgstr "Sveta Ana"
 
 msgid "Sveti Nikole"
@@ -11429,14 +12296,17 @@
 
 msgid "Sóc Trăng"
 msgstr "Soc Trang"
 
 msgid "Södermanlands län [SE-04]"
 msgstr "Södermanlands län"
 
+msgid "Súðavíkurhreppur"
+msgstr "Súðavíkurhreppur"
+
 msgid "Sühbaatar"
 msgstr "Sühbaatar"
 
 msgid "Sălaj"
 msgstr "Sălaj"
 
 msgid "Sējas novads"
@@ -11450,14 +12320,17 @@
 
 msgid "Sơn La"
 msgstr "Son La"
 
 msgid "Sədərək"
 msgstr "Sadarak"
 
+msgid "Ta' Xbiex"
+msgstr "Ta' Xbiex"
+
 msgid "Taakaev"
 msgstr "Takev"
 
 msgid "Tabasco"
 msgstr "Tabasco"
 
 msgid "Tabor"
@@ -11543,14 +12416,17 @@
 
 msgid "Tambovskaja oblast'"
 msgstr "Tambov, Oblast"
 
 msgid "Tameside"
 msgstr "Tameside"
 
+msgid "Tamil Nādu"
+msgstr "Tamil Nadu"
+
 msgid "Tan-Tan (EH-partial)"
 msgstr "Tan-Tan (EH-gedeeltelijk)"
 
 msgid "Tana River"
 msgstr "Tana River"
 
 msgid "Tandjilé"
@@ -11558,14 +12434,17 @@
 
 msgid "Tanga"
 msgstr "Tanga"
 
 msgid "Tangail"
 msgstr "Tangail"
 
+msgid "Tanganyika"
+msgstr "Tanganyika"
+
 msgid "Tanger-Assilah"
 msgstr "Tanger-Assilah"
 
 msgid "Tanger-Tétouan-Al Hoceïma"
 msgstr "Tanger-Tétouan-Al Hoceïma"
 
 msgid "Tanintharyi"
@@ -11618,14 +12497,17 @@
 
 msgid "Tarn"
 msgstr "Tarn"
 
 msgid "Tarn-et-Garonne"
 msgstr "Tarn en Garonne"
 
+msgid "Taroudannt"
+msgstr "Taroudant"
+
 msgid "Tarrafal"
 msgstr "Tarrafal"
 
 msgid "Tarrafal de São Nicolau"
 msgstr "Tarrafal de São Nicolau"
 
 msgid "Tarragona [Tarragona]"
@@ -11636,14 +12518,17 @@
 
 msgid "Tartumaa"
 msgstr "Tartumaa"
 
 msgid "Tarxien"
 msgstr "Tarxien"
 
+msgid "Tasman"
+msgstr "Tasman"
+
 msgid "Tasmania"
 msgstr "Tasmanië"
 
 msgid "Tata"
 msgstr "Tata"
 
 msgid "Tatabánya"
@@ -11654,44 +12539,56 @@
 
 msgid "Tatarstan, Respublika"
 msgstr "Tatarije, Republiek; Tatarstan, Republiek"
 
 msgid "Tauragė"
 msgstr "Tauragė"
 
+msgid "Tauragės apskritis"
+msgstr "Tauragė"
+
 msgid "Tavuš"
 msgstr "Tavus"
 
 msgid "Tawi-Tawi"
 msgstr "Tawi-Tawi"
 
 msgid "Taza"
 msgstr "Taza"
 
 msgid "Tbilisi"
 msgstr "Tbilisi"
 
+msgid "Tbong Khmum"
+msgstr "Tbong Khmum"
+
 msgid "Tearce"
 msgstr "Tearce"
 
 msgid "Tehrān"
 msgstr "Teheran"
 
 msgid "Tekirdağ"
 msgstr "Tekirdağ"
 
+msgid "Telangāna"
+msgstr "Telangana"
+
 msgid "Telenești"
 msgstr "Telenești"
 
 msgid "Teleorman"
 msgstr "Teleorman"
 
 msgid "Telford and Wrekin"
 msgstr "Telford en Wrekin"
 
+msgid "Telšiai"
+msgstr "Telšiai"
+
 msgid "Telšių apskritis"
 msgstr "Telšiai (district)"
 
 msgid "Temburong"
 msgstr "Temburong"
 
 msgid "Temotu"
@@ -11786,14 +12683,17 @@
 
 msgid "Ticino"
 msgstr "Ticino"
 
 msgid "Tierra del Fuego"
 msgstr "Tierra del Fuego"
 
+msgid "Tigrai"
+msgstr "Tigray"
+
 msgid "Tillabéri"
 msgstr "Tillabéri"
 
 msgid "Timiș"
 msgstr "Timiș"
 
 msgid "Tindouf"
@@ -11834,14 +12734,17 @@
 
 msgid "Tiền Giang"
 msgstr "Tien Giang"
 
 msgid "Tjumenskaja oblast'"
 msgstr "Tjoemen, Oblast"
 
+msgid "Tjörneshreppur"
+msgstr "Tjörneshreppur"
+
 msgid "Tlaxcala"
 msgstr "Tlaxcala"
 
 msgid "Tlemcen"
 msgstr "Tlemcen"
 
 msgid "Toamasina"
@@ -11948,14 +12851,17 @@
 
 msgid "Trabzon"
 msgstr "Trabzon"
 
 msgid "Trafford"
 msgstr "Trafford"
 
+msgid "Trakai"
+msgstr "Trakai"
+
 msgid "Trang"
 msgstr "Trang"
 
 msgid "Trans Nzoia"
 msgstr "Trans-Nzoia"
 
 msgid "Trapani"
@@ -12116,14 +13022,17 @@
 
 msgid "Tábor"
 msgstr "Tábor"
 
 msgid "Táchira"
 msgstr "Táchira"
 
+msgid "Tálknafjarðarhreppur"
+msgstr "Tálknafjarðarhreppur"
+
 msgid "Tây Ninh"
 msgstr "Tay Ninh"
 
 msgid "Tébessa"
 msgstr "Tébessa"
 
 msgid "Télimélé"
@@ -12179,17 +13088,23 @@
 
 msgid "Uherské Hradiště"
 msgstr "Uherské Hradiště"
 
 msgid "Ujae"
 msgstr "Ujae"
 
+msgid "Ukmergė"
+msgstr "Ukmergė"
+
 msgid "Ul'janovskaja oblast'"
 msgstr "Oeljanovsk, Oblast"
 
+msgid "Ulaanbaatar"
+msgstr "Ulaanbaatar"
+
 msgid "Ulcinj"
 msgstr "Ulcinj"
 
 msgid "Ulsan-gwangyeoksi"
 msgstr "Ulsan Metropolitan City"
 
 msgid "Ulster"
@@ -12197,14 +13112,17 @@
 
 msgid "Umbria"
 msgstr "Umbrië"
 
 msgid "Umm al Qaywayn"
 msgstr "Umm al-Qawain"
 
+msgid "Umm Şalāl"
+msgstr "Umm Salal"
+
 msgid "Ungheni"
 msgstr "Ungheni"
 
 msgid "United States Minor Outlying Islands"
 msgstr "Kleine afgelegen eilanden van de Verenigde Staten"
 
 msgid "Unity"
@@ -12260,17 +13178,23 @@
 
 msgid "Uttar Pradesh"
 msgstr "Uttar Pradesh"
 
 msgid "Uttaradit"
 msgstr "Uttaradit"
 
+msgid "Uttarākhand"
+msgstr "Uttarakhand"
+
 msgid "Uusimaa"
 msgstr "Uusimaa"
 
+msgid "Uva Province"
+msgstr "Provincie Uva"
+
 msgid "Uvea"
 msgstr "Uvea"
 
 msgid "Uvs"
 msgstr "Uvs"
 
 msgid "Uíge"
@@ -12377,14 +13301,17 @@
 
 msgid "Varna"
 msgstr "Varna"
 
 msgid "Varsinais-Suomi"
 msgstr "Zuidwest-Finland"
 
+msgid "Varėna"
+msgstr "Varėna"
+
 msgid "Vas"
 msgstr "Vas"
 
 msgid "Vasilevo"
 msgstr "Vasilevo"
 
 msgid "Vaslui"
@@ -12398,14 +13325,17 @@
 
 msgid "Vaupés"
 msgstr "Vaupés"
 
 msgid "Vava'u"
 msgstr "Vava'u"
 
+msgid "Vavuniya"
+msgstr "Vavuniya"
+
 msgid "Vayoć Jor"
 msgstr "Vayoc Jor"
 
 msgid "Vecpiebalgas novads"
 msgstr "Vecpiebalga"
 
 msgid "Vecumnieku novads"
@@ -12470,14 +13400,20 @@
 
 msgid "Vestfold og Telemark"
 msgstr "Vestfold og Telemark"
 
 msgid "Vestland"
 msgstr "Vestland"
 
+msgid "Vestmannaeyjabær"
+msgstr "Vestmannaeyjabær"
+
+msgid "Vesturbyggð"
+msgstr "Vesturbyggð"
+
 msgid "Vesturland"
 msgstr "Westland"
 
 msgid "Veszprém"
 msgstr "Veszprém"
 
 msgid "Vevčani"
@@ -12536,14 +13472,17 @@
 
 msgid "Viljandi"
 msgstr "Viljandi"
 
 msgid "Viljandimaa"
 msgstr "Viljandimaa"
 
+msgid "Vilkaviškis"
+msgstr "Vilkaviškis"
+
 msgid "Villa Clara"
 msgstr "Villa Clara"
 
 msgid "Vilniaus apskritis"
 msgstr "Vilnius (district)"
 
 msgid "Vilniaus miestas"
@@ -12623,14 +13562,17 @@
 
 msgid "Volta"
 msgstr "Volta"
 
 msgid "Volynska oblast"
 msgstr "Wolynië, Provincie"
 
+msgid "Vopnafjarðarhreppur"
+msgstr "Vopnafjarðarhreppur"
+
 msgid "Vorarlberg"
 msgstr "Vorarlberg"
 
 msgid "Vormsi"
 msgstr "Vormsi"
 
 msgid "Voronezhskaya oblast'"
@@ -12839,14 +13781,17 @@
 
 msgid "Western Highlands"
 msgstr "Western Highlands"
 
 msgid "Western North"
 msgstr "Western North"
 
+msgid "Western Province"
+msgstr "Westelijke Provincie"
+
 msgid "Western Visayas (Region VI)"
 msgstr "Western Visayas (Regio VI)"
 
 msgid "Westmeath"
 msgstr "Westmeath"
 
 msgid "Westminster"
@@ -12926,14 +13871,20 @@
 
 msgid "Wyoming"
 msgstr "Wyoming"
 
 msgid "Wādī al Ḩayāt"
 msgstr "Wadi al Hayat"
 
+msgid "Wādī ash Shāţi’"
+msgstr "Wādī ash Shāţi’"
+
+msgid "Wāsiţ"
+msgstr "Wasit"
+
 msgid "Xagħra"
 msgstr "Xagħra"
 
 msgid "Xaignabouli"
 msgstr "Sainyabuli"
 
 msgid "Xaisômboun"
@@ -13118,14 +14069,17 @@
 
 msgid "Zalaegerszeg"
 msgstr "Zalaegerszeg"
 
 msgid "Zambales"
 msgstr "Zambales"
 
+msgid "Zambezi"
+msgstr "Zambezi"
+
 msgid "Zamboanga Peninsula (Region IX)"
 msgstr "Zamboanga Peninsula (Regio IX)"
 
 msgid "Zamboanga Sibugay"
 msgstr "Zamboanga Sibugay"
 
 msgid "Zamboanga del Norte"
@@ -13274,14 +14228,20 @@
 
 msgid "Ágion Óros"
 msgstr "Oros Athos"
 
 msgid "Água Grande"
 msgstr "Água Grande"
 
+msgid "Árneshreppur"
+msgstr "Árneshreppur"
+
+msgid "Ásahreppur"
+msgstr "Ásahreppur"
+
 msgid "Ávila"
 msgstr "Ávila"
 
 msgid "Åland"
 msgstr "Åland"
 
 msgid "Çanakkale"
@@ -13301,23 +14261,29 @@
 
 msgid "Évora"
 msgstr "Évora"
 
 msgid "Ípeiros"
 msgstr "Epirus"
 
+msgid "Ísafjarðarbær"
+msgstr "Ísafjarðarbær"
+
 msgid "Île-de-France"
 msgstr "Île-de-France"
 
 msgid "Ñeembucú"
 msgstr "Ñeembucú"
 
 msgid "Ñuble"
 msgstr "Ñuble"
 
+msgid "Ömnögovĭ"
+msgstr "Ömnögovĭ"
+
 msgid "Örebro län [SE-18]"
 msgstr "Örebro län"
 
 msgid "Östergötlands län [SE-05]"
 msgstr "Östergötlands län"
 
 msgid "Övörhangay"
@@ -13328,17 +14294,29 @@
 
 msgid "Ústí nad Labem"
 msgstr "Ústí nad Labem"
 
 msgid "Ústí nad Orlicí"
 msgstr "Ústí nad Orlicí"
 
+msgid "Þingeyjarsveit"
+msgstr "Þingeyjarsveit"
+
 msgid "Ādažu novads"
 msgstr "Ādaži"
 
+msgid "Āz̄ārbāyjān-e Ghārbī"
+msgstr "West-Azerbeidzjan"
+
+msgid "Āz̄ārbāyjān-e Shārqī"
+msgstr "Oost-Azerbeidzjan"
+
+msgid "Čair †"
+msgstr "Čair †"
+
 msgid "Čaška"
 msgstr "Čaška"
 
 msgid "Česká Lípa"
 msgstr "Česká Lípa"
 
 msgid "České Budějovice"
@@ -13355,14 +14333,17 @@
 
 msgid "Črna na Koroškem"
 msgstr "Crna na Koroskem"
 
 msgid "Črnomelj"
 msgstr "Crnomelj"
 
+msgid "Čučer-Sandevo"
+msgstr "Čučer-Sandevo"
+
 msgid "Điện Biên"
 msgstr "Dien Bien"
 
 msgid "Đà Nẵng"
 msgstr "Da Nang (stad)"
 
 msgid "Đắk Nông"
@@ -13412,14 +14393,17 @@
 
 msgid "Şabran"
 msgstr "Şabran"
 
 msgid "Şahbuz"
 msgstr "Sahbuz"
 
+msgid "Şalāḩ ad Dīn"
+msgstr "Salah ad Din"
+
 msgid "Şamaxı"
 msgstr "Samaxi"
 
 msgid "Şanlıurfa"
 msgstr "Şanlıurfa"
 
 msgid "Şanʻā’"
@@ -13442,17 +14426,23 @@
 
 msgid "Şəmkir"
 msgstr "Samkir"
 
 msgid "Şərur"
 msgstr "Sarur"
 
+msgid "Šakiai"
+msgstr "Šakiai"
+
 msgid "Šalovci"
 msgstr "Salovci"
 
+msgid "Šalčininkai"
+msgstr "Šalčininkai"
+
 msgid "Šavnik"
 msgstr "Šavnik"
 
 msgid "Šempeter-Vrtojba"
 msgstr "Sempeter-Vrtojba"
 
 msgid "Šentilj"
@@ -13466,23 +14456,38 @@
 
 msgid "Šentrupert"
 msgstr "Šentrupert"
 
 msgid "Šenčur"
 msgstr "Sencur"
 
+msgid "Šiauliai"
+msgstr "Šiauliai"
+
 msgid "Šiaulių apskritis"
 msgstr "Šiauliai (district)"
 
+msgid "Šiaulių miestas"
+msgstr "Šiauliai"
+
 msgid "Šibensko-kninska županija"
 msgstr "Sibenik-Knin, Provincie"
 
+msgid "Šilalė"
+msgstr "Šilalė"
+
+msgid "Šilutė"
+msgstr "Šilutė"
+
 msgid "Širak"
 msgstr "Sirak"
 
+msgid "Širvintos"
+msgstr "Širvintos"
+
 msgid "Škocjan"
 msgstr "Skocjan"
 
 msgid "Škofja Loka"
 msgstr "Skofja Loka"
 
 msgid "Škofljica"
@@ -13508,23 +14513,32 @@
 
 msgid "Šumadijski okrug"
 msgstr "Šumadija"
 
 msgid "Šumperk"
 msgstr "Šumperk"
 
+msgid "Šuto Orizari †"
+msgstr "Šuto Orizari †"
+
+msgid "Švenčionys"
+msgstr "Švenčionys"
+
 msgid "Ţarābulus"
 msgstr "Tarabulus"
 
 msgid "Ţarţūs"
 msgstr "Tartous; Tartus; Tartoes"
 
 msgid "Żabbar"
 msgstr "Żabbar"
 
+msgid "Żebbuġ Gozo"
+msgstr "Żebbuġ"
+
 msgid "Żebbuġ Malta"
 msgstr "Żebbuġ Malta"
 
 msgid "Żejtun"
 msgstr "Żejtun"
 
 msgid "Żurrieq"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-11-28 15:17+0000\n"
-"Last-Translator: Pander <pander@users.sourceforge.net>\n"
+"PO-Revision-Date: 2023-03-18 21:41+0000\n"
+"Last-Translator: Frans Spiesschaert <frans.spiesschaert@gmail.com>\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-3/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 "X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "British Antarctic Territory"
 msgstr "Brits Antarctisch Territorium"
 
 msgid "Burma, Socialist Republic of the Union of"
 msgstr "Birma, Socialistische Republiek van de Unie van"
@@ -100,9 +100,12 @@
 
 msgid "Wake Island"
 msgstr "Wake-eiland"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
 msgstr "Yemen, Republiek"
 
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Joegoslavië, (Socialistische) Federale Republiek"
+
 msgid "Zaire, Republic of"
 msgstr "Zaïre, Republiek"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_639-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-07-22 11:11+0000\n"
+"PO-Revision-Date: 2023-04-22 14:41+0000\n"
 "Last-Translator: Pander <pander@users.sourceforge.net>\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/iso-codes/"
 "iso-639-3/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "Aari"
 msgstr "Aari"
 
 msgid "Aasáx"
 msgstr "Aasáx"
@@ -347,14 +347,17 @@
 
 msgid "Aleut"
 msgstr "Aleut"
 
 msgid "Algerian Arabic"
 msgstr "Algerijns Arabisch"
 
+msgid "Algerian Jewish Sign Language"
+msgstr "Algerijns-joodse Gebarentaal"
+
 msgid "Algerian Saharan Arabic"
 msgstr "Algerijns Sahara Arabisch"
 
 msgid "Algerian Sign Language"
 msgstr "Algerijnse Gebarentaal"
 
 msgid "Algonquin"
@@ -791,14 +794,17 @@
 
 msgid "Ata"
 msgstr "Ata"
 
 msgid "Atampaya"
 msgstr "Atampaya"
 
+msgid "Atauran"
+msgstr "Wetarees"
+
 msgid "Athpariya"
 msgstr "Athpariya"
 
 msgid "Atong (Cameroon)"
 msgstr "Atong (Kameroen)"
 
 msgid "Atong (India)"
@@ -815,17 +821,14 @@
 
 msgid "Aushi"
 msgstr "Aushi"
 
 msgid "Aushiri"
 msgstr "Aushiri"
 
-msgid "Australian Aborigines Sign Language"
-msgstr "Australische Aborigines Gebarentaal"
-
 msgid "Austrian Sign Language"
 msgstr "Oostenrijkse Gebarentaal"
 
 msgid "Avar, Old"
 msgstr "Avaars, Oud"
 
 msgid "Avaric"
@@ -2294,14 +2297,17 @@
 
 msgid "Callawalla"
 msgstr "Callawalla"
 
 msgid "Caluyanun"
 msgstr "Caluyanun"
 
+msgid "Cambodian Sign Language"
+msgstr "Cambodjaanse Gebarentaal"
+
 msgid "Cameroon Pidgin"
 msgstr "Kameroens Pidgin"
 
 msgid "Canichana"
 msgstr "Canichana"
 
 msgid "Cara"
@@ -3308,14 +3314,17 @@
 
 msgid "Ipulo"
 msgstr "Ipulo"
 
 msgid "Iquito"
 msgstr "Iquito"
 
+msgid "Iranian Sign Language"
+msgstr "Iraanse Gebarentaal"
+
 msgid "Irish"
 msgstr "Iers"
 
 msgid "Irish Sign Language"
 msgstr "Ierse Gebarentaal"
 
 msgid "Irish, Middle (900-1200)"
@@ -3725,14 +3734,17 @@
 
 msgid "Libyan Arabic"
 msgstr "Libisch Arabisch"
 
 msgid "Libyan Sign Language"
 msgstr "Lybische Gebarentaal"
 
+msgid "Lidzonka"
+msgstr "Dzodinka"
+
 msgid "Limbu"
 msgstr "Limbu"
 
 msgid "Limos Kalinga"
 msgstr "Limos Kalinga"
 
 msgid "Linear A"
@@ -4973,14 +4985,17 @@
 
 msgid "Slovenian"
 msgstr "Sloveens"
 
 msgid "Sogdian"
 msgstr "Sogdiaans"
 
+msgid "Solomon Islands Sign Language"
+msgstr "Solomon Eilanden Gebarentaal"
+
 msgid "Solong"
 msgstr "Solong"
 
 msgid "Som"
 msgstr "Kirgizische som"
 
 msgid "Somali"
@@ -5213,14 +5228,17 @@
 
 msgid "Thangal Naga"
 msgstr "Thangal Naga"
 
 msgid "Tibetan"
 msgstr "Tibetaans"
 
+msgid "Tibetan Sign Language"
+msgstr "Tibetaanse Gebarentaal"
+
 msgid "Tibetan, Amdo"
 msgstr "Tibetaans, Amdo"
 
 msgid "Tigre"
 msgstr "Tigre"
 
 msgid "Tigrinya"
@@ -5438,14 +5456,17 @@
 
 msgid "Welsh"
 msgstr "Welsh"
 
 msgid "Welsh Romani"
 msgstr "Wales Romani"
 
+msgid "West Bengal Sign Language"
+msgstr "West Bengaalse Gebarentaal"
+
 msgid "West Coast Bajau"
 msgstr "Westkust Bajau"
 
 msgid "Western Abnaki"
 msgstr "Westelijk Abnaki"
 
 msgid "Western Bru"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,104 +1,108 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: nn\n"
+"Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2013-02-12 13:17+0100\n"
-"Last-Translator: Haavard Korsvoll\n"
-"Language-Team: Norwegian Nynorsk <i18n-nn@lister.ping.uio.no>\n"
-"Language: nn\n"
+"PO-Revision-Date: 2023-02-24 21:01+0000\n"
+"Last-Translator: Anders Jonsson <anders.jonsson@norsjovallen.se>\n"
+"Language-Team: Swedish <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-3/sv/>\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Lokalize 1.4\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 msgid "British Antarctic Territory"
-msgstr "Britisk antarktis"
+msgstr "Brittiska antarktiska territoriet"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Unionen Myanmar"
+msgstr "Burman, socialistrepubliken"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Den sovjetiske sosialistiske republikk kviterussland"
+msgstr "Vitryska SSR"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Kanton og Endebury øyane"
+msgstr "Canton och Enderburyöarna"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Tsjekkoslovakia, tsjekkoslovakisk sosialistisk republikk"
+msgstr "Tjeckoslovakien, tjeckoslovakiska socialistrepubliken"
 
 msgid "Dahomey"
 msgstr "Dahomey"
 
 msgid "Dronning Maud Land"
-msgstr "Dronning Maud Land"
+msgstr "Drottning Mauds land"
 
 msgid "East Timor"
-msgstr "Aust-Timor"
+msgstr "Östtimor"
 
 msgid "France, Metropolitan"
-msgstr "Metropolitan-Frankrike"
+msgstr "Frankrike, Metropolitan"
 
 msgid "French Afars and Issas"
-msgstr "Fransk Afars og Issas"
+msgstr "Franska Afars och Issas"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Franske sørlege og antarktiske territorium"
+msgstr "Franska antarktiska och sydterritorierna"
 
 msgid "German Democratic Republic"
-msgstr "Den tyske demokratiske republikken"
+msgstr "Tyska demokratiska republiken"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Gilbert og Ellice-øyane"
+msgstr "Gilbert och Elliceöarna"
 
 msgid "Johnston Island"
-msgstr "Johnstonøyane"
+msgstr "Johnstonön"
 
 msgid "Midway Islands"
-msgstr "Midwayøyane"
+msgstr "Midwayöarna"
 
 msgid "Netherlands Antilles"
-msgstr "Dei nederlandske Antillane"
+msgstr "Nederländska Antillerna"
 
 msgid "Neutral Zone"
-msgstr "Nøytral sone"
+msgstr "Neutral zon"
 
 msgid "New Hebrides"
-msgstr "Nye hebridane"
+msgstr "Nya Hebriderna"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Stillehavsøyane (trust territory)"
+msgstr "Stillahavsöar (trust territory)"
 
 msgid "Panama Canal Zone"
-msgstr "Panama kanalsone"
+msgstr "Panamas kanalzon"
 
 msgid "Serbia and Montenegro"
-msgstr "Serbia og Montenegro"
+msgstr "Serbien och Montenegro"
 
 msgid "Sikkim"
 msgstr "Sikkim"
 
 msgid "Southern Rhodesia"
-msgstr "Sør-Rhodesia"
+msgstr "Södra Rhodesia"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "US ymse stillehavsøyar"
+msgstr "Diverse amerikanska stillahavsöar"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "SSSR, Sambandet av Sosialistiske Sovjet-Republikkar"
+msgstr "Sovjetunionen"
 
 msgid "Upper Volta, Republic of"
-msgstr "Republikken Øvre Volta"
+msgstr "Övre Volta, republiken"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Den demokratiske republikken Vietnam"
+msgstr "Vietnam, demokratiska republiken"
 
 msgid "Wake Island"
-msgstr "Wake Island"
+msgstr "Wakeöarna"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr "Den demokratiske folkerepublikken Jemen"
+msgstr "Jemen, demokratiska, demokratiska folkrepubliken"
+
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Jugoslavien, socialistiska federativa republiken"
 
 msgid "Zaire, Republic of"
-msgstr "Republikken Zaire"
+msgstr "Zaire, republiken"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,1269 +1,1256 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-06-03 20:17+0000\n"
-"Last-Translator: Quentin PAGÈS <quentinantonin@free.fr>\n"
-"Language-Team: Occitan <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-1/oc/>\n"
-"Language: oc\n"
+"PO-Revision-Date: 2018-11-30 15:08+0000\n"
+"Last-Translator: Andrei POPESCU <andreimpopescu@gmail.com>\n"
+"Language-Team: Romanian <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-1/ro/>\n"
+"Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.13-dev\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
+"20)) ? 1 : 2;\n"
+"X-Generator: Weblate 3.3\n"
+"X-Launchpad-Export-Date: 2010-08-16 11:01+0000\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albania"
 
 msgid "Algeria"
-msgstr "Argeria"
+msgstr "Algeria"
 
 msgid "American Samoa"
-msgstr "Samoa americana"
+msgstr "Samoa americană"
 
 msgid "Andorra"
-msgstr "Andòrra"
+msgstr "Andora"
 
 msgid "Angola"
-msgstr "Angòla"
+msgstr "Angola"
 
 msgid "Anguilla"
 msgstr "Anguilla"
 
 msgid "Antarctica"
-msgstr "Antartica"
+msgstr "Antarctica"
 
 msgid "Antigua and Barbuda"
-msgstr "Antigua e Barbuda"
+msgstr "Antigua și Barbuda"
 
 msgid "Arab Republic of Egypt"
-msgstr "Republica araba d’Egipte"
+msgstr "Republica arabă Egipt"
 
 msgid "Argentina"
 msgstr "Argentina"
 
 msgid "Argentine Republic"
-msgstr "Republica argentina"
+msgstr "Republica Argentina"
 
 msgid "Armenia"
 msgstr "Armenia"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
 msgstr "Australia"
 
 msgid "Austria"
-msgstr "Àustria"
+msgstr "Austria"
 
 msgid "Azerbaijan"
-msgstr "Azerbaitjan"
+msgstr "Azerbaijan"
 
 msgid "Bahamas"
 msgstr "Bahamas"
 
 msgid "Bahrain"
-msgstr "Barein"
+msgstr "Bahrein"
 
 msgid "Bangladesh"
-msgstr "Bangladèsh"
+msgstr "Bangladeș"
 
 msgid "Barbados"
-msgstr "Barbada"
+msgstr "Barbados"
 
 msgid "Belarus"
-msgstr "Bielorussia"
+msgstr "Bielorusia"
 
 msgid "Belgium"
-msgstr "Belgica"
+msgstr "Belgia"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
 msgstr "Benin"
 
 msgid "Bermuda"
-msgstr "Bermudas"
+msgstr "Bermude"
 
 msgid "Bhutan"
-msgstr "Botan"
+msgstr "Bhutan"
 
 msgid "Bolivarian Republic of Venezuela"
-msgstr "Republica bolivariana de Venecuèla"
+msgstr "Republica Bolivariană a Venezuelei"
 
 msgid "Bolivia"
 msgstr "Bolivia"
 
 msgid "Bolivia, Plurinational State of"
-msgstr "Bolívia, Estat plurinacional de"
+msgstr "Bolivia"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire, Sant Eustaqui e Saba"
+msgstr "Bonaire, Sint Eustatius și Saba"
 
 msgid "Bosnia and Herzegovina"
-msgstr "Bòsnia e Ercegovina"
+msgstr "Bosnia și Herțegovina"
 
 msgid "Botswana"
 msgstr "Botswana"
 
 msgid "Bouvet Island"
-msgstr "Illa Bouvet"
+msgstr "Insula Bouvet"
 
 msgid "Brazil"
-msgstr "Brasil"
+msgstr "Brazilia"
 
 msgid "British Indian Ocean Territory"
-msgstr "Territòris britanics de l'ocean indian"
+msgstr "Teritoriul britanic din Oceanul Indian"
 
 msgid "British Virgin Islands"
-msgstr "Illas Verges britanicas"
+msgstr "Insulele virgine britanice"
 
 msgid "Brunei Darussalam"
 msgstr "Brunei"
 
 msgid "Bulgaria"
 msgstr "Bulgaria"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
 msgid "Burundi"
 msgstr "Burundi"
 
 msgid "Cabo Verde"
-msgstr "Cap Verd"
+msgstr "Capul Verde"
 
 msgid "Cambodia"
-msgstr "Cambòtja"
+msgstr "Cambogia"
 
 msgid "Cameroon"
-msgstr "Cameron"
+msgstr "Camerun"
 
 msgid "Canada"
-msgstr "Canadà"
+msgstr "Canada"
 
 msgid "Cayman Islands"
-msgstr "Illas Caiman"
+msgstr "Insulele Caiman"
 
 msgid "Central African Republic"
-msgstr "Republica de Centrafrica"
+msgstr "Republica Central Africană"
 
 msgid "Chad"
-msgstr "Chad"
+msgstr "Ciad"
 
 msgid "Chile"
 msgstr "Chile"
 
 msgid "China"
 msgstr "China"
 
 msgid "Christmas Island"
-msgstr "Illa Cristmas"
+msgstr "Insula Crăciunului"
 
 msgid "Cocos (Keeling) Islands"
-msgstr "Illas Cocos (Keeling)"
+msgstr "Insulele Cocos (Keeling)"
 
 msgid "Colombia"
-msgstr "Colombia"
+msgstr "Columbia"
 
 msgid "Commonwealth of Dominica"
-msgstr "Commonwealth de la Dominica"
+msgstr "Comitatul Dominican"
 
 msgid "Commonwealth of the Bahamas"
-msgstr "Commonwealth de las Bahamas"
+msgstr "Comitatul Bahamas"
+
+msgid "Commonwealth of the Northern Mariana Islands"
+msgstr "Comitatul Insulelor Mariane Nordice"
 
 msgid "Comoros"
-msgstr "Comòras"
+msgstr "Comoros"
 
 msgid "Congo"
-msgstr "Còngo"
+msgstr "Congo"
 
 msgid "Congo, The Democratic Republic of the"
-msgstr "Còngo, Republica Democratica de"
+msgstr "Congo, Republica democrată"
 
 msgid "Cook Islands"
-msgstr "Illas Cook"
+msgstr "Insulele Cook"
 
 msgid "Costa Rica"
-msgstr "Còsta Rica"
+msgstr "Costa Rica"
 
 msgid "Croatia"
-msgstr "Croàcia"
+msgstr "Croația"
 
 msgid "Cuba"
 msgstr "Cuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Chipre"
+msgstr "Cipru"
 
 msgid "Czech Republic"
-msgstr "Republica chèca"
+msgstr "Cehia"
 
 msgid "Czechia"
-msgstr "Chequia"
+msgstr "Cehia"
 
 msgid "Côte d'Ivoire"
-msgstr "Còsta d'Evòri"
+msgstr "Coasta de Fildeș"
 
 msgid "Democratic People's Republic of Korea"
-msgstr "Republica populara democratica de Corèa"
+msgstr "Republica populară democrată Coreea"
 
 msgid "Democratic Republic of Sao Tome and Principe"
-msgstr "Republica Democratica de São Tomé e Príncipe"
+msgstr "Republica democrată Sao Tome și Principe"
+
+msgid "Democratic Republic of Timor-Leste"
+msgstr "Republica democrată Timorul de Est"
 
 msgid "Democratic Socialist Republic of Sri Lanka"
-msgstr "Republica Democratica Socialista d'Sri Lanka"
+msgstr "Republica socialistă democrată Sri Lanka"
 
 msgid "Denmark"
-msgstr "Danemarc"
+msgstr "Danemarca"
 
 msgid "Djibouti"
-msgstr "Jiboti"
+msgstr "Djibouti"
 
 msgid "Dominica"
 msgstr "Dominica"
 
 msgid "Dominican Republic"
-msgstr "Republica Dominicana"
+msgstr "Republica Dominicană"
 
 msgid "Eastern Republic of Uruguay"
-msgstr "Republica orientala d’Uruguai"
+msgstr "Republica Estică Uruguay"
 
 msgid "Ecuador"
-msgstr "Eqüator"
+msgstr "Ecuador"
 
 msgid "Egypt"
-msgstr "Egipte"
+msgstr "Egipt"
 
 msgid "El Salvador"
 msgstr "El Salvador"
 
 msgid "Equatorial Guinea"
-msgstr "Guinèa eqüatoriala"
+msgstr "Guinea Ecuatorială"
 
 msgid "Eritrea"
-msgstr "Eritrèa"
+msgstr "Eritreea"
 
 msgid "Estonia"
-msgstr "Estònia"
-
-msgid "Eswatini"
-msgstr "Eswatini"
+msgstr "Estonia"
 
 msgid "Ethiopia"
 msgstr "Etiopia"
 
 msgid "Falkland Islands (Malvinas)"
-msgstr "Illas Falkand (Malvinas)"
+msgstr "Insulele Falkland (Insulele Malvine)"
 
 msgid "Faroe Islands"
-msgstr "Illas Feròe"
+msgstr "Insulele Feroe"
 
 msgid "Federal Democratic Republic of Ethiopia"
-msgstr "Republica Democratica Federala d'Etiopia"
+msgstr "Republica federală democrată Etiopia"
 
 msgid "Federal Democratic Republic of Nepal"
-msgstr "Republica democratica federala del Nepam"
+msgstr "Republica federală democrată Nepal"
 
 msgid "Federal Republic of Germany"
-msgstr "Republica federala d’Alemanha"
+msgstr "Republica federală Germană"
 
 msgid "Federal Republic of Nigeria"
-msgstr "Republica federala del Nigèria"
+msgstr "Republica federală Nigeria"
 
 msgid "Federal Republic of Somalia"
-msgstr "Republica federala de Somalia"
+msgstr "Republica Federală Somalia"
 
 msgid "Federated States of Micronesia"
-msgstr "Estats federats de Micronesia"
+msgstr "Statele federale ale Microneziei"
 
 msgid "Federative Republic of Brazil"
-msgstr "Republica federativa de Brasil"
+msgstr "Republica federală Brazilia"
 
 msgid "Fiji"
 msgstr "Fiji"
 
 msgid "Finland"
-msgstr "Finlàndia"
+msgstr "Finlanda"
 
 msgid "France"
-msgstr "França"
+msgstr "Franța"
 
 msgid "French Guiana"
-msgstr "Guaiana francesa"
+msgstr "Guiana Franceză"
 
 msgid "French Polynesia"
-msgstr "Polinesia francesa"
+msgstr "Polinezia Franceză"
 
 msgid "French Republic"
-msgstr "Republica francesa"
+msgstr "Republica Franceză"
 
 msgid "French Southern Territories"
-msgstr "Tèrras australas francesas"
+msgstr "Teritoriile franceze de sud"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gabonese Republic"
-msgstr "Republica gabonesa"
+msgstr "Republica Gabon"
 
 msgid "Gambia"
-msgstr "Gàmbia"
+msgstr "Gambia"
 
 msgid "Georgia"
 msgstr "Georgia"
 
 msgid "Germany"
-msgstr "Alemanha"
+msgstr "Germania"
 
 msgid "Ghana"
-msgstr "Gana"
+msgstr "Ghana"
 
 msgid "Gibraltar"
-msgstr "Gibartar"
+msgstr "Gibraltar"
 
 msgid "Grand Duchy of Luxembourg"
-msgstr "Grand Ducat de Luxemborg"
+msgstr "Marele Ducat al Luxemburgului"
 
 msgid "Greece"
-msgstr "Grècia"
+msgstr "Grecia"
 
 msgid "Greenland"
-msgstr "Groenlàndia"
+msgstr "Groenlanda"
 
 msgid "Grenada"
-msgstr "Granada"
+msgstr "Grenada"
 
 msgid "Guadeloupe"
-msgstr "Guadalope"
+msgstr "Guadelupa"
 
 msgid "Guam"
 msgstr "Guam"
 
 msgid "Guatemala"
 msgstr "Guatemala"
 
 msgid "Guernsey"
-msgstr "Guernesey"
+msgstr "Guernsey"
 
 msgid "Guinea"
-msgstr "Guinèa"
+msgstr "Guinea"
 
 msgid "Guinea-Bissau"
-msgstr "Guinèa-Bissau"
+msgstr "Guinea-Bissau"
 
 msgid "Guyana"
 msgstr "Guyana"
 
 msgid "Haiti"
-msgstr "Haití"
+msgstr "Haiti"
 
 msgid "Hashemite Kingdom of Jordan"
-msgstr "Reialme Hashimita de Jordania"
+msgstr "Regatul Hașemit Iordanian"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Illas Heard e McDonald"
+msgstr "Insula Heard și Insulele McDonald"
 
 msgid "Hellenic Republic"
-msgstr "Republica ellenica"
+msgstr "Republica Elenă"
 
 msgid "Holy See (Vatican City State)"
-msgstr "Santa Ses (Estat de la Ciutat de Vatican)"
+msgstr "Vatican"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
 msgstr "Hong Kong"
 
 msgid "Hong Kong Special Administrative Region of China"
-msgstr "Region administrativa especiala chinesa de Honk Hong"
+msgstr "Regiunea Chineză cu administrare specială Hong Kong"
 
 msgid "Hungary"
-msgstr "Ongria"
+msgstr "Ungaria"
 
 msgid "Iceland"
-msgstr "Islàndia"
+msgstr "Islanda"
 
 msgid "Independent State of Papua New Guinea"
-msgstr "Estat independent de Papoa-Nòva Guinèa"
+msgstr "Statul Independent Papua Noua Guinee"
 
 msgid "Independent State of Samoa"
-msgstr "Estat independent de Samoa"
+msgstr "Statul Independent Samoa"
 
 msgid "India"
-msgstr "Índia"
+msgstr "India"
 
 msgid "Indonesia"
-msgstr "Indonesia"
+msgstr "Indonezia"
 
 msgid "Iran, Islamic Republic of"
-msgstr "Republica Dominicana"
+msgstr "Iran, Republica islamică"
 
 msgid "Iraq"
-msgstr "Iraq"
+msgstr "Irak"
 
 msgid "Ireland"
 msgstr "Irlanda"
 
 msgid "Islamic Republic of Afghanistan"
-msgstr "Republica Dominicana"
+msgstr "Republica islamică Afganistan"
 
 msgid "Islamic Republic of Iran"
-msgstr "Republica Dominicana"
+msgstr "Republica islamică Iran"
 
 msgid "Islamic Republic of Mauritania"
-msgstr "Republica islamica de Mauritània"
+msgstr "Republica islamică Mauritania"
 
 msgid "Islamic Republic of Pakistan"
-msgstr "Republica islamica de Paquistan"
+msgstr "Republica islamică Pakistan"
 
 msgid "Isle of Man"
-msgstr "Illa de Man"
+msgstr "Insula Man"
 
 msgid "Israel"
 msgstr "Israel"
 
 msgid "Italian Republic"
-msgstr "Republica italiana"
+msgstr "Republica Italiană"
 
 msgid "Italy"
-msgstr "Itàlia"
+msgstr "Italia"
 
 msgid "Jamaica"
 msgstr "Jamaica"
 
 msgid "Japan"
-msgstr "Japon"
+msgstr "Japonia"
 
 msgid "Jersey"
-msgstr "Jersei"
+msgstr "Jersey"
 
 msgid "Jordan"
-msgstr "Jordania"
+msgstr "Iordania"
 
 msgid "Kazakhstan"
-msgstr "Cazacstan"
+msgstr "Kazakhstan"
 
 msgid "Kenya"
-msgstr "Kenya"
+msgstr "Kenia"
 
 msgid "Kingdom of Bahrain"
-msgstr "Reialme de Bahrain"
+msgstr "Regatul Bahrein"
 
 msgid "Kingdom of Belgium"
-msgstr "Reialme de Belgica"
+msgstr "Regatul Belgiei"
 
 msgid "Kingdom of Bhutan"
-msgstr "Reialme de Botan"
+msgstr "Regatul Bhutan"
 
 msgid "Kingdom of Cambodia"
-msgstr "Reialme de Cambòtja"
+msgstr "Regatul Cambodgiei"
 
 msgid "Kingdom of Denmark"
-msgstr "Reialme de Danemarc"
-
-msgid "Kingdom of Eswatini"
-msgstr "Reialme d'Eswatini"
+msgstr "Regatul Danemarcei"
 
 msgid "Kingdom of Lesotho"
-msgstr "Reialme de Lesotho"
+msgstr "Regatul Lesotho"
 
 msgid "Kingdom of Morocco"
-msgstr "Reialme de Marròc"
+msgstr "Regatul Marocului"
 
 msgid "Kingdom of Norway"
-msgstr "Reialme de Norvègia"
+msgstr "Regatul Norvegiei"
 
 msgid "Kingdom of Saudi Arabia"
-msgstr "Reialme d’Arabia Saudita"
+msgstr "Regatul Arabiei Saudite"
 
 msgid "Kingdom of Spain"
-msgstr "Reialme d'Espanha"
+msgstr "Regatul Spaniei"
 
 msgid "Kingdom of Sweden"
-msgstr "Reialme de Suècia"
+msgstr "Regatul Suediei"
 
 msgid "Kingdom of Thailand"
-msgstr "Reialme de Tailàndia"
+msgstr "Regatul Tailandei"
 
 msgid "Kingdom of Tonga"
-msgstr "Reialme de Tònga"
+msgstr "Regatul Tonga"
 
 msgid "Kingdom of the Netherlands"
-msgstr "Reialme dels Païses Basses"
+msgstr "Regatul Olandei"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea, Democratic People's Republic of"
-msgstr "Corèa, Republica Populara Democratica de"
+msgstr "Republica democrată populară Coreea"
 
 msgid "Korea, Republic of"
-msgstr "Corèa, republica de"
+msgstr "Republica Coreea"
 
 msgid "Kuwait"
-msgstr "Koweit"
+msgstr "Kuweit"
 
 msgid "Kyrgyz Republic"
-msgstr "Republica Dominicana"
+msgstr "Republica kârgâză"
 
 msgid "Kyrgyzstan"
-msgstr "Kirguizstan"
+msgstr "Kârgâzstan"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Republica democratica populara del Laos"
+msgstr "Republica populară democrată Lao"
 
 msgid "Latvia"
-msgstr "Letònia"
+msgstr "Letonia"
 
 msgid "Lebanese Republic"
-msgstr "Republica libanesa"
+msgstr "Republica Libaneză"
 
 msgid "Lebanon"
 msgstr "Liban"
 
 msgid "Lesotho"
-msgstr "Lesoto"
+msgstr "Lesotho"
 
 msgid "Liberia"
-msgstr "Libèria"
+msgstr "Liberia"
 
 msgid "Libya"
 msgstr "Libia"
 
 msgid "Liechtenstein"
 msgstr "Liechtenstein"
 
 msgid "Lithuania"
-msgstr "Lituània"
+msgstr "Lituania"
 
 msgid "Luxembourg"
-msgstr "Luxemborg"
+msgstr "Luxemburg"
 
 msgid "Macao"
-msgstr "Macau"
+msgstr "Macao"
 
 msgid "Macao Special Administrative Region of China"
-msgstr "Region administrativa especiala chinesa de Macau"
+msgstr "Regiunea chineză cu administrare specială Macao"
 
 msgid "Madagascar"
 msgstr "Madagascar"
 
 msgid "Malawi"
 msgstr "Malawi"
 
 msgid "Malaysia"
-msgstr "Malàisia"
+msgstr "Malaezia"
 
 msgid "Maldives"
-msgstr "Maldivas"
+msgstr "Maldive"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Illas Marshall"
+msgstr "Insulele Marshall"
 
 msgid "Martinique"
 msgstr "Martinica"
 
 msgid "Mauritania"
-msgstr "Mauritània"
+msgstr "Mauritania"
 
 msgid "Mauritius"
-msgstr "Maurici"
+msgstr "Maurițius"
 
 msgid "Mayotte"
-msgstr "Maiòta"
+msgstr "Mayotte"
 
 msgid "Mexico"
 msgstr "Mexic"
 
 msgid "Micronesia, Federated States of"
-msgstr "Micronesia, Estats Federats de"
+msgstr "Micronesia, Statele federale ale"
 
 msgid "Moldova"
-msgstr "Moldàvia"
+msgstr "Moldova"
 
 msgid "Moldova, Republic of"
-msgstr "Moldàvia, Republica de"
+msgstr "Moldova, Republica"
 
 msgid "Monaco"
-msgstr "Mónegue"
+msgstr "Monaco"
 
 msgid "Mongolia"
 msgstr "Mongolia"
 
 msgid "Montenegro"
-msgstr "Montenegro"
+msgstr "Muntenegru"
 
 msgid "Montserrat"
 msgstr "Montserrat"
 
 msgid "Morocco"
-msgstr "Marròc"
+msgstr "Maroc"
 
 msgid "Mozambique"
-msgstr "Moçambic"
+msgstr "Mozambic"
 
 msgid "Myanmar"
-msgstr "Birmania"
+msgstr "Myanmar"
 
 msgid "Namibia"
 msgstr "Namibia"
 
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepal"
 
 msgid "Netherlands"
-msgstr "Païses Basses"
+msgstr "Olanda"
 
 msgid "New Caledonia"
-msgstr "Nòva Caledònia"
+msgstr "Noua Caledonie"
 
 msgid "New Zealand"
-msgstr "Novèla Zelanda"
+msgstr "Noua Zeelandă"
 
 msgid "Nicaragua"
 msgstr "Nicaragua"
 
 msgid "Niger"
-msgstr "Nigèr"
+msgstr "Niger"
 
 msgid "Nigeria"
-msgstr "Nigèria"
+msgstr "Nigeria"
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
-msgstr "Illa Norfolk"
-
-msgid "North Korea"
-msgstr "Corèa del Nòrd"
-
-msgid "North Macedonia"
-msgstr "Macedònia del Nòrd"
+msgstr "Insula Norfolk"
 
 msgid "Northern Mariana Islands"
-msgstr "Illas Marianas del Nòrd"
+msgstr "Insulele Mariane de Nord"
 
 msgid "Norway"
-msgstr "Norvègia"
+msgstr "Norvegia"
 
 msgid "Oman"
 msgstr "Oman"
 
 msgid "Pakistan"
-msgstr "Paquistan"
+msgstr "Pakistan"
 
 msgid "Palau"
-msgstr "Belau"
+msgstr "Palau"
 
 msgid "Palestine, State of"
-msgstr "Palestina, estat de"
+msgstr "Palestina, Statul"
 
 msgid "Panama"
-msgstr "Panamà"
+msgstr "Panama"
 
 msgid "Papua New Guinea"
-msgstr "Papoa Nòva Guinèa"
+msgstr "Papua Noua Guinee"
 
 msgid "Paraguay"
-msgstr "Paraguai"
+msgstr "Paraguay"
 
 msgid "People's Democratic Republic of Algeria"
-msgstr "Republica Argeriana Democratica e Populara"
+msgstr "Republica populară Democratică Algeria"
 
 msgid "People's Republic of Bangladesh"
-msgstr "Republica populara de Bangladèsh"
+msgstr "Republica populară Bangladeș"
 
 msgid "People's Republic of China"
-msgstr "Republica populara de China"
+msgstr "Republica populară Chineză"
 
 msgid "Peru"
-msgstr "Peró"
+msgstr "Peru"
 
 msgid "Philippines"
-msgstr "Filipinas"
+msgstr "Filipine"
 
 msgid "Pitcairn"
-msgstr "Illa de Pitcairn"
+msgstr "Pitcairn"
 
 msgid "Plurinational State of Bolivia"
-msgstr "Estat plurinacional de Bolívia"
+msgstr "Statul plurinațional al Boliviei"
 
 msgid "Poland"
-msgstr "Polonha"
+msgstr "Polonia"
 
 msgid "Portugal"
-msgstr "Portugal"
+msgstr "Portugalia"
 
 msgid "Portuguese Republic"
-msgstr "Republica portuguesa"
+msgstr "Republica Portugheză"
 
 msgid "Principality of Andorra"
-msgstr "Principat d'Andòrra"
+msgstr "Principatul Andorra"
 
 msgid "Principality of Liechtenstein"
-msgstr "Principat de Liechtenstein"
+msgstr "Principatul Liechtenstein"
 
 msgid "Principality of Monaco"
-msgstr "Principat de Mónegue"
+msgstr "Principatul Monaco"
 
 msgid "Puerto Rico"
 msgstr "Puerto Rico"
 
 msgid "Qatar"
 msgstr "Qatar"
 
 msgid "Republic of Albania"
-msgstr "Republica d'Albania"
+msgstr "Republica Albania"
 
 msgid "Republic of Angola"
-msgstr "Republica d’Angòla"
+msgstr "Republica Angola"
 
 msgid "Republic of Armenia"
-msgstr "Republicar d'Armenia"
+msgstr "Republica Armenia"
 
 msgid "Republic of Austria"
-msgstr "Republica d'Àustria"
+msgstr "Republica Austria"
 
 msgid "Republic of Azerbaijan"
-msgstr "Republica d’Azerbaitjan"
+msgstr "Republica Azerbaijan"
 
 msgid "Republic of Belarus"
-msgstr "Republica de Bielorussia"
+msgstr "Republica Bielorusă"
 
 msgid "Republic of Benin"
-msgstr "Republica del Benin"
+msgstr "Republica Benin"
 
 msgid "Republic of Bosnia and Herzegovina"
-msgstr "Republica de Bòsnia e Ercegovina"
+msgstr "Republica Bosnia-Herțegovina"
 
 msgid "Republic of Botswana"
-msgstr "Republica de Botswana"
+msgstr "Republica Botswana"
 
 msgid "Republic of Bulgaria"
-msgstr "Republica de Bulgaria"
+msgstr "Republica Bulgară"
 
 msgid "Republic of Burundi"
-msgstr "Republica de Burundi"
+msgstr "Republica Burundi"
 
 msgid "Republic of Cabo Verde"
-msgstr "Republica del Cap Verd"
+msgstr "Republica Capul Verde"
 
 msgid "Republic of Cameroon"
-msgstr "Republica de Cameron"
+msgstr "Republica Camerun"
 
 msgid "Republic of Chad"
-msgstr "Republica del Chad"
+msgstr "Republica Ciad"
 
 msgid "Republic of Chile"
-msgstr "Republica del Chile"
+msgstr "Republica Chile"
 
 msgid "Republic of Colombia"
-msgstr "Republica de Colómbia"
+msgstr "Republica Columbia"
 
 msgid "Republic of Costa Rica"
-msgstr "Republica de la Còsta Rica"
+msgstr "Republica Costa Rica"
 
 msgid "Republic of Croatia"
-msgstr "Republica de Croàcia"
+msgstr "Republica Croația"
 
 msgid "Republic of Cuba"
-msgstr "Republica de Cuba"
+msgstr "Republica Cuba"
 
 msgid "Republic of Cyprus"
-msgstr "Republica de Chipre"
+msgstr "Republica Cipru"
 
 msgid "Republic of Côte d'Ivoire"
-msgstr "Republica de Còsta d'Evòri"
+msgstr "Republica Coasta de Fildeș"
 
 msgid "Republic of Djibouti"
-msgstr "Republica de Jiboti"
+msgstr "Republica Djibouti"
 
 msgid "Republic of Ecuador"
-msgstr "Republica de l'Eqüator"
+msgstr "Republica Ecuador"
 
 msgid "Republic of El Salvador"
-msgstr "Republica del Salvador"
+msgstr "Republica El Salvador"
 
 msgid "Republic of Equatorial Guinea"
-msgstr "Republica de Guinèa Eqüatoriala"
+msgstr "Republica Guinea Ecuatorială"
 
 msgid "Republic of Estonia"
-msgstr "Republica d'Estònia"
+msgstr "Republica Estonă"
 
 msgid "Republic of Fiji"
-msgstr "Republica de Fiji"
+msgstr "Republica Fiji"
 
 msgid "Republic of Finland"
-msgstr "Republica de Finlàndia"
+msgstr "Republica Finlanda"
 
 msgid "Republic of Ghana"
-msgstr "Republica del Gana"
+msgstr "Republica Ghana"
 
 msgid "Republic of Guatemala"
-msgstr "Republica del Guatemala"
+msgstr "Republica Guatemala"
 
 msgid "Republic of Guinea"
-msgstr "Republica de Guinèa"
+msgstr "Republica Guinea"
 
 msgid "Republic of Guinea-Bissau"
-msgstr "Republica de Guinèa Bissau"
+msgstr "Republica Guinea-Bissau"
 
 msgid "Republic of Guyana"
-msgstr "Republica de Guyana"
+msgstr "Republica Guyana"
 
 msgid "Republic of Haiti"
-msgstr "Republica d’Haití"
+msgstr "Republica Haiti"
 
 msgid "Republic of Honduras"
-msgstr "Republica d'Honduras"
+msgstr "Republica Honduras"
 
 msgid "Republic of Iceland"
-msgstr "Republica d'Islàndia"
+msgstr "Republica Islanda"
 
 msgid "Republic of India"
-msgstr "Republica d’Índia"
+msgstr "Republica India"
 
 msgid "Republic of Indonesia"
-msgstr "Republica d’Indonesia"
+msgstr "Republica Indonezia"
 
 msgid "Republic of Iraq"
-msgstr "Republica d’Iraq"
+msgstr "Republica Irak"
 
 msgid "Republic of Kazakhstan"
-msgstr "Republica del Cazacstan"
+msgstr "Republica Kazakhstan"
 
 msgid "Republic of Kenya"
-msgstr "Republica del Kenya"
+msgstr "Republica Kenia"
 
 msgid "Republic of Kiribati"
-msgstr "Republica de Kiribati"
+msgstr "Republica Kiribati"
 
 msgid "Republic of Latvia"
-msgstr "Republica letona"
+msgstr "Republica Letonă"
 
 msgid "Republic of Liberia"
-msgstr "Republica de Libèria"
+msgstr "Republica Liberia"
 
 msgid "Republic of Lithuania"
-msgstr "Republica de Lituània"
+msgstr "Republica Lituania"
 
 msgid "Republic of Madagascar"
-msgstr "Republica de Madagascar"
+msgstr "Republica Madagascar"
 
 msgid "Republic of Malawi"
-msgstr "Republica de Malawi"
+msgstr "Republica Malawi"
 
 msgid "Republic of Maldives"
-msgstr "Republica de las Maldivas"
+msgstr "Republica Maldive"
 
 msgid "Republic of Mali"
-msgstr "Republica de Mali"
+msgstr "Republica Mali"
 
 msgid "Republic of Malta"
-msgstr "Republica de Malta"
+msgstr "Republica Malta"
 
 msgid "Republic of Mauritius"
-msgstr "Republica de Maurici"
+msgstr "Republica Maurițius"
 
 msgid "Republic of Moldova"
-msgstr "Republica de Moldàvia"
+msgstr "Republica Moldova"
 
 msgid "Republic of Mozambique"
-msgstr "Republica de Moçambic"
+msgstr "Republica Mozambic"
 
 msgid "Republic of Myanmar"
-msgstr "Republica de Birmania"
+msgstr "Republica Myanmar"
 
 msgid "Republic of Namibia"
-msgstr "Republica de Namibia"
+msgstr "Republica Namibia"
 
 msgid "Republic of Nauru"
-msgstr "Republica de Nauru"
+msgstr "Republica Nauru"
 
 msgid "Republic of Nicaragua"
-msgstr "Paraguai"
-
-msgid "Republic of North Macedonia"
-msgstr "Republica de Macedònia del Nòrd"
+msgstr "Republica Nicaragua"
 
 msgid "Republic of Palau"
-msgstr "Republica de Belau"
+msgstr "Republica Palau"
 
 msgid "Republic of Panama"
-msgstr "Republica del Panamà"
+msgstr "Republica Panama"
 
 msgid "Republic of Paraguay"
-msgstr "Republica de Paraguai"
+msgstr "Republica Paraguay"
 
 msgid "Republic of Peru"
-msgstr "Republica del Peró"
+msgstr "Republica Peru"
 
 msgid "Republic of Poland"
-msgstr "Republica de Polonha"
+msgstr "Republica Polonă"
 
 msgid "Republic of San Marino"
-msgstr "Republica de Sant Marin"
+msgstr "Republica San Marino"
 
 msgid "Republic of Senegal"
-msgstr "Republica de Senegal"
+msgstr "Republica Senegal"
 
 msgid "Republic of Serbia"
-msgstr "Republica de Serbia"
+msgstr "Republica Serbia"
 
 msgid "Republic of Seychelles"
-msgstr "Republica de las Seichèlas"
+msgstr "Republica Seychelles"
 
 msgid "Republic of Sierra Leone"
-msgstr "Republica de Sierra Leone"
+msgstr "Republica Sierra Leone"
 
 msgid "Republic of Singapore"
-msgstr "Republica de Singapor"
+msgstr "Republica Singapore"
 
 msgid "Republic of Slovenia"
-msgstr "Republica d'Eslovènia"
+msgstr "Republica Slovenă"
 
 msgid "Republic of South Africa"
-msgstr "Republica de Sudafrica"
+msgstr "Republica Africa de sud"
 
 msgid "Republic of South Sudan"
-msgstr "Republica de Sodan del Sud"
+msgstr "Republica Sudanului de Sud"
 
 msgid "Republic of Suriname"
-msgstr "Republica de Surinam"
+msgstr "Republica Suriname"
 
 msgid "Republic of Tajikistan"
-msgstr "Republica de Tatgiquistan"
+msgstr "Republica Tajikistan"
 
 msgid "Republic of Trinidad and Tobago"
-msgstr "Republica de Trinitat e Tobago"
+msgstr "Republica Trinidad-Tobago"
 
 msgid "Republic of Tunisia"
-msgstr "Republica tunisiana"
+msgstr "Republica Tunisia"
 
 msgid "Republic of Uganda"
-msgstr "Republica d’Oganda"
+msgstr "Republica Uganda"
 
 msgid "Republic of Uzbekistan"
-msgstr "Republica d'Ozbequistan"
+msgstr "Republica Uzbekistan"
 
 msgid "Republic of Vanuatu"
-msgstr "Republica de Vanuatu"
+msgstr "Republica Vanuatu"
 
 msgid "Republic of Yemen"
-msgstr "Republica de Iemèn"
+msgstr "Republica Yemen"
 
 msgid "Republic of Zambia"
-msgstr "Republica de Zambia"
+msgstr "Republica Zambia"
 
 msgid "Republic of Zimbabwe"
-msgstr "Republica de Zimbabwe"
+msgstr "Republica Zimbabwe"
 
 msgid "Republic of the Congo"
-msgstr "Republica de Còngo"
-
-msgid "Republic of the Gambia"
-msgstr "Republica de Gàmbia"
+msgstr "Republica Congo"
 
 msgid "Republic of the Marshall Islands"
-msgstr "Republica de las Illas Marshall"
+msgstr "Republica Insulele Marshall"
 
 msgid "Republic of the Niger"
-msgstr "Republica de Nigèr"
+msgstr "Republica Nigeria"
 
 msgid "Republic of the Philippines"
-msgstr "Republica de las Filipinas"
+msgstr "Republica Filipine"
 
 msgid "Republic of the Sudan"
-msgstr "Republica de Sodan"
+msgstr "Republica Sudan"
 
 msgid "Romania"
-msgstr "Romania"
+msgstr "România"
 
 msgid "Russian Federation"
-msgstr "Federacion russa"
+msgstr "Federația Rusă"
 
 msgid "Rwanda"
 msgstr "Rwanda"
 
 msgid "Rwandese Republic"
-msgstr "Republica rewandesa"
+msgstr "Republica Rwanda"
 
 msgid "Réunion"
 msgstr "Réunion"
 
 msgid "Saint Barthélemy"
-msgstr "Sant Bertomieu"
+msgstr "Sfântul Bartolomeu"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Santa Elena, Ascension, e Tristan da Cunha"
+msgstr "Sfânta Elena, Ascension și Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "St. Kitts e Nevis"
+msgstr "Saint Kitts și Nevis"
 
 msgid "Saint Lucia"
-msgstr "St. Lucia"
+msgstr "Sfânta Lucia"
 
 msgid "Saint Martin (French part)"
-msgstr "Sant Martin (Part francesa)"
+msgstr "Sfântul Martin (partea franceză)"
 
 msgid "Saint Pierre and Miquelon"
-msgstr "Sant Pèire e Miquelon"
+msgstr "Saint Pierre și Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Sant Vincenç e las Grenadinas"
+msgstr "Saint Vincent și Grenadinele"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
-msgstr "Sant Marin"
+msgstr "San Marino"
 
 msgid "Sao Tome and Principe"
-msgstr "Sao Tomé e Principe"
+msgstr "Sao Tome și Principe"
 
 msgid "Saudi Arabia"
-msgstr "Arabia saudita"
+msgstr "Arabia Saudită"
 
 msgid "Senegal"
 msgstr "Senegal"
 
 msgid "Serbia"
 msgstr "Serbia"
 
 msgid "Seychelles"
-msgstr "Seichèlas"
+msgstr "Seychelles"
 
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
-msgstr "Singapor"
+msgstr "Singapore"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Sant Martin (Part neerlandesa)"
+msgstr "Sfântul Martin (partea olandeză)"
 
 msgid "Slovak Republic"
-msgstr "Republica eslovaquia"
+msgstr "Republica Slovacă"
 
 msgid "Slovakia"
-msgstr "Eslovaquia"
+msgstr "Slovacia"
 
 msgid "Slovenia"
-msgstr "Eslovènia"
+msgstr "Slovenia"
 
 msgid "Socialist Republic of Viet Nam"
-msgstr "Republica socialista de Vietnam"
+msgstr "Republica socialistă Vietnam"
 
 msgid "Solomon Islands"
-msgstr "Illas Salomon"
+msgstr "Insulele Solomon"
 
 msgid "Somalia"
 msgstr "Somalia"
 
 msgid "South Africa"
-msgstr "Sudafrica"
+msgstr "Africa de sud"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "Illas Georgia del Sud e Sandwich del Sud"
-
-msgid "South Korea"
-msgstr "Corèa del Sud"
+msgstr "Georgia de Sud și Insulele Sandwich de sud"
 
 msgid "South Sudan"
-msgstr "Sodan del Sud"
+msgstr "Sudanul de Sud"
 
 msgid "Spain"
-msgstr "Espanha"
+msgstr "Spania"
 
 msgid "Sri Lanka"
 msgstr "Sri Lanka"
 
 msgid "State of Israel"
-msgstr "Estat d'Israèl"
+msgstr "Statul Israel"
 
 msgid "State of Kuwait"
-msgstr "Estat de Kowait"
+msgstr "Statul Kuweit"
 
 msgid "State of Qatar"
-msgstr "Estat de Qatar"
+msgstr "Statul Qatar"
 
 msgid "Sudan"
-msgstr "Sodan"
+msgstr "Sudan"
 
 msgid "Sultanate of Oman"
-msgstr "Soudanat d’Oman"
+msgstr "Sultanatul Omanului"
 
 msgid "Suriname"
 msgstr "Surinam"
 
 msgid "Svalbard and Jan Mayen"
-msgstr "Svalbard e Jan Mayen"
+msgstr "Svalbard și Jan Mayen"
 
 msgid "Sweden"
-msgstr "Suècia"
+msgstr "Suedia"
 
 msgid "Swiss Confederation"
-msgstr "Confederacion Soïssa"
+msgstr "Confederația Elvețiană"
 
 msgid "Switzerland"
-msgstr "Soïssa"
+msgstr "Elveția"
 
 msgid "Syrian Arab Republic"
-msgstr "Republica Dominicana"
+msgstr "Republica Araba Siria"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan, Province of China"
-msgstr "Taiwan, província de China"
+msgstr "Taiwan"
 
 msgid "Tajikistan"
-msgstr "Tatgiquistan"
+msgstr "Tajikistan"
 
 msgid "Tanzania"
 msgstr "Tanzania"
 
 msgid "Tanzania, United Republic of"
-msgstr "Tanzania, republica unida de"
+msgstr "Republica Unită Tanzania"
 
 msgid "Thailand"
-msgstr "Tailàndia"
+msgstr "Tailanda"
 
 msgid "Timor-Leste"
-msgstr "Timòr Èst"
+msgstr "Timorul de Est"
 
 msgid "Togo"
-msgstr "Tògo"
+msgstr "Togo"
 
 msgid "Togolese Republic"
-msgstr "Republica togolesa"
+msgstr "Republica Togoleză"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
 msgid "Tonga"
-msgstr "Tònga"
+msgstr "Tonga"
 
 msgid "Trinidad and Tobago"
-msgstr "Trinitat e Tobago"
+msgstr "Trinidad și Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
 msgid "Turkmenistan"
-msgstr "Turcmenistan"
+msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
-msgstr "Illas Turcas e Caïcas"
+msgstr "Insulele Turks și Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
 msgid "Uganda"
-msgstr "Oganda"
+msgstr "Uganda"
 
 msgid "Ukraine"
-msgstr "Ucraïna"
+msgstr "Ucraina"
 
 msgid "Union of the Comoros"
-msgstr "Union de las Comòras"
+msgstr "Uniunea Comoros"
 
 msgid "United Arab Emirates"
-msgstr "Emirats Arabs Units"
+msgstr "Emiratele Arabe Unite"
 
 msgid "United Kingdom"
-msgstr "Reialme Unit"
+msgstr "Regatul Unit"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "Reialme Unit de Grand Bretanha e d’Irlanda del Nòrd"
+msgstr "Regatul Unit al Marii Britanii și Insulelor Nordice"
 
 msgid "United Mexican States"
-msgstr "Estats Units del Mexic"
+msgstr "Statele Unite Mexicane"
 
 msgid "United Republic of Tanzania"
-msgstr "Republica unida de Tanzania"
+msgstr "Republica Unită Tanzania"
 
 msgid "United States"
-msgstr "Estats Units"
+msgstr "Statele Unite"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Islas perifericas Menores dels Estats Units"
+msgstr "Insulele de Coasta ale Statelor Unite"
 
 msgid "United States of America"
-msgstr "Estats Units d’America"
+msgstr "Statele Unite ale Americii"
 
 msgid "Uruguay"
-msgstr "Uruguai"
+msgstr "Uruguay"
 
 msgid "Uzbekistan"
-msgstr "Ozbequistan"
+msgstr "Uzbekistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
-msgstr "Veneçuèla"
+msgstr "Venezuela"
 
 msgid "Venezuela, Bolivarian Republic of"
-msgstr "Veneçuèla, Republica Dominicana bolivariana del"
+msgstr "Venezuela, Republica Bolivariană"
 
 msgid "Viet Nam"
-msgstr "Viet Nam"
+msgstr "Vietnam"
 
 msgid "Vietnam"
 msgstr "Vietnam"
 
 msgid "Virgin Islands of the United States"
-msgstr "Islas Verges dels Estats Units d’America"
+msgstr "Insulele virgine ale Statelor Unite"
 
 msgid "Virgin Islands, British"
-msgstr "Illas Verges, britanicas"
+msgstr "Insulele virgine (britanice)"
 
 msgid "Virgin Islands, U.S."
-msgstr "illas Verges, EU"
+msgstr "Insulele virgine (SUA)"
 
 msgid "Wallis and Futuna"
-msgstr "Wallis e Futuna"
+msgstr "Wallis și Futuna"
 
 msgid "Western Sahara"
-msgstr "Sahara occidental"
+msgstr "Sahara de Vest"
 
 msgid "Yemen"
-msgstr "Iemèn"
+msgstr "Yemen"
 
 msgid "Zambia"
 msgstr "Zambia"
 
 msgid "Zimbabwe"
 msgstr "Zimbabwe"
 
 msgid "the State of Eritrea"
-msgstr "l’Estat d’Eritrèa"
+msgstr "Statul Eritrea"
 
 msgid "the State of Palestine"
-msgstr "l’estat de Palestina"
+msgstr "Statul Palestina"
 
 msgid "Åland Islands"
-msgstr "llas Åland"
+msgstr "Insulele Åland"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2023-01-20 19:59+0000\n"
+"PO-Revision-Date: 2023-04-20 19:53+0000\n"
 "Last-Translator: Jakub Bogusz <qboosh@pld-linux.org>\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.15.1\n"
+"X-Generator: Weblate 4.18-dev\n"
 "X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albania"
@@ -238,15 +238,15 @@
 msgid "Djibouti"
 msgstr "Dżibuti"
 
 msgid "Dominica"
 msgstr "Dominika"
 
 msgid "Dominican Republic"
-msgstr "Dominikana"
+msgstr "Republika Dominikańska"
 
 msgid "Eastern Republic of Uruguay"
 msgstr "Wschodnia Republika Urugwaju"
 
 msgid "Ecuador"
 msgstr "Ekwador"
 
@@ -382,15 +382,15 @@
 msgid "Heard Island and McDonald Islands"
 msgstr "Wyspy Heard i McDonalda"
 
 msgid "Hellenic Republic"
 msgstr "Republika Grecka"
 
 msgid "Holy See (Vatican City State)"
-msgstr "Watykan"
+msgstr "Państwo Watykańskie (Stolica Apostolska)"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
 msgstr "Hongkong"
 
@@ -412,17 +412,20 @@
 
 msgid "India"
 msgstr "Indie"
 
 msgid "Indonesia"
 msgstr "Indonezja"
 
-msgid "Iran, Islamic Republic of"
+msgid "Iran"
 msgstr "Iran"
 
+msgid "Iran, Islamic Republic of"
+msgstr "Iran, Islamska Republika"
+
 msgid "Iraq"
 msgstr "Irak"
 
 msgid "Ireland"
 msgstr "Irlandia"
 
 msgid "Islamic Republic of Afghanistan"
@@ -512,29 +515,32 @@
 msgid "Kingdom of the Netherlands"
 msgstr "Królestwo Holandii"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea, Democratic People's Republic of"
-msgstr "Korea Północna"
+msgstr "Korea - Republika Ludowo-Demokratyczna"
 
 msgid "Korea, Republic of"
-msgstr "Korea Południowa"
+msgstr "Republika Korei"
 
 msgid "Kuwait"
 msgstr "Kuwejt"
 
 msgid "Kyrgyz Republic"
 msgstr "Republika Kirgiska"
 
 msgid "Kyrgyzstan"
 msgstr "Kirgistan"
 
 msgid "Lao People's Democratic Republic"
+msgstr "Laotańska Republika Ludowo-Demokratyczna"
+
+msgid "Laos"
 msgstr "Laos"
 
 msgid "Latvia"
 msgstr "Łotwa"
 
 msgid "Lebanese Republic"
 msgstr "Republika Libańska"
@@ -899,15 +905,15 @@
 msgid "Republic of Moldova"
 msgstr "Republika Mołdawii"
 
 msgid "Republic of Mozambique"
 msgstr "Republika Mozambiku"
 
 msgid "Republic of Myanmar"
-msgstr "Związek Birmański"
+msgstr "Republika Związku Mjanmy"
 
 msgid "Republic of Namibia"
 msgstr "Republika Namibii"
 
 msgid "Republic of Nauru"
 msgstr "Republika Nauru"
 
@@ -1091,15 +1097,15 @@
 msgid "Solomon Islands"
 msgstr "Wyspy Salomona"
 
 msgid "Somalia"
 msgstr "Somalia"
 
 msgid "South Africa"
-msgstr "Republika Południowej Afryki"
+msgstr "Południowa Afryka"
 
 msgid "South Georgia and the South Sandwich Islands"
 msgstr "Georgia Południowa i Sandwich Południowy"
 
 msgid "South Korea"
 msgstr "Korea Południowa"
 
@@ -1138,14 +1144,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Konfederacja Szwajcarska"
 
 msgid "Switzerland"
 msgstr "Szwajcaria"
 
+msgid "Syria"
+msgstr "Syria"
+
 msgid "Syrian Arab Republic"
 msgstr "Syryjska Republika Arabska"
 
 msgid "Taiwan"
 msgstr "Tajwan"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,108 +1,104 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2019-09-20 18:28+0000\n"
-"Last-Translator: Jakub Bogusz <qboosh@pld-linux.org>\n"
-"Language-Team: Polish <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-3/pl/>\n"
-"Language: pl\n"
+"PO-Revision-Date: 2015-12-26 21:20+0200\n"
+"Last-Translator: Miroslav Nikolić <miroslavnikolic@rocketmail.com>\n"
+"Language-Team: Serbian <(nothing)>\n"
+"Language: sr@latin\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 3.9-dev\n"
-"X-Bugs: Report translation errors to the Language-Team address.\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 
 msgid "British Antarctic Territory"
-msgstr "Brytyjskie Terytorium Antarktyczne"
+msgstr "Britanska Antarktička Teritorija"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Birma, Socjalistyczna Republika Związku Birmańskiego"
+msgstr "Burma, Socijalistička Republika Unije"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Białoruska SRR (Socjalistyczna Republika Radziecka)"
+msgstr "Beloruska SSR (Sovjetska Socijalistička Republika)"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Canton i Enderbury"
+msgstr "Ostrva Kanton i Enderberi"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Czechosłowacja, Czechosłowacka Republika Socjalistyczna"
+msgstr "Čehoslovačka, Čehoslovačka Socijalistička Republika"
 
 msgid "Dahomey"
 msgstr "Dahomej"
 
 msgid "Dronning Maud Land"
-msgstr "Ziemia Królowej Maud"
+msgstr "Zemlja Droning Mod"
 
 msgid "East Timor"
-msgstr "Timor Wschodni"
+msgstr "Istočni Timor"
 
 msgid "France, Metropolitan"
-msgstr "Francja metropolitalna"
+msgstr "Francuska, Metropolis"
 
 msgid "French Afars and Issas"
-msgstr "Francuskie Terytorium Afarów i Issów"
+msgstr "Francuski Afari i Ise"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Francuskie Terytoria Południowe i Antarktyczne"
+msgstr "Francuske Južne i Antarktičke Teritorije"
 
 msgid "German Democratic Republic"
-msgstr "Niemiecka Republika Demokratyczna"
+msgstr "Nemačka Demokratska Republika"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Wyspy Gilberta i Ellice"
+msgstr "Ostrva Gilbert i Elis"
 
 msgid "Johnston Island"
-msgstr "Johnston"
+msgstr "Ostrvo Džonston"
 
 msgid "Midway Islands"
-msgstr "Midway"
+msgstr "Ostrva Midvej"
 
 msgid "Netherlands Antilles"
-msgstr "Antyle Holenderskie"
+msgstr "Holandski Antili"
 
 msgid "Neutral Zone"
-msgstr "Strefa Neutralna"
+msgstr "Neutralna zona"
 
 msgid "New Hebrides"
-msgstr "Nowe Hebrydy"
+msgstr "Novi Hebridi"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Powiernicze Wyspy Pacyfiku"
+msgstr "Pacifička ostrva (poverena teritorija)"
 
 msgid "Panama Canal Zone"
-msgstr "Strefa Kanału Panamskiego"
+msgstr "Panamska zona kanala"
 
 msgid "Serbia and Montenegro"
-msgstr "Serbia i Czarnogóra"
+msgstr "Srbija i Crna Gora"
 
 msgid "Sikkim"
-msgstr "Sikkim"
+msgstr "Sikim"
 
 msgid "Southern Rhodesia"
-msgstr "Rodezja Południowa"
+msgstr "Južna Rodezija"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "Wyspy Stanów Zjednoczonych na Pacyfiku"
+msgstr "Razna pacifička ostrva SAD"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "ZSSR, Związek Socjalistycznych Republik Radzieckich"
+msgstr "SSSR, Savez Sovjetskih Socijalističkih Republika"
 
 msgid "Upper Volta, Republic of"
-msgstr "Górna Wolta, Republika Górnej Wolty"
+msgstr "Gornja Volta, Republika"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Wietnam Północny, Demokratyczna Republika Wietnamu"
+msgstr "Vijetnam, Demokratska Republika"
 
 msgid "Wake Island"
-msgstr "Wake"
+msgstr "Ostrvo Vejk"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr ""
-"Jemen Południowy, Jemen Demokratyczny, Ludowo-Demokratyczna Republika Jemenu"
+msgstr "Jemen, Demokratski, Demokratska Narodna Republika"
 
 msgid "Zaire, Republic of"
-msgstr "Zair, Republika Zairu"
+msgstr "Zair, Republika"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,166 +1,164 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_4217\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
 "PO-Revision-Date: 2019-04-27 17:48+0000\n"
 "Last-Translator: Rui Mendes <xz9@protonmail.com>\n"
-"Language-Team: Portuguese <https://hosted.weblate.org/projects/iso-codes/"
-"iso-4217/pt/>\n"
-"Language: pt\n"
+"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/iso-"
+"codes/iso-4217/pt_BR/>\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 3.6.1\n"
 
 msgid "ADB Unit of Account"
 msgstr "Unidade de conta ADB"
 
 msgid "Afghani"
-msgstr "Afegâni"
+msgstr "Afegane"
 
 msgid "Algerian Dinar"
 msgstr "Dinar argelino"
 
 msgid "Argentine Peso"
 msgstr "Peso argentino"
 
 msgid "Armenian Dram"
-msgstr "Dram da Arménia"
+msgstr "Dram armênio"
 
 msgid "Aruban Florin"
-msgstr "Florim arubano"
+msgstr "Florim de Aruba"
 
 msgid "Australian Dollar"
 msgstr "Dólar australiano"
 
 msgid "Bahamian Dollar"
 msgstr "Dólar das Bahamas"
 
 msgid "Bahraini Dinar"
-msgstr "Dinar baremita"
+msgstr "Dinar do Bahrein"
 
 msgid "Baht"
 msgstr "Baht"
 
 msgid "Balboa"
 msgstr "Balboa"
 
 msgid "Barbados Dollar"
-msgstr "Dólar dos Barbados"
+msgstr "Dólar barbadiano"
 
 msgid "Belarusian Ruble"
 msgstr "Rublo bielorrusso"
 
 msgid "Belize Dollar"
 msgstr "Dólar de Belize"
 
 msgid "Bermudian Dollar"
 msgstr "Dólar das Bermudas"
 
 msgid "Boliviano"
 msgstr "Boliviano"
 
 msgid "Bond Markets Unit European Composite Unit (EURCO)"
-msgstr "Unidade Composta Europeia de Mercados de Obrigações (EURCO)"
+msgstr "European Composite Unit (EURCO) (unidade de mercado de títulos)"
 
 msgid "Bond Markets Unit European Monetary Unit (E.M.U.-6)"
-msgstr ""
-"Unidade Monetária Europeia (E.M.U.-6) (unidade de mercado de obrigações)"
+msgstr "European Monetary Unit (E.M.U.-6) (unidade de mercado de títulos)"
 
 msgid "Bond Markets Unit European Unit of Account 17 (E.U.A.-17)"
 msgstr ""
-"Unidade Europeia de Conta 17 (E.U.A.-17) (unidade de mercado de obrigações)"
+"European Unit of Account 17 (E.U.A.-17) (unidade de mercado de títulos)"
 
 msgid "Bond Markets Unit European Unit of Account 9 (E.U.A.-9)"
-msgstr ""
-"Unidade Europeia de Conta 9 (E.U.A.-9) (unidade de mercado de obrigações)"
+msgstr "European Unit of Account 9 (E.U.A.-9) (unidade de mercado de títulos)"
 
 msgid "Brazilian Real"
 msgstr "Real brasileiro"
 
 msgid "Brunei Dollar"
-msgstr "Dólar do Brunei"
+msgstr "Dólar de Brunei"
 
 msgid "Bulgarian Lev"
 msgstr "Lev búlgaro"
 
 msgid "Burundi Franc"
 msgstr "Franco do Burundi"
 
 msgid "CFA Franc BCEAO"
-msgstr "Franco CFA da África Ocidental"
+msgstr "Franco CFA BCEAO"
 
 msgid "CFA Franc BEAC"
-msgstr "Franco CFA da África Central"
+msgstr "Franco CFA BEAC"
 
 msgid "CFP Franc"
 msgstr "Franco CFP"
 
 msgid "Cabo Verde Escudo"
-msgstr "Escudo cabo-verdiano"
+msgstr "Escudo de Cabo Verde"
 
 msgid "Canadian Dollar"
-msgstr "Dólar canadiano"
+msgstr "Dólar canadense"
 
 msgid "Cayman Islands Dollar"
-msgstr "Dólar das Ilhas Caimão"
+msgstr "Dólar das Ilhas Caimã"
 
 msgid "Chilean Peso"
 msgstr "Peso chileno"
 
 msgid "Codes specifically reserved for testing purposes"
-msgstr "Código reservado especificamente para testes"
+msgstr "Códigos reservado especificamente para testes"
 
 msgid "Colombian Peso"
 msgstr "Peso colombiano"
 
 msgid "Congolese Franc"
 msgstr "Franco congolês"
 
 msgid "Convertible Mark"
 msgstr "Marco conversível"
 
 msgid "Cordoba Oro"
-msgstr "Córdoba ouro"
+msgstr "Córdoba oro"
 
 msgid "Costa Rican Colon"
-msgstr "Colón costa-riquenho"
+msgstr "Cólon costa-riquenho"
 
 msgid "Cuban Peso"
 msgstr "Peso cubano"
 
 msgid "Czech Koruna"
-msgstr "Coroa checa"
+msgstr "Coroa Tcheca"
 
 msgid "Dalasi"
 msgstr "Dalasi"
 
 msgid "Danish Krone"
 msgstr "Coroa dinamarquesa"
 
 msgid "Denar"
-msgstr "Dinar macedónio"
+msgstr "Dinar"
 
 msgid "Djibouti Franc"
-msgstr "Franco jibutiano"
+msgstr "Franco do Djibuti"
 
 msgid "Dobra"
 msgstr "Dobra"
 
 msgid "Dominican Peso"
 msgstr "Peso dominicano"
 
 msgid "Dong"
-msgstr "Dongue"
+msgstr "Dong"
 
 msgid "East Caribbean Dollar"
-msgstr "Dólar das Caraíbas Orientais"
+msgstr "Dólar do Caribe do Leste"
 
 msgid "Egyptian Pound"
 msgstr "Libra egípcia"
 
 msgid "El Salvador Colon"
 msgstr "Colón salvadorenho"
 
@@ -170,66 +168,66 @@
 msgid "Euro"
 msgstr "Euro"
 
 msgid "Falkland Islands Pound"
 msgstr "Libra das Ilhas Malvinas"
 
 msgid "Fiji Dollar"
-msgstr "Dólar fijiano"
+msgstr "Dólar de Fiji"
 
 msgid "Forint"
-msgstr "Florim húngaro"
+msgstr "Florim"
 
 msgid "Ghana Cedi"
 msgstr "Cedi do Gana"
 
 msgid "Gibraltar Pound"
 msgstr "Libra de Gibraltar"
 
 msgid "Gold"
 msgstr "Ouro"
 
 msgid "Gourde"
-msgstr "Gurde"
+msgstr "Gourde"
 
 msgid "Guarani"
 msgstr "Guarani"
 
 msgid "Guyana Dollar"
 msgstr "Dólar da Guiana"
 
 msgid "Hong Kong Dollar"
 msgstr "Dólar de Hong Kong"
 
 msgid "Hryvnia"
 msgstr "Grívnia"
 
 msgid "Iceland Krona"
-msgstr "Coroa islandesa"
+msgstr "Nova coroa islandesa"
 
 msgid "Indian Rupee"
-msgstr "Rupia indiana"
+msgstr "Rúpia indiana"
 
 msgid "Iranian Rial"
 msgstr "Rial iraniano"
 
 msgid "Iraqi Dinar"
 msgstr "Dinar iraquiano"
 
 msgid "Jamaican Dollar"
 msgstr "Dólar jamaicano"
 
 msgid "Jordanian Dinar"
-msgstr "Dinar jordano"
+msgstr "Dinar jordaniano"
 
 msgid "Kenyan Shilling"
 msgstr "Xelim queniano"
 
 msgid "Kina"
-msgstr "Quina"
+msgstr "Kina"
 
 msgid "Kuna"
 msgstr "Kuna"
 
 msgid "Kuwaiti Dinar"
 msgstr "Dinar kuwaitiano"
 
@@ -242,174 +240,174 @@
 msgid "Lari"
 msgstr "Lari"
 
 msgid "Lebanese Pound"
 msgstr "Libra libanesa"
 
 msgid "Lek"
-msgstr "Leque da Albânia"
+msgstr "Lek"
 
 msgid "Lempira"
 msgstr "Lempira"
 
 msgid "Leone"
 msgstr "Leone"
 
 msgid "Liberian Dollar"
 msgstr "Dólar liberiano"
 
 msgid "Libyan Dinar"
-msgstr "Dinar líbio"
+msgstr "Dinar da Líbia"
 
 msgid "Lilangeni"
-msgstr "Lilanguéni suázi"
+msgstr "Lilangeni"
 
 msgid "Loti"
 msgstr "Loti"
 
 msgid "Malagasy Ariary"
-msgstr "Ariari malgaxe"
+msgstr "Ariary de Madagáscar"
 
 msgid "Malawi Kwacha"
-msgstr "Kwacha do Maláui"
+msgstr "Quacha de Maláui"
 
 msgid "Malaysian Ringgit"
-msgstr "Ringgit malaio"
+msgstr "Ringgit da Malásia"
 
 msgid "Mauritius Rupee"
-msgstr "Rupia mauriciana"
+msgstr "Rúpia da Maurícia"
 
 msgid "Mexican Peso"
 msgstr "Peso mexicano"
 
 msgid "Moldovan Leu"
-msgstr "Leu moldavo"
+msgstr "Leu moldávio"
 
 msgid "Moroccan Dirham"
-msgstr "Dirame marroquino"
+msgstr "Dirham marroquino"
 
 msgid "Mozambique Metical"
-msgstr "Metical moçambicano"
+msgstr "Metical de Moçambique"
 
 msgid "Naira"
 msgstr "Naira"
 
 msgid "Nakfa"
 msgstr "Nakfa"
 
 msgid "Namibia Dollar"
-msgstr "Dólar namibiano"
+msgstr "Dólar da Namíbia"
 
 msgid "Nepalese Rupee"
-msgstr "Rupia nepalesa"
+msgstr "Rúpia nepalesa"
 
 msgid "Netherlands Antillean Guilder"
-msgstr "Florim das Antilhas Neerlandesas"
+msgstr "Florim das Antilhas Holandesas"
 
 msgid "New Israeli Sheqel"
-msgstr "Novo shekel israelita"
+msgstr "Novo shekel israelense"
 
 msgid "New Taiwan Dollar"
-msgstr "Novo dólar taiwanês"
+msgstr "Novo dólar de Taiwan"
 
 msgid "New Zealand Dollar"
-msgstr "Dólar neozelandês"
+msgstr "Dólar da Nova Zelândia"
 
 msgid "Ngultrum"
 msgstr "Ngultrum"
 
 msgid "North Korean Won"
 msgstr "Won norte-coreano"
 
 msgid "Norwegian Krone"
 msgstr "Coroa norueguesa"
 
 msgid "Ouguiya"
 msgstr "Uguia"
 
 msgid "Pakistan Rupee"
-msgstr "Rupia paquistanesa"
+msgstr "Rúpia paquistanesa"
 
 msgid "Palladium"
 msgstr "Paládio"
 
 msgid "Pataca"
-msgstr "Pataca macaense"
+msgstr "Pataca"
 
 msgid "Pa’anga"
-msgstr "Paanga"
+msgstr "Pa’anga"
 
 msgid "Peso Convertible"
-msgstr "Peso convertível"
+msgstr "Peso conversível"
 
 msgid "Peso Uruguayo"
 msgstr "Peso uruguaio"
 
 msgid "Philippine Peso"
 msgstr "Peso filipino"
 
 msgid "Platinum"
-msgstr "Platina"
+msgstr "Platinum"
 
 msgid "Pound Sterling"
 msgstr "Libra esterlina"
 
 msgid "Pula"
 msgstr "Pula"
 
 msgid "Qatari Rial"
-msgstr "Rial catariano"
+msgstr "Rial de Qatar"
 
 msgid "Quetzal"
 msgstr "Quetzal"
 
 msgid "Rand"
-msgstr "Rande"
+msgstr "Rand"
 
 msgid "Rial Omani"
-msgstr "Rial omanense"
+msgstr "Rial de Omã"
 
 msgid "Riel"
 msgstr "Riel"
 
 msgid "Romanian Leu"
 msgstr "Leu romeno"
 
 msgid "Rufiyaa"
-msgstr "Rupia maldiva"
+msgstr "Rúpia"
 
 msgid "Rupiah"
-msgstr "Rupia indonésia"
+msgstr "Rúpia"
 
 msgid "Russian Ruble"
 msgstr "Rublo russo"
 
 msgid "Rwanda Franc"
-msgstr "Franco ruandês"
+msgstr "Franco de Ruanda"
 
 msgid "SDR (Special Drawing Right)"
-msgstr "SDR (direitos especiais de saque)"
+msgstr "SDR (Special Drawing Right)"
 
 msgid "Saint Helena Pound"
 msgstr "Libra de Santa Helena"
 
 msgid "Saudi Riyal"
 msgstr "Rial saudita"
 
 msgid "Serbian Dinar"
 msgstr "Dinar sérvio"
 
 msgid "Seychelles Rupee"
-msgstr "Rupia das Seicheles"
+msgstr "Rúpia das Seychelles"
 
 msgid "Silver"
 msgstr "Prata"
 
 msgid "Singapore Dollar"
-msgstr "Dólar de Singapura"
+msgstr "Dólar de Cingapura"
 
 msgid "Sol"
 msgstr "Novo sol"
 
 msgid "Solomon Islands Dollar"
 msgstr "Dólar das Ilhas Salomão"
 
@@ -422,18 +420,18 @@
 msgid "Somoni"
 msgstr "Somoni"
 
 msgid "South Sudanese Pound"
 msgstr "Libra sul-sudanesa"
 
 msgid "Sri Lanka Rupee"
-msgstr "Rupia do Sri Lanka"
+msgstr "Rúpia do Sri Lanka"
 
 msgid "Sucre"
-msgstr "SUCRE"
+msgstr "Sucre"
 
 msgid "Sudanese Pound"
 msgstr "Libra sudanesa"
 
 msgid "Surinam Dollar"
 msgstr "Dólar do Suriname"
 
@@ -443,15 +441,15 @@
 msgid "Swiss Franc"
 msgstr "Franco suíço"
 
 msgid "Syrian Pound"
 msgstr "Libra síria"
 
 msgid "Taka"
-msgstr "Taka"
+msgstr "Taca"
 
 msgid "Tala"
 msgstr "Tala"
 
 msgid "Tanzanian Shilling"
 msgstr "Xelim tanzaniano"
 
@@ -459,56 +457,56 @@
 msgstr "Tenge"
 
 msgid "The codes assigned for transactions where no currency is involved"
 msgstr ""
 "Os códigos atribuídos para transações nas quais nenhuma moeda está envolvida"
 
 msgid "Trinidad and Tobago Dollar"
-msgstr "Dólar de Trindade e Tobago"
+msgstr "Dólar de Trinidade e Tobago"
 
 msgid "Tugrik"
-msgstr "Tugrique"
+msgstr "Tugrik"
 
 msgid "Tunisian Dinar"
-msgstr "Dinar tunisino"
+msgstr "Dinar tunisiano"
 
 msgid "Turkish Lira"
 msgstr "Lira turca"
 
 msgid "Turkmenistan New Manat"
-msgstr "Manat turcomeno"
+msgstr "Novo manate turcomano"
 
 msgid "UAE Dirham"
-msgstr "Dirham dos Emirados Árabes"
+msgstr "Dirham dos Emirados"
 
 msgid "US Dollar"
 msgstr "Dólar americano"
 
 msgid "Uganda Shilling"
-msgstr "Xelim ugandês"
+msgstr "Xelim do Uganda"
 
 msgid "Uzbekistan Sum"
-msgstr "Som usbeque"
+msgstr "Som do Uzbequistão"
 
 msgid "Vatu"
 msgstr "Vatu"
 
 msgid "Won"
-msgstr "Won sul-coreano"
+msgstr "Won"
 
 msgid "Yemeni Rial"
 msgstr "Rial iemenita"
 
 msgid "Yen"
 msgstr "Iene"
 
 msgid "Yuan Renminbi"
-msgstr "Renminbi chinês"
+msgstr "Renminbi Iuan"
 
 msgid "Zambian Kwacha"
-msgstr "Kwacha zambiano"
+msgstr "Kwacha Zambiano"
 
 msgid "Zimbabwe Dollar"
-msgstr "Dólar zimbabuense"
+msgstr "Dólar de Zimbábue"
 
 msgid "Zloty"
-msgstr "Zlóti"
+msgstr "Zloty"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,512 +1,529 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_4217\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2019-04-27 17:48+0000\n"
-"Last-Translator: Rui Mendes <xz9@protonmail.com>\n"
-"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/iso-"
-"codes/iso-4217/pt_BR/>\n"
-"Language: pt_BR\n"
+"PO-Revision-Date: 2023-03-29 20:40+0000\n"
+"Last-Translator: d <dmanye@gmail.com>\n"
+"Language-Team: Catalan <https://hosted.weblate.org/projects/iso-codes/"
+"iso-4217/ca/>\n"
+"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 3.6.1\n"
-
-msgid "ADB Unit of Account"
-msgstr "Unidade de conta ADB"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17-dev\n"
+"X-Bugs: Report translation errors to the Language-Team address.\n"
 
 msgid "Afghani"
-msgstr "Afegane"
+msgstr "Afgani"
 
 msgid "Algerian Dinar"
-msgstr "Dinar argelino"
+msgstr "Dinar algerià"
 
 msgid "Argentine Peso"
-msgstr "Peso argentino"
+msgstr "Peso argentí"
 
 msgid "Armenian Dram"
-msgstr "Dram armênio"
+msgstr "Dram armeni"
 
 msgid "Aruban Florin"
-msgstr "Florim de Aruba"
+msgstr "Florí d'Aruba"
 
 msgid "Australian Dollar"
-msgstr "Dólar australiano"
+msgstr "Dòlar australià"
+
+msgid "Azerbaijan Manat"
+msgstr "Manat azerbaidjanès"
 
 msgid "Bahamian Dollar"
-msgstr "Dólar das Bahamas"
+msgstr "Dòlar de les Bahames"
 
 msgid "Bahraini Dinar"
-msgstr "Dinar do Bahrein"
+msgstr "Dinar de Bahrain"
 
 msgid "Baht"
 msgstr "Baht"
 
 msgid "Balboa"
 msgstr "Balboa"
 
 msgid "Barbados Dollar"
-msgstr "Dólar barbadiano"
+msgstr "Dòlar de Barbados"
 
 msgid "Belarusian Ruble"
-msgstr "Rublo bielorrusso"
+msgstr "Ruble bielorús"
 
 msgid "Belize Dollar"
-msgstr "Dólar de Belize"
+msgstr "Dòlar de Belize"
 
 msgid "Bermudian Dollar"
-msgstr "Dólar das Bermudas"
+msgstr "Dòlar de les Bermudes"
 
 msgid "Boliviano"
 msgstr "Boliviano"
 
+msgid "Bolívar Soberano"
+msgstr "Bolívar Sobirà"
+
 msgid "Bond Markets Unit European Composite Unit (EURCO)"
-msgstr "European Composite Unit (EURCO) (unidade de mercado de títulos)"
+msgstr "Unitat composta europea per al mercat d'obligacions (EURCO)"
 
 msgid "Bond Markets Unit European Monetary Unit (E.M.U.-6)"
-msgstr "European Monetary Unit (E.M.U.-6) (unidade de mercado de títulos)"
-
-msgid "Bond Markets Unit European Unit of Account 17 (E.U.A.-17)"
-msgstr ""
-"European Unit of Account 17 (E.U.A.-17) (unidade de mercado de títulos)"
-
-msgid "Bond Markets Unit European Unit of Account 9 (E.U.A.-9)"
-msgstr "European Unit of Account 9 (E.U.A.-9) (unidade de mercado de títulos)"
+msgstr "Unitat monetària europea per al mercat d'obligacions (EMU-6)"
 
 msgid "Brazilian Real"
-msgstr "Real brasileiro"
+msgstr "Real brasiler"
 
 msgid "Brunei Dollar"
-msgstr "Dólar de Brunei"
+msgstr "Dòlar de Brunei"
 
 msgid "Bulgarian Lev"
-msgstr "Lev búlgaro"
+msgstr "Lev búlgar"
 
 msgid "Burundi Franc"
-msgstr "Franco do Burundi"
+msgstr "Franc de Burundi"
 
 msgid "CFA Franc BCEAO"
-msgstr "Franco CFA BCEAO"
+msgstr "Franc CFA de la BCEAO"
 
 msgid "CFA Franc BEAC"
-msgstr "Franco CFA BEAC"
+msgstr "Franc CFA de la BEAC"
 
 msgid "CFP Franc"
-msgstr "Franco CFP"
+msgstr "Franc CFP"
 
 msgid "Cabo Verde Escudo"
-msgstr "Escudo de Cabo Verde"
+msgstr "Escut de Cap Verd"
 
 msgid "Canadian Dollar"
-msgstr "Dólar canadense"
+msgstr "Dòlar canadenc"
 
 msgid "Cayman Islands Dollar"
-msgstr "Dólar das Ilhas Caimã"
+msgstr "Dòlar de les Illes Caiman"
 
 msgid "Chilean Peso"
-msgstr "Peso chileno"
+msgstr "Peso xilè"
 
 msgid "Codes specifically reserved for testing purposes"
-msgstr "Códigos reservado especificamente para testes"
+msgstr "Codis específicament reservats per proves"
 
 msgid "Colombian Peso"
-msgstr "Peso colombiano"
+msgstr "Peso colombià"
+
+msgid "Comorian Franc"
+msgstr "Franc de les Comores"
 
 msgid "Congolese Franc"
-msgstr "Franco congolês"
+msgstr "Franc congolès"
 
 msgid "Convertible Mark"
-msgstr "Marco conversível"
+msgstr "Marc convertible"
 
 msgid "Cordoba Oro"
-msgstr "Córdoba oro"
+msgstr "Córdoba or"
 
 msgid "Costa Rican Colon"
-msgstr "Cólon costa-riquenho"
+msgstr "Colon costa-riqueny"
 
 msgid "Cuban Peso"
-msgstr "Peso cubano"
+msgstr "Peso cubà"
 
 msgid "Czech Koruna"
-msgstr "Coroa Tcheca"
+msgstr "Corona txeca"
 
 msgid "Dalasi"
 msgstr "Dalasi"
 
 msgid "Danish Krone"
-msgstr "Coroa dinamarquesa"
+msgstr "Corona danesa"
 
 msgid "Denar"
-msgstr "Dinar"
+msgstr "Denar"
 
 msgid "Djibouti Franc"
-msgstr "Franco do Djibuti"
+msgstr "Franc de Djibouti"
 
 msgid "Dobra"
 msgstr "Dobra"
 
 msgid "Dominican Peso"
-msgstr "Peso dominicano"
+msgstr "Peso dominicà"
 
 msgid "Dong"
 msgstr "Dong"
 
 msgid "East Caribbean Dollar"
-msgstr "Dólar do Caribe do Leste"
+msgstr "Dòlar del Carib Oriental"
 
 msgid "Egyptian Pound"
-msgstr "Libra egípcia"
+msgstr "Lliura egípcia"
 
 msgid "El Salvador Colon"
-msgstr "Colón salvadorenho"
+msgstr "Colon salvadorenc"
 
 msgid "Ethiopian Birr"
-msgstr "Birr etíope"
+msgstr "Birr etíop"
 
 msgid "Euro"
 msgstr "Euro"
 
 msgid "Falkland Islands Pound"
-msgstr "Libra das Ilhas Malvinas"
+msgstr "Lliura de les Malvines"
 
 msgid "Fiji Dollar"
-msgstr "Dólar de Fiji"
+msgstr "Dòlar de Fiji"
 
 msgid "Forint"
-msgstr "Florim"
+msgstr "Fòrint"
 
 msgid "Ghana Cedi"
-msgstr "Cedi do Gana"
+msgstr "Cedi de Ghana"
 
 msgid "Gibraltar Pound"
-msgstr "Libra de Gibraltar"
+msgstr "Lliura de Gibraltar"
 
 msgid "Gold"
-msgstr "Ouro"
+msgstr "Or"
 
 msgid "Gourde"
 msgstr "Gourde"
 
 msgid "Guarani"
-msgstr "Guarani"
+msgstr "Guaraní"
+
+msgid "Guinean Franc"
+msgstr "Franc de Guinea"
 
 msgid "Guyana Dollar"
-msgstr "Dólar da Guiana"
+msgstr "Dòlar de Guyana"
 
 msgid "Hong Kong Dollar"
-msgstr "Dólar de Hong Kong"
+msgstr "Dòlar de Hong Kong"
 
 msgid "Hryvnia"
-msgstr "Grívnia"
+msgstr "Hrívnia"
 
 msgid "Iceland Krona"
-msgstr "Nova coroa islandesa"
+msgstr "Corona islandesa"
 
 msgid "Indian Rupee"
-msgstr "Rúpia indiana"
+msgstr "Rupia índia"
 
 msgid "Iranian Rial"
-msgstr "Rial iraniano"
+msgstr "Rial iranià"
 
 msgid "Iraqi Dinar"
-msgstr "Dinar iraquiano"
+msgstr "Dinar iraquià"
 
 msgid "Jamaican Dollar"
-msgstr "Dólar jamaicano"
+msgstr "Dòlar jamaicà"
 
 msgid "Jordanian Dinar"
-msgstr "Dinar jordaniano"
+msgstr "Dinar jordà"
 
 msgid "Kenyan Shilling"
-msgstr "Xelim queniano"
+msgstr "Xíling kenyà"
 
 msgid "Kina"
 msgstr "Kina"
 
 msgid "Kuna"
 msgstr "Kuna"
 
 msgid "Kuwaiti Dinar"
-msgstr "Dinar kuwaitiano"
+msgstr "Dinar kuwaitià"
 
 msgid "Kwanza"
 msgstr "Kwanza"
 
 msgid "Kyat"
-msgstr "Quiate"
+msgstr "Kyat"
+
+msgid "Lao Kip"
+msgstr "kip laosià"
 
 msgid "Lari"
 msgstr "Lari"
 
 msgid "Lebanese Pound"
-msgstr "Libra libanesa"
+msgstr "Lliura libanesa"
 
 msgid "Lek"
 msgstr "Lek"
 
 msgid "Lempira"
 msgstr "Lempira"
 
 msgid "Leone"
 msgstr "Leone"
 
 msgid "Liberian Dollar"
-msgstr "Dólar liberiano"
+msgstr "Dòlar liberià"
 
 msgid "Libyan Dinar"
-msgstr "Dinar da Líbia"
+msgstr "Dinar libi"
 
 msgid "Lilangeni"
 msgstr "Lilangeni"
 
 msgid "Loti"
 msgstr "Loti"
 
 msgid "Malagasy Ariary"
-msgstr "Ariary de Madagáscar"
+msgstr "Ariary malgaix"
 
 msgid "Malawi Kwacha"
-msgstr "Quacha de Maláui"
+msgstr "Kwacha malawià"
 
 msgid "Malaysian Ringgit"
-msgstr "Ringgit da Malásia"
+msgstr "Ringgit de Malàisia"
 
 msgid "Mauritius Rupee"
-msgstr "Rúpia da Maurícia"
+msgstr "Rupia mauriciana"
 
 msgid "Mexican Peso"
-msgstr "Peso mexicano"
+msgstr "Peso mexicà"
 
 msgid "Moldovan Leu"
-msgstr "Leu moldávio"
+msgstr "Leu moldau"
 
 msgid "Moroccan Dirham"
-msgstr "Dirham marroquino"
+msgstr "Dírham marroquí"
 
 msgid "Mozambique Metical"
-msgstr "Metical de Moçambique"
+msgstr "Metical de Moçambic"
+
+msgid "Mvdol"
+msgstr "Mvdol"
 
 msgid "Naira"
 msgstr "Naira"
 
 msgid "Nakfa"
 msgstr "Nakfa"
 
 msgid "Namibia Dollar"
-msgstr "Dólar da Namíbia"
+msgstr "Dòlar namibià"
 
 msgid "Nepalese Rupee"
-msgstr "Rúpia nepalesa"
+msgstr "Rupia nepalesa"
 
 msgid "Netherlands Antillean Guilder"
-msgstr "Florim das Antilhas Holandesas"
+msgstr "Florí de les Antilles Neerlandeses"
 
 msgid "New Israeli Sheqel"
-msgstr "Novo shekel israelense"
+msgstr "Nou xéquel israelià"
 
 msgid "New Taiwan Dollar"
-msgstr "Novo dólar de Taiwan"
+msgstr "Nou dòlar de Taiwan"
 
 msgid "New Zealand Dollar"
-msgstr "Dólar da Nova Zelândia"
+msgstr "Dòlar neozelandès"
 
 msgid "Ngultrum"
 msgstr "Ngultrum"
 
 msgid "North Korean Won"
-msgstr "Won norte-coreano"
+msgstr "Won nord-coreà"
 
 msgid "Norwegian Krone"
-msgstr "Coroa norueguesa"
+msgstr "Corona noruega"
 
 msgid "Ouguiya"
-msgstr "Uguia"
+msgstr "Ouguiya"
 
 msgid "Pakistan Rupee"
-msgstr "Rúpia paquistanesa"
+msgstr "Rupia pakistanesa"
 
 msgid "Palladium"
-msgstr "Paládio"
+msgstr "Pal·ladi"
 
 msgid "Pataca"
 msgstr "Pataca"
 
 msgid "Pa’anga"
-msgstr "Pa’anga"
+msgstr "Pa'anga"
 
 msgid "Peso Convertible"
-msgstr "Peso conversível"
+msgstr "Peso convertible"
 
 msgid "Peso Uruguayo"
-msgstr "Peso uruguaio"
+msgstr "Peso uruguaià"
 
 msgid "Philippine Peso"
-msgstr "Peso filipino"
+msgstr "Peso filipí"
 
 msgid "Platinum"
-msgstr "Platinum"
+msgstr "Platí"
 
 msgid "Pound Sterling"
-msgstr "Libra esterlina"
+msgstr "Lliura esterlina"
 
 msgid "Pula"
 msgstr "Pula"
 
 msgid "Qatari Rial"
 msgstr "Rial de Qatar"
 
 msgid "Quetzal"
 msgstr "Quetzal"
 
 msgid "Rand"
 msgstr "Rand"
 
 msgid "Rial Omani"
-msgstr "Rial de Omã"
+msgstr "Rial omanita"
 
 msgid "Riel"
 msgstr "Riel"
 
 msgid "Romanian Leu"
-msgstr "Leu romeno"
+msgstr "Leu romanès"
 
 msgid "Rufiyaa"
-msgstr "Rúpia"
+msgstr "Rufiyaa"
 
 msgid "Rupiah"
-msgstr "Rúpia"
+msgstr "Rupia"
 
 msgid "Russian Ruble"
-msgstr "Rublo russo"
+msgstr "Ruble rus"
 
 msgid "Rwanda Franc"
-msgstr "Franco de Ruanda"
+msgstr "Franc de Ruanda"
 
 msgid "SDR (Special Drawing Right)"
-msgstr "SDR (Special Drawing Right)"
+msgstr "DEG (drets especials de gir)"
 
 msgid "Saint Helena Pound"
-msgstr "Libra de Santa Helena"
+msgstr "Lliura de Santa Helena"
 
 msgid "Saudi Riyal"
 msgstr "Rial saudita"
 
 msgid "Serbian Dinar"
-msgstr "Dinar sérvio"
+msgstr "Dinar serbi"
 
 msgid "Seychelles Rupee"
-msgstr "Rúpia das Seychelles"
+msgstr "Rupia de les Seychelles"
 
 msgid "Silver"
-msgstr "Prata"
+msgstr "Plata"
 
 msgid "Singapore Dollar"
-msgstr "Dólar de Cingapura"
+msgstr "Dòlar de Singapur"
 
 msgid "Sol"
-msgstr "Novo sol"
+msgstr "Sol"
 
 msgid "Solomon Islands Dollar"
-msgstr "Dólar das Ilhas Salomão"
+msgstr "Dòlar de les Illes Salomó"
 
 msgid "Som"
 msgstr "Som"
 
 msgid "Somali Shilling"
-msgstr "Xelim somaliano"
+msgstr "Xíling somali"
 
 msgid "Somoni"
 msgstr "Somoni"
 
 msgid "South Sudanese Pound"
-msgstr "Libra sul-sudanesa"
+msgstr "Lliura sud-sudanesa"
 
 msgid "Sri Lanka Rupee"
-msgstr "Rúpia do Sri Lanka"
+msgstr "Rupia de Sri Lanka"
 
 msgid "Sucre"
 msgstr "Sucre"
 
 msgid "Sudanese Pound"
-msgstr "Libra sudanesa"
+msgstr "Lliura sudanesa"
 
 msgid "Surinam Dollar"
-msgstr "Dólar do Suriname"
+msgstr "Dòlar de Singapur"
 
 msgid "Swedish Krona"
-msgstr "Coroa sueca"
+msgstr "Corona sueca"
 
 msgid "Swiss Franc"
-msgstr "Franco suíço"
+msgstr "Franc suís"
 
 msgid "Syrian Pound"
-msgstr "Libra síria"
+msgstr "Lliura siriana"
 
 msgid "Taka"
-msgstr "Taca"
+msgstr "Taka"
 
 msgid "Tala"
 msgstr "Tala"
 
 msgid "Tanzanian Shilling"
-msgstr "Xelim tanzaniano"
+msgstr "Xíling tanzà"
 
 msgid "Tenge"
 msgstr "Tenge"
 
 msgid "The codes assigned for transactions where no currency is involved"
-msgstr ""
-"Os códigos atribuídos para transações nas quais nenhuma moeda está envolvida"
+msgstr "Els codis assignats per a transaccions on no hi ha moneda involucrada"
 
 msgid "Trinidad and Tobago Dollar"
-msgstr "Dólar de Trinidade e Tobago"
+msgstr "Dòlar de Trinitat i Tobago"
 
 msgid "Tugrik"
 msgstr "Tugrik"
 
 msgid "Tunisian Dinar"
-msgstr "Dinar tunisiano"
+msgstr "Dinar tunisià"
 
 msgid "Turkish Lira"
 msgstr "Lira turca"
 
 msgid "Turkmenistan New Manat"
-msgstr "Novo manate turcomano"
+msgstr "Manat turcman"
 
 msgid "UAE Dirham"
-msgstr "Dirham dos Emirados"
+msgstr "Dírham dels EAU"
 
 msgid "US Dollar"
-msgstr "Dólar americano"
+msgstr "Dòlar dels Estats Units"
+
+msgid "US Dollar (Next day)"
+msgstr "Dòlar dels Estats Units (per a l'endemà)"
 
 msgid "Uganda Shilling"
-msgstr "Xelim do Uganda"
+msgstr "Xíling ugandès"
 
 msgid "Uzbekistan Sum"
-msgstr "Som do Uzbequistão"
+msgstr "Som d'Uzbekistan"
 
 msgid "Vatu"
 msgstr "Vatu"
 
+msgid "WIR Euro"
+msgstr "Euro WIR"
+
+msgid "WIR Franc"
+msgstr "Franc WIR"
+
 msgid "Won"
 msgstr "Won"
 
 msgid "Yemeni Rial"
 msgstr "Rial iemenita"
 
 msgid "Yen"
-msgstr "Iene"
+msgstr "Ien"
 
 msgid "Yuan Renminbi"
-msgstr "Renminbi Iuan"
+msgstr "Iuan renminbi"
 
 msgid "Zambian Kwacha"
-msgstr "Kwacha Zambiano"
+msgstr "Kwacha zambià"
 
 msgid "Zimbabwe Dollar"
-msgstr "Dólar de Zimbábue"
+msgstr "Dòlar de Zimbàbue"
 
 msgid "Zloty"
 msgstr "Zloty"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,1256 +1,1287 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2018-11-30 15:08+0000\n"
-"Last-Translator: Andrei POPESCU <andreimpopescu@gmail.com>\n"
-"Language-Team: Romanian <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-1/ro/>\n"
-"Language: ro\n"
+"PO-Revision-Date: 2023-03-20 09:23+0000\n"
+"Last-Translator: Quentin PAGÈS <quentinantonin@free.fr>\n"
+"Language-Team: Occitan <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-1/oc/>\n"
+"Language: oc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
-"20)) ? 1 : 2;\n"
-"X-Generator: Weblate 3.3\n"
-"X-Launchpad-Export-Date: 2010-08-16 11:01+0000\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albania"
 
 msgid "Algeria"
-msgstr "Algeria"
+msgstr "Argeria"
 
 msgid "American Samoa"
-msgstr "Samoa americană"
+msgstr "Samoa americana"
 
 msgid "Andorra"
-msgstr "Andora"
+msgstr "Andòrra"
 
 msgid "Angola"
-msgstr "Angola"
+msgstr "Angòla"
 
 msgid "Anguilla"
 msgstr "Anguilla"
 
 msgid "Antarctica"
-msgstr "Antarctica"
+msgstr "Antartica"
 
 msgid "Antigua and Barbuda"
-msgstr "Antigua și Barbuda"
+msgstr "Antigua e Barbuda"
 
 msgid "Arab Republic of Egypt"
-msgstr "Republica arabă Egipt"
+msgstr "Republica araba d’Egipte"
 
 msgid "Argentina"
 msgstr "Argentina"
 
 msgid "Argentine Republic"
-msgstr "Republica Argentina"
+msgstr "Republica argentina"
 
 msgid "Armenia"
 msgstr "Armenia"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
 msgstr "Australia"
 
 msgid "Austria"
-msgstr "Austria"
+msgstr "Àustria"
 
 msgid "Azerbaijan"
-msgstr "Azerbaijan"
+msgstr "Azerbaitjan"
 
 msgid "Bahamas"
 msgstr "Bahamas"
 
 msgid "Bahrain"
-msgstr "Bahrein"
+msgstr "Barein"
 
 msgid "Bangladesh"
-msgstr "Bangladeș"
+msgstr "Bangladèsh"
 
 msgid "Barbados"
-msgstr "Barbados"
+msgstr "Barbada"
 
 msgid "Belarus"
-msgstr "Bielorusia"
+msgstr "Bielorussia"
 
 msgid "Belgium"
-msgstr "Belgia"
+msgstr "Belgica"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
 msgstr "Benin"
 
 msgid "Bermuda"
-msgstr "Bermude"
+msgstr "Bermudas"
 
 msgid "Bhutan"
-msgstr "Bhutan"
+msgstr "Botan"
 
 msgid "Bolivarian Republic of Venezuela"
-msgstr "Republica Bolivariană a Venezuelei"
+msgstr "Republica bolivariana de Venecuèla"
 
 msgid "Bolivia"
 msgstr "Bolivia"
 
 msgid "Bolivia, Plurinational State of"
-msgstr "Bolivia"
+msgstr "Bolívia, Estat plurinacional de"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire, Sint Eustatius și Saba"
+msgstr "Bonaire, Sant Eustaqui e Saba"
 
 msgid "Bosnia and Herzegovina"
-msgstr "Bosnia și Herțegovina"
+msgstr "Bòsnia e Ercegovina"
 
 msgid "Botswana"
 msgstr "Botswana"
 
 msgid "Bouvet Island"
-msgstr "Insula Bouvet"
+msgstr "Illa Bouvet"
 
 msgid "Brazil"
-msgstr "Brazilia"
+msgstr "Brasil"
 
 msgid "British Indian Ocean Territory"
-msgstr "Teritoriul britanic din Oceanul Indian"
+msgstr "Territòris britanics de l'ocean indian"
 
 msgid "British Virgin Islands"
-msgstr "Insulele virgine britanice"
+msgstr "Illas Verges britanicas"
 
 msgid "Brunei Darussalam"
 msgstr "Brunei"
 
 msgid "Bulgaria"
 msgstr "Bulgaria"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
 msgid "Burundi"
 msgstr "Burundi"
 
 msgid "Cabo Verde"
-msgstr "Capul Verde"
+msgstr "Cap Verd"
 
 msgid "Cambodia"
-msgstr "Cambogia"
+msgstr "Cambòtja"
 
 msgid "Cameroon"
-msgstr "Camerun"
+msgstr "Cameron"
 
 msgid "Canada"
-msgstr "Canada"
+msgstr "Canadà"
 
 msgid "Cayman Islands"
-msgstr "Insulele Caiman"
+msgstr "Illas Caiman"
 
 msgid "Central African Republic"
-msgstr "Republica Central Africană"
+msgstr "Republica de Centrafrica"
 
 msgid "Chad"
-msgstr "Ciad"
+msgstr "Chad"
 
 msgid "Chile"
 msgstr "Chile"
 
 msgid "China"
 msgstr "China"
 
 msgid "Christmas Island"
-msgstr "Insula Crăciunului"
+msgstr "Illa Cristmas"
 
 msgid "Cocos (Keeling) Islands"
-msgstr "Insulele Cocos (Keeling)"
+msgstr "Illas Cocos (Keeling)"
 
 msgid "Colombia"
-msgstr "Columbia"
+msgstr "Colombia"
 
 msgid "Commonwealth of Dominica"
-msgstr "Comitatul Dominican"
+msgstr "Commonwealth de la Dominica"
 
 msgid "Commonwealth of the Bahamas"
-msgstr "Comitatul Bahamas"
-
-msgid "Commonwealth of the Northern Mariana Islands"
-msgstr "Comitatul Insulelor Mariane Nordice"
+msgstr "Commonwealth de las Bahamas"
 
 msgid "Comoros"
-msgstr "Comoros"
+msgstr "Comòras"
 
 msgid "Congo"
-msgstr "Congo"
+msgstr "Còngo"
 
 msgid "Congo, The Democratic Republic of the"
-msgstr "Congo, Republica democrată"
+msgstr "Còngo, Republica Democratica de"
 
 msgid "Cook Islands"
-msgstr "Insulele Cook"
+msgstr "Illas Cook"
 
 msgid "Costa Rica"
-msgstr "Costa Rica"
+msgstr "Còsta Rica"
 
 msgid "Croatia"
-msgstr "Croația"
+msgstr "Croàcia"
 
 msgid "Cuba"
 msgstr "Cuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Cipru"
+msgstr "Chipre"
 
 msgid "Czech Republic"
-msgstr "Cehia"
+msgstr "Republica chèca"
 
 msgid "Czechia"
-msgstr "Cehia"
+msgstr "Chequia"
 
 msgid "Côte d'Ivoire"
-msgstr "Coasta de Fildeș"
+msgstr "Còsta d'Evòri"
 
 msgid "Democratic People's Republic of Korea"
-msgstr "Republica populară democrată Coreea"
+msgstr "Republica populara democratica de Corèa"
 
 msgid "Democratic Republic of Sao Tome and Principe"
-msgstr "Republica democrată Sao Tome și Principe"
+msgstr "Republica Democratica de São Tomé e Príncipe"
 
 msgid "Democratic Republic of Timor-Leste"
-msgstr "Republica democrată Timorul de Est"
+msgstr "Republica democratica del Timòr Èst"
 
 msgid "Democratic Socialist Republic of Sri Lanka"
-msgstr "Republica socialistă democrată Sri Lanka"
+msgstr "Republica Democratica Socialista d'Sri Lanka"
 
 msgid "Denmark"
-msgstr "Danemarca"
+msgstr "Danemarc"
 
 msgid "Djibouti"
-msgstr "Djibouti"
+msgstr "Jiboti"
 
 msgid "Dominica"
 msgstr "Dominica"
 
 msgid "Dominican Republic"
-msgstr "Republica Dominicană"
+msgstr "Republica Dominicana"
 
 msgid "Eastern Republic of Uruguay"
-msgstr "Republica Estică Uruguay"
+msgstr "Republica orientala d’Uruguai"
 
 msgid "Ecuador"
-msgstr "Ecuador"
+msgstr "Eqüator"
 
 msgid "Egypt"
-msgstr "Egipt"
+msgstr "Egipte"
 
 msgid "El Salvador"
 msgstr "El Salvador"
 
 msgid "Equatorial Guinea"
-msgstr "Guinea Ecuatorială"
+msgstr "Guinèa eqüatoriala"
 
 msgid "Eritrea"
-msgstr "Eritreea"
+msgstr "Eritrèa"
 
 msgid "Estonia"
-msgstr "Estonia"
+msgstr "Estònia"
+
+msgid "Eswatini"
+msgstr "Eswatini"
 
 msgid "Ethiopia"
 msgstr "Etiopia"
 
 msgid "Falkland Islands (Malvinas)"
-msgstr "Insulele Falkland (Insulele Malvine)"
+msgstr "Illas Falkand (Malvinas)"
 
 msgid "Faroe Islands"
-msgstr "Insulele Feroe"
+msgstr "Illas Feròe"
 
 msgid "Federal Democratic Republic of Ethiopia"
-msgstr "Republica federală democrată Etiopia"
+msgstr "Republica Democratica Federala d'Etiopia"
 
 msgid "Federal Democratic Republic of Nepal"
-msgstr "Republica federală democrată Nepal"
+msgstr "Republica democratica federala del Nepam"
 
 msgid "Federal Republic of Germany"
-msgstr "Republica federală Germană"
+msgstr "Republica federala d’Alemanha"
 
 msgid "Federal Republic of Nigeria"
-msgstr "Republica federală Nigeria"
+msgstr "Republica federala del Nigèria"
 
 msgid "Federal Republic of Somalia"
-msgstr "Republica Federală Somalia"
+msgstr "Republica federala de Somalia"
 
 msgid "Federated States of Micronesia"
-msgstr "Statele federale ale Microneziei"
+msgstr "Estats federats de Micronesia"
 
 msgid "Federative Republic of Brazil"
-msgstr "Republica federală Brazilia"
+msgstr "Republica federativa de Brasil"
 
 msgid "Fiji"
 msgstr "Fiji"
 
 msgid "Finland"
-msgstr "Finlanda"
+msgstr "Finlàndia"
 
 msgid "France"
-msgstr "Franța"
+msgstr "França"
 
 msgid "French Guiana"
-msgstr "Guiana Franceză"
+msgstr "Guaiana francesa"
 
 msgid "French Polynesia"
-msgstr "Polinezia Franceză"
+msgstr "Polinesia francesa"
 
 msgid "French Republic"
-msgstr "Republica Franceză"
+msgstr "Republica francesa"
 
 msgid "French Southern Territories"
-msgstr "Teritoriile franceze de sud"
+msgstr "Tèrras australas francesas"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gabonese Republic"
-msgstr "Republica Gabon"
+msgstr "Republica gabonesa"
 
 msgid "Gambia"
-msgstr "Gambia"
+msgstr "Gàmbia"
 
 msgid "Georgia"
 msgstr "Georgia"
 
 msgid "Germany"
-msgstr "Germania"
+msgstr "Alemanha"
 
 msgid "Ghana"
-msgstr "Ghana"
+msgstr "Gana"
 
 msgid "Gibraltar"
-msgstr "Gibraltar"
+msgstr "Gibartar"
 
 msgid "Grand Duchy of Luxembourg"
-msgstr "Marele Ducat al Luxemburgului"
+msgstr "Grand Ducat de Luxemborg"
 
 msgid "Greece"
-msgstr "Grecia"
+msgstr "Grècia"
 
 msgid "Greenland"
-msgstr "Groenlanda"
+msgstr "Groenlàndia"
 
 msgid "Grenada"
-msgstr "Grenada"
+msgstr "Granada"
 
 msgid "Guadeloupe"
-msgstr "Guadelupa"
+msgstr "Guadalope"
 
 msgid "Guam"
 msgstr "Guam"
 
 msgid "Guatemala"
 msgstr "Guatemala"
 
 msgid "Guernsey"
-msgstr "Guernsey"
+msgstr "Guernesey"
 
 msgid "Guinea"
-msgstr "Guinea"
+msgstr "Guinèa"
 
 msgid "Guinea-Bissau"
-msgstr "Guinea-Bissau"
+msgstr "Guinèa-Bissau"
 
 msgid "Guyana"
 msgstr "Guyana"
 
 msgid "Haiti"
-msgstr "Haiti"
+msgstr "Haití"
 
 msgid "Hashemite Kingdom of Jordan"
-msgstr "Regatul Hașemit Iordanian"
+msgstr "Reialme Hashimita de Jordania"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Insula Heard și Insulele McDonald"
+msgstr "Illas Heard e McDonald"
 
 msgid "Hellenic Republic"
-msgstr "Republica Elenă"
+msgstr "Republica ellenica"
 
 msgid "Holy See (Vatican City State)"
-msgstr "Vatican"
+msgstr "Santa Ses (Estat de la Ciutat de Vatican)"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
 msgstr "Hong Kong"
 
 msgid "Hong Kong Special Administrative Region of China"
-msgstr "Regiunea Chineză cu administrare specială Hong Kong"
+msgstr "Region administrativa especiala chinesa de Honk Hong"
 
 msgid "Hungary"
-msgstr "Ungaria"
+msgstr "Ongria"
 
 msgid "Iceland"
-msgstr "Islanda"
+msgstr "Islàndia"
 
 msgid "Independent State of Papua New Guinea"
-msgstr "Statul Independent Papua Noua Guinee"
+msgstr "Estat independent de Papoa-Nòva Guinèa"
 
 msgid "Independent State of Samoa"
-msgstr "Statul Independent Samoa"
+msgstr "Estat independent de Samoa"
 
 msgid "India"
-msgstr "India"
+msgstr "Índia"
 
 msgid "Indonesia"
-msgstr "Indonezia"
+msgstr "Indonesia"
+
+msgid "Iran"
+msgstr "Iran"
 
 msgid "Iran, Islamic Republic of"
-msgstr "Iran, Republica islamică"
+msgstr "Republica Dominicana"
 
 msgid "Iraq"
-msgstr "Irak"
+msgstr "Iraq"
 
 msgid "Ireland"
 msgstr "Irlanda"
 
 msgid "Islamic Republic of Afghanistan"
-msgstr "Republica islamică Afganistan"
+msgstr "Republica Dominicana"
 
 msgid "Islamic Republic of Iran"
-msgstr "Republica islamică Iran"
+msgstr "Republica Dominicana"
 
 msgid "Islamic Republic of Mauritania"
-msgstr "Republica islamică Mauritania"
+msgstr "Republica islamica de Mauritània"
 
 msgid "Islamic Republic of Pakistan"
-msgstr "Republica islamică Pakistan"
+msgstr "Republica islamica de Paquistan"
 
 msgid "Isle of Man"
-msgstr "Insula Man"
+msgstr "Illa de Man"
 
 msgid "Israel"
 msgstr "Israel"
 
 msgid "Italian Republic"
-msgstr "Republica Italiană"
+msgstr "Republica italiana"
 
 msgid "Italy"
-msgstr "Italia"
+msgstr "Itàlia"
 
 msgid "Jamaica"
 msgstr "Jamaica"
 
 msgid "Japan"
-msgstr "Japonia"
+msgstr "Japon"
 
 msgid "Jersey"
-msgstr "Jersey"
+msgstr "Jersei"
 
 msgid "Jordan"
-msgstr "Iordania"
+msgstr "Jordania"
 
 msgid "Kazakhstan"
-msgstr "Kazakhstan"
+msgstr "Cazacstan"
 
 msgid "Kenya"
-msgstr "Kenia"
+msgstr "Kenya"
 
 msgid "Kingdom of Bahrain"
-msgstr "Regatul Bahrein"
+msgstr "Reialme de Bahrain"
 
 msgid "Kingdom of Belgium"
-msgstr "Regatul Belgiei"
+msgstr "Reialme de Belgica"
 
 msgid "Kingdom of Bhutan"
-msgstr "Regatul Bhutan"
+msgstr "Reialme de Botan"
 
 msgid "Kingdom of Cambodia"
-msgstr "Regatul Cambodgiei"
+msgstr "Reialme de Cambòtja"
 
 msgid "Kingdom of Denmark"
-msgstr "Regatul Danemarcei"
+msgstr "Reialme de Danemarc"
+
+msgid "Kingdom of Eswatini"
+msgstr "Reialme d'Eswatini"
 
 msgid "Kingdom of Lesotho"
-msgstr "Regatul Lesotho"
+msgstr "Reialme de Lesotho"
 
 msgid "Kingdom of Morocco"
-msgstr "Regatul Marocului"
+msgstr "Reialme de Marròc"
 
 msgid "Kingdom of Norway"
-msgstr "Regatul Norvegiei"
+msgstr "Reialme de Norvègia"
 
 msgid "Kingdom of Saudi Arabia"
-msgstr "Regatul Arabiei Saudite"
+msgstr "Reialme d’Arabia Saudita"
 
 msgid "Kingdom of Spain"
-msgstr "Regatul Spaniei"
+msgstr "Reialme d'Espanha"
 
 msgid "Kingdom of Sweden"
-msgstr "Regatul Suediei"
+msgstr "Reialme de Suècia"
 
 msgid "Kingdom of Thailand"
-msgstr "Regatul Tailandei"
+msgstr "Reialme de Tailàndia"
 
 msgid "Kingdom of Tonga"
-msgstr "Regatul Tonga"
+msgstr "Reialme de Tònga"
 
 msgid "Kingdom of the Netherlands"
-msgstr "Regatul Olandei"
+msgstr "Reialme dels Païses Basses"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea, Democratic People's Republic of"
-msgstr "Republica democrată populară Coreea"
+msgstr "Corèa, Republica Populara Democratica de"
 
 msgid "Korea, Republic of"
-msgstr "Republica Coreea"
+msgstr "Corèa, republica de"
 
 msgid "Kuwait"
-msgstr "Kuweit"
+msgstr "Koweit"
 
 msgid "Kyrgyz Republic"
-msgstr "Republica kârgâză"
+msgstr "Republica Dominicana"
 
 msgid "Kyrgyzstan"
-msgstr "Kârgâzstan"
+msgstr "Kirguizstan"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Republica populară democrată Lao"
+msgstr "Republica democratica populara del Laos"
+
+msgid "Laos"
+msgstr "Laos"
 
 msgid "Latvia"
-msgstr "Letonia"
+msgstr "Letònia"
 
 msgid "Lebanese Republic"
-msgstr "Republica Libaneză"
+msgstr "Republica libanesa"
 
 msgid "Lebanon"
 msgstr "Liban"
 
 msgid "Lesotho"
-msgstr "Lesotho"
+msgstr "Lesoto"
 
 msgid "Liberia"
-msgstr "Liberia"
+msgstr "Libèria"
 
 msgid "Libya"
 msgstr "Libia"
 
 msgid "Liechtenstein"
 msgstr "Liechtenstein"
 
 msgid "Lithuania"
-msgstr "Lituania"
+msgstr "Lituània"
 
 msgid "Luxembourg"
-msgstr "Luxemburg"
+msgstr "Luxemborg"
 
 msgid "Macao"
-msgstr "Macao"
+msgstr "Macau"
 
 msgid "Macao Special Administrative Region of China"
-msgstr "Regiunea chineză cu administrare specială Macao"
+msgstr "Region administrativa especiala chinesa de Macau"
 
 msgid "Madagascar"
 msgstr "Madagascar"
 
 msgid "Malawi"
 msgstr "Malawi"
 
 msgid "Malaysia"
-msgstr "Malaezia"
+msgstr "Malàisia"
 
 msgid "Maldives"
-msgstr "Maldive"
+msgstr "Maldivas"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Insulele Marshall"
+msgstr "Illas Marshall"
 
 msgid "Martinique"
 msgstr "Martinica"
 
 msgid "Mauritania"
-msgstr "Mauritania"
+msgstr "Mauritània"
 
 msgid "Mauritius"
-msgstr "Maurițius"
+msgstr "Maurici"
 
 msgid "Mayotte"
-msgstr "Mayotte"
+msgstr "Maiòta"
 
 msgid "Mexico"
 msgstr "Mexic"
 
 msgid "Micronesia, Federated States of"
-msgstr "Micronesia, Statele federale ale"
+msgstr "Micronesia, Estats Federats de"
 
 msgid "Moldova"
-msgstr "Moldova"
+msgstr "Moldàvia"
 
 msgid "Moldova, Republic of"
-msgstr "Moldova, Republica"
+msgstr "Moldàvia, Republica de"
 
 msgid "Monaco"
-msgstr "Monaco"
+msgstr "Mónegue"
 
 msgid "Mongolia"
 msgstr "Mongolia"
 
 msgid "Montenegro"
-msgstr "Muntenegru"
+msgstr "Montenegro"
 
 msgid "Montserrat"
 msgstr "Montserrat"
 
 msgid "Morocco"
-msgstr "Maroc"
+msgstr "Marròc"
 
 msgid "Mozambique"
-msgstr "Mozambic"
+msgstr "Moçambic"
 
 msgid "Myanmar"
-msgstr "Myanmar"
+msgstr "Birmania"
 
 msgid "Namibia"
 msgstr "Namibia"
 
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepal"
 
 msgid "Netherlands"
-msgstr "Olanda"
+msgstr "Païses Basses"
 
 msgid "New Caledonia"
-msgstr "Noua Caledonie"
+msgstr "Nòva Caledònia"
 
 msgid "New Zealand"
-msgstr "Noua Zeelandă"
+msgstr "Novèla Zelanda"
 
 msgid "Nicaragua"
 msgstr "Nicaragua"
 
 msgid "Niger"
-msgstr "Niger"
+msgstr "Nigèr"
 
 msgid "Nigeria"
-msgstr "Nigeria"
+msgstr "Nigèria"
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
-msgstr "Insula Norfolk"
+msgstr "Illa Norfolk"
+
+msgid "North Korea"
+msgstr "Corèa del Nòrd"
+
+msgid "North Macedonia"
+msgstr "Macedònia del Nòrd"
 
 msgid "Northern Mariana Islands"
-msgstr "Insulele Mariane de Nord"
+msgstr "Illas Marianas del Nòrd"
 
 msgid "Norway"
-msgstr "Norvegia"
+msgstr "Norvègia"
 
 msgid "Oman"
 msgstr "Oman"
 
 msgid "Pakistan"
-msgstr "Pakistan"
+msgstr "Paquistan"
 
 msgid "Palau"
-msgstr "Palau"
+msgstr "Belau"
 
 msgid "Palestine, State of"
-msgstr "Palestina, Statul"
+msgstr "Palestina, estat de"
 
 msgid "Panama"
-msgstr "Panama"
+msgstr "Panamà"
 
 msgid "Papua New Guinea"
-msgstr "Papua Noua Guinee"
+msgstr "Papoa Nòva Guinèa"
 
 msgid "Paraguay"
-msgstr "Paraguay"
+msgstr "Paraguai"
 
 msgid "People's Democratic Republic of Algeria"
-msgstr "Republica populară Democratică Algeria"
+msgstr "Republica Argeriana Democratica e Populara"
 
 msgid "People's Republic of Bangladesh"
-msgstr "Republica populară Bangladeș"
+msgstr "Republica populara de Bangladèsh"
 
 msgid "People's Republic of China"
-msgstr "Republica populară Chineză"
+msgstr "Republica populara de China"
 
 msgid "Peru"
-msgstr "Peru"
+msgstr "Peró"
 
 msgid "Philippines"
-msgstr "Filipine"
+msgstr "Filipinas"
 
 msgid "Pitcairn"
-msgstr "Pitcairn"
+msgstr "Illa de Pitcairn"
 
 msgid "Plurinational State of Bolivia"
-msgstr "Statul plurinațional al Boliviei"
+msgstr "Estat plurinacional de Bolívia"
 
 msgid "Poland"
-msgstr "Polonia"
+msgstr "Polonha"
 
 msgid "Portugal"
-msgstr "Portugalia"
+msgstr "Portugal"
 
 msgid "Portuguese Republic"
-msgstr "Republica Portugheză"
+msgstr "Republica portuguesa"
 
 msgid "Principality of Andorra"
-msgstr "Principatul Andorra"
+msgstr "Principat d'Andòrra"
 
 msgid "Principality of Liechtenstein"
-msgstr "Principatul Liechtenstein"
+msgstr "Principat de Liechtenstein"
 
 msgid "Principality of Monaco"
-msgstr "Principatul Monaco"
+msgstr "Principat de Mónegue"
 
 msgid "Puerto Rico"
 msgstr "Puerto Rico"
 
 msgid "Qatar"
 msgstr "Qatar"
 
 msgid "Republic of Albania"
-msgstr "Republica Albania"
+msgstr "Republica d'Albania"
 
 msgid "Republic of Angola"
-msgstr "Republica Angola"
+msgstr "Republica d’Angòla"
 
 msgid "Republic of Armenia"
-msgstr "Republica Armenia"
+msgstr "Republicar d'Armenia"
 
 msgid "Republic of Austria"
-msgstr "Republica Austria"
+msgstr "Republica d'Àustria"
 
 msgid "Republic of Azerbaijan"
-msgstr "Republica Azerbaijan"
+msgstr "Republica d’Azerbaitjan"
 
 msgid "Republic of Belarus"
-msgstr "Republica Bielorusă"
+msgstr "Republica de Bielorussia"
 
 msgid "Republic of Benin"
-msgstr "Republica Benin"
+msgstr "Republica del Benin"
 
 msgid "Republic of Bosnia and Herzegovina"
-msgstr "Republica Bosnia-Herțegovina"
+msgstr "Republica de Bòsnia e Ercegovina"
 
 msgid "Republic of Botswana"
-msgstr "Republica Botswana"
+msgstr "Republica de Botswana"
 
 msgid "Republic of Bulgaria"
-msgstr "Republica Bulgară"
+msgstr "Republica de Bulgaria"
 
 msgid "Republic of Burundi"
-msgstr "Republica Burundi"
+msgstr "Republica de Burundi"
 
 msgid "Republic of Cabo Verde"
-msgstr "Republica Capul Verde"
+msgstr "Republica del Cap Verd"
 
 msgid "Republic of Cameroon"
-msgstr "Republica Camerun"
+msgstr "Republica de Cameron"
 
 msgid "Republic of Chad"
-msgstr "Republica Ciad"
+msgstr "Republica del Chad"
 
 msgid "Republic of Chile"
-msgstr "Republica Chile"
+msgstr "Republica del Chile"
 
 msgid "Republic of Colombia"
-msgstr "Republica Columbia"
+msgstr "Republica de Colómbia"
 
 msgid "Republic of Costa Rica"
-msgstr "Republica Costa Rica"
+msgstr "Republica de la Còsta Rica"
 
 msgid "Republic of Croatia"
-msgstr "Republica Croația"
+msgstr "Republica de Croàcia"
 
 msgid "Republic of Cuba"
-msgstr "Republica Cuba"
+msgstr "Republica de Cuba"
 
 msgid "Republic of Cyprus"
-msgstr "Republica Cipru"
+msgstr "Republica de Chipre"
 
 msgid "Republic of Côte d'Ivoire"
-msgstr "Republica Coasta de Fildeș"
+msgstr "Republica de Còsta d'Evòri"
 
 msgid "Republic of Djibouti"
-msgstr "Republica Djibouti"
+msgstr "Republica de Jiboti"
 
 msgid "Republic of Ecuador"
-msgstr "Republica Ecuador"
+msgstr "Republica de l'Eqüator"
 
 msgid "Republic of El Salvador"
-msgstr "Republica El Salvador"
+msgstr "Republica del Salvador"
 
 msgid "Republic of Equatorial Guinea"
-msgstr "Republica Guinea Ecuatorială"
+msgstr "Republica de Guinèa Eqüatoriala"
 
 msgid "Republic of Estonia"
-msgstr "Republica Estonă"
+msgstr "Republica d'Estònia"
 
 msgid "Republic of Fiji"
-msgstr "Republica Fiji"
+msgstr "Republica de Fiji"
 
 msgid "Republic of Finland"
-msgstr "Republica Finlanda"
+msgstr "Republica de Finlàndia"
 
 msgid "Republic of Ghana"
-msgstr "Republica Ghana"
+msgstr "Republica del Gana"
 
 msgid "Republic of Guatemala"
-msgstr "Republica Guatemala"
+msgstr "Republica del Guatemala"
 
 msgid "Republic of Guinea"
-msgstr "Republica Guinea"
+msgstr "Republica de Guinèa"
 
 msgid "Republic of Guinea-Bissau"
-msgstr "Republica Guinea-Bissau"
+msgstr "Republica de Guinèa Bissau"
 
 msgid "Republic of Guyana"
-msgstr "Republica Guyana"
+msgstr "Republica de Guyana"
 
 msgid "Republic of Haiti"
-msgstr "Republica Haiti"
+msgstr "Republica d’Haití"
 
 msgid "Republic of Honduras"
-msgstr "Republica Honduras"
+msgstr "Republica d'Honduras"
 
 msgid "Republic of Iceland"
-msgstr "Republica Islanda"
+msgstr "Republica d'Islàndia"
 
 msgid "Republic of India"
-msgstr "Republica India"
+msgstr "Republica d’Índia"
 
 msgid "Republic of Indonesia"
-msgstr "Republica Indonezia"
+msgstr "Republica d’Indonesia"
 
 msgid "Republic of Iraq"
-msgstr "Republica Irak"
+msgstr "Republica d’Iraq"
 
 msgid "Republic of Kazakhstan"
-msgstr "Republica Kazakhstan"
+msgstr "Republica del Cazacstan"
 
 msgid "Republic of Kenya"
-msgstr "Republica Kenia"
+msgstr "Republica del Kenya"
 
 msgid "Republic of Kiribati"
-msgstr "Republica Kiribati"
+msgstr "Republica de Kiribati"
 
 msgid "Republic of Latvia"
-msgstr "Republica Letonă"
+msgstr "Republica letona"
 
 msgid "Republic of Liberia"
-msgstr "Republica Liberia"
+msgstr "Republica de Libèria"
 
 msgid "Republic of Lithuania"
-msgstr "Republica Lituania"
+msgstr "Republica de Lituània"
 
 msgid "Republic of Madagascar"
-msgstr "Republica Madagascar"
+msgstr "Republica de Madagascar"
 
 msgid "Republic of Malawi"
-msgstr "Republica Malawi"
+msgstr "Republica de Malawi"
 
 msgid "Republic of Maldives"
-msgstr "Republica Maldive"
+msgstr "Republica de las Maldivas"
 
 msgid "Republic of Mali"
-msgstr "Republica Mali"
+msgstr "Republica de Mali"
 
 msgid "Republic of Malta"
-msgstr "Republica Malta"
+msgstr "Republica de Malta"
 
 msgid "Republic of Mauritius"
-msgstr "Republica Maurițius"
+msgstr "Republica de Maurici"
 
 msgid "Republic of Moldova"
-msgstr "Republica Moldova"
+msgstr "Republica de Moldàvia"
 
 msgid "Republic of Mozambique"
-msgstr "Republica Mozambic"
+msgstr "Republica de Moçambic"
 
 msgid "Republic of Myanmar"
-msgstr "Republica Myanmar"
+msgstr "Republica de Birmania"
 
 msgid "Republic of Namibia"
-msgstr "Republica Namibia"
+msgstr "Republica de Namibia"
 
 msgid "Republic of Nauru"
-msgstr "Republica Nauru"
+msgstr "Republica de Nauru"
 
 msgid "Republic of Nicaragua"
-msgstr "Republica Nicaragua"
+msgstr "Paraguai"
+
+msgid "Republic of North Macedonia"
+msgstr "Republica de Macedònia del Nòrd"
 
 msgid "Republic of Palau"
-msgstr "Republica Palau"
+msgstr "Republica de Belau"
 
 msgid "Republic of Panama"
-msgstr "Republica Panama"
+msgstr "Republica del Panamà"
 
 msgid "Republic of Paraguay"
-msgstr "Republica Paraguay"
+msgstr "Republica de Paraguai"
 
 msgid "Republic of Peru"
-msgstr "Republica Peru"
+msgstr "Republica del Peró"
 
 msgid "Republic of Poland"
-msgstr "Republica Polonă"
+msgstr "Republica de Polonha"
 
 msgid "Republic of San Marino"
-msgstr "Republica San Marino"
+msgstr "Republica de Sant Marin"
 
 msgid "Republic of Senegal"
-msgstr "Republica Senegal"
+msgstr "Republica de Senegal"
 
 msgid "Republic of Serbia"
-msgstr "Republica Serbia"
+msgstr "Republica de Serbia"
 
 msgid "Republic of Seychelles"
-msgstr "Republica Seychelles"
+msgstr "Republica de las Seichèlas"
 
 msgid "Republic of Sierra Leone"
-msgstr "Republica Sierra Leone"
+msgstr "Republica de Sierra Leone"
 
 msgid "Republic of Singapore"
-msgstr "Republica Singapore"
+msgstr "Republica de Singapor"
 
 msgid "Republic of Slovenia"
-msgstr "Republica Slovenă"
+msgstr "Republica d'Eslovènia"
 
 msgid "Republic of South Africa"
-msgstr "Republica Africa de sud"
+msgstr "Republica de Sudafrica"
 
 msgid "Republic of South Sudan"
-msgstr "Republica Sudanului de Sud"
+msgstr "Republica de Sodan del Sud"
 
 msgid "Republic of Suriname"
-msgstr "Republica Suriname"
+msgstr "Republica de Surinam"
 
 msgid "Republic of Tajikistan"
-msgstr "Republica Tajikistan"
+msgstr "Republica de Tatgiquistan"
 
 msgid "Republic of Trinidad and Tobago"
-msgstr "Republica Trinidad-Tobago"
+msgstr "Republica de Trinitat e Tobago"
 
 msgid "Republic of Tunisia"
-msgstr "Republica Tunisia"
+msgstr "Republica tunisiana"
+
+msgid "Republic of Türkiye"
+msgstr "Republica de Turquia"
 
 msgid "Republic of Uganda"
-msgstr "Republica Uganda"
+msgstr "Republica d’Oganda"
 
 msgid "Republic of Uzbekistan"
-msgstr "Republica Uzbekistan"
+msgstr "Republica d'Ozbequistan"
 
 msgid "Republic of Vanuatu"
-msgstr "Republica Vanuatu"
+msgstr "Republica de Vanuatu"
 
 msgid "Republic of Yemen"
-msgstr "Republica Yemen"
+msgstr "Republica de Iemèn"
 
 msgid "Republic of Zambia"
-msgstr "Republica Zambia"
+msgstr "Republica de Zambia"
 
 msgid "Republic of Zimbabwe"
-msgstr "Republica Zimbabwe"
+msgstr "Republica de Zimbabwe"
 
 msgid "Republic of the Congo"
-msgstr "Republica Congo"
+msgstr "Republica de Còngo"
+
+msgid "Republic of the Gambia"
+msgstr "Republica de Gàmbia"
 
 msgid "Republic of the Marshall Islands"
-msgstr "Republica Insulele Marshall"
+msgstr "Republica de las Illas Marshall"
 
 msgid "Republic of the Niger"
-msgstr "Republica Nigeria"
+msgstr "Republica de Nigèr"
 
 msgid "Republic of the Philippines"
-msgstr "Republica Filipine"
+msgstr "Republica de las Filipinas"
 
 msgid "Republic of the Sudan"
-msgstr "Republica Sudan"
+msgstr "Republica de Sodan"
 
 msgid "Romania"
-msgstr "România"
+msgstr "Romania"
 
 msgid "Russian Federation"
-msgstr "Federația Rusă"
+msgstr "Federacion russa"
 
 msgid "Rwanda"
 msgstr "Rwanda"
 
 msgid "Rwandese Republic"
-msgstr "Republica Rwanda"
+msgstr "Republica rewandesa"
 
 msgid "Réunion"
 msgstr "Réunion"
 
 msgid "Saint Barthélemy"
-msgstr "Sfântul Bartolomeu"
+msgstr "Sant Bertomieu"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Sfânta Elena, Ascension și Tristan da Cunha"
+msgstr "Santa Elena, Ascension, e Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "Saint Kitts și Nevis"
+msgstr "St. Kitts e Nevis"
 
 msgid "Saint Lucia"
-msgstr "Sfânta Lucia"
+msgstr "St. Lucia"
 
 msgid "Saint Martin (French part)"
-msgstr "Sfântul Martin (partea franceză)"
+msgstr "Sant Martin (Part francesa)"
 
 msgid "Saint Pierre and Miquelon"
-msgstr "Saint Pierre și Miquelon"
+msgstr "Sant Pèire e Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Saint Vincent și Grenadinele"
+msgstr "Sant Vincenç e las Grenadinas"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
-msgstr "San Marino"
+msgstr "Sant Marin"
 
 msgid "Sao Tome and Principe"
-msgstr "Sao Tome și Principe"
+msgstr "Sao Tomé e Principe"
 
 msgid "Saudi Arabia"
-msgstr "Arabia Saudită"
+msgstr "Arabia saudita"
 
 msgid "Senegal"
 msgstr "Senegal"
 
 msgid "Serbia"
 msgstr "Serbia"
 
 msgid "Seychelles"
-msgstr "Seychelles"
+msgstr "Seichèlas"
 
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
-msgstr "Singapore"
+msgstr "Singapor"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Sfântul Martin (partea olandeză)"
+msgstr "Sant Martin (Part neerlandesa)"
 
 msgid "Slovak Republic"
-msgstr "Republica Slovacă"
+msgstr "Republica eslovaquia"
 
 msgid "Slovakia"
-msgstr "Slovacia"
+msgstr "Eslovaquia"
 
 msgid "Slovenia"
-msgstr "Slovenia"
+msgstr "Eslovènia"
 
 msgid "Socialist Republic of Viet Nam"
-msgstr "Republica socialistă Vietnam"
+msgstr "Republica socialista de Vietnam"
 
 msgid "Solomon Islands"
-msgstr "Insulele Solomon"
+msgstr "Illas Salomon"
 
 msgid "Somalia"
 msgstr "Somalia"
 
 msgid "South Africa"
-msgstr "Africa de sud"
+msgstr "Sudafrica"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "Georgia de Sud și Insulele Sandwich de sud"
+msgstr "Illas Georgia del Sud e Sandwich del Sud"
+
+msgid "South Korea"
+msgstr "Corèa del Sud"
 
 msgid "South Sudan"
-msgstr "Sudanul de Sud"
+msgstr "Sodan del Sud"
 
 msgid "Spain"
-msgstr "Spania"
+msgstr "Espanha"
 
 msgid "Sri Lanka"
 msgstr "Sri Lanka"
 
 msgid "State of Israel"
-msgstr "Statul Israel"
+msgstr "Estat d'Israèl"
 
 msgid "State of Kuwait"
-msgstr "Statul Kuweit"
+msgstr "Estat de Kowait"
 
 msgid "State of Qatar"
-msgstr "Statul Qatar"
+msgstr "Estat de Qatar"
 
 msgid "Sudan"
-msgstr "Sudan"
+msgstr "Sodan"
 
 msgid "Sultanate of Oman"
-msgstr "Sultanatul Omanului"
+msgstr "Soudanat d’Oman"
 
 msgid "Suriname"
 msgstr "Surinam"
 
 msgid "Svalbard and Jan Mayen"
-msgstr "Svalbard și Jan Mayen"
+msgstr "Svalbard e Jan Mayen"
 
 msgid "Sweden"
-msgstr "Suedia"
+msgstr "Suècia"
 
 msgid "Swiss Confederation"
-msgstr "Confederația Elvețiană"
+msgstr "Confederacion Soïssa"
 
 msgid "Switzerland"
-msgstr "Elveția"
+msgstr "Soïssa"
+
+msgid "Syria"
+msgstr "Siria"
 
 msgid "Syrian Arab Republic"
-msgstr "Republica Araba Siria"
+msgstr "Republica Dominicana"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan, Province of China"
-msgstr "Taiwan"
+msgstr "Taiwan, província de China"
 
 msgid "Tajikistan"
-msgstr "Tajikistan"
+msgstr "Tatgiquistan"
 
 msgid "Tanzania"
 msgstr "Tanzania"
 
 msgid "Tanzania, United Republic of"
-msgstr "Republica Unită Tanzania"
+msgstr "Tanzania, republica unida de"
 
 msgid "Thailand"
-msgstr "Tailanda"
+msgstr "Tailàndia"
 
 msgid "Timor-Leste"
-msgstr "Timorul de Est"
+msgstr "Timòr Èst"
 
 msgid "Togo"
-msgstr "Togo"
+msgstr "Tògo"
 
 msgid "Togolese Republic"
-msgstr "Republica Togoleză"
+msgstr "Republica togolesa"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
 msgid "Tonga"
-msgstr "Tonga"
+msgstr "Tònga"
 
 msgid "Trinidad and Tobago"
-msgstr "Trinidad și Tobago"
+msgstr "Trinitat e Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
 msgid "Turkmenistan"
-msgstr "Turkmenistan"
+msgstr "Turcmenistan"
 
 msgid "Turks and Caicos Islands"
-msgstr "Insulele Turks și Caicos"
+msgstr "Illas Turcas e Caïcas"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turquia"
+
 msgid "Uganda"
-msgstr "Uganda"
+msgstr "Oganda"
 
 msgid "Ukraine"
-msgstr "Ucraina"
+msgstr "Ucraïna"
 
 msgid "Union of the Comoros"
-msgstr "Uniunea Comoros"
+msgstr "Union de las Comòras"
 
 msgid "United Arab Emirates"
-msgstr "Emiratele Arabe Unite"
+msgstr "Emirats Arabs Units"
 
 msgid "United Kingdom"
-msgstr "Regatul Unit"
+msgstr "Reialme Unit"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "Regatul Unit al Marii Britanii și Insulelor Nordice"
+msgstr "Reialme Unit de Grand Bretanha e d’Irlanda del Nòrd"
 
 msgid "United Mexican States"
-msgstr "Statele Unite Mexicane"
+msgstr "Estats Units del Mexic"
 
 msgid "United Republic of Tanzania"
-msgstr "Republica Unită Tanzania"
+msgstr "Republica unida de Tanzania"
 
 msgid "United States"
-msgstr "Statele Unite"
+msgstr "Estats Units"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Insulele de Coasta ale Statelor Unite"
+msgstr "Islas perifericas Menores dels Estats Units"
 
 msgid "United States of America"
-msgstr "Statele Unite ale Americii"
+msgstr "Estats Units d’America"
 
 msgid "Uruguay"
-msgstr "Uruguay"
+msgstr "Uruguai"
 
 msgid "Uzbekistan"
-msgstr "Uzbekistan"
+msgstr "Ozbequistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
-msgstr "Venezuela"
+msgstr "Veneçuèla"
 
 msgid "Venezuela, Bolivarian Republic of"
-msgstr "Venezuela, Republica Bolivariană"
+msgstr "Veneçuèla, Republica Dominicana bolivariana del"
 
 msgid "Viet Nam"
-msgstr "Vietnam"
+msgstr "Viet Nam"
 
 msgid "Vietnam"
 msgstr "Vietnam"
 
 msgid "Virgin Islands of the United States"
-msgstr "Insulele virgine ale Statelor Unite"
+msgstr "Islas Verges dels Estats Units d’America"
 
 msgid "Virgin Islands, British"
-msgstr "Insulele virgine (britanice)"
+msgstr "Illas Verges, britanicas"
 
 msgid "Virgin Islands, U.S."
-msgstr "Insulele virgine (SUA)"
+msgstr "illas Verges, EU"
 
 msgid "Wallis and Futuna"
-msgstr "Wallis și Futuna"
+msgstr "Wallis e Futuna"
 
 msgid "Western Sahara"
-msgstr "Sahara de Vest"
+msgstr "Sahara occidental"
 
 msgid "Yemen"
-msgstr "Yemen"
+msgstr "Iemèn"
 
 msgid "Zambia"
 msgstr "Zambia"
 
 msgid "Zimbabwe"
 msgstr "Zimbabwe"
 
 msgid "the State of Eritrea"
-msgstr "Statul Eritrea"
+msgstr "l’Estat d’Eritrèa"
 
 msgid "the State of Palestine"
-msgstr "Statul Palestina"
+msgstr "l’estat de Palestina"
 
 msgid "Åland Islands"
-msgstr "Insulele Åland"
+msgstr "llas Åland"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-09-07 21:02+0000\n"
+"PO-Revision-Date: 2023-03-10 01:39+0000\n"
 "Last-Translator: Ajeje Brazorf <lmelonimamo@yahoo.it>\n"
 "Language-Team: Sardinian <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-1/sc/>\n"
 "Language: sc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "Afghanistan"
 msgstr "Afghànistan"
 
 msgid "Albania"
 msgstr "Albania"
 
@@ -409,14 +409,17 @@
 
 msgid "India"
 msgstr "Ìndia"
 
 msgid "Indonesia"
 msgstr "Indonèsia"
 
+msgid "Iran"
+msgstr "Iràn"
+
 msgid "Iran, Islamic Republic of"
 msgstr "Iran, Repùblica Islàmica de"
 
 msgid "Iraq"
 msgstr "Iraq"
 
 msgid "Ireland"
@@ -526,14 +529,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "Kirghìzistan"
 
 msgid "Lao People's Democratic Republic"
 msgstr "Repùblica Democràtica Populare de Lao"
 
+msgid "Laos"
+msgstr "Laos"
+
 msgid "Latvia"
 msgstr "Letònia"
 
 msgid "Lebanese Republic"
 msgstr "Repùblica Libanesa"
 
 msgid "Lebanon"
@@ -1135,14 +1141,17 @@
 
 msgid "Swiss Confederation"
 msgstr "Confederatzione Isvìtzera"
 
 msgid "Switzerland"
 msgstr "Isvìtzera"
 
+msgid "Syria"
+msgstr "Sìria"
+
 msgid "Syrian Arab Republic"
 msgstr "Repùblica Àraba de Sìria"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan, Province of China"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2018-06-29 19:49+0000\n"
+"PO-Revision-Date: 2023-03-10 01:39+0000\n"
 "Last-Translator: Ajeje Brazorf <lmelonimamo@yahoo.it>\n"
 "Language-Team: Sardinian <https://hosted.weblate.org/projects/iso-codes/"
 "iso-3166-3/sc/>\n"
 "Language: sc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.1-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 msgid "British Antarctic Territory"
 msgstr "Territòriu Britànnicu Antàrticu"
 
 msgid "Burma, Socialist Republic of the Union of"
 msgstr "Birmània, Repùblica Sotzialista de s'Unione de"
 
@@ -97,9 +97,12 @@
 
 msgid "Wake Island"
 msgstr "Ìsula Wake"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
 msgstr "Yemen, Repùblica Democràtica Populare de su"
 
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Yugoslàvia, Repùblica (Sotzialista) Federale de sa"
+
 msgid "Zaire, Republic of"
 msgstr "Zaire, Repùblica de su"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,104 +1,108 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2015-12-26 21:20+0200\n"
-"Last-Translator: Miroslav Nikolić <miroslavnikolic@rocketmail.com>\n"
-"Language-Team: Serbian <(nothing)>\n"
-"Language: sr@latin\n"
+"PO-Revision-Date: 2023-02-26 15:37+0000\n"
+"Last-Translator: Oğuz Ersen <oguz@ersen.moe>\n"
+"Language-Team: Turkish <https://hosted.weblate.org/projects/iso-codes/"
+"iso-3166-3/tr/>\n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 msgid "British Antarctic Territory"
-msgstr "Britanska Antarktička Teritorija"
+msgstr "İngiliz Antarktika Bölgesi"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Burma, Socijalistička Republika Unije"
+msgstr "Burma Birliği Sosyalist Cumhuriyeti"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Beloruska SSR (Sovjetska Socijalistička Republika)"
+msgstr "Beyaz Rusya SSC Sovyet Sosyalist Cumhuriyeti"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Ostrva Kanton i Enderberi"
+msgstr "Canton ve Enderbury Adaları"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Čehoslovačka, Čehoslovačka Socijalistička Republika"
+msgstr "Çekoslovakya, Çekoslovak Sosyalist Cumhuriyeti"
 
 msgid "Dahomey"
-msgstr "Dahomej"
+msgstr "Dahomey"
 
 msgid "Dronning Maud Land"
-msgstr "Zemlja Droning Mod"
+msgstr "Kraliçe Maud Arazisi"
 
 msgid "East Timor"
-msgstr "Istočni Timor"
+msgstr "Doğu Timor"
 
 msgid "France, Metropolitan"
-msgstr "Francuska, Metropolis"
+msgstr "Fransa, Metropolitan"
 
 msgid "French Afars and Issas"
-msgstr "Francuski Afari i Ise"
+msgstr "Fransız Somalilandı"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Francuske Južne i Antarktičke Teritorije"
+msgstr "Fransız Güney ve Antarktik Bölgeleri"
 
 msgid "German Democratic Republic"
-msgstr "Nemačka Demokratska Republika"
+msgstr "Alman Demokratik Cumhuriyeti"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Ostrva Gilbert i Elis"
+msgstr "Gilbert ve Ellice Adaları"
 
 msgid "Johnston Island"
-msgstr "Ostrvo Džonston"
+msgstr "Johnston Adası"
 
 msgid "Midway Islands"
-msgstr "Ostrva Midvej"
+msgstr "Midway Adaları"
 
 msgid "Netherlands Antilles"
-msgstr "Holandski Antili"
+msgstr "Hollanda Antilleri"
 
 msgid "Neutral Zone"
-msgstr "Neutralna zona"
+msgstr "Tarafsız Bölge"
 
 msgid "New Hebrides"
-msgstr "Novi Hebridi"
+msgstr "Yeni Hebridler"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Pacifička ostrva (poverena teritorija)"
+msgstr "Pasifik Adaları (vesayet ülkeleri)"
 
 msgid "Panama Canal Zone"
-msgstr "Panamska zona kanala"
+msgstr "Panama Kanalı Bölgesi"
 
 msgid "Serbia and Montenegro"
-msgstr "Srbija i Crna Gora"
+msgstr "Sırbistan-Karadağ"
 
 msgid "Sikkim"
-msgstr "Sikim"
+msgstr "Sikkim"
 
 msgid "Southern Rhodesia"
-msgstr "Južna Rodezija"
+msgstr "Güney Rodezya"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "Razna pacifička ostrva SAD"
+msgstr "ABD Çeşitli Pasifik Adaları"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "SSSR, Savez Sovjetskih Socijalističkih Republika"
+msgstr "SSCB, Sovyet Sosyalist Cumhuriyetler Birliği"
 
 msgid "Upper Volta, Republic of"
-msgstr "Gornja Volta, Republika"
+msgstr "Yukarı Volta Cumhuriyeti"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Vijetnam, Demokratska Republika"
+msgstr "Vietnam Demokratik Cumhuriyeti"
 
 msgid "Wake Island"
-msgstr "Ostrvo Vejk"
+msgstr "Wake Adası"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr "Jemen, Demokratski, Demokratska Narodna Republika"
+msgstr "Yemen Demokratik Halk Cumhuriyeti"
+
+msgid "Yugoslavia, (Socialist) Federal Republic of"
+msgstr "Yugoslavya (Sosyalist) Federal Cumhuriyeti"
 
 msgid "Zaire, Republic of"
-msgstr "Zair, Republika"
+msgstr "Zaire Cumhuriyeti"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-3.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,108 +1,108 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2023-02-24 21:01+0000\n"
-"Last-Translator: Anders Jonsson <anders.jonsson@norsjovallen.se>\n"
-"Language-Team: Swedish <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-3/sv/>\n"
-"Language: sv\n"
+"PO-Revision-Date: 2023-04-09 22:52+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
+"Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
+"iso-codes/iso-3166-3/zh_Hant/>\n"
+"Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "British Antarctic Territory"
-msgstr "Brittiska antarktiska territoriet"
+msgstr "英屬南極洲領地"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Burman, socialistrepubliken"
+msgstr "緬甸聯邦社會主義共和國"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Vitryska SSR"
+msgstr "白俄羅斯蘇維埃社會主義共和國"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Canton och Enderburyöarna"
+msgstr "坎呑及恩得伯利群島"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Tjeckoslovakien, tjeckoslovakiska socialistrepubliken"
+msgstr "捷克斯洛伐克社會主義共和國"
 
 msgid "Dahomey"
-msgstr "Dahomey"
+msgstr "達荷美"
 
 msgid "Dronning Maud Land"
-msgstr "Drottning Mauds land"
+msgstr "莫德皇后地"
 
 msgid "East Timor"
-msgstr "Östtimor"
+msgstr "東帝汶"
 
 msgid "France, Metropolitan"
-msgstr "Frankrike, Metropolitan"
+msgstr "法國本土"
 
 msgid "French Afars and Issas"
-msgstr "Franska Afars och Issas"
+msgstr "法屬阿法爾及伊薩"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Franska antarktiska och sydterritorierna"
+msgstr "法屬南方及南極領地"
 
 msgid "German Democratic Republic"
-msgstr "Tyska demokratiska republiken"
+msgstr "德意志民主共和國"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Gilbert och Elliceöarna"
+msgstr "吉爾柏特及埃里斯群島"
 
 msgid "Johnston Island"
-msgstr "Johnstonön"
+msgstr "約翰斯頓島"
 
 msgid "Midway Islands"
-msgstr "Midwayöarna"
+msgstr "中途群島"
 
 msgid "Netherlands Antilles"
-msgstr "Nederländska Antillerna"
+msgstr "荷屬安地列斯"
 
 msgid "Neutral Zone"
-msgstr "Neutral zon"
+msgstr "中立區"
 
 msgid "New Hebrides"
-msgstr "Nya Hebriderna"
+msgstr "新赫布里"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Stillahavsöar (trust territory)"
+msgstr "太平洋島嶼託管地"
 
 msgid "Panama Canal Zone"
-msgstr "Panamas kanalzon"
+msgstr "巴拿馬運河區"
 
 msgid "Serbia and Montenegro"
-msgstr "Serbien och Montenegro"
+msgstr "塞爾維亞及蒙特內哥羅"
 
 msgid "Sikkim"
-msgstr "Sikkim"
+msgstr "錫金"
 
 msgid "Southern Rhodesia"
-msgstr "Södra Rhodesia"
+msgstr "南羅得西亞"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "Diverse amerikanska stillahavsöar"
+msgstr "美屬太平洋諸島"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "Sovjetunionen"
+msgstr "蘇維埃社會主義共和國聯邦"
 
 msgid "Upper Volta, Republic of"
-msgstr "Övre Volta, republiken"
+msgstr "上伏塔共和國"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Vietnam, demokratiska republiken"
+msgstr "越南民主共和國"
 
 msgid "Wake Island"
-msgstr "Wakeöarna"
+msgstr "威克島"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr "Jemen, demokratiska, demokratiska folkrepubliken"
+msgstr "葉門民主人民共和國"
 
 msgid "Yugoslavia, (Socialist) Federal Republic of"
-msgstr "Jugoslavien, socialistiska federativa republiken"
+msgstr "南斯拉夫社會主義聯邦共和國"
 
 msgid "Zaire, Republic of"
-msgstr "Zaire, republiken"
+msgstr "薩伊共和國"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-3.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,108 +1,108 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-3\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2023-02-26 15:37+0000\n"
-"Last-Translator: Oğuz Ersen <oguz@ersen.moe>\n"
-"Language-Team: Turkish <https://hosted.weblate.org/projects/iso-codes/"
-"iso-3166-3/tr/>\n"
-"Language: tr\n"
+"PO-Revision-Date: 2023-04-10 05:19+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
+"Language-Team: Chinese (Traditional, Hong Kong) <https://hosted.weblate.org/"
+"projects/iso-codes/iso-3166-3/zh_Hant_HK/>\n"
+"Language: zh_HK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "British Antarctic Territory"
-msgstr "İngiliz Antarktika Bölgesi"
+msgstr "英屬南極洲地區"
 
 msgid "Burma, Socialist Republic of the Union of"
-msgstr "Burma Birliği Sosyalist Cumhuriyeti"
+msgstr "緬甸聯邦社會主義共和國"
 
 msgid "Byelorussian SSR Soviet Socialist Republic"
-msgstr "Beyaz Rusya SSC Sovyet Sosyalist Cumhuriyeti"
+msgstr "白俄羅斯蘇維埃社會主義共和國"
 
 msgid "Canton and Enderbury Islands"
-msgstr "Canton ve Enderbury Adaları"
+msgstr "坎頓和恩德貝里羣島"
 
 msgid "Czechoslovakia, Czechoslovak Socialist Republic"
-msgstr "Çekoslovakya, Çekoslovak Sosyalist Cumhuriyeti"
+msgstr "捷克斯洛伐克社會主義共和國"
 
 msgid "Dahomey"
-msgstr "Dahomey"
+msgstr "達荷美"
 
 msgid "Dronning Maud Land"
-msgstr "Kraliçe Maud Arazisi"
+msgstr "慕德皇后地"
 
 msgid "East Timor"
-msgstr "Doğu Timor"
+msgstr "東帝汶"
 
 msgid "France, Metropolitan"
-msgstr "Fransa, Metropolitan"
+msgstr "法國本土"
 
 msgid "French Afars and Issas"
-msgstr "Fransız Somalilandı"
+msgstr "阿法爾及伊薩"
 
 msgid "French Southern and Antarctic Territories"
-msgstr "Fransız Güney ve Antarktik Bölgeleri"
+msgstr "法屬南半球及南極屬地"
 
 msgid "German Democratic Republic"
-msgstr "Alman Demokratik Cumhuriyeti"
+msgstr "德意志民主共和國"
 
 msgid "Gilbert and Ellice Islands"
-msgstr "Gilbert ve Ellice Adaları"
+msgstr "吉爾柏特及埃里斯羣島"
 
 msgid "Johnston Island"
-msgstr "Johnston Adası"
+msgstr "強斯頓環礁"
 
 msgid "Midway Islands"
-msgstr "Midway Adaları"
+msgstr "中途羣島"
 
 msgid "Netherlands Antilles"
-msgstr "Hollanda Antilleri"
+msgstr "荷屬安的列斯羣島"
 
 msgid "Neutral Zone"
-msgstr "Tarafsız Bölge"
+msgstr "中立區"
 
 msgid "New Hebrides"
-msgstr "Yeni Hebridler"
+msgstr "新赫布里底羣島"
 
 msgid "Pacific Islands (trust territory)"
-msgstr "Pasifik Adaları (vesayet ülkeleri)"
+msgstr "太平洋島嶼（託管地）"
 
 msgid "Panama Canal Zone"
-msgstr "Panama Kanalı Bölgesi"
+msgstr "巴拿馬運河區"
 
 msgid "Serbia and Montenegro"
-msgstr "Sırbistan-Karadağ"
+msgstr "塞爾維亞和黑山"
 
 msgid "Sikkim"
-msgstr "Sikkim"
+msgstr "錫金"
 
 msgid "Southern Rhodesia"
-msgstr "Güney Rodezya"
+msgstr "南羅得西亞"
 
 msgid "US Miscellaneous Pacific Islands"
-msgstr "ABD Çeşitli Pasifik Adaları"
+msgstr "美屬太平洋島嶼"
 
 msgid "USSR, Union of Soviet Socialist Republics"
-msgstr "SSCB, Sovyet Sosyalist Cumhuriyetler Birliği"
+msgstr "蘇維埃社會主義共和國聯邦"
 
 msgid "Upper Volta, Republic of"
-msgstr "Yukarı Volta Cumhuriyeti"
+msgstr "上沃爾特共和國"
 
 msgid "Viet-Nam, Democratic Republic of"
-msgstr "Vietnam Demokratik Cumhuriyeti"
+msgstr "越南民主共和國"
 
 msgid "Wake Island"
-msgstr "Wake Adası"
+msgstr "威克島"
 
 msgid "Yemen, Democratic, People's Democratic Republic of"
-msgstr "Yemen Demokratik Halk Cumhuriyeti"
+msgstr "也門民主人民共和國"
 
 msgid "Yugoslavia, (Socialist) Federal Republic of"
-msgstr "Yugoslavya (Sosyalist) Federal Cumhuriyeti"
+msgstr "南斯拉夫社會主義聯邦共和國"
 
 msgid "Zaire, Republic of"
-msgstr "Zaire Cumhuriyeti"
+msgstr "扎伊爾共和國"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2019-09-26 07:28+0000\n"
-"Last-Translator: Walter Cheuk <wwycheuk@gmail.com>\n"
-"Language-Team: Chinese (Hong Kong) <https://hosted.weblate.org/projects/iso-"
-"codes/iso-3166-1/zh_Hant_HK/>\n"
+"PO-Revision-Date: 2023-04-10 05:19+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
+"Language-Team: Chinese (Traditional, Hong Kong) <https://hosted.weblate.org/"
+"projects/iso-codes/iso-3166-1/zh_Hant_HK/>\n"
 "Language: zh_HK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 3.9-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "Afghanistan"
 msgstr "阿富汗"
 
 msgid "Albania"
 msgstr "阿爾巴尼亞"
 
@@ -50,15 +50,15 @@
 msgid "Argentine Republic"
 msgstr "阿根廷共和國"
 
 msgid "Armenia"
 msgstr "亞美尼亞"
 
 msgid "Aruba"
-msgstr "阿盧巴島"
+msgstr "阿魯巴"
 
 msgid "Australia"
 msgstr "澳大利亞"
 
 msgid "Austria"
 msgstr "奧地利"
 
@@ -251,15 +251,15 @@
 msgid "Egypt"
 msgstr "埃及"
 
 msgid "El Salvador"
 msgstr "薩爾瓦多"
 
 msgid "Equatorial Guinea"
-msgstr "赤道畿內亞"
+msgstr "赤道幾內亞"
 
 msgid "Eritrea"
 msgstr "厄立特里亞"
 
 msgid "Estonia"
 msgstr "愛沙尼亞"
 
@@ -311,15 +311,15 @@
 msgid "French Polynesia"
 msgstr "法屬玻利尼西亞"
 
 msgid "French Republic"
 msgstr "法蘭西共和國"
 
 msgid "French Southern Territories"
-msgstr "法屬南部屬地"
+msgstr "法屬南半球領土"
 
 msgid "Gabon"
 msgstr "加蓬"
 
 msgid "Gabonese Republic"
 msgstr "加蓬共和國"
 
@@ -359,18 +359,18 @@
 msgid "Guatemala"
 msgstr "危地馬拉"
 
 msgid "Guernsey"
 msgstr "根息"
 
 msgid "Guinea"
-msgstr "畿內亞"
+msgstr "幾內亞"
 
 msgid "Guinea-Bissau"
-msgstr "畿內亞比紹"
+msgstr "幾內亞比紹"
 
 msgid "Guyana"
 msgstr "圭亞那"
 
 msgid "Haiti"
 msgstr "海地"
 
@@ -398,25 +398,28 @@
 msgid "Hungary"
 msgstr "匈牙利"
 
 msgid "Iceland"
 msgstr "冰島"
 
 msgid "Independent State of Papua New Guinea"
-msgstr "巴布亞新畿內亞獨立國"
+msgstr "巴布亞新幾內亞獨立國"
 
 msgid "Independent State of Samoa"
 msgstr "薩摩亞獨立國"
 
 msgid "India"
 msgstr "印度"
 
 msgid "Indonesia"
 msgstr "印尼"
 
+msgid "Iran"
+msgstr "伊朗"
+
 msgid "Iran, Islamic Republic of"
 msgstr "伊朗"
 
 msgid "Iraq"
 msgstr "伊拉克"
 
 msgid "Ireland"
@@ -458,15 +461,15 @@
 msgid "Jordan"
 msgstr "約旦"
 
 msgid "Kazakhstan"
 msgstr "哈薩克"
 
 msgid "Kenya"
-msgstr "肯雅"
+msgstr "肯尼亞"
 
 msgid "Kingdom of Bahrain"
 msgstr "巴林王國"
 
 msgid "Kingdom of Belgium"
 msgstr "比利時王國"
 
@@ -526,14 +529,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "吉爾吉斯"
 
 msgid "Lao People's Democratic Republic"
 msgstr "老撾人民民主共和國"
 
+msgid "Laos"
+msgstr "老撾"
+
 msgid "Latvia"
 msgstr "拉脫維亞"
 
 msgid "Lebanese Republic"
 msgstr "黎巴嫩共和國"
 
 msgid "Lebanon"
@@ -587,15 +593,15 @@
 msgid "Martinique"
 msgstr "法屬馬丁尼克"
 
 msgid "Mauritania"
 msgstr "毛里塔尼亞"
 
 msgid "Mauritius"
-msgstr "毛里裘斯"
+msgstr "毛里求斯"
 
 msgid "Mayotte"
 msgstr "美亞特"
 
 msgid "Mexico"
 msgstr "墨西哥"
 
@@ -658,14 +664,17 @@
 
 msgid "Niue"
 msgstr "紐威島"
 
 msgid "Norfolk Island"
 msgstr "諾福克羣島"
 
+msgid "North Korea"
+msgstr "北韓"
+
 msgid "North Macedonia"
 msgstr "北馬其頓"
 
 msgid "Northern Mariana Islands"
 msgstr "北馬里亞納羣島"
 
 msgid "Norway"
@@ -683,15 +692,15 @@
 msgid "Palestine, State of"
 msgstr "巴勒斯坦"
 
 msgid "Panama"
 msgstr "巴拿馬"
 
 msgid "Papua New Guinea"
-msgstr "巴布亞新畿內亞"
+msgstr "巴布亞新幾內亞"
 
 msgid "Paraguay"
 msgstr "巴拉圭"
 
 msgid "People's Democratic Republic of Algeria"
 msgstr "阿爾及利亞民主人民共和國"
 
@@ -806,15 +815,15 @@
 msgid "Republic of Ecuador"
 msgstr "厄瓜多爾共和國"
 
 msgid "Republic of El Salvador"
 msgstr "薩爾瓦多共和國"
 
 msgid "Republic of Equatorial Guinea"
-msgstr "赤道畿內亞共和國"
+msgstr "赤道幾內亞共和國"
 
 msgid "Republic of Estonia"
 msgstr "愛沙尼亞共和國"
 
 msgid "Republic of Fiji"
 msgstr "斐濟共和國"
 
@@ -824,18 +833,18 @@
 msgid "Republic of Ghana"
 msgstr "加納共和國"
 
 msgid "Republic of Guatemala"
 msgstr "危地馬拉共和國"
 
 msgid "Republic of Guinea"
-msgstr "畿內亞共和國"
+msgstr "幾內亞共和國"
 
 msgid "Republic of Guinea-Bissau"
-msgstr "畿內亞比紹共和國"
+msgstr "幾內亞比紹共和國"
 
 msgid "Republic of Guyana"
 msgstr "圭亞那合作共和國"
 
 msgid "Republic of Haiti"
 msgstr "海地共和國"
 
@@ -854,15 +863,15 @@
 msgid "Republic of Iraq"
 msgstr "伊拉克共和國"
 
 msgid "Republic of Kazakhstan"
 msgstr "哈薩克斯坦共和國"
 
 msgid "Republic of Kenya"
-msgstr "肯雅共和國"
+msgstr "肯尼亞共和國"
 
 msgid "Republic of Kiribati"
 msgstr "基里巴斯共和國"
 
 msgid "Republic of Latvia"
 msgstr "拉脫維亞共和國"
 
@@ -884,15 +893,15 @@
 msgid "Republic of Mali"
 msgstr "馬里共和國"
 
 msgid "Republic of Malta"
 msgstr "馬耳他共和國"
 
 msgid "Republic of Mauritius"
-msgstr "毛里裘斯共和國"
+msgstr "毛里求斯共和國"
 
 msgid "Republic of Moldova"
 msgstr "摩爾多瓦共和國"
 
 msgid "Republic of Mozambique"
 msgstr "莫桑比克共和國"
 
@@ -961,14 +970,17 @@
 
 msgid "Republic of Trinidad and Tobago"
 msgstr "特立尼達和多巴哥共和國"
 
 msgid "Republic of Tunisia"
 msgstr "突尼斯共和國"
 
+msgid "Republic of Türkiye"
+msgstr "土耳其共和國"
+
 msgid "Republic of Uganda"
 msgstr "烏干達共和國"
 
 msgid "Republic of Uzbekistan"
 msgstr "烏茲別克斯坦共和國"
 
 msgid "Republic of Vanuatu"
@@ -1025,15 +1037,15 @@
 msgid "Saint Kitts and Nevis"
 msgstr "聖基茨和尼維斯聯邦"
 
 msgid "Saint Lucia"
 msgstr "聖盧西亞"
 
 msgid "Saint Martin (French part)"
-msgstr "聖馬丁 (法屬)"
+msgstr "聖馬丁（法屬）"
 
 msgid "Saint Pierre and Miquelon"
 msgstr "聖皮耶及密克隆羣島"
 
 msgid "Saint Vincent and the Grenadines"
 msgstr "聖文森特和格林納丁斯"
 
@@ -1087,14 +1099,17 @@
 
 msgid "South Africa"
 msgstr "南非"
 
 msgid "South Georgia and the South Sandwich Islands"
 msgstr "南佐治亞及南三文治羣島"
 
+msgid "South Korea"
+msgstr "南韓"
+
 msgid "South Sudan"
 msgstr "南蘇丹"
 
 msgid "Spain"
 msgstr "西班牙"
 
 msgid "Sri Lanka"
@@ -1126,14 +1141,17 @@
 
 msgid "Swiss Confederation"
 msgstr "瑞士聯邦"
 
 msgid "Switzerland"
 msgstr "瑞士"
 
+msgid "Syria"
+msgstr "敍利亞"
+
 msgid "Syrian Arab Republic"
 msgstr "阿拉伯敍利亞共和國"
 
 msgid "Taiwan"
 msgstr "台灣"
 
 msgid "Taiwan, Province of China"
@@ -1142,15 +1160,15 @@
 msgid "Tajikistan"
 msgstr "塔吉克斯坦"
 
 msgid "Tanzania"
 msgstr "坦桑尼亞"
 
 msgid "Tanzania, United Republic of"
-msgstr "坦桑尼亞"
+msgstr "坦桑尼亞聯合共和國"
 
 msgid "Thailand"
 msgstr "泰國"
 
 msgid "Timor-Leste"
 msgstr "東帝汶"
 
@@ -1177,14 +1195,17 @@
 
 msgid "Turks and Caicos Islands"
 msgstr "土克凱可羣島"
 
 msgid "Tuvalu"
 msgstr "圖瓦盧"
 
+msgid "Türkiye"
+msgstr "土耳其"
+
 msgid "Uganda"
 msgstr "烏干達"
 
 msgid "Ukraine"
 msgstr "烏克蘭"
 
 msgid "Union of the Comoros"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,79 +1,79 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_639-2\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-02-22 02:55+0000\n"
-"Last-Translator: Jack Liu <ywp033319@gmail.com>\n"
-"Language-Team: Chinese (Traditional, Hong Kong) <https://hosted.weblate.org/"
-"projects/iso-codes/iso-639-2/zh_Hant_HK/>\n"
-"Language: zh_HK\n"
+"PO-Revision-Date: 2023-04-09 22:52+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
+"Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
+"iso-codes/iso-639-2/zh_Hant/>\n"
+"Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "Abkhazian"
-msgstr "阿布哈茲語"
+msgstr "亞布卡薩語"
 
 msgid "Achinese"
 msgstr "亞齊語"
 
 msgid "Acoli"
 msgstr "阿喬利語"
 
 msgid "Adangme"
 msgstr "阿當梅語"
 
 msgid "Adyghe; Adygei"
-msgstr "阿迪格語"
+msgstr "阿迪何語"
 
 msgid "Afar"
 msgstr "阿法爾語"
 
 msgid "Afrihili"
 msgstr "阿弗里希利語"
 
 msgid "Afrikaans"
-msgstr "南非荷蘭語"
+msgstr "南非荷蘭文"
 
 msgid "Afro-Asiatic languages"
 msgstr "亞非語系"
 
 msgid "Ainu"
 msgstr "阿依努語"
 
 msgid "Akan"
-msgstr "阿坎語"
+msgstr "迦納語"
 
 msgid "Akkadian"
 msgstr "阿卡德語"
 
 msgid "Albanian"
 msgstr "阿爾巴尼亞語"
 
 msgid "Aleut"
 msgstr "阿留申語"
 
 msgid "Algonquian languages"
-msgstr "阿爾岡昆諸語言"
+msgstr "阿爾岡基語系"
 
 msgid "Altaic languages"
 msgstr "阿爾泰語系"
 
 msgid "Amharic"
 msgstr "阿姆哈拉語"
 
 msgid "Angika"
 msgstr "昂加語"
 
 msgid "Apache languages"
-msgstr "阿帕切諸語言"
+msgstr "阿帕契語系"
 
 msgid "Arabic"
 msgstr "阿拉伯語"
 
 msgid "Aragonese"
 msgstr "阿拉貢語"
 
@@ -95,75 +95,75 @@
 msgid "Assamese"
 msgstr "阿薩姆語"
 
 msgid "Asturian; Bable; Leonese; Asturleonese"
 msgstr "阿斯圖里亞斯語"
 
 msgid "Athapascan languages"
-msgstr "阿薩帕斯坎諸語言"
+msgstr "阿薩帕斯坎語系"
 
 msgid "Australian languages"
-msgstr "澳大利亞諸語言"
+msgstr "澳大利亞語系"
 
 msgid "Austronesian languages"
 msgstr "南島語系"
 
 msgid "Avaric"
 msgstr "阿瓦爾語"
 
 msgid "Avestan"
-msgstr "阿維斯陀語"
+msgstr "阿維斯語"
 
 msgid "Awadhi"
 msgstr "阿瓦德語"
 
 msgid "Aymara"
-msgstr "艾馬拉語"
+msgstr "亞摩拉語"
 
 msgid "Azerbaijani"
-msgstr "阿塞拜疆語"
+msgstr "亞塞拜然語"
 
 msgid "Balinese"
 msgstr "峇里語"
 
 msgid "Baltic languages"
 msgstr "波羅的語系"
 
 msgid "Baluchi"
 msgstr "俾路支語"
 
 msgid "Bambara"
 msgstr "班巴拉語"
 
 msgid "Bamileke languages"
-msgstr "巴米累克諸語言"
+msgstr "巴米雷克語系"
 
 msgid "Banda languages"
-msgstr "班達語"
+msgstr "班達語系"
 
 msgid "Bangla"
-msgstr "孟加拉文"
+msgstr "孟加拉語"
 
 msgid "Bantu (Other)"
 msgstr "班圖語 (其他)"
 
 msgid "Basa"
 msgstr "巴薩語"
 
 msgid "Bashkir"
-msgstr "巴什基爾語"
+msgstr "巴什喀爾語"
 
 msgid "Basque"
 msgstr "巴斯克語"
 
 msgid "Batak languages"
-msgstr "巴塔克語"
+msgstr "巴塔克語系"
 
 msgid "Beja; Bedawiyet"
-msgstr "貝扎文"
+msgstr "貝札語"
 
 msgid "Belarusian"
 msgstr "白俄羅斯語"
 
 msgid "Bemba"
 msgstr "本巴語"
 
@@ -179,33 +179,39 @@
 msgid "Bihari languages"
 msgstr "比哈爾語系"
 
 msgid "Bikol"
 msgstr "比科爾語"
 
 msgid "Bini; Edo"
-msgstr "比尼語"
+msgstr "艾鬥語"
 
 msgid "Bislama"
-msgstr "比斯拉瑪語"
+msgstr "比斯拉馬語"
 
 msgid "Blin; Bilin"
 msgstr "比林語"
 
+msgid "Blissymbols; Blissymbolics; Bliss"
+msgstr "布利斯符號"
+
+msgid "Bokmål, Norwegian; Norwegian Bokmål"
+msgstr "書面挪威語"
+
 msgid "Bosnian"
-msgstr "波斯尼亞語"
+msgstr "波士尼亞語"
 
 msgid "Braj"
 msgstr "布拉吉語"
 
 msgid "Breton"
-msgstr "布里多尼語"
+msgstr "布里敦語"
 
 msgid "Buginese"
-msgstr "布吉語"
+msgstr "布吉斯語"
 
 msgid "Bulgarian"
 msgstr "保加利亞語"
 
 msgid "Buriat"
 msgstr "布里亞特語"
 
@@ -224,51 +230,51 @@
 msgid "Cebuano"
 msgstr "宿霧語"
 
 msgid "Celtic languages"
 msgstr "凱爾特語系"
 
 msgid "Central American Indian languages"
-msgstr "中美洲印第安諸語言"
+msgstr "中美洲原住民語系"
 
 msgid "Central Khmer"
-msgstr "高棉語"
+msgstr "中央高棉語"
 
 msgid "Chagatai"
-msgstr "查加台語"
+msgstr "察合臺語"
 
 msgid "Chamic languages"
-msgstr "占語諸語言"
+msgstr "查米克語系"
 
 msgid "Chamorro"
 msgstr "查莫羅語"
 
 msgid "Chechen"
 msgstr "車臣語"
 
 msgid "Cherokee"
-msgstr "切羅基語"
+msgstr "卻洛奇語"
 
 msgid "Cheyenne"
 msgstr "夏延語"
 
 msgid "Chibcha"
 msgstr "奇布查語"
 
 msgid "Chichewa; Chewa; Nyanja"
-msgstr "尼揚賈語"
+msgstr "契切瓦語"
 
 msgid "Chinese"
 msgstr "中文"
 
 msgid "Chinook jargon"
 msgstr "奇努克混合語"
 
 msgid "Chipewyan; Dene Suline"
-msgstr "奇佩維安文"
+msgstr "奇佩維安語"
 
 msgid "Choctaw"
 msgstr "喬克托語"
 
 msgid ""
 "Church Slavic; Old Slavonic; Church Slavonic; Old Bulgarian; Old Church "
 "Slavonic"
@@ -277,18 +283,18 @@
 msgid "Chuukese"
 msgstr "丘克語"
 
 msgid "Chuvash"
 msgstr "楚瓦什語"
 
 msgid "Classical Newari; Old Newari; Classical Nepal Bhasa"
-msgstr "尼瓦爾語"
+msgstr "古尼瓦爾語"
 
 msgid "Classical Syriac"
-msgstr "古敍利亞文"
+msgstr "古敘利亞語"
 
 msgid "Coptic"
 msgstr "科普特語"
 
 msgid "Cornish"
 msgstr "康沃爾語"
 
@@ -297,73 +303,82 @@
 
 msgid "Cree"
 msgstr "克里語"
 
 msgid "Creek"
 msgstr "克里克語"
 
+msgid "Creoles and pidgins"
+msgstr "混合語"
+
 msgid "Creoles and pidgins, English based"
 msgstr "英語克里奧爾混合語"
 
 msgid "Creoles and pidgins, French-based"
 msgstr "法語克里奧爾混合語"
 
 msgid "Creoles and pidgins, Portuguese-based"
-msgstr "葡萄牙語克里奧爾混合語"
+msgstr "葡萄牙語克里奧爾混合語系"
 
 msgid "Crimean Tatar; Crimean Turkish"
 msgstr "克里米亞韃靼語"
 
 msgid "Croatian"
-msgstr "克羅地亞語"
+msgstr "克羅埃西亞語"
+
+msgid "Cushitic languages"
+msgstr "庫希特語系"
 
 msgid "Czech"
 msgstr "捷克語"
 
 msgid "Dakota"
 msgstr "達科他語"
 
 msgid "Danish"
 msgstr "丹麥語"
 
 msgid "Dargwa"
 msgstr "達爾格瓦語"
 
 msgid "Delaware"
-msgstr "特拉華語"
+msgstr "德拉瓦語"
 
 msgid "Dinka"
 msgstr "丁卡語"
 
 msgid "Divehi; Dhivehi; Maldivian"
-msgstr "迪維希語"
+msgstr "迪維西語"
 
 msgid "Dogri"
 msgstr "多格拉語"
 
 msgid "Dogrib"
 msgstr "多格里布語"
 
+msgid "Dravidian languages"
+msgstr "達羅毗荼語系"
+
 msgid "Duala"
 msgstr "杜亞拉語"
 
 msgid "Dutch, Middle (ca. 1050-1350)"
-msgstr "中古荷蘭語"
+msgstr "中古荷蘭語 (約 1050-1350)"
 
 msgid "Dutch; Flemish"
 msgstr "荷蘭語"
 
 msgid "Dyula"
 msgstr "迪尤拉語"
 
 msgid "Dzongkha"
-msgstr "不丹語"
+msgstr "宗卡語(不丹)"
 
 msgid "Eastern Frisian"
-msgstr "東弗里西亞語"
+msgstr "東夫里斯蘭語"
 
 msgid "Efik"
 msgstr "埃菲克語"
 
 msgid "Egyptian (Ancient)"
 msgstr "古埃及語"
 
@@ -373,18 +388,18 @@
 msgid "Elamite"
 msgstr "埃蘭語"
 
 msgid "English"
 msgstr "英文"
 
 msgid "English, Middle (1100-1500)"
-msgstr "中古英文"
+msgstr "中古英語 (1100-1500)"
 
 msgid "English, Old (ca. 450-1100)"
-msgstr "古英語"
+msgstr "古英語 (約 450-1100)"
 
 msgid "Erzya"
 msgstr "厄爾茲亞語"
 
 msgid "Esperanto"
 msgstr "世界語"
 
@@ -400,144 +415,150 @@
 msgid "Fang"
 msgstr "芳語"
 
 msgid "Fanti"
 msgstr "芳蒂語"
 
 msgid "Faroese"
-msgstr "法羅語"
+msgstr "法羅群島語"
 
 msgid "Fijian"
 msgstr "斐濟語"
 
 msgid "Filipino; Pilipino"
 msgstr "菲律賓語"
 
 msgid "Finnish"
 msgstr "芬蘭語"
 
+msgid "Finno-Ugrian languages"
+msgstr "芬蘭-烏戈爾語系"
+
 msgid "Fon"
 msgstr "豐語"
 
 msgid "French"
-msgstr "法文"
+msgstr "法語"
 
 msgid "French, Middle (ca. 1400-1600)"
-msgstr "中古法文"
+msgstr "中古法語 (約 1400-1600)"
 
 msgid "French, Old (842-ca. 1400)"
-msgstr "古法文"
+msgstr "古法語 (842-約 1400)"
 
 msgid "Friulian"
 msgstr "弗留利語"
 
 msgid "Fulah"
 msgstr "富拉語"
 
 msgid "Ga"
-msgstr "加語"
+msgstr "格語"
 
 msgid "Gaelic; Scottish Gaelic"
 msgstr "蓋爾語"
 
 msgid "Galibi Carib"
-msgstr "加勒比諸語言"
+msgstr "加勒比語"
 
 msgid "Galician"
-msgstr "加利西亞語"
+msgstr "加里斯亞語"
 
 msgid "Ganda"
 msgstr "干達語"
 
 msgid "Gayo"
 msgstr "卡約語"
 
 msgid "Gbaya"
 msgstr "巴亞語"
 
 msgid "Geez"
 msgstr "吉茲語"
 
 msgid "Georgian"
-msgstr "格魯吉亞語"
+msgstr "喬治亞語"
 
 msgid "German"
-msgstr "德文"
+msgstr "德語"
 
 msgid "German, Middle High (ca. 1050-1500)"
-msgstr "中古高地德文"
+msgstr "中古高地德語 (約 1050-1500)"
 
 msgid "German, Old High (ca. 750-1050)"
-msgstr "古高地德文"
+msgstr "古高地德語 (約 750-1050)"
 
 msgid "Germanic languages"
 msgstr "日耳曼語系"
 
 msgid "Gilbertese"
 msgstr "吉伯特語"
 
 msgid "Gondi"
 msgstr "貢德語"
 
 msgid "Gorontalo"
 msgstr "哥倫打洛語"
 
 msgid "Gothic"
-msgstr "哥特語"
+msgstr "哥德語"
 
 msgid "Grebo"
 msgstr "格列博語"
 
 msgid "Greek, Ancient (to 1453)"
-msgstr "古希臘語"
+msgstr "古希臘語 (到 1453)"
 
 msgid "Greek, Modern (1453-)"
-msgstr "現代希臘語"
+msgstr "現代希臘語 (1453-)"
 
 msgid "Guarani"
 msgstr "巴拉圭瓜拉尼"
 
 msgid "Gujarati"
 msgstr "古吉拉特語"
 
 msgid "Gwich'in"
 msgstr "庫臣語"
 
 msgid "Haida"
 msgstr "海達語"
 
 msgid "Haitian; Haitian Creole"
-msgstr "海地克里奧爾語"
+msgstr "克里奧爾語(海地)"
 
 msgid "Hausa"
-msgstr "豪薩語"
+msgstr "豪撒語(蘇丹)"
 
 msgid "Hawaiian"
 msgstr "夏威夷語"
 
 msgid "Hebrew"
 msgstr "希伯來語"
 
 msgid "Herero"
 msgstr "赫雷羅語"
 
 msgid "Hiligaynon"
 msgstr "希利蓋農語"
 
+msgid "Himachali languages; Western Pahari languages"
+msgstr "喜馬偕爾諸語言；西帕哈爾諸語言"
+
 msgid "Hindi"
-msgstr "印地語"
+msgstr "印地語(北印度)"
 
 msgid "Hiri Motu"
 msgstr "希里莫圖語"
 
 msgid "Hittite"
 msgstr "赫梯語"
 
 msgid "Hmong; Mong"
-msgstr "苗文"
+msgstr "苗語"
 
 msgid "Hungarian"
 msgstr "匈牙利語"
 
 msgid "Hupa"
 msgstr "胡帕語"
 
@@ -547,24 +568,24 @@
 msgid "Icelandic"
 msgstr "冰島語"
 
 msgid "Ido"
 msgstr "伊多語"
 
 msgid "Igbo"
-msgstr "伊博語"
+msgstr "伊布語"
 
 msgid "Ijo languages"
-msgstr "伊喬語"
+msgstr "伊喬語系"
 
 msgid "Iloko"
 msgstr "伊洛卡諾語"
 
 msgid "Inari Sami"
-msgstr "伊納里薩莫斯語"
+msgstr "伊納里薩米語"
 
 msgid "Indic languages"
 msgstr "印度語系"
 
 msgid "Indo-European languages"
 msgstr "印歐語系"
 
@@ -577,39 +598,39 @@
 msgid "Interlingua (International Auxiliary Language Association)"
 msgstr "拉丁國際語"
 
 msgid "Interlingue; Occidental"
 msgstr "國際語"
 
 msgid "Inuktitut"
-msgstr "伊努伊特語"
+msgstr "伊努特語"
 
 msgid "Inupiaq"
 msgstr "依努庇克語"
 
 msgid "Iranian languages"
 msgstr "伊朗語系"
 
 msgid "Irish"
 msgstr "愛爾蘭語"
 
 msgid "Irish, Middle (900-1200)"
-msgstr "中古愛爾蘭語"
+msgstr "中古愛爾蘭語 (900-1200)"
 
 msgid "Irish, Old (to 900)"
-msgstr "古愛爾蘭語"
+msgstr "古愛爾蘭語 (至 900)"
 
 msgid "Iroquoian languages"
-msgstr "易洛魁語"
+msgstr "易洛魁語系"
 
 msgid "Italian"
-msgstr "意大利語"
+msgstr "義大利語"
 
 msgid "Japanese"
-msgstr "日文"
+msgstr "日語"
 
 msgid "Javanese"
 msgstr "爪哇語"
 
 msgid "Judeo-Arabic"
 msgstr "猶太-阿拉伯語"
 
@@ -628,36 +649,36 @@
 msgid "Kalaallisut; Greenlandic"
 msgstr "格陵蘭語"
 
 msgid "Kalmyk; Oirat"
 msgstr "卡爾梅克語"
 
 msgid "Kamba"
-msgstr "坎巴語"
+msgstr "卡姆帕語"
 
 msgid "Kannada"
 msgstr "卡納達語"
 
 msgid "Kanuri"
 msgstr "卡努里語"
 
 msgid "Kara-Kalpak"
-msgstr "卡拉卡爾帕克語"
+msgstr "卡拉-卡爾帕克語"
 
 msgid "Karachay-Balkar"
 msgstr "卡拉恰伊-巴爾卡爾語"
 
 msgid "Karelian"
 msgstr "卡累利阿語"
 
 msgid "Karen languages"
-msgstr "克倫語"
+msgstr "克倫語系"
 
 msgid "Kashmiri"
-msgstr "克什米爾語"
+msgstr "喀什米爾語"
 
 msgid "Kashubian"
 msgstr "卡舒比語"
 
 msgid "Kawi"
 msgstr "卡威語"
 
@@ -676,51 +697,51 @@
 msgid "Kikuyu; Gikuyu"
 msgstr "基庫尤語"
 
 msgid "Kimbundu"
 msgstr "金本杜語"
 
 msgid "Kinyarwanda"
-msgstr "基尼阿萬達語"
+msgstr "盧安達語"
 
 msgid "Kirghiz; Kyrgyz"
 msgstr "吉爾吉斯語"
 
 msgid "Klingon; tlhIngan-Hol"
 msgstr "克林貢語"
 
 msgid "Komi"
 msgstr "科米語"
 
 msgid "Kongo"
 msgstr "剛果語"
 
 msgid "Konkani"
-msgstr "孔卡尼語"
+msgstr "貢根語"
 
 msgid "Korean"
-msgstr "韓文"
+msgstr "韓語"
 
 msgid "Kosraean"
 msgstr "科斯拉伊語"
 
 msgid "Kpelle"
 msgstr "克佩勒語"
 
 msgid "Kru languages"
-msgstr "克魯語"
+msgstr "克魯語系"
 
 msgid "Kuanyama; Kwanyama"
 msgstr "寬亞瑪語"
 
 msgid "Kumyk"
 msgstr "庫梅克語"
 
 msgid "Kurdish"
-msgstr "庫爾德語"
+msgstr "庫德語"
 
 msgid "Kurukh"
 msgstr "庫盧克語"
 
 msgid "Kutenai"
 msgstr "庫特內語"
 
@@ -730,42 +751,42 @@
 msgid "Lahnda"
 msgstr "拉亨達語"
 
 msgid "Lamba"
 msgstr "蘭巴語"
 
 msgid "Land Dayak languages"
-msgstr "達雅克語"
+msgstr "陸達雅克語系"
 
 msgid "Lao"
 msgstr "老撾語"
 
 msgid "Latin"
-msgstr "拉丁文"
+msgstr "拉丁語"
 
 msgid "Latvian"
 msgstr "拉脫維亞語"
 
 msgid "Lezghian"
 msgstr "列茲金語"
 
 msgid "Limburgan; Limburger; Limburgish"
 msgstr "林堡語"
 
 msgid "Lingala"
-msgstr "林加拉語"
+msgstr "陵加拉語"
 
 msgid "Lithuanian"
 msgstr "立陶宛語"
 
 msgid "Lojban"
 msgstr "邏輯語"
 
 msgid "Low German; Low Saxon; German, Low; Saxon, Low"
-msgstr "低地德文; 低地撒克遜語"
+msgstr "低地德語"
 
 msgid "Lower Sorbian"
 msgstr "低地文德語"
 
 msgid "Lozi"
 msgstr "洛齊語"
 
@@ -775,21 +796,21 @@
 msgid "Luba-Lulua"
 msgstr "盧巴-盧拉語"
 
 msgid "Luiseno"
 msgstr "盧伊塞諾語"
 
 msgid "Lule Sami"
-msgstr "律勒歐薩莫斯語"
+msgstr "魯爾薩米語"
 
 msgid "Lunda"
 msgstr "隆達語"
 
 msgid "Luo (Kenya and Tanzania)"
-msgstr "盧奧語 (肯尼亞和坦桑尼亞)"
+msgstr "盧奧語(肯尼亞和坦桑尼亞)"
 
 msgid "Lushai"
 msgstr "盧薩語"
 
 msgid "Luxembourgish; Letzeburgesch"
 msgstr "盧森堡語"
 
@@ -811,36 +832,36 @@
 msgid "Malagasy"
 msgstr "馬達加斯加語"
 
 msgid "Malay"
 msgstr "馬來語"
 
 msgid "Malayalam"
-msgstr "馬拉雅拉姆語"
+msgstr "馬來亞拉姆語"
 
 msgid "Maltese"
-msgstr "馬耳他語"
+msgstr "馬爾他語"
 
 msgid "Manchu"
 msgstr "滿洲語"
 
 msgid "Mandar"
 msgstr "曼達語"
 
 msgid "Mandingo"
 msgstr "曼丁哥語"
 
 msgid "Manipuri"
 msgstr "曼尼普爾語"
 
 msgid "Manobo languages"
-msgstr "馬諾博諸語言"
+msgstr "馬諾博語系"
 
 msgid "Manx"
-msgstr "馬恩島語"
+msgstr "馬恩語"
 
 msgid "Maori"
 msgstr "毛利語"
 
 msgid "Mapudungun; Mapuche"
 msgstr "阿勞坎語"
 
@@ -853,18 +874,18 @@
 msgid "Marshallese"
 msgstr "馬紹爾語"
 
 msgid "Marwari"
 msgstr "馬爾瓦利語"
 
 msgid "Masai"
-msgstr "馬薩伊語"
+msgstr "馬塞語"
 
 msgid "Mayan languages"
-msgstr "瑪雅諸語言"
+msgstr "瑪雅語系"
 
 msgid "Mende"
 msgstr "門德語"
 
 msgid "Mi'kmaq; Micmac"
 msgstr "米克馬克語"
 
@@ -877,36 +898,42 @@
 msgid "Mohawk"
 msgstr "莫霍克語"
 
 msgid "Moksha"
 msgstr "莫克沙語"
 
 msgid "Mon-Khmer languages"
-msgstr "南亞語系"
+msgstr "孟高棉語系"
 
 msgid "Mongo"
 msgstr "芒戈語"
 
 msgid "Mongolian"
 msgstr "蒙古語"
 
+msgid "Montenegrin"
+msgstr "黑山語"
+
 msgid "Mossi"
 msgstr "莫西語"
 
 msgid "Multiple languages"
-msgstr "多語種"
+msgstr "多重諸語言"
 
 msgid "Munda languages"
-msgstr "蒙達諸語言"
+msgstr "蒙達語系"
+
+msgid "N'Ko"
+msgstr "西非書面語"
 
 msgid "Nahuatl languages"
-msgstr "納瓦特爾語"
+msgstr "納瓦特爾語系"
 
 msgid "Nauru"
-msgstr "瑙魯"
+msgstr "諾魯"
 
 msgid "Navajo; Navaho"
 msgstr "納瓦霍語"
 
 msgid "Ndebele, North; North Ndebele"
 msgstr "北恩德貝勒語"
 
@@ -915,214 +942,226 @@
 
 msgid "Ndonga"
 msgstr "恩敦加語"
 
 msgid "Neapolitan"
 msgstr "拿坡里語"
 
+msgid "Nepal Bhasa; Newari"
+msgstr "尼瓦爾語"
+
 msgid "Nepali"
 msgstr "尼泊爾語"
 
 msgid "Nias"
 msgstr "尼亞斯語"
 
 msgid "Niger-Kordofanian languages"
-msgstr "尼日爾-科爾多凡諸語言"
+msgstr "尼日-科爾多凡語系"
 
 msgid "Nilo-Saharan languages"
 msgstr "尼羅-撒哈拉語系"
 
 msgid "Niuean"
 msgstr "紐埃語"
 
 msgid "No linguistic content; Not applicable"
-msgstr "無語言內容; 不適用"
+msgstr "無語言內容"
 
 msgid "Nogai"
 msgstr "諾蓋語"
 
 msgid "Norse, Old"
 msgstr "古諾爾斯語"
 
 msgid "North American Indian languages"
-msgstr "北美洲土著諸語言"
+msgstr "北美洲原住民語系"
 
 msgid "Northern Frisian"
-msgstr "北弗里西亞語"
+msgstr "北夫里斯蘭語"
 
 msgid "Northern Sami"
-msgstr "北薩莫斯語"
+msgstr "北薩米語"
 
 msgid "Norwegian"
-msgstr "書面挪威語"
+msgstr "挪威語"
 
 msgid "Norwegian Nynorsk; Nynorsk, Norwegian"
 msgstr "新挪威語"
 
 msgid "Nubian languages"
-msgstr "努比亞語諸語言"
+msgstr "努比亞語系"
 
 msgid "Nyamwezi"
 msgstr "尼揚韋齊語"
 
 msgid "Nyankole"
-msgstr "尼揚科勒語"
+msgstr "尼揚科萊語"
 
 msgid "Nyoro"
 msgstr "尼奧羅語"
 
 msgid "Nzima"
-msgstr "恩濟馬語"
+msgstr "尼茲馬語"
 
 msgid "Occitan (post 1500); Provençal"
 msgstr "奧克西坦語 (1500 之後);普羅旺斯語"
 
 msgid "Official Aramaic (700-300 BCE); Imperial Aramaic (700-300 BCE)"
 msgstr "宮廷阿拉姆語(公元前 700-300)"
 
 msgid "Ojibwa"
 msgstr "奧杰布瓦語"
 
 msgid "Oriya"
-msgstr "奧利亞語"
+msgstr "歐利亞語"
 
 msgid "Oromo"
 msgstr "奧洛莫語"
 
 msgid "Osage"
-msgstr "奧薩格語"
+msgstr "歐塞奇語"
 
 msgid "Ossetian; Ossetic"
-msgstr "奧塞梯語"
+msgstr "奧塞提語"
 
 msgid "Otomian languages"
-msgstr "奧托米諸語言"
+msgstr "奧托米語系"
 
 msgid "Pahlavi"
-msgstr "缽羅缽語"
+msgstr "巴勒維語"
 
 msgid "Palauan"
-msgstr "帕勞語"
+msgstr "帛琉語"
 
 msgid "Pali"
 msgstr "巴利語"
 
+msgid "Pampanga; Kapampangan"
+msgstr "潘帕嘉語"
+
 msgid "Pangasinan"
-msgstr "邦阿西楠語"
+msgstr "龐加辛南語"
 
 msgid "Panjabi; Punjabi"
 msgstr "旁遮普語"
 
 msgid "Papiamento"
-msgstr "帕皮阿門托語"
+msgstr "巴皮亞曼多語"
 
 msgid "Papuan languages"
 msgstr "巴布亞語系"
 
+msgid "Pedi; Sepedi; Northern Sotho"
+msgstr "北方索托語"
+
 msgid "Persian"
 msgstr "波斯語"
 
 msgid "Persian, Old (ca. 600-400 B.C.)"
-msgstr "古波斯語"
+msgstr "古波斯語 (約公元前 600-400)"
 
 msgid "Philippine languages"
 msgstr "菲律賓語系"
 
 msgid "Phoenician"
 msgstr "腓尼基語"
 
 msgid "Pohnpeian"
-msgstr "波納佩語"
+msgstr "波那貝語"
 
 msgid "Polish"
 msgstr "波蘭語"
 
 msgid "Portuguese"
-msgstr "葡萄牙文"
+msgstr "葡萄牙語"
 
 msgid "Prakrit languages"
-msgstr "普拉克里特諸語言"
+msgstr "普拉克里特語系"
 
 msgid "Provençal, Old (to 1500)"
 msgstr "古普羅旺斯語 (至 1500)"
 
 msgid "Pushto; Pashto"
 msgstr "普什圖語"
 
 msgid "Quechua"
-msgstr "凱楚亞語"
+msgstr "克丘亞語"
 
 msgid "Rajasthani"
 msgstr "拉賈斯坦語"
 
 msgid "Rapanui"
-msgstr "拉帕努伊語"
+msgstr "拉巴怒伊語"
+
+msgid "Rarotongan; Cook Islands Maori"
+msgstr "拉羅東加語／庫克群島毛利語"
 
 msgid "Reserved for local use"
 msgstr "保留作內部使用"
 
 msgid "Romance languages"
 msgstr "羅曼語系"
 
 msgid "Romanian; Moldavian; Moldovan"
 msgstr "羅馬尼亞語;莫爾達維亞語;摩爾多瓦語"
 
 msgid "Romansh"
-msgstr "利托-羅曼語"
+msgstr "里托羅曼語"
 
 msgid "Romany"
-msgstr "吉普賽語"
+msgstr "羅曼尼語"
 
 msgid "Rundi"
-msgstr "基隆迪語"
+msgstr "克倫地語"
 
 msgid "Russian"
-msgstr "俄語"
+msgstr "俄羅斯語"
 
 msgid "Salishan languages"
-msgstr "薩利什諸語言"
+msgstr "薩利希語系"
 
 msgid "Samaritan Aramaic"
-msgstr "薩馬利亞阿拉米語"
+msgstr "撒瑪麗亞阿拉姆語"
 
 msgid "Sami languages"
 msgstr "薩米語系"
 
 msgid "Samoan"
 msgstr "薩摩亞語"
 
 msgid "Sandawe"
 msgstr "桑達韋語"
 
 msgid "Sango"
 msgstr "桑戈語"
 
 msgid "Sanskrit"
-msgstr "梵文"
+msgstr "梵語"
 
 msgid "Santali"
 msgstr "桑塔利語"
 
 msgid "Sardinian"
-msgstr "撒丁語"
+msgstr "薩丁尼亞語"
 
 msgid "Sasak"
-msgstr "薩薩克語"
+msgstr "莎莎克語"
 
 msgid "Scots"
 msgstr "蘇格蘭語"
 
 msgid "Selkup"
-msgstr "塞爾庫普語"
+msgstr "瑟爾卡普語"
 
 msgid "Semitic languages"
 msgstr "閃米語系"
 
 msgid "Serbian"
-msgstr "塞爾維亞文"
+msgstr "塞爾維亞語"
 
 msgid "Serer"
 msgstr "塞雷爾語"
 
 msgid "Shan"
 msgstr "撣語"
 
@@ -1132,299 +1171,311 @@
 msgid "Sichuan Yi; Nuosu"
 msgstr "四川彝語"
 
 msgid "Sicilian"
 msgstr "西西里語"
 
 msgid "Sidamo"
-msgstr "錫達莫語"
+msgstr "希達摩語"
 
 msgid "Sign Languages"
-msgstr "手語"
+msgstr "手語諸語言"
 
 msgid "Siksika"
 msgstr "西克西卡語"
 
 msgid "Sindhi"
 msgstr "信德語"
 
 msgid "Sinhala; Sinhalese"
-msgstr "僧加羅語"
+msgstr "僧加羅語(錫蘭)"
 
 msgid "Sino-Tibetan languages"
 msgstr "漢藏語系"
 
 msgid "Siouan languages"
-msgstr "蘇語諸語言"
+msgstr "大蘇丹語系"
 
 msgid "Skolt Sami"
-msgstr "斯高特薩莫斯語"
+msgstr "斯克特薩米語"
 
 msgid "Slave (Athapascan)"
-msgstr "史拉維語"
+msgstr "史拉維語 (阿薩帕斯坎語)"
 
 msgid "Slavic languages"
 msgstr "斯拉夫語系"
 
 msgid "Slovak"
 msgstr "斯洛伐克語"
 
 msgid "Slovenian"
-msgstr "斯洛文尼亞語"
+msgstr "斯洛維尼亞語"
 
 msgid "Sogdian"
 msgstr "粟特語"
 
 msgid "Somali"
-msgstr "索馬里語"
+msgstr "索馬利語"
 
 msgid "Songhai languages"
-msgstr "桑海語"
+msgstr "桑海語系"
 
 msgid "Soninke"
 msgstr "索寧克語"
 
 msgid "Sorbian languages"
-msgstr "索布諸語言"
+msgstr "文德語系"
 
 msgid "Sotho, Southern"
 msgstr "南索托語"
 
+msgid "South American Indian (Other)"
+msgstr "南美原住民語言（其他）"
+
 msgid "Southern Altai"
 msgstr "南阿爾泰語"
 
 msgid "Southern Sami"
-msgstr "南薩莫斯語"
+msgstr "南薩米語"
 
 msgid "Spanish; Castilian"
-msgstr "西班牙文"
+msgstr "西班牙語"
+
+msgid "Sranan Tongo"
+msgstr "蘇利南語"
+
+msgid "Standard Moroccan Tamazight"
+msgstr "標準摩洛哥塔馬塞特語"
 
 msgid "Sukuma"
 msgstr "蘇庫馬語"
 
 msgid "Sumerian"
-msgstr "蘇美爾語"
+msgstr "蘇美語"
 
 msgid "Sundanese"
-msgstr "巽他語"
+msgstr "巽丹語"
 
 msgid "Susu"
 msgstr "蘇蘇語"
 
 msgid "Swahili"
-msgstr "斯瓦希里語"
+msgstr "史瓦西里語"
 
 msgid "Swati"
-msgstr "斯瓦特語"
+msgstr "斯瓦齊語"
 
 msgid "Swedish"
 msgstr "瑞典語"
 
 msgid "Swiss German; Alemannic; Alsatian"
-msgstr "瑞士德文; 阿勒曼尼語; 亞爾薩斯語"
+msgstr "瑞士德語"
 
 msgid "Syriac"
-msgstr "敍利亞文"
+msgstr "敘利亞語"
 
 msgid "Tagalog"
-msgstr "塔加洛語"
+msgstr "塔加拉語"
 
 msgid "Tahitian"
 msgstr "大溪地語"
 
 msgid "Tai languages"
 msgstr "壯侗語系"
 
 msgid "Tajik"
 msgstr "塔吉克語"
 
 msgid "Tamashek"
-msgstr "塔馬奇克語"
+msgstr "泰瑪歇克語"
 
 msgid "Tamil"
-msgstr "泰米爾語"
+msgstr "坦米爾語"
 
 msgid "Tatar"
-msgstr "塔塔爾語"
+msgstr "韃靼語"
 
 msgid "Telugu"
-msgstr "泰盧固語"
+msgstr "特拉古語"
 
 msgid "Tereno"
-msgstr "特列納語"
+msgstr "特崙諾語"
 
 msgid "Tetum"
 msgstr "德頓語"
 
 msgid "Thai"
-msgstr "泰文"
+msgstr "泰語"
 
 msgid "Tibetan"
 msgstr "藏語"
 
 msgid "Tigre"
-msgstr "提格雷語"
+msgstr "泰格瑞語"
 
 msgid "Tigrinya"
-msgstr "提格里尼亞語"
+msgstr "提格利尼亞語"
 
 msgid "Timne"
-msgstr "滕內語"
+msgstr "堤姆奈語"
 
 msgid "Tiv"
-msgstr "蒂夫語"
+msgstr "提夫語"
 
 msgid "Tlingit"
 msgstr "特林吉特語"
 
 msgid "Tok Pisin"
-msgstr "托克皮辛語"
+msgstr "托比辛語"
 
 msgid "Tokelau"
-msgstr "托克勞羣島"
+msgstr "托克勞"
 
 msgid "Tonga (Nyasa)"
-msgstr "湯加語 (尼亞薩)"
+msgstr "東加語(尼亞沙)"
 
 msgid "Tonga (Tonga Islands)"
-msgstr "湯加語 (湯加島)"
+msgstr "東加語(東加群島)"
 
 msgid "Tsimshian"
 msgstr "欽西安語"
 
 msgid "Tsonga"
-msgstr "宗加語"
+msgstr "宋加語"
 
 msgid "Tswana"
-msgstr "塞茨瓦納語"
+msgstr "茨瓦納語"
 
 msgid "Tumbuka"
-msgstr "奇圖姆布卡語"
+msgstr "通布卡語"
 
 msgid "Tupi languages"
-msgstr "圖皮語諸語言"
+msgstr "圖皮語系"
 
 msgid "Turkish"
 msgstr "土耳其語"
 
 msgid "Turkish, Ottoman (1500-1928)"
-msgstr "古奧斯曼土耳其語"
+msgstr "鄂圖曼土耳其語 (1500-1928)"
 
 msgid "Turkmen"
 msgstr "土庫曼語"
 
 msgid "Tuvalu"
-msgstr "圖瓦盧語"
+msgstr "吐瓦魯"
 
 msgid "Tuvinian"
-msgstr "圖瓦語"
+msgstr "圖瓦尼安語"
 
 msgid "Twi"
-msgstr "特威語"
+msgstr "奇族語"
 
 msgid "Udmurt"
 msgstr "烏德穆爾特語"
 
 msgid "Ugaritic"
-msgstr "烏加里特語"
+msgstr "烏加里特楔形文字"
 
 msgid "Uighur; Uyghur"
 msgstr "維吾爾語"
 
 msgid "Ukrainian"
 msgstr "烏克蘭語"
 
 msgid "Umbundu"
-msgstr "翁本杜語"
+msgstr "姆本杜語"
 
 msgid "Uncoded languages"
 msgstr "未定碼諸語言"
 
 msgid "Undetermined"
-msgstr "未確定語種"
+msgstr "未確定"
 
 msgid "Upper Sorbian"
-msgstr "上索布語"
+msgstr "高地文德語"
 
 msgid "Urdu"
 msgstr "烏爾都語"
 
 msgid "Uzbek"
 msgstr "烏茲別克語"
 
 msgid "Vai"
 msgstr "瓦伊語"
 
 msgid "Venda"
-msgstr "文達語"
+msgstr "溫達語"
 
 msgid "Vietnamese"
-msgstr "越南文"
+msgstr "越南語"
 
 msgid "Volapük"
 msgstr "沃拉普克語"
 
 msgid "Votic"
 msgstr "沃提克語"
 
 msgid "Wakashan languages"
-msgstr "瓦卡什諸語言"
+msgstr "瓦卡時語系"
+
+msgid "Walamo"
+msgstr "瓦拉莫語"
 
 msgid "Walloon"
-msgstr "沃倫語"
+msgstr "瓦隆語"
 
 msgid "Waray"
-msgstr "瓦賴語"
+msgstr "瓦瑞語"
 
 msgid "Washo"
-msgstr "瓦肖語"
+msgstr "瓦紹語"
 
 msgid "Welsh"
 msgstr "威爾斯語"
 
 msgid "Western Frisian"
-msgstr "弗里西亞語"
+msgstr "西夫里斯蘭語"
 
 msgid "Wolof"
-msgstr "沃洛夫語"
+msgstr "渥魯夫語"
 
 msgid "Xhosa"
 msgstr "科薩語"
 
 msgid "Yakut"
 msgstr "雅庫特語"
 
 msgid "Yao"
-msgstr "瑤文"
+msgstr "瑤語"
 
 msgid "Yapese"
-msgstr "雅浦語"
+msgstr "雅蒲語"
 
 msgid "Yiddish"
-msgstr "依地語"
+msgstr "意第緒語"
 
 msgid "Yoruba"
 msgstr "約魯巴語"
 
 msgid "Yupik languages"
-msgstr "尤皮克諸語言"
+msgstr "尤皮克語系"
 
 msgid "Zande languages"
-msgstr "贊德語"
+msgstr "贊德語系"
 
 msgid "Zapotec"
 msgstr "薩波特克語"
 
 msgid "Zaza; Dimili; Dimli; Kirdki; Kirmanjki; Zazaki"
 msgstr "扎扎其語"
 
 msgid "Zenaga"
-msgstr "哲納加語"
+msgstr "澤納加語"
 
 msgid "Zhuang; Chuang"
-msgstr "壯文"
+msgstr "壯語"
 
 msgid "Zulu"
 msgstr "祖魯語"
 
 msgid "Zuni"
 msgstr "祖尼語"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_15924\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-02-22 02:55+0000\n"
-"Last-Translator: Jack Liu <ywp033319@gmail.com>\n"
+"PO-Revision-Date: 2023-04-10 05:19+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
 "Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
 "iso-codes/iso-15924/zh_Hant/>\n"
 "Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "Adlam"
 msgstr "阿德拉姆語"
 
 msgid "Afaka"
 msgstr "阿法卡文字"
 
@@ -119,15 +119,15 @@
 msgid "Cyrillic"
 msgstr "西里爾字母"
 
 msgid "Cyrillic (Old Church Slavonic variant)"
 msgstr "西里爾文 (古教會斯拉夫文的變體)"
 
 msgid "Deseret (Mormon)"
-msgstr "德瑟雷特文"
+msgstr "摩爾門教德撒律文"
 
 msgid "Devanagari (Nagari)"
 msgstr "梵文字母天城體 (城文)"
 
 msgid "Duployan shorthand, Duployan stenography"
 msgstr "杜洛耶速記"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_3166-1\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-02-22 02:55+0000\n"
-"Last-Translator: Jack Liu <ywp033319@gmail.com>\n"
+"PO-Revision-Date: 2023-04-09 22:52+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
 "Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
 "iso-codes/iso-3166-1/zh_Hant/>\n"
 "Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "Afghanistan"
 msgstr "阿富汗"
 
 msgid "Albania"
 msgstr "阿爾巴尼亞"
 
@@ -50,15 +50,15 @@
 msgid "Argentine Republic"
 msgstr "阿根廷共和國"
 
 msgid "Armenia"
 msgstr "亞美尼亞"
 
 msgid "Aruba"
-msgstr "阿魯巴"
+msgstr "阿路巴"
 
 msgid "Australia"
 msgstr "澳大利亞"
 
 msgid "Austria"
 msgstr "奧地利"
 
@@ -409,14 +409,17 @@
 
 msgid "India"
 msgstr "印度"
 
 msgid "Indonesia"
 msgstr "印度尼西亞"
 
+msgid "Iran"
+msgstr "伊朗"
+
 msgid "Iran, Islamic Republic of"
 msgstr "伊朗伊斯蘭共和國"
 
 msgid "Iraq"
 msgstr "伊拉克"
 
 msgid "Ireland"
@@ -526,14 +529,17 @@
 
 msgid "Kyrgyzstan"
 msgstr "吉爾吉斯"
 
 msgid "Lao People's Democratic Republic"
 msgstr "寮人民民主共和國"
 
+msgid "Laos"
+msgstr "寮國"
+
 msgid "Latvia"
 msgstr "拉脫維亞"
 
 msgid "Lebanese Republic"
 msgstr "黎巴嫩共和國"
 
 msgid "Lebanon"
@@ -964,14 +970,17 @@
 
 msgid "Republic of Trinidad and Tobago"
 msgstr "千里達及托巴哥共和國"
 
 msgid "Republic of Tunisia"
 msgstr "突尼西亞共和國"
 
+msgid "Republic of Türkiye"
+msgstr "土耳其共和國"
+
 msgid "Republic of Uganda"
 msgstr "烏干達共和國"
 
 msgid "Republic of Uzbekistan"
 msgstr "烏茲別克共和國"
 
 msgid "Republic of Vanuatu"
@@ -1132,14 +1141,17 @@
 
 msgid "Swiss Confederation"
 msgstr "瑞士邦聯"
 
 msgid "Switzerland"
 msgstr "瑞士"
 
+msgid "Syria"
+msgstr "敘利亞"
+
 msgid "Syrian Arab Republic"
 msgstr "敘利亞阿拉伯共和國"
 
 msgid "Taiwan"
 msgstr "臺灣"
 
 msgid "Taiwan, Province of China"
@@ -1183,14 +1195,17 @@
 
 msgid "Turks and Caicos Islands"
 msgstr "土克凱可群島"
 
 msgid "Tuvalu"
 msgstr "吐瓦魯"
 
+msgid "Türkiye"
+msgstr "土耳其"
+
 msgid "Uganda"
 msgstr "烏干達"
 
 msgid "Ukraine"
 msgstr "烏克蘭"
 
 msgid "Union of the Comoros"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_4217\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2019-10-18 14:54+0000\n"
-"Last-Translator: Walter Cheuk <wwycheuk@gmail.com>\n"
+"PO-Revision-Date: 2023-04-10 05:19+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
 "Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
 "iso-codes/iso-4217/zh_Hant/>\n"
 "Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 3.9.1-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "ADB Unit of Account"
 msgstr "亞行帳戶單位"
 
 msgid "Afghani"
 msgstr "阿富汗尼"
 
@@ -31,14 +31,17 @@
 
 msgid "Aruban Florin"
 msgstr "阿魯巴弗羅林"
 
 msgid "Australian Dollar"
 msgstr "澳大利亞元"
 
+msgid "Azerbaijan Manat"
+msgstr "亞塞拜然馬納特"
+
 msgid "Bahamian Dollar"
 msgstr "巴哈馬元"
 
 msgid "Bahraini Dinar"
 msgstr "巴林戴納"
 
 msgid "Baht"
@@ -58,14 +61,17 @@
 
 msgid "Bermudian Dollar"
 msgstr "百慕達幣"
 
 msgid "Boliviano"
 msgstr "玻利維亞諾"
 
+msgid "Bolívar Soberano"
+msgstr "主權玻利瓦"
+
 msgid "Bond Markets Unit European Composite Unit (EURCO)"
 msgstr "歐洲債券市場混合單位 (EURCO)"
 
 msgid "Bond Markets Unit European Monetary Unit (E.M.U.-6)"
 msgstr "歐洲債券市場混合單位 (E.M.U.-6)"
 
 msgid "Bond Markets Unit European Unit of Account 17 (E.U.A.-17)"
@@ -109,19 +115,22 @@
 
 msgid "Codes specifically reserved for testing purposes"
 msgstr "專門為測試目的保留代碼"
 
 msgid "Colombian Peso"
 msgstr "哥倫比亞披索"
 
+msgid "Comorian Franc"
+msgstr "葛摩法郎"
+
 msgid "Congolese Franc"
 msgstr "剛果法郎"
 
 msgid "Convertible Mark"
-msgstr "可兌換標記"
+msgstr "波黑可兌換馬克"
 
 msgid "Cordoba Oro"
 msgstr "尼加拉瓜科多巴"
 
 msgid "Costa Rican Colon"
 msgstr "哥斯大黎加科郎"
 
@@ -146,15 +155,15 @@
 msgid "Dobra"
 msgstr "聖多美及普林西比多布拉"
 
 msgid "Dominican Peso"
 msgstr "多明尼加披索"
 
 msgid "Dong"
-msgstr "侗語"
+msgstr "盾"
 
 msgid "East Caribbean Dollar"
 msgstr "東加勒比元"
 
 msgid "Egyptian Pound"
 msgstr "埃及鎊"
 
@@ -187,14 +196,17 @@
 
 msgid "Gourde"
 msgstr "海地古德"
 
 msgid "Guarani"
 msgstr "巴拉圭瓜拉尼"
 
+msgid "Guinean Franc"
+msgstr "幾內亞法郎"
+
 msgid "Guyana Dollar"
 msgstr "蓋亞那元"
 
 msgid "Hong Kong Dollar"
 msgstr "港元"
 
 msgid "Hryvnia"
@@ -283,14 +295,17 @@
 
 msgid "Moroccan Dirham"
 msgstr "摩洛哥迪拉姆"
 
 msgid "Mozambique Metical"
 msgstr "莫三比克梅蒂卡爾"
 
+msgid "Mvdol"
+msgstr "MVDOL"
+
 msgid "Naira"
 msgstr "奈及利亞奈拉"
 
 msgid "Nakfa"
 msgstr "厄立特里亞納克法"
 
 msgid "Namibia Dollar"
@@ -475,23 +490,35 @@
 
 msgid "UAE Dirham"
 msgstr "阿拉伯聯合大公國迪拉姆"
 
 msgid "US Dollar"
 msgstr "美元"
 
+msgid "US Dollar (Next day)"
+msgstr "美元（次日）"
+
 msgid "Uganda Shilling"
 msgstr "烏干達先令"
 
+msgid "Unidad de Fomento"
+msgstr "UF金融單位"
+
 msgid "Uzbekistan Sum"
 msgstr "烏茲別克頌"
 
 msgid "Vatu"
 msgstr "萬那杜瓦土"
 
+msgid "WIR Euro"
+msgstr "WIR 歐元"
+
+msgid "WIR Franc"
+msgstr "WIR 法郎"
+
 msgid "Won"
 msgstr "南韓韓圜"
 
 msgid "Yemeni Rial"
 msgstr "葉門里亞爾"
 
 msgid "Yen"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,79 +1,79 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: iso_639-2\n"
 "Report-Msgid-Bugs-To: https://salsa.debian.org/iso-codes-team/iso-codes/"
 "issues\n"
-"PO-Revision-Date: 2022-02-22 02:55+0000\n"
-"Last-Translator: Jack Liu <ywp033319@gmail.com>\n"
-"Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
-"iso-codes/iso-639-2/zh_Hant/>\n"
-"Language: zh_TW\n"
+"PO-Revision-Date: 2023-04-09 22:52+0000\n"
+"Last-Translator: Abel Cheung <abelcheung@gmail.com>\n"
+"Language-Team: Chinese (Traditional, Hong Kong) <https://hosted.weblate.org/"
+"projects/iso-codes/iso-639-2/zh_Hant_HK/>\n"
+"Language: zh_HK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 msgid "Abkhazian"
-msgstr "亞布卡薩語"
+msgstr "阿布哈茲語"
 
 msgid "Achinese"
 msgstr "亞齊語"
 
 msgid "Acoli"
 msgstr "阿喬利語"
 
 msgid "Adangme"
 msgstr "阿當梅語"
 
 msgid "Adyghe; Adygei"
-msgstr "阿迪何語"
+msgstr "阿迪格語"
 
 msgid "Afar"
 msgstr "阿法爾語"
 
 msgid "Afrihili"
 msgstr "阿弗里希利語"
 
 msgid "Afrikaans"
-msgstr "南非荷蘭文"
+msgstr "南非荷蘭語"
 
 msgid "Afro-Asiatic languages"
 msgstr "亞非語系"
 
 msgid "Ainu"
 msgstr "阿依努語"
 
 msgid "Akan"
-msgstr "迦納語"
+msgstr "阿坎語"
 
 msgid "Akkadian"
 msgstr "阿卡德語"
 
 msgid "Albanian"
 msgstr "阿爾巴尼亞語"
 
 msgid "Aleut"
 msgstr "阿留申語"
 
 msgid "Algonquian languages"
-msgstr "阿爾岡基語系"
+msgstr "阿爾岡昆諸語言"
 
 msgid "Altaic languages"
 msgstr "阿爾泰語系"
 
 msgid "Amharic"
 msgstr "阿姆哈拉語"
 
 msgid "Angika"
 msgstr "昂加語"
 
 msgid "Apache languages"
-msgstr "阿帕契語系"
+msgstr "阿帕切諸語言"
 
 msgid "Arabic"
 msgstr "阿拉伯語"
 
 msgid "Aragonese"
 msgstr "阿拉貢語"
 
@@ -86,84 +86,84 @@
 msgid "Armenian"
 msgstr "亞美尼亞語"
 
 msgid "Aromanian; Arumanian; Macedo-Romanian"
 msgstr "阿羅馬尼亞語"
 
 msgid "Artificial languages"
-msgstr "人造語系"
+msgstr "人工語言"
 
 msgid "Assamese"
 msgstr "阿薩姆語"
 
 msgid "Asturian; Bable; Leonese; Asturleonese"
 msgstr "阿斯圖里亞斯語"
 
 msgid "Athapascan languages"
-msgstr "阿薩帕斯坎語系"
+msgstr "阿薩帕斯坎諸語言"
 
 msgid "Australian languages"
-msgstr "澳大利亞語系"
+msgstr "澳大利亞諸語言"
 
 msgid "Austronesian languages"
 msgstr "南島語系"
 
 msgid "Avaric"
 msgstr "阿瓦爾語"
 
 msgid "Avestan"
-msgstr "阿維斯語"
+msgstr "阿維斯陀語"
 
 msgid "Awadhi"
 msgstr "阿瓦德語"
 
 msgid "Aymara"
-msgstr "亞摩拉語"
+msgstr "艾馬拉語"
 
 msgid "Azerbaijani"
-msgstr "亞塞拜然語"
+msgstr "阿塞拜疆語"
 
 msgid "Balinese"
 msgstr "峇里語"
 
 msgid "Baltic languages"
 msgstr "波羅的語系"
 
 msgid "Baluchi"
 msgstr "俾路支語"
 
 msgid "Bambara"
 msgstr "班巴拉語"
 
 msgid "Bamileke languages"
-msgstr "巴米雷克語系"
+msgstr "巴米累克諸語言"
 
 msgid "Banda languages"
-msgstr "班達語系"
+msgstr "班達語"
 
 msgid "Bangla"
-msgstr "孟加拉語"
+msgstr "孟加拉文"
 
 msgid "Bantu (Other)"
 msgstr "班圖語 (其他)"
 
 msgid "Basa"
 msgstr "巴薩語"
 
 msgid "Bashkir"
-msgstr "巴什喀爾語"
+msgstr "巴什基爾語"
 
 msgid "Basque"
 msgstr "巴斯克語"
 
 msgid "Batak languages"
-msgstr "巴塔克語系"
+msgstr "巴塔克語"
 
 msgid "Beja; Bedawiyet"
-msgstr "貝札語"
+msgstr "貝扎文"
 
 msgid "Belarusian"
 msgstr "白俄羅斯語"
 
 msgid "Bemba"
 msgstr "本巴語"
 
@@ -179,39 +179,39 @@
 msgid "Bihari languages"
 msgstr "比哈爾語系"
 
 msgid "Bikol"
 msgstr "比科爾語"
 
 msgid "Bini; Edo"
-msgstr "艾鬥語"
+msgstr "比尼語"
 
 msgid "Bislama"
-msgstr "比斯拉馬語"
+msgstr "比斯拉瑪語"
 
 msgid "Blin; Bilin"
 msgstr "比林語"
 
 msgid "Blissymbols; Blissymbolics; Bliss"
 msgstr "布利斯符號"
 
 msgid "Bokmål, Norwegian; Norwegian Bokmål"
 msgstr "書面挪威語"
 
 msgid "Bosnian"
-msgstr "波士尼亞語"
+msgstr "波斯尼亞語"
 
 msgid "Braj"
 msgstr "布拉吉語"
 
 msgid "Breton"
-msgstr "布里敦語"
+msgstr "布里多尼語"
 
 msgid "Buginese"
-msgstr "布吉斯語"
+msgstr "布吉語"
 
 msgid "Bulgarian"
 msgstr "保加利亞語"
 
 msgid "Buriat"
 msgstr "布里亞特語"
 
@@ -230,51 +230,51 @@
 msgid "Cebuano"
 msgstr "宿霧語"
 
 msgid "Celtic languages"
 msgstr "凱爾特語系"
 
 msgid "Central American Indian languages"
-msgstr "中美洲原住民語系"
+msgstr "中美洲印第安諸語言"
 
 msgid "Central Khmer"
-msgstr "中央高棉語"
+msgstr "高棉語"
 
 msgid "Chagatai"
-msgstr "察合臺語"
+msgstr "查加台語"
 
 msgid "Chamic languages"
-msgstr "查米克語系"
+msgstr "占語諸語言"
 
 msgid "Chamorro"
 msgstr "查莫羅語"
 
 msgid "Chechen"
 msgstr "車臣語"
 
 msgid "Cherokee"
-msgstr "卻洛奇語"
+msgstr "切羅基語"
 
 msgid "Cheyenne"
 msgstr "夏延語"
 
 msgid "Chibcha"
 msgstr "奇布查語"
 
 msgid "Chichewa; Chewa; Nyanja"
-msgstr "契切瓦語"
+msgstr "尼揚賈語"
 
 msgid "Chinese"
 msgstr "中文"
 
 msgid "Chinook jargon"
 msgstr "奇努克混合語"
 
 msgid "Chipewyan; Dene Suline"
-msgstr "奇佩維安語"
+msgstr "奇佩維安文"
 
 msgid "Choctaw"
 msgstr "喬克托語"
 
 msgid ""
 "Church Slavic; Old Slavonic; Church Slavonic; Old Bulgarian; Old Church "
 "Slavonic"
@@ -283,18 +283,18 @@
 msgid "Chuukese"
 msgstr "丘克語"
 
 msgid "Chuvash"
 msgstr "楚瓦什語"
 
 msgid "Classical Newari; Old Newari; Classical Nepal Bhasa"
-msgstr "古尼瓦爾語"
+msgstr "尼瓦爾語"
 
 msgid "Classical Syriac"
-msgstr "古敘利亞語"
+msgstr "古敍利亞文"
 
 msgid "Coptic"
 msgstr "科普特語"
 
 msgid "Cornish"
 msgstr "康沃爾語"
 
@@ -304,30 +304,30 @@
 msgid "Cree"
 msgstr "克里語"
 
 msgid "Creek"
 msgstr "克里克語"
 
 msgid "Creoles and pidgins"
-msgstr "克里奧爾混合語系"
+msgstr "混合語"
 
 msgid "Creoles and pidgins, English based"
 msgstr "英語克里奧爾混合語"
 
 msgid "Creoles and pidgins, French-based"
 msgstr "法語克里奧爾混合語"
 
 msgid "Creoles and pidgins, Portuguese-based"
-msgstr "葡萄牙語克里奧爾混合語系"
+msgstr "葡萄牙語克里奧爾混合語"
 
 msgid "Crimean Tatar; Crimean Turkish"
 msgstr "克里米亞韃靼語"
 
 msgid "Croatian"
-msgstr "克羅埃西亞語"
+msgstr "克羅地亞語"
 
 msgid "Cushitic languages"
 msgstr "庫希特語系"
 
 msgid "Czech"
 msgstr "捷克語"
 
@@ -337,48 +337,48 @@
 msgid "Danish"
 msgstr "丹麥語"
 
 msgid "Dargwa"
 msgstr "達爾格瓦語"
 
 msgid "Delaware"
-msgstr "德拉瓦語"
+msgstr "特拉華語"
 
 msgid "Dinka"
 msgstr "丁卡語"
 
 msgid "Divehi; Dhivehi; Maldivian"
-msgstr "迪維西語"
+msgstr "迪維希語"
 
 msgid "Dogri"
 msgstr "多格拉語"
 
 msgid "Dogrib"
 msgstr "多格里布語"
 
 msgid "Dravidian languages"
 msgstr "達羅毗荼語系"
 
 msgid "Duala"
 msgstr "杜亞拉語"
 
 msgid "Dutch, Middle (ca. 1050-1350)"
-msgstr "中古荷蘭語 (約 1050-1350)"
+msgstr "中古荷蘭語"
 
 msgid "Dutch; Flemish"
 msgstr "荷蘭語"
 
 msgid "Dyula"
 msgstr "迪尤拉語"
 
 msgid "Dzongkha"
-msgstr "宗卡語(不丹)"
+msgstr "不丹語"
 
 msgid "Eastern Frisian"
-msgstr "東夫里斯蘭語"
+msgstr "東弗里西亞語"
 
 msgid "Efik"
 msgstr "埃菲克語"
 
 msgid "Egyptian (Ancient)"
 msgstr "古埃及語"
 
@@ -388,18 +388,18 @@
 msgid "Elamite"
 msgstr "埃蘭語"
 
 msgid "English"
 msgstr "英文"
 
 msgid "English, Middle (1100-1500)"
-msgstr "中古英語 (1100-1500)"
+msgstr "中古英文"
 
 msgid "English, Old (ca. 450-1100)"
-msgstr "古英語 (約 450-1100)"
+msgstr "古英語"
 
 msgid "Erzya"
 msgstr "厄爾茲亞語"
 
 msgid "Esperanto"
 msgstr "世界語"
 
@@ -415,123 +415,123 @@
 msgid "Fang"
 msgstr "芳語"
 
 msgid "Fanti"
 msgstr "芳蒂語"
 
 msgid "Faroese"
-msgstr "法羅群島語"
+msgstr "法羅語"
 
 msgid "Fijian"
 msgstr "斐濟語"
 
 msgid "Filipino; Pilipino"
 msgstr "菲律賓語"
 
 msgid "Finnish"
 msgstr "芬蘭語"
 
 msgid "Finno-Ugrian languages"
-msgstr "芬蘭-烏戈爾語系"
+msgstr "芬蘭－烏戈爾語系"
 
 msgid "Fon"
 msgstr "豐語"
 
 msgid "French"
-msgstr "法語"
+msgstr "法文"
 
 msgid "French, Middle (ca. 1400-1600)"
-msgstr "中古法語 (約 1400-1600)"
+msgstr "中古法文"
 
 msgid "French, Old (842-ca. 1400)"
-msgstr "古法語 (842-約 1400)"
+msgstr "古法文"
 
 msgid "Friulian"
 msgstr "弗留利語"
 
 msgid "Fulah"
 msgstr "富拉語"
 
 msgid "Ga"
-msgstr "格語"
+msgstr "加語"
 
 msgid "Gaelic; Scottish Gaelic"
 msgstr "蓋爾語"
 
 msgid "Galibi Carib"
-msgstr "加勒比語"
+msgstr "加勒比諸語言"
 
 msgid "Galician"
-msgstr "加里斯亞語"
+msgstr "加利西亞語"
 
 msgid "Ganda"
 msgstr "干達語"
 
 msgid "Gayo"
 msgstr "卡約語"
 
 msgid "Gbaya"
 msgstr "巴亞語"
 
 msgid "Geez"
 msgstr "吉茲語"
 
 msgid "Georgian"
-msgstr "喬治亞語"
+msgstr "格魯吉亞語"
 
 msgid "German"
-msgstr "德語"
+msgstr "德文"
 
 msgid "German, Middle High (ca. 1050-1500)"
-msgstr "中古高地德語 (約 1050-1500)"
+msgstr "中古高地德文"
 
 msgid "German, Old High (ca. 750-1050)"
-msgstr "古高地德語 (約 750-1050)"
+msgstr "古高地德文"
 
 msgid "Germanic languages"
 msgstr "日耳曼語系"
 
 msgid "Gilbertese"
 msgstr "吉伯特語"
 
 msgid "Gondi"
 msgstr "貢德語"
 
 msgid "Gorontalo"
 msgstr "哥倫打洛語"
 
 msgid "Gothic"
-msgstr "哥德語"
+msgstr "哥特語"
 
 msgid "Grebo"
 msgstr "格列博語"
 
 msgid "Greek, Ancient (to 1453)"
-msgstr "古希臘語 (到 1453)"
+msgstr "古希臘語"
 
 msgid "Greek, Modern (1453-)"
-msgstr "現代希臘語 (1453-)"
+msgstr "現代希臘語"
 
 msgid "Guarani"
 msgstr "巴拉圭瓜拉尼"
 
 msgid "Gujarati"
 msgstr "古吉拉特語"
 
 msgid "Gwich'in"
 msgstr "庫臣語"
 
 msgid "Haida"
 msgstr "海達語"
 
 msgid "Haitian; Haitian Creole"
-msgstr "克里奧爾語(海地)"
+msgstr "海地克里奧爾語"
 
 msgid "Hausa"
-msgstr "豪撒語(蘇丹)"
+msgstr "豪薩語"
 
 msgid "Hawaiian"
 msgstr "夏威夷語"
 
 msgid "Hebrew"
 msgstr "希伯來語"
 
@@ -541,24 +541,24 @@
 msgid "Hiligaynon"
 msgstr "希利蓋農語"
 
 msgid "Himachali languages; Western Pahari languages"
 msgstr "喜馬偕爾諸語言；西帕哈爾諸語言"
 
 msgid "Hindi"
-msgstr "印地語(北印度)"
+msgstr "印地語"
 
 msgid "Hiri Motu"
 msgstr "希里莫圖語"
 
 msgid "Hittite"
 msgstr "赫梯語"
 
 msgid "Hmong; Mong"
-msgstr "苗語"
+msgstr "苗文"
 
 msgid "Hungarian"
 msgstr "匈牙利語"
 
 msgid "Hupa"
 msgstr "胡帕語"
 
@@ -568,24 +568,24 @@
 msgid "Icelandic"
 msgstr "冰島語"
 
 msgid "Ido"
 msgstr "伊多語"
 
 msgid "Igbo"
-msgstr "伊布語"
+msgstr "伊博語"
 
 msgid "Ijo languages"
-msgstr "伊喬語系"
+msgstr "伊喬語"
 
 msgid "Iloko"
 msgstr "伊洛卡諾語"
 
 msgid "Inari Sami"
-msgstr "伊納里薩米語"
+msgstr "伊納里薩莫斯語"
 
 msgid "Indic languages"
 msgstr "印度語系"
 
 msgid "Indo-European languages"
 msgstr "印歐語系"
 
@@ -598,39 +598,39 @@
 msgid "Interlingua (International Auxiliary Language Association)"
 msgstr "拉丁國際語"
 
 msgid "Interlingue; Occidental"
 msgstr "國際語"
 
 msgid "Inuktitut"
-msgstr "伊努特語"
+msgstr "伊努伊特語"
 
 msgid "Inupiaq"
 msgstr "依努庇克語"
 
 msgid "Iranian languages"
 msgstr "伊朗語系"
 
 msgid "Irish"
 msgstr "愛爾蘭語"
 
 msgid "Irish, Middle (900-1200)"
-msgstr "中古愛爾蘭語 (900-1200)"
+msgstr "中古愛爾蘭語"
 
 msgid "Irish, Old (to 900)"
-msgstr "古愛爾蘭語 (至 900)"
+msgstr "古愛爾蘭語"
 
 msgid "Iroquoian languages"
-msgstr "易洛魁語系"
+msgstr "易洛魁語"
 
 msgid "Italian"
-msgstr "義大利語"
+msgstr "意大利語"
 
 msgid "Japanese"
-msgstr "日語"
+msgstr "日文"
 
 msgid "Javanese"
 msgstr "爪哇語"
 
 msgid "Judeo-Arabic"
 msgstr "猶太-阿拉伯語"
 
@@ -649,36 +649,36 @@
 msgid "Kalaallisut; Greenlandic"
 msgstr "格陵蘭語"
 
 msgid "Kalmyk; Oirat"
 msgstr "卡爾梅克語"
 
 msgid "Kamba"
-msgstr "卡姆帕語"
+msgstr "坎巴語"
 
 msgid "Kannada"
 msgstr "卡納達語"
 
 msgid "Kanuri"
 msgstr "卡努里語"
 
 msgid "Kara-Kalpak"
-msgstr "卡拉-卡爾帕克語"
+msgstr "卡拉卡爾帕克語"
 
 msgid "Karachay-Balkar"
 msgstr "卡拉恰伊-巴爾卡爾語"
 
 msgid "Karelian"
 msgstr "卡累利阿語"
 
 msgid "Karen languages"
-msgstr "克倫語系"
+msgstr "克倫語"
 
 msgid "Kashmiri"
-msgstr "喀什米爾語"
+msgstr "克什米爾語"
 
 msgid "Kashubian"
 msgstr "卡舒比語"
 
 msgid "Kawi"
 msgstr "卡威語"
 
@@ -697,51 +697,51 @@
 msgid "Kikuyu; Gikuyu"
 msgstr "基庫尤語"
 
 msgid "Kimbundu"
 msgstr "金本杜語"
 
 msgid "Kinyarwanda"
-msgstr "盧安達語"
+msgstr "基尼阿萬達語"
 
 msgid "Kirghiz; Kyrgyz"
 msgstr "吉爾吉斯語"
 
 msgid "Klingon; tlhIngan-Hol"
 msgstr "克林貢語"
 
 msgid "Komi"
 msgstr "科米語"
 
 msgid "Kongo"
 msgstr "剛果語"
 
 msgid "Konkani"
-msgstr "貢根語"
+msgstr "孔卡尼語"
 
 msgid "Korean"
-msgstr "韓語"
+msgstr "韓文"
 
 msgid "Kosraean"
 msgstr "科斯拉伊語"
 
 msgid "Kpelle"
 msgstr "克佩勒語"
 
 msgid "Kru languages"
-msgstr "克魯語系"
+msgstr "克魯語"
 
 msgid "Kuanyama; Kwanyama"
 msgstr "寬亞瑪語"
 
 msgid "Kumyk"
 msgstr "庫梅克語"
 
 msgid "Kurdish"
-msgstr "庫德語"
+msgstr "庫爾德語"
 
 msgid "Kurukh"
 msgstr "庫盧克語"
 
 msgid "Kutenai"
 msgstr "庫特內語"
 
@@ -751,66 +751,66 @@
 msgid "Lahnda"
 msgstr "拉亨達語"
 
 msgid "Lamba"
 msgstr "蘭巴語"
 
 msgid "Land Dayak languages"
-msgstr "陸達雅克語系"
+msgstr "達雅克語"
 
 msgid "Lao"
 msgstr "老撾語"
 
 msgid "Latin"
-msgstr "拉丁語"
+msgstr "拉丁文"
 
 msgid "Latvian"
 msgstr "拉脫維亞語"
 
 msgid "Lezghian"
 msgstr "列茲金語"
 
 msgid "Limburgan; Limburger; Limburgish"
 msgstr "林堡語"
 
 msgid "Lingala"
-msgstr "陵加拉語"
+msgstr "林加拉語"
 
 msgid "Lithuanian"
 msgstr "立陶宛語"
 
 msgid "Lojban"
 msgstr "邏輯語"
 
 msgid "Low German; Low Saxon; German, Low; Saxon, Low"
-msgstr "低地德語"
+msgstr "低地德文; 低地撒克遜語"
 
 msgid "Lower Sorbian"
-msgstr "低地文德語"
+msgstr "低地索布語"
 
 msgid "Lozi"
 msgstr "洛齊語"
 
 msgid "Luba-Katanga"
 msgstr "盧巴-加丹加語"
 
 msgid "Luba-Lulua"
 msgstr "盧巴-盧拉語"
 
 msgid "Luiseno"
 msgstr "盧伊塞諾語"
 
 msgid "Lule Sami"
-msgstr "魯爾薩米語"
+msgstr "律勒歐薩莫斯語"
 
 msgid "Lunda"
 msgstr "隆達語"
 
 msgid "Luo (Kenya and Tanzania)"
-msgstr "盧奧語(肯尼亞和坦桑尼亞)"
+msgstr "盧奧語 (肯尼亞和坦桑尼亞)"
 
 msgid "Lushai"
 msgstr "盧薩語"
 
 msgid "Luxembourgish; Letzeburgesch"
 msgstr "盧森堡語"
 
@@ -832,36 +832,36 @@
 msgid "Malagasy"
 msgstr "馬達加斯加語"
 
 msgid "Malay"
 msgstr "馬來語"
 
 msgid "Malayalam"
-msgstr "馬來亞拉姆語"
+msgstr "馬拉雅拉姆語"
 
 msgid "Maltese"
-msgstr "馬爾他語"
+msgstr "馬耳他語"
 
 msgid "Manchu"
 msgstr "滿洲語"
 
 msgid "Mandar"
 msgstr "曼達語"
 
 msgid "Mandingo"
 msgstr "曼丁哥語"
 
 msgid "Manipuri"
 msgstr "曼尼普爾語"
 
 msgid "Manobo languages"
-msgstr "馬諾博語系"
+msgstr "馬諾博諸語言"
 
 msgid "Manx"
-msgstr "馬恩語"
+msgstr "馬恩島語"
 
 msgid "Maori"
 msgstr "毛利語"
 
 msgid "Mapudungun; Mapuche"
 msgstr "阿勞坎語"
 
@@ -874,18 +874,18 @@
 msgid "Marshallese"
 msgstr "馬紹爾語"
 
 msgid "Marwari"
 msgstr "馬爾瓦利語"
 
 msgid "Masai"
-msgstr "馬塞語"
+msgstr "馬薩伊語"
 
 msgid "Mayan languages"
-msgstr "瑪雅語系"
+msgstr "瑪雅諸語言"
 
 msgid "Mende"
 msgstr "門德語"
 
 msgid "Mi'kmaq; Micmac"
 msgstr "米克馬克語"
 
@@ -898,39 +898,42 @@
 msgid "Mohawk"
 msgstr "莫霍克語"
 
 msgid "Moksha"
 msgstr "莫克沙語"
 
 msgid "Mon-Khmer languages"
-msgstr "南亞語系"
+msgstr "孟高棉語系"
 
 msgid "Mongo"
 msgstr "芒戈語"
 
 msgid "Mongolian"
 msgstr "蒙古語"
 
+msgid "Montenegrin"
+msgstr "黑山語"
+
 msgid "Mossi"
 msgstr "莫西語"
 
 msgid "Multiple languages"
-msgstr "多重諸語言"
+msgstr "多語種"
 
 msgid "Munda languages"
-msgstr "蒙達語系"
+msgstr "蒙達諸語言"
 
 msgid "N'Ko"
 msgstr "西非書面語"
 
 msgid "Nahuatl languages"
-msgstr "納瓦特爾語系"
+msgstr "納瓦特爾語"
 
 msgid "Nauru"
-msgstr "諾魯"
+msgstr "瑙魯"
 
 msgid "Navajo; Navaho"
 msgstr "納瓦霍語"
 
 msgid "Ndebele, North; North Ndebele"
 msgstr "北恩德貝勒語"
 
@@ -949,216 +952,216 @@
 msgid "Nepali"
 msgstr "尼泊爾語"
 
 msgid "Nias"
 msgstr "尼亞斯語"
 
 msgid "Niger-Kordofanian languages"
-msgstr "尼日-科爾多凡語系"
+msgstr "尼日爾-科爾多凡諸語言"
 
 msgid "Nilo-Saharan languages"
 msgstr "尼羅-撒哈拉語系"
 
 msgid "Niuean"
 msgstr "紐埃語"
 
 msgid "No linguistic content; Not applicable"
-msgstr "無語言內容"
+msgstr "無語言內容; 不適用"
 
 msgid "Nogai"
 msgstr "諾蓋語"
 
 msgid "Norse, Old"
 msgstr "古諾爾斯語"
 
 msgid "North American Indian languages"
-msgstr "北美洲原住民語系"
+msgstr "北美洲土著諸語言"
 
 msgid "Northern Frisian"
-msgstr "北夫里斯蘭語"
+msgstr "北弗里西亞語"
 
 msgid "Northern Sami"
-msgstr "北薩米語"
+msgstr "北薩莫斯語"
 
 msgid "Norwegian"
 msgstr "挪威語"
 
 msgid "Norwegian Nynorsk; Nynorsk, Norwegian"
 msgstr "新挪威語"
 
 msgid "Nubian languages"
-msgstr "努比亞語系"
+msgstr "努比亞語諸語言"
 
 msgid "Nyamwezi"
 msgstr "尼揚韋齊語"
 
 msgid "Nyankole"
-msgstr "尼揚科萊語"
+msgstr "尼揚科勒語"
 
 msgid "Nyoro"
 msgstr "尼奧羅語"
 
 msgid "Nzima"
-msgstr "尼茲馬語"
+msgstr "恩濟馬語"
 
 msgid "Occitan (post 1500); Provençal"
 msgstr "奧克西坦語 (1500 之後);普羅旺斯語"
 
 msgid "Official Aramaic (700-300 BCE); Imperial Aramaic (700-300 BCE)"
 msgstr "宮廷阿拉姆語(公元前 700-300)"
 
 msgid "Ojibwa"
 msgstr "奧杰布瓦語"
 
 msgid "Oriya"
-msgstr "歐利亞語"
+msgstr "奧利亞語"
 
 msgid "Oromo"
 msgstr "奧洛莫語"
 
 msgid "Osage"
-msgstr "歐塞奇語"
+msgstr "奧薩格語"
 
 msgid "Ossetian; Ossetic"
-msgstr "奧塞提語"
+msgstr "奧塞梯語"
 
 msgid "Otomian languages"
-msgstr "奧托米語系"
+msgstr "奧托米諸語言"
 
 msgid "Pahlavi"
-msgstr "巴勒維語"
+msgstr "缽羅缽語"
 
 msgid "Palauan"
-msgstr "帛琉語"
+msgstr "帕勞語"
 
 msgid "Pali"
 msgstr "巴利語"
 
 msgid "Pampanga; Kapampangan"
 msgstr "潘帕嘉語"
 
 msgid "Pangasinan"
-msgstr "龐加辛南語"
+msgstr "邦阿西楠語"
 
 msgid "Panjabi; Punjabi"
 msgstr "旁遮普語"
 
 msgid "Papiamento"
-msgstr "巴皮亞曼多語"
+msgstr "帕皮阿門托語"
 
 msgid "Papuan languages"
 msgstr "巴布亞語系"
 
 msgid "Pedi; Sepedi; Northern Sotho"
-msgstr "北方索托語"
+msgstr "北索托語"
 
 msgid "Persian"
 msgstr "波斯語"
 
 msgid "Persian, Old (ca. 600-400 B.C.)"
-msgstr "古波斯語 (約公元前 600-400)"
+msgstr "古波斯語"
 
 msgid "Philippine languages"
 msgstr "菲律賓語系"
 
 msgid "Phoenician"
 msgstr "腓尼基語"
 
 msgid "Pohnpeian"
-msgstr "波那貝語"
+msgstr "波納佩語"
 
 msgid "Polish"
 msgstr "波蘭語"
 
 msgid "Portuguese"
-msgstr "葡萄牙語"
+msgstr "葡萄牙文"
 
 msgid "Prakrit languages"
-msgstr "普拉克里特語系"
+msgstr "普拉克里特諸語言"
 
 msgid "Provençal, Old (to 1500)"
 msgstr "古普羅旺斯語 (至 1500)"
 
 msgid "Pushto; Pashto"
 msgstr "普什圖語"
 
 msgid "Quechua"
-msgstr "克丘亞語"
+msgstr "凱楚亞語"
 
 msgid "Rajasthani"
 msgstr "拉賈斯坦語"
 
 msgid "Rapanui"
-msgstr "拉巴怒伊語"
+msgstr "拉帕努伊語"
 
 msgid "Rarotongan; Cook Islands Maori"
-msgstr "拉羅通加語"
+msgstr "拉羅湯加語／庫克羣島毛利語"
 
 msgid "Reserved for local use"
 msgstr "保留作內部使用"
 
 msgid "Romance languages"
 msgstr "羅曼語系"
 
 msgid "Romanian; Moldavian; Moldovan"
 msgstr "羅馬尼亞語;莫爾達維亞語;摩爾多瓦語"
 
 msgid "Romansh"
-msgstr "里托羅曼語"
+msgstr "利托-羅曼語"
 
 msgid "Romany"
-msgstr "羅曼尼語"
+msgstr "吉普賽語"
 
 msgid "Rundi"
-msgstr "克倫地語"
+msgstr "基隆迪語"
 
 msgid "Russian"
-msgstr "俄羅斯語"
+msgstr "俄語"
 
 msgid "Salishan languages"
-msgstr "薩利希語系"
+msgstr "薩利什諸語言"
 
 msgid "Samaritan Aramaic"
-msgstr "撒瑪麗亞阿拉姆語"
+msgstr "薩馬利亞阿拉米語"
 
 msgid "Sami languages"
 msgstr "薩米語系"
 
 msgid "Samoan"
 msgstr "薩摩亞語"
 
 msgid "Sandawe"
 msgstr "桑達韋語"
 
 msgid "Sango"
 msgstr "桑戈語"
 
 msgid "Sanskrit"
-msgstr "梵語"
+msgstr "梵文"
 
 msgid "Santali"
 msgstr "桑塔利語"
 
 msgid "Sardinian"
-msgstr "薩丁尼亞語"
+msgstr "撒丁語"
 
 msgid "Sasak"
-msgstr "莎莎克語"
+msgstr "薩薩克語"
 
 msgid "Scots"
 msgstr "蘇格蘭語"
 
 msgid "Selkup"
-msgstr "瑟爾卡普語"
+msgstr "塞爾庫普語"
 
 msgid "Semitic languages"
 msgstr "閃米語系"
 
 msgid "Serbian"
-msgstr "塞爾維亞語"
+msgstr "塞爾維亞文"
 
 msgid "Serer"
 msgstr "塞雷爾語"
 
 msgid "Shan"
 msgstr "撣語"
 
@@ -1168,311 +1171,311 @@
 msgid "Sichuan Yi; Nuosu"
 msgstr "四川彝語"
 
 msgid "Sicilian"
 msgstr "西西里語"
 
 msgid "Sidamo"
-msgstr "希達摩語"
+msgstr "錫達莫語"
 
 msgid "Sign Languages"
-msgstr "手語諸語言"
+msgstr "手語"
 
 msgid "Siksika"
 msgstr "西克西卡語"
 
 msgid "Sindhi"
 msgstr "信德語"
 
 msgid "Sinhala; Sinhalese"
-msgstr "僧加羅語(錫蘭)"
+msgstr "僧加羅語"
 
 msgid "Sino-Tibetan languages"
 msgstr "漢藏語系"
 
 msgid "Siouan languages"
-msgstr "大蘇丹語系"
+msgstr "蘇語諸語言"
 
 msgid "Skolt Sami"
-msgstr "斯克特薩米語"
+msgstr "斯高特薩莫斯語"
 
 msgid "Slave (Athapascan)"
-msgstr "史拉維語 (阿薩帕斯坎語)"
+msgstr "史拉維語"
 
 msgid "Slavic languages"
 msgstr "斯拉夫語系"
 
 msgid "Slovak"
 msgstr "斯洛伐克語"
 
 msgid "Slovenian"
-msgstr "斯洛維尼亞語"
+msgstr "斯洛文尼亞語"
 
 msgid "Sogdian"
 msgstr "粟特語"
 
 msgid "Somali"
-msgstr "索馬利語"
+msgstr "索馬里語"
 
 msgid "Songhai languages"
-msgstr "桑海語系"
+msgstr "桑海語"
 
 msgid "Soninke"
 msgstr "索寧克語"
 
 msgid "Sorbian languages"
-msgstr "文德語系"
+msgstr "索布語系"
 
 msgid "Sotho, Southern"
 msgstr "南索托語"
 
 msgid "South American Indian (Other)"
-msgstr "南美印地安諸語言 (其他)"
+msgstr "南美原居民語言（其他）"
 
 msgid "Southern Altai"
 msgstr "南阿爾泰語"
 
 msgid "Southern Sami"
-msgstr "南薩米語"
+msgstr "南薩莫斯語"
 
 msgid "Spanish; Castilian"
-msgstr "西班牙語"
+msgstr "西班牙文"
 
 msgid "Sranan Tongo"
-msgstr "蘇利南東墎語"
+msgstr "蘇利南語"
 
 msgid "Standard Moroccan Tamazight"
-msgstr "標準摩洛哥塔馬塞特語"
+msgstr "摩洛哥標準柏柏語"
 
 msgid "Sukuma"
 msgstr "蘇庫馬語"
 
 msgid "Sumerian"
-msgstr "蘇美語"
+msgstr "蘇美爾語"
 
 msgid "Sundanese"
-msgstr "巽丹語"
+msgstr "巽他語"
 
 msgid "Susu"
 msgstr "蘇蘇語"
 
 msgid "Swahili"
-msgstr "史瓦西里語"
+msgstr "斯瓦希里語"
 
 msgid "Swati"
-msgstr "斯瓦齊語"
+msgstr "斯瓦特語"
 
 msgid "Swedish"
 msgstr "瑞典語"
 
 msgid "Swiss German; Alemannic; Alsatian"
-msgstr "瑞士德語"
+msgstr "瑞士德文; 阿勒曼尼語; 亞爾薩斯語"
 
 msgid "Syriac"
-msgstr "敘利亞語"
+msgstr "敍利亞文"
 
 msgid "Tagalog"
-msgstr "塔加拉語"
+msgstr "塔加洛語"
 
 msgid "Tahitian"
 msgstr "大溪地語"
 
 msgid "Tai languages"
 msgstr "壯侗語系"
 
 msgid "Tajik"
 msgstr "塔吉克語"
 
 msgid "Tamashek"
-msgstr "泰瑪歇克語"
+msgstr "塔馬奇克語"
 
 msgid "Tamil"
-msgstr "坦米爾語"
+msgstr "泰米爾語"
 
 msgid "Tatar"
-msgstr "韃靼語"
+msgstr "塔塔爾語"
 
 msgid "Telugu"
-msgstr "特拉古語"
+msgstr "泰盧固語"
 
 msgid "Tereno"
-msgstr "特崙諾語"
+msgstr "特列納語"
 
 msgid "Tetum"
 msgstr "德頓語"
 
 msgid "Thai"
-msgstr "泰語"
+msgstr "泰文"
 
 msgid "Tibetan"
 msgstr "藏語"
 
 msgid "Tigre"
-msgstr "泰格瑞語"
+msgstr "提格雷語"
 
 msgid "Tigrinya"
-msgstr "提格利尼亞語"
+msgstr "提格里尼亞語"
 
 msgid "Timne"
-msgstr "堤姆奈語"
+msgstr "滕內語"
 
 msgid "Tiv"
-msgstr "提夫語"
+msgstr "蒂夫語"
 
 msgid "Tlingit"
 msgstr "特林吉特語"
 
 msgid "Tok Pisin"
-msgstr "托比辛語"
+msgstr "托克皮辛語"
 
 msgid "Tokelau"
-msgstr "托克勞"
+msgstr "托克勞羣島"
 
 msgid "Tonga (Nyasa)"
-msgstr "東加語(尼亞沙)"
+msgstr "湯加語 (尼亞薩)"
 
 msgid "Tonga (Tonga Islands)"
-msgstr "東加語(東加群島)"
+msgstr "湯加語 (湯加島)"
 
 msgid "Tsimshian"
 msgstr "欽西安語"
 
 msgid "Tsonga"
-msgstr "宋加語"
+msgstr "宗加語"
 
 msgid "Tswana"
-msgstr "茨瓦納語"
+msgstr "塞茨瓦納語"
 
 msgid "Tumbuka"
-msgstr "通布卡語"
+msgstr "奇圖姆布卡語"
 
 msgid "Tupi languages"
-msgstr "圖皮語系"
+msgstr "圖皮語諸語言"
 
 msgid "Turkish"
 msgstr "土耳其語"
 
 msgid "Turkish, Ottoman (1500-1928)"
-msgstr "鄂圖曼土耳其語 (1500-1928)"
+msgstr "古奧斯曼土耳其語"
 
 msgid "Turkmen"
 msgstr "土庫曼語"
 
 msgid "Tuvalu"
-msgstr "吐瓦魯"
+msgstr "圖瓦盧語"
 
 msgid "Tuvinian"
-msgstr "圖瓦尼安語"
+msgstr "圖瓦語"
 
 msgid "Twi"
-msgstr "奇族語"
+msgstr "特威語"
 
 msgid "Udmurt"
 msgstr "烏德穆爾特語"
 
 msgid "Ugaritic"
-msgstr "烏加里特楔形文字"
+msgstr "烏加里特語"
 
 msgid "Uighur; Uyghur"
 msgstr "維吾爾語"
 
 msgid "Ukrainian"
 msgstr "烏克蘭語"
 
 msgid "Umbundu"
-msgstr "姆本杜語"
+msgstr "翁本杜語"
 
 msgid "Uncoded languages"
 msgstr "未定碼諸語言"
 
 msgid "Undetermined"
-msgstr "未確定"
+msgstr "未確定語種"
 
 msgid "Upper Sorbian"
-msgstr "高地文德語"
+msgstr "高地索布語"
 
 msgid "Urdu"
 msgstr "烏爾都語"
 
 msgid "Uzbek"
 msgstr "烏茲別克語"
 
 msgid "Vai"
 msgstr "瓦伊語"
 
 msgid "Venda"
-msgstr "溫達語"
+msgstr "文達語"
 
 msgid "Vietnamese"
-msgstr "越南語"
+msgstr "越南文"
 
 msgid "Volapük"
 msgstr "沃拉普克語"
 
 msgid "Votic"
 msgstr "沃提克語"
 
 msgid "Wakashan languages"
-msgstr "瓦卡時語系"
+msgstr "瓦卡什諸語言"
 
 msgid "Walamo"
 msgstr "瓦拉莫語"
 
 msgid "Walloon"
-msgstr "瓦隆語"
+msgstr "沃倫語"
 
 msgid "Waray"
-msgstr "瓦瑞語"
+msgstr "瓦賴語"
 
 msgid "Washo"
-msgstr "瓦紹語"
+msgstr "瓦肖語"
 
 msgid "Welsh"
 msgstr "威爾斯語"
 
 msgid "Western Frisian"
-msgstr "西夫里斯蘭語"
+msgstr "弗里西亞語"
 
 msgid "Wolof"
-msgstr "渥魯夫語"
+msgstr "沃洛夫語"
 
 msgid "Xhosa"
 msgstr "科薩語"
 
 msgid "Yakut"
 msgstr "雅庫特語"
 
 msgid "Yao"
-msgstr "瑤語"
+msgstr "瑤文"
 
 msgid "Yapese"
-msgstr "雅蒲語"
+msgstr "雅浦語"
 
 msgid "Yiddish"
-msgstr "意第緒語"
+msgstr "依地語"
 
 msgid "Yoruba"
 msgstr "約魯巴語"
 
 msgid "Yupik languages"
-msgstr "尤皮克語系"
+msgstr "尤皮克諸語言"
 
 msgid "Zande languages"
-msgstr "贊德語系"
+msgstr "贊德語"
 
 msgid "Zapotec"
 msgstr "薩波特克語"
 
 msgid "Zaza; Dimili; Dimli; Kirdki; Kirmanjki; Zazaki"
 msgstr "扎扎其語"
 
 msgid "Zenaga"
-msgstr "澤納加語"
+msgstr "哲納加語"
 
 msgid "Zhuang; Chuang"
-msgstr "壯語"
+msgstr "壯文"
 
 msgid "Zulu"
 msgstr "祖魯語"
 
 msgid "Zuni"
 msgstr "祖尼語"
```

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_15924.xml` & `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_15924.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_3166-1.xml` & `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-1.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_3166-2.xml` & `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-2.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_4217.xml` & `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_4217.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639-2.xml` & `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-2.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639-3.xml` & `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-3.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/isocodes/share/xml/iso-codes/iso_639-5.xml` & `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-5.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/requirements/build-requirements.txt` & `isocodes-2023.6.13/requirements/build-requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,106 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=build --output-file=requirements/build-requirements.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
+cffi==1.15.1
+    # via cryptography
 click==8.1.3
     # via
     #   hatch
     #   userpath
+cryptography==41.0.0
+    # via secretstorage
 distlib==0.3.6
     # via virtualenv
 editables==0.3
     # via hatchling
-filelock==3.9.0
+filelock==3.11.0
     # via virtualenv
 h11==0.14.0
     # via httpcore
-hatch==1.6.3
+hatch==1.7.0
     # via isocodes (pyproject.toml)
-hatchling==1.13.0
+hatchling==1.18.0
     # via hatch
-httpcore==0.16.3
+httpcore==0.17.2
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via hatch
 hyperlink==21.0.0
     # via hatch
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   hyperlink
-    #   rfc3986
-importlib-metadata==6.0.0
+importlib-metadata==6.6.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
+jeepney==0.8.0
+    # via
+    #   keyring
+    #   secretstorage
 keyring==23.13.1
     # via hatch
 markdown-it-py==2.2.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
-packaging==23.0
+packaging==23.1
     # via
     #   hatch
     #   hatchling
-pathspec==0.11.0
+pathspec==0.11.1
     # via hatchling
 pexpect==4.8.0
     # via hatch
-platformdirs==3.1.0
+platformdirs==3.5.3
     # via
     #   hatch
     #   virtualenv
 pluggy==1.0.0
     # via hatchling
 ptyprocess==0.7.0
     # via pexpect
-pygments==2.14.0
+pycparser==2.21
+    # via cffi
+pygments==2.15.1
     # via rich
 pyperclip==1.8.2
     # via hatch
-rfc3986[idna2008]==1.5.0
-    # via httpx
-rich==13.3.2
+rich==13.3.4
     # via hatch
+secretstorage==3.3.3
+    # via keyring
 shellingham==1.5.0.post1
     # via hatch
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
+tomli==2.0.1
+    # via hatchling
 tomli-w==1.0.0
     # via hatch
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via hatch
+trove-classifiers==2023.5.2
+    # via hatchling
 userpath==1.8.0
     # via hatch
-virtualenv==20.20.0
+virtualenv==20.21.0
     # via hatch
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `isocodes-2023.3.9/requirements/dev-requirements.txt` & `isocodes-2023.6.13/requirements/dev-requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements/dev-requirements.txt --resolver=backtracking pyproject.toml
 #
 cfgv==3.3.1
     # via pre-commit
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.11.0
     # via virtualenv
-identify==2.5.19
+identify==2.5.24
     # via pre-commit
 mypy==1.1.1
     # via isocodes (pyproject.toml)
 mypy-extensions==1.0.0
     # via mypy
 nodeenv==1.7.0
     # via pre-commit
-platformdirs==3.1.0
+platformdirs==3.5.3
     # via virtualenv
 pre-commit==2.21.0
     # via isocodes (pyproject.toml)
 pyyaml==6.0
     # via pre-commit
 ruff==0.0.254
     # via isocodes (pyproject.toml)
+tomli==2.0.1
+    # via mypy
 typing-extensions==4.5.0
     # via mypy
-virtualenv==20.20.0
+virtualenv==20.21.0
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `isocodes-2023.3.9/requirements/doc-requirements.txt` & `isocodes-2023.6.13/requirements/doc-requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=doc --output-file=requirements/doc-requirements.txt --resolver=backtracking pyproject.toml
 #
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
@@ -17,15 +17,15 @@
 idna==3.4
     # via requests
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
-markdown==3.3.7
+markdown==3.4.3
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.2
@@ -38,40 +38,40 @@
     # via
     #   isocodes (pyproject.toml)
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-material==9.0.2
+mkdocs-material==9.1.15
     # via isocodes (pyproject.toml)
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
 mkdocstrings==0.19.1
     # via isocodes (pyproject.toml)
-packaging==23.0
+packaging==23.1
     # via mkdocs
-pygments==2.14.0
+pygments==2.15.1
     # via mkdocs-material
-pymdown-extensions==9.10
+pymdown-extensions==10.0
     # via
     #   mkdocs-material
     #   mkdocstrings
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2022.10.31
+regex==2023.3.23
     # via mkdocs-material
-requests==2.28.2
+requests==2.31.0
     # via mkdocs-material
 six==1.16.0
     # via python-dateutil
-urllib3==1.26.14
+urllib3==1.26.15
     # via requests
-watchdog==2.3.1
+watchdog==3.0.0
     # via mkdocs
```

### Comparing `isocodes-2023.3.9/requirements/test-requirements.txt` & `isocodes-2023.6.13/requirements/test-requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-requirements.txt --resolver=backtracking pyproject.toml
 #
-attrs==22.2.0
+attrs==23.1.0
     # via pytest
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+exceptiongroup==1.1.1
+    # via pytest
+filelock==3.11.0
     # via
     #   tox
     #   virtualenv
 iniconfig==2.0.0
     # via pytest
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   pytest
     #   tox
-platformdirs==3.1.0
+platformdirs==3.5.3
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
-pyproject-api==1.5.0
+pyproject-api==1.5.1
     # via tox
 pytest==7.2.0
     # via isocodes (pyproject.toml)
-tox==4.2.8
+tomli==2.0.1
+    # via
+    #   pyproject-api
+    #   pytest
+    #   tox
+tox==4.5.1
     # via isocodes (pyproject.toml)
-virtualenv==20.20.0
+virtualenv==20.21.0
     # via tox
```

### Comparing `isocodes-2023.3.9/.gitignore` & `isocodes-2023.6.13/.gitignore`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/LICENSE` & `isocodes-2023.6.13/LICENSE`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/README.md` & `isocodes-2023.6.13/README.md`

 * *Files identical despite different names*

### Comparing `isocodes-2023.3.9/pyproject.toml` & `isocodes-2023.6.13/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "isocodes"
-version = "2023.03.09"
+version = "2023.06.13"
 description = "This project provides lists of various ISO standards (e.g. country, language, language scripts, and currency names) in one place"
 authors = [{ name = "Atem18", email = "contact@atemlire.io" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 homepage = "https://github.com/Atem18/isocodes"
 repository = "https://github.com/Atem18/isocodes"
 keywords = ["iso"]
@@ -18,12 +18,12 @@
     "Programming Language :: Python :: 3.7",
 ]
 dependencies = []
 
 [project.optional-dependencies]
 dev = ["pre-commit >=2.17.0,<3.0.0", "ruff == 0.0.254", "mypy == 1.1.1"]
 
-doc = ["mkdocs == 1.4.2", "mkdocs-material == 9.0.2", "mkdocstrings == 0.19.1"]
+doc = ["mkdocs == 1.4.2", "mkdocs-material == 9.1.15", "mkdocstrings == 0.19.1"]
 
-test = ["pytest == 7.2.0", "tox == 4.2.8"]
+test = ["pytest == 7.2.0", "tox == 4.5.1"]
 
-build = ["hatch == 1.6.3"]
+build = ["hatch == 1.7.0"]
```

### Comparing `isocodes-2023.3.9/PKG-INFO` & `isocodes-2023.6.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isocodes
-Version: 2023.3.9
+Version: 2023.6.13
 Summary: This project provides lists of various ISO standards (e.g. country, language, language scripts, and currency names) in one place
 Author-email: Atem18 <contact@atemlire.io>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -463,26 +463,26 @@
                              END OF TERMS AND CONDITIONS
 License-File: LICENSE
 Keywords: iso
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: build
-Requires-Dist: hatch==1.6.3; extra == 'build'
+Requires-Dist: hatch==1.7.0; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: mypy==1.1.1; extra == 'dev'
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: ruff==0.0.254; extra == 'dev'
 Provides-Extra: doc
-Requires-Dist: mkdocs-material==9.0.2; extra == 'doc'
+Requires-Dist: mkdocs-material==9.1.15; extra == 'doc'
 Requires-Dist: mkdocs==1.4.2; extra == 'doc'
 Requires-Dist: mkdocstrings==0.19.1; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest==7.2.0; extra == 'test'
-Requires-Dist: tox==4.2.8; extra == 'test'
+Requires-Dist: tox==4.5.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # isocodes
 
 isocodes provides you access to lists of various ISO standards (e.g. country, language, language scripts, and currency names).
 
 The data is coming from https://salsa.debian.org/iso-codes-team/iso-codes, many thanks to them.
```

