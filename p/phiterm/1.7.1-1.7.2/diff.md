# Comparing `tmp/phiterm-1.7.1.tar.gz` & `tmp/phiterm-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.7.1.tar", last modified: Mon Jun 12 21:44:46 2023, max compression
+gzip compressed data, was "phiterm-1.7.2.tar", last modified: Tue Jun 13 16:38:51 2023, max compression
```

## Comparing `phiterm-1.7.1.tar` & `phiterm-1.7.2.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.171494 phiterm-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-12 21:44:25.000000 phiterm-1.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 21:44:46.171494 phiterm-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 21:44:25.000000 phiterm-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.155493 phiterm-1.7.1/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.155493 phiterm-1.7.1/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.155493 phiterm-1.7.1/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36902 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.159494 phiterm-1.7.1/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.163493 phiterm-1.7.1/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.163493 phiterm-1.7.1/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.163493 phiterm-1.7.1/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.163493 phiterm-1.7.1/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.155493 phiterm-1.7.1/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.163493 phiterm-1.7.1/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.163493 phiterm-1.7.1/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.167494 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.167494 phiterm-1.7.1/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.167494 phiterm-1.7.1/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.167494 phiterm-1.7.1/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/get_python_objects_from_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.167494 phiterm-1.7.1/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.171494 phiterm-1.7.1/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-12 21:44:25.000000 phiterm-1.7.1/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.155493 phiterm-1.7.1/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 21:44:46.000000 phiterm-1.7.1/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-12 21:44:46.000000 phiterm-1.7.1/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:44:46.000000 phiterm-1.7.1/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 21:44:46.000000 phiterm-1.7.1/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 21:44:46.000000 phiterm-1.7.1/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 21:44:46.000000 phiterm-1.7.1/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-12 21:44:25.000000 phiterm-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:44:46.171494 phiterm-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 21:44:25.000000 phiterm-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:44:46.171494 phiterm-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 21:44:25.000000 phiterm-1.7.1/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.367716 phiterm-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-13 16:38:29.000000 phiterm-1.7.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 16:38:51.367716 phiterm-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 16:38:29.000000 phiterm-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.351716 phiterm-1.7.2/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36914 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.355716 phiterm-1.7.2/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.359716 phiterm-1.7.2/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.359716 phiterm-1.7.2/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.359716 phiterm-1.7.2/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.359716 phiterm-1.7.2/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.351716 phiterm-1.7.2/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.359716 phiterm-1.7.2/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.363716 phiterm-1.7.2/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.363716 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.363716 phiterm-1.7.2/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.363716 phiterm-1.7.2/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.363716 phiterm-1.7.2/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/get_python_objects_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.363716 phiterm-1.7.2/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.367716 phiterm-1.7.2/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-13 16:38:29.000000 phiterm-1.7.2/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.351716 phiterm-1.7.2/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 16:38:51.000000 phiterm-1.7.2/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-13 16:38:51.000000 phiterm-1.7.2/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:38:51.000000 phiterm-1.7.2/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 16:38:51.000000 phiterm-1.7.2/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 16:38:51.000000 phiterm-1.7.2/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 16:38:51.000000 phiterm-1.7.2/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-13 16:38:29.000000 phiterm-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:38:51.367716 phiterm-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 16:38:29.000000 phiterm-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:38:51.367716 phiterm-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-13 16:38:29.000000 phiterm-1.7.2/tests/test_backend_api.py
```

### Comparing `phiterm-1.7.1/LICENSE.md` & `phiterm-1.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/api/client.py` & `phiterm-1.7.2/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/api/routes.py` & `phiterm-1.7.2/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/api/user.py` & `phiterm-1.7.2/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/api/workspace.py` & `phiterm-1.7.2/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/aws/aws_operator.py` & `phiterm-1.7.2/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/cli_app.py` & `phiterm-1.7.2/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/cli_operator.py` & `phiterm-1.7.2/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/dx/dx_app.py` & `phiterm-1.7.2/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.7.2/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.7.2/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.7.2/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/wf/wf_app.py` & `phiterm-1.7.2/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/cli/ws/ws_app.py` & `phiterm-1.7.2/phiterm/cli/ws/ws_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     setup_workspace(ws_root_path=ws_root_path)
 
 
 @ws_app.command(short_help="Create resources for active workspace")
 def up(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
+        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
         metavar="[FILTER]",
     ),
     env_filter: Optional[str] = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to deploy"
     ),
     config_filter: Optional[str] = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config to deploy"
@@ -163,22 +163,22 @@
     Options can be used to limit the resources to create.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
+    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
     \b
     Examples:
     > `phi ws up`            -> Deploy all resources
     > `phi ws up dev`        -> Deploy all dev resources
     > `phi ws up prd`        -> Deploy all prd resources
     > `phi ws up prd:aws`    -> Deploy all prd aws resources
-    > `phi ws up prd::s3`    -> Deploy prd resources matching name s3
+    > `phi ws up prd:::s3`    -> Deploy prd resources matching name s3
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import deploy_workspace
     from phiterm.utils.load_env import load_env
     from phiterm.utils.ws_filter import parse_ws_filter
 
     if print_debug_log:
@@ -218,51 +218,51 @@
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
     target_env: Optional[str] = None
     target_config_str: Optional[str] = None
     target_config: Optional[WorkspaceConfigType] = None
+    target_group: Optional[str] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_group: Optional[str] = None
 
     # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
+            target_group,
             target_name,
             target_type,
-            target_group,
         ) = parse_ws_filter(resource_filter)
 
     # derive env:config:name:type:group from command options
     if target_env is None and env_filter is not None and isinstance(env_filter, str):
         target_env = env_filter
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
-    if target_name is None and name_filter is not None and isinstance(name_filter, str):
-        target_name = name_filter
-    if target_type is None and type_filter is not None and isinstance(type_filter, str):
-        target_type = type_filter
     if (
         target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
         target_group = group_filter
+    if target_name is None and name_filter is not None and isinstance(name_filter, str):
+        target_name = name_filter
+    if target_type is None and type_filter is not None and isinstance(type_filter, str):
+        target_type = type_filter
 
     # derive env:config:name:type:group from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
         )
     if target_config_str is None:
@@ -281,17 +281,17 @@
             WorkspaceConfigType,
             WorkspaceConfigType.from_str(target_config_str),
         )
 
     logger.debug("Deploying workspace")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Deploying workspace: {}\n".format(active_ws_data.ws_name))
     deploy_workspace(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
@@ -303,15 +303,15 @@
     )
 
 
 @ws_app.command(short_help="Delete resources for active workspace")
 def down(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
+        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to shut down"
     ),
     config_filter: str = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config to shut down"
@@ -359,15 +359,15 @@
     Options can be used to limit the resources to delete.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
+    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
     \b
     Examples:
     > `phi ws down`            -> Delete all resources
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import shutdown_workspace
     from phiterm.utils.load_env import load_env
@@ -410,49 +410,49 @@
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
     target_env: Optional[str] = None
     target_config_str: Optional[str] = None
     target_config: Optional[WorkspaceConfigType] = None
+    target_group: Optional[str] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_group: Optional[str] = None
 
     # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
+            target_group,
             target_name,
             target_type,
-            target_group,
         ) = parse_ws_filter(resource_filter)
 
     # derive env:config:name:type:group from command options
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
-    if target_name is None and name_filter is not None and isinstance(name_filter, str):
-        target_name = name_filter
-    if target_type is None and type_filter is not None and isinstance(type_filter, str):
-        target_type = type_filter
     if (
         target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
         target_group = group_filter
+    if target_name is None and name_filter is not None and isinstance(name_filter, str):
+        target_name = name_filter
+    if target_type is None and type_filter is not None and isinstance(type_filter, str):
+        target_type = type_filter
     if target_env is None and env_filter is not None and isinstance(env_filter, str):
         target_env = env_filter
 
     # derive env:config:name:type:group from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
@@ -473,17 +473,17 @@
             WorkspaceConfigType,
             WorkspaceConfigType.from_str(target_config_str),
         )
 
     logger.debug("Shutting down workspace")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Shutdown workspace: {}\n".format(active_ws_data.ws_name))
     shutdown_workspace(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
@@ -495,15 +495,15 @@
     )
 
 
 @ws_app.command(short_help="Update resources for active workspace")
 def patch(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
+        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to patch"
     ),
     config_filter: str = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config to patch"
@@ -551,15 +551,15 @@
     Options can be used to limit the resources to update.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
+    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
     Examples:
     \b
     > `phi ws patch`           -> Patch all resources
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import patch_workspace
     from phiterm.utils.load_env import load_env
@@ -602,49 +602,49 @@
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
     target_env: Optional[str] = None
     target_config_str: Optional[str] = None
     target_config: Optional[WorkspaceConfigType] = None
+    target_group: Optional[str] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_group: Optional[str] = None
 
     # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
+            target_group,
             target_name,
             target_type,
-            target_group,
         ) = parse_ws_filter(resource_filter)
 
     # derive env:config:name:type:group from command options
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
-    if target_name is None and name_filter is not None and isinstance(name_filter, str):
-        target_name = name_filter
-    if target_type is None and type_filter is not None and isinstance(type_filter, str):
-        target_type = type_filter
     if (
         target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
         target_group = group_filter
+    if target_name is None and name_filter is not None and isinstance(name_filter, str):
+        target_name = name_filter
+    if target_type is None and type_filter is not None and isinstance(type_filter, str):
+        target_type = type_filter
     if target_env is None and env_filter is not None and isinstance(env_filter, str):
         target_env = env_filter
 
     # derive env:config:name:type:group from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
@@ -665,17 +665,17 @@
             WorkspaceConfigType,
             WorkspaceConfigType.from_str(target_config_str),
         )
 
     logger.debug("Patching workspace")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Patching workspace: {}\n".format(active_ws_data.ws_name))
     patch_workspace(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
@@ -687,15 +687,15 @@
     )
 
 
 @ws_app.command(short_help="Restart resources for active workspace")
 def restart(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
+        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to restart"
     ),
     config_filter: str = typer.Option(
         None, "-i", "--config", metavar="", help="Filter the config to restart"
@@ -775,15 +775,15 @@
     )
 
 
 @ws_app.command(short_help="Show status for workspace resources")
 def status(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
+        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment"
     ),
     config_filter: str = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config"
@@ -831,18 +831,18 @@
     Options can be used to limit the resources to update.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
+    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
     Examples:
     \b
-    > `phi ws patch`           -> Patch all resources
+    > `phi ws status`           -> Show status for all resources
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import print_workspace_status
     from phiterm.utils.load_env import load_env
     from phiterm.utils.ws_filter import parse_ws_filter
 
     if print_debug_log:
@@ -882,49 +882,49 @@
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
     target_env: Optional[str] = None
     target_config_str: Optional[str] = None
     target_config: Optional[WorkspaceConfigType] = None
+    target_group: Optional[str] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_group: Optional[str] = None
 
     # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
+            target_group,
             target_name,
             target_type,
-            target_group,
         ) = parse_ws_filter(resource_filter)
 
     # derive env:config:name:type:group from command options
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
-    if target_name is None and name_filter is not None and isinstance(name_filter, str):
-        target_name = name_filter
-    if target_type is None and type_filter is not None and isinstance(type_filter, str):
-        target_type = type_filter
     if (
         target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
         target_group = group_filter
+    if target_name is None and name_filter is not None and isinstance(name_filter, str):
+        target_name = name_filter
+    if target_type is None and type_filter is not None and isinstance(type_filter, str):
+        target_type = type_filter
     if target_env is None and env_filter is not None and isinstance(env_filter, str):
         target_env = env_filter
 
     # derive env/config/name/type from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
@@ -945,17 +945,17 @@
             WorkspaceConfigType,
             WorkspaceConfigType.from_str(target_config_str),
         )
 
     logger.debug("Reading workspace status")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Reading workspace status: {}\n".format(active_ws_data.ws_name))
     print_workspace_status(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
```

### Comparing `phiterm-1.7.1/phiterm/conf/auth.py` & `phiterm-1.7.2/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/conf/constants.py` & `phiterm-1.7.2/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/conf/phi_conf.py` & `phiterm-1.7.2/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/databox/databox_operator.py` & `phiterm-1.7.2/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/docker/docker_operator.py` & `phiterm-1.7.2/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/enums/user.py` & `phiterm-1.7.2/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/k8s/k8s_operator.py` & `phiterm-1.7.2/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.7.2/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.7.2/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.7.2/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.7.2/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/local/local_operator.py` & `phiterm-1.7.2/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/release/release_schemas.py` & `phiterm-1.7.2/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/release/ws_releases.py` & `phiterm-1.7.2/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/schemas/user.py` & `phiterm-1.7.2/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/schemas/user_schemas.py` & `phiterm-1.7.2/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/schemas/workspace.py` & `phiterm-1.7.2/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.7.2/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.7.2/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.7.2/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.7.2/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.7.2/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.7.2/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.7.2/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.7.2/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/cli_auth_server.py` & `phiterm-1.7.2/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/cli_console.py` & `phiterm-1.7.2/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/common.py` & `phiterm-1.7.2/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/dttm.py` & `phiterm-1.7.2/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/enums.py` & `phiterm-1.7.2/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/filesystem.py` & `phiterm-1.7.2/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/get_python_objects_from_module.py` & `phiterm-1.7.2/phiterm/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/git.py` & `phiterm-1.7.2/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/load_env.py` & `phiterm-1.7.2/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/log.py` & `phiterm-1.7.2/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/prep_infra_config.py` & `phiterm-1.7.2/phiterm/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/pyproject.py` & `phiterm-1.7.2/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/utils/ws_filter.py` & `phiterm-1.7.2/phiterm/utils/ws_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 
 def parse_ws_filter(
     ws_filter: str,
 ) -> Tuple[Optional[str], Optional[str], Optional[str], Optional[str], Optional[str]]:
     target_env: Optional[str] = None
     target_config: Optional[str] = None
+    target_group: Optional[str] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_group: Optional[str] = None
 
     filters = ws_filter.split(":")
     num_filters = len(filters)
     if num_filters >= 1:
         if filters[0] != "":
             target_env = filters[0]
     if num_filters >= 2:
         if filters[1] != "":
             target_config = filters[1]
     if num_filters >= 3:
         if filters[2] != "":
-            target_name = filters[2]
+            target_group = filters[2]
     if num_filters >= 4:
         if filters[3] != "":
-            target_type = filters[3]
+            target_name = filters[3]
     if num_filters >= 5:
         if filters[4] != "":
-            target_group = filters[4]
+            target_type = filters[4]
 
-    return target_env, target_config, target_name, target_type, target_group
+    return target_env, target_config, target_group, target_name, target_type
```

### Comparing `phiterm-1.7.1/phiterm/workflow/wf_operator.py` & `phiterm-1.7.2/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/workflow/wf_utils.py` & `phiterm-1.7.2/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/workspace/phi_ws_data.py` & `phiterm-1.7.2/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/workspace/ws_enums.py` & `phiterm-1.7.2/phiterm/workspace/ws_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/workspace/ws_loader.py` & `phiterm-1.7.2/phiterm/workspace/ws_loader.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/workspace/ws_operator.py` & `phiterm-1.7.2/phiterm/workspace/ws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/workspace/ws_schemas.py` & `phiterm-1.7.2/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm/workspace/ws_utils.py` & `phiterm-1.7.2/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/phiterm.egg-info/SOURCES.txt` & `phiterm-1.7.2/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.1/pyproject.toml` & `phiterm-1.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.7.1"
+version = "1.7.2"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

