# Comparing `tmp/pyaogmaneo-2.0.4.tar.gz` & `tmp/pyaogmaneo-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.0.4.tar", last modified: Thu Apr 27 21:18:55 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.0.5.tar", last modified: Mon Jun 12 22:04:58 2023, max compression
```

## Comparing `pyaogmaneo-2.0.4.tar` & `pyaogmaneo-2.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.4/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-04-27 21:17:42.000000 pyaogmaneo-2.0.4/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.4/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.4/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-03-26 23:58:01.000000 pyaogmaneo-2.0.4/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-04-27 21:18:55.000000 pyaogmaneo-2.0.4/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.4/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-04-27 21:16:13.000000 pyaogmaneo-2.0.4/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-04-27 21:18:55.268853 pyaogmaneo-2.0.4/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-03-26 23:58:01.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-03-26 23:58:01.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     9352 2023-04-23 00:53:41.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     6430 2023-04-27 21:16:02.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     5920 2023-04-22 23:35:15.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3029 2023-04-27 21:15:53.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8641 2023-04-27 19:20:12.000000 pyaogmaneo-2.0.4/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.5/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-12 22:02:11.000000 pyaogmaneo-2.0.5/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.5/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.5/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-05-18 17:15:10.000000 pyaogmaneo-2.0.5/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-12 22:04:58.000000 pyaogmaneo-2.0.5/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.5/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-12 22:01:38.000000 pyaogmaneo-2.0.5/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.814855 pyaogmaneo-2.0.5/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-12 22:04:58.818188 pyaogmaneo-2.0.5/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-09 23:28:26.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-09 23:43:55.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-12 02:04:51.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-12 22:02:24.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8183 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-12 22:02:33.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8963 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.5/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.0.4/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.0.5/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.4/CMakeLists.txt` & `pyaogmaneo-2.0.5/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 7332a07731274779cf476b5810101f5aec2d20a3
+        GIT_TAG 39b1c24a17f0330b44b4194f084086378115f8fc
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.0.4/LICENSE.md` & `pyaogmaneo-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.4/PKG-INFO` & `pyaogmaneo-2.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.4/README.md` & `pyaogmaneo-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.4/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.0.5/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.4/setup.py` & `pyaogmaneo-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.0.4",
+    version="2.0.5",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.4/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.0.5/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.4/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.0.5/source/pyaogmaneo/py_hierarchy.h`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace pyaon {
-const int hierarchy_magic = 1188221;
+const int hierarchy_magic = 1138225;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
 
@@ -139,14 +139,19 @@
         int i
     ) const;
 
     std::vector<float> get_prediction_acts(
         int i
     ) const;
 
+    std::vector<int> sample_prediction(
+        int i,
+        float temperature
+    ) const;
+
     std::vector<int> get_hidden_cis(
         int l
     ) {
         if (l < 0 || l >= h.get_num_layers())
             throw std::runtime_error("error: " + std::to_string(l) + " is not a valid layer index!");
 
         std::vector<int> hidden_cis(h.get_encoder(l).get_hidden_cis().size());
@@ -249,9 +254,23 @@
         int i
     ) const {
         if (i < 0 || i >= h.get_num_io() || h.get_io_type(i) != aon::action)
             throw std::runtime_error("error: " + std::to_string(i) + " is not a valid input index!");
 
         return h.get_actor(i).get_history_capacity();
     }
+
+    // for visualization mostly
+    std::tuple<std::vector<float>, std::tuple<int, int, int>> get_encoder_receptive_field(
+        int l,
+        int i,
+        const std::tuple<int, int, int> &cell_pos
+    );
+
+    std::tuple<std::vector<float>, std::tuple<int, int, int>> get_decoder_receptive_field(
+        int l,
+        int i,
+        bool feedback,
+        const std::tuple<int, int, int> &cell_pos
+    );
 };
 }
```

### Comparing `pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -167,7 +167,59 @@
             throw std::runtime_error("recon csdr (recon_cis) has an out-of-bounds column index (" + std::to_string(recon_cis[j]) + ") at column index " + std::to_string(j) + ". it must be in the range [0, " + std::to_string(enc.get_hidden_size().z - 1) + "]");
 
         c_recon_cis_backing[j] = recon_cis[j];
     }
 
     enc.reconstruct(&c_recon_cis_backing);
 }
+
+std::tuple<std::vector<float>, std::tuple<int, int, int>> Image_Encoder::get_receptive_field(
+    int i,
+    const std::tuple<int, int, int> &cell_pos
+) {
+    assert(i >= 0 && i < enc.get_num_visible_layers());
+
+    const aon::Int3 &hidden_size = enc.get_hidden_size();
+
+    const aon::Image_Encoder::Visible_Layer &vl = enc.get_visible_layer(i);
+    const aon::Image_Encoder::Visible_Layer_Desc &vld = enc.get_visible_layer_desc(i);
+
+    int diam = vld.radius * 2 + 1;
+
+    // projection
+    aon::Float2 h_to_v = aon::Float2(static_cast<float>(vld.size.x) / static_cast<float>(hidden_size.x),
+        static_cast<float>(vld.size.y) / static_cast<float>(hidden_size.y));
+
+    aon::Int2 visible_center = project(aon::Int2(std::get<0>(cell_pos), std::get<1>(cell_pos)), h_to_v);
+
+    // lower corner
+    aon::Int2 field_lower_bound(visible_center.x - vld.radius, visible_center.y - vld.radius);
+
+    // bounds of receptive field, clamped to input size
+    aon::Int2 iter_lower_bound(aon::max(0, field_lower_bound.x), aon::max(0, field_lower_bound.y));
+    aon::Int2 iter_upper_bound(aon::min(vld.size.x - 1, visible_center.x + vld.radius), aon::min(vld.size.y - 1, visible_center.y + vld.radius));
+
+    aon::Int3 size(iter_upper_bound.x - iter_lower_bound.x, iter_upper_bound.y - iter_lower_bound.y, vld.size.z);
+
+    int hidden_cell_index = aon::address3(aon::Int3(std::get<0>(cell_pos), std::get<1>(cell_pos), std::get<2>(cell_pos)), hidden_size);
+
+    // get weights
+    std::vector<float> field(size.x * size.y * size.z, 0.0f);
+
+    for (int ix = iter_lower_bound.x; ix <= iter_upper_bound.x; ix++)
+        for (int iy = iter_lower_bound.y; iy <= iter_upper_bound.y; iy++) {
+            aon::Int2 offset(ix - field_lower_bound.x, iy - field_lower_bound.y);
+
+            int wi_start = vld.size.z * (offset.y + diam * (offset.x + diam * hidden_cell_index));
+
+            int field_start = vld.size.z * (offset.y + diam * offset.x);
+
+            for (int vc = 0; vc < vld.size.z; vc++) {
+                float w0 = vl.weights0[vc + wi_start];
+                float w1 = vl.weights1[vc + wi_start];
+
+                field[vc + field_start] = (w0 + w1) * 0.5f;
+            }
+        }
+
+    return std::make_tuple(field, std::make_tuple(size.x, size.y, size.z));
+}
```

### Comparing `pyaogmaneo-2.0.4/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.0.5/source/pyaogmaneo/py_image_encoder.h`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/image_encoder.h>
 
 namespace pyaon {
-const int image_encoder_magic = 6121137;
+const int image_encoder_magic = 2111637;
 
 struct Image_Visible_Layer_Desc {
     std::tuple<int, int, int> size;
 
     int radius;
 
     Image_Visible_Layer_Desc(
@@ -109,9 +109,15 @@
     std::tuple<int, int, int> get_visible_size(
         int i
     ) const {
         aon::Int3 size = enc.get_visible_layer_desc(i).size;
 
         return { size.x, size.y, size.z };
     }
+
+    // for visualization mostly
+    std::tuple<std::vector<float>, std::tuple<int, int, int>> get_receptive_field(
+        int i,
+        const std::tuple<int, int, int> &cell_pos
+    );
 };
 }
```

### Comparing `pyaogmaneo-2.0.4/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.0.5/source/pyaogmaneo/py_module.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -66,27 +66,27 @@
         .def_readwrite("down_radius", &pyaon::Layer_Desc::down_radius)
         .def_readwrite("ticks_per_update", &pyaon::Layer_Desc::ticks_per_update)
         .def_readwrite("temporal_horizon", &pyaon::Layer_Desc::temporal_horizon);
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
-        .def_readwrite("code_iters", &aon::Encoder::Params::code_iters)
         .def_readwrite("lr", &aon::Encoder::Params::lr)
         .def_readwrite("gcurve", &aon::Encoder::Params::gcurve);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
         .def_readwrite("lr", &aon::Decoder::Params::lr)
         .def_readwrite("gcurve", &aon::Decoder::Params::gcurve);
 
     py::class_<aon::Actor::Params>(m, "Actorparams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
         .def_readwrite("alr", &aon::Actor::Params::alr)
+        .def_readwrite("bias", &aon::Actor::Params::bias)
         .def_readwrite("discount", &aon::Actor::Params::discount)
         .def_readwrite("temperature", &aon::Actor::Params::temperature)
         .def_readwrite("min_steps", &aon::Actor::Params::min_steps)
         .def_readwrite("history_iters", &aon::Actor::Params::history_iters);
 
     py::class_<aon::Hierarchy::Layer_Params>(m, "LayerParams")
         .def(py::init<>())
@@ -127,25 +127,28 @@
             py::arg("reward") = 0.0f,
             py::arg("mimic") = 0.0f
         )
         .def("clear_state", &pyaon::Hierarchy::clear_state)
         .def("get_num_layers", &pyaon::Hierarchy::get_num_layers)
         .def("get_prediction_cis", &pyaon::Hierarchy::get_prediction_cis)
         .def("get_prediction_acts", &pyaon::Hierarchy::get_prediction_acts)
+        .def("sample_prediction", &pyaon::Hierarchy::sample_prediction)
         .def("get_hidden_cis", &pyaon::Hierarchy::get_hidden_cis)
         .def("get_hidden_size", &pyaon::Hierarchy::get_hidden_size)
         .def("get_num_encoder_visible_layers", &pyaon::Hierarchy::get_num_encoder_visible_layers)
         .def("get_ticks", &pyaon::Hierarchy::get_ticks)
         .def("get_ticks_per_update", &pyaon::Hierarchy::get_ticks_per_update)
         .def("get_num_io", &pyaon::Hierarchy::get_num_io)
         .def("get_io_size", &pyaon::Hierarchy::get_io_size)
         .def("get_io_type", &pyaon::Hierarchy::get_io_type)
         .def("get_up_radius", &pyaon::Hierarchy::get_up_radius)
         .def("get_down_radius", &pyaon::Hierarchy::get_down_radius)
-        .def("get_actor_history_capacity", &pyaon::Hierarchy::get_actor_history_capacity);
+        .def("get_actor_history_capacity", &pyaon::Hierarchy::get_actor_history_capacity)
+        .def("get_encoder_receptive_field", &pyaon::Hierarchy::get_encoder_receptive_field)
+        .def("get_decoder_receptive_field", &pyaon::Hierarchy::get_decoder_receptive_field);
 
     py::class_<pyaon::Image_Visible_Layer_Desc>(m, "ImageVisibleLayerDesc")
         .def(py::init<
                 std::tuple<int, int, int>,
                 int
             >(),
             py::arg("size") = std::tuple<int, int, int>({ 4, 4, 16 }),
@@ -181,9 +184,10 @@
             py::arg("learn_enabled") = true
         )
         .def("reconstruct", &pyaon::Image_Encoder::reconstruct)
         .def("get_num_visible_layers", &pyaon::Image_Encoder::get_num_visible_layers)
         .def("get_reconstruction", &pyaon::Image_Encoder::get_reconstruction)
         .def("get_hidden_cis", &pyaon::Image_Encoder::get_hidden_cis)
         .def("get_hidden_size", &pyaon::Image_Encoder::get_hidden_size)
-        .def("get_visible_size", &pyaon::Image_Encoder::get_visible_size);
+        .def("get_visible_size", &pyaon::Image_Encoder::get_visible_size)
+        .def("get_receptive_field", &pyaon::Image_Encoder::get_receptive_field);
 }
```

