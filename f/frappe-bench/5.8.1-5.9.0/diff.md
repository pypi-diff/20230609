# Comparing `tmp/frappe_bench-5.8.1-py2.py3-none-any.whl.zip` & `tmp/frappe_bench-5.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,167 +1,168 @@
-Zip file size: 147580 bytes, number of entries: 165
--rw-r--r--  2.0 unx      336 b- defN 22-Mar-22 07:40 bench/__init__.py
--rw-r--r--  2.0 unx    15458 b- defN 22-Mar-22 07:40 bench/app.py
--rw-r--r--  2.0 unx     9872 b- defN 22-Mar-22 07:40 bench/bench.py
--rw-r--r--  2.0 unx     5510 b- defN 22-Mar-22 07:40 bench/cli.py
--rw-r--r--  2.0 unx      431 b- defN 22-Mar-22 07:40 bench/exceptions.py
--rw-r--r--  2.0 unx     3224 b- defN 22-Mar-22 07:40 bench/prepare_beta_release.py
--rw-r--r--  2.0 unx    11453 b- defN 22-Mar-22 07:40 bench/release.py
--rw-r--r--  2.0 unx     3203 b- defN 22-Mar-22 07:40 bench/commands/__init__.py
--rw-r--r--  2.0 unx     2821 b- defN 22-Mar-22 07:40 bench/commands/config.py
--rw-r--r--  2.0 unx     1009 b- defN 22-Mar-22 07:40 bench/commands/git.py
--rw-r--r--  2.0 unx     3334 b- defN 22-Mar-22 07:40 bench/commands/install.py
--rw-r--r--  2.0 unx     5671 b- defN 22-Mar-22 07:40 bench/commands/make.py
--rw-r--r--  2.0 unx    11910 b- defN 22-Mar-22 07:40 bench/commands/setup.py
--rw-r--r--  2.0 unx     2738 b- defN 22-Mar-22 07:40 bench/commands/update.py
--rw-r--r--  2.0 unx     6745 b- defN 22-Mar-22 07:40 bench/commands/utils.py
--rw-r--r--  2.0 unx      189 b- defN 22-Mar-22 07:40 bench/config/__init__.py
--rw-r--r--  2.0 unx     3229 b- defN 22-Mar-22 07:40 bench/config/common_site_config.py
--rw-r--r--  2.0 unx     5437 b- defN 22-Mar-22 07:40 bench/config/lets_encrypt.py
--rw-r--r--  2.0 unx     8224 b- defN 22-Mar-22 07:40 bench/config/nginx.py
--rw-r--r--  2.0 unx      854 b- defN 22-Mar-22 07:40 bench/config/procfile.py
--rw-r--r--  2.0 unx     5481 b- defN 22-Mar-22 07:40 bench/config/production_setup.py
--rw-r--r--  2.0 unx     2732 b- defN 22-Mar-22 07:40 bench/config/redis.py
--rw-r--r--  2.0 unx     3548 b- defN 22-Mar-22 07:40 bench/config/site_config.py
--rw-r--r--  2.0 unx     4281 b- defN 22-Mar-22 07:40 bench/config/supervisor.py
--rw-r--r--  2.0 unx     9858 b- defN 22-Mar-22 07:40 bench/config/systemd.py
--rw-r--r--  2.0 unx     5444 b- defN 22-Mar-22 07:40 bench/config/templates/502.html
--rw-r--r--  2.0 unx     1412 b- defN 22-Mar-22 07:40 bench/config/templates/Procfile
--rw-r--r--  2.0 unx     2619 b- defN 22-Mar-22 07:40 bench/config/templates/bench_manager_nginx.conf
--rw-r--r--  2.0 unx      514 b- defN 22-Mar-22 07:40 bench/config/templates/frappe_sudoers
--rwxr-xr-x  2.0 unx      620 b- defN 22-Mar-22 07:40 bench/config/templates/letsencrypt.cfg
--rw-r--r--  2.0 unx     5722 b- defN 22-Mar-22 07:40 bench/config/templates/nginx.conf
--rw-r--r--  2.0 unx     1169 b- defN 22-Mar-22 07:40 bench/config/templates/nginx_default.conf
--rw-r--r--  2.0 unx      357 b- defN 22-Mar-22 07:40 bench/config/templates/redis_cache.conf
--rw-r--r--  2.0 unx      218 b- defN 22-Mar-22 07:40 bench/config/templates/redis_queue.conf
--rw-r--r--  2.0 unx      227 b- defN 22-Mar-22 07:40 bench/config/templates/redis_socketio.conf
--rw-r--r--  2.0 unx     6106 b- defN 22-Mar-22 07:40 bench/config/templates/supervisor.conf
--rw-r--r--  2.0 unx      352 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-frappe-default-worker.service
--rw-r--r--  2.0 unx      347 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-frappe-long-worker.service
--rw-r--r--  2.0 unx      333 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-frappe-schedule.service
--rw-r--r--  2.0 unx      348 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-frappe-short-worker.service
--rw-r--r--  2.0 unx      437 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-frappe-web.service
--rw-r--r--  2.0 unx      405 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-node-socketio.service
--rw-r--r--  2.0 unx      352 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-redis-cache.service
--rw-r--r--  2.0 unx      352 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-redis-queue.service
--rw-r--r--  2.0 unx      364 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-redis-socketio.service
--rw-r--r--  2.0 unx      186 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-redis.target
--rw-r--r--  2.0 unx      147 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-web.target
--rw-r--r--  2.0 unx       98 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench-workers.target
--rw-r--r--  2.0 unx      165 b- defN 22-Mar-22 07:40 bench/config/templates/systemd/frappe-bench.target
--rw-r--r--  2.0 unx      907 b- defN 22-Mar-22 07:40 bench/patches/__init__.py
--rw-r--r--  2.0 unx      346 b- defN 22-Mar-22 07:40 bench/patches/patches.txt
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-22 07:40 bench/patches/v3/__init__.py
--rw-r--r--  2.0 unx      915 b- defN 22-Mar-22 07:40 bench/patches/v3/celery_to_rq.py
--rw-r--r--  2.0 unx     1091 b- defN 22-Mar-22 07:40 bench/patches/v3/deprecate_old_config.py
--rw-r--r--  2.0 unx      328 b- defN 22-Mar-22 07:40 bench/patches/v3/redis_bind_ip.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-22 07:40 bench/patches/v4/__init__.py
--rw-r--r--  2.0 unx      140 b- defN 22-Mar-22 07:40 bench/patches/v4/install_yarn.py
--rw-r--r--  2.0 unx     1227 b- defN 22-Mar-22 07:40 bench/patches/v4/update_node.py
--rw-r--r--  2.0 unx      101 b- defN 22-Mar-22 07:40 bench/patches/v4/update_socketio.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-22 07:40 bench/patches/v5/__init__.py
--rw-r--r--  2.0 unx      426 b- defN 22-Mar-22 07:40 bench/patches/v5/fix_backup_cronjob.py
--rw-r--r--  2.0 unx     1786 b- defN 22-Mar-22 07:40 bench/patches/v5/fix_user_permissions.py
--rw-r--r--  2.0 unx      135 b- defN 22-Mar-22 07:40 bench/patches/v5/set_live_reload_config.py
--rw-r--r--  2.0 unx     1400 b- defN 22-Mar-22 07:40 bench/patches/v5/update_archived_sites.py
--rw-r--r--  2.0 unx      345 b- defN 22-Mar-22 07:40 bench/playbooks/README.md
--rw-r--r--  2.0 unx      649 b- defN 22-Mar-22 07:40 bench/playbooks/create_user.yml
--rw-r--r--  2.0 unx      882 b- defN 22-Mar-22 07:40 bench/playbooks/macosx.yml
--rw-r--r--  2.0 unx     2425 b- defN 22-Mar-22 07:40 bench/playbooks/site.yml
--rw-r--r--  2.0 unx      187 b- defN 22-Mar-22 07:40 bench/playbooks/vm_build.yml
--rw-r--r--  2.0 unx      115 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bash_screen_wall/files/screen_wall.sh
--rw-r--r--  2.0 unx      100 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bash_screen_wall/tasks/main.yml
--rw-r--r--  2.0 unx      428 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bench/tasks/change_ssh_port.yml
--rw-r--r--  2.0 unx     2278 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bench/tasks/main.yml
--rw-r--r--  2.0 unx      590 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bench/tasks/setup_bench_production.yml
--rw-r--r--  2.0 unx      983 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bench/tasks/setup_erpnext.yml
--rw-r--r--  2.0 unx     1424 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bench/tasks/setup_firewall.yml
--rw-r--r--  2.0 unx      247 b- defN 22-Mar-22 07:40 bench/playbooks/roles/bench/tasks/setup_inputrc.yml
--rw-r--r--  2.0 unx     1148 b- defN 22-Mar-22 07:40 bench/playbooks/roles/common/tasks/debian.yml
--rw-r--r--  2.0 unx     1158 b- defN 22-Mar-22 07:40 bench/playbooks/roles/common/tasks/debian_family.yml
--rw-r--r--  2.0 unx      862 b- defN 22-Mar-22 07:40 bench/playbooks/roles/common/tasks/macos.yml
--rw-r--r--  2.0 unx      236 b- defN 22-Mar-22 07:40 bench/playbooks/roles/common/tasks/main.yml
--rw-r--r--  2.0 unx      956 b- defN 22-Mar-22 07:40 bench/playbooks/roles/common/tasks/redhat_family.yml
--rw-r--r--  2.0 unx      896 b- defN 22-Mar-22 07:40 bench/playbooks/roles/common/tasks/ubuntu.yml
--rw-r--r--  2.0 unx       86 b- defN 22-Mar-22 07:40 bench/playbooks/roles/dns_caching/handlers/main.yml
--rw-r--r--  2.0 unx      463 b- defN 22-Mar-22 07:40 bench/playbooks/roles/dns_caching/tasks/main.yml
--rw-r--r--  2.0 unx       95 b- defN 22-Mar-22 07:40 bench/playbooks/roles/fail2ban/defaults/main.yml
--rw-r--r--  2.0 unx       69 b- defN 22-Mar-22 07:40 bench/playbooks/roles/fail2ban/handlers/main.yml
--rw-r--r--  2.0 unx      343 b- defN 22-Mar-22 07:40 bench/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
--rw-r--r--  2.0 unx      716 b- defN 22-Mar-22 07:40 bench/playbooks/roles/fail2ban/tasks/main.yml
--rw-r--r--  2.0 unx      542 b- defN 22-Mar-22 07:40 bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
--rw-r--r--  2.0 unx      295 b- defN 22-Mar-22 07:40 bench/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
--rw-r--r--  2.0 unx      848 b- defN 22-Mar-22 07:40 bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te
--rw-r--r--  2.0 unx      774 b- defN 22-Mar-22 07:40 bench/playbooks/roles/frappe_selinux/tasks/main.yml
--rw-r--r--  2.0 unx       49 b- defN 22-Mar-22 07:40 bench/playbooks/roles/locale/defaults/main.yml
--rw-r--r--  2.0 unx      768 b- defN 22-Mar-22 07:40 bench/playbooks/roles/locale/tasks/main.yml
--rw-r--r--  2.0 unx       67 b- defN 22-Mar-22 07:40 bench/playbooks/roles/logwatch/defaults/main.yml
--rw-r--r--  2.0 unx      410 b- defN 22-Mar-22 07:40 bench/playbooks/roles/logwatch/tasks/main.yml
--rw-r--r--  2.0 unx       61 b- defN 22-Mar-22 07:40 bench/playbooks/roles/logwatch/templates/logwatch.conf.j2
--rw-r--r--  2.0 unx      740 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/README.md
--rw-r--r--  2.0 unx       94 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/defaults/main.yml
--rw-r--r--  2.0 unx      294 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
--rw-r--r--  2.0 unx     1877 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/files/mariadb_config.cnf
--rw-r--r--  2.0 unx       64 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/handlers/main.yml
--rw-r--r--  2.0 unx      455 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/tasks/centos.yml
--rw-r--r--  2.0 unx     1333 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/tasks/debian.yml
--rw-r--r--  2.0 unx     2274 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/tasks/main.yml
--rw-r--r--  2.0 unx     1529 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
--rw-r--r--  2.0 unx      878 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
--rw-r--r--  2.0 unx      878 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
--rw-r--r--  2.0 unx      320 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
--rw-r--r--  2.0 unx      407 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
--rw-r--r--  2.0 unx      385 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
--rw-r--r--  2.0 unx       54 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/templates/my.cnf.j2
--rw-r--r--  2.0 unx      183 b- defN 22-Mar-22 07:40 bench/playbooks/roles/mariadb/vars/main.yml
--rw-r--r--  2.0 unx     4551 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/README.md
--rw-r--r--  2.0 unx     1238 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/defaults/main.yml
--rw-r--r--  2.0 unx       64 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/handlers/main.yml
--rw-r--r--  2.0 unx      379 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/meta/main.yml
--rw-r--r--  2.0 unx     1248 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/tasks/main.yml
--rw-r--r--  2.0 unx      666 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/tasks/setup-Debian.yml
--rw-r--r--  2.0 unx      237 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/tasks/setup-RedHat.yml
--rw-r--r--  2.0 unx      600 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/tasks/vhosts.yml
--rw-r--r--  2.0 unx     1916 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/templates/nginx.conf.j2
--rw-r--r--  2.0 unx      138 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/templates/nginx.repo.j2
--rw-r--r--  2.0 unx      626 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/templates/vhosts.j2
--rw-r--r--  2.0 unx       10 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/tests/inventory
--rw-r--r--  2.0 unx       77 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/tests/test.yml
--rw-r--r--  2.0 unx      131 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/vars/Debian.yml
--rw-r--r--  2.0 unx      119 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nginx/vars/RedHat.yml
--rw-r--r--  2.0 unx       24 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nodejs/defaults/main.yml
--rw-r--r--  2.0 unx      280 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nodejs/tasks/debian_family.yml
--rw-r--r--  2.0 unx      241 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nodejs/tasks/main.yml
--rw-r--r--  2.0 unx      307 b- defN 22-Mar-22 07:40 bench/playbooks/roles/nodejs/tasks/redhat_family.yml
--rw-r--r--  2.0 unx      548 b- defN 22-Mar-22 07:40 bench/playbooks/roles/ntpd/tasks/main.yml
--rw-r--r--  2.0 unx      100 b- defN 22-Mar-22 07:40 bench/playbooks/roles/packer/tasks/debian_family.yml
--rw-r--r--  2.0 unx     1225 b- defN 22-Mar-22 07:40 bench/playbooks/roles/packer/tasks/main.yml
--rw-r--r--  2.0 unx       81 b- defN 22-Mar-22 07:40 bench/playbooks/roles/packer/tasks/redhat_family.yml
--rw-r--r--  2.0 unx       58 b- defN 22-Mar-22 07:40 bench/playbooks/roles/psutil/tasks/main.yml
--rw-r--r--  2.0 unx      541 b- defN 22-Mar-22 07:40 bench/playbooks/roles/redis/tasks/main.yml
--rw-r--r--  2.0 unx      277 b- defN 22-Mar-22 07:40 bench/playbooks/roles/supervisor/tasks/main.yml
--rw-r--r--  2.0 unx       26 b- defN 22-Mar-22 07:40 bench/playbooks/roles/swap/defaults/main.yml
--rw-r--r--  2.0 unx      514 b- defN 22-Mar-22 07:40 bench/playbooks/roles/swap/tasks/main.yml
--rw-r--r--  2.0 unx       31 b- defN 22-Mar-22 07:40 bench/playbooks/roles/virtualbox/defaults/main.yml
--rw-r--r--  2.0 unx      258 b- defN 22-Mar-22 07:40 bench/playbooks/roles/virtualbox/files/virtualbox_centos.repo
--rw-r--r--  2.0 unx     1122 b- defN 22-Mar-22 07:40 bench/playbooks/roles/virtualbox/tasks/debian_family.yml
--rw-r--r--  2.0 unx      154 b- defN 22-Mar-22 07:40 bench/playbooks/roles/virtualbox/tasks/main.yml
--rw-r--r--  2.0 unx      428 b- defN 22-Mar-22 07:40 bench/playbooks/roles/virtualbox/tasks/redhat_family.yml
--rw-r--r--  2.0 unx     5717 b- defN 22-Mar-22 07:40 bench/playbooks/roles/wkhtmltopdf/tasks/main.yml
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-22 07:40 bench/tests/__init__.py
--rw-r--r--  2.0 unx     3724 b- defN 22-Mar-22 07:40 bench/tests/test_base.py
--rw-r--r--  2.0 unx     6459 b- defN 22-Mar-22 07:40 bench/tests/test_init.py
--rw-r--r--  2.0 unx     5530 b- defN 22-Mar-22 07:40 bench/tests/test_setup_production.py
--rw-r--r--  2.0 unx    12430 b- defN 22-Mar-22 07:40 bench/utils/__init__.py
--rw-r--r--  2.0 unx     6680 b- defN 22-Mar-22 07:40 bench/utils/app.py
--rw-r--r--  2.0 unx    17257 b- defN 22-Mar-22 07:40 bench/utils/bench.py
--rw-r--r--  2.0 unx     1582 b- defN 22-Mar-22 07:40 bench/utils/cli.py
--rw-r--r--  2.0 unx     2829 b- defN 22-Mar-22 07:40 bench/utils/render.py
--rw-r--r--  2.0 unx     4827 b- defN 22-Mar-22 07:40 bench/utils/system.py
--rw-r--r--  2.0 unx     1333 b- defN 22-Mar-22 07:40 bench/utils/translation.py
--rw-r--r--  2.0 unx    35121 b- defN 22-Mar-22 07:40 frappe_bench-5.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13246 b- defN 22-Mar-22 07:40 frappe_bench-5.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Mar-22 07:40 frappe_bench-5.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 22-Mar-22 07:40 frappe_bench-5.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Mar-22 07:40 frappe_bench-5.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    16055 b- defN 22-Mar-22 07:40 frappe_bench-5.8.1.dist-info/RECORD
-165 files, 349066 bytes uncompressed, 121356 bytes compressed:  65.2%
+Zip file size: 151620 bytes, number of entries: 166
+-rw-r--r--  2.0 unx      336 b- defN 22-Jun-08 08:03 bench/__init__.py
+-rw-r--r--  2.0 unx    19589 b- defN 22-Jun-08 08:02 bench/app.py
+-rw-r--r--  2.0 unx    12816 b- defN 22-Jun-08 08:02 bench/bench.py
+-rw-r--r--  2.0 unx     5510 b- defN 22-Jun-08 08:02 bench/cli.py
+-rw-r--r--  2.0 unx      527 b- defN 22-Jun-08 08:02 bench/exceptions.py
+-rw-r--r--  2.0 unx     3224 b- defN 22-Jun-08 08:02 bench/prepare_beta_release.py
+-rw-r--r--  2.0 unx    11453 b- defN 22-Jun-08 08:02 bench/release.py
+-rw-r--r--  2.0 unx     3203 b- defN 22-Jun-08 08:02 bench/commands/__init__.py
+-rw-r--r--  2.0 unx     2821 b- defN 22-Jun-08 08:02 bench/commands/config.py
+-rw-r--r--  2.0 unx     1009 b- defN 22-Jun-08 08:02 bench/commands/git.py
+-rw-r--r--  2.0 unx     3334 b- defN 22-Jun-08 08:02 bench/commands/install.py
+-rw-r--r--  2.0 unx     6058 b- defN 22-Jun-08 08:02 bench/commands/make.py
+-rw-r--r--  2.0 unx    11910 b- defN 22-Jun-08 08:02 bench/commands/setup.py
+-rw-r--r--  2.0 unx     2738 b- defN 22-Jun-08 08:02 bench/commands/update.py
+-rw-r--r--  2.0 unx     6745 b- defN 22-Jun-08 08:02 bench/commands/utils.py
+-rw-r--r--  2.0 unx      189 b- defN 22-Jun-08 08:02 bench/config/__init__.py
+-rw-r--r--  2.0 unx     3229 b- defN 22-Jun-08 08:02 bench/config/common_site_config.py
+-rw-r--r--  2.0 unx     5363 b- defN 22-Jun-08 08:02 bench/config/lets_encrypt.py
+-rw-r--r--  2.0 unx     8224 b- defN 22-Jun-08 08:02 bench/config/nginx.py
+-rw-r--r--  2.0 unx      854 b- defN 22-Jun-08 08:02 bench/config/procfile.py
+-rw-r--r--  2.0 unx     5481 b- defN 22-Jun-08 08:02 bench/config/production_setup.py
+-rw-r--r--  2.0 unx     2732 b- defN 22-Jun-08 08:02 bench/config/redis.py
+-rw-r--r--  2.0 unx     3548 b- defN 22-Jun-08 08:02 bench/config/site_config.py
+-rw-r--r--  2.0 unx     4281 b- defN 22-Jun-08 08:02 bench/config/supervisor.py
+-rw-r--r--  2.0 unx     9858 b- defN 22-Jun-08 08:02 bench/config/systemd.py
+-rw-r--r--  2.0 unx     5444 b- defN 22-Jun-08 08:02 bench/config/templates/502.html
+-rw-r--r--  2.0 unx     1412 b- defN 22-Jun-08 08:02 bench/config/templates/Procfile
+-rw-r--r--  2.0 unx     2619 b- defN 22-Jun-08 08:02 bench/config/templates/bench_manager_nginx.conf
+-rw-r--r--  2.0 unx      509 b- defN 22-Jun-08 08:02 bench/config/templates/frappe_sudoers
+-rwxr-xr-x  2.0 unx      620 b- defN 22-Jun-08 08:02 bench/config/templates/letsencrypt.cfg
+-rw-r--r--  2.0 unx     5777 b- defN 22-Jun-08 08:02 bench/config/templates/nginx.conf
+-rw-r--r--  2.0 unx     1169 b- defN 22-Jun-08 08:02 bench/config/templates/nginx_default.conf
+-rw-r--r--  2.0 unx      357 b- defN 22-Jun-08 08:02 bench/config/templates/redis_cache.conf
+-rw-r--r--  2.0 unx      218 b- defN 22-Jun-08 08:02 bench/config/templates/redis_queue.conf
+-rw-r--r--  2.0 unx      227 b- defN 22-Jun-08 08:02 bench/config/templates/redis_socketio.conf
+-rw-r--r--  2.0 unx     6106 b- defN 22-Jun-08 08:02 bench/config/templates/supervisor.conf
+-rw-r--r--  2.0 unx      352 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-frappe-default-worker.service
+-rw-r--r--  2.0 unx      347 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-frappe-long-worker.service
+-rw-r--r--  2.0 unx      333 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-frappe-schedule.service
+-rw-r--r--  2.0 unx      348 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-frappe-short-worker.service
+-rw-r--r--  2.0 unx      437 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-frappe-web.service
+-rw-r--r--  2.0 unx      405 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-node-socketio.service
+-rw-r--r--  2.0 unx      352 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-redis-cache.service
+-rw-r--r--  2.0 unx      352 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-redis-queue.service
+-rw-r--r--  2.0 unx      364 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-redis-socketio.service
+-rw-r--r--  2.0 unx      186 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-redis.target
+-rw-r--r--  2.0 unx      147 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-web.target
+-rw-r--r--  2.0 unx       98 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench-workers.target
+-rw-r--r--  2.0 unx      165 b- defN 22-Jun-08 08:02 bench/config/templates/systemd/frappe-bench.target
+-rw-r--r--  2.0 unx      907 b- defN 22-Jun-08 08:02 bench/patches/__init__.py
+-rw-r--r--  2.0 unx      346 b- defN 22-Jun-08 08:02 bench/patches/patches.txt
+-rw-r--r--  2.0 unx        0 b- defN 22-Jun-08 08:02 bench/patches/v3/__init__.py
+-rw-r--r--  2.0 unx      915 b- defN 22-Jun-08 08:02 bench/patches/v3/celery_to_rq.py
+-rw-r--r--  2.0 unx     1091 b- defN 22-Jun-08 08:02 bench/patches/v3/deprecate_old_config.py
+-rw-r--r--  2.0 unx      328 b- defN 22-Jun-08 08:02 bench/patches/v3/redis_bind_ip.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jun-08 08:02 bench/patches/v4/__init__.py
+-rw-r--r--  2.0 unx      140 b- defN 22-Jun-08 08:02 bench/patches/v4/install_yarn.py
+-rw-r--r--  2.0 unx     1227 b- defN 22-Jun-08 08:02 bench/patches/v4/update_node.py
+-rw-r--r--  2.0 unx      101 b- defN 22-Jun-08 08:02 bench/patches/v4/update_socketio.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jun-08 08:02 bench/patches/v5/__init__.py
+-rw-r--r--  2.0 unx      426 b- defN 22-Jun-08 08:02 bench/patches/v5/fix_backup_cronjob.py
+-rw-r--r--  2.0 unx     1786 b- defN 22-Jun-08 08:02 bench/patches/v5/fix_user_permissions.py
+-rw-r--r--  2.0 unx      135 b- defN 22-Jun-08 08:02 bench/patches/v5/set_live_reload_config.py
+-rw-r--r--  2.0 unx     1400 b- defN 22-Jun-08 08:02 bench/patches/v5/update_archived_sites.py
+-rw-r--r--  2.0 unx      345 b- defN 22-Jun-08 08:02 bench/playbooks/README.md
+-rw-r--r--  2.0 unx      649 b- defN 22-Jun-08 08:02 bench/playbooks/create_user.yml
+-rw-r--r--  2.0 unx      882 b- defN 22-Jun-08 08:02 bench/playbooks/macosx.yml
+-rw-r--r--  2.0 unx     2425 b- defN 22-Jun-08 08:02 bench/playbooks/site.yml
+-rw-r--r--  2.0 unx      187 b- defN 22-Jun-08 08:02 bench/playbooks/vm_build.yml
+-rw-r--r--  2.0 unx      115 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bash_screen_wall/files/screen_wall.sh
+-rw-r--r--  2.0 unx      100 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bash_screen_wall/tasks/main.yml
+-rw-r--r--  2.0 unx      428 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bench/tasks/change_ssh_port.yml
+-rw-r--r--  2.0 unx     2278 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bench/tasks/main.yml
+-rw-r--r--  2.0 unx      590 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bench/tasks/setup_bench_production.yml
+-rw-r--r--  2.0 unx      983 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bench/tasks/setup_erpnext.yml
+-rw-r--r--  2.0 unx     1424 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bench/tasks/setup_firewall.yml
+-rw-r--r--  2.0 unx      247 b- defN 22-Jun-08 08:02 bench/playbooks/roles/bench/tasks/setup_inputrc.yml
+-rw-r--r--  2.0 unx     1148 b- defN 22-Jun-08 08:02 bench/playbooks/roles/common/tasks/debian.yml
+-rw-r--r--  2.0 unx     1158 b- defN 22-Jun-08 08:02 bench/playbooks/roles/common/tasks/debian_family.yml
+-rw-r--r--  2.0 unx      862 b- defN 22-Jun-08 08:02 bench/playbooks/roles/common/tasks/macos.yml
+-rw-r--r--  2.0 unx      236 b- defN 22-Jun-08 08:02 bench/playbooks/roles/common/tasks/main.yml
+-rw-r--r--  2.0 unx      956 b- defN 22-Jun-08 08:02 bench/playbooks/roles/common/tasks/redhat_family.yml
+-rw-r--r--  2.0 unx      896 b- defN 22-Jun-08 08:02 bench/playbooks/roles/common/tasks/ubuntu.yml
+-rw-r--r--  2.0 unx       86 b- defN 22-Jun-08 08:02 bench/playbooks/roles/dns_caching/handlers/main.yml
+-rw-r--r--  2.0 unx      463 b- defN 22-Jun-08 08:02 bench/playbooks/roles/dns_caching/tasks/main.yml
+-rw-r--r--  2.0 unx       95 b- defN 22-Jun-08 08:02 bench/playbooks/roles/fail2ban/defaults/main.yml
+-rw-r--r--  2.0 unx       69 b- defN 22-Jun-08 08:02 bench/playbooks/roles/fail2ban/handlers/main.yml
+-rw-r--r--  2.0 unx      343 b- defN 22-Jun-08 08:02 bench/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
+-rw-r--r--  2.0 unx      716 b- defN 22-Jun-08 08:02 bench/playbooks/roles/fail2ban/tasks/main.yml
+-rw-r--r--  2.0 unx      542 b- defN 22-Jun-08 08:02 bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
+-rw-r--r--  2.0 unx      295 b- defN 22-Jun-08 08:02 bench/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
+-rw-r--r--  2.0 unx      848 b- defN 22-Jun-08 08:02 bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te
+-rw-r--r--  2.0 unx      774 b- defN 22-Jun-08 08:02 bench/playbooks/roles/frappe_selinux/tasks/main.yml
+-rw-r--r--  2.0 unx       49 b- defN 22-Jun-08 08:02 bench/playbooks/roles/locale/defaults/main.yml
+-rw-r--r--  2.0 unx      768 b- defN 22-Jun-08 08:02 bench/playbooks/roles/locale/tasks/main.yml
+-rw-r--r--  2.0 unx       67 b- defN 22-Jun-08 08:02 bench/playbooks/roles/logwatch/defaults/main.yml
+-rw-r--r--  2.0 unx      410 b- defN 22-Jun-08 08:02 bench/playbooks/roles/logwatch/tasks/main.yml
+-rw-r--r--  2.0 unx       61 b- defN 22-Jun-08 08:02 bench/playbooks/roles/logwatch/templates/logwatch.conf.j2
+-rw-r--r--  2.0 unx      740 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/README.md
+-rw-r--r--  2.0 unx       94 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/defaults/main.yml
+-rw-r--r--  2.0 unx      294 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
+-rw-r--r--  2.0 unx     1877 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/files/mariadb_config.cnf
+-rw-r--r--  2.0 unx       64 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/handlers/main.yml
+-rw-r--r--  2.0 unx      455 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/tasks/centos.yml
+-rw-r--r--  2.0 unx     1333 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/tasks/debian.yml
+-rw-r--r--  2.0 unx     2274 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/tasks/main.yml
+-rw-r--r--  2.0 unx     1529 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
+-rw-r--r--  2.0 unx      878 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
+-rw-r--r--  2.0 unx      878 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
+-rw-r--r--  2.0 unx      320 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
+-rw-r--r--  2.0 unx      407 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
+-rw-r--r--  2.0 unx      385 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
+-rw-r--r--  2.0 unx       54 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/templates/my.cnf.j2
+-rw-r--r--  2.0 unx      183 b- defN 22-Jun-08 08:02 bench/playbooks/roles/mariadb/vars/main.yml
+-rw-r--r--  2.0 unx     4551 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/README.md
+-rw-r--r--  2.0 unx     1238 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/defaults/main.yml
+-rw-r--r--  2.0 unx       64 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/handlers/main.yml
+-rw-r--r--  2.0 unx      379 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/meta/main.yml
+-rw-r--r--  2.0 unx     1248 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/tasks/main.yml
+-rw-r--r--  2.0 unx      666 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/tasks/setup-Debian.yml
+-rw-r--r--  2.0 unx      237 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/tasks/setup-RedHat.yml
+-rw-r--r--  2.0 unx      600 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/tasks/vhosts.yml
+-rw-r--r--  2.0 unx     1916 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/templates/nginx.conf.j2
+-rw-r--r--  2.0 unx      138 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/templates/nginx.repo.j2
+-rw-r--r--  2.0 unx      626 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/templates/vhosts.j2
+-rw-r--r--  2.0 unx       10 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/tests/inventory
+-rw-r--r--  2.0 unx       77 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/tests/test.yml
+-rw-r--r--  2.0 unx      131 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/vars/Debian.yml
+-rw-r--r--  2.0 unx      119 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nginx/vars/RedHat.yml
+-rw-r--r--  2.0 unx       24 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nodejs/defaults/main.yml
+-rw-r--r--  2.0 unx      280 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nodejs/tasks/debian_family.yml
+-rw-r--r--  2.0 unx      241 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nodejs/tasks/main.yml
+-rw-r--r--  2.0 unx      307 b- defN 22-Jun-08 08:02 bench/playbooks/roles/nodejs/tasks/redhat_family.yml
+-rw-r--r--  2.0 unx      548 b- defN 22-Jun-08 08:02 bench/playbooks/roles/ntpd/tasks/main.yml
+-rw-r--r--  2.0 unx      100 b- defN 22-Jun-08 08:02 bench/playbooks/roles/packer/tasks/debian_family.yml
+-rw-r--r--  2.0 unx     1225 b- defN 22-Jun-08 08:02 bench/playbooks/roles/packer/tasks/main.yml
+-rw-r--r--  2.0 unx       81 b- defN 22-Jun-08 08:02 bench/playbooks/roles/packer/tasks/redhat_family.yml
+-rw-r--r--  2.0 unx       58 b- defN 22-Jun-08 08:02 bench/playbooks/roles/psutil/tasks/main.yml
+-rw-r--r--  2.0 unx      541 b- defN 22-Jun-08 08:02 bench/playbooks/roles/redis/tasks/main.yml
+-rw-r--r--  2.0 unx      277 b- defN 22-Jun-08 08:02 bench/playbooks/roles/supervisor/tasks/main.yml
+-rw-r--r--  2.0 unx       26 b- defN 22-Jun-08 08:02 bench/playbooks/roles/swap/defaults/main.yml
+-rw-r--r--  2.0 unx      514 b- defN 22-Jun-08 08:02 bench/playbooks/roles/swap/tasks/main.yml
+-rw-r--r--  2.0 unx       31 b- defN 22-Jun-08 08:02 bench/playbooks/roles/virtualbox/defaults/main.yml
+-rw-r--r--  2.0 unx      258 b- defN 22-Jun-08 08:02 bench/playbooks/roles/virtualbox/files/virtualbox_centos.repo
+-rw-r--r--  2.0 unx     1122 b- defN 22-Jun-08 08:02 bench/playbooks/roles/virtualbox/tasks/debian_family.yml
+-rw-r--r--  2.0 unx      154 b- defN 22-Jun-08 08:02 bench/playbooks/roles/virtualbox/tasks/main.yml
+-rw-r--r--  2.0 unx      428 b- defN 22-Jun-08 08:02 bench/playbooks/roles/virtualbox/tasks/redhat_family.yml
+-rw-r--r--  2.0 unx     5717 b- defN 22-Jun-08 08:02 bench/playbooks/roles/wkhtmltopdf/tasks/main.yml
+-rw-r--r--  2.0 unx        0 b- defN 22-Jun-08 08:02 bench/tests/__init__.py
+-rw-r--r--  2.0 unx     3724 b- defN 22-Jun-08 08:02 bench/tests/test_base.py
+-rw-r--r--  2.0 unx     7196 b- defN 22-Jun-08 08:02 bench/tests/test_init.py
+-rw-r--r--  2.0 unx     5530 b- defN 22-Jun-08 08:02 bench/tests/test_setup_production.py
+-rw-r--r--  2.0 unx     2526 b- defN 22-Jun-08 08:02 bench/tests/test_utils.py
+-rw-r--r--  2.0 unx    13421 b- defN 22-Jun-08 08:02 bench/utils/__init__.py
+-rw-r--r--  2.0 unx     7866 b- defN 22-Jun-08 08:02 bench/utils/app.py
+-rw-r--r--  2.0 unx    17401 b- defN 22-Jun-08 08:02 bench/utils/bench.py
+-rw-r--r--  2.0 unx     1582 b- defN 22-Jun-08 08:02 bench/utils/cli.py
+-rw-r--r--  2.0 unx     2829 b- defN 22-Jun-08 08:02 bench/utils/render.py
+-rw-r--r--  2.0 unx     5093 b- defN 22-Jun-08 08:02 bench/utils/system.py
+-rw-r--r--  2.0 unx     1333 b- defN 22-Jun-08 08:02 bench/utils/translation.py
+-rw-r--r--  2.0 unx    35121 b- defN 22-Jun-08 08:03 frappe_bench-5.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13145 b- defN 22-Jun-08 08:03 frappe_bench-5.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Jun-08 08:03 frappe_bench-5.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 22-Jun-08 08:03 frappe_bench-5.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 22-Jun-08 08:03 frappe_bench-5.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    16138 b- defN 22-Jun-08 08:03 frappe_bench-5.9.0.dist-info/RECORD
+166 files, 362432 bytes uncompressed, 125270 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -450,14 +450,17 @@
 
 Filename: bench/tests/test_init.py
 Comment: 
 
 Filename: bench/tests/test_setup_production.py
 Comment: 
 
+Filename: bench/tests/test_utils.py
+Comment: 
+
 Filename: bench/utils/__init__.py
 Comment: 
 
 Filename: bench/utils/app.py
 Comment: 
 
 Filename: bench/utils/bench.py
@@ -471,26 +474,26 @@
 
 Filename: bench/utils/system.py
 Comment: 
 
 Filename: bench/utils/translation.py
 Comment: 
 
-Filename: frappe_bench-5.8.1.dist-info/LICENSE
+Filename: frappe_bench-5.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: frappe_bench-5.8.1.dist-info/METADATA
+Filename: frappe_bench-5.9.0.dist-info/METADATA
 Comment: 
 
-Filename: frappe_bench-5.8.1.dist-info/WHEEL
+Filename: frappe_bench-5.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: frappe_bench-5.8.1.dist-info/entry_points.txt
+Filename: frappe_bench-5.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: frappe_bench-5.8.1.dist-info/top_level.txt
+Filename: frappe_bench-5.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: frappe_bench-5.8.1.dist-info/RECORD
+Filename: frappe_bench-5.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bench/__init__.py

```diff
@@ -1,8 +1,8 @@
-VERSION = "5.8.1"
+VERSION = "5.9.0"
 PROJECT_NAME = "frappe-bench"
 FRAPPE_VERSION = None
 current_path = None
 updated_path = None
 LOG_BUFFER = []
```

## bench/app.py

```diff
@@ -4,28 +4,32 @@
 import logging
 import os
 import re
 import shutil
 import subprocess
 import sys
 import typing
+from collections import OrderedDict
 from datetime import date
 from urllib.parse import urlparse
+import os
 
 # imports - third party imports
 import click
+from git import Repo
 
 # imports - module imports
 import bench
 from bench.exceptions import NotInBenchDirectoryError
 from bench.utils import (
 	fetch_details_from_tag,
 	get_available_folder_name,
 	is_bench_directory,
 	is_git_url,
+	is_valid_frappe_branch,
 	log,
 	run_frappe_cmd,
 )
 from bench.utils.bench import (
 	build_assets,
 	install_python_dev_dependencies,
 )
@@ -51,89 +55,96 @@
 		References for Version Identifiers:
 		 * https://www.python.org/dev/peps/pep-0440/#version-specifiers
 		 * https://docs.npmjs.com/about-semantic-versioning
 
 		class Healthcare(AppConfig):
 			dependencies = [{"frappe/erpnext": "~13.17.0"}]
 		"""
-		self.name = name.rstrip('/')
+		self.name = name.rstrip("/")
 		self.remote_server = "github.com"
 		self.to_clone = to_clone
 		self.on_disk = False
 		self.use_ssh = False
 		self.from_apps = False
 		self.is_url = False
 		self.branch = branch
+		self.app_name = None
+		self.git_repo = None
 		self.mount_path = os.path.abspath(
 			os.path.join(urlparse(self.name).netloc, urlparse(self.name).path)
 		)
 		self.setup_details()
 
 	def setup_details(self):
 		# fetch meta from installed apps
-		if (
-			not self.to_clone
-			and hasattr(self, "bench")
-			and os.path.exists(os.path.join(self.bench.name, "apps", self.name))
+		if self.bench and os.path.exists(
+			os.path.join(self.bench.name, "apps", self.name)
 		):
+			self.mount_path = os.path.join(self.bench.name, "apps", self.name)
 			self.from_apps = True
-			self._setup_details_from_installed_apps()
+			self._setup_details_from_mounted_disk()
 
 		# fetch meta for repo on mounted disk
 		elif os.path.exists(self.mount_path):
 			self.on_disk = True
 			self._setup_details_from_mounted_disk()
 
 		# fetch meta for repo from remote git server - traditional get-app url
 		elif is_git_url(self.name):
 			self.is_url = True
-			if self.name.startswith("git@") or self.name.startswith("ssh://"):
-				self.use_ssh = True
 			self._setup_details_from_git_url()
 
 		# fetch meta from new styled name tags & first party apps on github
 		else:
 			self._setup_details_from_name_tag()
 
+		if self.git_repo:
+			self.app_name = os.path.basename(
+				os.path.normpath(self.git_repo.working_tree_dir)
+			)
+		else:
+			self.app_name = self.repo
+
 	def _setup_details_from_mounted_disk(self):
-		self.org, self.repo, self.tag = os.path.split(self.mount_path)[-2:] + (
-			self.branch,
-		)
+		# If app is a git repo
+		self.git_repo = Repo(self.mount_path)
+		try:
+			self._setup_details_from_git_url(self.git_repo.remotes[0].url)
+			if not (self.branch or self.tag):
+				self.tag = self.branch = self.git_repo.active_branch.name
+		except IndexError:
+			self.org, self.repo, self.tag = os.path.split(self.mount_path)[-2:] + (self.branch,)
+		except TypeError:
+			# faced a "a detached symbolic reference as it points" in case you're in the middle of
+			# some git shenanigans
+			self.tag = self.branch = None
 
 	def _setup_details_from_name_tag(self):
 		self.org, self.repo, self.tag = fetch_details_from_tag(self.name)
 		self.tag = self.tag or self.branch
 
-	def _setup_details_from_installed_apps(self):
-		self.org, self.repo, self.tag = os.path.split(
-			os.path.join(self.bench.name, "apps", self.name)
-		)[-2:] + (self.branch,)
+	def _setup_details_from_git_url(self, url=None):
+		return self.__setup_details_from_git(url)
 
-	def _setup_details_from_git_url(self):
-		return self.__setup_details_from_git()
-
-	def __setup_details_from_git(self):
-		if self.use_ssh:
-			_first_part, _second_part = self.name.split(":")
+	def __setup_details_from_git(self, url=None):
+		name = url if url else self.name
+		if name.startswith("git@") or name.startswith("ssh://"):
+			self.use_ssh = True
+			_first_part, _second_part = name.rsplit(":", 1)
 			self.remote_server = _first_part.split("@")[-1]
 			self.org, _repo = _second_part.rsplit("/", 1)
 		else:
-			self.remote_server, self.org, _repo = self.name.rsplit("/", 2)
+			protocal = "https://" if "https://" in name else "http://"
+			self.remote_server, self.org, _repo = name.replace(protocal, "").rsplit("/", 2)
 
 		self.tag = self.branch
 		self.repo = _repo.split(".")[0]
 
 	@property
 	def url(self):
-		if self.from_apps:
-			return os.path.abspath(os.path.join("apps", self.name))
-
-		if self.on_disk:
-			return self.mount_path
-
 		if self.is_url:
 			return self.name
 
 		if self.use_ssh:
 			return self.get_ssh_url()
 
 		return self.get_http_url()
@@ -143,18 +154,18 @@
 
 	def get_ssh_url(self):
 		return f"git@{self.remote_server}:{self.org}/{self.repo}.git"
 
 
 @functools.lru_cache(maxsize=None)
 class App(AppMeta):
-	def __init__(
-		self, name: str, branch: str = None, bench: "Bench" = None, *args, **kwargs
-	):
+	def __init__(self, name: str, branch: str = None, bench: "Bench" = None, *args, **kwargs):
 		self.bench = bench
+		self.required_by = None
+		self.local_resolution = []
 		super().__init__(name, branch, *args, **kwargs)
 
 	@step(title="Fetching App {repo}", success="App {repo} Fetched")
 	def get(self):
 		branch = f"--branch {self.tag}" if self.tag else ""
 		shallow = "--depth 1" if self.bench.shallow_clone else ""
 
@@ -164,52 +175,108 @@
 
 		self.bench.run(
 			f"git clone {self.url} {branch} {shallow} --origin upstream",
 			cwd=os.path.join(self.bench.name, "apps"),
 		)
 
 	@step(title="Archiving App {repo}", success="App {repo} Archived")
-	def remove(self):
-		active_app_path = os.path.join("apps", self.repo)
-		archived_path = os.path.join("archived", "apps")
-		archived_name = get_available_folder_name(
-			f"{self.repo}-{date.today()}", archived_path
-		)
-		archived_app_path = os.path.join(archived_path, archived_name)
-		log(f"App moved from {active_app_path} to {archived_app_path}")
-		shutil.move(active_app_path, archived_app_path)
+	def remove(self, no_backup: bool = False):
+		active_app_path = os.path.join("apps", self.name)
+
+		if no_backup:
+			shutil.rmtree(active_app_path)
+			log(f"App deleted from {active_app_path}")
+		else:
+			archived_path = os.path.join("archived", "apps")
+			archived_name = get_available_folder_name(f"{self.repo}-{date.today()}", archived_path)
+			archived_app_path = os.path.join(archived_path, archived_name)
+
+			shutil.move(active_app_path, archived_app_path)
+			log(f"App moved from {active_app_path} to {archived_app_path}")
 
 	@step(title="Installing App {repo}", success="App {repo} Installed")
-	def install(self, skip_assets=False, verbose=False, restart_bench=True):
+	def install(
+		self,
+		skip_assets=False,
+		verbose=False,
+		resolved=False,
+		restart_bench=True,
+		ignore_resolution=False,
+	):
 		import bench.cli
 		from bench.utils.app import get_app_name
 
 		verbose = bench.cli.verbose or verbose
-		app_name = get_app_name(self.bench.name, self.repo)
-
-		# TODO: this should go inside install_app only tho - issue: default/resolved branch
-		setup_app_dependencies(
-			repo_name=self.repo,
-			bench_path=self.bench.name,
-			branch=self.tag,
-			verbose=verbose,
-			skip_assets=skip_assets,
-		)
+		app_name = get_app_name(self.bench.name, self.app_name)
+		if not resolved and self.repo != "frappe" and not ignore_resolution:
+			click.secho(
+				f"Ignoring dependencies of {self.name}. To install dependencies use --resolve-deps",
+				fg="yellow",
+			)
 
 		install_app(
 			app=app_name,
+			tag=self.tag,
 			bench_path=self.bench.name,
 			verbose=verbose,
 			skip_assets=skip_assets,
-			restart_bench=restart_bench
+			restart_bench=restart_bench,
+			resolution=self.local_resolution
 		)
 
+	@step(title="Cloning and installing {repo}", success="App {repo} Installed")
+	def install_resolved_apps(self, *args, **kwargs):
+		self.get()
+		self.install(*args, **kwargs, resolved=True)
+
 	@step(title="Uninstalling App {repo}", success="App {repo} Uninstalled")
 	def uninstall(self):
-		self.bench.run(f"{self.bench.python} -m pip uninstall -y {self.repo}")
+		self.bench.run(f"{self.bench.python} -m pip uninstall -y {self.name}")
+
+	def _get_dependencies(self):
+		from bench.utils.app import get_required_deps, required_apps_from_hooks
+
+		if self.on_disk:
+			required_deps = os.path.join(self.mount_path, self.repo,'hooks.py')
+			try:
+				return required_apps_from_hooks(required_deps, local=True)
+			except IndexError:
+				return []
+		try:
+			required_deps = get_required_deps(self.org, self.repo, self.tag or self.branch)
+			return required_apps_from_hooks(required_deps)
+		except Exception:
+			return []
+
+	def update_app_state(self):
+		from bench.bench import Bench
+		bench = Bench(self.bench.name)
+		bench.apps.sync(app_dir=self.app_name, app_name=self.name,
+						branch=self.tag, required_list=self.local_resolution)
+
+
+
+def make_resolution_plan(app: App, bench: "Bench"):
+	"""
+	decide what apps and versions to install and in what order
+	"""
+	resolution = OrderedDict()
+	resolution[app.repo] = app
+
+	for app_name in app._get_dependencies():
+		dep_app = App(app_name, bench=bench)
+		is_valid_frappe_branch(dep_app.url, dep_app.branch)
+		dep_app.required_by = app.name
+		if dep_app.repo in resolution:
+			click.secho(f"{dep_app.repo} is already resolved skipping", fg="yellow")
+			continue
+		resolution[dep_app.repo] = dep_app
+		resolution.update(make_resolution_plan(dep_app, bench))
+		app.local_resolution = [repo_name for repo_name, _ in reversed(resolution.items())]
+	return resolution
 
 
 def add_to_appstxt(app, bench_path="."):
 	from bench.bench import Bench
 
 	apps = Bench(bench_path).apps
 
@@ -260,96 +327,94 @@
 def remove_from_excluded_apps_txt(app, bench_path="."):
 	apps = get_excluded_apps(bench_path=bench_path)
 	if app in apps:
 		apps.remove(app)
 		return write_excluded_apps_txt(apps, bench_path=bench_path)
 
 
-def setup_app_dependencies(
-	repo_name, bench_path=".", branch=None, skip_assets=False, verbose=False
-):
-	# branch kwarg is somewhat of a hack here; since we're assuming the same branches for all apps
-	# for eg: if you're installing erpnext@develop, you'll want frappe@develop and healthcare@develop too
-	import glob
-	import bench.cli
-	from bench.bench import Bench
-
-	verbose = bench.cli.verbose or verbose
-	apps_path = os.path.join(os.path.abspath(bench_path), "apps")
-	files = glob.glob(os.path.join(apps_path, repo_name, "**", "hooks.py"))
-
-	if files:
-		with open(files[0]) as f:
-			lines = [x for x in f.read().split("\n") if x.strip().startswith("required_apps")]
-		if lines:
-			required_apps = eval(lines[0].strip("required_apps").strip().lstrip("=").strip())
-			# TODO: when the time comes, add version check here
-			for app in required_apps:
-				if app not in Bench(bench_path).apps:
-					get_app(
-						app,
-						bench_path=bench_path,
-						branch=branch,
-						skip_assets=skip_assets,
-						verbose=verbose,
-					)
-
-
 def get_app(
 	git_url,
 	branch=None,
 	bench_path=".",
 	skip_assets=False,
 	verbose=False,
 	overwrite=False,
 	init_bench=False,
+	resolve_deps=False,
 ):
 	"""bench get-app clones a Frappe App from remote (GitHub or any other git server),
 	and installs it on the current bench. This also resolves dependencies based on the
 	apps' required_apps defined in the hooks.py file.
 
 	If the bench_path is not a bench directory, a new bench is created named using the
 	git_url parameter.
 	"""
-	from bench.bench import Bench
 	import bench as _bench
 	import bench.cli as bench_cli
+	from bench.bench import Bench
+	from bench.utils.app import check_existing_dir
 
 	bench = Bench(bench_path)
 	app = App(git_url, branch=branch, bench=bench)
 	git_url = app.url
 	repo_name = app.repo
 	branch = app.tag
 	bench_setup = False
 	restart_bench = not init_bench
+	frappe_path, frappe_branch = None, None
+
+	if resolve_deps:
+		resolution = make_resolution_plan(app, bench)
+		click.secho("Following apps will be installed", fg="bright_blue")
+		for idx, app in enumerate(reversed(resolution.values()), start=1):
+			print(f"{idx}. {app.name} {f'(required by {app.required_by})' if app.required_by else ''}")
+
+		if "frappe" in resolution:
+			# Todo: Make frappe a terminal dependency for all frappe apps.
+			frappe_path, frappe_branch = resolution["frappe"].url, resolution["frappe"].tag
 
 	if not is_bench_directory(bench_path):
 		if not init_bench:
 			raise NotInBenchDirectoryError(
 				f"{os.path.realpath(bench_path)} is not a valid bench directory. "
 				"Run with --init-bench if you'd like to create a Bench too."
 			)
 
 		from bench.utils.system import init
 
 		bench_path = get_available_folder_name(f"{app.repo}-bench", bench_path)
-		init(path=bench_path, frappe_branch=branch)
+		init(
+			path=bench_path,
+			frappe_path=frappe_path,
+			frappe_branch=frappe_branch if frappe_branch else branch,
+		)
 		os.chdir(bench_path)
 		bench_setup = True
 
 	if bench_setup and bench_cli.from_command_line and bench_cli.dynamic_feed:
-		_bench.LOG_BUFFER.append({
-			"message": f"Fetching App {repo_name}",
-			"prefix": click.style('⏼', fg='bright_yellow'),
-			"is_parent": True,
-			"color": None,
-		})
+		_bench.LOG_BUFFER.append(
+			{
+				"message": f"Fetching App {repo_name}",
+				"prefix": click.style("⏼", fg="bright_yellow"),
+				"is_parent": True,
+				"color": None,
+			}
+		)
+
+	if resolve_deps:
+		install_resolved_deps(
+			bench,
+			resolution,
+			bench_path=bench_path,
+			skip_assets=skip_assets,
+			verbose=verbose,
+		)
+		return
 
-	cloned_path = os.path.join(bench_path, "apps", repo_name)
-	dir_already_exists = os.path.isdir(cloned_path)
+	dir_already_exists, cloned_path = check_existing_dir(bench_path, repo_name)
 	to_clone = not dir_already_exists
 
 	# application directory already exists
 	# prompt user to overwrite it
 	if dir_already_exists and (
 		overwrite
 		or click.confirm(
@@ -367,45 +432,114 @@
 		to_clone
 		or overwrite
 		or click.confirm("Do you want to reinstall the existing application?")
 	):
 		app.install(verbose=verbose, skip_assets=skip_assets, restart_bench=restart_bench)
 
 
+def install_resolved_deps(
+	bench,
+	resolution,
+	bench_path=".",
+	skip_assets=False,
+	verbose=False,
+):
+	from bench.utils.app import check_existing_dir
+
+	if "frappe" in resolution:
+		# Terminal dependency
+		del resolution["frappe"]
+
+	for repo_name, app in reversed(resolution.items()):
+		existing_dir, path_to_app = check_existing_dir(bench_path, repo_name)
+		if existing_dir:
+			is_compatible = False
+
+			try:
+				installed_branch = bench.apps.states[repo_name]["resolution"]["branch"].strip()
+			except Exception:
+				installed_branch = (
+					subprocess.
+					check_output("git rev-parse --abbrev-ref HEAD", shell=True, cwd=path_to_app)
+					.decode("utf-8")
+					.rstrip()
+					)
+			try:
+				if app.tag is None:
+					current_remote = (
+						subprocess.check_output(f"git config branch.{installed_branch}.remote", shell=True, cwd=path_to_app)
+						.decode("utf-8")
+						.rstrip()
+					)
+
+					default_branch = (
+						subprocess.check_output(
+							f"git symbolic-ref refs/remotes/{current_remote}/HEAD", shell=True, cwd=path_to_app
+						)
+						.decode("utf-8")
+						.rsplit("/")[-1]
+						.strip()
+					)
+					is_compatible = default_branch == installed_branch
+				else:
+					is_compatible = installed_branch == app.tag
+			except Exception:
+				is_compatible = False
+
+			prefix = 'C' if is_compatible else 'Inc'
+			click.secho(
+				f"{prefix}ompatible version of {repo_name} is already installed",
+				fg="green" if is_compatible else "red",
+			)
+			app.update_app_state()
+			if click.confirm(
+				f"Do you wish to clone and install the already installed {prefix}ompatible app"
+			):
+				click.secho(f"Removing installed app {app.name}", fg="yellow")
+				shutil.rmtree(path_to_app)
+			else:
+				continue
+		app.install_resolved_apps(skip_assets=skip_assets, verbose=verbose)
+
+
 def new_app(app, no_git=None, bench_path="."):
 	if bench.FRAPPE_VERSION in (0, None):
-		raise NotInBenchDirectoryError(
-			f"{os.path.realpath(bench_path)} is not a valid bench directory."
-		)
+		raise NotInBenchDirectoryError(f"{os.path.realpath(bench_path)} is not a valid bench directory.")
 
 	# For backwards compatibility
 	app = app.lower().replace(" ", "_").replace("-", "_")
+	if app[0].isdigit() or "." in app:
+		click.secho(
+			"App names cannot start with numbers(digits) or have dot(.) in them",
+			fg="red"
+		)
+		return
+
 	apps = os.path.abspath(os.path.join(bench_path, "apps"))
 	args = ["make-app", apps, app]
 	if no_git:
 		if bench.FRAPPE_VERSION < 14:
-			click.secho(
-				"Frappe v14 or greater is needed for '--no-git' flag",
-				fg="red"
-			)
+			click.secho("Frappe v14 or greater is needed for '--no-git' flag", fg="red")
 			return
 		args.append(no_git)
 
 	logger.log(f"creating new app {app}")
 	run_frappe_cmd(*args, bench_path=bench_path)
 	install_app(app, bench_path=bench_path)
 
 
 def install_app(
 	app,
+	tag=None,
 	bench_path=".",
 	verbose=False,
 	no_cache=False,
 	restart_bench=True,
 	skip_assets=False,
+	resolution=[]
 ):
 	import bench.cli as bench_cli
 	from bench.bench import Bench
 
 	install_text = f"Installing {app}"
 	click.secho(install_text, fg="yellow")
 	logger.log(install_text)
@@ -423,15 +557,15 @@
 
 	if conf.get("developer_mode"):
 		install_python_dev_dependencies(apps=app, bench_path=bench_path, verbose=verbose)
 
 	if os.path.exists(os.path.join(app_path, "package.json")):
 		bench.run("yarn install", cwd=app_path)
 
-	bench.apps.sync()
+	bench.apps.sync(app_name=app, required=resolution, branch=tag, app_dir=app_path)
 
 	if not skip_assets:
 		build_assets(bench_path=bench_path, app=app)
 
 	if restart_bench:
 		bench.reload()
 
@@ -522,15 +656,18 @@
 	return os.path.join(bench_path, "apps", app)
 
 
 def install_apps_from_path(path, bench_path="."):
 	apps = get_apps_json(path)
 	for app in apps:
 		get_app(
-			app["url"], branch=app.get("branch"), bench_path=bench_path, skip_assets=True,
+			app["url"],
+			branch=app.get("branch"),
+			bench_path=bench_path,
+			skip_assets=True,
 		)
 
 
 def get_apps_json(path):
 	import requests
 
 	if path.startswith("http"):
```

## bench/bench.py

```diff
@@ -1,18 +1,20 @@
 # imports - standard imports
+import subprocess
 import functools
 import os
 import shutil
+import json
 import sys
 import logging
-from typing import List, MutableSequence, TYPE_CHECKING
+from typing import List, MutableSequence, TYPE_CHECKING, Union
 
 # imports - module imports
 import bench
-from bench.exceptions import ValidationError
+from bench.exceptions import AppNotInstalledError, InvalidRemoteException
 from bench.config.common_site_config import setup_config
 from bench.utils import (
 	paths_in_bench,
 	exec_cmd,
 	is_bench_directory,
 	is_frappe_app,
 	get_cmd_output,
@@ -23,17 +25,19 @@
 from bench.utils.bench import (
 	validate_app_installed_on_sites,
 	restart_supervisor_processes,
 	restart_systemd_processes,
 	restart_process_manager,
 	remove_backups_crontab,
 	get_venv_path,
+	get_virtualenv_path,
 	get_env_cmd,
 )
 from bench.utils.render import job, step
+from bench.utils.app import get_current_version
 
 
 if TYPE_CHECKING:
 	from bench.app import App
 
 logger = logging.getLogger(bench.PROJECT_NAME)
 
@@ -42,15 +46,15 @@
 	def run(self, cmd, cwd=None):
 		return exec_cmd(cmd, cwd=cwd or self.cwd)
 
 
 class Validator:
 	def validate_app_uninstall(self, app):
 		if app not in self.apps:
-			raise ValidationError(f"No app named {app}")
+			raise AppNotInstalledError(f"No app named {app}")
 		validate_app_installed_on_sites(app, bench_path=self.name)
 
 
 @functools.lru_cache(maxsize=None)
 class Bench(Base, Validator):
 	def __init__(self, path):
 		self.name = path
@@ -112,19 +116,24 @@
 	def install(self, app, branch=None):
 		from bench.app import App
 
 		app = App(app, branch=branch)
 		self.apps.append(app)
 		self.apps.sync()
 
-	def uninstall(self, app):
+	def uninstall(self, app, no_backup=False, force=False):
 		from bench.app import App
 
-		self.validate_app_uninstall(app)
-		self.apps.remove(App(app, bench=self, to_clone=False))
+		if not force:
+			self.validate_app_uninstall(app)
+		try:
+			self.apps.remove(App(app, bench=self, to_clone=False), no_backup=no_backup)
+		except InvalidRemoteException:
+			if not force:
+				raise
 		self.apps.sync()
 		# self.build() - removed because it seems unnecessary
 		self.reload()
 
 	@step(title="Building Bench Assets", success="Bench Assets Built")
 	def build(self):
 		# build assets & stuff
@@ -151,20 +160,110 @@
 		apps.insert(0, "frappe")
 		return apps
 
 
 class BenchApps(MutableSequence):
 	def __init__(self, bench: Bench):
 		self.bench = bench
+		self.states_path = os.path.join(self.bench.name, "sites", "apps.json")
+		self.apps_path = os.path.join(self.bench.name, "apps")
 		self.initialize_apps()
+		self.set_states()
+
+	def set_states(self):
+		try:
+			with open(self.states_path, "r") as f:
+				self.states = json.loads(f.read() or "{}")
+		except FileNotFoundError:
+			self.states = {}
 
-	def sync(self):
+	def update_apps_states(
+			self,
+			app_dir: str = None,
+			app_name: Union[str, None] = None,
+			branch: Union[str, None] = None,
+			required: List = [],
+	):
+		if self.apps and not os.path.exists(self.states_path):
+			# idx according to apps listed in apps.txt (backwards compatibility)
+			# Keeping frappe as the first app.
+			if "frappe" in self.apps:
+				self.apps.remove("frappe")
+				self.apps.insert(0, "frappe")
+				with open(self.bench.apps_txt, "w") as f:
+					f.write("\n".join(self.apps))
+
+			print("Found existing apps updating states...")
+			for idx, app in enumerate(self.apps, start=1):
+				self.states[app] = {
+					"resolution": {
+					"commit_hash": None,
+					"branch": None
+				},
+				"required": required,
+				"idx": idx,
+				"version": get_current_version(app, self.bench.name),
+				}
+
+		apps_to_remove = []
+		for app in self.states:
+			if app not in self.apps:
+				apps_to_remove.append(app)
+
+		for app in apps_to_remove:
+			del self.states[app]
+
+		if app_name and not app_dir:
+			app_dir = app_name
+
+		if app_name and app_name not in self.states:
+			version = get_current_version(app_name, self.bench.name)
+
+			app_dir = os.path.join(self.apps_path, app_dir)
+			if not branch:
+				branch = (
+						subprocess
+						.check_output("git rev-parse --abbrev-ref HEAD", shell=True, cwd=app_dir)
+						.decode("utf-8")
+						.rstrip()
+						)
+
+			commit_hash = subprocess.check_output(f"git rev-parse {branch}", shell=True, cwd=app_dir).decode("utf-8").rstrip()
+
+			self.states[app_name] = {
+				"resolution": {
+					"commit_hash":commit_hash,
+					"branch": branch
+				},
+				"required":required,
+				"idx":len(self.states) + 1,
+				"version": version,
+			}
+
+		with open(self.states_path, "w") as f:
+			f.write(json.dumps(self.states, indent=4))
+
+	def sync(
+		self,
+		app_name: Union[str, None] = None,
+		app_dir: Union[str, None] = None,
+		branch: Union[str, None] = None,
+		required: List = []
+	):
 		self.initialize_apps()
+
 		with open(self.bench.apps_txt, "w") as f:
-			return f.write("\n".join(self.apps))
+			f.write("\n".join(self.apps))
+
+		self.update_apps_states(
+			app_name=app_name,
+			app_dir=app_dir,
+			branch=branch,
+			required=required
+		)
 
 	def initialize_apps(self):
 		is_installed = lambda app: app in installed_packages
 
 		try:
 			installed_packages = get_cmd_output(f"{self.bench.python} -m pip freeze", cwd=self.bench.name)
 		except Exception:
@@ -176,15 +275,14 @@
 				x
 				for x in os.listdir(os.path.join(self.bench.name, "apps"))
 				if (
 					is_frappe_app(os.path.join(self.bench.name, "apps", x))
 					and is_installed(x)
 				)
 			]
-			self.apps.sort()
 		except FileNotFoundError:
 			self.apps = []
 
 	def __getitem__(self, key):
 		""" retrieves an item by its index, key"""
 		return self.apps[key]
 
@@ -209,17 +307,17 @@
 
 	def add(self, app: "App"):
 		app.get()
 		app.install()
 		super().append(app.repo)
 		self.apps.sort()
 
-	def remove(self, app: "App"):
+	def remove(self, app: "App", no_backup: bool = False):
 		app.uninstall()
-		app.remove()
+		app.remove(no_backup=no_backup)
 		super().remove(app.repo)
 
 	def append(self, app: "App"):
 		return self.add(app)
 
 	def __repr__(self):
 		return self.__str__()
@@ -244,21 +342,30 @@
 	def env(self, python="python3"):
 		"""Setup env folder
 		- create env if not exists
 		- upgrade env pip
 		- install frappe python dependencies
 		"""
 		import bench.cli
+		import click
+
+		verbose = bench.cli.verbose
+
+		click.secho("Setting Up Environment", fg="yellow")
 
 		frappe = os.path.join(self.bench.name, "apps", "frappe")
-		virtualenv = get_venv_path()
-		quiet_flag = "" if bench.cli.verbose else "--quiet"
+		virtualenv = get_virtualenv_path(verbose=verbose)
+		quiet_flag = "" if verbose else "--quiet"
 
 		if not os.path.exists(self.bench.python):
-			self.run(f"{virtualenv} {quiet_flag} env -p {python}")
+			if virtualenv:
+				self.run(f"{virtualenv} {quiet_flag} env -p {python}")
+			else:
+				venv = get_venv_path(verbose=verbose)
+				self.run(f"{venv} env")
 
 		self.pip()
 
 		if os.path.exists(frappe):
 			self.run(f"{self.bench.python} -m pip install {quiet_flag} --upgrade -e {frappe}")
 
 	@step(title="Setting Up Bench Config", success="Bench Config Set Up")
@@ -335,15 +442,18 @@
 			apps = self.bench.get_installed_apps()
 
 		self.pip()
 
 		print(f"Installing {len(apps)} applications...")
 
 		for app in apps:
-			App(app, bench=self.bench, to_clone=False).install( skip_assets=True, restart_bench=False)
+			path_to_app = os.path.join(self.bench.name, "apps", app)
+			app = App(path_to_app, bench=self.bench, to_clone=False).install(
+				skip_assets=True, restart_bench=False, ignore_resolution=True
+			)
 
 	def python(self, apps=None):
 		"""Install and upgrade Python dependencies for specified / all installed apps on given Bench
 		"""
 		import bench.cli
 
 		if not apps:
```

## bench/exceptions.py

```diff
@@ -17,16 +17,26 @@
 class BenchNotFoundError(Exception):
 	pass
 
 
 class ValidationError(Exception):
 	pass
 
+
+class AppNotInstalledError(ValidationError):
+	pass
+
+
 class CannotUpdateReleaseBench(ValidationError):
 	pass
 
+
 class FeatureDoesNotExistError(CommandFailedError):
 	pass
 
 
 class NotInBenchDirectoryError(Exception):
 	pass
+
+
+class VersionNotFound(Exception):
+	pass
```

## bench/commands/make.py

```diff
@@ -129,29 +129,41 @@
 @click.argument("git-url")
 @click.option("--branch", default=None, help="branch to checkout")
 @click.option("--overwrite", is_flag=True, default=False)
 @click.option("--skip-assets", is_flag=True, default=False, help="Do not build assets")
 @click.option(
 	"--init-bench", is_flag=True, default=False, help="Initialize Bench if not in one"
 )
+@click.option(
+	"--resolve-deps",
+	is_flag=True,
+	default=False,
+	help="Resolve dependencies before installing app",
+)
 def get_app(
-	git_url, branch, name=None, overwrite=False, skip_assets=False, init_bench=False
+	git_url,
+	branch,
+	name=None,
+	overwrite=False,
+	skip_assets=False,
+	init_bench=False,
+	resolve_deps=False,
 ):
 	"clone an app from the internet and set it up in your bench"
 	from bench.app import get_app
 
 	get_app(
 		git_url,
 		branch=branch,
 		skip_assets=skip_assets,
 		overwrite=overwrite,
 		init_bench=init_bench,
+		resolve_deps=resolve_deps,
 	)
 
-
 @click.command("new-app", help="Create a new Frappe application under apps folder")
 @click.option(
 	"--no-git",
 	is_flag=True,
 	flag_value="--no-git",
 	help="Do not initialize git repository for the app (available in Frappe v14+)"
 )
@@ -164,20 +176,22 @@
 
 @click.command(
 	["remove", "rm", "remove-app"],
 	help=(
 		"Completely remove app from bench and re-build assets if not installed on any site"
 	),
 )
+@click.option("--no-backup", is_flag=True, help="Do not backup app before removing")
+@click.option("--force", is_flag=True, help="Force remove app")
 @click.argument("app-name")
-def remove_app(app_name):
+def remove_app(app_name, no_backup=False, force=False):
 	from bench.bench import Bench
 
 	bench = Bench(".")
-	bench.uninstall(app_name)
+	bench.uninstall(app_name, no_backup=no_backup, force=force)
 
 
 @click.command("exclude-app", help="Exclude app from updating")
 @click.argument("app_name")
 def exclude_app_for_update(app_name):
 	from bench.app import add_to_excluded_apps_txt
```

## bench/config/lets_encrypt.py

```diff
@@ -6,19 +6,18 @@
 
 # imports - module imports
 import bench
 from bench.config.nginx import make_nginx_conf
 from bench.config.production_setup import service
 from bench.config.site_config import get_domains, remove_domain, update_site_config
 from bench.bench import Bench
-from bench.utils import exec_cmd
+from bench.utils import exec_cmd, which
 from bench.utils.bench import update_common_site_config
 from bench.exceptions import CommandFailedError
 
-
 def setup_letsencrypt(site, custom_domain, bench_path, interactive):
 
 	site_path = os.path.join(bench_path, "sites", site, "site_config.json")
 	if not os.path.exists(os.path.dirname(site_path)):
 		print("No site named "+site)
 		return
 
@@ -54,15 +53,14 @@
 
 	with open(config_path, 'w') as f:
 		f.write(config)
 
 
 def run_certbot_and_setup_ssl(site, custom_domain, bench_path, interactive=True):
 	service('nginx', 'stop')
-	get_certbot()
 
 	try:
 		interactive = '' if interactive else '-n'
 		exec_cmd(f"{get_certbot_path()} {interactive} --config /etc/letsencrypt/configs/{custom_domain or site}.cfg certonly")
 	except CommandFailedError:
 		service('nginx', 'start')
 		print("There was a problem trying to setup SSL for your site")
@@ -84,15 +82,15 @@
 	make_nginx_conf(bench_path)
 	service('nginx', 'start')
 
 
 def setup_crontab():
 	from crontab import CronTab
 
-	job_command = '/opt/certbot-auto renew -a nginx --post-hook "systemctl reload nginx"'
+	job_command = f'{get_certbot_path()} renew -a nginx --post-hook "systemctl reload nginx"'
 	job_comment = 'Renew lets-encrypt every month'
 	print(f"Setting Up cron job to {job_comment}")
 
 	system_crontab = CronTab(user='root')
 
 	for job in system_crontab.find_comment(comment=job_comment): # Removes older entries
 		system_crontab.remove(job)
@@ -103,28 +101,19 @@
 
 
 def create_dir_if_missing(path):
 	if not os.path.exists(os.path.dirname(path)):
 		os.makedirs(os.path.dirname(path))
 
 
-def get_certbot():
-	from urllib.request import urlretrieve
-
-	certbot_path = get_certbot_path()
-	create_dir_if_missing(certbot_path)
-
-	if not os.path.isfile(certbot_path):
-		urlretrieve("https://dl.eff.org/certbot-auto", certbot_path)
-		os.chmod(certbot_path, 0o744)
-
-
 def get_certbot_path():
-	return "/opt/certbot-auto"
-
+	try:
+		return which("certbot", raise_err=True)
+	except FileNotFoundError:
+		raise CommandFailedError("Certbot is not installed on your system. Please visit https://certbot.eff.org/instructions for installation instructions, then try again.")
 
 def renew_certs():
 	# Needs to be run with sudo
 	click.confirm('Running this will stop the nginx service temporarily causing your sites to go offline\n'
 		'Do you want to continue?',
 		abort=True)
 
@@ -152,15 +141,14 @@
 
 		return domain_list
 
 	if not Bench(bench_path).conf.get("dns_multitenant"):
 		print("You cannot setup SSL without DNS Multitenancy")
 		return
 
-	get_certbot()
 	domain_list = _get_domains(domain.strip())
 
 	email_param = ''
 	if email:
 		email_param = f'--email {email}'
 
 	try:
```

## bench/config/templates/frappe_sudoers

```diff
@@ -11,10 +11,9 @@
 {{ user }} ALL = (root) NOPASSWD: {{ systemctl }} * nginx
 {% endif %}
 
 {% if nginx %}
 {{ user }} ALL = (root) NOPASSWD: {{ nginx }}
 {% endif %}
 
-{{ user }} ALL = (root) NOPASSWD: /opt/certbot-auto
+{{ user }} ALL = (root) NOPASSWD: {{ certbot }}
 Defaults:{{ user }} !requiretty
-
```

## bench/config/templates/nginx.conf

```diff
@@ -10,16 +10,18 @@
 }
 {%- endmacro %}
 
 {%- macro server_block(bench_name, port, server_names, site_name, sites_path, ssl_certificate, ssl_certificate_key) %}
 server {
 	{% if ssl_certificate and ssl_certificate_key %}
 	listen {{ port }} ssl;
+	listen [::]:{{ port }} ssl;
 	{% else %}
 	listen {{ port }};
+	listen [::]:{{ port }};
 	{% endif %}
 
 	server_name
 		{% for name in server_names -%}
 		{{ name }}
 		{% endfor -%}
 		;
@@ -76,15 +78,15 @@
 
 	location / {
 
  		rewrite ^(.+)/$ $1 permanent;
   		rewrite ^(.+)/index\.html$ $1 permanent;
   		rewrite ^(.+)\.html$ $1 permanent;
 
-		location ~ ^/files/.*.(htm|html|svg|xml) {
+		location ~* ^/files/.*.(htm|html|svg|xml) {
 			add_header Content-disposition "attachment";
 			try_files /{{ site_name }}/public/$uri @webserver;
 		}
 
 		try_files /{{ site_name }}/public/$uri @webserver;
 	}
```

## bench/tests/test_init.py

```diff
@@ -8,14 +8,15 @@
 import git
 
 # imports - module imports
 from bench.utils import exec_cmd
 from bench.release import get_bumped_version
 from bench.app import App
 from bench.tests.test_base import FRAPPE_BRANCH, TestBenchBase
+from bench.bench import Bench
 
 
 # changed from frappe_theme because it wasn't maintained and incompatible,
 # chat app & wiki was breaking too. hopefully frappe_docs will be maintained
 # for longer since docs.erpnext.com is powered by it ;)
 TEST_FRAPPE_APP = "frappe_docs"
 
@@ -34,19 +35,22 @@
 
 	def test_utils(self):
 		self.assertEqual(subprocess.call("bench"), 0)
 
 	def test_init(self, bench_name="test-bench", **kwargs):
 		self.init_bench(bench_name, **kwargs)
 		app = App("file:///tmp/frappe")
-		self.assertEqual(app.url, "/tmp/frappe")
+		self.assertEqual(app.mount_path, "/tmp/frappe")
+		self.assertEqual(app.url, "https://github.com/frappe/frappe.git")
 		self.assert_folders(bench_name)
 		self.assert_virtual_env(bench_name)
 		self.assert_config(bench_name)
-
+		test_bench = Bench(bench_name)
+		app = App("frappe", bench=test_bench)
+		self.assertEqual(app.from_apps, True)
 
 	def basic(self):
 		try:
 			self.test_init()
 		except Exception:
 			print(self.get_traceback())
 
@@ -103,14 +107,28 @@
 		self.init_bench("test-bench")
 		bench_path = os.path.join(self.benches_path, "test-bench")
 		exec_cmd(f"bench get-app {TEST_FRAPPE_APP}", cwd=bench_path)
 		self.assertTrue(os.path.exists(os.path.join(bench_path, "apps", TEST_FRAPPE_APP)))
 		app_installed_in_env = TEST_FRAPPE_APP in subprocess.check_output(["bench", "pip", "freeze"], cwd=bench_path).decode('utf8')
 		self.assertTrue(app_installed_in_env)
 
+	def test_get_app_resolve_deps(self):
+		FRAPPE_APP = "healthcare"
+		self.init_bench("test-bench")
+		bench_path = os.path.join(self.benches_path, "test-bench")
+		exec_cmd(f"bench get-app {FRAPPE_APP} --resolve-deps", cwd=bench_path)
+		self.assertTrue(os.path.exists(os.path.join(bench_path, "apps", FRAPPE_APP)))
+
+		states_path = os.path.join(bench_path, "sites", "apps.json")
+		self.assert_(os.path.exists(states_path))
+
+		with open(states_path, "r") as f:
+			states = json.load(f)
+
+		self.assert_(FRAPPE_APP in states)
 
 	def test_install_app(self):
 		bench_name = "test-bench"
 		site_name = "install-app.test"
 		bench_path = os.path.join(self.benches_path, "test-bench")
 
 		self.init_bench(bench_name)
```

## bench/utils/__init__.py

```diff
@@ -4,22 +4,24 @@
 import os
 import subprocess
 import re
 import sys
 from glob import glob
 from shlex import split
 from typing import List, Tuple
+from functools import lru_cache
 
 # imports - third party imports
 import click
+import requests
 
 # imports - module imports
 from bench import PROJECT_NAME, VERSION
 
-from bench.exceptions import CommandFailedError, InvalidRemoteException, ValidationError
+from bench.exceptions import CommandFailedError, InvalidRemoteException, AppNotInstalledError
 
 
 logger = logging.getLogger(PROJECT_NAME)
 bench_cache_file = ".bench.cmd"
 paths_in_app = ("hooks.py", "modules.txt", "patches.txt")
 paths_in_bench = ("apps", "sites", "config", "logs", "config/pids")
 sudoers_file = "/etc/sudoers.d/frappe"
@@ -44,31 +46,56 @@
 
 		path = glob(os.path.join(directory, "**", folder))
 		is_frappe_app = is_frappe_app and path
 
 	return bool(is_frappe_app)
 
 
+@lru_cache(maxsize=None)
+def is_valid_frappe_branch(frappe_path:str, frappe_branch:str):
+	"""Check if a branch exists in a repo. Throws InvalidRemoteException if branch is not found
+
+	Uses native git command to check for branches on a remote.
+
+	:param frappe_path: git url
+	:type frappe_path: str
+	:param frappe_branch: branch to check
+	:type frappe_branch: str
+	:raises InvalidRemoteException: branch for this repo doesn't exist
+	"""
+	import git
+
+	g = git.cmd.Git()
+
+	if frappe_branch:
+		try:
+			res = g.ls_remote("--heads", "--tags", frappe_path, frappe_branch)
+			if not res:
+				raise InvalidRemoteException(
+					f"Invalid branch or tag: {frappe_branch} for the remote {frappe_path}"
+				)
+		except git.exc.GitCommandError:
+			raise InvalidRemoteException(f"Invalid frappe path: {frappe_path}")
+
+
 def log(message, level=0, no_log=False):
 	import bench
 	import bench.cli
 
 	levels = {
 		0: ("blue", "INFO"),  # normal
 		1: ("green", "SUCCESS"),  # success
 		2: ("red", "ERROR"),  # fail
 		3: ("yellow", "WARN"),  # warn/suggest
 	}
 
 	color, prefix = levels.get(level, levels[0])
 
 	if bench.cli.from_command_line and bench.cli.dynamic_feed:
-		bench.LOG_BUFFER.append(
-			{"prefix": prefix, "message": message, "color": color}
-		)
+		bench.LOG_BUFFER.append({"prefix": prefix, "message": message, "color": color})
 
 	if no_log:
 		click.secho(message, fg=color)
 	else:
 		loggers = {2: logger.error, 3: logger.warning}
 		level_logger = loggers.get(level, logger.info)
 
@@ -178,17 +205,15 @@
 	version = ".".join(version.split(".")[0:2])
 	return float(version)
 
 
 def get_cmd_output(cmd, cwd=".", _raise=True):
 	output = ""
 	try:
-		output = subprocess.check_output(
-			cmd, cwd=cwd, shell=True, stderr=subprocess.PIPE, encoding="utf-8"
-		).strip()
+		output = subprocess.check_output(cmd, cwd=cwd, shell=True, stderr=subprocess.PIPE, encoding="utf-8").strip()
 	except subprocess.CalledProcessError as e:
 		if e.output:
 			output = e.output
 		elif _raise:
 			raise
 	return output
 
@@ -265,15 +290,15 @@
 	"Set app remote git url"
 	from bench.app import get_repo_dir
 	from bench.bench import Bench
 
 	app = git_url.rsplit("/", 1)[1].rsplit(".", 1)[0]
 
 	if app not in Bench(bench_path).apps:
-		raise ValidationError(f"No app named {app}")
+		raise AppNotInstalledError(f"No app named {app}")
 
 	app_dir = get_repo_dir(app, bench_path=bench_path)
 
 	if os.path.exists(os.path.join(app_dir, ".git")):
 		exec_cmd(f"git remote set-url upstream {git_url}", cwd=app_dir)
 
 
@@ -396,18 +421,20 @@
 def find_org(org_repo):
 	import requests
 
 	org_repo = org_repo[0]
 
 	for org in ["frappe", "erpnext"]:
 		res = requests.head(f"https://api.github.com/repos/{org}/{org_repo}")
+		if res.status_code in (400, 403):
+			res = requests.head(f"https://github.com/{org}/{org_repo}")
 		if res.ok:
 			return org, org_repo
 
-	raise InvalidRemoteException
+	raise InvalidRemoteException(f"{org_repo} not found in frappe or erpnext")
 
 
 def fetch_details_from_tag(_tag: str) -> Tuple[str, str, str]:
 	if not _tag:
 		raise Exception("Tag is not provided")
 
 	app_tag = _tag.split("@")
```

## bench/utils/app.py

```diff
@@ -3,16 +3,18 @@
 from setuptools.config import read_configuration
 import sys
 import subprocess
 from bench.exceptions import (
 	InvalidRemoteException,
 	InvalidBranchException,
 	CommandFailedError,
+	VersionNotFound,
 )
 from bench.app import get_repo_dir
+from functools import lru_cache
 
 
 def is_version_upgrade(app="frappe", bench_path=".", branch=None):
 	upstream_version = get_upstream_version(app=app, branch=branch, bench_path=bench_path)
 
 	if not upstream_version:
 		raise InvalidBranchException(
@@ -103,15 +105,17 @@
 
 
 def switch_to_develop(apps=None, bench_path=".", upgrade=True):
 	switch_branch("develop", apps=apps, bench_path=bench_path, upgrade=upgrade)
 
 
 def get_version_from_string(contents, field="__version__"):
-	match = re.search(r"^(\s*%s\s*=\s*['\\\"])(.+?)(['\"])(?sm)" % field, contents)
+	match = re.search(r"^(\s*%s\s*=\s*['\\\"])(.+?)(['\"])" % field, contents, flags=(re.S | re.M))
+	if not match:
+		raise VersionNotFound(f"{contents} is not a valid version")
 	return match.group(2)
 
 
 def get_major_version(version):
 	import semantic_version
 
 	return semantic_version.Version(version).major
@@ -161,14 +165,39 @@
 def get_current_branch(app, bench_path="."):
 	from bench.utils import get_cmd_output
 
 	repo_dir = get_repo_dir(app, bench_path=bench_path)
 	return get_cmd_output("basename $(git symbolic-ref -q HEAD)", cwd=repo_dir)
 
 
+@lru_cache(maxsize=5)
+def get_required_deps(org, name, branch, deps="hooks.py"):
+	import requests
+	import base64
+
+	git_api_url = f"https://api.github.com/repos/{org}/{name}/contents/{name}/{deps}"
+	params = {"branch": branch or "develop"}
+	res = requests.get(url=git_api_url, params=params).json()
+
+	if "message" in res:
+		git_url = f"https://raw.githubusercontent.com/{org}/{name}/{params['branch']}/{deps}"
+		return requests.get(git_url).text
+
+	return base64.decodebytes(res["content"].encode()).decode()
+
+
+def required_apps_from_hooks(required_deps, local=False):
+	if local:
+		with open(required_deps) as f:
+			required_deps = f.read()
+	lines = [x for x in required_deps.split("\n") if x.strip().startswith("required_apps")]
+	required_apps = eval(lines[0].strip("required_apps").strip().lstrip("=").strip())
+	return required_apps
+
+
 def get_remote(app, bench_path="."):
 	repo_dir = get_repo_dir(app, bench_path=bench_path)
 	contents = subprocess.check_output(
 		["git", "remote", "-v"], cwd=repo_dir, stderr=subprocess.STDOUT
 	)
 	contents = contents.decode("utf-8")
 	if re.findall(r"upstream[\s]+", contents):
@@ -177,33 +206,38 @@
 		# if contents is an empty string => remote doesn't exist
 		return False
 	else:
 		# get the first remote
 		return contents.splitlines()[0].split()[0]
 
 
-def get_app_name(bench_path, repo_name):
+def get_app_name(bench_path, folder_name):
 	app_name = None
 	apps_path = os.path.join(os.path.abspath(bench_path), "apps")
-	config_path = os.path.join(apps_path, repo_name, "setup.cfg")
+	config_path = os.path.join(apps_path, folder_name, "setup.cfg")
 	if os.path.exists(config_path):
 		config = read_configuration(config_path)
 		app_name = config.get("metadata", {}).get("name")
 
 	if not app_name:
 		# retrieve app name from setup.py as fallback
-		app_path = os.path.join(apps_path, repo_name, "setup.py")
+		app_path = os.path.join(apps_path, folder_name, "setup.py")
 		with open(app_path, "rb") as f:
 			app_name = re.search(r'name\s*=\s*[\'"](.*)[\'"]', f.read().decode("utf-8")).group(1)
 
-	if app_name and repo_name != app_name:
-		os.rename(os.path.join(apps_path, repo_name), os.path.join(apps_path, app_name))
+	if app_name and folder_name != app_name:
+		os.rename(os.path.join(apps_path, folder_name), os.path.join(apps_path, app_name))
 		return app_name
 
-	return repo_name
+	return folder_name
+
+def check_existing_dir(bench_path, repo_name):
+	cloned_path = os.path.join(bench_path, "apps", repo_name)
+	dir_already_exists = os.path.isdir(cloned_path)
+	return dir_already_exists, cloned_path
 
 
 def get_current_version(app, bench_path="."):
 	current_version = None
 	repo_dir = get_repo_dir(app, bench_path=bench_path)
 	config_path = os.path.join(repo_dir, "setup.cfg")
 	init_path = os.path.join(repo_dir, os.path.basename(repo_dir), "__init__.py")
```

## bench/utils/bench.py

```diff
@@ -29,27 +29,33 @@
 logger = logging.getLogger(bench.PROJECT_NAME)
 
 
 def get_env_cmd(cmd, bench_path="."):
 	return os.path.abspath(os.path.join(bench_path, "env", "bin", cmd))
 
 
-def get_venv_path():
-	venv = which("virtualenv")
+def get_virtualenv_path(verbose=False):
+	virtualenv_path = which("virtualenv")
 
-	if not venv:
-		current_python = sys.executable
-		with open(os.devnull, "wb") as devnull:
-			is_venv_installed = not subprocess.call(
-				[current_python, "-m", "venv", "--help"], stdout=devnull
-			)
-		if is_venv_installed:
-			venv = f"{current_python} -m venv"
+	if not virtualenv_path and verbose:
+		log("virtualenv cannot be found", level=2)
 
-	return venv or log("virtualenv cannot be found", level=2)
+	return virtualenv_path
+
+
+def get_venv_path(verbose=False):
+	current_python = sys.executable
+	with open(os.devnull, "wb") as devnull:
+		is_venv_installed = not subprocess.call(
+			[current_python, "-m", "venv", "--help"], stdout=devnull
+		)
+	if is_venv_installed:
+		return f"{current_python} -m venv"
+	else:
+		log("virtualenv cannot be found", level=2)
 
 
 def update_node_packages(bench_path=".", apps=None):
 	print("Updating node packages...")
 	from bench.utils.app import get_develop_version
 	from distutils.version import LooseVersion
```

## bench/utils/system.py

```diff
@@ -10,14 +10,15 @@
 from bench.utils import (
 	exec_cmd,
 	get_process_manager,
 	log,
 	run_frappe_cmd,
 	sudoers_file,
 	which,
+	is_valid_frappe_branch,
 )
 from bench.utils.bench import build_assets, clone_apps_from
 from bench.utils.render import job
 
 
 @job(title="Initializing Bench {path}", success="Bench {path} initialized")
 def init(
@@ -70,37 +71,49 @@
 		clone_apps_from(
 			bench_path=path, clone_from=clone_from, update_app=not clone_without_update
 		)
 
 	# remote apps
 	else:
 		frappe_path = frappe_path or "https://github.com/frappe/frappe.git"
-
+		is_valid_frappe_branch(frappe_path=frappe_path, frappe_branch=frappe_branch)
 		get_app(
-			frappe_path, branch=frappe_branch, bench_path=path, skip_assets=True, verbose=verbose
+			frappe_path,
+			branch=frappe_branch,
+			bench_path=path,
+			skip_assets=True,
+			verbose=verbose,
+			resolve_deps=False,
 		)
 
 		# fetch remote apps using config file - deprecate this!
 		if apps_path:
 			install_apps_from_path(apps_path, bench_path=path)
 
 	# getting app on bench init using --install-app
 	if install_app:
 		get_app(
-			install_app, branch=frappe_branch, bench_path=path, skip_assets=True, verbose=verbose
+			install_app,
+			branch=frappe_branch,
+			bench_path=path,
+			skip_assets=True,
+			verbose=verbose,
+			resolve_deps=False,
 		)
 
 	if not skip_assets:
 		build_assets(bench_path=path)
 
 	if not no_backups:
 		bench.setup.backups()
 
 
 def setup_sudoers(user):
+	from bench.config.lets_encrypt import get_certbot_path
+
 	if not os.path.exists("/etc/sudoers.d"):
 		os.makedirs("/etc/sudoers.d")
 
 		set_permissions = False
 		if not os.path.exists("/etc/sudoers"):
 			set_permissions = True
 
@@ -113,14 +126,15 @@
 	template = bench.config.env().get_template("frappe_sudoers")
 	frappe_sudoers = template.render(
 		**{
 			"user": user,
 			"service": which("service"),
 			"systemctl": which("systemctl"),
 			"nginx": which("nginx"),
+			"certbot": get_certbot_path(),
 		}
 	)
 
 	with open(sudoers_file, "w") as f:
 		f.write(frappe_sudoers)
 
 	os.chmod(sudoers_file, 0o440)
```

## Comparing `frappe_bench-5.8.1.dist-info/LICENSE` & `frappe_bench-5.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `frappe_bench-5.8.1.dist-info/METADATA` & `frappe_bench-5.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frappe-bench
-Version: 5.8.1
+Version: 5.9.0
 Summary: CLI to manage Multi-tenant deployments for Frappe apps
 Home-page: https://frappe.io/bench
 Author: Frappe Technologies Pvt Ltd
 Author-email: developers@frappe.io
 License: GPLv3
 Project-URL: Source, https://github.com/frappe/bench
 Project-URL: Documentation, https://frappeframework.com/docs/user/en/bench
@@ -25,15 +25,14 @@
 Requires-Dist: GitPython (~=2.1.15)
 Requires-Dist: honcho
 Requires-Dist: Jinja2 (~=3.0.3)
 Requires-Dist: python-crontab (~=2.4.0)
 Requires-Dist: requests
 Requires-Dist: semantic-version (~=2.8.2)
 Requires-Dist: setuptools
-Requires-Dist: virtualenv
 
 <div align="center">
 	<img src="https://github.com/frappe/design/raw/master/logos/png/bench-logo.png" height="128">
 	<h2>Bench</h2>
 </div>
 
 Bench is a command-line utility that helps you to install, update, and manage multiple sites for Frappe/ERPNext applications on [*nix systems](https://en.wikipedia.org/wiki/Unix-like) for development and production.
@@ -83,15 +82,15 @@
 
  - [Containerized Installation](#containerized-installation)
  - [Easy Install Script](#easy-install-script)
  - [Manual Installation](#manual-installation)
 
 We recommend using either the Docker Installation or the Easy Install Script to setup a Production Environment. For Development, you may choose either of the three methods to setup an instance.
 
-Otherwise, if you are looking to evaluate ERPNext, you can also download the [Virtual Machine Image](https://erpnext.com/download) or register for [a free trial on erpnext.com](https://erpnext.com/pricing).
+Otherwise, if you are looking to evaluate ERPNext, you can register for [a free trial on erpnext.com](https://erpnext.com/pricing).
 
 
 ### Containerized Installation
 
 A Frappe/ERPNext instance can be setup and replicated easily using [Docker](https://docker.com). The officially supported Docker installation can be used to setup either of both Development and Production environments.
 
 To setup either of the environments, you will need to clone the official docker repository:
```

## Comparing `frappe_bench-5.8.1.dist-info/RECORD` & `frappe_bench-5.9.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-bench/__init__.py,sha256=abYxvBQCjq2gfBBmQWouwYN85CizlQXPZFMSRJLu4PA,336
-bench/app.py,sha256=erir4iSn4BG3Ym1m5Y4aNwY0Es0pVkw1416GcJp2vwI,15458
-bench/bench.py,sha256=qBv-2v1g7Rt9QPOhXXLAvNQ3wQdsuXKtofOH0jxuBrE,9872
+bench/__init__.py,sha256=zuP9iM9V78umsjYMm8a2DgFeERPGRkgWUbueG0Jqf7w,336
+bench/app.py,sha256=7y7NajFycu7l1TgE48Q59kQcY01kIizEpXcZGgXDgS0,19589
+bench/bench.py,sha256=BOf7cOgqMTNgBJ_YB75XnHPmROFvUabU9umyPGWyn6A,12816
 bench/cli.py,sha256=ehLxhgEl1KSzADep5Y7e3BkyKH6XrD4QZNxDGOqClhA,5510
-bench/exceptions.py,sha256=L75TLxWHiKVWZEej-wGxPNiSIiEwOXAJ1D8R6FsRbzU,431
+bench/exceptions.py,sha256=TV0gyhL6-8gpMNQspjR8sLGl3sRUFzKtRNhueyfkhyU,527
 bench/prepare_beta_release.py,sha256=oAhxc9XZmckFX3haTIwZFYvsSQijfHGVolA9nZCLfW8,3224
 bench/release.py,sha256=yj-mumqtx2Dx7nWz_Onh8jc_8cDioe0RswKBH2avat4,11453
 bench/commands/__init__.py,sha256=Dw0qsgtdeLMKPTd-0qQrWAyyX0hBazM-kZrCTuAfQC4,3203
 bench/commands/config.py,sha256=v-mBtWWk8ZhGA3KbzStBQzPVAlgbF5GFlYa-EwNiwGc,2821
 bench/commands/git.py,sha256=1koGttv7LZZgHpvbNtAemqJJCQRfOo0Mho_ghD-CfuQ,1009
 bench/commands/install.py,sha256=NxmQXrRad5yikQhbdE-L29rnzFLSY_RqESa-F21xLOM,3334
-bench/commands/make.py,sha256=gBbzRnSnF7MVGs_RX-OjGNT7DTiCpKu7_0d2g6gZo_s,5671
+bench/commands/make.py,sha256=rlx3Djhv-6gKWTfrWwfYjwJjlulp0xALBQ3D0KMYDXQ,6058
 bench/commands/setup.py,sha256=EGwvFs3G41evu-bSmzjMNHStk3m9tyhjbLRg2ipnKUs,11910
 bench/commands/update.py,sha256=h5da4ySyXReemKluRy7Udp5aK6dlR9TWxL6Bh8kEnOE,2738
 bench/commands/utils.py,sha256=Wd2E4KLTh74xLUiz5mAaES3HczC9L1tXevhVHz-gHFU,6745
 bench/config/__init__.py,sha256=f5o9KdiHsOKKnAhCamGSOdJJfoIuI_RUwgoU3lqxFkc,189
 bench/config/common_site_config.py,sha256=110DZaXIPAWgN06ETlMSpB6D4eM3t6H8YdzAIUfDhtM,3229
-bench/config/lets_encrypt.py,sha256=jzIiuUIJUXAarEqNlYkB8NB4n1HiOA1yz9xA0L5sKhE,5437
+bench/config/lets_encrypt.py,sha256=pNvyMBk5behcRSFe2eVVksVc1YFpTDjrXSyeJfcJ3eU,5363
 bench/config/nginx.py,sha256=qKA3Pm4cZoU1uZCuWxwYixrwCfJYj1WRvl8NUnRBR1k,8224
 bench/config/procfile.py,sha256=ms8jIOB8Dp4vnuLFYJw0Hj87ww1N32WxAEI2kRppnmg,854
 bench/config/production_setup.py,sha256=t48LZqOpAkMpsGO7KGrHCvngHD2yID41oe4xL591t2M,5481
 bench/config/redis.py,sha256=9ACbrHW4qXo1qS6p5u87AbxtYXCEiZxyUfWphrh5qdM,2732
 bench/config/site_config.py,sha256=8CNaPlaKCVcFjBu4JJyJQQFKOELF-dDv90Pr7JqZbg0,3548
 bench/config/supervisor.py,sha256=aMajzrK6rkb_CQb73t5Mon7L3SfAYjzdjwEj60f0adU,4281
 bench/config/systemd.py,sha256=v-4xFr6XL2Evp4G4SKP5drxeWsAWkwLFY2oMuSSN-p0,9858
 bench/config/templates/502.html,sha256=gFOcZV-I74C6PKBPxJr2yVVVvciX2hj3uPqya4BX78w,5444
 bench/config/templates/Procfile,sha256=h8tN0oJWZmx3xkLUl-y_eiM1YavF4a2fzjFI2FHIOEw,1412
 bench/config/templates/bench_manager_nginx.conf,sha256=L6FescyzNtz5u99sAumP2jKT5ubIqzBg_aoXL30lx0s,2619
-bench/config/templates/frappe_sudoers,sha256=N98d8WYNerQ2ZFACxckmjlsYGdk1geDNbKzn73t0VhM,514
+bench/config/templates/frappe_sudoers,sha256=u0H3tRTuCRCV6qQ0AlBhcrsNxvWWVlSUTfTx2FBwp-c,509
 bench/config/templates/letsencrypt.cfg,sha256=EoC3ElXU7QjVP35PQMnLC-91-9Rn9qw0UF-nJju-ds0,620
-bench/config/templates/nginx.conf,sha256=_VFRkzcrVpSQCHTiMD8lltOneq-tlK88aicQrLi9690,5722
+bench/config/templates/nginx.conf,sha256=5dkKe95tKBQ08ebalbHnE0R4b-yq-vMoZ8HtpubLFjM,5777
 bench/config/templates/nginx_default.conf,sha256=-sre3LgFEq94Q0bE9D14zzrBB1Wwzgts9MmN4gCIKxk,1169
 bench/config/templates/redis_cache.conf,sha256=E8NVlxjrLP9TcLPtgptCwL6BZ5UBpqsPhNUX3F_C0xY,357
 bench/config/templates/redis_queue.conf,sha256=ygC_ZJU2NrP92phwa1tlQvAyPhU5R1BWftags1_b73Q,218
 bench/config/templates/redis_socketio.conf,sha256=aM8OKRkCvVLS5MdKw9jxq-lw0vYB1GhwolbMkROWGE8,227
 bench/config/templates/supervisor.conf,sha256=GdnhBq5-Wx1CJyAGhxRmI73q4g_y4IyHH_fE3LnmaIM,6106
 bench/config/templates/systemd/frappe-bench-frappe-default-worker.service,sha256=sVDBEMpS4HowT6QqstAAh1nus01NAxAWSx0gii6yOi0,352
 bench/config/templates/systemd/frappe-bench-frappe-long-worker.service,sha256=3VyaLnqkyFtQT_OlzuKUIMTsphvrf5TGA58lVNma2RQ,347
@@ -144,22 +144,23 @@
 bench/playbooks/roles/virtualbox/files/virtualbox_centos.repo,sha256=G5T3vd6qxUQvkdGnqtqdmqKAd-PhO-tdCW8AoSfma64,258
 bench/playbooks/roles/virtualbox/tasks/debian_family.yml,sha256=UY4QBHZO7600w5px2nNcRU3QPY_HSDyfQEzbpQqydXE,1122
 bench/playbooks/roles/virtualbox/tasks/main.yml,sha256=Ev3mlsw9e-80pLcUVgOEFynErPibLgsAJjTlgPFsbf0,154
 bench/playbooks/roles/virtualbox/tasks/redhat_family.yml,sha256=jDX6HvfH2OmsomlhU38B-s8ENuUGBA4vlMeabT41ABQ,428
 bench/playbooks/roles/wkhtmltopdf/tasks/main.yml,sha256=w1-s6zc8EUbKkgt1rt7fTZAgrcceIO6lB0DGMxdvWYs,5717
 bench/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bench/tests/test_base.py,sha256=qrqL2uTjh_Bwa_8579L_dYSnBZ_FcGLTzqhuvVeU4J8,3724
-bench/tests/test_init.py,sha256=YJ4X4cOBTZ0dmHUDvX2iifWSazo9_PwJuGcEohx4CTM,6459
+bench/tests/test_init.py,sha256=G-3ofK9QmLRwP_cWmgAUAdHVZ18yXkH-nP7LTUaptzo,7196
 bench/tests/test_setup_production.py,sha256=4d0GsSCJ8EY1SlP6tYq2L8-ayPyIFq8_pIGDeva4x54,5530
-bench/utils/__init__.py,sha256=WaMMdY77qVfKwNtB3KgTZn9pKvpNBwjVLfgLrWaKB4E,12430
-bench/utils/app.py,sha256=smu924_GNZIdaKgvsdJhqf94txV2Lza5AfZ95NQ6nwM,6680
-bench/utils/bench.py,sha256=6NJu6zm3SDki-Ylnvnf7S3lJj2ptPpv2VuheC5s8i54,17257
+bench/tests/test_utils.py,sha256=J6AuIyVOzRL9PF6PcphxdIYENJeQ0NyvhlVnfZGtzHM,2526
+bench/utils/__init__.py,sha256=FTNt98Ht951a3jw9kgoMeaTtmBnQH9rUaIwL-6Mz1XI,13421
+bench/utils/app.py,sha256=GvbinLUz1ZEmOhtfc7iXzA0_P7JR9-1sKv1Pt3IktCQ,7866
+bench/utils/bench.py,sha256=Ql0Td5LhjYpV33lamSDFEdRNUIsZttPZ0RSD4YVWFvk,17401
 bench/utils/cli.py,sha256=nZD-mmXtbZ6n5QpKhbu2hCochvpfl_8LJddBs9tthgA,1582
 bench/utils/render.py,sha256=UU2s8D0GVY6IYdtJlQWadS5XmwFvi9xxAAyXbMDH3DM,2829
-bench/utils/system.py,sha256=JPCxYsgFcWsaXf_tatXzwz1_pb0ebjYDvVAfgfteHAE,4827
+bench/utils/system.py,sha256=sURyMHKbn_bAVZ5_twp9nOWnNknY3DZDfsQ-xU1NQOU,5093
 bench/utils/translation.py,sha256=RgHpFrWz3nMViPWBykkP01i-3JlQXsP4qUMqYtse7aQ,1333
-frappe_bench-5.8.1.dist-info/LICENSE,sha256=4cCtcomD2KVzNeUs8QZPGv_R1FQXPYzr0-2LSnK0hwQ,35121
-frappe_bench-5.8.1.dist-info/METADATA,sha256=cyXxieXtJg9eZntB39ZUStGXj2FaUTXdoMhC-TX1gjY,13246
-frappe_bench-5.8.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-frappe_bench-5.8.1.dist-info/entry_points.txt,sha256=NjczH_M8PA3rC8LANHrERkEFaTH5ET6E4Yix-MDyImo,41
-frappe_bench-5.8.1.dist-info/top_level.txt,sha256=S5dMoM5b5eB-M6N0925gZ2nYyEp8vsKq12fsr5iMt5I,6
-frappe_bench-5.8.1.dist-info/RECORD,,
+frappe_bench-5.9.0.dist-info/LICENSE,sha256=4cCtcomD2KVzNeUs8QZPGv_R1FQXPYzr0-2LSnK0hwQ,35121
+frappe_bench-5.9.0.dist-info/METADATA,sha256=JnsQyYqbYzeVWB6EzoSRCs-YbEyEkAdMuZggPDx_bZs,13145
+frappe_bench-5.9.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+frappe_bench-5.9.0.dist-info/entry_points.txt,sha256=NjczH_M8PA3rC8LANHrERkEFaTH5ET6E4Yix-MDyImo,41
+frappe_bench-5.9.0.dist-info/top_level.txt,sha256=S5dMoM5b5eB-M6N0925gZ2nYyEp8vsKq12fsr5iMt5I,6
+frappe_bench-5.9.0.dist-info/RECORD,,
```

