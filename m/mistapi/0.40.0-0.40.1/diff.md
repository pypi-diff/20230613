# Comparing `tmp/mistapi-0.40.0.tar.gz` & `tmp/mistapi-0.40.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.40.0.tar", last modified: Tue May 30 10:33:53 2023, max compression
+gzip compressed data, was "mistapi-0.40.1.tar", last modified: Tue Jun 13 20:28:16 2023, max compression
```

## Comparing `mistapi-0.40.0.tar` & `mistapi-0.40.1.tar`

### file list

```diff
@@ -1,234 +1,237 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.651244 mistapi-0.40.0/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.40.0/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-05-30 10:33:53.651367 mistapi-0.40.0/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10556 2023-02-22 14:11:31.000000 mistapi-0.40.0/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-05-30 10:33:26.000000 mistapi-0.40.0/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-05-30 10:33:53.651761 mistapi-0.40.0/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.533791 mistapi-0.40.0/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.543086 mistapi-0.40.0/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)     7909 2023-04-20 13:57:39.000000 mistapi-0.40.0/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.40.0/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    21519 2023-05-30 10:13:58.000000 mistapi-0.40.0/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.40.0/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.546008 mistapi-0.40.0/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.40.0/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.40.0/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.40.0/src/mistapi/__pagination.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.546486 mistapi-0.40.0/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.547060 mistapi-0.40.0/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      902 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.555066 mistapi-0.40.0/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1181 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2027 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1730 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1713 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/call_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1402 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1794 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1712 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1055 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/license_types.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.555420 mistapi-0.40.0/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.558171 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7123 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1972 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1947 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1940 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7487 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.558968 mistapi-0.40.0/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1168 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.562177 mistapi-0.40.0/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1099 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.573537 mistapi-0.40.0/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2628 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1155 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.574222 mistapi-0.40.0/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      984 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.574981 mistapi-0.40.0/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1257 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.585094 mistapi-0.40.0/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2620 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1828 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3330 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2981 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5244 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1660 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4002 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5981 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3637 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1476 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/suggestion.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3225 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.623098 mistapi-0.40.0/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3119 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3255 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6440 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7576 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5989 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2344 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1709 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11381 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1236 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1846 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20091 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4812 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4870 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6514 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2978 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5034 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6927 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2503 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4955 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1434 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4754 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15280 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4618 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4872 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1407 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2975 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5923 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1913 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8274 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6892 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4719 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4721 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4825 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15912 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8619 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4788 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8223 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4767 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    32140 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1747 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5449 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6846 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4541 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3540 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7466 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5236 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5887 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.624075 mistapi-0.40.0/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1110 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.625257 mistapi-0.40.0/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1161 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1103 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.628675 mistapi-0.40.0/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2916 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2596 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2015 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2109 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.631300 mistapi-0.40.0/src/mistapi/api/v1/site/
--rw-r--r--   0 tmunzer    (502) staff       (20)      637 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2334 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2292 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2341 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2292 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2264 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/site/vpns.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.649900 mistapi-0.40.0/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2273 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8657 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2655 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6038 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4659 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17187 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2327 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    58343 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5037 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4073 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9142 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8539 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    14930 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3117 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5810 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7530 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5752 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5721 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3809 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5978 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2404 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3837 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20771 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1970 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    61251 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1905 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4633 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4683 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2239 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5300 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3839 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6811 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5279 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5936 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4599 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.650961 mistapi-0.40.0/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1072 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-05-30 10:33:26.000000 mistapi-0.40.0/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2023-05-30 10:31:44.000000 mistapi-0.40.0/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-05-30 10:33:53.545377 mistapi-0.40.0/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     7608 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-05-30 10:33:53.000000 mistapi-0.40.0/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.480102 mistapi-0.40.1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.40.1/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-13 20:28:16.480228 mistapi-0.40.1/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10505 2023-06-13 20:27:38.000000 mistapi-0.40.1/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-06-13 20:28:05.000000 mistapi-0.40.1/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-06-13 20:28:16.480650 mistapi-0.40.1/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.309313 mistapi-0.40.1/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.324350 mistapi-0.40.1/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7909 2023-04-20 13:57:39.000000 mistapi-0.40.1/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.40.1/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    21804 2023-06-01 19:27:20.000000 mistapi-0.40.1/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.40.1/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.327114 mistapi-0.40.1/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.40.1/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.40.1/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.40.1/src/mistapi/__pagination.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.327677 mistapi-0.40.1/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.328071 mistapi-0.40.1/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.335713 mistapi-0.40.1/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1235 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2027 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1730 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1713 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/call_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1402 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1712 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1055 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1807 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/other_device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.339406 mistapi-0.40.1/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.355910 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7123 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1972 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1947 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1940 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7487 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.356976 mistapi-0.40.1/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1168 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.357876 mistapi-0.40.1/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1099 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.361064 mistapi-0.40.1/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2628 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1155 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.362065 mistapi-0.40.1/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      984 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.364218 mistapi-0.40.1/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1257 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.372494 mistapi-0.40.1/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2620 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1828 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4444 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2981 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5244 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1660 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4002 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5981 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3637 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1476 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3225 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.425419 mistapi-0.40.1/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3208 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3255 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6440 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7576 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5989 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2344 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1709 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11397 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1236 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1846 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20091 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4812 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4870 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6514 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2978 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5034 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6927 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2503 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5217 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1434 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4754 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15280 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4618 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4872 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1407 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2975 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8802 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1913 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8274 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6892 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4719 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4721 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4825 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    16586 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8619 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4788 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8223 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4767 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    32140 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1747 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5449 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6846 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4541 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1344 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4779 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3540 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7466 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5236 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5887 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.426516 mistapi-0.40.1/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1110 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.427648 mistapi-0.40.1/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1161 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1103 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.431521 mistapi-0.40.1/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2916 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2596 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2015 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2109 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.478405 mistapi-0.40.1/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2588 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8657 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2655 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6038 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4659 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17283 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2327 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2336 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    58343 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5037 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4073 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9142 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8539 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    14930 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2294 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6008 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5810 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7530 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5752 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5737 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3809 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2343 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2294 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6042 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2404 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3837 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20771 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1970 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    61323 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1905 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4633 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4683 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2239 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2266 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1350 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5300 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3839 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6811 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5279 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5936 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4599 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.479811 mistapi-0.40.1/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1072 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11557 2023-06-07 14:42:24.000000 mistapi-0.40.1/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.326381 mistapi-0.40.1/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7781 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.40.0/LICENSE` & `mistapi-0.40.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/PKG-INFO` & `mistapi-0.40.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.40.0
+Version: 0.40.1
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
@@ -77,15 +77,14 @@
 LOGGING_LOG_LEVEL | int | 10 | The minimum log level to log on the file, using `logging` schema (0 = Disabled, 10 = Debug, 20 = Info, 30 = Warning, 40 = Error, 50 = Critical). This is only used when the script calling `mistapi` is using Python `logging` package and is configured to log to a file |
 
 
 An example of the environment file content is:
 ```
 MIST_HOST = api.mist.com
 MIST_APITOKEN = xxxxxx
-MIST_ORG_ID = 203d3d02-xxxx-xxxx-xxxx-76896a3330f4
 ```
 
 ## Usage
 Usage examples are available in the [mist_library repository](https://github.com/tmunzer/mist_library).
 
 To use it, 
 ### 1. `APISession` must be instanciated:
```

### Comparing `mistapi-0.40.0/README.md` & `mistapi-0.40.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 LOGGING_LOG_LEVEL | int | 10 | The minimum log level to log on the file, using `logging` schema (0 = Disabled, 10 = Debug, 20 = Info, 30 = Warning, 40 = Error, 50 = Critical). This is only used when the script calling `mistapi` is using Python `logging` package and is configured to log to a file |
 
 
 An example of the environment file content is:
 ```
 MIST_HOST = api.mist.com
 MIST_APITOKEN = xxxxxx
-MIST_ORG_ID = 203d3d02-xxxx-xxxx-xxxx-76896a3330f4
 ```
 
 ## Usage
 Usage examples are available in the [mist_library repository](https://github.com/tmunzer/mist_library).
 
 To use it, 
 ### 1. `APISession` must be instanciated:
```

### Comparing `mistapi-0.40.0/pyproject.toml` & `mistapi-0.40.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.40.0"
+version = "0.40.1"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.40.0/src/mistapi/__api_request.py` & `mistapi-0.40.1/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/__api_response.py` & `mistapi-0.40.1/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/__api_session.py` & `mistapi-0.40.1/src/mistapi/__api_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,19 +160,24 @@
 
         PARAMS
         -----------
         :param str cloud_uri - Mist FQDN to reach ("api.mist.com", "api.eu.mist.com", ...)
         """
         logger.debug(f"apisession:in  > set_cloud")
         self._cloud_uri = None
-        for cloud in clouds:
-            if cloud["host"] == cloud_uri:
+        if cloud_uri == "api.mistsys.com":
                 self._cloud_uri = cloud_uri
                 logger.debug(f"apisession:Mist Cloud configured to {self._cloud_uri}")
                 console.debug(f"Mist Cloud configured to {self._cloud_uri}")
+        else:
+            for cloud in clouds:
+                if cloud["host"] == cloud_uri:
+                    self._cloud_uri = cloud_uri
+                    logger.debug(f"apisession:Mist Cloud configured to {self._cloud_uri}")
+                    console.debug(f"Mist Cloud configured to {self._cloud_uri}")
         if not self._cloud_uri:
             logger.error(f"apisession:{cloud_uri} is not valid")
             console.error(f"{cloud_uri} is not valid")
 
     def get_cloud(self):
         """
         Return the Mist Cloud currently configured
```

### Comparing `mistapi-0.40.0/src/mistapi/__init__.py` & `mistapi-0.40.1/src/mistapi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 '''
 
 from mistapi.__api_session import APISession
 from mistapi import api
 from mistapi import cli
 from mistapi.__pagination import get_next, get_all
 
-__version__ = "0.40.0"
+__version__ = "0.40.1"
 __author__ = "Thomas Munzer <tmunzer@juniper.net>"
```

### Comparing `mistapi-0.40.0/src/mistapi/__logger.py` & `mistapi-0.40.1/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/__models/privilege.py` & `mistapi-0.40.1/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/__pagination.py` & `mistapi-0.40.1/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,10 +17,9 @@
 from mistapi.api.v1 import logout
 from mistapi.api.v1 import mobile
 from mistapi.api.v1 import msps
 from mistapi.api.v1 import orgs
 from mistapi.api.v1 import recover
 from mistapi.api.v1 import register
 from mistapi.api.v1 import self
-from mistapi.api.v1 import site
 from mistapi.api.v1 import sites
 from mistapi.api.v1 import utils
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 from mistapi.api.v1.const import device_events
 from mistapi.api.v1.const import device_models
 from mistapi.api.v1.const import insight_metrics
 from mistapi.api.v1.const import languages
 from mistapi.api.v1.const import license_types
 from mistapi.api.v1.const import mxedge_events
 from mistapi.api.v1.const import mxedge_models
+from mistapi.api.v1.const import other_device_events
 from mistapi.api.v1.const import traffic_types
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/applications.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listAlarmDefinitions")  
-def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApplications")  
+def getApplications(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/alarm_defs"
+    uri = f"/api/v1/const/applications"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
+def listApplications(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/alarm_defs"
+    uri = f"/api/v1/const/applications"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApChannels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApChannels")  
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApLedDefinition")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApLedDefinition")  
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/applications.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/device_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApplications")  
-def getApplications(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listDeviceModels")  
+def getDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listApplications
+    API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/applications"
+    uri = f"/api/v1/const/device_models"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listApplications(mist_session:_APISession) -> _APIResponse:
+def listDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listApplications
+    API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/applications"
+    uri = f"/api/v1/const/device_models"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/call_events.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/call_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listCallEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listCallEventsDefinitions")  
 def getCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCallEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/client_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listClientEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listClientEventsDefinitions")  
 def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/countries.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listCountryCodes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listCountryCodes")  
 def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/device_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listDeviceEventsDefinitions")  
 def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/other_device_events.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listDeviceModels")  
-def getDeviceModels(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOtherDeviceEventsDefinitions")  
+def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
+    API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/device_models"
+    uri = f"/api/v1/const/other_device_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listDeviceModels(mist_session:_APISession) -> _APIResponse:
+def listOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
+    API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/device_models"
+    uri = f"/api/v1/const/other_device_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAvailableInsightMetrics")  
-def getSiteAvailableInsightMetrics(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listTrafficTypes")  
+def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableInsightMetrics
+    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/insight_metrics"
+    uri = f"/api/v1/const/traffic_types"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteAvailableInsightMetrics(mist_session:_APISession) -> _APIResponse:
+def listTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableInsightMetrics
+    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/insight_metrics"
+    uri = f"/api/v1/const/traffic_types"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/languages.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/languages.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteLanguages")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteLanguages")  
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/license_types.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/license_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMxEdgeEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMxEdgeEventsDefinitions")  
 def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMxEdgeModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMxEdgeModels")  
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/ssr.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,42 +10,54 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listTrafficTypes")  
-def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
+def getSiteSsrUpgrade(mist_session:_APISession, site_id:str, upgrade_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSsrUpgrade
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str upgrade_id        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/traffic_types"
+    uri = f"/api/v1/sites/{site_id}/ssr/upgrade/{upgrade_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listTrafficTypes(mist_session:_APISession) -> _APIResponse:
+def upgradeSiteSsr(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
+    API doc: https://doc.mist-lab.fr/#operation/upgradeSiteSsr
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str device_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/traffic_types"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/ssr/{device_id}/upgrade"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerAlarmTemplates")  
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerDeviceProfiles")  
 def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
 def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerRfTemplatesNames")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerRfTemplatesNames")  
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerSecPolicies")  
 def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerSiteGroups")  
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerSites")  
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -78,15 +78,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listInstallerMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerMaps")  
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.40.1/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.40.1/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/login/login.py` & `mistapi-0.40.1/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.40.1/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.40.1/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.40.1/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.40.1/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.40.1/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/admins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspAdmins")  
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/licenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspLicenses")  
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/insights.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,94 +10,80 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspLogs")  
-def getMspLogs(mist_session:_APISession, msp_id:str, org_id:str=None, admin_name:str=None, message:str=None) -> _APIResponse:
+def getOrgSitesSle(mist_session:_APISession, org_id:str, sle:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d", interval:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listMspLogs
+    API doc: https://doc.mist-lab.fr/#operation/getOrgSitesSle
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str org_id        
     
     QUERY PARAMS
     ------------
-    :param str org_id
-    :param str admin_name - admin name or email
-    :param str message        
+    :param str sle(wan, wired, wifi)
+    :param int start
+    :param int end
+    :param int limit
+    :param int page
+    :param str duration
+    :param str interval        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/logs"
+    uri = f"/api/v1/orgs/{org_id}/insights/sites-sle"
     query_params={}
-    if org_id: query_params["org_id"]=org_id
-    if admin_name: query_params["admin_name"]=admin_name
-    if message: query_params["message"]=message
+    if sle: query_params["sle"]=sle
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
+    if duration: query_params["duration"]=duration
+    if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listMspLogs(mist_session:_APISession, msp_id:str, org_id:str=None, admin_name:str=None, message:str=None) -> _APIResponse:
+def getOrgSle(mist_session:_APISession, org_id:str, metric:str, sle:str=None, duration:str="1d", interval:str=None, start:int=None, end:int=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listMspLogs
+    API doc: https://doc.mist-lab.fr/#operation/getOrgSle
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
-    
-    QUERY PARAMS
-    ------------
     :param str org_id
-    :param str admin_name - admin name or email
-    :param str message        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/msps/{msp_id}/logs"
-    query_params={}
-    if org_id: query_params["org_id"]=org_id
-    if admin_name: query_params["admin_name"]=admin_name
-    if message: query_params["message"]=message
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def countMspLogs(mist_session:_APISession, msp_id:str, distinct:str="admin_name") -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/countMspLogs
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str msp_id        
+    :param str metric        
     
     QUERY PARAMS
     ------------
-    :param str distinct(admin_id, admin_name, message, org_id)        
+    :param str sle - see [/api/v1/const/insight_metrics](/#tag/Constants/operation/getSiteAvailableInsightMetrics) for more details
+    :param str duration
+    :param str interval
+    :param int start
+    :param int end        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/logs/count"
+    uri = f"/api/v1/orgs/{org_id}/insights/{metric}"
     query_params={}
-    if distinct: query_params["distinct"]=distinct
+    if sle: query_params["sle"]=sle
+    if duration: query_params["duration"]=duration
+    if interval: query_params["interval"]=interval
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgGroups")  
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/orgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgs")  
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/search.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspSsoRoles")  
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspSsoLatestFailures")  
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgLicenses")  
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -53,15 +53,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspOrgStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgStats")  
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/suggestion.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/suggestion.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.40.1/src/mistapi/api/v1/msps/tickets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listMspTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspTickets")  
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,13 +64,15 @@
 from mistapi.api.v1.orgs import ssos
 from mistapi.api.v1.orgs import stats
 from mistapi.api.v1.orgs import subscriptions
 from mistapi.api.v1.orgs import templates
 from mistapi.api.v1.orgs import tickets
 from mistapi.api.v1.orgs import troubleshoot
 from mistapi.api.v1.orgs import vpns
+from mistapi.api.v1.orgs import wan_client
+from mistapi.api.v1.orgs import wan_clients
 from mistapi.api.v1.orgs import webhooks
 from mistapi.api.v1.orgs import wired_clients
 from mistapi.api.v1.orgs import wlans
 from mistapi.api.v1.orgs import wxrules
 from mistapi.api.v1.orgs import wxtags
 from mistapi.api.v1.orgs import wxtunnels
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/admins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAdmins")  
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAlarmTemplates")  
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -77,15 +77,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSuppressedAlarms")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSuppressedAlarms")  
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgApiTokens")  
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAptemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAptemplates")  
 def getOrgAptemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAssetFilters")  
 def getOrgAssetFilters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAssets")  
 def getOrgAssets(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/clients.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countOrgClientsWireless(mist_session:_APISession, org_id:str, distinct:str="device", mac:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, vlan:str=None, ssid:str=None, ip_address:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countOrgWirelessClients(mist_session:_APISession, org_id:str, distinct:str="device", mac:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, vlan:str=None, ssid:str=None, ip_address:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgClientsWireless
+    API doc: https://doc.mist-lab.fr/#operation/countOrgWirelessClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -64,17 +64,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgClientsEvents(mist_session:_APISession, org_id:str, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchOrgWirelessClientsEvents(mist_session:_APISession, org_id:str, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgClientsEvents
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgWirelessClientsEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -110,17 +110,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgClientsWireless(mist_session:_APISession, org_id:str, site_id:str=None, mac:str=None, ip_address:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, psk_id:str=None, psk_name:str=None, vlan:str=None, ssid:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchOrgWirelessClients(mist_session:_APISession, org_id:str, site_id:str=None, mac:str=None, ip_address:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, psk_id:str=None, psk_name:str=None, vlan:str=None, ssid:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgClientsWireless
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgWirelessClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -220,17 +220,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgClientWirelessSessions(mist_session:_APISession, org_id:str, ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_username:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, psk_id:str=None, psk_name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchOrgWirelessClientSessions(mist_session:_APISession, org_id:str, ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_username:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, psk_id:str=None, psk_name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgClientWirelessSessions
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgWirelessClientSessions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgDeviceProfiles")  
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgDevices")  
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -279,15 +279,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgApsMacs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgApsMacs")  
 def getOrgApsMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -394,15 +394,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgEvpnTopologies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgEvpnTopologies")  
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgGatewayTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgGatewayTemplates")  
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/guests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgGuestAuthorizations")  
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,80 +10,91 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOrgSitesSle(mist_session:_APISession, org_id:str, sle:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d", interval:str=None) -> _APIResponse:
+def countOrgWiredClients(mist_session:_APISession, org_id:str, distinct:str="mac", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSitesSle
+    API doc: https://doc.mist-lab.fr/#operation/countOrgWiredClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     QUERY PARAMS
     ------------
-    :param str sle(wan, wired, wifi)
+    :param str distinct(port_id, vlan, mac, device_mac, site_id, type)
+    :param int page
+    :param int limit
     :param int start
     :param int end
-    :param int limit
-    :param int page
-    :param str duration
-    :param str interval        
+    :param str duration        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/insights/sites-sle"
+    uri = f"/api/v1/orgs/{org_id}/wired_clients/count"
     query_params={}
-    if sle: query_params["sle"]=sle
+    if distinct: query_params["distinct"]=distinct
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
-    if duration: query_params["duration"]=duration
-    if interval: query_params["interval"]=interval
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgSle(mist_session:_APISession, org_id:str, metric:str, sle:str=None, duration:str="1d", interval:str=None, start:int=None, end:int=None) -> _APIResponse:
+def searchOrgWiredClients(mist_session:_APISession, org_id:str, site_id:str=None, device_mac:str=None, mac:str=None, port_id:str=None, vlan:int=None, ip:str=None, manufacture:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSle
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgWiredClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str metric        
+    :param str org_id        
     
     QUERY PARAMS
     ------------
-    :param str sle - see [/api/v1/const/insight_metrics](/#tag/Constants/operation/getSiteAvailableInsightMetrics) for more details
-    :param str duration
-    :param str interval
+    :param str site_id - Site ID
+    :param str device_mac - device mac
+    :param str mac - client mac
+    :param str port_id - port id
+    :param int vlan - vlan
+    :param str ip - ip
+    :param str manufacture - client manufacture
+    :param str text - single entry of hostname/mac
+    :param int limit
     :param int start
-    :param int end        
+    :param int end
+    :param str duration        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/insights/{metric}"
+    uri = f"/api/v1/orgs/{org_id}/wired_clients/search"
     query_params={}
-    if sle: query_params["sle"]=sle
-    if duration: query_params["duration"]=duration
-    if interval: query_params["interval"]=interval
+    if site_id: query_params["site_id"]=site_id
+    if device_mac: query_params["device_mac"]=device_mac
+    if mac: query_params["mac"]=mac
+    if port_id: query_params["port_id"]=port_id
+    if vlan: query_params["vlan"]=vlan
+    if ip: query_params["ip"]=ip
+    if manufacture: query_params["manufacture"]=manufacture
+    if text: query_params["text"]=text
+    if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
-    if end: query_params["end"]=end
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgJsiDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgJsiDevices")  
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -146,15 +146,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgJsiPastPurchases")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgJsiPastPurchases")  
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/logs.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgLogs")  
-def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgLogs")  
+def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:any=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
@@ -28,14 +28,15 @@
     :param str org_id        
     
     QUERY PARAMS
     ------------
     :param str site_id - site id
     :param str admin_name - admin name or email
     :param str message - message
+    :param any sort(timestamp, -timestamp, site_id, admin_id) - sort order
     :param int start
     :param int end
     :param int limit
     :param int page
     :param str duration        
     
     RETURN
@@ -43,23 +44,24 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/logs"
     query_params={}
     if site_id: query_params["site_id"]=site_id
     if admin_name: query_params["admin_name"]=admin_name
     if message: query_params["message"]=message
+    if sort: query_params["sort"]=sort
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
+def listOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:any=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
@@ -68,14 +70,15 @@
     :param str org_id        
     
     QUERY PARAMS
     ------------
     :param str site_id - site id
     :param str admin_name - admin name or email
     :param str message - message
+    :param any sort(timestamp, -timestamp, site_id, admin_id) - sort order
     :param int start
     :param int end
     :param int limit
     :param int page
     :param str duration        
     
     RETURN
@@ -83,14 +86,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/logs"
     query_params={}
     if site_id: query_params["site_id"]=site_id
     if admin_name: query_params["admin_name"]=admin_name
     if message: query_params["message"]=message
+    if sort: query_params["sort"]=sort
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/maps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdgeClusters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdgeClusters")  
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdges")  
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -167,15 +167,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdgeUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdgeUpgrades")  
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxTunnels")  
 def getOrgMxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNacRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNacRules")  
 def getOrgNacRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNacTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNacTags")  
 def getOrgNacTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNetworks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNetworks")  
 def getOrgNetworks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgNetworkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNetworkTemplates")  
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/assets.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,177 +10,191 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgOtherDevices")  
-def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAssets")  
+def getSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id        
     
-    QUERY PARAMS
-    ------------
-    :param str vendor
-    :param str mac
-    :param str serial
-    :param str model
-    :param str name
-    :param int page
-    :param int limit        
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/assets"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/otherdevices"
-    query_params={}
-    if vendor: query_params["vendor"]=vendor
-    if mac: query_params["mac"]=mac
-    if serial: query_params["serial"]=serial
-    if model: query_params["model"]=model
-    if name: query_params["name"]=name
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    uri = f"/api/v1/sites/{site_id}/assets"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def createSiteAsset(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
+    API doc: https://doc.mist-lab.fr/#operation/createSiteAsset
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id        
     
-    QUERY PARAMS
-    ------------
-    :param str vendor
-    :param str mac
-    :param str serial
-    :param str model
-    :param str name
-    :param int page
-    :param int limit        
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/otherdevices"
-    query_params={}
-    if vendor: query_params["vendor"]=vendor
-    if mac: query_params["mac"]=mac
-    if serial: query_params["serial"]=serial
-    if model: query_params["model"]=model
-    if name: query_params["name"]=name
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/assets"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def updateOrgOtherDevices(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def importSiteAssetsFile(mist_session:_APISession, site_id:str, file_path:str="") -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/importSiteAssets
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    BODY PARAMS
+    -----------
+    :param str file_path - path to the file to upload
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgOtherDevices
+    uri = f"/api/v1/sites/{site_id}/assets/import"
+    resp = mist_session.mist_post_file(uri=uri, file=file_path)
+    return resp
+
+def importSiteAssets(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/importSiteAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/otherdevices"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/assets/import"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgOtherDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
+def getSiteAsset(mist_session:_APISession, site_id:str, asset_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgOtherDevice
+    API doc: https://doc.mist-lab.fr/#operation/getSiteAsset
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str site_id
+    :param str asset_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/otherdevices/{device_mac}"
+    uri = f"/api/v1/sites/{site_id}/assets/{asset_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgOtherDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
+def deleteSiteAsset(mist_session:_APISession, site_id:str, asset_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgOtherDevice
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteAsset
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str site_id
+    :param str asset_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/otherdevices/{device_mac}"
+    uri = f"/api/v1/sites/{site_id}/assets/{asset_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgOtherDevice(mist_session:_APISession, org_id:str, device_mac:str, body:object) -> _APIResponse:
+def updateSiteAsset(mist_session:_APISession, site_id:str, asset_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgOtherDevice
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteAsset
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str site_id
+    :param str asset_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/otherdevices/{device_mac}"
+    uri = f"/api/v1/sites/{site_id}/assets/{asset_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/pma.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgPmaDashboards")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgPmaDashboards")  
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgPskPortals")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgPskPortals")  
 def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgPsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgPsks")  
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgRfTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgRfTemplates")  
 def getOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSdkInvites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSdkInvites")  
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSdkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSdkTemplates")  
 def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSecPolicies")  
 def getOrgSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgServicePolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgServicePolicies")  
 def getOrgServicePolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgServices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgServices")  
 def getOrgServices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def deleteOrgClientsBlocklist(mist_session:_APISession, org_id:str) -> _APIResponse:
+def deleteOrgWirelessClientsBlocklist(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgClientsBlocklist
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWirelessClientsBlocklist
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -76,17 +76,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/blacklist"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def createOrgClientsBlocklist(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgWirelessClientsBlocklist(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgClientsBlocklist
+    API doc: https://doc.mist-lab.fr/#operation/createOrgWirelessClientsBlocklist
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -100,14 +100,35 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/blacklist"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def deleteOrgCradlepointConnection(mist_session:_APISession, org_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgCradlepointConnection
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/setting/cradlepoint/setup"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
 def setupOrgCradlepointConnectionToMist(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/setupOrgCradlepointConnectionToMist
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSiteGroups")  
 def getOrgSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSites")  
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSiteTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSiteTemplates")  
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsoRoles")  
 def getOrgSsoRoles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsos")  
 def getOrgSsos(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -146,15 +146,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsoLatestFailures")  
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgSsrUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsrUpgrades")  
 def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAssetsStats")  
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -241,15 +241,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgDevicesStats")  
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -334,15 +334,15 @@
     if site_id: query_params["site_id"]=site_id
     if mac: query_params["mac"]=mac
     if evpntopo_id: query_params["evpntopo_id"]=evpntopo_id
     if evpn_unused: query_params["evpn_unused"]=evpn_unused
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdgesStats")  
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgTemplates")  
 def getOrgTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgTickets")  
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgsVpns")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgsVpns")  
 def getOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWebhooks")  
 def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,89 +10,95 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countOrgClientsWired(mist_session:_APISession, org_id:str, distinct:str="mac", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteClientsWired(mist_session:_APISession, site_id:str, distinct:str="mac", mac:str=None, device_mac:str=None, port_id:str=None, vlan:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgClientsWired
+    API doc: https://doc.mist-lab.fr/#operation/countSiteClientsWired
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param str distinct(port_id, vlan, mac, device_mac, site_id, type)
+    :param str distinct(port_id, vlan, mac)
+    :param str mac - client mac
+    :param str device_mac - device mac
+    :param str port_id - port id
+    :param str vlan - vlan
     :param int page
     :param int limit
     :param int start
     :param int end
     :param str duration        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wired_clients/count"
+    uri = f"/api/v1/sites/{site_id}/wired_clients/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
+    if mac: query_params["mac"]=mac
+    if device_mac: query_params["device_mac"]=device_mac
+    if port_id: query_params["port_id"]=port_id
+    if vlan: query_params["vlan"]=vlan
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgClientsWired(mist_session:_APISession, org_id:str, site_id:str=None, device_mac:str=None, mac:str=None, port_id:str=None, vlan:int=None, ip:str=None, manufacture:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteClientsWired(mist_session:_APISession, site_id:str, device_mac:str=None, mac:str=None, port_id:str=None, vlan:str=None, ip_address:str=None, manufacture:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgClientsWired
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteClientsWired
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param str site_id - Site ID
     :param str device_mac - device mac
     :param str mac - client mac
     :param str port_id - port id
-    :param int vlan - vlan
-    :param str ip - ip
-    :param str manufacture - client manufacture
+    :param str vlan - vlan
+    :param str ip_address
+    :param str manufacture - manufacture
     :param str text - single entry of hostname/mac
     :param int limit
     :param int start
     :param int end
     :param str duration        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wired_clients/search"
+    uri = f"/api/v1/sites/{site_id}/wired_clients/search"
     query_params={}
-    if site_id: query_params["site_id"]=site_id
     if device_mac: query_params["device_mac"]=device_mac
     if mac: query_params["mac"]=mac
     if port_id: query_params["port_id"]=port_id
     if vlan: query_params["vlan"]=vlan
-    if ip: query_params["ip"]=ip
+    if ip_address: query_params["ip_address"]=ip_address
     if manufacture: query_params["manufacture"]=manufacture
     if text: query_params["text"]=text
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWlans")  
 def getOrgWlans(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWxRules")  
 def getOrgWxRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWxTags")  
 def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listOrgWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWxTunnels")  
 def getOrgWxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.40.1/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.40.1/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/register/register.py` & `mistapi-0.40.1/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/register/verify.py` & `mistapi-0.40.1/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/apitokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApiTokens")  
 def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/logs.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSelfAuditLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSelfAuditLogs")  
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/self.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listAlarmSubscriptions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listAlarmSubscriptions")  
 def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/self/update.py` & `mistapi-0.40.1/src/mistapi/api/v1/self/update.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/site/deviceprofiles.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/deviceprofiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteDeviceProfilesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDeviceProfilesDerived")  
 def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -31,15 +31,15 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/deviceprofiles/derived"
+    uri = f"/api/v1/sites/{site_id}/deviceprofiles/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def listSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
@@ -57,13 +57,13 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/deviceprofiles/derived"
+    uri = f"/api/v1/sites/{site_id}/deviceprofiles/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/site/networks.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteNetworksDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteNetworksDerived")  
 def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -31,15 +31,15 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/networks/derived"
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def listSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
@@ -57,13 +57,13 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/networks/derived"
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/site/servicepolicies.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteServicePoliciesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteServicePoliciesDerived")  
 def getSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicePoliciesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -31,15 +31,15 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/servicepolicies/derived"
+    uri = f"/api/v1/sites/{site_id}/servicepolicies/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def listSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
@@ -57,13 +57,13 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/servicepolicies/derived"
+    uri = f"/api/v1/sites/{site_id}/servicepolicies/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/site/services.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteServicesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteServicesDerived")  
 def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -31,15 +31,15 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/services/derived"
+    uri = f"/api/v1/sites/{site_id}/services/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def listSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
@@ -57,13 +57,13 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/services/derived"
+    uri = f"/api/v1/sites/{site_id}/services/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/site/vpns.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/vpns.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteVpnsDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteVpnsDerived")  
 def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -31,15 +31,15 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/vpns/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def listSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
@@ -57,13 +57,13 @@
     ------------
     :param bool resolve - whether resolve the site variables        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/site/{site_id}/vpns/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,40 +15,47 @@
 from mistapi.api.v1.sites import anomaly
 from mistapi.api.v1.sites import apps
 from mistapi.api.v1.sites import assetfilters
 from mistapi.api.v1.sites import assets
 from mistapi.api.v1.sites import beacons
 from mistapi.api.v1.sites import call
 from mistapi.api.v1.sites import clients
+from mistapi.api.v1.sites import deviceprofiles
 from mistapi.api.v1.sites import devices
 from mistapi.api.v1.sites import events
 from mistapi.api.v1.sites import evpn_topologies
 from mistapi.api.v1.sites import guests
 from mistapi.api.v1.sites import insights
 from mistapi.api.v1.sites import licenses
 from mistapi.api.v1.sites import location
 from mistapi.api.v1.sites import maps
 from mistapi.api.v1.sites import mxedges
 from mistapi.api.v1.sites import mxtunnels
+from mistapi.api.v1.sites import networks
 from mistapi.api.v1.sites import otherdevices
 from mistapi.api.v1.sites import pcaps
 from mistapi.api.v1.sites import psks
 from mistapi.api.v1.sites import rfdiags
 from mistapi.api.v1.sites import rogues
 from mistapi.api.v1.sites import rrm
 from mistapi.api.v1.sites import rssizones
+from mistapi.api.v1.sites import servicepolicies
+from mistapi.api.v1.sites import services
 from mistapi.api.v1.sites import setting
 from mistapi.api.v1.sites import skyatp
 from mistapi.api.v1.sites import sle
 from mistapi.api.v1.sites import ssr
 from mistapi.api.v1.sites import stats
 from mistapi.api.v1.sites import subscriptions
 from mistapi.api.v1.sites import synthetic_test
 from mistapi.api.v1.sites import uisettings
 from mistapi.api.v1.sites import vbeacons
+from mistapi.api.v1.sites import vpns
+from mistapi.api.v1.sites import wan_client
+from mistapi.api.v1.sites import wan_clients
 from mistapi.api.v1.sites import webhooks
 from mistapi.api.v1.sites import wired_clients
 from mistapi.api.v1.sites import wlans
 from mistapi.api.v1.sites import wxrules
 from mistapi.api.v1.sites import wxtags
 from mistapi.api.v1.sites import wxtunnels
 from mistapi.api.v1.sites import zones
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteApps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteApps")  
 def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAssetFilters")  
 def getSiteAssetFilters(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,60 +10,60 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAssets")  
-def getSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWxRules")  
+def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/assets"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/assets"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteAsset(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteAsset
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -73,128 +73,101 @@
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/assets"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def importSiteAssetsFile(mist_session:_APISession, site_id:str, file_path:str="") -> _APIResponse:
+def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/importSiteAssets
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
-    BODY PARAMS
-    -----------
-    :param str file_path - path to the file to upload
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/assets/import"
-    resp = mist_session.mist_post_file(uri=uri, file=file_path)
-    return resp
-
-def importSiteAssets(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/importSiteAssets
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/assets/import"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteAsset(mist_session:_APISession, site_id:str, asset_id:str) -> _APIResponse:
+def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAsset
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str asset_id        
+    :param str wxrules_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/assets/{asset_id}"
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteAsset(mist_session:_APISession, site_id:str, asset_id:str) -> _APIResponse:
+def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteAsset
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str asset_id        
+    :param str wxrules_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/assets/{asset_id}"
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteAsset(mist_session:_APISession, site_id:str, asset_id:str, body:object) -> _APIResponse:
+def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteAsset
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str asset_id        
+    :param str wxrules_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/assets/{asset_id}"
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/beacons.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteBeacons")  
 def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/call.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteClients(mist_session:_APISession, site_id:str, distinct:str, ssid:str=None, ap:str=None, ip_address:str=None, vlan:str=None, hostname:str=None, os:str=None, model:str=None, device:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteWirelessClients(mist_session:_APISession, site_id:str, distinct:str, ssid:str=None, ap:str=None, ip_address:str=None, vlan:str=None, hostname:str=None, os:str=None, model:str=None, device:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteClients
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -86,17 +86,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/clients/disconnect"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def countSiteClientsEvents(mist_session:_APISession, site_id:str, distinct:str=None, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteWirelessClientsEvents(mist_session:_APISession, site_id:str, distinct:str=None, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteClientsEvents
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClientsEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -136,17 +136,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteClientsEvents(mist_session:_APISession, site_id:str, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteWirelessClientsEvents(mist_session:_APISession, site_id:str, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteClientsEvents
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClientsEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -182,17 +182,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteClientsWireless(mist_session:_APISession, site_id:str, mac:str=None, ip_address:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, ssid:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteWirelessClients(mist_session:_APISession, site_id:str, mac:str=None, ip_address:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, ssid:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteClientsWireless
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -232,17 +232,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteClientSessions(mist_session:_APISession, site_id:str, distinct:str="mac", ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteWirelessClientSessions(mist_session:_APISession, site_id:str, distinct:str="mac", ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteClientSessions
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClientSessions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -284,17 +284,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteClientWirelessSessions(mist_session:_APISession, site_id:str, ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_username:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, psk_id:str=None, psk_name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteWirelessClientSessions(mist_session:_APISession, site_id:str, ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_username:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, psk_id:str=None, psk_name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteClientWirelessSessions
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClientSessions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -362,17 +362,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/clients/unauthorize"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def disconnectSiteClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+def disconnectSiteWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/disconnectSiteClient
+    API doc: https://doc.mist-lab.fr/#operation/disconnectSiteWirelessClient
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -430,17 +430,17 @@
     if end: query_params["end"]=end
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def unauthorizeSiteClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+def unauthorizeSiteWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unauthorizeSiteClient
+    API doc: https://doc.mist-lab.fr/#operation/unauthorizeSiteWirelessClient
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/count.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDevices")  
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -673,15 +673,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAvailableDeviceVersions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAvailableDeviceVersions")  
 def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/events.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAllGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAllGuestAuthorizations")  
 def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteRogueAPs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteRogueAPs")  
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -159,15 +159,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteRogueClients")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteRogueClients")  
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/location.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteMaps")  
 def getSiteMaps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteMxEdges")  
 def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/visits.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,84 +10,50 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteOtherDevices")  
-def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def searchSiteZoneSessions(mist_session:_APISession, site_id:str, zone_type:str, user_type:str="client", user:str=None, scope_id:str=None, scope:str="site", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteZoneSessions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id        
+    :param str site_id
+    :param str zone_type(zones, rssizones)        
     
     QUERY PARAMS
     ------------
-    :param str vendor
-    :param str mac
-    :param str serial
-    :param str model
-    :param str name
+    :param str user_type(client, sdkclient, asset) - user type, client (default) / sdkclient / asset
+    :param str user - client MAC / Asset MAC / SDK UUID
+    :param str scope_id - if `scope`==`map`/`zone`/`rssizone`, the scope id
+    :param str scope(site, map, zone, rssizone) - scope
     :param int page
-    :param int limit        
+    :param int limit
+    :param int start
+    :param int end
+    :param str duration        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/otherdevices"
+    uri = f"/api/v1/sites/{site_id}/{zone_type}/visits/search"
     query_params={}
-    if vendor: query_params["vendor"]=vendor
-    if mac: query_params["mac"]=mac
-    if serial: query_params["serial"]=serial
-    if model: query_params["model"]=model
-    if name: query_params["name"]=name
+    if user_type: query_params["user_type"]=user_type
+    if user: query_params["user"]=user
+    if scope_id: query_params["scope_id"]=scope_id
+    if scope: query_params["scope"]=scope
     if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def listSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    QUERY PARAMS
-    ------------
-    :param str vendor
-    :param str mac
-    :param str serial
-    :param str model
-    :param str name
-    :param int page
-    :param int limit        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/otherdevices"
-    query_params={}
-    if vendor: query_params["vendor"]=vendor
-    if mac: query_params["mac"]=mac
-    if serial: query_params["serial"]=serial
-    if model: query_params["model"]=model
-    if name: query_params["name"]=name
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSitePacketCaptures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSitePacketCaptures")  
 def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSitePsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSitePsks")  
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/rogues.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rogues/{rogue_bssid}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deauthSiteClientsConnectedToARogue(mist_session:_APISession, site_id:str, rogue_bssid:str) -> _APIResponse:
+def deauthSiteWirelessClientsConnectedToARogue(mist_session:_APISession, site_id:str, rogue_bssid:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deauthSiteClientsConnectedToARogue
+    API doc: https://doc.mist-lab.fr/#operation/deauthSiteWirelessClientsConnectedToARogue
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/rrm.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteRssiZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteRssiZones")  
 def getSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/setting.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def deleteSiteClientsBlocklist(mist_session:_APISession, site_id:str) -> _APIResponse:
+def deleteSiteWirelessClientsBlocklist(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteClientsBlocklist
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWirelessClientsBlocklist
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -76,17 +76,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting/blacklist"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def createSiteClientsBlocklist(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWirelessClientsBlocklist(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteClientsBlocklist
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWirelessClientsBlocklist
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -145,17 +145,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting/watched_station"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def deleteSiteClientsAllowlist(mist_session:_APISession, site_id:str) -> _APIResponse:
+def deleteSiteWirelessClientsAllowlist(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteClientsAllowlist
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWirelessClientsAllowlist
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -166,17 +166,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting/whitelist"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def createSiteClientsAllowlist(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWirelessClientsAllowlist(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteClientsAllowlist
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWirelessClientsAllowlist
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/sites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/sle.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,54 +10,48 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteSsrUpgrade(mist_session:_APISession, site_id:str, upgrade_id:str) -> _APIResponse:
+def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSsrUpgrade
+    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id
-    :param str upgrade_id        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/ssr/upgrade/{upgrade_id}"
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def upgradeSiteSsr(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/upgradeSiteSsr
+    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id
-    :param str device_id        
-    
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/ssr/{device_id}/upgrade"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAssetsStats")  
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -248,15 +248,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteBeaconsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteBeaconsStats")  
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -436,18 +436,18 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteClientsStats")  
-def getSiteClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWirelessClientsStats")  
+def getSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteClientsStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -463,17 +463,17 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
+def listSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteClientsStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -489,17 +489,17 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteClientStats(mist_session:_APISession, site_id:str, client_mac:str, wired:bool=None) -> _APIResponse:
+def getSiteWirelessClientStats(mist_session:_APISession, site_id:str, client_mac:str, wired:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteClientStats
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWirelessClientStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -516,15 +516,15 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDevicesStats")  
 def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -625,15 +625,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteDiscoveredAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDiscoveredAssets")  
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -893,17 +893,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/gateways/metrics"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteClientsStatsByMap(mist_session:_APISession, site_id:str, map_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def getSiteWirelessClientsStatsByMap(mist_session:_APISession, site_id:str, map_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteClientsStatsByMap
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWirelessClientsStatsByMap
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -972,15 +972,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteUnconnectedClientStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteUnconnectedClientStats")  
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -1017,15 +1017,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteMxEdgesStats")  
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -1519,15 +1519,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteZonesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteZonesStats")  
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,48 +10,52 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
     query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
+    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/wan_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,52 +10,33 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
+def countSiteWanClientEvents(mist_session:_APISession, site_id:str, distinct:str="type") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWanClientEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    :param str distinct(type, hostname, ip, mfg, mac)        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wan_client/events/count"
+    query_params={}
+    if distinct: query_params["distinct"]=distinct
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/uisettings.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteVBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteVBeacons")  
 def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWebhooks")  
 def getSiteWebhooks(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/wan_clients.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,97 +10,129 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteClientsWired(mist_session:_APISession, site_id:str, distinct:str="mac", mac:str=None, device_mac:str=None, port_id:str=None, vlan:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteWanClients(mist_session:_APISession, site_id:str, distinct:str="mac", start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteClientsWired
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWanClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param str distinct(port_id, vlan, mac)
-    :param str mac - client mac
-    :param str device_mac - device mac
-    :param str port_id - port id
-    :param str vlan - vlan
-    :param int page
-    :param int limit
+    :param str distinct(hostname, ip, mfg, mac)
     :param int start
     :param int end
-    :param str duration        
+    :param str duration
+    :param int limit
+    :param int page        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wired_clients/count"
+    uri = f"/api/v1/sites/{site_id}/wan_clients/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
-    if mac: query_params["mac"]=mac
-    if device_mac: query_params["device_mac"]=device_mac
-    if port_id: query_params["port_id"]=port_id
-    if vlan: query_params["vlan"]=vlan
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteClientsWired(mist_session:_APISession, site_id:str, device_mac:str=None, mac:str=None, port_id:str=None, vlan:str=None, ip_address:str=None, manufacture:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteWanClientsEvents(mist_session:_APISession, site_id:str, type:str=None, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteClientsWired
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWanClientsEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     QUERY PARAMS
     ------------
-    :param str device_mac - device mac
-    :param str mac - client mac
-    :param str port_id - port id
-    :param str vlan - vlan
-    :param str ip_address
-    :param str manufacture - manufacture
-    :param str text - single entry of hostname/mac
-    :param int limit
+    :param str type - Event type, e.g. CLIENT_IP_ASSIGNED, CLIENT_IP_RENEWED, CLIENT_IP_EXPIRED
+    :param str mac - partial / full MAC address
+    :param str hostname - partial / full hostname
+    :param str ip - client IP
+    :param str mfg - Manufacture
     :param int start
     :param int end
-    :param str duration        
+    :param str duration
+    :param int limit
+    :param int page        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wired_clients/search"
+    uri = f"/api/v1/sites/{site_id}/wan_clients/events/search"
     query_params={}
-    if device_mac: query_params["device_mac"]=device_mac
+    if type: query_params["type"]=type
     if mac: query_params["mac"]=mac
-    if port_id: query_params["port_id"]=port_id
-    if vlan: query_params["vlan"]=vlan
-    if ip_address: query_params["ip_address"]=ip_address
-    if manufacture: query_params["manufacture"]=manufacture
-    if text: query_params["text"]=text
+    if hostname: query_params["hostname"]=hostname
+    if ip: query_params["ip"]=ip
+    if mfg: query_params["mfg"]=mfg
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def searchSiteWanClients(mist_session:_APISession, site_id:str, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWanClients
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    QUERY PARAMS
+    ------------
+    :param str mac - partial / full MAC address
+    :param str hostname - partial / full hostname
+    :param str ip - client IP
+    :param str mfg - Manufacture
+    :param int start
+    :param int end
+    :param str duration
+    :param int limit
+    :param int page        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wan_clients/search"
+    query_params={}
+    if mac: query_params["mac"]=mac
+    if hostname: query_params["hostname"]=hostname
+    if ip: query_params["ip"]=ip
+    if mfg: query_params["mfg"]=mfg
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/wlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWlans")  
 def getSiteWlans(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,60 +10,60 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWxRules")  
-def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWxTunnels")  
+def getSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWxTunnel(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -73,101 +73,80 @@
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str wxtunnel_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+def deleteSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str wxtunnel_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
+def updateSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str wxtunnel_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWxTags")  
 def getSiteWxTags(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.40.1/src/mistapi/api/v1/sites/zones.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,60 +10,60 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteWxTunnels")  
-def getSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteZones")  
+def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxTunnel(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -73,80 +73,80 @@
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    uri = f"/api/v1/sites/{site_id}/zones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
+def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxtunnel_id        
+    :param str zone_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
+def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxtunnel_id        
+    :param str zone_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str, body:object) -> _APIResponse:
+def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxtunnel_id        
+    :param str zone_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/sites/zones.py` & `mistapi-0.40.1/src/mistapi/api/v1/orgs/wan_clients.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,143 +10,129 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.0", details="function replaced with listSiteZones")  
-def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
+def countOrgWanClients(mist_session:_APISession, org_id:str, distinct:str="mac", start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
+    API doc: https://doc.mist-lab.fr/#operation/countOrgWanClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id        
+    :param str org_id        
     
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/zones"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def listSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
+    QUERY PARAMS
+    ------------
+    :param str distinct(hostname, ip, mfg, mac)
+    :param int start
+    :param int end
+    :param str duration
+    :param int limit
+    :param int page        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/wan_clients/count"
+    query_params={}
+    if distinct: query_params["distinct"]=distinct
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def searchOrgWanClientsEvents(mist_session:_APISession, org_id:str, type:str=None, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgWanClientsEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id        
-    
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/zones"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
-    
-def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
+    :param str org_id        
     
-    PATH PARAMS
-    -----------
-    :param str site_id
-    :param str zone_id        
+    QUERY PARAMS
+    ------------
+    :param str type - Event type, e.g. CLIENT_IP_ASSIGNED, CLIENT_IP_RENEWED, CLIENT_IP_EXPIRED
+    :param str mac - partial / full MAC address
+    :param str hostname - partial / full hostname
+    :param str ip - client IP
+    :param str mfg - Manufacture
+    :param int start
+    :param int end
+    :param str duration
+    :param int limit
+    :param int page        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/wan_clients/events/search"
+    query_params={}
+    if type: query_params["type"]=type
+    if mac: query_params["mac"]=mac
+    if hostname: query_params["hostname"]=hostname
+    if ip: query_params["ip"]=ip
+    if mfg: query_params["mfg"]=mfg
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id
-    :param str zone_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
+def searchOrgWanClients(mist_session:_APISession, org_id:str, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgWanClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id
-    :param str zone_id        
+    :param str org_id        
     
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    :param str mac - partial / full MAC address
+    :param str hostname - partial / full hostname
+    :param str ip - client IP
+    :param str mfg - Manufacture
+    :param int start
+    :param int end
+    :param str duration
+    :param int limit
+    :param int page        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/wan_clients/search"
+    query_params={}
+    if mac: query_params["mac"]=mac
+    if hostname: query_params["hostname"]=hostname
+    if ip: query_params["ip"]=ip
+    if mfg: query_params["mfg"]=mfg
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.40.1/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.40.1/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.0/src/mistapi/cli.py` & `mistapi-0.40.1/src/mistapi/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,17 +84,19 @@
         msp_accounts = sorted(msp_accounts, key=lambda x: x["name"].lower())
         while True:
             i = -1
             print("\r\nAvailable MSP Accounts:")
             for privilege in msp_accounts:
                 i += 1
                 print(f"{i}) {privilege['name']} (id: {privilege['msp_id']})")
-
+            print()
+            print("n) Non-MSP Orgs")
+            print()
             resp = input(
-                f'\r\nSelect the MSP Account to use (0 to {i}, "n" for None, or "q" to quit): '
+                f'\r\nSelect the MSP Account to use (0 to {i}, "n" to access Orgs not attached to an MSP Account, or "q" to quit): '
             )
             if resp == "q":
                 sys.exit(0)
             elif resp.lower() == "n":
                 return [priv for priv in mist_session.privileges if not priv.get("msp_id")]
             else:
                 tested_val = _test_choice(resp, i)
```

### Comparing `mistapi-0.40.0/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.40.1/src/mistapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.40.0
+Version: 0.40.1
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
@@ -77,15 +77,14 @@
 LOGGING_LOG_LEVEL | int | 10 | The minimum log level to log on the file, using `logging` schema (0 = Disabled, 10 = Debug, 20 = Info, 30 = Warning, 40 = Error, 50 = Critical). This is only used when the script calling `mistapi` is using Python `logging` package and is configured to log to a file |
 
 
 An example of the environment file content is:
 ```
 MIST_HOST = api.mist.com
 MIST_APITOKEN = xxxxxx
-MIST_ORG_ID = 203d3d02-xxxx-xxxx-xxxx-76896a3330f4
 ```
 
 ## Usage
 Usage examples are available in the [mist_library repository](https://github.com/tmunzer/mist_library).
 
 To use it, 
 ### 1. `APISession` must be instanciated:
```

### Comparing `mistapi-0.40.0/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.40.1/src/mistapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 src/mistapi/api/v1/const/device_events.py
 src/mistapi/api/v1/const/device_models.py
 src/mistapi/api/v1/const/insight_metrics.py
 src/mistapi/api/v1/const/languages.py
 src/mistapi/api/v1/const/license_types.py
 src/mistapi/api/v1/const/mxedge_events.py
 src/mistapi/api/v1/const/mxedge_models.py
+src/mistapi/api/v1/const/other_device_events.py
 src/mistapi/api/v1/const/traffic_types.py
 src/mistapi/api/v1/installer/__init__.py
 src/mistapi/api/v1/installer/orgs/__init__.py
 src/mistapi/api/v1/installer/orgs/alarmtemplates.py
 src/mistapi/api/v1/installer/orgs/deviceprofiles.py
 src/mistapi/api/v1/installer/orgs/devices.py
 src/mistapi/api/v1/installer/orgs/rftemplates.py
@@ -130,14 +131,16 @@
 src/mistapi/api/v1/orgs/ssr.py
 src/mistapi/api/v1/orgs/stats.py
 src/mistapi/api/v1/orgs/subscriptions.py
 src/mistapi/api/v1/orgs/templates.py
 src/mistapi/api/v1/orgs/tickets.py
 src/mistapi/api/v1/orgs/troubleshoot.py
 src/mistapi/api/v1/orgs/vpns.py
+src/mistapi/api/v1/orgs/wan_client.py
+src/mistapi/api/v1/orgs/wan_clients.py
 src/mistapi/api/v1/orgs/webhooks.py
 src/mistapi/api/v1/orgs/wired_clients.py
 src/mistapi/api/v1/orgs/wlans.py
 src/mistapi/api/v1/orgs/wxrules.py
 src/mistapi/api/v1/orgs/wxtags.py
 src/mistapi/api/v1/orgs/wxtunnels.py
 src/mistapi/api/v1/recover/__init__.py
@@ -150,58 +153,59 @@
 src/mistapi/api/v1/self/apitokens.py
 src/mistapi/api/v1/self/logs.py
 src/mistapi/api/v1/self/oauth.py
 src/mistapi/api/v1/self/self.py
 src/mistapi/api/v1/self/subscriptions.py
 src/mistapi/api/v1/self/two_factor.py
 src/mistapi/api/v1/self/update.py
-src/mistapi/api/v1/site/__init__.py
-src/mistapi/api/v1/site/deviceprofiles.py
-src/mistapi/api/v1/site/networks.py
-src/mistapi/api/v1/site/servicepolicies.py
-src/mistapi/api/v1/site/services.py
-src/mistapi/api/v1/site/vpns.py
 src/mistapi/api/v1/sites/__init__.py
 src/mistapi/api/v1/sites/alarms.py
 src/mistapi/api/v1/sites/anomaly.py
 src/mistapi/api/v1/sites/apps.py
 src/mistapi/api/v1/sites/assetfilters.py
 src/mistapi/api/v1/sites/assets.py
 src/mistapi/api/v1/sites/beacons.py
 src/mistapi/api/v1/sites/call.py
 src/mistapi/api/v1/sites/clients.py
 src/mistapi/api/v1/sites/count.py
+src/mistapi/api/v1/sites/deviceprofiles.py
 src/mistapi/api/v1/sites/devices.py
 src/mistapi/api/v1/sites/events.py
 src/mistapi/api/v1/sites/evpn_topologies.py
 src/mistapi/api/v1/sites/guests.py
 src/mistapi/api/v1/sites/insights.py
 src/mistapi/api/v1/sites/licenses.py
 src/mistapi/api/v1/sites/location.py
 src/mistapi/api/v1/sites/maps.py
 src/mistapi/api/v1/sites/mxedges.py
 src/mistapi/api/v1/sites/mxtunnels.py
+src/mistapi/api/v1/sites/networks.py
 src/mistapi/api/v1/sites/otherdevices.py
 src/mistapi/api/v1/sites/pcaps.py
 src/mistapi/api/v1/sites/psks.py
 src/mistapi/api/v1/sites/rfdiags.py
 src/mistapi/api/v1/sites/rogues.py
 src/mistapi/api/v1/sites/rrm.py
 src/mistapi/api/v1/sites/rssizones.py
+src/mistapi/api/v1/sites/servicepolicies.py
+src/mistapi/api/v1/sites/services.py
 src/mistapi/api/v1/sites/setting.py
 src/mistapi/api/v1/sites/sites.py
 src/mistapi/api/v1/sites/skyatp.py
 src/mistapi/api/v1/sites/sle.py
 src/mistapi/api/v1/sites/ssr.py
 src/mistapi/api/v1/sites/stats.py
 src/mistapi/api/v1/sites/subscriptions.py
 src/mistapi/api/v1/sites/synthetic_test.py
 src/mistapi/api/v1/sites/uisettings.py
 src/mistapi/api/v1/sites/vbeacons.py
 src/mistapi/api/v1/sites/visits.py
+src/mistapi/api/v1/sites/vpns.py
+src/mistapi/api/v1/sites/wan_client.py
+src/mistapi/api/v1/sites/wan_clients.py
 src/mistapi/api/v1/sites/webhooks.py
 src/mistapi/api/v1/sites/wired_clients.py
 src/mistapi/api/v1/sites/wlans.py
 src/mistapi/api/v1/sites/wxrules.py
 src/mistapi/api/v1/sites/wxtags.py
 src/mistapi/api/v1/sites/wxtunnels.py
 src/mistapi/api/v1/sites/zones.py
```

