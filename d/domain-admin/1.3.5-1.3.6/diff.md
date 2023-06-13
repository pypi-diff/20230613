# Comparing `tmp/domain-admin-1.3.5.tar.gz` & `tmp/domain-admin-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.3.5.tar", last modified: Tue Jun 13 02:06:30 2023, max compression
+gzip compressed data, was "domain-admin-1.3.6.tar", last modified: Tue Jun 13 05:39:08 2023, max compression
```

## Comparing `domain-admin-1.3.5.tar` & `domain-admin-1.3.6.tar`

### file list

```diff
@@ -1,242 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.258985 domain-admin-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 02:06:19.000000 domain-admin-1.3.5/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-13 02:06:19.000000 domain-admin-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-13 02:06:30.258985 domain-admin-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-13 02:06:19.000000 domain-admin-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.238984 domain-admin-1.3.5/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.238984 domain-admin-1.3.5/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/api/whois_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.242984 domain-admin-1.3.5/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/config/default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.242984 domain-admin-1.3.5/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.242984 domain-admin-1.3.5/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/migrate/migrate_1213_to_131.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.242984 domain-admin-1.3.5/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/cache_domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.242984 domain-admin-1.3.5/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.242984 domain-admin-1.3.5/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.234984 domain-admin-1.3.5/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.234984 domain-admin-1.3.5/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.238984 domain-admin-1.3.5/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/1d/
--r--r--r--   0 runner    (1001) docker     (123)    10075 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/21/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/26/
--r--r--r--   0 runner    (1001) docker     (123)     4500 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/26/218174c51526b57fd0f60af4f6a572c80138bc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/30/
--r--r--r--   0 runner    (1001) docker     (123)    63296 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/30/618b1b56fd6d03066d7dc722c4a7a183377802
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/37/
--r--r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/37/2236332636716d30bed68884e5b6a4c2cbf5a2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/40/
--r--r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/40/60293e2ea143c10233675d3b2a12c7df256566
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/50/
--r--r--r--   0 runner    (1001) docker     (123)    12564 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/50/00186bef97a91c17efbe144d55a9cc36466a9c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/57/
--r--r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/57/55d0c159b607a0a5978e25659b818536dd0a76
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/5b/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/60/
--r--r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/60/08bb165b8e4ce1362e6747e06dc8320dafee0b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/6d/
--r--r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/6f/
--r--r--r--   0 runner    (1001) docker     (123)     3174 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/6f/a0b1561dba7efc2bb6125203256c575ce9e002
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/72/
--r--r--r--   0 runner    (1001) docker     (123)      466 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/72/f825fdc17d0105c0fb6e0b371a3bfa69e75729
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)   279768 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/8b/
--r--r--r--   0 runner    (1001) docker     (123)    41901 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/af/
--r--r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/af/7bfcd2a6dc374481326f9c9bc6a552070ac5a1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/b1/
--r--r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/b1/a85d7394114d497133010f10393de22d667043
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/b3/
--r--r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/b3/34c0f956d77d77ff4ef43a59f1a011a1b58e6f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/b5/
--r--r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/b5/e9c0ca71006d129884d73cea6e78c42af5e152
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/b8/
--r--r--r--   0 runner    (1001) docker     (123)      584 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/b8/6a8179b01a2b2520b74e6dcb7ecfc98f9c7734
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/ba/
--r--r--r--   0 runner    (1001) docker     (123)     4058 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/ba/ff73967492c194835e9a33fa5bbae61043850c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/ce/
--r--r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/ce/6e25e77863758b7d254d098ac0b06abcd4bb8e
--r--r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/ce/7cb1dd877823de333ada477f7d591ab481041d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/e5/
--r--r--r--   0 runner    (1001) docker     (123)     1738 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/e5/0917488520e3d5f612736a7d3295703d8c3b9c
--r--r--r--   0 runner    (1001) docker     (123)    75876 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/e5/f78c603c38d60c0d255f5b9e8a46e29fa011ab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/objects/fc/
--r--r--r--   0 runner    (1001) docker     (123)     1427 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/objects/fc/c33ef98e69a862151e8f67d3492c8891e223ab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.238984 domain-admin-1.3.5/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.238984 domain-admin-1.3.5/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.246984 domain-admin-1.3.5/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 02:06:28.000000 domain-admin-1.3.5/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.250985 domain-admin-1.3.5/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)   328716 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/css/index.7b938ee7.css
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/css/index.c44b2764.css
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/css/index.f0377688.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     6158 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.250985 domain-admin-1.3.5/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/ConnectStatus.1885a802.js
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/SelectGroup.4b54cf97.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/element-icon.ade3aa7e.js
--rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/element-plus.dcbfaaa8.js
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.0139032b.js
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.037936c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.0b7168d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.2bc0bb67.js
--rw-r--r--   0 runner    (1001) docker     (123)   231597 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.33b69268.js
--rw-r--r--   0 runner    (1001) docker     (123)    47724 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.408b451d.js
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.54d3b0f0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/index.c80eca09.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/validator.0c34c3e7.js
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/vendor-lib.4c56f242.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/js/vendor-vue.edbe275b.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.250985 domain-admin-1.3.5/domain_admin/public/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-13 02:06:29.000000 domain-admin-1.3.5/domain_admin/public/svg/logo.184a2d7d.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.254984 domain-admin-1.3.5/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.254984 domain-admin-1.3.5/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/cache_domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/email_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/global_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/version_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/service/work_weixin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.254984 domain-admin-1.3.5/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/templates/domain-cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.254984 domain-admin-1.3.5/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.258985 domain-admin-1.3.5/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/cert_util/cert_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.258985 domain-admin-1.3.5/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.258985 domain-admin-1.3.5/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/json_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.258985 domain-admin-1.3.5/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.258985 domain-admin-1.3.5/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/whois_util/whois_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/utils/work_weixin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-13 02:06:19.000000 domain-admin-1.3.5/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.238984 domain-admin-1.3.5/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-13 02:06:30.000000 domain-admin-1.3.5/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-13 02:06:30.000000 domain-admin-1.3.5/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:06:30.000000 domain-admin-1.3.5/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-13 02:06:30.000000 domain-admin-1.3.5/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 02:06:30.000000 domain-admin-1.3.5/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:06:30.000000 domain-admin-1.3.5/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:06:30.258985 domain-admin-1.3.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 02:06:19.000000 domain-admin-1.3.5/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:06:30.258985 domain-admin-1.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-13 02:06:19.000000 domain-admin-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.753986 domain-admin-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 05:38:58.000000 domain-admin-1.3.6/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-13 05:38:58.000000 domain-admin-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-13 05:39:08.753986 domain-admin-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-06-13 05:38:58.000000 domain-admin-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.737985 domain-admin-1.3.6/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.737985 domain-admin-1.3.6/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/api/whois_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.737985 domain-admin-1.3.6/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/config/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/config/env_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.737985 domain-admin-1.3.6/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.737985 domain-admin-1.3.6/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/migrate/migrate_1213_to_131.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/cache_domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.733985 domain-admin-1.3.6/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.733985 domain-admin-1.3.6/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.733985 domain-admin-1.3.6/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/1d/
+-r--r--r--   0 runner    (1001) docker     (123)    10075 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/21/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/26/
+-r--r--r--   0 runner    (1001) docker     (123)     4500 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/26/218174c51526b57fd0f60af4f6a572c80138bc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/30/
+-r--r--r--   0 runner    (1001) docker     (123)    63296 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/30/618b1b56fd6d03066d7dc722c4a7a183377802
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/37/
+-r--r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/37/2236332636716d30bed68884e5b6a4c2cbf5a2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/40/
+-r--r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/40/60293e2ea143c10233675d3b2a12c7df256566
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/50/
+-r--r--r--   0 runner    (1001) docker     (123)    12564 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/50/00186bef97a91c17efbe144d55a9cc36466a9c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/57/
+-r--r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/57/55d0c159b607a0a5978e25659b818536dd0a76
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/5b/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/60/
+-r--r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/60/08bb165b8e4ce1362e6747e06dc8320dafee0b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/6d/
+-r--r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/6f/
+-r--r--r--   0 runner    (1001) docker     (123)     3174 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/6f/a0b1561dba7efc2bb6125203256c575ce9e002
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/72/
+-r--r--r--   0 runner    (1001) docker     (123)      466 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/72/f825fdc17d0105c0fb6e0b371a3bfa69e75729
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/7a/
+-r--r--r--   0 runner    (1001) docker     (123)   279768 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/8b/
+-r--r--r--   0 runner    (1001) docker     (123)    41901 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/af/
+-r--r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/af/7bfcd2a6dc374481326f9c9bc6a552070ac5a1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.741985 domain-admin-1.3.6/domain_admin/public/.git/objects/b1/
+-r--r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/b1/a85d7394114d497133010f10393de22d667043
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/objects/b3/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/b3/34c0f956d77d77ff4ef43a59f1a011a1b58e6f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/objects/b5/
+-r--r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/b5/e9c0ca71006d129884d73cea6e78c42af5e152
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/objects/b8/
+-r--r--r--   0 runner    (1001) docker     (123)      584 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/b8/6a8179b01a2b2520b74e6dcb7ecfc98f9c7734
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/objects/ba/
+-r--r--r--   0 runner    (1001) docker     (123)     4058 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/ba/ff73967492c194835e9a33fa5bbae61043850c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/objects/ce/
+-r--r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/ce/6e25e77863758b7d254d098ac0b06abcd4bb8e
+-r--r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/ce/7cb1dd877823de333ada477f7d591ab481041d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/objects/e5/
+-r--r--r--   0 runner    (1001) docker     (123)     1738 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/e5/0917488520e3d5f612736a7d3295703d8c3b9c
+-r--r--r--   0 runner    (1001) docker     (123)    75876 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/e5/f78c603c38d60c0d255f5b9e8a46e29fa011ab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/objects/fc/
+-r--r--r--   0 runner    (1001) docker     (123)     1427 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/objects/fc/c33ef98e69a862151e8f67d3492c8891e223ab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.733985 domain-admin-1.3.6/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.733985 domain-admin-1.3.6/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   328716 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/css/index.7b938ee7.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/css/index.c44b2764.css
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/css/index.f0377688.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6158 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.745985 domain-admin-1.3.6/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/ConnectStatus.1885a802.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/SelectGroup.4b54cf97.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/element-icon.ade3aa7e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/element-plus.dcbfaaa8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.0139032b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.037936c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.0b7168d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.2bc0bb67.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231597 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.33b69268.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47724 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.408b451d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.54d3b0f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/index.c80eca09.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/validator.0c34c3e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/vendor-lib.4c56f242.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/js/vendor-vue.edbe275b.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.749986 domain-admin-1.3.6/domain_admin/public/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-13 05:39:06.000000 domain-admin-1.3.6/domain_admin/public/svg/logo.184a2d7d.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.749986 domain-admin-1.3.6/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.749986 domain-admin-1.3.6/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/cache_domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/email_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/global_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/version_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/service/work_weixin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.749986 domain-admin-1.3.6/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/templates/domain-cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.749986 domain-admin-1.3.6/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.749986 domain-admin-1.3.6/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/cert_util/cert_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.749986 domain-admin-1.3.6/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.753986 domain-admin-1.3.6/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/json_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.753986 domain-admin-1.3.6/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.753986 domain-admin-1.3.6/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/whois_util/whois_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/utils/work_weixin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-13 05:38:58.000000 domain-admin-1.3.6/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.737985 domain-admin-1.3.6/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-13 05:39:08.000000 domain-admin-1.3.6/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-13 05:39:08.000000 domain-admin-1.3.6/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:39:08.000000 domain-admin-1.3.6/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 05:39:08.000000 domain-admin-1.3.6/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 05:39:08.000000 domain-admin-1.3.6/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:39:08.000000 domain-admin-1.3.6/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:39:08.753986 domain-admin-1.3.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 05:38:58.000000 domain-admin-1.3.6/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:39:08.753986 domain-admin-1.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-13 05:38:58.000000 domain-admin-1.3.6/setup.py
```

### Comparing `domain-admin-1.3.5/LICENSE` & `domain-admin-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/PKG-INFO` & `domain-admin-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.3.5
+Version: 1.3.6
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain ssl cert
 Classifier: Programming Language :: Python :: 3.7
@@ -317,17 +317,29 @@
 域名:端口
 
 eg:
 
 www.baidu.com:8080
 ```
 
+### 8、修改数据库链接
+
+通过配置`.env` 文件或者直接设置系统环境变量
+
+```bash
+# sqlite 默认
+DB_CONNECT_URL=sqlite:///database/database.db
+
+# mysql
+DB_CONNECT_URL=mysql://root:123456@127.0.0.1:3306/data_domain
+```
+
 ## 问题反馈交流
 
-群号:731742868
+QQ群号:731742868
 
 邀请码：domain-admin
 
 <img src="https://raw.githubusercontent.com/mouday/domain-admin/master/image/qq-group.jpeg" width="300">
 
 开发计划
```

### Comparing `domain-admin-1.3.5/README.md` & `domain-admin-1.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -304,17 +304,29 @@
 域名:端口
 
 eg:
 
 www.baidu.com:8080
 ```
 
+### 8、修改数据库链接
+
+通过配置`.env` 文件或者直接设置系统环境变量
+
+```bash
+# sqlite 默认
+DB_CONNECT_URL=sqlite:///database/database.db
+
+# mysql
+DB_CONNECT_URL=mysql://root:123456@127.0.0.1:3306/data_domain
+```
+
 ## 问题反馈交流
 
-群号:731742868
+QQ群号:731742868
 
 邀请码：domain-admin
 
 <img src="https://raw.githubusercontent.com/mouday/domain-admin/master/image/qq-group.jpeg" width="300">
 
 开发计划
```

### Comparing `domain-admin-1.3.5/domain_admin/api/address_api.py` & `domain-admin-1.3.6/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/api/auth_api.py` & `domain-admin-1.3.6/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/api/domain_api.py` & `domain-admin-1.3.6/domain_admin/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/api/group_api.py` & `domain-admin-1.3.6/domain_admin/api/group_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         GroupModel.create_time.asc(),
         GroupModel.id.asc()
     )
 
     # 域名分组统计
     domain_groups = DomainModel.select(
         DomainModel.group_id,
-        fn.COUNT().alias('count')
+        fn.COUNT(1).alias('count')
     ).group_by(DomainModel.group_id)
 
     domain_groups_map = {
         row.group_id: row.count
         for row in domain_groups
     }
```

### Comparing `domain-admin-1.3.5/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.3.6/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/api/notify_api.py` & `domain-admin-1.3.6/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/api/system_api.py` & `domain-admin-1.3.6/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/api/user_api.py` & `domain-admin-1.3.6/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/config/default_config.py` & `domain-admin-1.3.6/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/enums/version_enum.py` & `domain-admin-1.3.6/domain_admin/enums/version_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/log.py` & `domain-admin-1.3.6/domain_admin/log.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/main.py` & `domain-admin-1.3.6/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.3.6/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.3.6/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.3.6/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.3.6/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.3.6/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/model/address_model.py` & `domain-admin-1.3.6/domain_admin/model/address_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 
-from peewee import CharField, IntegerField, DateTimeField, BooleanField
+from peewee import CharField, IntegerField, DateTimeField, BooleanField, AutoField
 
 from domain_admin.model.base_model import BaseModel
 from domain_admin.utils import datetime_util, time_util
 
 
 class AddressModel(BaseModel):
     """
     域名主机ip地址
     @since v1.2.24
     """
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 域名
     domain_id = CharField(null=False)
 
     # 主机地址
     host = CharField(default="")
```

### Comparing `domain-admin-1.3.5/domain_admin/model/base_model.py` & `domain-admin-1.3.6/domain_admin/model/base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 import logging
 from logging.handlers import RotatingFileHandler
 
-from peewee import Model, SqliteDatabase
+from peewee import Model, SqliteDatabase, MySQLDatabase
+from playhouse.db_url import connect
 from playhouse.sqlite_ext import SqliteExtDatabase
 from playhouse.sqliteq import SqliteQueueDatabase
 
-from domain_admin.config import SQLITE_DATABASE_PATH
+from domain_admin.config import SQLITE_DATABASE_PATH, DB_CONNECT_URL
 
 # 打印日志
 from domain_admin.service.file_service import resolve_log_file
 
 logger = logging.getLogger('peewee')
 # logger.addHandler(logging.StreamHandler())
 # logger.addHandler(logging.FileHandler(resolve_log_file("peewee.log")))
@@ -20,13 +21,15 @@
 logger.addHandler(handler)
 logger.setLevel(logging.DEBUG)
 
 # 多线程写入方式，会造成读取不到刚写入的数据
 # db = connect(SQLITE_DATABASE_URL)
 # db = SqliteQueueDatabase(database=SQLITE_DATABASE_PATH)
 # db = SqliteExtDatabase(database=SQLITE_DATABASE_PATH)
-db = SqliteDatabase(database=SQLITE_DATABASE_PATH)
+# db = SqliteDatabase(database=SQLITE_DATABASE_PATH)
+
+db = connect(url=DB_CONNECT_URL)
 
 
 class BaseModel(Model):
     class Meta:
         database = db
```

### Comparing `domain-admin-1.3.5/domain_admin/model/cache_domain_info_model.py` & `domain-admin-1.3.6/domain_admin/model/cache_domain_info_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 
-from peewee import CharField, IntegerField, DateTimeField
+from peewee import CharField, IntegerField, DateTimeField, AutoField
 
 from domain_admin.model.base_model import BaseModel
 from domain_admin.utils import time_util
 
 
 class CacheDomainInfoModel(BaseModel):
     """
     域名信息缓存表
     @since 1.2.12
     """
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 域名
     domain = CharField(unique=True)
 
     # 域名注册时间
     domain_start_time = DateTimeField(default=None, null=True)
```

### Comparing `domain-admin-1.3.5/domain_admin/model/database.py` & `domain-admin-1.3.6/domain_admin/model/database.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/model/domain_model.py` & `domain-admin-1.3.6/domain_admin/model/domain_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 import json
 from datetime import datetime
 
-from peewee import CharField, IntegerField, DateTimeField, BooleanField, TextField
+from peewee import CharField, IntegerField, DateTimeField, BooleanField, TextField, AutoField
 
 from domain_admin.model.base_model import BaseModel
 from domain_admin.model.group_model import GroupModel
 from domain_admin.utils import datetime_util, time_util
 
 
 class DomainModel(BaseModel):
     """域名"""
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 用户id
     user_id = IntegerField(default=0)
 
     # 域名
     domain = CharField()
```

### Comparing `domain-admin-1.3.5/domain_admin/model/group_model.py` & `domain-admin-1.3.6/domain_admin/model/group_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 
 from domain_admin.model.base_model import BaseModel
-from peewee import CharField, IntegerField, DateTimeField, BooleanField
+from peewee import CharField, IntegerField, DateTimeField, BooleanField, AutoField
 
 
 class GroupModel(BaseModel):
     """分组"""
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 名称
     name = CharField()
 
     # 用户id
     user_id = IntegerField(default=0)
```

### Comparing `domain-admin-1.3.5/domain_admin/model/log_scheduler_model.py` & `domain-admin-1.3.6/domain_admin/model/log_scheduler_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 import math
 from datetime import datetime
 
-from peewee import IntegerField, DateTimeField, BooleanField, TextField
+from peewee import IntegerField, DateTimeField, BooleanField, TextField, AutoField
 
 from domain_admin.model.base_model import BaseModel
 from domain_admin.utils import datetime_util
 
 
 class LogSchedulerModel(BaseModel):
     """日志"""
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 状态
     status = BooleanField(default=False)
 
     # 错误信息
     error_message = TextField(default='')
```

### Comparing `domain-admin-1.3.5/domain_admin/model/notify_model.py` & `domain-admin-1.3.6/domain_admin/model/notify_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 import json
 from datetime import datetime
 
-from peewee import IntegerField, DateTimeField, TextField
+from peewee import IntegerField, DateTimeField, TextField, AutoField
 
 from domain_admin.model.base_model import BaseModel
 
 
 class NotifyModel(BaseModel):
     """通知配置"""
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 用户id
     user_id = IntegerField(null=False)
 
     # 分类
     type_id = IntegerField(null=False, default=0)
```

### Comparing `domain-admin-1.3.5/domain_admin/model/system_model.py` & `domain-admin-1.3.6/domain_admin/model/system_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 
-from peewee import CharField, IntegerField, DateTimeField, BooleanField
+from peewee import CharField, IntegerField, DateTimeField, BooleanField, AutoField
 
 from domain_admin.model.base_model import BaseModel
 from domain_admin.utils import secret_util
 
 
 class SystemModel(BaseModel):
     """系统配置"""
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 键
     key = CharField(unique=True)
 
     # 值
     value = CharField()
```

### Comparing `domain-admin-1.3.5/domain_admin/model/user_model.py` & `domain-admin-1.3.6/domain_admin/model/user_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 import json
 from datetime import datetime
 import warnings
 from domain_admin.config import ADMIN_USERNAME
 from domain_admin.model.base_model import BaseModel
-from peewee import CharField, IntegerField, DateTimeField, BooleanField, TextField
+from peewee import CharField, IntegerField, DateTimeField, BooleanField, TextField, AutoField
 
 from domain_admin.utils import bcrypt_util
 
 
 class UserModel(BaseModel):
     """用户"""
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 用户名
     username = CharField(unique=True, null=None)
 
     # 密码
     password = CharField()
```

### Comparing `domain-admin-1.3.5/domain_admin/model/version_model.py` & `domain-admin-1.3.6/domain_admin/model/version_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 
-from peewee import CharField, IntegerField, DateTimeField
+from peewee import CharField, IntegerField, DateTimeField, AutoField
 
 from domain_admin.model.base_model import BaseModel
 
 
 class VersionModel(BaseModel):
     """记录版本号"""
-    id = IntegerField(primary_key=True)
+    id = AutoField(primary_key=True)
 
     # 版本号
     version = CharField(unique=True)
 
     # 创建时间
     create_time = DateTimeField(default=datetime.now)
```

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.3.6/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27` & `domain-admin-1.3.6/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/26/218174c51526b57fd0f60af4f6a572c80138bc` & `domain-admin-1.3.6/domain_admin/public/.git/objects/26/218174c51526b57fd0f60af4f6a572c80138bc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/30/618b1b56fd6d03066d7dc722c4a7a183377802` & `domain-admin-1.3.6/domain_admin/public/.git/objects/30/618b1b56fd6d03066d7dc722c4a7a183377802`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/37/2236332636716d30bed68884e5b6a4c2cbf5a2` & `domain-admin-1.3.6/domain_admin/public/.git/objects/37/2236332636716d30bed68884e5b6a4c2cbf5a2`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/50/00186bef97a91c17efbe144d55a9cc36466a9c` & `domain-admin-1.3.6/domain_admin/public/.git/objects/50/00186bef97a91c17efbe144d55a9cc36466a9c`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410` & `domain-admin-1.3.6/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc` & `domain-admin-1.3.6/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/6f/a0b1561dba7efc2bb6125203256c575ce9e002` & `domain-admin-1.3.6/domain_admin/public/.git/objects/6f/a0b1561dba7efc2bb6125203256c575ce9e002`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef` & `domain-admin-1.3.6/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a` & `domain-admin-1.3.6/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/b1/a85d7394114d497133010f10393de22d667043` & `domain-admin-1.3.6/domain_admin/public/.git/objects/b1/a85d7394114d497133010f10393de22d667043`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/b8/6a8179b01a2b2520b74e6dcb7ecfc98f9c7734` & `domain-admin-1.3.6/domain_admin/public/.git/objects/b8/6a8179b01a2b2520b74e6dcb7ecfc98f9c7734`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/ba/ff73967492c194835e9a33fa5bbae61043850c` & `domain-admin-1.3.6/domain_admin/public/.git/objects/ba/ff73967492c194835e9a33fa5bbae61043850c`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/ce/6e25e77863758b7d254d098ac0b06abcd4bb8e` & `domain-admin-1.3.6/domain_admin/public/.git/objects/ce/6e25e77863758b7d254d098ac0b06abcd4bb8e`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/ce/7cb1dd877823de333ada477f7d591ab481041d` & `domain-admin-1.3.6/domain_admin/public/.git/objects/ce/7cb1dd877823de333ada477f7d591ab481041d`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/e5/0917488520e3d5f612736a7d3295703d8c3b9c` & `domain-admin-1.3.6/domain_admin/public/.git/objects/e5/0917488520e3d5f612736a7d3295703d8c3b9c`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/e5/f78c603c38d60c0d255f5b9e8a46e29fa011ab` & `domain-admin-1.3.6/domain_admin/public/.git/objects/e5/f78c603c38d60c0d255f5b9e8a46e29fa011ab`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/.git/objects/fc/c33ef98e69a862151e8f67d3492c8891e223ab` & `domain-admin-1.3.6/domain_admin/public/.git/objects/fc/c33ef98e69a862151e8f67d3492c8891e223ab`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/css/index.7b938ee7.css` & `domain-admin-1.3.6/domain_admin/public/css/index.7b938ee7.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/css/index.c44b2764.css` & `domain-admin-1.3.6/domain_admin/public/css/index.c44b2764.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/favicon.ico` & `domain-admin-1.3.6/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/index.html` & `domain-admin-1.3.6/domain_admin/public/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/ConnectStatus.1885a802.js` & `domain-admin-1.3.6/domain_admin/public/js/ConnectStatus.1885a802.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/SelectGroup.4b54cf97.js` & `domain-admin-1.3.6/domain_admin/public/js/SelectGroup.4b54cf97.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/element-icon.ade3aa7e.js` & `domain-admin-1.3.6/domain_admin/public/js/element-icon.ade3aa7e.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/element-plus.dcbfaaa8.js` & `domain-admin-1.3.6/domain_admin/public/js/element-plus.dcbfaaa8.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.0139032b.js` & `domain-admin-1.3.6/domain_admin/public/js/index.0139032b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.037936c6.js` & `domain-admin-1.3.6/domain_admin/public/js/index.037936c6.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.0b7168d0.js` & `domain-admin-1.3.6/domain_admin/public/js/index.0b7168d0.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.2bc0bb67.js` & `domain-admin-1.3.6/domain_admin/public/js/index.2bc0bb67.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.33b69268.js` & `domain-admin-1.3.6/domain_admin/public/js/index.33b69268.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.408b451d.js` & `domain-admin-1.3.6/domain_admin/public/js/index.408b451d.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.54d3b0f0.js` & `domain-admin-1.3.6/domain_admin/public/js/index.54d3b0f0.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/index.c80eca09.js` & `domain-admin-1.3.6/domain_admin/public/js/index.c80eca09.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/vendor-lib.4c56f242.js` & `domain-admin-1.3.6/domain_admin/public/js/vendor-lib.4c56f242.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/js/vendor-vue.edbe275b.js` & `domain-admin-1.3.6/domain_admin/public/js/vendor-vue.edbe275b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/public/svg/logo.184a2d7d.svg` & `domain-admin-1.3.6/domain_admin/public/svg/logo.184a2d7d.svg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/router/api_map.py` & `domain-admin-1.3.6/domain_admin/router/api_map.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/router/permission.py` & `domain-admin-1.3.6/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/auth_service.py` & `domain-admin-1.3.6/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/cache_domain_info_service.py` & `domain-admin-1.3.6/domain_admin/service/cache_domain_info_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if domain_whois is None:
             raise Exception("域名信息获取失败")
 
         data = {
             "domain": root_domain,
             "domain_start_time": domain_whois['start_time'],
             "domain_expire_time": domain_whois['expire_time'],
-            "expire_time": domain_whois['expire_time'] - timedelta(minutes=3)
+            "expire_time": datetime.now() - timedelta(minutes=3)
         }
 
         if not row:
             row = CacheDomainInfoModel.create(**data)
         else:
             CacheDomainInfoModel.update(data).where(
                 CacheDomainInfoModel.id == row.id
```

### Comparing `domain-admin-1.3.5/domain_admin/service/domain_service.py` & `domain-admin-1.3.6/domain_admin/service/domain_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/email_service.py` & `domain-admin-1.3.6/domain_admin/service/email_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/file_service.py` & `domain-admin-1.3.6/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/notify_service.py` & `domain-admin-1.3.6/domain_admin/service/notify_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/scheduler_service.py` & `domain-admin-1.3.6/domain_admin/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/system_service.py` & `domain-admin-1.3.6/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/token_service.py` & `domain-admin-1.3.6/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/version_service.py` & `domain-admin-1.3.6/domain_admin/service/version_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/service/work_weixin_service.py` & `domain-admin-1.3.6/domain_admin/service/work_weixin_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/templates/domain-cert-email.html` & `domain-admin-1.3.6/domain_admin/templates/domain-cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.3.6/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/cert_util/__init__.py` & `domain-admin-1.3.6/domain_admin/utils/cert_util/__init__.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.3.6/domain_admin/utils/cert_util/cert_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/cert_util/cert_openssl.py` & `domain-admin-1.3.6/domain_admin/utils/cert_util/cert_openssl.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.3.6/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.3.6/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 def get_domain_host_list(domain: str, port: int = 80) -> typing.List[str]:
     """
     获取域名映射主机地址列表，一对多关系
     :param domain: 域名
     :param port: 端口
     :return: 主机地址列表
     """
-    ret = socket.getaddrinfo(host=domain, port=port, proto=socket.IPPROTO_TCP)
+    ret = socket.getaddrinfo(
+        host=domain,
+        port=port,
+        family=socket.AF_INET,  # 限制仅返回IPv4
+        proto=socket.IPPROTO_TCP)
 
     lst = []
     for item in ret:
         lst.append(item[4][0])
 
     return lst
```

### Comparing `domain-admin-1.3.5/domain_admin/utils/datetime_util.py` & `domain-admin-1.3.6/domain_admin/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/domain_util.py` & `domain-admin-1.3.6/domain_admin/utils/domain_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/email_util.py` & `domain-admin-1.3.6/domain_admin/utils/email_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.3.6/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.3.6/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.3.6/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.3.6/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/ip_util.py` & `domain-admin-1.3.6/domain_admin/utils/ip_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/json_util.py` & `domain-admin-1.3.6/domain_admin/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.3.6/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/text_util.py` & `domain-admin-1.3.6/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/time_util.py` & `domain-admin-1.3.6/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/whois_util/config.py` & `domain-admin-1.3.6/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/whois_util/util.py` & `domain-admin-1.3.6/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.3.6/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.3.6/domain_admin/utils/whois_util/whois_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin/utils/work_weixin_api.py` & `domain-admin-1.3.6/domain_admin/utils/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.5/domain_admin.egg-info/PKG-INFO` & `domain-admin-1.3.6/domain_admin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.3.5
+Version: 1.3.6
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain ssl cert
 Classifier: Programming Language :: Python :: 3.7
@@ -317,17 +317,29 @@
 域名:端口
 
 eg:
 
 www.baidu.com:8080
 ```
 
+### 8、修改数据库链接
+
+通过配置`.env` 文件或者直接设置系统环境变量
+
+```bash
+# sqlite 默认
+DB_CONNECT_URL=sqlite:///database/database.db
+
+# mysql
+DB_CONNECT_URL=mysql://root:123456@127.0.0.1:3306/data_domain
+```
+
 ## 问题反馈交流
 
-群号:731742868
+QQ群号:731742868
 
 邀请码：domain-admin
 
 <img src="https://raw.githubusercontent.com/mouday/domain-admin/master/image/qq-group.jpeg" width="300">
 
 开发计划
```

### Comparing `domain-admin-1.3.5/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.3.6/domain_admin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 domain_admin/api/log_scheduler_api.py
 domain_admin/api/notify_api.py
 domain_admin/api/system_api.py
 domain_admin/api/user_api.py
 domain_admin/api/whois_api.py
 domain_admin/config/__init__.py
 domain_admin/config/default_config.py
+domain_admin/config/env_config.py
 domain_admin/enums/__init__.py
 domain_admin/enums/notify_type_enum.py
 domain_admin/enums/version_enum.py
 domain_admin/migrate/__init__.py
 domain_admin/migrate/migrate_102_to_103.py
 domain_admin/migrate/migrate_106_to_110.py
 domain_admin/migrate/migrate_110_to_1212.py
```

### Comparing `domain-admin-1.3.5/setup.py` & `domain-admin-1.3.6/setup.py`

 * *Files identical despite different names*

