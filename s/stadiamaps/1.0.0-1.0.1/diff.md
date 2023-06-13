# Comparing `tmp/stadiamaps-1.0.0.tar.gz` & `tmp/stadiamaps-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadiamaps-1.0.0.tar", last modified: Mon Jun 12 15:36:31 2023, max compression
+gzip compressed data, was "stadiamaps-1.0.1.tar", last modified: Mon Jun 12 16:15:24 2023, max compression
```

## Comparing `stadiamaps-1.0.0.tar` & `stadiamaps-1.0.1.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:31.595524 stadiamaps-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-12 15:36:31.595524 stadiamaps-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 15:36:31.595524 stadiamaps-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:31.559522 stadiamaps-1.0.0/stadiamaps/
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:31.559522 stadiamaps-1.0.0/stadiamaps/api/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97488 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/api/geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/api/geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50673 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/api/routing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:31.575523 stadiamaps-1.0.0/stadiamaps/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/admin_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/administrative.py
--rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/bike_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/directions_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/edge_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/end_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/height_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/height_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/locate_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/locate_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/matched_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/restrictions.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/road_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/route_leg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/route_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/speeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13690 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/traversability.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/tz_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/models/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/stadiamaps/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:31.559522 stadiamaps-1.0.0/stadiamaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-12 15:36:31.000000 stadiamaps-1.0.0/stadiamaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-06-12 15:36:31.000000 stadiamaps-1.0.0/stadiamaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:36:31.000000 stadiamaps-1.0.0/stadiamaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 15:36:31.000000 stadiamaps-1.0.0/stadiamaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 15:36:31.000000 stadiamaps-1.0.0/stadiamaps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:31.595524 stadiamaps-1.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:31.595524 stadiamaps-1.0.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/integration/test_eu_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/integration/test_gecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/integration/test_geospatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/integration/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_admin_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_administrative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_bike_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_directions_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_edge_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_end_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_height_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_height_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_locate_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_locate_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_matched_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_road_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_route_leg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_route_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_routing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_speeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_traversability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_tz_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-12 15:36:19.000000 stadiamaps-1.0.0/test/test_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:15:24.155539 stadiamaps-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-12 16:15:24.155539 stadiamaps-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 16:15:24.155539 stadiamaps-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:15:24.095538 stadiamaps-1.0.1/stadiamaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:15:24.099538 stadiamaps-1.0.1/stadiamaps/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97488 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/api/geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/api/geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50673 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/api/routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:15:24.131538 stadiamaps-1.0.1/stadiamaps/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/administrative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/end_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/height_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/height_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/road_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/speeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13690 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/traversability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/models/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/stadiamaps/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:15:24.099538 stadiamaps-1.0.1/stadiamaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-12 16:15:24.000000 stadiamaps-1.0.1/stadiamaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-06-12 16:15:24.000000 stadiamaps-1.0.1/stadiamaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:15:24.000000 stadiamaps-1.0.1/stadiamaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 16:15:24.000000 stadiamaps-1.0.1/stadiamaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 16:15:24.000000 stadiamaps-1.0.1/stadiamaps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:15:24.155539 stadiamaps-1.0.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:15:24.155539 stadiamaps-1.0.1/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/integration/test_eu_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/integration/test_gecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/integration/test_geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/integration/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_administrative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_end_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_height_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_height_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_road_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_speeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_traversability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-12 16:14:59.000000 stadiamaps-1.0.1/test/test_warning.py
```

### Comparing `stadiamaps-1.0.0/LICENSE.txt` & `stadiamaps-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/PKG-INFO` & `stadiamaps-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 1.0.0
+Version: 1.0.1
 Summary: Stadia Maps Geospatial APIs
-Home-page: https://docs.stadiamaps.com/
+Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-1.0.0/README.md` & `stadiamaps-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/pyproject.toml` & `stadiamaps-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stadiamaps"
-version = "1.0.0"
+version = "1.0.1"
 description = "Stadia Maps Geospatial APIs"
 authors = ["Stadia Maps Support <support@stadiamaps.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/stadiamaps/stadiamaps-api-py"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Stadia Maps Geospatial APIs"]
```

### Comparing `stadiamaps-1.0.0/setup.py` & `stadiamaps-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "stadiamaps"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Stadia Maps Geospatial APIs",
     author="Stadia Maps Support",
     author_email="support@stadiamaps.com",
-    url="https://docs.stadiamaps.com/",
+    url="https://github.com/stadiamaps/stadiamaps-api-py",
     keywords=["OpenAPI", "OpenAPI-Generator", "Stadia Maps Geospatial APIs"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description_content_type='text/markdown',
     long_description="""
 # Stadia Maps Python API Client
```

### Comparing `stadiamaps-1.0.0/stadiamaps/__init__.py` & `stadiamaps-1.0.1/stadiamaps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 # import apis into sdk package
 from stadiamaps.api.geocoding_api import GeocodingApi
 from stadiamaps.api.geospatial_api import GeospatialApi
 from stadiamaps.api.routing_api import RoutingApi
 
 # import ApiClient
```

### Comparing `stadiamaps-1.0.0/stadiamaps/api/geocoding_api.py` & `stadiamaps-1.0.1/stadiamaps/api/geocoding_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/api/geospatial_api.py` & `stadiamaps-1.0.1/stadiamaps/api/geospatial_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/api/routing_api.py` & `stadiamaps-1.0.1/stadiamaps/api/routing_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/api_client.py` & `stadiamaps-1.0.1/stadiamaps/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `stadiamaps-1.0.0/stadiamaps/api_response.py` & `stadiamaps-1.0.1/stadiamaps/api_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/configuration.py` & `stadiamaps-1.0.1/stadiamaps/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 5.0.2\n"\
-               "SDK Package Version: 1.0.0".\
+               "SDK Package Version: 1.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `stadiamaps-1.0.0/stadiamaps/exceptions.py` & `stadiamaps-1.0.1/stadiamaps/exceptions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/__init__.py` & `stadiamaps-1.0.1/stadiamaps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/access.py` & `stadiamaps-1.0.1/stadiamaps/models/access.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/admin_region.py` & `stadiamaps-1.0.1/stadiamaps/models/admin_region.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/administrative.py` & `stadiamaps-1.0.1/stadiamaps/models/administrative.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/auto_costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/auto_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/auto_costing_options_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/auto_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/base_costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/base_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/base_trace_request.py` & `stadiamaps-1.0.1/stadiamaps/models/base_trace_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/bicycle_costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/bicycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/bicycle_costing_options_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/bicycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/bike_network.py` & `stadiamaps-1.0.1/stadiamaps/models/bike_network.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/contour.py` & `stadiamaps-1.0.1/stadiamaps/models/contour.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/coordinate.py` & `stadiamaps-1.0.1/stadiamaps/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/costing_model.py` & `stadiamaps-1.0.1/stadiamaps/models/costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/directions_options.py` & `stadiamaps-1.0.1/stadiamaps/models/directions_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/distance_unit.py` & `stadiamaps-1.0.1/stadiamaps/models/distance_unit.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/edge_sign.py` & `stadiamaps-1.0.1/stadiamaps/models/edge_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/edge_use.py` & `stadiamaps-1.0.1/stadiamaps/models/edge_use.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/end_node.py` & `stadiamaps-1.0.1/stadiamaps/models/end_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_attributes.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_attributes.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_geometry.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_geometry.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_geometry_base.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_geometry_base.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_line_string.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_line_string.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_line_string_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_line_string_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_point.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_point_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_point_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_polygon.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_polygon.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geo_json_polygon_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/geo_json_polygon_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/geocoding_object.py` & `stadiamaps-1.0.1/stadiamaps/models/geocoding_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/height_request.py` & `stadiamaps-1.0.1/stadiamaps/models/height_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/height_response.py` & `stadiamaps-1.0.1/stadiamaps/models/height_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/highway_classification.py` & `stadiamaps-1.0.1/stadiamaps/models/highway_classification.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/intersecting_edge.py` & `stadiamaps-1.0.1/stadiamaps/models/intersecting_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/isochrone_costing_model.py` & `stadiamaps-1.0.1/stadiamaps/models/isochrone_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/isochrone_feature.py` & `stadiamaps-1.0.1/stadiamaps/models/isochrone_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/isochrone_properties.py` & `stadiamaps-1.0.1/stadiamaps/models/isochrone_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/isochrone_request.py` & `stadiamaps-1.0.1/stadiamaps/models/isochrone_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/isochrone_response.py` & `stadiamaps-1.0.1/stadiamaps/models/isochrone_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/locate_detailed_edge.py` & `stadiamaps-1.0.1/stadiamaps/models/locate_detailed_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/locate_edge.py` & `stadiamaps-1.0.1/stadiamaps/models/locate_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/locate_edge_info.py` & `stadiamaps-1.0.1/stadiamaps/models/locate_edge_info.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/locate_node.py` & `stadiamaps-1.0.1/stadiamaps/models/locate_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/locate_node_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/locate_node_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/locate_object.py` & `stadiamaps-1.0.1/stadiamaps/models/locate_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/maneuver_sign.py` & `stadiamaps-1.0.1/stadiamaps/models/maneuver_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/maneuver_sign_element.py` & `stadiamaps-1.0.1/stadiamaps/models/maneuver_sign_element.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_costing_model.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_request.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_request_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_route_response.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_route_response_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_route_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_trace_options.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_trace_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_waypoint.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/map_match_waypoint_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/map_match_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/matched_point.py` & `stadiamaps-1.0.1/stadiamaps/models/matched_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/matrix_costing_model.py` & `stadiamaps-1.0.1/stadiamaps/models/matrix_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/matrix_distance.py` & `stadiamaps-1.0.1/stadiamaps/models/matrix_distance.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/matrix_request.py` & `stadiamaps-1.0.1/stadiamaps/models/matrix_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/matrix_response.py` & `stadiamaps-1.0.1/stadiamaps/models/matrix_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/motor_scooter_costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/motor_scooter_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/motor_scooter_costing_options_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/motor_scooter_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/motorcycle_costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/motorcycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/motorcycle_costing_options_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/motorcycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/nearest_roads_request.py` & `stadiamaps-1.0.1/stadiamaps/models/nearest_roads_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/node_id.py` & `stadiamaps-1.0.1/stadiamaps/models/node_id.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/node_type.py` & `stadiamaps-1.0.1/stadiamaps/models/node_type.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/optimized_route_request.py` & `stadiamaps-1.0.1/stadiamaps/models/optimized_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pedestrian_costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/pedestrian_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_feature.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_properties.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_properties_addendum.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_properties_addendum.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_layer.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_layer.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_response.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_response_geocoding.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_response_geocoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/pelias_source.py` & `stadiamaps-1.0.1/stadiamaps/models/pelias_source.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/restrictions.py` & `stadiamaps-1.0.1/stadiamaps/models/restrictions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/road_class.py` & `stadiamaps-1.0.1/stadiamaps/models/road_class.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/route_leg.py` & `stadiamaps-1.0.1/stadiamaps/models/route_leg.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/route_maneuver.py` & `stadiamaps-1.0.1/stadiamaps/models/route_maneuver.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/route_request.py` & `stadiamaps-1.0.1/stadiamaps/models/route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/route_response.py` & `stadiamaps-1.0.1/stadiamaps/models/route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/route_response_trip.py` & `stadiamaps-1.0.1/stadiamaps/models/route_response_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/route_summary.py` & `stadiamaps-1.0.1/stadiamaps/models/route_summary.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/routing_response_waypoint.py` & `stadiamaps-1.0.1/stadiamaps/models/routing_response_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/routing_response_waypoint_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/routing_response_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/routing_waypoint.py` & `stadiamaps-1.0.1/stadiamaps/models/routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/routing_waypoint_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py` & `stadiamaps-1.0.1/stadiamaps/models/routing_waypoint_all_of_search_filter.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/simple_routing_waypoint.py` & `stadiamaps-1.0.1/stadiamaps/models/simple_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/simple_routing_waypoint_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/simple_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/speeds.py` & `stadiamaps-1.0.1/stadiamaps/models/speeds.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attribute_filter_options.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attribute_filter_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attribute_key.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attribute_key.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attributes_base_response.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attributes_base_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attributes_request.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attributes_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attributes_request_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attributes_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attributes_request_all_of_filters.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attributes_request_all_of_filters.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attributes_response.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attributes_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_attributes_response_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_attributes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/trace_edge.py` & `stadiamaps-1.0.1/stadiamaps/models/trace_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/travel_mode.py` & `stadiamaps-1.0.1/stadiamaps/models/travel_mode.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/traversability.py` & `stadiamaps-1.0.1/stadiamaps/models/traversability.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/truck_costing_options.py` & `stadiamaps-1.0.1/stadiamaps/models/truck_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/truck_costing_options_all_of.py` & `stadiamaps-1.0.1/stadiamaps/models/truck_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/tz_response.py` & `stadiamaps-1.0.1/stadiamaps/models/tz_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/valhalla_languages.py` & `stadiamaps-1.0.1/stadiamaps/models/valhalla_languages.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/valhalla_long_units.py` & `stadiamaps-1.0.1/stadiamaps/models/valhalla_long_units.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/models/warning.py` & `stadiamaps-1.0.1/stadiamaps/models/warning.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps/rest.py` & `stadiamaps-1.0.1/stadiamaps/rest.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/stadiamaps.egg-info/PKG-INFO` & `stadiamaps-1.0.1/stadiamaps.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 1.0.0
+Version: 1.0.1
 Summary: Stadia Maps Geospatial APIs
-Home-page: https://docs.stadiamaps.com/
+Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-1.0.0/stadiamaps.egg-info/SOURCES.txt` & `stadiamaps-1.0.1/stadiamaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/integration/test_eu_endpoint.py` & `stadiamaps-1.0.1/test/integration/test_eu_endpoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/integration/test_gecoding.py` & `stadiamaps-1.0.1/test/integration/test_gecoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/integration/test_geospatial.py` & `stadiamaps-1.0.1/test/integration/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/integration/test_routing.py` & `stadiamaps-1.0.1/test/integration/test_routing.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_access.py` & `stadiamaps-1.0.1/test/test_access.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_admin_region.py` & `stadiamaps-1.0.1/test/test_admin_region.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_administrative.py` & `stadiamaps-1.0.1/test/test_administrative.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_auto_costing_options.py` & `stadiamaps-1.0.1/test/test_auto_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_auto_costing_options_all_of.py` & `stadiamaps-1.0.1/test/test_auto_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_base_costing_options.py` & `stadiamaps-1.0.1/test/test_base_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_base_trace_request.py` & `stadiamaps-1.0.1/test/test_base_trace_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_bicycle_costing_options.py` & `stadiamaps-1.0.1/test/test_bicycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_bicycle_costing_options_all_of.py` & `stadiamaps-1.0.1/test/test_bicycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_bike_network.py` & `stadiamaps-1.0.1/test/test_bike_network.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_contour.py` & `stadiamaps-1.0.1/test/test_contour.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_coordinate.py` & `stadiamaps-1.0.1/test/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_costing_model.py` & `stadiamaps-1.0.1/test/test_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_costing_options.py` & `stadiamaps-1.0.1/test/test_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_directions_options.py` & `stadiamaps-1.0.1/test/test_directions_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_distance_unit.py` & `stadiamaps-1.0.1/test/test_distance_unit.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_edge_sign.py` & `stadiamaps-1.0.1/test/test_edge_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_edge_use.py` & `stadiamaps-1.0.1/test/test_edge_use.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_end_node.py` & `stadiamaps-1.0.1/test/test_end_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_attributes.py` & `stadiamaps-1.0.1/test/test_geo_attributes.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_geometry.py` & `stadiamaps-1.0.1/test/test_geo_json_geometry.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_geometry_base.py` & `stadiamaps-1.0.1/test/test_geo_json_geometry_base.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_line_string.py` & `stadiamaps-1.0.1/test/test_geo_json_line_string.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_line_string_all_of.py` & `stadiamaps-1.0.1/test/test_geo_json_line_string_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_point.py` & `stadiamaps-1.0.1/test/test_geo_json_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_point_all_of.py` & `stadiamaps-1.0.1/test/test_geo_json_point_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_polygon.py` & `stadiamaps-1.0.1/test/test_geo_json_polygon.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geo_json_polygon_all_of.py` & `stadiamaps-1.0.1/test/test_geo_json_polygon_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geocoding_api.py` & `stadiamaps-1.0.1/test/test_geocoding_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geocoding_object.py` & `stadiamaps-1.0.1/test/test_geocoding_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_geospatial_api.py` & `stadiamaps-1.0.1/test/test_geospatial_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_height_request.py` & `stadiamaps-1.0.1/test/test_height_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_height_response.py` & `stadiamaps-1.0.1/test/test_height_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_highway_classification.py` & `stadiamaps-1.0.1/test/test_highway_classification.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_intersecting_edge.py` & `stadiamaps-1.0.1/test/test_intersecting_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_isochrone_costing_model.py` & `stadiamaps-1.0.1/test/test_isochrone_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_isochrone_feature.py` & `stadiamaps-1.0.1/test/test_isochrone_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_isochrone_properties.py` & `stadiamaps-1.0.1/test/test_isochrone_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_isochrone_request.py` & `stadiamaps-1.0.1/test/test_isochrone_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_isochrone_response.py` & `stadiamaps-1.0.1/test/test_isochrone_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_locate_detailed_edge.py` & `stadiamaps-1.0.1/test/test_locate_detailed_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_locate_edge.py` & `stadiamaps-1.0.1/test/test_locate_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_locate_edge_info.py` & `stadiamaps-1.0.1/test/test_locate_edge_info.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_locate_node.py` & `stadiamaps-1.0.1/test/test_locate_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_locate_node_all_of.py` & `stadiamaps-1.0.1/test/test_locate_node_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_locate_object.py` & `stadiamaps-1.0.1/test/test_locate_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_maneuver_sign.py` & `stadiamaps-1.0.1/test/test_maneuver_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_maneuver_sign_element.py` & `stadiamaps-1.0.1/test/test_maneuver_sign_element.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_costing_model.py` & `stadiamaps-1.0.1/test/test_map_match_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_request.py` & `stadiamaps-1.0.1/test/test_map_match_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_request_all_of.py` & `stadiamaps-1.0.1/test/test_map_match_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_route_response.py` & `stadiamaps-1.0.1/test/test_map_match_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_route_response_all_of.py` & `stadiamaps-1.0.1/test/test_map_match_route_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_trace_options.py` & `stadiamaps-1.0.1/test/test_map_match_trace_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_waypoint.py` & `stadiamaps-1.0.1/test/test_map_match_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_map_match_waypoint_all_of.py` & `stadiamaps-1.0.1/test/test_map_match_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_matched_point.py` & `stadiamaps-1.0.1/test/test_matched_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_matrix_costing_model.py` & `stadiamaps-1.0.1/test/test_matrix_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_matrix_distance.py` & `stadiamaps-1.0.1/test/test_matrix_distance.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_matrix_request.py` & `stadiamaps-1.0.1/test/test_matrix_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_matrix_response.py` & `stadiamaps-1.0.1/test/test_matrix_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_motor_scooter_costing_options.py` & `stadiamaps-1.0.1/test/test_motor_scooter_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_motor_scooter_costing_options_all_of.py` & `stadiamaps-1.0.1/test/test_motor_scooter_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_motorcycle_costing_options.py` & `stadiamaps-1.0.1/test/test_motorcycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_motorcycle_costing_options_all_of.py` & `stadiamaps-1.0.1/test/test_motorcycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_nearest_roads_request.py` & `stadiamaps-1.0.1/test/test_nearest_roads_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_node_id.py` & `stadiamaps-1.0.1/test/test_node_id.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_node_type.py` & `stadiamaps-1.0.1/test/test_node_type.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_optimized_route_request.py` & `stadiamaps-1.0.1/test/test_optimized_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pedestrian_costing_options.py` & `stadiamaps-1.0.1/test/test_pedestrian_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_geo_json_feature.py` & `stadiamaps-1.0.1/test/test_pelias_geo_json_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_geo_json_properties.py` & `stadiamaps-1.0.1/test/test_pelias_geo_json_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_geo_json_properties_addendum.py` & `stadiamaps-1.0.1/test/test_pelias_geo_json_properties_addendum.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-1.0.1/test/test_pelias_geo_json_properties_addendum_osm.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_layer.py` & `stadiamaps-1.0.1/test/test_pelias_layer.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_response.py` & `stadiamaps-1.0.1/test/test_pelias_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_response_geocoding.py` & `stadiamaps-1.0.1/test/test_pelias_response_geocoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_pelias_source.py` & `stadiamaps-1.0.1/test/test_pelias_source.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_restrictions.py` & `stadiamaps-1.0.1/test/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_road_class.py` & `stadiamaps-1.0.1/test/test_road_class.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_route_leg.py` & `stadiamaps-1.0.1/test/test_route_leg.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_route_maneuver.py` & `stadiamaps-1.0.1/test/test_route_maneuver.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_route_request.py` & `stadiamaps-1.0.1/test/test_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_route_response.py` & `stadiamaps-1.0.1/test/test_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_route_response_trip.py` & `stadiamaps-1.0.1/test/test_route_response_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_route_summary.py` & `stadiamaps-1.0.1/test/test_route_summary.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_routing_api.py` & `stadiamaps-1.0.1/test/test_routing_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_routing_response_waypoint.py` & `stadiamaps-1.0.1/test/test_routing_response_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_routing_response_waypoint_all_of.py` & `stadiamaps-1.0.1/test/test_routing_response_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_routing_waypoint.py` & `stadiamaps-1.0.1/test/test_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_routing_waypoint_all_of.py` & `stadiamaps-1.0.1/test/test_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_routing_waypoint_all_of_search_filter.py` & `stadiamaps-1.0.1/test/test_routing_waypoint_all_of_search_filter.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_simple_routing_waypoint.py` & `stadiamaps-1.0.1/test/test_simple_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_simple_routing_waypoint_all_of.py` & `stadiamaps-1.0.1/test/test_simple_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_speeds.py` & `stadiamaps-1.0.1/test/test_speeds.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attribute_filter_options.py` & `stadiamaps-1.0.1/test/test_trace_attribute_filter_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attribute_key.py` & `stadiamaps-1.0.1/test/test_trace_attribute_key.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attributes_base_response.py` & `stadiamaps-1.0.1/test/test_trace_attributes_base_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attributes_request.py` & `stadiamaps-1.0.1/test/test_trace_attributes_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attributes_request_all_of.py` & `stadiamaps-1.0.1/test/test_trace_attributes_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attributes_request_all_of_filters.py` & `stadiamaps-1.0.1/test/test_trace_attributes_request_all_of_filters.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attributes_response.py` & `stadiamaps-1.0.1/test/test_trace_attributes_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_attributes_response_all_of.py` & `stadiamaps-1.0.1/test/test_trace_attributes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_trace_edge.py` & `stadiamaps-1.0.1/test/test_trace_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_travel_mode.py` & `stadiamaps-1.0.1/test/test_travel_mode.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_traversability.py` & `stadiamaps-1.0.1/test/test_traversability.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_truck_costing_options.py` & `stadiamaps-1.0.1/test/test_truck_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_truck_costing_options_all_of.py` & `stadiamaps-1.0.1/test/test_truck_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_tz_response.py` & `stadiamaps-1.0.1/test/test_tz_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_valhalla_languages.py` & `stadiamaps-1.0.1/test/test_valhalla_languages.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_valhalla_long_units.py` & `stadiamaps-1.0.1/test/test_valhalla_long_units.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.0/test/test_warning.py` & `stadiamaps-1.0.1/test/test_warning.py`

 * *Files identical despite different names*

