# Comparing `tmp/duffy-3.3.5.tar.gz` & `tmp/duffy-3.3.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duffy-3.3.5.tar", max compression
+gzip compressed data, was "duffy-3.3.6rc1.tar", max compression
```

## Comparing `duffy-3.3.5.tar` & `duffy-3.3.6rc1.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0     1062 2022-04-01 09:18:05.729280 duffy-3.3.5/LICENSE
--rw-r--r--   0        0        0     2614 2022-03-17 11:36:00.362316 duffy-3.3.5/README.md
--rw-r--r--   0        0        0        0 2021-11-04 19:37:25.052374 duffy-3.3.5/duffy/__init__.py
--rw-r--r--   0        0        0     3797 2022-09-02 11:03:33.423166 duffy-3.3.5/duffy/admin.py
--rw-r--r--   0        0        0      763 2022-06-08 11:41:51.292538 duffy-3.3.5/duffy/api_models/__init__.py
--rw-r--r--   0        0        0      438 2022-05-05 09:39:16.752260 duffy-3.3.5/duffy/api_models/common.py
--rw-r--r--   0        0        0      901 2022-07-28 13:53:12.030479 duffy-3.3.5/duffy/api_models/node.py
--rw-r--r--   0        0        0      785 2022-07-28 13:53:12.031479 duffy-3.3.5/duffy/api_models/pool.py
--rw-r--r--   0        0        0     1276 2022-07-28 13:53:12.031479 duffy-3.3.5/duffy/api_models/session.py
--rw-r--r--   0        0        0     2168 2022-07-28 13:53:12.031479 duffy-3.3.5/duffy/api_models/tenant.py
--rw-r--r--   0        0        0        0 2021-11-04 19:37:25.053374 duffy-3.3.5/duffy/app/__init__.py
--rw-r--r--   0        0        0     1478 2021-12-23 11:53:40.419878 duffy-3.3.5/duffy/app/auth.py
--rw-r--r--   0        0        0        0 2021-12-09 12:35:44.361777 duffy-3.3.5/duffy/app/controllers/__init__.py
--rw-r--r--   0        0        0     2393 2022-08-03 14:42:56.259909 duffy-3.3.5/duffy/app/controllers/node.py
--rw-r--r--   0        0        0     2003 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/app/controllers/pool.py
--rw-r--r--   0        0        0    12176 2022-08-18 14:10:01.718566 duffy-3.3.5/duffy/app/controllers/session.py
--rw-r--r--   0        0        0     5820 2022-08-03 14:42:56.260908 duffy-3.3.5/duffy/app/controllers/tenant.py
--rw-r--r--   0        0        0      438 2022-08-03 14:42:56.260908 duffy-3.3.5/duffy/app/database.py
--rw-r--r--   0        0        0     1763 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/app/main.py
--rw-r--r--   0        0        0     1301 2022-08-18 14:10:01.719566 duffy-3.3.5/duffy/app/util.py
--rw-r--r--   0        0        0    22150 2022-07-04 10:55:12.946674 duffy-3.3.5/duffy/cli.py
--rw-r--r--   0        0        0       96 2022-06-02 11:13:08.951670 duffy-3.3.5/duffy/client/__init__.py
--rw-r--r--   0        0        0     4287 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/client/formatter.py
--rw-r--r--   0        0        0     4201 2022-08-19 09:32:26.820891 duffy-3.3.5/duffy/client/main.py
--rw-r--r--   0        0        0       71 2022-08-18 14:10:01.719566 duffy-3.3.5/duffy/configuration/__init__.py
--rw-r--r--   0        0        0     1736 2022-08-18 14:10:01.719566 duffy-3.3.5/duffy/configuration/main.py
--rw-r--r--   0        0        0     4804 2022-08-18 14:10:01.719566 duffy-3.3.5/duffy/configuration/validation.py
--rw-r--r--   0        0        0     2995 2022-09-02 09:08:44.309862 duffy-3.3.5/duffy/database/__init__.py
--rw-r--r--   0        0        0     1840 2022-02-14 16:30:16.414977 duffy-3.3.5/duffy/database/migrations/env.py
--rw-r--r--   0        0        0     2512 2022-05-12 07:53:02.330179 duffy-3.3.5/duffy/database/migrations/main.py
--rw-r--r--   0        0        0      530 2022-02-23 17:54:04.381223 duffy-3.3.5/duffy/database/migrations/script.py.mako
--rw-r--r--   0        0        0        0 2021-11-23 15:11:13.761517 duffy-3.3.5/duffy/database/migrations/versions/.empty
--rw-r--r--   0        0        0      611 2022-05-10 10:52:20.877943 duffy-3.3.5/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py
--rw-r--r--   0        0        0      134 2022-01-31 09:33:13.840537 duffy-3.3.5/duffy/database/model/__init__.py
--rw-r--r--   0        0        0     3032 2022-04-27 13:45:27.188353 duffy-3.3.5/duffy/database/model/node.py
--rw-r--r--   0        0        0     1082 2022-03-14 11:18:18.016981 duffy-3.3.5/duffy/database/model/session.py
--rw-r--r--   0        0        0     2851 2022-05-10 09:53:08.291828 duffy-3.3.5/duffy/database/model/tenant.py
--rw-r--r--   0        0        0     3811 2022-05-05 12:09:52.332014 duffy-3.3.5/duffy/database/setup.py
--rw-r--r--   0        0        0      281 2022-02-14 16:30:16.414977 duffy-3.3.5/duffy/database/types.py
--rw-r--r--   0        0        0     4590 2022-08-18 14:10:01.719566 duffy-3.3.5/duffy/database/util.py
--rw-r--r--   0        0        0      358 2021-11-24 14:21:28.066307 duffy-3.3.5/duffy/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-07 13:59:09.420061 duffy-3.3.5/duffy/legacy/__init__.py
--rw-r--r--   0        0        0       99 2022-02-07 13:59:09.420061 duffy-3.3.5/duffy/legacy/api_models.py
--rw-r--r--   0        0        0      949 2022-02-07 13:59:09.420061 duffy-3.3.5/duffy/legacy/auth.py
--rw-r--r--   0        0        0     8273 2022-08-03 14:42:56.260908 duffy-3.3.5/duffy/legacy/main.py
--rw-r--r--   0        0        0     3163 2022-08-03 14:42:56.260908 duffy-3.3.5/duffy/misc.py
--rw-r--r--   0        0        0        0 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/nodes/__init__.py
--rw-r--r--   0        0        0     2862 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/nodes/context.py
--rw-r--r--   0        0        0      102 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/nodes/mechanisms/__init__.py
--rw-r--r--   0        0        0     4076 2022-08-18 14:10:01.719566 duffy-3.3.5/duffy/nodes/mechanisms/ansible.py
--rw-r--r--   0        0        0     1211 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/nodes/mechanisms/main.py
--rw-r--r--   0        0        0     3856 2022-06-08 11:41:51.293538 duffy-3.3.5/duffy/nodes/pools.py
--rw-r--r--   0        0        0     2175 2022-05-03 12:14:31.685232 duffy-3.3.5/duffy/shell.py
--rw-r--r--   0        0        0      293 2022-03-14 11:18:18.016981 duffy-3.3.5/duffy/tasks/__init__.py
--rw-r--r--   0        0        0      171 2022-02-14 16:30:16.414977 duffy-3.3.5/duffy/tasks/base.py
--rw-r--r--   0        0        0     7168 2022-08-03 14:12:48.490273 duffy-3.3.5/duffy/tasks/deprovision.py
--rw-r--r--   0        0        0     1221 2022-03-15 09:19:01.122691 duffy-3.3.5/duffy/tasks/expire.py
--rw-r--r--   0        0        0      417 2022-03-15 09:19:01.122691 duffy-3.3.5/duffy/tasks/locking.py
--rw-r--r--   0        0        0     1326 2022-06-08 11:41:51.294538 duffy-3.3.5/duffy/tasks/main.py
--rw-r--r--   0        0        0    11136 2022-06-08 11:41:51.294538 duffy-3.3.5/duffy/tasks/provision.py
--rw-r--r--   0        0        0     7004 2022-08-18 14:10:01.719566 duffy-3.3.5/duffy/util.py
--rw-r--r--   0        0        0       72 2022-05-24 14:34:15.807836 duffy-3.3.5/duffy/version.py
--rw-r--r--   0        0        0     4319 2022-09-02 12:59:08.771232 duffy-3.3.5/pyproject.toml
--rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 duffy-3.3.5/setup.py
--rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 duffy-3.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-04-01 09:18:05.729280 duffy-3.3.6rc1/LICENSE
+-rw-r--r--   0        0        0     2614 2022-03-17 11:36:00.362316 duffy-3.3.6rc1/README.md
+-rw-r--r--   0        0        0        0 2021-11-04 19:37:25.052374 duffy-3.3.6rc1/duffy/__init__.py
+-rw-r--r--   0        0        0     3797 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/admin.py
+-rw-r--r--   0        0        0      763 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/__init__.py
+-rw-r--r--   0        0        0      438 2022-05-05 09:39:16.752260 duffy-3.3.6rc1/duffy/api_models/common.py
+-rw-r--r--   0        0        0      901 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/node.py
+-rw-r--r--   0        0        0      785 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/pool.py
+-rw-r--r--   0        0        0     1276 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/session.py
+-rw-r--r--   0        0        0     2168 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/tenant.py
+-rw-r--r--   0        0        0        0 2021-11-04 19:37:25.053374 duffy-3.3.6rc1/duffy/app/__init__.py
+-rw-r--r--   0        0        0     1478 2021-12-23 11:53:40.419878 duffy-3.3.6rc1/duffy/app/auth.py
+-rw-r--r--   0        0        0        0 2021-12-09 12:35:44.361777 duffy-3.3.6rc1/duffy/app/controllers/__init__.py
+-rw-r--r--   0        0        0     2393 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/node.py
+-rw-r--r--   0        0        0     2003 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/pool.py
+-rw-r--r--   0        0        0    13631 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/session.py
+-rw-r--r--   0        0        0     5820 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/tenant.py
+-rw-r--r--   0        0        0      438 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/database.py
+-rw-r--r--   0        0        0     1763 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/app/main.py
+-rw-r--r--   0        0        0     1301 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/app/util.py
+-rw-r--r--   0        0        0    22150 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/cli.py
+-rw-r--r--   0        0        0       96 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/client/__init__.py
+-rw-r--r--   0        0        0     4287 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/client/formatter.py
+-rw-r--r--   0        0        0     4201 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/client/main.py
+-rw-r--r--   0        0        0       71 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/configuration/__init__.py
+-rw-r--r--   0        0        0     1736 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/configuration/main.py
+-rw-r--r--   0        0        0     4804 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/configuration/validation.py
+-rw-r--r--   0        0        0     2675 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/database/__init__.py
+-rw-r--r--   0        0        0     1840 2022-02-14 16:30:16.414977 duffy-3.3.6rc1/duffy/database/migrations/env.py
+-rw-r--r--   0        0        0     2512 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/database/migrations/main.py
+-rw-r--r--   0        0        0      530 2022-02-23 17:54:04.381223 duffy-3.3.6rc1/duffy/database/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2021-11-23 15:11:13.761517 duffy-3.3.6rc1/duffy/database/migrations/versions/.empty
+-rw-r--r--   0        0        0      611 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py
+-rw-r--r--   0        0        0      134 2022-01-31 09:33:13.840537 duffy-3.3.6rc1/duffy/database/model/__init__.py
+-rw-r--r--   0        0        0     3032 2023-04-17 12:35:31.798781 duffy-3.3.6rc1/duffy/database/model/node.py
+-rw-r--r--   0        0        0     1082 2022-03-14 11:18:18.016981 duffy-3.3.6rc1/duffy/database/model/session.py
+-rw-r--r--   0        0        0     2845 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/database/model/tenant.py
+-rw-r--r--   0        0        0     3811 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/database/setup.py
+-rw-r--r--   0        0        0      281 2022-02-14 16:30:16.414977 duffy-3.3.6rc1/duffy/database/types.py
+-rw-r--r--   0        0        0     4590 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/database/util.py
+-rw-r--r--   0        0        0      358 2021-11-24 14:21:28.066307 duffy-3.3.6rc1/duffy/exceptions.py
+-rw-r--r--   0        0        0        0 2022-02-07 13:59:09.420061 duffy-3.3.6rc1/duffy/legacy/__init__.py
+-rw-r--r--   0        0        0       99 2022-02-07 13:59:09.420061 duffy-3.3.6rc1/duffy/legacy/api_models.py
+-rw-r--r--   0        0        0      949 2022-02-07 13:59:09.420061 duffy-3.3.6rc1/duffy/legacy/auth.py
+-rw-r--r--   0        0        0     8273 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/legacy/main.py
+-rw-r--r--   0        0        0     3163 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/misc.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/__init__.py
+-rw-r--r--   0        0        0     2862 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/context.py
+-rw-r--r--   0        0        0      102 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/mechanisms/__init__.py
+-rw-r--r--   0        0        0     4076 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/mechanisms/ansible.py
+-rw-r--r--   0        0        0     1210 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/mechanisms/main.py
+-rw-r--r--   0        0        0     3855 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/pools.py
+-rw-r--r--   0        0        0     2175 2022-05-03 12:14:31.685232 duffy-3.3.6rc1/duffy/shell.py
+-rw-r--r--   0        0        0      293 2022-03-14 11:18:18.016981 duffy-3.3.6rc1/duffy/tasks/__init__.py
+-rw-r--r--   0        0        0      171 2022-02-14 16:30:16.414977 duffy-3.3.6rc1/duffy/tasks/base.py
+-rw-r--r--   0        0        0     7168 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/tasks/deprovision.py
+-rw-r--r--   0        0        0     1221 2022-03-15 09:19:01.122691 duffy-3.3.6rc1/duffy/tasks/expire.py
+-rw-r--r--   0        0        0      417 2022-03-15 09:19:01.122691 duffy-3.3.6rc1/duffy/tasks/locking.py
+-rw-r--r--   0        0        0     1326 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/tasks/main.py
+-rw-r--r--   0        0        0    11136 2023-06-13 10:45:34.120491 duffy-3.3.6rc1/duffy/tasks/provision.py
+-rw-r--r--   0        0        0     7004 2023-06-13 10:45:34.120491 duffy-3.3.6rc1/duffy/util.py
+-rw-r--r--   0        0        0       72 2023-06-13 10:45:34.120491 duffy-3.3.6rc1/duffy/version.py
+-rw-r--r--   0        0        0     4299 2023-06-13 11:10:33.330273 duffy-3.3.6rc1/pyproject.toml
+-rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 duffy-3.3.6rc1/PKG-INFO
```

### Comparing `duffy-3.3.5/LICENSE` & `duffy-3.3.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/README.md` & `duffy-3.3.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/admin.py` & `duffy-3.3.6rc1/duffy/admin.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/api_models/__init__.py` & `duffy-3.3.6rc1/duffy/api_models/__init__.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/api_models/node.py` & `duffy-3.3.6rc1/duffy/api_models/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/api_models/pool.py` & `duffy-3.3.6rc1/duffy/api_models/pool.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/api_models/session.py` & `duffy-3.3.6rc1/duffy/api_models/session.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/api_models/tenant.py` & `duffy-3.3.6rc1/duffy/api_models/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/app/auth.py` & `duffy-3.3.6rc1/duffy/app/auth.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/app/controllers/node.py` & `duffy-3.3.6rc1/duffy/app/controllers/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/app/controllers/pool.py` & `duffy-3.3.6rc1/duffy/app/controllers/pool.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/app/controllers/session.py` & `duffy-3.3.6rc1/duffy/app/controllers/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     # Save tenant id to enable reloading it on retries
     tenant_id = tenant.id
 
     async with SerializationErrorRetryContext() as retry:
         async for attempt in retry.attempts:
             try:
-                if attempt > 1:
+                if attempt > 1:  # pragma: without-xdist
                     tenant = (
                         await db_async_session.execute(select(Tenant).filter_by(id=tenant_id))
                     ).scalar_one()
                 session = Session(
                     tenant=tenant,
                     data={"nodes_specs": [spec.dict() for spec in data.nodes_specs]},
                     expires_at=(
@@ -179,85 +179,117 @@
                         node.data["nodes_spec"] = nodes_spec.dict()
                         node.state = NodeState.contextualizing
                         session_node = SessionNode(
                             session=session, node=node, pool=nodes_spec.pool, data=node.data
                         )
                         session_nodes.append(session_node)
                         db_async_session.add(session_node)
-            except retry.exceptions as exc:
+                await db_async_session.commit()
+            except retry.exceptions as exc:  # pragma: without-xdist
                 retry.process_exception(exc)
                 await db_async_session.rollback()
 
+    # Sort the nodes so this one and dependent lists can be reloaded in one go.
+    nodes_in_transaction = sorted(nodes_in_transaction, key=lambda node: node.id)
+
     contextualized_ipaddrs = await contextualize(
         nodes=[node.ipaddr for node in nodes_in_transaction], ssh_pubkey=tenant.ssh_key
     )
 
     if None in contextualized_ipaddrs:
         # Undo the session object being added to the database above.
         for session_node in session_nodes:
             db_async_session.expunge(session_node)
         db_async_session.expunge(session)
 
         log.error("One or more nodes couldn't be contextualized:")
         nodes_to_decontextualize = []
         for node, ipaddr in zip(nodes_in_transaction, contextualized_ipaddrs):
             if not ipaddr:
-                log.error("    id: %s hostname: %s ipaddr: %s", node.id, node.hostname, node.ipaddr)
+                log.error(
+                    "    id: %s hostname: %s ipaddr: %s",
+                    node.id,
+                    node.hostname,
+                    node.ipaddr,
+                )
                 node.fail("contextualizing node failed")
             else:
                 nodes_to_decontextualize.append(node)
 
         decontextualized_ipaddrs = await decontextualize(
             nodes=[node.ipaddr for node in nodes_to_decontextualize]
         )
 
-        if None in decontextualized_ipaddrs:
-            log.error("One or more nodes couldn't be decontextualized:")
-            for node, ipaddr in zip(nodes_to_decontextualize, decontextualized_ipaddrs):
-                if not ipaddr:
-                    log.error(
-                        "    id: %s hostname: %s ipaddr: %s", node.id, node.hostname, node.ipaddr
+        async with SerializationErrorRetryContext() as retry:
+            async for attempt in retry.attempts:
+                if attempt > 1:  # pragma: without-xdist
+                    nodes_to_decontextualize = (
+                        (
+                            await db_async_session.execute(
+                                select(Node)
+                                .filter(Node.id.in_(node.id for node in nodes_to_decontextualize))
+                                .order_by(Node.id.asc())
+                            )
+                        )
+                        .scalars()
+                        .all()
                     )
-                    node.fail("decontextualizing node failed")
-                else:
-                    node.state = NodeState.ready
 
-        await db_async_session.flush()
+                if None in decontextualized_ipaddrs:
+                    log.error("One or more nodes couldn't be decontextualized:")
+                    for node, ipaddr in zip(nodes_to_decontextualize, decontextualized_ipaddrs):
+                        if not ipaddr:
+                            log.error(
+                                "    id: %s hostname: %s ipaddr: %s",
+                                node.id,
+                                node.hostname,
+                                node.ipaddr,
+                            )
+                            node.fail("decontextualizing node failed")
+                        else:
+                            node.state = NodeState.ready
+
+                await db_async_session.flush()
 
         # Some nodes are out of circulation, fill up pools.
         fill_pools.delay(pool_names=list(pools_to_fill_up)).forget()
 
         # Don't raise an HTTPException here, the transaction should be committed unless something
         # else fails.
         return JSONResponse(
             {"detail": "contextualization of nodes failed"},
             status_code=HTTP_503_SERVICE_UNAVAILABLE,
             headers={"Retry-After": "0"},
         )
-    else:  # None not in contextualized_ipaddrs
-        for node in nodes_in_transaction:
-            node.state = NodeState.deployed
-
-    # Meh. Reload the session instance to ensure all related objects are present in the session.
-    await db_async_session.flush()
-    session = (
-        await db_async_session.execute(
-            select(Session)
-            .filter_by(id=session.id)
-            .options(
-                selectinload(Session.tenant),
-                selectinload(Session.session_nodes).selectinload(SessionNode.node),
-            )
-        )
-    ).scalar_one()
 
-    try:
-        await db_async_session.flush()
-    except IntegrityError as exc:  # pragma: no cover
-        raise HTTPException(HTTP_422_UNPROCESSABLE_ENTITY, str(exc))
+    # None not in contextualized_ipaddrs -> carry on
+    async with SerializationErrorRetryContext() as retry:
+        async for attempt in retry.attempts:
+            for node in nodes_in_transaction:
+                node.state = NodeState.deployed
+
+            # Meh. Reload the session instance to ensure all related objects are present in the
+            # session.
+            await db_async_session.flush()
+
+            session = (
+                await db_async_session.execute(
+                    select(Session)
+                    .filter_by(id=session.id)
+                    .options(
+                        selectinload(Session.tenant),
+                        selectinload(Session.session_nodes).selectinload(SessionNode.node),
+                    )
+                )
+            ).scalar_one()
+
+            try:
+                await db_async_session.commit()
+            except IntegrityError as exc:  # pragma: no cover
+                raise HTTPException(HTTP_422_UNPROCESSABLE_ENTITY, str(exc))
 
     # Tell backend worker to fill up pools from which nodes were taken.
     fill_pools.delay(pool_names=list(pools_to_fill_up)).forget()
 
     return {"action": "post", "session": session}
```

### Comparing `duffy-3.3.5/duffy/app/controllers/tenant.py` & `duffy-3.3.6rc1/duffy/app/controllers/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/app/main.py` & `duffy-3.3.6rc1/duffy/app/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/app/util.py` & `duffy-3.3.6rc1/duffy/app/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/cli.py` & `duffy-3.3.6rc1/duffy/cli.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/client/formatter.py` & `duffy-3.3.6rc1/duffy/client/formatter.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/client/main.py` & `duffy-3.3.6rc1/duffy/client/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/configuration/main.py` & `duffy-3.3.6rc1/duffy/configuration/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/configuration/validation.py` & `duffy-3.3.6rc1/duffy/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/__init__.py` & `duffy-3.3.6rc1/duffy/database/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,35 +5,23 @@
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, create_async_engine
 from sqlalchemy.orm import declarative_base, sessionmaker
 
 from ..configuration import config
 from ..exceptions import DuffyConfigurationError
 
-
 # use custom metadata to specify naming convention
-def constraint_column_names(constraint, table):
-    return "_".join(c.name for c in constraint.columns)
-
-
-def constraint_column_labels(constraint, table):  # pragma: no cover
-    return "_".join(c._label for c in constraint.columns)
-
-
 naming_convention = {
-    "column_names": constraint_column_names,
-    "column_labels": constraint_column_labels,
-    "ix": "%(column_labels)s_index",
-    "uq": "%(table_name)s_%(column_names)s_key",
+    "ix": "%(column_0_N_label)s_index",
+    "uq": "%(table_name)s_%(column_0_N_name)s_key",
     "ck": "%(table_name)s_%(constraint_name)s_check",
-    "fk": "%(table_name)s_%(column_names)s_%(referred_table_name)s_fkey",
+    "fk": "%(table_name)s_%(column_0_N_name)s_%(referred_table_name)s_fkey",
     "pk": "%(table_name)s_pkey",
 }
 metadata = MetaData(naming_convention=naming_convention)
-
 Base = declarative_base(metadata=metadata)
 
 async_session_maker = sessionmaker(class_=AsyncSession, expire_on_commit=False, future=True)
 sync_session_maker = sessionmaker(future=True, expire_on_commit=False)
 
 
 def init_sync_model(sync_engine: Engine = None):
```

### Comparing `duffy-3.3.5/duffy/database/migrations/env.py` & `duffy-3.3.6rc1/duffy/database/migrations/env.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/migrations/main.py` & `duffy-3.3.6rc1/duffy/database/migrations/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/migrations/script.py.mako` & `duffy-3.3.6rc1/duffy/database/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py` & `duffy-3.3.6rc1/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/model/node.py` & `duffy-3.3.6rc1/duffy/database/model/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/model/session.py` & `duffy-3.3.6rc1/duffy/database/model/session.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/model/tenant.py` & `duffy-3.3.6rc1/duffy/database/model/tenant.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,38 +48,38 @@
             return self.node_quota
 
         return config["defaults"]["node-quota"]
 
     @effective_node_quota.expression
     def effective_node_quota(cls):
         return case(
-            [(cls.node_quota != None, cls.node_quota)],  # noqa: E711
+            (cls.node_quota != None, cls.node_quota),  # noqa: E711
             else_=_defaults_config().node_quota,
         )
 
     @hybrid_property
     def effective_session_lifetime(self):
         if self.session_lifetime is not None:
             return self.session_lifetime
 
         return _defaults_config().session_lifetime
 
     @effective_session_lifetime.expression
     def effective_session_lifetime(cls):
         return case(
-            [(cls.session_lifetime != None, cls.session_lifetime)],  # noqa: E711
+            (cls.session_lifetime != None, cls.session_lifetime),  # noqa: E711
             else_=_defaults_config().session_lifetime,
         )
 
     @hybrid_property
     def effective_session_lifetime_max(self):
         if self.session_lifetime_max is not None:
             return self.session_lifetime_max
 
         return _defaults_config().session_lifetime_max
 
     @effective_session_lifetime_max.expression
     def effective_session_lifetime_max(cls):
         return case(
-            [(cls.session_lifetime_max != None, cls.session_lifetime_max)],  # noqa: E711
+            (cls.session_lifetime_max != None, cls.session_lifetime_max),  # noqa: E711
             else_=_defaults_config().session_lifetime_max,
         )
```

### Comparing `duffy-3.3.5/duffy/database/setup.py` & `duffy-3.3.6rc1/duffy/database/setup.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/database/util.py` & `duffy-3.3.6rc1/duffy/database/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/legacy/auth.py` & `duffy-3.3.6rc1/duffy/legacy/auth.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/legacy/main.py` & `duffy-3.3.6rc1/duffy/legacy/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/misc.py` & `duffy-3.3.6rc1/duffy/misc.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/nodes/context.py` & `duffy-3.3.6rc1/duffy/nodes/context.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/nodes/mechanisms/ansible.py` & `duffy-3.3.6rc1/duffy/nodes/mechanisms/ansible.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/nodes/mechanisms/main.py` & `duffy-3.3.6rc1/duffy/nodes/mechanisms/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 
 class MechanismFailure(Exception):
     pass
 
 
 class Mechanism(dict):
-
     known_mechanisms: Dict[str, "Mechanism"] = {}
 
     def __init_subclass__(cls, mech_type: str, **kwargs):
         super().__init_subclass__()
 
         # Register subclasses.
         if mech_type in cls.known_mechanisms:
```

### Comparing `duffy-3.3.5/duffy/nodes/pools.py` & `duffy-3.3.6rc1/duffy/nodes/pools.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..configuration import config
 from ..database.model import Node
 from ..util import merge_dicts
 from .mechanisms import Mechanism
 
 
 class NodePool(dict):
-
     subcls_per_cls_type: Dict[str, type] = {}
     known_pools: Dict[str, "NodePool"] = {}
 
     def __init_subclass__(cls, cls_type: bool, **kwargs):
         if cls_type in cls.subcls_per_cls_type:
             raise TypeError(f"Subclass type isn't unique: {cls_type}")
```

### Comparing `duffy-3.3.5/duffy/shell.py` & `duffy-3.3.6rc1/duffy/shell.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/tasks/deprovision.py` & `duffy-3.3.6rc1/duffy/tasks/deprovision.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/tasks/expire.py` & `duffy-3.3.6rc1/duffy/tasks/expire.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/tasks/main.py` & `duffy-3.3.6rc1/duffy/tasks/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/tasks/provision.py` & `duffy-3.3.6rc1/duffy/tasks/provision.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/duffy/util.py` & `duffy-3.3.6rc1/duffy/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.5/pyproject.toml` & `duffy-3.3.6rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duffy"
-version = "3.3.5"
+version = "3.3.6rc1"
 description = "CentOS CI provisioner"
 authors = ["Nils Philippsen <nils@redhat.com>", "Vipul Siddharth <siddharthvipul1@gmail.com>", "Akashdeep Dhar <akashdeep@redhat.com>", "Ben Capper <bcapper@redhat.com>"]
 license = "MIT"
 maintainers = ["Nils Philippsen <nils@redhat.com>", "Vipul Siddharth <siddharthvipul1@gmail.com>", "Akashdeep Dhar <akashdeep@redhat.com>", "Ben Capper <bcapper@redhat.com>"]
 readme = "README.md"
 homepage = "https://github.com/CentOS/duffy"
 repository = "https://github.com/CentOS/duffy"
@@ -34,15 +34,15 @@
     "Topic :: System :: Operating System",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.3"
 PyYAML = "^6"
-SQLAlchemy = {version = "^1.4.25", extras=["asyncio"], optional = true}
+SQLAlchemy = {version = "^2.0.5", extras=["asyncio"], optional = true}
 alembic = {version = "^1.7.5", optional = true}
 bcrypt = {version = "^3.2 || ^4", optional = true}
 fastapi = {version = ">=0.70, <2", optional = true}
 uvicorn = {version = ">=0.15, <2", optional = true}
 Jinja2 = {version = "^3.0.3", optional = true}
 ansible-runner = {version = "^2.1.1", optional = true}
 asyncpg = {version = ">=0.25, <2", optional = true}
@@ -55,34 +55,33 @@
 aiodns = {version = "^3.0.0", optional = true}
 pydantic = ">=1.6.2"
 aiosqlite = {version = ">=0.17.0, <2", optional = true}
 pyxdg = ">=0.27, <2"
 
 [tool.poetry.dev-dependencies]
 Jinja2 = "^3.0.3"
-ansible = "^5.2 || ^6"
+ansible = "^5.2 || ^6 || ^7.0.0 || ^8.0.0"
 ansible-core = "^2.12.1"
 ansible-runner = "^2.1.1"
 black = ">=21.9b0"
-fastapi = {version = ">=0.70, <2", extras = ["test"]}
 flake8 = ">=3.9.2"
 httpx = ">=0.18.2, <2"
 isort = "^5.9.3"
 jmespath = ">=0.10, <2"
 poetry = "^1.2.0"
 pottery = "^3"
 pytest = ">=6.2.5"
 pytest-asyncio = ">=0.17, <2"
 pytest-black = ">=0.3.12, <2"
-pytest-cov = "^3"
-pytest-flake8 = "^1.0.7"
+pytest-cov = "^3 || ^4"
 pytest-isort = ">=2"
-tox = "^3.24.4"
+tox = "^3.24.4 || ^4.0.0"
 psycopg = "^3.0.16"
-pytest-postgresql = "^4.1.1"
+pytest-postgresql = "^4.1.1 || ^5.0.0"
+coverage-conditional-plugin = "^0.8.0 || ^0.9.0"
 
 [tool.poetry.extras]
 # the `serve` command
 app = [
     "SQLAlchemy", "alembic", "bcrypt", "fastapi", "uvicorn",
     "aiodns", "ansible-runner", "Jinja2", "jmespath", "pottery", "celery",
 ]
@@ -100,16 +99,15 @@
 tasks = ["aiodns", "ansible-runner", "Jinja2", "jmespath", "pottery", "celery"]
 # the `serve-legacy` command
 legacy = ["httpx", "Jinja2"]
 # the `client ...` commands
 client = ["httpx"]
 
 [tool.pytest.ini_options]
-addopts = "--black --cov-config .coveragerc --cov=duffy --cov-report term --cov-report xml --cov-report html --flake8 --isort"
-flake8-max-line-length = 100
+addopts = "--black --cov-config .coveragerc --cov=duffy --cov-report term --cov-report xml --cov-report html --isort"
 asyncio_mode = "auto"
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.black]
```

### Comparing `duffy-3.3.5/PKG-INFO` & `duffy-3.3.6rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duffy
-Version: 3.3.5
+Version: 3.3.6rc1
 Summary: CentOS CI provisioner
 Home-page: https://github.com/CentOS/duffy
 License: MIT
 Keywords: baremetal,ci,vm,opennebula,centos
 Author: Nils Philippsen
 Author-email: nils@redhat.com
 Maintainer: Nils Philippsen
@@ -20,19 +20,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Operating System
 Provides-Extra: admin
@@ -40,34 +36,34 @@
 Provides-Extra: client
 Provides-Extra: database
 Provides-Extra: dev-shell
 Provides-Extra: legacy
 Provides-Extra: postgresql
 Provides-Extra: sqlite
 Provides-Extra: tasks
-Requires-Dist: Jinja2 (>=3.0.3,<4.0.0); extra == "app" or extra == "tasks" or extra == "legacy"
+Requires-Dist: Jinja2 (>=3.0.3,<4.0.0) ; extra == "app" or extra == "tasks" or extra == "legacy"
 Requires-Dist: PyYAML (>=6,<7)
-Requires-Dist: SQLAlchemy[asyncio] (>=1.4.25,<2.0.0); extra == "app" or extra == "admin" or extra == "database" or extra == "dev-shell"
-Requires-Dist: aiodns (>=3.0.0,<4.0.0); extra == "app" or extra == "tasks"
-Requires-Dist: aiosqlite (>=0.17.0,<2); extra == "sqlite"
-Requires-Dist: alembic (>=1.7.5,<2.0.0); extra == "app" or extra == "database" or extra == "dev-shell"
-Requires-Dist: ansible-runner (>=2.1.1,<3.0.0); extra == "app" or extra == "tasks"
-Requires-Dist: asyncpg (>=0.25,<2); extra == "postgresql"
-Requires-Dist: bcrypt (>=3.2,<5); extra == "app" or extra == "admin" or extra == "database" or extra == "dev-shell"
-Requires-Dist: celery[redis] (>=5.2.1,<6.0.0); extra == "app" or extra == "tasks"
+Requires-Dist: SQLAlchemy[asyncio] (>=2.0.5,<3.0.0) ; extra == "app" or extra == "admin" or extra == "database" or extra == "dev-shell"
+Requires-Dist: aiodns (>=3.0.0,<4.0.0) ; extra == "app" or extra == "tasks"
+Requires-Dist: aiosqlite (>=0.17.0,<2) ; extra == "sqlite"
+Requires-Dist: alembic (>=1.7.5,<2.0.0) ; extra == "app" or extra == "database" or extra == "dev-shell"
+Requires-Dist: ansible-runner (>=2.1.1,<3.0.0) ; extra == "app" or extra == "tasks"
+Requires-Dist: asyncpg (>=0.25,<2) ; extra == "postgresql"
+Requires-Dist: bcrypt (>=3.2,<5) ; extra == "app" or extra == "admin" or extra == "database" or extra == "dev-shell"
+Requires-Dist: celery[redis] (>=5.2.1,<6.0.0) ; extra == "app" or extra == "tasks"
 Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: fastapi (>=0.70,<2); extra == "app" or extra == "admin"
-Requires-Dist: httpx (>=0.18.2,<2); extra == "legacy" or extra == "client"
-Requires-Dist: ipython (>=7.29); extra == "dev-shell"
-Requires-Dist: jmespath (>=0.10,<2); extra == "app" or extra == "tasks"
-Requires-Dist: pottery (>=3,<4); extra == "app" or extra == "tasks"
-Requires-Dist: psycopg2 (>=2.9.2,<3.0.0); extra == "postgresql"
+Requires-Dist: fastapi (>=0.70,<2) ; extra == "app" or extra == "admin"
+Requires-Dist: httpx (>=0.18.2,<2) ; extra == "legacy" or extra == "client"
+Requires-Dist: ipython (>=7.29) ; extra == "dev-shell"
+Requires-Dist: jmespath (>=0.10,<2) ; extra == "app" or extra == "tasks"
+Requires-Dist: pottery (>=3,<4) ; extra == "app" or extra == "tasks"
+Requires-Dist: psycopg2 (>=2.9.2,<3.0.0) ; extra == "postgresql"
 Requires-Dist: pydantic (>=1.6.2)
 Requires-Dist: pyxdg (>=0.27,<2)
-Requires-Dist: uvicorn (>=0.15,<2); extra == "app"
+Requires-Dist: uvicorn (>=0.15,<2) ; extra == "app"
 Project-URL: Documentation, https://github.com/CentOS/duffy/wiki
 Project-URL: Repository, https://github.com/CentOS/duffy
 Description-Content-Type: text/markdown
 
 ## Info
 Community Platform Engineering team (of Red Hat) is working on revamping this project and thus, have cleaned this repository by
 * marking other branches stale
```

