# Comparing `tmp/finance_enums-0.1.1.tar.gz` & `tmp/finance_enums-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finance_enums-0.1.1.tar", last modified: Thu May 26 18:37:30 2022, max compression
+gzip compressed data
```

## Comparing `finance_enums-0.1.1.tar` & `finance_enums-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,326 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-26 18:37:30.099438 finance_enums-0.1.1/
--rw-r--r--   0 timkpaine   (501) staff       (20)    11351 2022-05-26 17:52:57.000000 finance_enums-0.1.1/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      136 2022-05-26 18:04:05.000000 finance_enums-0.1.1/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     1524 2022-05-26 18:37:30.099592 finance_enums-0.1.1/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      663 2021-01-25 04:03:12.000000 finance_enums-0.1.1/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-26 18:37:30.093099 finance_enums-0.1.1/finance_enums/
--rw-r--r--   0 timkpaine   (501) staff       (20)      154 2022-05-26 18:37:22.000000 finance_enums-0.1.1/finance_enums/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-26 18:37:30.095061 finance_enums-0.1.1/finance_enums/data/
--rw-r--r--   0 timkpaine   (501) staff       (20)   261501 2018-09-20 03:00:30.000000 finance_enums-0.1.1/finance_enums/data/mics.csv
--rw-r--r--   0 timkpaine   (501) staff       (20)      352 2021-01-25 04:03:12.000000 finance_enums-0.1.1/finance_enums/exchange.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-26 18:37:30.098136 finance_enums-0.1.1/finance_enums/sectors/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2018-09-19 15:50:44.000000 finance_enums-0.1.1/finance_enums/sectors/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2727 2021-01-25 04:03:12.000000 finance_enums-0.1.1/finance_enums/sectors/us.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-26 18:37:30.098909 finance_enums-0.1.1/finance_enums/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2022-05-26 18:27:57.000000 finance_enums-0.1.1/finance_enums/tests/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      132 2022-05-26 18:27:57.000000 finance_enums-0.1.1/finance_enums/tests/test_all.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-26 18:37:30.094737 finance_enums-0.1.1/finance_enums.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1524 2022-05-26 18:37:29.000000 finance_enums-0.1.1/finance_enums.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      438 2022-05-26 18:37:29.000000 finance_enums-0.1.1/finance_enums.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2022-05-26 18:37:29.000000 finance_enums-0.1.1/finance_enums.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)      145 2022-05-26 18:37:29.000000 finance_enums-0.1.1/finance_enums.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       14 2022-05-26 18:37:29.000000 finance_enums-0.1.1/finance_enums.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)      530 2022-05-26 18:37:30.100332 finance_enums-0.1.1/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     1477 2022-05-26 18:37:22.000000 finance_enums-0.1.1/setup.py
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 finance_enums-0.2.0/local_dependencies/finance_enums/Cargo.toml
+-rw-r--r--   0     1001      123     1587 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/Makefile
+-rw-r--r--   0     1001      123        1 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/common/mod.rs
+-rw-r--r--   0     1001      123   157747 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/country/iso3166.rs
+-rw-r--r--   0     1001      123       34 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/country/mod.rs
+-rw-r--r--   0     1001      123    10861 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/currency/iso4217.rs
+-rw-r--r--   0     1001      123       33 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/currency/mod.rs
+-rw-r--r--   0     1001      123     3769 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/exchange/iso10383.rs
+-rw-r--r--   0     1001      123       87 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/exchange/mod.rs
+-rw-r--r--   0     1001      123       44 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/instrument/iso10962.rs
+-rw-r--r--   0     1001      123      457 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/instrument/mod.rs
+-rw-r--r--   0     1001      123      351 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/lib.rs
+-rw-r--r--   0     1001      123    22775 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/sector/industry.rs
+-rw-r--r--   0     1001      123    10828 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/sector/industry_group.rs
+-rw-r--r--   0     1001      123      314 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/sector/mod.rs
+-rw-r--r--   0     1001      123     5173 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/sector/sector.rs
+-rw-r--r--   0     1001      123    24083 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/sector/subindustry.rs
+-rw-r--r--   0     1001      123      239 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/bond.rs
+-rw-r--r--   0     1001      123     1229 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/commodity.rs
+-rw-r--r--   0     1001      123        1 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/currency.rs
+-rw-r--r--   0     1001      123      306 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/equity.rs
+-rw-r--r--   0     1001      123      623 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/fund.rs
+-rw-r--r--   0     1001      123      415 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/future.rs
+-rw-r--r--   0     1001      123      290 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/mod.rs
+-rw-r--r--   0     1001      123      422 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/option.rs
+-rw-r--r--   0     1001      123      349 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/security/security.rs
+-rw-r--r--   0     1001      123      796 2023-06-13 20:01:52.000000 finance_enums-0.2.0/local_dependencies/finance_enums/src/trading/mod.rs
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 finance_enums-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      414 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.bumpversion.cfg
+-rw-r--r--   0     1001      123      147 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.gitattributes
+-rw-r--r--   0     1001      123     3352 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123      834 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      595 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      294 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.github/dependabot.yml
+-rw-r--r--   0     1001      123     1608 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0     1001      123     4126 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123     2275 2023-06-13 20:01:52.000000 finance_enums-0.2.0/.gitignore
+-rw-r--r--   0     1001      123    11351 2023-06-13 20:01:52.000000 finance_enums-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1990 2023-06-13 20:01:52.000000 finance_enums-0.2.0/Makefile
+-rw-r--r--   0     1001      123     1246 2023-06-13 20:01:52.000000 finance_enums-0.2.0/README.md
+-rw-r--r--   0     1001      123       52 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/__init__.py
+-rw-r--r--   0     1001      123       52 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_all.py
+-rw-r--r--   0     1001      123      195 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_country.py
+-rw-r--r--   0     1001      123      239 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_currency.py
+-rw-r--r--   0     1001      123      137 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_exchange.py
+-rw-r--r--   0     1001      123        0 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_instrument.py
+-rw-r--r--   0     1001      123      428 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_sector.py
+-rw-r--r--   0     1001      123     1024 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_security.py
+-rw-r--r--   0     1001      123      413 2023-06-13 20:01:52.000000 finance_enums-0.2.0/finance_enums/tests/test_trading.py
+-rw-r--r--   0     1001      123      309 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AD.png
+-rw-r--r--   0     1001      123      122 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AE.png
+-rw-r--r--   0     1001      123      586 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AF.png
+-rw-r--r--   0     1001      123      443 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AG.png
+-rw-r--r--   0     1001      123      410 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AI.png
+-rw-r--r--   0     1001      123      315 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AL.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AM.png
+-rw-r--r--   0     1001      123      285 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AO.png
+-rw-r--r--   0     1001      123      300 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AQ.png
+-rw-r--r--   0     1001      123      150 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AR.png
+-rw-r--r--   0     1001      123      469 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AS.png
+-rw-r--r--   0     1001      123       93 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AT.png
+-rw-r--r--   0     1001      123      405 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AU.png
+-rw-r--r--   0     1001      123      176 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AW.png
+-rw-r--r--   0     1001      123      155 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AX.png
+-rw-r--r--   0     1001      123      165 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/AZ.png
+-rw-r--r--   0     1001      123      321 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BA.png
+-rw-r--r--   0     1001      123      235 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BB.png
+-rw-r--r--   0     1001      123      246 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BD.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BE.png
+-rw-r--r--   0     1001      123      173 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BF.png
+-rw-r--r--   0     1001      123      116 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BG.png
+-rw-r--r--   0     1001      123      189 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BH.png
+-rw-r--r--   0     1001      123      394 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BI.png
+-rw-r--r--   0     1001      123      122 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BJ.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BL.png
+-rw-r--r--   0     1001      123      461 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BM.png
+-rw-r--r--   0     1001      123      547 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BN.png
+-rw-r--r--   0     1001      123      217 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BO.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BQ.png
+-rw-r--r--   0     1001      123      438 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BR.png
+-rw-r--r--   0     1001      123      181 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BS.png
+-rw-r--r--   0     1001      123      570 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BT.png
+-rw-r--r--   0     1001      123      153 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BV.png
+-rw-r--r--   0     1001      123      111 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BW.png
+-rw-r--r--   0     1001      123      206 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BY.png
+-rw-r--r--   0     1001      123      378 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/BZ.png
+-rw-r--r--   0     1001      123      259 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CA.png
+-rw-r--r--   0     1001      123      365 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CC.png
+-rw-r--r--   0     1001      123      350 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CD.png
+-rw-r--r--   0     1001      123      246 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CF.png
+-rw-r--r--   0     1001      123      330 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CG.png
+-rw-r--r--   0     1001      123      113 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CH.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CI.png
+-rw-r--r--   0     1001      123      487 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CK.png
+-rw-r--r--   0     1001      123      186 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CL.png
+-rw-r--r--   0     1001      123      158 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CM.png
+-rw-r--r--   0     1001      123      214 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CN.png
+-rw-r--r--   0     1001      123      116 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CO.png
+-rw-r--r--   0     1001      123      123 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CR.png
+-rw-r--r--   0     1001      123      240 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CU.png
+-rw-r--r--   0     1001      123      267 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CV.png
+-rw-r--r--   0     1001      123      189 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CW.png
+-rw-r--r--   0     1001      123      508 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CX.png
+-rw-r--r--   0     1001      123      318 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CY.png
+-rw-r--r--   0     1001      123      273 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/CZ.png
+-rw-r--r--   0     1001      123      116 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/DE.png
+-rw-r--r--   0     1001      123      358 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/DJ.png
+-rw-r--r--   0     1001      123      124 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/DK.png
+-rw-r--r--   0     1001      123      269 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/DM.png
+-rw-r--r--   0     1001      123      158 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/DO.png
+-rw-r--r--   0     1001      123      276 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/DZ.png
+-rw-r--r--   0     1001      123      325 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/EC.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/EE.png
+-rw-r--r--   0     1001      123      175 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/EG.png
+-rw-r--r--   0     1001      123      271 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/EH.png
+-rw-r--r--   0     1001      123      465 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ER.png
+-rw-r--r--   0     1001      123      273 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ES.png
+-rw-r--r--   0     1001      123      324 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ET.png
+-rw-r--r--   0     1001      123      130 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/FI.png
+-rw-r--r--   0     1001      123      456 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/FJ.png
+-rw-r--r--   0     1001      123      475 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/FK.png
+-rw-r--r--   0     1001      123      183 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/FM.png
+-rw-r--r--   0     1001      123      150 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/FO.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/FR.png
+-rw-r--r--   0     1001      123       98 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GA.png
+-rw-r--r--   0     1001      123      490 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GB.png
+-rw-r--r--   0     1001      123      417 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GD.png
+-rw-r--r--   0     1001      123      155 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GE.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GF.png
+-rw-r--r--   0     1001      123      184 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GG.png
+-rw-r--r--   0     1001      123      180 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GH.png
+-rw-r--r--   0     1001      123      288 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GI.png
+-rw-r--r--   0     1001      123      302 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GL.png
+-rw-r--r--   0     1001      123      110 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GM.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GN.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GP.png
+-rw-r--r--   0     1001      123      305 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GQ.png
+-rw-r--r--   0     1001      123      180 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GR.png
+-rw-r--r--   0     1001      123      517 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GS.png
+-rw-r--r--   0     1001      123      210 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GT.png
+-rw-r--r--   0     1001      123      237 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GU.png
+-rw-r--r--   0     1001      123      168 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GW.png
+-rw-r--r--   0     1001      123      375 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/GY.png
+-rw-r--r--   0     1001      123      321 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/HK.png
+-rw-r--r--   0     1001      123      405 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/HM.png
+-rw-r--r--   0     1001      123      137 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/HN.png
+-rw-r--r--   0     1001      123      262 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/HR.png
+-rw-r--r--   0     1001      123      171 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/HT.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/HU.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ID.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IE.png
+-rw-r--r--   0     1001      123      170 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IL.png
+-rw-r--r--   0     1001      123      250 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IM.png
+-rw-r--r--   0     1001      123      182 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IN.png
+-rw-r--r--   0     1001      123      952 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IO.png
+-rw-r--r--   0     1001      123      203 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IQ.png
+-rw-r--r--   0     1001      123      356 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IR.png
+-rw-r--r--   0     1001      123      153 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IS.png
+-rw-r--r--   0     1001      123      122 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/IT.png
+-rw-r--r--   0     1001      123      453 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/JE.png
+-rw-r--r--   0     1001      123      322 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/JM.png
+-rw-r--r--   0     1001      123      250 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/JO.png
+-rw-r--r--   0     1001      123      240 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/JP.png
+-rw-r--r--   0     1001      123      294 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KE.png
+-rw-r--r--   0     1001      123      327 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KG.png
+-rw-r--r--   0     1001      123      271 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KH.png
+-rw-r--r--   0     1001      123      604 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KI.png
+-rw-r--r--   0     1001      123      413 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KM.png
+-rw-r--r--   0     1001      123      618 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KN.png
+-rw-r--r--   0     1001      123      233 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KP.png
+-rw-r--r--   0     1001      123      447 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KR.png
+-rw-r--r--   0     1001      123      195 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KW.png
+-rw-r--r--   0     1001      123      456 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KY.png
+-rw-r--r--   0     1001      123      331 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/KZ.png
+-rw-r--r--   0     1001      123      173 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LA.png
+-rw-r--r--   0     1001      123      308 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LB.png
+-rw-r--r--   0     1001      123      261 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LC.png
+-rw-r--r--   0     1001      123      199 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LI.png
+-rw-r--r--   0     1001      123      492 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LK.png
+-rw-r--r--   0     1001      123      205 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LR.png
+-rw-r--r--   0     1001      123      209 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LS.png
+-rw-r--r--   0     1001      123      116 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LT.png
+-rw-r--r--   0     1001      123      116 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LU.png
+-rw-r--r--   0     1001      123      103 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LV.png
+-rw-r--r--   0     1001      123      149 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/LY.png
+-rw-r--r--   0     1001      123      190 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MA.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MC.png
+-rw-r--r--   0     1001      123      249 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MD.png
+-rw-r--r--   0     1001      123      335 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ME.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MF.png
+-rw-r--r--   0     1001      123      122 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MG.png
+-rw-r--r--   0     1001      123      520 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MH.png
+-rw-r--r--   0     1001      123      418 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MK.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ML.png
+-rw-r--r--   0     1001      123      280 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MM.png
+-rw-r--r--   0     1001      123      243 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MN.png
+-rw-r--r--   0     1001      123      311 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MO.png
+-rw-r--r--   0     1001      123      450 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MP.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MQ.png
+-rw-r--r--   0     1001      123      266 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MR.png
+-rw-r--r--   0     1001      123      454 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MS.png
+-rw-r--r--   0     1001      123      174 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MT.png
+-rw-r--r--   0     1001      123      132 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MU.png
+-rw-r--r--   0     1001      123      187 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MV.png
+-rw-r--r--   0     1001      123      231 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MW.png
+-rw-r--r--   0     1001      123      247 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MX.png
+-rw-r--r--   0     1001      123      304 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MY.png
+-rw-r--r--   0     1001      123      395 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/MZ.png
+-rw-r--r--   0     1001      123      602 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NA.png
+-rw-r--r--   0     1001      123      393 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NC.png
+-rw-r--r--   0     1001      123      152 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NE.png
+-rw-r--r--   0     1001      123      284 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NF.png
+-rw-r--r--   0     1001      123       96 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NG.png
+-rw-r--r--   0     1001      123      193 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NI.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NL.png
+-rw-r--r--   0     1001      123      153 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NO.png
+-rw-r--r--   0     1001      123      646 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NP.png
+-rw-r--r--   0     1001      123      151 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NR.png
+-rw-r--r--   0     1001      123      336 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NU.png
+-rw-r--r--   0     1001      123      376 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/NZ.png
+-rw-r--r--   0     1001      123      179 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/OM.png
+-rw-r--r--   0     1001      123      294 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PA.png
+-rw-r--r--   0     1001      123       96 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PE.png
+-rw-r--r--   0     1001      123      294 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PF.png
+-rw-r--r--   0     1001      123      377 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PG.png
+-rw-r--r--   0     1001      123      319 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PH.png
+-rw-r--r--   0     1001      123      295 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PK.png
+-rw-r--r--   0     1001      123       92 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PL.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PM.png
+-rw-r--r--   0     1001      123      556 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PN.png
+-rw-r--r--   0     1001      123      296 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PR.png
+-rw-r--r--   0     1001      123      293 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PS.png
+-rw-r--r--   0     1001      123      354 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PT.png
+-rw-r--r--   0     1001      123      239 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PW.png
+-rw-r--r--   0     1001      123      190 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/PY.png
+-rw-r--r--   0     1001      123      104 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/QA.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/RE.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/RO.png
+-rw-r--r--   0     1001      123      398 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/RS.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/RU.png
+-rw-r--r--   0     1001      123      212 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/RW.png
+-rw-r--r--   0     1001      123      334 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SA.png
+-rw-r--r--   0     1001      123      477 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SB.png
+-rw-r--r--   0     1001      123      517 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SC.png
+-rw-r--r--   0     1001      123      222 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SD.png
+-rw-r--r--   0     1001      123      130 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SE.png
+-rw-r--r--   0     1001      123      249 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SG.png
+-rw-r--r--   0     1001      123      490 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SH.png
+-rw-r--r--   0     1001      123      173 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SI.png
+-rw-r--r--   0     1001      123      153 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SJ.png
+-rw-r--r--   0     1001      123      326 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SK.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SL.png
+-rw-r--r--   0     1001      123      362 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SM.png
+-rw-r--r--   0     1001      123      158 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SN.png
+-rw-r--r--   0     1001      123      198 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SO.png
+-rw-r--r--   0     1001      123      215 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SR.png
+-rw-r--r--   0     1001      123      264 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SS.png
+-rw-r--r--   0     1001      123      254 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ST.png
+-rw-r--r--   0     1001      123      195 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SV.png
+-rw-r--r--   0     1001      123      419 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SX.png
+-rw-r--r--   0     1001      123      182 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SY.png
+-rw-r--r--   0     1001      123      436 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/SZ.png
+-rw-r--r--   0     1001      123      414 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TC.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TD.png
+-rw-r--r--   0     1001      123      328 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TF.png
+-rw-r--r--   0     1001      123      248 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TG.png
+-rw-r--r--   0     1001      123      114 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TH.png
+-rw-r--r--   0     1001      123      196 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TJ.png
+-rw-r--r--   0     1001      123      384 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TK.png
+-rw-r--r--   0     1001      123      280 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TL.png
+-rw-r--r--   0     1001      123      486 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TM.png
+-rw-r--r--   0     1001      123      285 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TN.png
+-rw-r--r--   0     1001      123      142 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TO.png
+-rw-r--r--   0     1001      123      263 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TR.png
+-rw-r--r--   0     1001      123      466 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TT.png
+-rw-r--r--   0     1001      123      482 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TV.png
+-rw-r--r--   0     1001      123      235 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TW.png
+-rw-r--r--   0     1001      123      511 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/TZ.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/UA.png
+-rw-r--r--   0     1001      123      231 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/UG.png
+-rw-r--r--   0     1001      123      333 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/UM.png
+-rw-r--r--   0     1001      123      333 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/US.png
+-rw-r--r--   0     1001      123      294 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/UY.png
+-rw-r--r--   0     1001      123      213 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/UZ.png
+-rw-r--r--   0     1001      123      282 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/VA.png
+-rw-r--r--   0     1001      123      239 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/VC.png
+-rw-r--r--   0     1001      123      197 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/VE.png
+-rw-r--r--   0     1001      123      471 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/VG.png
+-rw-r--r--   0     1001      123      795 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/VI.png
+-rw-r--r--   0     1001      123      205 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/VN.png
+-rw-r--r--   0     1001      123      427 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/VU.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/WF.png
+-rw-r--r--   0     1001      123      182 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/WS.png
+-rw-r--r--   0     1001      123      100 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/YE.png
+-rw-r--r--   0     1001      123      108 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/YT.png
+-rw-r--r--   0     1001      123      406 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ZA.png
+-rw-r--r--   0     1001      123      225 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ZM.png
+-rw-r--r--   0     1001      123      295 2023-06-13 20:01:52.000000 finance_enums-0.2.0/flags/ZW.png
+-rw-r--r--   0     1001      123    79321 2023-06-13 20:01:52.000000 finance_enums-0.2.0/helpers/GICS Map 2023.xlsx
+-rw-r--r--   0     1001      123   509696 2023-06-13 20:01:52.000000 finance_enums-0.2.0/helpers/ISO10383_MIC.csv
+-rw-r--r--   0     1001      123      402 2023-06-13 20:01:52.000000 finance_enums-0.2.0/helpers/flags_to_strings.py
+-rw-r--r--   0     1001      123   149841 2023-06-13 20:01:52.000000 finance_enums-0.2.0/helpers/iso10383_generated.rs
+-rw-r--r--   0     1001      123     4962 2023-06-13 20:01:52.000000 finance_enums-0.2.0/helpers/process_mics.py
+-rw-r--r--   0     1001      123      577 2023-06-13 20:01:52.000000 finance_enums-0.2.0/helpers/scrape_flags.py
+-rw-r--r--   0     1001      123     1545 2023-06-13 20:01:52.000000 finance_enums-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123    58696 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/country/mod.rs
+-rw-r--r--   0     1001      123    27210 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/currency/mod.rs
+-rw-r--r--   0     1001      123     4106 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/exchange/mod.rs
+-rw-r--r--   0     1001      123        0 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/instrument/mod.rs
+-rw-r--r--   0     1001      123     1302 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123    14542 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/sector/industry.rs
+-rw-r--r--   0     1001      123     6641 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/sector/industry_group.rs
+-rw-r--r--   0     1001      123      190 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/sector/mod.rs
+-rw-r--r--   0     1001      123     3011 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/sector/sector.rs
+-rw-r--r--   0     1001      123    32067 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/sector/subindustry.rs
+-rw-r--r--   0     1001      123     1581 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/bond.rs
+-rw-r--r--   0     1001      123     1681 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/commodity.rs
+-rw-r--r--   0     1001      123        0 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/currency.rs
+-rw-r--r--   0     1001      123     2018 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/equity.rs
+-rw-r--r--   0     1001      123     4717 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/fund.rs
+-rw-r--r--   0     1001      123      259 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/mod.rs
+-rw-r--r--   0     1001      123     3113 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/option.rs
+-rw-r--r--   0     1001      123     3115 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/security/security.rs
+-rw-r--r--   0     1001      123     5933 2023-06-13 20:01:52.000000 finance_enums-0.2.0/src/trading/mod.rs
+-rw-r--r--   0     1001      123    17385 2023-06-13 20:02:29.000000 finance_enums-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     2749 1970-01-01 00:00:00.000000 finance_enums-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `finance_enums-0.1.1/LICENSE` & `finance_enums-0.2.0/LICENSE`

 * *Files identical despite different names*

