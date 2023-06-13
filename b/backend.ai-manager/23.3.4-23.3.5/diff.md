# Comparing `tmp/backend.ai-manager-23.3.4.tar.gz` & `tmp/backend.ai-manager-23.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-23.3.4.tar", last modified: Mon May 29 10:42:40 2023, max compression
+gzip compressed data, was "backend.ai-manager-23.3.5.tar", last modified: Tue Jun 13 03:42:12 2023, max compression
```

## Comparing `backend.ai-manager-23.3.4.tar` & `backend.ai-manager-23.3.5.tar`

### file list

```diff
@@ -1,244 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.703138 backend.ai-manager-23.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-29 10:42:40.703138 backend.ai-manager-23.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.675137 backend.ai-manager-23.3.4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.675137 backend.ai-manager-23.3.4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.679138 backend.ai-manager-23.3.4/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.683138 backend.ai-manager-23.3.4/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40846 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)   112592 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   117914 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.683138 backend.ai-manager-23.3.4/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    25764 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.683138 backend.ai-manager-23.3.4/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39619 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.687138 backend.ai-manager-23.3.4/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.687138 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.699138 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48343 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31774 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    51030 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.699138 backend.ai-manager-23.3.4/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    54702 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    42526 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.699138 backend.ai-manager-23.3.4/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   116503 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.703138 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52978 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/ai/backend/manager/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:40.703138 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:40.703138 backend.ai-manager-23.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-29 10:42:40.000000 backend.ai-manager-23.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.216278 backend.ai-manager-23.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-13 03:42:12.216278 backend.ai-manager-23.3.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.172279 backend.ai-manager-23.3.5/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.172279 backend.ai-manager-23.3.5/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.176278 backend.ai-manager-23.3.5/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.180279 backend.ai-manager-23.3.5/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40846 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76748 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119753 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.184279 backend.ai-manager-23.3.5/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.184279 backend.ai-manager-23.3.5/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39934 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.188279 backend.ai-manager-23.3.5/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.188279 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.212278 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33946 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49801 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51191 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.212278 backend.ai-manager-23.3.5/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42526 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46387 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.216278 backend.ai-manager-23.3.5/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   159742 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.216278 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61786 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30008 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/ai/backend/manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.216278 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-13 03:42:12.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-06-13 03:42:12.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 03:42:12.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 03:42:12.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:12.000000 backend.ai-manager-23.3.5/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:12.216278 backend.ai-manager-23.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-06-13 03:42:11.000000 backend.ai-manager-23.3.5/setup.py
```

### Comparing `backend.ai-manager-23.3.4/PKG-INFO` & `backend.ai-manager-23.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/acl.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/admin.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/auth.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/cluster_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/context.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/etcd.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/events.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/image.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/logs.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/manager.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/resource.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/service.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/service.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-import asyncio
 import logging
-import secrets
+import re
 import uuid
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Iterable, MutableMapping, Tuple, Union
+from typing import TYPE_CHECKING, Any, Iterable, Tuple
 
+import aiohttp
 import aiohttp_cors
 import aiotools
 import attrs
 import sqlalchemy as sa
 import trafaret as t
 from aiohttp import web
-from dateutil.parser import isoparse
-from dateutil.tz import tzutc
+from sqlalchemy.ext.asyncio import AsyncSession
+from sqlalchemy.orm import selectinload
+from sqlalchemy.orm.exc import NoResultFound
 
 from ai.backend.common import validators as tx
 from ai.backend.common.docker import ImageRef
-from ai.backend.common.exception import AliasResolutionFailed, UnknownImageReference
+from ai.backend.common.events import KernelLifecycleEventReason
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import ClusterMode, SessionTypes
-from ai.backend.common.utils import str_to_timedelta
+from ai.backend.common.types import ClusterMode, SessionTypes, VFolderUsageMode
+from ai.backend.manager.registry import check_scaling_group
 
-from ..defs import DEFAULT_IMAGE_ARCH, DEFAULT_ROLE
+from ..defs import DEFAULT_IMAGE_ARCH
 from ..models import (
     ImageRow,
-    UserRole,
-    domains,
-    query_bootstrap_script,
-    verify_vfolder_name,
+    UserRow,
+    query_accessible_vfolders,
+    resolve_group_name_or_id,
+    scaling_groups,
     vfolders,
 )
 from ..models.endpoint import EndpointRow
-from ..models.routing import RoutingRow
-from ..models.session import SessionRow, SessionStatus
-from ..models.utils import execute_with_retry
+from ..models.routing import RouteStatus, RoutingRow
 from ..types import UserScope
 from .auth import auth_required
 from .exceptions import (
-    BackendError,
-    ImageNotFound,
-    InsufficientPrivilege,
-    InternalServerError,
     InvalidAPIParameters,
-    UnknownImageReferenceError,
+    ObjectNotFound,
+    ServiceUnavailable,
+    VFolderNotFound,
 )
 from .manager import ALL_ALLOWED, READ_ALLOWED, server_status_required
 from .session import query_userinfo
 from .types import CORSOptions, WebMiddleware
-from .utils import check_api_params, get_access_key_scopes, undefined
+from .utils import check_api_params, get_access_key_scopes, get_user_uuid_scopes, undefined
 
 if TYPE_CHECKING:
     from .context import RootContext
 
 log = BraceStyleAdapter(logging.getLogger(__name__))
 
 
@@ -60,468 +57,528 @@
         if value == undefined:
             return value
         else:
             self._failure("Invalid Undef format", value=value)
             return None
 
 
+async def is_user_allowed_to_access_resource(
+    db_sess: AsyncSession,
+    request: web.Request,
+    resource_owner: uuid.UUID,
+) -> bool:
+    if request["user"]["is_superadmin"]:
+        return True
+    elif request["user"]["is_admin"]:
+        query = sa.select(UserRow).filter(UserRow.uuid == resource_owner)
+        result = await db_sess.execute(query)
+        user = result.scalar()
+        return user.domain_name == request["user"]["domain_name"]
+    else:
+        return request["user"]["uyud"] == resource_owner
+
+
 @auth_required
 @server_status_required(READ_ALLOWED)
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["project_id", "projectId"]): tx.UUID,
+            t.Key("name", default=None): t.Null | t.String,
         }
-    ),
+    )
 )
 async def list_serve(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
-    project_id = params["project_id"]
 
     log.info("SERVE.LIST (email:{}, ak:{})", request["user"]["email"], access_key)
+    query_conds = EndpointRow.session_owner == request["user"]["uuid"]
+    if params["name"]:
+        query_conds &= EndpointRow.name == params["name"]
 
     async with root_ctx.db.begin_readonly_session() as db_sess:
-        j = sa.join(SessionRow, RoutingRow, SessionRow.id == RoutingRow.session).join(
-            EndpointRow, RoutingRow.endpoint == EndpointRow.id
-        )
         query = (
-            sa.select(
-                SessionRow.id,
-                SessionRow.name,
-                SessionRow.status,
-            )
-            .select_from(j)
-            .where(SessionRow.group_id == project_id)
+            sa.select(EndpointRow).where(query_conds).options(selectinload(EndpointRow.routings))
         )
         result = await db_sess.execute(query)
         rows = result.scalars().all()
 
-    return web.json_response(rows, status=200)
+    return web.json_response(
+        [
+            {
+                "id": str(endpoint.id),
+                "name": endpoint.name,
+                "desired_session_count": endpoint.desired_session_count,
+                "active_route_count": len(
+                    [r for r in endpoint.routings if r.status == RouteStatus.HEALTHY]
+                ),
+                "service_endpoint": endpoint.url,
+                "is_public": endpoint.open_to_public,
+            }
+            for endpoint in rows
+        ],
+        status=200,
+    )
 
 
 @auth_required
 @server_status_required(READ_ALLOWED)
-@check_api_params(
-    t.Dict(
-        {
-            tx.AliasedKey(["endpoint_id", "endpointId"]): tx.UUID,
-        }
-    ),
-)
-async def get_info(request: web.Request, params: Any) -> web.Response:
+async def get_info(request: web.Request) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
+    service_id = uuid.UUID(request.match_info["service_id"])
 
-    log.info("SERVE.GET_INFO (email:{}, ak:{})", request["user"]["email"], access_key)
+    log.info(
+        "SERVE.GET_INFO (email:{}, ak:{}, s:{})", request["user"]["email"], access_key, service_id
+    )
 
     async with root_ctx.db.begin_readonly_session() as db_sess:
-        j = sa.join(SessionRow, RoutingRow, SessionRow.id == RoutingRow.session).join(
-            EndpointRow, RoutingRow.endpoint == EndpointRow.id
-        )
-        query = (
-            sa.select(
-                SessionRow.id,
-                SessionRow.name,
-                SessionRow.status,
-                EndpointRow.image,
-                EndpointRow.model,
-                EndpointRow.url,
-            )
-            .select_from(j)
-            .where(RoutingRow.endpoint == params["endpoint_id"])
-        )
-        result = await db_sess.execute(query)
-        rows = result.scalars().all()
+        try:
+            endpoint = await EndpointRow.get(db_sess, service_id, load_routes=True)
+        except NoResultFound:
+            raise ObjectNotFound
+
+    await get_user_uuid_scopes(request, {"owner_uuid": endpoint.session_owner})
+    resp = {
+        "endpoint_id": str(endpoint.id),
+        "name": endpoint.name,
+        "desired_session_count": endpoint.desired_session_count,
+        "active_routes": [
+            {
+                "route_id": str(r.id),
+                "session_id": str(r.session),
+                "traffic_ratio": r.traffic_ratio,
+            }
+            for r in endpoint.routings
+            if r.status == RouteStatus.HEALTHY
+        ],
+        "service_endpoint": endpoint.url,
+        "is_public": endpoint.open_to_public,
+    }
 
-    return web.json_response(rows, status=200)
+    return web.json_response(resp, status=200)
 
 
 @auth_required
 @server_status_required(ALL_ALLOWED)
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["endpoint_id", "endpointId"], default=None): tx.UUID | t.Null,
-            tx.AliasedKey(["service_name", "serviceName"]): t.String,
-            tx.AliasedKey(["model_id", "modelId"]): tx.UUID,
-            tx.AliasedKey(["model_version", "modelVersion"]): t.String,
-            tx.AliasedKey(["image_ref", "imageRef"]): t.String,
+            tx.AliasedKey(["name", "clientSessionToken"])
+            >> "service_name": t.Regexp(r"^(?=.{4,64}$)\w[\w.-]*\w$", re.ASCII),
+            tx.AliasedKey(["desired_session_count", "desiredSessionCount"]): t.Int,
+            tx.AliasedKey(["image", "lang"]): t.String,
             tx.AliasedKey(["arch", "architecture"], default=DEFAULT_IMAGE_ARCH)
             >> "architecture": t.String,
-            tx.AliasedKey(
-                ["group", "groupName", "group_name", "project", "project_name", "projectName"],
-                default="default",
-            ): t.String,
+            tx.AliasedKey(["group", "groupName", "group_name"], default="default"): t.String,
             tx.AliasedKey(["domain", "domainName", "domain_name"], default="default"): t.String,
-            tx.AliasedKey(["resource_opts", "resourceOpts"], default=dict): t.Mapping(
-                t.String, t.Any
-            ),
-            tx.AliasedKey(["cluster_size", "clusterSize"], default=1): t.ToInt[1:],
+            tx.AliasedKey(["cluster_size", "clusterSize"], default=1): t.ToInt[1:],  # new in APIv6
             tx.AliasedKey(["cluster_mode", "clusterMode"], default="single-node"): tx.Enum(
                 ClusterMode
-            ),
+            ),  # new in APIv6
             t.Key("tag", default=None): t.Null | t.String,
-            t.Key("config", default=dict): t.Mapping(t.String, t.Any),
+            tx.AliasedKey(["startup_command", "startupCommand"], default=None): t.Null | t.String,
+            tx.AliasedKey(["bootstrap_script", "bootstrapScript"], default=None): t.Null | t.String,
+            tx.AliasedKey(["callback_url", "callbackUrl", "callbackURL"], default=None): (
+                t.Null | tx.URL
+            ),
+            t.Key("owner_access_key", default=None): t.Null | t.String,
+            t.Key("open_to_public", default=False): t.Bool,
+            t.Key("config"): t.Dict(
+                {
+                    t.Key("model"): t.String,
+                    tx.AliasedKey(["model_version", "modelVersion"], default=None): (
+                        t.Null | t.String
+                    ),
+                    tx.AliasedKey(
+                        ["model_mount_destination", "modelMountDestination"], default="/models"
+                    ): t.String,
+                    t.Key("environ", default=None): t.Null | t.Mapping(t.String, t.String),
+                    # cluster_size is moved to the root-level parameters
+                    tx.AliasedKey(["scaling_group", "scalingGroup"], default=None): (
+                        t.Null | t.String
+                    ),
+                    t.Key("resources", default=None): t.Null | t.Mapping(t.String, t.Any),
+                    tx.AliasedKey(
+                        ["resource_opts", "resourceOpts"], default=None
+                    ): t.Null | t.Mapping(t.String, t.Any),
+                }
+            ),
         }
     ),
 )
 async def create(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
-    app_ctx: PrivateContext = request.app["services.context"]
-    access_key = request["keypair"]["access_key"]
-    domain_name = request["user"]["domain_name"]
-    user_role = request["user"]["role"]
-    model_id = params["model_id"]
-
-    params["owner_access_key"] = access_key
-    async with root_ctx.db.begin_readonly() as db_conn:
-        owner_uuid, group_id, resource_policy = await query_userinfo(request, params, db_conn)
-
-    log.info("SERVE.CREATE (email:{}, ak:{})", request["user"]["email"], access_key)
-    resp: MutableMapping[str, Any] = {}
-
-    # Resolve the image reference.
-    try:
-        async with root_ctx.db.begin_readonly_session() as session:
-            image_row = await ImageRow.resolve(
-                session,
-                [
-                    ImageRef(params["image_ref"], ["*"], params["architecture"]),
-                    params["image_ref"],
-                ],
-            )
-            img_id = image_row.id
-        requested_image_ref = image_row.image_ref
-        model_mount_path = image_row.labels.get("ai.backend.model-path")
-        async with root_ctx.db.begin_readonly() as conn:
-            query = (
-                sa.select([domains.c.allowed_docker_registries])
-                .select_from(domains)
-                .where(domains.c.name == params["domain"])
-            )
-            allowed_registries = await conn.scalar(query)
-            if requested_image_ref.registry not in allowed_registries:
-                raise AliasResolutionFailed
-    except AliasResolutionFailed:
-        raise ImageNotFound("unknown alias or disallowed registry")
-
-    # Check work directory and reserved name directory.
-    mount_map = params["config"].get("mount_map", {})
-    if mount_map is not None:
-        original_folders = mount_map.keys()
-        alias_folders = mount_map.values()
-        if len(alias_folders) != len(set(alias_folders)):
-            raise InvalidAPIParameters("Duplicate alias folder name exists.")
-
-        alias_name: str
-        for alias_name in alias_folders:
-            if alias_name is None:
-                continue
-            if alias_name.startswith("/home/work/"):
-                alias_name = alias_name.replace("/home/work/", "")
-            if alias_name == "":
-                raise InvalidAPIParameters("Alias name cannot be empty.")
-            if alias_name == model_mount_path:
-                raise InvalidAPIParameters(
-                    f"Alias name cannot be the same with model path: `{model_mount_path}`"
-                )
-            if not verify_vfolder_name(alias_name):
-                raise InvalidAPIParameters(str(alias_name) + " is reserved for internal path.")
-            if alias_name in original_folders:
-                raise InvalidAPIParameters(
-                    f"Alias name cannot be set to an existing folder name: {alias_name}"
-                )
-
-    # Append model mount path
-    mounts: list[str] = params["config"].get("mounts", [])
-    async with root_ctx.db.begin_readonly() as db_conn:
-        query = sa.select([vfolders.c.name]).where(vfolders.c.id == model_id)
-        result = await db_conn.execute(query)
-        vfolder_name = result.first()["name"]
-    model_path = f"{vfolder_name}/versions/{params['model_version']}"
-    mounts = [*mounts, model_path]
-    mount_map = {
-        **mount_map,
-        model_path: model_mount_path,
+    scopes_param = {
+        "owner_access_key": (
+            None if params["owner_access_key"] is undefined else params["owner_access_key"]
+        ),
     }
-    params["config"]["mounts"] = mounts
-    params["config"]["mount_map"] = mount_map
-    for kern_config in params["config"]["kernel_configs"]:
-        kern_config["mounts"] = mounts
-        kern_config["mount_map"] = mount_map
-
-    # Create endpoint
-    async def _create_endpoint() -> uuid.UUID:
-        async with root_ctx.db.begin_session() as db_sess:
-            endpoint_id = uuid.uuid4()
-            endpoint = EndpointRow(
-                id=endpoint_id,
-                image=img_id,
-                model=model_id,
-                domain=domain_name,
-                project=group_id,
-                resource_group=params["config"]["scaling_group"],
-            )
-            db_sess.add(endpoint)
-            return endpoint_id
+    requester_access_key, owner_access_key = await get_access_key_scopes(request, scopes_param)
 
-    if params["endpoint_id"] is None:
-        endpoint_id = await execute_with_retry(_create_endpoint)
-    else:
-        endpoint_id = params["endpoint_id"]
+    async with root_ctx.db.begin_readonly() as conn:
+        checked_scaling_group = await check_scaling_group(
+            conn,
+            params["config"]["scaling_group"],
+            SessionTypes.INFERENCE,
+            owner_access_key,
+            params["domain"],
+            params["group"],
+        )
 
-    # # Check existing (owner_access_key, session_name) instance
-    # try:
-    #     # NOTE: We can reuse the session IDs of TERMINATED sessions only.
-    #     # NOTE: Reusing a session in the PENDING status returns an empty value in service_ports.
-    #     async with root_ctx.db.begin_readonly_session() as db_sess:
-    #         sess = await SessionRow.get_session_with_main_kernel(
-    #             params["session_name"],
-    #             access_key,
-    #             db_session=db_sess,
-    #         )
-    #     running_image_ref = ImageRef(
-    #         sess.main_kernel.image, [sess.main_kernel.registry], sess.main_kernel.architecture
-    #     )
-    #     if running_image_ref != requested_image_ref:
-    #         # The image must be same if get_or_create() called multiple times
-    #         # against an existing (non-terminated) session
-    #         raise SessionAlreadyExists(extra_data={"existingSessionId": str(sess.id)})
-    #     if not params["reuse"]:
-    #         # Respond as error since the client did not request to reuse,
-    #         # but provide the overlapping session ID for later use.
-    #         raise SessionAlreadyExists(extra_data={"existingSessionId": str(sess.id)})
-    #     # Respond as success with the reused session's information.
-    #     return web.json_response(
-    #         {
-    #             "sessionId": str(sess.id),
-    #             "sessionName": str(sess.name),
-    #             "status": sess.status.name,
-    #             "service_ports": sess.main_kernel.service_ports,
-    #             "created": False,
-    #         },
-    #         status=200,
-    #     )
-    # except SessionNotFound:
-    #     # It's time to create a new session.
-    #     pass
-
-    # if params["session_type"] == SessionTypes.BATCH and not params["startup_command"]:
-    #     raise InvalidAPIParameters("Batch sessions must have a non-empty startup command.")
-    # if params["session_type"] != SessionTypes.BATCH and params["starts_at"]:
-    #     raise InvalidAPIParameters("Parameter starts_at should be used only for batch sessions")
+        query = (
+            sa.select([scaling_groups.c.wsproxy_addr])
+            .select_from(scaling_groups)
+            .where((scaling_groups.c.name == checked_scaling_group))
+        )
+
+        result = await conn.execute(query)
+        sgroup = result.first()
+        wsproxy_addr = sgroup["wsproxy_addr"]
+        if not wsproxy_addr:
+            raise ServiceUnavailable("No coordinator configured for this resource group")
+
+        params["config"]["scaling_group"] = checked_scaling_group
 
-    starts_at: Union[datetime, None] = None
-    if params["starts_at"]:
+        owner_uuid, group_id, resource_policy = await query_userinfo(request, params, conn)
+        allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
         try:
-            starts_at = isoparse(params["starts_at"])
-        except ValueError:
-            _td = str_to_timedelta(params["starts_at"])
-            starts_at = datetime.now(tzutc()) + _td
+            extra_vf_conds = (vfolders.c.id == uuid.UUID(params["config"]["model"])) & (
+                vfolders.c.usage_mode == VFolderUsageMode.MODEL
+            )
+            matched_vfolders = await query_accessible_vfolders(
+                conn,
+                owner_uuid,
+                user_role=request["user"]["role"],
+                domain_name=params["domain"],
+                allowed_vfolder_types=allowed_vfolder_types,
+                extra_vf_conds=extra_vf_conds,
+            )
+        except Exception as e:
+            # just catching ValueError | VFolderNotFound will raise
+            # TypeError: catching classes that do not inherit from BaseException is not allowed
+            if isinstance(e, ValueError) or isinstance(e, VFolderNotFound):
+                try:
+                    extra_vf_conds = (vfolders.c.name == params["config"]["model"]) & (
+                        vfolders.c.usage_mode == VFolderUsageMode.MODEL
+                    )
+                    matched_vfolders = await query_accessible_vfolders(
+                        conn,
+                        owner_uuid,
+                        user_role=request["user"]["role"],
+                        domain_name=params["domain"],
+                        allowed_vfolder_types=allowed_vfolder_types,
+                        extra_vf_conds=extra_vf_conds,
+                    )
+                except VFolderNotFound as e:
+                    raise VFolderNotFound("Cannot find model folder") from e
+            else:
+                raise
+        model_id = matched_vfolders[0]["id"]
+
+    async with root_ctx.db.begin_readonly_session() as session:
+        image_row = await ImageRow.resolve(
+            session,
+            [
+                ImageRef(params["image"], ["*"], params["architecture"]),
+                params["image"],
+            ],
+        )
 
-    # if params["cluster_size"] > 1:
-    #     log.debug(" -> cluster_mode:{} (replicate)", params["cluster_mode"])
+    params["config"]["mount_map"] = {model_id: params["config"]["model_mount_destination"]}
 
-    # if params["dependencies"] is None:
-    #     params["dependencies"] = []
+    # check if session is valid to be created
+    await root_ctx.registry.create_session(
+        "",
+        params["image"],
+        params["architecture"],
+        UserScope(
+            domain_name=params["domain"],
+            group_id=group_id,
+            user_uuid=request["user"]["uuid"],
+            user_role=request["user"]["role"],
+        ),
+        owner_access_key,
+        resource_policy,
+        SessionTypes.INFERENCE,
+        params["config"],
+        params["cluster_mode"],
+        params["cluster_size"],
+        dry_run=True,  # Setting this to True will prevent actual session from being enqueued
+        bootstrap_script=params["bootstrap_script"],
+        startup_command=params["startup_command"],
+        tag=params["tag"],
+        callback_url=params["callback_url"],
+    )
 
-    session_creation_id = secrets.token_urlsafe(16)
+    async with root_ctx.db.begin_session() as db_sess:
+        project_id = await resolve_group_name_or_id(
+            await db_sess.connection(), params["domain"], params["group"]
+        )
+        if project_id is None:
+            raise InvalidAPIParameters(f"Invalid group name {project_id}")
+        endpoint = EndpointRow(
+            params["service_name"],
+            request["user"]["uuid"],
+            owner_uuid,
+            params["desired_session_count"],
+            image_row,
+            model_id,
+            params["domain"],
+            project_id,
+            checked_scaling_group,
+            params["config"]["resources"],
+            params["cluster_mode"],
+            params["cluster_size"],
+            model_mount_destination=params["config"]["model_mount_destination"],
+            tag=params["tag"],
+            startup_command=params["startup_command"],
+            callback_url=params["callback_url"],
+            environ=params["config"]["environ"],
+            bootstrap_script=params["bootstrap_script"],
+            resource_opts=params["config"]["resource_opts"],
+            open_to_public=params["open_to_public"],
+        )
+        db_sess.add(endpoint)
+        await db_sess.commit()
 
-    async with root_ctx.db.begin_readonly() as conn:
-        # Use keypair bootstrap_script if it is not delivered as a parameter
-        if not params["bootstrap_script"]:
-            script, _ = await query_bootstrap_script(conn, access_key)
-            params["bootstrap_script"] = script
-
-    try:
-        session_id = await asyncio.shield(
-            app_ctx.database_ptask_group.create_task(
-                root_ctx.registry.enqueue_session(
-                    session_creation_id,
-                    params["service_name"],
-                    access_key,
-                    {
-                        "creation_config": params["config"],
-                        "kernel_configs": [
-                            {
-                                "image_ref": requested_image_ref,
-                                "cluster_role": DEFAULT_ROLE,
-                                "cluster_idx": 1,
-                                "local_rank": 0,
-                                "cluster_hostname": f"{DEFAULT_ROLE}1",
-                                "creation_config": params["config"],
-                                "bootstrap_script": params["bootstrap_script"],
-                                "startup_command": params["startup_command"],
-                            }
-                        ],
-                    },
-                    params["config"]["scaling_group"],
-                    SessionTypes.INFERENCE,
-                    resource_policy,
-                    user_scope=UserScope(
-                        domain_name=domain_name,
-                        group_id=group_id,
-                        user_uuid=owner_uuid,
-                        user_role=user_role,
-                    ),
-                    cluster_mode=params["cluster_mode"],
-                    cluster_size=params["cluster_size"],
-                    session_tag=params["tag"],
-                    starts_at=starts_at,
-                    agent_list=params["config"]["agent_list"],
-                    dependency_sessions=params["dependencies"],
-                )
-            ),
+    return web.json_response({"endpoint_id": str(endpoint.id)})
+
+
+@auth_required
+@server_status_required(READ_ALLOWED)
+async def delete(request: web.Request) -> web.Response:
+    root_ctx: RootContext = request.app["_root.context"]
+    access_key = request["keypair"]["access_key"]
+    service_id = uuid.UUID(request.match_info["service_id"])
+
+    log.info(
+        "SERVE.DELETE (email:{}, ak:{}, s:{})", request["user"]["email"], access_key, service_id
+    )
+
+    async with root_ctx.db.begin_readonly_session() as db_sess:
+        try:
+            endpoint = await EndpointRow.get(db_sess, service_id, load_routes=True)
+        except NoResultFound:
+            raise ObjectNotFound
+    await get_user_uuid_scopes(request, {"owner_uuid": endpoint.session_owner})
+
+    async with root_ctx.db.begin_session() as db_sess:
+        query = (
+            sa.update(EndpointRow)
+            .where(EndpointRow.id == service_id)
+            .values({"desired_session_count": -1})
         )
+        await db_sess.execute(query)
+    return web.json_response({"success": True}, status=200)
+
+
+@auth_required
+@server_status_required(READ_ALLOWED)
+async def sync(request: web.Request) -> web.Response:
+    root_ctx: RootContext = request.app["_root.context"]
+    access_key = request["keypair"]["access_key"]
+    service_id = uuid.UUID(request.match_info["service_id"])
+
+    log.info("SERVE.SYNC (email:{}, ak:{}, s:{})", request["user"]["email"], access_key, service_id)
 
-        # Create routing
-        await RoutingRow.create(root_ctx.db, endpoint_id, session_id)
+    async with root_ctx.db.begin_readonly_session() as db_sess:
+        try:
+            endpoint = await EndpointRow.get(db_sess, service_id, load_routes=True)
+        except NoResultFound:
+            raise ObjectNotFound
+    await get_user_uuid_scopes(request, {"owner_uuid": endpoint.session_owner})
 
-        resp["sessionId"] = str(session_id)  # changed since API v5
-        resp["sessionName"] = str(params["service_name"])
-        resp["status"] = SessionStatus.PENDING.name
-        resp["servicePorts"] = []
-        resp["created"] = True
-
-        # if not params["enqueue_only"]:
-        #     app_ctx.pending_waits.add(current_task)
-        #     max_wait = params["max_wait_seconds"]
-        #     try:
-        #         if max_wait > 0:
-        #             with timeout(max_wait):
-        #                 await start_event.wait()
-        #         else:
-        #             await start_event.wait()
-        #     except asyncio.TimeoutError:
-        #         resp["status"] = "TIMEOUT"
-        #     else:
-        #         await asyncio.sleep(0.5)
-        #         async with root_ctx.db.begin_readonly_session() as db_sess:
-        #             query = sa.select(KernelRow.status, KernelRow.service_ports).where(
-        #                 (KernelRow.session_id == session_id)
-        #                 & (KernelRow.cluster_role == DEFAULT_ROLE)
-        #             )
-        #             result = await db_sess.execute(query)
-        #             row = result.first()
-        #         if row.status == KernelStatus.RUNNING:
-        #             resp["status"] = "RUNNING"
-        #             for item in row.service_ports:
-        #                 response_dict = {
-        #                     "name": item["name"],
-        #                     "protocol": item["protocol"],
-        #                     "ports": item["container_ports"],
-        #                 }
-        #                 if "url_template" in item.keys():
-        #                     response_dict["url_template"] = item["url_template"]
-        #                 if "allowed_arguments" in item.keys():
-        #                     response_dict["allowed_arguments"] = item["allowed_arguments"]
-        #                 if "allowed_envs" in item.keys():
-        #                     response_dict["allowed_envs"] = item["allowed_envs"]
-        #                 resp["servicePorts"].append(response_dict)
-        #         else:
-        #             resp["status"] = row.status.name
-    except asyncio.CancelledError:
-        raise
-    except BackendError:
-        log.exception("GET_OR_CREATE: exception")
-        raise
-    except UnknownImageReference:
-        raise UnknownImageReferenceError(f"Unknown image reference: {params['image']}")
-    except Exception:
-        log.exception("GET_OR_CREATE: unexpected error!")
-        raise InternalServerError
-    return web.json_response(resp, status=201)
+    async with root_ctx.db.begin_session() as db_sess:
+        await root_ctx.registry.update_appproxy_endpoint_routes(db_sess, endpoint)
+    return web.json_response({"success": True}, status=200)
 
 
 @auth_required
 @server_status_required(READ_ALLOWED)
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["endpoint_id", "endpointId"]): tx.UUID | t.String,
+            t.Key("to"): t.Int,
         }
     ),
 )
-async def start(request: web.Request, params: Any) -> web.Response:
+async def scale(request: web.Request, params: Any) -> web.Response:
+    root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
+    service_id = uuid.UUID(request.match_info["service_id"])
 
-    log.info("SERVE.START (email:{}, ak:{})", request["user"]["email"], access_key)
-    return web.Response(status=204)
+    log.info(
+        "SERVE.SCALE (email:{}, ak:{}, s:{})", request["user"]["email"], access_key, service_id
+    )
+
+    async with root_ctx.db.begin_readonly_session() as db_sess:
+        try:
+            endpoint = await EndpointRow.get(db_sess, service_id, load_routes=True)
+        except NoResultFound:
+            raise ObjectNotFound
+    await get_user_uuid_scopes(request, {"owner_uuid": endpoint.session_owner})
+
+    if params["to"] < 0:
+        raise InvalidAPIParameters("Amount of desired session count cannot be a negative number")
+    if params["to"] == len(endpoint.routings):
+        return web.json_response(
+            {"current_route_count": len(endpoint.routings), "target_count": params["to"]}
+        )
+
+    async with root_ctx.db.begin_session() as db_sess:
+        query = (
+            sa.update(EndpointRow)
+            .where(EndpointRow.id == service_id)
+            .values({"desired_session_count": params["to"]})
+        )
+        await db_sess.execute(query)
+        return web.json_response(
+            {"current_route_count": len(endpoint.routings), "target_count": params["to"]}
+        )
 
 
 @auth_required
 @server_status_required(READ_ALLOWED)
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["endpoint_id", "endpointId"]): tx.UUID | t.String,
+            t.Key("traffic_ratio"): t.Float[0:],
         }
     ),
 )
-async def stop(request: web.Request, params: Any) -> web.Response:
+async def update_route(request: web.Request, params: Any) -> web.Response:
+    root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
+    service_id = uuid.UUID(request.match_info["service_id"])
+    route_id = uuid.UUID(request.match_info["route_id"])
+
+    log.info(
+        "SERVE.UPDATE_ROUTE (email:{}, ak:{}, s:{}, r:{})",
+        request["user"]["email"],
+        access_key,
+        service_id,
+        route_id,
+    )
+
+    async with root_ctx.db.begin_session() as db_sess:
+        try:
+            route = await RoutingRow.get(db_sess, route_id, load_endpoint=True)
+        except NoResultFound:
+            raise ObjectNotFound
+        if route.endpoint != service_id:
+            raise ObjectNotFound
+        await get_user_uuid_scopes(request, {"owner_uuid": route.endpoint_row.session_owner})
 
-    log.info("SERVE.STOP (email:{}, ak:{})", request["user"]["email"], access_key)
-    return web.Response(status=204)
+        query = (
+            sa.update(RoutingRow)
+            .where(RoutingRow.id == route_id)
+            .values({"traffic_ratio": params["traffic_ratio"]})
+        )
+        await db_sess.execute(query)
+        endpoint = await EndpointRow.get(db_sess, service_id, load_routes=True)
+        try:
+            await root_ctx.registry.update_appproxy_endpoint_routes(db_sess, endpoint)
+        except aiohttp.ClientError as e:
+            log.warn("failed to communicate with AppProxy endpoint: {}", str(e))
+        return web.json_response({"success": True})
 
 
 @auth_required
 @server_status_required(READ_ALLOWED)
-@check_api_params(
-    t.Dict(
-        {
-            tx.AliasedKey(["endpoint_id", "endpointId"]): tx.UUID | t.String,
-            tx.AliasedKey(["input_args", "inputArgs"], default=dict): t.Mapping(t.String, t.Any),
-        }
-    ),
-)
-async def invoke_serving(request: web.Request, params: Any) -> web.Response:
+async def delete_route(request: web.Request) -> web.Response:
+    root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
+    service_id = uuid.UUID(request.match_info["service_id"])
+    route_id = uuid.UUID(request.match_info["route_id"])
 
-    log.info("SERVE.INVOKE (email:{}, ak:{})", request["user"]["email"], access_key)
-    return web.Response(status=204)
+    log.info(
+        "SERVE.DELETE_ROUTE (email:{}, ak:{}, s:{})",
+        request["user"]["email"],
+        access_key,
+        service_id,
+    )
+    async with root_ctx.db.begin_readonly_session() as db_sess:
+        try:
+            route = await RoutingRow.get(db_sess, route_id, load_session=True)
+        except NoResultFound:
+            raise ObjectNotFound
+        if route.endpoint != service_id:
+            raise ObjectNotFound
+    await get_user_uuid_scopes(request, {"owner_uuid": route.endpoint_row.session_owner})
+    if route.status == RouteStatus.PROVISIONING:
+        raise InvalidAPIParameters("Cannot remove route in PROVISIONING status")
+
+    await root_ctx.registry.destroy_session(
+        route.session_row,
+        forced=False,
+        reason=KernelLifecycleEventReason.SERVICE_SCALED_DOWN,
+    )
+
+    async with root_ctx.db.begin_session() as db_sess:
+        query = (
+            sa.update(EndpointRow)
+            .where(EndpointRow.id == service_id)
+            .values({"desired_session_count": route.endpoint_row.desired_session_count})
+        )
+        await db_sess.execute(query)
+        return web.json_response({"success": True})
 
 
 @auth_required
 @server_status_required(READ_ALLOWED)
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["service_id", "serviceId"]): tx.UUID,
+            t.Key("duration"): tx.TimeDuration,
         }
     ),
 )
-async def delete(request: web.Request, params: Any) -> web.Response:
+async def generate_token(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
-    # session_name = request.match_info["session_name"]
-    service_id = params["service_id"]
-
-    log.info("SERVE.DELETE (email:{}, ak:{})", request["user"]["email"], access_key)
+    service_id = uuid.UUID(request.match_info["service_id"])
 
-    requester_access_key, owner_access_key = await get_access_key_scopes(request, params)
-    if requester_access_key != owner_access_key and request["user"]["role"] not in (
-        UserRole.ADMIN,
-        UserRole.SUPERADMIN,
-    ):
-        raise InsufficientPrivilege("You are not allowed to delete others's services")
+    log.info(
+        "SERVE.GENERATE_TOKEN (email:{}, ak:{}, s:{})",
+        request["user"]["email"],
+        access_key,
+        service_id,
+    )
 
-    async with root_ctx.db.begin_session() as db_sess:
-        # Delete endpoint first
-        await db_sess.execute(sa.delete(EndpointRow).where(session=service_id))
+    async with root_ctx.db.begin_readonly_session() as db_sess:
+        try:
+            endpoint = await EndpointRow.get(db_sess, service_id, load_routes=True)
+        except NoResultFound:
+            raise ObjectNotFound
+        query = (
+            sa.select([scaling_groups.c.wsproxy_addr, scaling_groups.c.wsproxy_api_token])
+            .select_from(scaling_groups)
+            .where((scaling_groups.c.name == endpoint.resource_group))
+        )
 
-        session = await SessionRow.get_session_with_kernels(service_id, db_session=db_sess)
-    last_stat = await root_ctx.registry.destroy_session(
-        session,
-    )
-    resp = {
-        "stats": last_stat,
-    }
-    return web.json_response(resp, status=200)
+        result = await db_sess.execute(query)
+        sgroup = result.first()
+        wsproxy_addr = sgroup["wsproxy_addr"]
+        wsproxy_api_token = sgroup["wsproxy_api_token"]
+
+    await get_user_uuid_scopes(request, {"owner_uuid": endpoint.session_owner})
+
+    exp = datetime.now() + params["duration"]
+    body = {"user_uuid": str(endpoint.session_owner), "exp": int(exp.timestamp())}
+    async with aiohttp.ClientSession() as session:
+        async with session.post(
+            f"{wsproxy_addr}/v2/endpoints/{endpoint.id}/token",
+            json=body,
+            headers={
+                "X-BackendAI-Token": wsproxy_api_token,
+            },
+        ) as resp:
+            token_json = await resp.json()
+            return web.json_response({"token": token_json["token"]})
 
 
 @attrs.define(slots=True, auto_attribs=True, init=False)
 class PrivateContext:
     database_ptask_group: aiotools.PersistentTaskGroup
 
 
@@ -545,13 +602,15 @@
     app.on_shutdown.append(shutdown)
     app["services.context"] = PrivateContext()
     cors = aiohttp_cors.setup(app, defaults=default_cors_options)
     add_route = app.router.add_route
     root_resource = cors.add(app.router.add_resource(r""))
     cors.add(root_resource.add_route("GET", list_serve))
     cors.add(root_resource.add_route("POST", create))
-    cors.add(root_resource.add_route("DELETE", delete))
-    cors.add(add_route("GET", r"/_/info", get_info))
-    cors.add(add_route("POST", r"/_/start", start))
-    cors.add(add_route("POST", r"/_/stop", stop))
-    cors.add(add_route("POST", r"/_/invoke", invoke_serving))
+    cors.add(add_route("GET", "/{service_id}", get_info))
+    cors.add(add_route("DELETE", "/{service_id}", delete))
+    cors.add(add_route("POST", "/{service_id}/scale", scale))
+    cors.add(add_route("POST", "/{service_id}/sync", sync))
+    cors.add(add_route("PUT", "/{service_id}/routings/{route_id}", update_route))
+    cors.add(add_route("DELETE", "/{service_id}/routings/{route_id}", delete_route))
+    cors.add(add_route("POST", "/{service_id}/token", generate_token))
     return app, []
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/session.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,26 @@
 import asyncio
 import base64
 import functools
 import json
 import logging
 import re
 import secrets
-import time
 import uuid
 from datetime import datetime, timedelta
 from decimal import Decimal
-from io import BytesIO
 from pathlib import PurePosixPath
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Mapping,
     MutableMapping,
-    Optional,
     Set,
     Tuple,
     Union,
     cast,
 )
 from urllib.parse import urlparse
 
@@ -36,107 +33,62 @@
 import aiohttp_cors
 import aiotools
 import attrs
 import multidict
 import sqlalchemy as sa
 import sqlalchemy.exc
 import trafaret as t
-import yarl
 from aiohttp import hdrs, web
-from async_timeout import timeout
-from dateutil.parser import isoparse
 from dateutil.tz import tzutc
 from redis.asyncio import Redis
 from sqlalchemy.sql.expression import null, true
 
-from ai.backend.manager.models.image import ImageRow
-
 if TYPE_CHECKING:
     from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection, AsyncSession as SASession
 
 from ai.backend.common import redis_helper
 from ai.backend.common import validators as tx
-from ai.backend.common.docker import ImageRef
 from ai.backend.common.events import (
-    AgentHeartbeatEvent,
-    AgentStartedEvent,
     AgentTerminatedEvent,
-    DoSyncKernelLogsEvent,
-    DoTerminateSessionEvent,
-    KernelCancelledEvent,
-    KernelCreatingEvent,
-    KernelLifecycleEventReason,
-    KernelPreparingEvent,
-    KernelPullingEvent,
-    KernelStartedEvent,
-    KernelTerminatedEvent,
-    KernelTerminatingEvent,
-    SessionCancelledEvent,
-    SessionEnqueuedEvent,
-    SessionFailureEvent,
-    SessionPreparingEvent,
-    SessionScheduledEvent,
-    SessionStartedEvent,
-    SessionSuccessEvent,
-    SessionTerminatedEvent,
-    SessionTerminatingEvent,
 )
-from ai.backend.common.exception import AliasResolutionFailed, UnknownImageReference
+from ai.backend.common.exception import UnknownImageReference
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.plugin.monitor import GAUGE
 from ai.backend.common.types import (
     AccessKey,
     AgentId,
     ClusterMode,
-    KernelEnqueueingConfig,
-    KernelId,
     SessionTypes,
-    check_typed_dict,
 )
-from ai.backend.common.utils import cancel_tasks, str_to_timedelta
 
 from ..config import DEFAULT_CHUNK_SIZE
-from ..defs import DEFAULT_IMAGE_ARCH, DEFAULT_ROLE, REDIS_STREAM_DB
+from ..defs import DEFAULT_IMAGE_ARCH, DEFAULT_ROLE
 from ..models import (
     AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     DEAD_SESSION_STATUSES,
-    PRIVATE_KERNEL_ROLES,
-    AgentStatus,
     KernelRole,
-    KernelRow,
-    KernelStatus,
-    RoutingRow,
     SessionRow,
     SessionStatus,
     UserRole,
-)
-from ..models import association_groups_users as agus
-from ..models import (
-    domains,
     groups,
     kernels,
-    keypair_resource_policies,
     keypairs,
     query_accessible_vfolders,
-    query_bootstrap_script,
     scaling_groups,
     session_templates,
-    users,
-    verify_vfolder_name,
     vfolders,
 )
 from ..models.session import SessionDependencyRow
-from ..models.utils import execute_with_retry
 from ..types import UserScope
+from ..utils import query_userinfo as _query_userinfo
 from .auth import auth_required
 from .exceptions import (
     AppNotFound,
     BackendError,
     GenericForbidden,
-    ImageNotFound,
     InsufficientPrivilege,
     InternalServerError,
     InvalidAPIParameters,
     ObjectNotFound,
     ServiceUnavailable,
     SessionAlreadyExists,
     SessionNotFound,
@@ -334,122 +286,37 @@
 
 
 async def query_userinfo(
     request: web.Request,
     params: Any,
     conn: SAConnection,
 ) -> Tuple[uuid.UUID, uuid.UUID, dict]:
-    if params["domain"] is None:
-        params["domain"] = request["user"]["domain_name"]
-    scopes_param = {
-        "owner_access_key": (
-            None if params["owner_access_key"] is undefined else params["owner_access_key"]
-        ),
-    }
-    requester_access_key, owner_access_key = await get_access_key_scopes(request, scopes_param)
-    requester_uuid = request["user"]["uuid"]
-
-    owner_uuid = None
-    group_id = None
-    resource_policy = None
-
-    if requester_access_key != owner_access_key:
-        # Admin or superadmin is creating sessions for another user.
-        # The check for admin privileges is already done in get_access_key_scope().
-        query = (
-            sa.select(
-                [keypairs.c.user, keypairs.c.resource_policy, users.c.role, users.c.domain_name]
-            )
-            .select_from(sa.join(keypairs, users, keypairs.c.user == users.c.uuid))
-            .where(keypairs.c.access_key == owner_access_key)
-        )
-        result = await conn.execute(query)
-        row = result.first()
-        owner_domain = row["domain_name"]
-        owner_uuid = row["user"]
-        owner_role = row["role"]
-        query = (
-            sa.select([keypair_resource_policies])
-            .select_from(keypair_resource_policies)
-            .where(keypair_resource_policies.c.name == row["resource_policy"])
-        )
-        result = await conn.execute(query)
-        resource_policy = result.first()
-    else:
-        # Normal case when the user is creating her/his own session.
-        owner_domain = request["user"]["domain_name"]
-        owner_uuid = requester_uuid
-        owner_role = UserRole.USER
-        resource_policy = request["keypair"]["resource_policy"]
-
-    query = (
-        sa.select([domains.c.name])
-        .select_from(domains)
-        .where(
-            (domains.c.name == owner_domain) & (domains.c.is_active),
-        )
-    )
-    qresult = await conn.execute(query)
-    domain_name = qresult.scalar()
-    if domain_name is None:
-        raise InvalidAPIParameters("Invalid domain")
-
-    if owner_role == UserRole.SUPERADMIN:
-        # superadmin can spawn container in any designated domain/group.
-        query = (
-            sa.select([groups.c.id])
-            .select_from(groups)
-            .where(
-                (groups.c.domain_name == params["domain"])
-                & (groups.c.name == params["group"])
-                & (groups.c.is_active),
-            )
-        )
-        qresult = await conn.execute(query)
-        group_id = qresult.scalar()
-    elif owner_role == UserRole.ADMIN:
-        # domain-admin can spawn container in any group in the same domain.
-        if params["domain"] != owner_domain:
-            raise InvalidAPIParameters("You can only set the domain to the owner's domain.")
-        query = (
-            sa.select([groups.c.id])
-            .select_from(groups)
-            .where(
-                (groups.c.domain_name == owner_domain)
-                & (groups.c.name == params["group"])
-                & (groups.c.is_active),
-            )
-        )
-        qresult = await conn.execute(query)
-        group_id = qresult.scalar()
-    else:
-        # normal users can spawn containers in their group and domain.
-        if params["domain"] != owner_domain:
-            raise InvalidAPIParameters("You can only set the domain to your domain.")
-        query = (
-            sa.select([agus.c.group_id])
-            .select_from(agus.join(groups, agus.c.group_id == groups.c.id))
-            .where(
-                (agus.c.user_id == owner_uuid)
-                & (groups.c.domain_name == owner_domain)
-                & (groups.c.name == params["group"])
-                & (groups.c.is_active),
-            )
+    try:
+        return await _query_userinfo(
+            conn,
+            request["user"]["uuid"],
+            request["user"]["role"],
+            request["keypair"]["access_key"],
+            request["user"]["domain_name"],
+            request["keypair"]["resource_policy"],
+            params["domain"] or request["user"]["domain_name"],
+            params["group"],
+            query_on_behalf_of=(
+                None if params["owner_access_key"] is undefined else params["owner_access_key"]
+            ),
         )
-        qresult = await conn.execute(query)
-        group_id = qresult.scalar()
-    if group_id is None:
-        raise InvalidAPIParameters("Invalid group")
-
-    return owner_uuid, group_id, resource_policy
+    except ValueError as e:
+        raise InvalidAPIParameters(str(e))
 
 
 async def _create(request: web.Request, params: dict[str, Any]) -> web.Response:
     if params["domain"] is None:
-        params["domain"] = request["user"]["domain_name"]
+        domain_name = request["user"]["domain_name"]
+    else:
+        domain_name = params["domain"]
     scopes_param = {
         "owner_access_key": (
             None if params["owner_access_key"] is undefined else params["owner_access_key"]
         ),
     }
     requester_access_key, owner_access_key = await get_access_key_scopes(request, scopes_param)
     log.info(
@@ -457,238 +324,55 @@
         requester_access_key,
         owner_access_key if owner_access_key != requester_access_key else "*",
         params["image"],
         params["session_name"],
     )
 
     root_ctx: RootContext = request.app["_root.context"]
-    app_ctx: PrivateContext = request.app["session.context"]
-
-    resp: MutableMapping[str, Any] = {}
-    current_task = asyncio.current_task()
-    assert current_task is not None
-
-    # Check work directory and reserved name directory.
-    mount_map = params["config"].get("mount_map")
-
-    if mount_map is not None:
-        original_folders = mount_map.keys()
-        alias_folders = mount_map.values()
-        if len(alias_folders) != len(set(alias_folders)):
-            raise InvalidAPIParameters("Duplicate alias folder name exists.")
-
-        alias_name: str
-        for alias_name in alias_folders:
-            if alias_name is None:
-                continue
-            if alias_name.startswith("/home/work/"):
-                alias_name = alias_name.replace("/home/work/", "")
-            if alias_name == "":
-                raise InvalidAPIParameters("Alias name cannot be empty.")
-            if not verify_vfolder_name(alias_name):
-                raise InvalidAPIParameters(str(alias_name) + " is reserved for internal path.")
-            if alias_name in original_folders:
-                raise InvalidAPIParameters(
-                    "Alias name cannot be set to an existing folder name: " + str(alias_name)
-                )
-
-    # Resolve the image reference.
-    try:
-        async with root_ctx.db.begin_readonly_session() as session:
-            image_row = await ImageRow.resolve(
-                session,
-                [
-                    ImageRef(params["image"], ["*"], params["architecture"]),
-                    params["image"],
-                ],
-            )
-        requested_image_ref = image_row.image_ref
-        if not requested_image_ref.is_local:
-            async with root_ctx.db.begin_readonly() as conn:
-                query = (
-                    sa.select([domains.c.allowed_docker_registries])
-                    .select_from(domains)
-                    .where(domains.c.name == params["domain"])
-                )
-                allowed_registries = await conn.scalar(query)
-                if requested_image_ref.registry not in allowed_registries:
-                    raise AliasResolutionFailed
-    except AliasResolutionFailed:
-        raise ImageNotFound("unknown alias or disallowed registry")
-
-    # Check existing (owner_access_key, session_name) instance
-    try:
-        # NOTE: We can reuse the session IDs of TERMINATED sessions only.
-        # NOTE: Reusing a session in the PENDING status returns an empty value in service_ports.
-        async with root_ctx.db.begin_readonly_session() as db_sess:
-            sess = await SessionRow.get_session_with_main_kernel(
-                params["session_name"],
-                owner_access_key,
-                db_session=db_sess,
-            )
-        running_image_ref = ImageRef(
-            sess.main_kernel.image, [sess.main_kernel.registry], sess.main_kernel.architecture
-        )
-        if running_image_ref != requested_image_ref:
-            # The image must be same if get_or_create() called multiple times
-            # against an existing (non-terminated) session
-            raise SessionAlreadyExists(extra_data={"existingSessionId": str(sess.id)})
-        if not params["reuse"]:
-            # Respond as error since the client did not request to reuse,
-            # but provide the overlapping session ID for later use.
-            raise SessionAlreadyExists(extra_data={"existingSessionId": str(sess.id)})
-        # Respond as success with the reused session's information.
-        return web.json_response(
-            {
-                "sessionId": str(sess.id),
-                "sessionName": str(sess.name),
-                "status": sess.status.name,
-                "service_ports": sess.main_kernel.service_ports,
-                "created": False,
-            },
-            status=200,
-        )
-    except SessionNotFound:
-        # It's time to create a new session.
-        pass
-
-    if params["session_type"] == SessionTypes.BATCH and not params["startup_command"]:
-        raise InvalidAPIParameters("Batch sessions must have a non-empty startup command.")
-    if params["session_type"] != SessionTypes.BATCH and params["starts_at"]:
-        raise InvalidAPIParameters("Parameter starts_at should be used only for batch sessions")
-    starts_at: Union[datetime, None] = None
-    if params["starts_at"]:
-        try:
-            starts_at = isoparse(params["starts_at"])
-        except ValueError:
-            _td = str_to_timedelta(params["starts_at"])
-            starts_at = datetime.now(tzutc()) + _td
-
-    if params["cluster_size"] > 1:
-        log.debug(" -> cluster_mode:{} (replicate)", params["cluster_mode"])
-
-    if params["dependencies"] is None:
-        params["dependencies"] = []
-
-    session_creation_id = secrets.token_urlsafe(16)
-    start_event = asyncio.Event()
-    session_creation_tracker = app_ctx.session_creation_tracker
-    session_creation_tracker[session_creation_id] = start_event
 
     async with root_ctx.db.begin_readonly() as conn:
         owner_uuid, group_id, resource_policy = await query_userinfo(request, params, conn)
 
-        # Use keypair bootstrap_script if it is not delivered as a parameter
-        if not params["bootstrap_script"]:
-            script, _ = await query_bootstrap_script(conn, owner_access_key)
-            params["bootstrap_script"] = script
-
-    public_sgroup_only = True
-    if _role_str := image_row.labels.get("ai.backend.role"):
-        public_sgroup_only = KernelRole(_role_str) not in PRIVATE_KERNEL_ROLES
-    try:
-        session_id = await asyncio.shield(
-            app_ctx.database_ptask_group.create_task(
-                root_ctx.registry.enqueue_session(
-                    session_creation_id,
-                    params["session_name"],
-                    owner_access_key,
-                    {
-                        "creation_config": params["config"],
-                        "kernel_configs": [
-                            {
-                                "image_ref": requested_image_ref,
-                                "cluster_role": DEFAULT_ROLE,
-                                "cluster_idx": 1,
-                                "local_rank": 0,
-                                "cluster_hostname": f"{DEFAULT_ROLE}1",
-                                "creation_config": params["config"],
-                                "bootstrap_script": params["bootstrap_script"],
-                                "startup_command": params["startup_command"],
-                            }
-                        ],
-                    },
-                    params["config"]["scaling_group"],
-                    params["session_type"],
-                    resource_policy,
-                    user_scope=UserScope(
-                        domain_name=params["domain"],  # type: ignore  # params always have it
-                        group_id=group_id,
-                        user_uuid=owner_uuid,
-                        user_role=request["user"]["role"],
-                    ),
-                    cluster_mode=params["cluster_mode"],
-                    cluster_size=params["cluster_size"],
-                    session_tag=params["tag"],
-                    starts_at=starts_at,
-                    agent_list=params["config"]["agent_list"],
-                    dependency_sessions=params["dependencies"],
-                    callback_url=params["callback_url"],
-                    public_sgroup_only=public_sgroup_only,
-                )
+    try:
+        resp = await root_ctx.registry.create_session(
+            params["session_name"],
+            params["image"],
+            params["architecture"],
+            UserScope(
+                domain_name=domain_name,
+                group_id=group_id,
+                user_uuid=request["user"]["uuid"],
+                user_role=request["user"]["role"],
             ),
+            owner_access_key,
+            resource_policy,
+            params["session_type"],
+            params["config"],
+            params["cluster_mode"],
+            params["cluster_size"],
+            reuse=params["reuse"],
+            enqueue_only=params["enqueue_only"],
+            max_wait_seconds=params["max_wait_seconds"],
+            bootstrap_script=params["bootstrap_script"],
+            dependencies=params["dependencies"],
+            startup_command=params["startup_command"],
+            starts_at_timestamp=params["starts_at"],
+            tag=params["tag"],
+            callback_url=params["callback_url"],
         )
-        resp["sessionId"] = str(session_id)  # changed since API v5
-        resp["sessionName"] = str(params["session_name"])
-        resp["status"] = "PENDING"
-        resp["servicePorts"] = []
-        resp["created"] = True
-
-        if not params["enqueue_only"]:
-            app_ctx.pending_waits.add(current_task)
-            max_wait = params["max_wait_seconds"]
-            try:
-                if max_wait > 0:
-                    with timeout(max_wait):
-                        await start_event.wait()
-                else:
-                    await start_event.wait()
-            except asyncio.TimeoutError:
-                resp["status"] = "TIMEOUT"
-            else:
-                await asyncio.sleep(0.5)
-                async with root_ctx.db.begin_readonly_session() as db_sess:
-                    query = sa.select(KernelRow.status, KernelRow.service_ports).where(
-                        (KernelRow.session_id == session_id)
-                        & (KernelRow.cluster_role == DEFAULT_ROLE)
-                    )
-                    result = await db_sess.execute(query)
-                    row = result.first()
-                if row.status == KernelStatus.RUNNING:
-                    resp["status"] = "RUNNING"
-                    for item in row.service_ports:
-                        response_dict = {
-                            "name": item["name"],
-                            "protocol": item["protocol"],
-                            "ports": item["container_ports"],
-                        }
-                        if "url_template" in item.keys():
-                            response_dict["url_template"] = item["url_template"]
-                        if "allowed_arguments" in item.keys():
-                            response_dict["allowed_arguments"] = item["allowed_arguments"]
-                        if "allowed_envs" in item.keys():
-                            response_dict["allowed_envs"] = item["allowed_envs"]
-                        resp["servicePorts"].append(response_dict)
-                else:
-                    resp["status"] = row.status.name
-    except asyncio.CancelledError:
-        raise
+        return web.json_response(resp, status=201)
+    except UnknownImageReference:
+        raise UnknownImageReferenceError(f"Unknown image reference: {params['image']}")
     except BackendError:
         log.exception("GET_OR_CREATE: exception")
         raise
-    except UnknownImageReference:
-        raise UnknownImageReferenceError(f"Unknown image reference: {params['image']}")
     except Exception:
         await root_ctx.error_monitor.capture_exception(context={"user": owner_uuid})
         log.exception("GET_OR_CREATE: unexpected error!")
         raise InternalServerError
-    finally:
-        app_ctx.pending_waits.discard(current_task)
-        del session_creation_tracker[session_creation_id]
-    return web.json_response(resp, status=201)
 
 
 @server_status_required(ALL_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
@@ -978,266 +662,75 @@
             t.Key("owner_access_key", default=None): t.Null | t.String,
         }
     ),
     loads=_json_loads,
 )
 async def create_cluster(request: web.Request, params: dict[str, Any]) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
-    app_ctx: PrivateContext = request.app["session.context"]
     if params["domain"] is None:
-        params["domain"] = request["user"]["domain_name"]
+        domain_name = request["user"]["domain_name"]
+    else:
+        domain_name = params["domain"]
     scopes_param = {
         "owner_access_key": (
             None if params["owner_access_key"] is undefined else params["owner_access_key"]
         ),
     }
     requester_access_key, owner_access_key = await get_access_key_scopes(request, scopes_param)
     log.info(
         "CREAT_CLUSTER (ak:{0}/{1}, s:{3})",
         requester_access_key,
         owner_access_key if owner_access_key != requester_access_key else "*",
         params["session_name"],
     )
 
-    resp: MutableMapping[str, Any] = {}
-
-    # Check existing (owner_access_key, session) kernel instance
-    try:
-        # NOTE: We can reuse the session IDs of TERMINATED sessions only.
-        # NOTE: Reusing a session in the PENDING status returns an empty value in service_ports.
-        async with root_ctx.db.begin_readonly_session() as db_sess:
-            await SessionRow.get_session(
-                params["session_name"],
-                owner_access_key,
-                db_session=db_sess,
-            )
-    except SessionNotFound:
-        pass
-    except TooManySessionsMatched:
-        raise SessionAlreadyExists
-    else:
-        raise SessionAlreadyExists
-
     async with root_ctx.db.begin_readonly() as conn:
         query = (
             sa.select([session_templates.c.template])
             .select_from(session_templates)
             .where(
                 (session_templates.c.id == params["template_id"]) & session_templates.c.is_active,
             )
         )
         template = await conn.scalar(query)
         log.debug("task template: {}", template)
         if not template:
             raise TaskTemplateNotFound
-
-    mounts = []
-    mount_map = {}
-    environ = {}
-
-    if _mounts := template["spec"].get("mounts"):  # noqa
-        mounts = list(_mounts.keys())
-        mount_map = {key: value for (key, value) in _mounts.items() if len(value) > 0}
-    if _environ := template["spec"].get("environ"):  # noqa
-        environ = _environ
-
-    log.debug("cluster template: {}", template)
-
-    kernel_configs: List[KernelEnqueueingConfig] = []
-    for node in template["spec"]["nodes"]:
-        # Resolve session template.
-        kernel_config = {
-            "image": template["spec"]["kernel"]["image"],
-            "architecture": template["spec"]["kernel"].get("architecture", DEFAULT_IMAGE_ARCH),
-            "cluster_role": node["cluster_role"],
-            "creation_config": {
-                "mount": mounts,
-                "mount_map": mount_map,
-                "environ": environ,
-            },
-        }
-
-        if template["spec"]["sess_type"] == "interactive":
-            kernel_config["sess_type"] = SessionTypes.INTERACTIVE
-        elif template["spec"]["sess_type"] == "batch":
-            kernel_config["sess_type"] = SessionTypes.BATCH
-        elif template["spec"]["sess_type"] == "inference":
-            kernel_config["sess_type"] = SessionTypes.INFERENCE
-
-        if tag := template["metadata"].get("tag", None):
-            kernel_config["tag"] = tag
-        if runtime_opt := template["spec"]["kernel"]["run"]:
-            if bootstrap := runtime_opt["bootstrap"]:
-                kernel_config["bootstrap_script"] = bootstrap
-            if startup := runtime_opt["startup_command"]:
-                kernel_config["startup_command"] = startup
-
-        if resources := template["spec"].get("resources"):
-            kernel_config["creation_config"]["resources"] = resources
-
-        if git := template["spec"]["kernel"]["git"]:
-            if _dest := git.get("dest_dir"):
-                target = _dest
-            else:
-                target = git["repository"].split("/")[-1]
-
-            cmd_builder = "git clone "
-            if credential := git.get("credential"):
-                proto, url = git["repository"].split("://")
-                cmd_builder += f'{proto}://{credential["username"]}:{credential["password"]}@{url}'
-            else:
-                cmd_builder += git["repository"]
-            if branch := git.get("branch"):
-                cmd_builder += f" -b {branch}"
-            cmd_builder += f" {target}\n"
-
-            if commit := git.get("commit"):
-                cmd_builder = "CWD=$(pwd)\n" + cmd_builder
-                cmd_builder += f"cd {target}\n"
-                cmd_builder += f"git checkout {commit}\n"
-                cmd_builder += "cd $CWD\n"
-
-            bootstrap = base64.b64decode(kernel_config.get("bootstrap_script") or b"").decode()
-            bootstrap += "\n"
-            bootstrap += cmd_builder
-            kernel_config["bootstrap_script"] = base64.b64encode(bootstrap.encode()).decode()
-
-        # Resolve the image reference.
-        try:
-            async with root_ctx.db.begin_readonly_session() as session:
-                image_row = await ImageRow.resolve(
-                    session,
-                    [
-                        ImageRef(kernel_config["image"], ["*"], kernel_config["architecture"]),
-                        kernel_config["image"],
-                    ],
-                )
-            requested_image_ref = image_row.image_ref
-            async with root_ctx.db.begin_readonly() as conn:
-                query = (
-                    sa.select([domains.c.allowed_docker_registries])
-                    .select_from(domains)
-                    .where(domains.c.name == params["domain"])
-                )
-                allowed_registries = await conn.scalar(query)
-                if requested_image_ref.registry not in allowed_registries:
-                    raise AliasResolutionFailed
-                kernel_config["image_ref"] = requested_image_ref
-        except AliasResolutionFailed:
-            raise ImageNotFound("unknown alias or disallowed registry")
-
-        for i in range(node["replicas"]):
-            kernel_config["cluster_idx"] = i + 1
-            kernel_configs.append(
-                check_typed_dict(kernel_config, KernelEnqueueingConfig),  # type: ignore
-            )
-
-    session_creation_id = secrets.token_urlsafe(16)
-    start_event = asyncio.Event()
-    kernel_id: Optional[KernelId] = None
-    session_creation_tracker = app_ctx.session_creation_tracker
-    session_creation_tracker[session_creation_id] = start_event
-    current_task = asyncio.current_task()
-    assert current_task is not None
+        owner_uuid, group_id, resource_policy = await query_userinfo(request, params, conn)
 
     try:
-        async with root_ctx.db.begin_readonly() as conn:
-            owner_uuid, group_id, resource_policy = await query_userinfo(request, params, conn)
-
-        session_id = await asyncio.shield(
-            app_ctx.database_ptask_group.create_task(
-                root_ctx.registry.enqueue_session(
-                    session_creation_id,
-                    params["session_name"],
-                    owner_access_key,
-                    {
-                        "creation_config": {
-                            "mount_map": mount_map,
-                            "environ": environ,
-                        },
-                        "kernel_configs": kernel_configs,
-                    },
-                    params["scaling_group"],
-                    params["sess_type"],
-                    resource_policy,
-                    user_scope=UserScope(
-                        domain_name=params["domain"],  # type: ignore
-                        group_id=group_id,
-                        user_uuid=owner_uuid,
-                        user_role=request["user"]["role"],
-                    ),
-                    session_tag=params["tag"],
-                ),
-            )
+        resp = await root_ctx.registry.create_cluster(
+            template,
+            params["session_name"],
+            UserScope(
+                domain_name=domain_name,
+                group_id=group_id,
+                user_uuid=request["user"]["uuid"],
+                user_role=request["user"]["role"],
+            ),
+            owner_access_key,
+            resource_policy,
+            params["scaling_group"],
+            params["sess_type"],
+            params["tag"],
+            enqueue_only=params["enqueue_only"],
+            max_wait_seconds=params["max_wait_seconds"],
         )
-        kernel_id = cast(KernelId, session_id)  # the main kernel's ID is the session ID.
-        resp["kernelId"] = str(kernel_id)
-        resp["status"] = "PENDING"
-        resp["servicePorts"] = []
-        resp["created"] = True
-
-        if not params["enqueue_only"]:
-            app_ctx.pending_waits.add(current_task)
-            max_wait = params["max_wait_seconds"]
-            try:
-                if max_wait > 0:
-                    with timeout(max_wait):
-                        await start_event.wait()
-                else:
-                    await start_event.wait()
-            except asyncio.TimeoutError:
-                resp["status"] = "TIMEOUT"
-            else:
-                await asyncio.sleep(0.5)
-                async with root_ctx.db.begin_readonly() as conn:
-                    query = (
-                        sa.select(
-                            [
-                                kernels.c.status,
-                                kernels.c.service_ports,
-                            ]
-                        )
-                        .select_from(kernels)
-                        .where(kernels.c.id == kernel_id)
-                    )
-                    result = await conn.execute(query)
-                    row = result.first()
-                if row["status"] == KernelStatus.RUNNING:
-                    resp["status"] = "RUNNING"
-                    for item in row["service_ports"]:
-                        response_dict = {
-                            "name": item["name"],
-                            "protocol": item["protocol"],
-                            "ports": item["container_ports"],
-                        }
-                        if "url_template" in item.keys():
-                            response_dict["url_template"] = item["url_template"]
-                        if "allowed_arguments" in item.keys():
-                            response_dict["allowed_arguments"] = item["allowed_arguments"]
-                        if "allowed_envs" in item.keys():
-                            response_dict["allowed_envs"] = item["allowed_envs"]
-                        resp["servicePorts"].append(response_dict)
-                else:
-                    resp["status"] = row["status"].name
-
-    except asyncio.CancelledError:
-        raise
+        return web.json_response(resp, status=201)
+    except TooManySessionsMatched:
+        raise SessionAlreadyExists
     except BackendError:
         log.exception("GET_OR_CREATE: exception")
         raise
     except UnknownImageReference:
         raise UnknownImageReferenceError(f"Unknown image reference: {params['image']}")
     except Exception:
         await root_ctx.error_monitor.capture_exception()
         log.exception("GET_OR_CREATE: unexpected error!")
         raise InternalServerError
-    finally:
-        app_ctx.pending_waits.discard(current_task)
-        del session_creation_tracker[session_creation_id]
-    return web.json_response(resp, status=201)
 
 
 @server_status_required(READ_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
@@ -1297,14 +790,19 @@
 
     if session.main_kernel.kernel_host is None:
         kernel_host = urlparse(session.main_kernel.agent_addr).hostname
     else:
         kernel_host = session.main_kernel.kernel_host
     for sport in session.main_kernel.service_ports:
         if sport["name"] == service:
+            if sport["is_inference"]:
+                raise InvalidAPIParameters(
+                    f"{service} is an inference app. Starting inference apps can only be done by"
+                    " starting an inference service."
+                )
             if params["port"]:
                 # using one of the primary/secondary ports of the app
                 try:
                     hport_idx = sport["container_ports"].index(params["port"])
                 except ValueError:
                     raise InvalidAPIParameters(
                         f"Service {service} does not open the port number {params['port']}."
@@ -1486,279 +984,14 @@
         )
     except BackendError:
         log.exception("COMMIT_SESSION: exception")
         raise
     return web.json_response(resp, status=201)
 
 
-async def handle_kernel_creation_lifecycle(
-    app: web.Application,
-    source: AgentId,
-    event: (
-        KernelPreparingEvent
-        | KernelPullingEvent
-        | KernelCreatingEvent
-        | KernelStartedEvent
-        | KernelCancelledEvent
-    ),
-) -> None:
-    """
-    Update the database and perform post_create_kernel() upon
-    the events for each step of kernel creation.
-
-    To avoid race condition between consumer and subscriber event handlers,
-    we only have this handler to subscribe all kernel creation events,
-    but distinguish which one to process using a unique creation_id
-    generated when initiating the create_kernels() agent RPC call.
-    """
-    root_ctx: RootContext = app["_root.context"]
-    log.debug(
-        "handle_kernel_creation_lifecycle: ev:{} k:{}",
-        event.name,
-        event.kernel_id,
-    )
-    if isinstance(event, KernelPreparingEvent):
-        # State transition is done by the DoPrepareEvent handler inside the scheduler-distpacher object.
-        pass
-    elif isinstance(event, KernelPullingEvent):
-        await KernelRow.set_kernel_status(
-            root_ctx.db, event.kernel_id, KernelStatus.PULLING, reason=event.reason
-        )
-    elif isinstance(event, KernelCreatingEvent):
-        await KernelRow.set_kernel_status(
-            root_ctx.db, event.kernel_id, KernelStatus.PREPARING, reason=event.reason
-        )
-    elif isinstance(event, KernelStartedEvent):
-        session_id = event.session_id
-        await root_ctx.registry.finalize_running(event.kernel_id, session_id, event.creation_info)
-        if (endpoint_id := event.creation_info.get("endpoint_id")) is not None:
-            await RoutingRow.create(root_ctx.db, uuid.UUID(endpoint_id), uuid.UUID(str(session_id)))
-    elif isinstance(event, KernelCancelledEvent):
-        log.warning(f"Kernel cancelled, {event.reason = }")
-
-
-async def handle_kernel_termination_lifecycle(
-    app: web.Application,
-    source: AgentId,
-    event: KernelTerminatingEvent | KernelTerminatedEvent,
-) -> None:
-    root_ctx: RootContext = app["_root.context"]
-    if isinstance(event, KernelTerminatingEvent):
-        # The destroy_kernel() API handler will set the "TERMINATING" status.
-        pass
-    elif isinstance(event, KernelTerminatedEvent):
-        await root_ctx.registry.mark_kernel_terminated(
-            event.kernel_id, event.reason, event.exit_code
-        )
-        session_id = event.session_id
-        await root_ctx.registry.check_session_terminated(session_id, event.reason)
-
-
-async def handle_session_creation_lifecycle(
-    app: web.Application,
-    source: AgentId,
-    event: SessionStartedEvent | SessionCancelledEvent,
-) -> None:
-    """
-    Update the database according to the session-level lifecycle events
-    published by the manager.
-    """
-    app_ctx: PrivateContext = app["session.context"]
-    if event.creation_id not in app_ctx.session_creation_tracker:
-        return
-    log.debug("handle_session_creation_lifecycle: ev:{} s:{}", event.name, event.session_id)
-    if isinstance(event, SessionStartedEvent):
-        if tracker := app_ctx.session_creation_tracker.get(event.creation_id):
-            tracker.set()
-    elif isinstance(event, SessionCancelledEvent):
-        if tracker := app_ctx.session_creation_tracker.get(event.creation_id):
-            tracker.set()
-
-
-async def handle_session_termination_lifecycle(
-    app: web.Application,
-    agent_id: AgentId,
-    event: SessionTerminatingEvent | SessionTerminatedEvent,
-) -> None:
-    """
-    Update the database according to the session-level lifecycle events
-    published by the manager.
-    """
-    root_ctx: RootContext = app["_root.context"]
-    if isinstance(event, SessionTerminatingEvent):
-        await root_ctx.registry.mark_session_terminating(event.session_id, event.reason)
-    elif isinstance(event, SessionTerminatedEvent):
-        await root_ctx.registry.mark_session_terminated(event.session_id, event.reason)
-
-
-async def handle_destroy_session(
-    app: web.Application,
-    source: AgentId,
-    event: DoTerminateSessionEvent,
-) -> None:
-    root_ctx: RootContext = app["_root.context"]
-    async with root_ctx.db.begin_session() as db_sess:
-        session = await SessionRow.get_session_with_kernels(event.session_id, db_session=db_sess)
-    await root_ctx.registry.destroy_session(
-        session,
-        forced=False,
-        reason=event.reason or KernelLifecycleEventReason.KILLED_BY_EVENT,
-    )
-
-
-async def _make_session_callback(data: dict[str, Any], url: yarl.URL) -> None:
-    log_func = log.info
-    log_msg: str = ""
-    log_fmt: str = ""
-    log_arg: Any = None
-    begin = time.monotonic()
-    try:
-        async with aiohttp.ClientSession(
-            timeout=aiohttp.ClientTimeout(total=30.0),
-        ) as session:
-            try:
-                async with session.post(url, json=data) as response:
-                    if response.content_length is not None and response.content_length > 0:
-                        log_func = log.warning
-                        log_msg = "warning"
-                        log_fmt = (
-                            "{3[0]} {3[1]} - the callback response body was not empty! "
-                            "(len: {3[2]:,} bytes)"
-                        )
-                        log_arg = (response.status, response.reason, response.content_length)
-                    else:
-                        log_msg = "result"
-                        log_fmt = "{3[0]} {3[1]}"
-                        log_arg = (response.status, response.reason)
-            except aiohttp.ClientError as e:
-                log_func = log.warning
-                log_msg, log_fmt, log_arg = "failed", "{3}", repr(e)
-    except asyncio.CancelledError:
-        log_func = log.warning
-        log_msg, log_fmt, log_arg = "cancelled", "elapsed_time = {3:.6f}", time.monotonic() - begin
-    except asyncio.TimeoutError:
-        log_func = log.warning
-        log_msg, log_fmt, log_arg = "timeout", "elapsed_time = {3:.6f}", time.monotonic() - begin
-    finally:
-        log_func(
-            "Session lifecycle callback " + log_msg + " (e:{0}, s:{1}, url:{2}): " + log_fmt,
-            data["event"],
-            data["session_id"],
-            url,
-            log_arg,
-        )
-
-
-async def invoke_session_callback(
-    app: web.Application,
-    source: AgentId,
-    event: SessionEnqueuedEvent
-    | SessionScheduledEvent
-    | SessionPreparingEvent
-    | SessionStartedEvent
-    | SessionCancelledEvent
-    | SessionTerminatingEvent
-    | SessionTerminatedEvent
-    | SessionSuccessEvent
-    | SessionFailureEvent,
-) -> None:
-    log.info("INVOKE_SESSION_CALLBACK (source:{}, event:{})", source, event)
-    app_ctx: PrivateContext = app["session.context"]
-    root_ctx: RootContext = app["_root.context"]
-
-    try:
-        allow_stale = isinstance(event, (SessionCancelledEvent, SessionTerminatedEvent))
-        async with root_ctx.db.begin_readonly_session() as db_sess:
-            session = await SessionRow.get_session_with_main_kernel(
-                event.session_id, db_session=db_sess, allow_stale=allow_stale
-            )
-    except SessionNotFound:
-        return
-
-    if (callback_url := session.callback_url) is None:
-        return
-
-    data = {
-        "type": "session_lifecycle",
-        "event": event.name.removeprefix("session_"),
-        "session_id": str(event.session_id),
-        "when": datetime.now(tzutc()).isoformat(),
-    }
-
-    app_ctx.webhook_ptask_group.create_task(
-        _make_session_callback(data, callback_url),
-    )
-
-
-async def handle_batch_result(
-    app: web.Application,
-    source: AgentId,
-    event: SessionSuccessEvent | SessionFailureEvent,
-) -> None:
-    """
-    Update the database according to the batch-job completion results
-    """
-    root_ctx: RootContext = app["_root.context"]
-    if isinstance(event, SessionSuccessEvent):
-        await SessionRow.set_session_result(root_ctx.db, event.session_id, True, event.exit_code)
-    elif isinstance(event, SessionFailureEvent):
-        await SessionRow.set_session_result(root_ctx.db, event.session_id, False, event.exit_code)
-    async with root_ctx.db.begin_session() as db_sess:
-        try:
-            session = await SessionRow.get_session_with_kernels(
-                event.session_id, db_session=db_sess
-            )
-        except SessionNotFound:
-            return
-    await root_ctx.registry.destroy_session(
-        session,
-        reason=KernelLifecycleEventReason.TASK_FINISHED,
-    )
-
-
-async def handle_agent_lifecycle(
-    app: web.Application,
-    source: AgentId,
-    event: AgentStartedEvent | AgentTerminatedEvent,
-) -> None:
-    root_ctx: RootContext = app["_root.context"]
-    if isinstance(event, AgentStartedEvent):
-        log.info("instance_lifecycle: ag:{0} joined ({1})", source, event.reason)
-        await root_ctx.registry.update_instance(
-            source,
-            {
-                "status": AgentStatus.ALIVE,
-            },
-        )
-    if isinstance(event, AgentTerminatedEvent):
-        if event.reason == "agent-lost":
-            await root_ctx.registry.mark_agent_terminated(source, AgentStatus.LOST)
-        elif event.reason == "agent-restart":
-            log.info("agent@{0} restarting for maintenance.", source)
-            await root_ctx.registry.update_instance(
-                source,
-                {
-                    "status": AgentStatus.RESTARTING,
-                },
-            )
-        else:
-            # On normal instance termination, kernel_terminated events were already
-            # triggered by the agent.
-            await root_ctx.registry.mark_agent_terminated(source, AgentStatus.TERMINATED)
-
-
-async def handle_agent_heartbeat(
-    app: web.Application,
-    source: AgentId,
-    event: AgentHeartbeatEvent,
-) -> None:
-    root_ctx: RootContext = app["_root.context"]
-    await root_ctx.registry.handle_heartbeat(source, event.agent_info)
-
-
 @catch_unexpected(log)
 async def check_agent_lost(root_ctx: RootContext, interval: float) -> None:
     try:
         now = datetime.now(tzutc())
         timeout = timedelta(seconds=root_ctx.local_config["manager"]["heartbeat-timeout"])
 
         async def _check_impl(r: Redis):
@@ -1770,70 +1003,14 @@
                     )
 
         await redis_helper.execute(root_ctx.redis_live, _check_impl)
     except asyncio.CancelledError:
         pass
 
 
-async def handle_kernel_log(
-    app: web.Application,
-    source: AgentId,
-    event: DoSyncKernelLogsEvent,
-) -> None:
-    root_ctx: RootContext = app["_root.context"]
-    redis_conn = redis_helper.get_redis_object(
-        root_ctx.shared_config.data["redis"], db=REDIS_STREAM_DB
-    )
-    # The log data is at most 10 MiB.
-    log_buffer = BytesIO()
-    log_key = f"containerlog.{event.container_id}"
-    try:
-        list_size = await redis_helper.execute(
-            redis_conn,
-            lambda r: r.llen(log_key),
-        )
-        if list_size is None:
-            # The log data is expired due to a very slow event delivery.
-            # (should never happen!)
-            log.warning(
-                "tried to store console logs for cid:{}, but the data is expired",
-                event.container_id,
-            )
-            return
-        for _ in range(list_size):
-            # Read chunk-by-chunk to allow interleaving with other Redis operations.
-            chunk = await redis_helper.execute(redis_conn, lambda r: r.lpop(log_key))
-            if chunk is None:  # maybe missing
-                log_buffer.write(b"(container log unavailable)\n")
-                break
-            log_buffer.write(chunk)
-        try:
-            log_data = log_buffer.getvalue()
-
-            async def _update_log() -> None:
-                async with root_ctx.db.begin() as conn:
-                    update_query = (
-                        sa.update(kernels)
-                        .values(container_log=log_data)
-                        .where(kernels.c.id == event.kernel_id)
-                    )
-                    await conn.execute(update_query)
-
-            await execute_with_retry(_update_log)
-        finally:
-            # Clear the log data from Redis when done.
-            await redis_helper.execute(
-                redis_conn,
-                lambda r: r.delete(log_key),
-            )
-    finally:
-        log_buffer.close()
-        await redis_conn.close()
-
-
 @catch_unexpected(log)
 async def report_stats(root_ctx: RootContext, interval: float) -> None:
     try:
         stats_monitor = root_ctx.stats_monitor
         await stats_monitor.report_metric(
             GAUGE, "ai.backend.manager.coroutines", len(asyncio.all_tasks())
         )
@@ -2671,103 +1848,28 @@
         if prepared:
             await response.write_eof()
     return response
 
 
 @attrs.define(slots=True, auto_attribs=True, init=False)
 class PrivateContext:
-    session_creation_tracker: Dict[str, asyncio.Event]
-    pending_waits: Set[asyncio.Task[None]]
     agent_lost_checker: asyncio.Task[None]
     stats_task: asyncio.Task[None]
     database_ptask_group: aiotools.PersistentTaskGroup
     rpc_ptask_group: aiotools.PersistentTaskGroup
     webhook_ptask_group: aiotools.PersistentTaskGroup
 
 
 async def init(app: web.Application) -> None:
     root_ctx: RootContext = app["_root.context"]
     app_ctx: PrivateContext = app["session.context"]
-    app_ctx.session_creation_tracker = {}
     app_ctx.database_ptask_group = aiotools.PersistentTaskGroup()
     app_ctx.rpc_ptask_group = aiotools.PersistentTaskGroup()
     app_ctx.webhook_ptask_group = aiotools.PersistentTaskGroup()
 
-    # passive events
-    evd = root_ctx.event_dispatcher
-    evd.consume(
-        KernelPreparingEvent, app, handle_kernel_creation_lifecycle, name="api.session.kprep"
-    )
-    evd.consume(KernelPullingEvent, app, handle_kernel_creation_lifecycle, name="api.session.kpull")
-    evd.consume(
-        KernelCreatingEvent, app, handle_kernel_creation_lifecycle, name="api.session.kcreat"
-    )
-    evd.consume(
-        KernelStartedEvent, app, handle_kernel_creation_lifecycle, name="api.session.kstart"
-    )
-    evd.consume(
-        KernelCancelledEvent, app, handle_kernel_creation_lifecycle, name="api.session.kstart"
-    )
-    evd.subscribe(
-        SessionStartedEvent,
-        app,
-        handle_session_creation_lifecycle,
-        name="api.session.sstart",
-    )
-    evd.subscribe(
-        SessionCancelledEvent,
-        app,
-        handle_session_creation_lifecycle,
-        name="api.session.scancel",
-    )
-    evd.consume(
-        KernelTerminatingEvent,
-        app,
-        handle_kernel_termination_lifecycle,
-        name="api.session.kterming",
-    )
-    evd.consume(
-        KernelTerminatedEvent,
-        app,
-        handle_kernel_termination_lifecycle,
-        name="api.session.kterm",
-    )
-    evd.consume(
-        SessionTerminatingEvent,
-        app,
-        handle_session_termination_lifecycle,
-        name="api.session.sterming",
-    ),
-    evd.consume(
-        SessionTerminatedEvent,
-        app,
-        handle_session_termination_lifecycle,
-        name="api.session.sterm",
-    )
-    evd.consume(SessionEnqueuedEvent, app, invoke_session_callback)
-    evd.consume(SessionScheduledEvent, app, invoke_session_callback)
-    evd.consume(SessionPreparingEvent, app, invoke_session_callback)
-    evd.consume(SessionStartedEvent, app, invoke_session_callback)
-    evd.consume(SessionCancelledEvent, app, invoke_session_callback)
-    evd.consume(SessionTerminatingEvent, app, invoke_session_callback)
-    evd.consume(SessionTerminatedEvent, app, invoke_session_callback)
-    evd.consume(SessionSuccessEvent, app, invoke_session_callback)
-    evd.consume(SessionFailureEvent, app, invoke_session_callback)
-    evd.consume(SessionSuccessEvent, app, handle_batch_result)
-    evd.consume(SessionFailureEvent, app, handle_batch_result)
-    evd.consume(AgentStartedEvent, app, handle_agent_lifecycle)
-    evd.consume(AgentTerminatedEvent, app, handle_agent_lifecycle)
-    evd.consume(AgentHeartbeatEvent, app, handle_agent_heartbeat)
-
-    # action-trigerring events
-    evd.consume(DoSyncKernelLogsEvent, app, handle_kernel_log, name="api.session.syncklog")
-    evd.consume(DoTerminateSessionEvent, app, handle_destroy_session, name="api.session.doterm")
-
-    app_ctx.pending_waits = set()
-
     # Scan ALIVE agents
     app_ctx.agent_lost_checker = aiotools.create_timer(
         functools.partial(check_agent_lost, root_ctx), 1.0
     )
     app_ctx.agent_lost_checker.set_name("agent_lost_checker")
     app_ctx.stats_task = aiotools.create_timer(
         functools.partial(report_stats, root_ctx),
@@ -2783,16 +1885,14 @@
     app_ctx.stats_task.cancel()
     await app_ctx.stats_task
 
     await app_ctx.webhook_ptask_group.shutdown()
     await app_ctx.database_ptask_group.shutdown()
     await app_ctx.rpc_ptask_group.shutdown()
 
-    await cancel_tasks(app_ctx.pending_waits)
-
 
 def create_app(
     default_cors_options: CORSOptions,
 ) -> Tuple[web.Application, Iterable[WebMiddleware]]:
     app = web.Application()
     app.on_startup.append(init)
     app.on_shutdown.append(shutdown)
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/session_template.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/stream.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/stream.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/types.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/utils.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 import trafaret as t
 import yaml
 from aiohttp import web
 
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import AccessKey
 
-from ..models import UserRole, keypairs, users
+from ..models import UserRole, users
+from ..utils import (
+    check_if_requester_is_eligible_to_act_as_target_access_key,
+    check_if_requester_is_eligible_to_act_as_target_user_uuid,
+)
 from .exceptions import GenericForbidden, InvalidAPIParameters, QueryNotImplemented
 
 if TYPE_CHECKING:
     from .context import RootContext
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
@@ -52,53 +56,54 @@
 
 async def get_access_key_scopes(
     request: web.Request, params: Any = None
 ) -> Tuple[AccessKey, AccessKey]:
     if not request["is_authorized"]:
         raise GenericForbidden("Only authorized requests may have access key scopes.")
     root_ctx: RootContext = request.app["_root.context"]
-    requester_access_key: AccessKey = request["keypair"]["access_key"]
-    if (
-        params is not None
-        and (owner_access_key := params.get("owner_access_key", None)) is not None
-        and owner_access_key != requester_access_key
-    ):
-        async with root_ctx.db.begin_readonly() as conn:
-            query = (
-                sa.select([users.c.domain_name, users.c.role])
-                .select_from(sa.join(keypairs, users, keypairs.c.user == users.c.uuid))
-                .where(keypairs.c.access_key == owner_access_key)
+    owner_access_key: Optional[AccessKey] = (params or {}).get("owner_access_key", None)
+    if owner_access_key is None or owner_access_key == request["keypair"]["access_key"]:
+        return request["keypair"]["access_key"], request["keypair"]["access_key"]
+    async with root_ctx.db.begin_readonly() as conn:
+        try:
+            await check_if_requester_is_eligible_to_act_as_target_access_key(
+                conn,
+                request["user"]["role"],
+                request["user"]["domain_name"],
+                owner_access_key,
             )
-            result = await conn.execute(query)
-            row = result.first()
-            if row is None:
-                raise InvalidAPIParameters("Unknown owner access key")
-            owner_domain = row["domain_name"]
-            owner_role = row["role"]
-        if request["is_superadmin"]:
-            pass
-        elif request["is_admin"]:
-            if request["user"]["domain_name"] != owner_domain:
-                raise GenericForbidden(
-                    (
-                        "Domain-admins can perform operations on behalf of "
-                        "other users in the same domain only."
-                    ),
-                )
-            if owner_role == UserRole.SUPERADMIN:
-                raise GenericForbidden(
-                    "Domain-admins cannot perform operations on behalf of super-admins.",
-                )
-            pass
-        else:
-            raise GenericForbidden(
-                "Only admins can perform operations on behalf of other users.",
+            return request["keypair"]["access_key"], owner_access_key
+        except ValueError as e:
+            raise InvalidAPIParameters(str(e))
+        except RuntimeError as e:
+            raise GenericForbidden(str(e))
+
+
+async def get_user_uuid_scopes(
+    request: web.Request, params: Any = None
+) -> Tuple[uuid.UUID, uuid.UUID]:
+    if not request["is_authorized"]:
+        raise GenericForbidden("Only authorized requests may have access key scopes.")
+    root_ctx: RootContext = request.app["_root.context"]
+    owner_uuid: Optional[uuid.UUID] = (params or {}).get("owner_uuid", None)
+    if owner_uuid is None or owner_uuid == request["user"]["uuid"]:
+        return request["user"]["uuid"], request["user"]["uuid"]
+    async with root_ctx.db.begin_readonly() as conn:
+        try:
+            await check_if_requester_is_eligible_to_act_as_target_user_uuid(
+                conn,
+                request["user"]["role"],
+                request["user"]["domain_name"],
+                owner_uuid,
             )
-        return requester_access_key, owner_access_key
-    return requester_access_key, requester_access_key
+            return request["user"]["uuid"], owner_uuid
+        except ValueError as e:
+            raise InvalidAPIParameters(str(e))
+        except RuntimeError as e:
+            raise GenericForbidden(str(e))
 
 
 async def get_user_scopes(
     request: web.Request,
     params: Optional[dict[str, Any]] = None,
 ) -> tuple[uuid.UUID, UserRole]:
     root_ctx: RootContext = request.app["_root.context"]
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/vfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 from pathlib import Path
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
+    Concatenate,
     Dict,
     List,
     Mapping,
     MutableMapping,
-    Optional,
+    ParamSpec,
     Sequence,
     Tuple,
-    Type,
+    TypeAlias,
 )
 
 import aiohttp
 import aiohttp_cors
 import aiotools
 import attrs
 import sqlalchemy as sa
@@ -37,31 +38,33 @@
 from ai.backend.common import msgpack, redis_helper
 from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import (
     RedisConnectionInfo,
     VFolderHostPermission,
     VFolderHostPermissionMap,
+    VFolderID,
+    VFolderUsageMode,
 )
 from ai.backend.manager.models.storage import StorageSessionManager
 
 from ..models import (
+    ACTIVE_USER_STATUSES,
     AgentStatus,
     KernelStatus,
     UserRole,
     UserStatus,
     VFolderAccessStatus,
     VFolderCloneInfo,
     VFolderDeletionInfo,
     VFolderInvitationState,
     VFolderOperationStatus,
     VFolderOwnershipType,
     VFolderPermission,
     VFolderPermissionValidator,
-    VFolderUsageMode,
     agents,
     ensure_host_permission_allowed,
     filter_host_allowed_permission,
     get_allowed_vfolder_hosts_by_group,
     get_allowed_vfolder_hosts_by_user,
     groups,
     initiate_vfolder_clone,
@@ -83,15 +86,14 @@
     BackendAgentError,
     GenericForbidden,
     GroupNotFound,
     InsufficientPrivilege,
     InternalServerError,
     InvalidAPIParameters,
     ObjectNotFound,
-    ServerMisconfiguredError,
     TooManyVFoldersFound,
     VFolderAlreadyExists,
     VFolderCreationFailed,
     VFolderFilterStatusFailed,
     VFolderFilterStatusNotAvailable,
     VFolderNotFound,
     VFolderOperationFailed,
@@ -101,41 +103,40 @@
 from .utils import check_api_params, get_user_scopes
 
 if TYPE_CHECKING:
     from .context import RootContext
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
-VFolderRow = Mapping[str, Any]
+VFolderRow: TypeAlias = Mapping[str, Any]
+P = ParamSpec("P")
 
 
 async def ensure_vfolder_status(
     request: web.Request,
     perm: VFolderAccessStatus,
-    folder_id: Optional[str] = None,
-    folder_name: Optional[str] = None,
-):
+    folder_id_or_name: uuid.UUID | str,
+) -> Sequence[VFolderRow]:
     """
     Checks if the target vfolder status is READY.
     This function should prevent user access
     while storage-proxy operations such as vfolder clone, deletion is handling.
     """
 
     root_ctx: RootContext = request.app["_root.context"]
     domain_name = request["user"]["domain_name"]
     user_role = request["user"]["role"]
     user_uuid = request["user"]["uuid"]
 
     allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
-    if folder_id:
-        vf_name_conds = vfolders.c.id == folder_id
-    elif folder_name:
-        vf_name_conds = vfolders.c.name == folder_name
-    else:
-        raise VFolderFilterStatusFailed("either vFolder id nor name not supplied")
+    match folder_id_or_name:
+        case uuid.UUID():
+            vf_name_conds = vfolders.c.id == folder_id_or_name
+        case str():
+            vf_name_conds = vfolders.c.name == folder_id_or_name
 
     available_vf_statuses = set()
     match perm:
         case VFolderAccessStatus.READABLE:
             # if READABLE access status is requested, all operation statuses are accepted.
             available_vf_statuses = {
                 VFolderOperationStatus.READY,
@@ -152,49 +153,53 @@
             }
         case VFolderAccessStatus.DELETABLE:
             # if DELETABLE access status is requested, only READY operation status is accepted.
             available_vf_statuses = {
                 VFolderOperationStatus.READY,
             }
         case _:
-            # Otherwise, raise VFolderFilterStatusNotAvailable()
             raise VFolderFilterStatusNotAvailable()
     async with root_ctx.db.begin_readonly() as conn:
         entries = await query_accessible_vfolders(
             conn,
             user_uuid,
             user_role=user_role,
             domain_name=domain_name,
             allowed_vfolder_types=allowed_vfolder_types,
             extra_vf_conds=vf_name_conds,
             allow_privileged_access=True,
         )
         if len(entries) == 0:
-            raise VFolderFilterStatusFailed(
-                f"Cannot find any folder with the given identity ({folder_id = }, {folder_name = })"
-            )
+            raise VFolderNotFound(extra_data=str(folder_id_or_name))
         for entry in entries:
             if entry["status"] not in available_vf_statuses:
                 raise VFolderFilterStatusFailed()
+        return entries
 
 
-def vfolder_permission_required(perm: VFolderPermission):
+def vfolder_permission_required(
+    perm: VFolderPermission,
+) -> Callable[
+    [Callable[Concatenate[web.Request, VFolderRow, P], Awaitable[web.Response]]],
+    Callable[Concatenate[web.Request, P], Awaitable[web.Response]],
+]:
     """
     Checks if the target vfolder exists and is either:
     - owned by the current access key, or
     - allowed accesses by the access key under the specified permission.
 
     The decorated handler should accept an extra argument
     which contains a dict object describing the matched VirtualFolder table row.
     """
 
-    # FIXME: replace ... with [web.Request, VFolderRow, Any...] in the future mypy
-    def _wrapper(handler: Callable[..., Awaitable[web.Response]]):
+    def _wrapper(
+        handler: Callable[Concatenate[web.Request, VFolderRow, P], Awaitable[web.Response]]
+    ) -> Callable[Concatenate[web.Request, P], Awaitable[web.Response]]:
         @functools.wraps(handler)
-        async def _wrapped(request: web.Request, *args, **kwargs) -> web.Response:
+        async def _wrapped(request: web.Request, *args: P.args, **kwargs: P.kwargs) -> web.Response:
             root_ctx: RootContext = request.app["_root.context"]
             domain_name = request["user"]["domain_name"]
             user_role = request["user"]["role"]
             user_uuid = request["user"]["uuid"]
             folder_name = request.match_info["name"]
             allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
             vf_user_cond = None
@@ -236,46 +241,47 @@
                 if not request["is_admin"]:
                     vf_group_cond = vfolders.c.permission == VFolderPermission.RW_DELETE
             else:
                 # Otherwise, just compare it as-is (for future compatibility).
                 invited_perm_cond = vfolder_permissions.c.permission == perm
                 if not request["is_admin"]:
                     vf_group_cond = vfolders.c.permission == perm
-            async with root_ctx.db.begin() as conn:
+            async with root_ctx.db.begin_readonly() as conn:
                 entries = await query_accessible_vfolders(
                     conn,
                     user_uuid,
                     user_role=user_role,
                     domain_name=domain_name,
                     allowed_vfolder_types=allowed_vfolder_types,
                     extra_vf_conds=(vfolders.c.name == folder_name),
                     extra_invited_vf_conds=invited_perm_cond,
                     extra_vf_user_conds=vf_user_cond,
                     extra_vf_group_conds=vf_group_cond,
                 )
                 if len(entries) == 0:
-                    raise VFolderNotFound("Your operation may be permission denied.")
+                    raise VFolderNotFound(extra_data=folder_name)
             return await handler(request, entries[0], *args, **kwargs)
 
         return _wrapped
 
     return _wrapper
 
 
-# FIXME: replace ... with [web.Request, VFolderRow, Any...] in the future mypy
-def vfolder_check_exists(handler: Callable[..., Awaitable[web.Response]]):
+def vfolder_check_exists(
+    handler: Callable[Concatenate[web.Request, VFolderRow, P], Awaitable[web.Response]]
+) -> Callable[Concatenate[web.Request, P], Awaitable[web.Response]]:
     """
     Checks if the target vfolder exists and is owned by the current user.
 
     The decorated handler should accept an extra "row" argument
     which contains the matched VirtualFolder table row.
     """
 
     @functools.wraps(handler)
-    async def _wrapped(request: web.Request, *args, **kwargs) -> web.Response:
+    async def _wrapped(request: web.Request, *args: P.args, **kwargs: P.kwargs) -> web.Response:
         root_ctx: RootContext = request.app["_root.context"]
         user_uuid = request["user"]["uuid"]
         folder_name = request.match_info["name"]
         async with root_ctx.db.begin() as conn:
             j = sa.join(
                 vfolders,
                 vfolder_permissions,
@@ -321,15 +327,15 @@
     ),
 )
 async def create(request: web.Request, params: Any) -> web.Response:
     resp: Dict[str, Any] = {}
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
     user_role = request["user"]["role"]
-    user_uuid = request["user"]["uuid"]
+    user_uuid: uuid.UUID = request["user"]["uuid"]
     resource_policy = request["keypair"]["resource_policy"]
     domain_name = request["user"]["domain_name"]
     group_id_or_name = params["group"]
     log.info(
         "VFOLDER.CREATE (email:{}, ak:{}, vf:{}, vfh:{}, umod:{}, perm:{})",
         request["user"]["email"],
         access_key,
@@ -349,148 +355,177 @@
         # Resolve host for the new virtual folder.
         if not folder_host:
             folder_host = await root_ctx.shared_config.etcd.get("volumes/default_host")
             if not folder_host:
                 raise InvalidAPIParameters(
                     "You must specify the vfolder host because the default host is not configured."
                 )
+
     allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
-    for vf_type in allowed_vfolder_types:
-        if vf_type not in ("user", "group"):
-            raise ServerMisconfiguredError(
-                f"Invalid vfolder type(s): {str(allowed_vfolder_types)}."
-                ' Only "user" or "group" is allowed.'
-            )
 
     if not verify_vfolder_name(params["name"]):
         raise InvalidAPIParameters(f'{params["name"]} is reserved for internal operations.')
     if params["name"].startswith(".") and params["name"] != ".local":
         if params["group"] is not None:
             raise InvalidAPIParameters("dot-prefixed vfolders cannot be a group folder.")
 
+    group_uuid: uuid.UUID | None = None
+
     async with root_ctx.db.begin() as conn:
-        # Convert group name to uuid if group name is given.
-        if isinstance(group_id_or_name, str):
-            query = (
-                sa.select([groups.c.id])
-                .select_from(groups)
-                .where(groups.c.domain_name == domain_name)
-                .where(groups.c.name == group_id_or_name)
-            )
-            group_id = await conn.scalar(query)
+        match group_id_or_name:
+            case str():
+                # Convert the group name to group uuid.
+                query = (
+                    sa.select([groups.c.id])
+                    .select_from(groups)
+                    .where(groups.c.domain_name == domain_name)
+                    .where(groups.c.name == group_id_or_name)
+                )
+                _gid = await conn.scalar(query)
+                if _gid is None:
+                    raise GroupNotFound(extra_data=group_id_or_name)
+                group_uuid = _gid
+            case uuid.UUID():
+                # Check if the group belongs to the current domain.
+                query = (
+                    sa.select([groups.c.id])
+                    .select_from(groups)
+                    .where(groups.c.domain_name == domain_name)
+                    .where(groups.c.id == group_id_or_name)
+                )
+                _gid = await conn.scalar(query)
+                if _gid is None:
+                    raise GroupNotFound(extra_data=group_id_or_name)
+                group_uuid = group_id_or_name
+            case None:
+                pass
+            case _:
+                raise GroupNotFound(extra_data=group_id_or_name)
+
+        # Check if group exists when it's given a non-empty value.
+        if group_id_or_name and group_uuid is None:
+            raise GroupNotFound(extra_data=group_id_or_name)
+
+        # Determine the ownership type and the quota scope ID.
+        if group_uuid is not None:
+            ownership_type = "group"
+            quota_scope_id = group_uuid.hex
+            if not request["is_admin"]:
+                raise GenericForbidden("no permission")
         else:
-            group_id = group_id_or_name
+            ownership_type = "user"
+            quota_scope_id = user_uuid.hex
+        if ownership_type not in allowed_vfolder_types:
+            raise InvalidAPIParameters(
+                f"{ownership_type}-owned vfolder is not allowed in this cluster"
+            )
+
         if not unmanaged_path:
             await ensure_host_permission_allowed(
                 conn,
                 folder_host,
                 allowed_vfolder_types=allowed_vfolder_types,
                 user_uuid=user_uuid,
                 resource_policy=resource_policy,
                 domain_name=domain_name,
-                group_id=group_id,
+                group_id=group_uuid,
                 permission=VFolderHostPermission.CREATE,
             )
 
         # Check resource policy's max_vfolder_count
         if resource_policy["max_vfolder_count"] > 0:
             query = sa.select([sa.func.count()]).where(vfolders.c.user == user_uuid)
             result = await conn.scalar(query)
             if result >= resource_policy["max_vfolder_count"]:
                 raise InvalidAPIParameters("You cannot create more vfolders.")
 
-        # Limit vfolder size quota if it is larger than max_vfolder_size of the resource policy.
-        max_vfolder_size = resource_policy.get("max_vfolder_size", 0)
-        if max_vfolder_size > 0 and (
-            params["quota"] is None or params["quota"] <= 0 or params["quota"] > max_vfolder_size
-        ):
-            params["quota"] = max_vfolder_size
+        # DEPRECATED: Limit vfolder size quota if it is larger than max_vfolder_size of the resource policy.
+        # max_vfolder_size = resource_policy.get("max_vfolder_size", 0)
+        # if max_vfolder_size > 0 and (
+        #     params["quota"] is None or params["quota"] <= 0 or params["quota"] > max_vfolder_size
+        # ):
+        #     params["quota"] = max_vfolder_size
 
         # Prevent creation of vfolder with duplicated name.
         extra_vf_conds = [vfolders.c.name == params["name"]]
         if not unmanaged_path:
             extra_vf_conds.append(vfolders.c.host == folder_host)
         entries = await query_accessible_vfolders(
             conn,
             user_uuid,
             user_role=user_role,
             domain_name=domain_name,
             allowed_vfolder_types=allowed_vfolder_types,
             extra_vf_conds=(sa.and_(*extra_vf_conds)),
         )
         if len(entries) > 0:
-            raise VFolderAlreadyExists
-
-        # Check if group exists.
-        if group_id_or_name and group_id is None:
-            raise GroupNotFound
-        if group_id is not None:
-            if "group" not in allowed_vfolder_types:
-                raise InvalidAPIParameters("group vfolder cannot be created in this host")
-            if not request["is_admin"]:
-                raise GenericForbidden("no permission")
-            query = (
-                sa.select([groups.c.id])
-                .select_from(groups)
-                .where(groups.c.domain_name == domain_name)
-                .where(groups.c.id == group_id)
-            )
-            _gid = await conn.scalar(query)
-            if str(_gid) != str(group_id):
-                raise InvalidAPIParameters("No such group.")
-        else:
-            if "user" not in allowed_vfolder_types:
-                raise InvalidAPIParameters("user vfolder cannot be created in this host")
+            raise VFolderAlreadyExists(extra_data=params["name"])
         try:
             folder_id = uuid.uuid4()
+            vfid = VFolderID(quota_scope_id, folder_id)
             if not unmanaged_path:
-                # Try to create actual only if vFolder is managed one
+                # Create the vfolder only when it is a managed one
+                # TODO: Create the quota scope with an unlimited quota config if not exists
+                #       The quota may be set later by the admin...
+                # TODO: Introduce "default quota config" for users and projects (which cannot be
+                #       modified by users)
+                # async with root_ctx.storage_manager.request(
+                #     folder_host,
+                #     "POST",
+                #     "quota-scope",
+                #     json={
+                #         "volume": root_ctx.storage_manager.split_host(folder_host)[1],
+                #         "qsid": str(quota_scope_id),
+                #         "options": None,
+                #     },
+                # ):
+                #     pass
                 async with root_ctx.storage_manager.request(
                     folder_host,
                     "POST",
                     "folder/create",
                     json={
                         "volume": root_ctx.storage_manager.split_host(folder_host)[1],
-                        "vfid": str(folder_id),
-                        "options": {"quota": params["quota"]},
+                        "vfid": str(vfid),
                     },
                 ):
                     pass
         except aiohttp.ClientResponseError:
             raise VFolderCreationFailed
-        user_uuid = str(user_uuid) if group_id is None else None
-        group_uuid = str(group_id) if group_id is not None else None
-        ownership_type = "group" if group_uuid is not None else "user"
+        # TODO: include quota scope ID in the database
+        # TODO: include quota scope ID in the API response
         insert_values = {
-            "id": folder_id.hex,
+            "id": vfid.folder_id.hex,
             "name": params["name"],
+            "quota_scope_id": quota_scope_id,
             "usage_mode": params["usage_mode"],
             "permission": params["permission"],
             "last_used": None,
             "max_size": int(params["quota"] / (2**20)) if params["quota"] else None,  # in MBytes
             "host": folder_host,
             "creator": request["user"]["email"],
             "ownership_type": VFolderOwnershipType(ownership_type),
-            "user": user_uuid,
-            "group": group_uuid,
+            "user": user_uuid if ownership_type == "user" else None,
+            "group": group_uuid if ownership_type == "group" else None,
             "unmanaged_path": "",
             "cloneable": params["cloneable"],
             "status": VFolderOperationStatus.READY,
         }
         resp = {
-            "id": folder_id.hex,
+            "id": vfid.folder_id.hex,
             "name": params["name"],
+            "quota_scope_id": quota_scope_id,
             "host": folder_host,
             "usage_mode": params["usage_mode"].value,
             "permission": params["permission"].value,
             "max_size": int(params["quota"] / (2**20)) if params["quota"] else None,  # in MBytes
             "creator": request["user"]["email"],
             "ownership_type": ownership_type,
-            "user": user_uuid,
-            "group": group_uuid,
+            "user": str(user_uuid) if ownership_type == "user" else None,
+            "group": str(group_uuid) if ownership_type == "group" else None,
             "cloneable": params["cloneable"],
             "status": VFolderOperationStatus.READY,
         }
         if unmanaged_path:
             insert_values.update(
                 {
                     "host": "",
@@ -547,14 +582,15 @@
                 extra_vf_conds=extra_vf_conds,
             )
         for entry in entries:
             resp.append(
                 {
                     "name": entry["name"],
                     "id": entry["id"].hex,
+                    "quota_scope_id": entry["quota_scope_id"],
                     "host": entry["host"],
                     "status": entry["status"],
                     "usage_mode": entry["usage_mode"].value,
                     "created_at": str(entry["created_at"]),
                     "is_owner": entry["is_owner"],
                     "permission": entry["permission"].value,
                     "user": str(entry["user"]) if entry["user"] else None,
@@ -579,44 +615,51 @@
     t.Dict(
         {
             t.Key("id"): t.String,
         }
     ),
 )
 async def delete_by_id(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(request, VFolderAccessStatus.DELETABLE, folder_id=params["id"])
+    await ensure_vfolder_status(request, VFolderAccessStatus.DELETABLE, params["id"])
     root_ctx: RootContext = request.app["_root.context"]
     app_ctx: PrivateContext = request.app["folders.context"]
 
     access_key = request["keypair"]["access_key"]
     user_uuid = request["user"]["uuid"]
     domain_name = request["user"]["domain_name"]
     resource_policy = request["keypair"]["resource_policy"]
     allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
     log.info(
         "VFOLDER.DELETE_BY_ID (email:{}, ak:{}, vf:{})",
         request["user"]["email"],
         access_key,
         params["id"],
     )
-    async with root_ctx.db.begin() as conn:
+    async with root_ctx.db.begin_readonly() as conn:
         query = (
-            sa.select([vfolders.c.host]).select_from(vfolders).where(vfolders.c.id == params["id"])
+            sa.select(
+                [
+                    vfolders.c.quota_scope_id,
+                    vfolders.c.host,
+                ]
+            )
+            .select_from(vfolders)
+            .where(vfolders.c.id == params["id"])
         )
-        folder_host = await conn.scalar(query)
+        quota_scope_id, folder_host = await conn.scalar(query)
         await ensure_host_permission_allowed(
             conn,
             folder_host,
             allowed_vfolder_types=allowed_vfolder_types,
             user_uuid=user_uuid,
             resource_policy=resource_policy,
             domain_name=domain_name,
             permission=VFolderHostPermission.DELETE,
         )
-    folder_id = uuid.UUID(params["id"])
+    folder_id = VFolderID(quota_scope_id, uuid.UUID(params["id"]))
     await initiate_vfolder_removal(
         root_ctx.db,
         [VFolderDeletionInfo(folder_id, folder_host)],
         root_ctx.storage_manager,
         app_ctx.storage_ptask_group,
     )
     return web.Response(status=204)
@@ -818,17 +861,15 @@
     return web.json_response(allowed_vfolder_types, status=200)
 
 
 @auth_required
 @server_status_required(READ_ALLOWED)
 @vfolder_permission_required(VFolderPermission.READ_ONLY)
 async def get_info(request: web.Request, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.READABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     resp: Dict[str, Any] = {}
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     log.info(
         "VFOLDER.GETINFO (email:{}, ak:{}, vf:{})",
         request["user"]["email"],
@@ -852,14 +893,15 @@
         },
     ) as (_, storage_resp):
         usage = await storage_resp.json()
     resp = {
         "name": row["name"],
         "id": row["id"].hex,
         "host": row["host"],
+        "quota_scope_id": row["quota_scope_id"],
         "status": row["status"],
         "numFiles": usage["file_count"],  # legacy
         "num_files": usage["file_count"],
         "used_bytes": usage["used_bytes"],  # added in v20.09
         "created": str(row["created_at"]),  # legacy
         "created_at": str(row["created_at"]),
         "last_used": str(row["created_at"]),
@@ -883,15 +925,15 @@
         {
             t.Key("folder_host"): t.String,
             t.Key("id"): tx.UUID,
         }
     )
 )
 async def get_quota(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, folder_id=params["id"])
+    await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, params["id"])
     root_ctx: RootContext = request.app["_root.context"]
     proxy_name, volume_name = root_ctx.storage_manager.split_host(params["folder_host"])
     log.info(
         "VFOLDER.GET_QUOTA (email:{}, volume_name:{}, vf:{})",
         request["user"]["email"],
         volume_name,
         params["id"],
@@ -911,16 +953,16 @@
                 conn,
                 user_uuid,
                 user_role=user_role,
                 domain_name=domain_name,
                 allowed_vfolder_types=allowed_vfolder_types,
                 extra_vf_conds=(sa.and_(*extra_vf_conds)),
             )
-        if len(entries) < 0:
-            raise VFolderNotFound("no such accessible vfolder")
+        if len(entries) == 0:
+            raise VFolderNotFound(extra_data=params["id"])
 
     async with root_ctx.storage_manager.request(
         proxy_name,
         "GET",
         "volume/quota",
         json={
             "volume": volume_name,
@@ -939,15 +981,15 @@
             t.Key("folder_host"): t.String,
             t.Key("id"): tx.UUID,
             t.Key("input"): t.Mapping(t.String, t.Any),
         }
     ),
 )
 async def update_quota(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, folder_id=params["id"])
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, params["id"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_host = params["folder_host"]
     proxy_name, volume_name = root_ctx.storage_manager.split_host(folder_host)
     quota = int(params["input"]["size_bytes"])
     log.info(
         "VFOLDER.UPDATE_QUOTA (email:{}, volume_name:{}, quota:{}, vf:{})",
         request["user"]["email"],
@@ -981,16 +1023,16 @@
                 conn,
                 user_uuid,
                 user_role=user_role,
                 domain_name=domain_name,
                 allowed_vfolder_types=allowed_vfolder_types,
                 extra_vf_conds=(sa.and_(*extra_vf_conds)),
             )
-        if len(entries) < 0:
-            raise VFolderNotFound("no such accessible vfolder")
+        if len(entries) == 0:
+            raise VFolderNotFound(extra_data=params["id"])
 
     # Limit vfolder size quota if it is larger than max_vfolder_size of the resource policy.
     max_vfolder_size = resource_policy.get("max_vfolder_size", 0)
     if max_vfolder_size > 0 and (quota <= 0 or quota > max_vfolder_size):
         quota = max_vfolder_size
 
     async with root_ctx.storage_manager.request(
@@ -1025,30 +1067,30 @@
         {
             t.Key("folder_host"): t.String,
             t.Key("id"): tx.UUID,
         }
     )
 )
 async def get_usage(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, folder_id=params["id"])
+    entries = await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, params["id"])
     root_ctx: RootContext = request.app["_root.context"]
     proxy_name, volume_name = root_ctx.storage_manager.split_host(params["folder_host"])
     log.info(
         "VFOLDER.GET_USAGE (email:{}, volume_name:{}, vf:{})",
         request["user"]["email"],
         volume_name,
         params["id"],
     )
     async with root_ctx.storage_manager.request(
         proxy_name,
         "GET",
         "folder/usage",
         json={
             "volume": volume_name,
-            "vfid": str(params["id"]),
+            "vfid": str(VFolderID(entries[0]["quota_scope_id"], params["id"])),
         },
     ) as (_, storage_resp):
         usage = await storage_resp.json()
     return web.json_response(usage, status=200)
 
 
 @superadmin_required
@@ -1058,25 +1100,25 @@
         {
             t.Key("folder_host"): t.String,
             t.Key("id"): tx.UUID,
         }
     )
 )
 async def get_used_bytes(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, folder_id=params["id"])
+    entries = await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, params["id"])
     root_ctx: RootContext = request.app["_root.context"]
     proxy_name, volume_name = root_ctx.storage_manager.split_host(params["folder_host"])
     log.info("VFOLDER.GET_USED_BYTES (volume_name:{}, vf:{})", volume_name, params["id"])
     async with root_ctx.storage_manager.request(
         proxy_name,
         "GET",
         "folder/used-bytes",
         json={
             "volume": volume_name,
-            "vfid": str(params["id"]),
+            "vfid": str(VFolderID(entries[0]["quota_scope_id"], params["id"])),
         },
     ) as (_, storage_resp):
         usage = await storage_resp.json()
     return web.json_response(usage, status=200)
 
 
 @auth_required
@@ -1086,17 +1128,15 @@
     t.Dict(
         {
             t.Key("new_name"): tx.Slug(allow_dot=True),
         }
     )
 )
 async def rename_vfolder(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     old_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     domain_name = request["user"]["domain_name"]
     user_role = request["user"]["role"]
     user_uuid = request["user"]["uuid"]
     resource_policy = request["keypair"]["resource_policy"]
@@ -1155,17 +1195,15 @@
             t.Key("permission", default=None): tx.Enum(VFolderPermission) | t.Null,
         }
     )
 )
 async def update_vfolder_options(
     request: web.Request, params: Any, row: VFolderRow
 ) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     user_uuid = request["user"]["uuid"]
     domain_name = request["user"]["domain_name"]
     resource_policy = request["keypair"]["resource_policy"]
     allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
     async with root_ctx.db.begin_readonly() as conn:
         query = sa.select([vfolders.c.host]).select_from(vfolders).where(vfolders.c.id == row["id"])
@@ -1206,17 +1244,15 @@
             t.Key("path"): t.String,
             t.Key("parents", default=True): t.ToBool,
             t.Key("exist_ok", default=False): t.ToBool,
         }
     )
 )
 async def mkdir(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     log.info(
         "VFOLDER.MKDIR (email:{}, ak:{}, vf:{}, path:{})",
         request["user"]["email"],
         access_key,
@@ -1226,15 +1262,15 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(row["host"])
     async with root_ctx.storage_manager.request(
         proxy_name,
         "POST",
         "folder/file/mkdir",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID(row["quota_scope_id"], row["id"])),
             "relpath": params["path"],
             "parents": params["parents"],
             "exist_ok": params["exist_ok"],
         },
     ):
         pass
     return web.Response(status=201)
@@ -1250,17 +1286,15 @@
             t.Key("archive", default=False): t.ToBool,
         }
     )
 )
 async def create_download_session(
     request: web.Request, params: Any, row: VFolderRow
 ) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     log_fmt = "VFOLDER.CREATE_DOWNLOAD_SESSION(email:{}, ak:{}, vf:{}, path:{})"
     log_args = (
         request["user"]["email"],
         request["keypair"]["access_key"],
         row["name"],
         params["path"],
@@ -1285,15 +1319,15 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(folder_host)
     async with root_ctx.storage_manager.request(
         proxy_name,
         "POST",
         "folder/file/download",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID(row["quota_scope_id"], row["id"])),
             "relpath": params["path"],
             "archive": params["archive"],
             "unmanaged_path": unmanaged_path if unmanaged_path else None,
         },
     ) as (client_api_url, storage_resp):
         storage_reply = await storage_resp.json()
         resp = {
@@ -1311,17 +1345,15 @@
         {
             t.Key("path"): t.String,
             t.Key("size"): t.ToInt,
         }
     )
 )
 async def create_upload_session(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     log_fmt = "VFOLDER.CREATE_UPLOAD_SESSION (email:{}, ak:{}, vf:{}, path:{})"
     log_args = (request["user"]["email"], access_key, folder_name, params["path"])
     log.info(log_fmt, *log_args)
     user_uuid = request["user"]["uuid"]
@@ -1342,15 +1374,15 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(folder_host)
     async with root_ctx.storage_manager.request(
         proxy_name,
         "POST",
         "folder/file/upload",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID(row["quota_scope_id"], row["id"])),
             "relpath": params["path"],
             "size": params["size"],
         },
     ) as (client_api_url, storage_resp):
         storage_reply = await storage_resp.json()
         resp = {
             "token": storage_reply["token"],
@@ -1368,17 +1400,15 @@
             t.Key("target_path"): t.String,
             t.Key("new_name"): t.String,
             t.Key("is_dir", default=False): t.ToBool,  # ignored since 22.03
         }
     )
 )
 async def rename_file(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     user_uuid = request["user"]["uuid"]
     domain_name = request["user"]["domain_name"]
     folder_host = row["host"]
     resource_policy = request["keypair"]["resource_policy"]
@@ -1404,15 +1434,15 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(folder_host)
     async with root_ctx.storage_manager.request(
         proxy_name,
         "POST",
         "folder/file/rename",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID(row["quota_scope_id"], row["id"])),
             "relpath": params["target_path"],
             "new_name": params["new_name"],
         },
     ):
         pass
     return web.json_response({}, status=200)
 
@@ -1425,17 +1455,15 @@
         {
             t.Key("src"): t.String,
             t.Key("dst"): t.String,
         }
     )
 )
 async def move_file(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     log.info(
         "VFOLDER.MOVE_FILE (email:{}, ak:{}, vf:{}, src:{}, dst:{})",
         request["user"]["email"],
         access_key,
@@ -1446,15 +1474,15 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(row["host"])
     async with root_ctx.storage_manager.request(
         proxy_name,
         "POST",
         "folder/file/move",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID(row["quota_scope_id"], row["id"])),
             "src_relpath": params["src"],
             "dst_relpath": params["dst"],
         },
     ):
         pass
     return web.json_response({}, status=200)
 
@@ -1467,17 +1495,15 @@
         {
             t.Key("files"): t.List(t.String),
             t.Key("recursive", default=False): t.ToBool,
         }
     )
 )
 async def delete_files(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     recursive = params["recursive"]
     log.info(
         "VFOLDER.DELETE_FILES (email:{}, ak:{}, vf:{}, path:{}, recursive:{})",
         request["user"]["email"],
@@ -1489,15 +1515,15 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(row["host"])
     async with root_ctx.storage_manager.request(
         proxy_name,
         "POST",
         "folder/file/delete",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID(row["quota_scope_id"], row["id"])),
             "relpaths": params["files"],
             "recursive": recursive,
         },
     ):
         pass
     return web.json_response({}, status=200)
 
@@ -1509,17 +1535,15 @@
     t.Dict(
         {
             t.Key("path", default=""): t.String(allow_blank=True),
         }
     )
 )
 async def list_files(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.READABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     log.info(
         "VFOLDER.LIST_FILES (email:{}, ak:{}, vf:{}, path:{})",
         request["user"]["email"],
         access_key,
@@ -1529,15 +1553,15 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(row["host"])
     async with root_ctx.storage_manager.request(
         proxy_name,
         "POST",
         "folder/file/list",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID(row["quota_scope_id"], row["id"])),
             "relpath": params["path"],
         },
     ) as (_, storage_resp):
         result = await storage_resp.json()
         resp = {
             "items": [
                 {
@@ -1653,17 +1677,15 @@
         {
             tx.AliasedKey(["perm", "permission"], default="rw"): VFolderPermissionValidator,
             tx.AliasedKey(["emails", "user_ids", "userIDs"]): t.List(t.String),
         }
     ),
 )
 async def invite(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     user_uuid = request["user"]["uuid"]
     perm = params["perm"]
     invitee_emails = params["emails"]
     log.info(
@@ -1700,19 +1722,23 @@
             user_uuid=user_uuid,
             resource_policy=resource_policy,
             domain_name=domain_name,
             permission=VFolderHostPermission.INVITE_OTHERS,
         )
     async with root_ctx.db.begin() as conn:
         # Get invited user's keypairs except vfolder owner.
+        # Add filter on keypair in `ACTIVE` status
         query = (
             sa.select([keypairs.c.user_id, keypairs.c.user])
             .select_from(keypairs)
-            .where(keypairs.c.user_id.in_(invitee_emails))
-            .where(keypairs.c.user_id != request["user"]["email"])
+            .where(
+                (keypairs.c.user_id.in_(invitee_emails))
+                & (keypairs.c.user_id != request["user"]["email"])
+                & (keypairs.c.is_active.is_(True))
+            )
         )
         try:
             result = await conn.execute(query)
         except sa.exc.DataError:
             raise InvalidAPIParameters
         kps = result.fetchall()
         if len(kps) < 1:
@@ -1979,17 +2005,15 @@
         {
             t.Key("permission", default="rw"): VFolderPermissionValidator,
             t.Key("emails"): t.List(t.String),
         }
     ),
 )
 async def share(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     """
     Share a group folder to users with overriding permission.
 
     This will create vfolder_permission(s) relation directly without
     creating invitation(s). Only group-type vfolders are allowed to
     be shared directly.
     """
@@ -2041,27 +2065,31 @@
         j = users.join(agus, users.c.uuid == agus.c.user_id)
         query = (
             sa.select([users.c.uuid, users.c.email])
             .select_from(j)
             .where(
                 (users.c.email.in_(params["emails"]))
                 & (users.c.email != request["user"]["email"])
-                & (agus.c.group_id == vf_info["group"]),
+                & (agus.c.group_id == vf_info["group"])
+                & (users.c.status == ACTIVE_USER_STATUSES),
             )
         )
         result = await conn.execute(query)
         user_info = result.fetchall()
         users_to_share = [u["uuid"] for u in user_info]
         emails_to_share = [u["email"] for u in user_info]
         if len(user_info) < 1:
             raise ObjectNotFound(object_name="user")
         if len(user_info) < len(params["emails"]):
             users_not_in_vfolder_group = list(set(params["emails"]) - set(emails_to_share))
             raise ObjectNotFound(
-                "Some user does not belong to folder's group: ,".join(users_not_in_vfolder_group),
+                (
+                    "Some users do not belong to folder's group:"
+                    f" {','.join(users_not_in_vfolder_group)}"
+                ),
                 object_name="user",
             )
 
         # Do not share to users who have already been shared the folder.
         query = (
             sa.select([vfolder_permissions.c.user])
             .select_from(vfolder_permissions)
@@ -2107,17 +2135,15 @@
         }
     ),
 )
 async def unshare(request: web.Request, params: Any) -> web.Response:
     """
     Unshare a group folder from users.
     """
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
     folder_name = request.match_info["name"]
     log.info(
         "VFOLDER.UNSHARE (email:{}, ak:{}, vf:{}, users:{})",
         request["user"]["email"],
         access_key,
@@ -2172,17 +2198,15 @@
         await conn.execute(query)
         return web.json_response({"unshared_emails": params["emails"]}, status=200)
 
 
 @auth_required
 @server_status_required(ALL_ALLOWED)
 async def delete_by_name(request: web.Request) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.DELETABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.DELETABLE, request.match_info["name"])
     root_ctx: RootContext = request.app["_root.context"]
     app_ctx: PrivateContext = request.app["folders.context"]
 
     folder_name = request.match_info["name"]
     access_key = request["keypair"]["access_key"]
     domain_name = request["user"]["domain_name"]
     user_role = request["user"]["role"]
@@ -2225,15 +2249,15 @@
                 [entry["host"] for entry in entries],
             )
             raise TooManyVFoldersFound(
                 extra_msg="Multiple folders with the same name.",
                 extra_data=None,
             )
         elif len(entries) == 0:
-            raise InvalidAPIParameters("No such vfolder.")
+            raise VFolderNotFound(extra_data=folder_name)
         # query_accesible_vfolders returns list
         entry = entries[0]
         folder_host = entry["host"]
         await ensure_host_permission_allowed(
             conn,
             folder_host,
             allowed_vfolder_types=allowed_vfolder_types,
@@ -2267,17 +2291,15 @@
 )
 async def leave(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
     """
     Leave a shared vfolder.
 
     Cannot leave a group vfolder or a vfolder that the requesting user owns.
     """
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     if row["ownership_type"] == VFolderOwnershipType.GROUP:
         raise InvalidAPIParameters("Cannot leave a group vfolder.")
 
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
     user_role = request["user"]["role"]
     rqst_user_uuid = request["user"]["uuid"]
@@ -2325,17 +2347,15 @@
             t.Key("target_host", default=None) >> "folder_host": t.String | t.Null,
             t.Key("usage_mode", default="general"): tx.Enum(VFolderUsageMode) | t.Null,
             t.Key("permission", default="rw"): tx.Enum(VFolderPermission) | t.Null,
         }
     ),
 )
 async def clone(request: web.Request, params: Any, row: VFolderRow) -> web.Response:
-    await ensure_vfolder_status(
-        request, VFolderAccessStatus.UPDATABLE, folder_name=request.match_info["name"]
-    )
+    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, request.match_info["name"])
     resp: Dict[str, Any] = {}
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
     user_role = request["user"]["role"]
     user_uuid = request["user"]["uuid"]
     resource_policy = request["keypair"]["resource_policy"]
     domain_name = request["user"]["domain_name"]
@@ -2346,16 +2366,17 @@
         row["name"],
         params["target_name"],
         params["folder_host"],
         params["usage_mode"].value,
         params["permission"].value,
     )
     source_folder_host = row["host"]
-    source_folder_id = row["id"]
+    source_folder_id = VFolderID(row["quota_scope_id"], row["id"])
     target_folder_host = params["folder_host"]
+    target_quota_scope_id = "..."  # TODO: implement
     source_proxy_name, source_volume_name = root_ctx.storage_manager.split_host(source_folder_host)
     target_proxy_name, target_volume_name = root_ctx.storage_manager.split_host(target_folder_host)
 
     # check if the source vfolder is allowed to be cloned
     if not row["cloneable"]:
         raise GenericForbidden("The source vfolder is not permitted to be cloned.")
 
@@ -2363,20 +2384,14 @@
         target_folder_host = await root_ctx.shared_config.etcd.get("volumes/default_host")
         if not target_folder_host:
             raise InvalidAPIParameters(
                 "You must specify the vfolder host because the default host is not configured."
             )
 
     allowed_vfolder_types = await root_ctx.shared_config.get_vfolder_types()
-    for vf_type in allowed_vfolder_types:
-        if vf_type not in ("user", "group"):
-            raise ServerMisconfiguredError(
-                f"Invalid vfolder type(s): {str(allowed_vfolder_types)}."
-                ' Only "user" or "group" is allowed.'
-            )
 
     if not verify_vfolder_name(params["target_name"]):
         raise InvalidAPIParameters(f'{params["target_name"]} is reserved for internal operations.')
 
     if source_proxy_name != target_proxy_name:
         raise InvalidAPIParameters("proxy name of source and target vfolders must be equal.")
 
@@ -2432,14 +2447,15 @@
     task_id, target_folder_id = await initiate_vfolder_clone(
         root_ctx.db,
         VFolderCloneInfo(
             source_folder_id,
             source_folder_host,
             params["target_name"],
             target_folder_host,
+            target_quota_scope_id,
             params["usage_mode"],
             params["permission"],
             request["user"]["email"],
             user_uuid,
             params["cloneable"],
         ),
         root_ctx.storage_manager,
@@ -2986,15 +3002,15 @@
                 continue
             resp["agents"][result[0]] = result[1]
 
     return web.json_response(resp, status=200)
 
 
 async def storage_task_exception_handler(
-    exc_type: Type[Exception],
+    exc_type: type[Exception],
     exc_obj: Exception,
     tb: TracebackType,
 ):
     log.exception("Error while removing vFolder", exc_info=exc_obj)
 
 
 @superadmin_required
@@ -3059,15 +3075,15 @@
     if folder_host not in allowed_hosts_by_user:
         raise VFolderOperationFailed("User to migrate vfolder needs an access to the storage host.")
 
     async def _update() -> None:
         async with root_ctx.db.begin() as conn:
             # TODO: we need to implement migration from project to other project
             #       for now we only support migration btw user folder only
-            #
+            # TODO: implement quota-scope migration and progress checks
             query = (
                 sa.update(vfolders)
                 .values(user=user_info.uuid)
                 .where(
                     (vfolders.c.id == vfolder_id)
                     & (vfolders.c.ownership_type == VFolderOwnershipType.USER)
                 )
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-23.3.5/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/context.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/dbschema.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/dbschema.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/gql.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/image.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-23.3.5/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/config.py` & `backend.ai-manager-23.3.5/ai/backend/manager/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,18 +118,17 @@
        + overlay
          - mtu: 1500  # Maximum Transmission Unit
        + rpc
          - keepalive-timeout: 60  # seconds
      + watcher
        - token: {some-secret}
    + volumes
-     # pre-20.09
-     - _mount: {path-to-mount-root-for-vfolder-partitions}
-     - _default_host: {default-vfolder-partition-name}
-     - _fsprefix: {path-prefix-inside-host-mounts}
+     - _types     # allowed vfolder types
+       + "user"   # enabled if present
+       + "group"  # enabled if present
      # 20.09 and later
      - default_host: "{default-proxy}:{default-volume}"
      + proxies:   # each proxy may provide multiple volumes
        + "local"  # proxy name
          - client_api: "http://localhost:6021"
          - manager_api: "http://localhost:6022"
          - secret: "xxxxxx..."       # for manager API
@@ -211,22 +210,14 @@
 
 _max_cpu_count = os.cpu_count()
 _file_perm = (Path(__file__).parent / "server.py").stat()
 
 DEFAULT_CHUNK_SIZE: Final = 256 * 1024  # 256 KiB
 DEFAULT_INFLIGHT_CHUNKS: Final = 8
 
-shared_config_defaults = {
-    "volumes/_mount": "/mnt",
-    "volumes/_default_host": "local",
-    "volumes/_fsprefix": "/",
-    "config/api/allow-origins": "*",
-    "config/docker/image/auto_pull": "digest",
-}
-
 current_vfolder_types: ContextVar[List[str]] = ContextVar("current_vfolder_types")
 
 manager_local_config_iv = (
     t.Dict(
         {
             t.Key("db"): t.Dict(
                 {
@@ -297,33 +288,39 @@
             ).allow_extra("*"),
         }
     )
     .merge(config.etcd_config_iv)
     .allow_extra("*")
 )
 
-_shdefs: Mapping[str, Any] = {
+_config_defaults: Mapping[str, Any] = {
     "system": {
         "timezone": "UTC",
     },
     "api": {
         "allow-origins": "*",
     },
     "redis": {
         "addr": "127.0.0.1:6379",
         "password": None,
     },
     "docker": {
         "registry": {},
+        "image": {
+            "auto_pull": "digest",
+        },
     },
     "network": {
         "subnet": {
             "agent": "0.0.0.0/0",
             "container": "0.0.0.0/0",
         },
+        "overlay": {
+            "mtu": "1500",
+        },
     },
     "plugins": {
         "accelerator": {},
         "scheduler": {},
     },
     "watcher": {
         "token": None,
@@ -339,100 +336,127 @@
         t.Key("project", default=None): t.Null | tx.StringList | t.List(t.String),
         t.Key("ssl-verify", default=True): t.ToBool,
     }
 ).allow_extra("*")
 
 shared_config_iv = t.Dict(
     {
-        t.Key("system", default=_shdefs["system"]): t.Dict(
+        t.Key("system", default=_config_defaults["system"]): t.Dict(
             {
-                t.Key("timezone", default=_shdefs["system"]["timezone"]): tx.TimeZone,
+                t.Key("timezone", default=_config_defaults["system"]["timezone"]): tx.TimeZone,
             }
         ).allow_extra("*"),
-        t.Key("api", default=_shdefs["api"]): t.Dict(
+        t.Key("api", default=_config_defaults["api"]): t.Dict(
             {
-                t.Key("allow-origins", default=_shdefs["api"]["allow-origins"]): t.String,
+                t.Key("allow-origins", default=_config_defaults["api"]["allow-origins"]): t.String,
             }
         ).allow_extra("*"),
-        t.Key("redis", default=_shdefs["redis"]): t.Dict(
+        t.Key("redis", default=_config_defaults["redis"]): t.Dict(
             {
-                t.Key("addr", default=_shdefs["redis"]["addr"]): t.Null | tx.HostPortPair,
+                t.Key("addr", default=_config_defaults["redis"]["addr"]): t.Null | tx.HostPortPair,
                 t.Key("sentinel", default=None): t.Null | tx.DelimiterSeperatedList(
                     tx.HostPortPair
                 ),
                 t.Key("service_name", default=None): t.Null | t.String,
-                t.Key("password", default=_shdefs["redis"]["password"]): t.Null | t.String,
+                t.Key("password", default=_config_defaults["redis"]["password"]): t.Null | t.String,
             }
         ).allow_extra("*"),
-        t.Key("docker", default=_shdefs["docker"]): t.Dict(
+        t.Key("docker", default=_config_defaults["docker"]): t.Dict(
             {
                 t.Key("registry"): t.Mapping(t.String, container_registry_iv),
+                t.Key("image", default=_config_defaults["docker"]["image"]): t.Dict(
+                    {
+                        t.Key(
+                            "auto_pull", default=_config_defaults["docker"]["image"]["auto_pull"]
+                        ): t.Enum("digest", "tag", "none"),
+                    }
+                ).allow_extra("*"),
             }
         ).allow_extra("*"),
-        t.Key("plugins", default=_shdefs["plugins"]): t.Dict(
+        t.Key("plugins", default=_config_defaults["plugins"]): t.Dict(
             {
-                t.Key("accelerator", default=_shdefs["plugins"]["accelerator"]): t.Mapping(
+                t.Key("accelerator", default=_config_defaults["plugins"]["accelerator"]): t.Mapping(
                     t.String, t.Mapping(t.String, t.Any)
                 ),
-                t.Key("scheduler", default=_shdefs["plugins"]["scheduler"]): t.Mapping(
+                t.Key("scheduler", default=_config_defaults["plugins"]["scheduler"]): t.Mapping(
                     t.String, t.Mapping(t.String, t.Any)
                 ),
             }
         ).allow_extra("*"),
-        t.Key("network", default=_shdefs["network"]): t.Dict(
+        t.Key("network", default=_config_defaults["network"]): t.Dict(
             {
-                t.Key("subnet", default=_shdefs["network"]["subnet"]): t.Dict(
+                t.Key("subnet", default=_config_defaults["network"]["subnet"]): t.Dict(
                     {
-                        t.Key("agent", default=_shdefs["network"]["subnet"]["agent"]): tx.IPNetwork,
                         t.Key(
-                            "container", default=_shdefs["network"]["subnet"]["container"]
+                            "agent", default=_config_defaults["network"]["subnet"]["agent"]
+                        ): tx.IPNetwork,
+                        t.Key(
+                            "container", default=_config_defaults["network"]["subnet"]["container"]
                         ): tx.IPNetwork,
                     }
                 ).allow_extra("*"),
-                t.Key("overlay", default=None): t.Null | t.Dict(
+                t.Key("overlay", default=_config_defaults["network"]["overlay"]): t.Null | t.Dict(
                     {
-                        t.Key("mtu", default=1500): t.Int[1:],
+                        t.Key(
+                            "mtu", default=_config_defaults["network"]["overlay"]["mtu"]
+                        ): t.ToInt(gte=1),
                     }
                 ).allow_extra("*"),
             }
         ).allow_extra("*"),
-        t.Key("watcher", default=_shdefs["watcher"]): t.Dict(
+        t.Key("watcher", default=_config_defaults["watcher"]): t.Dict(
             {
-                t.Key("token", default=_shdefs["watcher"]["token"]): t.Null | t.String,
+                t.Key("token", default=_config_defaults["watcher"]["token"]): t.Null | t.String,
             }
         ).allow_extra("*"),
         t.Key("auth", default=None): (
             t.Dict(
                 {
                     t.Key("max_password_age", default=None): t.Null | tx.TimeDuration(),
                 }
             ).allow_extra("*")
             | t.Null
         ),
     }
 ).allow_extra("*")
 
+_volume_defaults: dict[str, Any] = {
+    "_types": {
+        "user": {},
+    },
+}
+
 volume_config_iv = t.Dict(
     {
+        t.Key("_types", default=_volume_defaults["_types"]): t.Dict(
+            {
+                t.Key("user", optional=True): t.String(allow_blank=True) | t.Dict({}).allow_extra(
+                    "*"
+                ),
+                t.Key("group", optional=True): t.String(allow_blank=True) | t.Dict({}).allow_extra(
+                    "*"
+                ),
+            }
+        ).allow_extra("*"),
         t.Key("default_host"): t.String,
+        t.Key("exposed_volume_info", default="percentage"): tx.StringList(delimiter=","),
         t.Key("proxies"): t.Mapping(
             tx.Slug,
             t.Dict(
                 {
                     t.Key("client_api"): t.String,
                     t.Key("manager_api"): t.String,
                     t.Key("secret"): t.String,
                     t.Key("ssl_verify"): t.ToBool,
                     t.Key("sftp_scaling_groups", default=None): t.Null | tx.StringList(
                         delimiter=","
                     ),
                 }
             ),
         ),
-        t.Key("exposed_volume_info", default="percentage"): tx.StringList(delimiter=","),
     }
 ).allow_extra("*")
 
 
 ConfigWatchCallback = Callable[[Sequence[str]], Awaitable[None]]
 
 
@@ -555,16 +579,14 @@
     def __hash__(self) -> int:
         # When used as a key in dicts, we don't care our contents.
         # Just treat it lke an opaque object.
         return hash(id(self))
 
     async def get_raw(self, key: str, allow_null: bool = True) -> Optional[str]:
         value = await self.etcd.get(key)
-        if value is None:
-            value = shared_config_defaults.get(key, None)
         if not allow_null and value is None:
             raise ServerMisconfiguredError("A required etcd config is missing.", key)
         return value
 
     async def register_myself(self) -> None:
         instance_id = await get_instance_id()
         manager_info = {
@@ -618,16 +640,14 @@
         Returns the vfolder types currently set. One of "user" and/or "group".
         If none is specified, "user" type is implicitly assumed.
         """
         try:
             ret = current_vfolder_types.get()
         except LookupError:
             vf_types = await self._get_vfolder_types()
-            if not vf_types:
-                vf_types = {"user": ""}
             ret = list(vf_types.keys())
             current_vfolder_types.set(ret)
         return ret
 
     @aiotools.lru_cache(maxsize=1, expire_after=5.0)
     async def get_manager_nodes_info(self):
         return await self.etcd.get_prefix_dict("nodes/manager")
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-23.3.5/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-23.3.5/ai/backend/manager/container_registry/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-23.3.5/ai/backend/manager/container_registry/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/container_registry/harbor.py` & `backend.ai-manager-23.3.5/ai/backend/manager/container_registry/harbor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-23.3.5/ai/backend/manager/container_registry/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             items = await response.json()
             if (reporter := self.reporter.get()) is not None:
                 reporter.total_progress = len(items)
             for item in items:
                 labels = item["Labels"]
                 if not labels:
                     continue
-                if "ai.backend.kernelspec" in labels:
+                if "ai.backend.kernelspec" in labels and item["RepoTags"] is not None:
                     for image_ref_str in item["RepoTags"]:
                         if image_ref_str == "<none>:<none>":
                             # cache images
                             continue
                         yield image_ref_str  # this includes the tag part
 
     async def _scan_image(
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/defs.py` & `backend.ai-manager-23.3.5/ai/backend/manager/defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,9 +70,10 @@
 # To be used with PostgreSQL advisory locks, the values are defined as integers.
 class LockID(enum.IntEnum):
     LOCKID_TEST = 42
     LOCKID_SCHEDULE = 91
     LOCKID_PREPARE = 92
     LOCKID_SCHEDULE_TIMER = 191
     LOCKID_PREPARE_TIMER = 192
+    LOCKID_SCALE_TIMER = 193
     LOCKID_LOG_CLEANUP_TIMER = 195
     LOCKID_IDLE_CHECK_TIMER = 196
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/exceptions.py` & `backend.ai-manager-23.3.5/ai/backend/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/idle.py` & `backend.ai-manager-23.3.5/ai/backend/manager/idle.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,23 @@
         baseline = idle_baseline
     else:
         baseline = max(idle_baseline, grace_period_end)
     remaining = baseline - now + timeout_period
     return remaining.total_seconds()
 
 
+async def get_redis_now(redis_obj: RedisConnectionInfo) -> float:
+    t = await redis_helper.execute(redis_obj, lambda r: r.time())
+    return t[0] + (t[1] / (10**6))
+
+
+async def get_db_now(dbconn: SAConnection) -> datetime:
+    return await dbconn.scalar(sa.select(sa.func.now()))
+
+
 class UtilizationExtraInfo(NamedTuple):
     avg_util: float
     threshold: float
 
 
 class UtilizationResourceReport(UserDict):
     __slots__ = ("data",)
@@ -251,15 +260,17 @@
                         kernels.c.occupied_slots,
                         kernels.c.cluster_size,
                         users.c.created_at.label("user_created_at"),
                     ]
                 )
                 .select_from(j)
                 .where(
-                    (kernels.c.status.in_(LIVE_STATUS)) & (kernels.c.cluster_role == DEFAULT_ROLE),
+                    (kernels.c.status.in_(LIVE_STATUS))
+                    & (kernels.c.cluster_role == DEFAULT_ROLE)
+                    & (kernels.c.session_type != SessionTypes.INFERENCE),
                 )
             )
             result = await conn.execute(query)
             rows = result.fetchall()
             for kernel in rows:
                 grace_period_end = await self._grace_period_checker.get_grace_period_end(kernel)
                 policy = policy_cache.get(kernel["access_key"], None)
@@ -515,16 +526,16 @@
         self,
         event_dispatcher: EventDispatcher,
         redis_live: RedisConnectionInfo,
         redis_stat: RedisConnectionInfo,
     ) -> None:
         super().__init__(event_dispatcher, redis_live, redis_stat)
         d = self._event_dispatcher
+        d.subscribe(SessionStartedEvent, None, self._session_started_cb),  # type: ignore
         self._evhandlers = [
-            d.consume(SessionStartedEvent, None, self._session_started_cb),  # type: ignore
             d.consume(ExecutionStartedEvent, None, self._execution_started_cb),  # type: ignore
             d.consume(ExecutionFinishedEvent, None, self._execution_exited_cb),  # type: ignore
             d.consume(ExecutionTimeoutEvent, None, self._execution_exited_cb),  # type: ignore
             d.consume(ExecutionCancelledEvent, None, self._execution_exited_cb),  # type: ignore
         ]
 
     async def aclose(self) -> None:
@@ -575,14 +586,15 @@
 
     async def _session_started_cb(
         self,
         context: None,
         source: AgentId,
         event: SessionStartedEvent,
     ) -> None:
+        log.debug("Got SessionStartedEvent")
         await self._update_timeout(event.session_id)
 
     async def _execution_started_cb(
         self,
         context: None,
         source: AgentId,
         event: ExecutionStartedEvent,
@@ -624,16 +636,15 @@
                 f"session.{session_id}.active_app_connections",
                 float("-inf"),
                 float("+inf"),
             ),
         )
         if active_streams is not None and active_streams > 0:
             return True
-        t = await redis_helper.execute(self._redis_live, lambda r: r.time())
-        now: float = t[0] + (t[1] / (10**6))
+        now: float = await get_redis_now(self._redis_live)
         raw_last_access = await redis_helper.execute(
             self._redis_live,
             lambda r: r.get(f"session.{session_id}.last_access"),
         )
         if raw_last_access is None or raw_last_access == "0":
             return True
         last_access = float(raw_last_access)
@@ -696,15 +707,15 @@
         """
 
         session_id = kernel["session_id"]
         if (max_session_lifetime := policy["max_session_lifetime"]) > 0:
             # TODO: once per-status time tracking is implemented, let's change created_at
             #       to the timestamp when the session entered PREPARING status.
             idle_timeout = timedelta(seconds=max_session_lifetime)
-            now: datetime = await dbconn.scalar(sa.select(sa.func.now()))
+            now: datetime = await get_db_now(dbconn)
             kernel_created_at: datetime = kernel["created_at"]
             remaining = calculate_remaining_time(
                 now, kernel_created_at, idle_timeout, grace_period_end
             )
             await self.set_remaining_time_report(
                 redis_obj, session_id, remaining if remaining > 0 else IDLE_TIMEOUT_VALUE
             )
@@ -848,15 +859,15 @@
         util_last_collected: float = (
             float(raw_util_last_collected) if raw_util_last_collected else 0.0
         )
         if util_now - util_last_collected < interval:
             return True
 
         # Report time remaining until the first time window is full as expire time
-        db_now: datetime = await dbconn.scalar(sa.select(sa.func.now()))
+        db_now: datetime = await get_db_now(dbconn)
         kernel_created_at: datetime = kernel["created_at"]
         if grace_period_end is not None:
             start_from = max(grace_period_end, kernel_created_at)
         else:
             start_from = kernel_created_at
         total_initial_grace_period_end = start_from + self.initial_grace_period
         remaining = calculate_remaining_time(
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/__init__.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/acl.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/agent.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import postgresql
 from sqlalchemy.sql import text
 from sqlalchemy.sql.expression import bindparam
 
-from ai.backend.manager.models import VFolderOwnershipType, VFolderPermission, VFolderUsageMode
+from ai.backend.common.types import VFolderUsageMode
+from ai.backend.manager.models import VFolderOwnershipType, VFolderPermission
 from ai.backend.manager.models.base import GUID, EnumValueType, IDColumn, convention
 
 # revision identifiers, used by Alembic.
 revision = "529113b08c2c"
 down_revision = "c481d3dc6c7d"
 branch_labels = None
 depends_on = None
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/base.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -781,14 +781,16 @@
                     raise GenericForbidden
                 user_id = client_user_id
             else:
                 raise InvalidAPIParameters("Unknown client role")
             kwargs["domain_name"] = domain_name
             if group_id is not None:
                 kwargs["group_id"] = group_id
+            if kwargs.get("project", None) is not None:
+                kwargs["project"] = group_id
             kwargs[user_key] = user_id
             return await resolve_func(executor, info, *args, **kwargs)
 
         return wrapped
 
     return wrap
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/domain.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/gql.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,14 +503,17 @@
     endpoint_list = graphene.Field(
         EndpointList,
         limit=graphene.Int(required=True),
         offset=graphene.Int(required=True),
         filter=graphene.String(),
         order=graphene.String(),
         # filters
+        domain_name=graphene.String(),
+        group_id=graphene.String(),
+        access_key=graphene.String(),
         project=graphene.UUID(),
     )
 
     routing = graphene.Field(
         Routing,
         routing_id=graphene.UUID(required=True),
     )
@@ -1451,78 +1454,115 @@
         executor: AsyncioExecutor,
         info: graphene.ResolveInfo,
     ) -> PredefinedAtomicPermission:
         graph_ctx: GraphQueryContext = info.context
         return await PredefinedAtomicPermission.load_all(graph_ctx)
 
     @staticmethod
+    @scoped_query(autofill_user=False, user_key="user_uuid")
     async def resolve_endpoint(
         executor: AsyncioExecutor,
         info: graphene.ResolveInfo,
         endpoint_id: uuid.UUID,
+        project: Optional[uuid.UUID] = None,
+        domain_name: Optional[str] = None,
+        user_uuid: Optional[uuid.UUID] = None,
     ) -> Endpoint:
         graph_ctx: GraphQueryContext = info.context
-        return await Endpoint.load_item(graph_ctx, endpoint_id=endpoint_id)
+        return await Endpoint.load_item(
+            graph_ctx,
+            endpoint_id=endpoint_id,
+            project=project,
+            domain_name=domain_name,
+            user_uuid=user_uuid,
+        )
 
     @staticmethod
+    @scoped_query(autofill_user=False, user_key="user_uuid")
     async def resolve_endpoint_list(
         executor: AsyncioExecutor,
         info: graphene.ResolveInfo,
         limit: int,
         offset: int,
         *,
         filter: Optional[str] = None,
         order: Optional[str] = None,
         project: Optional[uuid.UUID] = None,
+        domain_name: Optional[str] = None,
+        user_uuid: Optional[uuid.UUID] = None,
     ) -> EndpointList:
         total_count = await Endpoint.load_count(
             info.context,
             project=project,
+            domain_name=domain_name,
+            user_uuid=user_uuid,
         )
         endpoint_list = await Endpoint.load_slice(
             info.context,
             limit,
             offset,
             project=project,
+            domain_name=domain_name,
+            user_uuid=user_uuid,
             filter=filter,
             order=order,
         )
         return EndpointList(endpoint_list, total_count)
 
     @staticmethod
+    @scoped_query(autofill_user=False, user_key="user_uuid")
     async def resolve_routing(
         executor: AsyncioExecutor,
         info: graphene.ResolveInfo,
         routing_id: uuid.UUID,
+        project: Optional[uuid.UUID] = None,
+        domain_name: Optional[str] = None,
+        user_uuid: Optional[uuid.UUID] = None,
     ) -> Routing:
         graph_ctx: GraphQueryContext = info.context
-        return await Routing.load_item(graph_ctx, routing_id=routing_id)
+        return await Routing.load_item(
+            graph_ctx,
+            routing_id=routing_id,
+            project=project,
+            domain_name=domain_name,
+            user_uuid=user_uuid,
+        )
 
     @staticmethod
+    @scoped_query(autofill_user=False, user_key="user_uuid")
     async def resolve_routing_list(
         executor: AsyncioExecutor,
         info: graphene.ResolveInfo,
         limit: int,
         offset: int,
         *,
         filter: Optional[str] = None,
         order: Optional[str] = None,
         endpoint_id: Optional[uuid.UUID] = None,
+        project: Optional[uuid.UUID] = None,
+        domain_name: Optional[str] = None,
+        user_uuid: Optional[uuid.UUID] = None,
     ) -> RoutingList:
         total_count = await Routing.load_count(
             info.context,
             endpoint_id=endpoint_id,
+            project=project,
+            domain_name=domain_name,
+            user_uuid=user_uuid,
         )
         routing_list = await Routing.load_slice(
             info.context,
             limit,
             offset,
             endpoint_id=endpoint_id,
             filter=filter,
             order=order,
+            project=project,
+            domain_name=domain_name,
+            user_uuid=user_uuid,
         )
         return RoutingList(routing_list, total_count)
 
 
 class GQLMutationPrivilegeCheckMiddleware:
     def resolve(self, next, root, info: graphene.ResolveInfo, **args) -> Any:
         graph_ctx: GraphQueryContext = info.context
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/group.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/image.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,15 @@
         query = (
             sa.select(ImageRow)
             .where(ImageRow.name.in_(image_names))
             .options(selectinload(ImageRow.aliases))
         )
         async with graph_ctx.db.begin_readonly_session() as session:
             result = await session.execute(query)
-            return [await Image.from_row(graph_ctx, row) for row in result.scalars.all()]
+            return [await Image.from_row(graph_ctx, row) for row in result.scalars().all()]
 
     @classmethod
     async def batch_load_by_image_ref(
         cls,
         graph_ctx: GraphQueryContext,
         image_refs: Sequence[ImageRef],
     ) -> Sequence[Optional[Image]]:
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/kernel.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,36 +566,39 @@
 
     @staticmethod
     async def get_kernel(
         db: ExtendedAsyncSAEngine, kern_id: uuid.UUID, allow_stale: bool = False
     ) -> KernelRow:
         from .agent import AgentStatus
 
-        async with db.begin_readonly_session() as db_sess:
-            query = (
-                sa.select(KernelRow)
-                .where(KernelRow.id == kern_id)
-                .options(
-                    noload("*"),
-                    selectinload(KernelRow.agent_row).options(noload("*")),
+        async def _query():
+            async with db.begin_readonly_session() as db_sess:
+                query = (
+                    sa.select(KernelRow)
+                    .where(KernelRow.id == kern_id)
+                    .options(
+                        noload("*"),
+                        selectinload(KernelRow.agent_row).options(noload("*")),
+                    )
                 )
-            )
-            result = (await db_sess.execute(query)).scalars().all()
+                result = (await db_sess.execute(query)).scalars().all()
 
-            cand = result
-            if not allow_stale:
-                cand = [
-                    k
-                    for k in result
-                    if (k.status not in DEAD_KERNEL_STATUSES)
-                    and (k.agent_row.status == AgentStatus.ALIVE)
-                ]
-            if not cand:
-                raise SessionNotFound
-            return cand[0]
+                cand = result
+                if not allow_stale:
+                    cand = [
+                        k
+                        for k in result
+                        if (k.status not in DEAD_KERNEL_STATUSES)
+                        and (k.agent_row.status == AgentStatus.ALIVE)
+                    ]
+                if not cand:
+                    raise SessionNotFound
+                return cand[0]
+
+        return await execute_with_retry(_query)
 
     @classmethod
     async def set_kernel_status(
         cls,
         db: ExtendedAsyncSAEngine,
         kernel_id: KernelId,
         status: KernelStatus,
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/keypair.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/minilang/ordering.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/resource_policy.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/resource_preset.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/scaling_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     sa.Column("description", sa.String(length=512)),
     sa.Column("is_active", sa.Boolean, index=True, default=True),
     sa.Column(
         "is_public", sa.Boolean, index=True, default=True, server_default=true(), nullable=False
     ),
     sa.Column("created_at", sa.DateTime(timezone=True), server_default=sa.func.now()),
     sa.Column("wsproxy_addr", sa.String(length=1024), nullable=True),
+    sa.Column("wsproxy_api_token", sa.String(length=128), nullable=True),
     sa.Column("driver", sa.String(length=64), nullable=False),
     sa.Column("driver_opts", pgsql.JSONB(), nullable=False, default={}),
     sa.Column("scheduler", sa.String(length=64), nullable=False),
     sa.Column("use_host_network", sa.Boolean, nullable=False, default=False),
     sa.Column(
         "scheduler_opts",
         StructuredJSONObjectColumn(ScalingGroupOpts),
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/session.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,27 +460,30 @@
         query = query.options(*eager_loading_op)
 
     return query
 
 
 async def _match_sessions_by_id(
     db_session: SASession,
-    session_id: SessionId,
+    session_id_or_list: SessionId | list[SessionId],
     access_key: AccessKey | None = None,
     *,
     allow_prefix: bool = False,
     allow_stale: bool = True,
     for_update: bool = False,
     max_matches: Optional[int] = None,
     eager_loading_op: Optional[Sequence] = None,
 ) -> List[SessionRow]:
-    if allow_prefix:
-        cond = sa.sql.expression.cast(SessionRow.id, sa.String).like(f"{session_id}%")
+    if isinstance(session_id_or_list, list):
+        cond = SessionRow.id.in_(session_id_or_list)
     else:
-        cond = SessionRow.id == session_id
+        if allow_prefix:
+            cond = sa.sql.expression.cast(SessionRow.id, sa.String).like(f"{session_id_or_list}%")
+        else:
+            cond = SessionRow.id == session_id_or_list
     query = _build_session_fetch_query(
         cond,
         access_key,
         max_matches=max_matches,
         allow_stale=allow_stale,
         for_update=for_update,
         eager_loading_op=eager_loading_op,
@@ -663,14 +666,16 @@
         index=True,
     )
 
     # Resource metrics measured upon termination
     num_queries = sa.Column("num_queries", sa.BigInteger(), default=0)
     last_stat = sa.Column("last_stat", pgsql.JSONB(), nullable=True, default=sa.null())
 
+    routing = relationship("RoutingRow", back_populates="session_row")
+
     __table_args__ = (
         # indexing
         sa.Index(
             "ix_sessions_updated_order",
             sa.func.greatest(
                 "created_at",
                 "terminated_at",
@@ -839,58 +844,67 @@
 
         await execute_with_retry(_update)
 
     @classmethod
     async def match_sessions(
         cls,
         db_session: SASession,
-        session_name_or_id: Union[str, UUID],
+        session_reference: str | UUID | list[UUID],
         access_key: Optional[AccessKey],
         *,
         allow_prefix: bool = False,
         allow_stale: bool = True,
         for_update: bool = False,
         max_matches: int = 10,
         eager_loading_op: Optional[Sequence] = None,
     ) -> List[SessionRow]:
         """
         Match the prefix of session ID or session name among the sessions
         that belongs to the given access key, and return the list of SessionRow.
         """
 
-        query_list = [
-            aiotools.apartial(
-                _match_sessions_by_name,
-                session_name=str(session_name_or_id),
-                allow_prefix=allow_prefix,
-            )
-        ]
-        try:
-            session_id = UUID(str(session_name_or_id))
-        except ValueError:
-            pass
-        else:
-            # Fetch id-based query first
+        if isinstance(session_reference, list):
             query_list = [
                 aiotools.apartial(
                     _match_sessions_by_id,
-                    session_id=SessionId(session_id),
+                    session_id_or_list=session_reference,
                     allow_prefix=False,
-                ),
-                *query_list,
+                )
+            ]
+        else:
+            query_list = [
+                aiotools.apartial(
+                    _match_sessions_by_name,
+                    session_name=str(session_reference),
+                    allow_prefix=allow_prefix,
+                )
             ]
-            if allow_prefix:
+            try:
+                session_id = UUID(str(session_reference))
+            except ValueError:
+                pass
+            else:
+                # Fetch id-based query first
                 query_list = [
                     aiotools.apartial(
                         _match_sessions_by_id,
-                        session_id=SessionId(session_id),
-                        allow_prefix=True,
+                        session_id_or_list=SessionId(session_id),
+                        allow_prefix=False,
                     ),
                     *query_list,
                 ]
+                if allow_prefix:
+                    query_list = [
+                        aiotools.apartial(
+                            _match_sessions_by_id,
+                            session_id_or_list=SessionId(session_id),
+                            allow_prefix=True,
+                        ),
+                        *query_list,
+                    ]
 
         for fetch_func in query_list:
             rows = await fetch_func(
                 db_session,
                 access_key=access_key,
                 allow_stale=allow_stale,
                 for_update=for_update,
@@ -977,14 +991,46 @@
         )
         try:
             return session_list[0]
         except IndexError:
             raise SessionNotFound(f"Session (id={session_name_or_id}) does not exist.")
 
     @classmethod
+    async def list_sessions_with_main_kernels(
+        cls,
+        session_ids: list[UUID],
+        access_key: Optional[AccessKey] = None,
+        *,
+        allow_stale: bool = False,
+        for_update: bool = False,
+        db_session: SASession,
+    ) -> Iterable[SessionRow]:
+        kernel_rel = SessionRow.kernels
+        kernel_rel.and_(KernelRow.cluster_role == DEFAULT_ROLE)
+        kernel_loading_op = (
+            noload("*"),
+            selectinload(kernel_rel).options(
+                noload("*"),
+                selectinload(KernelRow.agent_row).noload("*"),
+            ),
+        )
+        session_list = await cls.match_sessions(
+            db_session,
+            session_ids,
+            access_key,
+            allow_stale=allow_stale,
+            for_update=for_update,
+            eager_loading_op=kernel_loading_op,
+        )
+        try:
+            return session_list
+        except IndexError:
+            raise SessionNotFound(f"Session (ids={session_ids}) does not exist.")
+
+    @classmethod
     async def get_session_with_main_kernel(
         cls,
         session_name_or_id: str | UUID,
         access_key: Optional[AccessKey] = None,
         *,
         allow_stale: bool = False,
         for_update: bool = False,
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/session_template.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/storage.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,22 @@
     Iterable,
     List,
     Mapping,
     Sequence,
     Tuple,
     TypedDict,
 )
-from uuid import UUID
 
 import aiohttp
 import attrs
 import graphene
 import yarl
 
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import HardwareMetadata
+from ai.backend.common.types import HardwareMetadata, VFolderID
 
 from ..api.exceptions import InvalidAPIParameters, VFolderOperationFailed
 from ..exceptions import InvalidArgument
 from .base import Item, PaginatedList
 
 if TYPE_CHECKING:
     from .gql import GraphQueryContext
@@ -128,15 +127,15 @@
         if proxy_name not in self._proxies:
             raise IndexError(f"proxy {proxy_name} does not exist")
         return self._proxies[proxy_name].sftp_scaling_groups or []
 
     async def get_mount_path(
         self,
         vfolder_host: str,
-        vfolder_id: UUID,
+        vfolder_id: VFolderID,
         subpath: PurePosixPath = PurePosixPath("."),
     ) -> str:
         async with self.request(
             vfolder_host,
             "GET",
             "folder/mount",
             json={
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/user.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/utils.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-23.3.5/ai/backend/manager/models/vfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 from dateutil.parser import parse as dtparse
 from graphene.types.datetime import DateTime as GQLDateTime
 from sqlalchemy.engine.row import Row
 from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
 
 from ai.backend.common.bgtask import ProgressReporter
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import VFolderHostPermission, VFolderHostPermissionMap, VFolderMount
+from ai.backend.common.types import (
+    VFolderHostPermission,
+    VFolderHostPermissionMap,
+    VFolderID,
+    VFolderMount,
+    VFolderUsageMode,
+)
 
 from ..api.exceptions import InvalidAPIParameters, VFolderNotFound, VFolderOperationFailed
 from ..defs import RESERVED_VFOLDER_PATTERNS, RESERVED_VFOLDERS, VFOLDER_DSTPATHS_MAP
 from ..types import UserScope
 from .base import (
     GUID,
     BigInt,
@@ -45,15 +51,14 @@
     from .storage import StorageSessionManager
 
 __all__: Sequence[str] = (
     "vfolders",
     "vfolder_invitations",
     "vfolder_permissions",
     "VirtualFolder",
-    "VFolderUsageMode",
     "VFolderOwnershipType",
     "VFolderInvitationState",
     "VFolderPermission",
     "VFolderPermissionValidator",
     "VFolderOperationStatus",
     "VFolderAccessStatus",
     "VFolderCloneInfo",
@@ -69,28 +74,14 @@
     "ensure_host_permission_allowed",
 )
 
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
-class VFolderUsageMode(str, enum.Enum):
-    """
-    Usage mode of virtual folder.
-
-    GENERAL: normal virtual folder
-    MODEL: virtual folder which provides shared models
-    DATA: virtual folder which provides shared data
-    """
-
-    GENERAL = "general"
-    MODEL = "model"
-    DATA = "data"
-
-
 class VFolderOwnershipType(str, enum.Enum):
     """
     Ownership type of virtual folder.
     """
 
     USER = "user"
     GROUP = "group"
@@ -146,23 +137,24 @@
 
     READABLE = "readable"
     UPDATABLE = "updatable"
     DELETABLE = "deletable"
 
 
 class VFolderDeletionInfo(NamedTuple):
-    vfolder_id: uuid.UUID
+    vfolder_id: VFolderID
     host: str
 
 
 class VFolderCloneInfo(NamedTuple):
-    source_vfolder_id: uuid.UUID
+    source_vfolder_id: VFolderID
     source_host: str
 
     # Target Vfolder infos
+    target_quota_scope_id: str
     target_vfolder_name: str
     target_host: str
     usage_mode: VFolderUsageMode
     permission: VFolderPermission
     email: str
     user_id: uuid.UUID
     cloneable: bool
@@ -170,14 +162,15 @@
 
 vfolders = sa.Table(
     "vfolders",
     metadata,
     IDColumn("id"),
     # host will be '' if vFolder is unmanaged
     sa.Column("host", sa.String(length=128), nullable=False),
+    sa.Column("quota_scope_id", sa.String(length=64), nullable=False),
     sa.Column("name", sa.String(length=64), nullable=False, index=True),
     sa.Column(
         "usage_mode",
         EnumValueType(VFolderUsageMode),
         default=VFolderUsageMode.GENERAL,
         nullable=False,
     ),
@@ -310,14 +303,15 @@
     if allowed_vfolder_types is None:
         allowed_vfolder_types = ["user"]  # legacy default
 
     vfolders_selectors = [
         vfolders.c.name,
         vfolders.c.id,
         vfolders.c.host,
+        vfolders.c.quota_scope_id,
         vfolders.c.usage_mode,
         vfolders.c.created_at,
         vfolders.c.last_used,
         vfolders.c.max_files,
         vfolders.c.max_size,
         vfolders.c.ownership_type,
         vfolders.c.user,
@@ -345,14 +339,15 @@
                 else row.vfolders_permission
             )
             entries.append(
                 {
                     "name": row.vfolders_name,
                     "id": row.vfolders_id,
                     "host": row.vfolders_host,
+                    "quota_scope_id": row.vfolders_quota_scope_id,
                     "usage_mode": row.vfolders_usage_mode,
                     "created_at": row.vfolders_created_at,
                     "last_used": row.vfolders_last_used,
                     "max_size": row.vfolders_max_size,
                     "max_files": row.vfolders_max_files,
                     "ownership_type": row.vfolders_ownership_type,
                     "user": str(row.vfolders_user) if row.vfolders_user else None,
@@ -566,21 +561,42 @@
 
 async def prepare_vfolder_mounts(
     conn: SAConnection,
     storage_manager: StorageSessionManager,
     allowed_vfolder_types: Sequence[str],
     user_scope: UserScope,
     resource_policy: Mapping[str, Any],
-    requested_mounts: Sequence[str],
-    requested_mount_map: Mapping[str, str],
+    requested_mount_references: Sequence[str | uuid.UUID],
+    requested_mount_reference_map: Mapping[str | uuid.UUID, str],
 ) -> Sequence[VFolderMount]:
     """
     Determine the actual mount information from the requested vfolder lists,
     vfolder configurations, and the given user scope.
     """
+    requested_mounts: list[str] = [
+        name for name in requested_mount_references if isinstance(name, str)
+    ]
+    requested_mount_map: dict[str, str] = {
+        name: path for name, path in requested_mount_reference_map.items() if isinstance(name, str)
+    }
+
+    vfolder_ids_to_resolve = [
+        vfid for vfid in requested_mount_references if isinstance(vfid, uuid.UUID)
+    ]
+    query = (
+        sa.select([vfolders.c.id, vfolders.c.name])
+        .select_from(vfolders)
+        .where(vfolders.c.id.in_(vfolder_ids_to_resolve))
+    )
+    result = await conn.execute(query)
+
+    for vfid, name in result.fetchall():
+        requested_mounts.append(name)
+        if path := requested_mount_reference_map.get(vfid):
+            requested_mount_map[name] = path
 
     requested_vfolder_names: dict[str, str] = {}
     requested_vfolder_subpaths: dict[str, str] = {}
     requested_vfolder_dstpaths: dict[str, str] = {}
     matched_vfolder_mounts: list[VFolderMount] = []
 
     # Split the vfolder name and subpaths
@@ -650,21 +666,21 @@
             resource_policy=resource_policy,
             domain_name=user_scope.domain_name,
             group_id=user_scope.group_id,
             permission=VFolderHostPermission.MOUNT_IN_SESSION,
         )
         if vfolder["group"] is not None and vfolder["group"] != str(user_scope.group_id):
             # User's accessible group vfolders should not be mounted
-            # if not belong to the execution kernel.
+            # if they do not belong to the execution kernel.
             continue
         try:
             mount_base_path = PurePosixPath(
                 await storage_manager.get_mount_path(
                     vfolder["host"],
-                    vfolder["id"],
+                    VFolderID(vfolder["quota_scope_id"], vfolder["id"]),
                     PurePosixPath(requested_vfolder_subpaths[key]),
                 ),
             )
         except VFolderOperationFailed as e:
             raise InvalidAPIParameters(e.extra_msg, e.extra_data) from None
         if (_vfname := vfolder["name"]) in VFOLDER_DSTPATHS_MAP:
             requested_vfolder_dstpaths[_vfname] = VFOLDER_DSTPATHS_MAP[_vfname]
@@ -672,48 +688,50 @@
             # Auto-create per-user subdirectory inside the group-owned ".local" vfolder.
             async with storage_manager.request(
                 vfolder["host"],
                 "POST",
                 "folder/file/mkdir",
                 params={
                     "volume": storage_manager.split_host(vfolder["host"])[1],
-                    "vfid": vfolder["id"],
+                    "vfid": str(VFolderID(vfolder["quota_scope_id"], vfolder["id"])),
                     "relpath": str(user_scope.user_uuid.hex),
                     "exist_ok": True,
                 },
             ):
                 pass
             # Mount the per-user subdirectory as the ".local" vfolder.
             matched_vfolder_mounts.append(
                 VFolderMount(
                     name=vfolder["name"],
-                    vfid=vfolder["id"],
+                    vfid=VFolderID(vfolder["quota_scope_id"], vfolder["id"]),
                     vfsubpath=PurePosixPath(user_scope.user_uuid.hex),
                     host_path=mount_base_path / user_scope.user_uuid.hex,
                     kernel_path=PurePosixPath("/home/work/.local"),
                     mount_perm=vfolder["permission"],
+                    usage_mode=vfolder["usage_mode"],
                 )
             )
         else:
             # Normal vfolders
             kernel_path_raw = requested_vfolder_dstpaths.get(key)
             if kernel_path_raw is None:
                 kernel_path = PurePosixPath(f"/home/work/{vfolder['name']}")
             else:
                 kernel_path = PurePosixPath(kernel_path_raw)
                 if not kernel_path.is_absolute():
                     kernel_path = PurePosixPath("/home/work", kernel_path_raw)
             matched_vfolder_mounts.append(
                 VFolderMount(
                     name=vfolder["name"],
-                    vfid=vfolder["id"],
+                    vfid=VFolderID(vfolder["quota_scope_id"], vfolder["id"]),
                     vfsubpath=PurePosixPath(requested_vfolder_subpaths[key]),
                     host_path=mount_base_path / requested_vfolder_subpaths[key],
                     kernel_path=kernel_path,
                     mount_perm=vfolder["permission"],
+                    usage_mode=vfolder["usage_mode"],
                 )
             )
 
     # Check if there are overlapping mount targets
     for vf1 in matched_vfolder_mounts:
         for vf2 in matched_vfolder_mounts:
             if vf1.name == vf2.name:
@@ -822,14 +840,15 @@
                 insert_values = {
                     "id": target_folder_id,
                     "name": vfolder_info.target_vfolder_name,
                     "usage_mode": vfolder_info.usage_mode,
                     "permission": vfolder_info.permission,
                     "last_used": None,
                     "host": vfolder_info.target_host,
+                    # TODO: add quota_scope_id
                     "creator": vfolder_info.email,
                     "ownership_type": VFolderOwnershipType("user"),
                     "user": vfolder_info.user_id,
                     "group": None,
                     "unmanaged_path": "",
                     "cloneable": vfolder_info.cloneable,
                 }
@@ -927,14 +946,15 @@
 
 
 class VirtualFolder(graphene.ObjectType):
     class Meta:
         interfaces = (Item,)
 
     host = graphene.String()
+    quota_scope_id = graphene.String()
     name = graphene.String()
     user = graphene.UUID()  # User.id (current owner, null in project vfolders)
     user_email = graphene.String()  # User.email (current owner, null in project vfolders)
     group = graphene.UUID()  # Group.id (current owner, null in user vfolders)
     group_name = graphene.String()  # Group.name (current owenr, null in user vfolders)
     creator = graphene.String()  # User.email (always set)
     unmanaged_path = graphene.String()
@@ -955,14 +975,15 @@
     @classmethod
     def from_row(cls, ctx: GraphQueryContext, row: Row) -> Optional[VirtualFolder]:
         if row is None:
             return None
         return cls(
             id=row["id"],
             host=row["host"],
+            quota_scope_id=row["quota_scope_id"],
             name=row["name"],
             user=row["user"],
             user_email=row["users_email"],
             group=row["group"],
             group_name=row["groups_name"],
             creator=row["creator"],
             unmanaged_path=row["unmanaged_path"],
@@ -982,14 +1003,15 @@
     async def resolve_num_files(self, info: graphene.ResolveInfo) -> int:
         # TODO: measure on-the-fly
         return 0
 
     _queryfilter_fieldspec = {
         "id": ("vfolders_id", uuid.UUID),
         "host": ("vfolders_host", None),
+        "quota_scope_id": ("vfolders_quota_scope_id", None),
         "name": ("vfolders_name", None),
         "group": ("vfolders_group", uuid.UUID),
         "group_name": ("groups_name", None),
         "user": ("vfolders_user", uuid.UUID),
         "user_email": ("users_email", None),
         "creator": ("vfolders_creator", None),
         "unmanaged_path": ("vfolders_unmanaged_path", None),
@@ -1003,14 +1025,15 @@
         "cloneable": ("vfolders_cloneable", None),
         "status": ("vfolders_status", lambda s: VFolderOperationStatus[s]),
     }
 
     _queryorder_colmap = {
         "id": "vfolders_id",
         "host": "vfolders_host",
+        "quota_scope_id": "vfolders_quota_scope_id",
         "name": "vfolders_name",
         "group": "vfolders_group",
         "group_name": "groups_name",
         "user": "vfolders_user",
         "user_email": "users_email",
         "creator": "vfolders_creator",
         "usage_mode": "vfolders_usage_mode",
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/pglock.py` & `backend.ai-manager-23.3.5/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-23.3.5/ai/backend/manager/plugin/error_monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-23.3.5/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/registry.py` & `backend.ai-manager-23.3.5/ai/backend/manager/registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import asyncio
+import base64
 import copy
 import itertools
 import logging
 import re
+import secrets
 import time
 import typing
 import uuid
 import zlib
 from collections import defaultdict
 from contextlib import asynccontextmanager as actxmgr
 from contextvars import ContextVar
 from datetime import datetime
 from decimal import Decimal
+from io import BytesIO
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Callable,
     Dict,
     List,
@@ -26,44 +29,63 @@
     Optional,
     Sequence,
     Tuple,
     TypeAlias,
     Union,
     cast,
 )
+from urllib.parse import urlparse
 
 import aiodocker
+import aiohttp
 import aiotools
 import sqlalchemy as sa
+import yarl
 import zmq
 from async_timeout import timeout as _timeout
 from callosum.lower.zeromq import ZeroMQAddress, ZeroMQRPCTransport
 from callosum.rpc import Peer, RPCUserError
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
+from dateutil.parser import isoparse
 from dateutil.tz import tzutc
 from redis.asyncio import Redis
 from sqlalchemy.exc import DBAPIError
+from sqlalchemy.ext.asyncio import AsyncSession
 from yarl import URL
 
 from ai.backend.common import msgpack, redis_helper
+from ai.backend.common.asyncio import cancel_tasks
 from ai.backend.common.docker import ImageRef, get_known_registries, get_registry_info
 from ai.backend.common.events import (
+    AgentHeartbeatEvent,
     AgentStartedEvent,
+    AgentTerminatedEvent,
+    DoSyncKernelLogsEvent,
+    DoTerminateSessionEvent,
     KernelCancelledEvent,
+    KernelCreatingEvent,
     KernelLifecycleEventReason,
+    KernelPreparingEvent,
+    KernelPullingEvent,
+    KernelStartedEvent,
     KernelTerminatedEvent,
     KernelTerminatingEvent,
     SessionCancelledEvent,
     SessionEnqueuedEvent,
+    SessionFailureEvent,
+    SessionPreparingEvent,
+    SessionScheduledEvent,
     SessionStartedEvent,
+    SessionSuccessEvent,
     SessionTerminatedEvent,
     SessionTerminatingEvent,
 )
+from ai.backend.common.exception import AliasResolutionFailed
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.plugin.hook import ALL_COMPLETED, PASSED, HookPluginContext
 from ai.backend.common.service_ports import parse_service_ports
 from ai.backend.common.types import (
     AbuseReport,
     AccessKey,
     AgentId,
@@ -71,65 +93,81 @@
     ClusterInfo,
     ClusterMode,
     ClusterSSHKeyPair,
     ClusterSSHPortMapping,
     CommitStatus,
     DeviceId,
     HardwareMetadata,
+    ImageAlias,
     KernelEnqueueingConfig,
     KernelId,
     RedisConnectionInfo,
     ResourceSlot,
     SessionEnqueueingConfig,
     SessionId,
     SessionTypes,
     SlotName,
     SlotTypes,
     check_typed_dict,
 )
+from ai.backend.common.utils import str_to_timedelta
+from ai.backend.manager.models.routing import RouteStatus
 
 from .api.exceptions import (
     AgentError,
     BackendError,
     GenericForbidden,
+    ImageNotFound,
     InstanceNotFound,
     InvalidAPIParameters,
     QuotaExceeded,
     RejectedByHook,
     ScalingGroupNotFound,
+    SessionAlreadyExists,
     SessionNotFound,
+    TooManySessionsMatched,
+)
+from .config import LocalConfig, SharedConfig
+from .defs import (
+    DEFAULT_IMAGE_ARCH,
+    DEFAULT_ROLE,
+    INTRINSIC_SLOTS,
+    REDIS_STREAM_DB,
 )
-from .config import SharedConfig
-from .defs import DEFAULT_ROLE, INTRINSIC_SLOTS
 from .exceptions import MultiAgentError, convert_to_status_data
 from .models import (
     AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     PRIVATE_KERNEL_ROLES,
     USER_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     AgentRow,
     AgentStatus,
+    EndpointRow,
     ImageRow,
     KernelRole,
     KernelRow,
     KernelStatus,
     KeyPairResourcePolicyRow,
     KeyPairRow,
+    RoutingRow,
     SessionDependencyRow,
     SessionRow,
     SessionStatus,
     UserRow,
     agents,
+    domains,
     handle_session_exception,
     kernels,
     prepare_dotfiles,
     prepare_vfolder_mounts,
     query_allowed_sgroups,
+    query_bootstrap_script,
     recalc_agent_resource_occupancy,
     recalc_concurrency_used,
     scaling_groups,
+    verify_vfolder_name,
 )
 from .models.utils import (
     ExtendedAsyncSAEngine,
     execute_with_retry,
     reenter_txn,
     reenter_txn_session,
     sql_json_merge,
@@ -244,28 +282,36 @@
 
     The registry is also responsible to implement our resource management
     policy, such as the limitation of maximum number of kernels per instance.
     """
 
     _kernel_actual_allocated_resources: dict[KernelId, ResourceSlot]
 
+    local_config: LocalConfig
+    session_creation_tracker: dict[str, asyncio.Event]
+    pending_waits: set[asyncio.Task[None]]
+    database_ptask_group: aiotools.PersistentTaskGroup
+    webhook_ptask_group: aiotools.PersistentTaskGroup
+
     def __init__(
         self,
+        local_config: LocalConfig,
         shared_config: SharedConfig,
         db: ExtendedAsyncSAEngine,
         redis_stat: RedisConnectionInfo,
         redis_live: RedisConnectionInfo,
         redis_image: RedisConnectionInfo,
         event_dispatcher: EventDispatcher,
         event_producer: EventProducer,
         storage_manager: StorageSessionManager,
         hook_plugin_ctx: HookPluginContext,
         *,
         debug: bool = False,
     ) -> None:
+        self.local_config = local_config
         self.shared_config = shared_config
         self.docker = aiodocker.Docker()
         self.db = db
         self.redis_stat = redis_stat
         self.redis_live = redis_live
         self.redis_image = redis_image
         self.event_dispatcher = event_dispatcher
@@ -276,17 +322,91 @@
         self.debug = debug
         self.rpc_keepalive_timeout = int(
             shared_config.get("config/network/rpc/keepalive-timeout", "60")
         )
 
     async def init(self) -> None:
         self.heartbeat_lock = asyncio.Lock()
+        self.session_creation_tracker = {}
+        self.pending_waits = set()
+        self.database_ptask_group = aiotools.PersistentTaskGroup()
+        self.webhook_ptask_group = aiotools.PersistentTaskGroup()
+
+        # passive events
+        evd = self.event_dispatcher
+        evd.consume(
+            KernelPreparingEvent, self, handle_kernel_creation_lifecycle, name="api.session.kprep"
+        )
+        evd.consume(
+            KernelPullingEvent, self, handle_kernel_creation_lifecycle, name="api.session.kpull"
+        )
+        evd.consume(
+            KernelCreatingEvent, self, handle_kernel_creation_lifecycle, name="api.session.kcreat"
+        )
+        evd.consume(
+            KernelStartedEvent, self, handle_kernel_creation_lifecycle, name="api.session.kstart"
+        )
+        evd.consume(
+            KernelCancelledEvent, self, handle_kernel_creation_lifecycle, name="api.session.kstart"
+        )
+        evd.subscribe(
+            SessionStartedEvent,
+            self,
+            handle_session_creation_lifecycle,
+            name="api.session.sstart",
+        )
+        evd.subscribe(
+            SessionCancelledEvent,
+            self,
+            handle_session_creation_lifecycle,
+            name="api.session.scancel",
+        )
+        evd.consume(
+            KernelTerminatingEvent,
+            self,
+            handle_kernel_termination_lifecycle,
+            name="api.session.kterming",
+        )
+        evd.consume(
+            KernelTerminatedEvent,
+            self,
+            handle_kernel_termination_lifecycle,
+            name="api.session.kterm",
+        )
+        evd.consume(
+            SessionTerminatingEvent,
+            self,
+            handle_session_termination_lifecycle,
+            name="api.session.sterming",
+        ),
+        evd.consume(
+            SessionTerminatedEvent,
+            self,
+            handle_session_termination_lifecycle,
+            name="api.session.sterm",
+        )
+        evd.consume(SessionEnqueuedEvent, self, invoke_session_callback)
+        evd.consume(SessionScheduledEvent, self, invoke_session_callback)
+        evd.consume(SessionPreparingEvent, self, invoke_session_callback)
+        evd.consume(SessionSuccessEvent, self, handle_batch_result)
+        evd.consume(SessionFailureEvent, self, handle_batch_result)
+        evd.consume(AgentStartedEvent, self, handle_agent_lifecycle)
+        evd.consume(AgentTerminatedEvent, self, handle_agent_lifecycle)
+        evd.consume(AgentHeartbeatEvent, self, handle_agent_heartbeat)
+
+        # action-trigerring events
+        evd.consume(DoSyncKernelLogsEvent, self, handle_kernel_log, name="api.session.syncklog")
+        evd.consume(
+            DoTerminateSessionEvent, self, handle_destroy_session, name="api.session.doterm"
+        )
 
     async def shutdown(self) -> None:
-        pass
+        await cancel_tasks(self.pending_waits)
+        await self.database_ptask_group.shutdown()
+        await self.webhook_ptask_group.shutdown()
 
     async def get_instance(self, inst_id: AgentId, field=None):
         async with self.db.begin_readonly() as conn:
             cols = [agents.c.id]
             if field is not None:
                 cols.append(field)
             query = sa.select(cols).select_from(agents).where(agents.c.id == inst_id)
@@ -336,34 +456,491 @@
             raise_for_status=True,
         ) as (_, storage_resp):
             return check_typed_dict(
                 await storage_resp.json(),
                 HardwareMetadata,  # type: ignore  # (python/mypy#9827)
             )
 
+    async def create_session(
+        self,
+        session_name: str,
+        image: str,
+        architecture: str,
+        user_scope: UserScope,
+        owner_access_key: AccessKey,
+        resource_policy: dict,
+        session_type: SessionTypes,
+        config: dict[str, Any],
+        cluster_mode: ClusterMode,
+        cluster_size: int,
+        dry_run=False,
+        reuse=False,
+        enqueue_only=False,
+        max_wait_seconds=0,
+        bootstrap_script: Optional[str] = None,
+        dependencies: Optional[List[uuid.UUID]] = None,
+        startup_command: Optional[str] = None,
+        starts_at_timestamp: Optional[str] = None,
+        tag: Optional[str] = None,
+        callback_url: Optional[yarl.URL] = None,
+        endpoint_id: Optional[uuid.UUID] = None,
+        traffic_ratio: Optional[float] = None,
+    ) -> Mapping[str, Any]:
+        log.debug("create_session():")
+        resp: MutableMapping[str, Any] = {}
+
+        current_task = asyncio.current_task()
+        assert current_task is not None
+
+        # Check work directory and reserved name directory.
+        mount_map = config.get("mount_map")
+
+        if mount_map is not None:
+            original_folders = mount_map.keys()
+            alias_folders = mount_map.values()
+            if len(alias_folders) != len(set(alias_folders)):
+                raise InvalidAPIParameters("Duplicate alias folder name exists.")
+
+            alias_name: str
+            for alias_name in alias_folders:
+                if alias_name is None:
+                    continue
+                if alias_name.startswith("/home/work/"):
+                    alias_name = alias_name.replace("/home/work/", "")
+                if alias_name == "":
+                    raise InvalidAPIParameters("Alias name cannot be empty.")
+                if not verify_vfolder_name(alias_name):
+                    raise InvalidAPIParameters(str(alias_name) + " is reserved for internal path.")
+                if alias_name in original_folders:
+                    raise InvalidAPIParameters(
+                        "Alias name cannot be set to an existing folder name: " + str(alias_name)
+                    )
+
+        # Resolve the image reference.
+        try:
+            async with self.db.begin_readonly_session() as session:
+                image_row = await ImageRow.resolve(
+                    session,
+                    [
+                        ImageRef(image, ["*"], architecture),
+                        ImageAlias(image),
+                    ],
+                )
+            requested_image_ref = image_row.image_ref
+            if not requested_image_ref.is_local:
+                async with self.db.begin_readonly() as conn:
+                    query = (
+                        sa.select([domains.c.allowed_docker_registries])
+                        .select_from(domains)
+                        .where(domains.c.name == user_scope.domain_name)
+                    )
+                    allowed_registries = await conn.scalar(query)
+                    if requested_image_ref.registry not in allowed_registries:
+                        raise AliasResolutionFailed
+        except AliasResolutionFailed:
+            raise ImageNotFound("unknown alias or disallowed registry")
+
+        # Check existing (access_key, session_name) instance
+        try:
+            # NOTE: We can reuse the session IDs of TERMINATED sessions only.
+            # NOTE: Reusing a session in the PENDING status returns an empty value in service_ports.
+            async with self.db.begin_readonly_session() as db_sess:
+                sess = await SessionRow.get_session_with_main_kernel(
+                    session_name,
+                    owner_access_key,
+                    db_session=db_sess,
+                )
+            running_image_ref = ImageRef(
+                sess.main_kernel.image, [sess.main_kernel.registry], sess.main_kernel.architecture
+            )
+            if running_image_ref != requested_image_ref:
+                # The image must be same if get_or_create() called multiple times
+                # against an existing (non-terminated) session
+                raise SessionAlreadyExists(extra_data={"existingSessionId": str(sess.id)})
+            if not reuse:
+                # Respond as error since the client did not request to reuse,
+                # but provide the overlapping session ID for later use.
+                raise SessionAlreadyExists(extra_data={"existingSessionId": str(sess.id)})
+            # Respond as success with the reused session's information.
+            return {
+                "sessionId": str(sess.id),
+                "sessionName": str(sess.name),
+                "status": sess.status.name,
+                "service_ports": sess.main_kernel.service_ports,
+                "created": False,
+            }
+        except SessionNotFound:
+            # It's time to create a new session.
+            pass
+
+        if session_type == SessionTypes.BATCH and not startup_command:
+            raise InvalidAPIParameters("Batch sessions must have a non-empty startup command.")
+        if session_type != SessionTypes.BATCH and starts_at_timestamp:
+            raise InvalidAPIParameters("Parameter starts_at should be used only for batch sessions")
+        starts_at: Union[datetime, None] = None
+        if starts_at_timestamp:
+            try:
+                starts_at = isoparse(starts_at_timestamp)
+            except ValueError:
+                _td = str_to_timedelta(starts_at_timestamp)
+                starts_at = datetime.now(tzutc()) + _td
+
+        if cluster_size > 1:
+            log.debug(" -> cluster_mode:{} (replicate)", cluster_mode)
+
+        if dependencies is None:
+            dependencies = []
+
+        session_creation_id = secrets.token_urlsafe(16)
+        start_event = asyncio.Event()
+        self.session_creation_tracker[session_creation_id] = start_event
+
+        async with self.db.begin_readonly() as conn:
+            # Use keypair bootstrap_script if it is not delivered as a parameter
+            if not bootstrap_script:
+                script, _ = await query_bootstrap_script(conn, owner_access_key)
+                bootstrap_script = script
+
+        public_sgroup_only = True
+        if _role_str := image_row.labels.get("ai.backend.role"):
+            public_sgroup_only = KernelRole(_role_str) not in PRIVATE_KERNEL_ROLES
+        if dry_run:
+            return {}
+        try:
+            session_id = await asyncio.shield(
+                self.database_ptask_group.create_task(
+                    self.enqueue_session(
+                        session_creation_id,
+                        session_name,
+                        owner_access_key,
+                        {
+                            "creation_config": config,
+                            "kernel_configs": [
+                                {
+                                    "image_ref": requested_image_ref,
+                                    "cluster_role": DEFAULT_ROLE,
+                                    "cluster_idx": 1,
+                                    "local_rank": 0,
+                                    "cluster_hostname": f"{DEFAULT_ROLE}1",
+                                    "creation_config": config,
+                                    "bootstrap_script": bootstrap_script,
+                                    "startup_command": startup_command,
+                                }
+                            ],
+                        },
+                        config["scaling_group"],
+                        session_type,
+                        resource_policy,
+                        user_scope=user_scope,
+                        cluster_mode=cluster_mode,
+                        cluster_size=cluster_size,
+                        session_tag=tag,
+                        starts_at=starts_at,
+                        agent_list=config["agent_list"],
+                        dependency_sessions=[SessionId(d) for d in dependencies],
+                        callback_url=callback_url,
+                        public_sgroup_only=public_sgroup_only,
+                        endpoint_id=endpoint_id,
+                        traffic_ratio=traffic_ratio,
+                    )
+                ),
+            )
+            resp["sessionId"] = str(session_id)  # changed since API v5
+            resp["sessionName"] = str(session_name)
+            resp["status"] = "PENDING"
+            resp["servicePorts"] = []
+            resp["created"] = True
+
+            if not enqueue_only:
+                self.pending_waits.add(current_task)
+                max_wait = max_wait_seconds
+                try:
+                    if max_wait > 0:
+                        with _timeout(max_wait):
+                            await start_event.wait()
+                    else:
+                        await start_event.wait()
+                except asyncio.TimeoutError:
+                    resp["status"] = "TIMEOUT"
+                else:
+                    await asyncio.sleep(0.5)
+                    async with self.db.begin_readonly_session() as db_sess:
+                        query = sa.select(KernelRow.status, KernelRow.service_ports).where(
+                            (KernelRow.session_id == session_id)
+                            & (KernelRow.cluster_role == DEFAULT_ROLE)
+                        )
+                        result = await db_sess.execute(query)
+                        row = result.first()
+                    if row.status == KernelStatus.RUNNING:
+                        resp["status"] = "RUNNING"
+                        for item in row.service_ports:
+                            response_dict = {
+                                "name": item["name"],
+                                "protocol": item["protocol"],
+                                "ports": item["container_ports"],
+                            }
+                            if "url_template" in item.keys():
+                                response_dict["url_template"] = item["url_template"]
+                            if "allowed_arguments" in item.keys():
+                                response_dict["allowed_arguments"] = item["allowed_arguments"]
+                            if "allowed_envs" in item.keys():
+                                response_dict["allowed_envs"] = item["allowed_envs"]
+                            resp["servicePorts"].append(response_dict)
+                    else:
+                        resp["status"] = row.status.name
+            return resp
+        except asyncio.CancelledError:
+            raise
+        finally:
+            self.pending_waits.discard(current_task)
+            if not enqueue_only and session_creation_id in self.session_creation_tracker:
+                del self.session_creation_tracker[session_creation_id]
+
+    async def create_cluster(
+        self,
+        template: Any,
+        session_name: str,
+        user_scope: UserScope,
+        owner_access_key: AccessKey,
+        resource_policy: dict,
+        scaling_group: str,
+        sess_type: SessionTypes,
+        tag: str,
+        enqueue_only=False,
+        max_wait_seconds=0,
+    ) -> Mapping[str, Any]:
+        resp: MutableMapping[str, Any] = {}
+
+        current_task = asyncio.current_task()
+        assert current_task is not None
+
+        # Check existing (access_key, session) kernel instance
+        try:
+            # NOTE: We can reuse the session IDs of TERMINATED sessions only.
+            # NOTE: Reusing a session in the PENDING status returns an empty value in service_ports.
+            async with self.db.begin_readonly_session() as db_sess:
+                await SessionRow.get_session(
+                    session_name,
+                    owner_access_key,
+                    db_session=db_sess,
+                )
+        except SessionNotFound:
+            pass
+        else:
+            raise TooManySessionsMatched
+
+        mounts = []
+        mount_map = {}
+        environ = {}
+
+        if _mounts := template["spec"].get("mounts"):  # noqa
+            mounts = list(_mounts.keys())
+            mount_map = {key: value for (key, value) in _mounts.items() if len(value) > 0}
+        if _environ := template["spec"].get("environ"):  # noqa
+            environ = _environ
+
+        kernel_configs: List[KernelEnqueueingConfig] = []
+        for node in template["spec"]["nodes"]:
+            # Resolve session template.
+            kernel_config = {
+                "image": template["spec"]["kernel"]["image"],
+                "architecture": template["spec"]["kernel"].get("architecture", DEFAULT_IMAGE_ARCH),
+                "cluster_role": node["cluster_role"],
+                "creation_config": {
+                    "mount": mounts,
+                    "mount_map": mount_map,
+                    "environ": environ,
+                },
+            }
+
+            if template["spec"]["sess_type"] == "interactive":
+                kernel_config["sess_type"] = SessionTypes.INTERACTIVE
+            elif template["spec"]["sess_type"] == "batch":
+                kernel_config["sess_type"] = SessionTypes.BATCH
+            elif template["spec"]["sess_type"] == "inference":
+                kernel_config["sess_type"] = SessionTypes.INFERENCE
+
+            if tag := template["metadata"].get("tag", None):
+                kernel_config["tag"] = tag
+            if runtime_opt := template["spec"]["kernel"]["run"]:
+                if bootstrap := runtime_opt["bootstrap"]:
+                    kernel_config["bootstrap_script"] = bootstrap
+                if startup := runtime_opt["startup_command"]:
+                    kernel_config["startup_command"] = startup
+
+            if resources := template["spec"].get("resources"):
+                kernel_config["creation_config"]["resources"] = resources
+
+            if git := template["spec"]["kernel"]["git"]:
+                if _dest := git.get("dest_dir"):
+                    target = _dest
+                else:
+                    target = git["repository"].split("/")[-1]
+
+                cmd_builder = "git clone "
+                if credential := git.get("credential"):
+                    proto, url = git["repository"].split("://")
+                    cmd_builder += (
+                        f'{proto}://{credential["username"]}:{credential["password"]}@{url}'
+                    )
+                else:
+                    cmd_builder += git["repository"]
+                if branch := git.get("branch"):
+                    cmd_builder += f" -b {branch}"
+                cmd_builder += f" {target}\n"
+
+                if commit := git.get("commit"):
+                    cmd_builder = "CWD=$(pwd)\n" + cmd_builder
+                    cmd_builder += f"cd {target}\n"
+                    cmd_builder += f"git checkout {commit}\n"
+                    cmd_builder += "cd $CWD\n"
+
+                bootstrap = base64.b64decode(kernel_config.get("bootstrap_script") or b"").decode()
+                bootstrap += "\n"
+                bootstrap += cmd_builder
+                kernel_config["bootstrap_script"] = base64.b64encode(bootstrap.encode()).decode()
+
+            # Resolve the image reference.
+            try:
+                async with self.db.begin_readonly_session() as session:
+                    image_row = await ImageRow.resolve(
+                        session,
+                        [
+                            ImageRef(kernel_config["image"], ["*"], kernel_config["architecture"]),
+                            kernel_config["image"],
+                        ],
+                    )
+                requested_image_ref = image_row.image_ref
+                async with self.db.begin_readonly() as conn:
+                    query = (
+                        sa.select([domains.c.allowed_docker_registries])
+                        .select_from(domains)
+                        .where(domains.c.name == user_scope.domain_name)
+                    )
+                    allowed_registries = await conn.scalar(query)
+                    if requested_image_ref.registry not in allowed_registries:
+                        raise AliasResolutionFailed
+                    kernel_config["image_ref"] = requested_image_ref
+            except AliasResolutionFailed:
+                raise ImageNotFound("unknown alias or disallowed registry")
+
+            for i in range(node["replicas"]):
+                kernel_config["cluster_idx"] = i + 1
+                kernel_configs.append(
+                    check_typed_dict(kernel_config, KernelEnqueueingConfig),  # type: ignore
+                )
+
+        session_creation_id = secrets.token_urlsafe(16)
+        start_event = asyncio.Event()
+        kernel_id: Optional[KernelId] = None
+        self.session_creation_tracker[session_creation_id] = start_event
+        current_task = asyncio.current_task()
+        assert current_task is not None
+
+        try:
+            session_id = await asyncio.shield(
+                self.database_ptask_group.create_task(
+                    self.enqueue_session(
+                        session_creation_id,
+                        session_name,
+                        owner_access_key,
+                        {
+                            "creation_config": {
+                                "mount_map": mount_map,
+                                "environ": environ,
+                            },
+                            "kernel_configs": kernel_configs,
+                        },
+                        scaling_group,
+                        sess_type,
+                        resource_policy,
+                        user_scope=user_scope,
+                        session_tag=tag,
+                    ),
+                )
+            )
+            kernel_id = cast(KernelId, session_id)  # the main kernel's ID is the session ID.
+            resp["kernelId"] = str(kernel_id)
+            resp["status"] = "PENDING"
+            resp["servicePorts"] = []
+            resp["created"] = True
+
+            if not enqueue_only:
+                self.pending_waits.add(current_task)
+                max_wait = max_wait_seconds
+                try:
+                    if max_wait > 0:
+                        with _timeout(max_wait):
+                            await start_event.wait()
+                    else:
+                        await start_event.wait()
+                except asyncio.TimeoutError:
+                    resp["status"] = "TIMEOUT"
+                else:
+                    await asyncio.sleep(0.5)
+                    async with self.db.begin_readonly() as conn:
+                        query = (
+                            sa.select(
+                                [
+                                    kernels.c.status,
+                                    kernels.c.service_ports,
+                                ]
+                            )
+                            .select_from(kernels)
+                            .where(kernels.c.id == kernel_id)
+                        )
+                        result = await conn.execute(query)
+                        row = result.first()
+                    if row["status"] == KernelStatus.RUNNING:
+                        resp["status"] = "RUNNING"
+                        for item in row["service_ports"]:
+                            response_dict = {
+                                "name": item["name"],
+                                "protocol": item["protocol"],
+                                "ports": item["container_ports"],
+                            }
+                            if "url_template" in item.keys():
+                                response_dict["url_template"] = item["url_template"]
+                            if "allowed_arguments" in item.keys():
+                                response_dict["allowed_arguments"] = item["allowed_arguments"]
+                            if "allowed_envs" in item.keys():
+                                response_dict["allowed_envs"] = item["allowed_envs"]
+                            resp["servicePorts"].append(response_dict)
+                    else:
+                        resp["status"] = row["status"].name
+            return resp
+        except asyncio.CancelledError:
+            raise
+        finally:
+            self.pending_waits.discard(current_task)
+            if session_creation_id in self.session_creation_tracker:
+                del self.session_creation_tracker[session_creation_id]
+
     async def enqueue_session(
         self,
         session_creation_id: str,
         session_name: str,
         access_key: AccessKey,
         session_enqueue_configs: SessionEnqueueingConfig,
         scaling_group: Optional[str],
         session_type: SessionTypes,
         resource_policy: dict,
         *,
         user_scope: UserScope,
         public_sgroup_only: bool = True,
         cluster_mode: ClusterMode = ClusterMode.SINGLE_NODE,
         cluster_size: int = 1,
-        session_tag: str = None,
-        internal_data: dict = None,
-        starts_at: datetime = None,
-        agent_list: Sequence[str] = None,
-        dependency_sessions: Sequence[SessionId] = None,
-        callback_url: URL = None,
+        session_tag: Optional[str] = None,
+        internal_data: Optional[dict] = None,
+        starts_at: Optional[datetime] = None,
+        agent_list: Optional[Sequence[str]] = None,
+        dependency_sessions: Optional[Sequence[SessionId]] = None,
+        callback_url: Optional[URL] = None,
+        endpoint_id: Optional[uuid.UUID] = None,
+        traffic_ratio: Optional[float] = None,
     ) -> SessionId:
         session_id = SessionId(uuid.uuid4())
 
         kernel_enqueue_configs: List[KernelEnqueueingConfig] = session_enqueue_configs[
             "kernel_configs"
         ]
         assert len(kernel_enqueue_configs) >= 1
@@ -562,23 +1139,21 @@
                 shmem = labels.get("ai.backend.resource.preferred.shmem", "64m")
             shmem = BinarySize.from_str(shmem)
             resource_opts["shmem"] = shmem
             image_min_slots = copy.deepcopy(image_min_slots)
             image_min_slots["mem"] += shmem
 
             # Sanitize user input: does it have resource config?
-            if "resources" in creation_config:
+            if (resources := creation_config.get("resources")) is not None:
                 # Sanitize user input: does it have "known" resource slots only?
-                for slot_key, slot_value in creation_config["resources"].items():
+                for slot_key, slot_value in resources.items():
                     if slot_key not in known_slot_types:
                         raise InvalidAPIParameters(f"Unknown requested resource slot: {slot_key}")
                 try:
-                    requested_slots = ResourceSlot.from_user_input(
-                        creation_config["resources"], known_slot_types
-                    )
+                    requested_slots = ResourceSlot.from_user_input(resources, known_slot_types)
                 except ValueError:
                     log.exception("request_slots & image_slots calculation error")
                     # happens when requested_slots have more keys
                     # than the image-defined slots
                     # (e.g., image does not support accelerators
                     #  requested by the client)
                     raise InvalidAPIParameters(
@@ -704,41 +1279,53 @@
                 async with self.db.begin_session() as db_sess:
                     session_data["requested_slots"] = session_requested_slots
                     session = SessionRow(**session_data)
                     kernels = [KernelRow(**kernel) for kernel in kernel_data]
                     db_sess.add(session)
                     db_sess.add_all(kernels)
 
-                    if not dependency_sessions:
-                        return
+            await execute_with_retry(_enqueue)
 
-                    matched_dependency_session_ids = []
-                    for dependency_id in dependency_sessions:
-                        try:
-                            match_info = await SessionRow.get_session(
-                                dependency_id,
-                                access_key,
-                                db_session=db_sess,
-                            )
-                        except SessionNotFound:
-                            raise InvalidAPIParameters(
-                                "Unknown session ID or name in the dependency list",
-                                extra_data={"session_ref": dependency_id},
-                            )
-                        else:
-                            matched_dependency_session_ids.append(match_info.id)
+            async def _post_enqueue() -> None:
+                async with self.db.begin_session() as db_sess:
+                    if endpoint_id:
+                        routing_row = RoutingRow(
+                            endpoint_id,
+                            session_id,
+                            user_scope.user_uuid,
+                            user_scope.domain_name,
+                            user_scope.group_id,
+                            traffic_ratio=traffic_ratio or 1.0,
+                        )
+                        db_sess.add(routing_row)
+
+                    if dependency_sessions:
+                        matched_dependency_session_ids = []
+                        for dependency_id in dependency_sessions:
+                            try:
+                                match_info = await SessionRow.get_session(
+                                    dependency_id,
+                                    access_key,
+                                    db_session=db_sess,
+                                )
+                            except SessionNotFound:
+                                raise InvalidAPIParameters(
+                                    "Unknown session ID or name in the dependency list",
+                                    extra_data={"session_ref": dependency_id},
+                                )
+                            else:
+                                matched_dependency_session_ids.append(match_info.id)
 
-                    dependency_rows = [
-                        SessionDependencyRow(session_id=session_id, depends_on=depend_id)
-                        for depend_id in matched_dependency_session_ids
-                    ]
-                    db_sess.add_all(dependency_rows)
-                    await db_sess.commit()
+                        dependency_rows = [
+                            SessionDependencyRow(session_id=session_id, depends_on=depend_id)
+                            for depend_id in matched_dependency_session_ids
+                        ]
+                        db_sess.add_all(dependency_rows)
 
-            await execute_with_retry(_enqueue)
+            await execute_with_retry(_post_enqueue)
         except DBAPIError as e:
             if getattr(e.orig, "pgcode", None) == "23503":
                 match = re.search(r"Key \(agent\)=\((?P<agent>[^)]+)\)", repr(e.orig))
                 if match:
                     raise InvalidAPIParameters(f"No such agent: {match.group('agent')}")
                 else:
                     raise InvalidAPIParameters("No such agent")
@@ -792,15 +1379,15 @@
                 KeyPairRow.access_key == scheduled_session.access_key
             )
             query = sa.select(KeyPairResourcePolicyRow).where(
                 KeyPairResourcePolicyRow.name == resouce_policy_q.scalar_subquery()
             )
             result = await db_sess.execute(query)
             resource_policy = result.scalars().first()
-        auto_pull = await self.shared_config.get_raw("config/docker/image/auto_pull")
+        auto_pull = self.shared_config["docker"]["image"]["auto_pull"]
 
         # Aggregate image registry information
         keyfunc = lambda item: item.kernel.image_ref
         image_infos: MutableMapping[str, ImageRow] = {}
         is_local_image = True
         registry_url = URL("http://localhost")
         registry_creds: dict[str, str] = {}
@@ -852,15 +1439,15 @@
                         log.exception(f"Failed to create an agent-local network {network_name}")
                         raise
                 else:
                     network_name = None
             elif scheduled_session.cluster_mode == ClusterMode.MULTI_NODE:
                 # Create overlay network for multi-node sessions
                 network_name = f"bai-multinode-{scheduled_session.id}"
-                mtu = await self.shared_config.get_raw("config/network/overlay/mtu")
+                mtu = self.shared_config["network"]["overlay"]["mtu"]
                 try:
                     # Overlay networks can only be created at the Swarm manager.
                     create_options = {
                         "Name": network_name,
                         "Driver": "overlay",
                         "Attachable": True,
                         "Labels": {
@@ -1050,14 +1637,19 @@
 
             new_session_status = await SessionRow.transit_session_status(self.db, session_id)
             if new_session_status is None or new_session_status != SessionStatus.RUNNING:
                 return
 
             updated_session = await SessionRow.get_session_to_produce_event(self.db, session_id)
 
+            log.debug(
+                "Producing SessionStartedEvent({}, {})",
+                updated_session.id,
+                updated_session.creation_id,
+            )
             await self.event_producer.produce_event(
                 SessionStartedEvent(updated_session.id, updated_session.creation_id),
             )
             await self.hook_plugin_ctx.notify(
                 "POST_START_SESSION",
                 (
                     updated_session.id,
@@ -1625,15 +2217,15 @@
                                     SessionStatus.CANCELLED,
                                     reason=reason,
                                     status_changed_at=now,
                                 )
                                 await self.event_producer.produce_event(
                                     SessionCancelledEvent(
                                         session_id,
-                                        kernel.session_creation_id,
+                                        target_session.creation_id,
                                         reason,
                                     ),
                                 )
                         case KernelStatus.PULLING:
                             raise GenericForbidden("Cannot destroy kernels in pulling status")
                         case KernelStatus.SCHEDULED | KernelStatus.PREPARING | KernelStatus.TERMINATING | KernelStatus.ERROR:
                             if not forced:
@@ -2664,14 +3256,365 @@
         if abusing_report is None or (result := abusing_report.get(kern_id)) is None:
             return None
         return {
             "kernel": kern_id,
             "abuse_report": result,
         }
 
+    async def update_appproxy_endpoint_routes(
+        self, db_sess: AsyncSession, endpoint: EndpointRow
+    ) -> None:
+        active_routes = [r for r in endpoint.routings if r.status == RouteStatus.HEALTHY]
+
+        target_sessions = await SessionRow.list_sessions_with_main_kernels(
+            [r.session for r in active_routes],
+            db_session=db_sess,
+        )
+        query = (
+            sa.select([scaling_groups.c.wsproxy_addr, scaling_groups.c.wsproxy_api_token])
+            .select_from(scaling_groups)
+            .where((scaling_groups.c.name == endpoint.resource_group))
+        )
+
+        result = await db_sess.execute(query)
+        sgroup = result.first()
+        wsproxy_addr = sgroup["wsproxy_addr"]
+        wsproxy_api_token = sgroup["wsproxy_api_token"]
+
+        session_id_to_route_map = {r.session: r for r in active_routes}
+        inference_apps: defaultdict[str, list[dict[str, str]]] = defaultdict(list)
+        for target_session in target_sessions:
+            if target_session.main_kernel.kernel_host is None:
+                kernel_host = urlparse(target_session.main_kernel.agent_addr).hostname
+            else:
+                kernel_host = target_session.main_kernel.kernel_host
+            assert kernel_host is not None
+            for port_info in target_session.main_kernel.service_ports:
+                if not port_info["is_inference"]:
+                    continue
+                inference_apps[port_info["name"]].append(
+                    {
+                        "session_id": str(target_session.id),
+                        "kernel_host": kernel_host,
+                        "kernel_port": port_info["host_ports"][0],
+                        "traffic_ratio": session_id_to_route_map[target_session.id].traffic_ratio,
+                    }
+                )
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(
+                f"{wsproxy_addr}/v2/endpoints/{endpoint.id}",
+                json={
+                    "service_name": endpoint.name,
+                    "apps": inference_apps,
+                    "open_to_public": endpoint.open_to_public,
+                },  # TODO: support for multiple inference apps
+                headers={
+                    "X-BackendAI-Token": wsproxy_api_token,
+                },
+            ) as resp:
+                endpoint_json = await resp.json()
+                log.debug("resp: {}", endpoint_json)
+                async with self.db.begin_session() as db_sess:
+                    query = (
+                        sa.update(EndpointRow)
+                        .values({"url": endpoint_json["endpoint"]})
+                        .where(EndpointRow.id == endpoint.id)
+                    )
+                    await db_sess.execute(query)
+
+    async def delete_appproxy_endpoint(self, db_sess: AsyncSession, endpoint: EndpointRow) -> None:
+        query = (
+            sa.select([scaling_groups.c.wsproxy_addr, scaling_groups.c.wsproxy_api_token])
+            .select_from(scaling_groups)
+            .where((scaling_groups.c.name == endpoint.resource_group))
+        )
+
+        result = await db_sess.execute(query)
+        sgroup = result.first()
+        wsproxy_addr = sgroup["wsproxy_addr"]
+        wsproxy_api_token = sgroup["wsproxy_api_token"]
+
+        async with aiohttp.ClientSession() as session:
+            async with session.delete(
+                f"{wsproxy_addr}/v2/endpoints/{endpoint.id}",
+                headers={
+                    "X-BackendAI-Token": wsproxy_api_token,
+                },
+            ):
+                pass
+
+
+async def handle_kernel_creation_lifecycle(
+    context: AgentRegistry,
+    source: AgentId,
+    event: (
+        KernelPreparingEvent
+        | KernelPullingEvent
+        | KernelCreatingEvent
+        | KernelStartedEvent
+        | KernelCancelledEvent
+    ),
+) -> None:
+    """
+    Update the database and perform post_create_kernel() upon
+    the events for each step of kernel creation.
+
+    To avoid race condition between consumer and subscriber event handlers,
+    we only have this handler to subscribe all kernel creation events,
+    but distinguish which one to process using a unique creation_id
+    generated when initiating the create_kernels() agent RPC call.
+    """
+    log.debug(
+        "handle_kernel_creation_lifecycle: ev:{} k:{}",
+        event.name,
+        event.kernel_id,
+    )
+    if isinstance(event, KernelPreparingEvent):
+        # State transition is done by the DoPrepareEvent handler inside the scheduler-distpacher object.
+        pass
+    elif isinstance(event, KernelPullingEvent):
+        await KernelRow.set_kernel_status(
+            context.db, event.kernel_id, KernelStatus.PULLING, reason=event.reason
+        )
+        await SessionRow.set_session_status(context.db, event.session_id, SessionStatus.PULLING)
+    elif isinstance(event, KernelCreatingEvent):
+        await KernelRow.set_kernel_status(
+            context.db, event.kernel_id, KernelStatus.PREPARING, reason=event.reason
+        )
+    elif isinstance(event, KernelStartedEvent):
+        session_id = event.session_id
+        await context.finalize_running(event.kernel_id, session_id, event.creation_info)
+    elif isinstance(event, KernelCancelledEvent):
+        log.warning(f"Kernel cancelled, {event.reason = }")
+
+
+async def handle_kernel_termination_lifecycle(
+    context: AgentRegistry,
+    source: AgentId,
+    event: KernelTerminatingEvent | KernelTerminatedEvent,
+) -> None:
+    if isinstance(event, KernelTerminatingEvent):
+        # The destroy_kernel() API handler will set the "TERMINATING" status.
+        pass
+    elif isinstance(event, KernelTerminatedEvent):
+        await context.mark_kernel_terminated(event.kernel_id, event.reason, event.exit_code)
+        session_id = event.session_id
+        await context.check_session_terminated(session_id, event.reason)
+
+
+async def handle_session_creation_lifecycle(
+    context: AgentRegistry,
+    source: AgentId,
+    event: SessionStartedEvent | SessionCancelledEvent,
+) -> None:
+    """
+    Update the database according to the session-level lifecycle events
+    published by the manager.
+    """
+    if event.creation_id not in context.session_creation_tracker:
+        return
+    log.debug("handle_session_creation_lifecycle: ev:{} s:{}", event.name, event.session_id)
+    if isinstance(event, SessionStartedEvent):
+        if tracker := context.session_creation_tracker.get(event.creation_id):
+            tracker.set()
+    elif isinstance(event, SessionCancelledEvent):
+        if tracker := context.session_creation_tracker.get(event.creation_id):
+            tracker.set()
+
+    await invoke_session_callback(context, source, event)
+    if event.creation_id in context.session_creation_tracker:
+        del context.session_creation_tracker[event.creation_id]
+
+
+async def handle_session_termination_lifecycle(
+    context: AgentRegistry,
+    agent_id: AgentId,
+    event: SessionTerminatingEvent | SessionTerminatedEvent,
+) -> None:
+    """
+    Update the database according to the session-level lifecycle events
+    published by the manager.
+    """
+    if isinstance(event, SessionTerminatingEvent):
+        await context.mark_session_terminating(event.session_id, event.reason)
+    elif isinstance(event, SessionTerminatedEvent):
+        await context.mark_session_terminated(event.session_id, event.reason)
+
+    await invoke_session_callback(context, agent_id, event)
+
+
+async def handle_destroy_session(
+    context: AgentRegistry,
+    source: AgentId,
+    event: DoTerminateSessionEvent,
+) -> None:
+    async with context.db.begin_session() as db_sess:
+        session = await SessionRow.get_session_with_kernels(event.session_id, db_session=db_sess)
+    await context.destroy_session(
+        session,
+        forced=False,
+        reason=event.reason or KernelLifecycleEventReason.KILLED_BY_EVENT,
+    )
+
+
+async def invoke_session_callback(
+    context: AgentRegistry,
+    source: AgentId,
+    event: SessionEnqueuedEvent
+    | SessionScheduledEvent
+    | SessionPreparingEvent
+    | SessionStartedEvent
+    | SessionCancelledEvent
+    | SessionTerminatingEvent
+    | SessionTerminatedEvent
+    | SessionSuccessEvent
+    | SessionFailureEvent,
+) -> None:
+    log.info("INVOKE_SESSION_CALLBACK (source:{}, event:{})", source, event)
+    try:
+        allow_stale = isinstance(event, (SessionCancelledEvent, SessionTerminatedEvent))
+        async with context.db.begin_readonly_session() as db_sess:
+            session = await SessionRow.get_session_with_main_kernel(
+                event.session_id, db_session=db_sess, allow_stale=allow_stale
+            )
+    except SessionNotFound:
+        return
+
+    try:
+        # Update routing status
+        # TODO: Check session health
+        if session.session_type == SessionTypes.INFERENCE:
+
+            async def _update() -> None:
+                async with context.db.begin_session() as db_sess:
+                    route = await RoutingRow.get_by_session(db_sess, session.id, load_endpoint=True)
+                    endpoint = await EndpointRow.get(db_sess, route.endpoint, load_routes=True)
+
+                    if isinstance(event, SessionTerminatedEvent) or isinstance(
+                        event, SessionCancelledEvent
+                    ):
+                        await db_sess.delete(route)
+                        if (
+                            len(endpoint.routings) == 1
+                            and endpoint.desired_session_count < 0  # we just removed last one
+                        ):
+                            await db_sess.delete(endpoint)
+                            try:
+                                await context.delete_appproxy_endpoint(db_sess, endpoint)
+                            except aiohttp.ClientError as e:
+                                log.warn("failed to communicate with AppProxy endpoint: {}", str(e))
+                        else:
+                            try:
+                                await context.update_appproxy_endpoint_routes(db_sess, endpoint)
+                            except aiohttp.ClientError as e:
+                                log.warn("failed to communicate with AppProxy endpoint: {}", str(e))
+                        await db_sess.commit()
+                    else:
+                        new_route_status: Optional[RouteStatus] = None
+                        if isinstance(event, SessionStartedEvent):
+                            new_route_status = RouteStatus.HEALTHY
+                        elif isinstance(event, SessionTerminatingEvent):
+                            new_route_status = RouteStatus.TERMINATING
+
+                        if new_route_status:
+                            query = (
+                                sa.update(RoutingRow)
+                                .where(RoutingRow.id == route.id)
+                                .values({"status": new_route_status})
+                            )
+                            await db_sess.execute(query)
+                            try:
+                                await context.update_appproxy_endpoint_routes(db_sess, endpoint)
+                            except aiohttp.ClientError as e:
+                                log.warn("failed to communicate with AppProxy endpoint: {}", str(e))
+
+            await execute_with_retry(_update)
+    except Exception:
+        log.exception("error while updating route status:")
+
+    if (callback_url := session.callback_url) is None:
+        return
+
+    data = {
+        "type": "session_lifecycle",
+        "event": event.name.removeprefix("session_"),
+        "session_id": str(event.session_id),
+        "when": datetime.now(tzutc()).isoformat(),
+    }
+
+    context.webhook_ptask_group.create_task(
+        _make_session_callback(data, callback_url),
+    )
+
+
+async def handle_batch_result(
+    context: AgentRegistry,
+    source: AgentId,
+    event: SessionSuccessEvent | SessionFailureEvent,
+) -> None:
+    """
+    Update the database according to the batch-job completion results
+    """
+    if isinstance(event, SessionSuccessEvent):
+        await SessionRow.set_session_result(context.db, event.session_id, True, event.exit_code)
+    elif isinstance(event, SessionFailureEvent):
+        await SessionRow.set_session_result(context.db, event.session_id, False, event.exit_code)
+    async with context.db.begin_session() as db_sess:
+        try:
+            session = await SessionRow.get_session_with_kernels(
+                event.session_id, db_session=db_sess
+            )
+        except SessionNotFound:
+            return
+    await context.destroy_session(
+        session,
+        reason=KernelLifecycleEventReason.TASK_FINISHED,
+    )
+
+    await invoke_session_callback(context, source, event)
+
+
+async def handle_agent_lifecycle(
+    context: AgentRegistry,
+    source: AgentId,
+    event: AgentStartedEvent | AgentTerminatedEvent,
+) -> None:
+    if isinstance(event, AgentStartedEvent):
+        log.info("instance_lifecycle: ag:{0} joined ({1})", source, event.reason)
+        await context.update_instance(
+            source,
+            {
+                "status": AgentStatus.ALIVE,
+            },
+        )
+    if isinstance(event, AgentTerminatedEvent):
+        if event.reason == "agent-lost":
+            await context.mark_agent_terminated(source, AgentStatus.LOST)
+        elif event.reason == "agent-restart":
+            log.info("agent@{0} restarting for maintenance.", source)
+            await context.update_instance(
+                source,
+                {
+                    "status": AgentStatus.RESTARTING,
+                },
+            )
+        else:
+            # On normal instance termination, kernel_terminated events were already
+            # triggered by the agent.
+            await context.mark_agent_terminated(source, AgentStatus.TERMINATED)
+
+
+async def handle_agent_heartbeat(
+    context: AgentRegistry,
+    source: AgentId,
+    event: AgentHeartbeatEvent,
+) -> None:
+    await context.handle_heartbeat(source, event.agent_info)
+
 
 async def check_scaling_group(
     conn: SAConnection,
     scaling_group: str | None,
     session_type: SessionTypes,
     access_key: AccessKey,
     domain_name: str,
@@ -2719,7 +3662,105 @@
                     f"The scaling group '{scaling_group}' does not accept "
                     f"the session type '{session_type}'. "
                 )
         else:
             raise ScalingGroupNotFound(err_msg)
     assert scaling_group is not None
     return scaling_group
+
+
+async def handle_kernel_log(
+    context: AgentRegistry,
+    source: AgentId,
+    event: DoSyncKernelLogsEvent,
+) -> None:
+    redis_conn = redis_helper.get_redis_object(
+        context.shared_config.data["redis"], db=REDIS_STREAM_DB
+    )
+    # The log data is at most 10 MiB.
+    log_buffer = BytesIO()
+    log_key = f"containerlog.{event.container_id}"
+    try:
+        list_size = await redis_helper.execute(
+            redis_conn,
+            lambda r: r.llen(log_key),
+        )
+        if list_size is None:
+            # The log data is expired due to a very slow event delivery.
+            # (should never happen!)
+            log.warning(
+                "tried to store console logs for cid:{}, but the data is expired",
+                event.container_id,
+            )
+            return
+        for _ in range(list_size):
+            # Read chunk-by-chunk to allow interleaving with other Redis operations.
+            chunk = await redis_helper.execute(redis_conn, lambda r: r.lpop(log_key))
+            if chunk is None:  # maybe missing
+                log_buffer.write(b"(container log unavailable)\n")
+                break
+            log_buffer.write(chunk)
+        try:
+            log_data = log_buffer.getvalue()
+
+            async def _update_log() -> None:
+                async with context.db.begin() as conn:
+                    update_query = (
+                        sa.update(kernels)
+                        .values(container_log=log_data)
+                        .where(kernels.c.id == event.kernel_id)
+                    )
+                    await conn.execute(update_query)
+
+            await execute_with_retry(_update_log)
+        finally:
+            # Clear the log data from Redis when done.
+            await redis_helper.execute(
+                redis_conn,
+                lambda r: r.delete(log_key),
+            )
+    finally:
+        log_buffer.close()
+        await redis_conn.close()
+
+
+async def _make_session_callback(data: dict[str, Any], url: yarl.URL) -> None:
+    log_func = log.info
+    log_msg: str = ""
+    log_fmt: str = ""
+    log_arg: Any = None
+    begin = time.monotonic()
+    try:
+        async with aiohttp.ClientSession(
+            timeout=aiohttp.ClientTimeout(total=30.0),
+        ) as session:
+            try:
+                async with session.post(url, json=data) as response:
+                    if response.content_length is not None and response.content_length > 0:
+                        log_func = log.warning
+                        log_msg = "warning"
+                        log_fmt = (
+                            "{3[0]} {3[1]} - the callback response body was not empty! "
+                            "(len: {3[2]:,} bytes)"
+                        )
+                        log_arg = (response.status, response.reason, response.content_length)
+                    else:
+                        log_msg = "result"
+                        log_fmt = "{3[0]} {3[1]}"
+                        log_arg = (response.status, response.reason)
+            except aiohttp.ClientError as e:
+                log_func = log.warning
+                log_msg, log_fmt, log_arg = "failed", "{3}", repr(e)
+    except asyncio.CancelledError:
+        log_func = log.warning
+        log_msg, log_fmt, log_arg = "cancelled", "elapsed_time = {3:.6f}", time.monotonic() - begin
+    except asyncio.TimeoutError:
+        log_func = log.warning
+        log_msg, log_fmt, log_arg = "timeout", "elapsed_time = {3:.6f}", time.monotonic() - begin
+    finally:
+        log_func(
+            "Session lifecycle callback " + log_msg + " (e:{0}, s:{1}, url:{2}): " + log_fmt,
+            data["event"],
+            data["session_id"],
+            url,
+            log_arg,
+        )
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-23.3.5/ai/backend/manager/scheduler/dispatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,85 @@
 from __future__ import annotations
 
 import asyncio
 import itertools
 import logging
+import uuid
 from contextvars import ContextVar
 from datetime import datetime, timedelta
 from functools import partial
-from typing import TYPE_CHECKING, Any, Awaitable, Final, List, Optional, Sequence, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Final,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import aiotools
 import async_timeout
 import sqlalchemy as sa
 from dateutil.tz import tzutc
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.ext.asyncio import AsyncSession as SASession
 from sqlalchemy.orm import noload, selectinload
 
 from ai.backend.common.distributed import GlobalTimer
 from ai.backend.common.events import (
     AgentStartedEvent,
     CoalescingOptions,
     DoPrepareEvent,
+    DoScaleEvent,
     DoScheduleEvent,
     EventDispatcher,
     EventProducer,
     KernelLifecycleEventReason,
     SessionCancelledEvent,
     SessionEnqueuedEvent,
     SessionPreparingEvent,
     SessionScheduledEvent,
     SessionTerminatedEvent,
 )
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import AgentId, ClusterMode, ResourceSlot, SessionId, aobject
+from ai.backend.common.types import (
+    AgentId,
+    ClusterMode,
+    ResourceSlot,
+    SessionId,
+    SessionTypes,
+    aobject,
+)
 from ai.backend.manager.models.agent import AgentRow
-from ai.backend.manager.types import DistributedLockFactory
+from ai.backend.manager.models.session import _build_session_fetch_query
+from ai.backend.manager.types import DistributedLockFactory, UserScope
+from ai.backend.manager.utils import query_userinfo
 from ai.backend.plugin.entrypoint import scan_entrypoints
 
 from ..api.exceptions import GenericBadRequest, InstanceNotAvailable
 from ..defs import LockID
 from ..exceptions import convert_to_status_data
 from ..models import (
     AgentStatus,
+    EndpointRow,
     KernelRow,
     KernelStatus,
+    RouteStatus,
     ScalingGroupRow,
     SessionRow,
     SessionStatus,
+    keypair_resource_policies,
+    keypairs,
     list_schedulable_agents_by_sgroup,
     recalc_agent_resource_occupancy,
     recalc_concurrency_used,
+    users,
 )
 from ..models.scaling_group import ScalingGroupOpts
 from ..models.utils import ExtendedAsyncSAEngine as SAEngine
 from ..models.utils import execute_with_retry, sql_json_increment, sql_json_merge
 from .predicates import (
     check_concurrency,
     check_dependencies,
@@ -116,14 +142,15 @@
     registry: AgentRegistry
     db: SAEngine
 
     event_dispatcher: EventDispatcher
     event_producer: EventProducer
     schedule_timer: GlobalTimer
     prepare_timer: GlobalTimer
+    scale_timer: GlobalTimer
 
     def __init__(
         self,
         local_config: LocalConfig,
         shared_config: SharedConfig,
         event_dispatcher: EventDispatcher,
         event_producer: EventProducer,
@@ -150,33 +177,43 @@
         )
         evd.consume(
             SessionTerminatedEvent, None, self.schedule, coalescing_opts, name="dispatcher.term"
         )
         evd.consume(AgentStartedEvent, None, self.schedule)
         evd.consume(DoScheduleEvent, None, self.schedule, coalescing_opts)
         evd.consume(DoPrepareEvent, None, self.prepare)
+        evd.consume(DoScaleEvent, None, self.scale_services)
         self.schedule_timer = GlobalTimer(
             self.lock_factory(LockID.LOCKID_SCHEDULE_TIMER, 10.0),
             self.event_producer,
             lambda: DoScheduleEvent(),
             interval=10.0,
         )
         self.prepare_timer = GlobalTimer(
             self.lock_factory(LockID.LOCKID_PREPARE_TIMER, 10.0),
             self.event_producer,
             lambda: DoPrepareEvent(),
             interval=10.0,
             initial_delay=5.0,
         )
+        self.scale_timer = GlobalTimer(
+            self.lock_factory(LockID.LOCKID_SCALE_TIMER, 10.0),
+            self.event_producer,
+            lambda: DoScaleEvent(),
+            interval=10.0,
+            initial_delay=7.0,
+        )
         await self.schedule_timer.join()
         await self.prepare_timer.join()
+        await self.scale_timer.join()
         log.info("Session scheduler started")
 
     async def close(self) -> None:
         async with aiotools.TaskGroup() as tg:
+            tg.create_task(self.scale_timer.leave())
             tg.create_task(self.prepare_timer.leave())
             tg.create_task(self.schedule_timer.leave())
         log.info("Session scheduler stopped")
 
     async def schedule(
         self,
         context: None,
@@ -752,15 +789,16 @@
             # including scheduling failures of a kernel.
             # It ensures that occupied_slots are recovered when there are partial
             # scheduling failures.
             kernel: KernelRow
             for kernel in sess_ctx.kernels:
                 agent_alloc_ctx: AgentAllocationContext | None = None
                 try:
-                    agent = kernel.agent_row
+                    agent_id: Optional[AgentId] = None
+                    agent: Optional[AgentRow] = kernel.agent_row
                     if agent is not None:
                         # Check the resource availability of the manually designated agent
                         query = sa.select(AgentRow.available_slots).where(AgentRow.id == agent.id)
                         available_agent_slots = (await agent_db_sess.execute(query)).scalar()
                         if available_agent_slots is None:
                             raise GenericBadRequest(f"No such agent: {agent.id}")
                         for key in available_agent_slots:
@@ -771,49 +809,50 @@
                                     extra_msg=(
                                         f"The designated agent ({agent.id}) does not have "
                                         f"the enough remaining capacity ({key}, "
                                         f"requested: {sess_ctx.requested_slots[key]}, "
                                         f"available: {available_agent_slots[key]})."
                                     ),
                                 )
+                        agent_id = agent.id
                     else:
                         # Each kernel may have different images and different architectures
                         compatible_candidate_agents = [
                             ag for ag in candidate_agents if ag.architecture == kernel.architecture
                         ]
                         if not compatible_candidate_agents:
                             raise InstanceNotAvailable(
                                 extra_msg=(
                                     "No agents found to be compatible with the image acrhitecture "
                                     f"(image: {kernel.image_ref}, "
                                     f"arch: {kernel.architecture})"
                                 ),
                             )
                         # Let the scheduler check the resource availability and decide the target agent
-                        agent = scheduler.assign_agent_for_kernel(
+                        agent_id = scheduler.assign_agent_for_kernel(
                             compatible_candidate_agents, kernel
                         )
-                        if agent is None:
+                        if agent_id is None:
                             raise InstanceNotAvailable(
                                 extra_msg=(
                                     "Could not find a contiguous resource region in any agent big"
                                     f" enough to host a kernel in the session (id: {sess_ctx.id},"
                                     f" resource group: {sess_ctx.scaling_group_name})"
                                 ),
                             )
-                    assert agent is not None
+                    assert agent_id is not None
 
                     async def _reserve() -> None:
                         nonlocal agent_alloc_ctx, candidate_agents
                         async with agent_db_sess.begin_nested():
                             agent_alloc_ctx = await _reserve_agent(
                                 sched_ctx,
                                 agent_db_sess,
                                 sgroup_name,
-                                agent.id,
+                                agent_id,
                                 kernel.requested_slots,
                                 extra_conds=agent_query_extra_conds,
                             )
                             # Update the agent data to schedule the next kernel in the session
                             candidate_agents = await list_schedulable_agents_by_sgroup(
                                 agent_db_sess,
                                 sgroup_name,
@@ -1037,14 +1076,184 @@
                     "maybe another prepare() call is still running"
                 )
                 raise asyncio.CancelledError()
             raise
         except asyncio.TimeoutError:
             log.warn("prepare(): timeout while executing start_session()")
 
+    async def scale_services(
+        self,
+        context: None,
+        source: AgentId,
+        event: DoScaleEvent,
+    ) -> None:
+        log.debug("scale_services(): triggered")
+        # Altering inference sessions should only be done by this method
+        routes_to_destroy = []
+        endpoints_to_expand: dict[EndpointRow, Any] = {}
+        async with self.db.begin_readonly_session() as session:
+            endpoints = await EndpointRow.list(session, load_image=True, load_routes=True)
+        # endpoints_to_flush = [
+        #     endpoint.id
+        #     for endpoint in endpoints
+        #     if endpoint.desired_session_count < 0 and len(endpoint.routings) == 0
+        # ]
+        # async with self.db.begin_session() as session:
+        #     query = sa.delete(EndpointRow).where(EndpointRow.id.in_(endpoints_to_flush))
+        #     await session.execute(query)
+        for endpoint in endpoints:
+            desired_session_count = endpoint.desired_session_count
+            if desired_session_count < 0:
+                desired_session_count = 0
+            if len(endpoint.routings) > desired_session_count:
+                # We need to scale down!
+                destroy_count = len(endpoint.routings) - desired_session_count
+                routes_to_destroy += list(
+                    sorted(
+                        [
+                            route
+                            for route in endpoint.routings
+                            if (
+                                route.status != RouteStatus.PROVISIONING
+                                and route.status != RouteStatus.TERMINATING
+                            )
+                        ],
+                        key=lambda r: r.status == RouteStatus.UNHEALTHY,
+                    )
+                )[:destroy_count]
+                log.debug(
+                    "Shrinking {} from {} to {}",
+                    endpoint.name,
+                    len(endpoint.routings),
+                    endpoint.desired_session_count,
+                )
+            elif len(endpoint.routings) < desired_session_count:
+                # We need to scale up!
+                create_count = desired_session_count - len(endpoint.routings)
+                endpoints_to_expand[endpoint] = create_count
+                log.debug(
+                    "Expanding {} from {} to {}",
+                    endpoint.name,
+                    len(endpoint.routings),
+                    endpoint.desired_session_count,
+                )
+
+        async with self.db.begin_readonly_session() as db_session:
+            ids_of_session_to_destroy = [r.session for r in routes_to_destroy]
+            kernel_loading_op = (
+                noload("*"),
+                selectinload(SessionRow.kernels).options(
+                    noload("*"),
+                    selectinload(KernelRow.agent_row).noload("*"),
+                ),
+            )
+            query = _build_session_fetch_query(
+                SessionRow.id.in_(ids_of_session_to_destroy), eager_loading_op=kernel_loading_op
+            )
+            result = await db_session.execute(query)
+            target_sessions_to_destory = result.scalars().all()
+        # TODO: Update logic to not to wait for sessions to actually terminate
+        for session in target_sessions_to_destory:
+            await self.registry.destroy_session(
+                session,
+                forced=False,
+                reason=KernelLifecycleEventReason.SERVICE_SCALED_DOWN,
+            )
+
+        user_ids = tuple(
+            {endpoint.created_user for endpoint in endpoints_to_expand.keys()}
+            | {endpoint.session_owner for endpoint in endpoints_to_expand.keys()}
+        )
+
+        async with self.db.begin_readonly() as conn:
+            join = sa.join(
+                users, keypairs, (users.c.uuid == keypairs.c.user) & keypairs.c.is_active.is_(True)
+            )
+            query = (
+                sa.select(
+                    [
+                        users.c.uuid,
+                        users.c.role,
+                        users.c.domain_name,
+                        keypairs.c.access_key,
+                        keypairs.c.resource_policy,
+                    ]
+                )
+                .select_from(join)
+                .where(users.c.uuid.in_(user_ids))
+            )
+            result = await conn.execute(query)
+            user_id_row_mapping = {row.uuid: row for row in result.fetchall()}
+            keypair_resource_policy_names = {
+                row.resource_policy for row in user_id_row_mapping.values()
+            }
+            query = (
+                sa.select([keypair_resource_policies])
+                .select_from(keypair_resource_policies)
+                .where(keypair_resource_policies.c.name.in_(keypair_resource_policy_names))
+            )
+            result = await conn.execute(query)
+            keypair_resource_policy_name_policy_mapping = {
+                row.name: row for row in result.fetchall()
+            }
+
+        for endpoint, expand_count in endpoints_to_expand.items():
+            log.debug("Creating {} session(s) for {}", expand_count, endpoint.name)
+            async with self.db.begin_readonly() as conn:
+                _, group_id, resource_policy = await query_userinfo(
+                    conn,
+                    user_id_row_mapping[endpoint.created_user].uuid,
+                    user_id_row_mapping[endpoint.created_user].access_key,
+                    user_id_row_mapping[endpoint.created_user].role,
+                    user_id_row_mapping[endpoint.created_user].domain_name,
+                    keypair_resource_policy_name_policy_mapping[
+                        user_id_row_mapping[endpoint.created_user].resource_policy
+                    ],
+                    endpoint.domain,
+                    endpoint.project,
+                    query_on_behalf_of=user_id_row_mapping[endpoint.session_owner]["access_key"],
+                )
+            for _ in range(expand_count):
+                try:
+                    await self.registry.create_session(
+                        f"{endpoint.name}-{uuid.uuid4()}",
+                        endpoint.image_row.name,
+                        endpoint.image_row.architecture,
+                        UserScope(
+                            domain_name=endpoint.domain,
+                            group_id=group_id,
+                            user_uuid=user_id_row_mapping[endpoint.created_user].uuid,
+                            user_role=user_id_row_mapping[endpoint.created_user].role,
+                        ),
+                        user_id_row_mapping[endpoint.session_owner]["access_key"],
+                        resource_policy,
+                        SessionTypes.INFERENCE,
+                        {
+                            "mounts": [endpoint.model],
+                            "mount_map": {endpoint.model: endpoint.model_mount_destiation},
+                            "environ": endpoint.environ,
+                            "scaling_group": endpoint.resource_group,
+                            "resources": endpoint.resource_slots,
+                            "resource_opts": endpoint.resource_opts,
+                            "preopen_ports": None,
+                            "agent_list": None,
+                        },
+                        ClusterMode[endpoint.cluster_mode],
+                        endpoint.cluster_size,
+                        bootstrap_script=endpoint.bootstrap_script,
+                        startup_command=endpoint.startup_command,
+                        tag=endpoint.tag,
+                        callback_url=endpoint.callback_url,
+                        enqueue_only=True,
+                        endpoint_id=endpoint.id,
+                    )
+                except Exception:
+                    # TODO: Handle
+                    log.exception("error while creating session:")
+
     async def start_session(
         self,
         sched_ctx: SchedulingContext,
         session: SessionRow,
     ) -> None:
         log_fmt = (
             "prepare(s:{0.id}, type:{0.session_type}, name:{0.name}, "
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-23.3.5/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-23.3.5/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-23.3.5/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-23.3.5/ai/backend/manager/scheduler/predicates.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-23.3.5/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/server.py` & `backend.ai-manager-23.3.5/ai/backend/manager/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,14 +405,15 @@
 
 
 @actxmgr
 async def agent_registry_ctx(root_ctx: RootContext) -> AsyncIterator[None]:
     from .registry import AgentRegistry
 
     root_ctx.registry = AgentRegistry(
+        root_ctx.local_config,
         root_ctx.shared_config,
         root_ctx.db,
         root_ctx.redis_stat,
         root_ctx.redis_live,
         root_ctx.redis_image,
         root_ctx.event_dispatcher,
         root_ctx.event_producer,
```

### Comparing `backend.ai-manager-23.3.4/ai/backend/manager/types.py` & `backend.ai-manager-23.3.5/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/backend.ai_manager.egg-info/PKG-INFO` & `backend.ai-manager-23.3.5/backend.ai_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.4/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-23.3.5/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ai/backend/manager/exceptions.py
 ai/backend/manager/idle.py
 ai/backend/manager/pglock.py
 ai/backend/manager/py.typed
 ai/backend/manager/registry.py
 ai/backend/manager/server.py
 ai/backend/manager/types.py
+ai/backend/manager/utils.py
 ai/backend/manager/api/__init__.py
 ai/backend/manager/api/acl.py
 ai/backend/manager/api/admin.py
 ai/backend/manager/api/auth.py
 ai/backend/manager/api/cluster_template.py
 ai/backend/manager/api/context.py
 ai/backend/manager/api/domainconfig.py
@@ -129,27 +130,29 @@
 ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
 ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
 ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
 ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
 ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
 ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
 ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
 ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
 ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
 ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
 ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
 ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
 ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
 ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
 ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
 ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
 ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
 ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
 ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
 ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
 ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
 ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
 ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
 ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
 ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
 ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
 ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
```

### Comparing `backend.ai-manager-23.3.4/backend.ai_manager.egg-info/requires.txt` & `backend.ai-manager-23.3.5/backend.ai_manager.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 aiohttp_sse>=2.0
 aiohttp~=3.8.1
 aiomonitor-ng~=0.7.2
 aiotools~=1.6.1
 alembic~=1.8.1
 async_timeout~=4.0
 attrs>=20.3
-backend.ai-cli==23.03.4
-backend.ai-common==23.03.4
-backend.ai-plugin==23.03.4
+backend.ai-cli==23.03.5
+backend.ai-common==23.03.5
+backend.ai-plugin==23.03.5
 callosum~=0.9.10
 click>=7.1.2
 cryptography>=2.8
 graphene~=2.1.9
 lark-parser~=0.11.3
 more-itertools~=8.13.0
 msgpack>=1.0.5rc1
@@ -26,17 +26,19 @@
 python-dateutil>=2.8
 pyzmq~=24.0.1
 redis[hiredis]~=4.5.5
 setproctitle~=1.3.2
 tabulate~=0.8.9
 tenacity>=8.0
 trafaret~=2.1
+types-Jinja2
 types-PyYAML
 types-click
 types-python-dateutil
 types-redis
+types-six
 types-tabulate
 typing_extensions~=4.3
 yarl~=1.8.2
 
 [:sys_platform != "Windows"]
 uvloop>=0.17
```

### Comparing `backend.ai-manager-23.3.4/backend_shim.py` & `backend.ai-manager-23.3.5/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.4/setup.py` & `backend.ai-manager-23.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,19 @@
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'alembic~=1.8.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.4
+        """backend.ai-cli==23.03.5
 """,
-        """backend.ai-common==23.03.4
+        """backend.ai-common==23.03.5
 """,
-        """backend.ai-plugin==23.03.4
+        """backend.ai-plugin==23.03.5
 """,
         'callosum~=0.9.10',
         'click>=7.1.2',
         'cryptography>=2.8',
         'graphene~=2.1.9',
         'lark-parser~=0.11.3',
         'more-itertools~=8.13.0',
@@ -67,18 +67,20 @@
         'python-dateutil>=2.8',
         'pyzmq~=24.0.1',
         'redis[hiredis]~=4.5.5',
         'setproctitle~=1.3.2',
         'tabulate~=0.8.9',
         'tenacity>=8.0',
         'trafaret~=2.1',
+        'types-Jinja2',
         'types-PyYAML',
         'types-click',
         'types-python-dateutil',
         'types-redis',
+        'types-six',
         'types-tabulate',
         'typing_extensions~=4.3',
         'uvloop>=0.17; sys_platform != "Windows"',
         'yarl~=1.8.2',
     ),
     'license': 'LGPLv3',
     'long_description': """Backend.AI Manager with API Gateway
@@ -374,11 +376,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.4
+    'version': """23.03.5
 """,
     'zip_safe': False,
 })
```

