# Comparing `tmp/strongmind_deployment-1.0.5-py3-none-any.whl.zip` & `tmp/strongmind_deployment-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7604 bytes, number of entries: 8
+Zip file size: 7589 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx    11483 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx    11395 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
 -rw-r--r--  2.0 unx     7116 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
 -rw-r--r--  2.0 unx     1126 b- defN 20-Feb-02 00:00 strongmind_deployment/redis.py
-?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      711 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.5.dist-info/RECORD
-8 files, 22251 bytes uncompressed, 6346 bytes compressed:  71.5%
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      711 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.7.dist-info/RECORD
+8 files, 22163 bytes uncompressed, 6331 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
 Filename: strongmind_deployment/redis.py
 Comment: 
 
-Filename: strongmind_deployment-1.0.5.dist-info/METADATA
+Filename: strongmind_deployment-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-1.0.5.dist-info/WHEEL
+Filename: strongmind_deployment-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-1.0.5.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-1.0.7.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-1.0.5.dist-info/RECORD
+Filename: strongmind_deployment-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -70,14 +70,15 @@
         port_mappings = None
         if self.target_group is not None:
             port_mappings = [awsx.ecs.TaskDefinitionPortMappingArgs(
                     container_port=self.container_port,
                     host_port=self.container_port,
                     target_group=self.target_group,
                 )]
+
         execution_role = aws.iam.Role(
             f"{project_stack}-exec-role",
             name=f"{project_stack}-exec-role",
             assume_role_policy=json.dumps(
                 {
                     "Version": "2008-10-17",
                     "Statement": [
@@ -127,16 +128,14 @@
             ),
             opts=pulumi.ResourceOptions(parent=self),
         )
 
         task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
             skip_destroy=True,
             family=project_stack,
-            execution_role=execution_role.arn,
-            task_role=execution_role.arn,
             container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
                 name=project_stack,
                 log_configuration=awsx.ecs.TaskDefinitionLogConfigurationArgs(
                     log_driver="awslogs",
                     options={
                         "awslogs-group": logs.name,
                         "awslogs-region": "us-west-2",
```

## Comparing `strongmind_deployment-1.0.5.dist-info/METADATA` & `strongmind_deployment-1.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 1.0.5
+Version: 1.0.7
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-1.0.5.dist-info/licenses/LICENSE` & `strongmind_deployment-1.0.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-1.0.5.dist-info/RECORD` & `strongmind_deployment-1.0.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-strongmind_deployment/container.py,sha256=64jFhr3uA1K6w7_-q2vtOYduqCO4PDxHw4O50odnjb8,11483
+strongmind_deployment/container.py,sha256=Ybz6zLM2lU-DHFQSGJ0vyxeYmegJtb_dNkIkH_HqocI,11395
 strongmind_deployment/rails.py,sha256=FSUHNG2j7_0EFnSgJUN9_ZBsFaiEq7dQ_zBUIzpyvg8,7116
 strongmind_deployment/redis.py,sha256=pYiSCRBQtO9TU69KVt0GrmJyB_GhGEz_hQUucw9vBUA,1126
-strongmind_deployment-1.0.5.dist-info/METADATA,sha256=LwmFmQOv4k1fLw4vDg2LazziUqwnQfh0WQZZFbYKcII,675
-strongmind_deployment-1.0.5.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
-strongmind_deployment-1.0.5.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-1.0.5.dist-info/RECORD,,
+strongmind_deployment-1.0.7.dist-info/METADATA,sha256=703r08OJoXBKi5jJTzRWMakhQmT23huaJg4j0oRff98,675
+strongmind_deployment-1.0.7.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
+strongmind_deployment-1.0.7.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-1.0.7.dist-info/RECORD,,
```

