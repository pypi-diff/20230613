# Comparing `tmp/talos_install-0.2.0.dev356.tar.gz` & `tmp/talos_install-0.2.0.dev363.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.dev356.tar", last modified: Mon Apr 24 12:46:37 2023, max compression
+gzip compressed data, was "talos_install-0.2.0.dev363.tar", last modified: Tue Jun 13 15:45:10 2023, max compression
```

## Comparing `talos_install-0.2.0.dev356.tar` & `talos_install-0.2.0.dev363.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.424332 talos_install-0.2.0.dev356/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    11708 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     3400 2023-04-24 12:46:37.424332 talos_install-0.2.0.dev356/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     2740 2023-04-24 12:02:57.000000 talos_install-0.2.0.dev356/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.395332 talos_install-0.2.0.dev356/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.395332 talos_install-0.2.0.dev356/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      702 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.392332 talos_install-0.2.0.dev356/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.381332 talos_install-0.2.0.dev356/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.395332 talos_install-0.2.0.dev356/ansible/roles/cli/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/files/FOUNDMEDEVKEY
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.396332 talos_install-0.2.0.dev356/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.397332 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1227 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.399332 talos_install-0.2.0.dev356/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      484 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.381332 talos_install-0.2.0.dev356/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.400332 talos_install-0.2.0.dev356/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.400332 talos_install-0.2.0.dev356/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.382332 talos_install-0.2.0.dev356/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.401332 talos_install-0.2.0.dev356/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.401332 talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      930 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      929 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.382332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.382332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.401332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.383332 talos_install-0.2.0.dev356/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.383332 talos_install-0.2.0.dev356/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.384332 talos_install-0.2.0.dev356/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.385332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.384332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.385332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.386332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.387332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.387332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.407332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.407332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.408332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.408332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.409332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.409332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.409332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.410332 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.411332 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.391332 talos_install-0.2.0.dev356/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.412332 talos_install-0.2.0.dev356/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.413332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.389332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.389332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.413332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.413332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.390332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.390332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.390332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.414332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.414332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.415332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.415332 talos_install-0.2.0.dev356/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.416332 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.391332 talos_install-0.2.0.dev356/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-04-24 11:46:13.000000 talos_install-0.2.0.dev356/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.391332 talos_install-0.2.0.dev356/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.392332 talos_install-0.2.0.dev356/ansible/roles/uninstall/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.418332 talos_install-0.2.0.dev356/ansible/roles/uninstall/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.418332 talos_install-0.2.0.dev356/ansible/roles/uninstall/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.419332 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      660 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/cli.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/docker.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      345 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/user.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.419332 talos_install-0.2.0.dev356/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.419332 talos_install-0.2.0.dev356/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.420332 talos_install-0.2.0.dev356/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.420332 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.421332 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1810 2023-04-24 12:01:39.000000 talos_install-0.2.0.dev356/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.422332 talos_install-0.2.0.dev356/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      293 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/etc/globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev356/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1066 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/etc/talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-04-24 12:46:37.425332 talos_install-0.2.0.dev356/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)    10147 2023-04-24 12:24:19.000000 talos_install-0.2.0.dev356/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.423332 talos_install-0.2.0.dev356/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3400 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5583 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev356/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.371573 talos_install-0.2.0.dev363/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11906 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3400 2023-06-13 15:45:10.371573 talos_install-0.2.0.dev363/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2740 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.344573 talos_install-0.2.0.dev363/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.344573 talos_install-0.2.0.dev363/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      702 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.341573 talos_install-0.2.0.dev363/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.330573 talos_install-0.2.0.dev363/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.344573 talos_install-0.2.0.dev363/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.344573 talos_install-0.2.0.dev363/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.346573 talos_install-0.2.0.dev363/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-13 15:42:50.000000 talos_install-0.2.0.dev363/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1497 2023-06-13 15:42:50.000000 talos_install-0.2.0.dev363/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2718 2023-06-13 15:42:50.000000 talos_install-0.2.0.dev363/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.348573 talos_install-0.2.0.dev363/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      484 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-13 15:42:50.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.330573 talos_install-0.2.0.dev363/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.348573 talos_install-0.2.0.dev363/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.349573 talos_install-0.2.0.dev363/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.331573 talos_install-0.2.0.dev363/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.349573 talos_install-0.2.0.dev363/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.349573 talos_install-0.2.0.dev363/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      930 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      929 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.331573 talos_install-0.2.0.dev363/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.331573 talos_install-0.2.0.dev363/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.349573 talos_install-0.2.0.dev363/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.350573 talos_install-0.2.0.dev363/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.350573 talos_install-0.2.0.dev363/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.350573 talos_install-0.2.0.dev363/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.332573 talos_install-0.2.0.dev363/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.350573 talos_install-0.2.0.dev363/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.351573 talos_install-0.2.0.dev363/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.333573 talos_install-0.2.0.dev363/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.351573 talos_install-0.2.0.dev363/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.351573 talos_install-0.2.0.dev363/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.351573 talos_install-0.2.0.dev363/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/install_docker/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.352573 talos_install-0.2.0.dev363/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.333573 talos_install-0.2.0.dev363/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.352573 talos_install-0.2.0.dev363/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.352573 talos_install-0.2.0.dev363/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.337573 talos_install-0.2.0.dev363/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.352573 talos_install-0.2.0.dev363/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.334573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.334573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.353573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.353573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.353573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.337573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.353573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.334573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.353573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.335573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.354573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.354573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.354573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.354573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.336573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.336573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.355573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.355573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.356573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-05 12:43:41.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.356573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.357573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.336573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.357573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.337573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.337573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.357573 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.358573 talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.359573 talos_install-0.2.0.dev363/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-05 14:30:33.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.339573 talos_install-0.2.0.dev363/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.359573 talos_install-0.2.0.dev363/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.361573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.338573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.338573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.361573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.361573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.338573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.338573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.339573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.362573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.362573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-05 12:49:28.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-05 12:49:28.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.362573 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.363573 talos_install-0.2.0.dev363/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.364573 talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.364573 talos_install-0.2.0.dev363/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.340573 talos_install-0.2.0.dev363/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.364573 talos_install-0.2.0.dev363/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.340573 talos_install-0.2.0.dev363/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.365573 talos_install-0.2.0.dev363/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.365573 talos_install-0.2.0.dev363/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.365573 talos_install-0.2.0.dev363/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      650 2023-06-13 15:42:50.000000 talos_install-0.2.0.dev363/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.341573 talos_install-0.2.0.dev363/ansible/roles/uninstall/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.365573 talos_install-0.2.0.dev363/ansible/roles/uninstall/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/uninstall/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.365573 talos_install-0.2.0.dev363/ansible/roles/uninstall/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/uninstall/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.366573 talos_install-0.2.0.dev363/ansible/roles/uninstall/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      660 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/uninstall/tasks/cli.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/uninstall/tasks/docker.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/uninstall/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-13 15:42:50.000000 talos_install-0.2.0.dev363/ansible/roles/uninstall/tasks/user.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.367573 talos_install-0.2.0.dev363/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.367573 talos_install-0.2.0.dev363/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.367573 talos_install-0.2.0.dev363/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.368573 talos_install-0.2.0.dev363/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.368573 talos_install-0.2.0.dev363/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1835 2023-06-05 13:08:19.000000 talos_install-0.2.0.dev363/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.369573 talos_install-0.2.0.dev363/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      293 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/etc/globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev363/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1090 2023-06-13 15:42:50.000000 talos_install-0.2.0.dev363/etc/talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-06-13 15:45:10.382573 talos_install-0.2.0.dev363/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-05-29 11:27:25.000000 talos_install-0.2.0.dev363/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)    10147 2023-06-05 12:53:05.000000 talos_install-0.2.0.dev363/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-13 15:45:10.371573 talos_install-0.2.0.dev363/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3400 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5583 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev363/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-13 15:45:10.000000 talos_install-0.2.0.dev363/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0.dev356/ChangeLog` & `talos_install-0.2.0.dev363/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+* Fix Home position
+* Remove SWAP\_USAGE for Talos mgmt
+* Add Init Playbook on Reload
+* Add Init Playbook on Reload
+* Add Init Playbook on Reload
+* Add Init Playbook on Reload
+* fix install options
 * Enhance talos\_install
 * fix missing dev\_keys installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
```

### Comparing `talos_install-0.2.0.dev356/PKG-INFO` & `talos_install-0.2.0.dev363/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos_install
-Version: 0.2.0.dev356
+Version: 0.2.0.dev363
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `talos_install-0.2.0.dev356/README.md` & `talos_install-0.2.0.dev363/README.md`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/group_vars/all.yaml` & `talos_install-0.2.0.dev363/ansible/group_vars/all.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.0.dev363/ansible/roles/cli/tasks/clone.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 ---
 - name: Copy dev key
   ansible.builtin.copy:
     src: "{{ item.file }}"
-    dest: "/home/{{ master.user }}/.ssh/{{ item.file }}"
+    dest: "{{ master.home }}/.ssh/{{ item.file }}"
     mode: '{{ item.mode }}'
     owner: "{{ master.user }}"
     group: "{{ master.user }}"
   loop:
     - file: dev_key
       mode: "600"
     - file: dev_key.pub
       mode: "644"
   become_user: "{{ master.user }}"
   become: true
 
 - name: Ensure ssh config exist
   ansible.builtin.file:
-    path: "/home/{{ master.user }}/.ssh/config"
+    path: "{{ master.home }}/.ssh/config"
     state: touch
     mode: '0600'
     owner: "{{ master.user }}"
     group: "{{ master.user }}"
 
 - name: Enable Dev Key
   ansible.builtin.blockinfile:
     dest: "{{ item }}"
     block: |
       Host github.com
-        IdentityFile /home/{{ master.user }}/.ssh/dev_key
+        IdentityFile {{ master.home }}/.ssh/dev_key
         IdentitiesOnly yes
     marker: '# {mark} GIT configuration'
   loop:
-    - "/home/{{ master.user }}/.ssh/config"
+    - "{{ master.home }}/.ssh/config"
 
 - name: Git checkout talos cli
   ansible.builtin.git:
     repo: "{{ app.cli_repo }}"
     dest: "{{ app.clidir }}"
     version: main
     force: true
     update: true
   become_user: "{{ master.user }}"
   become: true
 
 - name: Remove dev key
   ansible.builtin.file:
-    path: "/home/{{ master.user }}/.ssh/{{ item }}"
+    path: "{{ master.home }}/.ssh/{{ item }}"
     state: absent
   loop:
     - dev_key
     - dev_key.pub
```

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.0.dev363/ansible/roles/cli/tasks/env.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 ---
 - name: Ensure bash-completion dir exist
   ansible.builtin.file:
-    path: "/home/{{ master.user }}/.bash_completion.d"
+    path: "{{ master.home }}/.bash_completion.d"
     state: directory
     mode: '0770'
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
 
 - name: Create talos directories
   ansible.builtin.file:
-    path: "/home/{{ master.user }}/.talos"
+    path: "{{ master.home }}/.talos"
     state: directory
     mode: '0770'
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
 
 - name: Copy env_talos templates
   ansible.builtin.template:
     src: "env_talos.j2"
-    dest: "/home/{{ master.user }}/.talos/env"
+    dest: "{{ master.home }}/.talos/env"
     mode: '0770'
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
 
 - name: "Ensure master.user env is sourced from the .bashrc"
   ansible.builtin.blockinfile:
-    dest: "/home/{{ master.user }}/.bashrc"
+    dest: "{{ master.home }}/.bashrc"
     block: |
       export PATH=$PATH:{{ app.clidir }}
-      source /home/{{ master.user }}/.talos/env
+      source {{ master.home }}/.talos/env
       if [[ -d ~/.bash_completion.d/ ]] && ! find ~/.bash_completion.d/. ! -name . -prune -exec false {} +
       then
         for f in ~/.bash_completion.d/*
         do
           source "$f"
         done
       fi
```

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.0.dev363/ansible/roles/cli/tasks/misc.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,55 +16,55 @@
     - "{{ app.etcdir }}/benchmarks"
     - "{{ app.logdir }}"
     - "{{ app.logdir }}/.tlist"
     - "{{ app.repodir }}"
     - "{{ app.etcdir }}/backup"
     - "{{ app.webdir }}/html/obj"
     - ~/MyPlaybooks
-    - "/home/{{ master.user }}/.talos"
+    - "{{ master.home }}/.talos"
 
 - name: Copy master ssh keys
   ansible.builtin.copy:
     src: "{{ item.origin }}"
     dest: "{{ item.dest }}"
     mode: "{{ item.mode }}"
     remote_src: true
     force: true
   loop:
-    - origin: "/home/{{ master.user }}/.ssh/id_rsa"
+    - origin: "{{ master.home }}/.ssh/id_rsa"
       dest: "{{ app.etcdir }}/backup/.master_rsa"
       mode: '0600'
-    - origin: "/home/{{ master.user }}/.ssh/id_rsa.pub"
+    - origin: "{{ master.home }}/.ssh/id_rsa.pub"
       dest: "{{ app.etcdir }}/backup/.master_rsa.pub"
       mode: '0644'
 
 - name: Configure Talos
   ansible.builtin.template:
     src: talos.conf.j2
     dest: "{{ app.etcdir }}/talos.conf"
     mode: '0660'
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
   when: talos_conf.use_default == 'true'
 
 - name: Generate CUSTOMER keypair
   community.crypto.openssh_keypair:
-    path: "/home/{{ master.user }}/.ssh/{{ item }}"
+    path: "{{ master.home }}/.ssh/{{ item }}"
     size: 2048
     type: rsa
     force: false
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
   loop:
     - CUSTOMER_CLI
   when: talos_conf.use_default == 'true'
 
 - name: Get CUSTOMER keypair
   ansible.builtin.fetch:
-    src: "/home/{{ master.user }}/.ssh/{{ item }}.pub"
+    src: "{{ master.home }}/.ssh/{{ item }}.pub"
     dest: "/tmp/{{ customer.name }}.{{ item }}.pub"
     flat: true
   loop:
     - CUSTOMER_CLI
   when: talos_conf.use_default == 'true'
 
 - name: Set Permissions
```

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.0.dev363/ansible/roles/cli/tasks/web.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.0.dev363/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.0.dev363/ansible/roles/cli/templates/cli.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.0.dev363/ansible/roles/cli/templates/env_talos.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.0.dev363/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.0.dev363/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.0.dev363/ansible/roles/cli/templates/talos.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.0.dev363/ansible/roles/common/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.0.dev363/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.0.dev363/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.0.dev363/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.0.dev363/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/install_ansible/templates/ansible.cfg.j2` & `talos_install-0.2.0.dev363/ansible/roles/install_ansible/templates/ansible.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.0.dev363/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/install_docker/tasks/main.yaml` & `talos_install-0.2.0.dev363/ansible/roles/install_docker/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.0.dev363/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/install_python/tasks/main.yaml` & `talos_install-0.2.0.dev363/ansible/roles/install_python/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 			<td class="infoBox">
 				<button type="button" class="btn btn-xs btn-default btn-noshadow"
 						ng-click="toggleDisplay()" ng-if="isCollapsable">
 					<span ng-hide="isPermanentlyCollapsed">&#x2227;</span>
 					<span ng-show="isPermanentlyCollapsed">&#x2228;</span>
 				</button>
 				<span class="infoBoxTitle">
-					{{decorationTitle}}
+					{{ decorationTitle }}
 				</span>
 				<div ng-hide="isCollapsed">
-					Last Updated: {{lastUpdate | date:'EEE dd MMM yyyy HH:mm:ss'}}
+					Last Updated: {{ lastUpdate | date:'EEE dd MMM yyyy HH:mm:ss' }}
 					<br>
-					TALOS: Nagios&reg; Core&trade; {{json.data.programstatus.version}} -
+					TALOS: Nagios&reg; Core&trade; {{ json.data.programstatus.version }} -
 	     			<br>
 					<span ng-show="updateInterval > 0">
-						Updated every {{updateInterval}} seconds
+						Updated every {{ updateInterval }} seconds
 						<br/>
 					</span>
 					<span ng-show="haveProgramStatus">
-						Logged in as <i>{{json.result.user}}</i>
+						Logged in as <i>{{ json.result.user }}</i>
 						<br>
 					</span>
 					<div class="infoBoxBadProcStatus"
 							ng-hide="haveProgramStatus">
 						Warning: Monitoring process may not be running!
 						<br/>
-						Click <a href="{{cgiurl}}extinfo.cgi?type=0">here</a>
+						Click <a href="{{ cgiurl }}extinfo.cgi?type=0">here</a>
 						for more info.
 					</div>
 					<!--div class="infoBoxBadProcStatus">
 						Warning: Could not read program status information!
 					</div-->
 					<div class="infoBoxBadProcStatus"
 							ng-show="notificationsDisabled()">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
- _______________________________________________________________
-| &#x2227; &#x2228;   {{decorationTitle}}                       |
-|Last Updated: {{lastUpdate | date:'EEE dd MMM yyyy HH:mm:ss'}} |
-|TALOS: Nagios® Core™ {{json.data.programstatus.version}} -  |
-| Updated every {{updateInterval}} seconds                      |
-|  Logged in as {{json.result.user}}                            |
-|Warning: Monitoring process may not be running!                |
-|Click here for more info.                                      |
-|- Notifications are disabled                                   |
-|-_Service_checks_are_disabled__________________________________|
+ _________________________________________________________________
+| &#x2227; &#x2228;   {{ decorationTitle }}                       |
+|Last Updated: {{ lastUpdate | date:'EEE dd MMM yyyy HH:mm:ss' }} |
+|TALOS: Nagios® Core™ {{ json.data.programstatus.version }} -  |
+| Updated every {{ updateInterval }} seconds                      |
+|  Logged in as {{ json.result.user }}                            |
+|Warning: Monitoring process may not be running!                  |
+|Click here for more info.                                        |
+|- Notifications are disabled                                     |
+|-_Service_checks_are_disabled____________________________________|
```

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.0.dev363/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.0.dev363/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.0.dev363/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.0.dev363/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.0.dev363/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.0.dev363/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files 17% similar despite different names*

```diff
@@ -71,30 +71,7 @@
 # Define a service to check the load on the local machine.
 define service{
   use                 local-service,graphed-service     ; Name of service template to use
   host_name           {{ inventory_hostname }}
   service_description LOAD
   check_command       check_local_load!15,25,30!35,40,50
 }
-
-# Define a service to check the swap usage the local machine.
-# Critical if less than 10% of swap is free, warning if less than 20% is free
-define service{
-  use                 local-service,graphed-service     ; Name of service template to use
-  host_name           {{ inventory_hostname }}
-  service_description SWAP_USAGE
-  check_command       check_local_swap!90!80
-}
-
-define service{
-  use                 local-service,graphed-service     ; Name of service template to use
-  host_name           {{ inventory_hostname }}
-  service_description WEB_AWX
-  check_command       check_website!"{{ ssh_ip }}:8080/#/login"
-}
-
-define service{
-  use                 local-service,graphed-service     ; Name of service template to use
-  host_name           {{ inventory_hostname }}
-  service_description WEB_ELK
-  check_command       check_website!"{{ ssh_ip }}:5601/app/home#/"
-}
```

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 .dcstats .table .title span { font-size: 0.6em; vertical-align: top;}
 .dcstats .table .title span:before { content:"  [ "; }
 .dcstats .table .title span:after { content:" ]";}
 .dcstats .table div {padding: 3px;}
 div#dcstats { display: table;}
 div#dcstats > div{ width: 100%;}
 div#dcstats .table + .table > div > div + div{white-space: pre; text-align: right;}
-.canvas {position: relative; background-repeat: no-repeat;}
+.canvas {position: relative; background-repeat: false-repeat;}
 .canvas img {position: absolute; top: 0; left: 0; z-index: 10;}
 .dcstats ~ #tt span {font-size: 1.5em; text-align: center; font-weight: bold;}
 .dcstats ~ #tt ul {list-style-type: none;}
 .dcstats ~ #tt ul li.red {background: url('../images/rs.png') left center no-repeat; line-height: 20px; padding-left: 20px;}
 .dcstats ~ #tt ul li.green {background: url('../images/gs.png') left center no-repeat; line-height: 20px; padding-left: 20px;}
 .dcstats ~ #tt ul li.yellow {background: url('../images/ys.png') left center no-repeat; line-height: 20px; padding-left: 20px;}
 .dcstats ~ #tt ul li.wtf {background: url('../images/us.png') left center no-repeat; line-height: 20px; padding-left: 20px;}
@@ -1010,15 +1010,15 @@
 	opacity: .4;
 	z-index: 5;
 }
 .imagem .preview > div > div:first-child {
 	background-size: contain;
 	height: 100px;
 	width: 100px;
-	background-repeat: no-repeat;
+	background-repeat: false-repeat;
 	background-position: center center;
 	margin: -1px auto 5px;
 	padding: 2px;
 }
 .preview .filename { max-width: 100px; word-break: break-all; }
 .imagem .heading { border-bottom: 1px solid; font-size: 2em; margin-bottom: 5px; text-align: right; }
```

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ----------------------------------*/
 
 /* states and images */
 .ui-icon {
 	display: block;
 	text-indent: -99999px;
 	overflow: hidden;
-	background-repeat: no-repeat;
+	background-repeat: false-repeat;
 }
 
 
 /* Misc visuals
 ----------------------------------*/
 
 /* Overlays */
```

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.0.dev363/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.0.dev363/ansible/roles/os_tune/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/cli.yaml` & `talos_install-0.2.0.dev363/ansible/roles/uninstall/tasks/cli.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.0.dev363/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.0.dev363/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.0.dev363/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/ansible/site.yaml` & `talos_install-0.2.0.dev363/ansible/site.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,16 @@
       become: true
       tags: ansible
       when: cli_action in ['deploy']
 
     - role: install_certificates
       become: true
       tags: certificates
-      when: cli_action in ['deploy']
-  
+      when: cli_action in ['build'] and ca_idm.enable == 'true'
+
     - role: common
       become: true
       tags: common
       when: cli_action in ['deploy']
 
     - role: cli
       become: true
```

### Comparing `talos_install-0.2.0.dev356/etc/talos.yaml` & `talos_install-0.2.0.dev363/etc/talos.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ---
 master:
   user: 'talos'
   group: 'talos'
-  uid: 3000
-  gid: 3000
+  uid: 1000
+  gid: 1000
   debug: false
-  password: 'Tpassword'
+  password: 'E4company!TM'
   mail: 'talosmaster@e4company.com'
+  home: '/usr/talos'
 
 guest:
   user: 'guest'
   password: 'guest'
 
 mgm_password: 'E4password!'
```

### Comparing `talos_install-0.2.0.dev356/setup.cfg` & `talos_install-0.2.0.dev363/setup.cfg`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/talos_install` & `talos_install-0.2.0.dev363/talos_install`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev356/talos_install.egg-info/PKG-INFO` & `talos_install-0.2.0.dev363/talos_install.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos-install
-Version: 0.2.0.dev356
+Version: 0.2.0.dev363
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `talos_install-0.2.0.dev356/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.0.dev363/talos_install.egg-info/SOURCES.txt`

 * *Files identical despite different names*

