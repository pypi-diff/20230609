# Comparing `tmp/pulumi_openstack-3.9.0a1654086724.tar.gz` & `tmp/pulumi_openstack-3.9.0a1659603007.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_openstack-3.9.0a1654086724.tar", last modified: Wed Jun  1 12:39:39 2022, max compression
+gzip compressed data, was "dist/pulumi_openstack-3.9.0a1659603007.tar", last modified: Thu Aug  4 08:54:17 2022, max compression
```

## Comparing `pulumi_openstack-3.9.0a1654086724.tar` & `pulumi_openstack-3.9.0a1659603007.tar`

### file list

```diff
@@ -1,221 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/
--rw-r--r--   0 runner    (1001) docker     (121)    10057 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8755 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/
--rw-r--r--   0 runner    (1001) docker     (121)    21379 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14216 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4794 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_availability_zones_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)     8176 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_quotaset_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)     7494 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_snapshot_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7494 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_snapshot_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)     7774 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_volume_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     8986 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_volume_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    14100 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12923 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/qos_association_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    13612 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/qos_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    29994 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/quote_set_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    29994 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/quote_set_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    42608 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    35348 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_attach.py
--rw-r--r--   0 runner    (1001) docker     (121)    37540 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_attach_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    12885 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_type_access_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    16837 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_type_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    29601 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    37561 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35790 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18016 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/aggregate_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    29898 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/flavor.py
--rw-r--r--   0 runner    (1001) docker     (121)    12691 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/flavor_access.py
--rw-r--r--   0 runner    (1001) docker     (121)    14584 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)    18733 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/floating_ip_associate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4958 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_aggregate_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4361 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_availability_zones.py
--rw-r--r--   0 runner    (1001) docker     (121)    10352 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_flavor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6079 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_hypervisor_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11142 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_instance_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_keypair.py
--rw-r--r--   0 runner    (1001) docker     (121)    11828 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_quota_set_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    90576 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)    20453 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/interface_attach.py
--rw-r--r--   0 runner    (1001) docker     (121)    19078 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/keypair.py
--rw-r--r--   0 runner    (1001) docker     (121)    33170 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    43803 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/quota_set_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    20111 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/sec_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    17577 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/server_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    22886 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/volume_attach.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7142 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    59099 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    94765 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    15500 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    20148 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/get_cluster_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11950 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17329 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9931 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    29281 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)     9831 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13292 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15453 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/get_dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (121)    30098 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/record_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    18719 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/transfer_accept.py
--rw-r--r--   0 runner    (1001) docker     (121)    21758 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/transfer_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    30902 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30027 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)     7256 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    27269 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    40007 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4892 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    34862 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/application_credential.py
--rw-r--r--   0 runner    (1001) docker     (121)    15519 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/ec2_credential_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    19225 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/endpoint_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    11727 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_auth_scope.py
--rw-r--r--   0 runner    (1001) docker     (121)     8614 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     7642 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     9519 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    12535 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/group_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)     8569 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21993 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    10581 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    15152 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (121)    13601 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/service_v3.py
--rw-r--r--   0 runner    (1001) docker     (121)    38026 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    13208 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/user_membership_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19238 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/get_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    15193 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/get_image_ids.py
--rw-r--r--   0 runner    (1001) docker     (121)    65652 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/image.py
--rw-r--r--   0 runner    (1001) docker     (121)    20262 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/image_access.py
--rw-r--r--   0 runner    (1001) docker     (121)    18191 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/image_access_accept.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14057 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    31996 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/container_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     8393 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/get_container.py
--rw-r--r--   0 runner    (1001) docker     (121)    18634 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (121)    22800 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/order_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    19501 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    44712 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/secret_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7224 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    30669 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/l7_policy_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    30234 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/l7_rule_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    54507 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)    44692 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)    27806 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/member.py
--rw-r--r--   0 runner    (1001) docker     (121)    20924 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/member_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    14464 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/members.py
--rw-r--r--   0 runner    (1001) docker     (121)    39261 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    34086 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/monitor_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     6851 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    32997 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    34923 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/pool_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    27900 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/quota.py
--rw-r--r--   0 runner    (1001) docker     (121)    38997 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/vip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17512 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18793 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/address_scope.py
--rw-r--r--   0 runner    (1001) docker     (121)    42903 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)    15112 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/floating_ip_associate.py
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_address_scope.py
--rw-r--r--   0 runner    (1001) docker     (121)    10412 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)    13871 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_network.py
--rw-r--r--   0 runner    (1001) docker     (121)    18605 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_port.py
--rw-r--r--   0 runner    (1001) docker     (121)    14914 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_port_ids.py
--rw-r--r--   0 runner    (1001) docker     (121)     6754 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     5215 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_dscp_marking_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     5952 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     9723 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7740 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_quota_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    12164 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_router.py
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_sec_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    16187 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_subnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    14960 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_subnet_ids_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    15659 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_subnet_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     9594 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_trunk.py
--rw-r--r--   0 runner    (1001) docker     (121)    53846 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/network.py
--rw-r--r--   0 runner    (1001) docker     (121)    25968 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    71097 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/port.py
--rw-r--r--   0 runner    (1001) docker     (121)    27361 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/port_forwarding_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    19347 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/port_sec_group_associate.py
--rw-r--r--   0 runner    (1001) docker     (121)    19630 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_bandwidth_limit_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    13470 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_dscp_marking_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    16399 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    29277 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    30082 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/quota_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    21061 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/rbac_policy_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    54401 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/router.py
--rw-r--r--   0 runner    (1001) docker     (121)    15721 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/router_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    17392 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/router_route.py
--rw-r--r--   0 runner    (1001) docker     (121)    19967 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/sec_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    39818 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/sec_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    66226 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/subnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    53095 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/subnet_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    16244 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/subnet_route.py
--rw-r--r--   0 runner    (1001) docker     (121)    27970 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    34090 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/container.py
--rw-r--r--   0 runner    (1001) docker     (121)    56135 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/container_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19918 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/temp_url.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    49597 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/stack_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    42516 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3839 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_availbility_zones.py
--rw-r--r--   0 runner    (1001) docker     (121)    12815 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_share.py
--rw-r--r--   0 runner    (1001) docker     (121)    11956 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_share_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     8157 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    29689 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/security_service.py
--rw-r--r--   0 runner    (1001) docker     (121)    42350 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/share.py
--rw-r--r--   0 runner    (1001) docker     (121)    23504 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/share_access.py
--rw-r--r--   0 runner    (1001) docker     (121)    30679 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/share_network.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5205 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22367 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/endpoint_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    33277 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/ike_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    33697 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/ip_sec_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    27849 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/service.py
--rw-r--r--   0 runner    (1001) docker     (121)    56897 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/site_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10057 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8423 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 12:39:39.000000 pulumi_openstack-3.9.0a1654086724/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-06-01 12:39:38.000000 pulumi_openstack-3.9.0a1654086724/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/
+-rw-r--r--   0 runner    (1001) docker     (121)    10057 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8755 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/
+-rw-r--r--   0 runner    (1001) docker     (121)    21571 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14228 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_availability_zones_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8135 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_quotaset_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7453 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_snapshot_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7453 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_snapshot_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7733 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_volume_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8945 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_volume_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14112 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12872 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/qos_association_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13561 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/qos_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29943 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/quote_set_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29943 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/quote_set_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42557 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35297 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_attach.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37489 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_attach_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12834 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_type_access_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16786 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_type_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29550 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37510 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35802 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17965 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/aggregate_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29847 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12640 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/flavor_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14533 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18682 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/floating_ip_associate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_aggregate_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_availability_zones.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10311 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6038 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_hypervisor_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11101 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_instance_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16045 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_limits_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11787 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_quota_set_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    91029 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20402 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/interface_attach.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21822 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33182 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43752 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/quota_set_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20060 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/sec_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17526 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/server_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22835 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/volume_attach.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7154 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59058 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    94714 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15459 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20107 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10023 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/get_node_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36117 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11962 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17278 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9880 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29230 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9843 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13241 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15412 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/get_dns_zone.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30047 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/record_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18668 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/transfer_accept.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21707 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30851 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29976 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7215 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27218 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39956 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4910 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34811 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/application_credential.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15468 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/ec2_credential_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19174 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/endpoint_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11686 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_auth_scope.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8573 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5034 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5580 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9478 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12484 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/group_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8587 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21942 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10530 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15101 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13550 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/service_v3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37975 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13157 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/user_membership_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19197 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15156 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/get_image_ids.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65601 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20211 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/image_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18140 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/image_access_accept.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14069 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31945 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/container_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8352 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/get_container.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18593 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22749 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/order_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19513 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44675 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/secret_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8691 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30674 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/l7_policy_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30204 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/l7_rule_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54456 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44641 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35059 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/member.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20873 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/member_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14413 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/members.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39210 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34035 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/monitor_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8099 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32946 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34872 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/pool_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27849 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/quota.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38946 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/vip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17524 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18742 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/address_scope.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42852 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15061 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/floating_ip_associate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_address_scope.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10371 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13830 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18564 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14873 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_port_ids.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_dscp_marking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5911 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9682 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_quota_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12123 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_router.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7320 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_sec_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16146 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14919 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_subnet_ids_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15618 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_subnet_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9553 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_trunk.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53795 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25980 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71046 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/port.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27310 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/port_forwarding_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19836 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/port_sec_group_associate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19579 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_bandwidth_limit_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13419 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_dscp_marking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16348 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29226 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30031 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/quota_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21010 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/rbac_policy_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54350 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/router.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15670 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/router_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17341 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/router_route.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19916 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/sec_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39767 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/sec_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66175 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53044 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/subnet_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16193 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/subnet_route.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27919 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36498 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/container.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56084 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/container_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19867 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/temp_url.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49550 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/stack_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42465 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3798 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_availbility_zones.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12774 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_share.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11915 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_share_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8116 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29645 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/security_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42299 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/share.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23453 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/share_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30628 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/share_network.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22316 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/endpoint_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33226 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/ike_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33646 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/ip_sec_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27798 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56846 2022-08-04 08:54:15.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/site_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10057 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8561 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-04 08:54:17.000000 pulumi_openstack-3.9.0a1659603007/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-08-04 08:54:16.000000 pulumi_openstack-3.9.0a1659603007/setup.py
```

### Comparing `pulumi_openstack-3.9.0a1654086724/PKG-INFO` & `pulumi_openstack-3.9.0a1659603007/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_openstack
-Version: 3.9.0a1654086724
+Version: 3.9.0a1659603007
 Summary: A Pulumi package for creating and managing OpenStack cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-openstack
 Description: [![Actions Status](https://github.com/pulumi/pulumi-openstack/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-openstack/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fopenstack.svg)](https://www.npmjs.com/package/@pulumi/openstack)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/README.md` & `pulumi_openstack-3.9.0a1659603007/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/__init__.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,22 @@
   "fqn": "pulumi_openstack.containerinfra",
   "classes": {
    "openstack:containerinfra/clusterTemplate:ClusterTemplate": "ClusterTemplate"
   }
  },
  {
   "pkg": "openstack",
+  "mod": "containerinfra/nodeGroup",
+  "fqn": "pulumi_openstack.containerinfra",
+  "classes": {
+   "openstack:containerinfra/nodeGroup:NodeGroup": "NodeGroup"
+  }
+ },
+ {
+  "pkg": "openstack",
   "mod": "database/configuration",
   "fqn": "pulumi_openstack.database",
   "classes": {
    "openstack:database/configuration:Configuration": "Configuration"
   }
  },
  {
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/_utilities.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -230,7 +241,10 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+def get_plugin_download_url():
+	return None
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/__init__.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_availability_zones_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_availability_zones_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -100,18 +101,15 @@
            If omitted, the `region` argument of the provider is used.
     :param str state: The `state` of the availability zones to match. Can
            either be `available` or `unavailable`. Default is `available`.
     """
     __args__ = dict()
     __args__['region'] = region
     __args__['state'] = state
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:blockstorage/getAvailabilityZonesV3:getAvailabilityZonesV3', __args__, opts=opts, typ=GetAvailabilityZonesV3Result).value
 
     return AwaitableGetAvailabilityZonesV3Result(
         id=__ret__.id,
         names=__ret__.names,
         region=__ret__.region,
         state=__ret__.state)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_quotaset_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_quotaset_v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -182,18 +183,15 @@
     :param str project_id: The id of the project to retrieve the quotaset.
     :param str region: The region in which to obtain the V3 Blockstorage client.
            If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['projectId'] = project_id
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:blockstorage/getQuotasetV3:getQuotasetV3', __args__, opts=opts, typ=GetQuotasetV3Result).value
 
     return AwaitableGetQuotasetV3Result(
         backup_gigabytes=__ret__.backup_gigabytes,
         backups=__ret__.backups,
         gigabytes=__ret__.gigabytes,
         groups=__ret__.groups,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_snapshot_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_snapshot_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -166,18 +167,15 @@
     """
     __args__ = dict()
     __args__['mostRecent'] = most_recent
     __args__['name'] = name
     __args__['region'] = region
     __args__['status'] = status
     __args__['volumeId'] = volume_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:blockstorage/getSnapshotV2:getSnapshotV2', __args__, opts=opts, typ=GetSnapshotV2Result).value
 
     return AwaitableGetSnapshotV2Result(
         description=__ret__.description,
         id=__ret__.id,
         metadata=__ret__.metadata,
         most_recent=__ret__.most_recent,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_snapshot_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_snapshot_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -166,18 +167,15 @@
     """
     __args__ = dict()
     __args__['mostRecent'] = most_recent
     __args__['name'] = name
     __args__['region'] = region
     __args__['status'] = status
     __args__['volumeId'] = volume_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:blockstorage/getSnapshotV3:getSnapshotV3', __args__, opts=opts, typ=GetSnapshotV3Result).value
 
     return AwaitableGetSnapshotV3Result(
         description=__ret__.description,
         id=__ret__.id,
         metadata=__ret__.metadata,
         most_recent=__ret__.most_recent,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_volume_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_volume_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -170,18 +171,15 @@
     __args__ = dict()
     __args__['bootable'] = bootable
     __args__['metadata'] = metadata
     __args__['name'] = name
     __args__['region'] = region
     __args__['status'] = status
     __args__['volumeType'] = volume_type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:blockstorage/getVolumeV2:getVolumeV2', __args__, opts=opts, typ=GetVolumeV2Result).value
 
     return AwaitableGetVolumeV2Result(
         bootable=__ret__.bootable,
         id=__ret__.id,
         metadata=__ret__.metadata,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/get_volume_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/get_volume_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -197,18 +198,15 @@
     __args__['bootable'] = bootable
     __args__['host'] = host
     __args__['metadata'] = metadata
     __args__['name'] = name
     __args__['region'] = region
     __args__['status'] = status
     __args__['volumeType'] = volume_type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:blockstorage/getVolumeV3:getVolumeV3', __args__, opts=opts, typ=GetVolumeV3Result).value
 
     return AwaitableGetVolumeV3Result(
         bootable=__ret__.bootable,
         host=__ret__.host,
         id=__ret__.id,
         metadata=__ret__.metadata,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/qos_association_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/qos_association_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QosAssociationV3Args', 'QosAssociationV3']
@@ -236,20 +237,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  qos_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  volume_type_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QosAssociationV3Args.__new__(QosAssociationV3Args)
 
             if qos_id is None and not opts.urn:
                 raise TypeError("Missing required property 'qos_id'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/qos_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/qos_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QosV3Args', 'QosV3']
@@ -267,20 +268,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  consumer: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QosV3Args.__new__(QosV3Args)
 
             __props__.__dict__["consumer"] = consumer
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/quote_set_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/quote_set_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QuoteSetV2Args', 'QuoteSetV2']
@@ -546,20 +547,17 @@
                  per_volume_gigabytes: Optional[pulumi.Input[int]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  snapshots: Optional[pulumi.Input[int]] = None,
                  volume_type_quota: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  volumes: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QuoteSetV2Args.__new__(QuoteSetV2Args)
 
             __props__.__dict__["backup_gigabytes"] = backup_gigabytes
             __props__.__dict__["backups"] = backups
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/quote_set_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/quote_set_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QuoteSetV3Args', 'QuoteSetV3']
@@ -546,20 +547,17 @@
                  per_volume_gigabytes: Optional[pulumi.Input[int]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  snapshots: Optional[pulumi.Input[int]] = None,
                  volume_type_quota: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  volumes: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QuoteSetV3Args.__new__(QuoteSetV3Args)
 
             __props__.__dict__["backup_gigabytes"] = backup_gigabytes
             __props__.__dict__["backups"] = backups
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -715,20 +716,17 @@
                  scheduler_hints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VolumeSchedulerHintArgs']]]]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
                  source_replica: Optional[pulumi.Input[str]] = None,
                  source_vol_id: Optional[pulumi.Input[str]] = None,
                  volume_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeArgs.__new__(VolumeArgs)
 
             __props__.__dict__["availability_zone"] = availability_zone
             __props__.__dict__["consistency_group_id"] = consistency_group_id
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_attach.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_attach.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['VolumeAttachArgs', 'VolumeAttach']
@@ -607,20 +608,17 @@
                  os_type: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  wwnn: Optional[pulumi.Input[str]] = None,
                  wwpns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeAttachArgs.__new__(VolumeAttachArgs)
 
             __props__.__dict__["attach_mode"] = attach_mode
             __props__.__dict__["device"] = device
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_attach_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_attach_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['VolumeAttachV2Args', 'VolumeAttachV2']
@@ -639,20 +640,17 @@
                  os_type: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  wwnn: Optional[pulumi.Input[str]] = None,
                  wwpns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeAttachV2Args.__new__(VolumeAttachV2Args)
 
             __props__.__dict__["attach_mode"] = attach_mode
             __props__.__dict__["device"] = device
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_type_access_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_type_access_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['VolumeTypeAccessV3Args', 'VolumeTypeAccessV3']
@@ -228,20 +229,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  volume_type_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeTypeAccessV3Args.__new__(VolumeTypeAccessV3Args)
 
             if project_id is None and not opts.urn:
                 raise TypeError("Missing required property 'project_id'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_type_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_type_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['VolumeTypeV3Args', 'VolumeTypeV3']
@@ -307,20 +308,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  extra_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  is_public: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeTypeV3Args.__new__(VolumeTypeV3Args)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["extra_specs"] = extra_specs
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -525,20 +526,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
                  source_vol_id: Optional[pulumi.Input[str]] = None,
                  volume_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeV1Args.__new__(VolumeV1Args)
 
             __props__.__dict__["availability_zone"] = availability_zone
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/blockstorage/volume_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/blockstorage/volume_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -640,20 +641,17 @@
                  scheduler_hints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VolumeV2SchedulerHintArgs']]]]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
                  source_replica: Optional[pulumi.Input[str]] = None,
                  source_vol_id: Optional[pulumi.Input[str]] = None,
                  volume_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeV2Args.__new__(VolumeV2Args)
 
             __props__.__dict__["availability_zone"] = availability_zone
             __props__.__dict__["consistency_group_id"] = consistency_group_id
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/__init__.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .floating_ip_associate import *
 from .get_aggregate_v2 import *
 from .get_availability_zones import *
 from .get_flavor import *
 from .get_hypervisor_v2 import *
 from .get_instance_v2 import *
 from .get_keypair import *
+from .get_limits_v2 import *
 from .get_quota_set_v2 import *
 from .instance import *
 from .interface_attach import *
 from .keypair import *
 from .quota_set_v2 import *
 from .sec_group import *
 from .server_group import *
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/aggregate_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/aggregate_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['AggregateV2Args', 'AggregateV2']
@@ -337,20 +338,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  hosts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AggregateV2Args.__new__(AggregateV2Args)
 
             __props__.__dict__["hosts"] = hosts
             __props__.__dict__["metadata"] = metadata
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/flavor.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/flavor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['FlavorArgs', 'Flavor']
@@ -549,20 +550,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  ram: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  rx_tx_factor: Optional[pulumi.Input[float]] = None,
                  swap: Optional[pulumi.Input[int]] = None,
                  vcpus: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FlavorArgs.__new__(FlavorArgs)
 
             if disk is None and not opts.urn:
                 raise TypeError("Missing required property 'disk'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/flavor_access.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/flavor_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['FlavorAccessArgs', 'FlavorAccess']
@@ -237,20 +238,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  flavor_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FlavorAccessArgs.__new__(FlavorAccessArgs)
 
             if flavor_id is None and not opts.urn:
                 raise TypeError("Missing required property 'flavor_id'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/floating_ip.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/floating_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['FloatingIpArgs', 'FloatingIp']
@@ -247,20 +248,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  pool: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FloatingIpArgs.__new__(FloatingIpArgs)
 
             if pool is None and not opts.urn:
                 raise TypeError("Missing required property 'pool'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/floating_ip_associate.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/floating_ip_associate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['FloatingIpAssociateArgs', 'FloatingIpAssociate']
@@ -340,20 +341,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  fixed_ip: Optional[pulumi.Input[str]] = None,
                  floating_ip: Optional[pulumi.Input[str]] = None,
                  instance_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  wait_until_associated: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FloatingIpAssociateArgs.__new__(FloatingIpAssociateArgs)
 
             __props__.__dict__["fixed_ip"] = fixed_ip
             if floating_ip is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_aggregate_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_aggregate_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -113,18 +114,15 @@
     :param Mapping[str, str] metadata: Metadata of the Host Aggregate
     :param str name: The name of the host aggregate
     """
     __args__ = dict()
     __args__['hosts'] = hosts
     __args__['metadata'] = metadata
     __args__['name'] = name
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:compute/getAggregateV2:getAggregateV2', __args__, opts=opts, typ=GetAggregateV2Result).value
 
     return AwaitableGetAggregateV2Result(
         hosts=__ret__.hosts,
         id=__ret__.id,
         metadata=__ret__.metadata,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_availability_zones.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_availability_zones.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -91,18 +92,15 @@
 
     :param str region: The `region` to fetch availability zones from, defaults to the provider's `region`
     :param str state: The `state` of the availability zones to match, default ("available").
     """
     __args__ = dict()
     __args__['region'] = region
     __args__['state'] = state
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:compute/getAvailabilityZones:getAvailabilityZones', __args__, opts=opts, typ=GetAvailabilityZonesResult).value
 
     return AwaitableGetAvailabilityZonesResult(
         id=__ret__.id,
         names=__ret__.names,
         region=__ret__.region,
         state=__ret__.state)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_flavor.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_flavor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -204,18 +205,15 @@
     __args__['minRam'] = min_ram
     __args__['name'] = name
     __args__['ram'] = ram
     __args__['region'] = region
     __args__['rxTxFactor'] = rx_tx_factor
     __args__['swap'] = swap
     __args__['vcpus'] = vcpus
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:compute/getFlavor:getFlavor', __args__, opts=opts, typ=GetFlavorResult).value
 
     return AwaitableGetFlavorResult(
         disk=__ret__.disk,
         extra_specs=__ret__.extra_specs,
         flavor_id=__ret__.flavor_id,
         id=__ret__.id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_hypervisor_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_hypervisor_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -155,18 +156,15 @@
     ```
 
 
     :param str hostname: The hostname of the hypervisor
     """
     __args__ = dict()
     __args__['hostname'] = hostname
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:compute/getHypervisorV2:getHypervisorV2', __args__, opts=opts, typ=GetHypervisorV2Result).value
 
     return AwaitableGetHypervisorV2Result(
         disk=__ret__.disk,
         host_ip=__ret__.host_ip,
         hostname=__ret__.hostname,
         id=__ret__.id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_instance_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_instance_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -251,18 +252,15 @@
     :param str user_data: The user data added when the server was created.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['networks'] = networks
     __args__['region'] = region
     __args__['userData'] = user_data
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:compute/getInstanceV2:getInstanceV2', __args__, opts=opts, typ=GetInstanceV2Result).value
 
     return AwaitableGetInstanceV2Result(
         access_ip_v4=__ret__.access_ip_v4,
         access_ip_v6=__ret__.access_ip_v6,
         availability_zone=__ret__.availability_zone,
         flavor_id=__ret__.flavor_id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_keypair.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_keypair.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -110,18 +111,15 @@
     :param str name: The unique name of the keypair.
     :param str region: The region in which to obtain the V2 Compute client.
            If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:compute/getKeypair:getKeypair', __args__, opts=opts, typ=GetKeypairResult).value
 
     return AwaitableGetKeypairResult(
         fingerprint=__ret__.fingerprint,
         id=__ret__.id,
         name=__ret__.name,
         public_key=__ret__.public_key,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/get_quota_set_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/get_quota_set_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -254,18 +255,15 @@
     :param str project_id: The id of the project to retrieve the quotaset.
     :param str region: The region in which to obtain the V2 Compute client.
            If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['projectId'] = project_id
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:compute/getQuotaSetV2:getQuotaSetV2', __args__, opts=opts, typ=GetQuotaSetV2Result).value
 
     return AwaitableGetQuotaSetV2Result(
         cores=__ret__.cores,
         fixed_ips=__ret__.fixed_ips,
         floating_ips=__ret__.floating_ips,
         id=__ret__.id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/instance.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -71,18 +72,19 @@
         :param pulumi.Input[str] flavor_name: The name of the
                desired flavor for the server. Changing this resizes the existing server.
         :param pulumi.Input[bool] force_delete: Whether to force the OpenStack instance to be
                forcefully deleted. This is useful for environments that have reclaim / soft
                deletion enabled.
         :param pulumi.Input[str] image_id: (Optional; Required if `image_name` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The image ID of
-               the desired image for the server. Changing this creates a new server.
+               the desired image for the server. Changing this rebuilds the existing
+               server.
         :param pulumi.Input[str] image_name: (Optional; Required if `image_id` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The name of the
-               desired image for the server. Changing this creates a new server.
+               desired image for the server. Changing this rebuilds the existing server.
         :param pulumi.Input[str] key_pair: The name of a key pair to put on the server. The key
                pair must already be created and associated with the tenant's account.
                Changing this creates a new server.
         :param pulumi.Input[Mapping[str, Any]] metadata: Metadata key/value pairs to make available from
                within the instance. Changing this updates the existing server metadata.
         :param pulumi.Input[str] name: The human-readable
                name of the network. Changing this creates a new server.
@@ -90,15 +92,15 @@
                the server. `network_mode` can be `"auto"` or `"none"`.
                Please see the following [reference](https://docs.openstack.org/api-ref/compute/?expanded=create-server-detail#id11) for more information. Conflicts with `network`.
         :param pulumi.Input[Sequence[pulumi.Input['InstanceNetworkArgs']]] networks: An array of one or more networks to attach to the
                instance. The network object structure is documented below. Changing this
                creates a new server.
         :param pulumi.Input[Sequence[pulumi.Input['InstancePersonalityArgs']]] personalities: Customize the personality of an instance by
                defining one or more files and their contents. The personality structure
-               is described below.
+               is described below. Changing this rebuilds the existing server.
         :param pulumi.Input[str] power_state: Provide the VM state. Only 'active' and 'shutoff'
                are supported values. *Note*: If the initial power_state is the shutoff
                the VM will be stopped immediately after build and the provisioners like
                remote-exec or files are not supported.
         :param pulumi.Input[str] region: The region in which to create the server instance. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new server.
@@ -332,29 +334,30 @@
 
     @property
     @pulumi.getter(name="imageId")
     def image_id(self) -> Optional[pulumi.Input[str]]:
         """
         (Optional; Required if `image_name` is empty and not booting
         from a volume. Do not specify if booting from a volume.) The image ID of
-        the desired image for the server. Changing this creates a new server.
+        the desired image for the server. Changing this rebuilds the existing
+        server.
         """
         return pulumi.get(self, "image_id")
 
     @image_id.setter
     def image_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_id", value)
 
     @property
     @pulumi.getter(name="imageName")
     def image_name(self) -> Optional[pulumi.Input[str]]:
         """
         (Optional; Required if `image_id` is empty and not booting
         from a volume. Do not specify if booting from a volume.) The name of the
-        desired image for the server. Changing this creates a new server.
+        desired image for the server. Changing this rebuilds the existing server.
         """
         return pulumi.get(self, "image_name")
 
     @image_name.setter
     def image_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_name", value)
 
@@ -428,15 +431,15 @@
 
     @property
     @pulumi.getter
     def personalities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['InstancePersonalityArgs']]]]:
         """
         Customize the personality of an instance by
         defining one or more files and their contents. The personality structure
-        is described below.
+        is described below. Changing this rebuilds the existing server.
         """
         return pulumi.get(self, "personalities")
 
     @personalities.setter
     def personalities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePersonalityArgs']]]]):
         pulumi.set(self, "personalities", value)
 
@@ -625,18 +628,19 @@
         :param pulumi.Input[str] flavor_name: The name of the
                desired flavor for the server. Changing this resizes the existing server.
         :param pulumi.Input[bool] force_delete: Whether to force the OpenStack instance to be
                forcefully deleted. This is useful for environments that have reclaim / soft
                deletion enabled.
         :param pulumi.Input[str] image_id: (Optional; Required if `image_name` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The image ID of
-               the desired image for the server. Changing this creates a new server.
+               the desired image for the server. Changing this rebuilds the existing
+               server.
         :param pulumi.Input[str] image_name: (Optional; Required if `image_id` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The name of the
-               desired image for the server. Changing this creates a new server.
+               desired image for the server. Changing this rebuilds the existing server.
         :param pulumi.Input[str] key_pair: The name of a key pair to put on the server. The key
                pair must already be created and associated with the tenant's account.
                Changing this creates a new server.
         :param pulumi.Input[Mapping[str, Any]] metadata: Metadata key/value pairs to make available from
                within the instance. Changing this updates the existing server metadata.
         :param pulumi.Input[str] name: The human-readable
                name of the network. Changing this creates a new server.
@@ -644,15 +648,15 @@
                the server. `network_mode` can be `"auto"` or `"none"`.
                Please see the following [reference](https://docs.openstack.org/api-ref/compute/?expanded=create-server-detail#id11) for more information. Conflicts with `network`.
         :param pulumi.Input[Sequence[pulumi.Input['InstanceNetworkArgs']]] networks: An array of one or more networks to attach to the
                instance. The network object structure is documented below. Changing this
                creates a new server.
         :param pulumi.Input[Sequence[pulumi.Input['InstancePersonalityArgs']]] personalities: Customize the personality of an instance by
                defining one or more files and their contents. The personality structure
-               is described below.
+               is described below. Changing this rebuilds the existing server.
         :param pulumi.Input[str] power_state: Provide the VM state. Only 'active' and 'shutoff'
                are supported values. *Note*: If the initial power_state is the shutoff
                the VM will be stopped immediately after build and the provisioners like
                remote-exec or files are not supported.
         :param pulumi.Input[str] region: The region in which to create the server instance. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new server.
@@ -912,29 +916,30 @@
 
     @property
     @pulumi.getter(name="imageId")
     def image_id(self) -> Optional[pulumi.Input[str]]:
         """
         (Optional; Required if `image_name` is empty and not booting
         from a volume. Do not specify if booting from a volume.) The image ID of
-        the desired image for the server. Changing this creates a new server.
+        the desired image for the server. Changing this rebuilds the existing
+        server.
         """
         return pulumi.get(self, "image_id")
 
     @image_id.setter
     def image_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_id", value)
 
     @property
     @pulumi.getter(name="imageName")
     def image_name(self) -> Optional[pulumi.Input[str]]:
         """
         (Optional; Required if `image_id` is empty and not booting
         from a volume. Do not specify if booting from a volume.) The name of the
-        desired image for the server. Changing this creates a new server.
+        desired image for the server. Changing this rebuilds the existing server.
         """
         return pulumi.get(self, "image_name")
 
     @image_name.setter
     def image_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_name", value)
 
@@ -1008,15 +1013,15 @@
 
     @property
     @pulumi.getter
     def personalities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['InstancePersonalityArgs']]]]:
         """
         Customize the personality of an instance by
         defining one or more files and their contents. The personality structure
-        is described below.
+        is described below. Changing this rebuilds the existing server.
         """
         return pulumi.get(self, "personalities")
 
     @personalities.setter
     def personalities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePersonalityArgs']]]]):
         pulumi.set(self, "personalities", value)
 
@@ -1206,18 +1211,19 @@
         :param pulumi.Input[str] flavor_name: The name of the
                desired flavor for the server. Changing this resizes the existing server.
         :param pulumi.Input[bool] force_delete: Whether to force the OpenStack instance to be
                forcefully deleted. This is useful for environments that have reclaim / soft
                deletion enabled.
         :param pulumi.Input[str] image_id: (Optional; Required if `image_name` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The image ID of
-               the desired image for the server. Changing this creates a new server.
+               the desired image for the server. Changing this rebuilds the existing
+               server.
         :param pulumi.Input[str] image_name: (Optional; Required if `image_id` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The name of the
-               desired image for the server. Changing this creates a new server.
+               desired image for the server. Changing this rebuilds the existing server.
         :param pulumi.Input[str] key_pair: The name of a key pair to put on the server. The key
                pair must already be created and associated with the tenant's account.
                Changing this creates a new server.
         :param pulumi.Input[Mapping[str, Any]] metadata: Metadata key/value pairs to make available from
                within the instance. Changing this updates the existing server metadata.
         :param pulumi.Input[str] name: The human-readable
                name of the network. Changing this creates a new server.
@@ -1225,15 +1231,15 @@
                the server. `network_mode` can be `"auto"` or `"none"`.
                Please see the following [reference](https://docs.openstack.org/api-ref/compute/?expanded=create-server-detail#id11) for more information. Conflicts with `network`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceNetworkArgs']]]] networks: An array of one or more networks to attach to the
                instance. The network object structure is documented below. Changing this
                creates a new server.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePersonalityArgs']]]] personalities: Customize the personality of an instance by
                defining one or more files and their contents. The personality structure
-               is described below.
+               is described below. Changing this rebuilds the existing server.
         :param pulumi.Input[str] power_state: Provide the VM state. Only 'active' and 'shutoff'
                are supported values. *Note*: If the initial power_state is the shutoff
                the VM will be stopped immediately after build and the provisioners like
                remote-exec or files are not supported.
         :param pulumi.Input[str] region: The region in which to create the server instance. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new server.
@@ -1303,20 +1309,17 @@
                  security_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  stop_before_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  vendor_options: Optional[pulumi.Input[pulumi.InputType['InstanceVendorOptionsArgs']]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceVolumeArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["access_ip_v4"] = access_ip_v4
             __props__.__dict__["access_ip_v6"] = access_ip_v6
@@ -1429,18 +1432,19 @@
         :param pulumi.Input[str] flavor_name: The name of the
                desired flavor for the server. Changing this resizes the existing server.
         :param pulumi.Input[bool] force_delete: Whether to force the OpenStack instance to be
                forcefully deleted. This is useful for environments that have reclaim / soft
                deletion enabled.
         :param pulumi.Input[str] image_id: (Optional; Required if `image_name` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The image ID of
-               the desired image for the server. Changing this creates a new server.
+               the desired image for the server. Changing this rebuilds the existing
+               server.
         :param pulumi.Input[str] image_name: (Optional; Required if `image_id` is empty and not booting
                from a volume. Do not specify if booting from a volume.) The name of the
-               desired image for the server. Changing this creates a new server.
+               desired image for the server. Changing this rebuilds the existing server.
         :param pulumi.Input[str] key_pair: The name of a key pair to put on the server. The key
                pair must already be created and associated with the tenant's account.
                Changing this creates a new server.
         :param pulumi.Input[Mapping[str, Any]] metadata: Metadata key/value pairs to make available from
                within the instance. Changing this updates the existing server metadata.
         :param pulumi.Input[str] name: The human-readable
                name of the network. Changing this creates a new server.
@@ -1448,15 +1452,15 @@
                the server. `network_mode` can be `"auto"` or `"none"`.
                Please see the following [reference](https://docs.openstack.org/api-ref/compute/?expanded=create-server-detail#id11) for more information. Conflicts with `network`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceNetworkArgs']]]] networks: An array of one or more networks to attach to the
                instance. The network object structure is documented below. Changing this
                creates a new server.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePersonalityArgs']]]] personalities: Customize the personality of an instance by
                defining one or more files and their contents. The personality structure
-               is described below.
+               is described below. Changing this rebuilds the existing server.
         :param pulumi.Input[str] power_state: Provide the VM state. Only 'active' and 'shutoff'
                are supported values. *Note*: If the initial power_state is the shutoff
                the VM will be stopped immediately after build and the provisioners like
                remote-exec or files are not supported.
         :param pulumi.Input[str] region: The region in which to create the server instance. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new server.
@@ -1633,25 +1637,26 @@
 
     @property
     @pulumi.getter(name="imageId")
     def image_id(self) -> pulumi.Output[str]:
         """
         (Optional; Required if `image_name` is empty and not booting
         from a volume. Do not specify if booting from a volume.) The image ID of
-        the desired image for the server. Changing this creates a new server.
+        the desired image for the server. Changing this rebuilds the existing
+        server.
         """
         return pulumi.get(self, "image_id")
 
     @property
     @pulumi.getter(name="imageName")
     def image_name(self) -> pulumi.Output[str]:
         """
         (Optional; Required if `image_id` is empty and not booting
         from a volume. Do not specify if booting from a volume.) The name of the
-        desired image for the server. Changing this creates a new server.
+        desired image for the server. Changing this rebuilds the existing server.
         """
         return pulumi.get(self, "image_name")
 
     @property
     @pulumi.getter(name="keyPair")
     def key_pair(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1701,15 +1706,15 @@
 
     @property
     @pulumi.getter
     def personalities(self) -> pulumi.Output[Optional[Sequence['outputs.InstancePersonality']]]:
         """
         Customize the personality of an instance by
         defining one or more files and their contents. The personality structure
-        is described below.
+        is described below. Changing this rebuilds the existing server.
         """
         return pulumi.get(self, "personalities")
 
     @property
     @pulumi.getter(name="powerState")
     def power_state(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/interface_attach.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/interface_attach.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['InterfaceAttachArgs', 'InterfaceAttach']
@@ -360,20 +361,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  fixed_ip: Optional[pulumi.Input[str]] = None,
                  instance_id: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  port_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InterfaceAttachArgs.__new__(InterfaceAttachArgs)
 
             __props__.__dict__["fixed_ip"] = fixed_ip
             if instance_id is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/keypair.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/keypair.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['KeypairArgs', 'Keypair']
 
 @pulumi.input_type
 class KeypairArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None):
         """
         The set of arguments for constructing a Keypair resource.
         :param pulumi.Input[str] name: A unique name for the keypair. Changing this creates a new
                keypair.
         :param pulumi.Input[str] public_key: A pregenerated OpenSSH-formatted public key.
                Changing this creates a new keypair. If a public key is not specified, then
                a public/private key pair will be automatically generated. If a pair is
                created, then destroying this resource means you will lose access to that
                keypair forever.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Compute client.
                Keypairs are associated with accounts, but a Compute client is needed to
                create one. If omitted, the `region` argument of the provider is used.
                Changing this creates a new keypair.
+        :param pulumi.Input[str] user_id: This allows administrative users to operate key-pairs
+               of specified user ID. For this feature your need to have openstack microversion
+               2.10 (Liberty) or later.
         :param pulumi.Input[Mapping[str, Any]] value_specs: Map of additional options.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
         if value_specs is not None:
             pulumi.set(__self__, "value_specs", value_specs)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
@@ -82,14 +89,28 @@
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        This allows administrative users to operate key-pairs
+        of specified user ID. For this feature your need to have openstack microversion
+        2.10 (Liberty) or later.
+        """
+        return pulumi.get(self, "user_id")
+
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
+
+    @property
     @pulumi.getter(name="valueSpecs")
     def value_specs(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Map of additional options.
         """
         return pulumi.get(self, "value_specs")
 
@@ -102,14 +123,15 @@
 class _KeypairState:
     def __init__(__self__, *,
                  fingerprint: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  private_key: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None):
         """
         Input properties used for looking up and filtering Keypair resources.
         :param pulumi.Input[str] fingerprint: The fingerprint of the public key.
         :param pulumi.Input[str] name: A unique name for the keypair. Changing this creates a new
                keypair.
         :param pulumi.Input[str] private_key: The generated private key when no public key is specified.
@@ -118,26 +140,31 @@
                a public/private key pair will be automatically generated. If a pair is
                created, then destroying this resource means you will lose access to that
                keypair forever.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Compute client.
                Keypairs are associated with accounts, but a Compute client is needed to
                create one. If omitted, the `region` argument of the provider is used.
                Changing this creates a new keypair.
+        :param pulumi.Input[str] user_id: This allows administrative users to operate key-pairs
+               of specified user ID. For this feature your need to have openstack microversion
+               2.10 (Liberty) or later.
         :param pulumi.Input[Mapping[str, Any]] value_specs: Map of additional options.
         """
         if fingerprint is not None:
             pulumi.set(__self__, "fingerprint", fingerprint)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if private_key is not None:
             pulumi.set(__self__, "private_key", private_key)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
         if value_specs is not None:
             pulumi.set(__self__, "value_specs", value_specs)
 
     @property
     @pulumi.getter
     def fingerprint(self) -> Optional[pulumi.Input[str]]:
         """
@@ -202,14 +229,28 @@
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        This allows administrative users to operate key-pairs
+        of specified user ID. For this feature your need to have openstack microversion
+        2.10 (Liberty) or later.
+        """
+        return pulumi.get(self, "user_id")
+
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
+
+    @property
     @pulumi.getter(name="valueSpecs")
     def value_specs(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Map of additional options.
         """
         return pulumi.get(self, "value_specs")
 
@@ -222,14 +263,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
         """
         ## Example Usage
         ### Import an Existing Public Key
 
         ```python
@@ -264,14 +306,17 @@
                a public/private key pair will be automatically generated. If a pair is
                created, then destroying this resource means you will lose access to that
                keypair forever.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Compute client.
                Keypairs are associated with accounts, but a Compute client is needed to
                create one. If omitted, the `region` argument of the provider is used.
                Changing this creates a new keypair.
+        :param pulumi.Input[str] user_id: This allows administrative users to operate key-pairs
+               of specified user ID. For this feature your need to have openstack microversion
+               2.10 (Liberty) or later.
         :param pulumi.Input[Mapping[str, Any]] value_specs: Map of additional options.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[KeypairArgs] = None,
@@ -317,30 +362,29 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KeypairArgs.__new__(KeypairArgs)
 
             __props__.__dict__["name"] = name
             __props__.__dict__["public_key"] = public_key
             __props__.__dict__["region"] = region
+            __props__.__dict__["user_id"] = user_id
             __props__.__dict__["value_specs"] = value_specs
             __props__.__dict__["fingerprint"] = None
             __props__.__dict__["private_key"] = None
         super(Keypair, __self__).__init__(
             'openstack:compute/keypair:Keypair',
             resource_name,
             __props__,
@@ -351,14 +395,15 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             fingerprint: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             private_key: Optional[pulumi.Input[str]] = None,
             public_key: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
+            user_id: Optional[pulumi.Input[str]] = None,
             value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None) -> 'Keypair':
         """
         Get an existing Keypair resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
@@ -372,25 +417,29 @@
                a public/private key pair will be automatically generated. If a pair is
                created, then destroying this resource means you will lose access to that
                keypair forever.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Compute client.
                Keypairs are associated with accounts, but a Compute client is needed to
                create one. If omitted, the `region` argument of the provider is used.
                Changing this creates a new keypair.
+        :param pulumi.Input[str] user_id: This allows administrative users to operate key-pairs
+               of specified user ID. For this feature your need to have openstack microversion
+               2.10 (Liberty) or later.
         :param pulumi.Input[Mapping[str, Any]] value_specs: Map of additional options.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _KeypairState.__new__(_KeypairState)
 
         __props__.__dict__["fingerprint"] = fingerprint
         __props__.__dict__["name"] = name
         __props__.__dict__["private_key"] = private_key
         __props__.__dict__["public_key"] = public_key
         __props__.__dict__["region"] = region
+        __props__.__dict__["user_id"] = user_id
         __props__.__dict__["value_specs"] = value_specs
         return Keypair(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def fingerprint(self) -> pulumi.Output[str]:
         """
@@ -435,14 +484,24 @@
         Keypairs are associated with accounts, but a Compute client is needed to
         create one. If omitted, the `region` argument of the provider is used.
         Changing this creates a new keypair.
         """
         return pulumi.get(self, "region")
 
     @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Output[str]:
+        """
+        This allows administrative users to operate key-pairs
+        of specified user ID. For this feature your need to have openstack microversion
+        2.10 (Liberty) or later.
+        """
+        return pulumi.get(self, "user_id")
+
+    @property
     @pulumi.getter(name="valueSpecs")
     def value_specs(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
         """
         Map of additional options.
         """
         return pulumi.get(self, "value_specs")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/quota_set_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/quota_set_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QuotaSetV2Args', 'QuotaSetV2']
@@ -769,20 +770,17 @@
                  ram: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  security_group_rules: Optional[pulumi.Input[int]] = None,
                  security_groups: Optional[pulumi.Input[int]] = None,
                  server_group_members: Optional[pulumi.Input[int]] = None,
                  server_groups: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QuotaSetV2Args.__new__(QuotaSetV2Args)
 
             __props__.__dict__["cores"] = cores
             __props__.__dict__["fixed_ips"] = fixed_ips
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/sec_group.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/sec_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -368,20 +369,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecGroupRuleArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecGroupArgs.__new__(SecGroupArgs)
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/server_group.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/server_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ServerGroupArgs', 'ServerGroup']
@@ -308,20 +309,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  policies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ServerGroupArgs.__new__(ServerGroupArgs)
 
             __props__.__dict__["name"] = name
             __props__.__dict__["policies"] = policies
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/compute/volume_attach.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/compute/volume_attach.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -399,20 +400,17 @@
                  device: Optional[pulumi.Input[str]] = None,
                  instance_id: Optional[pulumi.Input[str]] = None,
                  multiattach: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  vendor_options: Optional[pulumi.Input[pulumi.InputType['VolumeAttachVendorOptionsArgs']]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeAttachArgs.__new__(VolumeAttachArgs)
 
             __props__.__dict__["device"] = device
             if instance_id is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/config/vars.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/config/vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 import types
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/cluster.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ClusterArgs', 'Cluster']
@@ -976,20 +977,17 @@
                  master_count: Optional[pulumi.Input[int]] = None,
                  master_flavor: Optional[pulumi.Input[str]] = None,
                  merge_labels: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClusterArgs.__new__(ClusterArgs)
 
             if cluster_template_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster_template_id'")
@@ -1301,15 +1299,15 @@
     @property
     @pulumi.getter(name="nodeAddresses")
     def node_addresses(self) -> pulumi.Output[Sequence[str]]:
         return pulumi.get(self, "node_addresses")
 
     @property
     @pulumi.getter(name="nodeCount")
-    def node_count(self) -> pulumi.Output[int]:
+    def node_count(self) -> pulumi.Output[Optional[int]]:
         """
         The number of nodes for the cluster. Changing this
         creates a new cluster.
         """
         return pulumi.get(self, "node_count")
 
     @property
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/cluster_template.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/cluster_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ClusterTemplateArgs', 'ClusterTemplate']
@@ -1505,20 +1506,17 @@
                  public: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  registry_enabled: Optional[pulumi.Input[bool]] = None,
                  server_type: Optional[pulumi.Input[str]] = None,
                  tls_disabled: Optional[pulumi.Input[bool]] = None,
                  volume_driver: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClusterTemplateArgs.__new__(ClusterTemplateArgs)
 
             __props__.__dict__["apiserver_port"] = apiserver_port
             __props__.__dict__["cluster_distro"] = cluster_distro
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/get_cluster.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/get_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -358,18 +359,15 @@
     :param str region: The region in which to obtain the V1 Container Infra
            client.
            If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:containerinfra/getCluster:getCluster', __args__, opts=opts, typ=GetClusterResult).value
 
     return AwaitableGetClusterResult(
         api_address=__ret__.api_address,
         cluster_template_id=__ret__.cluster_template_id,
         coe_version=__ret__.coe_version,
         container_version=__ret__.container_version,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/containerinfra/get_cluster_template.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/containerinfra/get_cluster_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -460,18 +461,15 @@
     :param str region: The region in which to obtain the V1 Container Infra
            client.
            If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:containerinfra/getClusterTemplate:getClusterTemplate', __args__, opts=opts, typ=GetClusterTemplateResult).value
 
     return AwaitableGetClusterTemplateResult(
         apiserver_port=__ret__.apiserver_port,
         cluster_distro=__ret__.cluster_distro,
         coe=__ret__.coe,
         created_at=__ret__.created_at,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/configuration.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -282,20 +283,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  configurations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ConfigurationConfigurationArgs']]]]] = None,
                  datastore: Optional[pulumi.Input[pulumi.InputType['ConfigurationDatastoreArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ConfigurationArgs.__new__(ConfigurationArgs)
 
             __props__.__dict__["configurations"] = configurations
             if datastore is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/database.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['DatabaseArgs', 'Database']
@@ -199,20 +200,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  instance_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseArgs.__new__(DatabaseArgs)
 
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/instance.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -471,20 +472,17 @@
                  flavor_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  networks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceNetworkArgs']]]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  users: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceUserArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["configuration_id"] = configuration_id
             __props__.__dict__["databases"] = databases
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/database/user.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/database/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['UserArgs', 'User']
@@ -249,20 +250,17 @@
                  databases: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  host: Optional[pulumi.Input[str]] = None,
                  instance_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserArgs.__new__(UserArgs)
 
             __props__.__dict__["databases"] = databases
             __props__.__dict__["host"] = host
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/get_dns_zone.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/get_dns_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -311,18 +312,15 @@
     __args__['serial'] = serial
     __args__['status'] = status
     __args__['transferredAt'] = transferred_at
     __args__['ttl'] = ttl
     __args__['type'] = type
     __args__['updatedAt'] = updated_at
     __args__['version'] = version
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:dns/getDnsZone:getDnsZone', __args__, opts=opts, typ=GetDnsZoneResult).value
 
     return AwaitableGetDnsZoneResult(
         all_projects=__ret__.all_projects,
         attributes=__ret__.attributes,
         created_at=__ret__.created_at,
         description=__ret__.description,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/record_set.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/record_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RecordSetArgs', 'RecordSet']
@@ -524,20 +525,17 @@
                  records: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  zone_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RecordSetArgs.__new__(RecordSetArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["disable_status_check"] = disable_status_check
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/transfer_accept.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/transfer_accept.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['TransferAcceptArgs', 'TransferAccept']
@@ -318,20 +319,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  disable_status_check: Optional[pulumi.Input[bool]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  zone_transfer_request_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TransferAcceptArgs.__new__(TransferAcceptArgs)
 
             __props__.__dict__["disable_status_check"] = disable_status_check
             if key is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/transfer_request.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['TransferRequestArgs', 'TransferRequest']
@@ -379,20 +380,17 @@
                  disable_status_check: Optional[pulumi.Input[bool]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  target_project_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  zone_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TransferRequestArgs.__new__(TransferRequestArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["disable_status_check"] = disable_status_check
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/dns/zone.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/dns/zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ZoneArgs', 'Zone']
@@ -556,20 +557,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ZoneArgs.__new__(ZoneArgs)
 
             __props__.__dict__["attributes"] = attributes
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/firewall.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/firewall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['FirewallArgs', 'Firewall']
@@ -509,20 +510,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  no_routers: Optional[pulumi.Input[bool]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FirewallArgs.__new__(FirewallArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["associated_routers"] = associated_routers
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/get_policy.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/get_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -165,18 +166,15 @@
     :param str tenant_id: The owner of the firewall policy.
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['policyId'] = policy_id
     __args__['region'] = region
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:firewall/getPolicy:getPolicy', __args__, opts=opts, typ=GetPolicyResult).value
 
     return AwaitableGetPolicyResult(
         audited=__ret__.audited,
         description=__ret__.description,
         id=__ret__.id,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/policy.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PolicyArgs', 'Policy']
@@ -469,20 +470,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  shared: Optional[pulumi.Input[bool]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PolicyArgs.__new__(PolicyArgs)
 
             __props__.__dict__["audited"] = audited
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/firewall/rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/firewall/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RuleArgs', 'Rule']
@@ -666,20 +667,17 @@
                  protocol: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  source_ip_address: Optional[pulumi.Input[str]] = None,
                  source_port: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RuleArgs.__new__(RuleArgs)
 
             if action is None and not opts.urn:
                 raise TypeError("Missing required property 'action'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/__init__.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -22,16 +23,16 @@
                  id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] method: The request method that the application credential is
                permitted to use for a given API endpoint. Allowed values: `POST`, `GET`,
                `HEAD`, `PATCH`, `PUT` and `DELETE`.
         :param pulumi.Input[str] path: The API path that the application credential is permitted
                to access. May use named wildcards such as **{tag}** or the unnamed wildcard
-               **\*** to match against any string in the path up to a **/**, or the recursive
-               wildcard **\*\*** to include **/** in the matched path.
+               **\\*** to match against any string in the path up to a **/**, or the recursive
+               wildcard **\\*\\*** to include **/** in the matched path.
         :param pulumi.Input[str] service: The service type identifier for the service that the
                application credential is granted to access. Must be a service type that is
                listed in the service catalog and not a code name for a service. E.g.
                **identity**, **compute**, **volumev3**, **image**, **network**,
                **object-store**, **sharev2**, **dns**, **key-manager**, **monitoring**, etc.
         :param pulumi.Input[str] id: The ID of the existing access rule. The access rule ID of
                another application credential can be provided.
@@ -58,16 +59,16 @@
 
     @property
     @pulumi.getter
     def path(self) -> pulumi.Input[str]:
         """
         The API path that the application credential is permitted
         to access. May use named wildcards such as **{tag}** or the unnamed wildcard
-        **\*** to match against any string in the path up to a **/**, or the recursive
-        wildcard **\*\*** to include **/** in the matched path.
+        **\\*** to match against any string in the path up to a **/**, or the recursive
+        wildcard **\\*\\*** to include **/** in the matched path.
         """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: pulumi.Input[str]):
         pulumi.set(self, "path", value)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/application_credential.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/application_credential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -572,20 +573,17 @@
                  expires_at: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  unrestricted: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ApplicationCredentialArgs.__new__(ApplicationCredentialArgs)
 
             __props__.__dict__["access_rules"] = access_rules
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/ec2_credential_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/ec2_credential_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['Ec2CredentialV3Args', 'Ec2CredentialV3']
@@ -280,20 +281,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = Ec2CredentialV3Args.__new__(Ec2CredentialV3Args)
 
             __props__.__dict__["project_id"] = project_id
             __props__.__dict__["region"] = region
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/endpoint_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/endpoint_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['EndpointV3Args', 'EndpointV3']
@@ -359,20 +360,17 @@
                  endpoint_region: Optional[pulumi.Input[str]] = None,
                  interface: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EndpointV3Args.__new__(EndpointV3Args)
 
             if endpoint_region is None and not opts.urn:
                 raise TypeError("Missing required property 'endpoint_region'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_auth_scope.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_auth_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -246,18 +247,15 @@
     :param str region: The region in which to obtain the V3 Identity client.
            A Identity client is needed to retrieve tokens IDs. If omitted, the
            `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:identity/getAuthScope:getAuthScope', __args__, opts=opts, typ=GetAuthScopeResult).value
 
     return AwaitableGetAuthScopeResult(
         domain_id=__ret__.domain_id,
         domain_name=__ret__.domain_name,
         id=__ret__.id,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_endpoint.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -177,18 +178,15 @@
     __args__['endpointRegion'] = endpoint_region
     __args__['interface'] = interface
     __args__['name'] = name
     __args__['region'] = region
     __args__['serviceId'] = service_id
     __args__['serviceName'] = service_name
     __args__['serviceType'] = service_type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:identity/getEndpoint:getEndpoint', __args__, opts=opts, typ=GetEndpointResult).value
 
     return AwaitableGetEndpointResult(
         endpoint_region=__ret__.endpoint_region,
         id=__ret__.id,
         interface=__ret__.interface,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_group.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -116,18 +117,15 @@
     :param str region: The region in which to obtain the V3 Keystone client.
            If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['domainId'] = domain_id
     __args__['name'] = name
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:identity/getGroup:getGroup', __args__, opts=opts, typ=GetGroupResult).value
 
     return AwaitableGetGroupResult(
         description=__ret__.description,
         domain_id=__ret__.domain_id,
         id=__ret__.id,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_project.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -171,18 +172,15 @@
     __args__ = dict()
     __args__['domainId'] = domain_id
     __args__['enabled'] = enabled
     __args__['isDomain'] = is_domain
     __args__['name'] = name
     __args__['parentId'] = parent_id
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:identity/getProject:getProject', __args__, opts=opts, typ=GetProjectResult).value
 
     return AwaitableGetProjectResult(
         description=__ret__.description,
         domain_id=__ret__.domain_id,
         enabled=__ret__.enabled,
         id=__ret__.id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_role.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -101,18 +102,15 @@
     :param str region: The region in which to obtain the V3 Keystone client.
            If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['domainId'] = domain_id
     __args__['name'] = name
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:identity/getRole:getRole', __args__, opts=opts, typ=GetRoleResult).value
 
     return AwaitableGetRoleResult(
         domain_id=__ret__.domain_id,
         id=__ret__.id,
         name=__ret__.name,
         region=__ret__.region)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_service.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -130,18 +131,15 @@
     :param str type: The service type.
     """
     __args__ = dict()
     __args__['enabled'] = enabled
     __args__['name'] = name
     __args__['region'] = region
     __args__['type'] = type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:identity/getService:getService', __args__, opts=opts, typ=GetServiceResult).value
 
     return AwaitableGetServiceResult(
         description=__ret__.description,
         enabled=__ret__.enabled,
         id=__ret__.id,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/get_user.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/get_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -200,18 +201,15 @@
     __args__['enabled'] = enabled
     __args__['idpId'] = idp_id
     __args__['name'] = name
     __args__['passwordExpiresAt'] = password_expires_at
     __args__['protocolId'] = protocol_id
     __args__['region'] = region
     __args__['uniqueId'] = unique_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:identity/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
         default_project_id=__ret__.default_project_id,
         description=__ret__.description,
         domain_id=__ret__.domain_id,
         enabled=__ret__.enabled,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/group_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/group_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['GroupV3Args', 'GroupV3']
@@ -249,20 +250,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  domain_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GroupV3Args.__new__(GroupV3Args)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["domain_id"] = domain_id
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -26,16 +27,16 @@
                  id: Optional[str] = None):
         """
         :param str method: The request method that the application credential is
                permitted to use for a given API endpoint. Allowed values: `POST`, `GET`,
                `HEAD`, `PATCH`, `PUT` and `DELETE`.
         :param str path: The API path that the application credential is permitted
                to access. May use named wildcards such as **{tag}** or the unnamed wildcard
-               **\*** to match against any string in the path up to a **/**, or the recursive
-               wildcard **\*\*** to include **/** in the matched path.
+               **\\*** to match against any string in the path up to a **/**, or the recursive
+               wildcard **\\*\\*** to include **/** in the matched path.
         :param str service: The service type identifier for the service that the
                application credential is granted to access. Must be a service type that is
                listed in the service catalog and not a code name for a service. E.g.
                **identity**, **compute**, **volumev3**, **image**, **network**,
                **object-store**, **sharev2**, **dns**, **key-manager**, **monitoring**, etc.
         :param str id: The ID of the existing access rule. The access rule ID of
                another application credential can be provided.
@@ -58,16 +59,16 @@
 
     @property
     @pulumi.getter
     def path(self) -> str:
         """
         The API path that the application credential is permitted
         to access. May use named wildcards such as **{tag}** or the unnamed wildcard
-        **\*** to match against any string in the path up to a **/**, or the recursive
-        wildcard **\*\*** to include **/** in the matched path.
+        **\\*** to match against any string in the path up to a **/**, or the recursive
+        wildcard **\\*\\*** to include **/** in the matched path.
         """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def service(self) -> str:
         """
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/project.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProjectArgs', 'Project']
@@ -414,20 +415,17 @@
                  enabled: Optional[pulumi.Input[bool]] = None,
                  is_domain: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectArgs.__new__(ProjectArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["domain_id"] = domain_id
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/role.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RoleArgs', 'Role']
@@ -214,20 +215,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  domain_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RoleArgs.__new__(RoleArgs)
 
             __props__.__dict__["domain_id"] = domain_id
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/role_assignment.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RoleAssignmentArgs', 'RoleAssignment']
@@ -295,20 +296,17 @@
                  domain_id: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RoleAssignmentArgs.__new__(RoleAssignmentArgs)
 
             __props__.__dict__["domain_id"] = domain_id
             __props__.__dict__["group_id"] = group_id
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/service_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/service_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ServiceV3Args', 'ServiceV3']
@@ -276,20 +277,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ServiceV3Args.__new__(ServiceV3Args)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["enabled"] = enabled
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/user.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -636,20 +637,17 @@
                  ignore_password_expiry: Optional[pulumi.Input[bool]] = None,
                  multi_factor_auth_enabled: Optional[pulumi.Input[bool]] = None,
                  multi_factor_auth_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserMultiFactorAuthRuleArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserArgs.__new__(UserArgs)
 
             __props__.__dict__["default_project_id"] = default_project_id
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/identity/user_membership_v3.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/identity/user_membership_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['UserMembershipV3Args', 'UserMembershipV3']
@@ -241,20 +242,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserMembershipV3Args.__new__(UserMembershipV3Args)
 
             if group_id is None and not opts.urn:
                 raise TypeError("Missing required property 'group_id'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/get_image.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/get_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -384,18 +385,15 @@
     __args__['region'] = region
     __args__['sizeMax'] = size_max
     __args__['sizeMin'] = size_min
     __args__['sortDirection'] = sort_direction
     __args__['sortKey'] = sort_key
     __args__['tag'] = tag
     __args__['visibility'] = visibility
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:images/getImage:getImage', __args__, opts=opts, typ=GetImageResult).value
 
     return AwaitableGetImageResult(
         checksum=__ret__.checksum,
         container_format=__ret__.container_format,
         created_at=__ret__.created_at,
         disk_format=__ret__.disk_format,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/get_image_ids.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/get_image_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -197,15 +198,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_openstack as openstack
 
-    images = openstack.images.get_image_ids(name_regex="^Ubuntu 16\\.04.*-amd64",
+    images = openstack.images.get_image_ids(name_regex="^Ubuntu 16\\\\.04.*-amd64",
         properties={
             "key": "value",
         },
         sort="updated_at")
     ```
 
 
@@ -253,18 +254,15 @@
     __args__['sizeMax'] = size_max
     __args__['sizeMin'] = size_min
     __args__['sort'] = sort
     __args__['sortDirection'] = sort_direction
     __args__['sortKey'] = sort_key
     __args__['tag'] = tag
     __args__['visibility'] = visibility
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:images/getImageIds:getImageIds', __args__, opts=opts, typ=GetImageIdsResult).value
 
     return AwaitableGetImageIdsResult(
         id=__ret__.id,
         ids=__ret__.ids,
         member_status=__ret__.member_status,
         name=__ret__.name,
@@ -302,15 +300,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_openstack as openstack
 
-    images = openstack.images.get_image_ids(name_regex="^Ubuntu 16\\.04.*-amd64",
+    images = openstack.images.get_image_ids(name_regex="^Ubuntu 16\\\\.04.*-amd64",
         properties={
             "key": "value",
         },
         sort="updated_at")
     ```
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/image.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ImageArgs', 'Image']
@@ -1080,20 +1081,17 @@
                  protected: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  verify_checksum: Optional[pulumi.Input[bool]] = None,
                  visibility: Optional[pulumi.Input[str]] = None,
                  web_download: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ImageArgs.__new__(ImageArgs)
 
             if container_format is None and not opts.urn:
                 raise TypeError("Missing required property 'container_format'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/image_access.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/image_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ImageAccessArgs', 'ImageAccess']
@@ -373,20 +374,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  image_id: Optional[pulumi.Input[str]] = None,
                  member_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ImageAccessArgs.__new__(ImageAccessArgs)
 
             if image_id is None and not opts.urn:
                 raise TypeError("Missing required property 'image_id'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/images/image_access_accept.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/images/image_access_accept.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ImageAccessAcceptArgs', 'ImageAccessAccept']
@@ -320,20 +321,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  image_id: Optional[pulumi.Input[str]] = None,
                  member_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ImageAccessAcceptArgs.__new__(ImageAccessAcceptArgs)
 
             if image_id is None and not opts.urn:
                 raise TypeError("Missing required property 'image_id'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/container_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/container_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -537,20 +538,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acl: Optional[pulumi.Input[pulumi.InputType['ContainerV1AclArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  secret_refs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ContainerV1SecretRefArgs']]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ContainerV1Args.__new__(ContainerV1Args)
 
             __props__.__dict__["acl"] = acl
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/get_container.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/get_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -199,18 +200,15 @@
     :param str region: The region in which to obtain the V1 KeyManager client.
            A KeyManager client is needed to fetch a container. If omitted, the `region`
            argument of the provider is used.
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:keymanager/getContainer:getContainer', __args__, opts=opts, typ=GetContainerResult).value
 
     return AwaitableGetContainerResult(
         acls=__ret__.acls,
         consumers=__ret__.consumers,
         container_ref=__ret__.container_ref,
         created_at=__ret__.created_at,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/get_secret.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/get_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -379,18 +380,15 @@
     __args__['createdAtFilter'] = created_at_filter
     __args__['expirationFilter'] = expiration_filter
     __args__['mode'] = mode
     __args__['name'] = name
     __args__['region'] = region
     __args__['secretType'] = secret_type
     __args__['updatedAtFilter'] = updated_at_filter
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:keymanager/getSecret:getSecret', __args__, opts=opts, typ=GetSecretResult).value
 
     return AwaitableGetSecretResult(
         acl_only=__ret__.acl_only,
         acls=__ret__.acls,
         algorithm=__ret__.algorithm,
         bit_length=__ret__.bit_length,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/order_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/order_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -401,20 +402,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  meta: Optional[pulumi.Input[pulumi.InputType['OrderV1MetaArgs']]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = OrderV1Args.__new__(OrderV1Args)
 
             if meta is None and not opts.urn:
                 raise TypeError("Missing required property 'meta'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/keymanager/secret_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/keymanager/secret_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -35,15 +36,15 @@
         :param pulumi.Input[str] algorithm: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[int] bit_length: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[str] expiration: The expiration time of the secret in the RFC3339 timestamp format (e.g. `2019-03-09T12:58:49Z`). If omitted, a secret will never expire. Changing this creates a new secret.
         :param pulumi.Input[Mapping[str, Any]] metadata: Additional Metadata for the secret.
         :param pulumi.Input[str] mode: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[str] name: Human-readable name for the Secret. Does not have
                to be unique.
-        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\_content\_type** must also be supplied if **payload** is included.
+        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\\_content\\_type** must also be supplied if **payload** is included.
         :param pulumi.Input[str] payload_content_encoding: (required if **payload** is encoded) The encoding used for the payload to be able to include it in the JSON request. Must be either `base64` or `binary`.
         :param pulumi.Input[str] payload_content_type: (required if **payload** is included) The media type for the content of the payload. Must be one of `text/plain`, `text/plain;charset=utf-8`, `text/plain; charset=utf-8`, `application/octet-stream`, `application/pkcs8`.
         :param pulumi.Input[str] region: The region in which to obtain the V1 KeyManager client.
                A KeyManager client is needed to create a secret. If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                V1 secret.
         :param pulumi.Input[str] secret_type: Used to indicate the type of secret being stored. For more information see [Secret types](https://docs.openstack.org/barbican/latest/api/reference/secret_types.html).
@@ -160,15 +161,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def payload(self) -> Optional[pulumi.Input[str]]:
         """
-        The secret's data to be stored. **payload\_content\_type** must also be supplied if **payload** is included.
+        The secret's data to be stored. **payload\\_content\\_type** must also be supplied if **payload** is included.
         """
         return pulumi.get(self, "payload")
 
     @payload.setter
     def payload(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "payload", value)
 
@@ -259,15 +260,15 @@
         :param pulumi.Input[str] created_at: The date the secret ACL was created.
         :param pulumi.Input[str] creator_id: The creator of the secret.
         :param pulumi.Input[str] expiration: The expiration time of the secret in the RFC3339 timestamp format (e.g. `2019-03-09T12:58:49Z`). If omitted, a secret will never expire. Changing this creates a new secret.
         :param pulumi.Input[Mapping[str, Any]] metadata: Additional Metadata for the secret.
         :param pulumi.Input[str] mode: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[str] name: Human-readable name for the Secret. Does not have
                to be unique.
-        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\_content\_type** must also be supplied if **payload** is included.
+        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\\_content\\_type** must also be supplied if **payload** is included.
         :param pulumi.Input[str] payload_content_encoding: (required if **payload** is encoded) The encoding used for the payload to be able to include it in the JSON request. Must be either `base64` or `binary`.
         :param pulumi.Input[str] payload_content_type: (required if **payload** is included) The media type for the content of the payload. Must be one of `text/plain`, `text/plain;charset=utf-8`, `text/plain; charset=utf-8`, `application/octet-stream`, `application/pkcs8`.
         :param pulumi.Input[str] region: The region in which to obtain the V1 KeyManager client.
                A KeyManager client is needed to create a secret. If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                V1 secret.
         :param pulumi.Input[str] secret_ref: The secret reference / where to find the secret.
@@ -450,15 +451,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def payload(self) -> Optional[pulumi.Input[str]]:
         """
-        The secret's data to be stored. **payload\_content\_type** must also be supplied if **payload** is included.
+        The secret's data to be stored. **payload\\_content\\_type** must also be supplied if **payload** is included.
         """
         return pulumi.get(self, "payload")
 
     @payload.setter
     def payload(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "payload", value)
 
@@ -626,15 +627,15 @@
         :param pulumi.Input[str] algorithm: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[int] bit_length: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[str] expiration: The expiration time of the secret in the RFC3339 timestamp format (e.g. `2019-03-09T12:58:49Z`). If omitted, a secret will never expire. Changing this creates a new secret.
         :param pulumi.Input[Mapping[str, Any]] metadata: Additional Metadata for the secret.
         :param pulumi.Input[str] mode: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[str] name: Human-readable name for the Secret. Does not have
                to be unique.
-        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\_content\_type** must also be supplied if **payload** is included.
+        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\\_content\\_type** must also be supplied if **payload** is included.
         :param pulumi.Input[str] payload_content_encoding: (required if **payload** is encoded) The encoding used for the payload to be able to include it in the JSON request. Must be either `base64` or `binary`.
         :param pulumi.Input[str] payload_content_type: (required if **payload** is included) The media type for the content of the payload. Must be one of `text/plain`, `text/plain;charset=utf-8`, `text/plain; charset=utf-8`, `application/octet-stream`, `application/pkcs8`.
         :param pulumi.Input[str] region: The region in which to obtain the V1 KeyManager client.
                A KeyManager client is needed to create a secret. If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                V1 secret.
         :param pulumi.Input[str] secret_type: Used to indicate the type of secret being stored. For more information see [Secret types](https://docs.openstack.org/barbican/latest/api/reference/secret_types.html).
@@ -719,20 +720,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  payload: Optional[pulumi.Input[str]] = None,
                  payload_content_encoding: Optional[pulumi.Input[str]] = None,
                  payload_content_type: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  secret_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecretV1Args.__new__(SecretV1Args)
 
             __props__.__dict__["acl"] = acl
             __props__.__dict__["algorithm"] = algorithm
@@ -800,15 +798,15 @@
         :param pulumi.Input[str] created_at: The date the secret ACL was created.
         :param pulumi.Input[str] creator_id: The creator of the secret.
         :param pulumi.Input[str] expiration: The expiration time of the secret in the RFC3339 timestamp format (e.g. `2019-03-09T12:58:49Z`). If omitted, a secret will never expire. Changing this creates a new secret.
         :param pulumi.Input[Mapping[str, Any]] metadata: Additional Metadata for the secret.
         :param pulumi.Input[str] mode: Metadata provided by a user or system for informational purposes.
         :param pulumi.Input[str] name: Human-readable name for the Secret. Does not have
                to be unique.
-        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\_content\_type** must also be supplied if **payload** is included.
+        :param pulumi.Input[str] payload: The secret's data to be stored. **payload\\_content\\_type** must also be supplied if **payload** is included.
         :param pulumi.Input[str] payload_content_encoding: (required if **payload** is encoded) The encoding used for the payload to be able to include it in the JSON request. Must be either `base64` or `binary`.
         :param pulumi.Input[str] payload_content_type: (required if **payload** is included) The media type for the content of the payload. Must be one of `text/plain`, `text/plain;charset=utf-8`, `text/plain; charset=utf-8`, `application/octet-stream`, `application/pkcs8`.
         :param pulumi.Input[str] region: The region in which to obtain the V1 KeyManager client.
                A KeyManager client is needed to create a secret. If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                V1 secret.
         :param pulumi.Input[str] secret_ref: The secret reference / where to find the secret.
@@ -933,15 +931,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def payload(self) -> pulumi.Output[str]:
         """
-        The secret's data to be stored. **payload\_content\_type** must also be supplied if **payload** is included.
+        The secret's data to be stored. **payload\\_content\\_type** must also be supplied if **payload** is included.
         """
         return pulumi.get(self, "payload")
 
     @property
     @pulumi.getter(name="payloadContentEncoding")
     def payload_content_encoding(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/__init__.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/_inputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -17,26 +18,32 @@
 class MembersMemberArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  protocol_port: pulumi.Input[int],
                  admin_state_up: Optional[pulumi.Input[bool]] = None,
                  backup: Optional[pulumi.Input[bool]] = None,
                  id: Optional[pulumi.Input[str]] = None,
+                 monitor_address: Optional[pulumi.Input[str]] = None,
+                 monitor_port: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] address: The IP address of the members to receive traffic from
                the load balancer.
         :param pulumi.Input[int] protocol_port: The port on which to listen for client traffic.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the member.
                A valid value is true (UP) or false (DOWN). Defaults to true.
         :param pulumi.Input[bool] backup: A bool that indicates whether the member is
                backup. **Requires octavia minor version 2.1 or later**.
         :param pulumi.Input[str] id: The unique ID for the members.
+        :param pulumi.Input[str] monitor_address: An alternate IP address used for health 
+               monitoring a backend member.
+        :param pulumi.Input[int] monitor_port: An alternate protocol port used for health 
+               monitoring a backend member.
         :param pulumi.Input[str] name: Human-readable name for the member.
         :param pulumi.Input[str] subnet_id: The subnet in which to access the member.
         :param pulumi.Input[int] weight: A positive integer value that indicates the relative
                portion of traffic that this members should receive from the pool. For
                example, a member with a weight of 10 receives five times as much traffic
                as a member with a weight of 2. Defaults to 1.
         """
@@ -44,14 +51,18 @@
         pulumi.set(__self__, "protocol_port", protocol_port)
         if admin_state_up is not None:
             pulumi.set(__self__, "admin_state_up", admin_state_up)
         if backup is not None:
             pulumi.set(__self__, "backup", backup)
         if id is not None:
             pulumi.set(__self__, "id", id)
+        if monitor_address is not None:
+            pulumi.set(__self__, "monitor_address", monitor_address)
+        if monitor_port is not None:
+            pulumi.set(__self__, "monitor_port", monitor_port)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if subnet_id is not None:
             pulumi.set(__self__, "subnet_id", subnet_id)
         if weight is not None:
             pulumi.set(__self__, "weight", weight)
 
@@ -115,14 +126,40 @@
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
     @property
+    @pulumi.getter(name="monitorAddress")
+    def monitor_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        An alternate IP address used for health 
+        monitoring a backend member.
+        """
+        return pulumi.get(self, "monitor_address")
+
+    @monitor_address.setter
+    def monitor_address(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "monitor_address", value)
+
+    @property
+    @pulumi.getter(name="monitorPort")
+    def monitor_port(self) -> Optional[pulumi.Input[int]]:
+        """
+        An alternate protocol port used for health 
+        monitoring a backend member.
+        """
+        return pulumi.get(self, "monitor_port")
+
+    @monitor_port.setter
+    def monitor_port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "monitor_port", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Human-readable name for the member.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/l7_policy_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/l7_policy_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['L7PolicyV2Args', 'L7PolicyV2']
@@ -21,28 +22,28 @@
                  position: Optional[pulumi.Input[int]] = None,
                  redirect_pool_id: Optional[pulumi.Input[str]] = None,
                  redirect_url: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a L7PolicyV2 resource.
-        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\_TO\_POOL,
-               REDIRECT\_TO\_URL or REJECT.
+        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\\_TO\\_POOL,
+               REDIRECT\\_TO\\_URL or REJECT.
         :param pulumi.Input[str] listener_id: The Listener on which the L7 Policy will be associated with.
                Changing this creates a new L7 Policy.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Policy.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[str] description: Human-readable description for the L7 Policy.
         :param pulumi.Input[str] name: Human-readable name for the L7 Policy. Does not have
                to be unique.
         :param pulumi.Input[int] position: The position of this policy on the listener. Positions start at 1.
         :param pulumi.Input[str] redirect_pool_id: Requests matching this policy will be redirected to the
-               pool with this ID. Only valid if action is REDIRECT\_TO\_POOL.
+               pool with this ID. Only valid if action is REDIRECT\\_TO\\_POOL.
         :param pulumi.Input[str] redirect_url: Requests matching this policy will be redirected to this URL.
-               Only valid if action is REDIRECT\_TO\_URL.
+               Only valid if action is REDIRECT\\_TO\\_URL.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create an . If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                L7 Policy.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
                the L7 Policy.  Only administrative users can specify a tenant UUID
                other than their own. Changing this creates a new L7 Policy.
@@ -66,16 +67,16 @@
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter
     def action(self) -> pulumi.Input[str]:
         """
-        The L7 Policy action - can either be REDIRECT\_TO\_POOL,
-        REDIRECT\_TO\_URL or REJECT.
+        The L7 Policy action - can either be REDIRECT\\_TO\\_POOL,
+        REDIRECT\\_TO\\_URL or REJECT.
         """
         return pulumi.get(self, "action")
 
     @action.setter
     def action(self, value: pulumi.Input[str]):
         pulumi.set(self, "action", value)
 
@@ -143,28 +144,28 @@
         pulumi.set(self, "position", value)
 
     @property
     @pulumi.getter(name="redirectPoolId")
     def redirect_pool_id(self) -> Optional[pulumi.Input[str]]:
         """
         Requests matching this policy will be redirected to the
-        pool with this ID. Only valid if action is REDIRECT\_TO\_POOL.
+        pool with this ID. Only valid if action is REDIRECT\\_TO\\_POOL.
         """
         return pulumi.get(self, "redirect_pool_id")
 
     @redirect_pool_id.setter
     def redirect_pool_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "redirect_pool_id", value)
 
     @property
     @pulumi.getter(name="redirectUrl")
     def redirect_url(self) -> Optional[pulumi.Input[str]]:
         """
         Requests matching this policy will be redirected to this URL.
-        Only valid if action is REDIRECT\_TO\_URL.
+        Only valid if action is REDIRECT\\_TO\\_URL.
         """
         return pulumi.get(self, "redirect_url")
 
     @redirect_url.setter
     def redirect_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "redirect_url", value)
 
@@ -209,28 +210,28 @@
                  position: Optional[pulumi.Input[int]] = None,
                  redirect_pool_id: Optional[pulumi.Input[str]] = None,
                  redirect_url: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering L7PolicyV2 resources.
-        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\_TO\_POOL,
-               REDIRECT\_TO\_URL or REJECT.
+        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\\_TO\\_POOL,
+               REDIRECT\\_TO\\_URL or REJECT.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Policy.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[str] description: Human-readable description for the L7 Policy.
         :param pulumi.Input[str] listener_id: The Listener on which the L7 Policy will be associated with.
                Changing this creates a new L7 Policy.
         :param pulumi.Input[str] name: Human-readable name for the L7 Policy. Does not have
                to be unique.
         :param pulumi.Input[int] position: The position of this policy on the listener. Positions start at 1.
         :param pulumi.Input[str] redirect_pool_id: Requests matching this policy will be redirected to the
-               pool with this ID. Only valid if action is REDIRECT\_TO\_POOL.
+               pool with this ID. Only valid if action is REDIRECT\\_TO\\_POOL.
         :param pulumi.Input[str] redirect_url: Requests matching this policy will be redirected to this URL.
-               Only valid if action is REDIRECT\_TO\_URL.
+               Only valid if action is REDIRECT\\_TO\\_URL.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create an . If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                L7 Policy.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
                the L7 Policy.  Only administrative users can specify a tenant UUID
                other than their own. Changing this creates a new L7 Policy.
@@ -256,16 +257,16 @@
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter
     def action(self) -> Optional[pulumi.Input[str]]:
         """
-        The L7 Policy action - can either be REDIRECT\_TO\_POOL,
-        REDIRECT\_TO\_URL or REJECT.
+        The L7 Policy action - can either be REDIRECT\\_TO\\_POOL,
+        REDIRECT\\_TO\\_URL or REJECT.
         """
         return pulumi.get(self, "action")
 
     @action.setter
     def action(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "action", value)
 
@@ -333,28 +334,28 @@
         pulumi.set(self, "position", value)
 
     @property
     @pulumi.getter(name="redirectPoolId")
     def redirect_pool_id(self) -> Optional[pulumi.Input[str]]:
         """
         Requests matching this policy will be redirected to the
-        pool with this ID. Only valid if action is REDIRECT\_TO\_POOL.
+        pool with this ID. Only valid if action is REDIRECT\\_TO\\_POOL.
         """
         return pulumi.get(self, "redirect_pool_id")
 
     @redirect_pool_id.setter
     def redirect_pool_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "redirect_pool_id", value)
 
     @property
     @pulumi.getter(name="redirectUrl")
     def redirect_url(self) -> Optional[pulumi.Input[str]]:
         """
         Requests matching this policy will be redirected to this URL.
-        Only valid if action is REDIRECT\_TO\_URL.
+        Only valid if action is REDIRECT\\_TO\\_URL.
         """
         return pulumi.get(self, "redirect_url")
 
     @redirect_url.setter
     def redirect_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "redirect_url", value)
 
@@ -441,28 +442,28 @@
 
         ```sh
          $ pulumi import openstack:loadbalancer/l7PolicyV2:L7PolicyV2 l7policy_1 8a7a79c2-cf17-4e65-b2ae-ddc8bfcf6c74
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\_TO\_POOL,
-               REDIRECT\_TO\_URL or REJECT.
+        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\\_TO\\_POOL,
+               REDIRECT\\_TO\\_URL or REJECT.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Policy.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[str] description: Human-readable description for the L7 Policy.
         :param pulumi.Input[str] listener_id: The Listener on which the L7 Policy will be associated with.
                Changing this creates a new L7 Policy.
         :param pulumi.Input[str] name: Human-readable name for the L7 Policy. Does not have
                to be unique.
         :param pulumi.Input[int] position: The position of this policy on the listener. Positions start at 1.
         :param pulumi.Input[str] redirect_pool_id: Requests matching this policy will be redirected to the
-               pool with this ID. Only valid if action is REDIRECT\_TO\_POOL.
+               pool with this ID. Only valid if action is REDIRECT\\_TO\\_POOL.
         :param pulumi.Input[str] redirect_url: Requests matching this policy will be redirected to this URL.
-               Only valid if action is REDIRECT\_TO\_URL.
+               Only valid if action is REDIRECT\\_TO\\_URL.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create an . If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                L7 Policy.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
                the L7 Policy.  Only administrative users can specify a tenant UUID
                other than their own. Changing this creates a new L7 Policy.
@@ -534,20 +535,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  position: Optional[pulumi.Input[int]] = None,
                  redirect_pool_id: Optional[pulumi.Input[str]] = None,
                  redirect_url: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = L7PolicyV2Args.__new__(L7PolicyV2Args)
 
             if action is None and not opts.urn:
                 raise TypeError("Missing required property 'action'")
@@ -586,28 +584,28 @@
         """
         Get an existing L7PolicyV2 resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\_TO\_POOL,
-               REDIRECT\_TO\_URL or REJECT.
+        :param pulumi.Input[str] action: The L7 Policy action - can either be REDIRECT\\_TO\\_POOL,
+               REDIRECT\\_TO\\_URL or REJECT.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Policy.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[str] description: Human-readable description for the L7 Policy.
         :param pulumi.Input[str] listener_id: The Listener on which the L7 Policy will be associated with.
                Changing this creates a new L7 Policy.
         :param pulumi.Input[str] name: Human-readable name for the L7 Policy. Does not have
                to be unique.
         :param pulumi.Input[int] position: The position of this policy on the listener. Positions start at 1.
         :param pulumi.Input[str] redirect_pool_id: Requests matching this policy will be redirected to the
-               pool with this ID. Only valid if action is REDIRECT\_TO\_POOL.
+               pool with this ID. Only valid if action is REDIRECT\\_TO\\_POOL.
         :param pulumi.Input[str] redirect_url: Requests matching this policy will be redirected to this URL.
-               Only valid if action is REDIRECT\_TO\_URL.
+               Only valid if action is REDIRECT\\_TO\\_URL.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create an . If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                L7 Policy.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
                the L7 Policy.  Only administrative users can specify a tenant UUID
                other than their own. Changing this creates a new L7 Policy.
@@ -628,16 +626,16 @@
         __props__.__dict__["tenant_id"] = tenant_id
         return L7PolicyV2(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def action(self) -> pulumi.Output[str]:
         """
-        The L7 Policy action - can either be REDIRECT\_TO\_POOL,
-        REDIRECT\_TO\_URL or REJECT.
+        The L7 Policy action - can either be REDIRECT\\_TO\\_POOL,
+        REDIRECT\\_TO\\_URL or REJECT.
         """
         return pulumi.get(self, "action")
 
     @property
     @pulumi.getter(name="adminStateUp")
     def admin_state_up(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -681,24 +679,24 @@
         return pulumi.get(self, "position")
 
     @property
     @pulumi.getter(name="redirectPoolId")
     def redirect_pool_id(self) -> pulumi.Output[Optional[str]]:
         """
         Requests matching this policy will be redirected to the
-        pool with this ID. Only valid if action is REDIRECT\_TO\_POOL.
+        pool with this ID. Only valid if action is REDIRECT\\_TO\\_POOL.
         """
         return pulumi.get(self, "redirect_pool_id")
 
     @property
     @pulumi.getter(name="redirectUrl")
     def redirect_url(self) -> pulumi.Output[Optional[str]]:
         """
         Requests matching this policy will be redirected to this URL.
-        Only valid if action is REDIRECT\_TO\_URL.
+        Only valid if action is REDIRECT\\_TO\\_URL.
         """
         return pulumi.get(self, "redirect_url")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/l7_rule_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/l7_rule_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['L7RuleV2Args', 'L7RuleV2']
@@ -21,19 +22,19 @@
                  invert: Optional[pulumi.Input[bool]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a L7RuleV2 resource.
         :param pulumi.Input[str] compare_type: The comparison type for the L7 rule - can either be
-               CONTAINS, STARTS\_WITH, ENDS_WITH, EQUAL_TO or REGEX
+               CONTAINS, STARTS\\_WITH, ENDS_WITH, EQUAL_TO or REGEX
         :param pulumi.Input[str] l7policy_id: The ID of the L7 Policy to query. Changing this creates a new
                L7 Rule.
-        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\_TYPE, HEADER,
-               HOST\_NAME or PATH.
+        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\\_TYPE, HEADER,
+               HOST\\_NAME or PATH.
         :param pulumi.Input[str] value: The value to use for the comparison. For example, the file type to
                compare.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Rule.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[bool] invert: When true the logic of the rule is inverted. For example, with invert
                true, equal to would become not equal to. Default is false.
         :param pulumi.Input[str] key: The key to use for the comparison. For example, the name of the cookie to
@@ -62,15 +63,15 @@
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter(name="compareType")
     def compare_type(self) -> pulumi.Input[str]:
         """
         The comparison type for the L7 rule - can either be
-        CONTAINS, STARTS\_WITH, ENDS_WITH, EQUAL_TO or REGEX
+        CONTAINS, STARTS\\_WITH, ENDS_WITH, EQUAL_TO or REGEX
         """
         return pulumi.get(self, "compare_type")
 
     @compare_type.setter
     def compare_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "compare_type", value)
 
@@ -87,16 +88,16 @@
     def l7policy_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "l7policy_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The L7 Rule type - can either be COOKIE, FILE\_TYPE, HEADER,
-        HOST\_NAME or PATH.
+        The L7 Rule type - can either be COOKIE, FILE\\_TYPE, HEADER,
+        HOST\\_NAME or PATH.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -196,31 +197,31 @@
                  type: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering L7RuleV2 resources.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Rule.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[str] compare_type: The comparison type for the L7 rule - can either be
-               CONTAINS, STARTS\_WITH, ENDS_WITH, EQUAL_TO or REGEX
+               CONTAINS, STARTS\\_WITH, ENDS_WITH, EQUAL_TO or REGEX
         :param pulumi.Input[bool] invert: When true the logic of the rule is inverted. For example, with invert
                true, equal to would become not equal to. Default is false.
         :param pulumi.Input[str] key: The key to use for the comparison. For example, the name of the cookie to
                evaluate. Valid when `type` is set to COOKIE or HEADER.
         :param pulumi.Input[str] l7policy_id: The ID of the L7 Policy to query. Changing this creates a new
                L7 Rule.
         :param pulumi.Input[str] listener_id: The ID of the Listener owning this resource.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create an . If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                L7 Rule.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
                the L7 Rule.  Only administrative users can specify a tenant UUID
                other than their own. Changing this creates a new L7 Rule.
-        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\_TYPE, HEADER,
-               HOST\_NAME or PATH.
+        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\\_TYPE, HEADER,
+               HOST\\_NAME or PATH.
         :param pulumi.Input[str] value: The value to use for the comparison. For example, the file type to
                compare.
         """
         if admin_state_up is not None:
             pulumi.set(__self__, "admin_state_up", admin_state_up)
         if compare_type is not None:
             pulumi.set(__self__, "compare_type", compare_type)
@@ -255,15 +256,15 @@
         pulumi.set(self, "admin_state_up", value)
 
     @property
     @pulumi.getter(name="compareType")
     def compare_type(self) -> Optional[pulumi.Input[str]]:
         """
         The comparison type for the L7 rule - can either be
-        CONTAINS, STARTS\_WITH, ENDS_WITH, EQUAL_TO or REGEX
+        CONTAINS, STARTS\\_WITH, ENDS_WITH, EQUAL_TO or REGEX
         """
         return pulumi.get(self, "compare_type")
 
     @compare_type.setter
     def compare_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compare_type", value)
 
@@ -347,16 +348,16 @@
     def tenant_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The L7 Rule type - can either be COOKIE, FILE\_TYPE, HEADER,
-        HOST\_NAME or PATH.
+        The L7 Rule type - can either be COOKIE, FILE\\_TYPE, HEADER,
+        HOST\\_NAME or PATH.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -434,30 +435,30 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Rule.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[str] compare_type: The comparison type for the L7 rule - can either be
-               CONTAINS, STARTS\_WITH, ENDS_WITH, EQUAL_TO or REGEX
+               CONTAINS, STARTS\\_WITH, ENDS_WITH, EQUAL_TO or REGEX
         :param pulumi.Input[bool] invert: When true the logic of the rule is inverted. For example, with invert
                true, equal to would become not equal to. Default is false.
         :param pulumi.Input[str] key: The key to use for the comparison. For example, the name of the cookie to
                evaluate. Valid when `type` is set to COOKIE or HEADER.
         :param pulumi.Input[str] l7policy_id: The ID of the L7 Policy to query. Changing this creates a new
                L7 Rule.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create an . If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                L7 Rule.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
                the L7 Rule.  Only administrative users can specify a tenant UUID
                other than their own. Changing this creates a new L7 Rule.
-        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\_TYPE, HEADER,
-               HOST\_NAME or PATH.
+        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\\_TYPE, HEADER,
+               HOST\\_NAME or PATH.
         :param pulumi.Input[str] value: The value to use for the comparison. For example, the file type to
                compare.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -528,20 +529,17 @@
                  key: Optional[pulumi.Input[str]] = None,
                  l7policy_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = L7RuleV2Args.__new__(L7RuleV2Args)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             if compare_type is None and not opts.urn:
@@ -587,31 +585,31 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the L7 Rule.
                A valid value is true (UP) or false (DOWN).
         :param pulumi.Input[str] compare_type: The comparison type for the L7 rule - can either be
-               CONTAINS, STARTS\_WITH, ENDS_WITH, EQUAL_TO or REGEX
+               CONTAINS, STARTS\\_WITH, ENDS_WITH, EQUAL_TO or REGEX
         :param pulumi.Input[bool] invert: When true the logic of the rule is inverted. For example, with invert
                true, equal to would become not equal to. Default is false.
         :param pulumi.Input[str] key: The key to use for the comparison. For example, the name of the cookie to
                evaluate. Valid when `type` is set to COOKIE or HEADER.
         :param pulumi.Input[str] l7policy_id: The ID of the L7 Policy to query. Changing this creates a new
                L7 Rule.
         :param pulumi.Input[str] listener_id: The ID of the Listener owning this resource.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create an . If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                L7 Rule.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
                the L7 Rule.  Only administrative users can specify a tenant UUID
                other than their own. Changing this creates a new L7 Rule.
-        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\_TYPE, HEADER,
-               HOST\_NAME or PATH.
+        :param pulumi.Input[str] type: The L7 Rule type - can either be COOKIE, FILE\\_TYPE, HEADER,
+               HOST\\_NAME or PATH.
         :param pulumi.Input[str] value: The value to use for the comparison. For example, the file type to
                compare.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _L7RuleV2State.__new__(_L7RuleV2State)
 
@@ -637,15 +635,15 @@
         return pulumi.get(self, "admin_state_up")
 
     @property
     @pulumi.getter(name="compareType")
     def compare_type(self) -> pulumi.Output[str]:
         """
         The comparison type for the L7 rule - can either be
-        CONTAINS, STARTS\_WITH, ENDS_WITH, EQUAL_TO or REGEX
+        CONTAINS, STARTS\\_WITH, ENDS_WITH, EQUAL_TO or REGEX
         """
         return pulumi.get(self, "compare_type")
 
     @property
     @pulumi.getter
     def invert(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -701,16 +699,16 @@
         """
         return pulumi.get(self, "tenant_id")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The L7 Rule type - can either be COOKIE, FILE\_TYPE, HEADER,
-        HOST\_NAME or PATH.
+        The L7 Rule type - can either be COOKIE, FILE\\_TYPE, HEADER,
+        HOST\\_NAME or PATH.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/listener.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ListenerArgs', 'Listener']
@@ -858,20 +859,17 @@
                  sni_container_refs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  timeout_client_data: Optional[pulumi.Input[int]] = None,
                  timeout_member_connect: Optional[pulumi.Input[int]] = None,
                  timeout_member_data: Optional[pulumi.Input[int]] = None,
                  timeout_tcp_inspect: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ListenerArgs.__new__(ListenerArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["allowed_cidrs"] = allowed_cidrs
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/load_balancer.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/load_balancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['LoadBalancerArgs', 'LoadBalancer']
@@ -709,20 +710,17 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  vip_address: Optional[pulumi.Input[str]] = None,
                  vip_network_id: Optional[pulumi.Input[str]] = None,
                  vip_port_id: Optional[pulumi.Input[str]] = None,
                  vip_subnet_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = LoadBalancerArgs.__new__(LoadBalancerArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["availability_zone"] = availability_zone
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/member.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/member.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['MemberArgs', 'Member']
@@ -13,14 +14,17 @@
 @pulumi.input_type
 class MemberArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  pool_id: pulumi.Input[str],
                  protocol_port: pulumi.Input[int],
                  admin_state_up: Optional[pulumi.Input[bool]] = None,
+                 backup: Optional[pulumi.Input[bool]] = None,
+                 monitor_address: Optional[pulumi.Input[str]] = None,
+                 monitor_port: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Member resource.
@@ -28,14 +32,20 @@
                the load balancer. Changing this creates a new member.
         :param pulumi.Input[str] pool_id: The id of the pool that this member will be assigned
                to. Changing this creates a new member.
         :param pulumi.Input[int] protocol_port: The port on which to listen for client traffic.
                Changing this creates a new member.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the member.
                A valid value is true (UP) or false (DOWN). Defaults to true.
+        :param pulumi.Input[bool] backup: Boolean that indicates whether that member works as a backup or not. Available 
+               only for Octavia >= 2.1.
+        :param pulumi.Input[str] monitor_address: An alternate IP address used for health monitoring a backend member.
+               Available only for Octavia
+        :param pulumi.Input[int] monitor_port: An alternate protocol port used for health monitoring a backend member.
+               Available only for Octavia
         :param pulumi.Input[str] name: Human-readable name for the member.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create a member. If omitted, the `region`
                argument of the provider is used. Changing this creates a new member.
         :param pulumi.Input[str] subnet_id: The subnet in which to access the member. Changing
                this creates a new member.
         :param pulumi.Input[str] tenant_id: Required for admins. The UUID of the tenant who owns
@@ -47,14 +57,20 @@
                as a member with a weight of 2. Defaults to 1.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "pool_id", pool_id)
         pulumi.set(__self__, "protocol_port", protocol_port)
         if admin_state_up is not None:
             pulumi.set(__self__, "admin_state_up", admin_state_up)
+        if backup is not None:
+            pulumi.set(__self__, "backup", backup)
+        if monitor_address is not None:
+            pulumi.set(__self__, "monitor_address", monitor_address)
+        if monitor_port is not None:
+            pulumi.set(__self__, "monitor_port", monitor_port)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if subnet_id is not None:
             pulumi.set(__self__, "subnet_id", subnet_id)
         if tenant_id is not None:
@@ -112,14 +128,53 @@
 
     @admin_state_up.setter
     def admin_state_up(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "admin_state_up", value)
 
     @property
     @pulumi.getter
+    def backup(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Boolean that indicates whether that member works as a backup or not. Available 
+        only for Octavia >= 2.1.
+        """
+        return pulumi.get(self, "backup")
+
+    @backup.setter
+    def backup(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "backup", value)
+
+    @property
+    @pulumi.getter(name="monitorAddress")
+    def monitor_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        An alternate IP address used for health monitoring a backend member.
+        Available only for Octavia
+        """
+        return pulumi.get(self, "monitor_address")
+
+    @monitor_address.setter
+    def monitor_address(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "monitor_address", value)
+
+    @property
+    @pulumi.getter(name="monitorPort")
+    def monitor_port(self) -> Optional[pulumi.Input[int]]:
+        """
+        An alternate protocol port used for health monitoring a backend member.
+        Available only for Octavia
+        """
+        return pulumi.get(self, "monitor_port")
+
+    @monitor_port.setter
+    def monitor_port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "monitor_port", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Human-readable name for the member.
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -184,27 +239,36 @@
 
 
 @pulumi.input_type
 class _MemberState:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  admin_state_up: Optional[pulumi.Input[bool]] = None,
+                 backup: Optional[pulumi.Input[bool]] = None,
+                 monitor_address: Optional[pulumi.Input[str]] = None,
+                 monitor_port: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  protocol_port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Member resources.
         :param pulumi.Input[str] address: The IP address of the member to receive traffic from
                the load balancer. Changing this creates a new member.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the member.
                A valid value is true (UP) or false (DOWN). Defaults to true.
+        :param pulumi.Input[bool] backup: Boolean that indicates whether that member works as a backup or not. Available 
+               only for Octavia >= 2.1.
+        :param pulumi.Input[str] monitor_address: An alternate IP address used for health monitoring a backend member.
+               Available only for Octavia
+        :param pulumi.Input[int] monitor_port: An alternate protocol port used for health monitoring a backend member.
+               Available only for Octavia
         :param pulumi.Input[str] name: Human-readable name for the member.
         :param pulumi.Input[str] pool_id: The id of the pool that this member will be assigned
                to. Changing this creates a new member.
         :param pulumi.Input[int] protocol_port: The port on which to listen for client traffic.
                Changing this creates a new member.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create a member. If omitted, the `region`
@@ -219,14 +283,20 @@
                example, a member with a weight of 10 receives five times as much traffic
                as a member with a weight of 2. Defaults to 1.
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if admin_state_up is not None:
             pulumi.set(__self__, "admin_state_up", admin_state_up)
+        if backup is not None:
+            pulumi.set(__self__, "backup", backup)
+        if monitor_address is not None:
+            pulumi.set(__self__, "monitor_address", monitor_address)
+        if monitor_port is not None:
+            pulumi.set(__self__, "monitor_port", monitor_port)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if pool_id is not None:
             pulumi.set(__self__, "pool_id", pool_id)
         if protocol_port is not None:
             pulumi.set(__self__, "protocol_port", protocol_port)
         if region is not None:
@@ -262,14 +332,53 @@
 
     @admin_state_up.setter
     def admin_state_up(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "admin_state_up", value)
 
     @property
     @pulumi.getter
+    def backup(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Boolean that indicates whether that member works as a backup or not. Available 
+        only for Octavia >= 2.1.
+        """
+        return pulumi.get(self, "backup")
+
+    @backup.setter
+    def backup(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "backup", value)
+
+    @property
+    @pulumi.getter(name="monitorAddress")
+    def monitor_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        An alternate IP address used for health monitoring a backend member.
+        Available only for Octavia
+        """
+        return pulumi.get(self, "monitor_address")
+
+    @monitor_address.setter
+    def monitor_address(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "monitor_address", value)
+
+    @property
+    @pulumi.getter(name="monitorPort")
+    def monitor_port(self) -> Optional[pulumi.Input[int]]:
+        """
+        An alternate protocol port used for health monitoring a backend member.
+        Available only for Octavia
+        """
+        return pulumi.get(self, "monitor_port")
+
+    @monitor_port.setter
+    def monitor_port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "monitor_port", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Human-readable name for the member.
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -362,14 +471,17 @@
 class Member(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  address: Optional[pulumi.Input[str]] = None,
                  admin_state_up: Optional[pulumi.Input[bool]] = None,
+                 backup: Optional[pulumi.Input[bool]] = None,
+                 monitor_address: Optional[pulumi.Input[str]] = None,
+                 monitor_port: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  protocol_port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
@@ -399,14 +511,20 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: The IP address of the member to receive traffic from
                the load balancer. Changing this creates a new member.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the member.
                A valid value is true (UP) or false (DOWN). Defaults to true.
+        :param pulumi.Input[bool] backup: Boolean that indicates whether that member works as a backup or not. Available 
+               only for Octavia >= 2.1.
+        :param pulumi.Input[str] monitor_address: An alternate IP address used for health monitoring a backend member.
+               Available only for Octavia
+        :param pulumi.Input[int] monitor_port: An alternate protocol port used for health monitoring a backend member.
+               Available only for Octavia
         :param pulumi.Input[str] name: Human-readable name for the member.
         :param pulumi.Input[str] pool_id: The id of the pool that this member will be assigned
                to. Changing this creates a new member.
         :param pulumi.Input[int] protocol_port: The port on which to listen for client traffic.
                Changing this creates a new member.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create a member. If omitted, the `region`
@@ -463,37 +581,40 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  address: Optional[pulumi.Input[str]] = None,
                  admin_state_up: Optional[pulumi.Input[bool]] = None,
+                 backup: Optional[pulumi.Input[bool]] = None,
+                 monitor_address: Optional[pulumi.Input[str]] = None,
+                 monitor_port: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  protocol_port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MemberArgs.__new__(MemberArgs)
 
             if address is None and not opts.urn:
                 raise TypeError("Missing required property 'address'")
             __props__.__dict__["address"] = address
             __props__.__dict__["admin_state_up"] = admin_state_up
+            __props__.__dict__["backup"] = backup
+            __props__.__dict__["monitor_address"] = monitor_address
+            __props__.__dict__["monitor_port"] = monitor_port
             __props__.__dict__["name"] = name
             if pool_id is None and not opts.urn:
                 raise TypeError("Missing required property 'pool_id'")
             __props__.__dict__["pool_id"] = pool_id
             if protocol_port is None and not opts.urn:
                 raise TypeError("Missing required property 'protocol_port'")
             __props__.__dict__["protocol_port"] = protocol_port
@@ -509,14 +630,17 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             address: Optional[pulumi.Input[str]] = None,
             admin_state_up: Optional[pulumi.Input[bool]] = None,
+            backup: Optional[pulumi.Input[bool]] = None,
+            monitor_address: Optional[pulumi.Input[str]] = None,
+            monitor_port: Optional[pulumi.Input[int]] = None,
             name: Optional[pulumi.Input[str]] = None,
             pool_id: Optional[pulumi.Input[str]] = None,
             protocol_port: Optional[pulumi.Input[int]] = None,
             region: Optional[pulumi.Input[str]] = None,
             subnet_id: Optional[pulumi.Input[str]] = None,
             tenant_id: Optional[pulumi.Input[str]] = None,
             weight: Optional[pulumi.Input[int]] = None) -> 'Member':
@@ -527,14 +651,20 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: The IP address of the member to receive traffic from
                the load balancer. Changing this creates a new member.
         :param pulumi.Input[bool] admin_state_up: The administrative state of the member.
                A valid value is true (UP) or false (DOWN). Defaults to true.
+        :param pulumi.Input[bool] backup: Boolean that indicates whether that member works as a backup or not. Available 
+               only for Octavia >= 2.1.
+        :param pulumi.Input[str] monitor_address: An alternate IP address used for health monitoring a backend member.
+               Available only for Octavia
+        :param pulumi.Input[int] monitor_port: An alternate protocol port used for health monitoring a backend member.
+               Available only for Octavia
         :param pulumi.Input[str] name: Human-readable name for the member.
         :param pulumi.Input[str] pool_id: The id of the pool that this member will be assigned
                to. Changing this creates a new member.
         :param pulumi.Input[int] protocol_port: The port on which to listen for client traffic.
                Changing this creates a new member.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Networking client.
                A Networking client is needed to create a member. If omitted, the `region`
@@ -551,14 +681,17 @@
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MemberState.__new__(_MemberState)
 
         __props__.__dict__["address"] = address
         __props__.__dict__["admin_state_up"] = admin_state_up
+        __props__.__dict__["backup"] = backup
+        __props__.__dict__["monitor_address"] = monitor_address
+        __props__.__dict__["monitor_port"] = monitor_port
         __props__.__dict__["name"] = name
         __props__.__dict__["pool_id"] = pool_id
         __props__.__dict__["protocol_port"] = protocol_port
         __props__.__dict__["region"] = region
         __props__.__dict__["subnet_id"] = subnet_id
         __props__.__dict__["tenant_id"] = tenant_id
         __props__.__dict__["weight"] = weight
@@ -580,14 +713,41 @@
         The administrative state of the member.
         A valid value is true (UP) or false (DOWN). Defaults to true.
         """
         return pulumi.get(self, "admin_state_up")
 
     @property
     @pulumi.getter
+    def backup(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Boolean that indicates whether that member works as a backup or not. Available 
+        only for Octavia >= 2.1.
+        """
+        return pulumi.get(self, "backup")
+
+    @property
+    @pulumi.getter(name="monitorAddress")
+    def monitor_address(self) -> pulumi.Output[Optional[str]]:
+        """
+        An alternate IP address used for health monitoring a backend member.
+        Available only for Octavia
+        """
+        return pulumi.get(self, "monitor_address")
+
+    @property
+    @pulumi.getter(name="monitorPort")
+    def monitor_port(self) -> pulumi.Output[Optional[int]]:
+        """
+        An alternate protocol port used for health monitoring a backend member.
+        Available only for Octavia
+        """
+        return pulumi.get(self, "monitor_port")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         Human-readable name for the member.
         """
         return pulumi.get(self, "name")
 
     @property
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/member_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/member_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['MemberV1Args', 'MemberV1']
@@ -377,20 +378,17 @@
                  admin_state_up: Optional[pulumi.Input[bool]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MemberV1Args.__new__(MemberV1Args)
 
             if address is None and not opts.urn:
                 raise TypeError("Missing required property 'address'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/members.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/members.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -260,20 +261,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  members: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MembersMemberArgs']]]]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MembersArgs.__new__(MembersArgs)
 
             __props__.__dict__["members"] = members
             if pool_id is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/monitor.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['MonitorArgs', 'Monitor']
@@ -660,20 +661,17 @@
                  pool_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  url_path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MonitorArgs.__new__(MonitorArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             if delay is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/monitor_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/monitor_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['MonitorV1Args', 'MonitorV1']
@@ -549,20 +550,17 @@
                  max_retries: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  url_path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MonitorV1Args.__new__(MonitorV1Args)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             if delay is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/outputs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -18,14 +19,18 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "protocolPort":
             suggest = "protocol_port"
         elif key == "adminStateUp":
             suggest = "admin_state_up"
+        elif key == "monitorAddress":
+            suggest = "monitor_address"
+        elif key == "monitorPort":
+            suggest = "monitor_port"
         elif key == "subnetId":
             suggest = "subnet_id"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in MembersMember. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -38,26 +43,32 @@
 
     def __init__(__self__, *,
                  address: str,
                  protocol_port: int,
                  admin_state_up: Optional[bool] = None,
                  backup: Optional[bool] = None,
                  id: Optional[str] = None,
+                 monitor_address: Optional[str] = None,
+                 monitor_port: Optional[int] = None,
                  name: Optional[str] = None,
                  subnet_id: Optional[str] = None,
                  weight: Optional[int] = None):
         """
         :param str address: The IP address of the members to receive traffic from
                the load balancer.
         :param int protocol_port: The port on which to listen for client traffic.
         :param bool admin_state_up: The administrative state of the member.
                A valid value is true (UP) or false (DOWN). Defaults to true.
         :param bool backup: A bool that indicates whether the member is
                backup. **Requires octavia minor version 2.1 or later**.
         :param str id: The unique ID for the members.
+        :param str monitor_address: An alternate IP address used for health 
+               monitoring a backend member.
+        :param int monitor_port: An alternate protocol port used for health 
+               monitoring a backend member.
         :param str name: Human-readable name for the member.
         :param str subnet_id: The subnet in which to access the member.
         :param int weight: A positive integer value that indicates the relative
                portion of traffic that this members should receive from the pool. For
                example, a member with a weight of 10 receives five times as much traffic
                as a member with a weight of 2. Defaults to 1.
         """
@@ -65,14 +76,18 @@
         pulumi.set(__self__, "protocol_port", protocol_port)
         if admin_state_up is not None:
             pulumi.set(__self__, "admin_state_up", admin_state_up)
         if backup is not None:
             pulumi.set(__self__, "backup", backup)
         if id is not None:
             pulumi.set(__self__, "id", id)
+        if monitor_address is not None:
+            pulumi.set(__self__, "monitor_address", monitor_address)
+        if monitor_port is not None:
+            pulumi.set(__self__, "monitor_port", monitor_port)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if subnet_id is not None:
             pulumi.set(__self__, "subnet_id", subnet_id)
         if weight is not None:
             pulumi.set(__self__, "weight", weight)
 
@@ -116,14 +131,32 @@
     def id(self) -> Optional[str]:
         """
         The unique ID for the members.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="monitorAddress")
+    def monitor_address(self) -> Optional[str]:
+        """
+        An alternate IP address used for health 
+        monitoring a backend member.
+        """
+        return pulumi.get(self, "monitor_address")
+
+    @property
+    @pulumi.getter(name="monitorPort")
+    def monitor_port(self) -> Optional[int]:
+        """
+        An alternate protocol port used for health 
+        monitoring a backend member.
+        """
+        return pulumi.get(self, "monitor_port")
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Human-readable name for the member.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/pool.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -548,20 +549,17 @@
                  loadbalancer_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  persistence: Optional[pulumi.Input[pulumi.InputType['PoolPersistenceArgs']]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PoolArgs.__new__(PoolArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/pool_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/pool_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PoolV1Args', 'PoolV1']
@@ -640,20 +641,17 @@
                  monitor_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PoolV1Args.__new__(PoolV1Args)
 
             if lb_method is None and not opts.urn:
                 raise TypeError("Missing required property 'lb_method'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/quota.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QuotaArgs', 'Quota']
@@ -506,20 +507,17 @@
                  listener: Optional[pulumi.Input[int]] = None,
                  loadbalancer: Optional[pulumi.Input[int]] = None,
                  member: Optional[pulumi.Input[int]] = None,
                  pool: Optional[pulumi.Input[int]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QuotaArgs.__new__(QuotaArgs)
 
             __props__.__dict__["health_monitor"] = health_monitor
             __props__.__dict__["l7_policy"] = l7_policy
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/loadbalancer/vip.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/loadbalancer/vip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['VipArgs', 'Vip']
@@ -668,20 +669,17 @@
                  pool_id: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VipArgs.__new__(VipArgs)
 
             __props__.__dict__["address"] = address
             __props__.__dict__["admin_state_up"] = admin_state_up
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/__init__.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/address_scope.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/address_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['AddressScopeArgs', 'AddressScope']
@@ -343,20 +344,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  ip_version: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  shared: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AddressScopeArgs.__new__(AddressScopeArgs)
 
             __props__.__dict__["ip_version"] = ip_version
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/floating_ip.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/floating_ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['FloatingIpArgs', 'FloatingIp']
@@ -658,20 +659,17 @@
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FloatingIpArgs.__new__(FloatingIpArgs)
 
             __props__.__dict__["address"] = address
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/floating_ip_associate.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/floating_ip_associate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['FloatingIpAssociateArgs', 'FloatingIpAssociate']
@@ -257,20 +258,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  fixed_ip: Optional[pulumi.Input[str]] = None,
                  floating_ip: Optional[pulumi.Input[str]] = None,
                  port_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FloatingIpAssociateArgs.__new__(FloatingIpAssociateArgs)
 
             __props__.__dict__["fixed_ip"] = fixed_ip
             if floating_ip is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_address_scope.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_address_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -132,18 +133,15 @@
     """
     __args__ = dict()
     __args__['ipVersion'] = ip_version
     __args__['name'] = name
     __args__['projectId'] = project_id
     __args__['region'] = region
     __args__['shared'] = shared
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getAddressScope:getAddressScope', __args__, opts=opts, typ=GetAddressScopeResult).value
 
     return AwaitableGetAddressScopeResult(
         id=__ret__.id,
         ip_version=__ret__.ip_version,
         name=__ret__.name,
         project_id=__ret__.project_id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_floating_ip.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_floating_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -203,18 +204,15 @@
     __args__['fixedIp'] = fixed_ip
     __args__['pool'] = pool
     __args__['portId'] = port_id
     __args__['region'] = region
     __args__['status'] = status
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getFloatingIp:getFloatingIp', __args__, opts=opts, typ=GetFloatingIpResult).value
 
     return AwaitableGetFloatingIpResult(
         address=__ret__.address,
         all_tags=__ret__.all_tags,
         description=__ret__.description,
         dns_domain=__ret__.dns_domain,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_network.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -283,18 +284,15 @@
     __args__['name'] = name
     __args__['networkId'] = network_id
     __args__['region'] = region
     __args__['status'] = status
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
     __args__['transparentVlan'] = transparent_vlan
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getNetwork:getNetwork', __args__, opts=opts, typ=GetNetworkResult).value
 
     return AwaitableGetNetworkResult(
         admin_state_up=__ret__.admin_state_up,
         all_tags=__ret__.all_tags,
         availability_zone_hints=__ret__.availability_zone_hints,
         description=__ret__.description,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_port.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -371,18 +372,15 @@
     __args__['portId'] = port_id
     __args__['projectId'] = project_id
     __args__['region'] = region
     __args__['securityGroupIds'] = security_group_ids
     __args__['status'] = status
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getPort:getPort', __args__, opts=opts, typ=GetPortResult).value
 
     return AwaitableGetPortResult(
         admin_state_up=__ret__.admin_state_up,
         all_fixed_ips=__ret__.all_fixed_ips,
         all_security_group_ids=__ret__.all_security_group_ids,
         all_tags=__ret__.all_tags,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_port_ids.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_port_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -270,18 +271,15 @@
     __args__['region'] = region
     __args__['securityGroupIds'] = security_group_ids
     __args__['sortDirection'] = sort_direction
     __args__['sortKey'] = sort_key
     __args__['status'] = status
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getPortIds:getPortIds', __args__, opts=opts, typ=GetPortIdsResult).value
 
     return AwaitableGetPortIdsResult(
         admin_state_up=__ret__.admin_state_up,
         description=__ret__.description,
         device_id=__ret__.device_id,
         device_owner=__ret__.device_owner,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -129,18 +130,15 @@
            `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['maxBurstKbps'] = max_burst_kbps
     __args__['maxKbps'] = max_kbps
     __args__['qosPolicyId'] = qos_policy_id
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getQosBandwidthLimitRule:getQosBandwidthLimitRule', __args__, opts=opts, typ=GetQosBandwidthLimitRuleResult).value
 
     return AwaitableGetQosBandwidthLimitRuleResult(
         direction=__ret__.direction,
         id=__ret__.id,
         max_burst_kbps=__ret__.max_burst_kbps,
         max_kbps=__ret__.max_kbps,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_dscp_marking_rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_dscp_marking_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -102,18 +103,15 @@
            A Networking client is needed to create a Neutron QoS DSCP marking rule. If omitted, the
            `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['dscpMark'] = dscp_mark
     __args__['qosPolicyId'] = qos_policy_id
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getQosDscpMarkingRule:getQosDscpMarkingRule', __args__, opts=opts, typ=GetQosDscpMarkingRuleResult).value
 
     return AwaitableGetQosDscpMarkingRuleResult(
         dscp_mark=__ret__.dscp_mark,
         id=__ret__.id,
         qos_policy_id=__ret__.qos_policy_id,
         region=__ret__.region)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -113,18 +114,15 @@
            `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['direction'] = direction
     __args__['minKbps'] = min_kbps
     __args__['qosPolicyId'] = qos_policy_id
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getQosMinimumBandwidthRule:getQosMinimumBandwidthRule', __args__, opts=opts, typ=GetQosMinimumBandwidthRuleResult).value
 
     return AwaitableGetQosMinimumBandwidthRuleResult(
         direction=__ret__.direction,
         id=__ret__.id,
         min_kbps=__ret__.min_kbps,
         qos_policy_id=__ret__.qos_policy_id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_qos_policy.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_qos_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -204,18 +205,15 @@
     __args__['description'] = description
     __args__['isDefault'] = is_default
     __args__['name'] = name
     __args__['projectId'] = project_id
     __args__['region'] = region
     __args__['shared'] = shared
     __args__['tags'] = tags
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getQosPolicy:getQosPolicy', __args__, opts=opts, typ=GetQosPolicyResult).value
 
     return AwaitableGetQosPolicyResult(
         all_tags=__ret__.all_tags,
         created_at=__ret__.created_at,
         description=__ret__.description,
         id=__ret__.id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_quota_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_quota_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -170,14 +171,15 @@
             security_group=self.security_group,
             security_group_rule=self.security_group_rule,
             subnet=self.subnet,
             subnetpool=self.subnetpool)
 
 
 def get_quota_v2(project_id: Optional[str] = None,
+                 region: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetQuotaV2Result:
     """
     Use this data source to get the networking quota of an OpenStack project.
 
     ## Example Usage
 
     ```python
@@ -185,21 +187,21 @@
     import pulumi_openstack as openstack
 
     quota = openstack.networking.get_quota_v2(project_id="2e367a3d29f94fd988e6ec54e305ec9d")
     ```
 
 
     :param str project_id: The id of the project to retrieve the quota.
+    :param str region: The region in which to obtain the V2 Network client.
+           If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['projectId'] = project_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    __args__['region'] = region
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getQuotaV2:getQuotaV2', __args__, opts=opts, typ=GetQuotaV2Result).value
 
     return AwaitableGetQuotaV2Result(
         floatingip=__ret__.floatingip,
         id=__ret__.id,
         network=__ret__.network,
         port=__ret__.port,
@@ -211,14 +213,15 @@
         security_group_rule=__ret__.security_group_rule,
         subnet=__ret__.subnet,
         subnetpool=__ret__.subnetpool)
 
 
 @_utilities.lift_output_func(get_quota_v2)
 def get_quota_v2_output(project_id: Optional[pulumi.Input[str]] = None,
+                        region: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetQuotaV2Result]:
     """
     Use this data source to get the networking quota of an OpenStack project.
 
     ## Example Usage
 
     ```python
@@ -226,9 +229,11 @@
     import pulumi_openstack as openstack
 
     quota = openstack.networking.get_quota_v2(project_id="2e367a3d29f94fd988e6ec54e305ec9d")
     ```
 
 
     :param str project_id: The id of the project to retrieve the quota.
+    :param str region: The region in which to obtain the V2 Network client.
+           If omitted, the `region` argument of the provider is used.
     """
     ...
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_router.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -229,18 +230,15 @@
     __args__['enableSnat'] = enable_snat
     __args__['name'] = name
     __args__['region'] = region
     __args__['routerId'] = router_id
     __args__['status'] = status
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getRouter:getRouter', __args__, opts=opts, typ=GetRouterResult).value
 
     return AwaitableGetRouterResult(
         admin_state_up=__ret__.admin_state_up,
         all_tags=__ret__.all_tags,
         availability_zone_hints=__ret__.availability_zone_hints,
         description=__ret__.description,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_sec_group.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_sec_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -148,18 +149,15 @@
     __args__ = dict()
     __args__['description'] = description
     __args__['name'] = name
     __args__['region'] = region
     __args__['secgroupId'] = secgroup_id
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getSecGroup:getSecGroup', __args__, opts=opts, typ=GetSecGroupResult).value
 
     return AwaitableGetSecGroupResult(
         all_tags=__ret__.all_tags,
         description=__ret__.description,
         id=__ret__.id,
         name=__ret__.name,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_subnet.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_subnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -306,18 +307,15 @@
     __args__['name'] = name
     __args__['networkId'] = network_id
     __args__['region'] = region
     __args__['subnetId'] = subnet_id
     __args__['subnetpoolId'] = subnetpool_id
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getSubnet:getSubnet', __args__, opts=opts, typ=GetSubnetResult).value
 
     return AwaitableGetSubnetResult(
         all_tags=__ret__.all_tags,
         allocation_pools=__ret__.allocation_pools,
         cidr=__ret__.cidr,
         description=__ret__.description,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_subnet_ids_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_subnet_ids_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -262,18 +263,15 @@
     __args__['networkId'] = network_id
     __args__['region'] = region
     __args__['sortDirection'] = sort_direction
     __args__['sortKey'] = sort_key
     __args__['subnetpoolId'] = subnetpool_id
     __args__['tags'] = tags
     __args__['tenantId'] = tenant_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getSubnetIdsV2:getSubnetIdsV2', __args__, opts=opts, typ=GetSubnetIdsV2Result).value
 
     return AwaitableGetSubnetIdsV2Result(
         cidr=__ret__.cidr,
         description=__ret__.description,
         dhcp_enabled=__ret__.dhcp_enabled,
         gateway_ip=__ret__.gateway_ip,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_subnet_pool.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_subnet_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -310,18 +311,15 @@
     __args__['maxPrefixlen'] = max_prefixlen
     __args__['minPrefixlen'] = min_prefixlen
     __args__['name'] = name
     __args__['projectId'] = project_id
     __args__['region'] = region
     __args__['shared'] = shared
     __args__['tags'] = tags
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getSubnetPool:getSubnetPool', __args__, opts=opts, typ=GetSubnetPoolResult).value
 
     return AwaitableGetSubnetPoolResult(
         address_scope_id=__ret__.address_scope_id,
         all_tags=__ret__.all_tags,
         created_at=__ret__.created_at,
         default_prefixlen=__ret__.default_prefixlen,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/get_trunk.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/get_trunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -194,18 +195,15 @@
     __args__['name'] = name
     __args__['portId'] = port_id
     __args__['projectId'] = project_id
     __args__['region'] = region
     __args__['status'] = status
     __args__['tags'] = tags
     __args__['trunkId'] = trunk_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:networking/getTrunk:getTrunk', __args__, opts=opts, typ=GetTrunkResult).value
 
     return AwaitableGetTrunkResult(
         admin_state_up=__ret__.admin_state_up,
         all_tags=__ret__.all_tags,
         description=__ret__.description,
         id=__ret__.id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/network.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -858,20 +859,17 @@
                  segments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkSegmentArgs']]]]] = None,
                  shared: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  transparent_vlan: Optional[pulumi.Input[bool]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetworkArgs.__new__(NetworkArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["availability_zone_hints"] = availability_zone_hints
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/port.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/port.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -1144,20 +1145,17 @@
                  qos_policy_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PortArgs.__new__(PortArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["allowed_address_pairs"] = allowed_address_pairs
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/port_forwarding_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/port_forwarding_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PortForwardingV2Args', 'PortForwardingV2']
@@ -408,20 +409,17 @@
                  floatingip_id: Optional[pulumi.Input[str]] = None,
                  internal_ip_address: Optional[pulumi.Input[str]] = None,
                  internal_port: Optional[pulumi.Input[int]] = None,
                  internal_port_id: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PortForwardingV2Args.__new__(PortForwardingV2Args)
 
             __props__.__dict__["description"] = description
             if external_port is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/port_sec_group_associate.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/port_sec_group_associate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PortSecGroupAssociateArgs', 'PortSecGroupAssociate']
@@ -240,14 +241,22 @@
         system_port = openstack.networking.get_port(fixed_ip="10.0.0.10")
         port1 = openstack.networking.PortSecGroupAssociate("port1",
             enforce=True,
             port_id=system_port.id,
             security_group_ids=[])
         ```
 
+        ## Import
+
+        Port security group association can be imported using the `id` of the port, e.g.
+
+        ```sh
+         $ pulumi import openstack:networking/portSecGroupAssociate:PortSecGroupAssociate port_1 eae26a3e-1c33-4cc1-9c31-0cd729c438a1
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enforce: Whether to replace or append the list of security
                groups, specified in the `security_group_ids`. Defaults to `false`.
         :param pulumi.Input[str] port_id: An UUID of the port to apply security groups to.
         :param pulumi.Input[str] region: The region in which to obtain the V2 networking client.
                A networking client is needed to manage a port. If omitted, the
@@ -299,14 +308,22 @@
         system_port = openstack.networking.get_port(fixed_ip="10.0.0.10")
         port1 = openstack.networking.PortSecGroupAssociate("port1",
             enforce=True,
             port_id=system_port.id,
             security_group_ids=[])
         ```
 
+        ## Import
+
+        Port security group association can be imported using the `id` of the port, e.g.
+
+        ```sh
+         $ pulumi import openstack:networking/portSecGroupAssociate:PortSecGroupAssociate port_1 eae26a3e-1c33-4cc1-9c31-0cd729c438a1
+        ```
+
         :param str resource_name: The name of the resource.
         :param PortSecGroupAssociateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(PortSecGroupAssociateArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -319,20 +336,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enforce: Optional[pulumi.Input[bool]] = None,
                  port_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PortSecGroupAssociateArgs.__new__(PortSecGroupAssociateArgs)
 
             __props__.__dict__["enforce"] = enforce
             if port_id is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_bandwidth_limit_rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_bandwidth_limit_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QosBandwidthLimitRuleArgs', 'QosBandwidthLimitRule']
@@ -303,20 +304,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  direction: Optional[pulumi.Input[str]] = None,
                  max_burst_kbps: Optional[pulumi.Input[int]] = None,
                  max_kbps: Optional[pulumi.Input[int]] = None,
                  qos_policy_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QosBandwidthLimitRuleArgs.__new__(QosBandwidthLimitRuleArgs)
 
             __props__.__dict__["direction"] = direction
             __props__.__dict__["max_burst_kbps"] = max_burst_kbps
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_dscp_marking_rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_dscp_marking_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QosDscpMarkingRuleArgs', 'QosDscpMarkingRule']
@@ -219,20 +220,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  dscp_mark: Optional[pulumi.Input[int]] = None,
                  qos_policy_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QosDscpMarkingRuleArgs.__new__(QosDscpMarkingRuleArgs)
 
             if dscp_mark is None and not opts.urn:
                 raise TypeError("Missing required property 'dscp_mark'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QosMinimumBandwidthRuleArgs', 'QosMinimumBandwidthRule']
@@ -259,20 +260,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  direction: Optional[pulumi.Input[str]] = None,
                  min_kbps: Optional[pulumi.Input[int]] = None,
                  qos_policy_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QosMinimumBandwidthRuleArgs.__new__(QosMinimumBandwidthRuleArgs)
 
             __props__.__dict__["direction"] = direction
             if min_kbps is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/qos_policy.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/qos_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QosPolicyArgs', 'QosPolicy']
@@ -491,20 +492,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  shared: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QosPolicyArgs.__new__(QosPolicyArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["is_default"] = is_default
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/quota_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/quota_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['QuotaV2Args', 'QuotaV2']
@@ -575,20 +576,17 @@
                  region: Optional[pulumi.Input[str]] = None,
                  router: Optional[pulumi.Input[int]] = None,
                  security_group: Optional[pulumi.Input[int]] = None,
                  security_group_rule: Optional[pulumi.Input[int]] = None,
                  subnet: Optional[pulumi.Input[int]] = None,
                  subnetpool: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = QuotaV2Args.__new__(QuotaV2Args)
 
             __props__.__dict__["floatingip"] = floatingip
             __props__.__dict__["network"] = network
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/rbac_policy_v2.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/rbac_policy_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RbacPolicyV2Args', 'RbacPolicyV2']
@@ -355,20 +356,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  action: Optional[pulumi.Input[str]] = None,
                  object_id: Optional[pulumi.Input[str]] = None,
                  object_type: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  target_tenant: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RbacPolicyV2Args.__new__(RbacPolicyV2Args)
 
             if action is None and not opts.urn:
                 raise TypeError("Missing required property 'action'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/router.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -803,20 +804,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  vendor_options: Optional[pulumi.Input[pulumi.InputType['RouterVendorOptionsArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouterArgs.__new__(RouterArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["availability_zone_hints"] = availability_zone_hints
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/router_interface.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/router_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RouterInterfaceArgs', 'RouterInterface']
@@ -278,20 +279,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  port_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  router_id: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouterInterfaceArgs.__new__(RouterInterfaceArgs)
 
             __props__.__dict__["port_id"] = port_id
             __props__.__dict__["region"] = region
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/router_route.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/router_route.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RouterRouteArgs', 'RouterRoute']
@@ -296,20 +297,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  destination_cidr: Optional[pulumi.Input[str]] = None,
                  next_hop: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  router_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouterRouteArgs.__new__(RouterRouteArgs)
 
             if destination_cidr is None and not opts.urn:
                 raise TypeError("Missing required property 'destination_cidr'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/sec_group.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/sec_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SecGroupArgs', 'SecGroup']
@@ -334,20 +335,17 @@
                  delete_default_rules: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecGroupArgs.__new__(SecGroupArgs)
 
             __props__.__dict__["delete_default_rules"] = delete_default_rules
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/sec_group_rule.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/sec_group_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SecGroupRuleArgs', 'SecGroupRule']
@@ -680,20 +681,17 @@
                  protocol: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  remote_group_id: Optional[pulumi.Input[str]] = None,
                  remote_ip_prefix: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecGroupRuleArgs.__new__(SecGroupRuleArgs)
 
             __props__.__dict__["description"] = description
             if direction is None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/subnet.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/subnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -1000,20 +1001,17 @@
                  prefix_length: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnetpool_id: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SubnetArgs.__new__(SubnetArgs)
 
             __props__.__dict__["allocation_pools"] = allocation_pools
             if allocation_pools_collection is not None and not opts.urn:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/subnet_pool.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/subnet_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SubnetPoolArgs', 'SubnetPool']
@@ -851,20 +852,17 @@
                  prefixes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  shared: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SubnetPoolArgs.__new__(SubnetPoolArgs)
 
             __props__.__dict__["address_scope_id"] = address_scope_id
             __props__.__dict__["default_prefixlen"] = default_prefixlen
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/subnet_route.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/subnet_route.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SubnetRouteArgs', 'SubnetRoute']
@@ -278,20 +279,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  destination_cidr: Optional[pulumi.Input[str]] = None,
                  next_hop: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SubnetRouteArgs.__new__(SubnetRouteArgs)
 
             if destination_cidr is None and not opts.urn:
                 raise TypeError("Missing required property 'destination_cidr'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/networking/trunk.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/networking/trunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -475,20 +476,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  port_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  sub_ports: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TrunkSubPortArgs']]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TrunkArgs.__new__(TrunkArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/container.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/container.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -20,14 +21,15 @@
                  container_sync_to: Optional[pulumi.Input[str]] = None,
                  container_write: Optional[pulumi.Input[str]] = None,
                  content_type: Optional[pulumi.Input[str]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 storage_policy: Optional[pulumi.Input[str]] = None,
                  versioning: Optional[pulumi.Input['ContainerVersioningArgs']] = None):
         """
         The set of arguments for constructing a Container resource.
         :param pulumi.Input[str] container_read: Sets an access control list (ACL) that grants
                read access. This header can contain a comma-delimited list of users that
                can read the container (allows the GET method for all objects in the
                container). Changing this updates the access control list read access.
@@ -43,14 +45,16 @@
         :param pulumi.Input[Mapping[str, Any]] metadata: Custom key/value pairs to associate with the container.
                Changing this updates the existing container metadata.
         :param pulumi.Input[str] name: A unique name for the container. Changing this creates a
                new container.
         :param pulumi.Input[str] region: The region in which to create the container. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new container.
+        :param pulumi.Input[str] storage_policy: The storage policy to be used for the container. 
+               Changing this creates a new container.
         :param pulumi.Input['ContainerVersioningArgs'] versioning: Enable object versioning. The structure is described below.
         """
         if container_read is not None:
             pulumi.set(__self__, "container_read", container_read)
         if container_sync_key is not None:
             pulumi.set(__self__, "container_sync_key", container_sync_key)
         if container_sync_to is not None:
@@ -63,14 +67,16 @@
             pulumi.set(__self__, "force_destroy", force_destroy)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if storage_policy is not None:
+            pulumi.set(__self__, "storage_policy", storage_policy)
         if versioning is not None:
             pulumi.set(__self__, "versioning", versioning)
 
     @property
     @pulumi.getter(name="containerRead")
     def container_read(self) -> Optional[pulumi.Input[str]]:
         """
@@ -186,14 +192,27 @@
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="storagePolicy")
+    def storage_policy(self) -> Optional[pulumi.Input[str]]:
+        """
+        The storage policy to be used for the container. 
+        Changing this creates a new container.
+        """
+        return pulumi.get(self, "storage_policy")
+
+    @storage_policy.setter
+    def storage_policy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "storage_policy", value)
+
+    @property
     @pulumi.getter
     def versioning(self) -> Optional[pulumi.Input['ContainerVersioningArgs']]:
         """
         Enable object versioning. The structure is described below.
         """
         return pulumi.get(self, "versioning")
 
@@ -210,14 +229,15 @@
                  container_sync_to: Optional[pulumi.Input[str]] = None,
                  container_write: Optional[pulumi.Input[str]] = None,
                  content_type: Optional[pulumi.Input[str]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 storage_policy: Optional[pulumi.Input[str]] = None,
                  versioning: Optional[pulumi.Input['ContainerVersioningArgs']] = None):
         """
         Input properties used for looking up and filtering Container resources.
         :param pulumi.Input[str] container_read: Sets an access control list (ACL) that grants
                read access. This header can contain a comma-delimited list of users that
                can read the container (allows the GET method for all objects in the
                container). Changing this updates the access control list read access.
@@ -233,14 +253,16 @@
         :param pulumi.Input[Mapping[str, Any]] metadata: Custom key/value pairs to associate with the container.
                Changing this updates the existing container metadata.
         :param pulumi.Input[str] name: A unique name for the container. Changing this creates a
                new container.
         :param pulumi.Input[str] region: The region in which to create the container. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new container.
+        :param pulumi.Input[str] storage_policy: The storage policy to be used for the container. 
+               Changing this creates a new container.
         :param pulumi.Input['ContainerVersioningArgs'] versioning: Enable object versioning. The structure is described below.
         """
         if container_read is not None:
             pulumi.set(__self__, "container_read", container_read)
         if container_sync_key is not None:
             pulumi.set(__self__, "container_sync_key", container_sync_key)
         if container_sync_to is not None:
@@ -253,14 +275,16 @@
             pulumi.set(__self__, "force_destroy", force_destroy)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if storage_policy is not None:
+            pulumi.set(__self__, "storage_policy", storage_policy)
         if versioning is not None:
             pulumi.set(__self__, "versioning", versioning)
 
     @property
     @pulumi.getter(name="containerRead")
     def container_read(self) -> Optional[pulumi.Input[str]]:
         """
@@ -376,14 +400,27 @@
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="storagePolicy")
+    def storage_policy(self) -> Optional[pulumi.Input[str]]:
+        """
+        The storage policy to be used for the container. 
+        Changing this creates a new container.
+        """
+        return pulumi.get(self, "storage_policy")
+
+    @storage_policy.setter
+    def storage_policy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "storage_policy", value)
+
+    @property
     @pulumi.getter
     def versioning(self) -> Optional[pulumi.Input['ContainerVersioningArgs']]:
         """
         Enable object versioning. The structure is described below.
         """
         return pulumi.get(self, "versioning")
 
@@ -402,14 +439,15 @@
                  container_sync_to: Optional[pulumi.Input[str]] = None,
                  container_write: Optional[pulumi.Input[str]] = None,
                  content_type: Optional[pulumi.Input[str]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 storage_policy: Optional[pulumi.Input[str]] = None,
                  versioning: Optional[pulumi.Input[pulumi.InputType['ContainerVersioningArgs']]] = None,
                  __props__=None):
         """
         Manages a V1 container resource within OpenStack.
 
         ## Example Usage
         ### Basic Container
@@ -488,14 +526,16 @@
         :param pulumi.Input[Mapping[str, Any]] metadata: Custom key/value pairs to associate with the container.
                Changing this updates the existing container metadata.
         :param pulumi.Input[str] name: A unique name for the container. Changing this creates a
                new container.
         :param pulumi.Input[str] region: The region in which to create the container. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new container.
+        :param pulumi.Input[str] storage_policy: The storage policy to be used for the container. 
+               Changing this creates a new container.
         :param pulumi.Input[pulumi.InputType['ContainerVersioningArgs']] versioning: Enable object versioning. The structure is described below.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ContainerArgs] = None,
@@ -582,36 +622,35 @@
                  container_sync_to: Optional[pulumi.Input[str]] = None,
                  container_write: Optional[pulumi.Input[str]] = None,
                  content_type: Optional[pulumi.Input[str]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 storage_policy: Optional[pulumi.Input[str]] = None,
                  versioning: Optional[pulumi.Input[pulumi.InputType['ContainerVersioningArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ContainerArgs.__new__(ContainerArgs)
 
             __props__.__dict__["container_read"] = container_read
             __props__.__dict__["container_sync_key"] = container_sync_key
             __props__.__dict__["container_sync_to"] = container_sync_to
             __props__.__dict__["container_write"] = container_write
             __props__.__dict__["content_type"] = content_type
             __props__.__dict__["force_destroy"] = force_destroy
             __props__.__dict__["metadata"] = metadata
             __props__.__dict__["name"] = name
             __props__.__dict__["region"] = region
+            __props__.__dict__["storage_policy"] = storage_policy
             __props__.__dict__["versioning"] = versioning
         super(Container, __self__).__init__(
             'openstack:objectstorage/container:Container',
             resource_name,
             __props__,
             opts)
 
@@ -624,14 +663,15 @@
             container_sync_to: Optional[pulumi.Input[str]] = None,
             container_write: Optional[pulumi.Input[str]] = None,
             content_type: Optional[pulumi.Input[str]] = None,
             force_destroy: Optional[pulumi.Input[bool]] = None,
             metadata: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
+            storage_policy: Optional[pulumi.Input[str]] = None,
             versioning: Optional[pulumi.Input[pulumi.InputType['ContainerVersioningArgs']]] = None) -> 'Container':
         """
         Get an existing Container resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
@@ -652,14 +692,16 @@
         :param pulumi.Input[Mapping[str, Any]] metadata: Custom key/value pairs to associate with the container.
                Changing this updates the existing container metadata.
         :param pulumi.Input[str] name: A unique name for the container. Changing this creates a
                new container.
         :param pulumi.Input[str] region: The region in which to create the container. If
                omitted, the `region` argument of the provider is used. Changing this
                creates a new container.
+        :param pulumi.Input[str] storage_policy: The storage policy to be used for the container. 
+               Changing this creates a new container.
         :param pulumi.Input[pulumi.InputType['ContainerVersioningArgs']] versioning: Enable object versioning. The structure is described below.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ContainerState.__new__(_ContainerState)
 
         __props__.__dict__["container_read"] = container_read
@@ -667,14 +709,15 @@
         __props__.__dict__["container_sync_to"] = container_sync_to
         __props__.__dict__["container_write"] = container_write
         __props__.__dict__["content_type"] = content_type
         __props__.__dict__["force_destroy"] = force_destroy
         __props__.__dict__["metadata"] = metadata
         __props__.__dict__["name"] = name
         __props__.__dict__["region"] = region
+        __props__.__dict__["storage_policy"] = storage_policy
         __props__.__dict__["versioning"] = versioning
         return Container(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="containerRead")
     def container_read(self) -> pulumi.Output[Optional[str]]:
         """
@@ -754,14 +797,23 @@
         The region in which to create the container. If
         omitted, the `region` argument of the provider is used. Changing this
         creates a new container.
         """
         return pulumi.get(self, "region")
 
     @property
+    @pulumi.getter(name="storagePolicy")
+    def storage_policy(self) -> pulumi.Output[str]:
+        """
+        The storage policy to be used for the container. 
+        Changing this creates a new container.
+        """
+        return pulumi.get(self, "storage_policy")
+
+    @property
     @pulumi.getter
     def versioning(self) -> pulumi.Output[Optional['outputs.ContainerVersioning']]:
         """
         Enable object versioning. The structure is described below.
         """
         return pulumi.get(self, "versioning")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/container_object.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/container_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ContainerObjectArgs', 'ContainerObject']
@@ -877,20 +878,17 @@
                  etag: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  object_manifest: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  source: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ContainerObjectArgs.__new__(ContainerObjectArgs)
 
             if container_name is None and not opts.urn:
                 raise TypeError("Missing required property 'container_name'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/objectstorage/temp_url.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/objectstorage/temp_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['TempUrlArgs', 'TempUrl']
@@ -378,20 +379,17 @@
                  method: Optional[pulumi.Input[str]] = None,
                  object: Optional[pulumi.Input[str]] = None,
                  regenerate: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  split: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TempUrlArgs.__new__(TempUrlArgs)
 
             if container is None and not opts.urn:
                 raise TypeError("Missing required property 'container'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/orchestration/stack_v1.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/orchestration/stack_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -674,15 +675,15 @@
         ```python
         import pulumi
         import pulumi_openstack as openstack
 
         stack1 = openstack.orchestration.StackV1("stack1",
             disable_rollback=True,
             environment_opts={
-                "Bin": "\n\n",
+                "Bin": "\\n\\n",
             },
             parameters={
                 "length": 4,
             },
             template_opts={
                 "Bin": \"\"\"heat_template_version: 2013-05-23
         parameters:
@@ -761,15 +762,15 @@
         ```python
         import pulumi
         import pulumi_openstack as openstack
 
         stack1 = openstack.orchestration.StackV1("stack1",
             disable_rollback=True,
             environment_opts={
-                "Bin": "\n\n",
+                "Bin": "\\n\\n",
             },
             parameters={
                 "length": 4,
             },
             template_opts={
                 "Bin": \"\"\"heat_template_version: 2013-05-23
         parameters:
@@ -825,20 +826,17 @@
                  status_reason: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template_description: Optional[pulumi.Input[str]] = None,
                  template_opts: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  updated_time: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = StackV1Args.__new__(StackV1Args)
 
             __props__.__dict__["stack_outputs"] = stack_outputs
             __props__.__dict__["capabilities"] = capabilities
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/provider.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
@@ -682,20 +683,17 @@
                  token: Optional[pulumi.Input[str]] = None,
                  use_octavia: Optional[pulumi.Input[bool]] = None,
                  user_domain_id: Optional[pulumi.Input[str]] = None,
                  user_domain_name: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             if allow_reauth is None:
                 allow_reauth = _utilities.get_env_bool('OS_ALLOW_REAUTH')
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/__init__.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/_inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_availbility_zones.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_availbility_zones.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -84,18 +85,15 @@
 
 
     :param str region: The region in which to obtain the V2 Shared File System
            client. If omitted, the `region` argument of the provider is used.
     """
     __args__ = dict()
     __args__['region'] = region
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:sharedfilesystem/getAvailbilityZones:getAvailbilityZones', __args__, opts=opts, typ=GetAvailbilityZonesResult).value
 
     return AwaitableGetAvailbilityZonesResult(
         id=__ret__.id,
         names=__ret__.names,
         region=__ret__.region)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_share.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_share.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -260,18 +261,15 @@
     __args__['isPublic'] = is_public
     __args__['metadata'] = metadata
     __args__['name'] = name
     __args__['region'] = region
     __args__['shareNetworkId'] = share_network_id
     __args__['snapshotId'] = snapshot_id
     __args__['status'] = status
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:sharedfilesystem/getShare:getShare', __args__, opts=opts, typ=GetShareResult).value
 
     return AwaitableGetShareResult(
         availability_zone=__ret__.availability_zone,
         description=__ret__.description,
         export_location_path=__ret__.export_location_path,
         export_locations=__ret__.export_locations,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_share_network.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_share_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -231,18 +232,15 @@
     __args__['name'] = name
     __args__['networkType'] = network_type
     __args__['neutronNetId'] = neutron_net_id
     __args__['neutronSubnetId'] = neutron_subnet_id
     __args__['region'] = region
     __args__['securityServiceId'] = security_service_id
     __args__['segmentationId'] = segmentation_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:sharedfilesystem/getShareNetwork:getShareNetwork', __args__, opts=opts, typ=GetShareNetworkResult).value
 
     return AwaitableGetShareNetworkResult(
         cidr=__ret__.cidr,
         description=__ret__.description,
         id=__ret__.id,
         ip_version=__ret__.ip_version,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/get_snapshot.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/get_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -177,18 +178,15 @@
     """
     __args__ = dict()
     __args__['description'] = description
     __args__['name'] = name
     __args__['region'] = region
     __args__['shareId'] = share_id
     __args__['status'] = status
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('openstack:sharedfilesystem/getSnapshot:getSnapshot', __args__, opts=opts, typ=GetSnapshotResult).value
 
     return AwaitableGetSnapshotResult(
         description=__ret__.description,
         id=__ret__.id,
         name=__ret__.name,
         project_id=__ret__.project_id,
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/security_service.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/security_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SecurityServiceArgs', 'SecurityService']
@@ -21,15 +22,15 @@
                  ou: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  server: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityService resource.
-        :param pulumi.Input[str] type: The security service type - can either be active\_directory,
+        :param pulumi.Input[str] type: The security service type - can either be active\\_directory,
                kerberos or ldap.  Changing this updates the existing security service.
         :param pulumi.Input[str] description: The human-readable description for the security service.
                Changing this updates the description of the existing security service.
         :param pulumi.Input[str] dns_ip: The security service DNS IP address that is used inside the
                tenant network.
         :param pulumi.Input[str] domain: The security service domain.
         :param pulumi.Input[str] name: The name of the security service. Changing this updates the name
@@ -65,15 +66,15 @@
         if user is not None:
             pulumi.set(__self__, "user", user)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The security service type - can either be active\_directory,
+        The security service type - can either be active\\_directory,
         kerberos or ldap.  Changing this updates the existing security service.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
@@ -223,15 +224,15 @@
         :param pulumi.Input[str] password: The user password, if you specify a user.
         :param pulumi.Input[str] project_id: The owner of the Security Service.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Shared File System client.
                A Shared File System client is needed to create a security service. If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                security service.
         :param pulumi.Input[str] server: The security service host name or IP address.
-        :param pulumi.Input[str] type: The security service type - can either be active\_directory,
+        :param pulumi.Input[str] type: The security service type - can either be active\\_directory,
                kerberos or ldap.  Changing this updates the existing security service.
         :param pulumi.Input[str] user: The security service user or group name that is used by the
                tenant.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if dns_ip is not None:
@@ -370,15 +371,15 @@
     def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The security service type - can either be active\_directory,
+        The security service type - can either be active\\_directory,
         kerberos or ldap.  Changing this updates the existing security service.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
@@ -465,15 +466,15 @@
                specify where the share ends up. New in Manila microversion 2.44.
         :param pulumi.Input[str] password: The user password, if you specify a user.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Shared File System client.
                A Shared File System client is needed to create a security service. If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                security service.
         :param pulumi.Input[str] server: The security service host name or IP address.
-        :param pulumi.Input[str] type: The security service type - can either be active\_directory,
+        :param pulumi.Input[str] type: The security service type - can either be active\\_directory,
                kerberos or ldap.  Changing this updates the existing security service.
         :param pulumi.Input[str] user: The security service user or group name that is used by the
                tenant.
         """
         ...
     @overload
     def __init__(__self__,
@@ -541,20 +542,17 @@
                  ou: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  server: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecurityServiceArgs.__new__(SecurityServiceArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["dns_ip"] = dns_ip
@@ -609,15 +607,15 @@
         :param pulumi.Input[str] password: The user password, if you specify a user.
         :param pulumi.Input[str] project_id: The owner of the Security Service.
         :param pulumi.Input[str] region: The region in which to obtain the V2 Shared File System client.
                A Shared File System client is needed to create a security service. If omitted, the
                `region` argument of the provider is used. Changing this creates a new
                security service.
         :param pulumi.Input[str] server: The security service host name or IP address.
-        :param pulumi.Input[str] type: The security service type - can either be active\_directory,
+        :param pulumi.Input[str] type: The security service type - can either be active\\_directory,
                kerberos or ldap.  Changing this updates the existing security service.
         :param pulumi.Input[str] user: The security service user or group name that is used by the
                tenant.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityServiceState.__new__(_SecurityServiceState)
@@ -714,15 +712,15 @@
         """
         return pulumi.get(self, "server")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The security service type - can either be active\_directory,
+        The security service type - can either be active\\_directory,
         kerberos or ldap.  Changing this updates the existing security service.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def user(self) -> pulumi.Output[Optional[str]]:
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/share.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/share.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -690,20 +691,17 @@
                  region: Optional[pulumi.Input[str]] = None,
                  share_network_id: Optional[pulumi.Input[str]] = None,
                  share_proto: Optional[pulumi.Input[str]] = None,
                  share_type: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ShareArgs.__new__(ShareArgs)
 
             __props__.__dict__["availability_zone"] = availability_zone
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/share_access.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/share_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ShareAccessArgs', 'ShareAccess']
@@ -421,20 +422,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  access_to: Optional[pulumi.Input[str]] = None,
                  access_type: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  share_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ShareAccessArgs.__new__(ShareAccessArgs)
 
             if access_level is None and not opts.urn:
                 raise TypeError("Missing required property 'access_level'")
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/sharedfilesystem/share_network.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/sharedfilesystem/share_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ShareNetworkArgs', 'ShareNetwork']
@@ -507,20 +508,17 @@
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  neutron_net_id: Optional[pulumi.Input[str]] = None,
                  neutron_subnet_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  security_service_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ShareNetworkArgs.__new__(ShareNetworkArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["name"] = name
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/_inputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/endpoint_group.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/endpoint_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['EndpointGroupArgs', 'EndpointGroup']
@@ -388,20 +389,17 @@
                  endpoints: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EndpointGroupArgs.__new__(EndpointGroupArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["endpoints"] = endpoints
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/ike_policy.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/ike_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -535,20 +536,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  pfs: Optional[pulumi.Input[str]] = None,
                  phase1_negotiation_mode: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IkePolicyArgs.__new__(IkePolicyArgs)
 
             __props__.__dict__["auth_algorithm"] = auth_algorithm
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/ip_sec_policy.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/ip_sec_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -535,20 +536,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  pfs: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  transform_protocol: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IpSecPolicyArgs.__new__(IpSecPolicyArgs)
 
             __props__.__dict__["auth_algorithm"] = auth_algorithm
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/outputs.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/service.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ServiceArgs', 'Service']
@@ -459,20 +460,17 @@
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  router_id: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ServiceArgs.__new__(ServiceArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack/vpnaas/site_connection.py` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack/vpnaas/site_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -863,20 +864,17 @@
                  peer_id: Optional[pulumi.Input[str]] = None,
                  psk: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  value_specs: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  vpnservice_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SiteConnectionArgs.__new__(SiteConnectionArgs)
 
             __props__.__dict__["admin_state_up"] = admin_state_up
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/PKG-INFO` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-openstack
-Version: 3.9.0a1654086724
+Version: 3.9.0a1659603007
 Summary: A Pulumi package for creating and managing OpenStack cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-openstack
 Description: [![Actions Status](https://github.com/pulumi/pulumi-openstack/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-openstack/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fopenstack.svg)](https://www.npmjs.com/package/@pulumi/openstack)
```

### Comparing `pulumi_openstack-3.9.0a1654086724/pulumi_openstack.egg-info/SOURCES.txt` & `pulumi_openstack-3.9.0a1659603007/pulumi_openstack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 pulumi_openstack/compute/floating_ip_associate.py
 pulumi_openstack/compute/get_aggregate_v2.py
 pulumi_openstack/compute/get_availability_zones.py
 pulumi_openstack/compute/get_flavor.py
 pulumi_openstack/compute/get_hypervisor_v2.py
 pulumi_openstack/compute/get_instance_v2.py
 pulumi_openstack/compute/get_keypair.py
+pulumi_openstack/compute/get_limits_v2.py
 pulumi_openstack/compute/get_quota_set_v2.py
 pulumi_openstack/compute/instance.py
 pulumi_openstack/compute/interface_attach.py
 pulumi_openstack/compute/keypair.py
 pulumi_openstack/compute/outputs.py
 pulumi_openstack/compute/quota_set_v2.py
 pulumi_openstack/compute/sec_group.py
@@ -56,14 +57,16 @@
 pulumi_openstack/config/__init__.py
 pulumi_openstack/config/vars.py
 pulumi_openstack/containerinfra/__init__.py
 pulumi_openstack/containerinfra/cluster.py
 pulumi_openstack/containerinfra/cluster_template.py
 pulumi_openstack/containerinfra/get_cluster.py
 pulumi_openstack/containerinfra/get_cluster_template.py
+pulumi_openstack/containerinfra/get_node_group.py
+pulumi_openstack/containerinfra/node_group.py
 pulumi_openstack/database/__init__.py
 pulumi_openstack/database/_inputs.py
 pulumi_openstack/database/configuration.py
 pulumi_openstack/database/database.py
 pulumi_openstack/database/instance.py
 pulumi_openstack/database/outputs.py
 pulumi_openstack/database/user.py
```

### Comparing `pulumi_openstack-3.9.0a1654086724/setup.py` & `pulumi_openstack-3.9.0a1659603007/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.0a1654086724"
-PLUGIN_VERSION = "3.9.0-alpha.1654086724+007bb9de"
+VERSION = "3.9.0a1659603007"
+PLUGIN_VERSION = "3.9.0-alpha.1659603007+e0710191"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'openstack', PLUGIN_VERSION])
         except OSError as error:
```

