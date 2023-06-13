# Comparing `tmp/pm20_3-1.0.tar.gz` & `tmp/pm20_3-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm20_3-1.0.tar", last modified: Tue Jun 13 09:22:26 2023, max compression
+gzip compressed data, was "pm20_3-1.1.tar", last modified: Tue Jun 13 09:44:22 2023, max compression
```

## Comparing `pm20_3-1.0.tar` & `pm20_3-1.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:22:26.794950 pm20_3-1.0/
--rw-rw-rw-   0        0        0       26 2023-06-12 18:43:23.000000 pm20_3-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      992 2023-06-13 09:22:26.794950 pm20_3-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-12 17:52:57.000000 pm20_3-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 09:22:26.518361 pm20_3-1.0/pm20_3/
--rw-rw-rw-   0        0        0       37 2023-06-13 09:21:29.000000 pm20_3-1.0/pm20_3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:22:26.528334 pm20_3-1.0/pm20_3/__pycache__/
--rw-rw-rw-   0        0        0      192 2023-06-13 08:49:22.000000 pm20_3-1.0/pm20_3/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1416 2023-06-13 08:53:12.000000 pm20_3-1.0/pm20_3/__pycache__/questions.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-06-13 09:22:26.790961 pm20_3-1.0/pm20_3/q/
--rw-rw-rw-   0        0        0    22332 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/1.png
--rw-rw-rw-   0        0        0    13076 2023-06-12 14:12:00.000000 pm20_3-1.0/pm20_3/q/100_1.png
--rw-rw-rw-   0        0        0    19820 2023-06-12 14:12:00.000000 pm20_3-1.0/pm20_3/q/100_2.png
--rw-rw-rw-   0        0        0    35413 2023-06-12 17:24:14.000000 pm20_3-1.0/pm20_3/q/101.png
--rw-rw-rw-   0        0        0    31641 2023-06-12 17:24:14.000000 pm20_3-1.0/pm20_3/q/102_1.png
--rw-rw-rw-   0        0        0    43027 2023-06-12 17:24:14.000000 pm20_3-1.0/pm20_3/q/102_2.png
--rw-rw-rw-   0        0        0    22381 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/103.png
--rw-rw-rw-   0        0        0    18175 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/104.png
--rw-rw-rw-   0        0        0    17204 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/105.png
--rw-rw-rw-   0        0        0    21939 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/106.png
--rw-rw-rw-   0        0        0    22657 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/107.png
--rw-rw-rw-   0        0        0    20422 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/108.png
--rw-rw-rw-   0        0        0    19033 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/109_1.png
--rw-rw-rw-   0        0        0    10710 2023-06-12 17:24:15.000000 pm20_3-1.0/pm20_3/q/109_2.png
--rw-rw-rw-   0        0        0    24896 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/10_1.png
--rw-rw-rw-   0        0        0    11980 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/10_2.png
--rw-rw-rw-   0        0        0    25238 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/11_1.png
--rw-rw-rw-   0        0        0    11242 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/11_2.png
--rw-rw-rw-   0        0        0    25827 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/12_1.png
--rw-rw-rw-   0        0        0    15607 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/12_2.png
--rw-rw-rw-   0        0        0    23559 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/13_1.png
--rw-rw-rw-   0        0        0    12135 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/13_2.png
--rw-rw-rw-   0        0        0    17871 2023-06-12 10:32:37.000000 pm20_3-1.0/pm20_3/q/14.png
--rw-rw-rw-   0        0        0    47983 2023-06-12 10:32:37.000000 pm20_3-1.0/pm20_3/q/15.png
--rw-rw-rw-   0        0        0    14560 2023-06-12 10:32:37.000000 pm20_3-1.0/pm20_3/q/16.png
--rw-rw-rw-   0        0        0    30806 2023-06-12 10:32:37.000000 pm20_3-1.0/pm20_3/q/17.png
--rw-rw-rw-   0        0        0    25570 2023-06-12 10:32:37.000000 pm20_3-1.0/pm20_3/q/18.png
--rw-rw-rw-   0        0        0    18952 2023-06-12 10:32:37.000000 pm20_3-1.0/pm20_3/q/19.png
--rw-rw-rw-   0        0        0    36031 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/2.png
--rw-rw-rw-   0        0        0    18386 2023-06-12 10:32:38.000000 pm20_3-1.0/pm20_3/q/20.png
--rw-rw-rw-   0        0        0    13506 2023-06-12 10:32:38.000000 pm20_3-1.0/pm20_3/q/21.png
--rw-rw-rw-   0        0        0    17480 2023-06-12 10:32:38.000000 pm20_3-1.0/pm20_3/q/22.png
--rw-rw-rw-   0        0        0    20865 2023-06-12 10:32:38.000000 pm20_3-1.0/pm20_3/q/23.png
--rw-rw-rw-   0        0        0    16150 2023-06-12 16:24:49.000000 pm20_3-1.0/pm20_3/q/24.png
--rw-rw-rw-   0        0        0    17873 2023-06-12 16:24:49.000000 pm20_3-1.0/pm20_3/q/25.png
--rw-rw-rw-   0        0        0    17632 2023-06-12 16:24:49.000000 pm20_3-1.0/pm20_3/q/26.png
--rw-rw-rw-   0        0        0    24749 2023-06-12 16:24:49.000000 pm20_3-1.0/pm20_3/q/27.png
--rw-rw-rw-   0        0        0    30463 2023-06-12 16:24:49.000000 pm20_3-1.0/pm20_3/q/28_1.png
--rw-rw-rw-   0        0        0    26196 2023-06-12 16:24:49.000000 pm20_3-1.0/pm20_3/q/28_2.png
--rw-rw-rw-   0        0        0     7463 2023-06-12 16:24:49.000000 pm20_3-1.0/pm20_3/q/28_3.png
--rw-rw-rw-   0        0        0    24175 2023-06-12 16:24:50.000000 pm20_3-1.0/pm20_3/q/29.png
--rw-rw-rw-   0        0        0    14997 2023-06-12 16:24:50.000000 pm20_3-1.0/pm20_3/q/30.png
--rw-rw-rw-   0        0        0    32838 2023-06-12 16:24:50.000000 pm20_3-1.0/pm20_3/q/31.png
--rw-rw-rw-   0        0        0    31497 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/32.png
--rw-rw-rw-   0        0        0    36121 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/33.png
--rw-rw-rw-   0        0        0    24766 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/34.png
--rw-rw-rw-   0        0        0    24693 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/35.png
--rw-rw-rw-   0        0        0    17212 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/36.png
--rw-rw-rw-   0        0        0    14414 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/37.png
--rw-rw-rw-   0        0        0    28049 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/38.png
--rw-rw-rw-   0        0        0    22897 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/39.png
--rw-rw-rw-   0        0        0    22808 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/3_1.png
--rw-rw-rw-   0        0        0    18430 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/3_2.png
--rw-rw-rw-   0        0        0    17794 2023-06-12 17:07:45.000000 pm20_3-1.0/pm20_3/q/40.png
--rw-rw-rw-   0        0        0    22946 2023-06-12 14:09:12.000000 pm20_3-1.0/pm20_3/q/41.png
--rw-rw-rw-   0        0        0     5229 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/42.png
--rw-rw-rw-   0        0        0   142205 2023-06-13 09:20:28.000000 pm20_3-1.0/pm20_3/q/43.png
--rw-rw-rw-   0        0        0    14311 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/44.png
--rw-rw-rw-   0        0        0    17569 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/45_1.png
--rw-rw-rw-   0        0        0    11219 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/45_2.png
--rw-rw-rw-   0        0        0   190511 2023-06-13 09:20:49.000000 pm20_3-1.0/pm20_3/q/46_1.png
--rw-rw-rw-   0        0        0   112240 2023-06-13 09:21:06.000000 pm20_3-1.0/pm20_3/q/46_2.png
--rw-rw-rw-   0        0        0    13042 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/47.png
--rw-rw-rw-   0        0        0    23492 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/48.png
--rw-rw-rw-   0        0        0    14396 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/49.png
--rw-rw-rw-   0        0        0    22250 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/4_1.png
--rw-rw-rw-   0        0        0     9394 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/4_2.png
--rw-rw-rw-   0        0        0     9631 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/50.png
--rw-rw-rw-   0        0        0    21267 2023-06-12 14:09:13.000000 pm20_3-1.0/pm20_3/q/51.png
--rw-rw-rw-   0        0        0    24781 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/52.png
--rw-rw-rw-   0        0        0    15292 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/53.png
--rw-rw-rw-   0        0        0    15971 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/54.png
--rw-rw-rw-   0        0        0    12039 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/55.png
--rw-rw-rw-   0        0        0     6877 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/56.png
--rw-rw-rw-   0        0        0     8127 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/57.png
--rw-rw-rw-   0        0        0    16492 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/58.png
--rw-rw-rw-   0        0        0    15539 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/59.png
--rw-rw-rw-   0        0        0    39623 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/5_1.png
--rw-rw-rw-   0        0        0    21741 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/5_2.png
--rw-rw-rw-   0        0        0    35512 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/6.png
--rw-rw-rw-   0        0        0    16512 2023-06-12 14:10:27.000000 pm20_3-1.0/pm20_3/q/60.png
--rw-rw-rw-   0        0        0    24946 2023-06-12 09:47:25.000000 pm20_3-1.0/pm20_3/q/61.png
--rw-rw-rw-   0        0        0    12308 2023-06-12 09:47:25.000000 pm20_3-1.0/pm20_3/q/62.png
--rw-rw-rw-   0        0        0    14477 2023-06-12 09:47:25.000000 pm20_3-1.0/pm20_3/q/63.png
--rw-rw-rw-   0        0        0    29479 2023-06-12 09:47:25.000000 pm20_3-1.0/pm20_3/q/64_1.png
--rw-rw-rw-   0        0        0     7143 2023-06-12 09:47:25.000000 pm20_3-1.0/pm20_3/q/64_2.png
--rw-rw-rw-   0        0        0    20260 2023-06-12 09:47:26.000000 pm20_3-1.0/pm20_3/q/65.png
--rw-rw-rw-   0        0        0    24172 2023-06-12 09:47:26.000000 pm20_3-1.0/pm20_3/q/66.png
--rw-rw-rw-   0        0        0    25316 2023-06-12 09:47:26.000000 pm20_3-1.0/pm20_3/q/67.png
--rw-rw-rw-   0        0        0    24259 2023-06-12 09:47:26.000000 pm20_3-1.0/pm20_3/q/68.png
--rw-rw-rw-   0        0        0    24844 2023-06-12 09:47:26.000000 pm20_3-1.0/pm20_3/q/69.png
--rw-rw-rw-   0        0        0    29634 2023-06-11 23:36:53.000000 pm20_3-1.0/pm20_3/q/7.png
--rw-rw-rw-   0        0        0    22730 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/70.png
--rw-rw-rw-   0        0        0    20214 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/71.png
--rw-rw-rw-   0        0        0    20354 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/72.png
--rw-rw-rw-   0        0        0    20613 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/73.png
--rw-rw-rw-   0        0        0    19630 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/74.png
--rw-rw-rw-   0        0        0    19406 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/75.png
--rw-rw-rw-   0        0        0    19924 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/76.png
--rw-rw-rw-   0        0        0    22668 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/77.png
--rw-rw-rw-   0        0        0    27086 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/78_1.png
--rw-rw-rw-   0        0        0    20610 2023-06-12 09:58:57.000000 pm20_3-1.0/pm20_3/q/78_2.png
--rw-rw-rw-   0        0        0    17744 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/79.png
--rw-rw-rw-   0        0        0    41510 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/8.png
--rw-rw-rw-   0        0        0    27180 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/80.png
--rw-rw-rw-   0        0        0    22585 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/81.png
--rw-rw-rw-   0        0        0    26583 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/82.png
--rw-rw-rw-   0        0        0    18612 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/83.png
--rw-rw-rw-   0        0        0    20070 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/84.png
--rw-rw-rw-   0        0        0    10496 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/85.png
--rw-rw-rw-   0        0        0    15364 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/86.png
--rw-rw-rw-   0        0        0    17654 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/87.png
--rw-rw-rw-   0        0        0    21594 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/88_1.png
--rw-rw-rw-   0        0        0     8979 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/88_2.png
--rw-rw-rw-   0        0        0    15442 2023-06-12 22:14:29.000000 pm20_3-1.0/pm20_3/q/89_1.png
--rw-rw-rw-   0        0        0    13482 2023-06-12 22:14:30.000000 pm20_3-1.0/pm20_3/q/89_2.png
--rw-rw-rw-   0        0        0    24624 2023-06-12 10:14:10.000000 pm20_3-1.0/pm20_3/q/9.png
--rw-rw-rw-   0        0        0    19880 2023-06-12 22:14:29.000000 pm20_3-1.0/pm20_3/q/90.png
--rw-rw-rw-   0        0        0    22857 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/91_1.png
--rw-rw-rw-   0        0        0    14390 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/91_2.png
--rw-rw-rw-   0        0        0    39595 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/92.png
--rw-rw-rw-   0        0        0    12829 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/93.png
--rw-rw-rw-   0        0        0    17694 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/94.png
--rw-rw-rw-   0        0        0    25458 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/95.png
--rw-rw-rw-   0        0        0    19844 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/96_1.png
--rw-rw-rw-   0        0        0    11215 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/96_2.png
--rw-rw-rw-   0        0        0    15567 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/97.png
--rw-rw-rw-   0        0        0    16770 2023-06-12 14:11:23.000000 pm20_3-1.0/pm20_3/q/98.png
--rw-rw-rw-   0        0        0    15343 2023-06-12 14:12:00.000000 pm20_3-1.0/pm20_3/q/99.png
--rw-rw-rw-   0        0        0        0 2023-06-12 21:04:56.000000 pm20_3-1.0/pm20_3/q/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:22:26.792956 pm20_3-1.0/pm20_3/q/__pycache__/
--rw-rw-rw-   0        0        0      129 2023-06-13 08:54:40.000000 pm20_3-1.0/pm20_3/q/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    24796 2023-06-11 23:13:18.000000 pm20_3-1.0/pm20_3/q/task_1.png
--rw-rw-rw-   0        0        0    26421 2023-06-11 23:13:18.000000 pm20_3-1.0/pm20_3/q/task_2.png
--rw-rw-rw-   0        0        0    25932 2023-06-11 23:13:18.000000 pm20_3-1.0/pm20_3/q/task_3.png
--rw-rw-rw-   0        0        0    25398 2023-06-11 23:13:18.000000 pm20_3-1.0/pm20_3/q/task_4.png
--rw-rw-rw-   0        0        0    26943 2023-06-11 23:13:18.000000 pm20_3-1.0/pm20_3/q/task_5.png
--rw-rw-rw-   0        0        0    10322 2023-06-11 23:13:18.000000 pm20_3-1.0/pm20_3/q/task_6.png
--rw-rw-rw-   0        0        0     1622 2023-06-13 09:22:25.000000 pm20_3-1.0/pm20_3/questions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:22:26.525343 pm20_3-1.0/pm20_3.egg-info/
--rw-rw-rw-   0        0        0      992 2023-06-13 09:22:26.000000 pm20_3-1.0/pm20_3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2644 2023-06-13 09:22:26.000000 pm20_3-1.0/pm20_3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:22:26.000000 pm20_3-1.0/pm20_3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-13 09:22:26.000000 pm20_3-1.0/pm20_3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 09:22:26.000000 pm20_3-1.0/pm20_3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 09:22:26.795948 pm20_3-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1909 2023-06-13 09:22:25.000000 pm20_3-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:44:22.879742 pm20_3-1.1/
+-rw-rw-rw-   0        0        0       26 2023-06-12 18:43:23.000000 pm20_3-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      992 2023-06-13 09:44:22.879742 pm20_3-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-12 17:52:57.000000 pm20_3-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 09:44:22.605752 pm20_3-1.1/pm20_3/
+-rw-rw-rw-   0        0        0       37 2023-06-13 09:21:29.000000 pm20_3-1.1/pm20_3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:44:22.615725 pm20_3-1.1/pm20_3/__pycache__/
+-rw-rw-rw-   0        0        0      192 2023-06-13 08:49:22.000000 pm20_3-1.1/pm20_3/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1416 2023-06-13 08:53:12.000000 pm20_3-1.1/pm20_3/__pycache__/questions.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-13 09:44:22.876750 pm20_3-1.1/pm20_3/q/
+-rw-rw-rw-   0        0        0        0 2023-06-12 21:04:56.000000 pm20_3-1.1/pm20_3/q/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:44:22.877747 pm20_3-1.1/pm20_3/q/__pycache__/
+-rw-rw-rw-   0        0        0      129 2023-06-13 08:54:40.000000 pm20_3-1.1/pm20_3/q/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    22332 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_1.png
+-rw-rw-rw-   0        0        0    13076 2023-06-12 14:12:00.000000 pm20_3-1.1/pm20_3/q/q_100_1.png
+-rw-rw-rw-   0        0        0    19820 2023-06-12 14:12:00.000000 pm20_3-1.1/pm20_3/q/q_100_2.png
+-rw-rw-rw-   0        0        0    35413 2023-06-12 17:24:14.000000 pm20_3-1.1/pm20_3/q/q_101.png
+-rw-rw-rw-   0        0        0    31641 2023-06-12 17:24:14.000000 pm20_3-1.1/pm20_3/q/q_102_1.png
+-rw-rw-rw-   0        0        0    43027 2023-06-12 17:24:14.000000 pm20_3-1.1/pm20_3/q/q_102_2.png
+-rw-rw-rw-   0        0        0    22381 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_103.png
+-rw-rw-rw-   0        0        0    18175 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_104.png
+-rw-rw-rw-   0        0        0    17204 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_105.png
+-rw-rw-rw-   0        0        0    21939 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_106.png
+-rw-rw-rw-   0        0        0    22657 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_107.png
+-rw-rw-rw-   0        0        0    20422 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_108.png
+-rw-rw-rw-   0        0        0    19033 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_109_1.png
+-rw-rw-rw-   0        0        0    10710 2023-06-12 17:24:15.000000 pm20_3-1.1/pm20_3/q/q_109_2.png
+-rw-rw-rw-   0        0        0    24896 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_10_1.png
+-rw-rw-rw-   0        0        0    11980 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_10_2.png
+-rw-rw-rw-   0        0        0    25238 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_11_1.png
+-rw-rw-rw-   0        0        0    11242 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_11_2.png
+-rw-rw-rw-   0        0        0    25827 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_12_1.png
+-rw-rw-rw-   0        0        0    15607 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_12_2.png
+-rw-rw-rw-   0        0        0    23559 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_13_1.png
+-rw-rw-rw-   0        0        0    12135 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_13_2.png
+-rw-rw-rw-   0        0        0    17871 2023-06-12 10:32:37.000000 pm20_3-1.1/pm20_3/q/q_14.png
+-rw-rw-rw-   0        0        0    47983 2023-06-12 10:32:37.000000 pm20_3-1.1/pm20_3/q/q_15.png
+-rw-rw-rw-   0        0        0    14560 2023-06-12 10:32:37.000000 pm20_3-1.1/pm20_3/q/q_16.png
+-rw-rw-rw-   0        0        0    30806 2023-06-12 10:32:37.000000 pm20_3-1.1/pm20_3/q/q_17.png
+-rw-rw-rw-   0        0        0    25570 2023-06-12 10:32:37.000000 pm20_3-1.1/pm20_3/q/q_18.png
+-rw-rw-rw-   0        0        0    18952 2023-06-12 10:32:37.000000 pm20_3-1.1/pm20_3/q/q_19.png
+-rw-rw-rw-   0        0        0    36031 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_2.png
+-rw-rw-rw-   0        0        0    18386 2023-06-12 10:32:38.000000 pm20_3-1.1/pm20_3/q/q_20.png
+-rw-rw-rw-   0        0        0    13506 2023-06-12 10:32:38.000000 pm20_3-1.1/pm20_3/q/q_21.png
+-rw-rw-rw-   0        0        0    17480 2023-06-12 10:32:38.000000 pm20_3-1.1/pm20_3/q/q_22.png
+-rw-rw-rw-   0        0        0    20865 2023-06-12 10:32:38.000000 pm20_3-1.1/pm20_3/q/q_23.png
+-rw-rw-rw-   0        0        0    16150 2023-06-12 16:24:49.000000 pm20_3-1.1/pm20_3/q/q_24.png
+-rw-rw-rw-   0        0        0    17873 2023-06-12 16:24:49.000000 pm20_3-1.1/pm20_3/q/q_25.png
+-rw-rw-rw-   0        0        0    17632 2023-06-12 16:24:49.000000 pm20_3-1.1/pm20_3/q/q_26.png
+-rw-rw-rw-   0        0        0    24749 2023-06-12 16:24:49.000000 pm20_3-1.1/pm20_3/q/q_27.png
+-rw-rw-rw-   0        0        0    30463 2023-06-12 16:24:49.000000 pm20_3-1.1/pm20_3/q/q_28_1.png
+-rw-rw-rw-   0        0        0    26196 2023-06-12 16:24:49.000000 pm20_3-1.1/pm20_3/q/q_28_2.png
+-rw-rw-rw-   0        0        0     7463 2023-06-12 16:24:49.000000 pm20_3-1.1/pm20_3/q/q_28_3.png
+-rw-rw-rw-   0        0        0    24175 2023-06-12 16:24:50.000000 pm20_3-1.1/pm20_3/q/q_29.png
+-rw-rw-rw-   0        0        0    14997 2023-06-12 16:24:50.000000 pm20_3-1.1/pm20_3/q/q_30.png
+-rw-rw-rw-   0        0        0    32838 2023-06-12 16:24:50.000000 pm20_3-1.1/pm20_3/q/q_31.png
+-rw-rw-rw-   0        0        0    31497 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_32.png
+-rw-rw-rw-   0        0        0    36121 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_33.png
+-rw-rw-rw-   0        0        0    24766 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_34.png
+-rw-rw-rw-   0        0        0    24693 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_35.png
+-rw-rw-rw-   0        0        0    17212 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_36.png
+-rw-rw-rw-   0        0        0    14414 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_37.png
+-rw-rw-rw-   0        0        0    28049 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_38.png
+-rw-rw-rw-   0        0        0    22897 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_39.png
+-rw-rw-rw-   0        0        0    22808 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_3_1.png
+-rw-rw-rw-   0        0        0    18430 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_3_2.png
+-rw-rw-rw-   0        0        0    17794 2023-06-12 17:07:45.000000 pm20_3-1.1/pm20_3/q/q_40.png
+-rw-rw-rw-   0        0        0    22946 2023-06-12 14:09:12.000000 pm20_3-1.1/pm20_3/q/q_41.png
+-rw-rw-rw-   0        0        0     5229 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_42.png
+-rw-rw-rw-   0        0        0   142205 2023-06-13 09:20:28.000000 pm20_3-1.1/pm20_3/q/q_43.png
+-rw-rw-rw-   0        0        0    14311 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_44.png
+-rw-rw-rw-   0        0        0    17569 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_45_1.png
+-rw-rw-rw-   0        0        0    11219 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_45_2.png
+-rw-rw-rw-   0        0        0   190511 2023-06-13 09:20:49.000000 pm20_3-1.1/pm20_3/q/q_46_1.png
+-rw-rw-rw-   0        0        0   112240 2023-06-13 09:21:06.000000 pm20_3-1.1/pm20_3/q/q_46_2.png
+-rw-rw-rw-   0        0        0    13042 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_47.png
+-rw-rw-rw-   0        0        0    23492 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_48.png
+-rw-rw-rw-   0        0        0    14396 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_49.png
+-rw-rw-rw-   0        0        0    22250 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_4_1.png
+-rw-rw-rw-   0        0        0     9394 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_4_2.png
+-rw-rw-rw-   0        0        0     9631 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_50.png
+-rw-rw-rw-   0        0        0    21267 2023-06-12 14:09:13.000000 pm20_3-1.1/pm20_3/q/q_51.png
+-rw-rw-rw-   0        0        0    24781 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_52.png
+-rw-rw-rw-   0        0        0    15292 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_53.png
+-rw-rw-rw-   0        0        0    15971 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_54.png
+-rw-rw-rw-   0        0        0    12039 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_55.png
+-rw-rw-rw-   0        0        0     6877 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_56.png
+-rw-rw-rw-   0        0        0     8127 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_57.png
+-rw-rw-rw-   0        0        0    16492 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_58.png
+-rw-rw-rw-   0        0        0    15539 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_59.png
+-rw-rw-rw-   0        0        0    39623 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_5_1.png
+-rw-rw-rw-   0        0        0    21741 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_5_2.png
+-rw-rw-rw-   0        0        0    35512 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_6.png
+-rw-rw-rw-   0        0        0    16512 2023-06-12 14:10:27.000000 pm20_3-1.1/pm20_3/q/q_60.png
+-rw-rw-rw-   0        0        0    24946 2023-06-12 09:47:25.000000 pm20_3-1.1/pm20_3/q/q_61.png
+-rw-rw-rw-   0        0        0    12308 2023-06-12 09:47:25.000000 pm20_3-1.1/pm20_3/q/q_62.png
+-rw-rw-rw-   0        0        0    14477 2023-06-12 09:47:25.000000 pm20_3-1.1/pm20_3/q/q_63.png
+-rw-rw-rw-   0        0        0    29479 2023-06-12 09:47:25.000000 pm20_3-1.1/pm20_3/q/q_64_1.png
+-rw-rw-rw-   0        0        0     7143 2023-06-12 09:47:25.000000 pm20_3-1.1/pm20_3/q/q_64_2.png
+-rw-rw-rw-   0        0        0    20260 2023-06-12 09:47:26.000000 pm20_3-1.1/pm20_3/q/q_65.png
+-rw-rw-rw-   0        0        0    24172 2023-06-12 09:47:26.000000 pm20_3-1.1/pm20_3/q/q_66.png
+-rw-rw-rw-   0        0        0    25316 2023-06-12 09:47:26.000000 pm20_3-1.1/pm20_3/q/q_67.png
+-rw-rw-rw-   0        0        0    24259 2023-06-12 09:47:26.000000 pm20_3-1.1/pm20_3/q/q_68.png
+-rw-rw-rw-   0        0        0    24844 2023-06-12 09:47:26.000000 pm20_3-1.1/pm20_3/q/q_69.png
+-rw-rw-rw-   0        0        0    29634 2023-06-11 23:36:53.000000 pm20_3-1.1/pm20_3/q/q_7.png
+-rw-rw-rw-   0        0        0    22730 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_70.png
+-rw-rw-rw-   0        0        0    20214 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_71.png
+-rw-rw-rw-   0        0        0    20354 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_72.png
+-rw-rw-rw-   0        0        0    20613 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_73.png
+-rw-rw-rw-   0        0        0    19630 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_74.png
+-rw-rw-rw-   0        0        0    19406 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_75.png
+-rw-rw-rw-   0        0        0    19924 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_76.png
+-rw-rw-rw-   0        0        0    22668 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_77.png
+-rw-rw-rw-   0        0        0    27086 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_78_1.png
+-rw-rw-rw-   0        0        0    20610 2023-06-12 09:58:57.000000 pm20_3-1.1/pm20_3/q/q_78_2.png
+-rw-rw-rw-   0        0        0    17744 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_79.png
+-rw-rw-rw-   0        0        0    41510 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_8.png
+-rw-rw-rw-   0        0        0    27180 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_80.png
+-rw-rw-rw-   0        0        0    22585 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_81.png
+-rw-rw-rw-   0        0        0    26583 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_82.png
+-rw-rw-rw-   0        0        0    18612 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_83.png
+-rw-rw-rw-   0        0        0    20070 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_84.png
+-rw-rw-rw-   0        0        0    10496 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_85.png
+-rw-rw-rw-   0        0        0    15364 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_86.png
+-rw-rw-rw-   0        0        0    17654 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_87.png
+-rw-rw-rw-   0        0        0    21594 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_88_1.png
+-rw-rw-rw-   0        0        0     8979 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_88_2.png
+-rw-rw-rw-   0        0        0    15442 2023-06-12 22:14:29.000000 pm20_3-1.1/pm20_3/q/q_89_1.png
+-rw-rw-rw-   0        0        0    13482 2023-06-12 22:14:30.000000 pm20_3-1.1/pm20_3/q/q_89_2.png
+-rw-rw-rw-   0        0        0    24624 2023-06-12 10:14:10.000000 pm20_3-1.1/pm20_3/q/q_9.png
+-rw-rw-rw-   0        0        0    19880 2023-06-12 22:14:29.000000 pm20_3-1.1/pm20_3/q/q_90.png
+-rw-rw-rw-   0        0        0    22857 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_91_1.png
+-rw-rw-rw-   0        0        0    14390 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_91_2.png
+-rw-rw-rw-   0        0        0    39595 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_92.png
+-rw-rw-rw-   0        0        0    12829 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_93.png
+-rw-rw-rw-   0        0        0    17694 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_94.png
+-rw-rw-rw-   0        0        0    25458 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_95.png
+-rw-rw-rw-   0        0        0    19844 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_96_1.png
+-rw-rw-rw-   0        0        0    11215 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_96_2.png
+-rw-rw-rw-   0        0        0    15567 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_97.png
+-rw-rw-rw-   0        0        0    16770 2023-06-12 14:11:23.000000 pm20_3-1.1/pm20_3/q/q_98.png
+-rw-rw-rw-   0        0        0    15343 2023-06-12 14:12:00.000000 pm20_3-1.1/pm20_3/q/q_99.png
+-rw-rw-rw-   0        0        0    24796 2023-06-11 23:13:18.000000 pm20_3-1.1/pm20_3/q/task_1.png
+-rw-rw-rw-   0        0        0    26421 2023-06-11 23:13:18.000000 pm20_3-1.1/pm20_3/q/task_2.png
+-rw-rw-rw-   0        0        0    25932 2023-06-11 23:13:18.000000 pm20_3-1.1/pm20_3/q/task_3.png
+-rw-rw-rw-   0        0        0    25398 2023-06-11 23:13:18.000000 pm20_3-1.1/pm20_3/q/task_4.png
+-rw-rw-rw-   0        0        0    26943 2023-06-11 23:13:18.000000 pm20_3-1.1/pm20_3/q/task_5.png
+-rw-rw-rw-   0        0        0    10322 2023-06-11 23:13:18.000000 pm20_3-1.1/pm20_3/q/task_6.png
+-rw-rw-rw-   0        0        0     1638 2023-06-13 09:44:21.000000 pm20_3-1.1/pm20_3/questions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:44:22.612733 pm20_3-1.1/pm20_3.egg-info/
+-rw-rw-rw-   0        0        0      992 2023-06-13 09:44:22.000000 pm20_3-1.1/pm20_3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-06-13 09:44:22.000000 pm20_3-1.1/pm20_3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:44:22.000000 pm20_3-1.1/pm20_3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-13 09:44:22.000000 pm20_3-1.1/pm20_3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 09:44:22.000000 pm20_3-1.1/pm20_3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 09:44:22.880739 pm20_3-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1910 2023-06-13 09:44:21.000000 pm20_3-1.1/setup.py
```

### Comparing `pm20_3-1.0/PKG-INFO` & `pm20_3-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pm20_3
-Version: 1.0
+Version: 1.1
 Summary: For cheating again..
 Home-page: http://www.fa.ru/Pages/Home.aspx
 Author: Anatoliy Nesterov
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `pm20_3-1.0/pm20_3/__pycache__/questions.cpython-39.pyc` & `pm20_3-1.1/pm20_3/__pycache__/questions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/1.png` & `pm20_3-1.1/pm20_3/q/q_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/100_1.png` & `pm20_3-1.1/pm20_3/q/q_100_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/100_2.png` & `pm20_3-1.1/pm20_3/q/q_100_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/101.png` & `pm20_3-1.1/pm20_3/q/q_101.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/102_1.png` & `pm20_3-1.1/pm20_3/q/q_102_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/102_2.png` & `pm20_3-1.1/pm20_3/q/q_102_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/103.png` & `pm20_3-1.1/pm20_3/q/q_103.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/104.png` & `pm20_3-1.1/pm20_3/q/q_104.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/105.png` & `pm20_3-1.1/pm20_3/q/q_105.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/106.png` & `pm20_3-1.1/pm20_3/q/q_106.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/107.png` & `pm20_3-1.1/pm20_3/q/q_107.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/108.png` & `pm20_3-1.1/pm20_3/q/q_108.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/109_1.png` & `pm20_3-1.1/pm20_3/q/q_109_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/109_2.png` & `pm20_3-1.1/pm20_3/q/q_109_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/10_1.png` & `pm20_3-1.1/pm20_3/q/q_10_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/10_2.png` & `pm20_3-1.1/pm20_3/q/q_10_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/11_1.png` & `pm20_3-1.1/pm20_3/q/q_11_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/11_2.png` & `pm20_3-1.1/pm20_3/q/q_11_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/12_1.png` & `pm20_3-1.1/pm20_3/q/q_12_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/12_2.png` & `pm20_3-1.1/pm20_3/q/q_12_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/13_1.png` & `pm20_3-1.1/pm20_3/q/q_13_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/13_2.png` & `pm20_3-1.1/pm20_3/q/q_13_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/14.png` & `pm20_3-1.1/pm20_3/q/q_14.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/15.png` & `pm20_3-1.1/pm20_3/q/q_15.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/16.png` & `pm20_3-1.1/pm20_3/q/q_16.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/17.png` & `pm20_3-1.1/pm20_3/q/q_17.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/18.png` & `pm20_3-1.1/pm20_3/q/q_18.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/19.png` & `pm20_3-1.1/pm20_3/q/q_19.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/2.png` & `pm20_3-1.1/pm20_3/q/q_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/20.png` & `pm20_3-1.1/pm20_3/q/q_20.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/21.png` & `pm20_3-1.1/pm20_3/q/q_21.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/22.png` & `pm20_3-1.1/pm20_3/q/q_22.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/23.png` & `pm20_3-1.1/pm20_3/q/q_23.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/24.png` & `pm20_3-1.1/pm20_3/q/q_24.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/25.png` & `pm20_3-1.1/pm20_3/q/q_25.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/26.png` & `pm20_3-1.1/pm20_3/q/q_26.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/27.png` & `pm20_3-1.1/pm20_3/q/q_27.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/28_1.png` & `pm20_3-1.1/pm20_3/q/q_28_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/28_2.png` & `pm20_3-1.1/pm20_3/q/q_28_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/28_3.png` & `pm20_3-1.1/pm20_3/q/q_28_3.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/29.png` & `pm20_3-1.1/pm20_3/q/q_29.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/30.png` & `pm20_3-1.1/pm20_3/q/q_30.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/31.png` & `pm20_3-1.1/pm20_3/q/q_31.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/32.png` & `pm20_3-1.1/pm20_3/q/q_32.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/33.png` & `pm20_3-1.1/pm20_3/q/q_33.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/34.png` & `pm20_3-1.1/pm20_3/q/q_34.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/35.png` & `pm20_3-1.1/pm20_3/q/q_35.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/36.png` & `pm20_3-1.1/pm20_3/q/q_36.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/37.png` & `pm20_3-1.1/pm20_3/q/q_37.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/38.png` & `pm20_3-1.1/pm20_3/q/q_38.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/39.png` & `pm20_3-1.1/pm20_3/q/q_39.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/3_1.png` & `pm20_3-1.1/pm20_3/q/q_3_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/3_2.png` & `pm20_3-1.1/pm20_3/q/q_3_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/40.png` & `pm20_3-1.1/pm20_3/q/q_40.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/41.png` & `pm20_3-1.1/pm20_3/q/q_41.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/42.png` & `pm20_3-1.1/pm20_3/q/q_42.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/43.png` & `pm20_3-1.1/pm20_3/q/q_43.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/44.png` & `pm20_3-1.1/pm20_3/q/q_44.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/45_1.png` & `pm20_3-1.1/pm20_3/q/q_45_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/45_2.png` & `pm20_3-1.1/pm20_3/q/q_45_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/46_1.png` & `pm20_3-1.1/pm20_3/q/q_46_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/46_2.png` & `pm20_3-1.1/pm20_3/q/q_46_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/47.png` & `pm20_3-1.1/pm20_3/q/q_47.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/48.png` & `pm20_3-1.1/pm20_3/q/q_48.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/49.png` & `pm20_3-1.1/pm20_3/q/q_49.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/4_1.png` & `pm20_3-1.1/pm20_3/q/q_4_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/4_2.png` & `pm20_3-1.1/pm20_3/q/q_4_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/50.png` & `pm20_3-1.1/pm20_3/q/q_50.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/51.png` & `pm20_3-1.1/pm20_3/q/q_51.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/52.png` & `pm20_3-1.1/pm20_3/q/q_52.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/53.png` & `pm20_3-1.1/pm20_3/q/q_53.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/54.png` & `pm20_3-1.1/pm20_3/q/q_54.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/55.png` & `pm20_3-1.1/pm20_3/q/q_55.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/56.png` & `pm20_3-1.1/pm20_3/q/q_56.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/57.png` & `pm20_3-1.1/pm20_3/q/q_57.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/58.png` & `pm20_3-1.1/pm20_3/q/q_58.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/59.png` & `pm20_3-1.1/pm20_3/q/q_59.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/5_1.png` & `pm20_3-1.1/pm20_3/q/q_5_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/5_2.png` & `pm20_3-1.1/pm20_3/q/q_5_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/6.png` & `pm20_3-1.1/pm20_3/q/q_6.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/60.png` & `pm20_3-1.1/pm20_3/q/q_60.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/61.png` & `pm20_3-1.1/pm20_3/q/q_61.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/62.png` & `pm20_3-1.1/pm20_3/q/q_62.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/63.png` & `pm20_3-1.1/pm20_3/q/q_63.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/64_1.png` & `pm20_3-1.1/pm20_3/q/q_64_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/64_2.png` & `pm20_3-1.1/pm20_3/q/q_64_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/65.png` & `pm20_3-1.1/pm20_3/q/q_65.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/66.png` & `pm20_3-1.1/pm20_3/q/q_66.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/67.png` & `pm20_3-1.1/pm20_3/q/q_67.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/68.png` & `pm20_3-1.1/pm20_3/q/q_68.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/69.png` & `pm20_3-1.1/pm20_3/q/q_69.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/7.png` & `pm20_3-1.1/pm20_3/q/q_7.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/70.png` & `pm20_3-1.1/pm20_3/q/q_70.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/71.png` & `pm20_3-1.1/pm20_3/q/q_71.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/72.png` & `pm20_3-1.1/pm20_3/q/q_72.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/73.png` & `pm20_3-1.1/pm20_3/q/q_73.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/74.png` & `pm20_3-1.1/pm20_3/q/q_74.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/75.png` & `pm20_3-1.1/pm20_3/q/q_75.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/76.png` & `pm20_3-1.1/pm20_3/q/q_76.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/77.png` & `pm20_3-1.1/pm20_3/q/q_77.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/78_1.png` & `pm20_3-1.1/pm20_3/q/q_78_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/78_2.png` & `pm20_3-1.1/pm20_3/q/q_78_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/79.png` & `pm20_3-1.1/pm20_3/q/q_79.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/8.png` & `pm20_3-1.1/pm20_3/q/q_8.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/80.png` & `pm20_3-1.1/pm20_3/q/q_80.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/81.png` & `pm20_3-1.1/pm20_3/q/q_81.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/82.png` & `pm20_3-1.1/pm20_3/q/q_82.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/83.png` & `pm20_3-1.1/pm20_3/q/q_83.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/84.png` & `pm20_3-1.1/pm20_3/q/q_84.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/85.png` & `pm20_3-1.1/pm20_3/q/q_85.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/86.png` & `pm20_3-1.1/pm20_3/q/q_86.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/87.png` & `pm20_3-1.1/pm20_3/q/q_87.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/88_1.png` & `pm20_3-1.1/pm20_3/q/q_88_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/88_2.png` & `pm20_3-1.1/pm20_3/q/q_88_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/89_1.png` & `pm20_3-1.1/pm20_3/q/q_89_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/89_2.png` & `pm20_3-1.1/pm20_3/q/q_89_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/9.png` & `pm20_3-1.1/pm20_3/q/q_9.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/90.png` & `pm20_3-1.1/pm20_3/q/q_90.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/91_1.png` & `pm20_3-1.1/pm20_3/q/q_91_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/91_2.png` & `pm20_3-1.1/pm20_3/q/q_91_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/92.png` & `pm20_3-1.1/pm20_3/q/q_92.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/93.png` & `pm20_3-1.1/pm20_3/q/q_93.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/94.png` & `pm20_3-1.1/pm20_3/q/q_94.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/95.png` & `pm20_3-1.1/pm20_3/q/q_95.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/96_1.png` & `pm20_3-1.1/pm20_3/q/q_96_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/96_2.png` & `pm20_3-1.1/pm20_3/q/q_96_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/97.png` & `pm20_3-1.1/pm20_3/q/q_97.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/98.png` & `pm20_3-1.1/pm20_3/q/q_98.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/99.png` & `pm20_3-1.1/pm20_3/q/q_99.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/task_1.png` & `pm20_3-1.1/pm20_3/q/task_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/task_2.png` & `pm20_3-1.1/pm20_3/q/task_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/task_3.png` & `pm20_3-1.1/pm20_3/q/task_3.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/task_4.png` & `pm20_3-1.1/pm20_3/q/task_4.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/task_5.png` & `pm20_3-1.1/pm20_3/q/task_5.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/q/task_6.png` & `pm20_3-1.1/pm20_3/q/task_6.png`

 * *Files identical despite different names*

### Comparing `pm20_3-1.0/pm20_3/questions.py` & `pm20_3-1.1/pm20_3/questions.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,19 +47,20 @@
             img = Image(filename=pt)
             display(img)
 
     else:
         qn = str(qn)
         files = sorted(contents('pm20_3.q'))
         to_disp = []
+
         for elem in files:
-            if qn + '_' in elem:
+            if 'q_' + qn + '_' in elem:
                 to_disp.append(elem)
         if not to_disp:
-            to_disp.append(qn + '.png')
+            to_disp.append('q_' + qn + '.png')
         to_disp.sort()
         for elem in to_disp:
             with path(
                     'pm20_3.q',
                     elem
             ) as pt:
                 img = Image(filename=pt)
```

### Comparing `pm20_3-1.0/pm20_3.egg-info/PKG-INFO` & `pm20_3-1.1/pm20_3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pm20-3
-Version: 1.0
+Version: 1.1
 Summary: For cheating again..
 Home-page: http://www.fa.ru/Pages/Home.aspx
 Author: Anatoliy Nesterov
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `pm20_3-1.0/pm20_3.egg-info/SOURCES.txt` & `pm20_3-1.1/pm20_3.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,144 +7,144 @@
 pm20_3.egg-info/PKG-INFO
 pm20_3.egg-info/SOURCES.txt
 pm20_3.egg-info/dependency_links.txt
 pm20_3.egg-info/requires.txt
 pm20_3.egg-info/top_level.txt
 pm20_3/__pycache__/__init__.cpython-39.pyc
 pm20_3/__pycache__/questions.cpython-39.pyc
-pm20_3/q/1.png
-pm20_3/q/100_1.png
-pm20_3/q/100_2.png
-pm20_3/q/101.png
-pm20_3/q/102_1.png
-pm20_3/q/102_2.png
-pm20_3/q/103.png
-pm20_3/q/104.png
-pm20_3/q/105.png
-pm20_3/q/106.png
-pm20_3/q/107.png
-pm20_3/q/108.png
-pm20_3/q/109_1.png
-pm20_3/q/109_2.png
-pm20_3/q/10_1.png
-pm20_3/q/10_2.png
-pm20_3/q/11_1.png
-pm20_3/q/11_2.png
-pm20_3/q/12_1.png
-pm20_3/q/12_2.png
-pm20_3/q/13_1.png
-pm20_3/q/13_2.png
-pm20_3/q/14.png
-pm20_3/q/15.png
-pm20_3/q/16.png
-pm20_3/q/17.png
-pm20_3/q/18.png
-pm20_3/q/19.png
-pm20_3/q/2.png
-pm20_3/q/20.png
-pm20_3/q/21.png
-pm20_3/q/22.png
-pm20_3/q/23.png
-pm20_3/q/24.png
-pm20_3/q/25.png
-pm20_3/q/26.png
-pm20_3/q/27.png
-pm20_3/q/28_1.png
-pm20_3/q/28_2.png
-pm20_3/q/28_3.png
-pm20_3/q/29.png
-pm20_3/q/30.png
-pm20_3/q/31.png
-pm20_3/q/32.png
-pm20_3/q/33.png
-pm20_3/q/34.png
-pm20_3/q/35.png
-pm20_3/q/36.png
-pm20_3/q/37.png
-pm20_3/q/38.png
-pm20_3/q/39.png
-pm20_3/q/3_1.png
-pm20_3/q/3_2.png
-pm20_3/q/40.png
-pm20_3/q/41.png
-pm20_3/q/42.png
-pm20_3/q/43.png
-pm20_3/q/44.png
-pm20_3/q/45_1.png
-pm20_3/q/45_2.png
-pm20_3/q/46_1.png
-pm20_3/q/46_2.png
-pm20_3/q/47.png
-pm20_3/q/48.png
-pm20_3/q/49.png
-pm20_3/q/4_1.png
-pm20_3/q/4_2.png
-pm20_3/q/50.png
-pm20_3/q/51.png
-pm20_3/q/52.png
-pm20_3/q/53.png
-pm20_3/q/54.png
-pm20_3/q/55.png
-pm20_3/q/56.png
-pm20_3/q/57.png
-pm20_3/q/58.png
-pm20_3/q/59.png
-pm20_3/q/5_1.png
-pm20_3/q/5_2.png
-pm20_3/q/6.png
-pm20_3/q/60.png
-pm20_3/q/61.png
-pm20_3/q/62.png
-pm20_3/q/63.png
-pm20_3/q/64_1.png
-pm20_3/q/64_2.png
-pm20_3/q/65.png
-pm20_3/q/66.png
-pm20_3/q/67.png
-pm20_3/q/68.png
-pm20_3/q/69.png
-pm20_3/q/7.png
-pm20_3/q/70.png
-pm20_3/q/71.png
-pm20_3/q/72.png
-pm20_3/q/73.png
-pm20_3/q/74.png
-pm20_3/q/75.png
-pm20_3/q/76.png
-pm20_3/q/77.png
-pm20_3/q/78_1.png
-pm20_3/q/78_2.png
-pm20_3/q/79.png
-pm20_3/q/8.png
-pm20_3/q/80.png
-pm20_3/q/81.png
-pm20_3/q/82.png
-pm20_3/q/83.png
-pm20_3/q/84.png
-pm20_3/q/85.png
-pm20_3/q/86.png
-pm20_3/q/87.png
-pm20_3/q/88_1.png
-pm20_3/q/88_2.png
-pm20_3/q/89_1.png
-pm20_3/q/89_2.png
-pm20_3/q/9.png
-pm20_3/q/90.png
-pm20_3/q/91_1.png
-pm20_3/q/91_2.png
-pm20_3/q/92.png
-pm20_3/q/93.png
-pm20_3/q/94.png
-pm20_3/q/95.png
-pm20_3/q/96_1.png
-pm20_3/q/96_2.png
-pm20_3/q/97.png
-pm20_3/q/98.png
-pm20_3/q/99.png
 pm20_3/q/__init__.py
+pm20_3/q/q_1.png
+pm20_3/q/q_100_1.png
+pm20_3/q/q_100_2.png
+pm20_3/q/q_101.png
+pm20_3/q/q_102_1.png
+pm20_3/q/q_102_2.png
+pm20_3/q/q_103.png
+pm20_3/q/q_104.png
+pm20_3/q/q_105.png
+pm20_3/q/q_106.png
+pm20_3/q/q_107.png
+pm20_3/q/q_108.png
+pm20_3/q/q_109_1.png
+pm20_3/q/q_109_2.png
+pm20_3/q/q_10_1.png
+pm20_3/q/q_10_2.png
+pm20_3/q/q_11_1.png
+pm20_3/q/q_11_2.png
+pm20_3/q/q_12_1.png
+pm20_3/q/q_12_2.png
+pm20_3/q/q_13_1.png
+pm20_3/q/q_13_2.png
+pm20_3/q/q_14.png
+pm20_3/q/q_15.png
+pm20_3/q/q_16.png
+pm20_3/q/q_17.png
+pm20_3/q/q_18.png
+pm20_3/q/q_19.png
+pm20_3/q/q_2.png
+pm20_3/q/q_20.png
+pm20_3/q/q_21.png
+pm20_3/q/q_22.png
+pm20_3/q/q_23.png
+pm20_3/q/q_24.png
+pm20_3/q/q_25.png
+pm20_3/q/q_26.png
+pm20_3/q/q_27.png
+pm20_3/q/q_28_1.png
+pm20_3/q/q_28_2.png
+pm20_3/q/q_28_3.png
+pm20_3/q/q_29.png
+pm20_3/q/q_30.png
+pm20_3/q/q_31.png
+pm20_3/q/q_32.png
+pm20_3/q/q_33.png
+pm20_3/q/q_34.png
+pm20_3/q/q_35.png
+pm20_3/q/q_36.png
+pm20_3/q/q_37.png
+pm20_3/q/q_38.png
+pm20_3/q/q_39.png
+pm20_3/q/q_3_1.png
+pm20_3/q/q_3_2.png
+pm20_3/q/q_40.png
+pm20_3/q/q_41.png
+pm20_3/q/q_42.png
+pm20_3/q/q_43.png
+pm20_3/q/q_44.png
+pm20_3/q/q_45_1.png
+pm20_3/q/q_45_2.png
+pm20_3/q/q_46_1.png
+pm20_3/q/q_46_2.png
+pm20_3/q/q_47.png
+pm20_3/q/q_48.png
+pm20_3/q/q_49.png
+pm20_3/q/q_4_1.png
+pm20_3/q/q_4_2.png
+pm20_3/q/q_50.png
+pm20_3/q/q_51.png
+pm20_3/q/q_52.png
+pm20_3/q/q_53.png
+pm20_3/q/q_54.png
+pm20_3/q/q_55.png
+pm20_3/q/q_56.png
+pm20_3/q/q_57.png
+pm20_3/q/q_58.png
+pm20_3/q/q_59.png
+pm20_3/q/q_5_1.png
+pm20_3/q/q_5_2.png
+pm20_3/q/q_6.png
+pm20_3/q/q_60.png
+pm20_3/q/q_61.png
+pm20_3/q/q_62.png
+pm20_3/q/q_63.png
+pm20_3/q/q_64_1.png
+pm20_3/q/q_64_2.png
+pm20_3/q/q_65.png
+pm20_3/q/q_66.png
+pm20_3/q/q_67.png
+pm20_3/q/q_68.png
+pm20_3/q/q_69.png
+pm20_3/q/q_7.png
+pm20_3/q/q_70.png
+pm20_3/q/q_71.png
+pm20_3/q/q_72.png
+pm20_3/q/q_73.png
+pm20_3/q/q_74.png
+pm20_3/q/q_75.png
+pm20_3/q/q_76.png
+pm20_3/q/q_77.png
+pm20_3/q/q_78_1.png
+pm20_3/q/q_78_2.png
+pm20_3/q/q_79.png
+pm20_3/q/q_8.png
+pm20_3/q/q_80.png
+pm20_3/q/q_81.png
+pm20_3/q/q_82.png
+pm20_3/q/q_83.png
+pm20_3/q/q_84.png
+pm20_3/q/q_85.png
+pm20_3/q/q_86.png
+pm20_3/q/q_87.png
+pm20_3/q/q_88_1.png
+pm20_3/q/q_88_2.png
+pm20_3/q/q_89_1.png
+pm20_3/q/q_89_2.png
+pm20_3/q/q_9.png
+pm20_3/q/q_90.png
+pm20_3/q/q_91_1.png
+pm20_3/q/q_91_2.png
+pm20_3/q/q_92.png
+pm20_3/q/q_93.png
+pm20_3/q/q_94.png
+pm20_3/q/q_95.png
+pm20_3/q/q_96_1.png
+pm20_3/q/q_96_2.png
+pm20_3/q/q_97.png
+pm20_3/q/q_98.png
+pm20_3/q/q_99.png
 pm20_3/q/task_1.png
 pm20_3/q/task_2.png
 pm20_3/q/task_3.png
 pm20_3/q/task_4.png
 pm20_3/q/task_5.png
 pm20_3/q/task_6.png
 pm20_3/q/__pycache__/__init__.cpython-39.pyc
```

### Comparing `pm20_3-1.0/setup.py` & `pm20_3-1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='pm20_3',  # How you named your package folder (MyLib)
     packages=['pm20_3'],  # Chose the same as "name"
-    version='1.0',  # Start with a small number and increase it with every change you make
+    version='1.01',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='For cheating again..',  # Give a short description about your library
     author='Anatoliy Nesterov',  # Type in your name
     author_email='your.email@domain.com',  # Type in your E-Mail
     url='http://www.fa.ru/Pages/Home.aspx',  # Provide either the link to your github or to your website
     download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     keywords=['CHEATING'],  # Keywords that define your package best
```

