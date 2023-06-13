# Comparing `tmp/seldon-deploy-sdk-2.0.1.tar.gz` & `tmp/seldon-deploy-sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldon-deploy-sdk-2.0.1.tar", last modified: Tue Jan 31 16:22:33 2023, max compression
+gzip compressed data, was "seldon-deploy-sdk-2.1.0.tar", last modified: Tue Jun 13 11:37:42 2023, max compression
```

## Comparing `seldon-deploy-sdk-2.0.1.tar` & `seldon-deploy-sdk-2.1.0.tar`

### file list

```diff
@@ -1,731 +1,733 @@
-drwxr-xr-x   0 agm       (1000) agm       (1000)        0 2023-01-31 16:22:33.645223 seldon-deploy-sdk-2.0.1/
--rw-r--r--   0 agm       (1000) agm       (1000)      319 2023-01-31 16:22:33.645223 seldon-deploy-sdk-2.0.1/PKG-INFO
--rw-r--r--   0 agm       (1000) agm       (1000)    43146 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/README.md
-drwxr-xr-x   0 agm       (1000) agm       (1000)        0 2023-01-31 16:22:33.548556 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/
--rw-r--r--   0 agm       (1000) agm       (1000)    26398 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/__init__.py
-drwxr-xr-x   0 agm       (1000) agm       (1000)        0 2023-01-31 16:22:33.551890 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/
--rw-r--r--   0 agm       (1000) agm       (1000)     1548 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/__init__.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8336 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/alerting_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4659 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/application_logs_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    31711 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/batch_jobs_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    42774 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/drift_detector_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    13688 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/environment_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    50925 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/experiments_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    10390 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/explain_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    51681 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/git_ops_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4939 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/healthcheck_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5892 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/kubernetes_resources_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    32716 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/loadtest_jobs_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    21880 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/metrics_server_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    28065 2023-01-31 16:16:42.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/model_metadata_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    19938 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/models_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    22732 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/monitor_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    43012 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/outlier_detector_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    69483 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/permission_management_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    43795 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/pipelines_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    26886 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/predict_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    32824 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/secrets_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    29601 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/seldon_deployments_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)    27033 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api_client.py
-drwxr-xr-x   0 agm       (1000) agm       (1000)        0 2023-01-31 16:22:33.551890 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/
--rw-r--r--   0 agm       (1000) agm       (1000)      180 2023-01-31 16:16:27.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/__init__.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2700 2023-01-31 16:16:27.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/base.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4894 2023-01-31 16:16:27.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/openid.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1633 2023-01-31 16:16:27.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/session.py
--rw-r--r--   0 agm       (1000) agm       (1000)     9184 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/configuration.py
-drwxr-xr-x   0 agm       (1000) agm       (1000)        0 2023-01-31 16:22:33.605223 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/
--rw-r--r--   0 agm       (1000) agm       (1000)    24778 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/__init__.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4936 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/advanced_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4830 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2504 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/alibi_explainer_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3833 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/application_log.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6973 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/application_logs_params.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3837 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/application_logs_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5975 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/audit_log.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7810 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/aws_elastic_block_store_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2528 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_data_disk_caching_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2500 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_data_disk_kind.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7731 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5215 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_file_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6624 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/basic_detector_configuration.py
--rw-r--r--   0 agm       (1000) agm       (1000)    13641 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_definition.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6476 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_description.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2524 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_description_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4071 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_get_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4190 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_post_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5714 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_jobs_list_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3900 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/capabilities.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2472 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/capability.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8275 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ceph_fs_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6548 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/cinder_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3738 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/client_ip_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3205 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/cluster_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5117 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/component.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2492 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/condition_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2472 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/conditions.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4341 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_env_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5058 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_key_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6068 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7842 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)    27627 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7103 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_port.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4654 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3251 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state_running.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8413 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state_terminated.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4180 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state_waiting.py
--rw-r--r--   0 agm       (1000) agm       (1000)    10805 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5236 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/cross_version_object_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7696 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/csi_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)    29580 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment.py
--rw-r--r--   0 agm       (1000) agm       (1000)    13742 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_feature_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)    12920 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)    10752 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6772 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4022 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_strategy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2520 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_strategy_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3800 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_config_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4035 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_configuration.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7406 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)     9796 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_deployment_configuration.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2488 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2468 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/dns_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3369 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/downward_api_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6781 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/downward_api_volume_file.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5271 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/downward_api_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3934 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/empty_dir_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5814 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/endpoint.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2480 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/endpoint_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4905 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/env_from_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5349 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/env_var.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5835 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/env_var_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)    28868 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ephemeral_container.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4492 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ephemeral_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4456 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/error.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3975 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/exec_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)    29580 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3758 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_candidate.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3742 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_mirror.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5359 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5692 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     9979 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/explainer.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4895 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/explainer_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5987 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/external_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3925 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/fallback.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7242 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/fc_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3369 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4873 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution_bucket.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6309 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution_parameters.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7016 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)    10851 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_filter.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2504 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_interaction.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6807 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_statistics_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8824 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_stats.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3847 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_stats_bucket.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2464 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/fields_v1.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7684 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/file_diff.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2484 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/finalizer_name.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6921 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/flex_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4518 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/flocker_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7778 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/gce_persistent_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5385 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/git_repo_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5585 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/glusterfs_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4435 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/handler.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3850 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/health_check_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4132 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/horizontal_pod_autoscaler_behavior.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3357 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/horizontal_pod_autoscaler_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3906 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/host_alias.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2480 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/host_path_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4151 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/host_path_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5157 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/hpa_scaling_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2512 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/hpa_scaling_policy_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6397 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/hpa_scaling_rules.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6281 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/http_get_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3808 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/http_header.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4316 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/int_or_string.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2464 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ip_family.py
--rw-r--r--   0 agm       (1000) agm       (1000)    13463 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/iscsi_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2464 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/join_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5467 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/key_to_path.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5004 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/label_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2516 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/label_selector_operator.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5335 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/label_selector_requirement.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3820 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/lifecycle.py
--rw-r--r--   0 agm       (1000) agm       (1000)     9445 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/list_meta.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3517 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/local_object_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3707 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/logger.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2472 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/logger_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3213 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/logging_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7766 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/managed_fields_entry.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2536 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/managed_fields_operation_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3748 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/message.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2496 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/metric_source_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5742 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/metric_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2496 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/metric_target_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)    29130 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/model.py
--rw-r--r--   0 agm       (1000) agm       (1000)    15228 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/model_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6405 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/model_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)    13023 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/monitor_input_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2512 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/mount_propagation_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)    29490 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6191 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_condition.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2520 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_condition_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2488 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_phase.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3649 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4206 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5351 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/nfs_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6911 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2468 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_phase.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3578 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2512 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector_operator.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5432 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector_requirement.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4604 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4360 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/object_field_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)    25763 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/object_meta.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6382 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/object_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8033 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/owner_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4210 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/parameter.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3666 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/parameter_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2480 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/parmeter_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2536 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_access_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)     9184 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_claim_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)    27766 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_claim_template.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4739 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_claim_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2512 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4498 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/photon_persistent_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)    29400 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4389 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_batch.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5842 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_output.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3902 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5660 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8882 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_step.py
--rw-r--r--   0 agm       (1000) agm       (1000)    28950 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7984 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5855 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_affinity_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8072 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_anti_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7101 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_condition.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2496 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_condition_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5870 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_dns_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3854 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_dns_config_option.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2520 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_fs_group_change_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3115 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_ip.py
--rw-r--r--   0 agm       (1000) agm       (1000)    12825 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2464 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_phase.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2476 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_qos_class.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3327 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_readiness_gate.py
--rw-r--r--   0 agm       (1000) agm       (1000)    14501 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_security_context.py
--rw-r--r--   0 agm       (1000) agm       (1000)    47379 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)    16815 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)    26704 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_template_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pods_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5409 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/portworx_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)    11520 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2544 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit_implementation.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2512 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit_method.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2504 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)    11794 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictor_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2496 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/preemption_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4185 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/preferred_scheduling_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)    10232 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/probe.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2484 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/proc_mount_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5030 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/projected_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4045 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/protobuf_any.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2571 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/protobuf_null_value.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2464 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/protocol.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2472 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pull_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2464 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/quantity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8014 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/quobyte_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)    10285 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/rbd_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4995 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_field_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2480 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5581 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2480 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_name.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3904 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_requirements.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2480 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2484 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/restart_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4132 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/rolling_update_deployment.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4325 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/rpc_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)    11895 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scale_io_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6071 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scale_triggers.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3932 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scaled_object_auth_ref.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2508 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scaling_policy_select.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5584 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/se_linux_options.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4568 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seccomp_profile.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2504 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seccomp_profile_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4299 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_env_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5100 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_key_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6000 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7811 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)    14871 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/security_context.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3077 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_addressable.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7139 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5259 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     9181 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)    10449 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5813 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_experiment.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4644 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_hpa_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5663 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_model.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5126 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_model_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4092 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pdb_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5753 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pipeline.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5195 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pipeline_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6537 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pod_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     9364 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_scaled_object_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2472 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/server_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)    29310 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6474 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_account_token_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2492 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2560 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_external_traffic_policy_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)    12781 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8960 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_port.py
--rw-r--r--   0 agm       (1000) agm       (1000)    23953 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5424 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2476 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3261 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/session_affinity_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3223 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ssl.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2476 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/status_state.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2484 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/storage_medium.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8160 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/storage_os_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4433 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/svc_orch_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3776 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/sysctl.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2476 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/taint_effect.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3876 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/tcp_socket_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2528 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/termination_message_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2448 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/time.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7267 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/toleration.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2504 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/toleration_operator.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8242 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/topology_spread_constraint.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2468 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/transport.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2448 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5238 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/typed_local_object_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2444 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/uid.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2548 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/unsatisfiable_constraint_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2468 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/uri_scheme.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4746 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/user_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2528 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_add_user_to_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2845 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_artifact_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2556 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_gcs_bucket_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3322 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_group_request.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2516 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2520 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_policy_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2568 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_rclone_bucket_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2552 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_registry_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2552 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_s3_bucket_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6097 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_user_request.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2512 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_user_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2609 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_data_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2667 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_default_protocol.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2516 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2520 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_policy_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2520 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2548 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_user_from_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2512 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_user_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3549 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_dependency_health_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2967 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deploy_dependency.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6567 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deploy_dependency_health.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2735 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deploy_dependency_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2617 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deployment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2707 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deployment_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3969 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_feature_category_schema.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7355 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_feature_schema.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2659 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_feature_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5743 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_firing_alert.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3248 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_group_members_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3183 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_groups_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3362 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_permissions_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3898 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_policy_targets_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3215 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_user_groups_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3152 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_users_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3017 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_group.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3837 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_group_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3348 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_list_alerts_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3222 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_list_secrets_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)    12833 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2548 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_create_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2548 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_delete_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4366 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_list_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2548 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_update_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3977 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4169 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_prediction_schema.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3416 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_rclone_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2540 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_reset_user_password_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3850 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_resource_action_pair.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3678 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_runtime_defaults.py
--rw-r--r--   0 agm       (1000) agm       (1000)    16411 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_runtime_metadata.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4619 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_runtime_metadata_list_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4224 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_s3_credentials.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3891 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_secret.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2585 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_secret_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2536 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_trigger_test_alert_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     7104 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_user.py
--rw-r--r--   0 agm       (1000) agm       (1000)     3805 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_user_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6728 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/version_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)    24357 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4151 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume_device.py
--rw-r--r--   0 agm       (1000) agm       (1000)     8220 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume_mount.py
--rw-r--r--   0 agm       (1000) agm       (1000)     5743 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6856 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/vsphere_virtual_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     4318 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/weighted_pod_affinity_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6759 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/windows_security_context_options.py
--rw-r--r--   0 agm       (1000) agm       (1000)    13235 2023-01-31 16:16:27.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/rest.py
-drwxr-xr-x   0 agm       (1000) agm       (1000)        0 2023-01-31 16:22:33.548556 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk.egg-info/
--rw-r--r--   0 agm       (1000) agm       (1000)      319 2023-01-31 16:22:33.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk.egg-info/PKG-INFO
--rw-r--r--   0 agm       (1000) agm       (1000)    28447 2023-01-31 16:22:33.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 agm       (1000) agm       (1000)        1 2023-01-31 16:22:33.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 agm       (1000) agm       (1000)      103 2023-01-31 16:22:33.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk.egg-info/requires.txt
--rw-r--r--   0 agm       (1000) agm       (1000)       23 2023-01-31 16:22:33.000000 seldon-deploy-sdk-2.0.1/seldon_deploy_sdk.egg-info/top_level.txt
--rw-r--r--   0 agm       (1000) agm       (1000)       38 2023-01-31 16:22:33.645223 seldon-deploy-sdk-2.0.1/setup.cfg
--rw-r--r--   0 agm       (1000) agm       (1000)     1165 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/setup.py
-drwxr-xr-x   0 agm       (1000) agm       (1000)        0 2023-01-31 16:22:33.645223 seldon-deploy-sdk-2.0.1/test/
--rw-r--r--   0 agm       (1000) agm       (1000)        0 2023-01-31 16:16:27.000000 seldon-deploy-sdk-2.0.1/test/__init__.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_advanced_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)      931 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1225 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_alerting_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_alibi_explainer_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_application_log.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1018 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_application_logs_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_application_logs_params.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1055 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_application_logs_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_audit_log.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1133 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_aws_elastic_block_store_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1067 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_azure_data_disk_caching_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1009 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_azure_data_disk_kind.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_azure_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_azure_file_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1079 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_basic_detector_configuration.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_batch_job_definition.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1023 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_batch_job_description.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1057 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_batch_job_description_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1025 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_batch_job_get_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_batch_job_post_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1559 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_batch_jobs_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_batch_jobs_list_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      963 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_capabilities.py
--rw-r--r--   0 agm       (1000) agm       (1000)      947 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_capability.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1017 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_ceph_fs_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_cinder_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      983 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_client_ip_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_cluster_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)      939 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_component.py
--rw-r--r--   0 agm       (1000) agm       (1000)      989 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_condition_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)      947 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_conditions.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1017 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_config_map_env_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_config_map_key_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1023 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_config_map_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_config_map_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      939 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_container.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_container_port.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_container_state.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_container_state_running.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1063 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_container_state_terminated.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_container_state_waiting.py
--rw-r--r--   0 agm       (1000) agm       (1000)      989 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_container_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1089 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_cross_version_object_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_csi_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      947 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_deployment.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_deployment_feature_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_deployment_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_deployment_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_deployment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1013 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_deployment_strategy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1047 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_deployment_strategy_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_detector_config_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1037 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_detector_configuration.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_detector_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1119 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_detector_deployment_configuration.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_detector_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)      941 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_dns_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_downward_api_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_downward_api_volume_file.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1057 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_downward_api_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_drift_detector_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_empty_dir_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      931 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_endpoint.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_endpoint_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_env_from_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      917 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_env_var.py
--rw-r--r--   0 agm       (1000) agm       (1000)      967 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_env_var_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1197 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_environment_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1013 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_ephemeral_container.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_ephemeral_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      907 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_error.py
--rw-r--r--   0 agm       (1000) agm       (1000)      949 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_exec_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)      947 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_experiment.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1021 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_experiment_candidate.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_experiment_mirror.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_experiment_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_experiment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1947 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_experiments_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1021 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_explain_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      939 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_explainer.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_explainer_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_external_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      931 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_fallback.py
--rw-r--r--   0 agm       (1000) agm       (1000)      983 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_fc_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1021 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_distribution.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1071 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_distribution_bucket.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1103 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_distribution_parameters.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1087 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_distribution_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_filter.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1013 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_interaction.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1071 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_statistics_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_stats.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_feature_stats_bucket.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_fields_v1.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_file_diff.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_finalizer_name.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_flex_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1023 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_flocker_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1107 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_gce_persistent_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2123 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/test/test_git_ops_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1025 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_git_repo_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_glusterfs_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      923 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_handler.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_health_check_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1101 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/test/test_healthcheck_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1121 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_horizontal_pod_autoscaler_behavior.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1105 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_horizontal_pod_autoscaler_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)      941 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_host_alias.py
--rw-r--r--   0 agm       (1000) agm       (1000)      967 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_host_path_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_host_path_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_hpa_scaling_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_hpa_scaling_policy_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_hpa_scaling_rules.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_http_get_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)      949 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_http_header.py
--rw-r--r--   0 agm       (1000) agm       (1000)      959 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_int_or_string.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_ip_family.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1007 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_iscsi_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_join_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      943 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_key_to_path.py
--rw-r--r--   0 agm       (1000) agm       (1000)      989 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_kubernetes_resources_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_label_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_label_selector_operator.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1063 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_label_selector_requirement.py
--rw-r--r--   0 agm       (1000) agm       (1000)      939 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_lifecycle.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_list_meta.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1587 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_loadtest_jobs_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_local_object_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)      915 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_logger.py
--rw-r--r--   0 agm       (1000) agm       (1000)      949 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_logger_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_logging_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_managed_fields_entry.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1081 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_managed_fields_operation_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      923 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_message.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:25.000000 seldon-deploy-sdk-2.0.1/test/test_metric_source_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      949 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_metric_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_metric_target_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1415 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_metrics_server_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      907 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_model.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1984 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_model_metadata_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      941 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_model_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_model_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1159 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_models_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1365 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_monitor_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_monitor_input_data.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_mount_propagation_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)      939 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_namespace.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1013 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_namespace_condition.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1047 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_namespace_condition_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_namespace_phase.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_namespace_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      989 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_namespace_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_nfs_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_node_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)      941 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_node_phase.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_node_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_node_selector_operator.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1055 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_node_selector_requirement.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_node_selector_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1023 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_object_field_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)      949 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_object_meta.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_object_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2043 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_outlier_detector_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_owner_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)      939 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_parameter.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_parameter_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_parmeter_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     6351 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_permission_management_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1081 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_persistent_volume_access_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1073 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_persistent_volume_claim_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1105 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_persistent_volume_claim_template.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1139 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_persistent_volume_claim_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_persistent_volume_mode.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1131 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_photon_persistent_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      931 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pipeline.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pipeline_batch.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pipeline_output.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pipeline_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pipeline_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pipeline_step.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1785 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pipelines_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      891 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_affinity_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_anti_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_condition.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_condition_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      967 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_dns_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1017 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_dns_config_option.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1051 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_fs_group_change_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)      909 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_ip.py
--rw-r--r--   0 agm       (1000) agm       (1000)      925 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_phase.py
--rw-r--r--   0 agm       (1000) agm       (1000)      959 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_qos_class.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_readiness_gate.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_security_context.py
--rw-r--r--   0 agm       (1000) agm       (1000)      925 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      941 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pod_template_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pods_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_portworx_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1449 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_predict_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_predictive_unit.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1095 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_predictive_unit_implementation.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_predictive_unit_method.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_predictive_unit_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_predictor_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_preemption_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1055 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_preferred_scheduling_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)      907 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_probe.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_proc_mount_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_projected_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_protobuf_any.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1007 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_protobuf_null_value.py
--rw-r--r--   0 agm       (1000) agm       (1000)      931 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_protocol.py
--rw-r--r--   0 agm       (1000) agm       (1000)      949 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_pull_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)      931 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_quantity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1023 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_quobyte_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_rbd_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_resource_field_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_resource_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_resource_metric_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_resource_name.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1029 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_resource_requirements.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_resource_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_restart_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1055 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_rolling_update_deployment.py
--rw-r--r--   0 agm       (1000) agm       (1000)      941 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_rpc_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1025 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_scale_io_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_scale_triggers.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1025 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_scaled_object_auth_ref.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1023 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_scaling_policy_select.py
--rw-r--r--   0 agm       (1000) agm       (1000)      983 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_se_linux_options.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seccomp_profile.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seccomp_profile_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_secret_env_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1007 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_secret_key_selector.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_secret_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_secret_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     2184 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_secrets_service_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      989 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_security_context.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1005 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_addressable.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_deployment.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_deployment_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1031 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_deployment_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1047 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_deployment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1569 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_deployments_api.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_experiment.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_hpa_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_model.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_model_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_pdb_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      981 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_pipeline.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_pipeline_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_pod_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1049 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_seldon_scaled_object_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      949 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_server_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      923 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1105 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_account_token_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)      989 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_affinity.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1131 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_external_traffic_policy_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_list.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_port.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_service_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1039 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_session_affinity_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)      891 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_ssl.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_status_state.py
--rw-r--r--   0 agm       (1000) agm       (1000)      973 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_storage_medium.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_storage_os_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)      959 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_svc_orch_spec.py
--rw-r--r--   0 agm       (1000) agm       (1000)      915 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_sysctl.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_taint_effect.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_tcp_socket_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1063 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_termination_message_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)      899 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_time.py
--rw-r--r--   0 agm       (1000) agm       (1000)      947 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_toleration.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1013 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_toleration_operator.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1063 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_topology_spread_constraint.py
--rw-r--r--   0 agm       (1000) agm       (1000)      939 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_transport.py
--rw-r--r--   0 agm       (1000) agm       (1000)      899 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1073 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_typed_local_object_reference.py
--rw-r--r--   0 agm       (1000) agm       (1000)      891 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_uid.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1103 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_unsatisfiable_constraint_action.py
--rw-r--r--   0 agm       (1000) agm       (1000)      941 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_uri_scheme.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_user_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1069 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_add_user_to_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      983 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_artifact_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1125 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_gcs_bucket_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_group_request.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1049 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_policy_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1149 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_rclone_bucket_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1115 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_registry_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1117 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_s3_bucket_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1025 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_user_request.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_create_user_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      951 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_data_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1007 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_default_protocol.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_delete_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1049 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_delete_policy_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1049 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_delete_secret_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1109 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_delete_user_from_group_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_delete_user_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1081 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/test/test_v1_dependency_health_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/test/test_v1_deploy_dependency.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1065 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/test/test_v1_deploy_dependency_health.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1065 2023-01-31 16:22:15.000000 seldon-deploy-sdk-2.0.1/test/test_v1_deploy_dependency_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_deployment_status.py
--rw-r--r--   0 agm       (1000) agm       (1000)      999 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_deployment_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1057 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_feature_category_schema.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_feature_schema.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_feature_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_firing_alert.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1075 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_get_group_members_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1025 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_get_groups_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1065 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_get_permissions_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1083 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_get_policy_targets_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1059 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_get_user_groups_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1017 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_get_users_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      925 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_group.py
--rw-r--r--   0 agm       (1000) agm       (1000)      975 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_group_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_list_alerts_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1041 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_list_secrets_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      925 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_model.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1107 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_create_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1107 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_delete_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1091 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_list_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1107 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_update_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1015 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_prediction_schema.py
--rw-r--r--   0 agm       (1000) agm       (1000)      983 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_rclone_config.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1091 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_reset_user_password_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1033 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_resource_action_pair.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1007 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_runtime_defaults.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1007 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_runtime_metadata.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1107 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_runtime_metadata_list_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      991 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_s3_credentials.py
--rw-r--r--   0 agm       (1000) agm       (1000)      933 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_secret.py
--rw-r--r--   0 agm       (1000) agm       (1000)      967 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_secret_type.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1083 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_trigger_test_alert_response.py
--rw-r--r--   0 agm       (1000) agm       (1000)      917 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_user.py
--rw-r--r--   0 agm       (1000) agm       (1000)      967 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_v1_user_policy.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_version_info.py
--rw-r--r--   0 agm       (1000) agm       (1000)      915 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_volume.py
--rw-r--r--   0 agm       (1000) agm       (1000)      965 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_volume_device.py
--rw-r--r--   0 agm       (1000) agm       (1000)      957 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_volume_mount.py
--rw-r--r--   0 agm       (1000) agm       (1000)      997 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_volume_projection.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1115 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_vsphere_virtual_disk_volume_source.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1057 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_weighted_pod_affinity_term.py
--rw-r--r--   0 agm       (1000) agm       (1000)     1105 2023-01-31 16:16:26.000000 seldon-deploy-sdk-2.0.1/test/test_windows_security_context_options.py
+drwxrwxr-x   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:37:42.047436 seldon-deploy-sdk-2.1.0/
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      355 2023-06-13 11:37:42.047436 seldon-deploy-sdk-2.1.0/PKG-INFO
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    43480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/README.md
+drwxrwxr-x   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:37:41.939434 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    26480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/__init__.py
+drwxrwxr-x   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:37:41.943434 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1548 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/__init__.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8336 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/alerting_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4659 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/application_logs_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    31711 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/batch_jobs_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    42774 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/drift_detector_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    13688 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/environment_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    50925 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/experiments_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    10390 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/explain_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    56647 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/git_ops_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/healthcheck_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5892 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/kubernetes_resources_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    32716 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/loadtest_jobs_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    21880 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/metrics_server_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    28065 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/model_metadata_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    19938 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/models_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    22732 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/monitor_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    43012 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/outlier_detector_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    69483 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/permission_management_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    49240 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/pipelines_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    26886 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/predict_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    34096 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/secrets_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    29601 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/seldon_deployments_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    27033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api_client.py
+drwxrwxr-x   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:37:41.943434 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      180 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/__init__.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2700 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/base.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5120 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/openid.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1633 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/session.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     9184 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/configuration.py
+drwxrwxr-x   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:37:41.995435 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    24860 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/__init__.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4936 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/advanced_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4830 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2504 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/alibi_explainer_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3833 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/application_log.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/application_logs_params.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3837 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/application_logs_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/audit_log.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7810 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/aws_elastic_block_store_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2528 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_data_disk_caching_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2500 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_data_disk_kind.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7731 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5215 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_file_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6624 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/basic_detector_configuration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    13683 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_definition.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6476 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_description.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2524 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_description_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4071 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_get_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4190 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_post_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5714 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_jobs_list_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3900 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/capabilities.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2472 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/capability.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8275 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ceph_fs_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6548 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/cinder_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3738 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/client_ip_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3205 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/cluster_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5117 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/component.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2492 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/condition_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2472 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/conditions.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4341 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_env_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5058 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_key_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6068 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7842 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    27627 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7103 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_port.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4654 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3251 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state_running.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8413 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state_terminated.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4180 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state_waiting.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    10805 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5236 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/cross_version_object_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7696 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/csi_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    29580 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    13742 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_feature_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    12920 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    10752 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6772 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4022 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_strategy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2520 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_strategy_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3800 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_config_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4035 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_configuration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7406 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     9796 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_deployment_configuration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2488 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2468 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/dns_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3369 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/downward_api_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6781 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/downward_api_volume_file.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5271 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/downward_api_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3934 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/empty_dir_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5814 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/endpoint.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/endpoint_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4905 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/env_from_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5349 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/env_var.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5835 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/env_var_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    28868 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ephemeral_container.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4492 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ephemeral_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4456 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/error.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/exec_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    29580 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3758 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_candidate.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3742 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_mirror.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5359 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5692 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     9979 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/explainer.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4895 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/explainer_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5987 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/external_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3925 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/fallback.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7242 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/fc_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3369 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4873 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution_bucket.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6309 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution_parameters.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7016 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    10851 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_filter.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2504 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_interaction.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6807 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_statistics_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8824 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_stats.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3847 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_stats_bucket.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2464 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/fields_v1.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7684 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/file_diff.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2484 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/finalizer_name.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6921 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/flex_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4518 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/flocker_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7778 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/gce_persistent_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5385 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/git_repo_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5585 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/glusterfs_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4435 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/handler.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3850 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/health_check_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4132 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/horizontal_pod_autoscaler_behavior.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3357 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/horizontal_pod_autoscaler_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3906 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/host_alias.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/host_path_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4151 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/host_path_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5157 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/hpa_scaling_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2512 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/hpa_scaling_policy_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6397 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/hpa_scaling_rules.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6281 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/http_get_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3808 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/http_header.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4316 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/int_or_string.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2464 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ip_family.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    13463 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/iscsi_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2464 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/join_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5467 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/key_to_path.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5004 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/label_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2516 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/label_selector_operator.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5335 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/label_selector_requirement.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3820 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/lifecycle.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     9445 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/list_meta.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3517 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/local_object_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3707 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/logger.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2472 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/logger_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3213 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/logging_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7766 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/managed_fields_entry.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2536 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/managed_fields_operation_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3748 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/message.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2496 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/metric_source_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5742 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/metric_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2496 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/metric_target_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    29130 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/model.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    15228 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/model_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6405 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/model_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    13023 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/monitor_input_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2512 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/mount_propagation_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    29490 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6191 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_condition.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2520 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_condition_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2488 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_phase.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3649 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4206 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5351 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/nfs_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6911 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2468 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_phase.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3578 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2512 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector_operator.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5432 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector_requirement.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4604 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4360 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/object_field_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    25763 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/object_meta.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6382 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/object_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/owner_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4210 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/parameter.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3666 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/parameter_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/parmeter_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2536 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_access_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     9184 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_claim_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    27766 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_claim_template.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4739 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_claim_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2512 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4498 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/photon_persistent_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    29400 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4389 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_batch.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5842 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_output.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3902 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5660 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8882 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_step.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    28950 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7984 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5855 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_affinity_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8072 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_anti_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7101 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_condition.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2496 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_condition_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5870 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_dns_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3854 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_dns_config_option.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2520 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_fs_group_change_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3115 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_ip.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    12825 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2464 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_phase.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2476 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_qos_class.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3327 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_readiness_gate.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    14501 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_security_context.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    47379 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    16815 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    26704 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_template_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pods_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5409 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/portworx_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    11520 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2544 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit_implementation.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2512 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit_method.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2504 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    11794 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictor_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2496 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/preemption_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4185 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/preferred_scheduling_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    10232 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/probe.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2484 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/proc_mount_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5030 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/projected_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4045 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/protobuf_any.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2571 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/protobuf_null_value.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2464 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/protocol.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2472 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pull_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2464 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/quantity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8014 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/quobyte_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    10285 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/rbd_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4995 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_field_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5581 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_name.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3904 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_requirements.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2480 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2484 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/restart_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4132 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/rolling_update_deployment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4325 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/rpc_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    11895 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scale_io_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6071 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scale_triggers.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3932 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scaled_object_auth_ref.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2508 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scaling_policy_select.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5584 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/se_linux_options.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4568 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seccomp_profile.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2504 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seccomp_profile_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4299 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_env_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5100 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_key_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6000 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7811 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    14871 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/security_context.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3077 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_addressable.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7139 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5259 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     9181 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    10449 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5813 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_experiment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4644 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_hpa_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5663 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_model.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5126 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_model_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4092 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pdb_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5753 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pipeline.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5195 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pipeline_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6537 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pod_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     9364 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_scaled_object_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2472 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/server_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    29310 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6474 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_account_token_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2492 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2560 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_external_traffic_policy_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    12781 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8960 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_port.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    23953 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5424 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2476 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3261 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/session_affinity_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3223 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ssl.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2476 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/status_state.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2484 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/storage_medium.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8160 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/storage_os_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4433 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/svc_orch_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3776 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/sysctl.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2476 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/taint_effect.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3876 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/tcp_socket_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2528 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/termination_message_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2448 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/time.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7267 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/toleration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2504 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/toleration_operator.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8242 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/topology_spread_constraint.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2468 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/transport.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2448 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5238 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/typed_local_object_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2444 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/uid.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2548 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/unsatisfiable_constraint_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2468 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/uri_scheme.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4746 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/user_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2528 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_add_user_to_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2921 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_artifact_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2611 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_bucket_secret_format.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2556 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_gcs_bucket_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3322 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_group_request.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2516 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2520 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_policy_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2568 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_rclone_bucket_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2552 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_registry_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2552 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_s3_bucket_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6097 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_user_request.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2512 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_user_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2609 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_data_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2667 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_default_protocol.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2516 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2520 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_policy_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2520 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2548 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_user_from_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2512 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_user_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3549 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_dependency_health_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deploy_dependency.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6567 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deploy_dependency_health.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2735 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deploy_dependency_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2617 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deployment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2707 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deployment_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3969 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_feature_category_schema.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7355 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_feature_schema.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2659 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_feature_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5743 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_firing_alert.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3248 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_group_members_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3183 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_groups_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3362 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_permissions_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3898 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_policy_targets_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3215 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_user_groups_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3152 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_users_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3017 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_group.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3837 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_group_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3348 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_list_alerts_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3222 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_list_secrets_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    12833 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2548 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_create_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2548 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_delete_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4366 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_list_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2548 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_update_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3977 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4169 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_prediction_schema.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4360 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_rclone_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2540 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_reset_user_password_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3850 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_resource_action_pair.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3678 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_runtime_defaults.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    16411 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_runtime_metadata.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4619 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_runtime_metadata_list_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4224 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_s3_credentials.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4935 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_secret.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2585 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_secret_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2536 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_trigger_test_alert_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     7104 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_user.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     3805 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_user_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6728 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/version_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    24357 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4151 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume_device.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     8220 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume_mount.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     5743 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6856 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/vsphere_virtual_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     4318 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/weighted_pod_affinity_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6759 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/windows_security_context_options.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    13235 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/rest.py
+drwxrwxr-x   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:37:41.939434 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk.egg-info/
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      355 2023-06-13 11:37:41.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)    28536 2023-06-13 11:37:41.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)        1 2023-06-13 11:37:41.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      103 2023-06-13 11:37:41.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk.egg-info/requires.txt
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)       23 2023-06-13 11:37:41.000000 seldon-deploy-sdk-2.1.0/seldon_deploy_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)       38 2023-06-13 11:37:42.047436 seldon-deploy-sdk-2.1.0/setup.cfg
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1165 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/setup.py
+drwxrwxr-x   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:37:42.047436 seldon-deploy-sdk-2.1.0/test/
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)        0 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/__init__.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_advanced_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      931 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1225 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_alerting_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_alibi_explainer_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_application_log.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1018 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_application_logs_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_application_logs_params.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1055 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_application_logs_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_audit_log.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1133 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_aws_elastic_block_store_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1067 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_azure_data_disk_caching_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1009 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_azure_data_disk_kind.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_azure_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_azure_file_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1079 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_basic_detector_configuration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_batch_job_definition.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1023 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_batch_job_description.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1057 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_batch_job_description_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1025 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_batch_job_get_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_batch_job_post_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1559 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_batch_jobs_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_batch_jobs_list_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      963 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_capabilities.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      947 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_capability.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1017 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_ceph_fs_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_cinder_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      983 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_client_ip_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_cluster_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_component.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      989 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_condition_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      947 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_conditions.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1017 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_config_map_env_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_config_map_key_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1023 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_config_map_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_config_map_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_container.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_container_port.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_container_state.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_container_state_running.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1063 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_container_state_terminated.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_container_state_waiting.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      989 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_container_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1089 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_cross_version_object_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_csi_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      947 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_deployment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_deployment_feature_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_deployment_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_deployment_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_deployment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1013 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_deployment_strategy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1047 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_deployment_strategy_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_detector_config_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1037 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_detector_configuration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_detector_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1119 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_detector_deployment_configuration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_detector_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      941 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_dns_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_downward_api_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_downward_api_volume_file.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1057 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_downward_api_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_drift_detector_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_empty_dir_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      931 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_endpoint.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_endpoint_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_env_from_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      917 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_env_var.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      967 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_env_var_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1197 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_environment_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1013 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_ephemeral_container.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_ephemeral_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      907 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_error.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      949 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_exec_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      947 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_experiment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1021 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_experiment_candidate.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_experiment_mirror.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_experiment_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_experiment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1947 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_experiments_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1021 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_explain_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_explainer.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_explainer_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_external_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      931 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_fallback.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      983 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_fc_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1021 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_distribution.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1071 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_distribution_bucket.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1103 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_distribution_parameters.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1087 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_distribution_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_filter.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1013 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_interaction.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1071 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_statistics_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_stats.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_feature_stats_bucket.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_fields_v1.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_file_diff.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_finalizer_name.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_flex_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1023 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_flocker_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1107 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_gce_persistent_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2225 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_git_ops_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1025 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_git_repo_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_glusterfs_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      923 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_handler.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_health_check_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1101 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_healthcheck_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1121 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_horizontal_pod_autoscaler_behavior.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1105 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_horizontal_pod_autoscaler_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      941 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_host_alias.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      967 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_host_path_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_host_path_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_hpa_scaling_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_hpa_scaling_policy_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_hpa_scaling_rules.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_http_get_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      949 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_http_header.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      959 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_int_or_string.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_ip_family.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1007 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_iscsi_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_join_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      943 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_key_to_path.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      989 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_kubernetes_resources_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_label_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_label_selector_operator.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1063 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_label_selector_requirement.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_lifecycle.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_list_meta.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1587 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_loadtest_jobs_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_local_object_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      915 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_logger.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      949 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_logger_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_logging_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_managed_fields_entry.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1081 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_managed_fields_operation_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      923 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_message.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_metric_source_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      949 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_metric_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_metric_target_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1415 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_metrics_server_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      907 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_model.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1984 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_model_metadata_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      941 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_model_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_model_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1159 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_models_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1365 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_monitor_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_monitor_input_data.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_mount_propagation_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_namespace.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1013 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_namespace_condition.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1047 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_namespace_condition_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_namespace_phase.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_namespace_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      989 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_namespace_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_nfs_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_node_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      941 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_node_phase.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_node_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_node_selector_operator.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1055 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_node_selector_requirement.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_node_selector_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1023 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_object_field_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      949 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_object_meta.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_object_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2043 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_outlier_detector_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_owner_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_parameter.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_parameter_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_parmeter_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     6351 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_permission_management_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1081 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_persistent_volume_access_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1073 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_persistent_volume_claim_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1105 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_persistent_volume_claim_template.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1139 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_persistent_volume_claim_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_persistent_volume_mode.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1131 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_photon_persistent_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      931 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pipeline.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pipeline_batch.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pipeline_output.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pipeline_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pipeline_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pipeline_step.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1909 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pipelines_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      891 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_affinity_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_anti_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_condition.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_condition_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      967 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_dns_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1017 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_dns_config_option.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1051 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_fs_group_change_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      909 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_ip.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      925 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_phase.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      959 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_qos_class.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_readiness_gate.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_security_context.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      925 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      941 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pod_template_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pods_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_portworx_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1449 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_predict_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_predictive_unit.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1095 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_predictive_unit_implementation.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_predictive_unit_method.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_predictive_unit_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_predictor_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_preemption_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1055 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_preferred_scheduling_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      907 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_probe.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_proc_mount_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_projected_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_protobuf_any.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1007 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_protobuf_null_value.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      931 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_protocol.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      949 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_pull_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      931 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_quantity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1023 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_quobyte_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_rbd_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_resource_field_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_resource_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_resource_metric_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_resource_name.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1029 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_resource_requirements.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_resource_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_restart_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1055 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_rolling_update_deployment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      941 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_rpc_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1025 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_scale_io_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_scale_triggers.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1025 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_scaled_object_auth_ref.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1023 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_scaling_policy_select.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      983 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_se_linux_options.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seccomp_profile.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seccomp_profile_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_secret_env_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1007 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_secret_key_selector.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_secret_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_secret_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     2184 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_secrets_service_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      989 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_security_context.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1005 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_addressable.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_deployment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_deployment_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1031 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_deployment_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1047 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_deployment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1569 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_deployments_api.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_experiment.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_hpa_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_model.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_model_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_pdb_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      981 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_pipeline.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_pipeline_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_pod_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1049 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_seldon_scaled_object_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      949 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_server_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      923 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1105 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_account_token_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      989 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_affinity.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1131 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_external_traffic_policy_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_list.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_port.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_service_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1039 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_session_affinity_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      891 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_ssl.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_status_state.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      973 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_storage_medium.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_storage_os_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      959 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_svc_orch_spec.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      915 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_sysctl.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_taint_effect.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_tcp_socket_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1063 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_termination_message_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      899 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_time.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      947 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_toleration.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1013 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_toleration_operator.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1063 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_topology_spread_constraint.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      939 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_transport.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      899 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1073 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_typed_local_object_reference.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      891 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_uid.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1103 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_unsatisfiable_constraint_action.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      941 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_uri_scheme.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_user_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1069 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_add_user_to_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      983 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_artifact_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_bucket_secret_format.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1125 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_gcs_bucket_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_group_request.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1049 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_policy_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1149 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_rclone_bucket_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1115 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_registry_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1117 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_s3_bucket_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1025 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_user_request.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_create_user_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      951 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_data_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1007 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_default_protocol.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_delete_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1049 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_delete_policy_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1049 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_delete_secret_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1109 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_delete_user_from_group_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_delete_user_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1081 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_dependency_health_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_deploy_dependency.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1065 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_deploy_dependency_health.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1065 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_deploy_dependency_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_deployment_status.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      999 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_deployment_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1057 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_feature_category_schema.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_feature_schema.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_feature_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_firing_alert.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1075 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_get_group_members_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1025 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_get_groups_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1065 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_get_permissions_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1083 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_get_policy_targets_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1059 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_get_user_groups_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1017 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_get_users_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      925 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_group.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      975 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_group_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_list_alerts_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1041 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_list_secrets_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      925 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_model.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1107 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_create_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1107 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_delete_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1091 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_list_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1107 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_update_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1015 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_prediction_schema.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      983 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_rclone_config.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1091 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_reset_user_password_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1033 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_resource_action_pair.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1007 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_runtime_defaults.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1007 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_runtime_metadata.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1107 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_runtime_metadata_list_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      991 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_s3_credentials.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      933 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_secret.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      967 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_secret_type.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1083 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_trigger_test_alert_response.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      917 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_user.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      967 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_v1_user_policy.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_version_info.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      915 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_volume.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      965 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_volume_device.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      957 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_volume_mount.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)      997 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_volume_projection.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1115 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_vsphere_virtual_disk_volume_source.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1057 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_weighted_pod_affinity_term.py
+-rw-rw-r--   0 gsunner   (1000) gsunner   (1000)     1105 2023-06-13 11:34:47.000000 seldon-deploy-sdk-2.1.0/test/test_windows_security_context_options.py
```

### Comparing `seldon-deploy-sdk-2.0.1/README.md` & `seldon-deploy-sdk-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # seldon-deploy-sdk
 API to interact and manage the lifecycle of your machine learning models deployed through Seldon Deploy.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: v1alpha1
-- Package version: 2.0.1
+- Package version: 2.1.0
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.6+
 
 ## Installation & Usage
@@ -109,23 +109,24 @@
 *ExperimentsApi* | [**remove_canary**](docs/ExperimentsApi.md#remove_canary) | **DELETE** /namespaces/{namespace}/pipelines/{name}/experiment/canary | 
 *ExperimentsApi* | [**remove_shadow**](docs/ExperimentsApi.md#remove_shadow) | **DELETE** /namespaces/{namespace}/pipelines/{name}/experiment/shadow | 
 *ExperimentsApi* | [**update_pipeline_experiment**](docs/ExperimentsApi.md#update_pipeline_experiment) | **PUT** /namespaces/{namespace}/pipelines/{name}/experiment | 
 *ExplainApi* | [**explain_seldon_deployment**](docs/ExplainApi.md#explain_seldon_deployment) | **POST** /namespaces/{namespace}/seldondeployments/{name}/explain | 
 *ExplainApi* | [**explain_seldon_pipeline**](docs/ExplainApi.md#explain_seldon_pipeline) | **POST** /namespaces/{namespace}/pipelines/{name}/explain | 
 *GitOpsApi* | [**read_experiment_git_diff**](docs/GitOpsApi.md#read_experiment_git_diff) | **GET** /namespaces/{namespace}/experiments/{name}/gitdiff | 
 *GitOpsApi* | [**read_experiment_git_logs**](docs/GitOpsApi.md#read_experiment_git_logs) | **GET** /namespaces/{namespace}/experiments/{name}/gitlogs | 
+*GitOpsApi* | [**read_git_diffs**](docs/GitOpsApi.md#read_git_diffs) | **GET** /namespaces/{namespace}/gitdiffs | 
 *GitOpsApi* | [**read_git_ops_status**](docs/GitOpsApi.md#read_git_ops_status) | **GET** /namespaces/{namespace}/gitops-status | 
 *GitOpsApi* | [**read_model_git_diff**](docs/GitOpsApi.md#read_model_git_diff) | **GET** /namespaces/{namespace}/models/{name}/gitdiff | 
 *GitOpsApi* | [**read_model_git_logs**](docs/GitOpsApi.md#read_model_git_logs) | **GET** /namespaces/{namespace}/models/{name}/gitlogs | 
 *GitOpsApi* | [**read_pipeline_git_diff**](docs/GitOpsApi.md#read_pipeline_git_diff) | **GET** /namespaces/{namespace}/pipelines/{name}/gitdiff | 
 *GitOpsApi* | [**read_pipeline_git_logs**](docs/GitOpsApi.md#read_pipeline_git_logs) | **GET** /namespaces/{namespace}/pipelines/{name}/gitlogs | 
 *GitOpsApi* | [**read_seldon_deployment_git_diff**](docs/GitOpsApi.md#read_seldon_deployment_git_diff) | **GET** /namespaces/{namespace}/seldondeployments/{name}/gitdiff | 
 *GitOpsApi* | [**read_seldon_deployment_git_logs**](docs/GitOpsApi.md#read_seldon_deployment_git_logs) | **GET** /namespaces/{namespace}/seldondeployments/{name}/gitlogs | 
-*GitOpsApi* | [**seldon_deployment_git_restore**](docs/GitOpsApi.md#seldon_deployment_git_restore) | **GET** /namespaces/{namespace}/seldondeployments/{name}/gitrestore | 
-*GitOpsApi* | [**seldon_deployment_git_revert**](docs/GitOpsApi.md#seldon_deployment_git_revert) | **GET** /namespaces/{namespace}/seldondeployments/{name}/gitrevert | 
+*GitOpsApi* | [**seldon_deployment_git_restore**](docs/GitOpsApi.md#seldon_deployment_git_restore) | **POST** /namespaces/{namespace}/seldondeployments/{name}/gitrestore | 
+*GitOpsApi* | [**seldon_deployment_git_revert**](docs/GitOpsApi.md#seldon_deployment_git_revert) | **POST** /namespaces/{namespace}/seldondeployments/{name}/gitrevert | 
 *HealthcheckServiceApi* | [**healthcheck_service_get_dependency_health**](docs/HealthcheckServiceApi.md#healthcheck_service_get_dependency_health) | **GET** /healthcheck/{dependency} | List the current health of a specific Seldon Deploy dependency or all of them
 *KubernetesResourcesApi* | [**list_seldon_deployment_resources**](docs/KubernetesResourcesApi.md#list_seldon_deployment_resources) | **GET** /namespaces/{namespace}/seldondeployments/{name}/resources | 
 *LoadtestJobsApi* | [**create_loadtest_pipeline**](docs/LoadtestJobsApi.md#create_loadtest_pipeline) | **POST** /namespaces/{namespace}/pipelines/{name}/loadtestjobs | 
 *LoadtestJobsApi* | [**create_loadtest_seldon_deployment**](docs/LoadtestJobsApi.md#create_loadtest_seldon_deployment) | **POST** /namespaces/{namespace}/seldondeployments/{name}/loadtestjobs | 
 *LoadtestJobsApi* | [**delete_loadtest_pipeline**](docs/LoadtestJobsApi.md#delete_loadtest_pipeline) | **DELETE** /namespaces/{namespace}/pipelines/{name}/loadtestjobs/{jobName} | 
 *LoadtestJobsApi* | [**delete_loadtest_seldon_deployment**](docs/LoadtestJobsApi.md#delete_loadtest_seldon_deployment) | **DELETE** /namespaces/{namespace}/seldondeployments/{name}/loadtestjobs/{jobName} | 
 *LoadtestJobsApi* | [**list_loadtest_pipeline**](docs/LoadtestJobsApi.md#list_loadtest_pipeline) | **GET** /namespaces/{namespace}/pipelines/{name}/loadtestjobs | 
@@ -175,14 +176,15 @@
 *PipelinesApi* | [**delete_pipeline**](docs/PipelinesApi.md#delete_pipeline) | **DELETE** /namespaces/{namespace}/pipelines/{name} | 
 *PipelinesApi* | [**delete_pipeline_explainer**](docs/PipelinesApi.md#delete_pipeline_explainer) | **DELETE** /namespaces/{namespace}/pipelines/{name}/explainer | 
 *PipelinesApi* | [**list_pipeline_models**](docs/PipelinesApi.md#list_pipeline_models) | **GET** /namespaces/{namespace}/pipelines/{name}/models | 
 *PipelinesApi* | [**list_pipelines**](docs/PipelinesApi.md#list_pipelines) | **GET** /namespaces/{namespace}/pipelines | 
 *PipelinesApi* | [**read_pipeline**](docs/PipelinesApi.md#read_pipeline) | **GET** /namespaces/{namespace}/pipelines/{name} | 
 *PipelinesApi* | [**read_pipeline_explainer**](docs/PipelinesApi.md#read_pipeline_explainer) | **GET** /namespaces/{namespace}/pipelines/{name}/explainer | 
 *PipelinesApi* | [**update_pipeline**](docs/PipelinesApi.md#update_pipeline) | **PUT** /namespaces/{namespace}/pipelines/{name} | 
+*PipelinesApi* | [**update_pipeline_explainer**](docs/PipelinesApi.md#update_pipeline_explainer) | **PUT** /namespaces/{namespace}/pipelines/{name}/explainer | 
 *PredictApi* | [**predict_file_seldon_deployment**](docs/PredictApi.md#predict_file_seldon_deployment) | **POST** /namespaces/{namespace}/seldondeployments/{name}/predictfile | 
 *PredictApi* | [**predict_file_seldon_pipeline**](docs/PredictApi.md#predict_file_seldon_pipeline) | **POST** /namespaces/{namespace}/pipelines/{name}/predictfile | 
 *PredictApi* | [**predict_seldon_deployment**](docs/PredictApi.md#predict_seldon_deployment) | **POST** /namespaces/{namespace}/seldondeployments/{name}/predict | 
 *PredictApi* | [**read_predict_curl_seldon_deployment**](docs/PredictApi.md#read_predict_curl_seldon_deployment) | **PUT** /namespaces/{namespace}/seldondeployments/{name}/predictcurl | 
 *PredictApi* | [**read_predict_curl_seldon_pipeline**](docs/PredictApi.md#read_predict_curl_seldon_pipeline) | **PUT** /namespaces/{namespace}/pipelines/{name}/predictcurl | 
 *SecretsServiceApi* | [**secrets_service_create_gcs_bucket_secret**](docs/SecretsServiceApi.md#secrets_service_create_gcs_bucket_secret) | **POST** /secrets/{namespace}/bucket/gcs/{remote} | Creates a GCS bucket secret according to specified parameters.
 *SecretsServiceApi* | [**secrets_service_create_rclone_bucket_secret**](docs/SecretsServiceApi.md#secrets_service_create_rclone_bucket_secret) | **POST** /secrets/{namespace}/bucket/rclone/{remote} | Creates a generic rclone bucket secret according to specified parameters.
@@ -464,14 +466,15 @@
  - [TypedLocalObjectReference](docs/TypedLocalObjectReference.md)
  - [UID](docs/UID.md)
  - [URIScheme](docs/URIScheme.md)
  - [UnsatisfiableConstraintAction](docs/UnsatisfiableConstraintAction.md)
  - [UserInfo](docs/UserInfo.md)
  - [V1AddUserToGroupResponse](docs/V1AddUserToGroupResponse.md)
  - [V1ArtifactType](docs/V1ArtifactType.md)
+ - [V1BucketSecretFormat](docs/V1BucketSecretFormat.md)
  - [V1CreateGCSBucketSecretResponse](docs/V1CreateGCSBucketSecretResponse.md)
  - [V1CreateGroupRequest](docs/V1CreateGroupRequest.md)
  - [V1CreateGroupResponse](docs/V1CreateGroupResponse.md)
  - [V1CreatePolicyResponse](docs/V1CreatePolicyResponse.md)
  - [V1CreateRcloneBucketSecretResponse](docs/V1CreateRcloneBucketSecretResponse.md)
  - [V1CreateRegistrySecretResponse](docs/V1CreateRegistrySecretResponse.md)
  - [V1CreateS3BucketSecretResponse](docs/V1CreateS3BucketSecretResponse.md)
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/__init__.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,15 @@
 from seldon_deploy_sdk.models.typed_local_object_reference import TypedLocalObjectReference
 from seldon_deploy_sdk.models.uid import UID
 from seldon_deploy_sdk.models.uri_scheme import URIScheme
 from seldon_deploy_sdk.models.unsatisfiable_constraint_action import UnsatisfiableConstraintAction
 from seldon_deploy_sdk.models.user_info import UserInfo
 from seldon_deploy_sdk.models.v1_add_user_to_group_response import V1AddUserToGroupResponse
 from seldon_deploy_sdk.models.v1_artifact_type import V1ArtifactType
+from seldon_deploy_sdk.models.v1_bucket_secret_format import V1BucketSecretFormat
 from seldon_deploy_sdk.models.v1_create_gcs_bucket_secret_response import V1CreateGCSBucketSecretResponse
 from seldon_deploy_sdk.models.v1_create_group_request import V1CreateGroupRequest
 from seldon_deploy_sdk.models.v1_create_group_response import V1CreateGroupResponse
 from seldon_deploy_sdk.models.v1_create_policy_response import V1CreatePolicyResponse
 from seldon_deploy_sdk.models.v1_create_rclone_bucket_secret_response import V1CreateRcloneBucketSecretResponse
 from seldon_deploy_sdk.models.v1_create_registry_secret_response import V1CreateRegistrySecretResponse
 from seldon_deploy_sdk.models.v1_create_s3_bucket_secret_response import V1CreateS3BucketSecretResponse
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/__init__.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/alerting_service_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/alerting_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/application_logs_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/application_logs_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/batch_jobs_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/batch_jobs_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/drift_detector_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/drift_detector_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/environment_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/environment_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/experiments_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/experiments_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/explain_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/explain_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/git_ops_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/git_ops_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,122 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def read_git_diffs(self, hashes, namespace, **kwargs):  # noqa: E501
+        """read_git_diffs  # noqa: E501
+
+        Read the git diffs from hashes  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.read_git_diffs(hashes, namespace, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param list[str] hashes: Hashes is an array of git commit hashes to get diffs for (required)
+        :param str namespace: Namespace provides a logical grouping of resources (required)
+        :return: list[FileDiff]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.read_git_diffs_with_http_info(hashes, namespace, **kwargs)  # noqa: E501
+        else:
+            (data) = self.read_git_diffs_with_http_info(hashes, namespace, **kwargs)  # noqa: E501
+            return data
+
+    def read_git_diffs_with_http_info(self, hashes, namespace, **kwargs):  # noqa: E501
+        """read_git_diffs  # noqa: E501
+
+        Read the git diffs from hashes  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.read_git_diffs_with_http_info(hashes, namespace, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param list[str] hashes: Hashes is an array of git commit hashes to get diffs for (required)
+        :param str namespace: Namespace provides a logical grouping of resources (required)
+        :return: list[FileDiff]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['hashes', 'namespace']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method read_git_diffs" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'hashes' is set
+        if ('hashes' not in params or
+                params['hashes'] is None):
+            raise ValueError("Missing the required parameter `hashes` when calling `read_git_diffs`")  # noqa: E501
+        # verify the required parameter 'namespace' is set
+        if ('namespace' not in params or
+                params['namespace'] is None):
+            raise ValueError("Missing the required parameter `namespace` when calling `read_git_diffs`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'namespace' in params:
+            path_params['namespace'] = params['namespace']  # noqa: E501
+
+        query_params = []
+        if 'hashes' in params:
+            query_params.append(('hashes', params['hashes']))  # noqa: E501
+            collection_formats['hashes'] = 'csv'  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/namespaces/{namespace}/gitdiffs', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[FileDiff]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def read_git_ops_status(self, namespace, **kwargs):  # noqa: E501
         """read_git_ops_status  # noqa: E501
 
         Read the GitOps status  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_git_ops_status(namespace, async_req=True)
@@ -1013,14 +1121,15 @@
         >>> thread = api.seldon_deployment_git_restore(name, namespace, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: Name identifies a resource (required)
         :param str namespace: Namespace provides a logical grouping of resources (required)
         :param str hash: Hash
+        :param str action: Action
         :param str message: Message
         :return: Message
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -1038,21 +1147,22 @@
         >>> thread = api.seldon_deployment_git_restore_with_http_info(name, namespace, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: Name identifies a resource (required)
         :param str namespace: Namespace provides a logical grouping of resources (required)
         :param str hash: Hash
+        :param str action: Action
         :param str message: Message
         :return: Message
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name', 'namespace', 'hash', 'message']  # noqa: E501
+        all_params = ['name', 'namespace', 'hash', 'action', 'message']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1079,14 +1189,16 @@
             path_params['name'] = params['name']  # noqa: E501
         if 'namespace' in params:
             path_params['namespace'] = params['namespace']  # noqa: E501
 
         query_params = []
         if 'hash' in params:
             query_params.append(('hash', params['hash']))  # noqa: E501
+        if 'action' in params:
+            query_params.append(('action', params['action']))  # noqa: E501
         if 'message' in params:
             query_params.append(('message', params['message']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -1100,15 +1212,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['OAuth2']  # noqa: E501
 
         return self.api_client.call_api(
-            '/namespaces/{namespace}/seldondeployments/{name}/gitrestore', 'GET',
+            '/namespaces/{namespace}/seldondeployments/{name}/gitrestore', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Message',  # noqa: E501
@@ -1128,14 +1240,15 @@
         >>> thread = api.seldon_deployment_git_revert(name, namespace, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: Name identifies a resource (required)
         :param str namespace: Namespace provides a logical grouping of resources (required)
         :param str hash: Hash
+        :param str action: Action
         :param str message: Message
         :return: Message
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -1153,21 +1266,22 @@
         >>> thread = api.seldon_deployment_git_revert_with_http_info(name, namespace, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: Name identifies a resource (required)
         :param str namespace: Namespace provides a logical grouping of resources (required)
         :param str hash: Hash
+        :param str action: Action
         :param str message: Message
         :return: Message
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name', 'namespace', 'hash', 'message']  # noqa: E501
+        all_params = ['name', 'namespace', 'hash', 'action', 'message']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1194,14 +1308,16 @@
             path_params['name'] = params['name']  # noqa: E501
         if 'namespace' in params:
             path_params['namespace'] = params['namespace']  # noqa: E501
 
         query_params = []
         if 'hash' in params:
             query_params.append(('hash', params['hash']))  # noqa: E501
+        if 'action' in params:
+            query_params.append(('action', params['action']))  # noqa: E501
         if 'message' in params:
             query_params.append(('message', params['message']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -1215,15 +1331,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['OAuth2']  # noqa: E501
 
         return self.api_client.call_api(
-            '/namespaces/{namespace}/seldondeployments/{name}/gitrevert', 'GET',
+            '/namespaces/{namespace}/seldondeployments/{name}/gitrevert', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Message',  # noqa: E501
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/healthcheck_service_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/healthcheck_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/kubernetes_resources_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/kubernetes_resources_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/loadtest_jobs_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/loadtest_jobs_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/metrics_server_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/metrics_server_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/model_metadata_service_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/model_metadata_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/models_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/models_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/monitor_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/outlier_detector_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/outlier_detector_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/permission_management_service_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/permission_management_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/pipelines_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/pipelines_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1039,7 +1039,130 @@
             response_type='SeldonPipeline',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def update_pipeline_explainer(self, name, namespace, model, **kwargs):  # noqa: E501
+        """update_pipeline_explainer  # noqa: E501
+
+        Update the specified Seldon Pipeline Explainer  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_pipeline_explainer(name, namespace, model, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: Name identifies a resource (required)
+        :param str namespace: Namespace provides a logical grouping of resources (required)
+        :param Model model: Seldon Model (required)
+        :param str action: Action
+        :param str message: Message
+        :return: SeldonModel
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.update_pipeline_explainer_with_http_info(name, namespace, model, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_pipeline_explainer_with_http_info(name, namespace, model, **kwargs)  # noqa: E501
+            return data
+
+    def update_pipeline_explainer_with_http_info(self, name, namespace, model, **kwargs):  # noqa: E501
+        """update_pipeline_explainer  # noqa: E501
+
+        Update the specified Seldon Pipeline Explainer  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_pipeline_explainer_with_http_info(name, namespace, model, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: Name identifies a resource (required)
+        :param str namespace: Namespace provides a logical grouping of resources (required)
+        :param Model model: Seldon Model (required)
+        :param str action: Action
+        :param str message: Message
+        :return: SeldonModel
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['name', 'namespace', 'model', 'action', 'message']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_pipeline_explainer" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `update_pipeline_explainer`")  # noqa: E501
+        # verify the required parameter 'namespace' is set
+        if ('namespace' not in params or
+                params['namespace'] is None):
+            raise ValueError("Missing the required parameter `namespace` when calling `update_pipeline_explainer`")  # noqa: E501
+        # verify the required parameter 'model' is set
+        if ('model' not in params or
+                params['model'] is None):
+            raise ValueError("Missing the required parameter `model` when calling `update_pipeline_explainer`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
+        if 'namespace' in params:
+            path_params['namespace'] = params['namespace']  # noqa: E501
+
+        query_params = []
+        if 'action' in params:
+            query_params.append(('action', params['action']))  # noqa: E501
+        if 'message' in params:
+            query_params.append(('message', params['message']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'model' in params:
+            body_params = params['model']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/namespaces/{namespace}/pipelines/{name}/explainer', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SeldonModel',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/predict_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/predict_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/secrets_service_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/secrets_service_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,14 +154,15 @@
         >>> thread = api.secrets_service_create_rclone_bucket_secret(namespace, remote, body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str namespace: The namespace to create secret in. (required)
         :param str remote: The name of the remote to create, can be lowercase characters or numbers up to 10 characters long. The created secret will be named {remote}-bucket. (required)
         :param V1RcloneConfig body: The rclone key value pairs. (required)
+        :param str format: The format for the secret. Must be one of (env_var, config_param). env_var formats the secret as environment variables, each with a key and a value. env_var is suitable for Seldon Core v1 and Argo Workflows. config_param formats the secret to be compatible with Rclone's HTTP API. config_param is suitable for Seldon Core v2.
         :return: V1CreateRcloneBucketSecretResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.secrets_service_create_rclone_bucket_secret_with_http_info(namespace, remote, body, **kwargs)  # noqa: E501
@@ -177,20 +178,21 @@
         >>> thread = api.secrets_service_create_rclone_bucket_secret_with_http_info(namespace, remote, body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str namespace: The namespace to create secret in. (required)
         :param str remote: The name of the remote to create, can be lowercase characters or numbers up to 10 characters long. The created secret will be named {remote}-bucket. (required)
         :param V1RcloneConfig body: The rclone key value pairs. (required)
+        :param str format: The format for the secret. Must be one of (env_var, config_param). env_var formats the secret as environment variables, each with a key and a value. env_var is suitable for Seldon Core v1 and Argo Workflows. config_param formats the secret to be compatible with Rclone's HTTP API. config_param is suitable for Seldon Core v2.
         :return: V1CreateRcloneBucketSecretResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['namespace', 'remote', 'body']  # noqa: E501
+        all_params = ['namespace', 'remote', 'body', 'format']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -219,14 +221,16 @@
         path_params = {}
         if 'namespace' in params:
             path_params['namespace'] = params['namespace']  # noqa: E501
         if 'remote' in params:
             path_params['remote'] = params['remote']  # noqa: E501
 
         query_params = []
+        if 'format' in params:
+            query_params.append(('format', params['format']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -605,14 +609,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.secrets_service_list_secrets(namespace, secret_type, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str namespace: The namespace to list secrets in. (required)
         :param str secret_type: The secret type, can be one of (`bucket`, `registry`) or `all` to list all secrets used by Seldon Deploy. (required)
+        :param str bucket_secret_format: Optional filter for the format of bucket secrets. Only applicable when `secret_type` is `bucket.`
         :return: V1ListSecretsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.secrets_service_list_secrets_with_http_info(namespace, secret_type, **kwargs)  # noqa: E501
@@ -627,20 +632,21 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.secrets_service_list_secrets_with_http_info(namespace, secret_type, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str namespace: The namespace to list secrets in. (required)
         :param str secret_type: The secret type, can be one of (`bucket`, `registry`) or `all` to list all secrets used by Seldon Deploy. (required)
+        :param str bucket_secret_format: Optional filter for the format of bucket secrets. Only applicable when `secret_type` is `bucket.`
         :return: V1ListSecretsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['namespace', 'secret_type']  # noqa: E501
+        all_params = ['namespace', 'secret_type', 'bucket_secret_format']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -665,14 +671,16 @@
         path_params = {}
         if 'namespace' in params:
             path_params['namespace'] = params['namespace']  # noqa: E501
         if 'secret_type' in params:
             path_params['secretType'] = params['secret_type']  # noqa: E501
 
         query_params = []
+        if 'bucket_secret_format' in params:
+            query_params.append(('bucketSecretFormat', params['bucket_secret_format']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api/seldon_deployments_api.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api/seldon_deployments_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/api_client.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self.authenticator = authenticator
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.0.1/python'
+        self.user_agent = 'Swagger-Codegen/2.1.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/base.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/base.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/openid.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/openid.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,18 @@
             authorize_params = {"resource": config.oidc_resource}
             access_token_params = {"resource": config.oidc_resource}
 
         server_metadata_url = f"{config.oidc_server}/.well-known/openid-configuration"
 
         self._app = OAuth2Mixin(
             framework=FrameworkIntegration,
-            client_kwargs={"verify": config.verify_ssl},
+            client_kwargs={
+                "verify": config.verify_ssl,
+                "code_challenge_method": "S256",
+            },
             client_id=config.oidc_client_id,
             client_secret=config.oidc_client_secret,
             server_metadata_url=server_metadata_url,
             authorize_params=authorize_params,
             access_token_params=access_token_params,
         )
         self._app.client_cls = OAuth2Session
@@ -101,19 +104,21 @@
         )
 
         return _get_token(token)
 
     def _use_authorization_code(self):
         deploy_callback_url = f"{self._host}/seldon-deploy/auth/callback"
 
-        request_url = self._app.create_authorization_url(
+        auth_code_request = self._app.create_authorization_url(
             redirect_uri=deploy_callback_url,
             state=self._AuthCodeState,
             scope=self._config.scope,
-        )["url"]
+        )
+        request_url = auth_code_request["url"]
+        code_verifier = auth_code_request["code_verifier"]
 
         webbrowser.open_new_tab(request_url)
         print(
             "The following URL should have opened now on a new tab, where you "
             "will be able to log in.\n"
             "If it hasn't, please copy the following URL into a browser.\n"
             "Once you have logged in, you will be redirected and will be shown a code "
@@ -124,14 +129,15 @@
         response_code_query = urlencode({"code": response_code})
         response_url = f"{deploy_callback_url}?{response_code_query}"
 
         token = self._app.fetch_access_token(
             authorization_response=response_url,
             redirect_uri=deploy_callback_url,
             scope=self._config.scope,
+            code_verifier=code_verifier,
         )
 
         return _get_token(token)
 
     def _get_response_code(self):
         response_code = None
         while not response_code:
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/auth/session.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/auth/session.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/configuration.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,9 +279,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1alpha1\n"\
-               "SDK Package Version: 2.0.1".\
+               "SDK Package Version: 2.1.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/__init__.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,15 @@
 from seldon_deploy_sdk.models.typed_local_object_reference import TypedLocalObjectReference
 from seldon_deploy_sdk.models.uid import UID
 from seldon_deploy_sdk.models.uri_scheme import URIScheme
 from seldon_deploy_sdk.models.unsatisfiable_constraint_action import UnsatisfiableConstraintAction
 from seldon_deploy_sdk.models.user_info import UserInfo
 from seldon_deploy_sdk.models.v1_add_user_to_group_response import V1AddUserToGroupResponse
 from seldon_deploy_sdk.models.v1_artifact_type import V1ArtifactType
+from seldon_deploy_sdk.models.v1_bucket_secret_format import V1BucketSecretFormat
 from seldon_deploy_sdk.models.v1_create_gcs_bucket_secret_response import V1CreateGCSBucketSecretResponse
 from seldon_deploy_sdk.models.v1_create_group_request import V1CreateGroupRequest
 from seldon_deploy_sdk.models.v1_create_group_response import V1CreateGroupResponse
 from seldon_deploy_sdk.models.v1_create_policy_response import V1CreatePolicyResponse
 from seldon_deploy_sdk.models.v1_create_rclone_bucket_secret_response import V1CreateRcloneBucketSecretResponse
 from seldon_deploy_sdk.models.v1_create_registry_secret_response import V1CreateRegistrySecretResponse
 from seldon_deploy_sdk.models.v1_create_s3_bucket_secret_response import V1CreateS3BucketSecretResponse
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/advanced_config.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/advanced_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/affinity.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/alibi_explainer_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/alibi_explainer_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/application_log.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/application_log.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/application_logs_params.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/application_logs_params.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/application_logs_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/application_logs_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/audit_log.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/aws_elastic_block_store_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/aws_elastic_block_store_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_data_disk_caching_mode.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_data_disk_caching_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_data_disk_kind.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_data_disk_kind.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/azure_file_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/azure_file_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/basic_detector_configuration.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/basic_detector_configuration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_definition.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,26 +148,26 @@
 
         self._batch_interval = batch_interval
 
     @property
     def batch_method(self):
         """Gets the batch_method of this BatchJobDefinition.  # noqa: E501
 
-        Batch Method (predict)  # noqa: E501
+        Batch Method (predict, feedback (for SCv1))  # noqa: E501
 
         :return: The batch_method of this BatchJobDefinition.  # noqa: E501
         :rtype: str
         """
         return self._batch_method
 
     @batch_method.setter
     def batch_method(self, batch_method):
         """Sets the batch_method of this BatchJobDefinition.
 
-        Batch Method (predict)  # noqa: E501
+        Batch Method (predict, feedback (for SCv1))  # noqa: E501
 
         :param batch_method: The batch_method of this BatchJobDefinition.  # noqa: E501
         :type: str
         """
 
         self._batch_method = batch_method
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_description.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_description.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_description_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_description_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_get_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_get_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_job_post_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_job_post_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/batch_jobs_list_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/batch_jobs_list_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/capabilities.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/capability.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/capability.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ceph_fs_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ceph_fs_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/cinder_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/cinder_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/client_ip_config.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/client_ip_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/cluster_info.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/cluster_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/component.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/component.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/condition_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/condition_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/conditions.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/conditions.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_env_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_env_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_key_selector.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_key_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_projection.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/config_map_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/config_map_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_port.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_port.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state_running.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state_running.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state_terminated.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state_terminated.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_state_waiting.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_state_waiting.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/container_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/container_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/cross_version_object_reference.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/cross_version_object_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/csi_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/csi_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_feature_data.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_feature_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_strategy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/deployment_strategy_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/deployment_strategy_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_config_data.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_config_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_configuration.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_configuration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_data.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_deployment_configuration.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_deployment_configuration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/detector_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/detector_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/dns_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/dns_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/downward_api_projection.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/downward_api_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/downward_api_volume_file.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/downward_api_volume_file.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/downward_api_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/downward_api_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/empty_dir_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/empty_dir_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/endpoint.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/endpoint_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/endpoint_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/env_from_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/env_var.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/env_var.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/env_var_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ephemeral_container.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ephemeral_container.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ephemeral_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ephemeral_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/error.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/error.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/exec_action.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/exec_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_candidate.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_candidate.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_mirror.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_mirror.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/experiment_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/experiment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/explainer.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/explainer.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/explainer_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/explainer_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/external_metric_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/external_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/fallback.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/fallback.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/fc_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/fc_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution_bucket.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution_bucket.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution_parameters.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution_parameters.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_distribution_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_distribution_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_filter.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_filter.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_interaction.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_interaction.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_statistics_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_statistics_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_stats.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_stats.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/feature_stats_bucket.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/feature_stats_bucket.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/fields_v1.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/fields_v1.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/file_diff.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/file_diff.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/finalizer_name.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/finalizer_name.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/flex_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/flex_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/flocker_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/flocker_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/gce_persistent_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/gce_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/git_repo_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/git_repo_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/glusterfs_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/glusterfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/handler.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/handler.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/health_check_info.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/health_check_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/horizontal_pod_autoscaler_behavior.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/horizontal_pod_autoscaler_behavior.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/horizontal_pod_autoscaler_config.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/horizontal_pod_autoscaler_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/host_alias.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/host_alias.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/host_path_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/host_path_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/host_path_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/host_path_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/hpa_scaling_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/hpa_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/hpa_scaling_policy_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/hpa_scaling_policy_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/hpa_scaling_rules.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/hpa_scaling_rules.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/http_get_action.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/http_get_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/http_header.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/http_header.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/int_or_string.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/int_or_string.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ip_family.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ip_family.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/iscsi_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/iscsi_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/join_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/join_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/key_to_path.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/key_to_path.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/label_selector.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/label_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/label_selector_operator.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/label_selector_operator.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/label_selector_requirement.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/label_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/lifecycle.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/lifecycle.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/list_meta.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/list_meta.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/local_object_reference.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/logger.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/logger.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/logger_mode.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/logger_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/logging_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/managed_fields_entry.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/managed_fields_entry.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/managed_fields_operation_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/managed_fields_operation_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/message.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/message.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/metric_source_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/metric_source_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/metric_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/metric_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/metric_target_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/metric_target_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/model.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/model.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/model_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/model_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/model_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/model_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/monitor_input_data.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/monitor_input_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/mount_propagation_mode.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/mount_propagation_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_condition.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_condition.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_condition_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_condition_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_phase.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_phase.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/namespace_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/namespace_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/nfs_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/nfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_affinity.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_phase.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_phase.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector_operator.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector_operator.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector_requirement.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/node_selector_term.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/object_field_selector.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/object_meta.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/object_meta.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/object_metric_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/object_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/owner_reference.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/owner_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/parameter.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/parameter.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/parameter_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/parameter_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/parmeter_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/parmeter_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_access_mode.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_access_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_claim_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_claim_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_claim_template.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_claim_template.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_claim_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_claim_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/persistent_volume_mode.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/persistent_volume_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/photon_persistent_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/photon_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_batch.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_batch.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_output.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_output.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pipeline_step.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_affinity.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_affinity_term.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_anti_affinity.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_condition.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_condition.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_condition_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_condition_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_dns_config.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_dns_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_dns_config_option.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_dns_config_option.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_fs_group_change_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_fs_group_change_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_ip.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_ip.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_phase.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_phase.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_qos_class.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_qos_class.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_readiness_gate.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_readiness_gate.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_security_context.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_security_context.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pod_template_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pods_metric_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pods_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/portworx_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/portworx_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit_implementation.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit_implementation.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit_method.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit_method.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictive_unit_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictive_unit_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/predictor_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/predictor_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/preemption_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/preemption_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/preferred_scheduling_term.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/probe.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/probe.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/proc_mount_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/proc_mount_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/projected_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/projected_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/protobuf_any.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/protobuf_null_value.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/protocol.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/protocol.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/pull_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/pull_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/quantity.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/quantity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/quobyte_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/quobyte_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/rbd_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/rbd_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_field_selector.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_field_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_metric_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_name.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_name.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_requirements.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/resource_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/restart_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/restart_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/rolling_update_deployment.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/rolling_update_deployment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/rpc_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scale_io_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scale_io_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scale_triggers.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scale_triggers.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scaled_object_auth_ref.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scaled_object_auth_ref.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/scaling_policy_select.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/scaling_policy_select.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/se_linux_options.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/se_linux_options.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seccomp_profile.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seccomp_profile.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seccomp_profile_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seccomp_profile_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_env_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_env_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_key_selector.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_key_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_projection.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/secret_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/secret_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/security_context.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/security_context.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_addressable.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_addressable.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_deployment_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_deployment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_experiment.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_experiment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_hpa_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_hpa_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_model.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_model.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_model_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_model_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pdb_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pdb_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pipeline.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pipeline.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pipeline_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pipeline_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_pod_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_pod_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/seldon_scaled_object_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/seldon_scaled_object_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/server_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/server_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_account_token_projection.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_account_token_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_affinity.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_external_traffic_policy_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_external_traffic_policy_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_list.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_port.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_port.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/service_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/service_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/session_affinity_config.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/session_affinity_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/ssl.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/ssl.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/status_state.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/status_state.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/storage_medium.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/storage_medium.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/storage_os_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/storage_os_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/svc_orch_spec.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/svc_orch_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/sysctl.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/sysctl.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/taint_effect.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/taint_effect.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/tcp_socket_action.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/tcp_socket_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/termination_message_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/termination_message_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/time.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/time.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/toleration.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/toleration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/toleration_operator.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/toleration_operator.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/topology_spread_constraint.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/topology_spread_constraint.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/transport.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/transport.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/typed_local_object_reference.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/typed_local_object_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/uid.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/uid.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/unsatisfiable_constraint_action.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/unsatisfiable_constraint_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/uri_scheme.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/uri_scheme.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/user_info.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/user_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_add_user_to_group_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_add_user_to_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_artifact_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_artifact_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     MLFLOW = "MLFLOW"
     PYTORCH = "PYTORCH"
     ONNX = "ONNX"
     TENSORRT = "TENSORRT"
     ALIBI_EXPLAIN = "ALIBI_EXPLAIN"
     ALIBI_DETECT = "ALIBI_DETECT"
     HUGGINGFACE = "HUGGINGFACE"
+    MLSERVER_PYTHON = "MLSERVER_PYTHON"
+    TRITON_PYTHON = "TRITON_PYTHON"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_gcs_bucket_secret_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_gcs_bucket_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_group_request.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_group_request.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_group_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_policy_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_policy_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_rclone_bucket_secret_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_rclone_bucket_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_registry_secret_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_registry_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_s3_bucket_secret_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_s3_bucket_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_user_request.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_user_request.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_create_user_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_create_user_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_data_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_data_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_default_protocol.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_default_protocol.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_group_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_policy_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_policy_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_secret_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_user_from_group_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_user_from_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_delete_user_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_delete_user_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_dependency_health_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_dependency_health_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deploy_dependency.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deploy_dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     allowed enum values
     """
     ALL = "ALL"
     PROMETHEUS = "PROMETHEUS"
     ELASTICSEARCH = "ELASTICSEARCH"
     ALERTMANAGER = "ALERTMANAGER"
     POSTGRES = "POSTGRES"
-    KEYCLOACK = "KEYCLOACK"
+    KEYCLOAK = "KEYCLOAK"
     KAFKA = "KAFKA"
     SELDONCORE_V1 = "SELDONCORE_V1"
     SELDONCORE_V2 = "SELDONCORE_V2"
     GITEA = "GITEA"
     ARGOCD = "ARGOCD"
     ARGOWF = "ARGOWF"
     KNATIVE = "KNATIVE"
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deploy_dependency_health.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deploy_dependency_health.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deploy_dependency_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deploy_dependency_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deployment_status.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deployment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_deployment_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_deployment_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_feature_category_schema.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_feature_category_schema.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_feature_schema.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_feature_schema.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_feature_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_feature_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_firing_alert.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_firing_alert.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_group_members_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_group_members_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_groups_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_groups_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_permissions_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_permissions_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_policy_targets_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_policy_targets_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_user_groups_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_user_groups_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_get_users_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_get_users_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_group.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_group.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_group_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_group_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_list_alerts_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_list_alerts_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_list_secrets_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_list_secrets_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_create_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_create_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_delete_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_delete_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_list_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_list_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_model_metadata_update_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_model_metadata_update_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_prediction_schema.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_prediction_schema.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_rclone_config.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_secret_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,67 +13,44 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class V1RcloneConfig(object):
+class V1SecretType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    ALL = "all"
+    BUCKET = "bucket"
+    REGISTRY = "registry"
+
+    """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'variables': 'dict(str, str)'
     }
 
     attribute_map = {
-        'variables': 'variables'
     }
 
-    def __init__(self, variables=None):  # noqa: E501
-        """V1RcloneConfig - a model defined in Swagger"""  # noqa: E501
-
-        self._variables = None
+    def __init__(self):  # noqa: E501
+        """V1SecretType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
-        if variables is not None:
-            self.variables = variables
-
-    @property
-    def variables(self):
-        """Gets the variables of this V1RcloneConfig.  # noqa: E501
-
-        The rclone key value pairs for your secret, see the documentation for more detail.  # noqa: E501
-
-        :return: The variables of this V1RcloneConfig.  # noqa: E501
-        :rtype: dict(str, str)
-        """
-        return self._variables
-
-    @variables.setter
-    def variables(self, variables):
-        """Sets the variables of this V1RcloneConfig.
-
-        The rclone key value pairs for your secret, see the documentation for more detail.  # noqa: E501
-
-        :param variables: The variables of this V1RcloneConfig.  # noqa: E501
-        :type: dict(str, str)
-        """
-
-        self._variables = variables
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -87,15 +64,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(V1RcloneConfig, dict):
+        if issubclass(V1SecretType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -103,15 +80,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1RcloneConfig):
+        if not isinstance(other, V1SecretType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_reset_user_password_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_reset_user_password_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_resource_action_pair.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_resource_action_pair.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_runtime_defaults.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_runtime_defaults.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_runtime_metadata.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_runtime_metadata.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_runtime_metadata_list_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_runtime_metadata_list_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_s3_credentials.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_s3_credentials.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_secret.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_secret.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,33 +28,38 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'secret_name': 'str',
-        'secret_type': 'V1SecretType'
+        'secret_type': 'V1SecretType',
+        'bucket_secret_format': 'V1BucketSecretFormat'
     }
 
     attribute_map = {
         'secret_name': 'secretName',
-        'secret_type': 'secretType'
+        'secret_type': 'secretType',
+        'bucket_secret_format': 'bucketSecretFormat'
     }
 
-    def __init__(self, secret_name=None, secret_type=None):  # noqa: E501
+    def __init__(self, secret_name=None, secret_type=None, bucket_secret_format=None):  # noqa: E501
         """V1Secret - a model defined in Swagger"""  # noqa: E501
 
         self._secret_name = None
         self._secret_type = None
+        self._bucket_secret_format = None
         self.discriminator = None
 
         if secret_name is not None:
             self.secret_name = secret_name
         if secret_type is not None:
             self.secret_type = secret_type
+        if bucket_secret_format is not None:
+            self.bucket_secret_format = bucket_secret_format
 
     @property
     def secret_name(self):
         """Gets the secret_name of this V1Secret.  # noqa: E501
 
 
         :return: The secret_name of this V1Secret.  # noqa: E501
@@ -90,14 +95,37 @@
 
         :param secret_type: The secret_type of this V1Secret.  # noqa: E501
         :type: V1SecretType
         """
 
         self._secret_type = secret_type
 
+    @property
+    def bucket_secret_format(self):
+        """Gets the bucket_secret_format of this V1Secret.  # noqa: E501
+
+        Only available for bucket secrets.  # noqa: E501
+
+        :return: The bucket_secret_format of this V1Secret.  # noqa: E501
+        :rtype: V1BucketSecretFormat
+        """
+        return self._bucket_secret_format
+
+    @bucket_secret_format.setter
+    def bucket_secret_format(self, bucket_secret_format):
+        """Sets the bucket_secret_format of this V1Secret.
+
+        Only available for bucket secrets.  # noqa: E501
+
+        :param bucket_secret_format: The bucket_secret_format of this V1Secret.  # noqa: E501
+        :type: V1BucketSecretFormat
+        """
+
+        self._bucket_secret_format = bucket_secret_format
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_secret_type.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_bucket_secret_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class V1SecretType(object):
+class V1BucketSecretFormat(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    ALL = "all"
-    BUCKET = "bucket"
-    REGISTRY = "registry"
+    ENV_VAR = "env_var"
+    CONFIG_PARAM = "config_param"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -40,15 +39,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """V1SecretType - a model defined in Swagger"""  # noqa: E501
+        """V1BucketSecretFormat - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -64,15 +63,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(V1SecretType, dict):
+        if issubclass(V1BucketSecretFormat, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -80,15 +79,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1SecretType):
+        if not isinstance(other, V1BucketSecretFormat):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_trigger_test_alert_response.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_trigger_test_alert_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_user.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_user.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/v1_user_policy.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/v1_user_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/version_info.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/version_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume_device.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume_mount.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/volume_projection.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/volume_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/vsphere_virtual_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/vsphere_virtual_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/weighted_pod_affinity_term.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/models/windows_security_context_options.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/models/windows_security_context_options.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk/rest.py` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/seldon_deploy_sdk.egg-info/SOURCES.txt` & `seldon-deploy-sdk-2.1.0/seldon_deploy_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,15 @@
 seldon_deploy_sdk/models/typed_local_object_reference.py
 seldon_deploy_sdk/models/uid.py
 seldon_deploy_sdk/models/unsatisfiable_constraint_action.py
 seldon_deploy_sdk/models/uri_scheme.py
 seldon_deploy_sdk/models/user_info.py
 seldon_deploy_sdk/models/v1_add_user_to_group_response.py
 seldon_deploy_sdk/models/v1_artifact_type.py
+seldon_deploy_sdk/models/v1_bucket_secret_format.py
 seldon_deploy_sdk/models/v1_create_gcs_bucket_secret_response.py
 seldon_deploy_sdk/models/v1_create_group_request.py
 seldon_deploy_sdk/models/v1_create_group_response.py
 seldon_deploy_sdk/models/v1_create_policy_response.py
 seldon_deploy_sdk/models/v1_create_rclone_bucket_secret_response.py
 seldon_deploy_sdk/models/v1_create_registry_secret_response.py
 seldon_deploy_sdk/models/v1_create_s3_bucket_secret_response.py
@@ -653,14 +654,15 @@
 test/test_typed_local_object_reference.py
 test/test_uid.py
 test/test_unsatisfiable_constraint_action.py
 test/test_uri_scheme.py
 test/test_user_info.py
 test/test_v1_add_user_to_group_response.py
 test/test_v1_artifact_type.py
+test/test_v1_bucket_secret_format.py
 test/test_v1_create_gcs_bucket_secret_response.py
 test/test_v1_create_group_request.py
 test/test_v1_create_group_response.py
 test/test_v1_create_policy_response.py
 test/test_v1_create_rclone_bucket_secret_response.py
 test/test_v1_create_registry_secret_response.py
 test/test_v1_create_s3_bucket_secret_response.py
```

### Comparing `seldon-deploy-sdk-2.0.1/setup.py` & `seldon-deploy-sdk-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "seldon-deploy-sdk"
-VERSION = "2.0.1"
+VERSION = "2.1.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `seldon-deploy-sdk-2.0.1/test/test_advanced_config.py` & `seldon-deploy-sdk-2.1.0/test/test_advanced_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_affinity.py` & `seldon-deploy-sdk-2.1.0/test/test_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_alerting_service_api.py` & `seldon-deploy-sdk-2.1.0/test/test_alerting_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_alibi_explainer_type.py` & `seldon-deploy-sdk-2.1.0/test/test_alibi_explainer_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_application_log.py` & `seldon-deploy-sdk-2.1.0/test/test_application_log.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_application_logs_api.py` & `seldon-deploy-sdk-2.1.0/test/test_application_logs_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_application_logs_params.py` & `seldon-deploy-sdk-2.1.0/test/test_application_logs_params.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_application_logs_response.py` & `seldon-deploy-sdk-2.1.0/test/test_application_logs_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_audit_log.py` & `seldon-deploy-sdk-2.1.0/test/test_audit_log.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_aws_elastic_block_store_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_aws_elastic_block_store_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_azure_data_disk_caching_mode.py` & `seldon-deploy-sdk-2.1.0/test/test_azure_data_disk_caching_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_azure_data_disk_kind.py` & `seldon-deploy-sdk-2.1.0/test/test_azure_data_disk_kind.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_azure_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_azure_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_azure_file_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_azure_file_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_basic_detector_configuration.py` & `seldon-deploy-sdk-2.1.0/test/test_basic_detector_configuration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_batch_job_definition.py` & `seldon-deploy-sdk-2.1.0/test/test_batch_job_definition.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_batch_job_description.py` & `seldon-deploy-sdk-2.1.0/test/test_batch_job_description.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_batch_job_description_list.py` & `seldon-deploy-sdk-2.1.0/test/test_batch_job_description_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_batch_job_get_response.py` & `seldon-deploy-sdk-2.1.0/test/test_batch_job_get_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_batch_job_post_response.py` & `seldon-deploy-sdk-2.1.0/test/test_batch_job_post_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_batch_jobs_api.py` & `seldon-deploy-sdk-2.1.0/test/test_batch_jobs_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_batch_jobs_list_response.py` & `seldon-deploy-sdk-2.1.0/test/test_batch_jobs_list_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_capabilities.py` & `seldon-deploy-sdk-2.1.0/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_capability.py` & `seldon-deploy-sdk-2.1.0/test/test_capability.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_ceph_fs_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_ceph_fs_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_cinder_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_cinder_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_client_ip_config.py` & `seldon-deploy-sdk-2.1.0/test/test_client_ip_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_cluster_info.py` & `seldon-deploy-sdk-2.1.0/test/test_cluster_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_component.py` & `seldon-deploy-sdk-2.1.0/test/test_component.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_condition_status.py` & `seldon-deploy-sdk-2.1.0/test/test_condition_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_conditions.py` & `seldon-deploy-sdk-2.1.0/test/test_conditions.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_config_map_env_source.py` & `seldon-deploy-sdk-2.1.0/test/test_config_map_env_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_config_map_key_selector.py` & `seldon-deploy-sdk-2.1.0/test/test_config_map_key_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_config_map_projection.py` & `seldon-deploy-sdk-2.1.0/test/test_config_map_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_config_map_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_config_map_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_container.py` & `seldon-deploy-sdk-2.1.0/test/test_container.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_container_port.py` & `seldon-deploy-sdk-2.1.0/test/test_container_port.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_container_state.py` & `seldon-deploy-sdk-2.1.0/test/test_container_state.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_container_state_running.py` & `seldon-deploy-sdk-2.1.0/test/test_container_state_running.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_container_state_terminated.py` & `seldon-deploy-sdk-2.1.0/test/test_container_state_terminated.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_container_state_waiting.py` & `seldon-deploy-sdk-2.1.0/test/test_container_state_waiting.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_container_status.py` & `seldon-deploy-sdk-2.1.0/test/test_container_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_cross_version_object_reference.py` & `seldon-deploy-sdk-2.1.0/test/test_cross_version_object_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_csi_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_csi_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_deployment.py` & `seldon-deploy-sdk-2.1.0/test/test_deployment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_deployment_feature_data.py` & `seldon-deploy-sdk-2.1.0/test/test_deployment_feature_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_deployment_list.py` & `seldon-deploy-sdk-2.1.0/test/test_deployment_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_deployment_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_deployment_status.py` & `seldon-deploy-sdk-2.1.0/test/test_deployment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_deployment_strategy.py` & `seldon-deploy-sdk-2.1.0/test/test_deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_deployment_strategy_type.py` & `seldon-deploy-sdk-2.1.0/test/test_deployment_strategy_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_detector_config_data.py` & `seldon-deploy-sdk-2.1.0/test/test_detector_config_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_detector_configuration.py` & `seldon-deploy-sdk-2.1.0/test/test_detector_configuration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_detector_data.py` & `seldon-deploy-sdk-2.1.0/test/test_detector_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_detector_deployment_configuration.py` & `seldon-deploy-sdk-2.1.0/test/test_detector_deployment_configuration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_detector_status.py` & `seldon-deploy-sdk-2.1.0/test/test_detector_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_dns_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_dns_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_downward_api_projection.py` & `seldon-deploy-sdk-2.1.0/test/test_downward_api_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_downward_api_volume_file.py` & `seldon-deploy-sdk-2.1.0/test/test_downward_api_volume_file.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_downward_api_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_downward_api_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_drift_detector_api.py` & `seldon-deploy-sdk-2.1.0/test/test_drift_detector_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_empty_dir_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_empty_dir_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_endpoint.py` & `seldon-deploy-sdk-2.1.0/test/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_endpoint_type.py` & `seldon-deploy-sdk-2.1.0/test/test_endpoint_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_env_from_source.py` & `seldon-deploy-sdk-2.1.0/test/test_env_from_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_env_var.py` & `seldon-deploy-sdk-2.1.0/test/test_env_var.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_env_var_source.py` & `seldon-deploy-sdk-2.1.0/test/test_env_var_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_environment_api.py` & `seldon-deploy-sdk-2.1.0/test/test_environment_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_ephemeral_container.py` & `seldon-deploy-sdk-2.1.0/test/test_ephemeral_container.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_ephemeral_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_ephemeral_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_error.py` & `seldon-deploy-sdk-2.1.0/test/test_error.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_exec_action.py` & `seldon-deploy-sdk-2.1.0/test/test_exec_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_experiment.py` & `seldon-deploy-sdk-2.1.0/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_experiment_candidate.py` & `seldon-deploy-sdk-2.1.0/test/test_experiment_candidate.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_experiment_mirror.py` & `seldon-deploy-sdk-2.1.0/test/test_experiment_mirror.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_experiment_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_experiment_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_experiment_status.py` & `seldon-deploy-sdk-2.1.0/test/test_experiment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_experiments_api.py` & `seldon-deploy-sdk-2.1.0/test/test_experiments_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_explain_api.py` & `seldon-deploy-sdk-2.1.0/test/test_explain_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_explainer.py` & `seldon-deploy-sdk-2.1.0/test/test_explainer.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_explainer_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_external_metric_source.py` & `seldon-deploy-sdk-2.1.0/test/test_external_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_fallback.py` & `seldon-deploy-sdk-2.1.0/test/test_fallback.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_fc_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_fc_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_distribution.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_distribution.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_distribution_bucket.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_distribution_bucket.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_distribution_parameters.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_distribution_parameters.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_distribution_response.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_distribution_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_filter.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_filter.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_interaction.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_interaction.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_statistics_response.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_statistics_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_stats.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_stats.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_feature_stats_bucket.py` & `seldon-deploy-sdk-2.1.0/test/test_feature_stats_bucket.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_fields_v1.py` & `seldon-deploy-sdk-2.1.0/test/test_fields_v1.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_file_diff.py` & `seldon-deploy-sdk-2.1.0/test/test_file_diff.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_finalizer_name.py` & `seldon-deploy-sdk-2.1.0/test/test_finalizer_name.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_flex_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_flex_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_flocker_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_flocker_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_gce_persistent_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_gce_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_git_ops_api.py` & `seldon-deploy-sdk-2.1.0/test/test_git_ops_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
     def test_read_experiment_git_logs(self):
         """Test case for read_experiment_git_logs
 
         """
         pass
 
+    def test_read_git_diffs(self):
+        """Test case for read_git_diffs
+
+        """
+        pass
+
     def test_read_git_ops_status(self):
         """Test case for read_git_ops_status
 
         """
         pass
 
     def test_read_model_git_diff(self):
```

### Comparing `seldon-deploy-sdk-2.0.1/test/test_git_repo_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_git_repo_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_glusterfs_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_glusterfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_handler.py` & `seldon-deploy-sdk-2.1.0/test/test_handler.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_health_check_info.py` & `seldon-deploy-sdk-2.1.0/test/test_health_check_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_healthcheck_service_api.py` & `seldon-deploy-sdk-2.1.0/test/test_healthcheck_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_horizontal_pod_autoscaler_behavior.py` & `seldon-deploy-sdk-2.1.0/test/test_horizontal_pod_autoscaler_behavior.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_horizontal_pod_autoscaler_config.py` & `seldon-deploy-sdk-2.1.0/test/test_horizontal_pod_autoscaler_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_host_alias.py` & `seldon-deploy-sdk-2.1.0/test/test_host_alias.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_host_path_type.py` & `seldon-deploy-sdk-2.1.0/test/test_host_path_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_host_path_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_host_path_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_hpa_scaling_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_hpa_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_hpa_scaling_policy_type.py` & `seldon-deploy-sdk-2.1.0/test/test_hpa_scaling_policy_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_hpa_scaling_rules.py` & `seldon-deploy-sdk-2.1.0/test/test_hpa_scaling_rules.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_http_get_action.py` & `seldon-deploy-sdk-2.1.0/test/test_http_get_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_http_header.py` & `seldon-deploy-sdk-2.1.0/test/test_http_header.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_int_or_string.py` & `seldon-deploy-sdk-2.1.0/test/test_int_or_string.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_ip_family.py` & `seldon-deploy-sdk-2.1.0/test/test_ip_family.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_iscsi_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_iscsi_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_join_type.py` & `seldon-deploy-sdk-2.1.0/test/test_join_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_key_to_path.py` & `seldon-deploy-sdk-2.1.0/test/test_key_to_path.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_kubernetes_resources_api.py` & `seldon-deploy-sdk-2.1.0/test/test_kubernetes_resources_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_label_selector.py` & `seldon-deploy-sdk-2.1.0/test/test_label_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_label_selector_operator.py` & `seldon-deploy-sdk-2.1.0/test/test_label_selector_operator.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_label_selector_requirement.py` & `seldon-deploy-sdk-2.1.0/test/test_label_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_lifecycle.py` & `seldon-deploy-sdk-2.1.0/test/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_list_meta.py` & `seldon-deploy-sdk-2.1.0/test/test_list_meta.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_loadtest_jobs_api.py` & `seldon-deploy-sdk-2.1.0/test/test_loadtest_jobs_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_local_object_reference.py` & `seldon-deploy-sdk-2.1.0/test/test_local_object_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_logger.py` & `seldon-deploy-sdk-2.1.0/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_logger_mode.py` & `seldon-deploy-sdk-2.1.0/test/test_logger_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_logging_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_managed_fields_entry.py` & `seldon-deploy-sdk-2.1.0/test/test_managed_fields_entry.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_managed_fields_operation_type.py` & `seldon-deploy-sdk-2.1.0/test/test_managed_fields_operation_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_message.py` & `seldon-deploy-sdk-2.1.0/test/test_message.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_metric_source_type.py` & `seldon-deploy-sdk-2.1.0/test/test_metric_source_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_metric_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_metric_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_metric_target_type.py` & `seldon-deploy-sdk-2.1.0/test/test_metric_target_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_metrics_server_api.py` & `seldon-deploy-sdk-2.1.0/test/test_metrics_server_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_model.py` & `seldon-deploy-sdk-2.1.0/test/test_model.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_model_metadata_service_api.py` & `seldon-deploy-sdk-2.1.0/test/test_model_metadata_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_model_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_model_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_model_status.py` & `seldon-deploy-sdk-2.1.0/test/test_model_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_models_api.py` & `seldon-deploy-sdk-2.1.0/test/test_models_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_monitor_api.py` & `seldon-deploy-sdk-2.1.0/test/test_monitor_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_monitor_input_data.py` & `seldon-deploy-sdk-2.1.0/test/test_monitor_input_data.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_mount_propagation_mode.py` & `seldon-deploy-sdk-2.1.0/test/test_mount_propagation_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_namespace.py` & `seldon-deploy-sdk-2.1.0/test/test_namespace.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_namespace_condition.py` & `seldon-deploy-sdk-2.1.0/test/test_namespace_condition.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_namespace_condition_type.py` & `seldon-deploy-sdk-2.1.0/test/test_namespace_condition_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_namespace_phase.py` & `seldon-deploy-sdk-2.1.0/test/test_namespace_phase.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_namespace_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_namespace_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_namespace_status.py` & `seldon-deploy-sdk-2.1.0/test/test_namespace_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_nfs_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_nfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_node_affinity.py` & `seldon-deploy-sdk-2.1.0/test/test_node_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_node_phase.py` & `seldon-deploy-sdk-2.1.0/test/test_node_phase.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_node_selector.py` & `seldon-deploy-sdk-2.1.0/test/test_node_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_node_selector_operator.py` & `seldon-deploy-sdk-2.1.0/test/test_node_selector_operator.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_node_selector_requirement.py` & `seldon-deploy-sdk-2.1.0/test/test_node_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_node_selector_term.py` & `seldon-deploy-sdk-2.1.0/test/test_node_selector_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_object_field_selector.py` & `seldon-deploy-sdk-2.1.0/test/test_object_field_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_object_meta.py` & `seldon-deploy-sdk-2.1.0/test/test_object_meta.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_object_metric_source.py` & `seldon-deploy-sdk-2.1.0/test/test_object_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_outlier_detector_api.py` & `seldon-deploy-sdk-2.1.0/test/test_outlier_detector_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_owner_reference.py` & `seldon-deploy-sdk-2.1.0/test/test_owner_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_parameter.py` & `seldon-deploy-sdk-2.1.0/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_parameter_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_parameter_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_parmeter_type.py` & `seldon-deploy-sdk-2.1.0/test/test_parmeter_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_permission_management_service_api.py` & `seldon-deploy-sdk-2.1.0/test/test_permission_management_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_persistent_volume_access_mode.py` & `seldon-deploy-sdk-2.1.0/test/test_persistent_volume_access_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_persistent_volume_claim_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_persistent_volume_claim_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_persistent_volume_claim_template.py` & `seldon-deploy-sdk-2.1.0/test/test_persistent_volume_claim_template.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_persistent_volume_claim_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_persistent_volume_claim_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_persistent_volume_mode.py` & `seldon-deploy-sdk-2.1.0/test/test_persistent_volume_mode.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_photon_persistent_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_photon_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pipeline.py` & `seldon-deploy-sdk-2.1.0/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pipeline_batch.py` & `seldon-deploy-sdk-2.1.0/test/test_pipeline_batch.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pipeline_output.py` & `seldon-deploy-sdk-2.1.0/test/test_pipeline_output.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pipeline_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pipeline_status.py` & `seldon-deploy-sdk-2.1.0/test/test_pipeline_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pipeline_step.py` & `seldon-deploy-sdk-2.1.0/test/test_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pipelines_api.py` & `seldon-deploy-sdk-2.1.0/test/test_pipelines_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,10 +79,16 @@
 
     def test_update_pipeline(self):
         """Test case for update_pipeline
 
         """
         pass
 
+    def test_update_pipeline_explainer(self):
+        """Test case for update_pipeline_explainer
+
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod.py` & `seldon-deploy-sdk-2.1.0/test/test_pod.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_affinity.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_affinity_term.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_anti_affinity.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_condition.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_condition.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_condition_type.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_condition_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_dns_config.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_dns_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_dns_config_option.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_dns_config_option.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_fs_group_change_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_fs_group_change_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_ip.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_ip.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_list.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_phase.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_phase.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_qos_class.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_qos_class.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_readiness_gate.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_readiness_gate.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_security_context.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_security_context.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_status.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pod_template_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pods_metric_source.py` & `seldon-deploy-sdk-2.1.0/test/test_pods_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_portworx_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_portworx_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_predict_api.py` & `seldon-deploy-sdk-2.1.0/test/test_predict_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_predictive_unit.py` & `seldon-deploy-sdk-2.1.0/test/test_predictive_unit.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_predictive_unit_implementation.py` & `seldon-deploy-sdk-2.1.0/test/test_predictive_unit_implementation.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_predictive_unit_method.py` & `seldon-deploy-sdk-2.1.0/test/test_predictive_unit_method.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_predictive_unit_type.py` & `seldon-deploy-sdk-2.1.0/test/test_predictive_unit_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_predictor_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_predictor_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_preemption_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_preemption_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_preferred_scheduling_term.py` & `seldon-deploy-sdk-2.1.0/test/test_preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_probe.py` & `seldon-deploy-sdk-2.1.0/test/test_probe.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_proc_mount_type.py` & `seldon-deploy-sdk-2.1.0/test/test_proc_mount_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_projected_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_projected_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_protobuf_any.py` & `seldon-deploy-sdk-2.1.0/test/test_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_protobuf_null_value.py` & `seldon-deploy-sdk-2.1.0/test/test_protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_protocol.py` & `seldon-deploy-sdk-2.1.0/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_pull_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_pull_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_quantity.py` & `seldon-deploy-sdk-2.1.0/test/test_quantity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_quobyte_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_quobyte_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_rbd_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_rbd_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_resource_field_selector.py` & `seldon-deploy-sdk-2.1.0/test/test_resource_field_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_resource_list.py` & `seldon-deploy-sdk-2.1.0/test/test_resource_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_resource_metric_source.py` & `seldon-deploy-sdk-2.1.0/test/test_resource_metric_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_resource_name.py` & `seldon-deploy-sdk-2.1.0/test/test_resource_name.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_resource_requirements.py` & `seldon-deploy-sdk-2.1.0/test/test_resource_requirements.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_resource_type.py` & `seldon-deploy-sdk-2.1.0/test/test_resource_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_restart_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_restart_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_rolling_update_deployment.py` & `seldon-deploy-sdk-2.1.0/test/test_rolling_update_deployment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_rpc_status.py` & `seldon-deploy-sdk-2.1.0/test/test_rpc_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_scale_io_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_scale_io_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_scale_triggers.py` & `seldon-deploy-sdk-2.1.0/test/test_scale_triggers.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_scaled_object_auth_ref.py` & `seldon-deploy-sdk-2.1.0/test/test_scaled_object_auth_ref.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_scaling_policy_select.py` & `seldon-deploy-sdk-2.1.0/test/test_scaling_policy_select.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_se_linux_options.py` & `seldon-deploy-sdk-2.1.0/test/test_se_linux_options.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seccomp_profile.py` & `seldon-deploy-sdk-2.1.0/test/test_seccomp_profile.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seccomp_profile_type.py` & `seldon-deploy-sdk-2.1.0/test/test_seccomp_profile_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_secret_env_source.py` & `seldon-deploy-sdk-2.1.0/test/test_secret_env_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_secret_key_selector.py` & `seldon-deploy-sdk-2.1.0/test/test_secret_key_selector.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_secret_projection.py` & `seldon-deploy-sdk-2.1.0/test/test_secret_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_secret_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_secret_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_secrets_service_api.py` & `seldon-deploy-sdk-2.1.0/test/test_secrets_service_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_security_context.py` & `seldon-deploy-sdk-2.1.0/test/test_security_context.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_addressable.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_addressable.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_deployment.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_deployment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_deployment_list.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_deployment_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_deployment_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_deployment_status.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_deployment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_deployments_api.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_deployments_api.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_experiment.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_experiment.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_hpa_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_hpa_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_model.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_model.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_model_list.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_model_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_pdb_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_pdb_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_pipeline.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_pipeline.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_pipeline_list.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_pipeline_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_pod_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_pod_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_seldon_scaled_object_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_seldon_scaled_object_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_server_type.py` & `seldon-deploy-sdk-2.1.0/test/test_server_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service.py` & `seldon-deploy-sdk-2.1.0/test/test_service.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_account_token_projection.py` & `seldon-deploy-sdk-2.1.0/test/test_service_account_token_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_affinity.py` & `seldon-deploy-sdk-2.1.0/test/test_service_affinity.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_external_traffic_policy_type.py` & `seldon-deploy-sdk-2.1.0/test/test_service_external_traffic_policy_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_list.py` & `seldon-deploy-sdk-2.1.0/test/test_service_list.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_port.py` & `seldon-deploy-sdk-2.1.0/test/test_service_port.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_service_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_status.py` & `seldon-deploy-sdk-2.1.0/test/test_service_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_service_type.py` & `seldon-deploy-sdk-2.1.0/test/test_service_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_session_affinity_config.py` & `seldon-deploy-sdk-2.1.0/test/test_session_affinity_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_ssl.py` & `seldon-deploy-sdk-2.1.0/test/test_ssl.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_status_state.py` & `seldon-deploy-sdk-2.1.0/test/test_status_state.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_storage_medium.py` & `seldon-deploy-sdk-2.1.0/test/test_storage_medium.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_storage_os_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_storage_os_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_svc_orch_spec.py` & `seldon-deploy-sdk-2.1.0/test/test_svc_orch_spec.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_sysctl.py` & `seldon-deploy-sdk-2.1.0/test/test_sysctl.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_taint_effect.py` & `seldon-deploy-sdk-2.1.0/test/test_taint_effect.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_tcp_socket_action.py` & `seldon-deploy-sdk-2.1.0/test/test_tcp_socket_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_termination_message_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_termination_message_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_time.py` & `seldon-deploy-sdk-2.1.0/test/test_time.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_toleration.py` & `seldon-deploy-sdk-2.1.0/test/test_toleration.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_toleration_operator.py` & `seldon-deploy-sdk-2.1.0/test/test_toleration_operator.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_topology_spread_constraint.py` & `seldon-deploy-sdk-2.1.0/test/test_topology_spread_constraint.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_transport.py` & `seldon-deploy-sdk-2.1.0/test/test_transport.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_type.py` & `seldon-deploy-sdk-2.1.0/test/test_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_typed_local_object_reference.py` & `seldon-deploy-sdk-2.1.0/test/test_typed_local_object_reference.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_uid.py` & `seldon-deploy-sdk-2.1.0/test/test_uid.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_unsatisfiable_constraint_action.py` & `seldon-deploy-sdk-2.1.0/test/test_unsatisfiable_constraint_action.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_uri_scheme.py` & `seldon-deploy-sdk-2.1.0/test/test_uri_scheme.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_user_info.py` & `seldon-deploy-sdk-2.1.0/test/test_user_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_add_user_to_group_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_add_user_to_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_artifact_type.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_artifact_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_gcs_bucket_secret_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_gcs_bucket_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_group_request.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_group_request.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_group_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_policy_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_policy_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_rclone_bucket_secret_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_rclone_bucket_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_registry_secret_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_registry_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_s3_bucket_secret_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_s3_bucket_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_user_request.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_user_request.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_create_user_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_create_user_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_data_type.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_data_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_default_protocol.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_default_protocol.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_delete_group_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_delete_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_delete_policy_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_delete_policy_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_delete_secret_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_delete_secret_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_delete_user_from_group_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_delete_user_from_group_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_delete_user_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_delete_user_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_dependency_health_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_dependency_health_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_deploy_dependency.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_deploy_dependency.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_deploy_dependency_health.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_deploy_dependency_health.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_deploy_dependency_status.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_deploy_dependency_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_deployment_status.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_deployment_status.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_deployment_type.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_deployment_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_feature_category_schema.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_feature_category_schema.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_feature_schema.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_feature_schema.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_feature_type.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_feature_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_firing_alert.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_firing_alert.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_get_group_members_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_get_group_members_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_get_groups_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_get_groups_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_get_permissions_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_get_permissions_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_get_policy_targets_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_get_policy_targets_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_get_user_groups_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_get_user_groups_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_get_users_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_get_users_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_group.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_group.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_group_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_group_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_list_alerts_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_list_alerts_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_list_secrets_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_list_secrets_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_model.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_model.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_create_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_create_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_delete_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_delete_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_list_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_list_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_model_metadata_update_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_model_metadata_update_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_prediction_schema.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_prediction_schema.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_rclone_config.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_rclone_config.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_reset_user_password_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_reset_user_password_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_resource_action_pair.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_resource_action_pair.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_runtime_defaults.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_runtime_defaults.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_runtime_metadata.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_runtime_metadata.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_runtime_metadata_list_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_runtime_metadata_list_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_s3_credentials.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_s3_credentials.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_secret.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_secret.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_secret_type.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_secret_type.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_trigger_test_alert_response.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_trigger_test_alert_response.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_user.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_user.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_v1_user_policy.py` & `seldon-deploy-sdk-2.1.0/test/test_v1_user_policy.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_version_info.py` & `seldon-deploy-sdk-2.1.0/test/test_version_info.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_volume.py` & `seldon-deploy-sdk-2.1.0/test/test_volume.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_volume_device.py` & `seldon-deploy-sdk-2.1.0/test/test_volume_device.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_volume_mount.py` & `seldon-deploy-sdk-2.1.0/test/test_volume_mount.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_volume_projection.py` & `seldon-deploy-sdk-2.1.0/test/test_volume_projection.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_vsphere_virtual_disk_volume_source.py` & `seldon-deploy-sdk-2.1.0/test/test_vsphere_virtual_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_weighted_pod_affinity_term.py` & `seldon-deploy-sdk-2.1.0/test/test_weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `seldon-deploy-sdk-2.0.1/test/test_windows_security_context_options.py` & `seldon-deploy-sdk-2.1.0/test/test_windows_security_context_options.py`

 * *Files identical despite different names*

