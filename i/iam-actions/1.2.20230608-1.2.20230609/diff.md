# Comparing `tmp/iam_actions-1.2.20230608.tar.gz` & `tmp/iam_actions-1.2.20230609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230608.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230609.tar", max compression
```

## Comparing `iam_actions-1.2.20230608.tar` & `iam_actions-1.2.20230609.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-08 02:47:50.052026 iam_actions-1.2.20230608/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-08 02:47:50.052026 iam_actions-1.2.20230608/README.md
--rw-r--r--   0        0        0      228 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/__init__.py
--rw-r--r--   0        0        0  4297233 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/services.py
--rw-r--r--   0        0        0   552341 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/policies.json
--rw-r--r--   0        0        0   196565 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   535757 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-08 02:49:25.257757 iam_actions-1.2.20230608/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230608/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230608/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/README.md
+-rw-r--r--   0        0        0      228 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4300020 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   552817 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/policies.json
+-rw-r--r--   0        0        0   196565 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   536179 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-09 02:52:29.944206 iam_actions-1.2.20230609/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230609/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230609/PKG-INFO
```

### Comparing `iam_actions-1.2.20230608/LICENSE` & `iam_actions-1.2.20230609/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/README.md` & `iam_actions-1.2.20230609/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/actions.json` & `iam_actions-1.2.20230609/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994674744897959%*

 * *Differences: {"'cloudfront'": "{delete: ['UpdateDistributionWithStagingConfig']}",*

 * * "'profile'": "{'ListCalculatedAttributesForProfile': OrderedDict([('access_level', "*

 * *              "'Undocumented'), ('action', 'ListCalculatedAttributesForProfile'), "*

 * *              "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *              "False), ('resources', [])]), 'ListCalculatedAttributeDefinitions': "*

 * *              "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'Lis […]*

```diff
@@ -20274,24 +20274,14 @@
             "condition_keys": [],
             "description": "Grants permission to update the configuration for a web distribution",
             "orphan": false,
             "resources": [
                 "distribution"
             ]
         },
-        "UpdateDistributionWithStagingConfig": {
-            "access_level": "Write",
-            "action": "UpdateDistributionWithStagingConfig",
-            "condition_keys": [],
-            "description": "Grants permission to copy the staging distribution's configuration to its corresponding primary distribution",
-            "orphan": false,
-            "resources": [
-                "distribution"
-            ]
-        },
         "UpdateFieldLevelEncryptionConfig": {
             "access_level": "Write",
             "action": "UpdateFieldLevelEncryptionConfig",
             "condition_keys": [],
             "description": "Grants permission to update a field-level encryption configuration",
             "orphan": false,
             "resources": []
@@ -107687,27 +107677,43 @@
             "condition_keys": [],
             "description": "Grants permission to add a profile key",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
+        "CreateCalculatedAttributeDefinition": {
+            "access_level": "Undocumented",
+            "action": "CreateCalculatedAttributeDefinition",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateDomain": {
             "access_level": "Write",
             "action": "CreateDomain",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a Domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
+        "CreateEventStream": {
+            "access_level": "Undocumented",
+            "action": "CreateEventStream",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateIntegrationWorkflow": {
             "access_level": "Write",
             "action": "CreateIntegrationWorkflow",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -107723,24 +107729,40 @@
             "condition_keys": [],
             "description": "Grants permission to create a profile in the domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
+        "DeleteCalculatedAttributeDefinition": {
+            "access_level": "Undocumented",
+            "action": "DeleteCalculatedAttributeDefinition",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteDomain": {
             "access_level": "Write",
             "action": "DeleteDomain",
             "condition_keys": [],
             "description": "Grants permission to delete a Domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
+        "DeleteEventStream": {
+            "access_level": "Undocumented",
+            "action": "DeleteEventStream",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteIntegration": {
             "access_level": "Write",
             "action": "DeleteIntegration",
             "condition_keys": [],
             "description": "Grants permission to delete a integration in a domain",
             "orphan": false,
             "resources": [
@@ -107806,24 +107828,48 @@
             "condition_keys": [],
             "description": "Grants permission to get a preview of auto merging in a domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
+        "GetCalculatedAttributeDefinition": {
+            "access_level": "Undocumented",
+            "action": "GetCalculatedAttributeDefinition",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetCalculatedAttributeForProfile": {
+            "access_level": "Undocumented",
+            "action": "GetCalculatedAttributeForProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetDomain": {
             "access_level": "Read",
             "action": "GetDomain",
             "condition_keys": [],
             "description": "Grants permission to get a specific domain in an account",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
+        "GetEventStream": {
+            "access_level": "Undocumented",
+            "action": "GetEventStream",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetIdentityResolutionJob": {
             "access_level": "Read",
             "action": "GetIdentityResolutionJob",
             "condition_keys": [],
             "description": "Grants permission to get an identity resolution job in a domain",
             "orphan": false,
             "resources": [
@@ -107894,22 +107940,46 @@
             "access_level": "List",
             "action": "ListAccountIntegrations",
             "condition_keys": [],
             "description": "Grants permission to list all the integrations in the account",
             "orphan": false,
             "resources": []
         },
+        "ListCalculatedAttributeDefinitions": {
+            "access_level": "Undocumented",
+            "action": "ListCalculatedAttributeDefinitions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListCalculatedAttributesForProfile": {
+            "access_level": "Undocumented",
+            "action": "ListCalculatedAttributesForProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListDomains": {
             "access_level": "List",
             "action": "ListDomains",
             "condition_keys": [],
             "description": "Grants permission to list all the domains in an account",
             "orphan": false,
             "resources": []
         },
+        "ListEventStreams": {
+            "access_level": "Undocumented",
+            "action": "ListEventStreams",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListIdentityResolutionJobs": {
             "access_level": "List",
             "action": "ListIdentityResolutionJobs",
             "condition_keys": [],
             "description": "Grants permission to list identity resolution jobs in a domain",
             "orphan": false,
             "resources": [
@@ -108050,14 +108120,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove tags from a resource",
             "orphan": false,
             "resources": []
         },
+        "UpdateCalculatedAttributeDefinition": {
+            "access_level": "Undocumented",
+            "action": "UpdateCalculatedAttributeDefinition",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateDomain": {
             "access_level": "Write",
             "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Grants permission to update a Domain",
             "orphan": false,
             "resources": [
@@ -137131,14 +137209,22 @@
             "condition_keys": [],
             "description": "Grants permission to a queue for a specific principal",
             "orphan": false,
             "resources": [
                 "queue"
             ]
         },
+        "CancelMessageMoveTask": {
+            "access_level": "Undocumented",
+            "action": "CancelMessageMoveTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ChangeMessageVisibility": {
             "access_level": "Write",
             "action": "ChangeMessageVisibility",
             "condition_keys": [],
             "description": "Grants permission to change the visibility timeout of a specified message in a queue to a new value",
             "orphan": false,
             "resources": [
@@ -137204,14 +137290,22 @@
             "condition_keys": [],
             "description": "Grants permission to return a list of your queues that have the RedrivePolicy queue attribute configured with a dead letter queue",
             "orphan": false,
             "resources": [
                 "queue"
             ]
         },
+        "ListMessageMoveTasks": {
+            "access_level": "Undocumented",
+            "action": "ListMessageMoveTasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListQueueTags": {
             "access_level": "Read",
             "action": "ListQueueTags",
             "condition_keys": [],
             "description": "Grants permission to list tags added to an SQS queue",
             "orphan": false,
             "resources": [
@@ -137272,14 +137366,22 @@
             "condition_keys": [],
             "description": "Grants permission to set the value of one or more queue attributes",
             "orphan": false,
             "resources": [
                 "queue"
             ]
         },
+        "StartMessageMoveTask": {
+            "access_level": "Undocumented",
+            "action": "StartMessageMoveTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagQueue": {
             "access_level": "Tagging",
             "action": "TagQueue",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
```

### Comparing `iam_actions-1.2.20230608/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230609/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230609/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/generate/generate.py` & `iam_actions-1.2.20230609/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230609/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230609/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/generate/services.py` & `iam_actions-1.2.20230609/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/policies.json` & `iam_actions-1.2.20230609/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994666730779613%*

 * *Differences: {"'serviceMap'": "{'Amazon Connect Customer Profiles': {'Actions': {insert: [(1, "*

 * *                 "'CreateCalculatedAttributeDefinition'), (3, 'CreateEventStream'), (6, "*

 * *                 "'DeleteCalculatedAttributeDefinition'), (8, 'DeleteEventStream'), (16, "*

 * *                 "'GetCalculatedAttributeDefinition'), (17, 'GetCalculatedAttributeForProfile'), "*

 * *                 "(19, 'GetEventStream'), (28, 'ListCalculatedAttributeDefinitions'), (29, "*

 * *                 "'ListCalculatedAttributesForProfile'), […]*

```diff
@@ -3356,14 +3356,64 @@
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "elasticloadbalancing:CreateAction",
                 "elasticloadbalancing:ResourceTag/",
                 "elasticloadbalancing:ResourceTag/${TagKey}"
             ]
         },
+        "AWS Elastic Load Balancing V2": {
+            "ARNFormat": "arn:aws:elasticloadbalancing:${Region}:${Account}:${ResourceType}/${ResourceId}",
+            "ARNRegex": "^arn:aws:elasticloadbalancing:.+",
+            "Actions": [
+                "AddListenerCertificates",
+                "AddTags",
+                "CreateListener",
+                "CreateLoadBalancer",
+                "CreateRule",
+                "CreateTargetGroup",
+                "DeleteListener",
+                "DeleteLoadBalancer",
+                "DeleteRule",
+                "DeleteTargetGroup",
+                "DeregisterTargets",
+                "DescribeAccountLimits",
+                "DescribeListenerCertificates",
+                "DescribeListeners",
+                "DescribeLoadBalancerAttributes",
+                "DescribeLoadBalancers",
+                "DescribeRules",
+                "DescribeSSLPolicies",
+                "DescribeTags",
+                "DescribeTargetGroupAttributes",
+                "DescribeTargetGroups",
+                "DescribeTargetHealth",
+                "ModifyListener",
+                "ModifyLoadBalancerAttributes",
+                "ModifyRule",
+                "ModifyTargetGroup",
+                "ModifyTargetGroupAttributes",
+                "RegisterTargets",
+                "RemoveListenerCertificates",
+                "RemoveTags",
+                "SetIpAddressType",
+                "SetRulePriorities",
+                "SetSecurityGroups",
+                "SetSubnets",
+                "SetWebAcl"
+            ],
+            "HasResource": true,
+            "StringPrefix": "elasticloadbalancing",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "elasticloadbalancing:CreateAction",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ]
+        },
         "AWS Elemental Appliances and Software": {
             "ARNFormat": "arn:aws:elemental-appliances-software:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:elemental-appliances-software:.+:.+:.+",
             "Actions": [
                 "CompleteUpload",
                 "CreateOrderV1",
                 "CreateQuote",
@@ -10524,15 +10574,14 @@
                 "TagResource",
                 "TestFunction",
                 "UntagResource",
                 "UpdateCachePolicy",
                 "UpdateCloudFrontOriginAccessIdentity",
                 "UpdateContinuousDeploymentPolicy",
                 "UpdateDistribution",
-                "UpdateDistributionWithStagingConfig",
                 "UpdateFieldLevelEncryptionConfig",
                 "UpdateFieldLevelEncryptionProfile",
                 "UpdateFunction",
                 "UpdateKeyGroup",
                 "UpdateOriginAccessControl",
                 "UpdateOriginRequestPolicy",
                 "UpdatePublicKey",
@@ -11615,49 +11664,60 @@
             ]
         },
         "Amazon Connect Customer Profiles": {
             "ARNFormat": "arn:aws:profile:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:profile:.+:.+:.+",
             "Actions": [
                 "AddProfileKey",
+                "CreateCalculatedAttributeDefinition",
                 "CreateDomain",
+                "CreateEventStream",
                 "CreateIntegrationWorkflow",
                 "CreateProfile",
+                "DeleteCalculatedAttributeDefinition",
                 "DeleteDomain",
+                "DeleteEventStream",
                 "DeleteIntegration",
                 "DeleteProfile",
                 "DeleteProfileKey",
                 "DeleteProfileObject",
                 "DeleteProfileObjectType",
                 "DeleteWorkflow",
                 "GetAutoMergingPreview",
+                "GetCalculatedAttributeDefinition",
+                "GetCalculatedAttributeForProfile",
                 "GetDomain",
+                "GetEventStream",
                 "GetIdentityResolutionJob",
                 "GetIntegration",
                 "GetMatches",
                 "GetProfileObjectType",
                 "GetProfileObjectTypeTemplate",
                 "GetWorkflow",
                 "GetWorkflowSteps",
                 "ListAccountIntegrations",
+                "ListCalculatedAttributeDefinitions",
+                "ListCalculatedAttributesForProfile",
                 "ListDomains",
+                "ListEventStreams",
                 "ListIdentityResolutionJobs",
                 "ListIntegrations",
                 "ListProfileObjectTypeTemplates",
                 "ListProfileObjectTypes",
                 "ListProfileObjects",
                 "ListTagsForResource",
                 "ListWorkflows",
                 "MergeProfiles",
                 "PutIntegration",
                 "PutProfileObject",
                 "PutProfileObjectType",
                 "SearchProfiles",
                 "TagResource",
                 "UntagResource",
+                "UpdateCalculatedAttributeDefinition",
                 "UpdateDomain",
                 "UpdateProfile"
             ],
             "HasResource": true,
             "StringPrefix": "profile",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
@@ -18301,28 +18361,31 @@
             ]
         },
         "Amazon SQS": {
             "ARNFormat": "arn:aws:sqs:${Region}:${Account}:${QueueName}",
             "ARNRegex": "^arn:aws:sqs:.+",
             "Actions": [
                 "AddPermission",
+                "CancelMessageMoveTask",
                 "ChangeMessageVisibility",
                 "CreateQueue",
                 "DeleteMessage",
                 "DeleteQueue",
                 "GetQueueAttributes",
                 "GetQueueUrl",
                 "ListDeadLetterSourceQueues",
+                "ListMessageMoveTasks",
                 "ListQueueTags",
                 "ListQueues",
                 "PurgeQueue",
                 "ReceiveMessage",
                 "RemovePermission",
                 "SendMessage",
                 "SetQueueAttributes",
+                "StartMessageMoveTask",
                 "TagQueue",
                 "UntagQueue"
             ],
             "HasResource": true,
             "StringPrefix": "sqs",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
@@ -19750,63 +19813,14 @@
                 "UpdateFavoriteQuery",
                 "UpdateQueryHistory",
                 "UpdateTab"
             ],
             "HasResource": false,
             "StringPrefix": "dbqms"
         },
-        "Elastic Load Balancing V2": {
-            "ARNFormat": "arn:aws:elasticloadbalancing:${Region}:${Account}:${ResourceType}/${ResourceId}",
-            "ARNRegex": "^arn:aws:elasticloadbalancing:.+",
-            "Actions": [
-                "AddListenerCertificates",
-                "AddTags",
-                "CreateListener",
-                "CreateLoadBalancer",
-                "CreateRule",
-                "CreateTargetGroup",
-                "DeleteListener",
-                "DeleteLoadBalancer",
-                "DeleteRule",
-                "DeleteTargetGroup",
-                "DeregisterTargets",
-                "DescribeAccountLimits",
-                "DescribeListenerCertificates",
-                "DescribeListeners",
-                "DescribeLoadBalancerAttributes",
-                "DescribeLoadBalancers",
-                "DescribeRules",
-                "DescribeSSLPolicies",
-                "DescribeTags",
-                "DescribeTargetGroupAttributes",
-                "DescribeTargetGroups",
-                "DescribeTargetHealth",
-                "ModifyListener",
-                "ModifyLoadBalancerAttributes",
-                "ModifyRule",
-                "ModifyTargetGroup",
-                "ModifyTargetGroupAttributes",
-                "RegisterTargets",
-                "RemoveListenerCertificates",
-                "RemoveTags",
-                "SetIpAddressType",
-                "SetRulePriorities",
-                "SetSecurityGroups",
-                "SetSubnets",
-                "SetWebAcl"
-            ],
-            "HasResource": true,
-            "StringPrefix": "elasticloadbalancing",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "elasticloadbalancing:ResourceTag/${TagKey}"
-            ]
-        },
         "High-volume outbound communications": {
             "ARNFormat": "arn:aws:connect-campaigns:${Region}:${Account}:campaign/${CampaignId}",
             "ARNRegex": "^arn:aws:connect-campaigns:.+:.*:campaign/.*",
             "Actions": [
                 "CreateCampaign",
                 "DeleteCampaign",
                 "DeleteConnectInstanceConfig",
```

### Comparing `iam_actions-1.2.20230608/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230609/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230608/iam_actions/services.json` & `iam_actions-1.2.20230609/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998784623803224%*

 * *Differences: {"'cloudfront'": "{'Actions': {delete: [100]}}",*

 * * "'elasticloadbalancing'": "{'ServiceNames': {insert: [(1, 'AWS Elastic Load Balancing V2')], "*

 * *                           'delete: [1]}}',*

 * * "'profile'": "{'Actions': {insert: [(1, 'CreateCalculatedAttributeDefinition'), (3, "*

 * *              "'CreateEventStream'), (6, 'DeleteCalculatedAttributeDefinition'), (8, "*

 * *              "'DeleteEventStream'), (16, 'GetCalculatedAttributeDefinition'), (17, "*

 * *              "'GetCalculatedAttributeForProfile'), (19, 'GetEv […]*

```diff
@@ -3059,15 +3059,14 @@
             "TagResource",
             "TestFunction",
             "UntagResource",
             "UpdateCachePolicy",
             "UpdateCloudFrontOriginAccessIdentity",
             "UpdateContinuousDeploymentPolicy",
             "UpdateDistribution",
-            "UpdateDistributionWithStagingConfig",
             "UpdateFieldLevelEncryptionConfig",
             "UpdateFieldLevelEncryptionProfile",
             "UpdateFunction",
             "UpdateKeyGroup",
             "UpdateOriginAccessControl",
             "UpdateOriginRequestPolicy",
             "UpdatePublicKey",
@@ -7638,15 +7637,15 @@
             "elasticloadbalancing:CreateAction",
             "elasticloadbalancing:ResourceTag/",
             "elasticloadbalancing:ResourceTag/${TagKey}"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Elastic Load Balancing",
-            "Elastic Load Balancing V2"
+            "AWS Elastic Load Balancing V2"
         ]
     },
     "elasticmapreduce": {
         "ARNFormats": [
             "arn:aws:elasticmapreduce:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
@@ -15165,49 +15164,60 @@
             "arn:aws:profile:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:profile:.+:.+:.+"
         ],
         "Actions": [
             "AddProfileKey",
+            "CreateCalculatedAttributeDefinition",
             "CreateDomain",
+            "CreateEventStream",
             "CreateIntegrationWorkflow",
             "CreateProfile",
+            "DeleteCalculatedAttributeDefinition",
             "DeleteDomain",
+            "DeleteEventStream",
             "DeleteIntegration",
             "DeleteProfile",
             "DeleteProfileKey",
             "DeleteProfileObject",
             "DeleteProfileObjectType",
             "DeleteWorkflow",
             "GetAutoMergingPreview",
+            "GetCalculatedAttributeDefinition",
+            "GetCalculatedAttributeForProfile",
             "GetDomain",
+            "GetEventStream",
             "GetIdentityResolutionJob",
             "GetIntegration",
             "GetMatches",
             "GetProfileObjectType",
             "GetProfileObjectTypeTemplate",
             "GetWorkflow",
             "GetWorkflowSteps",
             "ListAccountIntegrations",
+            "ListCalculatedAttributeDefinitions",
+            "ListCalculatedAttributesForProfile",
             "ListDomains",
+            "ListEventStreams",
             "ListIdentityResolutionJobs",
             "ListIntegrations",
             "ListProfileObjectTypeTemplates",
             "ListProfileObjectTypes",
             "ListProfileObjects",
             "ListTagsForResource",
             "ListWorkflows",
             "MergeProfiles",
             "PutIntegration",
             "PutProfileObject",
             "PutProfileObjectType",
             "SearchProfiles",
             "TagResource",
             "UntagResource",
+            "UpdateCalculatedAttributeDefinition",
             "UpdateDomain",
             "UpdateProfile"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
@@ -19059,28 +19069,31 @@
             "arn:aws:sqs:${Region}:${Account}:${QueueName}"
         ],
         "ARNRegexes": [
             "^arn:aws:sqs:.+"
         ],
         "Actions": [
             "AddPermission",
+            "CancelMessageMoveTask",
             "ChangeMessageVisibility",
             "CreateQueue",
             "DeleteMessage",
             "DeleteQueue",
             "GetQueueAttributes",
             "GetQueueUrl",
             "ListDeadLetterSourceQueues",
+            "ListMessageMoveTasks",
             "ListQueueTags",
             "ListQueues",
             "PurgeQueue",
             "ReceiveMessage",
             "RemovePermission",
             "SendMessage",
             "SetQueueAttributes",
+            "StartMessageMoveTask",
             "TagQueue",
             "UntagQueue"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20230608/pyproject.toml` & `iam_actions-1.2.20230609/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230608"
+version = "1.2.20230609"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230608/setup.py` & `iam_actions-1.2.20230609/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230608',
+    'version': '1.2.20230609',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230608/PKG-INFO` & `iam_actions-1.2.20230609/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230608
+Version: 1.2.20230609
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

