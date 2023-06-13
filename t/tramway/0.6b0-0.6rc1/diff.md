# Comparing `tmp/tramway-0.6b0.tar.gz` & `tmp/tramway-0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tramway-0.6b0.tar", last modified: Tue Jun 29 15:36:32 2021, max compression
+gzip compressed data, was "tramway-0.6rc1.tar", last modified: Thu Jul 15 15:56:29 2021, max compression
```

## Comparing `tramway-0.6b0.tar` & `tramway-0.6rc1.tar`

### file list

```diff
@@ -1,241 +1,242 @@
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    21778 2020-10-07 12:39:57.000000 tramway-0.6b0/LICENSE
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1518 2021-06-29 15:36:32.007455 tramway-0.6b0/PKG-INFO
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      791 2021-06-28 16:57:27.000000 tramway-0.6b0/README.rst
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.983455 tramway-0.6b0/scripts/
--rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)       96 2020-10-28 13:27:19.000000 tramway-0.6b0/scripts/tramway
--rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)     1878 2021-04-01 19:35:15.000000 tramway-0.6b0/scripts/tramway-browse
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       63 2021-06-29 15:36:32.007455 tramway-0.6b0/setup.cfg
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2888 2021-06-22 14:20:29.000000 tramway-0.6b0/setup.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.983455 tramway-0.6b0/tramway/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      297 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    29726 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/__main__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.987455 tramway-0.6b0/tramway/analyzer/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    18794 2021-06-23 11:20:01.000000 tramway-0.6b0/tramway/analyzer/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.987455 tramway-0.6b0/tramway/analyzer/artefact/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8232 2021-03-01 21:23:34.000000 tramway-0.6b0/tramway/analyzer/artefact/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.987455 tramway-0.6b0/tramway/analyzer/attribute/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11571 2021-06-03 17:05:07.000000 tramway-0.6b0/tramway/analyzer/attribute/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      998 2020-12-14 12:03:41.000000 tramway-0.6b0/tramway/analyzer/attribute/abc.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/browser/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7540 2021-06-09 18:33:43.000000 tramway-0.6b0/tramway/analyzer/browser/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/env/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1979 2020-12-07 17:58:53.000000 tramway-0.6b0/tramway/analyzer/env/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1575 2020-12-06 23:18:37.000000 tramway-0.6b0/tramway/analyzer/env/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    74936 2021-06-28 10:54:23.000000 tramway-0.6b0/tramway/analyzer/env/environments.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5490 2021-02-24 12:29:44.000000 tramway-0.6b0/tramway/analyzer/env/ssh.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/images/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    23632 2021-06-03 15:56:27.000000 tramway-0.6b0/tramway/analyzer/images/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1366 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/images/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      207 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/images/allsymbols.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1788 2021-05-23 15:45:29.000000 tramway-0.6b0/tramway/analyzer/images/mpl.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/localizer/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2042 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/localizer/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      765 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/localizer/abc.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/mapper/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4199 2021-06-23 11:18:16.000000 tramway-0.6b0/tramway/analyzer/mapper/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      779 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/mapper/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      199 2021-06-23 11:06:37.000000 tramway-0.6b0/tramway/analyzer/mapper/allsymbols.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4251 2021-06-29 11:24:50.000000 tramway-0.6b0/tramway/analyzer/mapper/models.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    18889 2021-06-24 12:59:56.000000 tramway-0.6b0/tramway/analyzer/mapper/mpl.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4551 2021-06-14 19:27:28.000000 tramway-0.6b0/tramway/analyzer/mapper/plotly.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4758 2021-06-23 11:27:11.000000 tramway-0.6b0/tramway/analyzer/mapper/plugin.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1839 2020-12-31 15:05:29.000000 tramway-0.6b0/tramway/analyzer/mapper/utils.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/pipeline/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    14148 2021-06-03 18:04:22.000000 tramway-0.6b0/tramway/analyzer/pipeline/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16332 2021-06-14 19:50:47.000000 tramway-0.6b0/tramway/analyzer/pipeline/stages.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/roi/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    51168 2021-06-14 17:34:01.000000 tramway-0.6b0/tramway/analyzer/roi/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1606 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/roi/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      577 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/roi/allsymbols.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      890 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/roi/collections.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1259 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/roi/mpl.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11018 2021-03-25 22:36:11.000000 tramway-0.6b0/tramway/analyzer/roi/utils.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/sampler/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8835 2021-06-09 21:03:58.000000 tramway-0.6b0/tramway/analyzer/sampler/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      806 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/sampler/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      453 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/sampler/allsymbols.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/spt_data/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    56367 2021-06-14 08:34:00.000000 tramway-0.6b0/tramway/analyzer/spt_data/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4267 2020-12-06 23:18:37.000000 tramway-0.6b0/tramway/analyzer/spt_data/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      941 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/spt_data/allsymbols.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    13865 2021-06-10 09:23:18.000000 tramway-0.6b0/tramway/analyzer/spt_data/mpl.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/tesseller/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2287 2020-12-31 15:05:29.000000 tramway-0.6b0/tramway/analyzer/tesseller/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1413 2021-01-11 23:11:23.000000 tramway-0.6b0/tramway/analyzer/tesseller/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      305 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/tesseller/allsymbols.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7621 2021-06-10 09:27:03.000000 tramway-0.6b0/tramway/analyzer/tesseller/mpl.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2234 2020-12-31 15:05:29.000000 tramway-0.6b0/tramway/analyzer/tesseller/plugin.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/tesseller/post/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1732 2020-12-06 23:18:37.000000 tramway-0.6b0/tramway/analyzer/tesseller/post/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2605 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/tesseller/post/merger.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    13773 2021-05-26 17:21:58.000000 tramway-0.6b0/tramway/analyzer/tesseller/proxied.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11911 2021-06-09 20:01:15.000000 tramway-0.6b0/tramway/analyzer/tesseller/proxy.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.991455 tramway-0.6b0/tramway/analyzer/time/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16889 2021-06-09 23:31:42.000000 tramway-0.6b0/tramway/analyzer/time/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2113 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/time/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      219 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/time/allsymbols.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/analyzer/tracker/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8983 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/tracker/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      782 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/analyzer/tracker/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      229 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/analyzer/tracker/allsymbols.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/core/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      738 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/core/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/core/analyses/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       92 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/core/analyses/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1382 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/core/analyses/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12856 2021-02-01 13:11:10.000000 tramway-0.6b0/tramway/core/analyses/auto.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25708 2021-05-27 14:07:49.000000 tramway-0.6b0/tramway/core/analyses/base.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2494 2020-10-19 11:01:25.000000 tramway-0.6b0/tramway/core/analyses/browser.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7961 2021-02-01 13:32:39.000000 tramway-0.6b0/tramway/core/analyses/lazy.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4403 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/chain.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1058 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/core/exceptions.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/core/hdf5/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6212 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/hdf5/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3827 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/hdf5/compat.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6565 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/hdf5/rules.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7994 2021-02-08 14:16:58.000000 tramway-0.6b0/tramway/core/hdf5/store.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6511 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/lazy.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2418 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/namedcolumns.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/core/parallel/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25019 2021-05-27 14:05:47.000000 tramway-0.6b0/tramway/core/parallel/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4478 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/parallel/abc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4509 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/parallel/abc_py2.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9455 2021-05-27 14:21:07.000000 tramway-0.6b0/tramway/core/plugin.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1214 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/core/rc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16991 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/core/scaler.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    29600 2021-03-15 15:27:44.000000 tramway-0.6b0/tramway/core/xyt.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/feature/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        2 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12888 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/adjacency.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6654 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/curl.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/feature/single_traj/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      312 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11500 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/batch_extraction.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7311 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/batch_generation.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12116 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/distribution.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2702 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/misc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    36644 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/rw_features.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    14867 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/rw_misc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    31731 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/rw_simulation.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    20305 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/utils_supervised.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6463 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/vae.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12822 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/feature/single_traj/visualization.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.995455 tramway-0.6b0/tramway/helper/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      643 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/helper/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4103 2020-10-20 09:48:18.000000 tramway-0.6b0/tramway/helper/animation.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16462 2020-12-01 22:15:11.000000 tramway-0.6b0/tramway/helper/base.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    51535 2021-06-24 15:13:33.000000 tramway-0.6b0/tramway/helper/inference.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    39904 2021-05-21 12:50:24.000000 tramway-0.6b0/tramway/helper/roi.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.999455 tramway-0.6b0/tramway/helper/simulation/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      100 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/helper/simulation/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15634 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/helper/simulation/categoricaltrap.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    14503 2020-12-01 22:15:11.000000 tramway-0.6b0/tramway/helper/simulation/functional.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    77562 2021-06-09 20:01:27.000000 tramway-0.6b0/tramway/helper/tessellation.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.999455 tramway-0.6b0/tramway/inference/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3139 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    79374 2021-06-21 10:57:54.000000 tramway-0.6b0/tramway/inference/base.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.999455 tramway-0.6b0/tramway/inference/bayes_factors/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2610 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/bayes_factors/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    10748 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/inference/bayes_factors/calculate_bayes_factors.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9078 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/inference/bayes_factors/calculate_marginalized_integral.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5381 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/inference/bayes_factors/calculate_posteriors.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      192 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/bayes_factors/convenience_functions.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3762 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/bayes_factors/find_marginalized_zeta_t_roots.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4666 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/bayes_factors/get_D_posterior.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2525 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/bayes_factors/group_by_sign.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      904 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/bayes_factors/stopwatch.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16540 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/bayes_factors/test_calculate_bayes_factor.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1162 2021-06-28 09:10:04.000000 tramway-0.6b0/tramway/inference/d.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4655 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/d_conj_prior.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1250 2021-06-28 09:10:25.000000 tramway-0.6b0/tramway/inference/ddrift.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3107 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/density.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1236 2021-06-28 09:10:14.000000 tramway-0.6b0/tramway/inference/df.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15609 2021-06-23 10:15:45.000000 tramway-0.6b0/tramway/inference/dv.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9852 2020-12-01 15:27:04.000000 tramway-0.6b0/tramway/inference/fast_grad_dv.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    27312 2021-06-22 19:24:02.000000 tramway-0.6b0/tramway/inference/gradient.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    81287 2021-06-28 07:08:31.000000 tramway-0.6b0/tramway/inference/optimization.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2535 2021-06-29 14:39:33.000000 tramway-0.6b0/tramway/inference/semi_stochastic_dv.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9101 2021-05-27 14:17:05.000000 tramway-0.6b0/tramway/inference/snr.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3713 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/spherical_volume.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5051 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/inference/srtesseler_density.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8592 2021-06-23 10:15:47.000000 tramway-0.6b0/tramway/inference/standard_d.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7440 2021-06-23 10:16:58.000000 tramway-0.6b0/tramway/inference/standard_ddrift.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7954 2021-06-23 10:17:14.000000 tramway-0.6b0/tramway/inference/standard_df.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    26460 2021-06-27 17:31:56.000000 tramway-0.6b0/tramway/inference/stochastic_dv.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8299 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/inference/time.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4999 2021-06-28 09:07:59.000000 tramway-0.6b0/tramway/inference/unsmooth_d.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4194 2021-06-28 09:08:48.000000 tramway-0.6b0/tramway/inference/unsmooth_ddrift.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5637 2021-06-28 09:08:22.000000 tramway-0.6b0/tramway/inference/unsmooth_df.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.999455 tramway-0.6b0/tramway/localization/
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.999455 tramway-0.6b0/tramway/localization/UNet/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/localization/UNet/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25817 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/localization/UNet/inference.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2494 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/localization/UNet/tf.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3920 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/localization/UNet/utility_function_inference.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/localization/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/plot/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      118 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/plot/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/plot/animation/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6423 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/plot/animation/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5849 2020-10-28 13:27:19.000000 tramway-0.6b0/tramway/plot/animation/map.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5322 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/plot/animation/xyt.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/plot/bokeh/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       21 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/plot/bokeh/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25235 2021-06-24 12:59:37.000000 tramway-0.6b0/tramway/plot/bokeh/analyzer.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    24574 2021-04-13 13:35:49.000000 tramway-0.6b0/tramway/plot/bokeh/map.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    20679 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/plot/bokeh/roi.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12351 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/plot/contour.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    37695 2021-06-17 12:53:47.000000 tramway-0.6b0/tramway/plot/map.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    19820 2021-06-09 22:51:32.000000 tramway-0.6b0/tramway/plot/mesh.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/plot/tk/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/plot/tk/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12639 2021-05-27 14:20:29.000000 tramway-0.6b0/tramway/plot/tk/contour.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tessellation/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      772 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    84526 2021-06-22 09:27:14.000000 tramway-0.6b0/tramway/tessellation/base.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tessellation/grid/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9393 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/tessellation/grid/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tessellation/gwr/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16605 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/tessellation/gwr/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       35 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/gwr/dichotomy.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    43590 2021-01-07 22:21:16.000000 tramway-0.6b0/tramway/tessellation/gwr/gas.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tessellation/gwr/graph/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      832 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/gwr/graph/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    10722 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/tessellation/gwr/graph/array.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4064 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/gwr/graph/base.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6749 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/gwr/graph/dict.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1584 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/gwr/graph/exception.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15166 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/hexagon.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tessellation/kdtree/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9434 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/kdtree/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    10316 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/kdtree/dichotomy.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tessellation/kmeans/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6167 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/tessellation/kmeans/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8512 2021-01-11 23:11:23.000000 tramway-0.6b0/tramway/tessellation/kohonen.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12825 2021-05-27 14:19:19.000000 tramway-0.6b0/tramway/tessellation/nesting.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3914 2021-05-27 16:56:21.000000 tramway-0.6b0/tramway/tessellation/random.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    30129 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/tessellation/time.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16109 2021-02-08 23:51:00.000000 tramway-0.6b0/tramway/tessellation/utils2d.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3074 2020-10-19 09:04:09.000000 tramway-0.6b0/tramway/tessellation/window.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tracking/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/tracking/__init__.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/tracking/track_non_track/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/tracking/track_non_track/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16438 2020-12-14 21:10:36.000000 tramway-0.6b0/tramway/tracking/track_non_track/file_processing_loc.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4353 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/tracking/track_non_track/non_tracking_T_0.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:32.003455 tramway-0.6b0/tramway/utils/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/utils/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      136 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/utils/contour.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1672 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/utils/crop.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3728 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/utils/deconvolve.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    17805 2020-12-01 21:11:52.000000 tramway-0.6b0/tramway/utils/inferencemap.py
--rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)     2442 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/utils/mapviz.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1399 2020-11-04 18:08:04.000000 tramway-0.6b0/tramway/utils/mean_std.py
--rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)     2665 2020-10-07 12:39:57.000000 tramway-0.6b0/tramway/utils/trajviz.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-06-29 15:36:31.987455 tramway-0.6b0/tramway.egg-info/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1518 2021-06-29 15:36:31.000000 tramway-0.6b0/tramway.egg-info/PKG-INFO
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6532 2021-06-29 15:36:31.000000 tramway-0.6b0/tramway.egg-info/SOURCES.txt
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        1 2021-06-29 15:36:31.000000 tramway-0.6b0/tramway.egg-info/dependency_links.txt
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      159 2021-06-29 15:36:31.000000 tramway-0.6b0/tramway.egg-info/requires.txt
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        8 2021-06-29 15:36:31.000000 tramway-0.6b0/tramway.egg-info/top_level.txt
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    21778 2020-10-07 12:39:57.000000 tramway-0.6rc1/LICENSE
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1537 2021-07-15 15:56:29.651926 tramway-0.6rc1/PKG-INFO
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      791 2021-06-28 16:57:27.000000 tramway-0.6rc1/README.rst
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.623926 tramway-0.6rc1/scripts/
+-rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)       96 2020-10-28 13:27:19.000000 tramway-0.6rc1/scripts/tramway
+-rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)     1878 2021-04-01 19:35:15.000000 tramway-0.6rc1/scripts/tramway-browse
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       63 2021-07-15 15:56:29.651926 tramway-0.6rc1/setup.cfg
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2905 2021-07-15 15:03:39.000000 tramway-0.6rc1/setup.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.623926 tramway-0.6rc1/tramway/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      297 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    29726 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/__main__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.623926 tramway-0.6rc1/tramway/analyzer/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    18821 2021-07-07 17:59:04.000000 tramway-0.6rc1/tramway/analyzer/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.623926 tramway-0.6rc1/tramway/analyzer/artefact/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8232 2021-03-01 21:23:34.000000 tramway-0.6rc1/tramway/analyzer/artefact/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.623926 tramway-0.6rc1/tramway/analyzer/attribute/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11925 2021-07-04 14:55:19.000000 tramway-0.6rc1/tramway/analyzer/attribute/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      998 2020-12-14 12:03:41.000000 tramway-0.6rc1/tramway/analyzer/attribute/abc.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.623926 tramway-0.6rc1/tramway/analyzer/browser/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7540 2021-07-07 17:56:46.000000 tramway-0.6rc1/tramway/analyzer/browser/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.627926 tramway-0.6rc1/tramway/analyzer/env/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1979 2020-12-07 17:58:53.000000 tramway-0.6rc1/tramway/analyzer/env/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1575 2020-12-06 23:18:37.000000 tramway-0.6rc1/tramway/analyzer/env/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    75311 2021-07-15 13:54:10.000000 tramway-0.6rc1/tramway/analyzer/env/environments.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5490 2021-02-24 12:29:44.000000 tramway-0.6rc1/tramway/analyzer/env/ssh.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.627926 tramway-0.6rc1/tramway/analyzer/images/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    23749 2021-07-07 14:58:11.000000 tramway-0.6rc1/tramway/analyzer/images/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1366 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/images/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      210 2021-07-04 14:57:51.000000 tramway-0.6rc1/tramway/analyzer/images/allsymbols.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2626 2021-07-12 18:47:15.000000 tramway-0.6rc1/tramway/analyzer/images/draw.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2904 2021-07-12 20:32:24.000000 tramway-0.6rc1/tramway/analyzer/images/mpl.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.627926 tramway-0.6rc1/tramway/analyzer/localizer/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2042 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/localizer/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      765 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/localizer/abc.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.631926 tramway-0.6rc1/tramway/analyzer/mapper/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4199 2021-06-23 11:18:16.000000 tramway-0.6rc1/tramway/analyzer/mapper/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      779 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/mapper/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      202 2021-07-04 14:57:18.000000 tramway-0.6rc1/tramway/analyzer/mapper/allsymbols.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4251 2021-06-29 11:24:50.000000 tramway-0.6rc1/tramway/analyzer/mapper/models.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    19174 2021-07-09 09:40:28.000000 tramway-0.6rc1/tramway/analyzer/mapper/mpl.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4551 2021-06-14 19:27:28.000000 tramway-0.6rc1/tramway/analyzer/mapper/plotly.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4946 2021-07-07 18:02:26.000000 tramway-0.6rc1/tramway/analyzer/mapper/plugin.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1839 2020-12-31 15:05:29.000000 tramway-0.6rc1/tramway/analyzer/mapper/utils.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.631926 tramway-0.6rc1/tramway/analyzer/pipeline/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    14148 2021-06-03 18:04:22.000000 tramway-0.6rc1/tramway/analyzer/pipeline/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16332 2021-06-14 19:50:47.000000 tramway-0.6rc1/tramway/analyzer/pipeline/stages.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.631926 tramway-0.6rc1/tramway/analyzer/roi/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    51491 2021-07-04 15:06:00.000000 tramway-0.6rc1/tramway/analyzer/roi/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1606 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/roi/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      584 2021-07-04 14:44:35.000000 tramway-0.6rc1/tramway/analyzer/roi/allsymbols.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      890 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/roi/collections.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1259 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/roi/mpl.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11018 2021-03-25 22:36:11.000000 tramway-0.6rc1/tramway/analyzer/roi/utils.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.631926 tramway-0.6rc1/tramway/analyzer/sampler/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8835 2021-06-09 21:03:58.000000 tramway-0.6rc1/tramway/analyzer/sampler/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      806 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/sampler/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      458 2021-07-04 14:57:08.000000 tramway-0.6rc1/tramway/analyzer/sampler/allsymbols.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.631926 tramway-0.6rc1/tramway/analyzer/spt_data/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    59282 2021-07-07 17:55:45.000000 tramway-0.6rc1/tramway/analyzer/spt_data/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4267 2020-12-06 23:18:37.000000 tramway-0.6rc1/tramway/analyzer/spt_data/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      953 2021-07-04 14:56:17.000000 tramway-0.6rc1/tramway/analyzer/spt_data/allsymbols.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    13865 2021-06-10 09:23:18.000000 tramway-0.6rc1/tramway/analyzer/spt_data/mpl.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.631926 tramway-0.6rc1/tramway/analyzer/tesseller/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2287 2020-12-31 15:05:29.000000 tramway-0.6rc1/tramway/analyzer/tesseller/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1413 2021-01-11 23:11:23.000000 tramway-0.6rc1/tramway/analyzer/tesseller/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      308 2021-07-04 14:56:46.000000 tramway-0.6rc1/tramway/analyzer/tesseller/allsymbols.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7621 2021-06-10 09:27:03.000000 tramway-0.6rc1/tramway/analyzer/tesseller/mpl.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2234 2020-12-31 15:05:29.000000 tramway-0.6rc1/tramway/analyzer/tesseller/plugin.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.635926 tramway-0.6rc1/tramway/analyzer/tesseller/post/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1732 2020-12-06 23:18:37.000000 tramway-0.6rc1/tramway/analyzer/tesseller/post/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2605 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/tesseller/post/merger.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    13773 2021-05-26 17:21:58.000000 tramway-0.6rc1/tramway/analyzer/tesseller/proxied.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11911 2021-06-09 20:01:15.000000 tramway-0.6rc1/tramway/analyzer/tesseller/proxy.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.635926 tramway-0.6rc1/tramway/analyzer/time/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16889 2021-06-09 23:31:42.000000 tramway-0.6rc1/tramway/analyzer/time/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2113 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/time/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      222 2021-07-04 14:56:59.000000 tramway-0.6rc1/tramway/analyzer/time/allsymbols.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.635926 tramway-0.6rc1/tramway/analyzer/tracker/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9627 2021-07-12 14:44:45.000000 tramway-0.6rc1/tramway/analyzer/tracker/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      782 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/analyzer/tracker/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      232 2021-07-04 14:56:27.000000 tramway-0.6rc1/tramway/analyzer/tracker/allsymbols.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.635926 tramway-0.6rc1/tramway/core/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      738 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/core/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.635926 tramway-0.6rc1/tramway/core/analyses/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       92 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/core/analyses/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1382 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/core/analyses/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12856 2021-02-01 13:11:10.000000 tramway-0.6rc1/tramway/core/analyses/auto.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25708 2021-05-27 14:07:49.000000 tramway-0.6rc1/tramway/core/analyses/base.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2494 2020-10-19 11:01:25.000000 tramway-0.6rc1/tramway/core/analyses/browser.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7961 2021-02-01 13:32:39.000000 tramway-0.6rc1/tramway/core/analyses/lazy.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4403 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/chain.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1058 2020-12-14 21:10:36.000000 tramway-0.6rc1/tramway/core/exceptions.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.639926 tramway-0.6rc1/tramway/core/hdf5/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6212 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/hdf5/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3827 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/hdf5/compat.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6565 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/hdf5/rules.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7994 2021-02-08 14:16:58.000000 tramway-0.6rc1/tramway/core/hdf5/store.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6511 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/lazy.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2418 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/namedcolumns.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.639926 tramway-0.6rc1/tramway/core/parallel/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25019 2021-05-27 14:05:47.000000 tramway-0.6rc1/tramway/core/parallel/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4478 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/parallel/abc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4509 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/parallel/abc_py2.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9455 2021-05-27 14:21:07.000000 tramway-0.6rc1/tramway/core/plugin.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1214 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/core/rc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16991 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/core/scaler.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    29616 2021-07-04 13:50:58.000000 tramway-0.6rc1/tramway/core/xyt.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.639926 tramway-0.6rc1/tramway/feature/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        2 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12888 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/adjacency.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6654 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/curl.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.639926 tramway-0.6rc1/tramway/feature/single_traj/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      312 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11500 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/batch_extraction.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7311 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/batch_generation.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12116 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/distribution.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2702 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/misc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    36644 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/rw_features.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    14867 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/rw_misc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    31731 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/rw_simulation.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    20305 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/utils_supervised.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6463 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/vae.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12822 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/feature/single_traj/visualization.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.643926 tramway-0.6rc1/tramway/helper/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      643 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/helper/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4103 2020-10-20 09:48:18.000000 tramway-0.6rc1/tramway/helper/animation.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16462 2020-12-01 22:15:11.000000 tramway-0.6rc1/tramway/helper/base.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    52101 2021-07-09 09:40:27.000000 tramway-0.6rc1/tramway/helper/inference.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    39904 2021-05-21 12:50:24.000000 tramway-0.6rc1/tramway/helper/roi.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.643926 tramway-0.6rc1/tramway/helper/simulation/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      100 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/helper/simulation/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15634 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/helper/simulation/categoricaltrap.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15222 2021-07-09 11:31:07.000000 tramway-0.6rc1/tramway/helper/simulation/functional.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    77562 2021-06-09 20:01:27.000000 tramway-0.6rc1/tramway/helper/tessellation.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.643926 tramway-0.6rc1/tramway/inference/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3139 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    79374 2021-06-21 10:57:54.000000 tramway-0.6rc1/tramway/inference/base.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/inference/bayes_factors/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2610 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/bayes_factors/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    10748 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/inference/bayes_factors/calculate_bayes_factors.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9078 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/inference/bayes_factors/calculate_marginalized_integral.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5381 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/inference/bayes_factors/calculate_posteriors.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      192 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/bayes_factors/convenience_functions.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3762 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/bayes_factors/find_marginalized_zeta_t_roots.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4666 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/bayes_factors/get_D_posterior.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2525 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/bayes_factors/group_by_sign.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      904 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/bayes_factors/stopwatch.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16540 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/bayes_factors/test_calculate_bayes_factor.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1162 2021-06-28 09:10:04.000000 tramway-0.6rc1/tramway/inference/d.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4655 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/d_conj_prior.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1250 2021-06-28 09:10:25.000000 tramway-0.6rc1/tramway/inference/ddrift.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3107 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/density.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1236 2021-06-28 09:10:14.000000 tramway-0.6rc1/tramway/inference/df.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15609 2021-06-23 10:15:45.000000 tramway-0.6rc1/tramway/inference/dv.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9852 2020-12-01 15:27:04.000000 tramway-0.6rc1/tramway/inference/fast_grad_dv.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    27312 2021-06-22 19:24:02.000000 tramway-0.6rc1/tramway/inference/gradient.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    81287 2021-06-28 07:08:31.000000 tramway-0.6rc1/tramway/inference/optimization.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2535 2021-06-29 14:39:33.000000 tramway-0.6rc1/tramway/inference/semi_stochastic_dv.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9101 2021-05-27 14:17:05.000000 tramway-0.6rc1/tramway/inference/snr.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3713 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/spherical_volume.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5051 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/inference/srtesseler_density.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8592 2021-06-23 10:15:47.000000 tramway-0.6rc1/tramway/inference/standard_d.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7440 2021-06-23 10:16:58.000000 tramway-0.6rc1/tramway/inference/standard_ddrift.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7954 2021-06-23 10:17:14.000000 tramway-0.6rc1/tramway/inference/standard_df.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    26460 2021-06-27 17:31:56.000000 tramway-0.6rc1/tramway/inference/stochastic_dv.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8299 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/inference/time.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4999 2021-06-28 09:07:59.000000 tramway-0.6rc1/tramway/inference/unsmooth_d.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4194 2021-06-28 09:08:48.000000 tramway-0.6rc1/tramway/inference/unsmooth_ddrift.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5637 2021-06-28 09:08:22.000000 tramway-0.6rc1/tramway/inference/unsmooth_df.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/localization/
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/localization/UNet/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/localization/UNet/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25817 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/localization/UNet/inference.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2494 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/localization/UNet/tf.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3920 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/localization/UNet/utility_function_inference.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/localization/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/plot/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      118 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/plot/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/plot/animation/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6423 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/plot/animation/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5849 2020-10-28 13:27:19.000000 tramway-0.6rc1/tramway/plot/animation/map.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     5322 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/plot/animation/xyt.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/plot/bokeh/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       21 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/plot/bokeh/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    25460 2021-07-09 09:43:32.000000 tramway-0.6rc1/tramway/plot/bokeh/analyzer.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    24574 2021-04-13 13:35:49.000000 tramway-0.6rc1/tramway/plot/bokeh/map.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    20679 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/plot/bokeh/roi.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12351 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/plot/contour.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    37695 2021-06-17 12:53:47.000000 tramway-0.6rc1/tramway/plot/map.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    19820 2021-06-09 22:51:32.000000 tramway-0.6rc1/tramway/plot/mesh.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/plot/tk/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/plot/tk/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12639 2021-05-27 14:20:29.000000 tramway-0.6rc1/tramway/plot/tk/contour.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/tessellation/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      772 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    84526 2021-06-22 09:27:14.000000 tramway-0.6rc1/tramway/tessellation/base.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.647926 tramway-0.6rc1/tramway/tessellation/grid/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9393 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/tessellation/grid/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/tramway/tessellation/gwr/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16605 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/tessellation/gwr/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       35 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/gwr/dichotomy.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    43590 2021-01-07 22:21:16.000000 tramway-0.6rc1/tramway/tessellation/gwr/gas.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/tramway/tessellation/gwr/graph/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      832 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/gwr/graph/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    10722 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/tessellation/gwr/graph/array.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4064 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/gwr/graph/base.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6749 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/gwr/graph/dict.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1584 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/gwr/graph/exception.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15166 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/hexagon.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/tramway/tessellation/kdtree/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9434 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/kdtree/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    10316 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/kdtree/dichotomy.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/tramway/tessellation/kmeans/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6167 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/tessellation/kmeans/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     8512 2021-01-11 23:11:23.000000 tramway-0.6rc1/tramway/tessellation/kohonen.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    12825 2021-05-27 14:19:19.000000 tramway-0.6rc1/tramway/tessellation/nesting.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3914 2021-05-27 16:56:21.000000 tramway-0.6rc1/tramway/tessellation/random.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    30129 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/tessellation/time.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16109 2021-02-08 23:51:00.000000 tramway-0.6rc1/tramway/tessellation/utils2d.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3074 2020-10-19 09:04:09.000000 tramway-0.6rc1/tramway/tessellation/window.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/tramway/tracking/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/tracking/__init__.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/tramway/tracking/track_non_track/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/tracking/track_non_track/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    16438 2020-12-14 21:10:36.000000 tramway-0.6rc1/tramway/tracking/track_non_track/file_processing_loc.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     4353 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/tracking/track_non_track/non_tracking_T_0.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.651926 tramway-0.6rc1/tramway/utils/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        0 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/utils/__init__.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      136 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/utils/contour.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1672 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/utils/crop.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3728 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/utils/deconvolve.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    17805 2020-12-01 21:11:52.000000 tramway-0.6rc1/tramway/utils/inferencemap.py
+-rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)     2442 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/utils/mapviz.py
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1399 2020-11-04 18:08:04.000000 tramway-0.6rc1/tramway/utils/mean_std.py
+-rwxrwxr-x   0 flaurent  (1000) flaurent  (1000)     2665 2020-10-07 12:39:57.000000 tramway-0.6rc1/tramway/utils/trajviz.py
+drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2021-07-15 15:56:29.623926 tramway-0.6rc1/tramway.egg-info/
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1537 2021-07-15 15:56:28.000000 tramway-0.6rc1/tramway.egg-info/PKG-INFO
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     6564 2021-07-15 15:56:28.000000 tramway-0.6rc1/tramway.egg-info/SOURCES.txt
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        1 2021-07-15 15:56:28.000000 tramway-0.6rc1/tramway.egg-info/dependency_links.txt
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      159 2021-07-15 15:56:28.000000 tramway-0.6rc1/tramway.egg-info/requires.txt
+-rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        8 2021-07-15 15:56:28.000000 tramway-0.6rc1/tramway.egg-info/top_level.txt
```

### Comparing `tramway-0.6b0/LICENSE` & `tramway-0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/PKG-INFO` & `tramway-0.6rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tramway
-Version: 0.6b0
+Version: 0.6rc1
 Summary: TRamWAy
 Home-page: https://github.com/DecBayComp/TRamWAy
-Author: François Laurent
+Author: Institut Pasteur, François Laurent
 Author-email: francois.laurent@pasteur.fr
 License: CECILL-2.1
 Description: TRamWAy
         =======
         
         *TRamWAy* helps analyzing single molecule dynamics.
         It infers the diffusivity, drift, force and potential energy across space and time.
```

### Comparing `tramway-0.6b0/README.rst` & `tramway-0.6rc1/README.rst`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/scripts/tramway-browse` & `tramway-0.6rc1/scripts/tramway-browse`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/setup.py` & `tramway-0.6rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 # Get the long description from the README file
 with open(path.join(pwd, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'tramway',
-    version = '0.6-beta',
+    version = '0.6-rc1',
     description = 'TRamWAy',
     long_description = long_description,
     url = 'https://github.com/DecBayComp/TRamWAy',
-    author = 'François Laurent',
+    author = 'Institut Pasteur, François Laurent',
     author_email = 'francois.laurent@pasteur.fr',
     license = 'CECILL-2.1',
     classifiers = [
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `tramway-0.6b0/tramway/__main__.py` & `tramway-0.6rc1/tramway/__main__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/__init__.py` & `tramway-0.6rc1/tramway/analyzer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 def report_misplaced_attribute(attr_name, proper_parent_name):
     warnings.warn(f'`{attr_name}` is an attribute of the initialized `{proper_parent_name}` attribute; this warning message can safely be silenced', MisplacedAttributeWarning)
 def proper_parent_name(attr_name):
     parent_name = None
     get_conditions, set_conditions = {}, {}
     set_conditions['initialized'] = True
     if attr_name in ('dt', 'time_step', 'frame_interval',
-            'localization_error', 'localization_precision', 'columns'):
+            'localization_error', 'localization_precision', 'columns',
+            'temperature'):
         parent_name = 'spt_data'
     elif attr_name in ('scaler', 'resolution'):
         parent_name = 'tesseller'
     elif attr_name in ('script',):
         parent_name = 'env'
     return parent_name, get_conditions, set_conditions
```

### Comparing `tramway-0.6b0/tramway/analyzer/artefact/__init__.py` & `tramway-0.6rc1/tramway/analyzer/artefact/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/attribute/__init__.py` & `tramway-0.6rc1/tramway/analyzer/attribute/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 
 from .abc import *
 import numpy as np
 from collections.abc import Iterable, Sequence, Set
 import logging
+import functools
 
 __all__ = ['GenericAttribute', 'Attribute']
 
 __all__.append('WithLogger')
 class WithLogger(object):
     __slots__ = ('_logger',)
     def __init__(self):
@@ -354,7 +355,19 @@
         except:
             raise AttributeError("cannot find a proper initializer for the '{}' attribute".format(self.attrname))
         attr = getattr(type(parent_analyzer), self.attrname)
         # TODO: add a freset method to the properties returned by selfinitializing_property
         attr.fset(parent_analyzer, cls)
         self.assign( parent_analyzer )
 
+__all__.append('initializer_method')
+def initializer_method(method, attrname=None):
+    """
+    Properly set the docstring for the wrapped method.
+    """
+    meth = InitializerMethod(method, attrname)
+    @functools.wraps(method)
+    def wrapped_method(*args, **kwargs):
+        return meth(*args, **kwargs)
+    return wrapped_method
+
+
```

### Comparing `tramway-0.6b0/tramway/analyzer/attribute/abc.py` & `tramway-0.6rc1/tramway/analyzer/attribute/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/browser/__init__.py` & `tramway-0.6rc1/tramway/analyzer/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/env/__init__.py` & `tramway-0.6rc1/tramway/analyzer/env/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/env/abc.py` & `tramway-0.6rc1/tramway/analyzer/env/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/env/environments.py` & `tramway-0.6rc1/tramway/analyzer/env/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1068,15 +1068,15 @@
                 time.sleep(self.refresh_interval)
         except:
             self.logger.info('killing jobs with: scancel '+self.job_id)
             subprocess.Popen(('scancel', self.job_id)).communicate()
             raise
 
 
-__remote_host_attrs__ = ('_ssh','_local_data_location','_remote_data_location','_directory_mapping','_remote_dependencies')
+__remote_host_attrs__ = ('_ssh','_local_data_location','_remote_data_location','_directory_mapping')
 
 class RemoteHost(object):
     """
     mixin class.
 
     children classes should define attributes listed in `__remote_host_attrs__`.
 
@@ -1115,15 +1115,14 @@
     """
     __slots__ = ()
     def __init__(self):
         self._ssh = None
         self._local_data_location = None
         self._remote_data_location = None
         self._directory_mapping = {}
-        self._remote_dependencies = None
     @property
     def ssh(self):
         """
         SSH communication interface.
 
         See also :class:`~tramway.analyzer.env.ssh.Client`.
         """
@@ -1173,23 +1172,14 @@
         Directory mapping with local paths as keys
         and the corresponding remote paths as values.
 
         Paths should not have slashes at the end.
         """
         return self._directory_mapping
     @property
-    def remote_dependencies(self):
-        """
-        Command to be run before batch submission.
-        """
-        return self._remote_dependencies
-    @remote_dependencies.setter
-    def remote_dependencies(self, deps):
-        self._remote_dependencies = deps
-    @property
     def collection_interpreter(self):
         return self.interpreter
     @property
     def wd_is_available(self):
         return self.worker_side
     def make_working_directory(self):
         if self.submit_side:
@@ -1248,18 +1238,21 @@
             #    dest = dest[:-5]+'py'
             dest = '/'.join((self.wd, dest))
             attrs = self.ssh.put(src, dest)
             self.logger.debug(attrs)
             self.script = dest
             self.logger.info('Python script location: '+dest)
             return True
+    @classmethod
+    def remote_dependencies(cls):
+        return None
     def exec_inline_python(self, inline_code):
         python = []
-        if self.remote_dependencies:
-            python.append(self.remote_dependencies)
+        if self.remote_dependencies():
+            python.append(self.remote_dependencies())
         python.append(self.collection_interpreter)
         python = '; '.join(python)
         return self.ssh.exec('{} -c "{}"'.format(python, inline_code.replace('"', r'\"')), shell=True, logger=self.logger)
     @classmethod
     def _collectible_prefix(cls, stage_index=None):
         """
         Computes the starting substring of the log message that reports
@@ -1320,16 +1313,18 @@
         local_script = self.make_temporary_file(suffix='.py', text=True)
         with open(local_script, 'w') as f:
             f.write(code)
         remote_script = '/'.join((self.wd, os.path.basename(local_script)))
         attrs = self.ssh.put(local_script, remote_script, confirm=True)
         self.logger.debug(attrs)
         log_file = os.path.splitext(remote_script)[0]+'.log'
-        cmd = '{}{} {}; rm {}'.format(
-                '' if self.remote_dependencies is None else self.remote_dependencies+'; ',
+        remote_deps = self.remote_dependencies()
+        if remote_deps and not remote_deps.rstrip().endswith(';'):
+            remote_deps = remote_deps+'; '
+        cmd = '{}{} {}; rm {}'.format(remote_deps,
                 self.collection_interpreter, remote_script, remote_script)
         out, err = self.ssh.exec(cmd, shell=True, logger=self.logger)
         out, err = out.rstrip(), err.rstrip()
         if err:
             if out:
                 self.logger.debug(out)
             self.logger.error(err)
@@ -1485,16 +1480,16 @@
         sbatch_script = self.make_sbatch_script()
         dest = '/'.join((self.wd, os.path.basename(sbatch_script)))
         attrs = self.ssh.put(sbatch_script, dest)
         self.logger.debug(attrs)
         self.logger.info('sbatch script transferred to: '+dest)
         #self.logger.info('running: module load singularity')
         #out, err = self.ssh.exec('module load singularity')
-        if self.remote_dependencies:
-            cmd = self.remote_dependencies+'; sbatch '+dest
+        if self.remote_dependencies():
+            cmd = self.remote_dependencies()+'; sbatch '+dest
         else:
             cmd = 'sbatch '+dest
         self.logger.info('running: '+cmd)
         out, err = self.ssh.exec(cmd, shell=True)
         if out:
             out = out.rstrip()
             self.logger.debug(out)
@@ -1745,29 +1740,36 @@
 Environment.register(SlurmOverSSH)
 
 
 class SingularitySlurm(SlurmOverSSH):
     """
     Runs TRamWAy jobs as Slurm jobs in a Singularity container.
 
-    The current default Singularity container is *tramway-hpc-210628.sif*.
+    The current default Singularity container is *tramway-hpc-210715.sif*.
     See also `available_images.rst <https://github.com/DecBayComp/TRamWAy/blob/master/containers/available_images.rst>`_.
 
     Children classes should define the :meth:`hostname` and :meth:`scratch` methods.
     They can be defined as standard methods or class methods.
     """
     @classmethod
     def hostname(cls):
         raise NotImplementedError
     @classmethod
     def scratch(cls, username):
         raise NotImplementedError
+    @classmethod
+    def singularity_options(cls):
+        return ''
     def __init__(self, **kwargs):
         SlurmOverSSH.__init__(self, **kwargs)
-        self.interpreter = 'singularity exec -H $HOME -B /pasteur tramway-hpc-210628.sif python3.6 -s'
+        singularity_options = self.singularity_options()
+        if singularity_options and singularity_options[0] != ' ':
+            singularity_options = ' '+singularity_options
+        default_container = self.default_container()
+        self.interpreter = f'singularity exec -H $HOME{singularity_options} {default_container} python3.6 -s'
         self.ssh.host = self.hostname()
     @property
     def username(self):
         try:
             username, _ = self.ssh.host.split('@')
         except (AttributeError, ValueError):
             import getpass
@@ -1803,15 +1805,19 @@
                 'tramway-hpc-210222.sif':   'http://dl.pasteur.fr/fop/rzx2LnjB/tramway-hpc-210222.sif',
                 'tramway-hpc-210301.sif':   'http://dl.pasteur.fr/fop/7jSSZCnb/tramway-hpc-210301.sif',
                 'tramway-hpc-210302.sif':   'http://dl.pasteur.fr/fop/53bfSkmM/tramway-hpc-210302.sif',
                 'tramway-hpc-210330.sif':   'http://dl.pasteur.fr/fop/FrDZQBuy/tramway-hpc-210330.sif',
                 'tramway-hpc-210527.sif':   'http://dl.pasteur.fr/fop/7F0LaOEX/tramway-hpc-210527.sif',
                 'tramway-hpc-210608.sif':   'http://dl.pasteur.fr/fop/5LCsGe80/tramway-hpc-210608.sif',
                 'tramway-hpc-210628.sif':   'http://dl.pasteur.fr/fop/Cr969IPb/tramway-hpc-210628.sif',
+                'tramway-hpc-210715.sif':   'http://dl.pasteur.fr/fop/lzFiPalM/tramway-hpc-210715.sif',
                 }.get(container, None)
+    @classmethod
+    def default_container(cls):
+        return 'tramway-hpc-210715.sif'
     def setup(self, *argv, **kwargs):
         SlurmOverSSH.setup(self, *argv, **kwargs)
         if self.submit_side:
             self.ssh.download_if_missing(self.container, self.get_container_url(), self.logger)
     @property
     def working_directory(self):
         if self._working_directory is None:
@@ -1831,17 +1837,20 @@
     """
     @classmethod
     def hostname(cls):
         return 'tars.pasteur.fr'
     @classmethod
     def scratch(cls, username):
         return os.path.join('/pasteur/scratch/users', username)
-    def __init__(self, **kwargs):
-        SingularitySlurm.__init__(self, **kwargs)
-        self.remote_dependencies = 'module load singularity'
+    @classmethod
+    def singularity_options(cls):
+        return ' -B /pasteur'
+    @classmethod
+    def remote_dependencies(cls):
+        return 'module load singularity'
 
 
 class GPULab(SingularitySlurm):
     """
     Designed for server *adm.inception.hubbioit.pasteur.fr*.
     """
     @classmethod
@@ -1861,14 +1870,17 @@
     """
     @classmethod
     def hostname(cls):
         return 'maestro.pasteur.fr'
     @classmethod
     def scratch(cls, username):
         return os.path.join('/pasteur/sonic/scratch/users', username)
-    def __init__(self, **kwargs):
-        SingularitySlurm.__init__(self, **kwargs)
-        self.remote_dependencies = 'module load singularity'
+    @classmethod
+    def singularity_options(cls):
+        return ' -B /pasteur'
+    @classmethod
+    def remote_dependencies(cls):
+        return 'module load singularity'
 
 
 __all__ = ['Environment', 'LocalHost', 'SlurmOverSSH', 'Tars', 'GPULab', 'Maestro']
```

### Comparing `tramway-0.6b0/tramway/analyzer/env/ssh.py` & `tramway-0.6rc1/tramway/analyzer/env/ssh.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/images/__init__.py` & `tramway-0.6rc1/tramway/analyzer/images/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                 yield t, frame[i_min:i_max, j_min:j_max]
         else:
             for frame in self.as_frames(index, return_time):
                 yield frame[i_min:i_max, j_min:j_max]
 
     def to_color_movie(self, output_file=None, fourcc='VP80', colormap='gray',
             locations=None, trajectories=None, frames=None, origin=None,
-            markersize=2, linecolor='many', linewidth=1,
+            markersize=2, linecolor='many', linewidth=None,
             magnification=None, playback_rate=None, light_intensity=1.):
         """
         Generates a movie of the images with overlaid locations or trajectories.
 
         Arguments:
 
             output_file (str): path of the movie file.
@@ -237,15 +237,15 @@
                 `origin` is useful only for overlaying locations or trajectories.
 
             markersize (int): location marker size in pixels (square side).
 
             linecolor (*str* or 3-column float array): color for trajectories;
                 value :const:`None` defaults to red.
 
-            linewidth (float): trajectory line width (not supported yet)
+            linewidth (int or float): trajectory line width
 
             magnification (*int* or *str*): the original image pixels can be represented as
                 square-patches of `magnification` video pixel side;
                 if *str*:
                 :const:`'1x'` = `round(pixel_size/localization_precision)`,
                 :const:`'2x'` = `round(2*pixel_size/localization_precision)`;
                 :const:`'2x'` is adequate for overlaid trajectories, even with the over-compressing
@@ -257,15 +257,15 @@
             light_intensity (float): scale the pixel intensity values;
                 works best with the 'gray' colormap.
 
         """
         import cv2
         # TODO: support PIL as an optional replacement for skimage
         from skimage.util import img_as_ubyte
-        from skimage import draw
+        from . import draw
         from matplotlib import cm, colors
 
         if output_file is None:
             try:
                 output_file = os.path.splitext(self.filepath)[0]+'.avi'
             except AttributeError:
                 raise ValueError('output_file is not defined')
@@ -401,31 +401,19 @@
                 frame = frame // color_scale
 
             frame = colormap(frame)[:,:,:3]
 
             if magnification:
                 frame = np.repeat(np.repeat(frame, magnification, axis=0), magnification, axis=1)
 
-            if locations is not None:
-                xy = locations[ isclose(locations['t'], t) ]
-                if xy0 is None:
-                    xy_f = xy[list('xy')].values / vid_pxsize - vid_offset
-                else:
-                    xy_f = (xy[list('xy')].values - xy0) / vid_pxsize + mag_offset
-                for j,i in xy_f:
-                    i = np.array([_floor(i), _ceil(i)], dtype=np.int)
-                    j = np.array([_floor(j), _ceil(j)], dtype=np.int)
-                    if np.any(i<0) or np.any(j<0):
-                        continue
-                    i,j = np.meshgrid(
-                            np.arange(i[0],i[1]+1),
-                            np.arange(j[0],j[1]+1), indexing='ij')
-                    frame[ii_max-np.ravel(i),np.ravel(j),:] = marker_color
-
             if trajectories is not None:
+                # anti-aliasing
+                lw = 0 if linewidth is None else linewidth
+                aa = bool(linewidth)
+
                 # get the ids of the active trajectories for frame f
                 active_trajectories = trajectories['n'][ isclose(trajectories['t'], t) ]
                 assert all_unique(active_trajectories)
 
                 # extract the corresponding coordinate series truncated at time t
                 trajs_f = []
                 for n in active_trajectories:
@@ -438,33 +426,52 @@
                         continue
                     if xy0 is None:
                         traj = xy_n.values / vid_pxsize - vid_offset
                     else:
                         traj = (xy_n.values - xy0) / vid_pxsize + mag_offset
                     if np.any(traj < 0): # this may occur with negative offsets
                         continue
-                    traj = np.round(traj).astype(np.uint32)
+                    if not aa:
+                        traj = np.round(traj).astype(np.uint32)
                     trajs_f.append((n, traj))
 
                 # overlay the truncated trajectories
                 if trajs_f:
-                    # TODO: draw a proper polyline with unique ii and jj and max(kk)
                     jj, ii, kk, nn = zip(*[ append_n(n,
-                            draw.line_aa(traj[p,0], traj[p,1], traj[p+1,0], traj[p+1,1])
-                        ) for n, traj in trajs_f for p in range(traj.shape[0]-1) ])
+                        draw.multiline_aa(traj[:,0], traj[:,1], thickness=lw)
+                        ) for n, traj in trajs_f ])
                     ii = np.concatenate(ii)
                     jj = np.concatenate(jj)
                     ok = (0<=ii)&(ii<=ii_max)&(0<=jj)&(jj<=jj_max)
                     ii, jj = ii[ok], jj[ok]
                     kk = np.concatenate(kk)[ok][:,np.newaxis]
                     if 1<len(line_color):
                         nn = np.concatenate(nn)[ok]
                         lc = line_color[nn % len(line_color)]
                     frame[ii_max-ii,jj,:] = (1.-kk) * frame[ii_max-ii,jj,:] + kk * lc
 
+            if locations is not None:
+                xy = locations[ isclose(locations['t'], t) ]
+                if xy0 is None:
+                    xy_f = xy[list('xy')].values / vid_pxsize - vid_offset
+                else:
+                    xy_f = (xy[list('xy')].values - xy0) / vid_pxsize + mag_offset
+                for j,i in xy_f:
+                    i = np.array([_floor(i), _ceil(i)], dtype=np.int)
+                    j = np.array([_floor(j), _ceil(j)], dtype=np.int)
+                    if np.any(i<0) or np.any(j<0):
+                        continue
+                    i,j = np.meshgrid(
+                            np.arange(i[0],i[1]+1),
+                            np.arange(j[0],j[1]+1), indexing='ij')
+                    try:
+                        frame[ii_max-np.ravel(i),np.ravel(j),:] = marker_color
+                    except IndexError:
+                        pass
+
             vid.write(img_as_ubyte(frame)[:,:,::-1])
         vid.release()
 
     @property
     def _mpl_impl(self):
         from .mpl import Mpl
         return Mpl
```

### Comparing `tramway-0.6b0/tramway/analyzer/images/abc.py` & `tramway-0.6rc1/tramway/analyzer/images/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/images/mpl.py` & `tramway-0.6rc1/tramway/analyzer/images/mpl.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,10 +51,41 @@
         x /= img.pixel_size
         y /= img.pixel_size
         if origin is None and img.loc_offset is not None:
             x -= img.loc_offset[0]
             y -= img.loc_offset[1]
         return axes.plot(x, height-1-y, *args, **kwargs)
 
+    def roi(self, frame, origin, *args, axes=None, colormap='gray', **kwargs):
+        """
+        Plots a frame corresponding to a region of interest.
+
+        `origin` should be provided by :meth:`cropping_bounds`,
+        if `frame` is given by :meth:`crop_frames`.
+
+        Extra input arguments are passed to the :func:`imshow` function.
+
+        This method works in combination with :meth:`spt_data.mpl.Mpl.plot`.
+        """
+        m, n = frame.shape
+        px = self._parent.pixel_size
+        x0, y0 = origin[0] - .5 * px, origin[1] - .5 * px
+        x1, y1 = origin[0] + (m - .5) * px, origin[1] + (n - .5) * px
+        try:
+            colormap = kwargs.pop('cmap')
+        except KeyError:
+            pass
+        for arg in ('origin', 'extent'):
+            try:
+                kwargs.pop(arg)
+            except KeyError:
+                pass
+            else:
+                self.logger.warning(f"argument '{arg}' ignored")
+        if axes is None:
+            import matplotlib.pyplot as axes
+        return axes.imshow(frame, cmap=colormap, extent=[x0, x1, y0, y1],
+                **kwargs)
+
 
 __all__ = ['Mpl']
```

### Comparing `tramway-0.6b0/tramway/analyzer/localizer/__init__.py` & `tramway-0.6rc1/tramway/analyzer/localizer/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/localizer/abc.py` & `tramway-0.6rc1/tramway/analyzer/localizer/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/mapper/__init__.py` & `tramway-0.6rc1/tramway/analyzer/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/mapper/abc.py` & `tramway-0.6rc1/tramway/analyzer/mapper/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/mapper/models.py` & `tramway-0.6rc1/tramway/analyzer/mapper/models.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/mapper/mpl.py` & `tramway-0.6rc1/tramway/analyzer/mapper/mpl.py`

 * *Files 5% similar despite different names*

```diff
@@ -296,27 +296,33 @@
         try:
             unit = kwargs.pop('unit')
         except KeyError:
             pass
         else:
             if unit == 'std':
                 if logscale is True:
-                    scale = lambda u: 'log[{}]'.format(u)
+                    scale = lambda u: f'log. {u}'
                 else:
                     scale = lambda u: u
+                # standard units are defined at multiple locations:
+                # * tramway.plot.bokeh.analyzer.Controller.draw_map
+                # * tramway.helper.inference.map_plot
+                # * tramway.analyzer.mapper.mpl.Mpl.clabel
                 unit = dict(
-                        diffusivity=scale('$\mu\\rm{m}^2\\rm{s}^{-1}$'),
-                        potential=scale('$[k_{\\rm{B}}T]$'),
-                        force='Amplitude' if logscale is False else 'Log. amplitude',
-                        drift=scale('$\mu\\rm{m}\\rm{s}^{-1}$'),
+                        diffusivity=scale(r'$\mu\rm{m}^2\rm{s}^{-1}$'),
+                        potential=scale(r'$k_{\rm{B}}T$'),
+                        force=('Log. ' if logscale else '')+\
+                            r'$k_{\rm{B}}T\mu\rm{m}^{-1}$',
+                        drift=scale(r'$\mu\rm{m}\rm{s}^{-1}$'),
                     ).get(feature, None)
             if unit is not None:
                 map_kwargs['unit'] = unit
-    def animate(self, fig, maps, feature, sampling=None, overlay_locations=False,
-            axes=None, aspect='equal', logscale=None, composable=True, **kwargs):
+    def animate(self, fig, maps, feature, sampling=None,
+            overlay_locations=False, axes=None, aspect='equal', logscale=None,
+            composable=True, **kwargs):
         """
         Animates the time-segmented inference parameters.
 
         Vector features are represented as amplitude,
         and especially force as log. amplitude.
 
         The `RWAnalyzer.time` attribute is accessed.
```

### Comparing `tramway-0.6b0/tramway/analyzer/mapper/plotly.py` & `tramway-0.6rc1/tramway/analyzer/mapper/plotly.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/mapper/plugin.py` & `tramway-0.6rc1/tramway/analyzer/mapper/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from ..artefact import analysis
 from .. import attribute
 from .abc import *
 from tramway.inference import plugins
 from tramway.helper.inference import Infer
 
 class MapperAttribute(object):
-    """ Mixin class for accessing the `localization_precision` and
-    `localization_error` attributes.
+    """ Mixin class for accessing the `localization_precision`,
+    `localization_error` and `temperature` attributes.
     """
     __slots__ = ()
 
     @property
     def localization_precision(self):
         return self._parent.localization_precision
     @localization_precision.setter
@@ -34,14 +34,21 @@
     @property
     def localization_error(self):
         return self._parent.localization_error
     @localization_error.setter
     def localization_error(self, sigma2):
         self._parent.localization_error = sigma2
 
+    @property
+    def temperature(self):
+        return self._parent.temperature
+    @temperature.setter
+    def temperature(self, T):
+        self._parent.temperature = T
+
 
 class MapperPlugin(AnalyzerNode, MapperAttribute):
     __slots__ = ('_name','_module','_setup','_mapper','_kwargs')
     def __init__(self, plugin, **kwargs):
         init_kwargs = {}
         for k in attribute.__analyzer_node_init_args__:
             try:
```

### Comparing `tramway-0.6b0/tramway/analyzer/mapper/utils.py` & `tramway-0.6rc1/tramway/analyzer/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/pipeline/__init__.py` & `tramway-0.6rc1/tramway/analyzer/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/pipeline/stages.py` & `tramway-0.6rc1/tramway/analyzer/pipeline/stages.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/roi/__init__.py` & `tramway-0.6rc1/tramway/analyzer/roi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,18 +341,24 @@
                 regions are unions of overlapping ROI
 
         See also :class:`BoundingBoxes`.
         """
         self.specialize( BoundingBoxes, bb, label, group_overlapping_roi )
     def from_squares(self, centers, side, label=None, group_overlapping_roi=False):
         """
-        Defines ROI as centers for squares/cubes of uniform size.
+        Defines spatial ROI as centers for squares/cubes of uniform size.
+
+        Centers should be provided as a sequence of :class:`ndarray`
+        or an NxD matrix, with D the number of spatial dimensions.
 
         See also :meth:`from_bounding_boxes`.
         """
+        if isinstance(centers, np.ndarray) and not \
+                (centers.shape[1:] and 1<centers.shape[1]):
+            raise ValueError('ROI centers are not a NxD matrix')
         bb = [ (center-.5*side, center+.5*side) for center in centers ]
         self.from_bounding_boxes(bb, label, group_overlapping_roi)
     def from_ascii_file(self, filepath, size=None,
             label=None, group_overlapping_roi=False):
         """
         Reads the ROI centers or bounds from a text file.
```

### Comparing `tramway-0.6b0/tramway/analyzer/roi/abc.py` & `tramway-0.6rc1/tramway/analyzer/roi/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/roi/allsymbols.py` & `tramway-0.6rc1/tramway/analyzer/roi/allsymbols.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from . import *
 from . import utils
-from ..attribute import InitializerMethod
+from ..attribute import initializer_method
 
-from_bounding_boxes = InitializerMethod( ROIInitializer.from_bounding_boxes )
-from_squares        = InitializerMethod( ROIInitializer.from_squares        )
-from_ascii_file     = InitializerMethod( ROIInitializer.from_ascii_file     )
-from_ascii_files    = InitializerMethod( ROIInitializer.from_ascii_files    )
-from_dedicated_rwa_record  = InitializerMethod( ROIInitializer.from_dedicated_rwa_record  )
-from_dedicated_rwa_records = InitializerMethod( ROIInitializer.from_dedicated_rwa_records )
+from_bounding_boxes = initializer_method( ROIInitializer.from_bounding_boxes )
+from_squares        = initializer_method( ROIInitializer.from_squares        )
+from_ascii_file     = initializer_method( ROIInitializer.from_ascii_file     )
+from_ascii_files    = initializer_method( ROIInitializer.from_ascii_files    )
+from_dedicated_rwa_record  = initializer_method( ROIInitializer.from_dedicated_rwa_record  )
+from_dedicated_rwa_records = initializer_method( ROIInitializer.from_dedicated_rwa_records )
```

### Comparing `tramway-0.6b0/tramway/analyzer/roi/collections.py` & `tramway-0.6rc1/tramway/analyzer/roi/collections.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/roi/mpl.py` & `tramway-0.6rc1/tramway/analyzer/roi/mpl.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/roi/utils.py` & `tramway-0.6rc1/tramway/analyzer/roi/utils.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/sampler/__init__.py` & `tramway-0.6rc1/tramway/analyzer/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/sampler/abc.py` & `tramway-0.6rc1/tramway/analyzer/sampler/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/spt_data/__init__.py` & `tramway-0.6rc1/tramway/analyzer/spt_data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,18 +70,25 @@
             files.append(f)
     else:
         files = _glob.glob(pattern)
     return files
 
 
 class SPTParameters(object):
-    """ Children classes should define the :attr:`_frame_interval` and :attr:`_localization_error`
-        attributes, or implement the :attr:`frame_interval` and :attr:`localization_error` properties.
+    """
+    Mixin class for storing common experimental parameters, including the
+    localization error, time interval and temperature.
+
+    Children classes should define the :attr:`_frame_interval`,
+    :attr:`_localization_error` and :attr:`_temperature` attributes,
+    or overload the :attr:`frame_interval`, :attr:`localization_error`
+    and :attr:`temperature` properties.
 
-        Default values should be :const:`None`."""
+    Default values should be :const:`None`.
+    """
     __slots__ = ()
     def __init__(self, localization_precision=None, localization_error=None):
         if localization_precision is None:
             if localization_error is not None:
                 self.localization_error = localization_error
         elif localization_error is None:
             self.localization_precision = localization_precision
@@ -144,14 +151,32 @@
     @property
     def dt(self):
         return self.frame_interval
     @dt.setter
     def dt(self, dt):
         self.frame_interval = dt
     dt.__doc__ = time_step.__doc__
+    @property
+    def temperature(self):
+        """ *float*: Temperature in *K*; can be set as a *value*-*unit* pair,
+            with *unit* any of :const:`'K'`, :const:`'C'` and :const:`'F'`
+        """
+        return self._temperature
+    @temperature.setter
+    def temperature(self, T):
+        if isinstance(T, (tuple, list)):
+            T, unit = T
+            if T is not None:
+                if unit == 'C':
+                    T = 273 + T
+                elif unit == 'F':
+                    T = 273 + (T - 32) / 1.8
+                elif unit != 'K':
+                    raise ValueError(f"temperature unit not supported: '{unit}'")
+        self._temperature = T
     def set_precision(self, precision):
         """
         Sets the numerical precision of the raw data.
 
         Arguments:
 
             precision (*dict* or *str*): any of :const:`'half'`, :const:`'single'`, :const:`'double'`,
@@ -166,15 +191,16 @@
 def _normalize(p):
     return os.path.expanduser(os.path.normpath(p))
 
 
 class SPTDataIterator(AnalyzerNode, SPTParameters):
     """ Partial implementation for multi-item :class:`SPTData`.
 
-    Children classes must implement the :meth:`__iter__` method. """
+    Children classes must implement the :meth:`__iter__` method.
+    """
     __slots__ = ('_bounds',)
     def __init__(self, **kwargs):
         prms = SPTParameters.__parse__(kwargs)
         AnalyzerNode.__init__(self, **kwargs)
         self._bounds = None
         SPTParameters.__init__(self, *prms)
     @property
@@ -220,19 +246,37 @@
         self.frame_interval = dt
     @property
     def time_step(self):
         return self.frame_interval
     @time_step.setter
     def time_step(self, dt):
         self.frame_interval = dt
+    @property
+    def temperature(self):
+        it = iter(self)
+        T = next(it).temperature
+        while True:
+            try:
+                _T = next(it).temperature
+            except StopIteration:
+                break
+            else:
+                if T != _T:
+                    raise AttributeError('not all the data blocks share the same temperature')
+        return T
+    @temperature.setter
+    def temperature(self, T):
+        for f in self:
+            f.temperature = T
     def as_dataframes(self, source=None, return_index=False):
         """ Generator function; yields :class:`pandas.DataFrame` objects.
         
         `source` can be a source name (filepath) or a boolean function
-        that takes a source string as input argument."""
+        that takes a source string as input argument.
+        """
         for f in self.filter_by_source(source, return_index):
             yield f.dataframe
     def filter_by_source(self, source_filter, return_index=False):
         """ Generator function; similar to :meth:`__iter__`;
         yields :class:`SPTDataItem` objects.
 
         *source* can be a single `str` value, or a set of `str` values,
@@ -488,17 +532,20 @@
         return StandaloneRWAFile.reload_from_rwa_files(self, skip_missing=skip_missing)
 
 
 class HasAnalysisTree(HasROI):
     """
     Partial implementation for :class:`SPTData` that complements :class:`SPTParameters`.
     """
-    __slots__ = ('_analyses','_frame_interval_cache','_localization_error_cache')
+    __slots__ = ('_analyses', '_frame_interval_cache',
+            '_localization_error_cache', '_temperature_cache')
     def __init__(self, df=None, **kwargs):
-        self._frame_interval_cache = self._localization_error_cache = None
+        self._frame_interval_cache = None
+        self._localization_error_cache = None
+        self._temperature_cache = None
         HasROI.__init__(self, **kwargs)
         self._analyses = None
         self.analyses = Analyses(df, standard_metadata(), autosave=True)
         self._analyses.hooks.append(lambda _: self.commit_cache(autoload=True))
     @property
     def _frame_interval(self):
         return self._frame_interval_cache
@@ -511,37 +558,52 @@
     def _localization_error(self):
         return self._localization_error_cache
     @_localization_error.setter
     def _localization_error(self, err):
         self._localization_error_cache = err
         if not islazy(self._dataframe) and self._dataframe is not None:
             self._dataframe.localization_error = err
+    @property
+    def _temperature(self):
+        return self._temperature_cache
+    @_temperature.setter
+    def _temperature(self, T):
+        self._temperature_cache = T
+        if not islazy(self._dataframe) and self._dataframe is not None:
+            self._dataframe.temperature = T
     def commit_cache(self, autoload=False):
         """
         Pushes the cached parameters into the :attr:`dataframe` object.
         """
         if islazy(self._dataframe) or self._dataframe is None:
             if not autoload:
                 raise RuntimeError('the SPT data has not been loaded')
         self.dataframe.frame_interval = self._frame_interval_cache
         self.dataframe.localization_error = self._localization_error_cache
+        self.dataframe.temperature = self._temperature_cache
     def clear_cache(self):
         """
         Clears the cached values and reads from the :attr:`dataframe` object.
         """
-        self._frame_interval_cache = self._localization_error_cache = None
+        self._frame_interval_cache = None
+        self._localization_error_cache = None
+        self._temperature_cache = None
         if not islazy(self._dataframe) and self._dataframe is not None:
             try:
                 self._frame_interval_cache = self._dataframe.frame_interval
             except AttributeError:
                 pass
             try:
                 self._localization_error_cache = self._dataframe.localization_error
             except AttributeError:
                 pass
+            try:
+                self._temperature_cache = self._dataframe.temperature
+            except AttributeError:
+                pass
     def check_cache(self, _raise=AttributeError):
         """
         Checks the parameter cache integrity.
 
         If differences are found with the values in :attr:`dataframe`,
         :meth:`check_cache` raises an exception of type `_raise`.
 
@@ -580,14 +642,24 @@
                 pass
             else:
                 if not ok:
                     if _return is None: # _raise is not None
                         raise _raise from None
                     else:
                         return not _return
+            try:
+                ok = self._temperature_cache == self._dataframe.temperature
+            except AttributeError:
+                pass
+            else:
+                if not ok:
+                    if _return is None: # _raise is not None
+                        raise _raise from None
+                    else:
+                        return not _return
         # the cache is alright
         if _return is not None:
             return _return
     def set_analyses(self, tree):
         if isinstance(tree, AutosaveCapable):
             autosaver = tree
             tree = autosaver.analyses.statefree()
@@ -608,28 +680,37 @@
             if rwa_file is not None:
                 self._analyses.rwa_file = rwa_file
             if autosave is not None:
                 self._analyses.autosave = autosave
         #
         err_cache = self._localization_error_cache
         dt_cache = self._frame_interval_cache
+        T_cache = self._temperature_cache
         if islazy(tree._data):
             store = tree._data.store
             record = store.getRecord(tree._data.locator, store.store)
             try:
                 err = store.peek('localization_error', record)
             except KeyError:
                 err = None
             try:
                 dt = store.peek('frame_interval', record)
             except KeyError:
                 dt = None
+            try:
+                T = store.peek('temperature', record)
+            except KeyError:
+                T = None
         else:
             df = tree.data
             try:
+                T = df.temperature
+            except AttributeError:
+                T = None
+            try:
                 dt = df.frame_interval
             except AttributeError:
                 dt = None
             try:
                 err = df.localization_error
             except AttributeError:
                 err = None
@@ -637,14 +718,18 @@
             if not (err_cache is None or err_cache == err):
                 self.logger.warning("localization error does not match with record: {} != {}".format(err_cache, err))
             self._localization_error_cache = err
         if dt is not None:
             if not (dt_cache is None or dt_cache == dt):
                 self.logger.warning("frame interval does not match with record: {} != {}".format(dt_cache, dt))
             self._frame_interval_cache = dt
+        if T is not None:
+            if not (T_cache is None or T_cache == T):
+                self.logger.warning(f"temperature does not match with record: {T_cache} != {T}")
+            self._temperature_cache = T
     @property
     def analyses(self):
         return self._analyses
     @analyses.setter
     def analyses(self, tree):
         self.set_analyses(tree)
     @property
@@ -1519,14 +1604,15 @@
         if filepath:
             df = self._bear_child( LocalizationFile, filepath, trajectories )
         else:
             df = self._bear_child( SPTDataFrame, trajectories, source )
         siblings = self._dataframes[0]
         df.frame_interval = siblings.frame_interval
         df.localization_error = siblings.localization_error
+        df.temperature = siblings.temperature
         if isinstance(siblings.dataframe, _FakeSPTData):
             assert not self._dataframes[1:]
             self._dataframes = [ df ]
         else:
             if tuple(df.columns) != tuple(siblings.columns):
                 raise ValueError("not all the dataframes feature the same column names")
             self._dataframes.append( df )
```

### Comparing `tramway-0.6b0/tramway/analyzer/spt_data/abc.py` & `tramway-0.6rc1/tramway/analyzer/spt_data/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/spt_data/allsymbols.py` & `tramway-0.6rc1/tramway/analyzer/spt_data/allsymbols.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 from . import *
-from ..attribute import InitializerMethod
+from ..attribute import initializer_method
 
-from_ascii_file    = InitializerMethod( SPTDataInitializer.from_ascii_file    )
-from_ascii_files   = InitializerMethod( SPTDataInitializer.from_ascii_files   )
-from_dataframe     = InitializerMethod( SPTDataInitializer.from_dataframe     )
-from_dataframes    = InitializerMethod( SPTDataInitializer.from_dataframes    )
-from_mat_file      = InitializerMethod( SPTDataInitializer.from_mat_file      )
-from_mat_files     = InitializerMethod( SPTDataInitializer.from_mat_files     )
-from_rwa_file      = InitializerMethod( SPTDataInitializer.from_rwa_file      )
-from_rwa_files     = InitializerMethod( SPTDataInitializer.from_rwa_files     )
-from_rw_generator  = InitializerMethod( SPTDataInitializer.from_rw_generator  )
-from_analysis_tree = InitializerMethod( SPTDataInitializer.from_analysis_tree )
-#from_tracker      = InitializerMethod( SPTDataInitializer.from_tracker       )
+from_ascii_file    = initializer_method( SPTDataInitializer.from_ascii_file    )
+from_ascii_files   = initializer_method( SPTDataInitializer.from_ascii_files   )
+from_dataframe     = initializer_method( SPTDataInitializer.from_dataframe     )
+from_dataframes    = initializer_method( SPTDataInitializer.from_dataframes    )
+from_mat_file      = initializer_method( SPTDataInitializer.from_mat_file      )
+from_mat_files     = initializer_method( SPTDataInitializer.from_mat_files     )
+from_rwa_file      = initializer_method( SPTDataInitializer.from_rwa_file      )
+from_rwa_files     = initializer_method( SPTDataInitializer.from_rwa_files     )
+from_rw_generator  = initializer_method( SPTDataInitializer.from_rw_generator  )
+from_analysis_tree = initializer_method( SPTDataInitializer.from_analysis_tree )
+#from_tracker      = initializer_method( SPTDataInitializer.from_tracker       )
```

### Comparing `tramway-0.6b0/tramway/analyzer/spt_data/mpl.py` & `tramway-0.6rc1/tramway/analyzer/spt_data/mpl.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/__init__.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/abc.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/mpl.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/mpl.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/plugin.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/plugin.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/post/__init__.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/post/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/post/merger.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/post/merger.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/proxied.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/proxied.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tesseller/proxy.py` & `tramway-0.6rc1/tramway/analyzer/tesseller/proxy.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/time/__init__.py` & `tramway-0.6rc1/tramway/analyzer/time/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/time/abc.py` & `tramway-0.6rc1/tramway/analyzer/time/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/analyzer/tracker/__init__.py` & `tramway-0.6rc1/tramway/analyzer/tracker/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,20 @@
         self.spt_data.localization_error = err
     @property
     def localization_precision(self):
         return self.spt_data.localization_precision
     @localization_precision.setter
     def localization_precision(self, sigma):
         self.spt_data.localization_precision = sigma
+    @property
+    def temperature(self):
+        return self.spt_data.temperature
+    @temperature.setter
+    def temperature(self, T):
+        self.spt_data.temperature = T
 
 
 class SingleParticleTracker(BaseTracker):
     __slots__ = ()
     def track(self, locations, register=False, source=None):
         if isinstance(locations, str):
             loc_file = locations
@@ -106,20 +112,23 @@
     @estimated_large_length.setter
     def estimated_large_length(self, length):
         self._large_length = length
     ###
     def track(self, locations, register=False, source=None):
         import tramway.tracking.track_non_track.file_processing_loc as nt
         images = self._eldest_parent.images
+        extra_cols = None
         if isinstance(locations, str):
             loc_file = locations
             locations = load_xyt(loc_file, columns=list('xyt'))
         else:
             loc_file = None
+            loc = locations
             locations = locations[list('xyt')]
+            extra_cols = [ col for col in loc if col not in locations ]
 
         movie_per_frame, n_unique = nt.convert_to_list(locations.values)
         dt_theo = self.dt
         t_init = self.dt * 1
         if images.initialized:
             t_end = self.dt * images.n_frames
         else:
@@ -208,22 +217,32 @@
             trajectory_indices.append(np.full((sum([len(t) for t in traj]),1), n))
             trajectory_coordinates.append(traj)
         trajectory_indices = np.vstack(trajectory_indices)
         trajectory_coordinates = np.vstack(list(itertools.chain(*trajectory_coordinates)))
         trajectories = pd.DataFrame(trajectory_indices, columns=['n']).join(
                 pd.DataFrame(trajectory_coordinates, columns=list('xyt')))
 
+        if extra_cols:
+            trajectories = join_by_values(trajectories, loc, list('xyt'))
+
         if register:
             self.spt_data.add_tracked_data(trajectories, filepath=loc_file if source is None else source)
 
         return trajectories
 
 Tracker.register(NonTrackingTracker)
 
 
+def join_by_values(sample, full, join_cols):
+    assert not any([ col in full for col in sample if col not in join_cols ])
+    ret = sample.merge(full, on=join_cols, how='left', validate='1:1')
+    assert len(ret) == len(sample)
+    return ret
+
+
 class TrackerInitializer(Initializer):
     """ Initializer class for the :class:`~tramway.analyzer.RWAnalyzer`
     :attr:`~tramway.analyzer.RWAnalyzer.tracker` main attribute.
 
     The :attr:`~tramway.analyzer.RWAnalyzer.tracker` attribute self-modifies
     on calling any of the *from_...* methods.
     """
```

### Comparing `tramway-0.6b0/tramway/analyzer/tracker/abc.py` & `tramway-0.6rc1/tramway/analyzer/tracker/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/__init__.py` & `tramway-0.6rc1/tramway/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/analyses/abc.py` & `tramway-0.6rc1/tramway/core/analyses/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/analyses/auto.py` & `tramway-0.6rc1/tramway/core/analyses/auto.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/analyses/base.py` & `tramway-0.6rc1/tramway/core/analyses/base.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/analyses/browser.py` & `tramway-0.6rc1/tramway/core/analyses/browser.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/analyses/lazy.py` & `tramway-0.6rc1/tramway/core/analyses/lazy.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/chain.py` & `tramway-0.6rc1/tramway/core/chain.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/exceptions.py` & `tramway-0.6rc1/tramway/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/hdf5/__init__.py` & `tramway-0.6rc1/tramway/core/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/hdf5/compat.py` & `tramway-0.6rc1/tramway/core/hdf5/compat.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/hdf5/rules.py` & `tramway-0.6rc1/tramway/core/hdf5/rules.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/hdf5/store.py` & `tramway-0.6rc1/tramway/core/hdf5/store.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/lazy.py` & `tramway-0.6rc1/tramway/core/lazy.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/namedcolumns.py` & `tramway-0.6rc1/tramway/core/namedcolumns.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/parallel/__init__.py` & `tramway-0.6rc1/tramway/core/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/parallel/abc.py` & `tramway-0.6rc1/tramway/core/parallel/abc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/parallel/abc_py2.py` & `tramway-0.6rc1/tramway/core/parallel/abc_py2.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/plugin.py` & `tramway-0.6rc1/tramway/core/plugin.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/rc.py` & `tramway-0.6rc1/tramway/core/rc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/scaler.py` & `tramway-0.6rc1/tramway/core/scaler.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/core/xyt.py` & `tramway-0.6rc1/tramway/core/xyt.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             still_active = []
             for traj in active_trajs:
                 traj_ts = ts[traj[0]:traj[1]]
                 row_ix = int(np.round((t-traj_ts[0])/dt))
                 if not np.isclose(traj_ts[row_ix], t):
                     traj_dt = np.diff(traj_ts)
                     ok = np.isclose(traj_dt , dt)
-                    if np.any(ok):
+                    if np.any(ok) or len(traj)==2:
                         raise ValueError('a trajectory is not contiguous in time:\n{}'.format(points[traj[0]:traj[1]]))
                     else:
                         raise ValueError('dt may not be properly set: {}'.format(dt))
                 frame.append(traj[0]+row_ix)
                 trajs.append(traj)
                 if t+dt/2<traj_ts[-1]:
                     still_active.append(traj)
```

### Comparing `tramway-0.6b0/tramway/feature/adjacency.py` & `tramway-0.6rc1/tramway/feature/adjacency.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/curl.py` & `tramway-0.6rc1/tramway/feature/curl.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/batch_extraction.py` & `tramway-0.6rc1/tramway/feature/single_traj/batch_extraction.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/batch_generation.py` & `tramway-0.6rc1/tramway/feature/single_traj/batch_generation.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/distribution.py` & `tramway-0.6rc1/tramway/feature/single_traj/distribution.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/misc.py` & `tramway-0.6rc1/tramway/feature/single_traj/misc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/rw_features.py` & `tramway-0.6rc1/tramway/feature/single_traj/rw_features.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/rw_misc.py` & `tramway-0.6rc1/tramway/feature/single_traj/rw_misc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/rw_simulation.py` & `tramway-0.6rc1/tramway/feature/single_traj/rw_simulation.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/utils_supervised.py` & `tramway-0.6rc1/tramway/feature/single_traj/utils_supervised.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/vae.py` & `tramway-0.6rc1/tramway/feature/single_traj/vae.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/feature/single_traj/visualization.py` & `tramway-0.6rc1/tramway/feature/single_traj/visualization.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/helper/__init__.py` & `tramway-0.6rc1/tramway/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/helper/animation.py` & `tramway-0.6rc1/tramway/helper/animation.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/helper/base.py` & `tramway-0.6rc1/tramway/helper/base.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/helper/inference.py` & `tramway-0.6rc1/tramway/helper/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -777,14 +777,18 @@
     figsize=None, dpi=None, aspect=None, show=None, verbose=False, \
     alpha=None, point_style=None, feature=None, variable=None, segment=None, \
     label=None, input_label=None, mode=None, title=True, inferencemap=False, \
     use_bokeh=None, **kwargs):
     """
     Plot scalar/vector 2D maps.
 
+    For consistency with *InferenceMAP*, the effective potential is showed
+    in :math:`µm^{-1}` while -- using ``unit='std'`` -- the colorbar
+    mentions :math:`k_{B}T`, whereas no conversion factor is applied.
+
     Arguments:
 
         maps (str or tramway.core.analyses.base.Analyses or pandas.DataFrame or Maps):
             maps as a path to a rwa map file,
             an analysis tree, a dataframe or a :class:`Maps`;
             filepaths and analysis trees may require `label` (or equivalently `input_label`)
             to be defined; dataframes and encapsulated maps require `cells` to be defined
@@ -840,14 +844,17 @@
         ylim (array-like): min and max values for the y-axis; this argument is keyworded only
 
         zlim (array-like): min and max values for the z-axis; this argument is keyworded only;
             applies only to scalar maps that are consequently plotted in 3D
 
         clim (array-like): min and max values for the colormap; this argument is keyworded only
 
+        unit (str): colorbar label; can be :const:`'std'` to take usual units,
+            with space coordinates in *µm* and and times in *s*
+
     Extra keyword arguments may be passed to :func:`~tramway.plot.map.scalar_map_2d`,
     :func:`~tramway.plot.map.field_map_2d` and :func:`scalar_map_3d`.
     They can be dictionnaries with feature names as keys and the corresponding values for the
     parameters.
 
     """
     # get cells and maps objects from the first input argument
@@ -924,17 +931,21 @@
             pd.DataFrame(
                 np.array([[xlim[0], ylim[0]], [xlim[1], ylim[1]]]),
                 columns=['x', 'y']),
             cells.tessellation)
 
     unit = kwargs.pop('unit', None)
     if unit == 'std':
+        # standard units are defined at multiple locations:
+        # * tramway.plot.bokeh.analyzer.Controller.draw_map
+        # * tramway.helper.inference.map_plot
+        # * tramway.analyzer.mapper.mpl.Mpl.clabel
         unit = {'diffusivity': r'$\mu\rm{m}^2\rm{s}^{-1}$',
-                'potential': r'$[k_{\rm{B}}T]$',
-                #'force': r'$k_{\rm{B}}T$', # depends on the model
+                'potential': r'$k_{\rm{B}}T$',
+                'force': r'$k_{\rm{B}}T\mu\rm{m}^{-1}$',
                 'drift': r'$\mu\rm{m}\rm{s}^{-1}$',
                }
 
     # identify time segments, if any
     try:
         import tramway.tessellation.time as lattice
         with_segments = isinstance(cells.tessellation, lattice.TimeLattice) \
```

### Comparing `tramway-0.6b0/tramway/helper/roi.py` & `tramway-0.6rc1/tramway/helper/roi.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/helper/simulation/categoricaltrap.py` & `tramway-0.6rc1/tramway/helper/simulation/categoricaltrap.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/helper/simulation/functional.py` & `tramway-0.6rc1/tramway/helper/simulation/functional.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,89 +14,103 @@
 
 import numpy as np
 import pandas as pd
 from tramway.core.xyt import crop
 import warnings
 
 
-def random_walk(diffusivity=None, force=None, viscosity=None, drift=None,
+def random_walk(diffusivity=None, force=None, friction=None, drift=None,
         trajectory_mean_count=100, trajectory_count_sd=0, turnover=None,
         initial_trajectory_count=None, new_trajectory_count=None,
         lifetime_tau=None, lifetime=None, single=False,
         box=(0., 0., 1., 1.), duration=10., time_step=.05, minor_step_count=99,
-        reflect=False, full=False, count_outside_trajectories=None):
+        reflect=False, full=False, count_outside_trajectories=None,
+        viscosity=None):
     r"""
     Generate random walks.
 
     Consider also the alternative generator
     :func:`~tramway.helper.simulation.categoricaltrap.random_walk_2d`.
 
-    The `trajectory_mean_count` and `trajectory_count_sd` arguments are not compatible with
-    the `initial_trajectory_count` and `new_trajectory_count` arguments.
+    The `trajectory_mean_count` and `trajectory_count_sd` arguments are not
+    compatible with the `initial_trajectory_count` and `new_trajectory_count`
+    arguments.
     Use either pair of arguments.
 
+    *new in 0.6*: argument `friction` replaces `viscosity`, and a warning is
+    issued if `viscosity` is used.
+
+    The units for `force` and `friction` can be adapted as long as the ratio
+    of force over friction is expressed as :math:`\mu m s^{-1}` (and drift is
+    not defined).
+
     Arguments:
 
         diffusivity (callable or float): if callable, takes a coordinate vector
-            (:class:`~numpy.ndarray`) and time (float),
-            and returns the local diffusivity (float) in :math:`\mu m^2.s^{-1}`
+            (:class:`~numpy.ndarray`) and time (float), and returns the local
+            diffusivity (float) with :math:`\mu m^2.s^{-1}` as a unit
 
-        force (callable): takes a coordinate vector (:class:`~numpy.ndarray`) and time (float)
-            and returns the local force vector (:class:`~numpy.ndarray`)
+        force (callable): takes a coordinate vector (:class:`~numpy.ndarray`)
+            and time (float) and returns the local force vector
+            (:class:`~numpy.ndarray`) with :math:`k_{\rm{B}}T\mu m^{-1}` as a
+            unit
+
+        friction (callable or float): if callable, takes a coordinate vector
+            (:class:`~numpy.ndarray`) and time (float), and returns the local
+            friction (float) divided by :math:`k_{\rm{B}}T`,
+            equal to the inverse of the diffusivity under equilibrium
 
-        viscosity (callable or float): if callable, takes a coordinate vector
-            (:class:`~numpy.ndarray`) and time (float),
-            and returns the local viscosity (float) that divides the local force;
-            the default viscosity ensures equilibrium conditions
-
-        drift (callable): takes a coordinate vector (:class:`~numpy.ndarray`) and time (float)
-            if `force` is not defined,
+        drift (callable): takes a coordinate vector (:class:`~numpy.ndarray`)
+            and time (float) if `force` is not defined,
             or the same two arguments plus the diffusivity (float) and force
             (:class:`~numpy.ndarray`) otherwise, and returns the local drift;
-            this lets `viscosity` unevaluated
+            this lets `friction` unevaluated
 
-        trajectory_mean_count (int or float): average number of active trajectories at any time
+        trajectory_mean_count (int or float): average number of active
+            trajectories at any time
 
-        trajectory_count_sd (int or float): standard deviation of the number of active
-            trajectories
+        trajectory_count_sd (int or float): standard deviation of the number of
+            active trajectories
 
-        turnover (float): fraction of trajectories that will end at each time step;
-            **deprecated**
+        turnover (float): fraction of trajectories that will end at each time
+            step; **deprecated**
 
         initial_trajectory_count (int): initial number of active trajectories
 
-        new_trajectory_count (int or callable): number of newly generated trajectories;
-            if `new_trajectory_count` is ``callable``, then it takes the time of a step as input
-            and returns the count for this step as an ``int``
+        new_trajectory_count (int or callable): number of newly generated
+            trajectories; if `new_trajectory_count` is ``callable``, then it
+            takes the time of a step as input and returns the count for this
+            step as an ``int``
 
         lifetime_tau (float): trajectory lifetime constant in seconds
 
         lifetime (callable or float): trajectory lifetime in seconds;
             if `lifetime` is a ``float``, then it acts like `lifetime_tau`;
-            if `lifetime` is ``callable``, then it takes as input the initial time of
-            the trajectory
+            if `lifetime` is ``callable``, then it takes as input the initial
+            time of the trajectory
 
         single (bool): allow single-point trajectories
 
         box (array-like): origin and size of the space bounding box
 
         duration (float): duration of the simulation in seconds
 
         time_step (float): duration between two consecutive observations
 
         minor_step_count (int): number of intermediate unobserved steps
 
-        reflect (bool): reflect the minor steps that would otherwise leave the bounding box
+        reflect (bool): reflect the minor steps that would otherwise leave the
+            bounding box
 
-        full (bool): include locations that are outside the bounding box and times that are
-            posterior to `duration`
+        full (bool): include locations that are outside the bounding box and
+            times that are posterior to `duration`
 
-        count_outside_trajectories (bool): include trajectories that have left the bounding box
-            in determining the number of trajectories at each observation step;
-            **deprecated**
+        count_outside_trajectories (bool): include trajectories that have left
+            the bounding box in determining the number of trajectories at each
+            observation step; **deprecated**
 
     Returns:
 
         pandas.DataFrame: simulated trajectories with 'n' the trajectory index,
             't' the time and with other columns for location coordinates
 
     """
@@ -117,31 +131,37 @@
     if callable(diffusivity):
         pass
     elif np.isscalar(diffusivity) and 0 < diffusivity:
         _D = diffusivity
         diffusivity = lambda x, t: _D
     else:
         raise ValueError('`diffusivity` must be callable or a positive float')
+    if viscosity is not None:
+        if friction is None:
+            friction = viscosity
+            warnings.warn(r"argument name 'viscosity' is misleading as it actually represents the friction divided by kT")
+        else:
+            warnings.warn(r"argument 'viscosity' is ignored")
     if force and not callable(force):
         raise TypeError('`force` must be callable')
     if drift:
         _drift = drift
         if force:
             drift = lambda x, t, D: _drift(x, t, D, force(x, t))
         else:
             drift = lambda x, t, D: _drift(x, t)
     elif force:
-        if viscosity is None:
+        if friction is None:
             drift = lambda x, t, D: D * force(x, t)
-        elif callable(viscosity):
-            drift = lambda x, t, D: force(x, t) / viscosity(x, t)
-        elif np.isscalar(viscosity) and 0 < viscosity:
-            drift = lambda x, t, D: force(x, t) / viscosity
+        elif callable(friction):
+            drift = lambda x, t, D: force(x, t) / friction(x, t)
+        elif np.isscalar(friction) and 0 < friction:
+            drift = lambda x, t, D: force(x, t) / friction
         else:
-            raise ValueError('`viscosity` must be callable or a positive float')
+            raise ValueError('`friction` must be callable or a positive float')
     else:
         drift = lambda x, t, D: 0
     #
     N = int(round(float(duration) / time_step)) # number of observed steps
     min_step_count = 1 if single else 2 # minimum number of observed steps per trajectory
     if callable(lifetime):
         lifetime_tau = None
```

### Comparing `tramway-0.6b0/tramway/helper/tessellation.py` & `tramway-0.6rc1/tramway/helper/tessellation.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/__init__.py` & `tramway-0.6rc1/tramway/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/base.py` & `tramway-0.6rc1/tramway/inference/base.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/__init__.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/calculate_bayes_factors.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/calculate_bayes_factors.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/calculate_marginalized_integral.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/calculate_marginalized_integral.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/calculate_posteriors.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/calculate_posteriors.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/find_marginalized_zeta_t_roots.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/find_marginalized_zeta_t_roots.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/get_D_posterior.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/get_D_posterior.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/group_by_sign.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/group_by_sign.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/stopwatch.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/stopwatch.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/bayes_factors/test_calculate_bayes_factor.py` & `tramway-0.6rc1/tramway/inference/bayes_factors/test_calculate_bayes_factor.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/d.py` & `tramway-0.6rc1/tramway/inference/d.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/d_conj_prior.py` & `tramway-0.6rc1/tramway/inference/d_conj_prior.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/ddrift.py` & `tramway-0.6rc1/tramway/inference/ddrift.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/density.py` & `tramway-0.6rc1/tramway/inference/density.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/df.py` & `tramway-0.6rc1/tramway/inference/df.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/dv.py` & `tramway-0.6rc1/tramway/inference/dv.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/fast_grad_dv.py` & `tramway-0.6rc1/tramway/inference/fast_grad_dv.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/gradient.py` & `tramway-0.6rc1/tramway/inference/gradient.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/optimization.py` & `tramway-0.6rc1/tramway/inference/optimization.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/semi_stochastic_dv.py` & `tramway-0.6rc1/tramway/inference/semi_stochastic_dv.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/snr.py` & `tramway-0.6rc1/tramway/inference/snr.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/spherical_volume.py` & `tramway-0.6rc1/tramway/inference/spherical_volume.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/srtesseler_density.py` & `tramway-0.6rc1/tramway/inference/srtesseler_density.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/standard_d.py` & `tramway-0.6rc1/tramway/inference/standard_d.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/standard_ddrift.py` & `tramway-0.6rc1/tramway/inference/standard_ddrift.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/standard_df.py` & `tramway-0.6rc1/tramway/inference/standard_df.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/stochastic_dv.py` & `tramway-0.6rc1/tramway/inference/stochastic_dv.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/time.py` & `tramway-0.6rc1/tramway/inference/time.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/unsmooth_d.py` & `tramway-0.6rc1/tramway/inference/unsmooth_d.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/unsmooth_ddrift.py` & `tramway-0.6rc1/tramway/inference/unsmooth_ddrift.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/inference/unsmooth_df.py` & `tramway-0.6rc1/tramway/inference/unsmooth_df.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/localization/UNet/inference.py` & `tramway-0.6rc1/tramway/localization/UNet/inference.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/localization/UNet/tf.py` & `tramway-0.6rc1/tramway/localization/UNet/tf.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/localization/UNet/utility_function_inference.py` & `tramway-0.6rc1/tramway/localization/UNet/utility_function_inference.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/animation/__init__.py` & `tramway-0.6rc1/tramway/plot/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/animation/map.py` & `tramway-0.6rc1/tramway/plot/animation/map.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/animation/xyt.py` & `tramway-0.6rc1/tramway/plot/animation/xyt.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/bokeh/analyzer.py` & `tramway-0.6rc1/tramway/plot/bokeh/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         
 class Controller(object):
     """
     Makes and manages the browser view.
 
     Note: time browsing is not supported yet.
     """
-    def __init__(self, model, side_panel=None, webdriver=None):
+    def __init__(self, model, side_panel=None, webdriver=None, **map_kwargs):
         """
         Arguments:
 
             model (Model): analyzer browsing state.
 
             side_panel (bool): show the side panel with experimental export features.
 
@@ -153,14 +153,18 @@
         self.sampling_dropdown.on_change('value', lambda attr, old, new: self.load_sampling(new))
         self.mapping_dropdown.on_change('value', lambda attr, old, new: self.load_mapping(new))
         self.feature_dropdown.on_change('value', lambda attr, old, new: self.load_feature(new))
         self.trajectories_kwargs = dict(color='r', line_width=.5, line_alpha=.5, loc_alpha=.1, loc_size=6)
         self.show_side_panel = webdriver is not None if side_panel is None else side_panel
         self.selenium_webdriver = webdriver
         self.figure_export_width = self.figure_export_height = None
+        # units may not be displayed on the colorbar, depending on bokeh
+        # version
+        self.map_kwargs = dict(unit='std')
+        self.map_kwargs.update(map_kwargs)
     def load_source(self, source_name):
         if self.model.current_spt_data is not None:
             self.unload_source()
         if source_name == 'None':
             #self.unload_source()
             return
         try:
@@ -306,15 +310,14 @@
             elif 1 not in old and 1 in new:
                 self.set_trajectory_visibility(True)
             if 2 in old and 2 not in new:
                 self.set_map_visibility(True)
             elif 2 not in old and 2 in new:
                 self.set_map_visibility(False)
         self.visibility_controls.on_change('active', _update)
-        self.map_kwargs = dict(unit='std')
         return row(self.main_figure, self.colorbar_figure, self.visibility_controls)
     def disable_space_view(self):
         self.main_figure.disabled = True
         self.colorbar_figure.disabled = True
         self.visibility_controls.disabled = True
     def enable_space_view(self):
         #self.colorbar_figure.visible = True
@@ -324,29 +327,26 @@
     def disable_time_view(self):
         self.time_slider.disabled = True
     def enable_time_view(self):
         self.time_slider.disabled = False
         assert 0<self.time_slider.start
         self.time_slider.value = 1
     def draw_map(self, feature):
-        kwargs = self.map_kwargs
+        kwargs = dict(self.map_kwargs)
         if kwargs.get('unit', None) == 'std':
-            kwargs = dict(kwargs)
-            unit = dict(
-                    diffusivity=r'$\mu\rm{m}^2\rm{s}^{-1}$',
-                    potential=r'$[k_{\rm{B}}T]$',
-                    force='Log. amplitude',
-                    drift=r'$\mu\rm{m}\rm{s}^{-1}$',
-                    ) # LaTeX not supported yet
+            # standard units are defined at multiple locations:
+            # * tramway.plot.bokeh.analyzer.Controller.draw_map
+            # * tramway.helper.inference.map_plot
+            # * tramway.analyzer.mapper.mpl.Mpl.clabel
             unit = dict(
                     diffusivity='µm²/s',
-                    potential='[kT]',
-                    force='Log. amplitude',
+                    potential='kT',
+                    force='log. kT/µm',
                     drift='µm/s',
-                    )
+                    ) # LaTeX is not supported
             kwargs['unit'] = unit.get(feature, None)
         if self.model.analyzer.browser.colormap is not None:
             kwargs['colormap'] = self.model.analyzer.browser.colormap
         if self.main_figure.renderers:
             self.main_figure.renderers = []
         try:
             self.visibility_controls.active = [ pos for pos in self.visibility_controls.active if pos != 2 ]
@@ -364,14 +364,17 @@
             else:
                 _seg -= 1
             _cells = _cells[_seg]
             _map = _map[_seg]
             kwargs['clim'] = self.model.clim[feature]
         elif self.model.clim is not None:
             kwargs['clim'] = self.model.clim[feature]
+        if temperature:
+            # convert from µm^-1 (inferenceMAP kT) to true kT
+            _map /= 6.950348e-5 * temperature
         if _map.shape[1] == 2:
             _vector_map = _map
             if feature == 'force':
                 _map = _map.pow(2).sum(1).apply(np.log)*.5
             else:
                 _map = _map.pow(2).sum(1).apply(np.sqrt)
         self.map_glyphs = scalar_map_2d(_cells, _map,
```

### Comparing `tramway-0.6b0/tramway/plot/bokeh/map.py` & `tramway-0.6rc1/tramway/plot/bokeh/map.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/bokeh/roi.py` & `tramway-0.6rc1/tramway/plot/bokeh/roi.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/contour.py` & `tramway-0.6rc1/tramway/plot/contour.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/map.py` & `tramway-0.6rc1/tramway/plot/map.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/mesh.py` & `tramway-0.6rc1/tramway/plot/mesh.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/plot/tk/contour.py` & `tramway-0.6rc1/tramway/plot/tk/contour.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/__init__.py` & `tramway-0.6rc1/tramway/tessellation/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/base.py` & `tramway-0.6rc1/tramway/tessellation/base.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/grid/__init__.py` & `tramway-0.6rc1/tramway/tessellation/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/gwr/__init__.py` & `tramway-0.6rc1/tramway/tessellation/gwr/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/gwr/gas.py` & `tramway-0.6rc1/tramway/tessellation/gwr/gas.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/gwr/graph/__init__.py` & `tramway-0.6rc1/tramway/tessellation/gwr/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/gwr/graph/array.py` & `tramway-0.6rc1/tramway/tessellation/gwr/graph/array.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/gwr/graph/base.py` & `tramway-0.6rc1/tramway/tessellation/gwr/graph/base.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/gwr/graph/dict.py` & `tramway-0.6rc1/tramway/tessellation/gwr/graph/dict.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/gwr/graph/exception.py` & `tramway-0.6rc1/tramway/tessellation/gwr/graph/exception.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/hexagon.py` & `tramway-0.6rc1/tramway/tessellation/hexagon.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/kdtree/__init__.py` & `tramway-0.6rc1/tramway/tessellation/kdtree/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/kdtree/dichotomy.py` & `tramway-0.6rc1/tramway/tessellation/kdtree/dichotomy.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/kmeans/__init__.py` & `tramway-0.6rc1/tramway/tessellation/kmeans/__init__.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/kohonen.py` & `tramway-0.6rc1/tramway/tessellation/kohonen.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/nesting.py` & `tramway-0.6rc1/tramway/tessellation/nesting.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/random.py` & `tramway-0.6rc1/tramway/tessellation/random.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/time.py` & `tramway-0.6rc1/tramway/tessellation/time.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/utils2d.py` & `tramway-0.6rc1/tramway/tessellation/utils2d.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tessellation/window.py` & `tramway-0.6rc1/tramway/tessellation/window.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tracking/track_non_track/file_processing_loc.py` & `tramway-0.6rc1/tramway/tracking/track_non_track/file_processing_loc.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/tracking/track_non_track/non_tracking_T_0.py` & `tramway-0.6rc1/tramway/tracking/track_non_track/non_tracking_T_0.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/utils/crop.py` & `tramway-0.6rc1/tramway/utils/crop.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/utils/deconvolve.py` & `tramway-0.6rc1/tramway/utils/deconvolve.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/utils/inferencemap.py` & `tramway-0.6rc1/tramway/utils/inferencemap.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/utils/mapviz.py` & `tramway-0.6rc1/tramway/utils/mapviz.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/utils/mean_std.py` & `tramway-0.6rc1/tramway/utils/mean_std.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway/utils/trajviz.py` & `tramway-0.6rc1/tramway/utils/trajviz.py`

 * *Files identical despite different names*

### Comparing `tramway-0.6b0/tramway.egg-info/PKG-INFO` & `tramway-0.6rc1/tramway.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tramway
-Version: 0.6b0
+Version: 0.6rc1
 Summary: TRamWAy
 Home-page: https://github.com/DecBayComp/TRamWAy
-Author: François Laurent
+Author: Institut Pasteur, François Laurent
 Author-email: francois.laurent@pasteur.fr
 License: CECILL-2.1
 Description: TRamWAy
         =======
         
         *TRamWAy* helps analyzing single molecule dynamics.
         It infers the diffusivity, drift, force and potential energy across space and time.
```

### Comparing `tramway-0.6b0/tramway.egg-info/SOURCES.txt` & `tramway-0.6rc1/tramway.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 tramway/analyzer/env/__init__.py
 tramway/analyzer/env/abc.py
 tramway/analyzer/env/environments.py
 tramway/analyzer/env/ssh.py
 tramway/analyzer/images/__init__.py
 tramway/analyzer/images/abc.py
 tramway/analyzer/images/allsymbols.py
+tramway/analyzer/images/draw.py
 tramway/analyzer/images/mpl.py
 tramway/analyzer/localizer/__init__.py
 tramway/analyzer/localizer/abc.py
 tramway/analyzer/mapper/__init__.py
 tramway/analyzer/mapper/abc.py
 tramway/analyzer/mapper/allsymbols.py
 tramway/analyzer/mapper/models.py
```

