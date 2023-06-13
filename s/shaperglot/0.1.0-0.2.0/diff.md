# Comparing `tmp/shaperglot-0.1.0.tar.gz` & `tmp/shaperglot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaperglot-0.1.0.tar", max compression
+gzip compressed data, was "shaperglot-0.2.0.tar", max compression
```

## Comparing `shaperglot-0.1.0.tar` & `shaperglot-0.2.0.tar`

### file list

```diff
@@ -1,446 +1,446 @@
--rw-r--r--   0        0        0    35147 2022-10-18 13:07:30.650622 shaperglot-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     6768 2023-05-22 09:11:30.139691 shaperglot-0.1.0/README.md
--rw-r--r--   0        0        0     1600 2023-05-22 09:11:48.826818 shaperglot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      185 2022-10-18 13:07:30.651786 shaperglot-0.1.0/shaperglot/__init__.py
--rw-r--r--   0        0        0      144 2022-10-18 13:07:30.651915 shaperglot-0.1.0/shaperglot/__main__.py
--rw-r--r--   0        0        0     2245 2022-12-01 14:51:30.745263 shaperglot-0.1.0/shaperglot/checker.py
--rw-r--r--   0        0        0      431 2022-11-21 16:30:15.886978 shaperglot-0.1.0/shaperglot/checks/__init__.py
--rw-r--r--   0        0        0     3048 2022-11-25 11:21:48.131068 shaperglot-0.1.0/shaperglot/checks/common.py
--rw-r--r--   0        0        0     3324 2022-12-01 12:22:23.920017 shaperglot-0.1.0/shaperglot/checks/no_orphaned_marks.py
--rw-r--r--   0        0        0     2734 2022-12-01 14:51:30.745911 shaperglot-0.1.0/shaperglot/checks/orthographies.py
--rw-r--r--   0        0        0     4183 2022-12-01 14:51:30.746146 shaperglot-0.1.0/shaperglot/checks/shaping_differs.py
--rw-r--r--   0        0        0     2266 2022-11-25 11:21:57.762374 shaperglot-0.1.0/shaperglot/checks/unencoded_variants.py
--rw-r--r--   0        0        0     6277 2022-12-01 14:51:30.755552 shaperglot-0.1.0/shaperglot/cli.py
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.141357 shaperglot-0.1.0/shaperglot/languages/aa_Latn.yaml
--rw-r--r--   0        0        0     5033 2023-05-22 09:11:30.141465 shaperglot-0.1.0/shaperglot/languages/abi_Latn.yaml
--rw-r--r--   0        0        0     3699 2023-05-22 09:11:30.141565 shaperglot-0.1.0/shaperglot/languages/abr_Latn.yaml
--rw-r--r--   0        0        0     5086 2023-05-22 09:11:30.141634 shaperglot-0.1.0/shaperglot/languages/acd_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.141733 shaperglot-0.1.0/shaperglot/languages/ada_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.141800 shaperglot-0.1.0/shaperglot/languages/ade_Latn.yaml
--rw-r--r--   0        0        0     5255 2023-05-22 09:11:30.141873 shaperglot-0.1.0/shaperglot/languages/adj_Latn.yaml
--rw-r--r--   0        0        0     8271 2023-05-22 09:11:30.141978 shaperglot-0.1.0/shaperglot/languages/aeb_Latn.yaml
--rw-r--r--   0        0        0     8582 2023-05-22 09:11:30.144862 shaperglot-0.1.0/shaperglot/languages/af_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.144965 shaperglot-0.1.0/shaperglot/languages/agc_Latn.yaml
--rw-r--r--   0        0        0     8886 2023-05-22 09:11:30.145539 shaperglot-0.1.0/shaperglot/languages/agq_Latn.yaml
--rw-r--r--   0        0        0     5202 2023-05-22 09:11:30.145607 shaperglot-0.1.0/shaperglot/languages/aha_Latn.yaml
--rw-r--r--   0        0        0     6773 2023-05-22 09:11:30.145700 shaperglot-0.1.0/shaperglot/languages/ahl_Latn.yaml
--rw-r--r--   0        0        0     6438 2023-05-22 09:11:30.145800 shaperglot-0.1.0/shaperglot/languages/ahs_Latn.yaml
--rw-r--r--   0        0        0      193 2022-10-19 14:11:13.581683 shaperglot-0.1.0/shaperglot/languages/ajg_Latn.yaml
--rw-r--r--   0        0        0     4529 2023-05-22 09:11:30.145896 shaperglot-0.1.0/shaperglot/languages/ak_Latn.yaml
--rw-r--r--   0        0        0     4876 2023-05-22 09:11:30.145966 shaperglot-0.1.0/shaperglot/languages/akp_Latn.yaml
--rw-r--r--   0        0        0     4526 2023-05-22 09:11:30.146041 shaperglot-0.1.0/shaperglot/languages/ala_Latn.yaml
--rw-r--r--   0        0        0     7239 2023-05-22 09:11:30.146123 shaperglot-0.1.0/shaperglot/languages/anc_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.146201 shaperglot-0.1.0/shaperglot/languages/ank_Latn.yaml
--rw-r--r--   0        0        0     6228 2023-05-22 09:11:30.146270 shaperglot-0.1.0/shaperglot/languages/ann_Latn.yaml
--rw-r--r--   0        0        0     4416 2023-05-22 09:11:30.146382 shaperglot-0.1.0/shaperglot/languages/anv_Latn.yaml
--rw-r--r--   0        0        0     5202 2023-05-22 09:11:30.146466 shaperglot-0.1.0/shaperglot/languages/any_Latn.yaml
--rw-r--r--   0        0        0     5217 2023-05-22 09:11:30.146539 shaperglot-0.1.0/shaperglot/languages/apd_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.146610 shaperglot-0.1.0/shaperglot/languages/asa_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.146682 shaperglot-0.1.0/shaperglot/languages/asg_Latn.yaml
--rw-r--r--   0        0        0     5039 2023-05-22 09:11:30.146749 shaperglot-0.1.0/shaperglot/languages/atg_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.146831 shaperglot-0.1.0/shaperglot/languages/avn_Latn.yaml
--rw-r--r--   0        0        0     4923 2023-05-22 09:11:30.146902 shaperglot-0.1.0/shaperglot/languages/avu_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.146969 shaperglot-0.1.0/shaperglot/languages/awo_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.147040 shaperglot-0.1.0/shaperglot/languages/ayb_Latn.yaml
--rw-r--r--   0        0        0    10210 2023-05-22 09:11:30.147642 shaperglot-0.1.0/shaperglot/languages/bas_Latn.yaml
--rw-r--r--   0        0        0     5424 2023-05-22 09:11:30.147754 shaperglot-0.1.0/shaperglot/languages/bav_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.147829 shaperglot-0.1.0/shaperglot/languages/bbp_Latn.yaml
--rw-r--r--   0        0        0     4197 2023-05-22 09:11:30.147901 shaperglot-0.1.0/shaperglot/languages/bci_Latn.yaml
--rw-r--r--   0        0        0     7915 2023-05-22 09:11:30.147993 shaperglot-0.1.0/shaperglot/languages/bcn_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.148080 shaperglot-0.1.0/shaperglot/languages/bcq_Latn.yaml
--rw-r--r--   0        0        0     4591 2023-05-22 09:11:30.148184 shaperglot-0.1.0/shaperglot/languages/bcw_Latn.yaml
--rw-r--r--   0        0        0     5205 2023-05-22 09:11:30.148293 shaperglot-0.1.0/shaperglot/languages/bcy_Latn.yaml
--rw-r--r--   0        0        0     5060 2023-05-22 09:11:30.148450 shaperglot-0.1.0/shaperglot/languages/bdh_Latn.yaml
--rw-r--r--   0        0        0     4526 2023-05-22 09:11:30.148537 shaperglot-0.1.0/shaperglot/languages/beh_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.148627 shaperglot-0.1.0/shaperglot/languages/bej_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.148709 shaperglot-0.1.0/shaperglot/languages/bem_Latn.yaml
--rw-r--r--   0        0        0     5543 2023-05-22 09:11:30.148789 shaperglot-0.1.0/shaperglot/languages/bet_Latn.yaml
--rw-r--r--   0        0        0     5756 2023-05-22 09:11:30.149013 shaperglot-0.1.0/shaperglot/languages/bex_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.149086 shaperglot-0.1.0/shaperglot/languages/bez_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.149161 shaperglot-0.1.0/shaperglot/languages/bhy_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.149234 shaperglot-0.1.0/shaperglot/languages/bib_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.149317 shaperglot-0.1.0/shaperglot/languages/bim_Latn.yaml
--rw-r--r--   0        0        0     5220 2023-05-22 09:11:30.149388 shaperglot-0.1.0/shaperglot/languages/bin_Latn.yaml
--rw-r--r--   0        0        0     4754 2023-05-22 09:11:30.149453 shaperglot-0.1.0/shaperglot/languages/biv_Latn.yaml
--rw-r--r--   0        0        0     4206 2023-05-22 09:11:30.149530 shaperglot-0.1.0/shaperglot/languages/bjv_Latn.yaml
--rw-r--r--   0        0        0     5033 2023-05-22 09:11:30.149626 shaperglot-0.1.0/shaperglot/languages/bkc_Latn.yaml
--rw-r--r--   0        0        0     8247 2023-05-22 09:11:30.149714 shaperglot-0.1.0/shaperglot/languages/bkv_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.149787 shaperglot-0.1.0/shaperglot/languages/blo_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.149848 shaperglot-0.1.0/shaperglot/languages/bm_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.149925 shaperglot-0.1.0/shaperglot/languages/bng_Latn.yaml
--rw-r--r--   0        0        0     4360 2023-05-22 09:11:30.149992 shaperglot-0.1.0/shaperglot/languages/bnm_Latn.yaml
--rw-r--r--   0        0        0     5748 2023-05-22 09:11:30.150056 shaperglot-0.1.0/shaperglot/languages/bom_Latn.yaml
--rw-r--r--   0        0        0     5045 2023-05-22 09:11:30.150123 shaperglot-0.1.0/shaperglot/languages/bov_Latn.yaml
--rw-r--r--   0        0        0     4876 2023-05-22 09:11:30.150207 shaperglot-0.1.0/shaperglot/languages/box_Latn.yaml
--rw-r--r--   0        0        0     4917 2023-05-22 09:11:30.150275 shaperglot-0.1.0/shaperglot/languages/boz_Latn.yaml
--rw-r--r--   0        0        0     6219 2023-05-22 09:11:30.150350 shaperglot-0.1.0/shaperglot/languages/bqc_Latn.yaml
--rw-r--r--   0        0        0     5433 2023-05-22 09:11:30.150433 shaperglot-0.1.0/shaperglot/languages/bqj_Latn.yaml
--rw-r--r--   0        0        0     7402 2023-05-22 09:11:30.150519 shaperglot-0.1.0/shaperglot/languages/bqp_Latn.yaml
--rw-r--r--   0        0        0     4926 2023-05-22 09:11:30.150605 shaperglot-0.1.0/shaperglot/languages/bsc_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.150670 shaperglot-0.1.0/shaperglot/languages/bsj_Latn.yaml
--rw-r--r--   0        0        0     4419 2023-05-22 09:11:30.150735 shaperglot-0.1.0/shaperglot/languages/bsp_Latn.yaml
--rw-r--r--   0        0        0     5036 2023-05-22 09:11:30.150818 shaperglot-0.1.0/shaperglot/languages/bsq_Latn.yaml
--rw-r--r--   0        0        0     8582 2023-05-22 09:11:30.150885 shaperglot-0.1.0/shaperglot/languages/btt_Latn.yaml
--rw-r--r--   0        0        0     7283 2023-05-22 09:11:30.150955 shaperglot-0.1.0/shaperglot/languages/bud_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.151026 shaperglot-0.1.0/shaperglot/languages/bus_Latn.yaml
--rw-r--r--   0        0        0     5033 2023-05-22 09:11:30.151094 shaperglot-0.1.0/shaperglot/languages/buu_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.151155 shaperglot-0.1.0/shaperglot/languages/bwr_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.151225 shaperglot-0.1.0/shaperglot/languages/byn_Latn.yaml
--rw-r--r--   0        0        0     6047 2023-05-22 09:11:30.151287 shaperglot-0.1.0/shaperglot/languages/bys_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.151350 shaperglot-0.1.0/shaperglot/languages/bza_Latn.yaml
--rw-r--r--   0        0        0     4917 2023-05-22 09:11:30.151422 shaperglot-0.1.0/shaperglot/languages/bzw_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.151480 shaperglot-0.1.0/shaperglot/languages/cbj_Latn.yaml
--rw-r--r--   0        0        0     5549 2023-05-22 09:11:30.151589 shaperglot-0.1.0/shaperglot/languages/cdr_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.151666 shaperglot-0.1.0/shaperglot/languages/cfa_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.151739 shaperglot-0.1.0/shaperglot/languages/cgg_Latn.yaml
--rw-r--r--   0        0        0     5878 2023-05-22 09:11:30.151841 shaperglot-0.1.0/shaperglot/languages/ckl_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.151910 shaperglot-0.1.0/shaperglot/languages/cko_Latn.yaml
--rw-r--r--   0        0        0     6554 2023-05-22 09:11:30.151982 shaperglot-0.1.0/shaperglot/languages/cky_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.152059 shaperglot-0.1.0/shaperglot/languages/cla_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.152128 shaperglot-0.1.0/shaperglot/languages/cme_Latn.yaml
--rw-r--r--   0        0        0     4594 2023-05-22 09:11:30.152194 shaperglot-0.1.0/shaperglot/languages/csk_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.152276 shaperglot-0.1.0/shaperglot/languages/cwe_Latn.yaml
--rw-r--r--   0        0        0     4419 2023-05-22 09:11:30.152379 shaperglot-0.1.0/shaperglot/languages/daa_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.152456 shaperglot-0.1.0/shaperglot/languages/dav_Latn.yaml
--rw-r--r--   0        0        0     6216 2023-05-22 09:11:30.152522 shaperglot-0.1.0/shaperglot/languages/dbd_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.152593 shaperglot-0.1.0/shaperglot/languages/dbq_Latn.yaml
--rw-r--r--   0        0        0     4526 2023-05-22 09:11:30.152669 shaperglot-0.1.0/shaperglot/languages/dgh_Latn.yaml
--rw-r--r--   0        0        0     6266 2023-05-22 09:11:30.152738 shaperglot-0.1.0/shaperglot/languages/dgi_Latn.yaml
--rw-r--r--   0        0        0     4882 2023-05-22 09:11:30.152807 shaperglot-0.1.0/shaperglot/languages/did_Latn.yaml
--rw-r--r--   0        0        0     5593 2023-05-22 09:11:30.152876 shaperglot-0.1.0/shaperglot/languages/dje_Latn.yaml
--rw-r--r--   0        0        0       91 2023-05-22 09:11:30.152946 shaperglot-0.1.0/shaperglot/languages/dnj_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.153014 shaperglot-0.1.0/shaperglot/languages/dop_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.153089 shaperglot-0.1.0/shaperglot/languages/dow_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.153152 shaperglot-0.1.0/shaperglot/languages/dri_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.153218 shaperglot-0.1.0/shaperglot/languages/dts_Latn.yaml
--rw-r--r--   0        0        0     6462 2023-05-22 09:11:30.153474 shaperglot-0.1.0/shaperglot/languages/dua_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.153556 shaperglot-0.1.0/shaperglot/languages/dug_Latn.yaml
--rw-r--r--   0        0        0     4191 2023-05-22 09:11:30.153626 shaperglot-0.1.0/shaperglot/languages/dwr_Latn.yaml
--rw-r--r--   0        0        0     4582 2023-05-22 09:11:30.153691 shaperglot-0.1.0/shaperglot/languages/dyi_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.153760 shaperglot-0.1.0/shaperglot/languages/dyo_Latn.yaml
--rw-r--r--   0        0        0     4751 2023-05-22 09:11:30.153831 shaperglot-0.1.0/shaperglot/languages/dyu_Latn.yaml
--rw-r--r--   0        0        0     5596 2023-05-22 09:11:30.153904 shaperglot-0.1.0/shaperglot/languages/dzg_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.153972 shaperglot-0.1.0/shaperglot/languages/ebu_Latn.yaml
--rw-r--r--   0        0        0    12275 2023-05-22 09:11:30.154092 shaperglot-0.1.0/shaperglot/languages/ee_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.154169 shaperglot-0.1.0/shaperglot/languages/ekm_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.154239 shaperglot-0.1.0/shaperglot/languages/ema_Latn.yaml
--rw-r--r--   0        0        0     6228 2023-05-22 09:11:30.154308 shaperglot-0.1.0/shaperglot/languages/enn_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.154384 shaperglot-0.1.0/shaperglot/languages/etu_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.154448 shaperglot-0.1.0/shaperglot/languages/etx_Latn.yaml
--rw-r--r--   0        0        0     9157 2023-05-22 09:11:30.154557 shaperglot-0.1.0/shaperglot/languages/ewo_Latn.yaml
--rw-r--r--   0        0        0     4713 2023-05-22 09:11:30.154626 shaperglot-0.1.0/shaperglot/languages/eza_Latn.yaml
--rw-r--r--   0        0        0     4754 2023-05-22 09:11:30.154690 shaperglot-0.1.0/shaperglot/languages/ffm_Latn.yaml
--rw-r--r--   0        0        0     4191 2023-05-22 09:11:30.154753 shaperglot-0.1.0/shaperglot/languages/flr_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.154818 shaperglot-0.1.0/shaperglot/languages/fmp_Latn.yaml
--rw-r--r--   0        0        0     6097 2023-05-22 09:11:30.154883 shaperglot-0.1.0/shaperglot/languages/fod_Latn.yaml
--rw-r--r--   0        0        0     6222 2023-05-22 09:11:30.154955 shaperglot-0.1.0/shaperglot/languages/fon_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.155018 shaperglot-0.1.0/shaperglot/languages/fub_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.155089 shaperglot-0.1.0/shaperglot/languages/fue_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.155152 shaperglot-0.1.0/shaperglot/languages/fuh_Latn.yaml
--rw-r--r--   0        0        0     4585 2023-05-22 09:11:30.155219 shaperglot-0.1.0/shaperglot/languages/fuq_Latn.yaml
--rw-r--r--   0        0        0     4197 2023-05-22 09:11:30.155291 shaperglot-0.1.0/shaperglot/languages/fuv_Latn.yaml
--rw-r--r--   0        0        0     5264 2023-05-22 09:11:30.155354 shaperglot-0.1.0/shaperglot/languages/gaa_Latn.yaml
--rw-r--r--   0        0        0     7909 2023-05-22 09:11:30.155423 shaperglot-0.1.0/shaperglot/languages/gby_Latn.yaml
--rw-r--r--   0        0        0     4751 2023-05-22 09:11:30.155488 shaperglot-0.1.0/shaperglot/languages/gde_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.155549 shaperglot-0.1.0/shaperglot/languages/gej_Latn.yaml
--rw-r--r--   0        0        0     6050 2023-05-22 09:11:30.155618 shaperglot-0.1.0/shaperglot/languages/gel_Latn.yaml
--rw-r--r--   0        0        0     8093 2023-05-22 09:11:30.155685 shaperglot-0.1.0/shaperglot/languages/gkn_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.155745 shaperglot-0.1.0/shaperglot/languages/gmm_Latn.yaml
--rw-r--r--   0        0        0     4191 2023-05-22 09:11:30.155808 shaperglot-0.1.0/shaperglot/languages/gmv_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.155871 shaperglot-0.1.0/shaperglot/languages/gnd_Latn.yaml
--rw-r--r--   0        0        0     6945 2023-05-22 09:11:30.155932 shaperglot-0.1.0/shaperglot/languages/gng_Latn.yaml
--rw-r--r--   0        0        0     5762 2023-05-22 09:11:30.155993 shaperglot-0.1.0/shaperglot/languages/god_Latn.yaml
--rw-r--r--   0        0        0     4191 2023-05-22 09:11:30.156059 shaperglot-0.1.0/shaperglot/languages/gof_Latn.yaml
--rw-r--r--   0        0        0     4206 2023-05-22 09:11:30.156125 shaperglot-0.1.0/shaperglot/languages/gqr_Latn.yaml
--rw-r--r--   0        0        0     5086 2023-05-22 09:11:30.156195 shaperglot-0.1.0/shaperglot/languages/gud_Latn.yaml
--rw-r--r--   0        0        0     4529 2023-05-22 09:11:30.156263 shaperglot-0.1.0/shaperglot/languages/guk_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.156332 shaperglot-0.1.0/shaperglot/languages/guw_Latn.yaml
--rw-r--r--   0        0        0     6435 2023-05-22 09:11:30.156399 shaperglot-0.1.0/shaperglot/languages/gux_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.156469 shaperglot-0.1.0/shaperglot/languages/guz_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.156534 shaperglot-0.1.0/shaperglot/languages/gyi_Latn.yaml
--rw-r--r--   0        0        0     7744 2023-05-22 09:11:30.156668 shaperglot-0.1.0/shaperglot/languages/ha_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.156731 shaperglot-0.1.0/shaperglot/languages/hag_Latn.yaml
--rw-r--r--   0        0        0     5033 2023-05-22 09:11:30.156800 shaperglot-0.1.0/shaperglot/languages/hia_Latn.yaml
--rw-r--r--   0        0        0     5540 2023-05-22 09:11:30.156868 shaperglot-0.1.0/shaperglot/languages/hig_Latn.yaml
--rw-r--r--   0        0        0     3877 2023-05-22 09:11:30.156932 shaperglot-0.1.0/shaperglot/languages/ibb_Latn.yaml
--rw-r--r--   0        0        0     7248 2023-05-22 09:11:30.156995 shaperglot-0.1.0/shaperglot/languages/iby_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.157056 shaperglot-0.1.0/shaperglot/languages/ica_Latn.yaml
--rw-r--r--   0        0        0     7230 2023-05-22 09:11:30.157118 shaperglot-0.1.0/shaperglot/languages/ich_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.157184 shaperglot-0.1.0/shaperglot/languages/idd_Latn.yaml
--rw-r--r--   0        0        0     8558 2023-05-22 09:11:30.157287 shaperglot-0.1.0/shaperglot/languages/ig_Latn.yaml
--rw-r--r--   0        0        0     8769 2023-05-22 09:11:30.157350 shaperglot-0.1.0/shaperglot/languages/igb_Latn.yaml
--rw-r--r--   0        0        0     6904 2023-05-22 09:11:30.157411 shaperglot-0.1.0/shaperglot/languages/ige_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.157470 shaperglot-0.1.0/shaperglot/languages/ijj_Latn.yaml
--rw-r--r--   0        0        0     5386 2023-05-22 09:11:30.157538 shaperglot-0.1.0/shaperglot/languages/ikk_Latn.yaml
--rw-r--r--   0        0        0     5890 2023-05-22 09:11:30.157595 shaperglot-0.1.0/shaperglot/languages/ikw_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.157653 shaperglot-0.1.0/shaperglot/languages/ikx_Latn.yaml
--rw-r--r--   0        0        0     4713 2023-05-22 09:11:30.157714 shaperglot-0.1.0/shaperglot/languages/iqw_Latn.yaml
--rw-r--r--   0        0        0     5540 2023-05-22 09:11:30.157774 shaperglot-0.1.0/shaperglot/languages/iri_Latn.yaml
--rw-r--r--   0        0        0     6047 2023-05-22 09:11:30.157831 shaperglot-0.1.0/shaperglot/languages/izr_Latn.yaml
--rw-r--r--   0        0        0     7417 2023-05-22 09:11:30.157887 shaperglot-0.1.0/shaperglot/languages/izz_Latn.yaml
--rw-r--r--   0        0        0     8075 2023-05-22 09:11:30.157945 shaperglot-0.1.0/shaperglot/languages/jab_Latn.yaml
--rw-r--r--   0        0        0     8591 2023-05-22 09:11:30.158026 shaperglot-0.1.0/shaperglot/languages/jbu_Latn.yaml
--rw-r--r--   0        0        0     7571 2023-05-22 09:11:30.158083 shaperglot-0.1.0/shaperglot/languages/jen_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.158147 shaperglot-0.1.0/shaperglot/languages/jgk_Latn.yaml
--rw-r--r--   0        0        0     7898 2023-05-22 09:11:30.158260 shaperglot-0.1.0/shaperglot/languages/jgo_Latn.yaml
--rw-r--r--   0        0        0     6557 2023-05-22 09:11:30.158323 shaperglot-0.1.0/shaperglot/languages/jib_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.158381 shaperglot-0.1.0/shaperglot/languages/jmc_Latn.yaml
--rw-r--r--   0        0        0     6065 2023-05-22 09:11:30.158453 shaperglot-0.1.0/shaperglot/languages/kab_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.158514 shaperglot-0.1.0/shaperglot/languages/kad_Latn.yaml
--rw-r--r--   0        0        0     5202 2023-05-22 09:11:30.158576 shaperglot-0.1.0/shaperglot/languages/kai_Latn.yaml
--rw-r--r--   0        0        0     4529 2023-05-22 09:11:30.158638 shaperglot-0.1.0/shaperglot/languages/kam_Latn.yaml
--rw-r--r--   0        0        0     4197 2023-05-22 09:11:30.158701 shaperglot-0.1.0/shaperglot/languages/kby_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.158773 shaperglot-0.1.0/shaperglot/languages/kdc_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.158838 shaperglot-0.1.0/shaperglot/languages/kde_Latn.yaml
--rw-r--r--   0        0        0     7336 2023-05-22 09:11:30.158900 shaperglot-0.1.0/shaperglot/languages/kdh_Latn.yaml
--rw-r--r--   0        0        0     4867 2023-05-22 09:11:30.158955 shaperglot-0.1.0/shaperglot/languages/kdl_Latn.yaml
--rw-r--r--   0        0        0     7787 2023-05-22 09:11:30.159012 shaperglot-0.1.0/shaperglot/languages/ken_Latn.yaml
--rw-r--r--   0        0        0     6385 2023-05-22 09:11:30.159071 shaperglot-0.1.0/shaperglot/languages/kez_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.159132 shaperglot-0.1.0/shaperglot/languages/kg_Latn.yaml
--rw-r--r--   0        0        0     5543 2023-05-22 09:11:30.159192 shaperglot-0.1.0/shaperglot/languages/khq_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.159250 shaperglot-0.1.0/shaperglot/languages/ki_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.159308 shaperglot-0.1.0/shaperglot/languages/kj_Latn.yaml
--rw-r--r--   0        0        0     8152 2023-05-22 09:11:30.159418 shaperglot-0.1.0/shaperglot/languages/kkj_Latn.yaml
--rw-r--r--   0        0        0     3361 2023-05-22 09:11:30.159476 shaperglot-0.1.0/shaperglot/languages/kmb_Latn.yaml
--rw-r--r--   0        0        0     4751 2023-05-22 09:11:30.159532 shaperglot-0.1.0/shaperglot/languages/kmy_Latn.yaml
--rw-r--r--   0        0        0     4707 2023-05-22 09:11:30.159590 shaperglot-0.1.0/shaperglot/languages/knf_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.159648 shaperglot-0.1.0/shaperglot/languages/knp_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.159708 shaperglot-0.1.0/shaperglot/languages/kpo_Latn.yaml
--rw-r--r--   0        0        0     5098 2023-05-22 09:11:30.159767 shaperglot-0.1.0/shaperglot/languages/kqp_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.159833 shaperglot-0.1.0/shaperglot/languages/krs_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.159899 shaperglot-0.1.0/shaperglot/languages/ksb_Latn.yaml
--rw-r--r--   0        0        0     6140 2023-05-22 09:11:30.160001 shaperglot-0.1.0/shaperglot/languages/ksf_Latn.yaml
--rw-r--r--   0        0        0     3696 2023-05-22 09:11:30.160064 shaperglot-0.1.0/shaperglot/languages/ksp_Latn.yaml
--rw-r--r--   0        0        0     4588 2023-05-22 09:11:30.160127 shaperglot-0.1.0/shaperglot/languages/ktj_Latn.yaml
--rw-r--r--   0        0        0     6388 2023-05-22 09:11:30.160186 shaperglot-0.1.0/shaperglot/languages/kub_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.160252 shaperglot-0.1.0/shaperglot/languages/kuj_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.160316 shaperglot-0.1.0/shaperglot/languages/kun_Latn.yaml
--rw-r--r--   0        0        0     4576 2023-05-22 09:11:30.160383 shaperglot-0.1.0/shaperglot/languages/kus_Latn.yaml
--rw-r--r--   0        0        0     4920 2023-05-22 09:11:30.160462 shaperglot-0.1.0/shaperglot/languages/kvf_Latn.yaml
--rw-r--r--   0        0        0     4920 2023-05-22 09:11:30.160534 shaperglot-0.1.0/shaperglot/languages/kye_Latn.yaml
--rw-r--r--   0        0        0     4920 2023-05-22 09:11:30.160602 shaperglot-0.1.0/shaperglot/languages/kyf_Latn.yaml
--rw-r--r--   0        0        0     4591 2023-05-22 09:11:30.160666 shaperglot-0.1.0/shaperglot/languages/kyq_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.160812 shaperglot-0.1.0/shaperglot/languages/kzr_Latn.yaml
--rw-r--r--   0        0        0     5540 2023-05-22 09:11:30.160886 shaperglot-0.1.0/shaperglot/languages/lag_Latn.yaml
--rw-r--r--   0        0        0     5928 2023-05-22 09:11:30.160948 shaperglot-0.1.0/shaperglot/languages/las_Latn.yaml
--rw-r--r--   0        0        0     5543 2023-05-22 09:11:30.161014 shaperglot-0.1.0/shaperglot/languages/ldb_Latn.yaml
--rw-r--r--   0        0        0     4698 2023-05-22 09:11:30.161083 shaperglot-0.1.0/shaperglot/languages/led_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.161150 shaperglot-0.1.0/shaperglot/languages/lee_Latn.yaml
--rw-r--r--   0        0        0     5925 2023-05-22 09:11:30.161219 shaperglot-0.1.0/shaperglot/languages/lem_Latn.yaml
--rw-r--r--   0        0        0     3699 2023-05-22 09:11:30.161284 shaperglot-0.1.0/shaperglot/languages/les_Latn.yaml
--rw-r--r--   0        0        0     4576 2023-05-22 09:11:30.161347 shaperglot-0.1.0/shaperglot/languages/lg_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.161411 shaperglot-0.1.0/shaperglot/languages/lgg_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.161475 shaperglot-0.1.0/shaperglot/languages/lig_Latn.yaml
--rw-r--r--   0        0        0     4369 2023-05-22 09:11:30.161555 shaperglot-0.1.0/shaperglot/languages/lip_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.161621 shaperglot-0.1.0/shaperglot/languages/lln_Latn.yaml
--rw-r--r--   0        0        0     7449 2023-05-22 09:11:30.161689 shaperglot-0.1.0/shaperglot/languages/lmp_Latn.yaml
--rw-r--r--   0        0        0     7152 2023-05-22 09:11:30.161910 shaperglot-0.1.0/shaperglot/languages/ln_Latn.yaml
--rw-r--r--   0        0        0     4698 2023-05-22 09:11:30.161975 shaperglot-0.1.0/shaperglot/languages/lnu_Latn.yaml
--rw-r--r--   0        0        0     4422 2023-05-22 09:11:30.162046 shaperglot-0.1.0/shaperglot/languages/log_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.162109 shaperglot-0.1.0/shaperglot/languages/lok_Latn.yaml
--rw-r--r--   0        0        0     4591 2023-05-22 09:11:30.162189 shaperglot-0.1.0/shaperglot/languages/loq_Latn.yaml
--rw-r--r--   0        0        0     5202 2023-05-22 09:11:30.162270 shaperglot-0.1.0/shaperglot/languages/lor_Latn.yaml
--rw-r--r--   0        0        0     3862 2023-05-22 09:11:30.162349 shaperglot-0.1.0/shaperglot/languages/loz_Latn.yaml
--rw-r--r--   0        0        0     6613 2023-05-22 09:11:30.162482 shaperglot-0.1.0/shaperglot/languages/lu_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.162552 shaperglot-0.1.0/shaperglot/languages/lua_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.162624 shaperglot-0.1.0/shaperglot/languages/luo_Latn.yaml
--rw-r--r--   0        0        0     3530 2023-05-22 09:11:30.162687 shaperglot-0.1.0/shaperglot/languages/lwo_Latn.yaml
--rw-r--r--   0        0        0     8812 2023-05-22 09:11:30.162795 shaperglot-0.1.0/shaperglot/languages/mas_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.162861 shaperglot-0.1.0/shaperglot/languages/maw_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.162925 shaperglot-0.1.0/shaperglot/languages/mbo_Latn.yaml
--rw-r--r--   0        0        0     7111 2023-05-22 09:11:30.162996 shaperglot-0.1.0/shaperglot/languages/mbu_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.163058 shaperglot-0.1.0/shaperglot/languages/mcp_Latn.yaml
--rw-r--r--   0        0        0     4745 2023-05-22 09:11:30.163165 shaperglot-0.1.0/shaperglot/languages/mcu_Latn.yaml
--rw-r--r--   0        0        0     8413 2023-05-22 09:11:30.163235 shaperglot-0.1.0/shaperglot/languages/mda_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.163306 shaperglot-0.1.0/shaperglot/languages/mdj_Latn.yaml
--rw-r--r--   0        0        0     3865 2023-05-22 09:11:30.163369 shaperglot-0.1.0/shaperglot/languages/men_Latn.yaml
--rw-r--r--   0        0        0     4926 2023-05-22 09:11:30.163433 shaperglot-0.1.0/shaperglot/languages/meq_Latn.yaml
--rw-r--r--   0        0        0     5857 2023-05-22 09:11:30.163498 shaperglot-0.1.0/shaperglot/languages/mer_Latn.yaml
--rw-r--r--   0        0        0     5264 2023-05-22 09:11:30.163566 shaperglot-0.1.0/shaperglot/languages/mfi_Latn.yaml
--rw-r--r--   0        0        0     6904 2023-05-22 09:11:30.163638 shaperglot-0.1.0/shaperglot/languages/mfn_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.163704 shaperglot-0.1.0/shaperglot/languages/mfo_Latn.yaml
--rw-r--r--   0        0        0     4754 2023-05-22 09:11:30.163869 shaperglot-0.1.0/shaperglot/languages/mfv_Latn.yaml
--rw-r--r--   0        0        0     6216 2023-05-22 09:11:30.163943 shaperglot-0.1.0/shaperglot/languages/mg_Latn.yaml
--rw-r--r--   0        0        0     5264 2023-05-22 09:11:30.164011 shaperglot-0.1.0/shaperglot/languages/mgc_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.164076 shaperglot-0.1.0/shaperglot/languages/mgh_Latn.yaml
--rw-r--r--   0        0        0     5955 2023-05-22 09:11:30.164294 shaperglot-0.1.0/shaperglot/languages/mgo_Latn.yaml
--rw-r--r--   0        0        0     4929 2023-05-22 09:11:30.164363 shaperglot-0.1.0/shaperglot/languages/mhi_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.164430 shaperglot-0.1.0/shaperglot/languages/mkl_Latn.yaml
--rw-r--r--   0        0        0     5878 2023-05-22 09:11:30.164525 shaperglot-0.1.0/shaperglot/languages/mlt_Latn.yaml
--rw-r--r--   0        0        0     5759 2023-05-22 09:11:30.164632 shaperglot-0.1.0/shaperglot/languages/mmu_Latn.yaml
--rw-r--r--   0        0        0     5083 2023-05-22 09:11:30.164704 shaperglot-0.1.0/shaperglot/languages/mnf_Latn.yaml
--rw-r--r--   0        0        0     5080 2023-05-22 09:11:30.164766 shaperglot-0.1.0/shaperglot/languages/moa_Latn.yaml
--rw-r--r--   0        0        0     4034 2023-05-22 09:11:30.164831 shaperglot-0.1.0/shaperglot/languages/mos_Latn.yaml
--rw-r--r--   0        0        0     6222 2023-05-22 09:11:30.164896 shaperglot-0.1.0/shaperglot/languages/mqb_Latn.yaml
--rw-r--r--   0        0        0     6898 2023-05-22 09:11:30.164969 shaperglot-0.1.0/shaperglot/languages/mql_Latn.yaml
--rw-r--r--   0        0        0     4200 2023-05-22 09:11:30.165035 shaperglot-0.1.0/shaperglot/languages/msc_Latn.yaml
--rw-r--r--   0        0        0     5931 2023-05-22 09:11:30.165098 shaperglot-0.1.0/shaperglot/languages/mua_Latn.yaml
--rw-r--r--   0        0        0     4704 2023-05-22 09:11:30.165160 shaperglot-0.1.0/shaperglot/languages/muh_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.165220 shaperglot-0.1.0/shaperglot/languages/mur_Latn.yaml
--rw-r--r--   0        0        0     6272 2023-05-22 09:11:30.165275 shaperglot-0.1.0/shaperglot/languages/muy_Latn.yaml
--rw-r--r--   0        0        0     6435 2023-05-22 09:11:30.165331 shaperglot-0.1.0/shaperglot/languages/myk_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.165393 shaperglot-0.1.0/shaperglot/languages/mym_Latn.yaml
--rw-r--r--   0        0        0     6047 2023-05-22 09:11:30.165451 shaperglot-0.1.0/shaperglot/languages/mzk_Latn.yaml
--rw-r--r--   0        0        0     9430 2023-05-22 09:11:30.165512 shaperglot-0.1.0/shaperglot/languages/mzm_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.165577 shaperglot-0.1.0/shaperglot/languages/mzw_Latn.yaml
--rw-r--r--   0        0        0     5033 2023-05-22 09:11:30.165635 shaperglot-0.1.0/shaperglot/languages/naq_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.165701 shaperglot-0.1.0/shaperglot/languages/nat_Latn.yaml
--rw-r--r--   0        0        0     4425 2023-05-22 09:11:30.165764 shaperglot-0.1.0/shaperglot/languages/naw_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.165826 shaperglot-0.1.0/shaperglot/languages/ncu_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.165888 shaperglot-0.1.0/shaperglot/languages/nd_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.166008 shaperglot-0.1.0/shaperglot/languages/ndj_Latn.yaml
--rw-r--r--   0        0        0     4422 2023-05-22 09:11:30.166077 shaperglot-0.1.0/shaperglot/languages/ndz_Latn.yaml
--rw-r--r--   0        0        0     4701 2023-05-22 09:11:30.166148 shaperglot-0.1.0/shaperglot/languages/neb_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.166223 shaperglot-0.1.0/shaperglot/languages/nfr_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.166289 shaperglot-0.1.0/shaperglot/languages/ng_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.166355 shaperglot-0.1.0/shaperglot/languages/nga_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.166415 shaperglot-0.1.0/shaperglot/languages/ngb_Latn.yaml
--rw-r--r--   0        0        0     4025 2023-05-22 09:11:30.166476 shaperglot-0.1.0/shaperglot/languages/ngp_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.166540 shaperglot-0.1.0/shaperglot/languages/nhb_Latn.yaml
--rw-r--r--   0        0        0     4081 2023-05-22 09:11:30.166605 shaperglot-0.1.0/shaperglot/languages/nhu_Latn.yaml
--rw-r--r--   0        0        0     9089 2023-05-22 09:11:30.166675 shaperglot-0.1.0/shaperglot/languages/nin_Latn.yaml
--rw-r--r--   0        0        0     5033 2023-05-22 09:11:30.166742 shaperglot-0.1.0/shaperglot/languages/niy_Latn.yaml
--rw-r--r--   0        0        0     6097 2023-05-22 09:11:30.166798 shaperglot-0.1.0/shaperglot/languages/nko_Latn.yaml
--rw-r--r--   0        0        0     9833 2023-05-22 09:11:30.166918 shaperglot-0.1.0/shaperglot/languages/nmg_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.166984 shaperglot-0.1.0/shaperglot/languages/nmz_Latn.yaml
--rw-r--r--   0        0        0     9163 2023-05-22 09:11:30.167104 shaperglot-0.1.0/shaperglot/languages/nnh_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.167171 shaperglot-0.1.0/shaperglot/languages/nnq_Latn.yaml
--rw-r--r--   0        0        0     5089 2023-05-22 09:11:30.167239 shaperglot-0.1.0/shaperglot/languages/nnw_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.167310 shaperglot-0.1.0/shaperglot/languages/nr_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.167370 shaperglot-0.1.0/shaperglot/languages/nrb_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.167432 shaperglot-0.1.0/shaperglot/languages/nso_Latn.yaml
--rw-r--r--   0        0        0     6400 2023-05-22 09:11:30.167498 shaperglot-0.1.0/shaperglot/languages/ntm_Latn.yaml
--rw-r--r--   0        0        0     5080 2023-05-22 09:11:30.167565 shaperglot-0.1.0/shaperglot/languages/ntr_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.167630 shaperglot-0.1.0/shaperglot/languages/nui_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.167688 shaperglot-0.1.0/shaperglot/languages/nup_Latn.yaml
--rw-r--r--   0        0        0     6083 2023-05-22 09:11:30.167802 shaperglot-0.1.0/shaperglot/languages/nus_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.167869 shaperglot-0.1.0/shaperglot/languages/nuv_Latn.yaml
--rw-r--r--   0        0        0     4867 2023-05-22 09:11:30.167934 shaperglot-0.1.0/shaperglot/languages/nwb_Latn.yaml
--rw-r--r--   0        0        0     4745 2023-05-22 09:11:30.167987 shaperglot-0.1.0/shaperglot/languages/ny_Latn.yaml
--rw-r--r--   0        0        0     3918 2023-05-22 09:11:30.168043 shaperglot-0.1.0/shaperglot/languages/nym_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.168098 shaperglot-0.1.0/shaperglot/languages/nyn_Latn.yaml
--rw-r--r--   0        0        0     4031 2023-05-22 09:11:30.168151 shaperglot-0.1.0/shaperglot/languages/nzi_Latn.yaml
--rw-r--r--   0        0        0     5881 2023-05-22 09:11:30.168214 shaperglot-0.1.0/shaperglot/languages/ogc_Latn.yaml
--rw-r--r--   0        0        0     5389 2023-05-22 09:11:30.168275 shaperglot-0.1.0/shaperglot/languages/okr_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.168328 shaperglot-0.1.0/shaperglot/languages/om_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.168386 shaperglot-0.1.0/shaperglot/languages/ozm_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.168441 shaperglot-0.1.0/shaperglot/languages/pbi_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.168501 shaperglot-0.1.0/shaperglot/languages/pil_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.168557 shaperglot-0.1.0/shaperglot/languages/pip_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.168613 shaperglot-0.1.0/shaperglot/languages/pko_Latn.yaml
--rw-r--r--   0        0        0     5374 2023-05-22 09:11:30.168677 shaperglot-0.1.0/shaperglot/languages/png_Latn.yaml
--rw-r--r--   0        0        0     4025 2023-05-22 09:11:30.168737 shaperglot-0.1.0/shaperglot/languages/poy_Latn.yaml
--rw-r--r--   0        0        0     4701 2023-05-22 09:11:30.168798 shaperglot-0.1.0/shaperglot/languages/pym_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.168862 shaperglot-0.1.0/shaperglot/languages/rel_Latn.yaml
--rw-r--r--   0        0        0     5033 2023-05-22 09:11:30.168921 shaperglot-0.1.0/shaperglot/languages/res_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.168977 shaperglot-0.1.0/shaperglot/languages/rn_Latn.yaml
--rw-r--r--   0        0        0      389 2022-10-19 11:48:51.019295 shaperglot-0.1.0/shaperglot/languages/ro_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.169034 shaperglot-0.1.0/shaperglot/languages/rof_Latn.yaml
--rw-r--r--   0        0        0     4244 2023-05-22 09:11:30.169097 shaperglot-0.1.0/shaperglot/languages/rub_Latn.yaml
--rw-r--r--   0        0        0     4025 2023-05-22 09:11:30.169154 shaperglot-0.1.0/shaperglot/languages/ruf_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.169215 shaperglot-0.1.0/shaperglot/languages/rw_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.169272 shaperglot-0.1.0/shaperglot/languages/rwk_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.169329 shaperglot-0.1.0/shaperglot/languages/saq_Latn.yaml
--rw-r--r--   0        0        0     4588 2023-05-22 09:11:30.169391 shaperglot-0.1.0/shaperglot/languages/sav_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.169453 shaperglot-0.1.0/shaperglot/languages/sba_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.169512 shaperglot-0.1.0/shaperglot/languages/sbp_Latn.yaml
--rw-r--r--   0        0        0     6554 2023-05-22 09:11:30.169574 shaperglot-0.1.0/shaperglot/languages/seh_Latn.yaml
--rw-r--r--   0        0        0     5593 2023-05-22 09:11:30.169633 shaperglot-0.1.0/shaperglot/languages/ses_Latn.yaml
--rw-r--r--   0        0        0     6216 2023-05-22 09:11:30.169695 shaperglot-0.1.0/shaperglot/languages/sg_Latn.yaml
--rw-r--r--   0        0        0     4360 2023-05-22 09:11:30.169757 shaperglot-0.1.0/shaperglot/languages/she_Latn.yaml
--rw-r--r--   0        0        0     5555 2023-05-22 09:11:30.169819 shaperglot-0.1.0/shaperglot/languages/shi_Latn.yaml
--rw-r--r--   0        0        0     6892 2023-05-22 09:11:30.169878 shaperglot-0.1.0/shaperglot/languages/shu_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.169941 shaperglot-0.1.0/shaperglot/languages/sig_Latn.yaml
--rw-r--r--   0        0        0     5086 2023-05-22 09:11:30.170007 shaperglot-0.1.0/shaperglot/languages/sil_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.170069 shaperglot-0.1.0/shaperglot/languages/sld_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.170129 shaperglot-0.1.0/shaperglot/languages/sn_Latn.yaml
--rw-r--r--   0        0        0     4025 2023-05-22 09:11:30.170194 shaperglot-0.1.0/shaperglot/languages/snk_Latn.yaml
--rw-r--r--   0        0        0     4541 2023-05-22 09:11:30.170258 shaperglot-0.1.0/shaperglot/languages/snw_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.170318 shaperglot-0.1.0/shaperglot/languages/so_Latn.yaml
--rw-r--r--   0        0        0     5759 2023-05-22 09:11:30.170379 shaperglot-0.1.0/shaperglot/languages/sok_Latn.yaml
--rw-r--r--   0        0        0     6782 2023-05-22 09:11:30.170440 shaperglot-0.1.0/shaperglot/languages/soy_Latn.yaml
--rw-r--r--   0        0        0     4751 2023-05-22 09:11:30.170505 shaperglot-0.1.0/shaperglot/languages/spp_Latn.yaml
--rw-r--r--   0        0        0     5427 2023-05-22 09:11:30.170572 shaperglot-0.1.0/shaperglot/languages/srr_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.170633 shaperglot-0.1.0/shaperglot/languages/ss_Latn.yaml
--rw-r--r--   0        0        0     5245 2023-05-22 09:11:30.170741 shaperglot-0.1.0/shaperglot/languages/st_Latn.yaml
--rw-r--r--   0        0        0     4194 2023-05-22 09:11:30.170805 shaperglot-0.1.0/shaperglot/languages/suk_Latn.yaml
--rw-r--r--   0        0        0     4529 2023-05-22 09:11:30.170867 shaperglot-0.1.0/shaperglot/languages/suq_Latn.yaml
--rw-r--r--   0        0        0     6554 2023-05-22 09:11:30.170925 shaperglot-0.1.0/shaperglot/languages/sur_Latn.yaml
--rw-r--r--   0        0        0     4034 2023-05-22 09:11:30.170985 shaperglot-0.1.0/shaperglot/languages/sus_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.171044 shaperglot-0.1.0/shaperglot/languages/sw_Latn.yaml
--rw-r--r--   0        0        0     4025 2023-05-22 09:11:30.171146 shaperglot-0.1.0/shaperglot/languages/swb_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.171218 shaperglot-0.1.0/shaperglot/languages/swc_Latn.yaml
--rw-r--r--   0        0        0     4025 2023-05-22 09:11:30.171283 shaperglot-0.1.0/shaperglot/languages/sxb_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.171346 shaperglot-0.1.0/shaperglot/languages/sxw_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.171405 shaperglot-0.1.0/shaperglot/languages/tal_Latn.yaml
--rw-r--r--   0        0        0     5724 2023-05-22 09:11:30.171470 shaperglot-0.1.0/shaperglot/languages/tan_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.171525 shaperglot-0.1.0/shaperglot/languages/ted_Latn.yaml
--rw-r--r--   0        0        0     4090 2023-05-22 09:11:30.171584 shaperglot-0.1.0/shaperglot/languages/tem_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.171652 shaperglot-0.1.0/shaperglot/languages/teo_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.171749 shaperglot-0.1.0/shaperglot/languages/tfi_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.171808 shaperglot-0.1.0/shaperglot/languages/tik_Latn.yaml
--rw-r--r--   0        0        0     4194 2023-05-22 09:11:30.171876 shaperglot-0.1.0/shaperglot/languages/tiv_Latn.yaml
--rw-r--r--   0        0        0     4191 2023-05-22 09:11:30.171929 shaperglot-0.1.0/shaperglot/languages/tke_Latn.yaml
--rw-r--r--   0        0        0     3693 2023-05-22 09:11:30.171981 shaperglot-0.1.0/shaperglot/languages/tlj_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.172032 shaperglot-0.1.0/shaperglot/languages/tn_Latn.yaml
--rw-r--r--   0        0        0     4926 2023-05-22 09:11:30.172084 shaperglot-0.1.0/shaperglot/languages/tnr_Latn.yaml
--rw-r--r--   0        0        0     4932 2023-05-22 09:11:30.172140 shaperglot-0.1.0/shaperglot/languages/tod_Latn.yaml
--rw-r--r--   0        0        0     4576 2023-05-22 09:11:30.172193 shaperglot-0.1.0/shaperglot/languages/toq_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.172249 shaperglot-0.1.0/shaperglot/languages/tpm_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.172303 shaperglot-0.1.0/shaperglot/languages/ts_Latn.yaml
--rw-r--r--   0        0        0     4867 2023-05-22 09:11:30.172362 shaperglot-0.1.0/shaperglot/languages/tsw_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.172414 shaperglot-0.1.0/shaperglot/languages/ttr_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.172466 shaperglot-0.1.0/shaperglot/languages/tul_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.172518 shaperglot-0.1.0/shaperglot/languages/tum_Latn.yaml
--rw-r--r--   0        0        0     5596 2023-05-22 09:11:30.172569 shaperglot-0.1.0/shaperglot/languages/tuq_Latn.yaml
--rw-r--r--   0        0        0     5371 2023-05-22 09:11:30.172623 shaperglot-0.1.0/shaperglot/languages/tvd_Latn.yaml
--rw-r--r--   0        0        0     5759 2023-05-22 09:11:30.172680 shaperglot-0.1.0/shaperglot/languages/tvu_Latn.yaml
--rw-r--r--   0        0        0     5593 2023-05-22 09:11:30.172740 shaperglot-0.1.0/shaperglot/languages/twq_Latn.yaml
--rw-r--r--   0        0        0     5555 2023-05-22 09:11:30.172805 shaperglot-0.1.0/shaperglot/languages/tzm_Latn.yaml
--rw-r--r--   0        0        0     4707 2023-05-22 09:11:30.172865 shaperglot-0.1.0/shaperglot/languages/umb_Latn.yaml
--rw-r--r--   0        0        0     6216 2023-05-22 09:11:30.172923 shaperglot-0.1.0/shaperglot/languages/uth_Latn.yaml
--rw-r--r--   0        0        0     4695 2023-05-22 09:11:30.172979 shaperglot-0.1.0/shaperglot/languages/utr_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.173031 shaperglot-0.1.0/shaperglot/languages/vag_Latn.yaml
--rw-r--r--   0        0        0     7173 2023-05-22 09:11:30.173128 shaperglot-0.1.0/shaperglot/languages/vai_Latn.yaml
--rw-r--r--   0        0        0     4719 2023-05-22 09:11:30.173190 shaperglot-0.1.0/shaperglot/languages/ve_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.173246 shaperglot-0.1.0/shaperglot/languages/vid_Latn.yaml
--rw-r--r--   0        0        0     5202 2023-05-22 09:11:30.173303 shaperglot-0.1.0/shaperglot/languages/vmw_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.173359 shaperglot-0.1.0/shaperglot/languages/vun_Latn.yaml
--rw-r--r--   0        0        0     5421 2023-05-22 09:11:30.173414 shaperglot-0.1.0/shaperglot/languages/vut_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.173472 shaperglot-0.1.0/shaperglot/languages/wal_Latn.yaml
--rw-r--r--   0        0        0     4748 2023-05-22 09:11:30.173526 shaperglot-0.1.0/shaperglot/languages/wan_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.173588 shaperglot-0.1.0/shaperglot/languages/wci_Latn.yaml
--rw-r--r--   0        0        0     4698 2023-05-22 09:11:30.173649 shaperglot-0.1.0/shaperglot/languages/wib_Latn.yaml
--rw-r--r--   0        0        0     5202 2023-05-22 09:11:30.173712 shaperglot-0.1.0/shaperglot/languages/wja_Latn.yaml
--rw-r--r--   0        0        0     4864 2023-05-22 09:11:30.173774 shaperglot-0.1.0/shaperglot/languages/wji_Latn.yaml
--rw-r--r--   0        0        0     4532 2023-05-22 09:11:30.173838 shaperglot-0.1.0/shaperglot/languages/wmw_Latn.yaml
--rw-r--r--   0        0        0     5590 2023-05-22 09:11:30.173900 shaperglot-0.1.0/shaperglot/languages/wo_Latn.yaml
--rw-r--r--   0        0        0     4701 2023-05-22 09:11:30.173961 shaperglot-0.1.0/shaperglot/languages/wob_Latn.yaml
--rw-r--r--   0        0        0     4591 2023-05-22 09:11:30.174020 shaperglot-0.1.0/shaperglot/languages/xed_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.174081 shaperglot-0.1.0/shaperglot/languages/xh_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.174141 shaperglot-0.1.0/shaperglot/languages/xog_Latn.yaml
--rw-r--r--   0        0        0     4911 2023-05-22 09:11:30.174200 shaperglot-0.1.0/shaperglot/languages/xon_Latn.yaml
--rw-r--r--   0        0        0     4914 2023-05-22 09:11:30.174260 shaperglot-0.1.0/shaperglot/languages/xrb_Latn.yaml
--rw-r--r--   0        0        0     5095 2023-05-22 09:11:30.174321 shaperglot-0.1.0/shaperglot/languages/xuo_Latn.yaml
--rw-r--r--   0        0        0     5252 2023-05-22 09:11:30.174376 shaperglot-0.1.0/shaperglot/languages/xwe_Latn.yaml
--rw-r--r--   0        0        0     4034 2023-05-22 09:11:30.174429 shaperglot-0.1.0/shaperglot/languages/yal_Latn.yaml
--rw-r--r--   0        0        0     4751 2023-05-22 09:11:30.174481 shaperglot-0.1.0/shaperglot/languages/yam_Latn.yaml
--rw-r--r--   0        0        0     3530 2023-05-22 09:11:30.174537 shaperglot-0.1.0/shaperglot/languages/yao_Latn.yaml
--rw-r--r--   0        0        0     5593 2023-05-22 09:11:30.174595 shaperglot-0.1.0/shaperglot/languages/yas_Latn.yaml
--rw-r--r--   0        0        0     5928 2023-05-22 09:11:30.174654 shaperglot-0.1.0/shaperglot/languages/yat_Latn.yaml
--rw-r--r--   0        0        0     8691 2023-05-22 09:11:30.174741 shaperglot-0.1.0/shaperglot/languages/yav_Latn.yaml
--rw-r--r--   0        0        0     5039 2023-05-22 09:11:30.174794 shaperglot-0.1.0/shaperglot/languages/yay_Latn.yaml
--rw-r--r--   0        0        0     5380 2023-05-22 09:11:30.174847 shaperglot-0.1.0/shaperglot/languages/yaz_Latn.yaml
--rw-r--r--   0        0        0     5540 2023-05-22 09:11:30.174906 shaperglot-0.1.0/shaperglot/languages/yba_Latn.yaml
--rw-r--r--   0        0        0     8078 2023-05-22 09:11:30.174957 shaperglot-0.1.0/shaperglot/languages/yer_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.175009 shaperglot-0.1.0/shaperglot/languages/yko_Latn.yaml
--rw-r--r--   0        0        0     7329 2023-05-22 09:11:30.175109 shaperglot-0.1.0/shaperglot/languages/yo_Latn.yaml
--rw-r--r--   0        0        0     4369 2023-05-22 09:11:30.175163 shaperglot-0.1.0/shaperglot/languages/yre_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.175215 shaperglot-0.1.0/shaperglot/languages/zay_Latn.yaml
--rw-r--r--   0        0        0     3859 2023-05-22 09:11:30.175270 shaperglot-0.1.0/shaperglot/languages/ziw_Latn.yaml
--rw-r--r--   0        0        0     4357 2023-05-22 09:11:30.175366 shaperglot-0.1.0/shaperglot/languages/zne_Latn.yaml
--rw-r--r--   0        0        0    10779 2023-05-22 09:11:30.175417 shaperglot-0.1.0/shaperglot/languages/zul_Latn.yaml
--rw-r--r--   0        0        0     2787 2022-11-04 12:29:25.793897 shaperglot-0.1.0/shaperglot/languages.py
--rw-r--r--   0        0        0     1645 2022-11-04 21:12:35.680551 shaperglot-0.1.0/shaperglot/reporter.py
--rw-r--r--   0        0        0     7922 1970-01-01 00:00:00.000000 shaperglot-0.1.0/setup.py
--rw-r--r--   0        0        0     8048 1970-01-01 00:00:00.000000 shaperglot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-08-17 10:00:19.663936 shaperglot-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     6768 2023-06-13 10:57:30.661338 shaperglot-0.2.0/README.md
+-rw-r--r--   0        0        0     1563 2023-06-13 10:57:47.706363 shaperglot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      185 2021-08-17 09:57:59.002337 shaperglot-0.2.0/shaperglot/__init__.py
+-rw-r--r--   0        0        0      144 2021-08-17 10:00:59.205150 shaperglot-0.2.0/shaperglot/__main__.py
+-rw-r--r--   0        0        0     2245 2023-06-13 10:57:30.663105 shaperglot-0.2.0/shaperglot/checker.py
+-rw-r--r--   0        0        0      431 2023-06-13 10:57:30.663264 shaperglot-0.2.0/shaperglot/checks/__init__.py
+-rw-r--r--   0        0        0     3048 2023-06-13 10:57:30.663420 shaperglot-0.2.0/shaperglot/checks/common.py
+-rw-r--r--   0        0        0     3673 2023-06-13 10:57:30.663572 shaperglot-0.2.0/shaperglot/checks/no_orphaned_marks.py
+-rw-r--r--   0        0        0     2734 2023-06-13 10:57:30.663733 shaperglot-0.2.0/shaperglot/checks/orthographies.py
+-rw-r--r--   0        0        0     4183 2023-06-13 10:57:30.663882 shaperglot-0.2.0/shaperglot/checks/shaping_differs.py
+-rw-r--r--   0        0        0     2266 2023-06-13 10:57:30.663984 shaperglot-0.2.0/shaperglot/checks/unencoded_variants.py
+-rw-r--r--   0        0        0     6277 2023-06-13 10:57:30.664140 shaperglot-0.2.0/shaperglot/cli.py
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.664594 shaperglot-0.2.0/shaperglot/languages/aa_Latn.yaml
+-rw-r--r--   0        0        0     5033 2023-06-13 10:57:30.664729 shaperglot-0.2.0/shaperglot/languages/abi_Latn.yaml
+-rw-r--r--   0        0        0     3699 2023-06-13 10:57:30.664868 shaperglot-0.2.0/shaperglot/languages/abr_Latn.yaml
+-rw-r--r--   0        0        0     5086 2023-06-13 10:57:30.665001 shaperglot-0.2.0/shaperglot/languages/acd_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.665180 shaperglot-0.2.0/shaperglot/languages/ada_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.665292 shaperglot-0.2.0/shaperglot/languages/ade_Latn.yaml
+-rw-r--r--   0        0        0     5255 2023-06-13 10:57:30.665410 shaperglot-0.2.0/shaperglot/languages/adj_Latn.yaml
+-rw-r--r--   0        0        0     8271 2023-06-13 10:57:30.665598 shaperglot-0.2.0/shaperglot/languages/aeb_Latn.yaml
+-rw-r--r--   0        0        0     8582 2023-06-13 10:57:30.665906 shaperglot-0.2.0/shaperglot/languages/af_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.666104 shaperglot-0.2.0/shaperglot/languages/agc_Latn.yaml
+-rw-r--r--   0        0        0     8886 2023-06-13 10:57:30.666250 shaperglot-0.2.0/shaperglot/languages/agq_Latn.yaml
+-rw-r--r--   0        0        0     5202 2023-06-13 10:57:30.666346 shaperglot-0.2.0/shaperglot/languages/aha_Latn.yaml
+-rw-r--r--   0        0        0     6773 2023-06-13 10:57:30.666507 shaperglot-0.2.0/shaperglot/languages/ahl_Latn.yaml
+-rw-r--r--   0        0        0     6438 2023-06-13 10:57:30.666654 shaperglot-0.2.0/shaperglot/languages/ahs_Latn.yaml
+-rw-r--r--   0        0        0      193 2022-11-02 15:26:07.712468 shaperglot-0.2.0/shaperglot/languages/ajg_Latn.yaml
+-rw-r--r--   0        0        0     4529 2023-06-13 10:57:30.666787 shaperglot-0.2.0/shaperglot/languages/ak_Latn.yaml
+-rw-r--r--   0        0        0     4876 2023-06-13 10:57:30.666880 shaperglot-0.2.0/shaperglot/languages/akp_Latn.yaml
+-rw-r--r--   0        0        0     4526 2023-06-13 10:57:30.666975 shaperglot-0.2.0/shaperglot/languages/ala_Latn.yaml
+-rw-r--r--   0        0        0     7239 2023-06-13 10:57:30.667125 shaperglot-0.2.0/shaperglot/languages/anc_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.667236 shaperglot-0.2.0/shaperglot/languages/ank_Latn.yaml
+-rw-r--r--   0        0        0     6228 2023-06-13 10:57:30.667344 shaperglot-0.2.0/shaperglot/languages/ann_Latn.yaml
+-rw-r--r--   0        0        0     4416 2023-06-13 10:57:30.667484 shaperglot-0.2.0/shaperglot/languages/anv_Latn.yaml
+-rw-r--r--   0        0        0     5202 2023-06-13 10:57:30.667588 shaperglot-0.2.0/shaperglot/languages/any_Latn.yaml
+-rw-r--r--   0        0        0     5217 2023-06-13 10:57:30.667679 shaperglot-0.2.0/shaperglot/languages/apd_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.667788 shaperglot-0.2.0/shaperglot/languages/asa_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.667951 shaperglot-0.2.0/shaperglot/languages/asg_Latn.yaml
+-rw-r--r--   0        0        0     5039 2023-06-13 10:57:30.668050 shaperglot-0.2.0/shaperglot/languages/atg_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.668185 shaperglot-0.2.0/shaperglot/languages/avn_Latn.yaml
+-rw-r--r--   0        0        0     4923 2023-06-13 10:57:30.668293 shaperglot-0.2.0/shaperglot/languages/avu_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.668390 shaperglot-0.2.0/shaperglot/languages/awo_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.668498 shaperglot-0.2.0/shaperglot/languages/ayb_Latn.yaml
+-rw-r--r--   0        0        0    10210 2023-06-13 10:57:30.668633 shaperglot-0.2.0/shaperglot/languages/bas_Latn.yaml
+-rw-r--r--   0        0        0     5424 2023-06-13 10:57:30.668823 shaperglot-0.2.0/shaperglot/languages/bav_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.668929 shaperglot-0.2.0/shaperglot/languages/bbp_Latn.yaml
+-rw-r--r--   0        0        0     4197 2023-06-13 10:57:30.669040 shaperglot-0.2.0/shaperglot/languages/bci_Latn.yaml
+-rw-r--r--   0        0        0     7915 2023-06-13 10:57:30.669133 shaperglot-0.2.0/shaperglot/languages/bcn_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.669237 shaperglot-0.2.0/shaperglot/languages/bcq_Latn.yaml
+-rw-r--r--   0        0        0     4591 2023-06-13 10:57:30.669357 shaperglot-0.2.0/shaperglot/languages/bcw_Latn.yaml
+-rw-r--r--   0        0        0     5205 2023-06-13 10:57:30.669449 shaperglot-0.2.0/shaperglot/languages/bcy_Latn.yaml
+-rw-r--r--   0        0        0     5060 2023-06-13 10:57:30.669552 shaperglot-0.2.0/shaperglot/languages/bdh_Latn.yaml
+-rw-r--r--   0        0        0     4526 2023-06-13 10:57:30.669653 shaperglot-0.2.0/shaperglot/languages/beh_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.669749 shaperglot-0.2.0/shaperglot/languages/bej_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.669856 shaperglot-0.2.0/shaperglot/languages/bem_Latn.yaml
+-rw-r--r--   0        0        0     5543 2023-06-13 10:57:30.669955 shaperglot-0.2.0/shaperglot/languages/bet_Latn.yaml
+-rw-r--r--   0        0        0     5756 2023-06-13 10:57:30.670049 shaperglot-0.2.0/shaperglot/languages/bex_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.670149 shaperglot-0.2.0/shaperglot/languages/bez_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.670250 shaperglot-0.2.0/shaperglot/languages/bhy_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.670348 shaperglot-0.2.0/shaperglot/languages/bib_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.670438 shaperglot-0.2.0/shaperglot/languages/bim_Latn.yaml
+-rw-r--r--   0        0        0     5220 2023-06-13 10:57:30.670534 shaperglot-0.2.0/shaperglot/languages/bin_Latn.yaml
+-rw-r--r--   0        0        0     4754 2023-06-13 10:57:30.670638 shaperglot-0.2.0/shaperglot/languages/biv_Latn.yaml
+-rw-r--r--   0        0        0     4206 2023-06-13 10:57:30.670735 shaperglot-0.2.0/shaperglot/languages/bjv_Latn.yaml
+-rw-r--r--   0        0        0     5033 2023-06-13 10:57:30.670834 shaperglot-0.2.0/shaperglot/languages/bkc_Latn.yaml
+-rw-r--r--   0        0        0     8247 2023-06-13 10:57:30.670926 shaperglot-0.2.0/shaperglot/languages/bkv_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.671023 shaperglot-0.2.0/shaperglot/languages/blo_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.671128 shaperglot-0.2.0/shaperglot/languages/bm_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.671255 shaperglot-0.2.0/shaperglot/languages/bng_Latn.yaml
+-rw-r--r--   0        0        0     4360 2023-06-13 10:57:30.671473 shaperglot-0.2.0/shaperglot/languages/bnm_Latn.yaml
+-rw-r--r--   0        0        0     5748 2023-06-13 10:57:30.671673 shaperglot-0.2.0/shaperglot/languages/bom_Latn.yaml
+-rw-r--r--   0        0        0     5045 2023-06-13 10:57:30.671832 shaperglot-0.2.0/shaperglot/languages/bov_Latn.yaml
+-rw-r--r--   0        0        0     4876 2023-06-13 10:57:30.671948 shaperglot-0.2.0/shaperglot/languages/box_Latn.yaml
+-rw-r--r--   0        0        0     4917 2023-06-13 10:57:30.672041 shaperglot-0.2.0/shaperglot/languages/boz_Latn.yaml
+-rw-r--r--   0        0        0     6219 2023-06-13 10:57:30.672132 shaperglot-0.2.0/shaperglot/languages/bqc_Latn.yaml
+-rw-r--r--   0        0        0     5433 2023-06-13 10:57:30.672222 shaperglot-0.2.0/shaperglot/languages/bqj_Latn.yaml
+-rw-r--r--   0        0        0     7402 2023-06-13 10:57:30.672320 shaperglot-0.2.0/shaperglot/languages/bqp_Latn.yaml
+-rw-r--r--   0        0        0     4926 2023-06-13 10:57:30.672417 shaperglot-0.2.0/shaperglot/languages/bsc_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.672576 shaperglot-0.2.0/shaperglot/languages/bsj_Latn.yaml
+-rw-r--r--   0        0        0     4419 2023-06-13 10:57:30.672786 shaperglot-0.2.0/shaperglot/languages/bsp_Latn.yaml
+-rw-r--r--   0        0        0     5036 2023-06-13 10:57:30.672943 shaperglot-0.2.0/shaperglot/languages/bsq_Latn.yaml
+-rw-r--r--   0        0        0     8582 2023-06-13 10:57:30.673079 shaperglot-0.2.0/shaperglot/languages/btt_Latn.yaml
+-rw-r--r--   0        0        0     7283 2023-06-13 10:57:30.673296 shaperglot-0.2.0/shaperglot/languages/bud_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.673478 shaperglot-0.2.0/shaperglot/languages/bus_Latn.yaml
+-rw-r--r--   0        0        0     5033 2023-06-13 10:57:30.673627 shaperglot-0.2.0/shaperglot/languages/buu_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.673761 shaperglot-0.2.0/shaperglot/languages/bwr_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.673941 shaperglot-0.2.0/shaperglot/languages/byn_Latn.yaml
+-rw-r--r--   0        0        0     6047 2023-06-13 10:57:30.674098 shaperglot-0.2.0/shaperglot/languages/bys_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.674275 shaperglot-0.2.0/shaperglot/languages/bza_Latn.yaml
+-rw-r--r--   0        0        0     4917 2023-06-13 10:57:30.674438 shaperglot-0.2.0/shaperglot/languages/bzw_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.674582 shaperglot-0.2.0/shaperglot/languages/cbj_Latn.yaml
+-rw-r--r--   0        0        0     5549 2023-06-13 10:57:30.674762 shaperglot-0.2.0/shaperglot/languages/cdr_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.674929 shaperglot-0.2.0/shaperglot/languages/cfa_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.675075 shaperglot-0.2.0/shaperglot/languages/cgg_Latn.yaml
+-rw-r--r--   0        0        0     5878 2023-06-13 10:57:30.675219 shaperglot-0.2.0/shaperglot/languages/ckl_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.675356 shaperglot-0.2.0/shaperglot/languages/cko_Latn.yaml
+-rw-r--r--   0        0        0     6554 2023-06-13 10:57:30.675489 shaperglot-0.2.0/shaperglot/languages/cky_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.675617 shaperglot-0.2.0/shaperglot/languages/cla_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.675747 shaperglot-0.2.0/shaperglot/languages/cme_Latn.yaml
+-rw-r--r--   0        0        0     4594 2023-06-13 10:57:30.675883 shaperglot-0.2.0/shaperglot/languages/csk_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.676011 shaperglot-0.2.0/shaperglot/languages/cwe_Latn.yaml
+-rw-r--r--   0        0        0     4419 2023-06-13 10:57:30.676139 shaperglot-0.2.0/shaperglot/languages/daa_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.676269 shaperglot-0.2.0/shaperglot/languages/dav_Latn.yaml
+-rw-r--r--   0        0        0     6216 2023-06-13 10:57:30.676398 shaperglot-0.2.0/shaperglot/languages/dbd_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.676579 shaperglot-0.2.0/shaperglot/languages/dbq_Latn.yaml
+-rw-r--r--   0        0        0     4526 2023-06-13 10:57:30.676786 shaperglot-0.2.0/shaperglot/languages/dgh_Latn.yaml
+-rw-r--r--   0        0        0     6266 2023-06-13 10:57:30.676925 shaperglot-0.2.0/shaperglot/languages/dgi_Latn.yaml
+-rw-r--r--   0        0        0     4882 2023-06-13 10:57:30.677055 shaperglot-0.2.0/shaperglot/languages/did_Latn.yaml
+-rw-r--r--   0        0        0     5593 2023-06-13 10:57:30.677215 shaperglot-0.2.0/shaperglot/languages/dje_Latn.yaml
+-rw-r--r--   0        0        0       91 2023-06-13 10:57:30.677357 shaperglot-0.2.0/shaperglot/languages/dnj_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.677553 shaperglot-0.2.0/shaperglot/languages/dop_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.677692 shaperglot-0.2.0/shaperglot/languages/dow_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.677820 shaperglot-0.2.0/shaperglot/languages/dri_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.677957 shaperglot-0.2.0/shaperglot/languages/dts_Latn.yaml
+-rw-r--r--   0        0        0     6462 2023-06-13 10:57:30.678096 shaperglot-0.2.0/shaperglot/languages/dua_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.678231 shaperglot-0.2.0/shaperglot/languages/dug_Latn.yaml
+-rw-r--r--   0        0        0     4191 2023-06-13 10:57:30.678374 shaperglot-0.2.0/shaperglot/languages/dwr_Latn.yaml
+-rw-r--r--   0        0        0     4582 2023-06-13 10:57:30.678515 shaperglot-0.2.0/shaperglot/languages/dyi_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.678616 shaperglot-0.2.0/shaperglot/languages/dyo_Latn.yaml
+-rw-r--r--   0        0        0     4751 2023-06-13 10:57:30.678727 shaperglot-0.2.0/shaperglot/languages/dyu_Latn.yaml
+-rw-r--r--   0        0        0     5596 2023-06-13 10:57:30.678828 shaperglot-0.2.0/shaperglot/languages/dzg_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.678940 shaperglot-0.2.0/shaperglot/languages/ebu_Latn.yaml
+-rw-r--r--   0        0        0    12275 2023-06-13 10:57:30.679039 shaperglot-0.2.0/shaperglot/languages/ee_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.679140 shaperglot-0.2.0/shaperglot/languages/ekm_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.679231 shaperglot-0.2.0/shaperglot/languages/ema_Latn.yaml
+-rw-r--r--   0        0        0     6228 2023-06-13 10:57:30.679316 shaperglot-0.2.0/shaperglot/languages/enn_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.679416 shaperglot-0.2.0/shaperglot/languages/etu_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.679521 shaperglot-0.2.0/shaperglot/languages/etx_Latn.yaml
+-rw-r--r--   0        0        0     9157 2023-06-13 10:57:30.679655 shaperglot-0.2.0/shaperglot/languages/ewo_Latn.yaml
+-rw-r--r--   0        0        0     4713 2023-06-13 10:57:30.679781 shaperglot-0.2.0/shaperglot/languages/eza_Latn.yaml
+-rw-r--r--   0        0        0     4754 2023-06-13 10:57:30.679888 shaperglot-0.2.0/shaperglot/languages/ffm_Latn.yaml
+-rw-r--r--   0        0        0     4191 2023-06-13 10:57:30.679983 shaperglot-0.2.0/shaperglot/languages/flr_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.680080 shaperglot-0.2.0/shaperglot/languages/fmp_Latn.yaml
+-rw-r--r--   0        0        0     6097 2023-06-13 10:57:30.680175 shaperglot-0.2.0/shaperglot/languages/fod_Latn.yaml
+-rw-r--r--   0        0        0     6222 2023-06-13 10:57:30.680283 shaperglot-0.2.0/shaperglot/languages/fon_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.680378 shaperglot-0.2.0/shaperglot/languages/fub_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.680469 shaperglot-0.2.0/shaperglot/languages/fue_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.680602 shaperglot-0.2.0/shaperglot/languages/fuh_Latn.yaml
+-rw-r--r--   0        0        0     4585 2023-06-13 10:57:30.680826 shaperglot-0.2.0/shaperglot/languages/fuq_Latn.yaml
+-rw-r--r--   0        0        0     4197 2023-06-13 10:57:30.681031 shaperglot-0.2.0/shaperglot/languages/fuv_Latn.yaml
+-rw-r--r--   0        0        0     5264 2023-06-13 10:57:30.681207 shaperglot-0.2.0/shaperglot/languages/gaa_Latn.yaml
+-rw-r--r--   0        0        0     7909 2023-06-13 10:57:30.681394 shaperglot-0.2.0/shaperglot/languages/gby_Latn.yaml
+-rw-r--r--   0        0        0     4751 2023-06-13 10:57:30.681564 shaperglot-0.2.0/shaperglot/languages/gde_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.681674 shaperglot-0.2.0/shaperglot/languages/gej_Latn.yaml
+-rw-r--r--   0        0        0     6050 2023-06-13 10:57:30.681780 shaperglot-0.2.0/shaperglot/languages/gel_Latn.yaml
+-rw-r--r--   0        0        0     8093 2023-06-13 10:57:30.681924 shaperglot-0.2.0/shaperglot/languages/gkn_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.682082 shaperglot-0.2.0/shaperglot/languages/gmm_Latn.yaml
+-rw-r--r--   0        0        0     4191 2023-06-13 10:57:30.682259 shaperglot-0.2.0/shaperglot/languages/gmv_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.682397 shaperglot-0.2.0/shaperglot/languages/gnd_Latn.yaml
+-rw-r--r--   0        0        0     6945 2023-06-13 10:57:30.682577 shaperglot-0.2.0/shaperglot/languages/gng_Latn.yaml
+-rw-r--r--   0        0        0     5762 2023-06-13 10:57:30.682720 shaperglot-0.2.0/shaperglot/languages/god_Latn.yaml
+-rw-r--r--   0        0        0     4191 2023-06-13 10:57:30.682861 shaperglot-0.2.0/shaperglot/languages/gof_Latn.yaml
+-rw-r--r--   0        0        0     4206 2023-06-13 10:57:30.683020 shaperglot-0.2.0/shaperglot/languages/gqr_Latn.yaml
+-rw-r--r--   0        0        0     5086 2023-06-13 10:57:30.683162 shaperglot-0.2.0/shaperglot/languages/gud_Latn.yaml
+-rw-r--r--   0        0        0     4529 2023-06-13 10:57:30.683328 shaperglot-0.2.0/shaperglot/languages/guk_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.683499 shaperglot-0.2.0/shaperglot/languages/guw_Latn.yaml
+-rw-r--r--   0        0        0     6435 2023-06-13 10:57:30.683653 shaperglot-0.2.0/shaperglot/languages/gux_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.683780 shaperglot-0.2.0/shaperglot/languages/guz_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.683875 shaperglot-0.2.0/shaperglot/languages/gyi_Latn.yaml
+-rw-r--r--   0        0        0     7744 2023-06-13 10:57:30.683974 shaperglot-0.2.0/shaperglot/languages/ha_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.684063 shaperglot-0.2.0/shaperglot/languages/hag_Latn.yaml
+-rw-r--r--   0        0        0     5033 2023-06-13 10:57:30.684156 shaperglot-0.2.0/shaperglot/languages/hia_Latn.yaml
+-rw-r--r--   0        0        0     5540 2023-06-13 10:57:30.684245 shaperglot-0.2.0/shaperglot/languages/hig_Latn.yaml
+-rw-r--r--   0        0        0     3877 2023-06-13 10:57:30.684364 shaperglot-0.2.0/shaperglot/languages/ibb_Latn.yaml
+-rw-r--r--   0        0        0     7248 2023-06-13 10:57:30.684499 shaperglot-0.2.0/shaperglot/languages/iby_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.684609 shaperglot-0.2.0/shaperglot/languages/ica_Latn.yaml
+-rw-r--r--   0        0        0     7230 2023-06-13 10:57:30.684696 shaperglot-0.2.0/shaperglot/languages/ich_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.684777 shaperglot-0.2.0/shaperglot/languages/idd_Latn.yaml
+-rw-r--r--   0        0        0     8558 2023-06-13 10:57:30.684870 shaperglot-0.2.0/shaperglot/languages/ig_Latn.yaml
+-rw-r--r--   0        0        0     8769 2023-06-13 10:57:30.684968 shaperglot-0.2.0/shaperglot/languages/igb_Latn.yaml
+-rw-r--r--   0        0        0     6904 2023-06-13 10:57:30.685054 shaperglot-0.2.0/shaperglot/languages/ige_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.685137 shaperglot-0.2.0/shaperglot/languages/ijj_Latn.yaml
+-rw-r--r--   0        0        0     5386 2023-06-13 10:57:30.685258 shaperglot-0.2.0/shaperglot/languages/ikk_Latn.yaml
+-rw-r--r--   0        0        0     5890 2023-06-13 10:57:30.685363 shaperglot-0.2.0/shaperglot/languages/ikw_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.685455 shaperglot-0.2.0/shaperglot/languages/ikx_Latn.yaml
+-rw-r--r--   0        0        0     4713 2023-06-13 10:57:30.685548 shaperglot-0.2.0/shaperglot/languages/iqw_Latn.yaml
+-rw-r--r--   0        0        0     5540 2023-06-13 10:57:30.685651 shaperglot-0.2.0/shaperglot/languages/iri_Latn.yaml
+-rw-r--r--   0        0        0     6047 2023-06-13 10:57:30.685773 shaperglot-0.2.0/shaperglot/languages/izr_Latn.yaml
+-rw-r--r--   0        0        0     7417 2023-06-13 10:57:30.685874 shaperglot-0.2.0/shaperglot/languages/izz_Latn.yaml
+-rw-r--r--   0        0        0     8075 2023-06-13 10:57:30.685963 shaperglot-0.2.0/shaperglot/languages/jab_Latn.yaml
+-rw-r--r--   0        0        0     8591 2023-06-13 10:57:30.686092 shaperglot-0.2.0/shaperglot/languages/jbu_Latn.yaml
+-rw-r--r--   0        0        0     7571 2023-06-13 10:57:30.686218 shaperglot-0.2.0/shaperglot/languages/jen_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.686313 shaperglot-0.2.0/shaperglot/languages/jgk_Latn.yaml
+-rw-r--r--   0        0        0     7898 2023-06-13 10:57:30.686438 shaperglot-0.2.0/shaperglot/languages/jgo_Latn.yaml
+-rw-r--r--   0        0        0     6557 2023-06-13 10:57:30.686531 shaperglot-0.2.0/shaperglot/languages/jib_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.686627 shaperglot-0.2.0/shaperglot/languages/jmc_Latn.yaml
+-rw-r--r--   0        0        0     6065 2023-06-13 10:57:30.686767 shaperglot-0.2.0/shaperglot/languages/kab_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.686876 shaperglot-0.2.0/shaperglot/languages/kad_Latn.yaml
+-rw-r--r--   0        0        0     5202 2023-06-13 10:57:30.687008 shaperglot-0.2.0/shaperglot/languages/kai_Latn.yaml
+-rw-r--r--   0        0        0     4529 2023-06-13 10:57:30.687133 shaperglot-0.2.0/shaperglot/languages/kam_Latn.yaml
+-rw-r--r--   0        0        0     4197 2023-06-13 10:57:30.687259 shaperglot-0.2.0/shaperglot/languages/kby_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.687401 shaperglot-0.2.0/shaperglot/languages/kdc_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.687540 shaperglot-0.2.0/shaperglot/languages/kde_Latn.yaml
+-rw-r--r--   0        0        0     7336 2023-06-13 10:57:30.687684 shaperglot-0.2.0/shaperglot/languages/kdh_Latn.yaml
+-rw-r--r--   0        0        0     4867 2023-06-13 10:57:30.687823 shaperglot-0.2.0/shaperglot/languages/kdl_Latn.yaml
+-rw-r--r--   0        0        0     7787 2023-06-13 10:57:30.687978 shaperglot-0.2.0/shaperglot/languages/ken_Latn.yaml
+-rw-r--r--   0        0        0     6385 2023-06-13 10:57:30.688108 shaperglot-0.2.0/shaperglot/languages/kez_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.688276 shaperglot-0.2.0/shaperglot/languages/kg_Latn.yaml
+-rw-r--r--   0        0        0     5543 2023-06-13 10:57:30.688433 shaperglot-0.2.0/shaperglot/languages/khq_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.688618 shaperglot-0.2.0/shaperglot/languages/ki_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.688792 shaperglot-0.2.0/shaperglot/languages/kj_Latn.yaml
+-rw-r--r--   0        0        0     8152 2023-06-13 10:57:30.688976 shaperglot-0.2.0/shaperglot/languages/kkj_Latn.yaml
+-rw-r--r--   0        0        0     3361 2023-06-13 10:57:30.689126 shaperglot-0.2.0/shaperglot/languages/kmb_Latn.yaml
+-rw-r--r--   0        0        0     4751 2023-06-13 10:57:30.689355 shaperglot-0.2.0/shaperglot/languages/kmy_Latn.yaml
+-rw-r--r--   0        0        0     4707 2023-06-13 10:57:30.689573 shaperglot-0.2.0/shaperglot/languages/knf_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.689783 shaperglot-0.2.0/shaperglot/languages/knp_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.689942 shaperglot-0.2.0/shaperglot/languages/kpo_Latn.yaml
+-rw-r--r--   0        0        0     5098 2023-06-13 10:57:30.690137 shaperglot-0.2.0/shaperglot/languages/kqp_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.690298 shaperglot-0.2.0/shaperglot/languages/krs_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.690432 shaperglot-0.2.0/shaperglot/languages/ksb_Latn.yaml
+-rw-r--r--   0        0        0     6140 2023-06-13 10:57:30.690561 shaperglot-0.2.0/shaperglot/languages/ksf_Latn.yaml
+-rw-r--r--   0        0        0     3696 2023-06-13 10:57:30.690708 shaperglot-0.2.0/shaperglot/languages/ksp_Latn.yaml
+-rw-r--r--   0        0        0     4588 2023-06-13 10:57:30.690857 shaperglot-0.2.0/shaperglot/languages/ktj_Latn.yaml
+-rw-r--r--   0        0        0     6388 2023-06-13 10:57:30.691001 shaperglot-0.2.0/shaperglot/languages/kub_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.691140 shaperglot-0.2.0/shaperglot/languages/kuj_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.691315 shaperglot-0.2.0/shaperglot/languages/kun_Latn.yaml
+-rw-r--r--   0        0        0     4576 2023-06-13 10:57:30.691474 shaperglot-0.2.0/shaperglot/languages/kus_Latn.yaml
+-rw-r--r--   0        0        0     4920 2023-06-13 10:57:30.691616 shaperglot-0.2.0/shaperglot/languages/kvf_Latn.yaml
+-rw-r--r--   0        0        0     4920 2023-06-13 10:57:30.691753 shaperglot-0.2.0/shaperglot/languages/kye_Latn.yaml
+-rw-r--r--   0        0        0     4920 2023-06-13 10:57:30.691904 shaperglot-0.2.0/shaperglot/languages/kyf_Latn.yaml
+-rw-r--r--   0        0        0     4591 2023-06-13 10:57:30.692051 shaperglot-0.2.0/shaperglot/languages/kyq_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.692186 shaperglot-0.2.0/shaperglot/languages/kzr_Latn.yaml
+-rw-r--r--   0        0        0     5540 2023-06-13 10:57:30.692323 shaperglot-0.2.0/shaperglot/languages/lag_Latn.yaml
+-rw-r--r--   0        0        0     5928 2023-06-13 10:57:30.692472 shaperglot-0.2.0/shaperglot/languages/las_Latn.yaml
+-rw-r--r--   0        0        0     5543 2023-06-13 10:57:30.692628 shaperglot-0.2.0/shaperglot/languages/ldb_Latn.yaml
+-rw-r--r--   0        0        0     4698 2023-06-13 10:57:30.692743 shaperglot-0.2.0/shaperglot/languages/led_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.692856 shaperglot-0.2.0/shaperglot/languages/lee_Latn.yaml
+-rw-r--r--   0        0        0     5925 2023-06-13 10:57:30.693009 shaperglot-0.2.0/shaperglot/languages/lem_Latn.yaml
+-rw-r--r--   0        0        0     3699 2023-06-13 10:57:30.693157 shaperglot-0.2.0/shaperglot/languages/les_Latn.yaml
+-rw-r--r--   0        0        0     4576 2023-06-13 10:57:30.693298 shaperglot-0.2.0/shaperglot/languages/lg_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.693434 shaperglot-0.2.0/shaperglot/languages/lgg_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.693569 shaperglot-0.2.0/shaperglot/languages/lig_Latn.yaml
+-rw-r--r--   0        0        0     4369 2023-06-13 10:57:30.693723 shaperglot-0.2.0/shaperglot/languages/lip_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.693856 shaperglot-0.2.0/shaperglot/languages/lln_Latn.yaml
+-rw-r--r--   0        0        0     7449 2023-06-13 10:57:30.693996 shaperglot-0.2.0/shaperglot/languages/lmp_Latn.yaml
+-rw-r--r--   0        0        0     7152 2023-06-13 10:57:30.694155 shaperglot-0.2.0/shaperglot/languages/ln_Latn.yaml
+-rw-r--r--   0        0        0     4698 2023-06-13 10:57:30.694297 shaperglot-0.2.0/shaperglot/languages/lnu_Latn.yaml
+-rw-r--r--   0        0        0     4422 2023-06-13 10:57:30.694442 shaperglot-0.2.0/shaperglot/languages/log_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.694578 shaperglot-0.2.0/shaperglot/languages/lok_Latn.yaml
+-rw-r--r--   0        0        0     4591 2023-06-13 10:57:30.694727 shaperglot-0.2.0/shaperglot/languages/loq_Latn.yaml
+-rw-r--r--   0        0        0     5202 2023-06-13 10:57:30.694875 shaperglot-0.2.0/shaperglot/languages/lor_Latn.yaml
+-rw-r--r--   0        0        0     3862 2023-06-13 10:57:30.694988 shaperglot-0.2.0/shaperglot/languages/loz_Latn.yaml
+-rw-r--r--   0        0        0     6613 2023-06-13 10:57:30.695093 shaperglot-0.2.0/shaperglot/languages/lu_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.695207 shaperglot-0.2.0/shaperglot/languages/lua_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.695305 shaperglot-0.2.0/shaperglot/languages/luo_Latn.yaml
+-rw-r--r--   0        0        0     3530 2023-06-13 10:57:30.695410 shaperglot-0.2.0/shaperglot/languages/lwo_Latn.yaml
+-rw-r--r--   0        0        0     8812 2023-06-13 10:57:30.695529 shaperglot-0.2.0/shaperglot/languages/mas_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.695630 shaperglot-0.2.0/shaperglot/languages/maw_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.695747 shaperglot-0.2.0/shaperglot/languages/mbo_Latn.yaml
+-rw-r--r--   0        0        0     7111 2023-06-13 10:57:30.695855 shaperglot-0.2.0/shaperglot/languages/mbu_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.695963 shaperglot-0.2.0/shaperglot/languages/mcp_Latn.yaml
+-rw-r--r--   0        0        0     4745 2023-06-13 10:57:30.696057 shaperglot-0.2.0/shaperglot/languages/mcu_Latn.yaml
+-rw-r--r--   0        0        0     8413 2023-06-13 10:57:30.696187 shaperglot-0.2.0/shaperglot/languages/mda_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.696302 shaperglot-0.2.0/shaperglot/languages/mdj_Latn.yaml
+-rw-r--r--   0        0        0     3865 2023-06-13 10:57:30.696484 shaperglot-0.2.0/shaperglot/languages/men_Latn.yaml
+-rw-r--r--   0        0        0     4926 2023-06-13 10:57:30.696640 shaperglot-0.2.0/shaperglot/languages/meq_Latn.yaml
+-rw-r--r--   0        0        0     5857 2023-06-13 10:57:30.696782 shaperglot-0.2.0/shaperglot/languages/mer_Latn.yaml
+-rw-r--r--   0        0        0     5264 2023-06-13 10:57:30.696924 shaperglot-0.2.0/shaperglot/languages/mfi_Latn.yaml
+-rw-r--r--   0        0        0     6904 2023-06-13 10:57:30.697066 shaperglot-0.2.0/shaperglot/languages/mfn_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.697199 shaperglot-0.2.0/shaperglot/languages/mfo_Latn.yaml
+-rw-r--r--   0        0        0     4754 2023-06-13 10:57:30.697344 shaperglot-0.2.0/shaperglot/languages/mfv_Latn.yaml
+-rw-r--r--   0        0        0     6216 2023-06-13 10:57:30.697497 shaperglot-0.2.0/shaperglot/languages/mg_Latn.yaml
+-rw-r--r--   0        0        0     5264 2023-06-13 10:57:30.697649 shaperglot-0.2.0/shaperglot/languages/mgc_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.697780 shaperglot-0.2.0/shaperglot/languages/mgh_Latn.yaml
+-rw-r--r--   0        0        0     5955 2023-06-13 10:57:30.697916 shaperglot-0.2.0/shaperglot/languages/mgo_Latn.yaml
+-rw-r--r--   0        0        0     4929 2023-06-13 10:57:30.698053 shaperglot-0.2.0/shaperglot/languages/mhi_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.698172 shaperglot-0.2.0/shaperglot/languages/mkl_Latn.yaml
+-rw-r--r--   0        0        0     5878 2023-06-13 10:57:30.698273 shaperglot-0.2.0/shaperglot/languages/mlt_Latn.yaml
+-rw-r--r--   0        0        0     5759 2023-06-13 10:57:30.698407 shaperglot-0.2.0/shaperglot/languages/mmu_Latn.yaml
+-rw-r--r--   0        0        0     5083 2023-06-13 10:57:30.698542 shaperglot-0.2.0/shaperglot/languages/mnf_Latn.yaml
+-rw-r--r--   0        0        0     5080 2023-06-13 10:57:30.698665 shaperglot-0.2.0/shaperglot/languages/moa_Latn.yaml
+-rw-r--r--   0        0        0     4034 2023-06-13 10:57:30.698855 shaperglot-0.2.0/shaperglot/languages/mos_Latn.yaml
+-rw-r--r--   0        0        0     6222 2023-06-13 10:57:30.699031 shaperglot-0.2.0/shaperglot/languages/mqb_Latn.yaml
+-rw-r--r--   0        0        0     6898 2023-06-13 10:57:30.699195 shaperglot-0.2.0/shaperglot/languages/mql_Latn.yaml
+-rw-r--r--   0        0        0     4200 2023-06-13 10:57:30.699335 shaperglot-0.2.0/shaperglot/languages/msc_Latn.yaml
+-rw-r--r--   0        0        0     5931 2023-06-13 10:57:30.699482 shaperglot-0.2.0/shaperglot/languages/mua_Latn.yaml
+-rw-r--r--   0        0        0     4704 2023-06-13 10:57:30.699621 shaperglot-0.2.0/shaperglot/languages/muh_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.699754 shaperglot-0.2.0/shaperglot/languages/mur_Latn.yaml
+-rw-r--r--   0        0        0     6272 2023-06-13 10:57:30.699884 shaperglot-0.2.0/shaperglot/languages/muy_Latn.yaml
+-rw-r--r--   0        0        0     6435 2023-06-13 10:57:30.700048 shaperglot-0.2.0/shaperglot/languages/myk_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.700213 shaperglot-0.2.0/shaperglot/languages/mym_Latn.yaml
+-rw-r--r--   0        0        0     6047 2023-06-13 10:57:30.700369 shaperglot-0.2.0/shaperglot/languages/mzk_Latn.yaml
+-rw-r--r--   0        0        0     9430 2023-06-13 10:57:30.700532 shaperglot-0.2.0/shaperglot/languages/mzm_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.700674 shaperglot-0.2.0/shaperglot/languages/mzw_Latn.yaml
+-rw-r--r--   0        0        0     5033 2023-06-13 10:57:30.700839 shaperglot-0.2.0/shaperglot/languages/naq_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.700984 shaperglot-0.2.0/shaperglot/languages/nat_Latn.yaml
+-rw-r--r--   0        0        0     4425 2023-06-13 10:57:30.701136 shaperglot-0.2.0/shaperglot/languages/naw_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.701274 shaperglot-0.2.0/shaperglot/languages/ncu_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.701405 shaperglot-0.2.0/shaperglot/languages/nd_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.701533 shaperglot-0.2.0/shaperglot/languages/ndj_Latn.yaml
+-rw-r--r--   0        0        0     4422 2023-06-13 10:57:30.701670 shaperglot-0.2.0/shaperglot/languages/ndz_Latn.yaml
+-rw-r--r--   0        0        0     4701 2023-06-13 10:57:30.701795 shaperglot-0.2.0/shaperglot/languages/neb_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.701916 shaperglot-0.2.0/shaperglot/languages/nfr_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.702048 shaperglot-0.2.0/shaperglot/languages/ng_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.702175 shaperglot-0.2.0/shaperglot/languages/nga_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.702303 shaperglot-0.2.0/shaperglot/languages/ngb_Latn.yaml
+-rw-r--r--   0        0        0     4025 2023-06-13 10:57:30.702430 shaperglot-0.2.0/shaperglot/languages/ngp_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.702559 shaperglot-0.2.0/shaperglot/languages/nhb_Latn.yaml
+-rw-r--r--   0        0        0     4081 2023-06-13 10:57:30.702701 shaperglot-0.2.0/shaperglot/languages/nhu_Latn.yaml
+-rw-r--r--   0        0        0     9089 2023-06-13 10:57:30.702827 shaperglot-0.2.0/shaperglot/languages/nin_Latn.yaml
+-rw-r--r--   0        0        0     5033 2023-06-13 10:57:30.702960 shaperglot-0.2.0/shaperglot/languages/niy_Latn.yaml
+-rw-r--r--   0        0        0     6097 2023-06-13 10:57:30.703079 shaperglot-0.2.0/shaperglot/languages/nko_Latn.yaml
+-rw-r--r--   0        0        0     9833 2023-06-13 10:57:30.703204 shaperglot-0.2.0/shaperglot/languages/nmg_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.703355 shaperglot-0.2.0/shaperglot/languages/nmz_Latn.yaml
+-rw-r--r--   0        0        0     9163 2023-06-13 10:57:30.703521 shaperglot-0.2.0/shaperglot/languages/nnh_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.703735 shaperglot-0.2.0/shaperglot/languages/nnq_Latn.yaml
+-rw-r--r--   0        0        0     5089 2023-06-13 10:57:30.703894 shaperglot-0.2.0/shaperglot/languages/nnw_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.704038 shaperglot-0.2.0/shaperglot/languages/nr_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.704184 shaperglot-0.2.0/shaperglot/languages/nrb_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.704338 shaperglot-0.2.0/shaperglot/languages/nso_Latn.yaml
+-rw-r--r--   0        0        0     6400 2023-06-13 10:57:30.704523 shaperglot-0.2.0/shaperglot/languages/ntm_Latn.yaml
+-rw-r--r--   0        0        0     5080 2023-06-13 10:57:30.704674 shaperglot-0.2.0/shaperglot/languages/ntr_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.704821 shaperglot-0.2.0/shaperglot/languages/nui_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.704988 shaperglot-0.2.0/shaperglot/languages/nup_Latn.yaml
+-rw-r--r--   0        0        0     6083 2023-06-13 10:57:30.705132 shaperglot-0.2.0/shaperglot/languages/nus_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.705268 shaperglot-0.2.0/shaperglot/languages/nuv_Latn.yaml
+-rw-r--r--   0        0        0     4867 2023-06-13 10:57:30.705499 shaperglot-0.2.0/shaperglot/languages/nwb_Latn.yaml
+-rw-r--r--   0        0        0     4745 2023-06-13 10:57:30.705750 shaperglot-0.2.0/shaperglot/languages/ny_Latn.yaml
+-rw-r--r--   0        0        0     3918 2023-06-13 10:57:30.705901 shaperglot-0.2.0/shaperglot/languages/nym_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.706103 shaperglot-0.2.0/shaperglot/languages/nyn_Latn.yaml
+-rw-r--r--   0        0        0     4031 2023-06-13 10:57:30.706245 shaperglot-0.2.0/shaperglot/languages/nzi_Latn.yaml
+-rw-r--r--   0        0        0     5881 2023-06-13 10:57:30.706412 shaperglot-0.2.0/shaperglot/languages/ogc_Latn.yaml
+-rw-r--r--   0        0        0     5389 2023-06-13 10:57:30.706570 shaperglot-0.2.0/shaperglot/languages/okr_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.706719 shaperglot-0.2.0/shaperglot/languages/om_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.706850 shaperglot-0.2.0/shaperglot/languages/ozm_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.706972 shaperglot-0.2.0/shaperglot/languages/pbi_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.707119 shaperglot-0.2.0/shaperglot/languages/pil_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.707244 shaperglot-0.2.0/shaperglot/languages/pip_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.707394 shaperglot-0.2.0/shaperglot/languages/pko_Latn.yaml
+-rw-r--r--   0        0        0     5374 2023-06-13 10:57:30.707534 shaperglot-0.2.0/shaperglot/languages/png_Latn.yaml
+-rw-r--r--   0        0        0     4025 2023-06-13 10:57:30.707657 shaperglot-0.2.0/shaperglot/languages/poy_Latn.yaml
+-rw-r--r--   0        0        0     4701 2023-06-13 10:57:30.707785 shaperglot-0.2.0/shaperglot/languages/pym_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.707950 shaperglot-0.2.0/shaperglot/languages/rel_Latn.yaml
+-rw-r--r--   0        0        0     5033 2023-06-13 10:57:30.708089 shaperglot-0.2.0/shaperglot/languages/res_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.708238 shaperglot-0.2.0/shaperglot/languages/rn_Latn.yaml
+-rw-r--r--   0        0        0      389 2022-11-02 15:26:07.712635 shaperglot-0.2.0/shaperglot/languages/ro_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.708403 shaperglot-0.2.0/shaperglot/languages/rof_Latn.yaml
+-rw-r--r--   0        0        0     4244 2023-06-13 10:57:30.708594 shaperglot-0.2.0/shaperglot/languages/rub_Latn.yaml
+-rw-r--r--   0        0        0     4025 2023-06-13 10:57:30.708748 shaperglot-0.2.0/shaperglot/languages/ruf_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.708894 shaperglot-0.2.0/shaperglot/languages/rw_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.709030 shaperglot-0.2.0/shaperglot/languages/rwk_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.709232 shaperglot-0.2.0/shaperglot/languages/saq_Latn.yaml
+-rw-r--r--   0        0        0     4588 2023-06-13 10:57:30.709370 shaperglot-0.2.0/shaperglot/languages/sav_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.709542 shaperglot-0.2.0/shaperglot/languages/sba_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.709676 shaperglot-0.2.0/shaperglot/languages/sbp_Latn.yaml
+-rw-r--r--   0        0        0     6554 2023-06-13 10:57:30.709813 shaperglot-0.2.0/shaperglot/languages/seh_Latn.yaml
+-rw-r--r--   0        0        0     5593 2023-06-13 10:57:30.709945 shaperglot-0.2.0/shaperglot/languages/ses_Latn.yaml
+-rw-r--r--   0        0        0     6216 2023-06-13 10:57:30.710075 shaperglot-0.2.0/shaperglot/languages/sg_Latn.yaml
+-rw-r--r--   0        0        0     4360 2023-06-13 10:57:30.710208 shaperglot-0.2.0/shaperglot/languages/she_Latn.yaml
+-rw-r--r--   0        0        0     5555 2023-06-13 10:57:30.710359 shaperglot-0.2.0/shaperglot/languages/shi_Latn.yaml
+-rw-r--r--   0        0        0     6892 2023-06-13 10:57:30.710492 shaperglot-0.2.0/shaperglot/languages/shu_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.710622 shaperglot-0.2.0/shaperglot/languages/sig_Latn.yaml
+-rw-r--r--   0        0        0     5086 2023-06-13 10:57:30.710745 shaperglot-0.2.0/shaperglot/languages/sil_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.710860 shaperglot-0.2.0/shaperglot/languages/sld_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.710975 shaperglot-0.2.0/shaperglot/languages/sn_Latn.yaml
+-rw-r--r--   0        0        0     4025 2023-06-13 10:57:30.711099 shaperglot-0.2.0/shaperglot/languages/snk_Latn.yaml
+-rw-r--r--   0        0        0     4541 2023-06-13 10:57:30.711220 shaperglot-0.2.0/shaperglot/languages/snw_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.711352 shaperglot-0.2.0/shaperglot/languages/so_Latn.yaml
+-rw-r--r--   0        0        0     5759 2023-06-13 10:57:30.711482 shaperglot-0.2.0/shaperglot/languages/sok_Latn.yaml
+-rw-r--r--   0        0        0     6782 2023-06-13 10:57:30.711645 shaperglot-0.2.0/shaperglot/languages/soy_Latn.yaml
+-rw-r--r--   0        0        0     4751 2023-06-13 10:57:30.711774 shaperglot-0.2.0/shaperglot/languages/spp_Latn.yaml
+-rw-r--r--   0        0        0     5427 2023-06-13 10:57:30.711901 shaperglot-0.2.0/shaperglot/languages/srr_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.712030 shaperglot-0.2.0/shaperglot/languages/ss_Latn.yaml
+-rw-r--r--   0        0        0     5245 2023-06-13 10:57:30.712170 shaperglot-0.2.0/shaperglot/languages/st_Latn.yaml
+-rw-r--r--   0        0        0     4194 2023-06-13 10:57:30.712311 shaperglot-0.2.0/shaperglot/languages/suk_Latn.yaml
+-rw-r--r--   0        0        0     4529 2023-06-13 10:57:30.712468 shaperglot-0.2.0/shaperglot/languages/suq_Latn.yaml
+-rw-r--r--   0        0        0     6554 2023-06-13 10:57:30.712604 shaperglot-0.2.0/shaperglot/languages/sur_Latn.yaml
+-rw-r--r--   0        0        0     4034 2023-06-13 10:57:30.712738 shaperglot-0.2.0/shaperglot/languages/sus_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.712877 shaperglot-0.2.0/shaperglot/languages/sw_Latn.yaml
+-rw-r--r--   0        0        0     4025 2023-06-13 10:57:30.713013 shaperglot-0.2.0/shaperglot/languages/swb_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.713146 shaperglot-0.2.0/shaperglot/languages/swc_Latn.yaml
+-rw-r--r--   0        0        0     4025 2023-06-13 10:57:30.713282 shaperglot-0.2.0/shaperglot/languages/sxb_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.713415 shaperglot-0.2.0/shaperglot/languages/sxw_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.713559 shaperglot-0.2.0/shaperglot/languages/tal_Latn.yaml
+-rw-r--r--   0        0        0     5724 2023-06-13 10:57:30.713703 shaperglot-0.2.0/shaperglot/languages/tan_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.713842 shaperglot-0.2.0/shaperglot/languages/ted_Latn.yaml
+-rw-r--r--   0        0        0     4090 2023-06-13 10:57:30.713976 shaperglot-0.2.0/shaperglot/languages/tem_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.714115 shaperglot-0.2.0/shaperglot/languages/teo_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.714253 shaperglot-0.2.0/shaperglot/languages/tfi_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.714390 shaperglot-0.2.0/shaperglot/languages/tik_Latn.yaml
+-rw-r--r--   0        0        0     4194 2023-06-13 10:57:30.714521 shaperglot-0.2.0/shaperglot/languages/tiv_Latn.yaml
+-rw-r--r--   0        0        0     4191 2023-06-13 10:57:30.714695 shaperglot-0.2.0/shaperglot/languages/tke_Latn.yaml
+-rw-r--r--   0        0        0     3693 2023-06-13 10:57:30.714847 shaperglot-0.2.0/shaperglot/languages/tlj_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.714985 shaperglot-0.2.0/shaperglot/languages/tn_Latn.yaml
+-rw-r--r--   0        0        0     4926 2023-06-13 10:57:30.715109 shaperglot-0.2.0/shaperglot/languages/tnr_Latn.yaml
+-rw-r--r--   0        0        0     4932 2023-06-13 10:57:30.715238 shaperglot-0.2.0/shaperglot/languages/tod_Latn.yaml
+-rw-r--r--   0        0        0     4576 2023-06-13 10:57:30.715367 shaperglot-0.2.0/shaperglot/languages/toq_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.715494 shaperglot-0.2.0/shaperglot/languages/tpm_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.715700 shaperglot-0.2.0/shaperglot/languages/ts_Latn.yaml
+-rw-r--r--   0        0        0     4867 2023-06-13 10:57:30.715881 shaperglot-0.2.0/shaperglot/languages/tsw_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.716038 shaperglot-0.2.0/shaperglot/languages/ttr_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.716186 shaperglot-0.2.0/shaperglot/languages/tul_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.716328 shaperglot-0.2.0/shaperglot/languages/tum_Latn.yaml
+-rw-r--r--   0        0        0     5596 2023-06-13 10:57:30.716466 shaperglot-0.2.0/shaperglot/languages/tuq_Latn.yaml
+-rw-r--r--   0        0        0     5371 2023-06-13 10:57:30.716615 shaperglot-0.2.0/shaperglot/languages/tvd_Latn.yaml
+-rw-r--r--   0        0        0     5759 2023-06-13 10:57:30.716750 shaperglot-0.2.0/shaperglot/languages/tvu_Latn.yaml
+-rw-r--r--   0        0        0     5593 2023-06-13 10:57:30.716874 shaperglot-0.2.0/shaperglot/languages/twq_Latn.yaml
+-rw-r--r--   0        0        0     5555 2023-06-13 10:57:30.716989 shaperglot-0.2.0/shaperglot/languages/tzm_Latn.yaml
+-rw-r--r--   0        0        0     4707 2023-06-13 10:57:30.717100 shaperglot-0.2.0/shaperglot/languages/umb_Latn.yaml
+-rw-r--r--   0        0        0     6216 2023-06-13 10:57:30.717206 shaperglot-0.2.0/shaperglot/languages/uth_Latn.yaml
+-rw-r--r--   0        0        0     4695 2023-06-13 10:57:30.717317 shaperglot-0.2.0/shaperglot/languages/utr_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.717410 shaperglot-0.2.0/shaperglot/languages/vag_Latn.yaml
+-rw-r--r--   0        0        0     7173 2023-06-13 10:57:30.717556 shaperglot-0.2.0/shaperglot/languages/vai_Latn.yaml
+-rw-r--r--   0        0        0     4719 2023-06-13 10:57:30.717707 shaperglot-0.2.0/shaperglot/languages/ve_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.717849 shaperglot-0.2.0/shaperglot/languages/vid_Latn.yaml
+-rw-r--r--   0        0        0     5202 2023-06-13 10:57:30.717980 shaperglot-0.2.0/shaperglot/languages/vmw_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.718115 shaperglot-0.2.0/shaperglot/languages/vun_Latn.yaml
+-rw-r--r--   0        0        0     5421 2023-06-13 10:57:30.718245 shaperglot-0.2.0/shaperglot/languages/vut_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.718401 shaperglot-0.2.0/shaperglot/languages/wal_Latn.yaml
+-rw-r--r--   0        0        0     4748 2023-06-13 10:57:30.718539 shaperglot-0.2.0/shaperglot/languages/wan_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.718671 shaperglot-0.2.0/shaperglot/languages/wci_Latn.yaml
+-rw-r--r--   0        0        0     4698 2023-06-13 10:57:30.718807 shaperglot-0.2.0/shaperglot/languages/wib_Latn.yaml
+-rw-r--r--   0        0        0     5202 2023-06-13 10:57:30.718939 shaperglot-0.2.0/shaperglot/languages/wja_Latn.yaml
+-rw-r--r--   0        0        0     4864 2023-06-13 10:57:30.719087 shaperglot-0.2.0/shaperglot/languages/wji_Latn.yaml
+-rw-r--r--   0        0        0     4532 2023-06-13 10:57:30.719225 shaperglot-0.2.0/shaperglot/languages/wmw_Latn.yaml
+-rw-r--r--   0        0        0     5590 2023-06-13 10:57:30.719369 shaperglot-0.2.0/shaperglot/languages/wo_Latn.yaml
+-rw-r--r--   0        0        0     4701 2023-06-13 10:57:30.719534 shaperglot-0.2.0/shaperglot/languages/wob_Latn.yaml
+-rw-r--r--   0        0        0     4591 2023-06-13 10:57:30.719679 shaperglot-0.2.0/shaperglot/languages/xed_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.719909 shaperglot-0.2.0/shaperglot/languages/xh_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.720135 shaperglot-0.2.0/shaperglot/languages/xog_Latn.yaml
+-rw-r--r--   0        0        0     4911 2023-06-13 10:57:30.720294 shaperglot-0.2.0/shaperglot/languages/xon_Latn.yaml
+-rw-r--r--   0        0        0     4914 2023-06-13 10:57:30.720424 shaperglot-0.2.0/shaperglot/languages/xrb_Latn.yaml
+-rw-r--r--   0        0        0     5095 2023-06-13 10:57:30.720554 shaperglot-0.2.0/shaperglot/languages/xuo_Latn.yaml
+-rw-r--r--   0        0        0     5252 2023-06-13 10:57:30.720679 shaperglot-0.2.0/shaperglot/languages/xwe_Latn.yaml
+-rw-r--r--   0        0        0     4034 2023-06-13 10:57:30.720825 shaperglot-0.2.0/shaperglot/languages/yal_Latn.yaml
+-rw-r--r--   0        0        0     4751 2023-06-13 10:57:30.720938 shaperglot-0.2.0/shaperglot/languages/yam_Latn.yaml
+-rw-r--r--   0        0        0     3530 2023-06-13 10:57:30.721035 shaperglot-0.2.0/shaperglot/languages/yao_Latn.yaml
+-rw-r--r--   0        0        0     5593 2023-06-13 10:57:30.721142 shaperglot-0.2.0/shaperglot/languages/yas_Latn.yaml
+-rw-r--r--   0        0        0     5928 2023-06-13 10:57:30.721240 shaperglot-0.2.0/shaperglot/languages/yat_Latn.yaml
+-rw-r--r--   0        0        0     8691 2023-06-13 10:57:30.721352 shaperglot-0.2.0/shaperglot/languages/yav_Latn.yaml
+-rw-r--r--   0        0        0     5039 2023-06-13 10:57:30.721458 shaperglot-0.2.0/shaperglot/languages/yay_Latn.yaml
+-rw-r--r--   0        0        0     5380 2023-06-13 10:57:30.721553 shaperglot-0.2.0/shaperglot/languages/yaz_Latn.yaml
+-rw-r--r--   0        0        0     5540 2023-06-13 10:57:30.721655 shaperglot-0.2.0/shaperglot/languages/yba_Latn.yaml
+-rw-r--r--   0        0        0     8078 2023-06-13 10:57:30.721780 shaperglot-0.2.0/shaperglot/languages/yer_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.721915 shaperglot-0.2.0/shaperglot/languages/yko_Latn.yaml
+-rw-r--r--   0        0        0     7329 2023-06-13 10:57:30.722063 shaperglot-0.2.0/shaperglot/languages/yo_Latn.yaml
+-rw-r--r--   0        0        0     4369 2023-06-13 10:57:30.722198 shaperglot-0.2.0/shaperglot/languages/yre_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.722328 shaperglot-0.2.0/shaperglot/languages/zay_Latn.yaml
+-rw-r--r--   0        0        0     3859 2023-06-13 10:57:30.722467 shaperglot-0.2.0/shaperglot/languages/ziw_Latn.yaml
+-rw-r--r--   0        0        0     4357 2023-06-13 10:57:30.722601 shaperglot-0.2.0/shaperglot/languages/zne_Latn.yaml
+-rw-r--r--   0        0        0    10779 2023-06-13 10:57:30.722729 shaperglot-0.2.0/shaperglot/languages/zul_Latn.yaml
+-rw-r--r--   0        0        0     2949 2023-06-13 10:57:30.664291 shaperglot-0.2.0/shaperglot/languages.py
+-rw-r--r--   0        0        0     1645 2023-06-13 10:57:30.722985 shaperglot-0.2.0/shaperglot/reporter.py
+-rw-r--r--   0        0        0     7883 2023-06-13 10:59:29.621430 shaperglot-0.2.0/setup.py
+-rw-r--r--   0        0        0     7867 2023-06-13 10:59:29.621871 shaperglot-0.2.0/PKG-INFO
```

### Comparing `shaperglot-0.1.0/LICENSE.md` & `shaperglot-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/README.md` & `shaperglot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/pyproject.toml` & `shaperglot-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "shaperglot"
-version = "0.1.0"
+version = "0.2.0"
 description = "Test font files for OpenType language support"
 
 license = "MIT"
 
 authors = ["Simon Cozens <simon@simon-cozens.org>"]
 
 readme = "README.md"
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
 
 python = ">= 3.7"
-gflanguages = { git = "https://github.com/googlefonts/lang" }
+gflanguages = ">= 0.4.7"
 termcolor = "1.1.0"
 vharfbuzz = "^0"
 strictyaml = "*"
 num2words = "^0.5"
 ufo2ft = "*"
 youseedee = "*"
 protobuf = "3.19.4"
```

### Comparing `shaperglot-0.1.0/shaperglot/checker.py` & `shaperglot-0.2.0/shaperglot/checker.py`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/checks/common.py` & `shaperglot-0.2.0/shaperglot/checks/common.py`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/checks/no_orphaned_marks.py` & `shaperglot-0.2.0/shaperglot/checks/no_orphaned_marks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from functools import cache
 
 from youseedee import ucd_data
 
+from shaperglot.checks.orthographies import OrthographiesCheck
+
 from .common import shaping_input_schema, ShaperglotCheck, check_schema
 
 
 @cache
 def _simple_mark_check(codepoint):
     return ucd_data(codepoint).get("General_Category") == "Mn"
 
@@ -78,7 +80,18 @@
         if passed:
             checker.results.okay(
                 check_name="no-orphaned-marks",
                 message="No unattached mark glyphs were produced "
                 + self.input.describe(),
                 context={"text": self.input.check_yaml},
             )
+
+
+class NoOrphanedMarksInOrthographiesCheck(NoOrphanedMarksCheck):
+    name = "no_orphaned_marks_in_orthographies"
+
+    def __init__(self, lang):
+        super().__init__({
+            "input": {
+                "text":" ".join(OrthographiesCheck(lang).bases)
+            }
+        })
```

### Comparing `shaperglot-0.1.0/shaperglot/checks/orthographies.py` & `shaperglot-0.2.0/shaperglot/checks/orthographies.py`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/checks/shaping_differs.py` & `shaperglot-0.2.0/shaperglot/checks/shaping_differs.py`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/checks/unencoded_variants.py` & `shaperglot-0.2.0/shaperglot/checks/unencoded_variants.py`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/cli.py` & `shaperglot-0.2.0/shaperglot/cli.py`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/aa_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/aa_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/abi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/abi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/abr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/abr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/acd_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/acd_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ada_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ada_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ade_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ade_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/adj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/adj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/aeb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/aeb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/af_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/af_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/agc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/agc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/agq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/agq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/aha_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/aha_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ahl_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ahl_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ahs_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ahs_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ak_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ak_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/akp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/akp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ala_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ala_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/anc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/anc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ank_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ank_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ann_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ann_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/anv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/anv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/any_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/any_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/apd_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/apd_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/asa_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/asa_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/asg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/asg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/atg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/atg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/avn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/avn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/avu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/avu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/awo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/awo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ayb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ayb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bas_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bas_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bav_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bav_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bbp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bbp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bci_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bci_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bcn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bcn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bcq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bcq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bcw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bcw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bcy_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bcy_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bdh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bdh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/beh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/beh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bej_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bej_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bem_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bem_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bet_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bet_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bex_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bex_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bez_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bez_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bhy_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bhy_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bib_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bib_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bim_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bim_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bin_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bin_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/biv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/biv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bjv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bjv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bkc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bkc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bkv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bkv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/blo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/blo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bng_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bng_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bnm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bnm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bom_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bom_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bov_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bov_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/box_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/box_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/boz_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/boz_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bqc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bqc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bqj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bqj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bqp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bqp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bsc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bsc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bsj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bsj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bsp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bsp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bsq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bsq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/btt_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/btt_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bud_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bud_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bus_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bus_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/buu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/buu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bwr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bwr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/byn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/byn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bys_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bys_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bza_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bza_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/bzw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/bzw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cbj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cbj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cdr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cdr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cfa_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cfa_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cgg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cgg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ckl_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ckl_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cko_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cko_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cky_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cky_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cla_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cla_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cme_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cme_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/csk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/csk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/cwe_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/cwe_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/daa_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/daa_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dav_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dav_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dbd_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dbd_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dbq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dbq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dgh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dgh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dgi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dgi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/did_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/did_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dje_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dje_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dop_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dop_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dow_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dow_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dri_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dri_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dts_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dts_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dua_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dua_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dug_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dug_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dwr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dwr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dyi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dyi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dyo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dyo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dyu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dyu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/dzg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/dzg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ebu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ebu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ee_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ee_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ekm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ekm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ema_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ema_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/enn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/enn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/etu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/etu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/etx_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/etx_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ewo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ewo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/eza_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/eza_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ffm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ffm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/flr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/flr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fmp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fmp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fod_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fod_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fon_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fon_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fub_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fub_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fue_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fue_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fuh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fuh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fuq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fuq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/fuv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/fuv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gaa_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gaa_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gby_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gby_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gde_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gde_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gej_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gej_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gel_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gel_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gkn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gkn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gmm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gmm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gmv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gmv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gnd_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gnd_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gng_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gng_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/god_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/god_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gof_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gof_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gqr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gqr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gud_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gud_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/guk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/guk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/guw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/guw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gux_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gux_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/guz_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/guz_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/gyi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/gyi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ha_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ha_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/hag_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/hag_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/hia_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/hia_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/hig_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/hig_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ibb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ibb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/iby_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/iby_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ica_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ica_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ich_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ich_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/idd_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/idd_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ig_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ig_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/igb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/igb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ige_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ige_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ijj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ijj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ikk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ikk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ikw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ikw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ikx_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ikx_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/iqw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/iqw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/iri_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/iri_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/izr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/izr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/izz_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/izz_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/jab_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/jab_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/jbu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/jbu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/jen_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/jen_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/jgk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/jgk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/jgo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/jgo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/jib_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/jib_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/jmc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/jmc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kab_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kab_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kad_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kad_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kai_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kai_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kam_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kam_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kby_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kby_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kdc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kdc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kde_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kde_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kdh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kdh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kdl_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kdl_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ken_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ken_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kez_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kez_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/khq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/khq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ki_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ki_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kkj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kkj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kmb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kmb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kmy_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kmy_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/knf_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/knf_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/knp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/knp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kpo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kpo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kqp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kqp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/krs_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/krs_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ksb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ksb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ksf_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ksf_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ksp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ksp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ktj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ktj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kub_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kub_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kuj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kuj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kun_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kun_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kus_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kus_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kvf_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kvf_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kye_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kye_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kyf_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kyf_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kyq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kyq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/kzr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/kzr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lag_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lag_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/las_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/las_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ldb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ldb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/led_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/led_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lee_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lee_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lem_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lem_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/les_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/les_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lgg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lgg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lig_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lig_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lip_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lip_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lln_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lln_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lmp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lmp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ln_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ln_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lnu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lnu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/log_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/log_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lok_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lok_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/loq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/loq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lor_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lor_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/loz_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/loz_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lua_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lua_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/luo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/luo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/lwo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/lwo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mas_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mas_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/maw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/maw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mbo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mbo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mbu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mbu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mcp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mcp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mcu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mcu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mda_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mda_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mdj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mdj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/men_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/men_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/meq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/meq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mer_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mer_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mfi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mfi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mfn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mfn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mfo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mfo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mfv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mfv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mgc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mgc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mgh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mgh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mgo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mgo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mhi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mhi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mkl_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mkl_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mlt_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mlt_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mmu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mmu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mnf_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mnf_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/moa_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/moa_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mos_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mos_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mqb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mqb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mql_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mql_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/msc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/msc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mua_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mua_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/muh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/muh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mur_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mur_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/muy_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/muy_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/myk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/myk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mym_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mym_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mzk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mzk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mzm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mzm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/mzw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/mzw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/naq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/naq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nat_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nat_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/naw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/naw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ncu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ncu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nd_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nd_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ndj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ndj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ndz_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ndz_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/neb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/neb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nfr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nfr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ng_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ng_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nga_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nga_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ngb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ngb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ngp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ngp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nhb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nhb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nhu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nhu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nin_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nin_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/niy_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/niy_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nko_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nko_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nmg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nmg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nmz_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nmz_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nnh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nnh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nnq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nnq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nnw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nnw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nrb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nrb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nso_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nso_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ntm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ntm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ntr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ntr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nui_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nui_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nup_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nup_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nus_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nus_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nuv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nuv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nwb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nwb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ny_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ny_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nym_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nym_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nyn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nyn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/nzi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/nzi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ogc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ogc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/okr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/okr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/om_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/om_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ozm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ozm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/pbi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/pbi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/pil_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/pil_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/pip_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/pip_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/pko_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/pko_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/png_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/png_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/poy_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/poy_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/pym_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/pym_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/rel_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/rel_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/res_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/res_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/rn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/rn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/rof_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/rof_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/rub_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/rub_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ruf_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ruf_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/rw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/rw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/rwk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/rwk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/saq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/saq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sav_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sav_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sba_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sba_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sbp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sbp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/seh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/seh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ses_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ses_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sg_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sg_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/she_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/she_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/shi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/shi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/shu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/shu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sig_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sig_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sil_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sil_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sld_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sld_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/snk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/snk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/snw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/snw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/so_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/so_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sok_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sok_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/soy_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/soy_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/spp_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/spp_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/srr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/srr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ss_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ss_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/st_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/st_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/suk_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/suk_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/suq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/suq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sur_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sur_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sus_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sus_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/swb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/swb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/swc_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/swc_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sxb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sxb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/sxw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/sxw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tal_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tal_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tan_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tan_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ted_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ted_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tem_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tem_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/teo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/teo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tfi_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tfi_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tik_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tik_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tiv_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tiv_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tke_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tke_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tlj_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tlj_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tn_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tn_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tnr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tnr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tod_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tod_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/toq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/toq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tpm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tpm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ts_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ts_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tsw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tsw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ttr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ttr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tul_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tul_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tum_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tum_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tuq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tuq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tvd_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tvd_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tvu_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tvu_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/twq_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/twq_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/tzm_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/tzm_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/umb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/umb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/uth_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/uth_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/utr_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/utr_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/vag_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/vag_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/vai_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/vai_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ve_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ve_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/vid_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/vid_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/vmw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/vmw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/vun_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/vun_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/vut_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/vut_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wal_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wal_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wan_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wan_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wci_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wci_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wib_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wib_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wja_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wja_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wji_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wji_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wmw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wmw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/wob_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/wob_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/xed_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/xed_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/xh_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/xh_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/xog_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/xog_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/xon_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/xon_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/xrb_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/xrb_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/xuo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/xuo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/xwe_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/xwe_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yal_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yal_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yam_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yam_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yao_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yao_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yas_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yas_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yat_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yat_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yav_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yav_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yay_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yay_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yaz_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yaz_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yba_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yba_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yer_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yer_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yko_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yko_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yo_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yo_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/yre_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/yre_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/zay_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/zay_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/ziw_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/ziw_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/zne_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/zne_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages/zul_Latn.yaml` & `shaperglot-0.2.0/shaperglot/languages/zul_Latn.yaml`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/shaperglot/languages.py` & `shaperglot-0.2.0/shaperglot/languages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 import sys
 
 from gflanguages import LoadLanguages, LoadScripts
 from strictyaml import YAMLValidationError, load
 from google.protobuf.json_format import MessageToDict
 
+from shaperglot.checks.no_orphaned_marks import NoOrphanedMarksInOrthographiesCheck
+
 from .checks import schemas, checks_map
 from .checks.orthographies import OrthographiesCheck
 
 gflangs = LoadLanguages()
 gfscripts = LoadScripts()
 
 definitions_directory = Path(__file__).parent / "languages"
@@ -64,15 +66,18 @@
             return self.loaded[item]
         if item not in gflangs:
             return None
         orig = MessageToDict(gflangs[item])
         orig["full_name"] = (
             orig["name"] + " in the " + gfscripts[orig["script"]].name + " script"
         )
-        orig["shaperglot_checks"] = [OrthographiesCheck(orig)]
+        orig["shaperglot_checks"] = [
+            OrthographiesCheck(orig),
+            NoOrphanedMarksInOrthographiesCheck(orig)
+        ]
         try:
             checks = load_shaperglot_definition(item, validate=True)
         except Exception as e:
             print(
                 f"The shaperglot definition for {item} is not valid. Please report a bug."
             )
             print(e)
```

### Comparing `shaperglot-0.1.0/shaperglot/reporter.py` & `shaperglot-0.2.0/shaperglot/reporter.py`

 * *Files identical despite different names*

### Comparing `shaperglot-0.1.0/setup.py` & `shaperglot-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 packages = \
 ['shaperglot', 'shaperglot.checks']
 
 package_data = \
 {'': ['*'], 'shaperglot': ['languages/*']}
 
 install_requires = \
-['gflanguages @ git+https://github.com/googlefonts/lang',
+['gflanguages>=0.4.7',
  'num2words>=0.5,<0.6',
  'protobuf==3.19.4',
  'strictyaml',
  'termcolor==1.1.0',
  'ufo2ft',
  'vharfbuzz>=0,<1',
  'youseedee']
 
 entry_points = \
 {'console_scripts': ['shaperglot = shaperglot.cli:main']}
 
 setup_kwargs = {
     'name': 'shaperglot',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Test font files for OpenType language support',
     'long_description': '# Shaperglot - Test font files for OpenType language support\n\n[![PyPI Version](https://img.shields.io/pypi/v/shaperglot.svg)](https://pypi.org/project/shaperglot)\n[![PyPI License](https://img.shields.io/pypi/l/shaperglot.svg)](https://pypi.org/project/shaperglot)\n\nShaperglot is a library and a utility for testing a font\'s language support.\nYou give it a font, and it tells you what languages are supported and to what\ndegree.\n\nMost other libraries to check for language support (for example, Rosetta\'s\nwonderful [hyperglot](https://hyperglot.rosettatype.com) library) do this by\nlooking at the Unicode codepoints that the font supports. Shaperglot takes\na different approach.\n\n## What\'s wrong with the Unicode codepoint coverage approach?\n\nFor many common languages, it\'s possible to check that the language is\nsupported just by looking at the Unicode coverage. For example, to support\nEnglish, you need the 26 lowercase and uppercase letters of the Latin alphabet.\n\nHowever, for the majority of scripts around the world, covering the codepoints\nneeded is not enough to say that a font really *supports* a particular language.\nFor correct language support, the font must also *behave* in a particular way.\n\nTake the case of Arabic as an example. A font might contain glyphs which cover\nall the codepoints in the Arabic block (0x600-0x6FF). But the font only *supports*\nArabic if it implements joining rules for the `init`, `medi` and `fina` features.\nTo say that a font supports Devanagari, it needs to implement conjuncts (which\nset of conjuncts need to be included before we can say the font "supports"\nDevanagari is debated...) and half forms, as well as contain a `languagesystem`\nstatement which triggers Indic reordering.\n\nEven within the Latin script, a font only supports a language such as Turkish\nif its casing behaving respects the dotless / dotted I distinction; a font\nonly supports Navajo if its ogonek anchoring is different to the anchoring used in\nPolish; and so on.\n\nBut there\'s a further problem with testing language support by codepoint coverage:\nit encourages designers to "fill in the blanks" to get to support, rather than\nnecessarily engage with the textual requirements of particular languages.\n\n## Testing for behaviour, not coverage\n\nShaperglot therefore determines language support not just on codepoint coverage,\nbut also by examining how the font behaves when confronted with certain character\nsequences.\n\nThe trick is to do this in a way which is not prescriptive. We know that there\nare many different ways of implementing language support within a font, and that\ndesign and other considerations will factor into precisely how a font is\nconstructed. Shaperglot presents the font with different strings, and makes sure\nthat "something interesting happened" - without necessarily specifying what.\n\nIn the case of Arabic, we need to know that the `init` feature is present, and that\nwhen we shape some Arabic glyphs, the output with `init` turned on is different\nto the output with `init` turned off. We don\'t care what\'s different; we only\ncare that something has happened. *(Yes, this still makes it possible to trick shaperglot into reporting support for a language which is not correctly implemented, but at that point, it\'s probably less effort to actually implement it...)*\n\nShaperglot includes (or will include) the following kinds of test:\n\n* Certain codepoints were mapped to base or mark glyphs.\n* A named feature was present.\n* A named feature changed the output glyphs.\n* A mark glyph was attached to a base glyph or composed into a precomposed glyph (but not left unattached).\n* Certain glyphs in the output were different to one another.\n* Languagesystems were defined in the font.\n* ...\n\nUsing this library of tests, we then create language support definitions which\nexercise the font\'s capabilities to obtain a fuller picture of its support for\na particular language. These language support definitions, expressed as YAML\nfiles, are the core of Shaperglot; to extend and improve Shaperglot, we need as\nmany language support definition files as possible - so if you know a language\nwell and can express what it means to "support" that language properly, please\ncontribute a definition!\n\n## Using Shaperglot\n\nTo report whether or not a given language is supported, pass a font and one or\nmore ISO639-3 language codes. \n\n```\n$ shaperglot -v -v MyFont.ttf urd\nFont does not fully support language \'urd\'\n * PASS: All base glyphs were present in the font\n * FAIL: Some mark glyphs were missing: ْ\n * PASS: Required feature \'mark\' was present\n * PASS: Mark glyph ◌َ  (FATHA) took part in a mark positioning rule\n * PASS: Mark glyph ◌ُ  (DAMMA) took part in a mark positioning rule\n * PASS: Mark glyph ◌ِ  (KASRA) took part in a mark positioning rule\n * PASS: Mark glyph ◌ٰ  (LONG_A) took part in a mark positioning rule\n * PASS: Required feature \'init\' was present\n * PASS: Glyph ع (AINu1) took part in a init rule\n * PASS: Required feature \'medi\' was present\n * PASS: Glyph ع (AINu1) took part in a medi rule\n * PASS: Required feature \'fina\' was present\n * PASS: Glyph ع (AINu1) took part in a fina rule\n * PASS: Repeated beh forms should produce different shapes\n * PASS: Initial and final forms should differ\n```\n\nShaperglot can also be run in bulk mode to check language support of entire font libraries. This is done by running `bulk-run-sg-.py` located in the scripts folder.\n\n```\n$ python bulk-run-sg.py ./<path-to-font-library>\n```\n\nThis script will automatically drill down the direcory tree and identify all .ttf font files and check them against a subset of language tags. At this time `bulk-run-sg.py` only checks fonts for Pan-African language support. The list of relevant language tags are defined in `language_tag_data/iso639-3-afr-all.txt`. Shaperglot results procesed in bulk can be quite large and may require additional tools to analyze. See [font-lang-support-afr](https://github.com/JamraPatel/font-lang-support-afr) for an example of how bulk results can be reported. Results are saved into two `.json` files.\n\n```\nresults.json\nafr_tag_overview.json\n```\n\n`results.json` contains the checker results (`<failure type>: <failure details>`) for each language tag, broken down by font.\n`afr_tag_overview.json` is a summary of which fonts in the library pass and fail for each language tag that was checked.\n\n\n# Setup\n\n## Requirements\n\n* Python 3.9+\n\n## Installation\n\nInstall it directly into an activated virtual environment:\n\n```text\n$ pip install shaperglot\n```\n\nor add it to your [Poetry](https://poetry.eustace.io/) project:\n\n```text\n$ poetry add shaperglot\n```\n\n# Usage\n\nAfter installation, the package can imported:\n\n```text\n$ python\n>>> import shaperglot\n>>> shaperglot.__version__\n```\n',
     'author': 'Simon Cozens',
     'author_email': 'simon@simon-cozens.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://pypi.org/project/shaperglot',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7',
 }
```

### Comparing `shaperglot-0.1.0/PKG-INFO` & `shaperglot-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaperglot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Test font files for OpenType language support
 Home-page: https://pypi.org/project/shaperglot
 License: MIT
 Author: Simon Cozens
 Author-email: simon@simon-cozens.org
 Requires-Python: >=3.7
 Classifier: Development Status :: 1 - Planning
@@ -12,18 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: gflanguages @ git+https://github.com/googlefonts/lang
+Requires-Dist: gflanguages (>=0.4.7)
 Requires-Dist: num2words (>=0.5,<0.6)
 Requires-Dist: protobuf (==3.19.4)
 Requires-Dist: strictyaml
 Requires-Dist: termcolor (==1.1.0)
 Requires-Dist: ufo2ft
 Requires-Dist: vharfbuzz (>=0,<1)
 Requires-Dist: youseedee
```

