# Comparing `tmp/pht_station-0.2.0.tar.gz` & `tmp/pht_station-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pht_station-0.2.0.tar", max compression
+gzip compressed data, was "pht_station-0.2.1.tar", max compression
```

## Comparing `pht_station-0.2.0.tar` & `pht_station-0.2.1.tar`

### file list

```diff
@@ -1,180 +1,179 @@
--rw-r--r--   0        0        0     1927 2023-06-05 07:01:36.971701 pht_station-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2652 2023-02-06 09:52:28.229709 pht_station-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/.dockerignore
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.847591 pht_station-0.2.0/station/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.568252 pht_station-0.2.0/station/app/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.305183 pht_station-0.2.0/station/app/api/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.288975 pht_station-0.2.0/station/app/api/api_v1/__init__.py
--rw-r--r--   0        0        0     1150 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/api.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.263471 pht_station-0.2.0/station/app/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     3612 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/endpoints/airflow.py
--rw-r--r--   0        0        0     7514 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/endpoints/datasets.py
--rw-r--r--   0        0        0     6235 2023-02-06 09:52:28.247709 pht_station-0.2.0/station/app/api/api_v1/endpoints/docker_trains.py
--rw-r--r--   0        0        0     2075 2023-02-06 09:52:28.248714 pht_station-0.2.0/station/app/api/api_v1/endpoints/fhir.py
--rw-r--r--   0        0        0     5162 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/endpoints/local_trains.py
--rw-r--r--   0        0        0     2470 2023-02-06 09:52:28.250721 pht_station-0.2.0/station/app/api/api_v1/endpoints/master_images.py
--rw-r--r--   0        0        0     1808 2023-02-06 09:52:28.251708 pht_station-0.2.0/station/app/api/api_v1/endpoints/notifications.py
--rw-r--r--   0        0        0      587 2023-02-06 09:52:28.252711 pht_station-0.2.0/station/app/api/api_v1/endpoints/station.py
--rw-r--r--   0        0        0     2342 2023-02-06 09:52:28.253712 pht_station-0.2.0/station/app/api/api_v1/endpoints/station_status.py
--rw-r--r--   0        0        0      679 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/dependencies.py
--rw-r--r--   0        0        0     5122 2023-02-06 09:52:28.257709 pht_station-0.2.0/station/app/auth.py
--rw-r--r--   0        0        0     1747 2023-02-06 09:52:28.258710 pht_station-0.2.0/station/app/cache.py
--rw-r--r--   0        0        0     3739 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/clients.py
--rw-r--r--   0        0        0      277 2023-02-06 09:52:28.260830 pht_station-0.2.0/station/app/config.py
--rw-r--r--   0        0        0      298 2023-02-06 09:52:28.261841 pht_station-0.2.0/station/app/crud/__init__.py
--rw-r--r--   0        0        0     2533 2023-02-06 09:52:28.262840 pht_station-0.2.0/station/app/crud/base.py
--rw-r--r--   0        0        0     2479 2023-02-06 09:52:28.265857 pht_station-0.2.0/station/app/crud/crud_datasets.py
--rw-r--r--   0        0        0      675 2023-02-06 09:52:28.266866 pht_station-0.2.0/station/app/crud/crud_discovery.py
--rw-r--r--   0        0        0     8668 2023-02-06 09:52:28.267868 pht_station-0.2.0/station/app/crud/crud_docker_trains.py
--rw-r--r--   0        0        0     1773 2023-02-06 09:52:28.268868 pht_station-0.2.0/station/app/crud/crud_fhir_servers.py
--rw-r--r--   0        0        0     3648 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/crud/crud_local_train.py
--rw-r--r--   0        0        0      546 2023-02-06 09:52:28.271866 pht_station-0.2.0/station/app/crud/crud_notifications.py
--rw-r--r--   0        0        0     1997 2023-02-06 09:52:28.272866 pht_station-0.2.0/station/app/crud/crud_train_configs.py
--rw-r--r--   0        0        0     1503 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/crud/local_train_master_image.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.545965 pht_station-0.2.0/station/app/datasets/__init__.py
--rw-r--r--   0        0        0     1799 2023-02-06 09:52:28.274865 pht_station-0.2.0/station/app/datasets/filesystem.py
--rw-r--r--   0        0        0     7734 2023-02-06 09:52:28.275865 pht_station-0.2.0/station/app/datasets/statistics.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.224536 pht_station-0.2.0/station/app/db/__init__.py
--rw-r--r--   0        0        0      750 2023-02-06 14:20:00.310226 pht_station-0.2.0/station/app/db/base.py
--rw-r--r--   0        0        0      289 2022-08-01 10:19:24.230970 pht_station-0.2.0/station/app/db/base_class.py
--rw-r--r--   0        0        0      459 2023-02-06 09:52:28.277962 pht_station-0.2.0/station/app/db/session.py
--rw-r--r--   0        0        0     1345 2023-02-06 09:52:28.278872 pht_station-0.2.0/station/app/db/setup_db.py
--rw-r--r--   0        0        0     1459 2022-08-01 10:19:24.403753 pht_station-0.2.0/station/app/env.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.345748 pht_station-0.2.0/station/app/fhir/__init__.py
--rw-r--r--   0        0        0     2595 2023-02-06 09:52:28.280868 pht_station-0.2.0/station/app/fhir/server.py
--rw-r--r--   0        0        0     2895 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/logger.py
--rw-r--r--   0        0        0      933 2023-05-09 10:32:59.163014 pht_station-0.2.0/station/app/main.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.406771 pht_station-0.2.0/station/app/models/__init__.py
--rw-r--r--   0        0        0      784 2023-02-06 09:52:28.292149 pht_station-0.2.0/station/app/models/datasets.py
--rw-r--r--   0        0        0      345 2023-02-06 09:52:28.294158 pht_station-0.2.0/station/app/models/discovery.py
--rw-r--r--   0        0        0     2808 2023-02-06 14:16:52.531459 pht_station-0.2.0/station/app/models/docker_trains.py
--rw-r--r--   0        0        0      963 2023-02-06 09:52:28.296161 pht_station-0.2.0/station/app/models/fhir_server.py
--rw-r--r--   0        0        0     3225 2023-02-06 09:52:28.298158 pht_station-0.2.0/station/app/models/local_trains.py
--rw-r--r--   0        0        0      569 2023-02-06 09:52:28.298158 pht_station-0.2.0/station/app/models/notification.py
--rw-r--r--   0        0        0     1502 2023-05-24 10:01:24.524827 pht_station-0.2.0/station/app/run_station.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.493050 pht_station-0.2.0/station/app/schemas/__init__.py
--rw-r--r--   0        0        0     1114 2023-02-06 09:52:28.300235 pht_station-0.2.0/station/app/schemas/airflow.py
--rw-r--r--   0        0        0     2651 2023-02-06 09:52:28.302162 pht_station-0.2.0/station/app/schemas/datasets.py
--rw-r--r--   0        0        0     1038 2023-02-06 09:52:28.302162 pht_station-0.2.0/station/app/schemas/discovery.py
--rw-r--r--   0        0        0     1004 2023-02-06 09:52:28.304512 pht_station-0.2.0/station/app/schemas/dl_models.py
--rw-r--r--   0        0        0     2888 2023-02-06 09:52:28.305506 pht_station-0.2.0/station/app/schemas/docker_trains.py
--rw-r--r--   0        0        0     2194 2023-02-06 09:52:28.306505 pht_station-0.2.0/station/app/schemas/fhir.py
--rw-r--r--   0        0        0     3149 2023-02-06 09:52:28.308508 pht_station-0.2.0/station/app/schemas/local_trains.py
--rw-r--r--   0        0        0      708 2023-02-06 09:52:28.309506 pht_station-0.2.0/station/app/schemas/notifications.py
--rw-r--r--   0        0        0      425 2023-02-06 09:52:28.310505 pht_station-0.2.0/station/app/schemas/protocol.py
--rw-r--r--   0        0        0      448 2023-02-06 09:52:28.311507 pht_station-0.2.0/station/app/schemas/station.py
--rw-r--r--   0        0        0      781 2023-02-06 09:52:28.312514 pht_station-0.2.0/station/app/schemas/station_status.py
--rw-r--r--   0        0        0      966 2023-02-06 09:52:28.312514 pht_station-0.2.0/station/app/schemas/trains.py
--rw-r--r--   0        0        0     1094 2023-02-06 09:52:28.313524 pht_station-0.2.0/station/app/schemas/users.py
--rw-r--r--   0        0        0    43179 2023-05-24 10:01:24.525938 pht_station-0.2.0/station/app/settings.py
--rw-r--r--   0        0        0    12288 2023-05-24 10:01:24.525938 pht_station-0.2.0/station/app/test.db
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.354010 pht_station-0.2.0/station/app/tests/__init__.py
--rw-r--r--   0        0        0     4184 2023-02-06 09:52:28.321353 pht_station-0.2.0/station/app/tests/test_api_airflow.py
--rw-r--r--   0        0        0      933 2023-02-06 09:52:28.322369 pht_station-0.2.0/station/app/tests/test_api_datasets.py
--rw-r--r--   0        0        0    13153 2023-02-06 09:52:28.323363 pht_station-0.2.0/station/app/tests/test_api_docker_trains.py
--rw-r--r--   0        0        0     3132 2023-02-06 09:52:28.324368 pht_station-0.2.0/station/app/tests/test_api_fhir_servers.py
--rw-r--r--   0        0        0     1585 2023-02-06 09:52:28.325364 pht_station-0.2.0/station/app/tests/test_api_local_trains.py
--rw-r--r--   0        0        0     2539 2023-02-06 09:52:28.325364 pht_station-0.2.0/station/app/tests/test_api_notifications.py
--rw-r--r--   0        0        0     1177 2023-02-06 09:52:28.326365 pht_station-0.2.0/station/app/tests/test_auth.py
--rw-r--r--   0        0        0     1188 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/app/tests/test_central_client.py
--rw-r--r--   0        0        0      826 2023-02-06 09:52:28.328370 pht_station-0.2.0/station/app/tests/test_db.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.351668 pht_station-0.2.0/station/app/tests/test_files/entrypoint.py
--rw-r--r--   0        0        0     1340 2023-02-06 09:52:28.329431 pht_station-0.2.0/station/app/tests/test_local_trains.py
--rw-r--r--   0        0        0     7944 2023-02-06 09:52:28.330453 pht_station-0.2.0/station/app/tests/test_settings.py
--rw-r--r--   0        0        0      420 2023-02-06 09:52:28.331363 pht_station-0.2.0/station/app/tests/test_status.py
--rw-r--r--   0        0        0        0 2022-08-11 07:11:09.946932 pht_station-0.2.0/station/app/trains/__init__.py
--rw-r--r--   0        0        0        0 2022-08-11 07:11:09.947785 pht_station-0.2.0/station/app/trains/docker/__init__.py
--rw-r--r--   0        0        0     6584 2023-02-06 09:52:28.333493 pht_station-0.2.0/station/app/trains/docker/airflow.py
--rw-r--r--   0        0        0      822 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/app/trains/docker/update.py
--rw-r--r--   0        0        0        0 2022-08-11 07:11:09.949200 pht_station-0.2.0/station/app/trains/local/__init__.py
--rw-r--r--   0        0        0       49 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/__init__.py
--rw-r--r--   0        0        0       55 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/airflow/__init__.py
--rw-r--r--   0        0        0     5057 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/airflow/client.py
--rw-r--r--   0        0        0     6616 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/airflow/docker_trains.py
--rw-r--r--   0        0        0     2394 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/base.py
--rw-r--r--   0        0        0       45 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/central/__init__.py
--rw-r--r--   0        0        0     3293 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/central/central_client.py
--rw-r--r--   0        0        0      137 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/central/schemas.py
--rw-r--r--   0        0        0       45 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/conductor/__init__.py
--rw-r--r--   0        0        0     1436 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/conductor/rest_client.py
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/docker/__init__.py
--rw-r--r--   0        0        0     3740 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/docker/client.py
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/fhir/__init__.py
--rw-r--r--   0        0        0     5243 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/fhir/client.py
--rw-r--r--   0        0        0     3507 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/harbor_client.py
--rw-r--r--   0        0        0       32 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/minio/__init__.py
--rw-r--r--   0        0        0    11455 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/minio/client.py
--rw-r--r--   0        0        0     2712 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/resource_client.py
--rw-r--r--   0        0        0       37 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/station/__init__.py
--rw-r--r--   0        0        0     1355 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/station/client.py
--rw-r--r--   0        0        0     1584 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/station/local_trains.py
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/tests/__init__.py
--rw-r--r--   0        0        0      853 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/tests/test_central_client.py
--rw-r--r--   0        0        0     1631 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/tests/test_station_client.py
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/__init__.py
--rw-r--r--   0        0        0     2519 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/fix.py
--rw-r--r--   0        0        0     2406 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/generators.py
--rw-r--r--   0        0        0    13204 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/station_config.py
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/__init__.py
--rw-r--r--   0        0        0     1265 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/cert.pem
--rw-r--r--   0        0        0     1679 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/key.pem
--rw-r--r--   0        0        0     3505 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/test_station_config.py
--rw-r--r--   0        0        0     2518 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/test_station_config.yml
--rw-r--r--   0        0        0     3668 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/validators.py
--rw-r--r--   0        0        0     1721 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/common/constants.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.710500 pht_station-0.2.0/station/ctl/__init__.py
--rw-r--r--   0        0        0     1562 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/cli.py
--rw-r--r--   0        0        0      107 2023-02-06 09:52:28.355911 pht_station-0.2.0/station/ctl/config/__init__.py
--rw-r--r--   0        0        0     2542 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/config/command.py
--rw-r--r--   0        0        0    10104 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/config/fix.py
--rw-r--r--   0        0        0     1075 2023-02-06 09:52:28.363917 pht_station-0.2.0/station/ctl/config/fs.py
--rw-r--r--   0        0        0     1816 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/config/validate.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.615591 pht_station-0.2.0/station/ctl/fhir/__init__.py
--rw-r--r--   0        0        0      774 2023-02-06 09:52:28.368916 pht_station-0.2.0/station/ctl/fhir/command.py
--rw-r--r--   0        0        0     1572 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/fhir/manage.py
--rw-r--r--   0        0        0     2411 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/fhir/setup.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.677002 pht_station-0.2.0/station/ctl/install/__init__.py
--rw-r--r--   0        0        0     2853 2023-02-06 09:52:28.371914 pht_station-0.2.0/station/ctl/install/certs.py
--rw-r--r--   0        0        0    12998 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/install/command.py
--rw-r--r--   0        0        0     3013 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/install/docker.py
--rw-r--r--   0        0        0     1837 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/install/fs.py
--rw-r--r--   0        0        0    13076 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/install/templates.py
--rw-r--r--   0        0        0    38914 2022-11-16 14:46:10.023598 pht_station-0.2.0/station/ctl/templates/airflow.cfg.tmpl
--rw-r--r--   0        0        0      296 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/authup/authup.api.conf.tmpl
--rw-r--r--   0        0        0     3693 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/docker-compose.yml.tmpl
--rw-r--r--   0        0        0      257 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/init.sql.tmpl
--rw-r--r--   0        0        0     3288 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/station_config.yml.tmpl
--rw-r--r--   0        0        0      382 2022-08-01 10:19:24.690599 pht_station-0.2.0/station/ctl/templates/traefik/config.yml.tmpl
--rw-r--r--   0        0        0      628 2022-11-16 13:15:51.913906 pht_station-0.2.0/station/ctl/templates/traefik/traefik.yml.tmpl
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.618548 pht_station-0.2.0/station/ctl/tests/__init__.py
--rw-r--r--   0        0        0     3010 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/tests/test_config.py
--rw-r--r--   0        0        0     2707 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/tests/test_install.py
--rw-r--r--   0        0        0     2465 2023-02-06 09:52:28.382289 pht_station-0.2.0/station/ctl/tests/test_validators.py
--rw-r--r--   0        0        0      338 2023-02-06 09:52:28.383299 pht_station-0.2.0/station/ctl/util.py
--rw-r--r--   0        0        0        0 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/scripts/__init__.py
--rw-r--r--   0        0        0      440 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/scripts/run_dev.py
--rw-r--r--   0        0        0        0 2023-01-31 12:11:18.164891 pht_station-0.2.0/station/trains/__init__.py
--rw-r--r--   0        0        0        0 2023-01-31 12:11:18.169904 pht_station-0.2.0/station/trains/local/__init__.py
--rw-r--r--   0        0        0     2803 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/trains/local/airflow.py
--rw-r--r--   0        0        0     2357 2023-02-06 09:52:28.385301 pht_station-0.2.0/station/trains/local/build.py
--rw-r--r--   0        0        0     1637 2023-02-06 09:52:28.386299 pht_station-0.2.0/station/trains/local/docker.py
--rw-r--r--   0        0        0      922 2023-02-06 09:52:28.387302 pht_station-0.2.0/station/trains/local/update.py
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.764517 pht_station-0.2.0/station/worker/__init__.py
--rw-r--r--   0        0        0       46 2022-08-01 10:19:24.757813 pht_station-0.2.0/station/worker/discovery/__init__.py
--rw-r--r--   0        0        0      823 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/discovery/data_discovery.py
--rw-r--r--   0        0        0      109 2022-08-01 10:19:24.719800 pht_station-0.2.0/station/worker/loader/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/loader/base_loader.py
--rw-r--r--   0        0        0     4434 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/loader/dataset.py
--rw-r--r--   0        0        0     3797 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/loader/model_loader.py
--rw-r--r--   0        0        0     2387 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/pht_worker.py
--rw-r--r--   0        0        0       64 2022-08-01 10:19:24.771945 pht_station-0.2.0/station/worker/requirements.txt
--rw-r--r--   0        0        0        0 2022-08-01 10:19:24.730047 pht_station-0.2.0/station/worker/testing/__init__.py
--rw-r--r--   0        0        0      393 2023-02-06 09:52:28.392304 pht_station-0.2.0/station/worker/testing/db.py
--rw-r--r--   0        0        0     2304 2023-02-06 09:52:28.393306 pht_station-0.2.0/station/worker/testing/populate_minio.py
--rw-r--r--   0        0        0     1333 2023-02-06 09:52:28.393306 pht_station-0.2.0/station/worker/testing/train_lightning_model.py
--rw-r--r--   0        0        0       87 2022-08-01 10:19:24.738767 pht_station-0.2.0/station/worker/trainer/__init__.py
--rw-r--r--   0        0        0     2709 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/trainer/base_trainer.py
--rw-r--r--   0        0        0     7008 2023-02-06 09:52:28.396298 pht_station-0.2.0/station/worker/trainer/federated_trainer.py
--rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 pht_station-0.2.0/setup.py
--rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 pht_station-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2652 2023-03-27 21:08:40.678085 pht_station-0.2.1/README.md
+-rw-r--r--   0        0        0     1929 2023-06-13 09:54:50.703087 pht_station-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/.dockerignore
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/__init__.py
+-rwxr-xr-x   0        0        0     1150 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/api/api_v1/api.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     3612 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/api/api_v1/endpoints/airflow.py
+-rwxr-xr-x   0        0        0     7514 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/api/api_v1/endpoints/datasets.py
+-rwxr-xr-x   0        0        0     6235 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/endpoints/docker_trains.py
+-rw-r--r--   0        0        0     2075 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/endpoints/fhir.py
+-rwxr-xr-x   0        0        0     5162 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/api/api_v1/endpoints/local_trains.py
+-rw-r--r--   0        0        0     2470 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/endpoints/master_images.py
+-rw-r--r--   0        0        0     1808 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/endpoints/notifications.py
+-rwxr-xr-x   0        0        0      587 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/endpoints/station.py
+-rwxr-xr-x   0        0        0     2342 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/api/api_v1/endpoints/station_status.py
+-rwxr-xr-x   0        0        0      679 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/api/dependencies.py
+-rwxr-xr-x   0        0        0     5122 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/auth.py
+-rw-r--r--   0        0        0     1747 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/cache.py
+-rw-r--r--   0        0        0     3739 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/clients.py
+-rw-r--r--   0        0        0      277 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/config.py
+-rwxr-xr-x   0        0        0      298 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/__init__.py
+-rwxr-xr-x   0        0        0     2533 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/base.py
+-rwxr-xr-x   0        0        0     2479 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/crud_datasets.py
+-rw-r--r--   0        0        0      675 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/crud_discovery.py
+-rwxr-xr-x   0        0        0     8668 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/crud_docker_trains.py
+-rw-r--r--   0        0        0     1773 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/crud_fhir_servers.py
+-rw-r--r--   0        0        0     3648 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/crud/crud_local_train.py
+-rwxr-xr-x   0        0        0      546 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/crud_notifications.py
+-rwxr-xr-x   0        0        0     1997 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/crud/crud_train_configs.py
+-rw-r--r--   0        0        0     1503 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/crud/local_train_master_image.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/datasets/__init__.py
+-rw-r--r--   0        0        0     1799 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/datasets/filesystem.py
+-rw-r--r--   0        0        0     7734 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/datasets/statistics.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/db/__init__.py
+-rwxr-xr-x   0        0        0      750 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/db/base.py
+-rwxr-xr-x   0        0        0      289 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/db/base_class.py
+-rwxr-xr-x   0        0        0      459 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/db/session.py
+-rwxr-xr-x   0        0        0     1345 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/db/setup_db.py
+-rw-r--r--   0        0        0     1459 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/env.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/fhir/__init__.py
+-rw-r--r--   0        0        0     2595 2023-03-27 21:08:40.678085 pht_station-0.2.1/station/app/fhir/server.py
+-rw-r--r--   0        0        0     2895 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/logger.py
+-rwxr-xr-x   0        0        0      933 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/main.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/models/__init__.py
+-rwxr-xr-x   0        0        0      784 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/models/datasets.py
+-rw-r--r--   0        0        0      345 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/models/discovery.py
+-rwxr-xr-x   0        0        0     2808 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/models/docker_trains.py
+-rw-r--r--   0        0        0      963 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/models/fhir_server.py
+-rw-r--r--   0        0        0     3225 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/models/local_trains.py
+-rwxr-xr-x   0        0        0      569 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/models/notification.py
+-rw-r--r--   0        0        0     1502 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/run_station.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/__init__.py
+-rw-r--r--   0        0        0     1114 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/airflow.py
+-rwxr-xr-x   0        0        0     2651 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/datasets.py
+-rw-r--r--   0        0        0     1038 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/discovery.py
+-rwxr-xr-x   0        0        0     1004 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/dl_models.py
+-rwxr-xr-x   0        0        0     2888 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/docker_trains.py
+-rw-r--r--   0        0        0     2194 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/fhir.py
+-rwxr-xr-x   0        0        0     3149 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/local_trains.py
+-rwxr-xr-x   0        0        0      708 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/notifications.py
+-rwxr-xr-x   0        0        0      425 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/protocol.py
+-rwxr-xr-x   0        0        0      448 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/station.py
+-rwxr-xr-x   0        0        0      781 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/station_status.py
+-rwxr-xr-x   0        0        0      966 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/trains.py
+-rw-r--r--   0        0        0     1094 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/schemas/users.py
+-rw-r--r--   0        0        0    43179 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/settings.py
+-rw-r--r--   0        0        0    12288 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/test.db
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/__init__.py
+-rw-r--r--   0        0        0     4184 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_api_airflow.py
+-rw-r--r--   0        0        0      933 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_api_datasets.py
+-rw-r--r--   0        0        0    13153 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_api_docker_trains.py
+-rw-r--r--   0        0        0     3132 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_api_fhir_servers.py
+-rw-r--r--   0        0        0     1585 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_api_local_trains.py
+-rw-r--r--   0        0        0     2539 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_api_notifications.py
+-rw-r--r--   0        0        0     1177 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_auth.py
+-rw-r--r--   0        0        0     1188 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/tests/test_central_client.py
+-rw-r--r--   0        0        0      826 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_db.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_files/entrypoint.py
+-rw-r--r--   0        0        0     1340 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_local_trains.py
+-rw-r--r--   0        0        0     7944 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_settings.py
+-rw-r--r--   0        0        0      420 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/tests/test_status.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/trains/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/trains/docker/__init__.py
+-rw-r--r--   0        0        0     6584 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/trains/docker/airflow.py
+-rw-r--r--   0        0        0      822 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/app/trains/docker/update.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/app/trains/local/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/__init__.py
+-rwxr-xr-x   0        0        0       55 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/airflow/__init__.py
+-rwxr-xr-x   0        0        0     5057 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/airflow/client.py
+-rwxr-xr-x   0        0        0     6616 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/airflow/docker_trains.py
+-rw-r--r--   0        0        0     2394 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/base.py
+-rw-r--r--   0        0        0       45 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/central/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/central/central_client.py
+-rw-r--r--   0        0        0      137 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/central/schemas.py
+-rwxr-xr-x   0        0        0       45 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/conductor/__init__.py
+-rwxr-xr-x   0        0        0     1436 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/conductor/rest_client.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/docker/__init__.py
+-rwxr-xr-x   0        0        0     3740 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/docker/client.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/fhir/__init__.py
+-rwxr-xr-x   0        0        0     5243 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/fhir/client.py
+-rwxr-xr-x   0        0        0     3507 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/harbor_client.py
+-rwxr-xr-x   0        0        0       32 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/minio/__init__.py
+-rwxr-xr-x   0        0        0    11455 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/minio/client.py
+-rw-r--r--   0        0        0     2712 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/resource_client.py
+-rw-r--r--   0        0        0       37 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/station/__init__.py
+-rw-r--r--   0        0        0     1355 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/station/client.py
+-rw-r--r--   0        0        0     1584 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/station/local_trains.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/tests/__init__.py
+-rw-r--r--   0        0        0      853 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/tests/test_central_client.py
+-rw-r--r--   0        0        0     1631 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/clients/tests/test_station_client.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/__init__.py
+-rw-r--r--   0        0        0     2519 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/fix.py
+-rw-r--r--   0        0        0     2406 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/generators.py
+-rw-r--r--   0        0        0    13204 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/station_config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/tests/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/tests/cert.pem
+-rw-r--r--   0        0        0     1679 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/tests/key.pem
+-rw-r--r--   0        0        0     3505 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/tests/test_station_config.py
+-rw-r--r--   0        0        0     2518 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/tests/test_station_config.yml
+-rw-r--r--   0        0        0     3668 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/config/validators.py
+-rw-r--r--   0        0        0     1721 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/common/constants.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/ctl/__init__.py
+-rw-r--r--   0        0        0     1562 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/cli.py
+-rw-r--r--   0        0        0      107 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/ctl/config/__init__.py
+-rw-r--r--   0        0        0     2542 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/config/command.py
+-rw-r--r--   0        0        0    10104 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/config/fix.py
+-rw-r--r--   0        0        0     1075 2023-03-27 21:08:40.688085 pht_station-0.2.1/station/ctl/config/fs.py
+-rw-r--r--   0        0        0     1816 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/config/validate.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/fhir/__init__.py
+-rw-r--r--   0        0        0      774 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/fhir/command.py
+-rw-r--r--   0        0        0     1572 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/fhir/manage.py
+-rw-r--r--   0        0        0     2411 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/fhir/setup.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/install/__init__.py
+-rw-r--r--   0        0        0     2853 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/install/certs.py
+-rw-r--r--   0        0        0    13052 2023-06-13 06:27:05.571181 pht_station-0.2.1/station/ctl/install/command.py
+-rw-r--r--   0        0        0     3013 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/install/docker.py
+-rw-r--r--   0        0        0     1837 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/install/fs.py
+-rw-r--r--   0        0        0    13076 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/install/templates.py
+-rw-r--r--   0        0        0    38914 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/templates/airflow.cfg.tmpl
+-rw-r--r--   0        0        0      296 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/templates/authup/authup.api.conf.tmpl
+-rw-r--r--   0        0        0     3693 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/templates/docker-compose.yml.tmpl
+-rw-r--r--   0        0        0      257 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/templates/init.sql.tmpl
+-rw-r--r--   0        0        0     3288 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/templates/station_config.yml.tmpl
+-rw-r--r--   0        0        0      382 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/templates/traefik/config.yml.tmpl
+-rw-r--r--   0        0        0      628 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/templates/traefik/traefik.yml.tmpl
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/tests/__init__.py
+-rw-r--r--   0        0        0     3010 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/tests/test_config.py
+-rw-r--r--   0        0        0     2707 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/ctl/tests/test_install.py
+-rw-r--r--   0        0        0     2465 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/tests/test_validators.py
+-rw-r--r--   0        0        0      338 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/ctl/util.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/scripts/__init__.py
+-rw-r--r--   0        0        0      440 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/scripts/run_dev.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/trains/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/trains/local/__init__.py
+-rw-r--r--   0        0        0     2803 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/trains/local/airflow.py
+-rw-r--r--   0        0        0     2357 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/trains/local/build.py
+-rw-r--r--   0        0        0     1637 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/trains/local/docker.py
+-rw-r--r--   0        0        0      922 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/trains/local/update.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/discovery/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/worker/discovery/data_discovery.py
+-rw-r--r--   0        0        0      109 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/loader/__init__.py
+-rw-r--r--   0        0        0     2019 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/worker/loader/base_loader.py
+-rw-r--r--   0        0        0     4434 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/worker/loader/dataset.py
+-rw-r--r--   0        0        0     3797 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/worker/loader/model_loader.py
+-rw-r--r--   0        0        0     2387 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/worker/pht_worker.py
+-rw-r--r--   0        0        0       64 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/testing/__init__.py
+-rw-r--r--   0        0        0      393 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/testing/db.py
+-rw-r--r--   0        0        0     2304 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/testing/populate_minio.py
+-rw-r--r--   0        0        0     1333 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/testing/train_lightning_model.py
+-rw-r--r--   0        0        0       87 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/trainer/__init__.py
+-rw-r--r--   0        0        0     2709 2023-06-13 06:25:35.067726 pht_station-0.2.1/station/worker/trainer/base_trainer.py
+-rw-r--r--   0        0        0     7008 2023-03-27 21:08:40.698085 pht_station-0.2.1/station/worker/trainer/federated_trainer.py
+-rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 pht_station-0.2.1/PKG-INFO
```

### Comparing `pht_station-0.2.0/pyproject.toml` & `pht_station-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pht-station"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python library for handling containerized PHT trains"
 authors = ["Michael Graf <michael.graf@uni-tuebingen.com>"]
 readme = "README.md"
 packages = [{ include = "station" }]
 include = [
     "station/ctl/templates/*.tmpl",
     "station/ctl/templates/traefik/*.tmpl",
@@ -33,15 +33,15 @@
 SQLAlchemy = "*"
 psutil = "*"
 loguru = "*"
 jinja2 = "*"
 click = "*"
 rich = "*"
 plotly = "*"
-s3fs = "*"
+# s3fs = "*"
 python-multipart = "*"
 redis = "*"
 authup = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
 pytest = "*"
```

### Comparing `pht_station-0.2.0/README.md` & `pht_station-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/api.py` & `pht_station-0.2.1/station/app/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/airflow.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/airflow.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/datasets.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/datasets.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/docker_trains.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/docker_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/fhir.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/fhir.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/local_trains.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/local_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/master_images.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/master_images.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/notifications.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/notifications.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/station.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/station.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/api_v1/endpoints/station_status.py` & `pht_station-0.2.1/station/app/api/api_v1/endpoints/station_status.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/api/dependencies.py` & `pht_station-0.2.1/station/app/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/auth.py` & `pht_station-0.2.1/station/app/auth.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/cache.py` & `pht_station-0.2.1/station/app/cache.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/clients.py` & `pht_station-0.2.1/station/app/clients.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/base.py` & `pht_station-0.2.1/station/app/crud/base.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/crud_datasets.py` & `pht_station-0.2.1/station/app/crud/crud_datasets.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/crud_discovery.py` & `pht_station-0.2.1/station/app/crud/crud_discovery.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/crud_docker_trains.py` & `pht_station-0.2.1/station/app/crud/crud_docker_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/crud_fhir_servers.py` & `pht_station-0.2.1/station/app/crud/crud_fhir_servers.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/crud_local_train.py` & `pht_station-0.2.1/station/app/crud/crud_local_train.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/crud_notifications.py` & `pht_station-0.2.1/station/app/crud/crud_notifications.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/crud_train_configs.py` & `pht_station-0.2.1/station/app/crud/crud_train_configs.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/crud/local_train_master_image.py` & `pht_station-0.2.1/station/app/crud/local_train_master_image.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/datasets/filesystem.py` & `pht_station-0.2.1/station/app/datasets/filesystem.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/datasets/statistics.py` & `pht_station-0.2.1/station/app/datasets/statistics.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/db/base.py` & `pht_station-0.2.1/station/app/db/base.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/db/setup_db.py` & `pht_station-0.2.1/station/app/db/setup_db.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/env.py` & `pht_station-0.2.1/station/app/env.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/fhir/server.py` & `pht_station-0.2.1/station/app/fhir/server.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/logger.py` & `pht_station-0.2.1/station/app/logger.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/main.py` & `pht_station-0.2.1/station/app/main.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/models/datasets.py` & `pht_station-0.2.1/station/app/models/datasets.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/models/docker_trains.py` & `pht_station-0.2.1/station/app/models/docker_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/models/fhir_server.py` & `pht_station-0.2.1/station/app/models/fhir_server.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/models/local_trains.py` & `pht_station-0.2.1/station/app/models/local_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/models/notification.py` & `pht_station-0.2.1/station/app/models/notification.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/run_station.py` & `pht_station-0.2.1/station/app/run_station.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/airflow.py` & `pht_station-0.2.1/station/app/schemas/airflow.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/datasets.py` & `pht_station-0.2.1/station/app/schemas/datasets.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/discovery.py` & `pht_station-0.2.1/station/app/schemas/discovery.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/dl_models.py` & `pht_station-0.2.1/station/app/schemas/dl_models.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/docker_trains.py` & `pht_station-0.2.1/station/app/schemas/docker_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/fhir.py` & `pht_station-0.2.1/station/app/schemas/fhir.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/local_trains.py` & `pht_station-0.2.1/station/app/schemas/local_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/notifications.py` & `pht_station-0.2.1/station/app/schemas/notifications.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/station_status.py` & `pht_station-0.2.1/station/app/schemas/station_status.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/trains.py` & `pht_station-0.2.1/station/app/schemas/trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/schemas/users.py` & `pht_station-0.2.1/station/app/schemas/users.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/settings.py` & `pht_station-0.2.1/station/app/settings.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/test.db` & `pht_station-0.2.1/station/app/test.db`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_api_airflow.py` & `pht_station-0.2.1/station/app/tests/test_api_airflow.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_api_datasets.py` & `pht_station-0.2.1/station/app/tests/test_api_datasets.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_api_docker_trains.py` & `pht_station-0.2.1/station/app/tests/test_api_docker_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_api_fhir_servers.py` & `pht_station-0.2.1/station/app/tests/test_api_fhir_servers.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_api_local_trains.py` & `pht_station-0.2.1/station/app/tests/test_api_local_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_api_notifications.py` & `pht_station-0.2.1/station/app/tests/test_api_notifications.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_auth.py` & `pht_station-0.2.1/station/app/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_central_client.py` & `pht_station-0.2.1/station/app/tests/test_central_client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_db.py` & `pht_station-0.2.1/station/app/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_local_trains.py` & `pht_station-0.2.1/station/app/tests/test_local_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/tests/test_settings.py` & `pht_station-0.2.1/station/app/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/trains/docker/airflow.py` & `pht_station-0.2.1/station/app/trains/docker/airflow.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/app/trains/docker/update.py` & `pht_station-0.2.1/station/app/trains/docker/update.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/airflow/client.py` & `pht_station-0.2.1/station/common/clients/airflow/client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/airflow/docker_trains.py` & `pht_station-0.2.1/station/common/clients/airflow/docker_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/base.py` & `pht_station-0.2.1/station/common/clients/base.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/central/central_client.py` & `pht_station-0.2.1/station/common/clients/central/central_client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/conductor/rest_client.py` & `pht_station-0.2.1/station/common/clients/conductor/rest_client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/docker/client.py` & `pht_station-0.2.1/station/common/clients/docker/client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/fhir/client.py` & `pht_station-0.2.1/station/common/clients/fhir/client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/harbor_client.py` & `pht_station-0.2.1/station/common/clients/harbor_client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/minio/client.py` & `pht_station-0.2.1/station/common/clients/minio/client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/resource_client.py` & `pht_station-0.2.1/station/common/clients/resource_client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/station/client.py` & `pht_station-0.2.1/station/common/clients/station/client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/station/local_trains.py` & `pht_station-0.2.1/station/common/clients/station/local_trains.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/tests/test_central_client.py` & `pht_station-0.2.1/station/common/clients/tests/test_central_client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/clients/tests/test_station_client.py` & `pht_station-0.2.1/station/common/clients/tests/test_station_client.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/fix.py` & `pht_station-0.2.1/station/common/config/fix.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/generators.py` & `pht_station-0.2.1/station/common/config/generators.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/station_config.py` & `pht_station-0.2.1/station/common/config/station_config.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/tests/cert.pem` & `pht_station-0.2.1/station/common/config/tests/cert.pem`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/tests/key.pem` & `pht_station-0.2.1/station/common/config/tests/key.pem`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/tests/test_station_config.py` & `pht_station-0.2.1/station/common/config/tests/test_station_config.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/tests/test_station_config.yml` & `pht_station-0.2.1/station/common/config/tests/test_station_config.yml`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/config/validators.py` & `pht_station-0.2.1/station/common/config/validators.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/common/constants.py` & `pht_station-0.2.1/station/common/constants.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/cli.py` & `pht_station-0.2.1/station/ctl/cli.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/config/command.py` & `pht_station-0.2.1/station/ctl/config/command.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/config/fix.py` & `pht_station-0.2.1/station/ctl/config/fix.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/config/fs.py` & `pht_station-0.2.1/station/ctl/config/fs.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/config/validate.py` & `pht_station-0.2.1/station/ctl/config/validate.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/fhir/command.py` & `pht_station-0.2.1/station/ctl/fhir/command.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/fhir/manage.py` & `pht_station-0.2.1/station/ctl/fhir/manage.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/fhir/setup.py` & `pht_station-0.2.1/station/ctl/fhir/setup.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/install/certs.py` & `pht_station-0.2.1/station/ctl/install/certs.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/install/command.py` & `pht_station-0.2.1/station/ctl/install/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,23 @@
 
     if result is not None:
         table, issues = result
         click.echo(Icons.CROSS.value)
         console = Console()
         console.print(table)
 
-        if ctx.obj["environment"] == "production":
+        if ctx.obj["station_config"]["environment"] == "production":
             click.confirm(
                 "Station configuration is invalid. Please fix the errors displayed above. \n"
                 "Would you like to fix the configuration now?",
                 abort=True,
             )
             fixed_config = fix_config(ctx.obj, ctx.obj["station_config"], issues)
             # merge config with fixed config
-            ctx.obj = ctx.obj | fixed_config
+            ctx.obj["station_config"] = ctx.obj["station_config"] | fixed_config
             render_config(ctx.obj["station_config"], ctx.obj["config_path"])
 
         else:
             res = click.prompt(
                 "Station configuration is invalid. Press enter to fix the configuration now. "
                 "[dev mode detected enter (skip) to continue]",
                 default="y",
```

### Comparing `pht_station-0.2.0/station/ctl/install/docker.py` & `pht_station-0.2.1/station/ctl/install/docker.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/install/fs.py` & `pht_station-0.2.1/station/ctl/install/fs.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/install/templates.py` & `pht_station-0.2.1/station/ctl/install/templates.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/templates/airflow.cfg.tmpl` & `pht_station-0.2.1/station/ctl/templates/airflow.cfg.tmpl`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/templates/docker-compose.yml.tmpl` & `pht_station-0.2.1/station/ctl/templates/docker-compose.yml.tmpl`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/templates/station_config.yml.tmpl` & `pht_station-0.2.1/station/ctl/templates/station_config.yml.tmpl`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/templates/traefik/traefik.yml.tmpl` & `pht_station-0.2.1/station/ctl/templates/traefik/traefik.yml.tmpl`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/tests/test_config.py` & `pht_station-0.2.1/station/ctl/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/tests/test_install.py` & `pht_station-0.2.1/station/ctl/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/ctl/tests/test_validators.py` & `pht_station-0.2.1/station/ctl/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/trains/local/airflow.py` & `pht_station-0.2.1/station/trains/local/airflow.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/trains/local/build.py` & `pht_station-0.2.1/station/trains/local/build.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/trains/local/docker.py` & `pht_station-0.2.1/station/trains/local/docker.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/trains/local/update.py` & `pht_station-0.2.1/station/trains/local/update.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/discovery/data_discovery.py` & `pht_station-0.2.1/station/worker/discovery/data_discovery.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/loader/base_loader.py` & `pht_station-0.2.1/station/worker/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/loader/dataset.py` & `pht_station-0.2.1/station/worker/loader/dataset.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/loader/model_loader.py` & `pht_station-0.2.1/station/worker/loader/model_loader.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/pht_worker.py` & `pht_station-0.2.1/station/worker/pht_worker.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/testing/populate_minio.py` & `pht_station-0.2.1/station/worker/testing/populate_minio.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/testing/train_lightning_model.py` & `pht_station-0.2.1/station/worker/testing/train_lightning_model.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/trainer/base_trainer.py` & `pht_station-0.2.1/station/worker/trainer/base_trainer.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/station/worker/trainer/federated_trainer.py` & `pht_station-0.2.1/station/worker/trainer/federated_trainer.py`

 * *Files identical despite different names*

### Comparing `pht_station-0.2.0/PKG-INFO` & `pht_station-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pht-station
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library for handling containerized PHT trains
 Author: Michael Graf
 Author-email: michael.graf@uni-tuebingen.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,15 +26,14 @@
 Requires-Dist: psycopg2-binary
 Requires-Dist: pycryptodome
 Requires-Dist: python-keycloak
 Requires-Dist: python-multipart
 Requires-Dist: redis
 Requires-Dist: requests
 Requires-Dist: rich
-Requires-Dist: s3fs
 Description-Content-Type: text/markdown
 
 [![Build](https://github.com/PHT-EU/station-backend/actions/workflows/Build.yml/badge.svg)](https://github.com/PHT-EU/station-backend/actions/workflows/Build.yml)
 [![Tests](https://github.com/PHT-EU/station-backend/actions/workflows/tests.yml/badge.svg)](https://github.com/PHT-EU/station-backend/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/PHT-Medic/station-backend/branch/master/graph/badge.svg?token=SWJRH1V44S)](https://codecov.io/gh/PHT-Medic/station-backend)
 
 # PHT Station Backend
```

