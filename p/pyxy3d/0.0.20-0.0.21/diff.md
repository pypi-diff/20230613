# Comparing `tmp/pyxy3d-0.0.20.tar.gz` & `tmp/pyxy3d-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.0.20.tar", max compression
+gzip compressed data, was "pyxy3d-0.0.21.tar", max compression
```

## Comparing `pyxy3d-0.0.20.tar` & `pyxy3d-0.0.21.tar`

### file list

```diff
@@ -1,233 +1,233 @@
--rw-r--r--   0        0        0    35184 2023-03-13 23:46:36.918754 pyxy3d-0.0.20/LICENSE.md
--rw-r--r--   0        0        0      925 2023-06-12 19:45:40.581459 pyxy3d-0.0.20/pyproject.toml
--rw-r--r--   0        0        0     2007 2023-05-20 12:18:55.240529 pyxy3d-0.0.20/pyxy3d/__init__.py
--rw-r--r--   0        0        0      934 2023-06-12 16:51:54.169618 pyxy3d-0.0.20/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.0.20/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.20/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.0.20/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.0.20/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0    11255 2023-06-10 20:05:09.592548 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.0.20/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.0.20/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.0.20/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.0.20/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    15573 2023-06-10 20:04:49.722607 pyxy3d-0.0.20/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.0.20/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.0.20/pyxy3d/export.py
--rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5684 2023-06-12 18:45:02.565389 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
--rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8098 2023-06-12 18:45:07.819053 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0    10204 2023-06-12 18:45:08.757113 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
--rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0    11941 2023-06-12 18:45:08.751113 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.0.20/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0     7438 2023-06-12 17:07:44.747202 pyxy3d-0.0.20/pyxy3d/gui/calibration_widget.py
--rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.0.20/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.0.20/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.0.20/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    10279 2023-06-12 16:49:05.520130 pyxy3d-0.0.20/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0     9807 2023-06-02 14:30:41.606273 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    14193 2023-06-02 00:29:03.392704 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.20/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.0.20/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    14273 2023-06-12 16:49:05.521130 pyxy3d-0.0.20/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.0.20/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.0.20/pyxy3d/gui/playback_widget.py
--rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.0.20/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.0.20/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    14618 2023-06-12 16:49:05.522130 pyxy3d-0.0.20/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.0.20/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.0.20/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.0.20/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.0.20/pyxy3d/helper.py
--rw-r--r--   0        0        0     6646 2023-06-01 14:21:56.755811 pyxy3d-0.0.20/pyxy3d/interface.py
--rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.0.20/pyxy3d/logger.py
--rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.0.20/pyxy3d/post_processor.py
--rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.0.20/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.0.20/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.0.20/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
--rw-r--r--   0        0        0    15991 2023-06-12 18:45:02.579375 pyxy3d-0.0.20/pyxy3d/session/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0    20797 2023-06-12 16:49:05.524130 pyxy3d-0.0.20/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.0.20/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
--rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.0.20/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.0.20/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.0.20/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.0.20/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.0.20/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.0.20/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.0.20/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
--rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
--rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
--rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
--rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
--rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
--rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
--rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
--rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
--rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
--rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
--rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
--rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
--rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
--rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
--rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
--rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
--rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
--rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
--rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
--rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
--rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
--rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
--rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
--rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.0.20/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.0.20/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.0.20/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     9401 2023-06-12 19:45:15.810322 pyxy3d-0.0.20/README.md
--rw-r--r--   0        0        0    10203 1970-01-01 00:00:00.000000 pyxy3d-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0    35184 2023-03-13 23:46:36.918754 pyxy3d-0.0.21/LICENSE.md
+-rw-r--r--   0        0        0      925 2023-06-12 22:16:34.127513 pyxy3d-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0     2007 2023-05-20 12:18:55.240529 pyxy3d-0.0.21/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-12 22:15:42.388447 pyxy3d-0.0.21/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.0.21/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.21/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.0.21/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.0.21/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0    11255 2023-06-10 20:05:09.592548 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.0.21/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.0.21/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.0.21/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.0.21/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    15573 2023-06-10 20:04:49.722607 pyxy3d-0.0.21/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.0.21/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.0.21/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5684 2023-06-12 18:45:02.565389 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8098 2023-06-12 18:45:07.819053 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    10204 2023-06-12 18:45:08.757113 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    11941 2023-06-12 18:45:08.751113 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.0.21/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0     7438 2023-06-12 22:15:42.390444 pyxy3d-0.0.21/pyxy3d/gui/calibration_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.0.21/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.0.21/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.0.21/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10279 2023-06-12 16:49:05.520130 pyxy3d-0.0.21/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9807 2023-06-02 14:30:41.606273 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    14193 2023-06-02 00:29:03.392704 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.21/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.0.21/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    14273 2023-06-12 16:49:05.521130 pyxy3d-0.0.21/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.0.21/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.0.21/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.0.21/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.0.21/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    14618 2023-06-12 16:49:05.522130 pyxy3d-0.0.21/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.0.21/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.0.21/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.0.21/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.0.21/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-01 14:21:56.755811 pyxy3d-0.0.21/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.0.21/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.0.21/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.0.21/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.0.21/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.0.21/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    15728 2023-06-12 22:04:21.160455 pyxy3d-0.0.21/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    20849 2023-06-12 22:15:55.087470 pyxy3d-0.0.21/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.0.21/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.0.21/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.0.21/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.0.21/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.0.21/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.0.21/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.0.21/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.0.21/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.0.21/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.0.21/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.0.21/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     9401 2023-06-12 22:15:42.383443 pyxy3d-0.0.21/README.md
+-rw-r--r--   0        0        0    10203 1970-01-01 00:00:00.000000 pyxy3d-0.0.21/PKG-INFO
```

### Comparing `pyxy3d-0.0.20/LICENSE.md` & `pyxy3d-0.0.21/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyproject.toml` & `pyxy3d-0.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.0.20"
+version = "0.0.21"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
```

### Comparing `pyxy3d-0.0.20/pyxy3d/__init__.py` & `pyxy3d-0.0.21/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/__main__.py` & `pyxy3d-0.0.21/pyxy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/charuco.py` & `pyxy3d-0.0.21/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.0.21/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.0.21/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.0.21/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/camera.py` & `pyxy3d-0.0.21/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.0.21/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.0.21/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.0.21/pyxy3d/cameras/live_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.0.21/pyxy3d/cameras/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/configurator.py` & `pyxy3d-0.0.21/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/export.py` & `pyxy3d-0.0.21/pyxy3d/export.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/calibration_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.0.21/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/log_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/main_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/main_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.0.21/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/playback_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/playback_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.0.21/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/recording_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.0.21/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/helper.py` & `pyxy3d-0.0.21/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/interface.py` & `pyxy3d-0.0.21/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/logger.py` & `pyxy3d-0.0.21/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/post_processor.py` & `pyxy3d-0.0.21/pyxy3d/post_processor.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.0.21/pyxy3d/recording/recorded_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.0.21/pyxy3d/recording/video_recorder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/session/__pycache__/session.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/session/__pycache__/session.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 16:49:05 2023 UTC, .py size: 20797 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 814c 8764 3d51 0000  o........L.d=Q..
+00000000: 6f0d 0d0a 0000 0000 6096 8764 c250 0000  o.......`..d.P..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6402 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6403 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6400 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -97,15 +97,15 @@
 00000600: 7c00 5f0b 6900 7c00 5f0c 6400 7c00 5f0d  |._.i.|._.d.|._.
 00000610: 7c00 6a03 a00e a100 7c00 5f0f 7c00 6a03  |.j.....|._.|.j.
 00000620: a010 a100 7c00 5f11 7c00 6a03 a012 a100  ....|._.|.j.....
 00000630: 7c00 5f13 7c00 6a03 a014 a100 7c00 5f15  |._.|.j.....|._.
 00000640: 7c00 6a03 a016 a100 7c00 5f17 6404 7c00  |.j.....|._.d.|.
 00000650: 5f18 7c00 6a03 a019 a100 7c00 5f1a 741b  _.|.j.....|._.t.
 00000660: 7c00 6a1a 8301 7c00 5f1c 741d 6a1e 7c00  |.j...|._.t.j.|.
-00000670: 5f1f 6400 5300 2905 4eda 0b63 616c 6962  _.d.S.).N..calib
+00000670: 5f1f 6400 5300 2905 4e5a 0b63 616c 6962  _.d.S.).NZ.calib
 00000680: 7261 7469 6f6e 5a09 6578 7472 696e 7369  rationZ.extrinsi
 00000690: 637a 0678 792e 6373 7646 2920 da05 7375  cz.xy.csvF) ..su
 000006a0: 7065 7272 2700 0000 da08 5f5f 696e 6974  perr'.....__init
 000006b0: 5f5f 7228 0000 00da 0c73 6573 7369 6f6e  __r(.....session
 000006c0: 5f70 6174 68da 0470 6174 6872 0500 0000  _path..pathr....
 000006d0: da18 6578 7472 696e 7369 635f 6361 6c69  ..extrinsic_cali
 000006e0: 6272 6174 696f 6e5f 7879 da07 6361 6d65  bration_xy..came
@@ -133,15 +133,15 @@
 00000840: 6e73 6963 da0c 6973 5f72 6563 6f72 6469  nsic..is_recordi
 00000850: 6e67 5a0b 6765 745f 6368 6172 7563 6fda  ngZ.get_charuco.
 00000860: 0763 6861 7275 636f 7209 0000 00da 0f63  .charucor......c
 00000870: 6861 7275 636f 5f74 7261 636b 6572 7219  haruco_trackerr.
 00000880: 0000 0072 1f00 0000 da04 6d6f 6465 2902  ...r......mode).
 00000890: da04 7365 6c66 7228 0000 00a9 01da 095f  ..selfr(......._
 000008a0: 5f63 6c61 7373 5f5f 7225 0000 0072 2600  _class__r%...r&.
-000008b0: 0000 722b 0000 0038 0000 0073 2a00 0000  ..r+...8...s*...
+000008b0: 0000 722a 0000 0038 0000 0073 2a00 0000  ..r*...8...s*...
 000008c0: 0e01 0601 0a02 0204 0a01 06ff 0605 0601  ................
 000008d0: 0601 0601 0602 0601 0c03 0c01 0c01 0c01  ................
 000008e0: 0c01 0602 0c02 0c01 0c01 7a10 5365 7373  ..........z.Sess
 000008f0: 696f 6e2e 5f5f 696e 6974 5f5f 6301 0000  ion.__init__c...
 00000900: 0000 0000 0000 0000 0005 0000 0003 0000  ................
 00000910: 0043 0000 0073 8a00 0000 7c00 6a00 a001  .C...s....|.j...
 00000920: a100 4400 5d09 5c02 7d01 7d02 7c02 6a02  ..D.].\.}.}.|.j.
@@ -155,35 +155,35 @@
 000009a0: 6401 5300 2902 7a72 0a20 2020 2020 2020  d.S.).zr.       
 000009b0: 2053 6875 7420 646f 776e 2074 6865 2073   Shut down the s
 000009c0: 7472 6561 6d73 2c20 636c 6f73 6520 7468  treams, close th
 000009d0: 6520 6361 6d65 7261 2063 6170 7475 7265  e camera capture
 000009e0: 7320 616e 6420 6465 6c65 7465 2074 6865  s and delete the
 000009f0: 206d 6f6e 6f63 616c 6962 7261 746f 7273   monocalibrators
 00000a00: 2061 6e64 2073 796e 6368 726f 6e69 7a65   and synchronize
-00000a10: 720a 2020 2020 2020 2020 4e29 0a72 3000  r.        N).r0.
+00000a10: 720a 2020 2020 2020 2020 4e29 0a72 2f00  r.        N).r/.
 00000a20: 0000 da05 6974 656d 735a 0a73 746f 705f  ....itemsZ.stop_
-00000a30: 6576 656e 74da 0373 6574 722f 0000 00da  event..setr/....
-00000a40: 0a64 6973 636f 6e6e 6563 7472 3300 0000  .disconnectr3...
+00000a30: 6576 656e 74da 0373 6574 722e 0000 00da  event..setr.....
+00000a40: 0a64 6973 636f 6e6e 6563 7472 3200 0000  .disconnectr2...
 00000a50: da0c 7379 6e63 6872 6f6e 697a 6572 da20  ..synchronizer. 
 00000a60: 7374 7265 616d 5f74 6f6f 6c73 5f64 6973  stream_tools_dis
 00000a70: 636f 6e6e 6563 7465 645f 7369 676e 616c  connected_signal
-00000a80: da04 656d 6974 2905 723c 0000 00da 0470  ..emit).r<.....p
+00000a80: da04 656d 6974 2905 723b 0000 00da 0470  ..emit).r;.....p
 00000a90: 6f72 74da 0673 7472 6561 6dda 0363 616d  ort..stream..cam
 00000aa0: da07 6d6f 6e6f 6361 6c72 2500 0000 7225  ..monocalr%...r%
 00000ab0: 0000 0072 2600 0000 da12 6469 7363 6f6e  ...r&.....discon
 00000ac0: 6e65 6374 5f63 616d 6572 6173 5a00 0000  nect_camerasZ...
 00000ad0: 7318 0000 0012 040c 0106 0112 010a 0106  s...............
 00000ae0: 0112 010c 0106 010c 0106 010e 027a 1a53  .............z.S
 00000af0: 6573 7369 6f6e 2e64 6973 636f 6e6e 6563  ession.disconnec
 00000b00: 745f 6361 6d65 7261 7363 0100 0000 0000  t_camerasc......
 00000b10: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
 00000b20: 0000 731e 0000 0074 007c 006a 0183 0164  ..s....t.|.j...d
 00000b30: 016b 0472 0b64 027d 017c 0153 0064 037d  .k.r.d.}.|.S.d.}
 00000b40: 017c 0153 0029 044e 7201 0000 0054 4629  .|.S.).Nr....TF)
-00000b50: 02da 036c 656e 722f 0000 0029 0272 3c00  ...lenr/...).r<.
+00000b50: 02da 036c 656e 722e 0000 0029 0272 3b00  ...lenr....).r;.
 00000b60: 0000 da08 656c 6967 6962 6c65 7225 0000  ....eligibler%..
 00000b70: 0072 2500 0000 7226 0000 00da 1869 735f  .r%...r&.....is_
 00000b80: 6361 6d65 7261 5f73 6574 7570 5f65 6c69  camera_setup_eli
 00000b90: 6769 626c 656c 0000 0073 0a00 0000 0e01  giblel...s......
 00000ba0: 0401 0403 04ff 0401 7a20 5365 7373 696f  ........z Sessio
 00000bb0: 6e2e 6973 5f63 616d 6572 615f 7365 7475  n.is_camera_setu
 00000bc0: 705f 656c 6967 6962 6c65 6301 0000 0000  p_eligiblec.....
@@ -193,18 +193,18 @@
 00000c00: 7d01 7c00 6a03 6a04 a005 a100 4400 5d10  }.|.j.j.....D.].
 00000c10: 5c02 7d02 7d03 7c03 6a06 6400 7500 7321  \.}.}.|.j.d.u.s!
 00000c20: 7c03 6a07 6400 7500 7223 6402 7d01 7113  |.j.d.u.r#d.}.q.
 00000c30: 7c01 5300 2903 4e54 4629 0872 2800 0000  |.S.).NTF).r(...
 00000c40: da11 7265 6672 6573 685f 6672 6f6d 5f74  ..refresh_from_t
 00000c50: 6f6d 6cda 1067 6574 5f63 616d 6572 615f  oml..get_camera_
 00000c60: 6172 7261 79da 0c63 616d 6572 615f 6172  array..camera_ar
-00000c70: 7261 7972 2f00 0000 723f 0000 005a 066d  rayr/...r?...Z.m
+00000c70: 7261 7972 2e00 0000 723e 0000 005a 066d  rayr....r>...Z.m
 00000c80: 6174 7269 785a 0b64 6973 746f 7274 696f  atrixZ.distortio
-00000c90: 6e73 a904 723c 0000 0072 4b00 0000 7245  ns..r<...rK...rE
-00000ca0: 0000 0072 4700 0000 7225 0000 0072 2500  ...rG...r%...r%.
+00000c90: 6e73 a904 723b 0000 0072 4a00 0000 7244  ns..r;...rJ...rD
+00000ca0: 0000 0072 4600 0000 7225 0000 0072 2500  ...rF...r%...r%.
 00000cb0: 0000 7226 0000 00da 2169 735f 6578 7472  ..r&....!is_extr
 00000cc0: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
 00000cd0: 6e5f 656c 6967 6962 6c65 7300 0000 7310  n_eligibles...s.
 00000ce0: 0000 000a 020c 0104 0114 0114 0104 0102  ................
 00000cf0: 8004 027a 2953 6573 7369 6f6e 2e69 735f  ...z)Session.is_
 00000d00: 6578 7472 696e 7369 635f 6361 6c69 6272  extrinsic_calibr
 00000d10: 6174 696f 6e5f 656c 6967 6962 6c65 6301  ation_eligiblec.
@@ -239,19 +239,19 @@
 00000ee0: 756d 6520 656c 6967 6962 696c 6974 7920  ume eligibility 
 00000ef0: 6475 6520 746f 2063 616d 6572 6120 7a02  due to camera z.
 00000f00: 3a20 7a45 456c 6967 6962 6c65 2074 6f20  : zEEligible to 
 00000f10: 6c6f 6164 2063 6170 7475 7265 2076 6f6c  load capture vol
 00000f20: 756d 653f 2028 692e 652e 2066 756c 6c79  ume? (i.e. fully
 00000f30: 2063 616c 6962 7261 7465 6420 6578 7472   calibrated extr
 00000f40: 696e 7369 6373 293a 2029 0c72 2800 0000  insics): ).r(...
-00000f50: 724d 0000 0072 4e00 0000 724f 0000 0072  rM...rN...rO...r
-00000f60: 4a00 0000 722f 0000 0072 3f00 0000 da08  J...r/...r?.....
+00000f50: 724c 0000 0072 4d00 0000 724e 0000 0072  rL...rM...rN...r
+00000f60: 4900 0000 722e 0000 0072 3e00 0000 da08  I...r....r>.....
 00000f70: 726f 7461 7469 6f6e da0b 7472 616e 736c  rotation..transl
 00000f80: 6174 696f 6eda 066c 6f67 6765 72da 0469  ation..logger..i
-00000f90: 6e66 6fda 085f 5f64 6963 745f 5f72 5000  nfo..__dict__rP.
+00000f90: 6e66 6fda 085f 5f64 6963 745f 5f72 4f00  nfo..__dict__rO.
 00000fa0: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
 00000fb0: 00da 1a69 735f 6361 7074 7572 655f 766f  ...is_capture_vo
 00000fc0: 6c75 6d65 5f65 6c69 6769 626c 657e 0000  lume_eligible~..
 00000fd0: 0073 2000 0000 0a08 0c01 0403 1001 0401  .s .............
 00000fe0: 1402 1401 0401 0401 1001 04ff 0280 0404  ................
 00000ff0: 0801 04ff 0404 7a22 5365 7373 696f 6e2e  ......z"Session.
 00001000: 6973 5f63 6170 7475 7265 5f76 6f6c 756d  is_capture_volum
@@ -266,735 +266,718 @@
 00001090: 6a09 6404 7500 723b 6403 7d01 740a a00b  j.d.u.r;d.}.t...
 000010a0: 6405 7c02 9b00 6406 9d03 a101 0100 711d  d.|...d.......q.
 000010b0: 7c01 7242 6401 7d01 7c01 5300 6403 7d01  |.rBd.}.|.S.d.}.
 000010c0: 7c01 5300 2907 7a44 0a20 2020 2020 2020  |.S.).zD.       
 000010d0: 2055 7365 6420 746f 2064 6574 6572 6d69   Used to determi
 000010e0: 6e65 2069 6620 7468 6520 5265 636f 7264  ne if the Record
 000010f0: 2042 7574 746f 6e20 6973 2065 6e61 626c   Button is enabl
-00001100: 6564 0a0a 2020 2020 2020 2020 5472 5200  ed..        TrR.
+00001100: 6564 0a0a 2020 2020 2020 2020 5472 5100  ed..        TrQ.
 00001110: 0000 464e 7a34 4361 6d65 7261 2061 7272  ..FNz4Camera arr
 00001120: 6179 2069 7320 6e6f 7420 6675 6c6c 7920  ay is not fully 
 00001130: 6361 6c69 6272 6174 6564 2062 6563 6175  calibrated becau
 00001140: 7365 2063 616d 6572 6120 7a11 206c 6163  se camera z. lac
 00001150: 6b73 2065 7874 7269 6e73 6963 7329 0c72  ks extrinsics).r
-00001160: 2800 0000 724d 0000 0072 4e00 0000 724f  (...rM...rN...rO
-00001170: 0000 0072 4a00 0000 722f 0000 0072 3f00  ...rJ...r/...r?.
-00001180: 0000 da06 6967 6e6f 7265 7253 0000 0072  ....ignorerS...r
-00001190: 5400 0000 7255 0000 0072 5600 0000 2904  T...rU...rV...).
-000011a0: 723c 0000 0072 4b00 0000 7245 0000 005a  r<...rK...rE...Z
+00001160: 2800 0000 724c 0000 0072 4d00 0000 724e  (...rL...rM...rN
+00001170: 0000 0072 4900 0000 722e 0000 0072 3e00  ...rI...r....r>.
+00001180: 0000 da06 6967 6e6f 7265 7252 0000 0072  ....ignorerR...r
+00001190: 5300 0000 7254 0000 0072 5500 0000 2904  S...rT...rU...).
+000011a0: 723b 0000 0072 4a00 0000 7244 0000 005a  r;...rJ...rD...Z
 000011b0: 0663 616d 6572 6172 2500 0000 7225 0000  .camerar%...r%..
 000011c0: 0072 2600 0000 da15 6973 5f72 6563 6f72  .r&.....is_recor
 000011d0: 6469 6e67 5f65 6c69 6769 626c 659b 0000  ding_eligible...
 000011e0: 0073 2a00 0000 0a07 0c01 0403 1001 0401  .s*.............
 000011f0: 1402 0a01 0801 02ff 0801 02ff 0403 0401  ................
 00001200: 0a01 04ff 0280 0403 0401 0404 04fe 0402  ................
 00001210: 7a1d 5365 7373 696f 6e2e 6973 5f72 6563  z.Session.is_rec
 00001220: 6f72 6469 6e67 5f65 6c69 6769 626c 6563  ording_eligiblec
-00001230: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-00001240: 0300 0000 0300 0000 7340 0000 0064 0164  ........s@...d.d
-00001250: 0267 0289 0087 0066 0164 0364 0484 087c  .g.....f.d.d...|
-00001260: 006a 00a0 01a1 0044 0083 017d 0174 027c  .j.....D...}.t.|
-00001270: 0183 017d 027c 0264 056b 0472 1c64 067d  ...}.|.d.k.r.d.}
-00001280: 037c 0353 0064 077d 037c 0353 0029 087a  .|.S.d.}.|.S.).z
-00001290: 690a 2020 2020 2020 2020 506f 7374 2070  i.        Post p
-000012a0: 726f 6365 7373 696e 6720 6361 6e20 6f6e  rocessing can on
-000012b0: 6c79 2062 6520 7065 7266 6f72 6d65 6420  ly be performed 
-000012c0: 6966 2072 6563 6f72 6469 6e67 7320 6578  if recordings ex
-000012d0: 6973 7420 616e 6420 6578 7472 696e 7369  ist and extrinsi
-000012e0: 6373 2061 7265 2063 616c 6962 7261 7465  cs are calibrate
-000012f0: 640a 2020 2020 2020 2020 7229 0000 007a  d.        r)...z
-00001300: 0b63 6f6e 6669 672e 746f 6d6c 6301 0000  .config.tomlc...
-00001310: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00001320: 0013 0000 0073 1a00 0000 6700 7c00 5d09  .....s....g.|.].
-00001330: 7d01 7c01 6a00 8800 7601 7202 7c01 9102  }.|.j...v.r.|...
-00001340: 7102 5300 7225 0000 0029 01da 046e 616d  q.S.r%...)...nam
-00001350: 6529 02da 022e 30da 0166 a901 5a0e 6578  e)....0..f..Z.ex
-00001360: 636c 7564 6564 5f69 7465 6d73 7225 0000  cluded_itemsr%..
-00001370: 0072 2600 0000 da0a 3c6c 6973 7463 6f6d  .r&.....<listcom
-00001380: 703e c000 0000 7302 0000 001a 007a 3753  p>....s......z7S
-00001390: 6573 7369 6f6e 2e69 735f 706f 7374 5f70  ession.is_post_p
-000013a0: 726f 6365 7373 696e 675f 656c 6967 6962  rocessing_eligib
-000013b0: 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  le.<locals>.<lis
-000013c0: 7463 6f6d 703e 7201 0000 0054 4629 0372  tcomp>r....TF).r
-000013d0: 2d00 0000 da07 6974 6572 6469 7272 4a00  -.....iterdirrJ.
-000013e0: 0000 2904 723c 0000 005a 0766 6f6c 6465  ..).r<...Z.folde
-000013f0: 7273 5a0f 7265 636f 7264 696e 675f 636f  rsZ.recording_co
-00001400: 756e 7472 4b00 0000 7225 0000 0072 5e00  untrK...r%...r^.
-00001410: 0000 7226 0000 00da 1b69 735f 706f 7374  ..r&.....is_post
-00001420: 5f70 726f 6365 7373 696e 675f 656c 6967  _processing_elig
-00001430: 6962 6c65 b900 0000 7310 0000 0008 0518  ible....s.......
-00001440: 0208 0108 0104 0104 0404 fe04 027a 2353  .............z#S
-00001450: 6573 7369 6f6e 2e69 735f 706f 7374 5f70  ession.is_post_p
-00001460: 726f 6365 7373 696e 675f 656c 6967 6962  rocessing_eligib
-00001470: 6c65 723b 0000 0063 0200 0000 0000 0000  ler;...c........
-00001480: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00001490: 7380 0100 007c 017c 005f 007c 00a0 01a1  s....|.|._.|....
-000014a0: 0001 007c 006a 0004 0074 026a 036b 0272  ...|.j...t.j.k.r
-000014b0: 1f01 007c 006a 0472 1d7c 006a 05a0 06a1  ...|.j.r.|.j....
-000014c0: 0001 007c 00a0 07a1 0001 0064 0353 0064  ...|.......d.S.d
-000014d0: 0353 0004 0074 026a 086b 0272 3501 007c  .S...t.j.k.r5..|
-000014e0: 006a 0472 337c 006a 05a0 06a1 0001 007c  .j.r3|.j.......|
-000014f0: 00a0 07a1 0001 0064 0353 0064 0353 0004  .......d.S.d.S..
-00001500: 0074 026a 096b 0272 6201 0074 0a7c 006a  .t.j.k.rb..t.|.j
-00001510: 0b83 017c 005f 0c7c 006a 0473 487c 00a0  ...|._.|.j.sH|..
-00001520: 0da1 0001 007c 006a 05a0 06a1 0001 007c  .....|.j.......|
-00001530: 00a0 07a1 0001 007c 00a0 0ea1 0001 007c  .......|.......|
-00001540: 00a0 0f64 01a1 0101 007c 00a0 107c 006a  ...d.....|...|.j
-00001550: 11a1 0101 0064 0353 0004 0074 026a 126b  .....d.S...t.j.k
-00001560: 0272 8901 0074 0a7c 006a 0b83 017c 005f  .r...t.|.j...|._
-00001570: 0c7c 006a 0473 757c 00a0 0da1 0001 007c  .|.j.su|.......|
-00001580: 00a0 07a1 0001 007c 00a0 0ea1 0001 007c  .......|.......|
-00001590: 00a0 0f64 01a1 0101 007c 006a 05a0 13a1  ...d.....|.j....
-000015a0: 0001 0064 0353 0004 0074 026a 146b 0272  ...d.S...t.j.k.r
-000015b0: 9f01 007c 006a 0472 9d7c 00a0 07a1 0001  ...|.j.r.|......
-000015c0: 007c 006a 05a0 06a1 0001 0064 0353 0064  .|.j.......d.S.d
-000015d0: 0353 0074 026a 156b 0272 be7c 006a 0473  .S.t.j.k.r.|.j.s
-000015e0: aa7c 00a0 0da1 0001 007c 00a0 07a1 0001  .|.......|......
-000015f0: 007c 00a0 0f64 02a1 0101 007c 00a0 01a1  .|...d.....|....
-00001600: 0001 007c 006a 05a0 13a1 0001 0064 0353  ...|.j.......d.S
-00001610: 0064 0353 0029 047a af0a 2020 2020 2020  .d.S.).z..      
-00001620: 2020 5669 6120 7468 6973 206d 6574 686f    Via this metho
-00001630: 642c 2074 6865 2066 7261 6d65 2072 6561  d, the frame rea
-00001640: 6469 6e67 2062 6568 6176 696f 7220 7769  ding behavior wi
-00001650: 6c6c 2062 6520 6368 616e 6765 6420 6279  ll be changed by
-00001660: 2074 6865 2047 5549 2e20 4966 2073 6f6d   the GUI. If som
-00001670: 6520 7072 6f70 6572 7469 6573 2061 7265  e properties are
-00001680: 0a20 2020 2020 2020 206e 6f74 2061 7661  .        not ava
-00001690: 696c 6162 6c65 2028 692e 652e 2073 796e  ilable (i.e. syn
-000016a0: 6368 726f 6e69 7a65 7229 2074 6865 7920  chronizer) they 
-000016b0: 7769 6c6c 2062 6520 6372 6561 7465 640a  will be created.
-000016c0: 2020 2020 2020 2020 5446 4e29 1672 3b00          TFN).r;.
-000016d0: 0000 da12 7570 6461 7465 5f73 7472 6561  ....update_strea
-000016e0: 6d73 5f66 7073 7219 0000 0072 1f00 0000  ms_fpsr....r....
-000016f0: 7232 0000 0072 4200 0000 da18 756e 7375  r2...rB.....unsu
-00001700: 6273 6372 6962 655f 6672 6f6d 5f73 7472  bscribe_from_str
-00001710: 6561 6d73 da19 7061 7573 655f 616c 6c5f  eams..pause_all_
-00001720: 6d6f 6e6f 6361 6c69 6272 6174 6f72 7372  monocalibratorsr
-00001730: 2400 0000 7220 0000 0072 0900 0000 7239  $...r ...r....r9
-00001740: 0000 0072 3a00 0000 da11 6c6f 6164 5f73  ...r:.....load_s
-00001750: 7472 6561 6d5f 746f 6f6c 73da 1373 6574  tream_tools..set
-00001760: 5f73 7472 6561 6d73 5f63 6861 7275 636f  _streams_charuco
-00001770: da14 7365 745f 7374 7265 616d 735f 7472  ..set_streams_tr
-00001780: 6163 6b69 6e67 da17 6163 7469 7661 7465  acking..activate
-00001790: 5f6d 6f6e 6f63 616c 6962 7261 746f 7272  _monocalibratorr
-000017a0: 3400 0000 7221 0000 00da 1473 7562 7363  4...r!.....subsc
-000017b0: 7269 6265 5f74 6f5f 7374 7265 616d 7372  ribe_to_streamsr
-000017c0: 2200 0000 7223 0000 0029 0272 3c00 0000  "...r#...).r<...
-000017d0: 723b 0000 0072 2500 0000 7225 0000 0072  r;...r%...r%...r
-000017e0: 2600 0000 da08 7365 745f 6d6f 6465 c900  &.....set_mode..
-000017f0: 0000 7356 0000 0006 0508 0104 020c 0106  ..sV............
-00001800: 010a 010c 0104 fe0c 0406 010a 010c 0104  ................
-00001810: fe0c 040c 0206 0208 010a 0108 0108 010a  ................
-00001820: 0110 010c 020c 0206 0108 0108 0208 010a  ................
-00001830: 010e 010c 0206 0108 010e 0104 fe08 0406  ................
-00001840: 0108 0108 020a 0108 010e 0104 f97a 1053  .............z.S
-00001850: 6573 7369 6f6e 2e73 6574 5f6d 6f64 65da  ession.set_mode.
-00001860: 0a66 7073 5f74 6172 6765 7463 0200 0000  .fps_targetc....
-00001870: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001880: 4300 0000 7386 0000 007c 006a 0004 0074  C...s....|.j...t
-00001890: 016a 026b 0272 0901 006e 3404 0074 016a  .j.k.r...n4..t.j
-000018a0: 036b 0272 1001 006e 2d04 0074 016a 046b  .k.r...n-..t.j.k
-000018b0: 0272 2001 007c 017c 005f 057c 006a 06a0  .r ..|.|._.|.j..
-000018c0: 077c 01a1 0101 006e 1d04 0074 016a 086b  .|.....n...t.j.k
-000018d0: 0272 3001 007c 017c 005f 097c 006a 06a0  .r0..|.|._.|.j..
-000018e0: 0a7c 01a1 0101 006e 0d74 016a 0b6b 0272  .|.....n.t.j.k.r
-000018f0: 3d7c 017c 005f 0c7c 006a 06a0 0d7c 01a1  =|.|._.|.j...|..
-00001900: 0101 007c 00a0 0ea1 0001 0064 0153 0029  ...|.......d.S.)
-00001910: 027a 780a 2020 2020 2020 2020 5570 6461  .zx.        Upda
-00001920: 7465 7320 7468 6520 4650 5320 7573 6564  tes the FPS used
-00001930: 2062 7920 7468 6520 6375 7272 656e 746c   by the currentl
-00001940: 7920 6163 7469 7665 2073 6573 7369 6f6e  y active session
-00001950: 206d 6f64 650a 2020 2020 2020 2020 5468   mode.        Th
-00001960: 6973 2075 7064 6174 6520 696e 636c 7564  is update includ
-00001970: 6573 2074 6865 2063 6f6e 6669 672e 746f  es the config.to
-00001980: 6d6c 0a20 2020 2020 2020 204e 290f 723b  ml.        N).r;
-00001990: 0000 0072 1900 0000 721f 0000 0072 2400  ...r....r....r$.
-000019a0: 0000 7220 0000 0072 3700 0000 7228 0000  ..r ...r7...r(..
-000019b0: 005a 1e73 6176 655f 6670 735f 696e 7472  .Z.save_fps_intr
-000019c0: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
-000019d0: 6e72 2100 0000 7236 0000 005a 1e73 6176  nr!...r6...Z.sav
-000019e0: 655f 6670 735f 6578 7472 696e 7369 635f  e_fps_extrinsic_
-000019f0: 6361 6c69 6272 6174 696f 6e72 2300 0000  calibrationr#...
-00001a00: 7235 0000 005a 1273 6176 655f 6670 735f  r5...Z.save_fps_
-00001a10: 7265 636f 7264 696e 6772 6200 0000 2902  recordingrb...).
-00001a20: 723c 0000 0072 6b00 0000 7225 0000 0072  r<...rk...r%...r
-00001a30: 2500 0000 7226 0000 00da 1373 6574 5f61  %...r&.....set_a
-00001a40: 6374 6976 655f 6d6f 6465 5f66 7073 0101  ctive_mode_fps..
-00001a50: 0000 731e 0000 0004 050c 0102 010c 0102  ..s.............
-00001a60: 010c 0106 010e 010c 0106 010e 0108 0106  ................
-00001a70: 010c 010c 027a 1b53 6573 7369 6f6e 2e73  .....z.Session.s
-00001a80: 6574 5f61 6374 6976 655f 6d6f 6465 5f66  et_active_mode_f
-00001a90: 7073 da06 7265 7475 726e 6301 0000 0000  ps..returnc.....
-00001aa0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00001ab0: 0000 0073 6e00 0000 6400 7d01 7c00 6a00  ...sn...d.}.|.j.
-00001ac0: 0400 7401 6a02 6b02 720d 0100 0900 7c01  ..t.j.k.r.....|.
-00001ad0: 5300 0400 7401 6a03 6b02 7216 0100 0900  S...t.j.k.r.....
-00001ae0: 7c01 5300 0400 7401 6a04 6b02 7221 0100  |.S...t.j.k.r!..
-00001af0: 7c00 6a05 7d01 7c01 5300 0400 7401 6a06  |.j.}.|.S...t.j.
-00001b00: 6b02 722c 0100 7c00 6a07 7d01 7c01 5300  k.r,..|.j.}.|.S.
-00001b10: 7401 6a08 6b02 7235 7c00 6a09 7d01 7c01  t.j.k.r5|.j.}.|.
-00001b20: 5300 7c01 5300 a901 4e29 0a72 3b00 0000  S.|.S...N).r;...
-00001b30: 7219 0000 0072 1f00 0000 7224 0000 0072  r....r....r$...r
-00001b40: 2000 0000 7237 0000 0072 2100 0000 7236   ...r7...r!...r6
-00001b50: 0000 0072 2300 0000 7235 0000 0029 0272  ...r#...r5...).r
-00001b60: 3c00 0000 5a03 6670 7372 2500 0000 7225  <...Z.fpsr%...r%
-00001b70: 0000 0072 2600 0000 da13 6765 745f 6163  ...r&.....get_ac
-00001b80: 7469 7665 5f6d 6f64 655f 6670 7317 0100  tive_mode_fps...
-00001b90: 0073 2200 0000 0401 0401 0c01 0201 0409  .s".............
-00001ba0: 0cf8 0201 0407 0cfa 0601 0405 0cfc 0601  ................
-00001bb0: 0403 08fe 0601 0801 7a1b 5365 7373 696f  ........z.Sessio
-00001bc0: 6e2e 6765 745f 6163 7469 7665 5f6d 6f64  n.get_active_mod
-00001bd0: 655f 6670 7363 0100 0000 0000 0000 0000  e_fpsc..........
-00001be0: 0000 0400 0000 0400 0000 4300 0000 7336  ..........C...s6
-00001bf0: 0000 007c 00a0 00a1 007d 017c 0164 0075  ...|.....}.|.d.u
-00001c00: 0172 177c 006a 01a0 02a1 0044 005d 0b5c  .r.|.j.....D.].\
-00001c10: 027d 027d 037c 03a0 037c 01a1 0101 0071  .}.}.|...|.....q
-00001c20: 0d64 0053 0064 0053 0072 6e00 0000 2904  .d.S.d.S.rn...).
-00001c30: 726f 0000 0072 3000 0000 723f 0000 005a  ro...r0...r?...Z
-00001c40: 0e73 6574 5f66 7073 5f74 6172 6765 7429  .set_fps_target)
-00001c50: 0472 3c00 0000 5a0f 6163 7469 7665 5f6d  .r<...Z.active_m
-00001c60: 6f64 655f 6670 7372 4500 0000 7246 0000  ode_fpsrE...rF..
-00001c70: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00001c80: 7262 0000 0026 0100 0073 0c00 0000 0801  rb...&...s......
-00001c90: 0801 1201 0c01 04fe 0401 7a1a 5365 7373  ..........z.Sess
-00001ca0: 696f 6e2e 7570 6461 7465 5f73 7472 6561  ion.update_strea
-00001cb0: 6d73 5f66 7073 da0b 7472 6163 6b69 6e67  ms_fps..tracking
-00001cc0: 5f6f 6e63 0200 0000 0000 0000 0000 0000  _onc............
-00001cd0: 0400 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
-00001ce0: 007c 006a 00a0 01a1 0044 005d 095c 027d  .|.j.....D.].\.}
-00001cf0: 027d 037c 03a0 027c 01a1 0101 0071 0564  .}.|...|.....q.d
-00001d00: 0053 0072 6e00 0000 2903 7230 0000 0072  .S.rn...).r0...r
-00001d10: 3f00 0000 5a0f 7365 745f 7472 6163 6b69  ?...Z.set_tracki
-00001d20: 6e67 5f6f 6e29 0472 3c00 0000 7270 0000  ng_on).r<...rp..
-00001d30: 0072 4500 0000 7246 0000 0072 2500 0000  .rE...rF...r%...
-00001d40: 7225 0000 0072 2600 0000 7267 0000 002c  r%...r&...rg...,
-00001d50: 0100 0073 0600 0000 1201 0c01 04ff 7a1c  ...s..........z.
-00001d60: 5365 7373 696f 6e2e 7365 745f 7374 7265  Session.set_stre
-00001d70: 616d 735f 7472 6163 6b69 6e67 6301 0000  ams_trackingc...
-00001d80: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00001d90: 0043 0000 0073 3a00 0000 7400 a001 6401  .C...s:...t...d.
-00001da0: a101 0100 7402 7c00 6a03 8301 7c00 5f04  ....t.|.j...|._.
-00001db0: 7c00 6a05 a006 a100 4400 5d0a 5c02 7d01  |.j.....D.].\.}.
-00001dc0: 7d02 7c02 a007 7c00 6a04 a101 0100 7110  }.|...|.j.....q.
-00001dd0: 6400 5300 2902 4e7a 2275 7064 6174 696e  d.S.).Nz"updatin
-00001de0: 6720 6368 6172 7563 6f20 696e 2063 6173  g charuco in cas
-00001df0: 6520 6e65 6365 7373 6172 7929 0872 5500  e necessary).rU.
-00001e00: 0000 7256 0000 0072 0900 0000 7239 0000  ..rV...r....r9..
-00001e10: 0072 3a00 0000 7230 0000 0072 3f00 0000  .r:...r0...r?...
-00001e20: 5a0e 7570 6461 7465 5f74 7261 636b 6572  Z.update_tracker
-00001e30: 2903 723c 0000 0072 4500 0000 7246 0000  ).r<...rE...rF..
-00001e40: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00001e50: 7266 0000 0030 0100 0073 0a00 0000 0a01  rf...0...s......
-00001e60: 0c01 1201 0e01 04ff 7a1b 5365 7373 696f  ........z.Sessio
-00001e70: 6e2e 7365 745f 7374 7265 616d 735f 6368  n.set_streams_ch
-00001e80: 6172 7563 6f63 0100 0000 0000 0000 0000  arucoc..........
-00001e90: 0000 0100 0000 0300 0000 4300 0000 7318  ..........C...s.
-00001ea0: 0000 0074 00a0 0164 01a1 0101 007c 006a  ...t...d.....|.j
-00001eb0: 02a0 03a1 0001 0064 0053 0029 024e 7a14  .......d.S.).Nz.
-00001ec0: 7061 7573 696e 6720 7379 6e63 6872 6f6e  pausing synchron
-00001ed0: 697a 6572 2904 7255 0000 0072 5600 0000  izer).rU...rV...
-00001ee0: 7242 0000 0072 6300 0000 a901 723c 0000  rB...rc.....r<..
-00001ef0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00001f00: da12 7061 7573 655f 7379 6e63 6872 6f6e  ..pause_synchron
-00001f10: 697a 6572 3601 0000 7304 0000 000a 010e  izer6...s.......
-00001f20: 017a 1a53 6573 7369 6f6e 2e70 6175 7365  .z.Session.pause
-00001f30: 5f73 796e 6368 726f 6e69 7a65 7263 0100  _synchronizerc..
-00001f40: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00001f50: 0000 4300 0000 731e 0000 007c 006a 00a0  ..C...s....|.j..
-00001f60: 01a1 0001 007c 006a 00a0 027c 006a 006a  .....|.j...|.j.j
-00001f70: 03a1 0101 0064 0053 0072 6e00 0000 2904  .....d.S.rn...).
-00001f80: 7242 0000 0072 6900 0000 5a0e 7365 745f  rB...ri...Z.set_
-00001f90: 7374 7265 616d 5f66 7073 726b 0000 0072  stream_fpsrk...r
-00001fa0: 7100 0000 7225 0000 0072 2500 0000 7226  q...r%...r%...r&
-00001fb0: 0000 00da 1475 6e70 6175 7365 5f73 796e  .....unpause_syn
-00001fc0: 6368 726f 6e69 7a65 723a 0100 0073 0400  chronizer:...s..
-00001fd0: 0000 0a01 1401 7a1c 5365 7373 696f 6e2e  ......z.Session.
-00001fe0: 756e 7061 7573 655f 7379 6e63 6872 6f6e  unpause_synchron
-00001ff0: 697a 6572 6301 0000 0000 0000 0000 0000  izerc...........
-00002000: 0004 0000 0004 0000 0043 0000 0073 3400  .........C...s4.
-00002010: 0000 6401 7d01 7c00 6a00 6a01 a002 a100  ..d.}.|.j.j.....
-00002020: a003 a100 4400 5d0d 5c02 7d02 7d03 7c02  ....D.].\.}.}.|.
-00002030: a004 6402 a101 7217 7c01 6403 3700 7d01  ..d...r.|.d.7.}.
-00002040: 710a 7c01 5300 2904 4e72 0100 0000 7247  q.|.S.).Nr....rG
-00002050: 0000 00e9 0100 0000 2905 7228 0000 00da  ........).r(....
-00002060: 0464 6963 74da 0463 6f70 7972 3f00 0000  .dict..copyr?...
-00002070: da0a 7374 6172 7473 7769 7468 2904 723c  ..startswith).r<
-00002080: 0000 00da 0563 6f75 6e74 da03 6b65 79da  .....count..key.
-00002090: 0670 6172 616d 7372 2500 0000 7225 0000  .paramsr%...r%..
-000020a0: 0072 2600 0000 da1b 6765 745f 636f 6e66  .r&.....get_conf
-000020b0: 6967 7572 6564 5f63 616d 6572 615f 636f  igured_camera_co
-000020c0: 756e 743e 0100 0073 0c00 0000 0401 1801  unt>...s........
-000020d0: 0a01 0801 0280 0401 7a23 5365 7373 696f  ........z#Sessio
-000020e0: 6e2e 6765 745f 636f 6e66 6967 7572 6564  n.get_configured
-000020f0: 5f63 616d 6572 615f 636f 756e 7463 0100  _camera_countc..
-00002100: 0000 0000 0000 0000 0000 0500 0000 0800  ................
-00002110: 0000 0300 0000 738c 0000 0087 0066 0164  ......s......f.d
-00002120: 0164 0284 087d 0174 0083 008f 1e7d 0274  .d...}.t.....}.t
-00002130: 0164 0374 0283 0244 005d 107d 037c 0388  .d.t...D.].}.|..
-00002140: 006a 03a0 04a1 0076 0072 1971 0f7c 02a0  .j.....v.r.q.|..
-00002150: 057c 017c 03a1 0201 0071 0f57 0064 0404  .|.|.....q.W.d..
-00002160: 0004 0083 0301 006e 0831 0073 2a77 0101  .......n.1.s*w..
-00002170: 0001 0001 0059 0001 0088 006a 066a 07a0  .....Y.....j.j..
-00002180: 08a1 00a0 04a1 0044 005d 0c7d 047c 04a0  .......D.].}.|..
-00002190: 0964 05a1 0172 4388 006a 066a 077c 043d  .d...rC..j.j.|.=
-000021a0: 0071 3764 0453 0029 067a a30a 2020 2020  .q7d.S.).z..    
-000021b0: 2020 2020 4361 6c6c 6564 2062 7920 6c6f      Called by lo
-000021c0: 6164 5f73 7472 6561 6d73 2069 6e20 7468  ad_streams in th
-000021d0: 6520 6576 656e 7420 7468 6174 206e 6f20  e event that no 
-000021e0: 6361 6d65 7261 7320 6172 6520 7265 7475  cameras are retu
-000021f0: 726e 6564 2062 7920 7468 6520 636f 6e66  rned by the conf
-00002200: 6967 7572 6174 6f72 2e2e 2e0a 2020 2020  igurator....    
-00002210: 2020 2020 5769 6c6c 2070 6f70 756c 6174      Will populat
-00002220: 6520 7365 6c66 2e63 616d 6572 6173 2075  e self.cameras u
-00002230: 7369 6e67 206d 756c 7469 706c 6520 7468  sing multiple th
-00002240: 7265 6164 730a 2020 2020 2020 2020 6301  reads.        c.
-00002250: 0000 0000 0000 0000 0000 0002 0000 0007  ................
-00002260: 0000 0013 0000 0073 8c00 0000 7a37 7400  .......s....z7t.
-00002270: a001 6401 7c00 9b00 9d02 a101 0100 7402  ..d.|.........t.
-00002280: 7c00 8301 7d01 7400 a001 6402 7c00 9b00  |...}.t...d.|...
-00002290: 9d02 a101 0100 7c01 8800 6a03 7c00 3c00  ......|...j.|.<.
-000022a0: 8800 6a04 a005 7c01 a101 0100 7400 a001  ..j...|.....t...
-000022b0: 6403 7c00 9b00 6404 9d03 a101 0100 7406  d.|...d.......t.
-000022c0: 7c01 7407 8800 6a08 8301 6405 8d02 8800  |.t...j...d.....
-000022d0: 6a09 7c00 3c00 5700 6400 5300 0100 0100  j.|.<.W.d.S.....
-000022e0: 0100 7400 a001 6406 7c00 9b00 9d02 a101  ..t...d.|.......
-000022f0: 0100 5900 6400 5300 2907 4e7a 0c54 7279  ..Y.d.S.).Nz.Try
-00002300: 696e 6720 706f 7274 207a 1053 7563 6365  ing port z.Succe
-00002310: 7373 2061 7420 706f 7274 207a 174c 6f61  ss at port z.Loa
-00002320: 6469 6e67 2073 7472 6561 6d20 6174 2070  ding stream at p
-00002330: 6f72 7420 7a25 2077 6974 6820 6368 6172  ort z% with char
-00002340: 7563 6f20 7472 6163 6b65 7220 666f 7220  uco tracker for 
-00002350: 6361 6c69 6272 6174 696f 6ea9 015a 0774  calibration..Z.t
-00002360: 7261 636b 6572 7a12 4e6f 2063 616d 6572  rackerz.No camer
-00002370: 6120 6174 2070 6f72 7420 290a 7255 0000  a at port ).rU..
-00002380: 0072 5600 0000 720b 0000 0072 2f00 0000  .rV...r....r/...
-00002390: 7228 0000 005a 0b73 6176 655f 6361 6d65  r(...Z.save_came
-000023a0: 7261 7216 0000 0072 0900 0000 7239 0000  rar....r....r9..
-000023b0: 0072 3000 0000 2902 7245 0000 0072 4700  .r0...).rE...rG.
-000023c0: 0000 7271 0000 0072 2500 0000 7226 0000  ..rq...r%...r&..
-000023d0: 00da 0761 6464 5f63 616d 4b01 0000 731c  ...add_camK...s.
-000023e0: 0000 0002 0110 0108 0110 010a 010c 0104  ................
-000023f0: 010a 0104 ff02 030a 0112 ff06 0316 017a  ...............z
-00002400: 2653 6573 7369 6f6e 2e5f 6669 6e64 5f63  &Session._find_c
-00002410: 616d 6572 6173 2e3c 6c6f 6361 6c73 3e2e  ameras.<locals>.
-00002420: 6164 645f 6361 6d72 0100 0000 4e5a 0673  add_camr....NZ.s
-00002430: 7465 7265 6f29 0a72 0400 0000 da05 7261  tereo).r......ra
-00002440: 6e67 65da 154d 4158 5f43 414d 4552 415f  nge..MAX_CAMERA_
-00002450: 504f 5254 5f43 4845 434b 722f 0000 00da  PORT_CHECKr/....
-00002460: 046b 6579 73da 0673 7562 6d69 7472 2800  .keys..submitr(.
-00002470: 0000 7275 0000 0072 7600 0000 7277 0000  ..ru...rv...rw..
-00002480: 0029 0572 3c00 0000 727d 0000 00da 0865  .).r<...r}.....e
-00002490: 7865 6375 746f 72da 0169 7279 0000 0072  xecutor..iry...r
-000024a0: 2500 0000 7271 0000 0072 2600 0000 da0d  %...rq...r&.....
-000024b0: 5f66 696e 645f 6361 6d65 7261 7345 0100  _find_camerasE..
-000024c0: 0073 1a00 0000 0c06 0810 0e01 0e01 0202  .s..............
-000024d0: 0e02 02fb 1cff 1409 0a01 0a01 0280 04fe  ................
-000024e0: 7a15 5365 7373 696f 6e2e 5f66 696e 645f  z.Session._find_
-000024f0: 6361 6d65 7261 7363 0100 0000 0000 0000  camerasc........
-00002500: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-00002510: 73d0 0000 0064 017c 005f 007c 006a 01a0  s....d.|._.|.j..
-00002520: 02a1 007c 005f 0374 047c 006a 0383 0164  ...|._.t.|.j...d
-00002530: 026b 0272 147c 00a0 05a1 0001 007c 006a  .k.r.|.......|.j
-00002540: 03a0 06a1 0044 005d 1e5c 027d 017d 027c  .....D.].\.}.}.|
-00002550: 017c 006a 07a0 08a1 0076 0072 2571 1974  .|.j.....v.r%q.t
-00002560: 09a0 0a64 037c 019b 009d 02a1 0101 0074  ...d.|.........t
-00002570: 0b7c 027c 006a 0c64 048d 027c 006a 077c  .|.|.j.d...|.j.|
-00002580: 013c 0071 197c 00a0 0da1 0001 007c 00a0  .<.q.|.......|..
-00002590: 0ea1 0001 0074 0f7c 006a 10a0 08a1 0083  .....t.|.j......
-000025a0: 017c 005f 1174 127c 006a 0783 017c 005f  .|._.t.|.j...|._
-000025b0: 1364 017c 005f 1464 057c 005f 0074 09a0  .d.|._.d.|._.t..
-000025c0: 0a64 06a1 0101 007c 006a 15a0 16a1 0001  .d.....|.j......
-000025d0: 007c 00a0 17a1 0001 007c 00a0 18a1 0001  .|.......|......
-000025e0: 0064 0753 0029 087a ad0a 2020 2020 2020  .d.S.).z..      
-000025f0: 2020 436f 6e6e 6563 7473 2074 6f20 7374    Connects to st
-00002600: 6f72 6564 2063 616d 6572 6173 2061 6e64  ored cameras and
-00002610: 2063 7265 6174 6573 2073 7472 6561 6d73   creates streams
-00002620: 2077 6974 6820 7072 6f76 6964 6564 2074   with provided t
-00002630: 7261 636b 696e 670a 2020 2020 2020 2020  racking.        
-00002640: 4265 6361 7573 6520 7468 6573 6520 7374  Because these st
-00002650: 7265 616d 7320 6172 6520 6176 6169 6c61  reams are availa
-00002660: 626c 652c 2074 6865 2073 796e 6368 726f  ble, the synchro
-00002670: 6e69 7a65 7220 6361 6e20 7468 656e 2062  nizer can then b
-00002680: 6520 696e 6974 6961 6c69 7a65 640a 2020  e initialized.  
-00002690: 2020 2020 2020 5472 0100 0000 7a18 4c6f        Tr....z.Lo
-000026a0: 6164 696e 6720 5374 7265 616d 2066 6f72  ading Stream for
-000026b0: 2070 6f72 7420 727c 0000 0046 7a2d 5369   port r|...Fz-Si
-000026c0: 676e 616c 6c69 6e67 2073 7563 6365 7373  gnalling success
-000026d0: 6675 6c20 6c6f 6164 696e 6720 6f66 2073  ful loading of s
-000026e0: 7472 6561 6d20 746f 6f6c 734e 2919 7231  tream toolsN).r1
-000026f0: 0000 0072 2800 0000 5a0b 6765 745f 6361  ...r(...Z.get_ca
-00002700: 6d65 7261 7372 2f00 0000 724a 0000 0072  merasr/...rJ...r
-00002710: 8400 0000 723f 0000 0072 3000 0000 7280  ....r?...r0...r.
-00002720: 0000 0072 5500 0000 7256 0000 0072 1600  ...rU...rV...r..
-00002730: 0000 723a 0000 00da 135f 6164 6a75 7374  ..r:....._adjust
-00002740: 5f72 6573 6f6c 7574 696f 6e73 da15 5f6c  _resolutions.._l
-00002750: 6f61 645f 6d6f 6e6f 6361 6c69 6272 6174  oad_monocalibrat
-00002760: 6f72 73da 036d 696e 7233 0000 0072 3400  ors..minr3...r4.
-00002770: 0000 720c 0000 0072 4200 0000 7232 0000  ..r....rB...r2..
-00002780: 00da 1a73 7472 6561 6d5f 746f 6f6c 735f  ...stream_tools_
-00002790: 6c6f 6164 6564 5f73 6967 6e61 6c72 4400  loaded_signalrD.
-000027a0: 0000 7264 0000 0072 7200 0000 a903 723c  ..rd...rr.....r<
-000027b0: 0000 0072 4500 0000 7247 0000 0072 2500  ...rE...rG...r%.
-000027c0: 0000 7225 0000 0072 2600 0000 7265 0000  ..r%...r&...re..
-000027d0: 0068 0100 0073 2a00 0000 0605 0c02 0e02  .h...s*.........
-000027e0: 0801 1202 0e01 0201 1002 1601 0802 0801  ................
-000027f0: 1003 0202 0401 06ff 0605 0601 0a01 0a01  ................
-00002800: 0802 0c01 7a19 5365 7373 696f 6e2e 6c6f  ....z.Session.lo
-00002810: 6164 5f73 7472 6561 6d5f 746f 6f6c 7363  ad_stream_toolsc
-00002820: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00002830: 0600 0000 4300 0000 735e 0000 007c 006a  ....C...s^...|.j
-00002840: 00a0 01a1 0044 005d 275c 027d 017d 027c  .....D.]'\.}.}.|
-00002850: 017c 006a 02a0 03a1 0076 0072 1a74 04a0  .|.j.....v.r.t..
-00002860: 0564 017c 019b 0064 029d 03a1 0101 0071  .d.|...d.......q
-00002870: 0574 04a0 0564 037c 019b 009d 02a1 0101  .t...d.|........
-00002880: 0074 067c 006a 077c 0119 0083 017c 006a  .t.|.j.|.....|.j
-00002890: 027c 013c 0071 0564 0053 0029 044e 7a2f  .|.<.q.d.S.).Nz/
-000028a0: 536b 6970 7069 6e67 206f 7665 7220 6d6f  Skipping over mo
-000028b0: 6e6f 6361 6c69 6272 6174 6f72 2063 7265  nocalibrator cre
-000028c0: 6174 696f 6e20 666f 7220 706f 7274 207a  ation for port z
-000028d0: 1b20 6265 6361 7573 6520 6974 2061 6c72  . because it alr
-000028e0: 6561 6479 2065 7869 7374 732e 7a20 4c6f  eady exists.z Lo
-000028f0: 6164 696e 6720 4d6f 6e6f 6361 6c69 6272  ading Monocalibr
-00002900: 6174 6f72 2066 6f72 2070 6f72 7420 2908  ator for port ).
-00002910: 722f 0000 0072 3f00 0000 7233 0000 0072  r/...r?...r3...r
-00002920: 8000 0000 7255 0000 0072 5600 0000 720a  ....rU...rV...r.
-00002930: 0000 0072 3000 0000 7289 0000 0072 2500  ...r0...r....r%.
-00002940: 0000 7225 0000 0072 2600 0000 7286 0000  ..r%...r&...r...
-00002950: 008e 0100 0073 1200 0000 1201 0e01 0401  .....s..........
-00002960: 0a01 04ff 0203 1002 1601 04f8 7a1d 5365  ............z.Se
-00002970: 7373 696f 6e2e 5f6c 6f61 645f 6d6f 6e6f  ssion._load_mono
-00002980: 6361 6c69 6272 6174 6f72 734e da0b 6163  calibratorsN..ac
-00002990: 7469 7665 5f70 6f72 7463 0200 0000 0000  tive_portc......
-000029a0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-000029b0: 0000 7346 0000 007c 0164 0175 0172 0f74  ..sF...|.d.u.r.t
-000029c0: 00a0 0164 027c 019b 009d 02a1 0101 007c  ...d.|.........|
-000029d0: 017c 005f 0274 00a0 0164 037c 006a 029b  .|._.t...d.|.j..
-000029e0: 0064 049d 03a1 0101 007c 006a 037c 006a  .d.......|.j.|.j
-000029f0: 0219 00a0 04a1 0001 0064 0153 0029 057a  .........d.S.).z
-00002a00: 7e0a 2020 2020 2020 2020 5573 6564 2074  ~.        Used t
-00002a10: 6f20 6d61 6b65 2073 7572 6520 7468 6174  o make sure that
-00002a20: 206f 6e6c 7920 7468 6520 6163 7469 7665   only the active
-00002a30: 2063 616d 6572 6120 7461 6220 6973 2072   camera tab is r
-00002a40: 6561 6469 6e67 2066 7261 6d65 7320 6475  eading frames du
-00002a50: 7269 6e67 2074 6865 2069 6e74 7269 6e73  ring the intrins
-00002a60: 6963 2063 616c 6962 7261 7469 6f6e 2070  ic calibration p
-00002a70: 726f 6365 7373 0a20 2020 2020 2020 204e  rocess.        N
-00002a80: 7a29 5365 7474 696e 6720 7365 7373 696f  z)Setting sessio
-00002a90: 6e20 6163 7469 7665 206d 6f6e 6f63 616c  n active monocal
-00002aa0: 6962 7261 746f 7220 746f 207a 1a41 6374  ibrator to z.Act
-00002ab0: 6976 6174 6520 7472 6163 6b69 6e67 206f  ivate tracking o
-00002ac0: 6e20 706f 7274 207a 1620 616e 6420 6465  n port z. and de
-00002ad0: 6163 7469 7661 7465 206f 7468 6572 7329  activate others)
-00002ae0: 0572 5500 0000 7256 0000 0072 3400 0000  .rU...rV...r4...
-00002af0: 7233 0000 005a 1373 7562 7363 7269 6265  r3...Z.subscribe
-00002b00: 5f74 6f5f 7374 7265 616d 2902 723c 0000  _to_stream).r<..
-00002b10: 0072 8a00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00002b20: 7226 0000 0072 6800 0000 9901 0000 730e  r&...rh.......s.
-00002b30: 0000 0008 0510 0106 0104 010c 0104 ff14  ................
-00002b40: 037a 1f53 6573 7369 6f6e 2e61 6374 6976  .z.Session.activ
-00002b50: 6174 655f 6d6f 6e6f 6361 6c69 6272 6174  ate_monocalibrat
-00002b60: 6f72 6301 0000 0000 0000 0000 0000 0003  orc.............
-00002b70: 0000 0003 0000 0043 0000 0073 2a00 0000  .......C...s*...
-00002b80: 7400 a001 6401 a101 0100 7c00 6a02 a003  t...d.....|.j...
-00002b90: a100 4400 5d08 5c02 7d01 7d02 7c02 a004  ..D.].\.}.}.|...
-00002ba0: a100 0100 710a 6402 5300 2903 7a8b 0a20  ....q.d.S.).z.. 
-00002bb0: 2020 2020 2020 2075 7365 6420 7768 656e         used when
-00002bc0: 206e 6f74 2061 6374 6976 656c 7920 6f6e   not actively on
-00002bd0: 2074 6865 2063 616d 6572 6120 6361 6c69   the camera cali
-00002be0: 6272 6174 696f 6e20 7461 620a 2020 2020  bration tab.    
-00002bf0: 2020 2020 6f72 2077 6865 6e20 7369 6c65      or when sile
-00002c00: 6e63 696e 6720 616c 6c20 696e 2070 7265  ncing all in pre
-00002c10: 7061 7261 7469 6f6e 2066 6f72 2061 6374  paration for act
-00002c20: 6976 6174 696e 6720 6f6e 6c79 206f 6e65  ivating only one
-00002c30: 0a20 2020 2020 2020 207a 2550 6175 7369  .        z%Pausi
-00002c40: 6e67 2061 6c6c 206d 6f6e 6f63 616c 6962  ng all monocalib
-00002c50: 7261 746f 7220 6c6f 6f70 696e 672e 2e2e  rator looping...
-00002c60: 4e29 0572 5500 0000 7256 0000 0072 3300  N).rU...rV...r3.
-00002c70: 0000 723f 0000 005a 1575 6e73 7562 7363  ..r?...Z.unsubsc
-00002c80: 7269 6265 5f74 6f5f 7374 7265 616d 2903  ribe_to_stream).
-00002c90: 723c 0000 0072 4500 0000 7248 0000 0072  r<...rE...rH...r
-00002ca0: 2500 0000 7225 0000 0072 2600 0000 7264  %...r%...r&...rd
-00002cb0: 0000 00a6 0100 0073 0800 0000 0a05 1201  .......s........
-00002cc0: 0a01 04ff 7a21 5365 7373 696f 6e2e 7061  ....z!Session.pa
-00002cd0: 7573 655f 616c 6c5f 6d6f 6e6f 6361 6c69  use_all_monocali
-00002ce0: 6272 6174 6f72 7346 da15 6465 7374 696e  bratorsF..destin
-00002cf0: 6174 696f 6e5f 6469 7265 6374 6f72 79da  ation_directory.
-00002d00: 1373 746f 7265 5f70 6f69 6e74 5f68 6973  .store_point_his
-00002d10: 746f 7279 6303 0000 0000 0000 0000 0000  toryc...........
-00002d20: 0003 0000 0004 0000 0043 0000 0073 3e00  .........C...s>.
-00002d30: 0000 7400 a001 6401 a101 0100 7c01 6a02  ..t...d.....|.j.
-00002d40: 6402 6402 6403 8d02 0100 7403 7c00 6a04  d.d.d.....t.|.j.
-00002d50: 8301 7c00 5f05 7c00 6a05 6a06 7c01 7c02  ..|._.|.j.j.|.|.
-00002d60: 6404 8d02 0100 6402 7c00 5f07 6400 5300  d.....d.|._.d.S.
-00002d70: 2905 4e7a 1749 6e69 7469 6174 696e 6720  ).Nz.Initiating 
-00002d80: 7265 636f 7264 696e 672e 2e2e 5429 02da  recording...T)..
-00002d90: 0770 6172 656e 7473 da08 6578 6973 745f  .parents..exist_
-00002da0: 6f6b 2901 728c 0000 0029 0872 5500 0000  ok).r....).rU...
-00002db0: 7256 0000 00da 056d 6b64 6972 7217 0000  rV.....mkdirr...
-00002dc0: 0072 4200 0000 da0e 7669 6465 6f5f 7265  .rB.....video_re
-00002dd0: 636f 7264 6572 da0f 7374 6172 745f 7265  corder..start_re
-00002de0: 636f 7264 696e 6772 3800 0000 2903 723c  cordingr8...).r<
-00002df0: 0000 0072 8b00 0000 728c 0000 0072 2500  ...r....r....r%.
-00002e00: 0000 7225 0000 0072 2600 0000 7291 0000  ..r%...r&...r...
-00002e10: 00af 0100 0073 0e00 0000 0a03 0e01 0c02  .....s..........
-00002e20: 0601 0401 06ff 0a03 7a17 5365 7373 696f  ........z.Sessio
-00002e30: 6e2e 7374 6172 745f 7265 636f 7264 696e  n.start_recordin
-00002e40: 6763 0100 0000 0000 0000 0000 0000 0100  gc..............
-00002e50: 0000 0300 0000 4300 0000 736a 0000 0074  ......C...sj...t
-00002e60: 00a0 0164 01a1 0101 007c 006a 02a0 03a1  ...d.....|.j....
-00002e70: 0001 007c 006a 026a 0472 1b74 00a0 0164  ...|.j.j.r.t...d
-00002e80: 02a1 0101 0074 0564 0383 0101 007c 006a  .....t.d.....|.j
-00002e90: 026a 0473 0e64 047c 005f 0674 00a0 0164  .j.s.d.|._.t...d
-00002ea0: 05a1 0101 007c 006a 07a0 08a1 0001 007c  .....|.j.......|
-00002eb0: 00a0 09a1 0072 337c 006a 0aa0 08a1 0001  .....r3|.j......
-00002ec0: 0064 0053 0064 0053 0029 064e 7a15 5374  .d.S.d.S.).Nz.St
-00002ed0: 6f70 7069 6e67 2072 6563 6f72 6469 6e67  opping recording
-00002ee0: 2e2e 2e7a 2e57 6169 7469 6e67 2066 6f72  ...z.Waiting for
-00002ef0: 2076 6964 656f 2072 6563 6f72 6465 7220   video recorder 
-00002f00: 746f 2073 6176 6520 6f75 7420 6461 7461  to save out data
-00002f10: 2e2e 2e67 0000 0000 0000 e03f 467a 3d52  ...g.......?Fz=R
-00002f20: 6563 6f72 6469 6e67 206f 6620 6672 616d  ecording of fram
-00002f30: 6573 2069 7320 636f 6d70 6c65 7465 2e2e  es is complete..
-00002f40: 2e73 6967 6e61 6c6c 696e 6720 6368 616e  .signalling chan
-00002f50: 6765 2069 6e20 7374 6174 7573 290b 7255  ge in status).rU
-00002f60: 0000 0072 5600 0000 7290 0000 00da 0e73  ...rV...r......s
-00002f70: 746f 705f 7265 636f 7264 696e 675a 0972  top_recordingZ.r
-00002f80: 6563 6f72 6469 6e67 7206 0000 0072 3800  ecordingr....r8.
-00002f90: 0000 da19 7265 636f 7264 696e 675f 636f  ....recording_co
-00002fa0: 6d70 6c65 7465 5f73 6967 6e61 6c72 4400  mplete_signalrD.
-00002fb0: 0000 7261 0000 00da 1575 6e6c 6f63 6b5f  ..ra.....unlock_
-00002fc0: 706f 7374 7072 6f63 6573 7369 6e67 7271  postprocessingrq
-00002fd0: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00002fe0: 0000 7292 0000 00bb 0100 0073 1800 0000  ..r........s....
-00002ff0: 0a01 0a01 0801 0a01 0801 08fe 0604 0a02  ................
-00003000: 0a01 0802 0e01 04ff 7a16 5365 7373 696f  ........z.Sessio
-00003010: 6e2e 7374 6f70 5f72 6563 6f72 6469 6e67  n.stop_recording
-00003020: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-00003030: 0008 0000 0003 0000 0073 5400 0000 8700  .........sT.....
-00003040: 6601 6401 6402 8408 7d01 7400 8300 8f17  f.d.d...}.t.....
-00003050: 7d02 8800 6a01 a002 a100 4400 5d08 7d03  }...j.....D.].}.
-00003060: 7c02 a003 7c01 7c03 a102 0100 710f 5700  |...|.|.....q.W.
-00003070: 6403 0400 0400 8303 0100 6403 5300 3100  d.........d.S.1.
-00003080: 7323 7701 0100 0100 0100 5900 0100 6403  s#w.......Y...d.
-00003090: 5300 2904 7a82 4368 616e 6765 7320 7468  S.).z.Changes th
-000030a0: 6520 6361 6d65 7261 2072 6573 6f6c 7574  e camera resolut
-000030b0: 696f 6e20 746f 2074 6865 2076 616c 7565  ion to the value
-000030c0: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
-000030d0: 6174 696f 6e2c 2061 730a 2020 2020 2020  ation, as.      
-000030e0: 2020 6c6f 6720 6173 2069 7420 6973 206e    log as it is n
-000030f0: 6f74 2063 6f6e 6669 6775 7265 6420 666f  ot configured fo
-00003100: 7220 7468 6520 6465 6661 756c 7420 7265  r the default re
-00003110: 736f 6c75 7469 6f6e 6301 0000 0000 0000  solutionc.......
-00003120: 0000 0000 0004 0000 000a 0000 0013 0000  ................
-00003130: 0073 b600 0000 8800 6a00 7c00 1900 7d01  .s......j.|...}.
-00003140: 8800 6a01 6a02 6401 7c00 9b00 9d02 1900  ..j.j.d.|.......
-00003150: 6402 1900 7d02 8800 6a03 7c00 1900 6a04  d...}...j.|...j.
-00003160: 7d03 7c02 6403 1900 7c03 6403 1900 6b03  }.|.d...|.d...k.
-00003170: 7326 7c02 6404 1900 7c03 6404 1900 6b03  s&|.d...|.d...k.
-00003180: 7259 7405 a006 6405 7c00 9b00 6406 7c03  rYt...d.|...d.|.
-00003190: 6403 6407 8502 1900 9b00 6408 7c02 6403  d.d.......d.|.d.
-000031a0: 6407 8502 1900 9b00 9d06 a101 0100 7c01  d.............|.
-000031b0: a007 7c02 a101 0100 7405 a006 6409 7c00  ..|.....t...d.|.
-000031c0: 9b00 6406 7c03 6403 6407 8502 1900 9b00  ..d.|.d.d.......
-000031d0: 6408 7c02 6403 6407 8502 1900 9b00 9d06  d.|.d.d.........
-000031e0: a101 0100 6400 5300 6400 5300 290a 4e5a  ....d.S.d.S.).NZ
-000031f0: 0463 616d 5fda 0473 697a 6572 0100 0000  .cam_..sizer....
-00003200: 7274 0000 007a 2742 6567 696e 6e69 6e67  rt...z'Beginning
-00003210: 2074 6f20 6368 616e 6765 2072 6573 6f6c   to change resol
-00003220: 7574 696f 6e20 6174 2070 6f72 7420 7a06  ution at port z.
-00003230: 2066 726f 6d20 7252 0000 007a 0420 746f   from rR...z. to
-00003240: 207a 2743 6f6d 706c 6574 6564 2063 6861   z'Completed cha
-00003250: 6e67 6520 6f66 2072 6573 6f6c 7574 696f  nge of resolutio
-00003260: 6e20 6174 2070 6f72 7420 2908 7230 0000  n at port ).r0..
-00003270: 0072 2800 0000 7275 0000 0072 2f00 0000  .r(...ru...r/...
-00003280: 5a12 6465 6661 756c 745f 7265 736f 6c75  Z.default_resolu
-00003290: 7469 6f6e 7255 0000 0072 5600 0000 5a11  tionrU...rV...Z.
-000032a0: 6368 616e 6765 5f72 6573 6f6c 7574 696f  change_resolutio
-000032b0: 6e29 0472 4500 0000 7246 0000 0072 9500  n).rE...rF...r..
-000032c0: 0000 5a0c 6465 6661 756c 745f 7369 7a65  ..Z.default_size
-000032d0: 7271 0000 0072 2500 0000 7226 0000 00da  rq...r%...r&....
-000032e0: 1161 646a 7573 745f 7265 735f 776f 726b  .adjust_res_work
-000032f0: 6572 ce01 0000 7318 0000 000a 0116 010c  er....s.........
-00003300: 0120 0204 0124 0104 ff0a 0304 0124 0108  . ...$.......$..
-00003310: ff04 fb7a 3653 6573 7369 6f6e 2e5f 6164  ...z6Session._ad
-00003320: 6a75 7374 5f72 6573 6f6c 7574 696f 6e73  just_resolutions
-00003330: 2e3c 6c6f 6361 6c73 3e2e 6164 6a75 7374  .<locals>.adjust
-00003340: 5f72 6573 5f77 6f72 6b65 724e 2904 7204  _res_workerN).r.
-00003350: 0000 0072 2f00 0000 7280 0000 0072 8100  ...r/...r....r..
-00003360: 0000 2904 723c 0000 0072 9600 0000 7282  ..).r<...r....r.
-00003370: 0000 0072 4500 0000 7225 0000 0072 7100  ...rE...r%...rq.
-00003380: 0000 7226 0000 0072 8500 0000 ca01 0000  ..r&...r........
-00003390: 730c 0000 000c 0408 0e0e 010e 0102 ff22  s.............."
-000033a0: ff7a 1b53 6573 7369 6f6e 2e5f 6164 6a75  .z.Session._adju
-000033b0: 7374 5f72 6573 6f6c 7574 696f 6e73 6301  st_resolutionsc.
-000033c0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000033d0: 0000 0043 0000 0073 7a00 0000 7c00 6a00  ...C...sz...|.j.
-000033e0: a001 a100 7c00 5f02 7c00 6a00 a003 a100  ....|._.|.j.....
-000033f0: 7c00 5f04 7405 7c00 6a04 7c00 6a02 8302  |._.t.|.j.|.j...
-00003400: 7c00 5f06 7c00 6a00 6a07 6401 1900 6402  |._.|.j.j.d...d.
-00003410: 1900 7c00 6a06 5f08 6403 7c00 6a00 6a07  ..|.j._.d.|.j.j.
-00003420: 6401 1900 a009 a100 7600 7232 7c00 6a00  d.......v.r2|.j.
-00003430: 6a07 6401 1900 6403 1900 7c00 6a06 5f0a  j.d...d...|.j._.
-00003440: 740b 7c00 6a06 7c00 6a0c 6404 8d02 7c00  t.|.j.|.j.d...|.
-00003450: 5f0d 6405 5300 2906 7af3 0a20 2020 2020  _.d.S.).z..     
-00003460: 2020 2046 6f6c 6c6f 7769 6e67 2063 6170     Following cap
-00003470: 7475 7265 2076 6f6c 756d 6520 6f70 7469  ture volume opti
-00003480: 6d69 7a61 7469 6f6e 2076 6961 2062 756e  mization via bun
-00003490: 646c 6520 6164 6a75 7374 6d65 6e74 2c20  dle adjustment, 
-000034a0: 6f72 2061 6c74 6572 6174 696f 6e0a 2020  or alteration.  
-000034b0: 2020 2020 2020 7669 6120 6120 7472 616e        via a tran
-000034c0: 7366 6f72 6d20 6f66 2074 6865 206f 7269  sform of the ori
-000034d0: 6769 6e2c 2074 6865 2065 6e74 6972 6520  gin, the entire 
-000034e0: 6361 7074 7572 6520 766f 6c75 6d65 2063  capture volume c
-000034f0: 616e 2062 6520 7265 6c6f 6164 6564 0a20  an be reloaded. 
-00003500: 2020 2020 2020 2066 726f 6d20 7468 6520         from the 
-00003510: 636f 6e66 6967 2064 6174 6120 7769 7468  config data with
-00003520: 6f75 7420 6e65 6564 696e 6720 746f 2067  out needing to g
-00003530: 6f20 7468 726f 7567 6820 7468 6520 7374  o through the st
-00003540: 6570 730a 0a20 2020 2020 2020 20da 0e63  eps..        ..c
-00003550: 6170 7475 7265 5f76 6f6c 756d 65da 0573  apture_volume..s
-00003560: 7461 6765 da11 6f72 6967 696e 5f73 796e  tage..origin_syn
-00003570: 635f 696e 6465 7829 0172 3900 0000 4e29  c_index).r9...N)
-00003580: 0e72 2800 0000 7214 0000 00da 0f70 6f69  .r(...r......poi
-00003590: 6e74 5f65 7374 696d 6174 6573 724e 0000  nt_estimatesrN..
-000035a0: 0072 4f00 0000 7211 0000 0072 9700 0000  .rO...r....r....
-000035b0: 7275 0000 0072 9800 0000 7280 0000 0072  ru...r....r....r
-000035c0: 9900 0000 7212 0000 0072 3900 0000 da12  ....r....r9.....
-000035d0: 7175 616c 6974 795f 636f 6e74 726f 6c6c  quality_controll
-000035e0: 6572 7271 0000 0072 2500 0000 7225 0000  errq...r%...r%..
-000035f0: 0072 2600 0000 da1d 6c6f 6164 5f65 7374  .r&.....load_est
-00003600: 696d 6174 6564 5f63 6170 7475 7265 5f76  imated_capture_v
-00003610: 6f6c 756d 65e0 0100 0073 1600 0000 0c07  olume....s......
-00003620: 0c01 1001 1402 1401 0a01 0201 08ff 0205  ................
-00003630: 0801 0cff 7a25 5365 7373 696f 6e2e 6c6f  ....z%Session.lo
-00003640: 6164 5f65 7374 696d 6174 6564 5f63 6170  ad_estimated_cap
-00003650: 7475 7265 5f76 6f6c 756d 6563 0100 0000  ture_volumec....
-00003660: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00003670: 4300 0000 73a6 0000 0074 007c 006a 016a  C...s....t.|.j.j
-00003680: 027c 006a 0383 027d 017c 016a 0464 0164  .|.j...}.|.j.d.d
-00003690: 028d 0101 0074 057c 006a 016a 0283 01a0  .....t.|.j.j....
-000036a0: 06a1 007c 005f 0774 087c 006a 077c 006a  ...|._.t.|.j.|.j
-000036b0: 0383 027c 005f 0974 0a7c 006a 077c 006a  ...|._.t.|.j.|.j
-000036c0: 0983 027c 005f 0b7c 006a 0ba0 0ca1 0001  ...|._.|.j......
-000036d0: 0074 0d7c 006a 0b7c 006a 0e83 027c 005f  .t.|.j.|.j...|._
-000036e0: 0f74 10a0 1164 0374 1264 0414 009b 0064  .t...d.t.d.....d
-000036f0: 059d 03a1 0101 007c 006a 0fa0 1374 12a1  .......|.j...t..
-00003700: 0101 007c 006a 0ba0 0ca1 0001 007c 006a  ...|.j.......|.j
-00003710: 01a0 147c 006a 0ba1 0101 0064 0653 0029  ...|.j.....d.S.)
-00003720: 077a d70a 2020 2020 2020 2020 5468 6973  .z..        This
-00003730: 2069 7320 7768 6572 6520 7468 6520 6361   is where the ca
-00003740: 6d65 7261 2061 7272 6179 2036 2044 6f46  mera array 6 DoF
-00003750: 2069 7320 7365 742e 204d 616e 792c 206d   is set. Many, m
-00003760: 616e 7920 7468 696e 6773 2061 7265 2068  any things are h
-00003770: 6170 7065 6e69 6e67 0a20 2020 2020 2020  appening.       
-00003780: 2068 6572 652c 2062 7574 2074 6865 7920   here, but they 
-00003790: 6172 6520 616c 6c20 6e65 6365 7373 6172  are all necessar
-000037a0: 7920 7374 6570 7320 6f66 2074 6865 2070  y steps of the p
-000037b0: 726f 6365 7373 2073 6f20 4920 6469 646e  rocess so I didn
-000037c0: 2774 2077 616e 7420 746f 0a20 2020 2020  't want to.     
-000037d0: 2020 2074 7279 2074 6f20 656e 6361 7073     try to encaps
-000037e0: 756c 6174 6520 616e 7920 6675 7274 6865  ulate any furthe
-000037f0: 720a 2020 2020 2020 2020 7218 0000 0029  r.        r....)
-00003800: 015a 0e62 6f61 7264 735f 7361 6d70 6c65  .Z.boards_sample
-00003810: 647a 1b52 656d 6f76 696e 6720 7468 6520  dz.Removing the 
-00003820: 776f 7273 7420 6669 7474 696e 6720 e964  worst fitting .d
-00003830: 0000 007a 2120 7065 7263 656e 7420 6f66  ...z! percent of
-00003840: 2070 6f69 6e74 7320 6672 6f6d 2074 6865   points from the
-00003850: 206d 6f64 656c 4e29 1572 0f00 0000 7228   modelN).r....r(
-00003860: 0000 005a 0974 6f6d 6c5f 7061 7468 722e  ...Z.toml_pathr.
-00003870: 0000 005a 1473 7465 7265 6f5f 6361 6c69  ...Z.stereo_cali
-00003880: 6272 6174 655f 616c 6c72 0d00 0000 5a15  brate_allr....Z.
-00003890: 6765 745f 6265 7374 5f63 616d 6572 615f  get_best_camera_
-000038a0: 6172 7261 7972 4f00 0000 7214 0000 0072  arrayrO...r....r
-000038b0: 9a00 0000 7211 0000 0072 9700 0000 da08  ....r....r......
-000038c0: 6f70 7469 6d69 7a65 7212 0000 0072 3900  optimizer....r9.
-000038d0: 0000 729b 0000 0072 5500 0000 7256 0000  ..r....rU...rV..
-000038e0: 00da 1146 494c 5445 5245 445f 4652 4143  ...FILTERED_FRAC
-000038f0: 5449 4f4e 5a16 6669 6c74 6572 5f70 6f69  TIONZ.filter_poi
-00003900: 6e74 5f65 7374 696d 6174 6573 5a13 7361  nt_estimatesZ.sa
-00003910: 7665 5f63 6170 7475 7265 5f76 6f6c 756d  ve_capture_volum
-00003920: 6529 0272 3c00 0000 5a10 7374 6572 656f  e).r<...Z.stereo
-00003930: 6361 6c69 6272 6174 6f72 7225 0000 0072  calibratorr%...r
-00003940: 2500 0000 7226 0000 00da 1365 7374 696d  %...r&.....estim
-00003950: 6174 655f 6578 7472 696e 7369 6373 f601  ate_extrinsics..
-00003960: 0000 732a 0000 0002 060a 0104 ff0c 0302  ..s*............
-00003970: 0206 0102 ff04 0204 fe02 0408 0106 ff10  ................
-00003980: 040a 0110 0204 020e 0104 ff0c 030a 0112  ................
-00003990: 027a 1b53 6573 7369 6f6e 2e65 7374 696d  .z.Session.estim
-000039a0: 6174 655f 6578 7472 696e 7369 6373 726e  ate_extrinsicsrn
-000039b0: 0000 0029 0146 2929 721b 0000 0072 1c00  ...).F))r....r..
-000039c0: 0000 721d 0000 0072 0300 0000 7288 0000  ..r....r....r...
-000039d0: 0072 4300 0000 7294 0000 0072 9300 0000  .rC...r....r....
-000039e0: 7219 0000 005a 136d 6f64 655f 6368 616e  r....Z.mode_chan
-000039f0: 6765 5f73 7563 6365 7373 7215 0000 0072  ge_successr....r
-00003a00: 2b00 0000 7249 0000 0072 4c00 0000 7251  +...rI...rL...rQ
-00003a10: 0000 0072 5800 0000 725a 0000 0072 6100  ...rX...rZ...ra.
-00003a20: 0000 726a 0000 00da 0369 6e74 726c 0000  ..rj.....intrl..
-00003a30: 0072 6f00 0000 7262 0000 00da 0462 6f6f  .ro...rb.....boo
-00003a40: 6c72 6700 0000 7266 0000 0072 7200 0000  lrg...rf...rr...
-00003a50: 7273 0000 0072 7b00 0000 7284 0000 0072  rs...r{...r....r
-00003a60: 6500 0000 7286 0000 0072 6800 0000 7264  e...r....rh...rd
-00003a70: 0000 0072 0500 0000 7291 0000 0072 9200  ...r....r....r..
-00003a80: 0000 7285 0000 0072 9c00 0000 72a0 0000  ..r....r....r...
-00003a90: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00003aa0: 7225 0000 0072 2500 0000 723d 0000 0072  r%...r%...r=...r
-00003ab0: 2600 0000 7227 0000 0030 0000 0073 4a00  &...r'...0...sJ.
-00003ac0: 0000 0800 0601 0601 0601 0601 0802 1202  ................
-00003ad0: 0822 0812 0807 080b 081d 081e 0e10 0e38  .".............8
-00003ae0: 0e16 080f 0e06 0804 0806 0804 0804 0807  ................
-00003af0: 0823 0826 100b 080d 020a 04ff 0201 02ff  .#.&............
-00003b00: 0201 0aff 080c 080f 0816 1016 7227 0000  ............r'..
-00003b10: 0029 33da 0d70 7978 7933 642e 6c6f 6767  .)3..pyxy3d.logg
-00003b20: 6572 da06 7079 7879 3364 7255 0000 00da  er..pyxy3drU....
-00003b30: 0367 6574 721b 0000 00da 0c50 7951 7436  .getr......PyQt6
-00003b40: 2e51 7443 6f72 6572 0200 0000 7203 0000  .QtCorer....r...
-00003b50: 005a 1263 6f6e 6375 7272 656e 742e 6675  .Z.concurrent.fu
-00003b60: 7475 7265 7372 0400 0000 da07 7061 7468  turesr......path
-00003b70: 6c69 6272 0500 0000 da04 7469 6d65 7206  libr......timer.
-00003b80: 0000 00da 0465 6e75 6d72 0700 0000 7208  .....enumr....r.
-00003b90: 0000 00da 1f70 7978 7933 642e 7472 6163  .....pyxy3d.trac
-00003ba0: 6b65 7273 2e63 6861 7275 636f 5f74 7261  kers.charuco_tra
-00003bb0: 636b 6572 7209 0000 005a 2170 7978 7933  ckerr....Z!pyxy3
-00003bc0: 642e 6361 6c69 6272 6174 696f 6e2e 6d6f  d.calibration.mo
-00003bd0: 6e6f 6361 6c69 6272 6174 6f72 720a 0000  nocalibratorr...
-00003be0: 005a 1570 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
-00003bf0: 732e 6361 6d65 7261 720b 0000 005a 1b70  s.camerar....Z.p
-00003c00: 7978 7933 642e 6361 6d65 7261 732e 7379  yxy3d.cameras.sy
-00003c10: 6e63 6872 6f6e 697a 6572 720c 0000 005a  nchronizerr....Z
-00003c20: 2770 7978 7933 642e 6361 6d65 7261 732e  'pyxy3d.cameras.
-00003c30: 6361 6d65 7261 5f61 7272 6179 5f69 6e69  camera_array_ini
-00003c40: 7469 616c 697a 6572 720d 0000 005a 1070  tializerr....Z.p
-00003c50: 7978 7933 642e 696e 7465 7266 6163 6572  yxy3d.interfacer
-00003c60: 0e00 0000 5a23 7079 7879 3364 2e63 616c  ....Z#pyxy3d.cal
-00003c70: 6962 7261 7469 6f6e 2e73 7465 7265 6f63  ibration.stereoc
-00003c80: 616c 6962 7261 746f 7272 0f00 0000 5a31  alibratorr....Z1
-00003c90: 7079 7879 3364 2e63 616c 6962 7261 7469  pyxy3d.calibrati
-00003ca0: 6f6e 2e63 6170 7475 7265 5f76 6f6c 756d  on.capture_volum
-00003cb0: 652e 706f 696e 745f 6573 7469 6d61 7465  e.point_estimate
-00003cc0: 7372 1000 0000 5a30 7079 7879 3364 2e63  sr....Z0pyxy3d.c
-00003cd0: 616c 6962 7261 7469 6f6e 2e63 6170 7475  alibration.captu
-00003ce0: 7265 5f76 6f6c 756d 652e 6361 7074 7572  re_volume.captur
-00003cf0: 655f 766f 6c75 6d65 7211 0000 005a 3470  e_volumer....Z4p
-00003d00: 7978 7933 642e 6361 6c69 6272 6174 696f  yxy3d.calibratio
-00003d10: 6e2e 6361 7074 7572 655f 766f 6c75 6d65  n.capture_volume
-00003d20: 2e71 7561 6c69 7479 5f63 6f6e 7472 6f6c  .quality_control
-00003d30: 6c65 7272 1200 0000 5a1b 7079 7879 3364  lerr....Z.pyxy3d
-00003d40: 2e63 616d 6572 6173 2e63 616d 6572 615f  .cameras.camera_
-00003d50: 6172 7261 7972 1300 0000 5a46 7079 7879  arrayr....ZFpyxy
-00003d60: 3364 2e63 616c 6962 7261 7469 6f6e 2e63  3d.calibration.c
-00003d70: 6170 7475 7265 5f76 6f6c 756d 652e 6865  apture_volume.he
-00003d80: 6c70 6572 5f66 756e 6374 696f 6e73 2e67  lper_functions.g
-00003d90: 6574 5f70 6f69 6e74 5f65 7374 696d 6174  et_point_estimat
-00003da0: 6573 7214 0000 00da 1370 7978 7933 642e  esr......pyxy3d.
-00003db0: 636f 6e66 6967 7572 6174 6f72 7215 0000  configuratorr...
-00003dc0: 005a 1a70 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
-00003dd0: 732e 6c69 7665 5f73 7472 6561 6d72 1600  s.live_streamr..
-00003de0: 0000 5a1f 7079 7879 3364 2e72 6563 6f72  ..Z.pyxy3d.recor
-00003df0: 6469 6e67 2e76 6964 656f 5f72 6563 6f72  ding.video_recor
-00003e00: 6465 7272 1700 0000 727f 0000 0072 9f00  derr....r....r..
-00003e10: 0000 7219 0000 0072 2700 0000 7225 0000  ..r....r'...r%..
-00003e20: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00003e30: da08 3c6d 6f64 756c 653e 0100 0000 7334  ..<module>....s4
-00003e40: 0000 0008 010c 0210 020c 010c 010c 0110  ................
-00003e50: 010c 020c 010c 010c 010c 010c 010c 020c  ................
-00003e60: 010c 010c 010c 020c 010c 030c 010c 0104  ................
-00003e70: 0304 0110 0314 0b                        .......
+00001230: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00001240: 0400 0000 4300 0000 7324 0000 0064 017d  ....C...s$...d.}
+00001250: 017c 006a 00a0 01a1 0044 005d 087d 0274  .|.j.....D.].}.t
+00001260: 02a0 037c 029b 00a1 0101 0071 077c 0153  ...|.......q.|.S
+00001270: 0029 027a 690a 2020 2020 2020 2020 506f  .).zi.        Po
+00001280: 7374 2070 726f 6365 7373 696e 6720 6361  st processing ca
+00001290: 6e20 6f6e 6c79 2062 6520 7065 7266 6f72  n only be perfor
+000012a0: 6d65 6420 6966 2072 6563 6f72 6469 6e67  med if recording
+000012b0: 7320 6578 6973 7420 616e 6420 6578 7472  s exist and extr
+000012c0: 696e 7369 6373 2061 7265 2063 616c 6962  insics are calib
+000012d0: 7261 7465 640a 2020 2020 2020 2020 4629  rated.        F)
+000012e0: 0472 2c00 0000 da07 6974 6572 6469 7272  .r,.....iterdirr
+000012f0: 5400 0000 da04 7761 726e 2903 723b 0000  T.....warn).r;..
+00001300: 0072 4a00 0000 da01 6672 2500 0000 7225  .rJ.....fr%...r%
+00001310: 0000 0072 2600 0000 da1b 6973 5f70 6f73  ...r&.....is_pos
+00001320: 745f 7072 6f63 6573 7369 6e67 5f65 6c69  t_processing_eli
+00001330: 6769 626c 65b9 0000 0073 0800 0000 0406  gible....s......
+00001340: 0e01 0e01 0403 7a23 5365 7373 696f 6e2e  ......z#Session.
+00001350: 6973 5f70 6f73 745f 7072 6f63 6573 7369  is_post_processi
+00001360: 6e67 5f65 6c69 6769 626c 6572 3a00 0000  ng_eligibler:...
+00001370: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001380: 0003 0000 0043 0000 0073 8001 0000 7c01  .....C...s....|.
+00001390: 7c00 5f00 7c00 a001 a100 0100 7c00 6a00  |._.|.......|.j.
+000013a0: 0400 7402 6a03 6b02 721f 0100 7c00 6a04  ..t.j.k.r...|.j.
+000013b0: 721d 7c00 6a05 a006 a100 0100 7c00 a007  r.|.j.......|...
+000013c0: a100 0100 6403 5300 6403 5300 0400 7402  ....d.S.d.S...t.
+000013d0: 6a08 6b02 7235 0100 7c00 6a04 7233 7c00  j.k.r5..|.j.r3|.
+000013e0: 6a05 a006 a100 0100 7c00 a007 a100 0100  j.......|.......
+000013f0: 6403 5300 6403 5300 0400 7402 6a09 6b02  d.S.d.S...t.j.k.
+00001400: 7262 0100 740a 7c00 6a0b 8301 7c00 5f0c  rb..t.|.j...|._.
+00001410: 7c00 6a04 7348 7c00 a00d a100 0100 7c00  |.j.sH|.......|.
+00001420: 6a05 a006 a100 0100 7c00 a007 a100 0100  j.......|.......
+00001430: 7c00 a00e a100 0100 7c00 a00f 6401 a101  |.......|...d...
+00001440: 0100 7c00 a010 7c00 6a11 a101 0100 6403  ..|...|.j.....d.
+00001450: 5300 0400 7402 6a12 6b02 7289 0100 740a  S...t.j.k.r...t.
+00001460: 7c00 6a0b 8301 7c00 5f0c 7c00 6a04 7375  |.j...|._.|.j.su
+00001470: 7c00 a00d a100 0100 7c00 a007 a100 0100  |.......|.......
+00001480: 7c00 a00e a100 0100 7c00 a00f 6401 a101  |.......|...d...
+00001490: 0100 7c00 6a05 a013 a100 0100 6403 5300  ..|.j.......d.S.
+000014a0: 0400 7402 6a14 6b02 729f 0100 7c00 6a04  ..t.j.k.r...|.j.
+000014b0: 729d 7c00 a007 a100 0100 7c00 6a05 a006  r.|.......|.j...
+000014c0: a100 0100 6403 5300 6403 5300 7402 6a15  ....d.S.d.S.t.j.
+000014d0: 6b02 72be 7c00 6a04 73aa 7c00 a00d a100  k.r.|.j.s.|.....
+000014e0: 0100 7c00 a007 a100 0100 7c00 a00f 6402  ..|.......|...d.
+000014f0: a101 0100 7c00 a001 a100 0100 7c00 6a05  ....|.......|.j.
+00001500: a013 a100 0100 6403 5300 6403 5300 2904  ......d.S.d.S.).
+00001510: 7aaf 0a20 2020 2020 2020 2056 6961 2074  z..        Via t
+00001520: 6869 7320 6d65 7468 6f64 2c20 7468 6520  his method, the 
+00001530: 6672 616d 6520 7265 6164 696e 6720 6265  frame reading be
+00001540: 6861 7669 6f72 2077 696c 6c20 6265 2063  havior will be c
+00001550: 6861 6e67 6564 2062 7920 7468 6520 4755  hanged by the GU
+00001560: 492e 2049 6620 736f 6d65 2070 726f 7065  I. If some prope
+00001570: 7274 6965 7320 6172 650a 2020 2020 2020  rties are.      
+00001580: 2020 6e6f 7420 6176 6169 6c61 626c 6520    not available 
+00001590: 2869 2e65 2e20 7379 6e63 6872 6f6e 697a  (i.e. synchroniz
+000015a0: 6572 2920 7468 6579 2077 696c 6c20 6265  er) they will be
+000015b0: 2063 7265 6174 6564 0a20 2020 2020 2020   created.       
+000015c0: 2054 464e 2916 723a 0000 00da 1275 7064   TFN).r:.....upd
+000015d0: 6174 655f 7374 7265 616d 735f 6670 7372  ate_streams_fpsr
+000015e0: 1900 0000 721f 0000 0072 3100 0000 7241  ....r....r1...rA
+000015f0: 0000 00da 1875 6e73 7562 7363 7269 6265  .....unsubscribe
+00001600: 5f66 726f 6d5f 7374 7265 616d 73da 1970  _from_streams..p
+00001610: 6175 7365 5f61 6c6c 5f6d 6f6e 6f63 616c  ause_all_monocal
+00001620: 6962 7261 746f 7273 7224 0000 0072 2000  ibratorsr$...r .
+00001630: 0000 7209 0000 0072 3800 0000 7239 0000  ..r....r8...r9..
+00001640: 00da 116c 6f61 645f 7374 7265 616d 5f74  ...load_stream_t
+00001650: 6f6f 6c73 da13 7365 745f 7374 7265 616d  ools..set_stream
+00001660: 735f 6368 6172 7563 6fda 1473 6574 5f73  s_charuco..set_s
+00001670: 7472 6561 6d73 5f74 7261 636b 696e 67da  treams_tracking.
+00001680: 1761 6374 6976 6174 655f 6d6f 6e6f 6361  .activate_monoca
+00001690: 6c69 6272 6174 6f72 7233 0000 0072 2100  libratorr3...r!.
+000016a0: 0000 da14 7375 6273 6372 6962 655f 746f  ....subscribe_to
+000016b0: 5f73 7472 6561 6d73 7222 0000 0072 2300  _streamsr"...r#.
+000016c0: 0000 2902 723b 0000 0072 3a00 0000 7225  ..).r;...r:...r%
+000016d0: 0000 0072 2500 0000 7226 0000 00da 0873  ...r%...r&.....s
+000016e0: 6574 5f6d 6f64 65c6 0000 0073 5600 0000  et_mode....sV...
+000016f0: 0605 0801 0402 0c01 0601 0a01 0c01 04fe  ................
+00001700: 0c04 0601 0a01 0c01 04fe 0c04 0c02 0602  ................
+00001710: 0801 0a01 0801 0801 0a01 1001 0c02 0c02  ................
+00001720: 0601 0801 0802 0801 0a01 0e01 0c02 0601  ................
+00001730: 0801 0e01 04fe 0804 0601 0801 0802 0a01  ................
+00001740: 0801 0e01 04f9 7a10 5365 7373 696f 6e2e  ......z.Session.
+00001750: 7365 745f 6d6f 6465 da0a 6670 735f 7461  set_mode..fps_ta
+00001760: 7267 6574 6302 0000 0000 0000 0000 0000  rgetc...........
+00001770: 0002 0000 0003 0000 0043 0000 0073 8600  .........C...s..
+00001780: 0000 7c00 6a00 0400 7401 6a02 6b02 7209  ..|.j...t.j.k.r.
+00001790: 0100 6e34 0400 7401 6a03 6b02 7210 0100  ..n4..t.j.k.r...
+000017a0: 6e2d 0400 7401 6a04 6b02 7220 0100 7c01  n-..t.j.k.r ..|.
+000017b0: 7c00 5f05 7c00 6a06 a007 7c01 a101 0100  |._.|.j...|.....
+000017c0: 6e1d 0400 7401 6a08 6b02 7230 0100 7c01  n...t.j.k.r0..|.
+000017d0: 7c00 5f09 7c00 6a06 a00a 7c01 a101 0100  |._.|.j...|.....
+000017e0: 6e0d 7401 6a0b 6b02 723d 7c01 7c00 5f0c  n.t.j.k.r=|.|._.
+000017f0: 7c00 6a06 a00d 7c01 a101 0100 7c00 a00e  |.j...|.....|...
+00001800: a100 0100 6401 5300 2902 7a78 0a20 2020  ....d.S.).zx.   
+00001810: 2020 2020 2055 7064 6174 6573 2074 6865       Updates the
+00001820: 2046 5053 2075 7365 6420 6279 2074 6865   FPS used by the
+00001830: 2063 7572 7265 6e74 6c79 2061 6374 6976   currently activ
+00001840: 6520 7365 7373 696f 6e20 6d6f 6465 0a20  e session mode. 
+00001850: 2020 2020 2020 2054 6869 7320 7570 6461         This upda
+00001860: 7465 2069 6e63 6c75 6465 7320 7468 6520  te includes the 
+00001870: 636f 6e66 6967 2e74 6f6d 6c0a 2020 2020  config.toml.    
+00001880: 2020 2020 4e29 0f72 3a00 0000 7219 0000      N).r:...r...
+00001890: 0072 1f00 0000 7224 0000 0072 2000 0000  .r....r$...r ...
+000018a0: 7236 0000 0072 2800 0000 5a1e 7361 7665  r6...r(...Z.save
+000018b0: 5f66 7073 5f69 6e74 7269 6e73 6963 5f63  _fps_intrinsic_c
+000018c0: 616c 6962 7261 7469 6f6e 7221 0000 0072  alibrationr!...r
+000018d0: 3500 0000 5a1e 7361 7665 5f66 7073 5f65  5...Z.save_fps_e
+000018e0: 7874 7269 6e73 6963 5f63 616c 6962 7261  xtrinsic_calibra
+000018f0: 7469 6f6e 7223 0000 0072 3400 0000 5a12  tionr#...r4...Z.
+00001900: 7361 7665 5f66 7073 5f72 6563 6f72 6469  save_fps_recordi
+00001910: 6e67 725e 0000 0029 0272 3b00 0000 7267  ngr^...).r;...rg
+00001920: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
+00001930: 0000 da13 7365 745f 6163 7469 7665 5f6d  ....set_active_m
+00001940: 6f64 655f 6670 73fe 0000 0073 1e00 0000  ode_fps....s....
+00001950: 0405 0c01 0201 0c01 0201 0c01 0601 0e01  ................
+00001960: 0c01 0601 0e01 0801 0601 0c01 0c02 7a1b  ..............z.
+00001970: 5365 7373 696f 6e2e 7365 745f 6163 7469  Session.set_acti
+00001980: 7665 5f6d 6f64 655f 6670 73da 0672 6574  ve_mode_fps..ret
+00001990: 7572 6e63 0100 0000 0000 0000 0000 0000  urnc............
+000019a0: 0200 0000 0300 0000 4300 0000 736e 0000  ........C...sn..
+000019b0: 0064 007d 017c 006a 0004 0074 016a 026b  .d.}.|.j...t.j.k
+000019c0: 0272 0d01 0009 007c 0153 0004 0074 016a  .r.....|.S...t.j
+000019d0: 036b 0272 1601 0009 007c 0153 0004 0074  .k.r.....|.S...t
+000019e0: 016a 046b 0272 2101 007c 006a 057d 017c  .j.k.r!..|.j.}.|
+000019f0: 0153 0004 0074 016a 066b 0272 2c01 007c  .S...t.j.k.r,..|
+00001a00: 006a 077d 017c 0153 0074 016a 086b 0272  .j.}.|.S.t.j.k.r
+00001a10: 357c 006a 097d 017c 0153 007c 0153 00a9  5|.j.}.|.S.|.S..
+00001a20: 014e 290a 723a 0000 0072 1900 0000 721f  .N).r:...r....r.
+00001a30: 0000 0072 2400 0000 7220 0000 0072 3600  ...r$...r ...r6.
+00001a40: 0000 7221 0000 0072 3500 0000 7223 0000  ..r!...r5...r#..
+00001a50: 0072 3400 0000 2902 723b 0000 005a 0366  .r4...).r;...Z.f
+00001a60: 7073 7225 0000 0072 2500 0000 7226 0000  psr%...r%...r&..
+00001a70: 00da 1367 6574 5f61 6374 6976 655f 6d6f  ...get_active_mo
+00001a80: 6465 5f66 7073 1401 0000 7322 0000 0004  de_fps....s"....
+00001a90: 0104 010c 0102 0104 090c f802 0104 070c  ................
+00001aa0: fa06 0104 050c fc06 0104 0308 fe06 0108  ................
+00001ab0: 017a 1b53 6573 7369 6f6e 2e67 6574 5f61  .z.Session.get_a
+00001ac0: 6374 6976 655f 6d6f 6465 5f66 7073 6301  ctive_mode_fpsc.
+00001ad0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00001ae0: 0000 0043 0000 0073 3600 0000 7c00 a000  ...C...s6...|...
+00001af0: a100 7d01 7c01 6400 7501 7217 7c00 6a01  ..}.|.d.u.r.|.j.
+00001b00: a002 a100 4400 5d0b 5c02 7d02 7d03 7c03  ....D.].\.}.}.|.
+00001b10: a003 7c01 a101 0100 710d 6400 5300 6400  ..|.....q.d.S.d.
+00001b20: 5300 726a 0000 0029 0472 6b00 0000 722f  S.rj...).rk...r/
+00001b30: 0000 0072 3e00 0000 5a0e 7365 745f 6670  ...r>...Z.set_fp
+00001b40: 735f 7461 7267 6574 2904 723b 0000 005a  s_target).r;...Z
+00001b50: 0f61 6374 6976 655f 6d6f 6465 5f66 7073  .active_mode_fps
+00001b60: 7244 0000 0072 4500 0000 7225 0000 0072  rD...rE...r%...r
+00001b70: 2500 0000 7226 0000 0072 5e00 0000 2301  %...r&...r^...#.
+00001b80: 0000 730c 0000 0008 0108 0112 010c 0104  ..s.............
+00001b90: fe04 017a 1a53 6573 7369 6f6e 2e75 7064  ...z.Session.upd
+00001ba0: 6174 655f 7374 7265 616d 735f 6670 73da  ate_streams_fps.
+00001bb0: 0b74 7261 636b 696e 675f 6f6e 6302 0000  .tracking_onc...
+00001bc0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00001bd0: 0043 0000 0073 2200 0000 7c00 6a00 a001  .C...s"...|.j...
+00001be0: a100 4400 5d09 5c02 7d02 7d03 7c03 a002  ..D.].\.}.}.|...
+00001bf0: 7c01 a101 0100 7105 6400 5300 726a 0000  |.....q.d.S.rj..
+00001c00: 0029 0372 2f00 0000 723e 0000 005a 0f73  .).r/...r>...Z.s
+00001c10: 6574 5f74 7261 636b 696e 675f 6f6e 2904  et_tracking_on).
+00001c20: 723b 0000 0072 6c00 0000 7244 0000 0072  r;...rl...rD...r
+00001c30: 4500 0000 7225 0000 0072 2500 0000 7226  E...r%...r%...r&
+00001c40: 0000 0072 6300 0000 2901 0000 7306 0000  ...rc...)...s...
+00001c50: 0012 010c 0104 ff7a 1c53 6573 7369 6f6e  .......z.Session
+00001c60: 2e73 6574 5f73 7472 6561 6d73 5f74 7261  .set_streams_tra
+00001c70: 636b 696e 6763 0100 0000 0000 0000 0000  ckingc..........
+00001c80: 0000 0300 0000 0400 0000 4300 0000 733a  ..........C...s:
+00001c90: 0000 0074 00a0 0164 01a1 0101 0074 027c  ...t...d.....t.|
+00001ca0: 006a 0383 017c 005f 047c 006a 05a0 06a1  .j...|._.|.j....
+00001cb0: 0044 005d 0a5c 027d 017d 027c 02a0 077c  .D.].\.}.}.|...|
+00001cc0: 006a 04a1 0101 0071 1064 0053 0029 024e  .j.....q.d.S.).N
+00001cd0: 7a22 7570 6461 7469 6e67 2063 6861 7275  z"updating charu
+00001ce0: 636f 2069 6e20 6361 7365 206e 6563 6573  co in case neces
+00001cf0: 7361 7279 2908 7254 0000 0072 5500 0000  sary).rT...rU...
+00001d00: 7209 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
+00001d10: 2f00 0000 723e 0000 005a 0e75 7064 6174  /...r>...Z.updat
+00001d20: 655f 7472 6163 6b65 7229 0372 3b00 0000  e_tracker).r;...
+00001d30: 7244 0000 0072 4500 0000 7225 0000 0072  rD...rE...r%...r
+00001d40: 2500 0000 7226 0000 0072 6200 0000 2d01  %...r&...rb...-.
+00001d50: 0000 730a 0000 000a 010c 0112 010e 0104  ..s.............
+00001d60: ff7a 1b53 6573 7369 6f6e 2e73 6574 5f73  .z.Session.set_s
+00001d70: 7472 6561 6d73 5f63 6861 7275 636f 6301  treams_charucoc.
+00001d80: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001d90: 0000 0043 0000 0073 1800 0000 7400 a001  ...C...s....t...
+00001da0: 6401 a101 0100 7c00 6a02 a003 a100 0100  d.....|.j.......
+00001db0: 6400 5300 2902 4e7a 1470 6175 7369 6e67  d.S.).Nz.pausing
+00001dc0: 2073 796e 6368 726f 6e69 7a65 7229 0472   synchronizer).r
+00001dd0: 5400 0000 7255 0000 0072 4100 0000 725f  T...rU...rA...r_
+00001de0: 0000 00a9 0172 3b00 0000 7225 0000 0072  .....r;...r%...r
+00001df0: 2500 0000 7226 0000 00da 1270 6175 7365  %...r&.....pause
+00001e00: 5f73 796e 6368 726f 6e69 7a65 7233 0100  _synchronizer3..
+00001e10: 0073 0400 0000 0a01 0e01 7a1a 5365 7373  .s........z.Sess
+00001e20: 696f 6e2e 7061 7573 655f 7379 6e63 6872  ion.pause_synchr
+00001e30: 6f6e 697a 6572 6301 0000 0000 0000 0000  onizerc.........
+00001e40: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00001e50: 1e00 0000 7c00 6a00 a001 a100 0100 7c00  ....|.j.......|.
+00001e60: 6a00 a002 7c00 6a00 6a03 a101 0100 6400  j...|.j.j.....d.
+00001e70: 5300 726a 0000 0029 0472 4100 0000 7265  S.rj...).rA...re
+00001e80: 0000 005a 0e73 6574 5f73 7472 6561 6d5f  ...Z.set_stream_
+00001e90: 6670 7372 6700 0000 726d 0000 0072 2500  fpsrg...rm...r%.
+00001ea0: 0000 7225 0000 0072 2600 0000 da14 756e  ..r%...r&.....un
+00001eb0: 7061 7573 655f 7379 6e63 6872 6f6e 697a  pause_synchroniz
+00001ec0: 6572 3701 0000 7304 0000 000a 0114 017a  er7...s........z
+00001ed0: 1c53 6573 7369 6f6e 2e75 6e70 6175 7365  .Session.unpause
+00001ee0: 5f73 796e 6368 726f 6e69 7a65 7263 0100  _synchronizerc..
+00001ef0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00001f00: 0000 4300 0000 7334 0000 0064 017d 017c  ..C...s4...d.}.|
+00001f10: 006a 006a 01a0 02a1 00a0 03a1 0044 005d  .j.j.........D.]
+00001f20: 0d5c 027d 027d 037c 02a0 0464 02a1 0172  .\.}.}.|...d...r
+00001f30: 177c 0164 0337 007d 0171 0a7c 0153 0029  .|.d.7.}.q.|.S.)
+00001f40: 044e 7201 0000 0072 4600 0000 e901 0000  .Nr....rF.......
+00001f50: 0029 0572 2800 0000 da04 6469 6374 da04  .).r(.....dict..
+00001f60: 636f 7079 723e 0000 00da 0a73 7461 7274  copyr>.....start
+00001f70: 7377 6974 6829 0472 3b00 0000 da05 636f  swith).r;.....co
+00001f80: 756e 74da 036b 6579 da06 7061 7261 6d73  unt..key..params
+00001f90: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+00001fa0: 1b67 6574 5f63 6f6e 6669 6775 7265 645f  .get_configured_
+00001fb0: 6361 6d65 7261 5f63 6f75 6e74 3b01 0000  camera_count;...
+00001fc0: 730c 0000 0004 0118 010a 0108 0102 8004  s...............
+00001fd0: 017a 2353 6573 7369 6f6e 2e67 6574 5f63  .z#Session.get_c
+00001fe0: 6f6e 6669 6775 7265 645f 6361 6d65 7261  onfigured_camera
+00001ff0: 5f63 6f75 6e74 6301 0000 0000 0000 0000  _countc.........
+00002000: 0000 0005 0000 0008 0000 0003 0000 0073  ...............s
+00002010: 8c00 0000 8700 6601 6401 6402 8408 7d01  ......f.d.d...}.
+00002020: 7400 8300 8f1e 7d02 7401 6403 7402 8302  t.....}.t.d.t...
+00002030: 4400 5d10 7d03 7c03 8800 6a03 a004 a100  D.].}.|...j.....
+00002040: 7600 7219 710f 7c02 a005 7c01 7c03 a102  v.r.q.|...|.|...
+00002050: 0100 710f 5700 6404 0400 0400 8303 0100  ..q.W.d.........
+00002060: 6e08 3100 732a 7701 0100 0100 0100 5900  n.1.s*w.......Y.
+00002070: 0100 8800 6a06 6a07 a008 a100 a004 a100  ....j.j.........
+00002080: 4400 5d0c 7d04 7c04 a009 6405 a101 7243  D.].}.|...d...rC
+00002090: 8800 6a06 6a07 7c04 3d00 7137 6404 5300  ..j.j.|.=.q7d.S.
+000020a0: 2906 7aa3 0a20 2020 2020 2020 2043 616c  ).z..        Cal
+000020b0: 6c65 6420 6279 206c 6f61 645f 7374 7265  led by load_stre
+000020c0: 616d 7320 696e 2074 6865 2065 7665 6e74  ams in the event
+000020d0: 2074 6861 7420 6e6f 2063 616d 6572 6173   that no cameras
+000020e0: 2061 7265 2072 6574 7572 6e65 6420 6279   are returned by
+000020f0: 2074 6865 2063 6f6e 6669 6775 7261 746f   the configurato
+00002100: 722e 2e2e 0a20 2020 2020 2020 2057 696c  r....        Wil
+00002110: 6c20 706f 7075 6c61 7465 2073 656c 662e  l populate self.
+00002120: 6361 6d65 7261 7320 7573 696e 6720 6d75  cameras using mu
+00002130: 6c74 6970 6c65 2074 6872 6561 6473 0a20  ltiple threads. 
+00002140: 2020 2020 2020 2063 0100 0000 0000 0000         c........
+00002150: 0000 0000 0200 0000 0700 0000 1300 0000  ................
+00002160: 738c 0000 007a 3774 00a0 0164 017c 009b  s....z7t...d.|..
+00002170: 009d 02a1 0101 0074 027c 0083 017d 0174  .......t.|...}.t
+00002180: 00a0 0164 027c 009b 009d 02a1 0101 007c  ...d.|.........|
+00002190: 0188 006a 037c 003c 0088 006a 04a0 057c  ...j.|.<...j...|
+000021a0: 01a1 0101 0074 00a0 0164 037c 009b 0064  .....t...d.|...d
+000021b0: 049d 03a1 0101 0074 067c 0174 0788 006a  .......t.|.t...j
+000021c0: 0883 0164 058d 0288 006a 097c 003c 0057  ...d.....j.|.<.W
+000021d0: 0064 0053 0001 0001 0001 0074 00a0 0164  .d.S.......t...d
+000021e0: 067c 009b 009d 02a1 0101 0059 0064 0053  .|.........Y.d.S
+000021f0: 0029 074e 7a0c 5472 7969 6e67 2070 6f72  .).Nz.Trying por
+00002200: 7420 7a10 5375 6363 6573 7320 6174 2070  t z.Success at p
+00002210: 6f72 7420 7a17 4c6f 6164 696e 6720 7374  ort z.Loading st
+00002220: 7265 616d 2061 7420 706f 7274 207a 2520  ream at port z% 
+00002230: 7769 7468 2063 6861 7275 636f 2074 7261  with charuco tra
+00002240: 636b 6572 2066 6f72 2063 616c 6962 7261  cker for calibra
+00002250: 7469 6f6e a901 da07 7472 6163 6b65 727a  tion....trackerz
+00002260: 124e 6f20 6361 6d65 7261 2061 7420 706f  .No camera at po
+00002270: 7274 2029 0a72 5400 0000 7255 0000 0072  rt ).rT...rU...r
+00002280: 0b00 0000 722e 0000 0072 2800 0000 5a0b  ....r....r(...Z.
+00002290: 7361 7665 5f63 616d 6572 6172 1600 0000  save_camerar....
+000022a0: 7209 0000 0072 3800 0000 722f 0000 0029  r....r8...r/...)
+000022b0: 0272 4400 0000 7246 0000 0072 6d00 0000  .rD...rF...rm...
+000022c0: 7225 0000 0072 2600 0000 da07 6164 645f  r%...r&.....add_
+000022d0: 6361 6d48 0100 0073 1c00 0000 0201 1001  camH...s........
+000022e0: 0801 1001 0a01 0c01 0401 0a01 04ff 0203  ................
+000022f0: 0a01 12ff 0603 1601 7a26 5365 7373 696f  ........z&Sessio
+00002300: 6e2e 5f66 696e 645f 6361 6d65 7261 732e  n._find_cameras.
+00002310: 3c6c 6f63 616c 733e 2e61 6464 5f63 616d  <locals>.add_cam
+00002320: 7201 0000 004e 5a06 7374 6572 656f 290a  r....NZ.stereo).
+00002330: 7204 0000 00da 0572 616e 6765 da15 4d41  r......range..MA
+00002340: 585f 4341 4d45 5241 5f50 4f52 545f 4348  X_CAMERA_PORT_CH
+00002350: 4543 4b72 2e00 0000 da04 6b65 7973 da06  ECKr......keys..
+00002360: 7375 626d 6974 7228 0000 0072 7100 0000  submitr(...rq...
+00002370: 7272 0000 0072 7300 0000 2905 723b 0000  rr...rs...).r;..
+00002380: 0072 7a00 0000 da08 6578 6563 7574 6f72  .rz.....executor
+00002390: da01 6972 7500 0000 7225 0000 0072 6d00  ..iru...r%...rm.
+000023a0: 0000 7226 0000 00da 0d5f 6669 6e64 5f63  ..r&....._find_c
+000023b0: 616d 6572 6173 4201 0000 731a 0000 000c  amerasB...s.....
+000023c0: 0608 100e 010e 0102 020e 0202 fb1c ff14  ................
+000023d0: 090a 010a 0102 8004 fe7a 1553 6573 7369  .........z.Sessi
+000023e0: 6f6e 2e5f 6669 6e64 5f63 616d 6572 6173  on._find_cameras
+000023f0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00002400: 0005 0000 0043 0000 0073 d000 0000 6401  .....C...s....d.
+00002410: 7c00 5f00 7c00 6a01 a002 a100 7c00 5f03  |._.|.j.....|._.
+00002420: 7404 7c00 6a03 8301 6402 6b02 7214 7c00  t.|.j...d.k.r.|.
+00002430: a005 a100 0100 7c00 6a03 a006 a100 4400  ......|.j.....D.
+00002440: 5d1e 5c02 7d01 7d02 7c01 7c00 6a07 a008  ].\.}.}.|.|.j...
+00002450: a100 7600 7225 7119 7409 a00a 6403 7c01  ..v.r%q.t...d.|.
+00002460: 9b00 9d02 a101 0100 740b 7c02 7c00 6a0c  ........t.|.|.j.
+00002470: 6404 8d02 7c00 6a07 7c01 3c00 7119 7c00  d...|.j.|.<.q.|.
+00002480: a00d a100 0100 7c00 a00e a100 0100 740f  ......|.......t.
+00002490: 7c00 6a10 a008 a100 8301 7c00 5f11 7412  |.j.......|._.t.
+000024a0: 7c00 6a07 8301 7c00 5f13 6401 7c00 5f14  |.j...|._.d.|._.
+000024b0: 6405 7c00 5f00 7409 a00a 6406 a101 0100  d.|._.t...d.....
+000024c0: 7c00 6a15 a016 a100 0100 7c00 a017 a100  |.j.......|.....
+000024d0: 0100 7c00 a018 a100 0100 6407 5300 2908  ..|.......d.S.).
+000024e0: 7aad 0a20 2020 2020 2020 2043 6f6e 6e65  z..        Conne
+000024f0: 6374 7320 746f 2073 746f 7265 6420 6361  cts to stored ca
+00002500: 6d65 7261 7320 616e 6420 6372 6561 7465  meras and create
+00002510: 7320 7374 7265 616d 7320 7769 7468 2070  s streams with p
+00002520: 726f 7669 6465 6420 7472 6163 6b69 6e67  rovided tracking
+00002530: 0a20 2020 2020 2020 2042 6563 6175 7365  .        Because
+00002540: 2074 6865 7365 2073 7472 6561 6d73 2061   these streams a
+00002550: 7265 2061 7661 696c 6162 6c65 2c20 7468  re available, th
+00002560: 6520 7379 6e63 6872 6f6e 697a 6572 2063  e synchronizer c
+00002570: 616e 2074 6865 6e20 6265 2069 6e69 7469  an then be initi
+00002580: 616c 697a 6564 0a20 2020 2020 2020 2054  alized.        T
+00002590: 7201 0000 007a 184c 6f61 6469 6e67 2053  r....z.Loading S
+000025a0: 7472 6561 6d20 666f 7220 706f 7274 2072  tream for port r
+000025b0: 7800 0000 467a 2d53 6967 6e61 6c6c 696e  x...Fz-Signallin
+000025c0: 6720 7375 6363 6573 7366 756c 206c 6f61  g successful loa
+000025d0: 6469 6e67 206f 6620 7374 7265 616d 2074  ding of stream t
+000025e0: 6f6f 6c73 4e29 1972 3000 0000 7228 0000  oolsN).r0...r(..
+000025f0: 005a 0b67 6574 5f63 616d 6572 6173 722e  .Z.get_camerasr.
+00002600: 0000 0072 4900 0000 7281 0000 0072 3e00  ...rI...r....r>.
+00002610: 0000 722f 0000 0072 7d00 0000 7254 0000  ..r/...r}...rT..
+00002620: 0072 5500 0000 7216 0000 0072 3900 0000  .rU...r....r9...
+00002630: da13 5f61 646a 7573 745f 7265 736f 6c75  .._adjust_resolu
+00002640: 7469 6f6e 73da 155f 6c6f 6164 5f6d 6f6e  tions.._load_mon
+00002650: 6f63 616c 6962 7261 746f 7273 da03 6d69  ocalibrators..mi
+00002660: 6e72 3200 0000 7233 0000 0072 0c00 0000  nr2...r3...r....
+00002670: 7241 0000 0072 3100 0000 da1a 7374 7265  rA...r1.....stre
+00002680: 616d 5f74 6f6f 6c73 5f6c 6f61 6465 645f  am_tools_loaded_
+00002690: 7369 676e 616c 7243 0000 0072 6000 0000  signalrC...r`...
+000026a0: 726e 0000 00a9 0372 3b00 0000 7244 0000  rn.....r;...rD..
+000026b0: 0072 4600 0000 7225 0000 0072 2500 0000  .rF...r%...r%...
+000026c0: 7226 0000 0072 6100 0000 6501 0000 732a  r&...ra...e...s*
+000026d0: 0000 0006 050c 020e 0208 0112 020e 0102  ................
+000026e0: 0110 0216 0108 0208 0110 0302 0204 0106  ................
+000026f0: ff06 0506 010a 010a 0108 020c 017a 1953  .............z.S
+00002700: 6573 7369 6f6e 2e6c 6f61 645f 7374 7265  ession.load_stre
+00002710: 616d 5f74 6f6f 6c73 6301 0000 0000 0000  am_toolsc.......
+00002720: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
+00002730: 0073 5e00 0000 7c00 6a00 a001 a100 4400  .s^...|.j.....D.
+00002740: 5d27 5c02 7d01 7d02 7c01 7c00 6a02 a003  ]'\.}.}.|.|.j...
+00002750: a100 7600 721a 7404 a005 6401 7c01 9b00  ..v.r.t...d.|...
+00002760: 6402 9d03 a101 0100 7105 7404 a005 6403  d.......q.t...d.
+00002770: 7c01 9b00 9d02 a101 0100 7406 7c00 6a07  |.........t.|.j.
+00002780: 7c01 1900 8301 7c00 6a02 7c01 3c00 7105  |.....|.j.|.<.q.
+00002790: 6400 5300 2904 4e7a 2f53 6b69 7070 696e  d.S.).Nz/Skippin
+000027a0: 6720 6f76 6572 206d 6f6e 6f63 616c 6962  g over monocalib
+000027b0: 7261 746f 7220 6372 6561 7469 6f6e 2066  rator creation f
+000027c0: 6f72 2070 6f72 7420 7a1b 2062 6563 6175  or port z. becau
+000027d0: 7365 2069 7420 616c 7265 6164 7920 6578  se it already ex
+000027e0: 6973 7473 2e7a 204c 6f61 6469 6e67 204d  ists.z Loading M
+000027f0: 6f6e 6f63 616c 6962 7261 746f 7220 666f  onocalibrator fo
+00002800: 7220 706f 7274 2029 0872 2e00 0000 723e  r port ).r....r>
+00002810: 0000 0072 3200 0000 727d 0000 0072 5400  ...r2...r}...rT.
+00002820: 0000 7255 0000 0072 0a00 0000 722f 0000  ..rU...r....r/..
+00002830: 0072 8600 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+00002840: 7226 0000 0072 8300 0000 8b01 0000 7312  r&...r........s.
+00002850: 0000 0012 010e 0104 010a 0104 ff02 0310  ................
+00002860: 0216 0104 f87a 1d53 6573 7369 6f6e 2e5f  .....z.Session._
+00002870: 6c6f 6164 5f6d 6f6e 6f63 616c 6962 7261  load_monocalibra
+00002880: 746f 7273 4eda 0b61 6374 6976 655f 706f  torsN..active_po
+00002890: 7274 6302 0000 0000 0000 0000 0000 0002  rtc.............
+000028a0: 0000 0005 0000 0043 0000 0073 4600 0000  .......C...sF...
+000028b0: 7c01 6401 7501 720f 7400 a001 6402 7c01  |.d.u.r.t...d.|.
+000028c0: 9b00 9d02 a101 0100 7c01 7c00 5f02 7400  ........|.|._.t.
+000028d0: a001 6403 7c00 6a02 9b00 6404 9d03 a101  ..d.|.j...d.....
+000028e0: 0100 7c00 6a03 7c00 6a02 1900 a004 a100  ..|.j.|.j.......
+000028f0: 0100 6401 5300 2905 7a7e 0a20 2020 2020  ..d.S.).z~.     
+00002900: 2020 2055 7365 6420 746f 206d 616b 6520     Used to make 
+00002910: 7375 7265 2074 6861 7420 6f6e 6c79 2074  sure that only t
+00002920: 6865 2061 6374 6976 6520 6361 6d65 7261  he active camera
+00002930: 2074 6162 2069 7320 7265 6164 696e 6720   tab is reading 
+00002940: 6672 616d 6573 2064 7572 696e 6720 7468  frames during th
+00002950: 6520 696e 7472 696e 7369 6320 6361 6c69  e intrinsic cali
+00002960: 6272 6174 696f 6e20 7072 6f63 6573 730a  bration process.
+00002970: 2020 2020 2020 2020 4e7a 2953 6574 7469          Nz)Setti
+00002980: 6e67 2073 6573 7369 6f6e 2061 6374 6976  ng session activ
+00002990: 6520 6d6f 6e6f 6361 6c69 6272 6174 6f72  e monocalibrator
+000029a0: 2074 6f20 7a1a 4163 7469 7661 7465 2074   to z.Activate t
+000029b0: 7261 636b 696e 6720 6f6e 2070 6f72 7420  racking on port 
+000029c0: 7a16 2061 6e64 2064 6561 6374 6976 6174  z. and deactivat
+000029d0: 6520 6f74 6865 7273 2905 7254 0000 0072  e others).rT...r
+000029e0: 5500 0000 7233 0000 0072 3200 0000 5a13  U...r3...r2...Z.
+000029f0: 7375 6273 6372 6962 655f 746f 5f73 7472  subscribe_to_str
+00002a00: 6561 6d29 0272 3b00 0000 7287 0000 0072  eam).r;...r....r
+00002a10: 2500 0000 7225 0000 0072 2600 0000 7264  %...r%...r&...rd
+00002a20: 0000 0096 0100 0073 0e00 0000 0805 1001  .......s........
+00002a30: 0601 0401 0c01 04ff 1403 7a1f 5365 7373  ..........z.Sess
+00002a40: 696f 6e2e 6163 7469 7661 7465 5f6d 6f6e  ion.activate_mon
+00002a50: 6f63 616c 6962 7261 746f 7263 0100 0000  ocalibratorc....
+00002a60: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00002a70: 4300 0000 732a 0000 0074 00a0 0164 01a1  C...s*...t...d..
+00002a80: 0101 007c 006a 02a0 03a1 0044 005d 085c  ...|.j.....D.].\
+00002a90: 027d 017d 027c 02a0 04a1 0001 0071 0a64  .}.}.|.......q.d
+00002aa0: 0253 0029 037a 8b0a 2020 2020 2020 2020  .S.).z..        
+00002ab0: 7573 6564 2077 6865 6e20 6e6f 7420 6163  used when not ac
+00002ac0: 7469 7665 6c79 206f 6e20 7468 6520 6361  tively on the ca
+00002ad0: 6d65 7261 2063 616c 6962 7261 7469 6f6e  mera calibration
+00002ae0: 2074 6162 0a20 2020 2020 2020 206f 7220   tab.        or 
+00002af0: 7768 656e 2073 696c 656e 6369 6e67 2061  when silencing a
+00002b00: 6c6c 2069 6e20 7072 6570 6172 6174 696f  ll in preparatio
+00002b10: 6e20 666f 7220 6163 7469 7661 7469 6e67  n for activating
+00002b20: 206f 6e6c 7920 6f6e 650a 2020 2020 2020   only one.      
+00002b30: 2020 7a25 5061 7573 696e 6720 616c 6c20    z%Pausing all 
+00002b40: 6d6f 6e6f 6361 6c69 6272 6174 6f72 206c  monocalibrator l
+00002b50: 6f6f 7069 6e67 2e2e 2e4e 2905 7254 0000  ooping...N).rT..
+00002b60: 0072 5500 0000 7232 0000 0072 3e00 0000  .rU...r2...r>...
+00002b70: 5a15 756e 7375 6273 6372 6962 655f 746f  Z.unsubscribe_to
+00002b80: 5f73 7472 6561 6d29 0372 3b00 0000 7244  _stream).r;...rD
+00002b90: 0000 0072 4700 0000 7225 0000 0072 2500  ...rG...r%...r%.
+00002ba0: 0000 7226 0000 0072 6000 0000 a301 0000  ..r&...r`.......
+00002bb0: 7308 0000 000a 0512 010a 0104 ff7a 2153  s............z!S
+00002bc0: 6573 7369 6f6e 2e70 6175 7365 5f61 6c6c  ession.pause_all
+00002bd0: 5f6d 6f6e 6f63 616c 6962 7261 746f 7273  _monocalibrators
+00002be0: 46da 1564 6573 7469 6e61 7469 6f6e 5f64  F..destination_d
+00002bf0: 6972 6563 746f 7279 da13 7374 6f72 655f  irectory..store_
+00002c00: 706f 696e 745f 6869 7374 6f72 7963 0300  point_historyc..
+00002c10: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00002c20: 0000 4300 0000 733e 0000 0074 00a0 0164  ..C...s>...t...d
+00002c30: 01a1 0101 007c 016a 0264 0264 0264 038d  .....|.j.d.d.d..
+00002c40: 0201 0074 037c 006a 0483 017c 005f 057c  ...t.|.j...|._.|
+00002c50: 006a 056a 067c 017c 0264 048d 0201 0064  .j.j.|.|.d.....d
+00002c60: 027c 005f 0764 0053 0029 054e 7a17 496e  .|._.d.S.).Nz.In
+00002c70: 6974 6961 7469 6e67 2072 6563 6f72 6469  itiating recordi
+00002c80: 6e67 2e2e 2e54 2902 da07 7061 7265 6e74  ng...T)...parent
+00002c90: 73da 0865 7869 7374 5f6f 6b29 0172 8900  s..exist_ok).r..
+00002ca0: 0000 2908 7254 0000 0072 5500 0000 da05  ..).rT...rU.....
+00002cb0: 6d6b 6469 7272 1700 0000 7241 0000 00da  mkdirr....rA....
+00002cc0: 0e76 6964 656f 5f72 6563 6f72 6465 72da  .video_recorder.
+00002cd0: 0f73 7461 7274 5f72 6563 6f72 6469 6e67  .start_recording
+00002ce0: 7237 0000 0029 0372 3b00 0000 7288 0000  r7...).r;...r...
+00002cf0: 0072 8900 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+00002d00: 7226 0000 0072 8e00 0000 ac01 0000 730e  r&...r........s.
+00002d10: 0000 000a 030e 010c 0206 0104 0106 ff0a  ................
+00002d20: 037a 1753 6573 7369 6f6e 2e73 7461 7274  .z.Session.start
+00002d30: 5f72 6563 6f72 6469 6e67 6301 0000 0000  _recordingc.....
+00002d40: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00002d50: 0000 0073 6a00 0000 7400 a001 6401 a101  ...sj...t...d...
+00002d60: 0100 7c00 6a02 a003 a100 0100 7c00 6a02  ..|.j.......|.j.
+00002d70: 6a04 721b 7400 a001 6402 a101 0100 7405  j.r.t...d.....t.
+00002d80: 6403 8301 0100 7c00 6a02 6a04 730e 6404  d.....|.j.j.s.d.
+00002d90: 7c00 5f06 7400 a001 6405 a101 0100 7c00  |._.t...d.....|.
+00002da0: 6a07 a008 a100 0100 7c00 a009 a100 7233  j.......|.....r3
+00002db0: 7c00 6a0a a008 a100 0100 6400 5300 6400  |.j.......d.S.d.
+00002dc0: 5300 2906 4e7a 1553 746f 7070 696e 6720  S.).Nz.Stopping 
+00002dd0: 7265 636f 7264 696e 672e 2e2e 7a2e 5761  recording...z.Wa
+00002de0: 6974 696e 6720 666f 7220 7669 6465 6f20  iting for video 
+00002df0: 7265 636f 7264 6572 2074 6f20 7361 7665  recorder to save
+00002e00: 206f 7574 2064 6174 612e 2e2e 6700 0000   out data...g...
+00002e10: 0000 00e0 3f46 7a3d 5265 636f 7264 696e  ....?Fz=Recordin
+00002e20: 6720 6f66 2066 7261 6d65 7320 6973 2063  g of frames is c
+00002e30: 6f6d 706c 6574 652e 2e2e 7369 676e 616c  omplete...signal
+00002e40: 6c69 6e67 2063 6861 6e67 6520 696e 2073  ling change in s
+00002e50: 7461 7475 7329 0b72 5400 0000 7255 0000  tatus).rT...rU..
+00002e60: 0072 8d00 0000 da0e 7374 6f70 5f72 6563  .r......stop_rec
+00002e70: 6f72 6469 6e67 5a09 7265 636f 7264 696e  ordingZ.recordin
+00002e80: 6772 0600 0000 7237 0000 00da 1972 6563  gr....r7.....rec
+00002e90: 6f72 6469 6e67 5f63 6f6d 706c 6574 655f  ording_complete_
+00002ea0: 7369 676e 616c 7243 0000 0072 5d00 0000  signalrC...r]...
+00002eb0: da15 756e 6c6f 636b 5f70 6f73 7470 726f  ..unlock_postpro
+00002ec0: 6365 7373 696e 6772 6d00 0000 7225 0000  cessingrm...r%..
+00002ed0: 0072 2500 0000 7226 0000 0072 8f00 0000  .r%...r&...r....
+00002ee0: b801 0000 7318 0000 000a 010a 0108 010a  ....s...........
+00002ef0: 0108 0108 fe06 040a 020a 0108 020e 0104  ................
+00002f00: ff7a 1653 6573 7369 6f6e 2e73 746f 705f  .z.Session.stop_
+00002f10: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
+00002f20: 0000 0000 0000 0400 0000 0800 0000 0300  ................
+00002f30: 0000 7354 0000 0087 0066 0164 0164 0284  ..sT.....f.d.d..
+00002f40: 087d 0174 0083 008f 177d 0288 006a 01a0  .}.t.....}...j..
+00002f50: 02a1 0044 005d 087d 037c 02a0 037c 017c  ...D.].}.|...|.|
+00002f60: 03a1 0201 0071 0f57 0064 0304 0004 0083  .....q.W.d......
+00002f70: 0301 0064 0353 0031 0073 2377 0101 0001  ...d.S.1.s#w....
+00002f80: 0001 0059 0001 0064 0353 0029 047a 8243  ...Y...d.S.).z.C
+00002f90: 6861 6e67 6573 2074 6865 2063 616d 6572  hanges the camer
+00002fa0: 6120 7265 736f 6c75 7469 6f6e 2074 6f20  a resolution to 
+00002fb0: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
+00002fc0: 2063 6f6e 6669 6775 7261 7469 6f6e 2c20   configuration, 
+00002fd0: 6173 0a20 2020 2020 2020 206c 6f67 2061  as.        log a
+00002fe0: 7320 6974 2069 7320 6e6f 7420 636f 6e66  s it is not conf
+00002ff0: 6967 7572 6564 2066 6f72 2074 6865 2064  igured for the d
+00003000: 6566 6175 6c74 2072 6573 6f6c 7574 696f  efault resolutio
+00003010: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
+00003020: 0000 0a00 0000 1300 0000 73b6 0000 0088  ..........s.....
+00003030: 006a 007c 0019 007d 0188 006a 016a 0264  .j.|...}...j.j.d
+00003040: 017c 009b 009d 0219 0064 0219 007d 0288  .|.......d...}..
+00003050: 006a 037c 0019 006a 047d 037c 0264 0319  .j.|...j.}.|.d..
+00003060: 007c 0364 0319 006b 0373 267c 0264 0419  .|.d...k.s&|.d..
+00003070: 007c 0364 0419 006b 0372 5974 05a0 0664  .|.d...k.rYt...d
+00003080: 057c 009b 0064 067c 0364 0364 0785 0219  .|...d.|.d.d....
+00003090: 009b 0064 087c 0264 0364 0785 0219 009b  ...d.|.d.d......
+000030a0: 009d 06a1 0101 007c 01a0 077c 02a1 0101  .......|...|....
+000030b0: 0074 05a0 0664 097c 009b 0064 067c 0364  .t...d.|...d.|.d
+000030c0: 0364 0785 0219 009b 0064 087c 0264 0364  .d.......d.|.d.d
+000030d0: 0785 0219 009b 009d 06a1 0101 0064 0053  .............d.S
+000030e0: 0064 0053 0029 0a4e 5a04 6361 6d5f da04  .d.S.).NZ.cam_..
+000030f0: 7369 7a65 7201 0000 0072 7000 0000 7a27  sizer....rp...z'
+00003100: 4265 6769 6e6e 696e 6720 746f 2063 6861  Beginning to cha
+00003110: 6e67 6520 7265 736f 6c75 7469 6f6e 2061  nge resolution a
+00003120: 7420 706f 7274 207a 0620 6672 6f6d 2072  t port z. from r
+00003130: 5100 0000 7a04 2074 6f20 7a27 436f 6d70  Q...z. to z'Comp
+00003140: 6c65 7465 6420 6368 616e 6765 206f 6620  leted change of 
+00003150: 7265 736f 6c75 7469 6f6e 2061 7420 706f  resolution at po
+00003160: 7274 2029 0872 2f00 0000 7228 0000 0072  rt ).r/...r(...r
+00003170: 7100 0000 722e 0000 005a 1264 6566 6175  q...r....Z.defau
+00003180: 6c74 5f72 6573 6f6c 7574 696f 6e72 5400  lt_resolutionrT.
+00003190: 0000 7255 0000 005a 1163 6861 6e67 655f  ..rU...Z.change_
+000031a0: 7265 736f 6c75 7469 6f6e 2904 7244 0000  resolution).rD..
+000031b0: 0072 4500 0000 7292 0000 005a 0c64 6566  .rE...r....Z.def
+000031c0: 6175 6c74 5f73 697a 6572 6d00 0000 7225  ault_sizerm...r%
+000031d0: 0000 0072 2600 0000 da11 6164 6a75 7374  ...r&.....adjust
+000031e0: 5f72 6573 5f77 6f72 6b65 72cb 0100 0073  _res_worker....s
+000031f0: 1800 0000 0a01 1601 0c01 2002 0401 2401  .......... ...$.
+00003200: 04ff 0a03 0401 2401 08ff 04fb 7a36 5365  ......$.....z6Se
+00003210: 7373 696f 6e2e 5f61 646a 7573 745f 7265  ssion._adjust_re
+00003220: 736f 6c75 7469 6f6e 732e 3c6c 6f63 616c  solutions.<local
+00003230: 733e 2e61 646a 7573 745f 7265 735f 776f  s>.adjust_res_wo
+00003240: 726b 6572 4e29 0472 0400 0000 722e 0000  rkerN).r....r...
+00003250: 0072 7d00 0000 727e 0000 0029 0472 3b00  .r}...r~...).r;.
+00003260: 0000 7293 0000 0072 7f00 0000 7244 0000  ..r....r....rD..
+00003270: 0072 2500 0000 726d 0000 0072 2600 0000  .r%...rm...r&...
+00003280: 7282 0000 00c7 0100 0073 0c00 0000 0c04  r........s......
+00003290: 080e 0e01 0e01 02ff 22ff 7a1b 5365 7373  ........".z.Sess
+000032a0: 696f 6e2e 5f61 646a 7573 745f 7265 736f  ion._adjust_reso
+000032b0: 6c75 7469 6f6e 7363 0100 0000 0000 0000  lutionsc........
+000032c0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+000032d0: 737a 0000 007c 006a 00a0 01a1 007c 005f  sz...|.j.....|._
+000032e0: 027c 006a 00a0 03a1 007c 005f 0474 057c  .|.j.....|._.t.|
+000032f0: 006a 047c 006a 0283 027c 005f 067c 006a  .j.|.j...|._.|.j
+00003300: 006a 0764 0119 0064 0219 007c 006a 065f  .j.d...d...|.j._
+00003310: 0864 037c 006a 006a 0764 0119 00a0 09a1  .d.|.j.j.d......
+00003320: 0076 0072 327c 006a 006a 0764 0119 0064  .v.r2|.j.j.d...d
+00003330: 0319 007c 006a 065f 0a74 0b7c 006a 067c  ...|.j._.t.|.j.|
+00003340: 006a 0c64 048d 027c 005f 0d64 0553 0029  .j.d...|._.d.S.)
+00003350: 067a f30a 2020 2020 2020 2020 466f 6c6c  .z..        Foll
+00003360: 6f77 696e 6720 6361 7074 7572 6520 766f  owing capture vo
+00003370: 6c75 6d65 206f 7074 696d 697a 6174 696f  lume optimizatio
+00003380: 6e20 7669 6120 6275 6e64 6c65 2061 646a  n via bundle adj
+00003390: 7573 746d 656e 742c 206f 7220 616c 7465  ustment, or alte
+000033a0: 7261 7469 6f6e 0a20 2020 2020 2020 2076  ration.        v
+000033b0: 6961 2061 2074 7261 6e73 666f 726d 206f  ia a transform o
+000033c0: 6620 7468 6520 6f72 6967 696e 2c20 7468  f the origin, th
+000033d0: 6520 656e 7469 7265 2063 6170 7475 7265  e entire capture
+000033e0: 2076 6f6c 756d 6520 6361 6e20 6265 2072   volume can be r
+000033f0: 656c 6f61 6465 640a 2020 2020 2020 2020  eloaded.        
+00003400: 6672 6f6d 2074 6865 2063 6f6e 6669 6720  from the config 
+00003410: 6461 7461 2077 6974 686f 7574 206e 6565  data without nee
+00003420: 6469 6e67 2074 6f20 676f 2074 6872 6f75  ding to go throu
+00003430: 6768 2074 6865 2073 7465 7073 0a0a 2020  gh the steps..  
+00003440: 2020 2020 2020 da0e 6361 7074 7572 655f        ..capture_
+00003450: 766f 6c75 6d65 da05 7374 6167 65da 116f  volume..stage..o
+00003460: 7269 6769 6e5f 7379 6e63 5f69 6e64 6578  rigin_sync_index
+00003470: 2901 7238 0000 004e 290e 7228 0000 0072  ).r8...N).r(...r
+00003480: 1400 0000 da0f 706f 696e 745f 6573 7469  ......point_esti
+00003490: 6d61 7465 7372 4d00 0000 724e 0000 0072  matesrM...rN...r
+000034a0: 1100 0000 7294 0000 0072 7100 0000 7295  ....r....rq...r.
+000034b0: 0000 0072 7d00 0000 7296 0000 0072 1200  ...r}...r....r..
+000034c0: 0000 7238 0000 00da 1271 7561 6c69 7479  ..r8.....quality
+000034d0: 5f63 6f6e 7472 6f6c 6c65 7272 6d00 0000  _controllerrm...
+000034e0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+000034f0: 1d6c 6f61 645f 6573 7469 6d61 7465 645f  .load_estimated_
+00003500: 6361 7074 7572 655f 766f 6c75 6d65 dd01  capture_volume..
+00003510: 0000 7316 0000 000c 070c 0110 0114 0214  ..s.............
+00003520: 010a 0102 0108 ff02 0508 010c ff7a 2553  .............z%S
+00003530: 6573 7369 6f6e 2e6c 6f61 645f 6573 7469  ession.load_esti
+00003540: 6d61 7465 645f 6361 7074 7572 655f 766f  mated_capture_vo
+00003550: 6c75 6d65 6301 0000 0000 0000 0000 0000  lumec...........
+00003560: 0002 0000 0005 0000 0043 0000 0073 a600  .........C...s..
+00003570: 0000 7400 7c00 6a01 6a02 7c00 6a03 8302  ..t.|.j.j.|.j...
+00003580: 7d01 7c01 6a04 6401 6402 8d01 0100 7405  }.|.j.d.d.....t.
+00003590: 7c00 6a01 6a02 8301 a006 a100 7c00 5f07  |.j.j.......|._.
+000035a0: 7408 7c00 6a07 7c00 6a03 8302 7c00 5f09  t.|.j.|.j...|._.
+000035b0: 740a 7c00 6a07 7c00 6a09 8302 7c00 5f0b  t.|.j.|.j...|._.
+000035c0: 7c00 6a0b a00c a100 0100 740d 7c00 6a0b  |.j.......t.|.j.
+000035d0: 7c00 6a0e 8302 7c00 5f0f 7410 a011 6403  |.j...|._.t...d.
+000035e0: 7412 6404 1400 9b00 6405 9d03 a101 0100  t.d.....d.......
+000035f0: 7c00 6a0f a013 7412 a101 0100 7c00 6a0b  |.j...t.....|.j.
+00003600: a00c a100 0100 7c00 6a01 a014 7c00 6a0b  ......|.j...|.j.
+00003610: a101 0100 6406 5300 2907 7ad7 0a20 2020  ....d.S.).z..   
+00003620: 2020 2020 2054 6869 7320 6973 2077 6865       This is whe
+00003630: 7265 2074 6865 2063 616d 6572 6120 6172  re the camera ar
+00003640: 7261 7920 3620 446f 4620 6973 2073 6574  ray 6 DoF is set
+00003650: 2e20 4d61 6e79 2c20 6d61 6e79 2074 6869  . Many, many thi
+00003660: 6e67 7320 6172 6520 6861 7070 656e 696e  ngs are happenin
+00003670: 670a 2020 2020 2020 2020 6865 7265 2c20  g.        here, 
+00003680: 6275 7420 7468 6579 2061 7265 2061 6c6c  but they are all
+00003690: 206e 6563 6573 7361 7279 2073 7465 7073   necessary steps
+000036a0: 206f 6620 7468 6520 7072 6f63 6573 7320   of the process 
+000036b0: 736f 2049 2064 6964 6e27 7420 7761 6e74  so I didn't want
+000036c0: 2074 6f0a 2020 2020 2020 2020 7472 7920   to.        try 
+000036d0: 746f 2065 6e63 6170 7375 6c61 7465 2061  to encapsulate a
+000036e0: 6e79 2066 7572 7468 6572 0a20 2020 2020  ny further.     
+000036f0: 2020 2072 1800 0000 2901 5a0e 626f 6172     r....).Z.boar
+00003700: 6473 5f73 616d 706c 6564 7a1b 5265 6d6f  ds_sampledz.Remo
+00003710: 7669 6e67 2074 6865 2077 6f72 7374 2066  ving the worst f
+00003720: 6974 7469 6e67 20e9 6400 0000 7a21 2070  itting .d...z! p
+00003730: 6572 6365 6e74 206f 6620 706f 696e 7473  ercent of points
+00003740: 2066 726f 6d20 7468 6520 6d6f 6465 6c4e   from the modelN
+00003750: 2915 720f 0000 0072 2800 0000 5a09 746f  ).r....r(...Z.to
+00003760: 6d6c 5f70 6174 6872 2d00 0000 5a14 7374  ml_pathr-...Z.st
+00003770: 6572 656f 5f63 616c 6962 7261 7465 5f61  ereo_calibrate_a
+00003780: 6c6c 720d 0000 005a 1567 6574 5f62 6573  llr....Z.get_bes
+00003790: 745f 6361 6d65 7261 5f61 7272 6179 724e  t_camera_arrayrN
+000037a0: 0000 0072 1400 0000 7297 0000 0072 1100  ...r....r....r..
+000037b0: 0000 7294 0000 00da 086f 7074 696d 697a  ..r......optimiz
+000037c0: 6572 1200 0000 7238 0000 0072 9800 0000  er....r8...r....
+000037d0: 7254 0000 0072 5500 0000 da11 4649 4c54  rT...rU.....FILT
+000037e0: 4552 4544 5f46 5241 4354 494f 4e5a 1666  ERED_FRACTIONZ.f
+000037f0: 696c 7465 725f 706f 696e 745f 6573 7469  ilter_point_esti
+00003800: 6d61 7465 735a 1373 6176 655f 6361 7074  matesZ.save_capt
+00003810: 7572 655f 766f 6c75 6d65 2902 723b 0000  ure_volume).r;..
+00003820: 005a 1073 7465 7265 6f63 616c 6962 7261  .Z.stereocalibra
+00003830: 746f 7272 2500 0000 7225 0000 0072 2600  torr%...r%...r&.
+00003840: 0000 da13 6573 7469 6d61 7465 5f65 7874  ....estimate_ext
+00003850: 7269 6e73 6963 73f3 0100 0073 2a00 0000  rinsics....s*...
+00003860: 0206 0a01 04ff 0c03 0202 0601 02ff 0402  ................
+00003870: 04fe 0204 0801 06ff 1004 0a01 1002 0402  ................
+00003880: 0e01 04ff 0c03 0a01 1202 7a1b 5365 7373  ..........z.Sess
+00003890: 696f 6e2e 6573 7469 6d61 7465 5f65 7874  ion.estimate_ext
+000038a0: 7269 6e73 6963 7372 6a00 0000 2901 4629  rinsicsrj...).F)
+000038b0: 2972 1b00 0000 721c 0000 0072 1d00 0000  )r....r....r....
+000038c0: 7203 0000 0072 8500 0000 7242 0000 0072  r....r....rB...r
+000038d0: 9100 0000 7290 0000 0072 1900 0000 5a13  ....r....r....Z.
+000038e0: 6d6f 6465 5f63 6861 6e67 655f 7375 6363  mode_change_succ
+000038f0: 6573 7372 1500 0000 722a 0000 0072 4800  essr....r*...rH.
+00003900: 0000 724b 0000 0072 5000 0000 7257 0000  ..rK...rP...rW..
+00003910: 0072 5900 0000 725d 0000 0072 6600 0000  .rY...r]...rf...
+00003920: da03 696e 7472 6800 0000 726b 0000 0072  ..intrh...rk...r
+00003930: 5e00 0000 da04 626f 6f6c 7263 0000 0072  ^.....boolrc...r
+00003940: 6200 0000 726e 0000 0072 6f00 0000 7277  b...rn...ro...rw
+00003950: 0000 0072 8100 0000 7261 0000 0072 8300  ...r....ra...r..
+00003960: 0000 7264 0000 0072 6000 0000 7205 0000  ..rd...r`...r...
+00003970: 0072 8e00 0000 728f 0000 0072 8200 0000  .r....r....r....
+00003980: 7299 0000 0072 9d00 0000 da0d 5f5f 636c  r....r......__cl
+00003990: 6173 7363 656c 6c5f 5f72 2500 0000 7225  asscell__r%...r%
+000039a0: 0000 0072 3c00 0000 7226 0000 0072 2700  ...r<...r&...r'.
+000039b0: 0000 3000 0000 734a 0000 0008 0006 0106  ..0...sJ........
+000039c0: 0106 0106 0108 0212 0208 2208 1208 0708  ..........".....
+000039d0: 0b08 1d08 1e0e 0d0e 380e 1608 0f0e 0608  ........8.......
+000039e0: 0408 0608 0408 0408 0708 2308 2610 0b08  ..........#.&...
+000039f0: 0d02 0a04 ff02 0102 ff02 010a ff08 0c08  ................
+00003a00: 0f08 1610 1672 2700 0000 2933 da0d 7079  .....r'...)3..py
+00003a10: 7879 3364 2e6c 6f67 6765 72da 0670 7978  xy3d.logger..pyx
+00003a20: 7933 6472 5400 0000 da03 6765 7472 1b00  y3drT.....getr..
+00003a30: 0000 da0c 5079 5174 362e 5174 436f 7265  ....PyQt6.QtCore
+00003a40: 7202 0000 0072 0300 0000 5a12 636f 6e63  r....r....Z.conc
+00003a50: 7572 7265 6e74 2e66 7574 7572 6573 7204  urrent.futuresr.
+00003a60: 0000 00da 0770 6174 686c 6962 7205 0000  .....pathlibr...
+00003a70: 00da 0474 696d 6572 0600 0000 da04 656e  ...timer......en
+00003a80: 756d 7207 0000 0072 0800 0000 5a1f 7079  umr....r....Z.py
+00003a90: 7879 3364 2e74 7261 636b 6572 732e 6368  xy3d.trackers.ch
+00003aa0: 6172 7563 6f5f 7472 6163 6b65 7272 0900  aruco_trackerr..
+00003ab0: 0000 5a21 7079 7879 3364 2e63 616c 6962  ..Z!pyxy3d.calib
+00003ac0: 7261 7469 6f6e 2e6d 6f6e 6f63 616c 6962  ration.monocalib
+00003ad0: 7261 746f 7272 0a00 0000 5a15 7079 7879  ratorr....Z.pyxy
+00003ae0: 3364 2e63 616d 6572 6173 2e63 616d 6572  3d.cameras.camer
+00003af0: 6172 0b00 0000 5a1b 7079 7879 3364 2e63  ar....Z.pyxy3d.c
+00003b00: 616d 6572 6173 2e73 796e 6368 726f 6e69  ameras.synchroni
+00003b10: 7a65 7272 0c00 0000 5a27 7079 7879 3364  zerr....Z'pyxy3d
+00003b20: 2e63 616d 6572 6173 2e63 616d 6572 615f  .cameras.camera_
+00003b30: 6172 7261 795f 696e 6974 6961 6c69 7a65  array_initialize
+00003b40: 7272 0d00 0000 5a10 7079 7879 3364 2e69  rr....Z.pyxy3d.i
+00003b50: 6e74 6572 6661 6365 720e 0000 005a 2370  nterfacer....Z#p
+00003b60: 7978 7933 642e 6361 6c69 6272 6174 696f  yxy3d.calibratio
+00003b70: 6e2e 7374 6572 656f 6361 6c69 6272 6174  n.stereocalibrat
+00003b80: 6f72 720f 0000 005a 3170 7978 7933 642e  orr....Z1pyxy3d.
+00003b90: 6361 6c69 6272 6174 696f 6e2e 6361 7074  calibration.capt
+00003ba0: 7572 655f 766f 6c75 6d65 2e70 6f69 6e74  ure_volume.point
+00003bb0: 5f65 7374 696d 6174 6573 7210 0000 005a  _estimatesr....Z
+00003bc0: 3070 7978 7933 642e 6361 6c69 6272 6174  0pyxy3d.calibrat
+00003bd0: 696f 6e2e 6361 7074 7572 655f 766f 6c75  ion.capture_volu
+00003be0: 6d65 2e63 6170 7475 7265 5f76 6f6c 756d  me.capture_volum
+00003bf0: 6572 1100 0000 5a34 7079 7879 3364 2e63  er....Z4pyxy3d.c
+00003c00: 616c 6962 7261 7469 6f6e 2e63 6170 7475  alibration.captu
+00003c10: 7265 5f76 6f6c 756d 652e 7175 616c 6974  re_volume.qualit
+00003c20: 795f 636f 6e74 726f 6c6c 6572 7212 0000  y_controllerr...
+00003c30: 005a 1b70 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
+00003c40: 732e 6361 6d65 7261 5f61 7272 6179 7213  s.camera_arrayr.
+00003c50: 0000 005a 4670 7978 7933 642e 6361 6c69  ...ZFpyxy3d.cali
+00003c60: 6272 6174 696f 6e2e 6361 7074 7572 655f  bration.capture_
+00003c70: 766f 6c75 6d65 2e68 656c 7065 725f 6675  volume.helper_fu
+00003c80: 6e63 7469 6f6e 732e 6765 745f 706f 696e  nctions.get_poin
+00003c90: 745f 6573 7469 6d61 7465 7372 1400 0000  t_estimatesr....
+00003ca0: da13 7079 7879 3364 2e63 6f6e 6669 6775  ..pyxy3d.configu
+00003cb0: 7261 746f 7272 1500 0000 5a1a 7079 7879  ratorr....Z.pyxy
+00003cc0: 3364 2e63 616d 6572 6173 2e6c 6976 655f  3d.cameras.live_
+00003cd0: 7374 7265 616d 7216 0000 005a 1f70 7978  streamr....Z.pyx
+00003ce0: 7933 642e 7265 636f 7264 696e 672e 7669  y3d.recording.vi
+00003cf0: 6465 6f5f 7265 636f 7264 6572 7217 0000  deo_recorderr...
+00003d00: 0072 7c00 0000 729c 0000 0072 1900 0000  .r|...r....r....
+00003d10: 7227 0000 0072 2500 0000 7225 0000 0072  r'...r%...r%...r
+00003d20: 2500 0000 7226 0000 00da 083c 6d6f 6475  %...r&.....<modu
+00003d30: 6c65 3e01 0000 0073 3400 0000 0801 0c02  le>....s4.......
+00003d40: 1002 0c01 0c01 0c01 1001 0c02 0c01 0c01  ................
+00003d50: 0c01 0c01 0c01 0c02 0c01 0c01 0c01 0c02  ................
+00003d60: 0c01 0c03 0c01 0c01 0403 0401 1003 140b  ................
```

### Comparing `pyxy3d-0.0.20/pyxy3d/session/session.py` & `pyxy3d-0.0.21/pyxy3d/session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,25 +180,25 @@
         else:
             eligible = False
 
         return eligible
 
     def is_post_processing_eligible(self):
         """
-        Post processing can only be performed if recordings exist and extrinsics are calibrated
+        Post processing can only be performed if recordings (mp4 files) exist and extrinsics 
+        (config.toml) are calibrated in the 'record' directory
         """
-        # the presence of these does not count as a recording
-        excluded_items = ["calibration", "config.toml"]
-
-        folders = [f for f in self.path.iterdir() if f.name not in excluded_items]
-        recording_count = len(folders)
-        if recording_count > 0:
-            eligible = True
-        else:
-            eligible = False
+        #assume false and prove otherwise
+        eligible = False
+        for child in self.path.iterdir():
+            if child.is_dir():
+                mp4_files = list(child.glob('*.mp4'))
+                config_file = child / 'config.toml'
+                if mp4_files and config_file.exists():
+                    eligible=True
 
         return eligible
 
     def set_mode(self, mode: SessionMode):
         """
         Via this method, the frame reading behavior will be changed by the GUI. If some properties are
         not available (i.e. synchronizer) they will be created
```

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.0.21/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.0.21/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/helper.py` & `pyxy3d-0.0.21/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.0.21/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.0.21/pyxy3d/trackers/holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.0.21/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.0.21/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc` & `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.0.21/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.0.21/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.0.21/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/README.md` & `pyxy3d-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.20/PKG-INFO` & `pyxy3d-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.0.20
+Version: 0.0.21
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

