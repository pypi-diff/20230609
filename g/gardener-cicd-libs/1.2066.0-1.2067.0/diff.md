# Comparing `tmp/gardener-cicd-libs-1.2066.0.tar.gz` & `tmp/gardener-cicd-libs-1.2067.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-libs-1.2066.0.tar", last modified: Fri Jun  2 05:01:03 2023, max compression
+gzip compressed data, was "gardener-cicd-libs-1.2067.0.tar", last modified: Fri Jun  9 14:05:36 2023, max compression
```

## Comparing `gardener-cicd-libs-1.2066.0.tar` & `gardener-cicd-libs-1.2067.0.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.186242 gardener-cicd-libs-1.2066.0/ccc/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/alicloud.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/aws.py
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/cfg.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/clamav.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/concourse.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/delivery.py
--rw-r--r--   0 root         (0) root         (0)     6490 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     8491 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/gcp.py
--rw-r--r--   0 root         (0) root         (0)    10735 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/github.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/grafeas_model.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/jira.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/oci.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/protecode.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.186242 gardener-cicd-libs-1.2066.0/cfg_mgmt/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/alicloud.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/aws.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/azure.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_application_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_service_binding.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/gcp.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/github.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/metrics.py
--rw-r--r--   0 root         (0) root         (0)     9811 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/model.py
--rw-r--r--   0 root         (0) root         (0)    16096 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/reporting.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/rotate.py
--rw-r--r--   0 root         (0) root         (0)     9393 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/util.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/cnudie/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/access.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/iter.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/migrate.py
--rw-r--r--   0 root         (0) root         (0)     5996 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/purge.py
--rw-r--r--   0 root         (0) root         (0)     3582 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/replicate.py
--rw-r--r--   0 root         (0) root         (0)    20986 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/retrieve.py
--rw-r--r--   0 root         (0) root         (0)    17536 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/util.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/concourse/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/concourse/client/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14969 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/api.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/model.py
--rw-r--r--   0 root         (0) root         (0)     6557 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/routes.py
--rw-r--r--   0 root         (0) root         (0)    12621 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/util.py
--rw-r--r--   0 root         (0) root         (0)    20369 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/enumerator.py
--rw-r--r--   0 root         (0) root         (0)    10077 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/concourse/model/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7643 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/base.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/job.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    12384 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/resources.py
--rw-r--r--   0 root         (0) root         (0)    17522 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.194242 gardener-cicd-libs-1.2066.0/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     2587 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14494 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     5217 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/cronjob.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/draft_release.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/filter.py
--rw-r--r--   0 root         (0) root         (0)    18964 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/image_scan.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/images.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/meta.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/notifications.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/options.py
--rw-r--r--   0 root         (0) root         (0)    17352 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/publish.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/pullrequest.py
--rw-r--r--   0 root         (0) root         (0)    11334 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/release.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/slack.py
--rw-r--r--   0 root         (0) root         (0)    10994 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/version.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/paths.py
--rw-r--r--   0 root         (0) root         (0)    27053 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/replicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.194242 gardener-cicd-libs-1.2066.0/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-02 05:00:59.000000 gardener-cicd-libs-1.2066.0/concourse/resources/LAST_RELEASED_TAG
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/defaults.mako
--rw-r--r--   0 root         (0) root         (0)     1039 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/email.mako
--rw-r--r--   0 root         (0) root         (0)     4192 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/github.mako
--rw-r--r--   0 root         (0) root         (0)      463 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/image.mako
--rw-r--r--   0 root         (0) root         (0)      639 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/resource_types.mako
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/time.mako
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/variants.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.198242 gardener-cicd-libs-1.2066.0/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/alter_container_images.py
--rw-r--r--   0 root         (0) root         (0)     9157 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.mako
--rw-r--r--   0 root         (0) root         (0)     3137 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.mako
--rw-r--r--   0 root         (0) root         (0)     4097 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.py
--rw-r--r--   0 root         (0) root         (0)    10914 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.mako
--rw-r--r--   0 root         (0) root         (0)     5609 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     2260 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor_util.py
--rw-r--r--   0 root         (0) root         (0)     3385 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/draft_release.mako
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/images.py
--rw-r--r--   0 root         (0) root         (0)     8967 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/malware_scan.mako
--rw-r--r--   0 root         (0) root         (0)      676 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/meta.mako
--rw-r--r--   0 root         (0) root         (0)      977 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/meta.py
--rw-r--r--   0 root         (0) root         (0)     8822 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/notification.mako
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/notification.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/os_id.mako
--rw-r--r--   0 root         (0) root         (0)     5271 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/os_id.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/prepare.mako
--rw-r--r--   0 root         (0) root         (0)     3660 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/publish.mako
--rw-r--r--   0 root         (0) root         (0)     4071 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/release.mako
--rw-r--r--   0 root         (0) root         (0)    36446 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/release.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.mako
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.mako
--rw-r--r--   0 root         (0) root         (0)     4902 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/rm_pr_label.mako
--rw-r--r--   0 root         (0) root         (0)     7028 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.mako
--rw-r--r--   0 root         (0) root         (0)     6837 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.mako
--rw-r--r--   0 root         (0) root         (0)     2107 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     6804 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.mako
--rw-r--r--   0 root         (0) root         (0)    19298 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/version.mako
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/concourse/templates/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23433 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/templates/default.mako
--rw-r--r--   0 root         (0) root         (0)     5362 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/util.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/container/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16315 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/container/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/cosign/
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cosign/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cosign/payload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/ctt/
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/cosign.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/filters.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/platform.py
--rwxr-xr-x   0 root         (0) root         (0)    26860 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/process_dependencies.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/processing_model.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/processors.py
--rw-r--r--   0 root         (0) root         (0)     6811 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/rbsc_bom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/ctt/test/
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/filters_test.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/platform_test.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/process_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/processors_test.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/uploaders_test.py
--rw-r--r--   0 root         (0) root         (0)     7562 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/uploaders.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/delivery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/client.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/model.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/util.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dockerutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/dso/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9639 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/cvss.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/labels.py
--rw-r--r--   0 root         (0) root         (0)     5163 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6165 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      939 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      229 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/github/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/codeowners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/github/compliance/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11313 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/issue.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/milestone.py
--rw-r--r--   0 root         (0) root         (0)     9092 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/model.py
--rw-r--r--   0 root         (0) root         (0)    34570 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/renderer.py
--rw-r--r--   0 root         (0) root         (0)    19222 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/util.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/retry.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/user.py
--rw-r--r--   0 root         (0) root         (0)    33961 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/util.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/webhook.py
--rw-r--r--   0 root         (0) root         (0)    15039 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/gitutil.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/gziputil.py
--rw-r--r--   0 root         (0) root         (0)     6926 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/http_requests.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ioutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/kube/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4912 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/ctx.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/helm.py
--rw-r--r--   0 root         (0) root         (0)    26693 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/mail/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/mail/template_mailer.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/mailutil.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/makoutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/product/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/product/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/product/util.py
--rw-r--r--   0 root         (0) root         (0)    22350 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/product/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/release_notes/
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11275 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/fetch.py
--rw-r--r--   0 root         (0) root         (0)     4645 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/markdown.py
--rw-r--r--   0 root         (0) root         (0)    10869 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)     7272 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/reutil.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/slackclient/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/slackclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/slackclient/util.py
--rw-r--r--   0 root         (0) root         (0)     6591 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/tarutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/client_test.py
--rw-r--r--   0 root         (0) root         (0)     4760 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/factory_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/model/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6657 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/job_test.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/resources_test.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/step_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     7482 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/filter_test.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/slack_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/resources/github_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     6544 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/notification_test.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/release_test.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/update_component_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/version_test.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/container/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/github/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6142 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/github_util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/default_util.py
--rw-r--r--   0 root         (0) root         (0)    18172 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/renderer_test.py
--rw-r--r--   0 root         (0) root         (0)    21822 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/util_test.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/kubeutil_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/product_/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/product_/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/reutil_test.py
--rw-r--r--   0 root         (0) root         (0)     5754 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/unixutil/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/unixutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/unixutil/model.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/unixutil/scan.py
--rw-r--r--   0 root         (0) root         (0)    15220 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.211190 gardener-cicd-libs-1.2067.0/ccc/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/aws.py
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/clamav.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     6490 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     8491 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    10735 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/github.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/grafeas_model.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/jira.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/oci.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ccc/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.211190 gardener-cicd-libs-1.2067.0/cfg_mgmt/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/azure.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/btp_application_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/btp_service_binding.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/github.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/model.py
+-rw-r--r--   0 root         (0) root         (0)    16096 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/reporting.py
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     9393 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cfg_mgmt/util.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.215190 gardener-cicd-libs-1.2067.0/cnudie/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/access.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/iter.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/migrate.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/purge.py
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/replicate.py
+-rw-r--r--   0 root         (0) root         (0)    20986 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/retrieve.py
+-rw-r--r--   0 root         (0) root         (0)    17536 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/util.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cnudie/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.215190 gardener-cicd-libs-1.2067.0/concourse/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.215190 gardener-cicd-libs-1.2067.0/concourse/client/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14969 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/client/api.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/client/model.py
+-rw-r--r--   0 root         (0) root         (0)     6557 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/client/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12621 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/client/util.py
+-rw-r--r--   0 root         (0) root         (0)    20369 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/enumerator.py
+-rw-r--r--   0 root         (0) root         (0)    10077 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.215190 gardener-cicd-libs-1.2067.0/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7643 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/base.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/job.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    12384 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/resources.py
+-rw-r--r--   0 root         (0) root         (0)    17522 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.219190 gardener-cicd-libs-1.2067.0/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14494 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/cronjob.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/draft_release.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/filter.py
+-rw-r--r--   0 root         (0) root         (0)    18964 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/image_scan.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/images.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/meta.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/options.py
+-rw-r--r--   0 root         (0) root         (0)    17352 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/publish.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/pullrequest.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/release.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/slack.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/model/traits/version.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/paths.py
+-rw-r--r--   0 root         (0) root         (0)    27053 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/replicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.219190 gardener-cicd-libs-1.2067.0/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 14:05:31.000000 gardener-cicd-libs-1.2067.0/concourse/resources/LAST_RELEASED_TAG
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/resources/defaults.mako
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/resources/email.mako
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/resources/github.mako
+-rw-r--r--   0 root         (0) root         (0)      463 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/resources/image.mako
+-rw-r--r--   0 root         (0) root         (0)      639 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/resources/resource_types.mako
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/resources/time.mako
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/resources/variants.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.227190 gardener-cicd-libs-1.2067.0/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/alter_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     9157 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/build_oci_image.mako
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/build_oci_image.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/cfg_reporting.mako
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/cfg_reporting.py
+-rw-r--r--   0 root         (0) root         (0)    10914 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/component_descriptor.mako
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/component_descriptor_util.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/draft_release.mako
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/images.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/malware_scan.mako
+-rw-r--r--   0 root         (0) root         (0)      676 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/meta.mako
+-rw-r--r--   0 root         (0) root         (0)      977 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8822 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/notification.mako
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/notification.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/os_id.mako
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/os_id.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/prepare.mako
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/publish.mako
+-rw-r--r--   0 root         (0) root         (0)     4071 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/release.mako
+-rw-r--r--   0 root         (0) root         (0)    36446 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/release.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/replicate_pipelines.mako
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/replicate_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/replicate_secrets.mako
+-rw-r--r--   0 root         (0) root         (0)     4902 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/replicate_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/rm_pr_label.mako
+-rw-r--r--   0 root         (0) root         (0)     7028 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/scan_container_images.mako
+-rw-r--r--   0 root         (0) root         (0)     6837 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/scan_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/scan_sources.mako
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     6828 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/update_component_deps.mako
+-rw-r--r--   0 root         (0) root         (0)    19345 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/version.mako
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/steps/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.227190 gardener-cicd-libs-1.2067.0/concourse/templates/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23433 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/templates/default.mako
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/util.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/concourse/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.227190 gardener-cicd-libs-1.2067.0/container/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/container/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16315 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/container/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.227190 gardener-cicd-libs-1.2067.0/cosign/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cosign/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/cosign/payload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.227190 gardener-cicd-libs-1.2067.0/ctt/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/cosign.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/filters.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/platform.py
+-rwxr-xr-x   0 root         (0) root         (0)    26860 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/process_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/processing_model.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/processors.py
+-rw-r--r--   0 root         (0) root         (0)     6811 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/rbsc_bom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.227190 gardener-cicd-libs-1.2067.0/ctt/test/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/test/filters_test.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/test/platform_test.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/test/process_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/test/processors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/test/uploaders_test.py
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/uploaders.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ctt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.231190 gardener-cicd-libs-1.2067.0/delivery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/delivery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/delivery/client.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/delivery/model.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/delivery/util.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/dockerutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.231190 gardener-cicd-libs-1.2067.0/dso/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/dso/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9639 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/dso/cvss.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/dso/labels.py
+-rw-r--r--   0 root         (0) root         (0)     5163 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/dso/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.231190 gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-09 14:05:36.000000 gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6165 2023-06-09 14:05:36.000000 gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 14:05:36.000000 gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      923 2023-06-09 14:05:36.000000 gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-06-09 14:05:36.000000 gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.231190 gardener-cicd-libs-1.2067.0/github/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/codeowners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.231190 gardener-cicd-libs-1.2067.0/github/compliance/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/compliance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11313 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/compliance/issue.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/compliance/milestone.py
+-rw-r--r--   0 root         (0) root         (0)     9092 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/compliance/model.py
+-rw-r--r--   0 root         (0) root         (0)    34570 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/compliance/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.231190 gardener-cicd-libs-1.2067.0/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/release_notes/renderer.py
+-rw-r--r--   0 root         (0) root         (0)    19222 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/release_notes/util.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/retry.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/user.py
+-rw-r--r--   0 root         (0) root         (0)    33961 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/util.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/github/webhook.py
+-rw-r--r--   0 root         (0) root         (0)    15233 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/gitutil.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/gziputil.py
+-rw-r--r--   0 root         (0) root         (0)     6926 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/http_requests.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/ioutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.231190 gardener-cicd-libs-1.2067.0/kube/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/kube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4912 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/kube/ctx.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/kube/helm.py
+-rw-r--r--   0 root         (0) root         (0)    26693 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/kube/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.235190 gardener-cicd-libs-1.2067.0/mail/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/mail/template_mailer.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/mailutil.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/makoutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.235190 gardener-cicd-libs-1.2067.0/product/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/product/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/product/util.py
+-rw-r--r--   0 root         (0) root         (0)    22350 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/product/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.235190 gardener-cicd-libs-1.2067.0/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/release_notes/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/release_notes/markdown.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)     7629 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/release_notes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/reutil.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.235190 gardener-cicd-libs-1.2067.0/slackclient/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/slackclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/slackclient/util.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/tarutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.235190 gardener-cicd-libs-1.2067.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.235190 gardener-cicd-libs-1.2067.0/test/concourse/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/client_test.py
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/factory_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.235190 gardener-cicd-libs-1.2067.0/test/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6657 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/job_test.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/resources_test.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/step_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/test/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/traits/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     7482 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/traits/filter_test.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/model/traits/slack_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/test/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/resources/github_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/test/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/steps/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/steps/notification_test.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/steps/release_test.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/steps/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/steps/update_component_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/steps/version_test.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/concourse/util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/test/container/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/test/github/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6142 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/github/github_util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/test/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/github/release_notes/default_util.py
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/github/release_notes/renderer_test.py
+-rw-r--r--   0 root         (0) root         (0)    21822 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/github/release_notes/util_test.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/kubeutil_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/test/product_/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/product_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/reutil_test.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/test/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:05:36.239190 gardener-cicd-libs-1.2067.0/unixutil/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/unixutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/unixutil/model.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/unixutil/scan.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2023-06-09 14:04:08.000000 gardener-cicd-libs-1.2067.0/version.py
```

### Comparing `gardener-cicd-libs-1.2066.0/LICENSE.md` & `gardener-cicd-libs-1.2067.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/README.md` & `gardener-cicd-libs-1.2067.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/__init__.py` & `gardener-cicd-libs-1.2067.0/ccc/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/alicloud.py` & `gardener-cicd-libs-1.2067.0/ccc/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/aws.py` & `gardener-cicd-libs-1.2067.0/ccc/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/clamav.py` & `gardener-cicd-libs-1.2067.0/ccc/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/concourse.py` & `gardener-cicd-libs-1.2067.0/ccc/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/delivery.py` & `gardener-cicd-libs-1.2067.0/ccc/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/elasticsearch.py` & `gardener-cicd-libs-1.2067.0/ccc/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/gcp.py` & `gardener-cicd-libs-1.2067.0/ccc/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/github.py` & `gardener-cicd-libs-1.2067.0/ccc/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/grafeas_model.py` & `gardener-cicd-libs-1.2067.0/ccc/grafeas_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/jira.py` & `gardener-cicd-libs-1.2067.0/ccc/jira.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/oci.py` & `gardener-cicd-libs-1.2067.0/ccc/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/protecode.py` & `gardener-cicd-libs-1.2067.0/ccc/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ccc/secrets_server.py` & `gardener-cicd-libs-1.2067.0/ccc/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/alicloud.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/aws.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/azure.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/azure.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_application_certificate.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/btp_application_certificate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_service_binding.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/btp_service_binding.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/gcp.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/github.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/kubernetes.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/kubernetes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/metrics.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/model.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/reporting.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/rotate.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/rotate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cfg_mgmt/util.py` & `gardener-cicd-libs-1.2067.0/cfg_mgmt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cli.py` & `gardener-cicd-libs-1.2067.0/cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cnudie/access.py` & `gardener-cicd-libs-1.2067.0/cnudie/access.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cnudie/iter.py` & `gardener-cicd-libs-1.2067.0/cnudie/iter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cnudie/purge.py` & `gardener-cicd-libs-1.2067.0/cnudie/purge.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cnudie/replicate.py` & `gardener-cicd-libs-1.2067.0/cnudie/replicate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cnudie/retrieve.py` & `gardener-cicd-libs-1.2067.0/cnudie/retrieve.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cnudie/util.py` & `gardener-cicd-libs-1.2067.0/cnudie/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cnudie/validate.py` & `gardener-cicd-libs-1.2067.0/cnudie/validate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/__init__.py` & `gardener-cicd-libs-1.2067.0/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/client/__init__.py` & `gardener-cicd-libs-1.2067.0/concourse/client/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/client/api.py` & `gardener-cicd-libs-1.2067.0/concourse/client/api.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/client/model.py` & `gardener-cicd-libs-1.2067.0/concourse/client/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/client/routes.py` & `gardener-cicd-libs-1.2067.0/concourse/client/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/client/util.py` & `gardener-cicd-libs-1.2067.0/concourse/client/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/enumerator.py` & `gardener-cicd-libs-1.2067.0/concourse/enumerator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/factory.py` & `gardener-cicd-libs-1.2067.0/concourse/factory.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/__init__.py` & `gardener-cicd-libs-1.2067.0/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/base.py` & `gardener-cicd-libs-1.2067.0/concourse/model/base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/job.py` & `gardener-cicd-libs-1.2067.0/concourse/model/job.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/pipeline.py` & `gardener-cicd-libs-1.2067.0/concourse/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/resources.py` & `gardener-cicd-libs-1.2067.0/concourse/model/resources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/step.py` & `gardener-cicd-libs-1.2067.0/concourse/model/step.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/component_descriptor.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/cronjob.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/cronjob.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/draft_release.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/draft_release.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,32 @@
   ScriptType,
   Trait,
   TraitTransformer,
 )
 from concourse.model.job import (
   JobVariant,
 )
+from concourse.model.traits.release import (
+    ReleaseNotesHandling,
+)
 
 ATTRIBUTES = (
     AttributeSpec.optional(
         name='preprocess',
         default='finalize',
         doc='version processing operation to set effective version',
     ),
+    AttributeSpec.optional(
+        name='release_notes_handling',
+        default=ReleaseNotesHandling.DEFAULT.value,
+        doc='''
+        configures which iteration of the code to use when generating release notes.
+        ''',
+        type=ReleaseNotesHandling,
+    ),
 )
 
 
 class DraftReleaseTrait(Trait):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -47,14 +58,17 @@
     @classmethod
     def _attribute_specs(cls):
         return ATTRIBUTES
 
     def _preprocess(self):
         return self.raw['preprocess']
 
+    def release_notes_handling(self) -> ReleaseNotesHandling:
+        return ReleaseNotesHandling(self.raw['release_notes_handling'])
+
     def validate(self):
         super().validate()
         if self._preprocess() != 'finalize':
             raise ModelValidationError(
                 "Only 'finalize' is supported as value for 'preprocess' in draft_release trait"
             )
```

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/filter.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/filter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/image_scan.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/image_scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/images.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/meta.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/notifications.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/notifications.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/options.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/options.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/publish.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/publish.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/pullrequest.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/pullrequest.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/release.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/scan_sources.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/scheduling.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/scheduling.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/slack.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/slack.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/update_component_deps.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/update_component_deps.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 from concourse.model.step import (
     PipelineStep,
     PrivilegeMode,
     PullRequestNotificationPolicy,
 )
 from concourse.model.base import (
     AttributeSpec,
-    EnumValueWithDocumentation,
-    EnumWithDocumentation,
     ModelBase,
     ScriptType,
     Trait,
     TraitTransformer,
 )
 from concourse.model.job import (
     JobVariant,
 )
+from concourse.model.traits.release import (
+    ReleaseNotesHandling,
+)
 from model.base import ModelValidationError
 
 import concourse.model.traits.component_descriptor
 import concourse.model.traits.images
 
 OciImageCfg = concourse.model.traits.images.OciImageCfg
 
@@ -53,35 +54,14 @@
 
 
 class UpstreamUpdatePolicy(enum.Enum):
     STRICTLY_FOLLOW = 'strictly_follow'
     ACCEPT_HOTFIXES = 'accept_hotfixes'
 
 
-class ReleaseNotesHandling(EnumWithDocumentation):
-    DEFAULT = EnumValueWithDocumentation(
-        value='default',
-        doc='''
-        Use default version of release note creation code. Use this if you are interested in
-        stability rather than the latest features.
-        ''',
-    )
-    PREVIEW = EnumValueWithDocumentation(
-        value='preview',
-        doc='''
-            Use preview version of release note creation code. Use this to join new features and
-            feature-rollouts.
-
-            .. note::
-                if no features are being tested/rolled-out, using this value is the same as using
-                `default`.
-        '''
-    )
-
-
 MERGE_POLICY_CONFIG_ATTRIBUTES = (
     AttributeSpec.optional(
         name='component_names',
         default=[],
         type=typing.List[str],
         doc=(
             'a sequence of regular expressions. This merge policy will be applied to matching '
```

### Comparing `gardener-cicd-libs-1.2066.0/concourse/model/traits/version.py` & `gardener-cicd-libs-1.2067.0/concourse/model/traits/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/replicator.py` & `gardener-cicd-libs-1.2067.0/concourse/replicator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/resources/defaults.mako` & `gardener-cicd-libs-1.2067.0/concourse/resources/defaults.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/resources/email.mako` & `gardener-cicd-libs-1.2067.0/concourse/resources/email.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/resources/github.mako` & `gardener-cicd-libs-1.2067.0/concourse/resources/github.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/resources/resource_types.mako` & `gardener-cicd-libs-1.2067.0/concourse/resources/resource_types.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/resources/variants.mako` & `gardener-cicd-libs-1.2067.0/concourse/resources/variants.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/alter_container_images.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/alter_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/build_oci_image.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/build_oci_image.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/cfg_reporting.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/cfg_reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/component_descriptor.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor_util.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/component_descriptor_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/draft_release.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/draft_release.mako`

 * *Files 17% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 component_descriptor_trait = job_variant.trait('component_descriptor')
 component_name = component_descriptor_trait.component_name()
 version_operation = draft_release_trait._preprocess()
 component_descriptor_path = os.path.join(
     job_step.input('component_descriptor_dir'),
     cdu.component_descriptor_fname(gci.componentmodel.SchemaVersion.V2),
 )
+release_notes_handling=draft_release_trait.release_notes_handling().value
 %>
 import version
 import os
 
-import ci.util
 import ccc.github
+import ci.util
 import cnudie.util
 import gci.componentmodel as cm
+import release_notes.fetch
+import release_notes.markdown
 
+from concourse.model.traits.release import ReleaseNotesHandling
 from gitutil import GitHelper
 from github.release_notes.util import (
     draft_release_name_for_version,
     ReleaseNotes,
     github_repo_path,
 )
 from github.util import (
@@ -80,24 +84,37 @@
     branch='${repo.branch()}',
 )
 
 github_helper = GitHubRepositoryHelper.from_githubrepobranch(
     githubrepobranch=githubrepobranch,
 )
 
-release_notes = ReleaseNotes(
-    component=component,
-    repo_dir=repo_dir,
+release_notes_handling = ReleaseNotesHandling(
+    '${release_notes_handling}'
 )
 
-release_notes.create(
-    start_ref='${repo.branch()}'
-)
+if release_notes_handling is ReleaseNotesHandling.DEFAULT:
+    release_notes = ReleaseNotes(
+        component=component,
+        repo_dir=repo_dir,
+    )
+    release_notes.create(
+        start_ref='${repo.branch()}'
+    )
+    release_notes_md = release_notes.to_markdown()
 
-release_notes_md = release_notes.to_markdown()
+elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
+    release_note_blocks = release_notes.fetch.fetch_release_notes(
+        repo_path=repo_dir,
+        component=component,
+        current_version=version.parse_to_semver(processed_version),
+    )
+    release_notes_md = '\n'.join(
+        str(i) for i in release_notes.markdown.render(release_note_blocks)
+    ) or 'no release notes available'
 
 draft_name = draft_release_name_for_version(processed_version)
 draft_release = github_helper.draft_release_with_name(draft_name)
 if not draft_release:
     github_helper.create_draft_release(
         name=draft_name,
         body=release_notes_md,
```

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/images.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/malware_scan.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/malware_scan.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/meta.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/meta.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/meta.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/notification.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/notification.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/notification.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/notification.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/os_id.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/os_id.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/os_id.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/os_id.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/prepare.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/prepare.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/publish.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/publish.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/release.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/release.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/release.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/replicate_pipelines.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/replicate_pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/replicate_secrets.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/replicate_secrets.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/rm_pr_label.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/rm_pr_label.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/scan_container_images.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/scan_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/scan_sources.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/update_component_deps.mako`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 import os
 import subprocess
 import sys
 
 import dacite
 
 import ci.util
+import concourse.model.traits.release
 import concourse.model.traits.update_component_deps
 import ctx
 import gci.componentmodel
 import github.util
 import gitutil
 
 logger = logging.getLogger('step.update_component_deps')
@@ -92,15 +93,15 @@
 ]
 merge_policy_and_filters = {
     p: component_ref_component_name_filter(
         include_regexes=p.component_names(),
         exclude_regexes=(),
     ) for p in merge_policy_configs
 }
-release_notes_handling = concourse.model.traits.update_component_deps.ReleaseNotesHandling(
+release_notes_handling = concourse.model.traits.release.ReleaseNotesHandling(
     '${release_notes_handling.value}'
 )
 # indicates whether or not an upstream component was defined as a reference
 upstream_component_name = os.environ.get('UPSTREAM_COMPONENT_NAME', None)
 UPGRADE_TO_UPSTREAM = bool(upstream_component_name)
 
 logger.info(f'{UPGRADE_TO_UPSTREAM=}')
```

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/update_component_deps.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 import dockerutil
 import github.util
 import gitutil
 import model.container_registry as cr
 import product.v2
 import release_notes.fetch as release_notes_fetch
 import version
+from concourse.model.traits.release import (
+    ReleaseNotesHandling,
+)
 from concourse.model.traits.update_component_deps import (
     MergePolicy,
     MergeMethod,
-    ReleaseNotesHandling,
 )
 from github.util import (
     GitHubRepoBranch,
 )
 from github.release_notes.util import ReleaseNotes
 
 logger = logging.getLogger('step.update_component_deps')
```

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/version.mako` & `gardener-cicd-libs-1.2067.0/concourse/steps/version.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/steps/version.py` & `gardener-cicd-libs-1.2067.0/concourse/steps/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/templates/__init__.py` & `gardener-cicd-libs-1.2067.0/concourse/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/templates/default.mako` & `gardener-cicd-libs-1.2067.0/concourse/templates/default.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/util.py` & `gardener-cicd-libs-1.2067.0/concourse/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/concourse/validator.py` & `gardener-cicd-libs-1.2067.0/concourse/validator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/container/__init__.py` & `gardener-cicd-libs-1.2067.0/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/container/util.py` & `gardener-cicd-libs-1.2067.0/container/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cosign/__init__.py` & `gardener-cicd-libs-1.2067.0/cosign/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/cosign/payload.py` & `gardener-cicd-libs-1.2067.0/cosign/payload.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/cosign.py` & `gardener-cicd-libs-1.2067.0/ctt/cosign.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/filters.py` & `gardener-cicd-libs-1.2067.0/ctt/filters.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/platform.py` & `gardener-cicd-libs-1.2067.0/ctt/platform.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/process_dependencies.py` & `gardener-cicd-libs-1.2067.0/ctt/process_dependencies.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/processing_model.py` & `gardener-cicd-libs-1.2067.0/ctt/processing_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/processors.py` & `gardener-cicd-libs-1.2067.0/ctt/processors.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/rbsc_bom.py` & `gardener-cicd-libs-1.2067.0/ctt/rbsc_bom.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/test/filters_test.py` & `gardener-cicd-libs-1.2067.0/ctt/test/filters_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/test/platform_test.py` & `gardener-cicd-libs-1.2067.0/ctt/test/platform_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/test/process_deps_test.py` & `gardener-cicd-libs-1.2067.0/ctt/test/process_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/test/processors_test.py` & `gardener-cicd-libs-1.2067.0/ctt/test/processors_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/test/uploaders_test.py` & `gardener-cicd-libs-1.2067.0/ctt/test/uploaders_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/uploaders.py` & `gardener-cicd-libs-1.2067.0/ctt/uploaders.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/ctt/util.py` & `gardener-cicd-libs-1.2067.0/ctt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/delivery/client.py` & `gardener-cicd-libs-1.2067.0/delivery/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/delivery/model.py` & `gardener-cicd-libs-1.2067.0/delivery/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/delivery/util.py` & `gardener-cicd-libs-1.2067.0/delivery/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/dockerutil.py` & `gardener-cicd-libs-1.2067.0/dockerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/dso/cvss.py` & `gardener-cicd-libs-1.2067.0/dso/cvss.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/dso/labels.py` & `gardener-cicd-libs-1.2067.0/dso/labels.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/dso/model.py` & `gardener-cicd-libs-1.2067.0/dso/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/SOURCES.txt` & `gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/requires.txt` & `gardener-cicd-libs-1.2067.0/gardener_cicd_libs.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-gardener-cicd-base>=1.2066.0
-gardener-oci>=1.2066.0
+gardener-cicd-base>=1.2067.0
+gardener-oci>=1.2067.0
 GitPython
 Mako<2.0.0
 Sphinx
 aliyun-python-sdk-core==2.13.36
 aliyun-python-sdk-ecs==4.24.63
 aliyun-python-sdk-ram==3.3.0
 awesomeversion
@@ -34,15 +34,14 @@
 openstacksdk
 oss2==2.17.0
 passlib<2.0.0
 pycryptodome
 pydash<8.0.0
 pylama
 pylint
-pymongo
 pytest
 python-dateutil
 python-gitlab
 python-keystoneclient
 python-magic
 python-swiftclient
 pytimeparse
@@ -52,10 +51,9 @@
 semver<4.0.0
 slackclient<3.0.0
 sphinx_rtd_theme<2.0.0
 sseclient-py<2.0.0
 tabulate<1.0.0
 termcolor<3.0.0
 urllib3<3.0.0
-uvicorn
 websockets
 yamllint
```

### Comparing `gardener-cicd-libs-1.2066.0/github/__init__.py` & `gardener-cicd-libs-1.2067.0/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/codeowners.py` & `gardener-cicd-libs-1.2067.0/github/codeowners.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/compliance/issue.py` & `gardener-cicd-libs-1.2067.0/github/compliance/issue.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/compliance/milestone.py` & `gardener-cicd-libs-1.2067.0/github/compliance/milestone.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/compliance/model.py` & `gardener-cicd-libs-1.2067.0/github/compliance/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/compliance/report.py` & `gardener-cicd-libs-1.2067.0/github/compliance/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2067.0/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/release_notes/model.py` & `gardener-cicd-libs-1.2067.0/github/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/release_notes/renderer.py` & `gardener-cicd-libs-1.2067.0/github/release_notes/renderer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/release_notes/util.py` & `gardener-cicd-libs-1.2067.0/github/release_notes/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/retry.py` & `gardener-cicd-libs-1.2067.0/github/retry.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/user.py` & `gardener-cicd-libs-1.2067.0/github/user.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/util.py` & `gardener-cicd-libs-1.2067.0/github/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/github/webhook.py` & `gardener-cicd-libs-1.2067.0/github/webhook.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/gitutil.py` & `gardener-cicd-libs-1.2067.0/gitutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,19 @@
 
     def fetch_head(self, ref: str):
         with self._authenticated_remote() as (cmd_env, remote):
             with remote.repo.git.custom_environment(**cmd_env):
                 fetch_result = remote.fetch(ref)[0]
                 return fetch_result.commit
 
+    def fetch_tags(self):
+        with self._authenticated_remote() as (cmd_env, remote):
+            with remote.repo.git.custom_environment(**cmd_env):
+                remote.fetch(tag=True)
+
 
 def url_with_credentials(
     github_cfg: GithubConfig,
     github_repo_path: str,
     technical_user_name: str | None =None
 ):
     base_url = urllib.parse.urlparse(github_cfg.http_url())
```

### Comparing `gardener-cicd-libs-1.2066.0/gziputil.py` & `gardener-cicd-libs-1.2067.0/gziputil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/http_requests.py` & `gardener-cicd-libs-1.2067.0/http_requests.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/kube/__init__.py` & `gardener-cicd-libs-1.2067.0/kube/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/kube/ctx.py` & `gardener-cicd-libs-1.2067.0/kube/ctx.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/kube/helm.py` & `gardener-cicd-libs-1.2067.0/kube/helm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/kube/helper.py` & `gardener-cicd-libs-1.2067.0/kube/helper.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/mail/__init__.py` & `gardener-cicd-libs-1.2067.0/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/mail/template_mailer.py` & `gardener-cicd-libs-1.2067.0/mail/template_mailer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/mailutil.py` & `gardener-cicd-libs-1.2067.0/mailutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/product/__init__.py` & `gardener-cicd-libs-1.2067.0/product/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/product/util.py` & `gardener-cicd-libs-1.2067.0/product/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/product/v2.py` & `gardener-cicd-libs-1.2067.0/product/v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/release_notes/__init__.py` & `gardener-cicd-libs-1.2067.0/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/release_notes/fetch.py` & `gardener-cicd-libs-1.2067.0/release_notes/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,32 @@
 
     if not (merge_commit_list := repo.merge_base(main_tag, other_tag)) or not \
             (merge_commit := merge_commit_list.pop()):
         raise RuntimeError('cannot find merge base')
     return tuple(repo.iter_commits(f'{main_tag.commit.hexsha}...{merge_commit.hexsha}'))
 
 
+def _list_commits_since_tag(
+        repo: git.Repo,
+        tag: git.TagReference,
+) -> tuple[git.Commit]:
+    '''Return a list of between the given tag and HEAD
+
+    :return: a tuple of commits'''
+    if repo.is_ancestor(tag.commit, 'HEAD'):
+        return tuple(repo.iter_commits(f'HEAD...{tag.commit.hexsha}'))
+
+    if (
+        not (merge_commit_list := repo.merge_base('HEAD', tag))
+        or not (merge_commit := merge_commit_list.pop())
+    ):
+        raise RuntimeError('cannot find merge base')
+    return tuple(repo.iter_commits(f'HEAD...{merge_commit.hexsha}'))
+
+
 def _get_release_note_commits_tuple_for_minor_release(
         previous_version: semver.VersionInfo,
         component_versions: dict[semver.VersionInfo, str],
         git_helper: gitutil.GitHelper,
         github_repo: github3.repos.Repository,
         current_version_tag: git.TagReference,
 ) -> tuple[tuple[git.Commit], tuple[git.Commit]]:
@@ -112,14 +130,21 @@
     '''
     # initial release
     if not previous_version or len(component_versions) == 1:
         logger.info('version appears to be an initial release.')
         # just return all commits starting from the current_version_tag
         return tuple(git_helper.repo.iter_commits(current_version_tag)), tuple()
 
+    if not current_version:
+        logger.info('No current version specified. Start fetching of release notes at HEAD')
+        return _list_commits_since_tag(
+            repo=git_helper.repo,
+            tag=previous_version_tag,
+        ), tuple()
+
     # new major release (not supported yet)
     if current_version.major != previous_version.major:
         raise NotImplementedError(
             'generating release notes for new major releases is not supported yet.'
         )
 
     # new minor release
@@ -151,43 +176,44 @@
         current_version: typing.Optional[semver.VersionInfo] = None,
         previous_version: typing.Optional[semver.VersionInfo] = None,
 ) -> set[rnm.ReleaseNote]:
     ''' Fetches and returns a set of release notes for the specified component.
 
     :param component: An instance of the Component class from the GCI component model.
     :param repo_path: The (local) path to the git-repository.
-    :param current_version: Optional argument to retrieve release notes for a specific version.
+    :param current_version: Optional argument to retrieve release notes up to a specific version.
+        If not given, the current `HEAD` is used.
+    :param previous_version: Optional argument to retrieve release notes starting at a specific
+        version. If not given, the closest version to `current_version` is used
+
     :return: A set of ReleaseNote objects for the specified component.
     '''
     source = cnudie.util.determine_main_source_for_component(component)
     github_helper = ghrnu.github_helper_from_github_access(source.access)
     git_helper = ghrnu.git_helper_from_github_access(source.access, repo_path)
+    # make sure _all_ tags are available locally
+    git_helper.fetch_tags()
 
     # find all available versions
     component_versions: dict[semver.VersionInfo, str] = {}
     for ver in cnudie.retrieve.component_versions(
             component.name,
             component.current_repository_ctx()
     ):
         parsed_version = version.parse_to_semver(ver)
         if parsed_version.prerelease:  # ignore pre-releases
             continue
         component_versions[parsed_version] = ver
 
     if not current_version:
-        if not source.version:
-            raise ValueError('current_version not passed and not found in component source')
-        current_version = version.parse_to_semver(source.version)
-        # access tag from component
-        current_version_tag = git_helper.repo.tag(source.access.ref)
+        current_version_tag = None
     else:
         current_version_tag = git_helper.repo.tag(component_versions[current_version])
-
-    if not current_version_tag:
-        raise RuntimeError(f'cannot find ref {source.access.ref} in repo')
+        if not current_version_tag:
+            raise RuntimeError(f'cannot find ref {source.access.ref} in repo')
 
     if not previous_version:
         previous_version = rnu.find_next_smallest_version(
             list(component_versions.keys()), current_version
         )
     previous_version_tag: typing.Optional[git.TagReference] = None
     if previous_version:
```

### Comparing `gardener-cicd-libs-1.2066.0/release_notes/markdown.py` & `gardener-cicd-libs-1.2067.0/release_notes/markdown.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/release_notes/model.py` & `gardener-cicd-libs-1.2067.0/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/release_notes/utils.py` & `gardener-cicd-libs-1.2067.0/release_notes/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,15 +74,25 @@
 
 
 def find_next_smallest_version(
         available_versions: list[semver.VersionInfo],
         current_version: semver.VersionInfo
 ) -> typing.Optional[semver.VersionInfo]:
     # find version before the requested version and sort by semver
-    return max((v for v in sorted(available_versions) if v < current_version), default=None)
+    # If no version requested, return greatest version
+    sorted_versions =  sorted(available_versions, reverse=True)
+    if not sorted_versions:
+        return None
+
+    if current_version:
+        # TODO: the desired version is always the first hit, so this can be optimised further.
+        # Do so in a way that keeps readability.
+        return max(v for v in sorted_versions if v < current_version)
+    else:
+        return sorted_versions[0]
 
 
 def _find_git_notes_for_commit(
         repo: git.Repo,
         commit: git.Commit
 ) -> typing.Optional[str]:
     try:
```

### Comparing `gardener-cicd-libs-1.2066.0/reutil.py` & `gardener-cicd-libs-1.2067.0/reutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/setup.py` & `gardener-cicd-libs-1.2067.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/slackclient/__init__.py` & `gardener-cicd-libs-1.2067.0/slackclient/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/slackclient/util.py` & `gardener-cicd-libs-1.2067.0/slackclient/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/tarutil.py` & `gardener-cicd-libs-1.2067.0/tarutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/__init__.py` & `gardener-cicd-libs-1.2067.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/_test_utils.py` & `gardener-cicd-libs-1.2067.0/test/_test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/__init__.py` & `gardener-cicd-libs-1.2067.0/test/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/client_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/client_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/factory_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/factory_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/__init__.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/job_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/job_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/resources_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/resources_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/step_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/step_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/component_descriptor_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/traits/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/filter_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/traits/filter_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/slack_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/model/traits/slack_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/resources/__init__.py` & `gardener-cicd-libs-1.2067.0/test/concourse/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/resources/github_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/resources/github_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2067.0/test/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/steps/component_descriptor_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/steps/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/steps/notification_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/steps/notification_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/steps/release_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/steps/release_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/steps/test_utils.py` & `gardener-cicd-libs-1.2067.0/test/concourse/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/steps/update_component_deps_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/steps/update_component_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/steps/version_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/steps/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/concourse/util_test.py` & `gardener-cicd-libs-1.2067.0/test/concourse/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/container/__init__.py` & `gardener-cicd-libs-1.2067.0/test/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/github/__init__.py` & `gardener-cicd-libs-1.2067.0/test/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/github/github_util_test.py` & `gardener-cicd-libs-1.2067.0/test/github/github_util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2067.0/test/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/github/release_notes/default_util.py` & `gardener-cicd-libs-1.2067.0/test/github/release_notes/default_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/github/release_notes/renderer_test.py` & `gardener-cicd-libs-1.2067.0/test/github/release_notes/renderer_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/github/release_notes/util_test.py` & `gardener-cicd-libs-1.2067.0/test/github/release_notes/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/kubeutil_test.py` & `gardener-cicd-libs-1.2067.0/test/kubeutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/product_/__init__.py` & `gardener-cicd-libs-1.2067.0/test/product_/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/reutil_test.py` & `gardener-cicd-libs-1.2067.0/test/reutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/test/version_test.py` & `gardener-cicd-libs-1.2067.0/test/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/unixutil/model.py` & `gardener-cicd-libs-1.2067.0/unixutil/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/unixutil/scan.py` & `gardener-cicd-libs-1.2067.0/unixutil/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2066.0/version.py` & `gardener-cicd-libs-1.2067.0/version.py`

 * *Files identical despite different names*

