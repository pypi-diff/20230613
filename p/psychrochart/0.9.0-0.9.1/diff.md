# Comparing `tmp/psychrochart-0.9.0.tar.gz` & `tmp/psychrochart-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.9.0.tar", max compression
+gzip compressed data, was "psychrochart-0.9.1.tar", max compression
```

## Comparing `psychrochart-0.9.0.tar` & `psychrochart-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11085 2023-06-12 15:33:00.015983 psychrochart-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-12 15:33:00.015983 psychrochart-0.9.0/LICENSE
--rw-r--r--   0        0        0     7077 2023-06-12 15:33:00.015983 psychrochart-0.9.0/README.md
--rw-r--r--   0        0        0      739 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/__init__.py
--rw-r--r--   0        0        0      336 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/__main__.py
--rw-r--r--   0        0        0    15270 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart.py
--rw-r--r--   0        0        0     2231 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_entities.py
--rw-r--r--   0        0        0     2157 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3097 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    15847 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chartdata.py
--rw-r--r--   0        0        0    14504 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chartzones.py
--rw-r--r--   0        0        0        0 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/__init__.py
--rw-r--r--   0        0        0     3350 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/annots.py
--rw-r--r--   0        0        0     1246 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/base.py
--rw-r--r--   0        0        0     8656 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/config.py
--rw-r--r--   0        0        0     3945 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/curves.py
--rw-r--r--   0        0        0     5844 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/parsers.py
--rw-r--r--   0        0        0     1909 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/styles.py
--rw-r--r--   0        0        0     1924 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/validators.py
--rw-r--r--   0        0        0    15798 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/plot_logic.py
--rw-r--r--   0        0        0     8135 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/process_logic.py
--rw-r--r--   0        0        0     4631 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/util.py
--rw-r--r--   0        0        0     2222 2023-06-12 15:33:00.031983 psychrochart-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8406 1970-01-01 00:00:00.000000 psychrochart-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11655 2023-06-13 09:33:41.663741 psychrochart-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-06-13 09:33:41.663741 psychrochart-0.9.1/LICENSE
+-rw-r--r--   0        0        0     7883 2023-06-13 09:33:41.663741 psychrochart-0.9.1/README.md
+-rw-r--r--   0        0        0      739 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/__main__.py
+-rw-r--r--   0        0        0    15292 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart.py
+-rw-r--r--   0        0        0     2231 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_entities.py
+-rw-r--r--   0        0        0     2157 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3097 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    15847 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chartdata.py
+-rw-r--r--   0        0        0    18332 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chartzones.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     3298 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     1246 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/base.py
+-rw-r--r--   0        0        0     8674 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/config.py
+-rw-r--r--   0        0        0     3945 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5844 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     2079 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1924 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/validators.py
+-rw-r--r--   0        0        0    16203 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     8135 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     4631 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/util.py
+-rw-r--r--   0        0        0     2222 2023-06-13 09:33:41.675741 psychrochart-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     9212 1970-01-01 00:00:00.000000 psychrochart-0.9.1/PKG-INFO
```

### Comparing `psychrochart-0.9.0/CHANGELOG.md` & `psychrochart-0.9.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.1] - ✨ Add zone kind 'dbt-wmax' with vapour content limit - 2023-06-13
+
+##### Changes
+
+- ✨ Add new kind of overlay **zone 'dbt-wmax'**, to define chart areas delimited between db-temps and absolute humidity values, solving #28
+- 🐛 Enable zones defined by 2 points (assume a rectangle defined by left-bottom/right-top coords)
+- 🐛 Fix logic for plot regeneration, to plot again if config changes _AFTER_ plotting the chart
+- 🐛 Fix ZoneStyle definition when linewidth is 0 and linestyle remains the default (passing inconsistent params to matplotlib)
+
 ## [0.9.0] - ✨ More kinds of chart zones + CSS for SVG styling - 2023-06-12
 
 Define new enclosed areas in chart between constant RH lines and constant volume or enthalpy values,
 and enable full potencial for SVG customization by including CSS and/or `<defs>` inside it.
 
 ##### Changes
```

### Comparing `psychrochart-0.9.0/LICENSE` & `psychrochart-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/README.md` & `psychrochart-0.9.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,28 +27,34 @@
 
 ```shell
 pip install psychrochart
 ```
 
 ## Features
 
-- **SI** units (with temperatures in celsius for better readability).
-- Easy style customization based on [**pydantic**](https://docs.pydantic.dev/latest/) models and config presets for full customization of colors, line styles, line widths, etc..
+- **SI** units (with temperatures in celsius for better readability), with _partial_ compatibility with IP system (imperial units)
+- Easy style customization based on [**pydantic**](https://docs.pydantic.dev/latest/) models and config presets for full customization of **chart limits**, included lines and labels, colors, line styles, line widths, etc..
 - Psychrometric charts within temperature and humidity ratio ranges, for any pressure\*, with:
   - **Saturation line**
   - **Constant RH lines**
   - **Constant enthalpy lines**
   - **Constant wet-bulb temperature lines**
   - **Constant specific volume lines**
   - **Constant dry-bulb temperature lines** (internal orthogonal grid, vertical)
   - **Constant humidity ratio lines** (internal orthogonal grid, horizontal)
-- Plot legend for each family of lines
+- Plot legend for each family of lines, labeled zones and annotations
 - Specify labels for each family of lines
-- **Overlay points, zones, convex hulls, and arrows**
-- **Export SVG, PNG files**
+- Overlay points, arrows, **data-series** (numpy arrays or pandas series), and convex hulls around points
+- Define multiple kinds of **zones limited by psychrometric values**:
+  - 'dbt-rh' for areas between dry-bulb temperature and relative humidity values,
+  - 'enthalpy-rh' for areas between constant enthalpy and relative humidity values
+  - 'volume-rh' for areas between constant volume and relative humidity values
+  - 'dbt-wmax' for an area between dry-bulb temperature and water vapor content values (:= a rectangle cut by the saturation line),
+  - 'xy-points' to define arbitrary closed paths in plot coordinates (dbt, abs humidity)
+- **Export as SVG, PNG files**, or generate dynamic SVGs with extra CSS and <defs> with `chart.make_svg(...)`
 
 > NOTE: The ranges of temperature, humidity and pressure where this library should provide good results are within the normal environments for people to live in.
 >
 > Don't expect right results if doing other type of thermodynamic calculations.
 >
 > ⚠️ **Over saturated water vapor states are not implemented**. This library is intended for HVAC applications only ⚠️
```

### Comparing `psychrochart-0.9.0/psychrochart/__init__.py` & `psychrochart-0.9.1/psychrochart/__init__.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chart.py` & `psychrochart-0.9.1/psychrochart/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,15 @@
     def rendered(self) -> bool:
         """Check if Axes object is assigned."""
         return self._axes is not None
 
     @property
     def axes(self) -> Axes:
         """Return the Axes object plotting the chart if necessary."""
-        self.process_chart()
-        if not self.rendered:
+        if not self.rendered or self.config.has_changed:
             self.plot()
         assert isinstance(self._axes, Axes)
         return self._axes
 
     @property
     def artists(self) -> ChartRegistry:
         """Access to registry of all matplotlib Artists in plot."""
@@ -418,15 +417,15 @@
 
     def make_svg(
         self,
         css_styles: str | Path | None = None,
         svg_definitions: str | None = None,
         **params,
     ) -> str:
-        """Generate chart as SVG and return as text."""
+        """Generate chart as SVG, with optional styling, and return as text."""
         svg_io = StringIO()
         self.save(svg_io, canvas_cls=FigureCanvasSVG, **params)
         svg_io.seek(0)
         return add_styling_to_svg(svg_io.read(), css_styles, svg_definitions)
 
     def close_fig(self) -> None:
         """Close the figure plot."""
```

### Comparing `psychrochart-0.9.0/psychrochart/chart_entities.py` & `psychrochart-0.9.1/psychrochart/chart_entities.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.9.1/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.9.1/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.9.1/psychrochart/chart_styles/default_chart_config.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.9.1/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.9.1/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.9.1/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chartdata.py` & `psychrochart-0.9.1/psychrochart/chartdata.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/chartzones.py` & `psychrochart-0.9.1/psychrochart/chartzones.py`

 * *Files 18% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         list(curve_rh_up) + list(curve_rh_down)[::-1] + [curve_rh_up[0]]
     )
     temps_zone: list[float] = list(temps) + list(temps)[::-1] + [temps[0]]
     return PsychroCurve(
         x_data=np.array(temps_zone),
         y_data=np.array(abs_humid),
         style=zone.style,
-        type_curve="dbt-rh",
+        type_curve=zone.zone_type,
         label=zone.label,
         internal_value=random_internal_value() if zone.label is None else None,
     )
 
 
 def _make_zone_delimited_by_volume_and_rh(
     zone: ChartZone,
@@ -326,14 +326,127 @@
         zone,
         rect_lines=v_lines,
         rh_lines=rh_lines,
         func_dbt_w_to_target=_points_to_volume,
     )
 
 
+def _make_zone_delimited_by_dbt_and_wmax(
+    zone: ChartZone,
+    pressure: float,
+    *,
+    step_temp: float,
+    dbt_min: float,
+    dbt_max: float,
+    w_min: float,
+    w_max: float,
+) -> PsychroCurve | None:
+    assert zone.zone_type == "dbt-wmax"
+    dbt_1, dbt_2 = zone.points_x
+    w_1, w_2 = zone.points_y
+
+    if dbt_1 > dbt_max or dbt_2 < dbt_min or w_1 > w_max or w_2 < w_min:
+        # zone outside limits
+        return None
+
+    w_1 = max(w_1, w_min)
+    w_2 = min(w_2, w_max)
+    dbt_1 = max(dbt_1, dbt_min)
+    dbt_2 = min(dbt_2, dbt_max)
+
+    saturation = make_saturation_line(dbt_1, dbt_2, step_temp, pressure)
+    if saturation.outside_limits(dbt_min, dbt_max, w_min, w_max):
+        # just make a rectangle
+        return PsychroCurve(
+            x_data=np.array([dbt_1, dbt_2]),
+            y_data=np.array([w_1, w_2]),
+            style=zone.style,
+            type_curve=zone.zone_type,
+            label=zone.label,
+            internal_value=w_2,
+        )
+
+    # build path clockwise starting in left bottom corner
+    path_x, path_y = [], []
+    if saturation.y_data[0] < w_1:  # saturation cuts lower w value
+        idx_start = (saturation.y_data > w_1).argmax()
+        t_start, t_end = (
+            saturation.x_data[idx_start - 1],
+            saturation.x_data[idx_start],
+        )
+        w_start, w_end = (
+            saturation.y_data[idx_start - 1],
+            saturation.y_data[idx_start],
+        )
+        t_cut1, _w_cut1 = _crossing_point_between_rect_lines(
+            segment_1_x=(dbt_1, dbt_2),
+            segment_1_y=(w_1, w_1),
+            segment_2_x=(t_start, t_end),
+            segment_2_y=(w_start, w_end),
+        )
+        path_x.append(t_cut1)
+        path_y.append(w_1)
+    else:  # saturation cuts left y-axis
+        idx_start = 0
+        t_cut1, w_cut1 = saturation.x_data[0], saturation.y_data[0]
+
+        path_x.append(dbt_1)
+        path_y.append(w_1)
+        path_x.append(t_cut1)
+        path_y.append(w_cut1)
+
+    if saturation.y_data[-1] < w_2:  # saturation cuts right dbt_2
+        path_x += saturation.x_data[idx_start:].tolist()
+        path_y += saturation.y_data[idx_start:].tolist()
+
+        t_cut2, w_cut2 = saturation.x_data[-1], saturation.y_data[-1]
+        path_x.append(t_cut2)
+        path_y.append(w_cut2)
+    else:  # saturation cuts top w_2
+        idx_end = (saturation.y_data < w_2).argmin()
+        path_x += saturation.x_data[idx_start:idx_end].tolist()
+        path_y += saturation.y_data[idx_start:idx_end].tolist()
+
+        t_start, t_end = (
+            saturation.x_data[idx_end - 1],
+            saturation.x_data[idx_end],
+        )
+        w_start, w_end = (
+            saturation.y_data[idx_end - 1],
+            saturation.y_data[idx_end],
+        )
+        t_cut2, _w_cut2 = _crossing_point_between_rect_lines(
+            segment_1_x=(dbt_1, dbt_2),
+            segment_1_y=(w_2, w_2),
+            segment_2_x=(t_start, t_end),
+            segment_2_y=(w_start, w_end),
+        )
+        path_x.append(t_cut2)
+        path_y.append(w_2)
+
+        path_x.append(dbt_2)
+        path_y.append(w_2)
+
+    path_x.append(dbt_2)
+    path_y.append(w_1)
+
+    # repeat 1st point to close path
+    path_x.append(path_x[0])
+    path_y.append(path_y[0])
+
+    return PsychroCurve(
+        x_data=np.array(path_x),
+        y_data=np.array(path_y),
+        style=zone.style,
+        type_curve=zone.zone_type,
+        label=zone.label,
+        internal_value=w_2,
+    )
+
+
 def make_zone_curve(
     zone_conf: ChartZone,
     *,
     pressure: float,
     step_temp: float,
     dbt_min: float,
     dbt_max: float,
@@ -366,22 +479,34 @@
             step_temp=step_temp,
             dbt_min=dbt_min,
             dbt_max=dbt_max,
             w_min=w_min,
             w_max=w_max,
         )
 
+    if zone_conf.zone_type == "dbt-wmax":
+        # points for zone between abs humid and dbt ranges
+        return _make_zone_delimited_by_dbt_and_wmax(
+            zone_conf,
+            pressure,
+            step_temp=step_temp,
+            dbt_min=dbt_min,
+            dbt_max=dbt_max,
+            w_min=w_min,
+            w_max=w_max,
+        )
+
     # expect points in plot coordinates!
     assert zone_conf.zone_type == "xy-points"
     zone_value = random_internal_value() if zone_conf.label is None else None
     return PsychroCurve(
         x_data=np.array(zone_conf.points_x),
         y_data=np.array(zone_conf.points_y),
         style=zone_conf.style,
-        type_curve="xy-points",
+        type_curve=zone_conf.zone_type,
         label=zone_conf.label,
         internal_value=zone_value,
     )
 
 
 def make_over_saturated_zone(
     saturation: PsychroCurve,
```

### Comparing `psychrochart-0.9.0/psychrochart/models/annots.py` & `psychrochart-0.9.1/psychrochart/models/annots.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     label: str | None = Field(default=None)
     style: dict[str, Any] = Field(default_factory=dict)
 
 
 class ChartSeries(BaseModel):
     """Input model for data-series point array annotation."""
 
-    # TODO fusion with PsychroCurve, + pandas ready
     x_data: np.ndarray
     y_data: np.ndarray
     style: dict[str, Any] = Field(default_factory=dict)
     label: str | None = None
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `psychrochart-0.9.0/psychrochart/models/base.py` & `psychrochart-0.9.1/psychrochart/models/base.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/models/config.py` & `psychrochart-0.9.1/psychrochart/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 _DEFAULT_STYLE_DRY_TEMP = CurveStyle(
     color=[0.855, 0.145, 0.114], linewidth=0.75, linestyle=":"
 )
 _DEFAULT_STYLE_HUMID = CurveStyle(
     color=[0.0, 0.125, 0.376], linewidth=0.75, linestyle=":"
 )
 
-ZoneKind = Literal["dbt-rh", "xy-points", "enthalpy-rh", "volume-rh"]
+ZoneKind = Literal[
+    "dbt-rh", "xy-points", "enthalpy-rh", "volume-rh", "dbt-wmax"
+]
 
 
 class ChartFigure(BaseConfig):
     """Psychrochart settings for matplotlib Figure."""
 
     figsize: tuple[float, float] = Field(default=(16, 9))
     dpi: int = Field(default=150)
```

### Comparing `psychrochart-0.9.0/psychrochart/models/curves.py` & `psychrochart-0.9.1/psychrochart/models/curves.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/models/parsers.py` & `psychrochart-0.9.1/psychrochart/models/parsers.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/models/styles.py` & `psychrochart-0.9.1/psychrochart/models/styles.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,9 +63,12 @@
         extra = Extra.allow
 
     @validator("edgecolor", "facecolor", pre=True, always=True)
     def _color_arr(cls, v, values):
         return parse_color(v)
 
     @root_validator(pre=True)
-    def _remove_aliases(cls, values):
+    def _remove_aliases_and_fix_defaults(cls, values):
+        if values.get("linewidth", 2) == 0:
+            # avoid matplotlib error with inconsistent line parameters
+            values["linestyle"] = "-"
         return reduce_field_abrs(values)
```

### Comparing `psychrochart-0.9.0/psychrochart/models/validators.py` & `psychrochart-0.9.1/psychrochart/models/validators.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/plot_logic.py` & `psychrochart-0.9.1/psychrochart/plot_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,36 +131,45 @@
             ymax,
             curve.x_data,
             curve.y_data,
         )
         return {}
 
     if isinstance(curve.style, ZoneStyle):
-        assert len(curve.y_data) > 2
-        verts = list(zip(curve.x_data, curve.y_data))
-        codes = (
-            [Path.MOVETO]
-            + [Path.LINETO] * (len(curve.y_data) - 2)
-            + [Path.CLOSEPOLY]
-        )
-        path = Path(verts, codes)
-        patch = patches.PathPatch(path, **curve.style.dict())
+        if len(curve.y_data) == 2:  # draw a rectangle!
+            patch = patches.Rectangle(
+                (curve.x_data[0], curve.y_data[0]),
+                width=curve.x_data[1] - curve.x_data[0],
+                height=curve.y_data[1] - curve.y_data[0],
+                **curve.style.dict(),
+            )
+            bbox_p = patch.get_extents()
+        else:
+            assert len(curve.y_data) > 2
+            verts = list(zip(curve.x_data, curve.y_data))
+            codes = (
+                [Path.MOVETO]
+                + [Path.LINETO] * (len(curve.y_data) - 2)
+                + [Path.CLOSEPOLY]
+            )
+            path = Path(verts, codes)
+            patch = patches.PathPatch(path, **curve.style.dict())
+            bbox_p = path.get_extents()
         ax.add_patch(patch)
         gid_zone = make_item_gid(
             "zone",
             family_label=label_prefix or curve.type_curve,
             name=curve.curve_id,
         )
         reg_artist(
             gid_zone,
             patch,
             artists,
         )
         if curve.label is not None:
-            bbox_p = path.get_extents()
             text_x = 0.5 * (bbox_p.x0 + bbox_p.x1)
             text_y = 0.5 * (bbox_p.y0 + bbox_p.y1)
             style_params = {
                 "ha": "center",
                 "va": "center",
                 "backgroundcolor": [1, 1, 1, 0.4],
             }
```

### Comparing `psychrochart-0.9.0/psychrochart/process_logic.py` & `psychrochart-0.9.1/psychrochart/process_logic.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/psychrochart/util.py` & `psychrochart-0.9.1/psychrochart/util.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.0/pyproject.toml` & `psychrochart-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 log_level = "INFO"
 log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.9.0"
+version = "0.9.1"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `psychrochart-0.9.0/PKG-INFO` & `psychrochart-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.10,<3.12
@@ -58,28 +58,34 @@
 
 ```shell
 pip install psychrochart
 ```
 
 ## Features
 
-- **SI** units (with temperatures in celsius for better readability).
-- Easy style customization based on [**pydantic**](https://docs.pydantic.dev/latest/) models and config presets for full customization of colors, line styles, line widths, etc..
+- **SI** units (with temperatures in celsius for better readability), with _partial_ compatibility with IP system (imperial units)
+- Easy style customization based on [**pydantic**](https://docs.pydantic.dev/latest/) models and config presets for full customization of **chart limits**, included lines and labels, colors, line styles, line widths, etc..
 - Psychrometric charts within temperature and humidity ratio ranges, for any pressure\*, with:
   - **Saturation line**
   - **Constant RH lines**
   - **Constant enthalpy lines**
   - **Constant wet-bulb temperature lines**
   - **Constant specific volume lines**
   - **Constant dry-bulb temperature lines** (internal orthogonal grid, vertical)
   - **Constant humidity ratio lines** (internal orthogonal grid, horizontal)
-- Plot legend for each family of lines
+- Plot legend for each family of lines, labeled zones and annotations
 - Specify labels for each family of lines
-- **Overlay points, zones, convex hulls, and arrows**
-- **Export SVG, PNG files**
+- Overlay points, arrows, **data-series** (numpy arrays or pandas series), and convex hulls around points
+- Define multiple kinds of **zones limited by psychrometric values**:
+  - 'dbt-rh' for areas between dry-bulb temperature and relative humidity values,
+  - 'enthalpy-rh' for areas between constant enthalpy and relative humidity values
+  - 'volume-rh' for areas between constant volume and relative humidity values
+  - 'dbt-wmax' for an area between dry-bulb temperature and water vapor content values (:= a rectangle cut by the saturation line),
+  - 'xy-points' to define arbitrary closed paths in plot coordinates (dbt, abs humidity)
+- **Export as SVG, PNG files**, or generate dynamic SVGs with extra CSS and <defs> with `chart.make_svg(...)`
 
 > NOTE: The ranges of temperature, humidity and pressure where this library should provide good results are within the normal environments for people to live in.
 >
 > Don't expect right results if doing other type of thermodynamic calculations.
 >
 > ⚠️ **Over saturated water vapor states are not implemented**. This library is intended for HVAC applications only ⚠️
```

