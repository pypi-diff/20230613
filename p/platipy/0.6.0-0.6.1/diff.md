# Comparing `tmp/platipy-0.6.0.tar.gz` & `tmp/platipy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platipy-0.6.0.tar", max compression
+gzip compressed data, was "platipy-0.6.1.tar", max compression
```

## Comparing `platipy-0.6.0.tar` & `platipy-0.6.1.tar`

### file list

```diff
@@ -1,404 +1,401 @@
--rw-r--r--   0        0        0     4474 2023-01-15 05:01:36.327022 platipy-0.6.0/README.md
--rw-r--r--   0        0        0      334 2023-02-28 20:20:56.079706 platipy-0.6.0/platipy/__init__.py
--rw-r--r--   0        0        0     6762 2023-01-10 23:30:32.208231 platipy-0.6.0/platipy/backend/README.md
--rw-r--r--   0        0        0     3025 2023-01-10 23:30:32.213712 platipy-0.6.0/platipy/backend/__init__.py
--rw-r--r--   0        0        0    18860 2023-01-10 23:30:32.219629 platipy-0.6.0/platipy/backend/api.py
--rw-r--r--   0        0        0     4341 2023-01-10 23:30:32.225181 platipy-0.6.0/platipy/backend/application.py
--rw-r--r--   0        0        0     4153 2022-04-03 01:48:02.277585 platipy-0.6.0/platipy/backend/manage.py
--rw-r--r--   0        0        0     6095 2023-01-10 23:30:32.231269 platipy-0.6.0/platipy/backend/models.py
--rw-r--r--   0        0        0    13946 2022-10-20 03:23:41.822311 platipy-0.6.0/platipy/backend/sample/SampleClient.ipynb
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.214839 platipy-0.6.0/platipy/backend/sample/__init__.py
--rw-r--r--   0        0        0     3838 2023-01-10 23:30:32.236380 platipy-0.6.0/platipy/backend/sample/sample.py
--rw-r--r--   0        0        0     3837 2022-09-30 08:24:03.899506 platipy-0.6.0/platipy/backend/sample/service.py
--rw-r--r--   0        0        0    37644 2020-09-24 01:07:55.221591 platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.css
--rw-r--r--   0        0        0    98559 2020-09-24 01:07:55.222728 platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    28977 2020-09-24 01:07:55.223189 platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0    68241 2020-09-24 01:07:55.223852 platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0     4896 2020-09-24 01:07:55.223995 platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.css
--rw-r--r--   0        0        0    60752 2020-09-24 01:07:55.224294 platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0     4019 2020-09-24 01:07:55.224435 platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    26084 2020-09-24 01:07:55.224733 platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0   173597 2020-09-24 01:07:55.225066 platipy-0.6.0/platipy/backend/static/css/bootstrap.css
--rw-r--r--   0        0        0   430003 2020-09-24 01:07:55.225772 platipy-0.6.0/platipy/backend/static/css/bootstrap.css.map
--rw-r--r--   0        0        0   140936 2020-09-24 01:07:55.226047 platipy-0.6.0/platipy/backend/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   562427 2020-09-24 01:07:55.226886 platipy-0.6.0/platipy/backend/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0     1822 2020-09-24 01:07:55.227009 platipy-0.6.0/platipy/backend/static/css/dashboard.css
--rw-r--r--   0        0        0     1081 2020-09-24 01:07:55.227178 platipy-0.6.0/platipy/backend/static/feather/LICENSE
--rw-r--r--   0        0        0    65962 2020-09-24 01:07:55.227723 platipy-0.6.0/platipy/backend/static/feather/feather.min.js
--rw-r--r--   0        0        0      282 2020-09-24 01:07:55.242734 platipy-0.6.0/platipy/backend/static/feather/icons/activity.svg
--rw-r--r--   0        0        0      362 2020-09-24 01:07:55.242862 platipy-0.6.0/platipy/backend/static/feather/icons/airplay.svg
--rw-r--r--   0        0        0      353 2020-09-24 01:07:55.242977 platipy-0.6.0/platipy/backend/static/feather/icons/alert-circle.svg
--rw-r--r--   0        0        0      413 2020-09-24 01:07:55.243082 platipy-0.6.0/platipy/backend/static/feather/icons/alert-octagon.svg
--rw-r--r--   0        0        0      421 2020-09-24 01:07:55.243188 platipy-0.6.0/platipy/backend/static/feather/icons/alert-triangle.svg
--rw-r--r--   0        0        0      398 2020-09-24 01:07:55.243284 platipy-0.6.0/platipy/backend/static/feather/icons/align-center.svg
--rw-r--r--   0        0        0      399 2020-09-24 01:07:55.243392 platipy-0.6.0/platipy/backend/static/feather/icons/align-justify.svg
--rw-r--r--   0        0        0      396 2020-09-24 01:07:55.243491 platipy-0.6.0/platipy/backend/static/feather/icons/align-left.svg
--rw-r--r--   0        0        0      397 2020-09-24 01:07:55.243641 platipy-0.6.0/platipy/backend/static/feather/icons/align-right.svg
--rw-r--r--   0        0        0      345 2020-09-24 01:07:55.243728 platipy-0.6.0/platipy/backend/static/feather/icons/anchor.svg
--rw-r--r--   0        0        0      568 2020-09-24 01:07:55.243835 platipy-0.6.0/platipy/backend/static/feather/icons/aperture.svg
--rw-r--r--   0        0        0      361 2020-09-24 01:07:55.243932 platipy-0.6.0/platipy/backend/static/feather/icons/archive.svg
--rw-r--r--   0        0        0      360 2020-09-24 01:07:55.244032 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-down-circle.svg
--rw-r--r--   0        0        0      315 2020-09-24 01:07:55.244139 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-down-left.svg
--rw-r--r--   0        0        0      317 2020-09-24 01:07:55.244221 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-down-right.svg
--rw-r--r--   0        0        0      313 2020-09-24 01:07:55.244305 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-down.svg
--rw-r--r--   0        0        0      359 2020-09-24 01:07:55.244421 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-left-circle.svg
--rw-r--r--   0        0        0      312 2020-09-24 01:07:55.244517 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-left.svg
--rw-r--r--   0        0        0      361 2020-09-24 01:07:55.244608 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-right-circle.svg
--rw-r--r--   0        0        0      314 2020-09-24 01:07:55.244694 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-right.svg
--rw-r--r--   0        0        0      357 2020-09-24 01:07:55.244785 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-up-circle.svg
--rw-r--r--   0        0        0      312 2020-09-24 01:07:55.244881 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-up-left.svg
--rw-r--r--   0        0        0      314 2020-09-24 01:07:55.244965 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-up-right.svg
--rw-r--r--   0        0        0      310 2020-09-24 01:07:55.245050 platipy-0.6.0/platipy/backend/static/feather/icons/arrow-up.svg
--rw-r--r--   0        0        0      322 2020-09-24 01:07:55.245400 platipy-0.6.0/platipy/backend/static/feather/icons/at-sign.svg
--rw-r--r--   0        0        0      325 2020-09-24 01:07:55.245500 platipy-0.6.0/platipy/backend/static/feather/icons/award.svg
--rw-r--r--   0        0        0      355 2020-09-24 01:07:55.245595 platipy-0.6.0/platipy/backend/static/feather/icons/bar-chart-2.svg
--rw-r--r--   0        0        0      353 2020-09-24 01:07:55.245682 platipy-0.6.0/platipy/backend/static/feather/icons/bar-chart.svg
--rw-r--r--   0        0        0      427 2020-09-24 01:07:55.245770 platipy-0.6.0/platipy/backend/static/feather/icons/battery-charging.svg
--rw-r--r--   0        0        0      326 2020-09-24 01:07:55.245867 platipy-0.6.0/platipy/backend/static/feather/icons/battery.svg
--rw-r--r--   0        0        0      375 2020-09-24 01:07:55.245967 platipy-0.6.0/platipy/backend/static/feather/icons/bell-off.svg
--rw-r--r--   0        0        0      315 2020-09-24 01:07:55.246096 platipy-0.6.0/platipy/backend/static/feather/icons/bell.svg
--rw-r--r--   0        0        0      298 2020-09-24 01:07:55.246179 platipy-0.6.0/platipy/backend/static/feather/icons/bluetooth.svg
--rw-r--r--   0        0        0      327 2020-09-24 01:07:55.246263 platipy-0.6.0/platipy/backend/static/feather/icons/bold.svg
--rw-r--r--   0        0        0      339 2020-09-24 01:07:55.246347 platipy-0.6.0/platipy/backend/static/feather/icons/book-open.svg
--rw-r--r--   0        0        0      345 2020-09-24 01:07:55.246442 platipy-0.6.0/platipy/backend/static/feather/icons/book.svg
--rw-r--r--   0        0        0      287 2020-09-24 01:07:55.246531 platipy-0.6.0/platipy/backend/static/feather/icons/bookmark.svg
--rw-r--r--   0        0        0      488 2020-09-24 01:07:55.246611 platipy-0.6.0/platipy/backend/static/feather/icons/box.svg
--rw-r--r--   0        0        0      343 2020-09-24 01:07:55.246696 platipy-0.6.0/platipy/backend/static/feather/icons/briefcase.svg
--rw-r--r--   0        0        0      410 2020-09-24 01:07:55.246827 platipy-0.6.0/platipy/backend/static/feather/icons/calendar.svg
--rw-r--r--   0        0        0      385 2020-09-24 01:07:55.246919 platipy-0.6.0/platipy/backend/static/feather/icons/camera-off.svg
--rw-r--r--   0        0        0      356 2020-09-24 01:07:55.247072 platipy-0.6.0/platipy/backend/static/feather/icons/camera.svg
--rw-r--r--   0        0        0      384 2020-09-24 01:07:55.247190 platipy-0.6.0/platipy/backend/static/feather/icons/cast.svg
--rw-r--r--   0        0        0      328 2020-09-24 01:07:55.247296 platipy-0.6.0/platipy/backend/static/feather/icons/check-circle.svg
--rw-r--r--   0        0        0      345 2020-09-24 01:07:55.247441 platipy-0.6.0/platipy/backend/static/feather/icons/check-square.svg
--rw-r--r--   0        0        0      262 2020-09-24 01:07:55.247557 platipy-0.6.0/platipy/backend/static/feather/icons/check.svg
--rw-r--r--   0        0        0      269 2020-09-24 01:07:55.247657 platipy-0.6.0/platipy/backend/static/feather/icons/chevron-down.svg
--rw-r--r--   0        0        0      270 2020-09-24 01:07:55.247761 platipy-0.6.0/platipy/backend/static/feather/icons/chevron-left.svg
--rw-r--r--   0        0        0      270 2020-09-24 01:07:55.247858 platipy-0.6.0/platipy/backend/static/feather/icons/chevron-right.svg
--rw-r--r--   0        0        0      268 2020-09-24 01:07:55.247955 platipy-0.6.0/platipy/backend/static/feather/icons/chevron-up.svg
--rw-r--r--   0        0        0      317 2020-09-24 01:07:55.248077 platipy-0.6.0/platipy/backend/static/feather/icons/chevrons-down.svg
--rw-r--r--   0        0        0      318 2020-09-24 01:07:55.248188 platipy-0.6.0/platipy/backend/static/feather/icons/chevrons-left.svg
--rw-r--r--   0        0        0      318 2020-09-24 01:07:55.248286 platipy-0.6.0/platipy/backend/static/feather/icons/chevrons-right.svg
--rw-r--r--   0        0        0      316 2020-09-24 01:07:55.248385 platipy-0.6.0/platipy/backend/static/feather/icons/chevrons-up.svg
--rw-r--r--   0        0        0      448 2020-09-24 01:07:55.248473 platipy-0.6.0/platipy/backend/static/feather/icons/chrome.svg
--rw-r--r--   0        0        0      258 2020-09-24 01:07:55.248604 platipy-0.6.0/platipy/backend/static/feather/icons/circle.svg
--rw-r--r--   0        0        0      371 2020-09-24 01:07:55.248690 platipy-0.6.0/platipy/backend/static/feather/icons/clipboard.svg
--rw-r--r--   0        0        0      304 2020-09-24 01:07:55.249168 platipy-0.6.0/platipy/backend/static/feather/icons/clock.svg
--rw-r--r--   0        0        0      557 2020-09-24 01:07:55.249306 platipy-0.6.0/platipy/backend/static/feather/icons/cloud-drizzle.svg
--rw-r--r--   0        0        0      345 2020-09-24 01:07:55.249433 platipy-0.6.0/platipy/backend/static/feather/icons/cloud-lightning.svg
--rw-r--r--   0        0        0      371 2020-09-24 01:07:55.249536 platipy-0.6.0/platipy/backend/static/feather/icons/cloud-off.svg
--rw-r--r--   0        0        0      421 2020-09-24 01:07:55.249630 platipy-0.6.0/platipy/backend/static/feather/icons/cloud-rain.svg
--rw-r--r--   0        0        0      554 2020-09-24 01:07:55.249729 platipy-0.6.0/platipy/backend/static/feather/icons/cloud-snow.svg
--rw-r--r--   0        0        0      280 2020-09-24 01:07:55.249878 platipy-0.6.0/platipy/backend/static/feather/icons/cloud.svg
--rw-r--r--   0        0        0      307 2020-09-24 01:07:55.250000 platipy-0.6.0/platipy/backend/static/feather/icons/code.svg
--rw-r--r--   0        0        0      486 2020-09-24 01:07:55.250093 platipy-0.6.0/platipy/backend/static/feather/icons/codepen.svg
--rw-r--r--   0        0        0      447 2020-09-24 01:07:55.250191 platipy-0.6.0/platipy/backend/static/feather/icons/coffee.svg
--rw-r--r--   0        0        0      421 2020-09-24 01:07:55.250335 platipy-0.6.0/platipy/backend/static/feather/icons/command.svg
--rw-r--r--   0        0        0      342 2020-09-24 01:07:55.250454 platipy-0.6.0/platipy/backend/static/feather/icons/compass.svg
--rw-r--r--   0        0        0      351 2020-09-24 01:07:55.250590 platipy-0.6.0/platipy/backend/static/feather/icons/copy.svg
--rw-r--r--   0        0        0      314 2020-09-24 01:07:55.250692 platipy-0.6.0/platipy/backend/static/feather/icons/corner-down-left.svg
--rw-r--r--   0        0        0      318 2020-09-24 01:07:55.250884 platipy-0.6.0/platipy/backend/static/feather/icons/corner-down-right.svg
--rw-r--r--   0        0        0      317 2020-09-24 01:07:55.251014 platipy-0.6.0/platipy/backend/static/feather/icons/corner-left-down.svg
--rw-r--r--   0        0        0      312 2020-09-24 01:07:55.251141 platipy-0.6.0/platipy/backend/static/feather/icons/corner-left-up.svg
--rw-r--r--   0        0        0      318 2020-09-24 01:07:55.251398 platipy-0.6.0/platipy/backend/static/feather/icons/corner-right-down.svg
--rw-r--r--   0        0        0      313 2020-09-24 01:07:55.251628 platipy-0.6.0/platipy/backend/static/feather/icons/corner-right-up.svg
--rw-r--r--   0        0        0      312 2020-09-24 01:07:55.251845 platipy-0.6.0/platipy/backend/static/feather/icons/corner-up-left.svg
--rw-r--r--   0        0        0      316 2020-09-24 01:07:55.252028 platipy-0.6.0/platipy/backend/static/feather/icons/corner-up-right.svg
--rw-r--r--   0        0        0      667 2020-09-24 01:07:55.252134 platipy-0.6.0/platipy/backend/static/feather/icons/cpu.svg
--rw-r--r--   0        0        0      329 2020-09-24 01:07:55.252234 platipy-0.6.0/platipy/backend/static/feather/icons/credit-card.svg
--rw-r--r--   0        0        0      310 2020-09-24 01:07:55.252341 platipy-0.6.0/platipy/backend/static/feather/icons/crop.svg
--rw-r--r--   0        0        0      437 2020-09-24 01:07:55.252439 platipy-0.6.0/platipy/backend/static/feather/icons/crosshair.svg
--rw-r--r--   0        0        0      372 2020-09-24 01:07:55.252581 platipy-0.6.0/platipy/backend/static/feather/icons/database.svg
--rw-r--r--   0        0        0      374 2020-09-24 01:07:55.252708 platipy-0.6.0/platipy/backend/static/feather/icons/delete.svg
--rw-r--r--   0        0        0      295 2020-09-24 01:07:55.252840 platipy-0.6.0/platipy/backend/static/feather/icons/disc.svg
--rw-r--r--   0        0        0      334 2020-09-24 01:07:55.253093 platipy-0.6.0/platipy/backend/static/feather/icons/dollar-sign.svg
--rw-r--r--   0        0        0      387 2020-09-24 01:07:55.253211 platipy-0.6.0/platipy/backend/static/feather/icons/download-cloud.svg
--rw-r--r--   0        0        0      370 2020-09-24 01:07:55.253316 platipy-0.6.0/platipy/backend/static/feather/icons/download.svg
--rw-r--r--   0        0        0      274 2020-09-24 01:07:55.253412 platipy-0.6.0/platipy/backend/static/feather/icons/droplet.svg
--rw-r--r--   0        0        0      276 2020-09-24 01:07:55.253510 platipy-0.6.0/platipy/backend/static/feather/icons/edit-2.svg
--rw-r--r--   0        0        0      320 2020-09-24 01:07:55.253620 platipy-0.6.0/platipy/backend/static/feather/icons/edit-3.svg
--rw-r--r--   0        0        0      356 2020-09-24 01:07:55.253712 platipy-0.6.0/platipy/backend/static/feather/icons/edit.svg
--rw-r--r--   0        0        0      388 2020-09-24 01:07:55.253806 platipy-0.6.0/platipy/backend/static/feather/icons/external-link.svg
--rw-r--r--   0        0        0      460 2020-09-24 01:07:55.253958 platipy-0.6.0/platipy/backend/static/feather/icons/eye-off.svg
--rw-r--r--   0        0        0      316 2020-09-24 01:07:55.254059 platipy-0.6.0/platipy/backend/static/feather/icons/eye.svg
--rw-r--r--   0        0        0      303 2020-09-24 01:07:55.254145 platipy-0.6.0/platipy/backend/static/feather/icons/facebook.svg
--rw-r--r--   0        0        0      323 2020-09-24 01:07:55.254229 platipy-0.6.0/platipy/backend/static/feather/icons/fast-forward.svg
--rw-r--r--   0        0        0      373 2020-09-24 01:07:55.254328 platipy-0.6.0/platipy/backend/static/feather/icons/feather.svg
--rw-r--r--   0        0        0      387 2020-09-24 01:07:55.254428 platipy-0.6.0/platipy/backend/static/feather/icons/file-minus.svg
--rw-r--r--   0        0        0      431 2020-09-24 01:07:55.254523 platipy-0.6.0/platipy/backend/static/feather/icons/file-plus.svg
--rw-r--r--   0        0        0      473 2020-09-24 01:07:55.254608 platipy-0.6.0/platipy/backend/static/feather/icons/file-text.svg
--rw-r--r--   0        0        0      337 2020-09-24 01:07:55.254737 platipy-0.6.0/platipy/backend/static/feather/icons/file.svg
--rw-r--r--   0        0        0      586 2020-09-24 01:07:55.254831 platipy-0.6.0/platipy/backend/static/feather/icons/film.svg
--rw-r--r--   0        0        0      290 2020-09-24 01:07:55.254914 platipy-0.6.0/platipy/backend/static/feather/icons/filter.svg
--rw-r--r--   0        0        0      334 2020-09-24 01:07:55.255003 platipy-0.6.0/platipy/backend/static/feather/icons/flag.svg
--rw-r--r--   0        0        0      361 2020-09-24 01:07:55.255089 platipy-0.6.0/platipy/backend/static/feather/icons/folder-minus.svg
--rw-r--r--   0        0        0      405 2020-09-24 01:07:55.255184 platipy-0.6.0/platipy/backend/static/feather/icons/folder-plus.svg
--rw-r--r--   0        0        0      311 2020-09-24 01:07:55.255269 platipy-0.6.0/platipy/backend/static/feather/icons/folder.svg
--rw-r--r--   0        0        0      390 2020-09-24 01:07:55.255352 platipy-0.6.0/platipy/backend/static/feather/icons/frown.svg
--rw-r--r--   0        0        0      481 2020-09-24 01:07:55.255479 platipy-0.6.0/platipy/backend/static/feather/icons/gift.svg
--rw-r--r--   0        0        0      377 2020-09-24 01:07:55.255582 platipy-0.6.0/platipy/backend/static/feather/icons/git-branch.svg
--rw-r--r--   0        0        0      358 2020-09-24 01:07:55.255671 platipy-0.6.0/platipy/backend/static/feather/icons/git-commit.svg
--rw-r--r--   0        0        0      336 2020-09-24 01:07:55.255764 platipy-0.6.0/platipy/backend/static/feather/icons/git-merge.svg
--rw-r--r--   0        0        0      387 2020-09-24 01:07:55.255846 platipy-0.6.0/platipy/backend/static/feather/icons/git-pull-request.svg
--rw-r--r--   0        0        0      527 2020-09-24 01:07:55.255938 platipy-0.6.0/platipy/backend/static/feather/icons/github.svg
--rw-r--r--   0        0        0      490 2020-09-24 01:07:55.256033 platipy-0.6.0/platipy/backend/static/feather/icons/gitlab.svg
--rw-r--r--   0        0        0      409 2020-09-24 01:07:55.256126 platipy-0.6.0/platipy/backend/static/feather/icons/globe.svg
--rw-r--r--   0        0        0      404 2020-09-24 01:07:55.256255 platipy-0.6.0/platipy/backend/static/feather/icons/grid.svg
--rw-r--r--   0        0        0      478 2020-09-24 01:07:55.256343 platipy-0.6.0/platipy/backend/static/feather/icons/hard-drive.svg
--rw-r--r--   0        0        0      389 2020-09-24 01:07:55.256440 platipy-0.6.0/platipy/backend/static/feather/icons/hash.svg
--rw-r--r--   0        0        0      395 2020-09-24 01:07:55.256535 platipy-0.6.0/platipy/backend/static/feather/icons/headphones.svg
--rw-r--r--   0        0        0      371 2020-09-24 01:07:55.256622 platipy-0.6.0/platipy/backend/static/feather/icons/heart.svg
--rw-r--r--   0        0        0      362 2020-09-24 01:07:55.256707 platipy-0.6.0/platipy/backend/static/feather/icons/help-circle.svg
--rw-r--r--   0        0        0      332 2020-09-24 01:07:55.256793 platipy-0.6.0/platipy/backend/static/feather/icons/home.svg
--rw-r--r--   0        0        0      369 2020-09-24 01:07:55.256878 platipy-0.6.0/platipy/backend/static/feather/icons/image.svg
--rw-r--r--   0        0        0      405 2020-09-24 01:07:55.257009 platipy-0.6.0/platipy/backend/static/feather/icons/inbox.svg
--rw-r--r--   0        0        0      344 2020-09-24 01:07:55.257091 platipy-0.6.0/platipy/backend/static/feather/icons/info.svg
--rw-r--r--   0        0        0      399 2020-09-24 01:07:55.257217 platipy-0.6.0/platipy/backend/static/feather/icons/instagram.svg
--rw-r--r--   0        0        0      348 2020-09-24 01:07:55.257330 platipy-0.6.0/platipy/backend/static/feather/icons/italic.svg
--rw-r--r--   0        0        0      365 2020-09-24 01:07:55.257425 platipy-0.6.0/platipy/backend/static/feather/icons/layers.svg
--rw-r--r--   0        0        0      364 2020-09-24 01:07:55.257516 platipy-0.6.0/platipy/backend/static/feather/icons/layout.svg
--rw-r--r--   0        0        0      575 2020-09-24 01:07:55.257615 platipy-0.6.0/platipy/backend/static/feather/icons/life-buoy.svg
--rw-r--r--   0        0        0      355 2020-09-24 01:07:55.257711 platipy-0.6.0/platipy/backend/static/feather/icons/link-2.svg
--rw-r--r--   0        0        0      371 2020-09-24 01:07:55.257845 platipy-0.6.0/platipy/backend/static/feather/icons/link.svg
--rw-r--r--   0        0        0      400 2020-09-24 01:07:55.257935 platipy-0.6.0/platipy/backend/static/feather/icons/linkedin.svg
--rw-r--r--   0        0        0      473 2020-09-24 01:07:55.258022 platipy-0.6.0/platipy/backend/static/feather/icons/list.svg
--rw-r--r--   0        0        0      614 2020-09-24 01:07:55.258120 platipy-0.6.0/platipy/backend/static/feather/icons/loader.svg
--rw-r--r--   0        0        0      321 2020-09-24 01:07:55.258213 platipy-0.6.0/platipy/backend/static/feather/icons/lock.svg
--rw-r--r--   0        0        0      368 2020-09-24 01:07:55.258315 platipy-0.6.0/platipy/backend/static/feather/icons/log-in.svg
--rw-r--r--   0        0        0      367 2020-09-24 01:07:55.258418 platipy-0.6.0/platipy/backend/static/feather/icons/log-out.svg
--rw-r--r--   0        0        0      354 2020-09-24 01:07:55.258508 platipy-0.6.0/platipy/backend/static/feather/icons/mail.svg
--rw-r--r--   0        0        0      322 2020-09-24 01:07:55.258651 platipy-0.6.0/platipy/backend/static/feather/icons/map-pin.svg
--rw-r--r--   0        0        0      373 2020-09-24 01:07:55.258737 platipy-0.6.0/platipy/backend/static/feather/icons/map.svg
--rw-r--r--   0        0        0      400 2020-09-24 01:07:55.258832 platipy-0.6.0/platipy/backend/static/feather/icons/maximize-2.svg
--rw-r--r--   0        0        0      331 2020-09-24 01:07:55.258936 platipy-0.6.0/platipy/backend/static/feather/icons/maximize.svg
--rw-r--r--   0        0        0      389 2020-09-24 01:07:55.259046 platipy-0.6.0/platipy/backend/static/feather/icons/meh.svg
--rw-r--r--   0        0        0      346 2020-09-24 01:07:55.259151 platipy-0.6.0/platipy/backend/static/feather/icons/menu.svg
--rw-r--r--   0        0        0      428 2020-09-24 01:07:55.259250 platipy-0.6.0/platipy/backend/static/feather/icons/message-circle.svg
--rw-r--r--   0        0        0      305 2020-09-24 01:07:55.259354 platipy-0.6.0/platipy/backend/static/feather/icons/message-square.svg
--rw-r--r--   0        0        0      494 2020-09-24 01:07:55.259498 platipy-0.6.0/platipy/backend/static/feather/icons/mic-off.svg
--rw-r--r--   0        0        0      418 2020-09-24 01:07:55.260294 platipy-0.6.0/platipy/backend/static/feather/icons/mic.svg
--rw-r--r--   0        0        0      404 2020-09-24 01:07:55.260930 platipy-0.6.0/platipy/backend/static/feather/icons/minimize-2.svg
--rw-r--r--   0        0        0      331 2020-09-24 01:07:55.261347 platipy-0.6.0/platipy/backend/static/feather/icons/minimize.svg
--rw-r--r--   0        0        0      308 2020-09-24 01:07:55.261448 platipy-0.6.0/platipy/backend/static/feather/icons/minus-circle.svg
--rw-r--r--   0        0        0      330 2020-09-24 01:07:55.261545 platipy-0.6.0/platipy/backend/static/feather/icons/minus-square.svg
--rw-r--r--   0        0        0      261 2020-09-24 01:07:55.261633 platipy-0.6.0/platipy/backend/static/feather/icons/minus.svg
--rw-r--r--   0        0        0      370 2020-09-24 01:07:55.261765 platipy-0.6.0/platipy/backend/static/feather/icons/monitor.svg
--rw-r--r--   0        0        0      281 2020-09-24 01:07:55.262512 platipy-0.6.0/platipy/backend/static/feather/icons/moon.svg
--rw-r--r--   0        0        0      343 2020-09-24 01:07:55.262612 platipy-0.6.0/platipy/backend/static/feather/icons/more-horizontal.svg
--rw-r--r--   0        0        0      341 2020-09-24 01:07:55.262706 platipy-0.6.0/platipy/backend/static/feather/icons/more-vertical.svg
--rw-r--r--   0        0        0      486 2020-09-24 01:07:55.262836 platipy-0.6.0/platipy/backend/static/feather/icons/move.svg
--rw-r--r--   0        0        0      390 2020-09-24 01:07:55.262979 platipy-0.6.0/platipy/backend/static/feather/icons/music.svg
--rw-r--r--   0        0        0      279 2020-09-24 01:07:55.263138 platipy-0.6.0/platipy/backend/static/feather/icons/navigation-2.svg
--rw-r--r--   0        0        0      277 2020-09-24 01:07:55.263296 platipy-0.6.0/platipy/backend/static/feather/icons/navigation.svg
--rw-r--r--   0        0        0      318 2020-09-24 01:07:55.263412 platipy-0.6.0/platipy/backend/static/feather/icons/octagon.svg
--rw-r--r--   0        0        0      538 2020-09-24 01:07:55.263512 platipy-0.6.0/platipy/backend/static/feather/icons/package.svg
--rw-r--r--   0        0        0      352 2020-09-24 01:07:55.263604 platipy-0.6.0/platipy/backend/static/feather/icons/paperclip.svg
--rw-r--r--   0        0        0      352 2020-09-24 01:07:55.263708 platipy-0.6.0/platipy/backend/static/feather/icons/pause-circle.svg
--rw-r--r--   0        0        0      312 2020-09-24 01:07:55.263853 platipy-0.6.0/platipy/backend/static/feather/icons/pause.svg
--rw-r--r--   0        0        0      350 2020-09-24 01:07:55.263954 platipy-0.6.0/platipy/backend/static/feather/icons/percent.svg
--rw-r--r--   0        0        0      576 2020-09-24 01:07:55.264100 platipy-0.6.0/platipy/backend/static/feather/icons/phone-call.svg
--rw-r--r--   0        0        0      618 2020-09-24 01:07:55.269524 platipy-0.6.0/platipy/backend/static/feather/icons/phone-forwarded.svg
--rw-r--r--   0        0        0      617 2020-09-24 01:07:55.269763 platipy-0.6.0/platipy/backend/static/feather/icons/phone-incoming.svg
--rw-r--r--   0        0        0      613 2020-09-24 01:07:55.269963 platipy-0.6.0/platipy/backend/static/feather/icons/phone-missed.svg
--rw-r--r--   0        0        0      591 2020-09-24 01:07:55.270130 platipy-0.6.0/platipy/backend/static/feather/icons/phone-off.svg
--rw-r--r--   0        0        0      617 2020-09-24 01:07:55.270302 platipy-0.6.0/platipy/backend/static/feather/icons/phone-outgoing.svg
--rw-r--r--   0        0        0      520 2020-09-24 01:07:55.270717 platipy-0.6.0/platipy/backend/static/feather/icons/phone.svg
--rw-r--r--   0        0        0      315 2020-09-24 01:07:55.270907 platipy-0.6.0/platipy/backend/static/feather/icons/pie-chart.svg
--rw-r--r--   0        0        0      313 2020-09-24 01:07:55.271081 platipy-0.6.0/platipy/backend/static/feather/icons/play-circle.svg
--rw-r--r--   0        0        0      263 2020-09-24 01:07:55.271247 platipy-0.6.0/platipy/backend/static/feather/icons/play.svg
--rw-r--r--   0        0        0      351 2020-09-24 01:07:55.271436 platipy-0.6.0/platipy/backend/static/feather/icons/plus-circle.svg
--rw-r--r--   0        0        0      373 2020-09-24 01:07:55.271580 platipy-0.6.0/platipy/backend/static/feather/icons/plus-square.svg
--rw-r--r--   0        0        0      304 2020-09-24 01:07:55.271766 platipy-0.6.0/platipy/backend/static/feather/icons/plus.svg
--rw-r--r--   0        0        0      358 2020-09-24 01:07:55.271953 platipy-0.6.0/platipy/backend/static/feather/icons/pocket.svg
--rw-r--r--   0        0        0      308 2020-09-24 01:07:55.272095 platipy-0.6.0/platipy/backend/static/feather/icons/power.svg
--rw-r--r--   0        0        0      407 2020-09-24 01:07:55.272239 platipy-0.6.0/platipy/backend/static/feather/icons/printer.svg
--rw-r--r--   0        0        0      389 2020-09-24 01:07:55.272385 platipy-0.6.0/platipy/backend/static/feather/icons/radio.svg
--rw-r--r--   0        0        0      400 2020-09-24 01:07:55.272569 platipy-0.6.0/platipy/backend/static/feather/icons/refresh-ccw.svg
--rw-r--r--   0        0        0      400 2020-09-24 01:07:55.272714 platipy-0.6.0/platipy/backend/static/feather/icons/refresh-cw.svg
--rw-r--r--   0        0        0      392 2020-09-24 01:07:55.272857 platipy-0.6.0/platipy/backend/static/feather/icons/repeat.svg
--rw-r--r--   0        0        0      319 2020-09-24 01:07:55.272994 platipy-0.6.0/platipy/backend/static/feather/icons/rewind.svg
--rw-r--r--   0        0        0      317 2020-09-24 01:07:55.273181 platipy-0.6.0/platipy/backend/static/feather/icons/rotate-ccw.svg
--rw-r--r--   0        0        0      321 2020-09-24 01:07:55.273357 platipy-0.6.0/platipy/backend/static/feather/icons/rotate-cw.svg
--rw-r--r--   0        0        0      330 2020-09-24 01:07:55.273516 platipy-0.6.0/platipy/backend/static/feather/icons/rss.svg
--rw-r--r--   0        0        0      392 2020-09-24 01:07:55.273651 platipy-0.6.0/platipy/backend/static/feather/icons/save.svg
--rw-r--r--   0        0        0      444 2020-09-24 01:07:55.273806 platipy-0.6.0/platipy/backend/static/feather/icons/scissors.svg
--rw-r--r--   0        0        0      308 2020-09-24 01:07:55.273957 platipy-0.6.0/platipy/backend/static/feather/icons/search.svg
--rw-r--r--   0        0        0      314 2020-09-24 01:07:55.274113 platipy-0.6.0/platipy/backend/static/feather/icons/send.svg
--rw-r--r--   0        0        0      425 2020-09-24 01:07:55.274257 platipy-0.6.0/platipy/backend/static/feather/icons/server.svg
--rw-r--r--   0        0        0     1011 2020-09-24 01:07:55.274381 platipy-0.6.0/platipy/backend/static/feather/icons/settings.svg
--rw-r--r--   0        0        0      445 2020-09-24 01:07:55.274524 platipy-0.6.0/platipy/backend/static/feather/icons/share-2.svg
--rw-r--r--   0        0        0      364 2020-09-24 01:07:55.274626 platipy-0.6.0/platipy/backend/static/feather/icons/share.svg
--rw-r--r--   0        0        0      405 2020-09-24 01:07:55.274751 platipy-0.6.0/platipy/backend/static/feather/icons/shield-off.svg
--rw-r--r--   0        0        0      279 2020-09-24 01:07:55.274859 platipy-0.6.0/platipy/backend/static/feather/icons/shield.svg
--rw-r--r--   0        0        0      372 2020-09-24 01:07:55.275061 platipy-0.6.0/platipy/backend/static/feather/icons/shopping-bag.svg
--rw-r--r--   0        0        0      383 2020-09-24 01:07:55.275213 platipy-0.6.0/platipy/backend/static/feather/icons/shopping-cart.svg
--rw-r--r--   0        0        0      441 2020-09-24 01:07:55.275374 platipy-0.6.0/platipy/backend/static/feather/icons/shuffle.svg
--rw-r--r--   0        0        0      323 2020-09-24 01:07:55.275583 platipy-0.6.0/platipy/backend/static/feather/icons/sidebar.svg
--rw-r--r--   0        0        0      313 2020-09-24 01:07:55.276108 platipy-0.6.0/platipy/backend/static/feather/icons/skip-back.svg
--rw-r--r--   0        0        0      315 2020-09-24 01:07:55.276337 platipy-0.6.0/platipy/backend/static/feather/icons/skip-forward.svg
--rw-r--r--   0        0        0      552 2020-09-24 01:07:55.276522 platipy-0.6.0/platipy/backend/static/feather/icons/slack.svg
--rw-r--r--   0        0        0      312 2020-09-24 01:07:55.276639 platipy-0.6.0/platipy/backend/static/feather/icons/slash.svg
--rw-r--r--   0        0        0      611 2020-09-24 01:07:55.276739 platipy-0.6.0/platipy/backend/static/feather/icons/sliders.svg
--rw-r--r--   0        0        0      329 2020-09-24 01:07:55.276832 platipy-0.6.0/platipy/backend/static/feather/icons/smartphone.svg
--rw-r--r--   0        0        0      388 2020-09-24 01:07:55.276927 platipy-0.6.0/platipy/backend/static/feather/icons/smile.svg
--rw-r--r--   0        0        0      363 2020-09-24 01:07:55.277017 platipy-0.6.0/platipy/backend/static/feather/icons/speaker.svg
--rw-r--r--   0        0        0      280 2020-09-24 01:07:55.277417 platipy-0.6.0/platipy/backend/static/feather/icons/square.svg
--rw-r--r--   0        0        0      339 2020-09-24 01:07:55.277602 platipy-0.6.0/platipy/backend/static/feather/icons/star.svg
--rw-r--r--   0        0        0      309 2020-09-24 01:07:55.277743 platipy-0.6.0/platipy/backend/static/feather/icons/stop-circle.svg
--rw-r--r--   0        0        0      650 2020-09-24 01:07:55.277878 platipy-0.6.0/platipy/backend/static/feather/icons/sun.svg
--rw-r--r--   0        0        0      589 2020-09-24 01:07:55.278210 platipy-0.6.0/platipy/backend/static/feather/icons/sunrise.svg
--rw-r--r--   0        0        0      588 2020-09-24 01:07:55.278327 platipy-0.6.0/platipy/backend/static/feather/icons/sunset.svg
--rw-r--r--   0        0        0      355 2020-09-24 01:07:55.278442 platipy-0.6.0/platipy/backend/static/feather/icons/tablet.svg
--rw-r--r--   0        0        0      352 2020-09-24 01:07:55.278596 platipy-0.6.0/platipy/backend/static/feather/icons/tag.svg
--rw-r--r--   0        0        0      336 2020-09-24 01:07:55.278689 platipy-0.6.0/platipy/backend/static/feather/icons/target.svg
--rw-r--r--   0        0        0      310 2020-09-24 01:07:55.278799 platipy-0.6.0/platipy/backend/static/feather/icons/terminal.svg
--rw-r--r--   0        0        0      297 2020-09-24 01:07:55.279177 platipy-0.6.0/platipy/backend/static/feather/icons/thermometer.svg
--rw-r--r--   0        0        0      374 2020-09-24 01:07:55.279296 platipy-0.6.0/platipy/backend/static/feather/icons/thumbs-down.svg
--rw-r--r--   0        0        0      354 2020-09-24 01:07:55.279483 platipy-0.6.0/platipy/backend/static/feather/icons/thumbs-up.svg
--rw-r--r--   0        0        0      323 2020-09-24 01:07:55.279800 platipy-0.6.0/platipy/backend/static/feather/icons/toggle-left.svg
--rw-r--r--   0        0        0      325 2020-09-24 01:07:55.279911 platipy-0.6.0/platipy/backend/static/feather/icons/toggle-right.svg
--rw-r--r--   0        0        0      448 2020-09-24 01:07:55.280031 platipy-0.6.0/platipy/backend/static/feather/icons/trash-2.svg
--rw-r--r--   0        0        0      356 2020-09-24 01:07:55.280135 platipy-0.6.0/platipy/backend/static/feather/icons/trash.svg
--rw-r--r--   0        0        0      373 2020-09-24 01:07:55.280270 platipy-0.6.0/platipy/backend/static/feather/icons/trello.svg
--rw-r--r--   0        0        0      331 2020-09-24 01:07:55.280389 platipy-0.6.0/platipy/backend/static/feather/icons/trending-down.svg
--rw-r--r--   0        0        0      328 2020-09-24 01:07:55.280502 platipy-0.6.0/platipy/backend/static/feather/icons/trending-up.svg
--rw-r--r--   0        0        0      326 2020-09-24 01:07:55.280599 platipy-0.6.0/platipy/backend/static/feather/icons/triangle.svg
--rw-r--r--   0        0        0      415 2020-09-24 01:07:55.280711 platipy-0.6.0/platipy/backend/static/feather/icons/truck.svg
--rw-r--r--   0        0        0      320 2020-09-24 01:07:55.280850 platipy-0.6.0/platipy/backend/static/feather/icons/tv.svg
--rw-r--r--   0        0        0      408 2020-09-24 01:07:55.281192 platipy-0.6.0/platipy/backend/static/feather/icons/twitter.svg
--rw-r--r--   0        0        0      352 2020-09-24 01:07:55.281304 platipy-0.6.0/platipy/backend/static/feather/icons/type.svg
--rw-r--r--   0        0        0      290 2020-09-24 01:07:55.281450 platipy-0.6.0/platipy/backend/static/feather/icons/umbrella.svg
--rw-r--r--   0        0        0      319 2020-09-24 01:07:55.281639 platipy-0.6.0/platipy/backend/static/feather/icons/underline.svg
--rw-r--r--   0        0        0      322 2020-09-24 01:07:55.281751 platipy-0.6.0/platipy/backend/static/feather/icons/unlock.svg
--rw-r--r--   0        0        0      431 2020-09-24 01:07:55.281875 platipy-0.6.0/platipy/backend/static/feather/icons/upload-cloud.svg
--rw-r--r--   0        0        0      365 2020-09-24 01:07:55.281967 platipy-0.6.0/platipy/backend/static/feather/icons/upload.svg
--rw-r--r--   0        0        0      367 2020-09-24 01:07:55.282147 platipy-0.6.0/platipy/backend/static/feather/icons/user-check.svg
--rw-r--r--   0        0        0      365 2020-09-24 01:07:55.282293 platipy-0.6.0/platipy/backend/static/feather/icons/user-minus.svg
--rw-r--r--   0        0        0      408 2020-09-24 01:07:55.282477 platipy-0.6.0/platipy/backend/static/feather/icons/user-plus.svg
--rw-r--r--   0        0        0      404 2020-09-24 01:07:55.282632 platipy-0.6.0/platipy/backend/static/feather/icons/user-x.svg
--rw-r--r--   0        0        0      313 2020-09-24 01:07:55.282793 platipy-0.6.0/platipy/backend/static/feather/icons/user.svg
--rw-r--r--   0        0        0      400 2020-09-24 01:07:55.282945 platipy-0.6.0/platipy/backend/static/feather/icons/users.svg
--rw-r--r--   0        0        0      379 2020-09-24 01:07:55.283095 platipy-0.6.0/platipy/backend/static/feather/icons/video-off.svg
--rw-r--r--   0        0        0      329 2020-09-24 01:07:55.283358 platipy-0.6.0/platipy/backend/static/feather/icons/video.svg
--rw-r--r--   0        0        0      358 2020-09-24 01:07:55.283515 platipy-0.6.0/platipy/backend/static/feather/icons/voicemail.svg
--rw-r--r--   0        0        0      328 2020-09-24 01:07:55.283665 platipy-0.6.0/platipy/backend/static/feather/icons/volume-1.svg
--rw-r--r--   0        0        0      359 2020-09-24 01:07:55.283895 platipy-0.6.0/platipy/backend/static/feather/icons/volume-2.svg
--rw-r--r--   0        0        0      370 2020-09-24 01:07:55.284059 platipy-0.6.0/platipy/backend/static/feather/icons/volume-x.svg
--rw-r--r--   0        0        0      280 2020-09-24 01:07:55.284197 platipy-0.6.0/platipy/backend/static/feather/icons/volume.svg
--rw-r--r--   0        0        0      462 2020-09-24 01:07:55.284318 platipy-0.6.0/platipy/backend/static/feather/icons/watch.svg
--rw-r--r--   0        0        0      566 2020-09-24 01:07:55.284429 platipy-0.6.0/platipy/backend/static/feather/icons/wifi-off.svg
--rw-r--r--   0        0        0      398 2020-09-24 01:07:55.284555 platipy-0.6.0/platipy/backend/static/feather/icons/wifi.svg
--rw-r--r--   0        0        0      326 2020-09-24 01:07:55.284718 platipy-0.6.0/platipy/backend/static/feather/icons/wind.svg
--rw-r--r--   0        0        0      346 2020-09-24 01:07:55.284942 platipy-0.6.0/platipy/backend/static/feather/icons/x-circle.svg
--rw-r--r--   0        0        0      368 2020-09-24 01:07:55.285110 platipy-0.6.0/platipy/backend/static/feather/icons/x-square.svg
--rw-r--r--   0        0        0      299 2020-09-24 01:07:55.285217 platipy-0.6.0/platipy/backend/static/feather/icons/x.svg
--rw-r--r--   0        0        0      565 2020-09-24 01:07:55.285373 platipy-0.6.0/platipy/backend/static/feather/icons/youtube.svg
--rw-r--r--   0        0        0      433 2020-09-24 01:07:55.285493 platipy-0.6.0/platipy/backend/static/feather/icons/zap-off.svg
--rw-r--r--   0        0        0      282 2020-09-24 01:07:55.285605 platipy-0.6.0/platipy/backend/static/feather/icons/zap.svg
--rw-r--r--   0        0        0      397 2020-09-24 01:07:55.285729 platipy-0.6.0/platipy/backend/static/feather/icons/zoom-in.svg
--rw-r--r--   0        0        0      354 2020-09-24 01:07:55.285866 platipy-0.6.0/platipy/backend/static/feather/icons/zoom-out.svg
--rw-r--r--   0        0        0   212345 2020-09-24 01:07:55.287195 platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   358832 2020-09-24 01:07:55.333909 platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    70966 2020-09-24 01:07:55.334430 platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   294126 2020-09-24 01:07:55.344337 platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   123765 2020-09-24 01:07:55.344560 platipy-0.6.0/platipy/backend/static/js/bootstrap.js
--rw-r--r--   0        0        0   211967 2020-09-24 01:07:55.352697 platipy-0.6.0/platipy/backend/static/js/bootstrap.js.map
--rw-r--r--   0        0        0    51039 2020-09-24 01:07:55.353918 platipy-0.6.0/platipy/backend/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   176087 2020-09-24 01:07:55.359888 platipy-0.6.0/platipy/backend/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    86926 2020-09-24 01:07:55.360700 platipy-0.6.0/platipy/backend/static/js/jquery.min.js
--rw-r--r--   0        0        0    15076 2020-09-24 01:07:55.373842 platipy-0.6.0/platipy/backend/static/js/vue-resource.min.js
--rw-r--r--   0        0        0    67478 2020-09-24 01:07:55.375525 platipy-0.6.0/platipy/backend/static/js/vue-router.js
--rw-r--r--   0        0        0    90027 2020-09-24 01:07:55.379499 platipy-0.6.0/platipy/backend/static/js/vue.min.js
--rw-r--r--   0        0        0     2788 2020-09-24 01:07:55.383421 platipy-0.6.0/platipy/backend/static/pages/logs.js
--rw-r--r--   0        0        0     5298 2020-09-24 01:07:55.384679 platipy-0.6.0/platipy/backend/static/pages/status.js
--rw-r--r--   0        0        0     7828 2023-01-10 23:30:32.242328 platipy-0.6.0/platipy/backend/tasks.py
--rw-r--r--   0        0        0     4140 2020-09-24 01:07:55.390456 platipy-0.6.0/platipy/backend/templates/base.html
--rw-r--r--   0        0        0     3921 2020-09-24 01:07:55.391181 platipy-0.6.0/platipy/backend/templates/dashboard.html
--rw-r--r--   0        0        0     6795 2020-09-24 01:07:55.391827 platipy-0.6.0/platipy/backend/templates/endpoint_add.html
--rw-r--r--   0        0        0     5467 2020-09-24 01:07:55.393095 platipy-0.6.0/platipy/backend/templates/endpoint_view.html
--rw-r--r--   0        0        0     6249 2021-12-05 22:50:37.831629 platipy-0.6.0/platipy/backend/templates/status.html
--rw-r--r--   0        0        0      741 2022-09-30 08:24:03.900257 platipy-0.6.0/platipy/backend/tests/test_sample.py
--rw-r--r--   0        0        0     3367 2023-01-10 23:30:32.248180 platipy-0.6.0/platipy/backend/views.py
--rw-r--r--   0        0        0     1169 2020-09-24 01:07:55.402666 platipy-0.6.0/platipy/cli/README.md
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.403575 platipy-0.6.0/platipy/cli/__init__.py
--rwxr-xr-x   0        0        0     5001 2023-01-10 23:30:32.254287 platipy-0.6.0/platipy/cli/dicom_crawler.py
--rw-r--r--   0        0        0     1236 2021-06-29 01:11:48.212054 platipy-0.6.0/platipy/cli/nifti_to_rtstruct.py
--rwxr-xr-x   0        0        0     1685 2021-06-29 01:11:48.269727 platipy-0.6.0/platipy/cli/nifti_to_series.py
--rw-r--r--   0        0        0     1886 2021-06-29 01:11:48.357085 platipy-0.6.0/platipy/cli/rtstruct_to_nifti.py
--rw-r--r--   0        0        0     2274 2023-01-10 23:30:32.259189 platipy-0.6.0/platipy/cli/run.py
--rw-r--r--   0        0        0     4024 2023-01-10 23:30:32.263751 platipy-0.6.0/platipy/cli/segmentation.py
--rw-r--r--   0        0        0     3417 2023-01-10 23:30:32.268527 platipy-0.6.0/platipy/cli/tcia_download.py
--rw-r--r--   0        0        0    15000 2023-01-10 23:30:32.273191 platipy-0.6.0/platipy/client.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.405120 platipy-0.6.0/platipy/dicom/__init__.py
--rw-r--r--   0        0        0       38 2020-09-24 01:07:55.405441 platipy-0.6.0/platipy/dicom/communication/__init__.py
--rw-r--r--   0        0        0    12944 2023-01-10 23:30:32.278483 platipy-0.6.0/platipy/dicom/communication/connector.py
--rw-r--r--   0        0        0        0 2021-01-18 23:20:44.779450 platipy-0.6.0/platipy/dicom/download/__init__.py
--rw-r--r--   0        0        0     7658 2023-01-10 23:30:32.286422 platipy-0.6.0/platipy/dicom/download/tcia.py
--rw-r--r--   0        0        0        0 2021-06-29 01:11:48.485359 platipy-0.6.0/platipy/dicom/io/__init__.py
--rw-r--r--   0        0        0    44991 2023-01-13 03:17:49.348332 platipy-0.6.0/platipy/dicom/io/crawl.py
--rw-r--r--   0        0        0     3018 2023-01-10 23:30:32.298217 platipy-0.6.0/platipy/dicom/io/nifti_to_rtstruct.py
--rw-r--r--   0        0        0     6650 2021-06-29 01:11:52.464604 platipy-0.6.0/platipy/dicom/io/nifti_to_series.py
--rw-r--r--   0        0        0     1407 2022-04-26 21:19:39.391633 platipy-0.6.0/platipy/dicom/io/rtdose_to_nifti.py
--rw-r--r--   0        0        0    10884 2023-01-13 03:17:49.353985 platipy-0.6.0/platipy/dicom/io/rtstruct_to_nifti.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.413381 platipy-0.6.0/platipy/dicom/tests/__init__.py
--rw-r--r--   0        0        0     5357 2022-04-03 01:48:02.309503 platipy-0.6.0/platipy/dicom/tests/test_convert.py
--rw-r--r--   0        0        0       54 2021-06-29 01:11:48.765014 platipy-0.6.0/platipy/imaging/__init__.py
--rw-r--r--   0        0        0     5795 2022-09-30 08:24:03.900765 platipy-0.6.0/platipy/imaging/cnn/augmentations.py
--rw-r--r--   0        0        0        0 2021-08-16 22:22:45.997483 platipy-0.6.0/platipy/imaging/dose/__init__.py
--rw-r--r--   0        0        0     7283 2023-01-10 23:30:32.308259 platipy-0.6.0/platipy/imaging/dose/dvh.py
--rw-r--r--   0        0        0     6037 2023-01-10 23:30:32.313195 platipy-0.6.0/platipy/imaging/dose/metric.py
--rw-r--r--   0        0        0        0 2021-06-29 01:11:48.825652 platipy-0.6.0/platipy/imaging/generation/__init__.py
--rw-r--r--   0        0        0     5784 2023-02-28 20:16:22.057156 platipy-0.6.0/platipy/imaging/generation/augment.py
--rw-r--r--   0        0        0    17281 2023-02-28 20:16:22.064367 platipy-0.6.0/platipy/imaging/generation/dvf.py
--rw-r--r--   0        0        0     4439 2021-06-29 01:11:48.892694 platipy-0.6.0/platipy/imaging/generation/image.py
--rw-r--r--   0        0        0     6409 2021-06-29 01:11:48.915174 platipy-0.6.0/platipy/imaging/generation/mask.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.423370 platipy-0.6.0/platipy/imaging/label/__init__.py
--rw-r--r--   0        0        0    14832 2023-02-28 20:17:14.429720 platipy-0.6.0/platipy/imaging/label/comparison.py
--rw-r--r--   0        0        0    11895 2023-01-10 23:30:32.330299 platipy-0.6.0/platipy/imaging/label/fusion.py
--rw-r--r--   0        0        0    11220 2023-01-10 23:30:32.335463 platipy-0.6.0/platipy/imaging/label/iar.py
--rw-r--r--   0        0        0     4516 2021-06-29 01:11:49.133936 platipy-0.6.0/platipy/imaging/label/projection.py
--rw-r--r--   0        0        0     8454 2023-02-28 20:16:22.071461 platipy-0.6.0/platipy/imaging/label/utils.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.427639 platipy-0.6.0/platipy/imaging/projects/__init__.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.428625 platipy-0.6.0/platipy/imaging/projects/bronchus/__init__.py
--rw-r--r--   0        0        0    12968 2021-06-29 01:11:49.214198 platipy-0.6.0/platipy/imaging/projects/bronchus/bronchus.py
--rw-r--r--   0        0        0     2050 2023-01-10 23:30:32.341169 platipy-0.6.0/platipy/imaging/projects/bronchus/run.py
--rw-r--r--   0        0        0     6879 2023-02-28 20:17:14.436424 platipy-0.6.0/platipy/imaging/projects/cardiac/README.md
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.435626 platipy-0.6.0/platipy/imaging/projects/cardiac/__init__.py
--rw-r--r--   0        0        0    39052 2023-01-10 23:30:32.353095 platipy-0.6.0/platipy/imaging/projects/cardiac/run.py
--rw-r--r--   0        0        0     5063 2023-01-10 23:30:32.358279 platipy-0.6.0/platipy/imaging/projects/cardiac/service.py
--rw-r--r--   0        0        0        0 2021-10-17 22:11:45.916849 platipy-0.6.0/platipy/imaging/projects/multiatlas/__init__.py
--rw-r--r--   0        0        0    14436 2023-01-10 23:30:32.364516 platipy-0.6.0/platipy/imaging/projects/multiatlas/run.py
--rw-r--r--   0        0        0        0 2023-01-10 23:30:32.364641 platipy-0.6.0/platipy/imaging/projects/nnunet/__init__.py
--rw-r--r--   0        0        0     6193 2023-01-10 23:30:32.370198 platipy-0.6.0/platipy/imaging/projects/nnunet/run.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.439657 platipy-0.6.0/platipy/imaging/registration/__init__.py
--rw-r--r--   0        0        0    20021 2022-04-03 01:48:02.435461 platipy-0.6.0/platipy/imaging/registration/deformable.py
--rw-r--r--   0        0        0    11311 2022-04-03 01:48:02.456068 platipy-0.6.0/platipy/imaging/registration/linear.py
--rw-r--r--   0        0        0    12096 2023-01-10 23:30:32.376266 platipy-0.6.0/platipy/imaging/registration/utils.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.441148 platipy-0.6.0/platipy/imaging/tests/__init__.py
--rw-r--r--   0        0        0     3286 2023-01-10 23:30:32.381276 platipy-0.6.0/platipy/imaging/tests/data.py
--rw-r--r--   0        0        0     4614 2021-08-30 05:53:39.106114 platipy-0.6.0/platipy/imaging/tests/test_bronchus.py
--rw-r--r--   0        0        0    10088 2023-01-10 23:30:32.386204 platipy-0.6.0/platipy/imaging/tests/test_cardiac.py
--rw-r--r--   0        0        0     2932 2023-01-10 23:30:32.391752 platipy-0.6.0/platipy/imaging/tests/test_dvh.py
--rw-r--r--   0        0        0     2768 2023-01-10 23:30:32.397418 platipy-0.6.0/platipy/imaging/tests/test_metrics.py
--rw-r--r--   0        0        0     3210 2022-04-03 01:48:02.475609 platipy-0.6.0/platipy/imaging/tests/test_visualiser.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.443446 platipy-0.6.0/platipy/imaging/utils/__init__.py
--rw-r--r--   0        0        0     9420 2021-08-16 22:22:46.086270 platipy-0.6.0/platipy/imaging/utils/conduction.py
--rw-r--r--   0        0        0     3450 2023-02-28 20:16:22.080833 platipy-0.6.0/platipy/imaging/utils/crop.py
--rw-r--r--   0        0        0     2741 2021-10-17 22:11:45.921450 platipy-0.6.0/platipy/imaging/utils/geometry.py
--rw-r--r--   0        0        0     4638 2021-12-01 07:02:34.691115 platipy-0.6.0/platipy/imaging/utils/io.py
--rw-r--r--   0        0        0     5130 2021-06-29 01:11:49.699425 platipy-0.6.0/platipy/imaging/utils/lung.py
--rw-r--r--   0        0        0     6476 2021-08-30 05:53:39.179312 platipy-0.6.0/platipy/imaging/utils/math.py
--rw-r--r--   0        0        0     6386 2021-12-07 05:43:58.738200 platipy-0.6.0/platipy/imaging/utils/valve.py
--rw-r--r--   0        0        0    22812 2023-01-10 23:30:32.403163 platipy-0.6.0/platipy/imaging/utils/ventricle.py
--rw-r--r--   0        0        0    16308 2023-01-10 23:30:32.408272 platipy-0.6.0/platipy/imaging/utils/vessel.py
--rw-r--r--   0        0        0        0 2020-09-24 01:07:55.445467 platipy-0.6.0/platipy/imaging/visualisation/__init__.py
--rw-r--r--   0        0        0     9059 2022-04-03 01:48:02.563052 platipy-0.6.0/platipy/imaging/visualisation/animation.py
--rw-r--r--   0        0        0    10242 2023-01-13 03:17:49.359041 platipy-0.6.0/platipy/imaging/visualisation/comparison.py
--rw-r--r--   0        0        0     7598 2023-02-28 20:17:14.441668 platipy-0.6.0/platipy/imaging/visualisation/dose.py
--rw-r--r--   0        0        0     2592 2022-06-07 07:16:16.418721 platipy-0.6.0/platipy/imaging/visualisation/tests/test_use_case.py
--rw-r--r--   0        0        0    11258 2023-01-10 23:30:32.414583 platipy-0.6.0/platipy/imaging/visualisation/utils.py
--rw-r--r--   0        0        0     2180 2023-01-10 23:30:32.415874 platipy-0.6.0/platipy/imaging/visualisation/view.py
--rw-r--r--   0        0        0    65392 2023-01-31 02:48:51.298180 platipy-0.6.0/platipy/imaging/visualisation/visualiser.py
--rw-r--r--   0        0        0      513 2023-01-10 23:30:32.427428 platipy-0.6.0/platipy/utils.py
--rw-r--r--   0        0        0     2221 2023-02-28 20:21:06.070341 platipy-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7005 1970-01-01 00:00:00.000000 platipy-0.6.0/setup.py
--rw-r--r--   0        0        0     6562 1970-01-01 00:00:00.000000 platipy-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4195 2023-06-13 11:22:02.713763 platipy-0.6.1/README.md
+-rw-r--r--   0        0        0      334 2023-06-13 11:26:10.669915 platipy-0.6.1/platipy/__init__.py
+-rw-r--r--   0        0        0     6762 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/README.md
+-rw-r--r--   0        0        0     3025 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/__init__.py
+-rw-r--r--   0        0        0    18860 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/api.py
+-rw-r--r--   0        0        0     4341 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/application.py
+-rw-r--r--   0        0        0     4153 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/manage.py
+-rw-r--r--   0        0        0     6095 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/models.py
+-rw-r--r--   0        0        0    13946 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/sample/SampleClient.ipynb
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/sample/__init__.py
+-rw-r--r--   0        0        0     3838 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/sample/sample.py
+-rw-r--r--   0        0        0    37644 2023-06-13 11:22:02.757763 platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.css
+-rw-r--r--   0        0        0    98559 2023-06-13 11:22:02.761763 platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    28977 2023-06-13 11:22:02.761763 platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0    68241 2023-06-13 11:22:02.761763 platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0     4896 2023-06-13 11:22:02.761763 platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0    60752 2023-06-13 11:22:02.761763 platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0     4019 2023-06-13 11:22:02.761763 platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    26084 2023-06-13 11:22:02.761763 platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0   173597 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/css/bootstrap.css
+-rw-r--r--   0        0        0   430003 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/css/bootstrap.css.map
+-rw-r--r--   0        0        0   140936 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   562427 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0     1822 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/css/dashboard.css
+-rw-r--r--   0        0        0     1081 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/LICENSE
+-rw-r--r--   0        0        0    65962 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/feather.min.js
+-rw-r--r--   0        0        0      282 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/activity.svg
+-rw-r--r--   0        0        0      362 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/airplay.svg
+-rw-r--r--   0        0        0      353 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/alert-circle.svg
+-rw-r--r--   0        0        0      413 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/alert-octagon.svg
+-rw-r--r--   0        0        0      421 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/alert-triangle.svg
+-rw-r--r--   0        0        0      398 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/align-center.svg
+-rw-r--r--   0        0        0      399 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/align-justify.svg
+-rw-r--r--   0        0        0      396 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/align-left.svg
+-rw-r--r--   0        0        0      397 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/align-right.svg
+-rw-r--r--   0        0        0      345 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/anchor.svg
+-rw-r--r--   0        0        0      568 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/aperture.svg
+-rw-r--r--   0        0        0      361 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/archive.svg
+-rw-r--r--   0        0        0      360 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-down-circle.svg
+-rw-r--r--   0        0        0      315 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-down-left.svg
+-rw-r--r--   0        0        0      317 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-down-right.svg
+-rw-r--r--   0        0        0      313 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-down.svg
+-rw-r--r--   0        0        0      359 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-left-circle.svg
+-rw-r--r--   0        0        0      312 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-left.svg
+-rw-r--r--   0        0        0      361 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-right-circle.svg
+-rw-r--r--   0        0        0      314 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-right.svg
+-rw-r--r--   0        0        0      357 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-up-circle.svg
+-rw-r--r--   0        0        0      312 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-up-left.svg
+-rw-r--r--   0        0        0      314 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-up-right.svg
+-rw-r--r--   0        0        0      310 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/arrow-up.svg
+-rw-r--r--   0        0        0      322 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/at-sign.svg
+-rw-r--r--   0        0        0      325 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/award.svg
+-rw-r--r--   0        0        0      355 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/bar-chart-2.svg
+-rw-r--r--   0        0        0      353 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/bar-chart.svg
+-rw-r--r--   0        0        0      427 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/battery-charging.svg
+-rw-r--r--   0        0        0      326 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/battery.svg
+-rw-r--r--   0        0        0      375 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/bell-off.svg
+-rw-r--r--   0        0        0      315 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/bell.svg
+-rw-r--r--   0        0        0      298 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/bluetooth.svg
+-rw-r--r--   0        0        0      327 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/bold.svg
+-rw-r--r--   0        0        0      339 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/book-open.svg
+-rw-r--r--   0        0        0      345 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/book.svg
+-rw-r--r--   0        0        0      287 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/bookmark.svg
+-rw-r--r--   0        0        0      488 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/box.svg
+-rw-r--r--   0        0        0      343 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/briefcase.svg
+-rw-r--r--   0        0        0      410 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/calendar.svg
+-rw-r--r--   0        0        0      385 2023-06-13 11:22:02.765763 platipy-0.6.1/platipy/backend/static/feather/icons/camera-off.svg
+-rw-r--r--   0        0        0      356 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/camera.svg
+-rw-r--r--   0        0        0      384 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cast.svg
+-rw-r--r--   0        0        0      328 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/check-circle.svg
+-rw-r--r--   0        0        0      345 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/check-square.svg
+-rw-r--r--   0        0        0      262 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/check.svg
+-rw-r--r--   0        0        0      269 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevron-down.svg
+-rw-r--r--   0        0        0      270 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevron-left.svg
+-rw-r--r--   0        0        0      270 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevron-right.svg
+-rw-r--r--   0        0        0      268 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevron-up.svg
+-rw-r--r--   0        0        0      317 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevrons-down.svg
+-rw-r--r--   0        0        0      318 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevrons-left.svg
+-rw-r--r--   0        0        0      318 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevrons-right.svg
+-rw-r--r--   0        0        0      316 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chevrons-up.svg
+-rw-r--r--   0        0        0      448 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/chrome.svg
+-rw-r--r--   0        0        0      258 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/circle.svg
+-rw-r--r--   0        0        0      371 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/clipboard.svg
+-rw-r--r--   0        0        0      304 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/clock.svg
+-rw-r--r--   0        0        0      557 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cloud-drizzle.svg
+-rw-r--r--   0        0        0      345 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cloud-lightning.svg
+-rw-r--r--   0        0        0      371 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cloud-off.svg
+-rw-r--r--   0        0        0      421 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cloud-rain.svg
+-rw-r--r--   0        0        0      554 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cloud-snow.svg
+-rw-r--r--   0        0        0      280 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cloud.svg
+-rw-r--r--   0        0        0      307 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/code.svg
+-rw-r--r--   0        0        0      486 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/codepen.svg
+-rw-r--r--   0        0        0      447 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/coffee.svg
+-rw-r--r--   0        0        0      421 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/command.svg
+-rw-r--r--   0        0        0      342 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/compass.svg
+-rw-r--r--   0        0        0      351 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/copy.svg
+-rw-r--r--   0        0        0      314 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-down-left.svg
+-rw-r--r--   0        0        0      318 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-down-right.svg
+-rw-r--r--   0        0        0      317 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-left-down.svg
+-rw-r--r--   0        0        0      312 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-left-up.svg
+-rw-r--r--   0        0        0      318 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-right-down.svg
+-rw-r--r--   0        0        0      313 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-right-up.svg
+-rw-r--r--   0        0        0      312 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-up-left.svg
+-rw-r--r--   0        0        0      316 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/corner-up-right.svg
+-rw-r--r--   0        0        0      667 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/cpu.svg
+-rw-r--r--   0        0        0      329 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/credit-card.svg
+-rw-r--r--   0        0        0      310 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/crop.svg
+-rw-r--r--   0        0        0      437 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/crosshair.svg
+-rw-r--r--   0        0        0      372 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/database.svg
+-rw-r--r--   0        0        0      374 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/delete.svg
+-rw-r--r--   0        0        0      295 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/disc.svg
+-rw-r--r--   0        0        0      334 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/dollar-sign.svg
+-rw-r--r--   0        0        0      387 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/download-cloud.svg
+-rw-r--r--   0        0        0      370 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/download.svg
+-rw-r--r--   0        0        0      274 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/droplet.svg
+-rw-r--r--   0        0        0      276 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/edit-2.svg
+-rw-r--r--   0        0        0      320 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/edit-3.svg
+-rw-r--r--   0        0        0      356 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/edit.svg
+-rw-r--r--   0        0        0      388 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/external-link.svg
+-rw-r--r--   0        0        0      460 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/eye-off.svg
+-rw-r--r--   0        0        0      316 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/eye.svg
+-rw-r--r--   0        0        0      303 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/facebook.svg
+-rw-r--r--   0        0        0      323 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/fast-forward.svg
+-rw-r--r--   0        0        0      373 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/feather.svg
+-rw-r--r--   0        0        0      387 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/file-minus.svg
+-rw-r--r--   0        0        0      431 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/file-plus.svg
+-rw-r--r--   0        0        0      473 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/file-text.svg
+-rw-r--r--   0        0        0      337 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/file.svg
+-rw-r--r--   0        0        0      586 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/film.svg
+-rw-r--r--   0        0        0      290 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/filter.svg
+-rw-r--r--   0        0        0      334 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/flag.svg
+-rw-r--r--   0        0        0      361 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/folder-minus.svg
+-rw-r--r--   0        0        0      405 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/folder-plus.svg
+-rw-r--r--   0        0        0      311 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/folder.svg
+-rw-r--r--   0        0        0      390 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/frown.svg
+-rw-r--r--   0        0        0      481 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/gift.svg
+-rw-r--r--   0        0        0      377 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/git-branch.svg
+-rw-r--r--   0        0        0      358 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/git-commit.svg
+-rw-r--r--   0        0        0      336 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/git-merge.svg
+-rw-r--r--   0        0        0      387 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/git-pull-request.svg
+-rw-r--r--   0        0        0      527 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/github.svg
+-rw-r--r--   0        0        0      490 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/gitlab.svg
+-rw-r--r--   0        0        0      409 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/globe.svg
+-rw-r--r--   0        0        0      404 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/grid.svg
+-rw-r--r--   0        0        0      478 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/hard-drive.svg
+-rw-r--r--   0        0        0      389 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/hash.svg
+-rw-r--r--   0        0        0      395 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/headphones.svg
+-rw-r--r--   0        0        0      371 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/heart.svg
+-rw-r--r--   0        0        0      362 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/help-circle.svg
+-rw-r--r--   0        0        0      332 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/home.svg
+-rw-r--r--   0        0        0      369 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/image.svg
+-rw-r--r--   0        0        0      405 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/inbox.svg
+-rw-r--r--   0        0        0      344 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/info.svg
+-rw-r--r--   0        0        0      399 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/instagram.svg
+-rw-r--r--   0        0        0      348 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/italic.svg
+-rw-r--r--   0        0        0      365 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/layers.svg
+-rw-r--r--   0        0        0      364 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/layout.svg
+-rw-r--r--   0        0        0      575 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/life-buoy.svg
+-rw-r--r--   0        0        0      355 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/link-2.svg
+-rw-r--r--   0        0        0      371 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/link.svg
+-rw-r--r--   0        0        0      400 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/linkedin.svg
+-rw-r--r--   0        0        0      473 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/list.svg
+-rw-r--r--   0        0        0      614 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/loader.svg
+-rw-r--r--   0        0        0      321 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/lock.svg
+-rw-r--r--   0        0        0      368 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/log-in.svg
+-rw-r--r--   0        0        0      367 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/log-out.svg
+-rw-r--r--   0        0        0      354 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/mail.svg
+-rw-r--r--   0        0        0      322 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/map-pin.svg
+-rw-r--r--   0        0        0      373 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/map.svg
+-rw-r--r--   0        0        0      400 2023-06-13 11:22:02.769763 platipy-0.6.1/platipy/backend/static/feather/icons/maximize-2.svg
+-rw-r--r--   0        0        0      331 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/maximize.svg
+-rw-r--r--   0        0        0      389 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/meh.svg
+-rw-r--r--   0        0        0      346 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/menu.svg
+-rw-r--r--   0        0        0      428 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/message-circle.svg
+-rw-r--r--   0        0        0      305 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/message-square.svg
+-rw-r--r--   0        0        0      494 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/mic-off.svg
+-rw-r--r--   0        0        0      418 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/mic.svg
+-rw-r--r--   0        0        0      404 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/minimize-2.svg
+-rw-r--r--   0        0        0      331 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/minimize.svg
+-rw-r--r--   0        0        0      308 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/minus-circle.svg
+-rw-r--r--   0        0        0      330 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/minus-square.svg
+-rw-r--r--   0        0        0      261 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/minus.svg
+-rw-r--r--   0        0        0      370 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/monitor.svg
+-rw-r--r--   0        0        0      281 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/moon.svg
+-rw-r--r--   0        0        0      343 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/more-horizontal.svg
+-rw-r--r--   0        0        0      341 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/more-vertical.svg
+-rw-r--r--   0        0        0      486 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/move.svg
+-rw-r--r--   0        0        0      390 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/music.svg
+-rw-r--r--   0        0        0      279 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/navigation-2.svg
+-rw-r--r--   0        0        0      277 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/navigation.svg
+-rw-r--r--   0        0        0      318 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/octagon.svg
+-rw-r--r--   0        0        0      538 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/package.svg
+-rw-r--r--   0        0        0      352 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/paperclip.svg
+-rw-r--r--   0        0        0      352 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/pause-circle.svg
+-rw-r--r--   0        0        0      312 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/pause.svg
+-rw-r--r--   0        0        0      350 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/percent.svg
+-rw-r--r--   0        0        0      576 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/phone-call.svg
+-rw-r--r--   0        0        0      618 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/phone-forwarded.svg
+-rw-r--r--   0        0        0      617 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/phone-incoming.svg
+-rw-r--r--   0        0        0      613 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/phone-missed.svg
+-rw-r--r--   0        0        0      591 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/phone-off.svg
+-rw-r--r--   0        0        0      617 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/phone-outgoing.svg
+-rw-r--r--   0        0        0      520 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/phone.svg
+-rw-r--r--   0        0        0      315 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/pie-chart.svg
+-rw-r--r--   0        0        0      313 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/play-circle.svg
+-rw-r--r--   0        0        0      263 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/play.svg
+-rw-r--r--   0        0        0      351 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/plus-circle.svg
+-rw-r--r--   0        0        0      373 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/plus-square.svg
+-rw-r--r--   0        0        0      304 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/plus.svg
+-rw-r--r--   0        0        0      358 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/pocket.svg
+-rw-r--r--   0        0        0      308 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/power.svg
+-rw-r--r--   0        0        0      407 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/printer.svg
+-rw-r--r--   0        0        0      389 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/radio.svg
+-rw-r--r--   0        0        0      400 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/refresh-ccw.svg
+-rw-r--r--   0        0        0      400 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/refresh-cw.svg
+-rw-r--r--   0        0        0      392 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/repeat.svg
+-rw-r--r--   0        0        0      319 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/rewind.svg
+-rw-r--r--   0        0        0      317 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/rotate-ccw.svg
+-rw-r--r--   0        0        0      321 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/rotate-cw.svg
+-rw-r--r--   0        0        0      330 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/rss.svg
+-rw-r--r--   0        0        0      392 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/save.svg
+-rw-r--r--   0        0        0      444 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/scissors.svg
+-rw-r--r--   0        0        0      308 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/search.svg
+-rw-r--r--   0        0        0      314 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/send.svg
+-rw-r--r--   0        0        0      425 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/server.svg
+-rw-r--r--   0        0        0     1011 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/settings.svg
+-rw-r--r--   0        0        0      445 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/share-2.svg
+-rw-r--r--   0        0        0      364 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/share.svg
+-rw-r--r--   0        0        0      405 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/shield-off.svg
+-rw-r--r--   0        0        0      279 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/shield.svg
+-rw-r--r--   0        0        0      372 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/shopping-bag.svg
+-rw-r--r--   0        0        0      383 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/shopping-cart.svg
+-rw-r--r--   0        0        0      441 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/shuffle.svg
+-rw-r--r--   0        0        0      323 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/sidebar.svg
+-rw-r--r--   0        0        0      313 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/skip-back.svg
+-rw-r--r--   0        0        0      315 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/skip-forward.svg
+-rw-r--r--   0        0        0      552 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/slack.svg
+-rw-r--r--   0        0        0      312 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/slash.svg
+-rw-r--r--   0        0        0      611 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/sliders.svg
+-rw-r--r--   0        0        0      329 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/smartphone.svg
+-rw-r--r--   0        0        0      388 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/smile.svg
+-rw-r--r--   0        0        0      363 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/speaker.svg
+-rw-r--r--   0        0        0      280 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/square.svg
+-rw-r--r--   0        0        0      339 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/star.svg
+-rw-r--r--   0        0        0      309 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/stop-circle.svg
+-rw-r--r--   0        0        0      650 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/sun.svg
+-rw-r--r--   0        0        0      589 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/sunrise.svg
+-rw-r--r--   0        0        0      588 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/sunset.svg
+-rw-r--r--   0        0        0      355 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/tablet.svg
+-rw-r--r--   0        0        0      352 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/tag.svg
+-rw-r--r--   0        0        0      336 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/target.svg
+-rw-r--r--   0        0        0      310 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/terminal.svg
+-rw-r--r--   0        0        0      297 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/thermometer.svg
+-rw-r--r--   0        0        0      374 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/thumbs-down.svg
+-rw-r--r--   0        0        0      354 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/thumbs-up.svg
+-rw-r--r--   0        0        0      323 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/toggle-left.svg
+-rw-r--r--   0        0        0      325 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/toggle-right.svg
+-rw-r--r--   0        0        0      448 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/trash-2.svg
+-rw-r--r--   0        0        0      356 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/trash.svg
+-rw-r--r--   0        0        0      373 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/trello.svg
+-rw-r--r--   0        0        0      331 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/trending-down.svg
+-rw-r--r--   0        0        0      328 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/trending-up.svg
+-rw-r--r--   0        0        0      326 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/triangle.svg
+-rw-r--r--   0        0        0      415 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/truck.svg
+-rw-r--r--   0        0        0      320 2023-06-13 11:22:02.773763 platipy-0.6.1/platipy/backend/static/feather/icons/tv.svg
+-rw-r--r--   0        0        0      408 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/twitter.svg
+-rw-r--r--   0        0        0      352 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/type.svg
+-rw-r--r--   0        0        0      290 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/umbrella.svg
+-rw-r--r--   0        0        0      319 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/underline.svg
+-rw-r--r--   0        0        0      322 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/unlock.svg
+-rw-r--r--   0        0        0      431 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/upload-cloud.svg
+-rw-r--r--   0        0        0      365 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/upload.svg
+-rw-r--r--   0        0        0      367 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/user-check.svg
+-rw-r--r--   0        0        0      365 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/user-minus.svg
+-rw-r--r--   0        0        0      408 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/user-plus.svg
+-rw-r--r--   0        0        0      404 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/user-x.svg
+-rw-r--r--   0        0        0      313 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/user.svg
+-rw-r--r--   0        0        0      400 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/users.svg
+-rw-r--r--   0        0        0      379 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/video-off.svg
+-rw-r--r--   0        0        0      329 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/video.svg
+-rw-r--r--   0        0        0      358 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/voicemail.svg
+-rw-r--r--   0        0        0      328 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/volume-1.svg
+-rw-r--r--   0        0        0      359 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/volume-2.svg
+-rw-r--r--   0        0        0      370 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/volume-x.svg
+-rw-r--r--   0        0        0      280 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/volume.svg
+-rw-r--r--   0        0        0      462 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/watch.svg
+-rw-r--r--   0        0        0      566 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/wifi-off.svg
+-rw-r--r--   0        0        0      398 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/wifi.svg
+-rw-r--r--   0        0        0      326 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/wind.svg
+-rw-r--r--   0        0        0      346 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/x-circle.svg
+-rw-r--r--   0        0        0      368 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/x-square.svg
+-rw-r--r--   0        0        0      299 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/x.svg
+-rw-r--r--   0        0        0      565 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/youtube.svg
+-rw-r--r--   0        0        0      433 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/zap-off.svg
+-rw-r--r--   0        0        0      282 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/zap.svg
+-rw-r--r--   0        0        0      397 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/zoom-in.svg
+-rw-r--r--   0        0        0      354 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/feather/icons/zoom-out.svg
+-rw-r--r--   0        0        0   212345 2023-06-13 11:22:02.777763 platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   358832 2023-06-13 11:22:02.781763 platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    70966 2023-06-13 11:22:02.781763 platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   294126 2023-06-13 11:22:02.781763 platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   123765 2023-06-13 11:22:02.781763 platipy-0.6.1/platipy/backend/static/js/bootstrap.js
+-rw-r--r--   0        0        0   211967 2023-06-13 11:22:02.781763 platipy-0.6.1/platipy/backend/static/js/bootstrap.js.map
+-rw-r--r--   0        0        0    51039 2023-06-13 11:22:02.781763 platipy-0.6.1/platipy/backend/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   176087 2023-06-13 11:22:02.781763 platipy-0.6.1/platipy/backend/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    86926 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/static/js/jquery.min.js
+-rw-r--r--   0        0        0    15076 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/static/js/vue-resource.min.js
+-rw-r--r--   0        0        0    67478 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/static/js/vue-router.js
+-rw-r--r--   0        0        0    90027 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/static/js/vue.min.js
+-rw-r--r--   0        0        0     2788 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/static/pages/logs.js
+-rw-r--r--   0        0        0     5298 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/static/pages/status.js
+-rw-r--r--   0        0        0     7828 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/tasks.py
+-rw-r--r--   0        0        0     4140 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/templates/base.html
+-rw-r--r--   0        0        0     3921 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/templates/dashboard.html
+-rw-r--r--   0        0        0     6795 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/templates/endpoint_add.html
+-rw-r--r--   0        0        0     5467 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/templates/endpoint_view.html
+-rw-r--r--   0        0        0     6249 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/templates/status.html
+-rw-r--r--   0        0        0     3367 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/backend/views.py
+-rw-r--r--   0        0        0     1169 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/__init__.py
+-rwxr-xr-x   0        0        0     5001 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/dicom_crawler.py
+-rw-r--r--   0        0        0     1236 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/nifti_to_rtstruct.py
+-rwxr-xr-x   0        0        0     1685 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/nifti_to_series.py
+-rw-r--r--   0        0        0     1886 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/rtstruct_to_nifti.py
+-rw-r--r--   0        0        0     2274 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/run.py
+-rw-r--r--   0        0        0     4024 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/segmentation.py
+-rw-r--r--   0        0        0     3417 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/cli/tcia_download.py
+-rw-r--r--   0        0        0    15000 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/client.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/communication/__init__.py
+-rw-r--r--   0        0        0    12944 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/communication/connector.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/download/__init__.py
+-rw-r--r--   0        0        0     7658 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/download/tcia.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/io/__init__.py
+-rw-r--r--   0        0        0    44991 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/io/crawl.py
+-rw-r--r--   0        0        0     3018 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/io/nifti_to_rtstruct.py
+-rw-r--r--   0        0        0     6650 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/io/nifti_to_series.py
+-rw-r--r--   0        0        0     1407 2023-06-13 11:22:02.785763 platipy-0.6.1/platipy/dicom/io/rtdose_to_nifti.py
+-rw-r--r--   0        0        0    10884 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/dicom/io/rtstruct_to_nifti.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/dicom/tests/__init__.py
+-rw-r--r--   0        0        0     5357 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/dicom/tests/test_convert.py
+-rw-r--r--   0        0        0       54 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/dose/__init__.py
+-rw-r--r--   0        0        0     7283 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/dose/dvh.py
+-rw-r--r--   0        0        0     6037 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/dose/metric.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/generation/__init__.py
+-rw-r--r--   0        0        0     5784 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/generation/augment.py
+-rw-r--r--   0        0        0    17281 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/generation/dvf.py
+-rw-r--r--   0        0        0     4439 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/generation/image.py
+-rw-r--r--   0        0        0     6409 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/generation/mask.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/label/__init__.py
+-rw-r--r--   0        0        0    14832 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/label/comparison.py
+-rw-r--r--   0        0        0    11895 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/label/fusion.py
+-rw-r--r--   0        0        0    11220 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/label/iar.py
+-rw-r--r--   0        0        0     4516 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/label/projection.py
+-rw-r--r--   0        0        0     8454 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/label/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/bronchus/__init__.py
+-rw-r--r--   0        0        0    12968 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/bronchus/bronchus.py
+-rw-r--r--   0        0        0     2050 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/bronchus/run.py
+-rw-r--r--   0        0        0     7524 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/cardiac/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/cardiac/__init__.py
+-rw-r--r--   0        0        0    39052 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/cardiac/run.py
+-rw-r--r--   0        0        0     5063 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/cardiac/service.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/multiatlas/__init__.py
+-rw-r--r--   0        0        0    14436 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/multiatlas/run.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/nnunet/__init__.py
+-rw-r--r--   0        0        0     6193 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/projects/nnunet/run.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/registration/__init__.py
+-rw-r--r--   0        0        0    20021 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/registration/deformable.py
+-rw-r--r--   0        0        0    11311 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/registration/linear.py
+-rw-r--r--   0        0        0    12096 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/registration/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/tests/__init__.py
+-rw-r--r--   0        0        0     3286 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/tests/data.py
+-rw-r--r--   0        0        0     4614 2023-06-13 11:22:02.789763 platipy-0.6.1/platipy/imaging/tests/test_bronchus.py
+-rw-r--r--   0        0        0    10088 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/tests/test_cardiac.py
+-rw-r--r--   0        0        0     2932 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/tests/test_dvh.py
+-rw-r--r--   0        0        0     2768 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/tests/test_metrics.py
+-rw-r--r--   0        0        0     3210 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/tests/test_visualiser.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/__init__.py
+-rw-r--r--   0        0        0     9420 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/conduction.py
+-rw-r--r--   0        0        0     3450 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/crop.py
+-rw-r--r--   0        0        0     2741 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/geometry.py
+-rw-r--r--   0        0        0     4638 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/io.py
+-rw-r--r--   0        0        0     5130 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/lung.py
+-rw-r--r--   0        0        0     6476 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/math.py
+-rw-r--r--   0        0        0     6386 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/valve.py
+-rw-r--r--   0        0        0    22953 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/ventricle.py
+-rw-r--r--   0        0        0    16308 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/utils/vessel.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/__init__.py
+-rw-r--r--   0        0        0     9059 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/animation.py
+-rw-r--r--   0        0        0    10242 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/comparison.py
+-rw-r--r--   0        0        0     7598 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/dose.py
+-rw-r--r--   0        0        0     2592 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/tests/test_use_case.py
+-rw-r--r--   0        0        0    11258 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/utils.py
+-rw-r--r--   0        0        0     2180 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/view.py
+-rw-r--r--   0        0        0    65392 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/imaging/visualisation/visualiser.py
+-rw-r--r--   0        0        0      513 2023-06-13 11:22:02.793763 platipy-0.6.1/platipy/utils.py
+-rw-r--r--   0        0        0     2229 2023-06-13 11:26:10.673915 platipy-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6669 1970-01-01 00:00:00.000000 platipy-0.6.1/setup.py
+-rw-r--r--   0        0        0     6283 1970-01-01 00:00:00.000000 platipy-0.6.1/PKG-INFO
```

### Comparing `platipy-0.6.0/README.md` & `platipy-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-# PlatiPy
-
+# PlatiPy 
 ## Processing Library and Analysis Toolkit for Medical Imaging in Python
 
-[![Tests](https://github.com/pyplati/platipy/actions/workflows/pull_request.yml/badge.svg?event=pull_request)](https://github.com/pyplati/platipy/actions/workflows/pull_request.yml)
-[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
-
 PlatiPy is a library of **amazing** tools for image processing and analysis - designed specifically
-for medical imaging!
+for medical imaging! 
 
 Check out the [PlatiPy documentation](https://pyplati.github.io/platipy/) for more info.
 
-This project was motivated by the need for a simple way to use, visualise, process, and analyse
+This project was motivated by the need for a simple way to use, visualise, process, and analyse 
 medical images. Many of the tools and algorithms are designed in the context of radiation therapy,
 although they are more widely applicable to other fields that use 2D, 3D, or 4D imaging.
 
 PlatiPy is written in Python, and uses SimpleITK, VTK, and standard Python libraries. Jupyter
 notebooks are provided where possible, mainly for guidance on getting started with using the tools.
 We welcome feedback and contributions from the community (yes, you!) and you can find more
 information about contributing [here](https://pyplati.github.io/platipy/contributing.html).
 
 ## What can I do with **platipy**?
-
-A lot! A good place to start is by looking in the
+A lot! A good place to start is by looking in the 
 [examples directory](https://github.com/pyplati/platipy/tree/master/examples).
 
 Some examples of what PlatiPy can do:
-
-- DICOM organising and converting:
-  - Bulk convert from multiple series and studies with a single function
-  - Convert DICOM-RT structure and dose filesto NIfTI images
-  - Create DICOM-RT structure files from binary masks e.g. from automatic contouring algorithms
-- Image registration
-  - Register images and transform labels with a few lines of code
-  - Linear transformations: rigid, affine, similarity
-  - Non-linear deformable transformations: demons, b-splines
-  - Multiple metrics for optimisation
-- Atlas-based segmentation
-  - A suite of tools that can be used out-of-the-box
-  - Includes advanced algorithms for
-      [iterative atlas selection](https://doi.org/10.1088/1361-6560/ab652a/) and
+ - DICOM organising and converting:
+    * Bulk convert from multiple series and studies with a single function
+    * Convert DICOM-RT structure and dose files to NIfTI images
+    * Create DICOM-RT structure files from binary masks e.g. from automatic contouring algorithms
+ - Image registration
+    * Register images and transform labels with a few lines of code
+    * Linear transformations: rigid, affine, similarity
+    * Non-linear deformable transformations: demons, b-splines
+    * Multiple metrics for optimisation
+ - Atlas-based segmentation
+    * A suite of tools that can be used out-of-the-box
+    * Includes advanced algorithms for 
+      [iterative atlas selection](https://doi.org/10.1088/1361-6560/ab652a/) and 
       [vessel splining](https://doi.org/10.1088/1361-6560/abcb1d/)
-- Synthetic deformation field generation
-  - Simulate anatomically realistic shifts, expansions, and bending
-  - Compare DIR results from clinical systems
-- Basic tools for image processing and analysis
-  - Computing label similarity metrics: DSC, mean distance to agreement, Hausdorff distance, and more
-  - Cropping images to a region of interest
-  - Rotate images and generate maximum/mean intensity projections (beams eye view modelling)
+ - Synthetic deformation field generation
+    * Simulate anatomically realistic shifts, expansions, and bending
+    * Compare DIR results from clinical systems
+ - Basic tools for image processing and analysis
+    * Computing label similarity metrics: DSC, mean distance to agreement, Hausdorff distance, and more
+    * Cropping images to a region of interest
+    * Rotate images and generate maximum/mean intensity projections (beams eye view modelling)
 
 A major part of this package is **visualisation**, and some examples are shown below!
 
 #### Visualise some contours
 
 ``` python
 from platipy.imaging import ImageVisualiser
@@ -76,15 +70,15 @@
 vis.add_comparison_overlay(image_2_registered)
 fig = vis.show()
 ```
 
 ![Figure 2](assets/figure_2.png)
 
 #### Calculate deformation vector fields
-
+    
 ```python
 from platipy.imaging.registration.deformable import fast_symmetric_forces_demons_registration
 
 image_2_deformed, tfm_dir, dvf = fast_symmetric_forces_demons_registration(
 image_1,
 image_2_registered
 )
@@ -101,15 +95,14 @@
 )
 fig = vis.show()
 ```
 
 ![Figure 3](assets/figure_3.png)
 
 ## Getting started
-
 There aren't many requirements, just an installed Python interpreter (3.7 or greater). PlatiPy can
 be installed with **pip**:
 
 ```bash
 pip install platipy
 ```
 
@@ -120,9 +113,9 @@
 pip install platipy[cardiac]
 pip install platipy[nnunet]
 pip install platipy[backend]
 ```
 
 ## Authors
 
-- **Phillip Chlap** - [phillip.chlap@unsw.edu.au](phillip.chlap@unsw.edu.au)
-- **Robert Finnegan** - [robert.finnegan@sydney.edu.au](robert.finnegan@sydney.edu.au)
+* **Phillip Chlap** - [phillip.chlap@unsw.edu.au](phillip.chlap@unsw.edu.au)
+* **Robert Finnegan** - [robert.finnegan@sydney.edu.au](robert.finnegan@sydney.edu.au)
```

### Comparing `platipy-0.6.0/platipy/backend/README.md` & `platipy-0.6.1/platipy/backend/README.md`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/__init__.py` & `platipy-0.6.1/platipy/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/api.py` & `platipy-0.6.1/platipy/backend/api.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/application.py` & `platipy-0.6.1/platipy/backend/application.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/manage.py` & `platipy-0.6.1/platipy/backend/manage.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/models.py` & `platipy-0.6.1/platipy/backend/models.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/sample/SampleClient.ipynb` & `platipy-0.6.1/platipy/backend/sample/SampleClient.ipynb`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/sample/sample.py` & `platipy-0.6.1/platipy/backend/sample/sample.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.css` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.css.map` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.min.css` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-grid.min.css.map` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.css` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.css.map` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.min.css` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap-reboot.min.css.map` & `platipy-0.6.1/platipy/backend/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap.css` & `platipy-0.6.1/platipy/backend/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap.css.map` & `platipy-0.6.1/platipy/backend/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap.min.css` & `platipy-0.6.1/platipy/backend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/bootstrap.min.css.map` & `platipy-0.6.1/platipy/backend/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/css/dashboard.css` & `platipy-0.6.1/platipy/backend/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/LICENSE` & `platipy-0.6.1/platipy/backend/static/feather/LICENSE`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/feather.min.js` & `platipy-0.6.1/platipy/backend/static/feather/feather.min.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/aperture.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/cloud-drizzle.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/cloud-snow.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/cpu.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/film.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/film.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/github.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/github.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/life-buoy.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/loader.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/loader.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/package.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/package.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/phone-call.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/phone-call.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/phone-forwarded.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/phone-incoming.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/phone-missed.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/phone-off.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/phone-off.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/phone-outgoing.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/phone.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/phone.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/settings.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/slack.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/sliders.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/sliders.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/sun.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/sunrise.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/sunset.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/wifi-off.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/feather/icons/youtube.svg` & `platipy-0.6.1/platipy/backend/static/feather/icons/youtube.svg`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.js` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.js.map` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.min.js` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.bundle.min.js.map` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.js` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.js.map` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.min.js` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/bootstrap.min.js.map` & `platipy-0.6.1/platipy/backend/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/jquery.min.js` & `platipy-0.6.1/platipy/backend/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/vue-resource.min.js` & `platipy-0.6.1/platipy/backend/static/js/vue-resource.min.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/vue-router.js` & `platipy-0.6.1/platipy/backend/static/js/vue-router.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/js/vue.min.js` & `platipy-0.6.1/platipy/backend/static/js/vue.min.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/pages/logs.js` & `platipy-0.6.1/platipy/backend/static/pages/logs.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/static/pages/status.js` & `platipy-0.6.1/platipy/backend/static/pages/status.js`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/tasks.py` & `platipy-0.6.1/platipy/backend/tasks.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/templates/base.html` & `platipy-0.6.1/platipy/backend/templates/base.html`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/templates/dashboard.html` & `platipy-0.6.1/platipy/backend/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/templates/endpoint_add.html` & `platipy-0.6.1/platipy/backend/templates/endpoint_add.html`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/templates/endpoint_view.html` & `platipy-0.6.1/platipy/backend/templates/endpoint_view.html`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/templates/status.html` & `platipy-0.6.1/platipy/backend/templates/status.html`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/backend/views.py` & `platipy-0.6.1/platipy/backend/views.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/README.md` & `platipy-0.6.1/platipy/cli/README.md`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/dicom_crawler.py` & `platipy-0.6.1/platipy/cli/dicom_crawler.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/nifti_to_rtstruct.py` & `platipy-0.6.1/platipy/cli/nifti_to_rtstruct.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/nifti_to_series.py` & `platipy-0.6.1/platipy/cli/nifti_to_series.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/rtstruct_to_nifti.py` & `platipy-0.6.1/platipy/cli/rtstruct_to_nifti.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/run.py` & `platipy-0.6.1/platipy/cli/run.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/segmentation.py` & `platipy-0.6.1/platipy/cli/segmentation.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/cli/tcia_download.py` & `platipy-0.6.1/platipy/cli/tcia_download.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/client.py` & `platipy-0.6.1/platipy/client.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/communication/connector.py` & `platipy-0.6.1/platipy/dicom/communication/connector.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/download/tcia.py` & `platipy-0.6.1/platipy/dicom/download/tcia.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/io/crawl.py` & `platipy-0.6.1/platipy/dicom/io/crawl.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/io/nifti_to_rtstruct.py` & `platipy-0.6.1/platipy/dicom/io/nifti_to_rtstruct.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/io/nifti_to_series.py` & `platipy-0.6.1/platipy/dicom/io/nifti_to_series.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/io/rtdose_to_nifti.py` & `platipy-0.6.1/platipy/dicom/io/rtdose_to_nifti.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/io/rtstruct_to_nifti.py` & `platipy-0.6.1/platipy/dicom/io/rtstruct_to_nifti.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/dicom/tests/test_convert.py` & `platipy-0.6.1/platipy/dicom/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/dose/dvh.py` & `platipy-0.6.1/platipy/imaging/dose/dvh.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/dose/metric.py` & `platipy-0.6.1/platipy/imaging/dose/metric.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/generation/augment.py` & `platipy-0.6.1/platipy/imaging/generation/augment.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/generation/dvf.py` & `platipy-0.6.1/platipy/imaging/generation/dvf.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/generation/image.py` & `platipy-0.6.1/platipy/imaging/generation/image.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/generation/mask.py` & `platipy-0.6.1/platipy/imaging/generation/mask.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/label/comparison.py` & `platipy-0.6.1/platipy/imaging/label/comparison.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/label/fusion.py` & `platipy-0.6.1/platipy/imaging/label/fusion.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/label/iar.py` & `platipy-0.6.1/platipy/imaging/label/iar.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/label/projection.py` & `platipy-0.6.1/platipy/imaging/label/projection.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/label/utils.py` & `platipy-0.6.1/platipy/imaging/label/utils.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/projects/bronchus/bronchus.py` & `platipy-0.6.1/platipy/imaging/projects/bronchus/bronchus.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/projects/bronchus/run.py` & `platipy-0.6.1/platipy/imaging/projects/bronchus/run.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/projects/cardiac/README.md` & `platipy-0.6.1/platipy/imaging/projects/cardiac/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -114,14 +114,22 @@
 ### Run from a Jupyter Notebook
 
 A [Jupyter Notebook](https://github.com/pyplati/platipy/blob/master/examples/cardiac_segmentation.ipynb)
 is available containing an example.
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pyplati/platipy/blob/master/examples/cardiac_segmentation.ipynb)
 
+## Left Ventricle 17 Segment Model
+
+PlatiPy provides a tool for automatically segmenting the 17 Left Ventricle segments as defined in: <https://www.ahajournals.org/doi/pdf/10.1161/hc0402.102975>
+
+A [Jupyter Notebook](https://github.com/pyplati/platipy/blob/master/examples/left_ventricle_17_segments.ipynb) is provided containing an example to segment the 17 segments. This can be combined with the output of the Cardiac auto-segmentation example above.
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pyplati/platipy/blob/master/examples/left_ventricle_17_segments.ipynb)
+
 ## Troubleshooting
 
 ### Problem: I get an error message indicating a `CUDA error: no kernel image is available for execution on the device`
 
 Solution: The pytorch version installed via the usual pip command above isn't always necessarily
 the correct version needed for your operating system and CUDA version. Follow instructions
 [here](https://pytorch.org/get-started/locally/) to install the correct version of pytorch.
```

### Comparing `platipy-0.6.0/platipy/imaging/projects/cardiac/run.py` & `platipy-0.6.1/platipy/imaging/projects/cardiac/run.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/projects/cardiac/service.py` & `platipy-0.6.1/platipy/imaging/projects/cardiac/service.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/projects/multiatlas/run.py` & `platipy-0.6.1/platipy/imaging/projects/multiatlas/run.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/projects/nnunet/run.py` & `platipy-0.6.1/platipy/imaging/projects/nnunet/run.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/registration/deformable.py` & `platipy-0.6.1/platipy/imaging/registration/deformable.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/registration/linear.py` & `platipy-0.6.1/platipy/imaging/registration/linear.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/registration/utils.py` & `platipy-0.6.1/platipy/imaging/registration/utils.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/tests/data.py` & `platipy-0.6.1/platipy/imaging/tests/data.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/tests/test_bronchus.py` & `platipy-0.6.1/platipy/imaging/tests/test_bronchus.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/tests/test_cardiac.py` & `platipy-0.6.1/platipy/imaging/tests/test_cardiac.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/tests/test_dvh.py` & `platipy-0.6.1/platipy/imaging/tests/test_dvh.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/tests/test_metrics.py` & `platipy-0.6.1/platipy/imaging/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/tests/test_visualiser.py` & `platipy-0.6.1/platipy/imaging/tests/test_visualiser.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/conduction.py` & `platipy-0.6.1/platipy/imaging/utils/conduction.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/crop.py` & `platipy-0.6.1/platipy/imaging/utils/crop.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/geometry.py` & `platipy-0.6.1/platipy/imaging/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/io.py` & `platipy-0.6.1/platipy/imaging/utils/io.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/lung.py` & `platipy-0.6.1/platipy/imaging/utils/lung.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/math.py` & `platipy-0.6.1/platipy/imaging/utils/math.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/valve.py` & `platipy-0.6.1/platipy/imaging/utils/valve.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/utils/ventricle.py` & `platipy-0.6.1/platipy/imaging/utils/ventricle.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,18 @@
         segment_img *= 0
 
     return sitk.Cast(segment_img, template_img.GetPixelID())
 
 
 def generate_left_ventricle_segments(
     contours,
-    label_left_ventricle="LEFTVENTRICLE",
-    label_left_atrium="LEFTATRIUM",
-    label_right_ventricle="RIGHTVENTRICLE",
-    label_heart="WHOLEHEART",
+    label_left_ventricle="Ventricle_L",
+    label_left_atrium="Atrium_L",
+    label_right_ventricle="Ventricle_R",
+    label_heart="Heart",
     myocardium_thickness_mm=10,
     hole_fill_mm=3,
     optimiser_tol_degrees=1,
     optimiser_max_iter=10,
     min_area_mm2=50,
     verbose=False,
 ):
@@ -98,18 +98,21 @@
         5.  Geometric operations are used to define the segments
         6.  Everything is rotated back to the normal orientation
         7.  Some post-processing *magic*
 
     Args:
         contours (dict): A dictionary containing strings (label names) as keys and SimpleITK.Image
             (masks) as values. Must contain at least the LV, RV, MV, and whole heart.
-        label_left_ventricle (str): The name for the left ventricle mask (contour)
-        label_left_atrium (str): The name for the left atrium mask (contour)
-        label_right_ventricle (str): The name for the right ventricle mask (contour)
-        label_heart (str): The name for the heart mask (contour)
+        label_left_ventricle (str, optional): The name for the left ventricle mask (contour).
+            Defaults to Ventricle_L.
+        label_left_atrium (str, optional): The name for the left atrium mask (contour). Defaults to
+            Atrium_L.
+        label_right_ventricle (str, optional): The name for the right ventricle mask (contour).
+            Defaults to Ventricle_R.
+        label_heart (str, optional): The name for the heart mask (contour). Defaults to Heart.
         myocardium_thickness_mm (float, optional): Moycardial thickness, in millimetres.
             Defaults to 10.
         hole_fill_mm (float, optional): Holes smaller than this get filled in. Defaults to 3.
         optimiser_tol_degrees (float, optional): Optimiser tolerance (change in angle per iter).
             Defaults to 1, which typically requires 3-4 iterations.
         optimiser_max_iter (int, optional): Maximum optimiser iterations. Defaults to 10
         verbose (bool, optional): Print of information for debugging. Defaults to False.
@@ -121,20 +124,15 @@
 
     if verbose:
         print("Beginning LV segmentation algorithm.")
 
     # Initial set up
     label_mitral_valve = "MITRALVALVE"
 
-    label_list = [
-        label_left_ventricle,
-        label_left_atrium,
-        label_right_ventricle,
-        label_heart
-    ]
+    label_list = [label_left_ventricle, label_left_atrium, label_right_ventricle, label_heart]
     working_contours = copy.deepcopy({s: contours[s] for s in label_list})
 
     label_list.append(label_mitral_valve)
 
     output_contours = {}
     overall_transform_list = []
 
@@ -226,15 +224,14 @@
 
     if verbose:
         print("Module 2: LV orientation alignment.")
         print("  Optimiser tolerance (degrees) =", optimiser_tol_degrees)
         print("  Beginning alignment process")
 
     while n < optimiser_max_iter and np.abs(rotation_angle) > optimiser_tol_radians:
-
         n += 1
 
         # Find the LV apex
         lv_locations = np.where(sitk.GetArrayViewFromImage(working_contours[label_left_ventricle]))
         lv_apex_z = lv_locations[0].min()
         lv_apex_y = lv_locations[1][lv_locations[0] == lv_apex_z].mean()
         lv_apex_x = lv_locations[2][lv_locations[0] == lv_apex_z].mean()
@@ -414,15 +411,14 @@
     working_contours[17] = label_lv_myo_apex
 
     if verbose:
         print("  Computing apical segments")
     # We are now going to compute the segments in cylindical sections
     # First up - apical slices
     for n in range(inf_limit_lv, apical_extent):
-
         label_lv_myo_slice = label_lv_myo[:, :, n]
 
         # We will need numpy arrays here
         arr_lv_myo_slice = sitk.GetArrayViewFromImage(label_lv_myo_slice)
         loc_y, loc_x = np.where(arr_lv_myo_slice)
 
         # Now the origin
@@ -479,15 +475,14 @@
             min_area_mm2=min_area_mm2,
         )
 
     if verbose:
         print("  Computing mid segments")
     # Second up - mid slices
     for n in range(apical_extent, mid_extent):
-
         label_lv_myo_slice = label_lv_myo[:, :, n]
 
         # We will need numpy arrays here
         arr_lv_myo_slice = sitk.GetArrayViewFromImage(label_lv_myo_slice)
         loc_y, loc_x = np.where(arr_lv_myo_slice)
 
         # Now the origin
@@ -556,15 +551,14 @@
             min_area_mm2=min_area_mm2,
         )
 
     if verbose:
         print("  Computing basal segments")
     # Third up - basal slices
     for n in range(mid_extent, basal_extent):
-
         label_lv_myo_slice = label_lv_myo[:, :, n]
 
         # We will need numpy arrays here
         arr_lv_myo_slice = sitk.GetArrayViewFromImage(label_lv_myo_slice)
         loc_y, loc_x = np.where(arr_lv_myo_slice)
 
         if arr_lv_myo_slice.sum() == 0:
@@ -678,13 +672,13 @@
             contours[label_heart] * 0,
             new_structure,
             new_structure.GetSize(),
             (0, 0, 0),
             cb_index,
         )
 
-        output_contours[segment + 1] = new_structure
+        output_contours[f"Ventricle_L_Segment{segment + 1}"] = new_structure
 
     if verbose:
         print("Complete!")
 
     return output_contours
```

### Comparing `platipy-0.6.0/platipy/imaging/utils/vessel.py` & `platipy-0.6.1/platipy/imaging/utils/vessel.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/visualisation/animation.py` & `platipy-0.6.1/platipy/imaging/visualisation/animation.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/visualisation/comparison.py` & `platipy-0.6.1/platipy/imaging/visualisation/comparison.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/visualisation/dose.py` & `platipy-0.6.1/platipy/imaging/visualisation/dose.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/visualisation/tests/test_use_case.py` & `platipy-0.6.1/platipy/imaging/visualisation/tests/test_use_case.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/visualisation/utils.py` & `platipy-0.6.1/platipy/imaging/visualisation/utils.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/visualisation/view.py` & `platipy-0.6.1/platipy/imaging/visualisation/view.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/imaging/visualisation/visualiser.py` & `platipy-0.6.1/platipy/imaging/visualisation/visualiser.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/platipy/utils.py` & `platipy-0.6.1/platipy/utils.py`

 * *Files identical despite different names*

### Comparing `platipy-0.6.0/pyproject.toml` & `platipy-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "platipy"
-version = "0.6.0"
+version = "0.6.1"
 description = "Processing Library and Analysis Toolkit for Medical Imaging in Python"
 authors = ["Phillip Chlap & Robert Finnegan"]
 license = "Apache 2.0 License"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
@@ -32,15 +32,15 @@
 
 vtk = { version = "^9.1.0", optional = true }
 nnunet = { version = "^1.7.0", optional = true }
 Flask = { version = "^2.1.0", optional = true }
 Flask-RESTful = { version = ">=0.3.8", optional = true }
 Flask-SQLAlchemy = { version = "^2.4.4", optional = true }
 celery = { version = "^5.2.3", optional = true }
-redis = { version = "^3.5.3", optional = true }
+redis = { version = ">=3.5.3,<5.0.0", optional = true }
 psutil = { version = "^5.8.0", optional = true }
 gunicorn = { version = "^20.0.4", optional = true }
 Jinja2 = { version = "^3.1", optional = true }
 pymedphys = { version = ">=0.38.0", optional = true }
  
 
 [tool.poetry.extras]
```

### Comparing `platipy-0.6.0/setup.py` & `platipy-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['platipy',
  'platipy.backend',
  'platipy.backend.sample',
- 'platipy.backend.tests',
  'platipy.cli',
  'platipy.dicom',
  'platipy.dicom.communication',
  'platipy.dicom.download',
  'platipy.dicom.io',
  'platipy.dicom.tests',
  'platipy.imaging',
- 'platipy.imaging.cnn',
  'platipy.imaging.dose',
  'platipy.imaging.generation',
  'platipy.imaging.label',
  'platipy.imaging.projects',
  'platipy.imaging.projects.bronchus',
  'platipy.imaging.projects.cardiac',
  'platipy.imaging.projects.multiatlas',
@@ -49,30 +47,30 @@
  'scikit-image>=0.18.1']
 
 extras_require = \
 {'backend': ['Flask>=2.1.0,<3.0.0',
              'Flask-RESTful>=0.3.8',
              'Flask-SQLAlchemy>=2.4.4,<3.0.0',
              'celery>=5.2.3,<6.0.0',
-             'redis>=3.5.3,<4.0.0',
+             'redis>=3.5.3,<5.0.0',
              'psutil>=5.8.0,<6.0.0',
              'gunicorn>=20.0.4,<21.0.0',
              'Jinja2>=3.1,<4.0',
              'pymedphys>=0.38.0'],
  'cardiac': ['vtk>=9.1.0,<10.0.0', 'nnunet>=1.7.0,<2.0.0'],
  'nnunet': ['nnunet>=1.7.0,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['platipy = platipy.cli.run:platipy_cli']}
 
 setup_kwargs = {
     'name': 'platipy',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Processing Library and Analysis Toolkit for Medical Imaging in Python',
-    'long_description': '# PlatiPy\n\n## Processing Library and Analysis Toolkit for Medical Imaging in Python\n\n[![Tests](https://github.com/pyplati/platipy/actions/workflows/pull_request.yml/badge.svg?event=pull_request)](https://github.com/pyplati/platipy/actions/workflows/pull_request.yml)\n[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)\n\nPlatiPy is a library of **amazing** tools for image processing and analysis - designed specifically\nfor medical imaging!\n\nCheck out the [PlatiPy documentation](https://pyplati.github.io/platipy/) for more info.\n\nThis project was motivated by the need for a simple way to use, visualise, process, and analyse\nmedical images. Many of the tools and algorithms are designed in the context of radiation therapy,\nalthough they are more widely applicable to other fields that use 2D, 3D, or 4D imaging.\n\nPlatiPy is written in Python, and uses SimpleITK, VTK, and standard Python libraries. Jupyter\nnotebooks are provided where possible, mainly for guidance on getting started with using the tools.\nWe welcome feedback and contributions from the community (yes, you!) and you can find more\ninformation about contributing [here](https://pyplati.github.io/platipy/contributing.html).\n\n## What can I do with **platipy**?\n\nA lot! A good place to start is by looking in the\n[examples directory](https://github.com/pyplati/platipy/tree/master/examples).\n\nSome examples of what PlatiPy can do:\n\n- DICOM organising and converting:\n  - Bulk convert from multiple series and studies with a single function\n  - Convert DICOM-RT structure and dose filesto NIfTI images\n  - Create DICOM-RT structure files from binary masks e.g. from automatic contouring algorithms\n- Image registration\n  - Register images and transform labels with a few lines of code\n  - Linear transformations: rigid, affine, similarity\n  - Non-linear deformable transformations: demons, b-splines\n  - Multiple metrics for optimisation\n- Atlas-based segmentation\n  - A suite of tools that can be used out-of-the-box\n  - Includes advanced algorithms for\n      [iterative atlas selection](https://doi.org/10.1088/1361-6560/ab652a/) and\n      [vessel splining](https://doi.org/10.1088/1361-6560/abcb1d/)\n- Synthetic deformation field generation\n  - Simulate anatomically realistic shifts, expansions, and bending\n  - Compare DIR results from clinical systems\n- Basic tools for image processing and analysis\n  - Computing label similarity metrics: DSC, mean distance to agreement, Hausdorff distance, and more\n  - Cropping images to a region of interest\n  - Rotate images and generate maximum/mean intensity projections (beams eye view modelling)\n\nA major part of this package is **visualisation**, and some examples are shown below!\n\n#### Visualise some contours\n\n``` python\nfrom platipy.imaging import ImageVisualiser\n\nvis = ImageVisualiser(image)\nvis.add_contour(contours)\nfig = vis.show()\n```\n\n![Figure 1](assets/figure_1.png)\n\n#### Register some images\n\n```python\nfrom platipy.imaging.registration.linear import linear_registration\n\nimage_2_registered, tfm = linear_registration(\nimage_1,\nimage_2\n)\n\nvis = ImageVisualiser(image_1)\nvis.add_comparison_overlay(image_2_registered)\nfig = vis.show()\n```\n\n![Figure 2](assets/figure_2.png)\n\n#### Calculate deformation vector fields\n\n```python\nfrom platipy.imaging.registration.deformable import fast_symmetric_forces_demons_registration\n\nimage_2_deformed, tfm_dir, dvf = fast_symmetric_forces_demons_registration(\nimage_1,\nimage_2_registered\n)\n\nvis = ImageVisualiser(image_2_deformed, axis="z")\nvis.add_vector_overlay(\n    dvf,\n    subsample=12,\n    arrow_scale=1,\n    arrow_width=2,\n    colormap=plt.cm.magma,\n    name="DVF magnitude [mm]",\n    color_function="magnitude"\n)\nfig = vis.show()\n```\n\n![Figure 3](assets/figure_3.png)\n\n## Getting started\n\nThere aren\'t many requirements, just an installed Python interpreter (3.7 or greater). PlatiPy can\nbe installed with **pip**:\n\n```bash\npip install platipy\n```\n\nThe base installation of platipy does not include some large libraries needed for various\ncomponents of platipy. The following extras are available to install to run specific platipy tools:\n\n```bash\npip install platipy[cardiac]\npip install platipy[nnunet]\npip install platipy[backend]\n```\n\n## Authors\n\n- **Phillip Chlap** - [phillip.chlap@unsw.edu.au](phillip.chlap@unsw.edu.au)\n- **Robert Finnegan** - [robert.finnegan@sydney.edu.au](robert.finnegan@sydney.edu.au)\n',
+    'long_description': '# PlatiPy \n## Processing Library and Analysis Toolkit for Medical Imaging in Python\n\nPlatiPy is a library of **amazing** tools for image processing and analysis - designed specifically\nfor medical imaging! \n\nCheck out the [PlatiPy documentation](https://pyplati.github.io/platipy/) for more info.\n\nThis project was motivated by the need for a simple way to use, visualise, process, and analyse \nmedical images. Many of the tools and algorithms are designed in the context of radiation therapy,\nalthough they are more widely applicable to other fields that use 2D, 3D, or 4D imaging.\n\nPlatiPy is written in Python, and uses SimpleITK, VTK, and standard Python libraries. Jupyter\nnotebooks are provided where possible, mainly for guidance on getting started with using the tools.\nWe welcome feedback and contributions from the community (yes, you!) and you can find more\ninformation about contributing [here](https://pyplati.github.io/platipy/contributing.html).\n\n## What can I do with **platipy**?\nA lot! A good place to start is by looking in the \n[examples directory](https://github.com/pyplati/platipy/tree/master/examples).\n\nSome examples of what PlatiPy can do:\n - DICOM organising and converting:\n    * Bulk convert from multiple series and studies with a single function\n    * Convert DICOM-RT structure and dose files to NIfTI images\n    * Create DICOM-RT structure files from binary masks e.g. from automatic contouring algorithms\n - Image registration\n    * Register images and transform labels with a few lines of code\n    * Linear transformations: rigid, affine, similarity\n    * Non-linear deformable transformations: demons, b-splines\n    * Multiple metrics for optimisation\n - Atlas-based segmentation\n    * A suite of tools that can be used out-of-the-box\n    * Includes advanced algorithms for \n      [iterative atlas selection](https://doi.org/10.1088/1361-6560/ab652a/) and \n      [vessel splining](https://doi.org/10.1088/1361-6560/abcb1d/)\n - Synthetic deformation field generation\n    * Simulate anatomically realistic shifts, expansions, and bending\n    * Compare DIR results from clinical systems\n - Basic tools for image processing and analysis\n    * Computing label similarity metrics: DSC, mean distance to agreement, Hausdorff distance, and more\n    * Cropping images to a region of interest\n    * Rotate images and generate maximum/mean intensity projections (beams eye view modelling)\n\nA major part of this package is **visualisation**, and some examples are shown below!\n\n#### Visualise some contours\n\n``` python\nfrom platipy.imaging import ImageVisualiser\n\nvis = ImageVisualiser(image)\nvis.add_contour(contours)\nfig = vis.show()\n```\n\n![Figure 1](assets/figure_1.png)\n\n#### Register some images\n\n```python\nfrom platipy.imaging.registration.linear import linear_registration\n\nimage_2_registered, tfm = linear_registration(\nimage_1,\nimage_2\n)\n\nvis = ImageVisualiser(image_1)\nvis.add_comparison_overlay(image_2_registered)\nfig = vis.show()\n```\n\n![Figure 2](assets/figure_2.png)\n\n#### Calculate deformation vector fields\n    \n```python\nfrom platipy.imaging.registration.deformable import fast_symmetric_forces_demons_registration\n\nimage_2_deformed, tfm_dir, dvf = fast_symmetric_forces_demons_registration(\nimage_1,\nimage_2_registered\n)\n\nvis = ImageVisualiser(image_2_deformed, axis="z")\nvis.add_vector_overlay(\n    dvf,\n    subsample=12,\n    arrow_scale=1,\n    arrow_width=2,\n    colormap=plt.cm.magma,\n    name="DVF magnitude [mm]",\n    color_function="magnitude"\n)\nfig = vis.show()\n```\n\n![Figure 3](assets/figure_3.png)\n\n## Getting started\nThere aren\'t many requirements, just an installed Python interpreter (3.7 or greater). PlatiPy can\nbe installed with **pip**:\n\n```bash\npip install platipy\n```\n\nThe base installation of platipy does not include some large libraries needed for various\ncomponents of platipy. The following extras are available to install to run specific platipy tools:\n\n```bash\npip install platipy[cardiac]\npip install platipy[nnunet]\npip install platipy[backend]\n```\n\n## Authors\n\n* **Phillip Chlap** - [phillip.chlap@unsw.edu.au](phillip.chlap@unsw.edu.au)\n* **Robert Finnegan** - [robert.finnegan@sydney.edu.au](robert.finnegan@sydney.edu.au)\n',
     'author': 'Phillip Chlap & Robert Finnegan',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `platipy-0.6.0/PKG-INFO` & `platipy-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platipy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Processing Library and Analysis Toolkit for Medical Imaging in Python
 License: Apache 2.0 License
 Author: Phillip Chlap & Robert Finnegan
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
@@ -32,70 +32,64 @@
 Requires-Dist: matplotlib (>=3.2.2,<4.0.0)
 Requires-Dist: nnunet (>=1.7.0,<2.0.0) ; extra == "cardiac" or extra == "nnunet"
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0) ; extra == "backend"
 Requires-Dist: pydicom (>=2.1.2,<3.0.0)
 Requires-Dist: pymedphys (>=0.38.0) ; extra == "backend"
 Requires-Dist: pynetdicom (>=2.0.2,<3.0.0)
-Requires-Dist: redis (>=3.5.3,<4.0.0) ; extra == "backend"
+Requires-Dist: redis (>=3.5.3,<5.0.0) ; extra == "backend"
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: rt-utils (>=1.1.4,<2.0.0)
 Requires-Dist: scikit-image (>=0.18.1)
 Requires-Dist: vtk (>=9.1.0,<10.0.0) ; extra == "cardiac"
 Description-Content-Type: text/markdown
 
-# PlatiPy
-
+# PlatiPy 
 ## Processing Library and Analysis Toolkit for Medical Imaging in Python
 
-[![Tests](https://github.com/pyplati/platipy/actions/workflows/pull_request.yml/badge.svg?event=pull_request)](https://github.com/pyplati/platipy/actions/workflows/pull_request.yml)
-[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
-
 PlatiPy is a library of **amazing** tools for image processing and analysis - designed specifically
-for medical imaging!
+for medical imaging! 
 
 Check out the [PlatiPy documentation](https://pyplati.github.io/platipy/) for more info.
 
-This project was motivated by the need for a simple way to use, visualise, process, and analyse
+This project was motivated by the need for a simple way to use, visualise, process, and analyse 
 medical images. Many of the tools and algorithms are designed in the context of radiation therapy,
 although they are more widely applicable to other fields that use 2D, 3D, or 4D imaging.
 
 PlatiPy is written in Python, and uses SimpleITK, VTK, and standard Python libraries. Jupyter
 notebooks are provided where possible, mainly for guidance on getting started with using the tools.
 We welcome feedback and contributions from the community (yes, you!) and you can find more
 information about contributing [here](https://pyplati.github.io/platipy/contributing.html).
 
 ## What can I do with **platipy**?
-
-A lot! A good place to start is by looking in the
+A lot! A good place to start is by looking in the 
 [examples directory](https://github.com/pyplati/platipy/tree/master/examples).
 
 Some examples of what PlatiPy can do:
-
-- DICOM organising and converting:
-  - Bulk convert from multiple series and studies with a single function
-  - Convert DICOM-RT structure and dose filesto NIfTI images
-  - Create DICOM-RT structure files from binary masks e.g. from automatic contouring algorithms
-- Image registration
-  - Register images and transform labels with a few lines of code
-  - Linear transformations: rigid, affine, similarity
-  - Non-linear deformable transformations: demons, b-splines
-  - Multiple metrics for optimisation
-- Atlas-based segmentation
-  - A suite of tools that can be used out-of-the-box
-  - Includes advanced algorithms for
-      [iterative atlas selection](https://doi.org/10.1088/1361-6560/ab652a/) and
+ - DICOM organising and converting:
+    * Bulk convert from multiple series and studies with a single function
+    * Convert DICOM-RT structure and dose files to NIfTI images
+    * Create DICOM-RT structure files from binary masks e.g. from automatic contouring algorithms
+ - Image registration
+    * Register images and transform labels with a few lines of code
+    * Linear transformations: rigid, affine, similarity
+    * Non-linear deformable transformations: demons, b-splines
+    * Multiple metrics for optimisation
+ - Atlas-based segmentation
+    * A suite of tools that can be used out-of-the-box
+    * Includes advanced algorithms for 
+      [iterative atlas selection](https://doi.org/10.1088/1361-6560/ab652a/) and 
       [vessel splining](https://doi.org/10.1088/1361-6560/abcb1d/)
-- Synthetic deformation field generation
-  - Simulate anatomically realistic shifts, expansions, and bending
-  - Compare DIR results from clinical systems
-- Basic tools for image processing and analysis
-  - Computing label similarity metrics: DSC, mean distance to agreement, Hausdorff distance, and more
-  - Cropping images to a region of interest
-  - Rotate images and generate maximum/mean intensity projections (beams eye view modelling)
+ - Synthetic deformation field generation
+    * Simulate anatomically realistic shifts, expansions, and bending
+    * Compare DIR results from clinical systems
+ - Basic tools for image processing and analysis
+    * Computing label similarity metrics: DSC, mean distance to agreement, Hausdorff distance, and more
+    * Cropping images to a region of interest
+    * Rotate images and generate maximum/mean intensity projections (beams eye view modelling)
 
 A major part of this package is **visualisation**, and some examples are shown below!
 
 #### Visualise some contours
 
 ``` python
 from platipy.imaging import ImageVisualiser
@@ -121,15 +115,15 @@
 vis.add_comparison_overlay(image_2_registered)
 fig = vis.show()
 ```
 
 ![Figure 2](assets/figure_2.png)
 
 #### Calculate deformation vector fields
-
+    
 ```python
 from platipy.imaging.registration.deformable import fast_symmetric_forces_demons_registration
 
 image_2_deformed, tfm_dir, dvf = fast_symmetric_forces_demons_registration(
 image_1,
 image_2_registered
 )
@@ -146,15 +140,14 @@
 )
 fig = vis.show()
 ```
 
 ![Figure 3](assets/figure_3.png)
 
 ## Getting started
-
 There aren't many requirements, just an installed Python interpreter (3.7 or greater). PlatiPy can
 be installed with **pip**:
 
 ```bash
 pip install platipy
 ```
 
@@ -165,10 +158,10 @@
 pip install platipy[cardiac]
 pip install platipy[nnunet]
 pip install platipy[backend]
 ```
 
 ## Authors
 
-- **Phillip Chlap** - [phillip.chlap@unsw.edu.au](phillip.chlap@unsw.edu.au)
-- **Robert Finnegan** - [robert.finnegan@sydney.edu.au](robert.finnegan@sydney.edu.au)
+* **Phillip Chlap** - [phillip.chlap@unsw.edu.au](phillip.chlap@unsw.edu.au)
+* **Robert Finnegan** - [robert.finnegan@sydney.edu.au](robert.finnegan@sydney.edu.au)
```

