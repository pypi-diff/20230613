# Comparing `tmp/ansible-modules-hashivault-5.1.0.tar.gz` & `tmp/ansible-modules-hashivault-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-modules-hashivault-5.1.0.tar", last modified: Tue Apr 18 18:54:10 2023, max compression
+gzip compressed data, was "ansible-modules-hashivault-5.1.1.tar", last modified: Tue Jun 13 14:15:20 2023, max compression
```

## Comparing `ansible-modules-hashivault-5.1.0.tar` & `ansible-modules-hashivault-5.1.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.866017 ansible-modules-hashivault-5.1.0/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.0/AUTHORS
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    29188 2023-04-18 18:54:02.000000 ansible-modules-hashivault-5.1.0/CHANGELOG.rst
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1079 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.0/LICENSE
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      114 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.0/MANIFEST.in
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6733 2023-04-18 18:54:10.866146 ansible-modules-hashivault-5.1.0/PKG-INFO
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6376 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/README.rst
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.795088 ansible-modules-hashivault-5.1.0/ansible/
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.800615 ansible-modules-hashivault-5.1.0/ansible/module_utils/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    14241 2023-03-11 12:45:43.000000 ansible-modules-hashivault-5.1.0/ansible/module_utils/hashivault.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.794902 ansible-modules-hashivault-5.1.0/ansible/modules/
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.861614 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)        0 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/__init__.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7661 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1673 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1762 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_id.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1565 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4722 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2069 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2312 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1970 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2933 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1228 2022-11-07 21:30:40.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    10086 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_ldap.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1289 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4973 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_method.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3499 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7274 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4221 2023-03-31 13:47:48.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7090 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4184 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3745 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2112 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_cluster_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2688 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5362 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7073 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6299 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_role.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3247 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_delete.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1536 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1435 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_cancel.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2125 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_init.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1172 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5903 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7527 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity_alias.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9178 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7489 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group_alias.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3901 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_init.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4121 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6187 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4059 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ldap_group.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1203 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_leader.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3967 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2487 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_namespace.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5426 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9444 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_role.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    11153 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2728 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca_set.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2065 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_get.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6029 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_issue.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1828 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_list.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2314 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_revoke.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6865 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_sign.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2708 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1987 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_get.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1965 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_rotate.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    18694 2023-03-11 12:45:43.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2115 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_get.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1839 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_list.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2948 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_set_signed.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3198 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_tidy.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3359 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1942 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3455 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1588 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_get.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1458 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_list.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1796 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1251 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read_to_file.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1789 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1337 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_cancel.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3530 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_init.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1152 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1702 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_verify.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1276 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_seal.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5971 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9583 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_engine.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1364 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    18577 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2267 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1189 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_status.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4688 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_create.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2140 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_lookup.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2531 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_renew.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2088 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_revoke.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)    12376 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2237 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role_list.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1392 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_unseal.py
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5748 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_userpass.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5301 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)      979 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write_from_file.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.795572 ansible-modules-hashivault-5.1.0/ansible/plugins/
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.862752 ansible-modules-hashivault-5.1.0/ansible/plugins/action/
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5319 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_read_to_file.py
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2108 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_write_from_file.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.863361 ansible-modules-hashivault-5.1.0/ansible/plugins/doc_fragments/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2695 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/doc_fragments/hashivault.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.863803 ansible-modules-hashivault-5.1.0/ansible/plugins/lookup/
--rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2846 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.0/ansible/plugins/lookup/hashivault.py
-drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-04-18 18:54:10.865780 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6733 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/PKG-INFO
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5306 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/SOURCES.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)        1 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/dependency_links.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/requires.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      231 2023-04-18 18:54:10.000000 ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/top_level.txt
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      119 2023-04-18 18:54:10.866608 ansible-modules-hashivault-5.1.0/setup.cfg
--rw-r--r--   0 tlhowe   (2038566311) staff       (20)      894 2023-04-18 18:53:07.000000 ansible-modules-hashivault-5.1.0/setup.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:20.078870 ansible-modules-hashivault-5.1.1/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.1/AUTHORS
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    29356 2023-06-13 14:15:13.000000 ansible-modules-hashivault-5.1.1/CHANGELOG.rst
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1079 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.1/LICENSE
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      114 2020-11-06 20:49:46.000000 ansible-modules-hashivault-5.1.1/MANIFEST.in
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6696 2023-06-13 14:15:20.079071 ansible-modules-hashivault-5.1.1/PKG-INFO
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6376 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/README.rst
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:19.973846 ansible-modules-hashivault-5.1.1/ansible/
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:19.978578 ansible-modules-hashivault-5.1.1/ansible/module_utils/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    14241 2023-03-11 12:45:43.000000 ansible-modules-hashivault-5.1.1/ansible/module_utils/hashivault.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:19.973651 ansible-modules-hashivault-5.1.1/ansible/modules/
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:20.068863 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)        0 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/__init__.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7661 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1673 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1762 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_id.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1565 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4722 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2069 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2312 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1970 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2933 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_audit.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1228 2022-11-07 21:30:40.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_audit_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    10086 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_auth_ldap.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1289 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_auth_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4973 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_auth_method.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3499 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_aws_auth_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7274 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_aws_auth_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4221 2023-03-31 13:47:48.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_auth_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7090 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_auth_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4184 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3745 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2112 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_cluster_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2688 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5362 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7414 2023-06-13 14:14:24.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_db_secret_engine_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6299 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_db_secret_engine_role.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3247 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_delete.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1536 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1435 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root_cancel.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2125 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root_init.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1172 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5903 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_entity.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7527 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_entity_alias.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9178 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_group.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     7489 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_group_alias.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3901 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_init.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4121 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_k8s_auth_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6187 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_k8s_auth_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4059 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_ldap_group.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1203 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_leader.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3967 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2487 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_namespace.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5426 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9444 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_oidc_auth_role.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    11153 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_ca.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2728 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_ca_set.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2065 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_get.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6029 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_issue.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1828 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_list.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2314 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_revoke.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     6865 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_sign.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2708 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_crl.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1987 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_crl_get.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1965 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_crl_rotate.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)    18694 2023-03-11 12:45:43.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_role.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2115 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_role_get.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1839 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_role_list.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2948 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_set_signed.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3198 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_tidy.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     3359 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_url.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1942 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_url_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3455 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_policy.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1588 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_policy_get.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1458 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_policy_list.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1796 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_read.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     1251 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_read_to_file.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1789 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1337 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_cancel.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     3530 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_init.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1152 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1702 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_verify.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1276 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_seal.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5971 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_secret.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     9583 2023-04-18 18:08:46.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_secret_engine.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1364 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_secret_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    18577 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_ssh_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2267 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_ssh_role_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1189 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_status.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     4688 2022-11-07 21:35:27.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_create.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2140 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_lookup.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2531 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_renew.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2088 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_revoke.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)    12376 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_role.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2237 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_role_list.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     1392 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_unseal.py
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5748 2022-11-07 21:34:42.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_userpass.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5301 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_write.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)      979 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_write_from_file.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:19.974425 ansible-modules-hashivault-5.1.1/ansible/plugins/
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:20.071249 ansible-modules-hashivault-5.1.1/ansible/plugins/action/
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     5319 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/plugins/action/hashivault_read_to_file.py
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2108 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/plugins/action/hashivault_write_from_file.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:20.072590 ansible-modules-hashivault-5.1.1/ansible/plugins/doc_fragments/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     2695 2022-04-05 19:55:19.000000 ansible-modules-hashivault-5.1.1/ansible/plugins/doc_fragments/hashivault.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:20.073619 ansible-modules-hashivault-5.1.1/ansible/plugins/lookup/
+-rwxr-xr-x   0 tlhowe   (2038566311) staff       (20)     2846 2023-03-11 13:32:18.000000 ansible-modules-hashivault-5.1.1/ansible/plugins/lookup/hashivault.py
+drwxr-xr-x   0 tlhowe   (2038566311) staff       (20)        0 2023-06-13 14:15:20.078376 ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     6696 2023-06-13 14:15:19.000000 ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/PKG-INFO
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)     5306 2023-06-13 14:15:19.000000 ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/SOURCES.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)        1 2023-06-13 14:15:19.000000 ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/dependency_links.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)       36 2023-06-13 14:15:19.000000 ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/requires.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      231 2023-06-13 14:15:19.000000 ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/top_level.txt
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      119 2023-06-13 14:15:20.080151 ansible-modules-hashivault-5.1.1/setup.cfg
+-rw-r--r--   0 tlhowe   (2038566311) staff       (20)      894 2023-06-13 14:14:51.000000 ansible-modules-hashivault-5.1.1/setup.py
```

### Comparing `ansible-modules-hashivault-5.1.0/CHANGELOG.rst` & `ansible-modules-hashivault-5.1.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+5.1.1 (2023-06-13)
+------------------
+- Add plugin_version params for the vault api. [Ankit]
+  Ref https://github.com/TerryHowe/ansible-modules-hashivault/issues/442
+
+
 5.1.0 (2023-04-18)
 ------------------
 - Refactor policy module. [Cees Moerkerken]
 - Add diff, fixes #439. [Cees Moerkerken]
 - Add path to return values. [Cees Moerkerken]
 - Fix line length linting. [Cees Moerkerken]
 - Only call enable or tune when changed. add comments. [Cees Moerkerken]
```

### Comparing `ansible-modules-hashivault-5.1.0/LICENSE` & `ansible-modules-hashivault-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/PKG-INFO` & `ansible-modules-hashivault-5.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ansible-modules-hashivault
-Version: 5.1.0
+Version: 5.1.1
 Summary: Ansible Modules for Hashicorp Vault
 Home-page: https://github.com/TerryHowe/ansible-modules-hashivault
 Author: Terry Howe
 Author-email: terrylhowe@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Ansible Modules Hashivault
 ==========================
 
@@ -187,9 +185,7 @@
     rm -rf dist; python setup.py sdist
     pip install ./dist/ansible-modules-hashivault-*.tar.gz
 
 License
 -------
 
 `MIT <https://github.com/TerryHowe/ansible-modules-hashivault/blob/master/LICENSE>`_.
-
-
```

### Comparing `ansible-modules-hashivault-5.1.0/README.rst` & `ansible-modules-hashivault-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/module_utils/hashivault.py` & `ansible-modules-hashivault-5.1.1/ansible/module_utils/hashivault.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_id.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_id.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret_accessor_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_approle_role_secret_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_approle_role_secret_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_audit.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_audit_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_audit_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_ldap.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_auth_ldap.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_auth_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_auth_method.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_auth_method.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_config.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_aws_auth_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_aws_auth_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_aws_auth_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_config.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_auth_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_auth_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_auth_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_secret_engine_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_azure_secret_engine_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_cluster_status.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_cluster_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_consul_secret_engine_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_consul_secret_engine_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_config.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_db_secret_engine_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     connection_details:
         description:
             - root level database credential for example username, password, connection_url.
     plugin_name:
         description:
             - name of database plugin used. see out of the box list at
               https://www.vaultproject.io/docs/secrets/databases/index.html
+    plugin_version:
+        description:
+            - Specifies the semantic version of the plugin to use for this connection
+              https://developer.hashicorp.com/vault/api-docs/secret/databases
     allowed_roles:
         description:
             - list of the roles allowed to use this connection. Defaults to empty (no roles), if contains a "*" any role
               can use this connection.
         default: []
     verify_connection:
         description:
@@ -78,14 +82,15 @@
 def main():
     argspec = hashivault_argspec()
     argspec['name'] = dict(required=True, type='str')
     argspec['state'] = dict(required=False, type='str', default='present', choices=['present', 'absent'])
     argspec['mount_point'] = dict(required=False, type='str', default='database')
     argspec['config_file'] = dict(required=False, type='str', default=None)
     argspec['plugin_name'] = dict(required=False, type='str')
+    argspec['plugin_version'] = dict(required=False, type='str')
     argspec['allowed_roles'] = dict(required=False, type='list', default=[])
     argspec['root_credentials_rotate_statements'] = dict(required=False, type='list',
                                                          aliases=['root_rotation_statements'], default=[])
     argspec['verify_connection'] = dict(required=False, type='bool', default=True)
     argspec['connection_details'] = dict(required=True, type='dict', no_log=True)
     argspec['password_policy'] = dict(required=False, type='str', no_log=True, default='')
     required_one_of = [['config_file', 'connection_details']]
@@ -110,14 +115,15 @@
 
     # if config_file is set value from file
     # else set from passed args
     if config_file:
         desired_state = json.loads(open(params.get('config_file'), 'r').read())
     else:
         desired_state['plugin_name'] = params.get('plugin_name')
+        desired_state['plugin_version'] = params.get('plugin_version')
         desired_state['allowed_roles'] = params.get('allowed_roles')
         desired_state['verify_connection'] = params.get('verify_connection')
         desired_state['password_policy'] = params.get('password_policy')
         desired_state['root_rotation_statements'] = params.get('root_credentials_rotate_statements')
         connection_details = params.get('connection_details')
         desired_state.update(connection_details)
         del connection_details["password"]
```

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_db_secret_engine_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_db_secret_engine_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_delete.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_delete.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_cancel.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root_cancel.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_init.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root_init.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_generate_root_status.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_generate_root_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_entity.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_entity_alias.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_entity_alias.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_group.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_identity_group_alias.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_identity_group_alias.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_init.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_init.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_config.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_k8s_auth_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_k8s_auth_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_k8s_auth_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ldap_group.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_ldap_group.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_leader.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_leader.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_namespace.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_namespace.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_oidc_auth_method_config.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_oidc_auth_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_oidc_auth_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_ca.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_ca_set.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_ca_set.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_issue.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_issue.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_revoke.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_revoke.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_cert_sign.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_cert_sign.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_crl.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_crl_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_crl_rotate.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_crl_rotate.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_role_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_role_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_set_signed.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_set_signed.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_tidy.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_tidy.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_url.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_pki_url_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_pki_url_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_policy.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_get.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_policy_get.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_policy_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_policy_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_read.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_read_to_file.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_read_to_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_cancel.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_cancel.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_init.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_init.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_status.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_rekey_verify.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_rekey_verify.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_seal.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_seal.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_secret.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_engine.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_secret_engine.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_secret_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_secret_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_ssh_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_ssh_role_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_ssh_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_status.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_status.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_create.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_create.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_lookup.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_lookup.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_renew.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_renew.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_revoke.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_revoke.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_role.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_token_role_list.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_token_role_list.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_unseal.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_unseal.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_userpass.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_userpass.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_write.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/modules/hashivault/hashivault_write_from_file.py` & `ansible-modules-hashivault-5.1.1/ansible/modules/hashivault/hashivault_write_from_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_read_to_file.py` & `ansible-modules-hashivault-5.1.1/ansible/plugins/action/hashivault_read_to_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/plugins/action/hashivault_write_from_file.py` & `ansible-modules-hashivault-5.1.1/ansible/plugins/action/hashivault_write_from_file.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/plugins/doc_fragments/hashivault.py` & `ansible-modules-hashivault-5.1.1/ansible/plugins/doc_fragments/hashivault.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible/plugins/lookup/hashivault.py` & `ansible-modules-hashivault-5.1.1/ansible/plugins/lookup/hashivault.py`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/PKG-INFO` & `ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ansible-modules-hashivault
-Version: 5.1.0
+Version: 5.1.1
 Summary: Ansible Modules for Hashicorp Vault
 Home-page: https://github.com/TerryHowe/ansible-modules-hashivault
 Author: Terry Howe
 Author-email: terrylhowe@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Ansible Modules Hashivault
 ==========================
 
@@ -187,9 +185,7 @@
     rm -rf dist; python setup.py sdist
     pip install ./dist/ansible-modules-hashivault-*.tar.gz
 
 License
 -------
 
 `MIT <https://github.com/TerryHowe/ansible-modules-hashivault/blob/master/LICENSE>`_.
-
-
```

### Comparing `ansible-modules-hashivault-5.1.0/ansible_modules_hashivault.egg-info/SOURCES.txt` & `ansible-modules-hashivault-5.1.1/ansible_modules_hashivault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-modules-hashivault-5.1.0/setup.py` & `ansible-modules-hashivault-5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "ansible/modules/hashivault",
 ]
 
 long_description = open('README.rst', 'r').read()
 
 setup(
     name='ansible-modules-hashivault',
-    version='5.1.0',
+    version='5.1.1',
     description='Ansible Modules for Hashicorp Vault',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Terry Howe',
     author_email='terrylhowe@example.com',
     url='https://github.com/TerryHowe/ansible-modules-hashivault',
     py_modules=py_files,
```

