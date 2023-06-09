# Comparing `tmp/cloudq-1.1.1-py3-none-any.whl.zip` & `tmp/cloudq-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,51 @@
-Zip file size: 60147 bytes, number of entries: 36
--rw-r--r--  2.0 unx      737 b- defN 22-Jul-04 06:43 cloudq/__init__.py
--rw-r--r--  2.0 unx    19533 b- defN 22-Jul-04 06:43 cloudq/abci.py
--rw-r--r--  2.0 unx    24696 b- defN 22-Jul-04 06:43 cloudq/agent.py
--rw-r--r--  2.0 unx     2878 b- defN 22-Jul-04 06:43 cloudq/base.py
--rw-r--r--  2.0 unx    27406 b- defN 22-Jul-04 06:43 cloudq/client.py
--rw-r--r--  2.0 unx     6663 b- defN 22-Jul-04 06:43 cloudq/common.py
--rw-r--r--  2.0 unx     4543 b- defN 22-Jul-04 06:43 cloudq/interface.py
--rw-r--r--  2.0 unx    17980 b- defN 22-Jul-04 06:43 cloudq/slurm.py
--rw-r--r--  2.0 unx      707 b- defN 22-Jul-04 06:43 cloudq/aws/__init__.py
--rw-r--r--  2.0 unx    13009 b- defN 22-Jul-04 06:43 cloudq/aws/cloudqaws.py
--rw-r--r--  2.0 unx    20661 b- defN 22-Jul-04 06:43 cloudq/aws/utils.py
--rw-r--r--  2.0 unx     3071 b- defN 22-Jul-04 06:43 cloudq/aws/data/add_log.py
--rw-r--r--  2.0 unx      924 b- defN 22-Jul-04 06:43 cloudq/aws/data/autoexec.sh
--rw-r--r--  2.0 unx     5124 b- defN 22-Jul-04 06:43 cloudq/aws/data/cloud-stack.yaml
--rw-r--r--  2.0 unx      247 b- defN 22-Jul-04 06:43 cloudq/aws/data/cloudq.service
--rw-r--r--  2.0 unx      866 b- defN 22-Jul-04 06:43 cloudq/aws/data/cluster-config.yaml
--rw-r--r--  2.0 unx       36 b- defN 22-Jul-04 06:43 cloudq/aws/data/config.ini
--rw-r--r--  2.0 unx     9636 b- defN 22-Jul-04 06:43 cloudq/aws/data/iam-user-policy.json
--rw-r--r--  2.0 unx     1126 b- defN 22-Jul-04 06:43 cloudq/aws/data/on-compute-node-start.sh
--rw-r--r--  2.0 unx     2304 b- defN 22-Jul-04 06:43 cloudq/aws/data/on-head-node-start.sh
--rw-r--r--  2.0 unx      278 b- defN 22-Jul-04 06:43 cloudq/data/config.ini
--rw-r--r--  2.0 unx      546 b- defN 22-Jul-04 06:43 cloudq/data/job_manifest.json
--rw-r--r--  2.0 unx       33 b- defN 22-Jul-04 06:43 cloudq/data/project.ini
--rw-r--r--  2.0 unx       35 b- defN 22-Jul-04 06:43 cloudq/data/resource.ini
--rw-r--r--  2.0 unx     1908 b- defN 22-Jul-04 06:43 cloudq/example/ljob_array.abci.sh
--rw-r--r--  2.0 unx     1432 b- defN 22-Jul-04 06:43 cloudq/example/ljob_pt_mnist.abci.sh
--rw-r--r--  2.0 unx     1464 b- defN 22-Jul-04 06:43 cloudq/example/ljob_tf_mnist.abci.sh
--rw-r--r--  2.0 unx     1704 b- defN 22-Jul-04 06:43 cloudq/example/mjob_array.sh
--rw-r--r--  2.0 unx     1292 b- defN 22-Jul-04 06:43 cloudq/example/mjob_pt_mnist.sh
--rw-r--r--  2.0 unx     1321 b- defN 22-Jul-04 06:43 cloudq/example/mjob_tf_mnist.sh
--rw-r--r--  2.0 unx    11358 b- defN 22-Jul-04 06:54 cloudq-1.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    12678 b- defN 22-Jul-04 06:54 cloudq-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-04 06:54 cloudq-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      115 b- defN 22-Jul-04 06:54 cloudq-1.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 22-Jul-04 06:54 cloudq-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2957 b- defN 22-Jul-04 06:54 cloudq-1.1.1.dist-info/RECORD
-36 files, 199367 bytes uncompressed, 55449 bytes compressed:  72.2%
+Zip file size: 73541 bytes, number of entries: 49
+-rw-r--r--  2.0 unx      742 b- defN 23-Jun-09 06:52 cloudq/__init__.py
+-rw-r--r--  2.0 unx    20269 b- defN 23-Jun-09 06:52 cloudq/abci.py
+-rw-r--r--  2.0 unx    27475 b- defN 23-Jun-09 06:52 cloudq/agent.py
+-rw-r--r--  2.0 unx     2883 b- defN 23-Jun-09 06:52 cloudq/base.py
+-rw-r--r--  2.0 unx    29585 b- defN 23-Jun-09 06:52 cloudq/client.py
+-rw-r--r--  2.0 unx     6668 b- defN 23-Jun-09 06:52 cloudq/common.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-Jun-09 06:52 cloudq/interface.py
+-rw-r--r--  2.0 unx    18753 b- defN 23-Jun-09 06:52 cloudq/slurm.py
+-rw-r--r--  2.0 unx      712 b- defN 23-Jun-09 06:52 cloudq/aws/__init__.py
+-rw-r--r--  2.0 unx    17744 b- defN 23-Jun-09 06:52 cloudq/aws/cloudqaws.py
+-rw-r--r--  2.0 unx    22715 b- defN 23-Jun-09 06:52 cloudq/aws/utils.py
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-09 06:52 cloudq/aws/data/config.ini
+-rw-r--r--  2.0 unx     3076 b- defN 23-Jun-09 06:52 cloudq/aws/data/default/add_log.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Jun-09 06:52 cloudq/aws/data/default/autoexec.sh
+-rw-r--r--  2.0 unx     5124 b- defN 23-Jun-09 06:52 cloudq/aws/data/default/cloud-stack.yaml
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-09 06:52 cloudq/aws/data/default/cloudq.service
+-rw-r--r--  2.0 unx      866 b- defN 23-Jun-09 06:52 cloudq/aws/data/default/cluster-config.yaml
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jun-09 06:52 cloudq/aws/data/default/on-compute-node-start.sh
+-rw-r--r--  2.0 unx     2309 b- defN 23-Jun-09 06:52 cloudq/aws/data/default/on-head-node-start.sh
+-rw-r--r--  2.0 unx     3076 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-docker/add_log.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-docker/autoexec.sh
+-rw-r--r--  2.0 unx     5124 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-docker/cloud-stack.yaml
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-docker/cloudq.service
+-rw-r--r--  2.0 unx      866 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-docker/cluster-config.yaml
+-rw-r--r--  2.0 unx     1893 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-docker/on-compute-node-start.sh
+-rw-r--r--  2.0 unx     2309 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-docker/on-head-node-start.sh
+-rw-r--r--  2.0 unx     3076 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-gpu/add_log.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-gpu/autoexec.sh
+-rw-r--r--  2.0 unx     5124 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-gpu/cloud-stack.yaml
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-gpu/cloudq.service
+-rw-r--r--  2.0 unx      872 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-gpu/cluster-config.yaml
+-rw-r--r--  2.0 unx     2612 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-gpu/on-compute-node-start.sh
+-rw-r--r--  2.0 unx     2309 b- defN 23-Jun-09 06:52 cloudq/aws/example/enable-gpu/on-head-node-start.sh
+-rw-r--r--  2.0 unx      296 b- defN 23-Jun-09 06:52 cloudq/data/config.ini
+-rw-r--r--  2.0 unx      546 b- defN 23-Jun-09 06:52 cloudq/data/job_manifest.json
+-rw-r--r--  2.0 unx       33 b- defN 23-Jun-09 06:52 cloudq/data/project.ini
+-rw-r--r--  2.0 unx       35 b- defN 23-Jun-09 06:52 cloudq/data/resource.ini
+-rw-r--r--  2.0 unx     1947 b- defN 23-Jun-09 06:52 cloudq/example/ljob_array.abci.sh
+-rw-r--r--  2.0 unx     1471 b- defN 23-Jun-09 06:52 cloudq/example/ljob_pt_mnist.abci.sh
+-rw-r--r--  2.0 unx     1469 b- defN 23-Jun-09 06:52 cloudq/example/ljob_tf_mnist.abci.sh
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jun-09 06:52 cloudq/example/mjob_array.sh
+-rw-r--r--  2.0 unx     1331 b- defN 23-Jun-09 06:52 cloudq/example/mjob_pt_mnist.sh
+-rw-r--r--  2.0 unx     1326 b- defN 23-Jun-09 06:52 cloudq/example/mjob_tf_mnist.sh
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jun-09 07:05 cloudq-1.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    10203 b- defN 23-Jun-09 07:05 cloudq-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 07:05 cloudq-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-09 07:05 cloudq-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-09 07:05 cloudq-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4383 b- defN 23-Jun-09 07:05 cloudq-1.2.0.dist-info/RECORD
+49 files, 231797 bytes uncompressed, 66473 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -27,39 +27,78 @@
 
 Filename: cloudq/aws/cloudqaws.py
 Comment: 
 
 Filename: cloudq/aws/utils.py
 Comment: 
 
-Filename: cloudq/aws/data/add_log.py
+Filename: cloudq/aws/data/config.ini
 Comment: 
 
-Filename: cloudq/aws/data/autoexec.sh
+Filename: cloudq/aws/data/default/add_log.py
 Comment: 
 
-Filename: cloudq/aws/data/cloud-stack.yaml
+Filename: cloudq/aws/data/default/autoexec.sh
 Comment: 
 
-Filename: cloudq/aws/data/cloudq.service
+Filename: cloudq/aws/data/default/cloud-stack.yaml
 Comment: 
 
-Filename: cloudq/aws/data/cluster-config.yaml
+Filename: cloudq/aws/data/default/cloudq.service
 Comment: 
 
-Filename: cloudq/aws/data/config.ini
+Filename: cloudq/aws/data/default/cluster-config.yaml
+Comment: 
+
+Filename: cloudq/aws/data/default/on-compute-node-start.sh
+Comment: 
+
+Filename: cloudq/aws/data/default/on-head-node-start.sh
+Comment: 
+
+Filename: cloudq/aws/example/enable-docker/add_log.py
+Comment: 
+
+Filename: cloudq/aws/example/enable-docker/autoexec.sh
+Comment: 
+
+Filename: cloudq/aws/example/enable-docker/cloud-stack.yaml
+Comment: 
+
+Filename: cloudq/aws/example/enable-docker/cloudq.service
+Comment: 
+
+Filename: cloudq/aws/example/enable-docker/cluster-config.yaml
+Comment: 
+
+Filename: cloudq/aws/example/enable-docker/on-compute-node-start.sh
+Comment: 
+
+Filename: cloudq/aws/example/enable-docker/on-head-node-start.sh
+Comment: 
+
+Filename: cloudq/aws/example/enable-gpu/add_log.py
+Comment: 
+
+Filename: cloudq/aws/example/enable-gpu/autoexec.sh
+Comment: 
+
+Filename: cloudq/aws/example/enable-gpu/cloud-stack.yaml
+Comment: 
+
+Filename: cloudq/aws/example/enable-gpu/cloudq.service
 Comment: 
 
-Filename: cloudq/aws/data/iam-user-policy.json
+Filename: cloudq/aws/example/enable-gpu/cluster-config.yaml
 Comment: 
 
-Filename: cloudq/aws/data/on-compute-node-start.sh
+Filename: cloudq/aws/example/enable-gpu/on-compute-node-start.sh
 Comment: 
 
-Filename: cloudq/aws/data/on-head-node-start.sh
+Filename: cloudq/aws/example/enable-gpu/on-head-node-start.sh
 Comment: 
 
 Filename: cloudq/data/config.ini
 Comment: 
 
 Filename: cloudq/data/job_manifest.json
 Comment: 
@@ -84,26 +123,26 @@
 
 Filename: cloudq/example/mjob_pt_mnist.sh
 Comment: 
 
 Filename: cloudq/example/mjob_tf_mnist.sh
 Comment: 
 
-Filename: cloudq-1.1.1.dist-info/LICENSE.txt
+Filename: cloudq-1.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cloudq-1.1.1.dist-info/METADATA
+Filename: cloudq-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cloudq-1.1.1.dist-info/WHEEL
+Filename: cloudq-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cloudq-1.1.1.dist-info/entry_points.txt
+Filename: cloudq-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudq-1.1.1.dist-info/top_level.txt
+Filename: cloudq-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudq-1.1.1.dist-info/RECORD
+Filename: cloudq-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudq/__init__.py

```diff
@@ -1,18 +1,18 @@
 # cloudq: cloud storage-based meta scheduler
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '1.1.1'
+__version__ = '1.2.0'
```

## cloudq/abci.py

```diff
@@ -1,10 +1,10 @@
 # abci: cloudq agent for ABCI
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -74,16 +74,16 @@
 export ARY_TASK_ID=$SGE_TASK_ID\n\
 export ARY_TASK_FIRST=$SGE_TASK_FIRST\n\
 export ARY_TASK_LAST=$SGE_TASK_LAST\n\
 export ARY_TASK_STEPSIZE=$SGE_TASK_STEPSIZE\n\
 export TMPDIR=$SGE_LOCALDIR\n\
 \n\
 source /etc/profile.d/modules.sh\n\
-module load singularitypro/3.7\n\
-module load aws-cli/2.1\n\
+module load singularitypro/3.9\n\
+module load aws-cli/2.11\n\
 \n\
 cq_container_run() {{\n\
     singularity exec --nv $@\n\
 }}\n\
 abci_cs_cp() {{\n\
     SRC=$1\n\
     DST=$2\n\
@@ -150,14 +150,15 @@
 
         Args:
             manifest (dict): a job manifest.
         Returns:
             dict: a job manifest added local parameters.
         '''
         logger.debug('submit_job start. UUID={}'.format(manifest[MANIFEST_PARAMS.UUID.value]))
+        logger.info('submit job (abci): start. UUID={}'.format(manifest[MANIFEST_PARAMS.UUID.value]))
         if MANIFEST_PARAMS.LOCAL_NAME.value in manifest:
             name = manifest[MANIFEST_PARAMS.LOCAL_NAME.value]
         else:
             name = manifest[MANIFEST_PARAMS.NAME.value]
         submit_cmd = ['qsub', name]
 
         if LOCAL_MANIFEST_PARAMS.LOCAL_SUBMIT_OPT.value in manifest:
@@ -191,41 +192,44 @@
             manifest[MANIFEST_PARAMS.JOB_ID.value] = job_id
             self.jobid_list.append(job_id)
         else:
             logger.info(err.decode())
             manifest[MANIFEST_PARAMS.ERROR_MSG.value] = err.decode()
         logger.debug('submit_job ended. UUID={} JobID={}'.format(
             manifest[MANIFEST_PARAMS.UUID.value], manifest[MANIFEST_PARAMS.JOB_ID.value]))
+        logger.info('submit job (abci): succeeded. UUID={} JobID={}'.format(
+            manifest[MANIFEST_PARAMS.UUID.value], manifest[MANIFEST_PARAMS.JOB_ID.value]))
         return manifest
 
     def get_jobs_status(self) -> dict:
         '''It returns job status list.
 
         Returns:
             list: job status list.
         '''
         logger.debug('get_jobs_status start.')
+        logger.info('stat job (abci): start.')
         jobs = []
         cmd = ['qstat']
         logger.debug('Run get job status command: {}'.format(' '.join(cmd)))
         proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (out, err) = proc.communicate()
         out = out.decode().splitlines()
         if out == []:
             logger.debug('get_jobs_status ended. {} jobs'.format(len(jobs)))
             return jobs
 
-        list = []
+        list_ = []
         for line in out:
             result = re.match(PATTERN_STAT_ABCI, line)
             if not result:
                 continue
 
             jobid = result.group(1)
-            list.append(jobid)
+            list_.append(jobid)
             qst = result.group(5)
             state = ''
             if qst == 'r':
                 state = JOB_STATE.RUN.value
             elif qst == 'qw':
                 state = JOB_STATE.READY.value
             elif qst == 'E':
@@ -234,18 +238,18 @@
                 state = JOB_STATE.DELETING.value
 
             if state != '':
                 logger.debug('  jobid:{}, state:{}'.format(jobid, state))
                 jobs.append((jobid, state))
 
         logger.debug('self.jobid_list: {}'.format(self.jobid_list))
-        logger.debug('list: {}'.format(list))
+        logger.debug('list: {}'.format(list_))
         for submitted_jobid in self.jobid_list:
             # Get the status of completed jobs
-            if submitted_jobid in list:
+            if submitted_jobid in list_:
                 continue
 
             check_stat_cmd = ['qacct', '-j', submitted_jobid]
             logger.debug('Run check timeout and deleted command: {}'.format(
                 ' '.join(check_stat_cmd)))
             proc = subprocess.Popen(check_stat_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             (out, err) = proc.communicate()
@@ -267,38 +271,43 @@
                     state = JOB_STATE.DELETED.value
                 else:
                     state = ''
                 logger.debug('  jobid:{}, state:{}'.format(submitted_jobid, state))
                 jobs.append((submitted_jobid, state))
 
         logger.debug('get_jobs_status ended. {} jobs'.format(len(jobs)))
+        logger.info('stat job (abci): succeeded. {} jobs'.format(len(jobs)))
         return jobs
 
     def cancel_job(self, manifest: dict, force: bool) -> dict:
         '''It cancels a job.
 
         Args:
             manifest (dict): a job manifest.
             force (bool): If true, the job cancels forcibly.
         Returns:
             dict: a job manifest.
         '''
         logger.debug('cancel_job start. UUID={} JobID={}'.format(
             manifest[MANIFEST_PARAMS.UUID.value], manifest[MANIFEST_PARAMS.JOB_ID.value]))
+        logger.info('cancel job (abci): start. UUID={} JobID={}'.format(
+            manifest[MANIFEST_PARAMS.UUID.value], manifest[MANIFEST_PARAMS.JOB_ID.value]))
         if force:
             cancel_cmd = ['qdel', '-f', manifest[MANIFEST_PARAMS.JOB_ID.value]]
         else:
             cancel_cmd = ['qdel', manifest[MANIFEST_PARAMS.JOB_ID.value]]
 
         logger.debug('Run cancel command: {}'.format(' '.join(cancel_cmd)))
         proc = subprocess.Popen(cancel_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (out, err) = proc.communicate()
         logger.info(out.decode())
         logger.debug('cancel_job ended. UUID={} JobID={}'.format(
             manifest[MANIFEST_PARAMS.UUID.value], manifest[MANIFEST_PARAMS.JOB_ID.value]))
+        logger.info('cancel job (abci): succeeded. UUID={} JobID={}'.format(
+            manifest[MANIFEST_PARAMS.UUID.value], manifest[MANIFEST_PARAMS.JOB_ID.value]))
         return manifest
 
     def get_job_log(self, manifest: dict, error: bool) -> dict:
         '''It saves a job log.
 
         Args:
             manifest (dict): a job manifest.
```

## cloudq/agent.py

```diff
@@ -1,10 +1,10 @@
 # agent: cloudq agent
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -25,15 +25,15 @@
 import shutil
 import subprocess
 import sys
 import time
 import traceback
 from enum import Enum
 import boto3
-from pathos.multiprocessing import ProcessingPool
+from concurrent.futures import ThreadPoolExecutor
 from .common import (get_manifest, put_manifest, current_time, iso_to_datetime,
                      is_exist_bucket_object, is_finished_job)
 from .common import (STAGEOUT_FILE, CANCEL_FILE, PROJECT_DEF_FILE,
                      RESOURCE_DEF_FILE, AGENT_LOG_PREFIX)
 from .common import JOB_STATE, MANIFEST_PARAMS, SCRIPT_TYPES
 from .interface import JobManagerAccessor
 from .interface import MetaJobScriptConverterAccessor
@@ -65,14 +65,16 @@
      'type': str, 'mandatory': True},
     {'section': 'default',  'key': 'aws_profile',
      'type': str, 'mandatory': True},
     {'section': 'default',  'key': 'cloudq_endpoint_url',
      'type': str, 'mandatory': True},
     {'section': 'default',  'key': 'cloudq_bucket',
      'type': str, 'mandatory': True},
+    {'section': 'default',  'key': 'log_level',
+     'type': str, 'mandatory': False,  'default': 'INFO'},
     {'section': 'agent',    'key': 'type',
      'type': str, 'mandatory': True},
     {'section': 'agent',    'key': 'num_procs',
      'type': int, 'mandatory': False,  'default': 8,    'min': 1},
     {'section': 'agent',    'key': 'daemon_interval',
      'type': int, 'mandatory': False,  'default': 5,    'min': 1},
     {'section': 'agent',    'key': 'cloudq_directory',
@@ -86,15 +88,15 @@
     ''' List of console messages.
     '''
 
     # success
     # SUBMIT_COMPLETED = 'Job ({}) {} has been submitted.'
 
     # information
-    META_JOB_CONVERTED = 'Meta job script'
+    META_JOB_CONVERTED = 'Meta job script {}'
     JOB_RECEIVED = 'submit job: job ({}) received.'
     JOB_SUBMITTED = 'submit job: job({}) is submitted. local-jobid:{}'
     JOB_SUBMISSION_FAILED = 'submit job: Failed to submit job ({})'
     JOB_UPDATED = 'stat job: job({}) is updated. status:{}'
     JOB_FINISHED = 'stat job: job ({}) is finished'
     JOB_ERROR_OCCURRED = 'stat job: Error occurred to job ({})'
     JOB_TIMEDOUT = 'stat job: job ({}) timed out'
@@ -126,61 +128,65 @@
 '''The object of job manager accessor.
 '''
 
 meta_job_converter = None
 '''The object of meta job script converter accessor.
 '''
 
-process_pool = None
-'''The object of process pool.
+thread_pool = None
+'''The object of thread pool.
 '''
 
 
 def submit_job(bucket: object, id_: str, manifest: dict) -> bool:
     '''It submits a job to the local scheduler.
 
     Args:
         bucket (S3.Bucket): A bucket where the job is stored.
         id_ (str): Job ID.
         manifest dict[str: obj]: A job manifest.
     Returns:
         bool: If the job is submitted, returns True.
     '''
     logger.debug('submit_job start. id:{}'.format(id_))
+    logger.info('submit job: start. id:{}'.format(id_))
     system_name = config['default']['name'].lower()
     if manifest[MANIFEST_PARAMS.SCRIPT_TYPE.value] == SCRIPT_TYPES.LOCAL.value:
         run_system = manifest[MANIFEST_PARAMS.SUBMIT_TO.value].lower()
         if run_system != system_name:
             logger.debug('submit_job ended. id:{}  (Other system\'s job.)'.format(id_))
+            logger.info('submit job: not processed. id:{}  (Other system\'s job.)'.format(id_))
             return False
 
     # check hold job.
     if MANIFEST_PARAMS.HOLD_JOB_ID.value in manifest:
         hold_jids = manifest[MANIFEST_PARAMS.HOLD_JOB_ID.value]
         if len(hold_jids) > 0:
-            logger.debug('check hold jods: {}'.format(hold_jids))
+            logger.info('submit job: check hold jods: {}'.format(hold_jids))
             for hold_jid in hold_jids.split(','):
                 hold_manifest = get_manifest(bucket, hold_jid.strip())
                 if hold_manifest:
                     if not is_finished_job(hold_manifest):
                         logstr = 'submit_job ended. id:{}  (Hold jod({}) is not finished.)'
                         logger.debug(logstr.format(id_, hold_jid))
+                        logstr = 'submit job: not processed. id:{}  (Hold jod({}) is not finished.)'
+                        logger.info(logstr.format(id_, hold_jid))
                         return False
-            logger.debug('hold jods are finished.')
+            logger.info('submit job: hold jods are finished.')
 
     try:
         manifest[MANIFEST_PARAMS.TIME_RECEIVE.value] = current_time()
         manifest[MANIFEST_PARAMS.RUN_SYSTEM.value] = system_name
 
         proc = subprocess.Popen('whoami', stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (out, err) = proc.communicate()
         manifest[MANIFEST_PARAMS.LOCAL_ACCOUNT.value] = out.decode().strip()
 
         name = manifest[MANIFEST_PARAMS.NAME.value]
-        logger.debug(MESSAGES.JOB_RECEIVED.value.format(id_))
+        logger.info(MESSAGES.JOB_RECEIVED.value.format(id_))
 
         workdir = os.path.join(cache_dir, id_)
         os.makedirs(workdir, exist_ok=True)
         os.chdir(workdir)
         manifest[MANIFEST_PARAMS.WORK_DIR.value] = workdir
 
         s3file = os.path.join(id_, name)
@@ -196,25 +202,26 @@
                 manifest, config['default']['cloudq_endpoint_url'],
                 config['default']['aws_profile'])
             if result:
                 manifest = result
             else:
                 remove_work_dir(manifest)
                 logger.debug('submit_job ended. id:{}  (Other system\'s job.)'.format(id_))
+                logger.info('submit job: not processed. id:{}  (Other system\'s job.)'.format(id_))
                 return False
             local_script = manifest[MANIFEST_PARAMS.LOCAL_NAME.value]
             s3file = os.path.join(id_, local_script)
             bucket.upload_file(local_script, s3file)
             logger.info(MESSAGES.META_JOB_CONVERTED.value.format(id_))
 
         manifest = job_manager.submit_job(manifest)
     except Exception as e:
         manifest[MANIFEST_PARAMS.ERROR_MSG.value] = str(e)
         logger.error('Error({}): {}\n\n'.format(id_, e))
-        logger.debug(traceback.format_exc())
+        logger.error(traceback.format_exc())
 
     if manifest[MANIFEST_PARAMS.JOB_ID.value]:
         logger.info(MESSAGES.JOB_SUBMITTED.value.format(
             id_, manifest[MANIFEST_PARAMS.JOB_ID.value]))
         manifest[MANIFEST_PARAMS.STATE.value] = JOB_STATE.READY.value
         manifest[MANIFEST_PARAMS.TIME_READY.value] = current_time()
     else:
@@ -280,14 +287,15 @@
 
     Args:
         bucket (S3.Bucket): A bucket where the job is stored.
         id_ (str): Job ID.
         manifest dict[str: obj]: A job manifest.
     '''
     logger.debug('stat_job start. id:{}'.format(id_))
+    logger.info('stat job: start. id:{}'.format(id_))
     jobs = job_manager.get_jobs_status()
 
     # update job's state
     for j in jobs:
         updated = False
         if j[0] != manifest[MANIFEST_PARAMS.JOB_ID.value]:
             continue
@@ -339,14 +347,15 @@
                     logger.info(MESSAGES.JOB_DELETED.value.format(id_))
                 if manifest[MANIFEST_PARAMS.STATE.value] == JOB_STATE.TIMEOUT.value:
                     logger.info(MESSAGES.JOB_TIMEDOUT.value.format(id_))
         elif manifest[MANIFEST_PARAMS.STATE.value] == JOB_STATE.RUN.value:
             upload_logs(bucket, manifest)
 
         logger.debug('stat_job ended. id:{}'.format(id_))
+        logger.info('stat job: succeeded. id:{}'.format(id_))
         return
 
     # job is already finished.
     if (manifest[MANIFEST_PARAMS.STATE.value] in
             (JOB_STATE.RUN.value, JOB_STATE.READY.value, JOB_STATE.DELETING.value,
              JOB_STATE.COMPLETING.value)):
         manifest[MANIFEST_PARAMS.TIME_SO_START.value] = current_time()
@@ -369,14 +378,15 @@
 
     Args:
         bucket (S3.Bucket): A bucket where the job is stored.
         id_ (str): Job ID.
         manifest dict[str: obj]: A job manifest.
     '''
     logger.debug('cancel_job start. id:{}'.format(id_))
+    logger.info('cancel job: start. id:{}'.format(id_))
 
     if manifest[MANIFEST_PARAMS.STATE.value] == JOB_STATE.INIT.value:
         manifest[MANIFEST_PARAMS.STATE.value] = JOB_STATE.DELETED.value
         manifest[MANIFEST_PARAMS.TIME_FINISH.value] = current_time()
         put_manifest(bucket, id_, manifest)
         remove_work_dir(manifest)
         logger.info(MESSAGES.JOB_FINISHED.value.format(id_))
@@ -388,25 +398,26 @@
     for job in jobs:
         if manifest[MANIFEST_PARAMS.JOB_ID.value] in job[0]:
             job_exists = True
             break
 
     if not job_exists:
         logger.debug('cancel_job ended (The job is already finished). id:{}'.format(id_))
+        logger.info('cancel job: not processed (The job is already finished). id:{}'.format(id_))
         return
 
     os.chdir(manifest[MANIFEST_PARAMS.WORK_DIR.value])
 
     s3file = os.path.join(id_, CANCEL_FILE)
     bucket.download_file(s3file, CANCEL_FILE)
     with open(CANCEL_FILE, 'r') as f:
         cancel_file_str = f.read()
 
     if len(cancel_file_str) > 0:
-        if (datetime.datetime.now() >=
+        if (datetime.datetime.now(datetime.timezone.utc) >=
                 iso_to_datetime(cancel_file_str) + datetime.timedelta(seconds=60)):
             logger.debug('cancel job (force): id:{}'.format(id_))
             manifest = job_manager.cancel_job(manifest, True)
             manifest[MANIFEST_PARAMS.STATE.value] = JOB_STATE.DONE.value
             logger.info(MESSAGES.JOB_FORCIBLY_CANCELED.value.format(id_))
             updated = True
         else:
@@ -424,25 +435,26 @@
         logger.info(MESSAGES.JOB_CANCELED.value.format(id_))
         updated = True
 
     if updated:
         put_manifest(bucket, id_, manifest)
 
     logger.debug('cancel_job ended. id:{}'.format(id_))
+    logger.info('cancel job: succeeded. id:{}'.format(id_))
 
 
 def remove_work_dir(manifest: dict) -> None:
     '''It removes a work directory.
 
     Args:
         manifest dict[str: obj]: A job manifest.
     '''
     work_dir = manifest[MANIFEST_PARAMS.WORK_DIR.value]
     if os.path.isdir(work_dir):
-        logger.debug('The working directory is removed:{}'.format(work_dir))
+        logger.info('The working directory is removed:{}'.format(work_dir))
         shutil.rmtree(work_dir)
 
 
 def checknrun() -> None:
     '''It process jobs in an object storage.
     '''
     logger.debug('checknrun start.')
@@ -455,51 +467,55 @@
             os.chdir(root_dir)
 
             _session = boto3.Session(profile_name=aws_profile)
             _s3 = _session.resource('s3', endpoint_url=endpoint_url)
             _bucket = _s3.Bucket(root_bucket)
             manifest = get_manifest(_bucket, jid)
             if manifest is None:
+                logger.info('[{}] manifest is None.'.format(jid))
                 return
             if MANIFEST_PARAMS.RUN_SYSTEM.value in manifest:
                 run_system = manifest[MANIFEST_PARAMS.RUN_SYSTEM.value]
                 if len(run_system) > 0 and run_system != config['default']['name']:
-                    logger.debug('[{}] processing by {}.'.format(jid, run_system))
+                    logger.info('[{}] processing by {}.'.format(jid, run_system))
                     return
             if is_finished_job(manifest):
-                logger.debug('[{}] already finished.'.format(jid))
+                logger.info('[{}] already finished.'.format(jid))
                 return
-            logger.debug('[{}] process start.'.format(jid))
+            logger.info('[{}] process start.'.format(jid))
             if (is_exist_bucket_object(_bucket, os.path.join(jid, CANCEL_FILE)) and
                     manifest[MANIFEST_PARAMS.STATE.value] != JOB_STATE.COMPLETING.value):
                 cancel_job(_bucket, jid, manifest)
             elif manifest[MANIFEST_PARAMS.STATE.value] == JOB_STATE.INIT.value:
                 if not submit_job(_bucket, jid, manifest):
                     skip_stat_job = True
 
             if 'skip_stat_job' not in locals():
                 stat_job(_bucket, jid, manifest)
-            logger.debug('[{}] process ended.'.format(jid))
+            logger.info('[{}] process succeeded.'.format(jid))
         except Exception as e:
             logger.error('Error ({}): {}\n\n'.format(jid, e))
-            logger.debug(traceback.format_exc())
+            logger.error(traceback.format_exc())
         upload_agent_log(config, _bucket)
 
     try:
         session = boto3.Session(profile_name=aws_profile)
         s3cli = session.client('s3', endpoint_url=endpoint_url)
         objs = s3cli.list_objects(Bucket=root_bucket, Delimiter='/')
         if not objs.get('CommonPrefixes'):
+            logger.info('Jids is None.')
             return
         jids = [obj.get('Prefix')[:-1] for obj in objs.get('CommonPrefixes')]
-        logger.debug('jids = {}'.format(jids))
-        process_pool.map(lambda jid: _process_job(jid), jids)
-    except Exception:
-        logger.error(sys.exc_info())
-        logger.debug(traceback.format_exc())
+        logger.info('jids = {}'.format(jids))
+        futures = thread_pool.map(lambda jid: _process_job(jid), jids)
+        for future in futures:
+            pass
+    except Exception as e:
+        logger.error('Error: {}\n\n'.format(e))
+        logger.error(traceback.format_exc())
     logger.debug('checknrun ended.')
 
 
 def upload_agent_log(config: configparser.ConfigParser, bucket: object) -> None:
     '''It uploads a agent logs to cloud storage.
 
     Args:
@@ -555,66 +571,116 @@
     cache_dir = os.path.join(root_dir, 'cache')
     try:
         os.makedirs(cache_dir, exist_ok=True)
     except Exception:
         raise Exception(MESSAGES.INVALID_CACHE_DIR_PATH.value.format(cache_dir))
 
 
-def init_logger() -> None:
+def show_config(config: configparser.ConfigParser) -> None:
+    '''It show configuration parameters.
+
+    Args:
+        config (configparser.ConfigParser): CloudQ CLI configuration.
+    '''
+    for param in CONFIG_PARAMS:
+        try:
+            logger.info('section={}, key={}, value={}'.format(
+                param['section'], param['key'],
+                config.get(param['section'], param['key'])
+            ))
+        except configparser.NoOptionError:
+            logger.info('section={}, key={}, value=None'.format(
+                param['section'], param['key']
+            ))
+
+
+def init_logger(args: argparse.Namespace, config: configparser.ConfigParser) -> None:
     '''It setups logger object.
     '''
     logfile = os.path.join(root_dir, LOG_FILE)
     if os.path.isfile(logfile):
         os.remove(logfile)
 
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setFormatter(logging.Formatter(LOG_STDOUT_FORMAT))
     file_handler = logging.FileHandler(filename=logfile)
     file_handler.setFormatter(logging.Formatter(LOG_FILE_FORMAT))
     handlers = [file_handler, stdout_handler]
     logging.basicConfig(handlers=handlers)
 
+    if args.log_level == 'INFO' or args.log_level == 'DEBUG':
+        log_level = args.log_level
+    else:
+        log_level = config['default']['log_level']
+
+    log_level = args.log_level
+    if not args.log_level:
+        log_level = logging.INFO
+
     global logger
     logger = logging.getLogger(PROCESS_NAME)
-    logger.setLevel(logging.INFO)
+    logger.setLevel(log_level)
+
+
+def create_default_config() -> str:
+    '''It creates default configuration files in home directory.
+
+    Returns:
+        str: configration file path.
+    '''
+    data_dir = os.path.expanduser('~/.cloudq/agent')
+    default_dir = os.path.join(os.path.dirname(__file__), 'data')
+    config_path = os.path.join(data_dir, CONFIG_FILE)
+
+    if not os.path.isdir(data_dir):
+        shutil.copytree(default_dir, data_dir)
+
+    if not os.path.isfile(config_path):
+        config_path = os.path.join(default_dir, CONFIG_FILE)
+
+    return config_path
 
 
 def main() -> None:
     '''the entry point.
     '''
-    global logger
     try:
-        data_dir = os.path.join(os.path.dirname(__file__), 'data')
-
-        if not os.path.isfile(os.path.join(data_dir, CONFIG_FILE)):
+        config_path = create_default_config()
+        if not os.path.isfile(config_path):
             raise Exception(MESSAGES.NO_CONFIG_FILE.value.format(CONFIG_FILE))
 
-        global config
-        config = configparser.ConfigParser()
-        config.read(os.path.join(data_dir, CONFIG_FILE), encoding=CONFIG_FILE_ENCODING)
-        _check_config(config)
-
-        init_logger()
-
         parser = argparse.ArgumentParser(add_help=True)
         parser.add_argument('--daemon', action='store_true', help='run daemon mode')
+        parser.add_argument('--log_level', help='specify log level. ')
         args = parser.parse_args()
 
+        global config
+        config = configparser.ConfigParser()
+        config.read(config_path, encoding=CONFIG_FILE_ENCODING)
+
+        _check_config(config)
+        init_logger(args, config)
+        logger.info('Agent start.')
+        logger.info('=================== config ====================')
+        show_config(config)
+        logger.info('===============================================')
+
         global job_manager
         job_manager = JobManagerAccessor(config['agent']['type'])
 
         global meta_job_converter
         meta_job_converter = MetaJobScriptConverterAccessor(config['agent']['type'])
         meta_job_converter.set_unique_name(config['default']['name'])
 
-        global process_pool
-        process_pool = ProcessingPool(nodes=int(config['agent']['num_procs']))
+        global thread_pool
+        thread_pool = ThreadPoolExecutor(max_workers=int(config['agent']['num_procs']))
 
         if not args.daemon:
             checknrun()
+            logger.info('Agent succeeded.')
             return
 
         # FIXME daemon mode
         run_interval = int(config['agent']['daemon_interval'])
         while True:
             checknrun()
             time.sleep(run_interval)
```

## cloudq/base.py

```diff
@@ -1,10 +1,10 @@
 # base: cloudq agent base
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## cloudq/client.py

```diff
@@ -1,10 +1,10 @@
 # client: cloudq client command line tool
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -21,14 +21,15 @@
 import logging
 import os
 import sys
 import tempfile
 import traceback
 import uuid
 from enum import Enum
+import shutil
 
 import boto3
 import botocore
 from pathos.multiprocessing import ProcessingPool
 
 from .common import put_manifest, get_manifest, current_time, time_iso_to_readable
 from .common import iso_to_datetime, is_finished_job, is_exist_bucket_object, combine_s3_path
@@ -60,14 +61,16 @@
      'type': str, 'mandatory': True},
     {'section': 'default',  'key': 'aws_profile',
      'type': str, 'mandatory': True},
     {'section': 'default',  'key': 'cloudq_endpoint_url',
      'type': str, 'mandatory': True},
     {'section': 'default',  'key': 'cloudq_bucket',
      'type': str, 'mandatory': True},
+    {'section': 'default',  'key': 'log_level',
+     'type': str, 'mandatory': False,  'default': 'INFO'},
     {'section': 'client',   'key': 'resource_profile',
      'type': str, 'mandatory': False, 'default': ''},
     {'section': 'client',   'key': 'project_profile',
      'type': str, 'mandatory': False, 'default': ''},
 ]
 '''Definition of mandatory configuration parameters.
 '''
@@ -242,21 +245,21 @@
 
         if args.tid:
             s3files[''] = combine_s3_path(args.id, '{}.{}'.format(filename, args.tid))
             if not is_exist_bucket_object(bucket, s3files['']):
                 raise Exception(MESSAGES.TASK_NOT_FOUND.value.format(args.tid))
         else:
             objects = bucket.objects.filter(Prefix=combine_s3_path(args.id, filename))
-            for object in objects:
-                pos = object.key.find('.')
+            for object_ in objects:
+                pos = object_.key.find('.')
                 if pos >= 0:
-                    tid = object.key[pos+1:]
+                    tid = object_.key[pos+1:]
                 else:
                     tid = ''
-                s3files[tid] = object.key
+                s3files[tid] = object_.key
 
     elif args.agent:
         s3files[''] = combine_s3_path(AGENT_LOG_PREFIX, args.agent)
         if not is_exist_bucket_object(bucket, s3files['']):
             raise Exception(MESSAGES.LOG_NOT_FOUND.value.format(args.agent))
 
     for key, val in s3files.items():
@@ -563,14 +566,32 @@
                 raise Exception(MESSAGES.CONFIG_PARAM_NOT_SPECIFIED.value.format(
                     param['section'], param['key']))
             else:
                 # if this parameter is optional, set detault value.
                 config[param['section']][param['key']] = param['default']
 
 
+def show_config(config: configparser.ConfigParser) -> None:
+    '''It show configuration parameters.
+
+    Args:
+        config (configparser.ConfigParser): CloudQ CLI configuration.
+    '''
+    for param in CONFIG_PARAMS:
+        try:
+            logger.info('section={}, key={}, value={}'.format(
+                param['section'], param['key'],
+                config.get(param['section'], param['key'])
+            ))
+        except configparser.NoOptionError:
+            logger.info('section={}, key={}, value=None'.format(
+                param['section'], param['key']
+            ))
+
+
 def _construct_argparser() -> argparse.ArgumentParser:
     '''It returns arguemnt parser.
 
     Returns:
         (argparse.ArgumentParser): the argument parser of CloudQ client.
     '''
     parser = argparse.ArgumentParser(description='CloudQ command line tool', add_help=True)
@@ -584,120 +605,153 @@
     parser_submit.add_argument('--script', help='job script')
     parser_submit.add_argument('--hold_jid', help='specify dependent jobs. ')
     parser_submit.add_argument('--array_tid', help='specify tasks to perform in an array job. ')
     parser_submit.add_argument('--submit_to', help='specify a system where the job script runs. '
                                'Available only to local job script')
     parser_submit.add_argument('--submit_opt', help='specify a command line arguments of job '
                                'submission command.  Available only to local job script')
+    parser_submit.add_argument('--log_level', help='specify log level. ')
     parser_submit.set_defaults(func=submit_job)
 
     # stat
     help_message_stat = 'Show the status of a job'
     parser_stat = subparsers.add_parser('stat', help=help_message_stat,
                                         description=help_message_stat)
     parser_stat.add_argument('--id', help='job id')
+    parser_stat.add_argument('--log_level', help='specify log level. ')
     parser_stat.set_defaults(func=stat_job)
 
     # log
     help_message_log = 'Show the standard output/error of a job'
     desc_message_log = help_message_log + '. ' + 'By default, it shows the standard output.'
     parser_log = subparsers.add_parser('log', help=help_message_log, description=desc_message_log)
     ex_group_log = parser_log.add_mutually_exclusive_group(required=True)
     ex_group_log.add_argument('--id', help='job id')
     ex_group_log.add_argument('--agent', help='agent name')
     parser_log.add_argument('--tid',
                             help='task id. It can specifies only when the job is array-job')
     parser_log.add_argument('--error',
                             help='show the standard error, instead of standard output',
                             action='store_true')
+    parser_log.add_argument('--log_level', help='specify log level. ')
     parser_log.set_defaults(func=show_job_log)
 
     # cancel
     help_message_cancel = 'Cancel a job'
     parser_cancel = subparsers.add_parser(
         'cancel', help=help_message_cancel, description=help_message_cancel)
     parser_cancel.add_argument('--id', help='job id')
+    parser_cancel.add_argument('--log_level', help='specify log level. ')
     parser_cancel.set_defaults(func=cancel_job)
 
     # delete
     help_message_del = 'Delete a job'
     parser_del = subparsers.add_parser(
         'delete', help=help_message_del, description=help_message_del)
     ex_group_del = parser_del.add_mutually_exclusive_group(required=True)
     ex_group_del.add_argument('--id', help='job id')
     ex_group_del.add_argument('--agent', help='agent name')
     ex_group_del.add_argument('--all', help='delete all completed jobs', action='store_true')
+    parser_del.add_argument('--log_level', help='specify log level. ')
     parser_del.set_defaults(func=del_job)
 
     # stage out
     help_message_stageout = 'Download outputs of a job'
     parser_stageout = subparsers.add_parser('stageout', help=help_message_stageout,
                                             description=help_message_stageout)
     parser_stageout.add_argument('--id', help='job id')
+    parser_stageout.add_argument('--log_level', help='specify log level. ')
     parser_stageout.set_defaults(func=stageout)
 
     # list
     help_message_list = 'Show list of waiting/running jobs'
     parser_list = subparsers.add_parser('list', help=help_message_list,
                                         description=help_message_list)
+    parser_list.add_argument('--log_level', help='specify log level. ')
     parser_list.set_defaults(func=list_jobs)
 
     # history
     help_message_history = 'Show list of completed jobs'
     parser_history = subparsers.add_parser('history', help=help_message_history,
                                            description=help_message_history)
+    parser_history.add_argument('--log_level', help='specify log level. ')
     parser_history.set_defaults(func=history_jobs)
 
     return parser
 
 
-def init_logger() -> None:
+def init_logger(args: argparse.Namespace, config: configparser.ConfigParser) -> None:
     '''It setups logger object.
     '''
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setFormatter(logging.Formatter(LOG_STDOUT_FORMAT))
     handlers = [stdout_handler]
 
     # If you want to output the log to both stdout and file, remove following commments.
     # file_handler = logging.FileHandler(filename=LOG_FILE)
     # file_handler.setFormatter(logging.Formatter(LOG_FILE_FORMAT))
     # handlers = [file_handler, stdout_handler]
 
     logging.basicConfig(handlers=handlers)
 
+    if args.log_level == 'INFO' or args.log_level == 'DEBUG':
+        log_level = args.log_level
+    else:
+        log_level = config['default']['log_level']
+
     global logger
     logger = logging.getLogger(PROCESS_NAME)
-    logger.setLevel(logging.INFO)
+    logger.setLevel(log_level)
+
+
+def create_default_config() -> str:
+    '''It creates default configuration files in home directory.
+
+    Returns:
+        str: configration file path.
+    '''
+    global DATA_DIR
+    DATA_DIR = os.path.expanduser('~/.cloudq/client')
+    default_dir = os.path.join(os.path.dirname(__file__), 'data')
+    config_path = os.path.join(DATA_DIR, CONFIG_FILE)
+
+    if not os.path.exists(DATA_DIR):
+        shutil.copytree(default_dir, DATA_DIR)
+
+    if not os.path.exists(config_path):
+        config_path = os.path.join(default_dir, CONFIG_FILE)
+
+    return config_path
 
 
 def main() -> None:
     '''the entry point.
     '''
-    init_logger()
-
     try:
-        global DATA_DIR
-        DATA_DIR = os.path.join(os.path.dirname(__file__), 'data')
-
-        if not os.path.isfile(os.path.join(DATA_DIR, CONFIG_FILE)):
+        config_path = create_default_config()
+        if not os.path.isfile(config_path):
             raise Exception(MESSAGES.NO_CONFIG_FILE.value.format(CONFIG_FILE))
 
-        config = configparser.ConfigParser()
-        config.read(os.path.join(DATA_DIR, CONFIG_FILE), encoding=CONFIG_FILE_ENCODING)
-
         parser = _construct_argparser()
         args = parser.parse_args()
 
+        config = configparser.ConfigParser()
+        config.read(config_path, encoding=CONFIG_FILE_ENCODING)
+
         _check_config(config)
+        init_logger(args, config)
+        logger.info('=================== config ====================')
+        show_config(config)
+        logger.info('===============================================')
 
         bucket = _get_bucket(config)
 
         args.func(config, args, bucket)
     except Exception as e:
         logger.error('Error: {}\n\n'.format(e))
-        logger.debug(traceback.format_exc())
+        logger.info(traceback.format_exc())
         if 'parser' in locals():
             parser.print_help()
 
 
 if __name__ == '__main__':
     main()
```

## cloudq/common.py

```diff
@@ -1,10 +1,10 @@
 # common: cloudq common library
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## cloudq/interface.py

```diff
@@ -1,10 +1,10 @@
 # interface: cloudq agent interface
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## cloudq/slurm.py

```diff
@@ -1,10 +1,10 @@
 # cloudqd: SLURM's job management and meta job script convert process
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -143,14 +143,15 @@
 
         Args:
             manifest (dict): a job manifest.
         Returns:
             dict: a job manifest added local parameters.
         '''
         logger.debug('submit_job start. UUID={}'.format(manifest[MANIFEST_PARAMS.UUID.value]))
+        logger.info('submit job (slurm): start. UUID={}'.format(manifest[MANIFEST_PARAMS.UUID.value]))
         if MANIFEST_PARAMS.LOCAL_NAME.value in manifest:
             name = manifest[MANIFEST_PARAMS.LOCAL_NAME.value]
         else:
             name = manifest[MANIFEST_PARAMS.NAME.value]
         submit_cmd = ['sbatch', name]
 
         if LOCAL_MANIFEST_PARAMS.LOCAL_SUBMIT_OPT.value in manifest:
@@ -186,23 +187,27 @@
             manifest[MANIFEST_PARAMS.JOB_ID.value] = result.group(1)
         else:
             logger.info(err.decode())
             manifest[MANIFEST_PARAMS.ERROR_MSG.value] = err.decode()
         logger.debug('submit_job ended. UUID={} JobID={}'.format(
             manifest[MANIFEST_PARAMS.UUID.value],
             manifest[MANIFEST_PARAMS.JOB_ID.value]))
+        logger.info('submit job (slurm): succeeded. UUID={} JobID={}'.format(
+            manifest[MANIFEST_PARAMS.UUID.value],
+            manifest[MANIFEST_PARAMS.JOB_ID.value]))
         return manifest
 
     def get_jobs_status(self) -> dict:
         '''It returns job status list.
 
         Returns:
             list: job status list.
         '''
         logger.debug('get_jobs_status start.')
+        logger.info('stat job (slurm): start.')
         jobs = []
         cmd = ['squeue', '-t', 'all']
         logger.debug('Run get job status command: {}'.format(' '.join(cmd)))
         proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (out, err) = proc.communicate()
         out = out.decode().splitlines()
         if out == []:
@@ -239,40 +244,47 @@
             idx = jobid.find(target)
             if idx > 0:
                 jobid = jobid[:idx]
 
             logger.debug('  jobid:{}, state:{}'.format(jobid, state))
             jobs.append((jobid, state))
         logger.debug('get_jobs_status ended. {} jobs'.format(len(jobs)))
+        logger.info('stat job (slurm): succeeded. {} jobs'.format(len(jobs)))
         return jobs
 
     def cancel_job(self, manifest: dict, force: bool) -> dict:
         '''It cancels a job.
 
         Args:
             manifest (dict): a job manifest.
             force (bool): If true, the job cancels forcibly.
         Returns:
             dict: a job manifest.
         '''
         logger.debug('cancel_job start. UUID={} JobID={}'.format(
             manifest[MANIFEST_PARAMS.UUID.value],
             manifest[MANIFEST_PARAMS.JOB_ID.value]))
+        logger.info('cancel job (slurm): start. UUID={} JobID={}'.format(
+            manifest[MANIFEST_PARAMS.UUID.value],
+            manifest[MANIFEST_PARAMS.JOB_ID.value]))
         if not force:
             cancel_cmd = ['scancel', manifest[MANIFEST_PARAMS.JOB_ID.value]]
         else:
             return
 
         logger.debug('Run cancel command: {}'.format(' '.join(cancel_cmd)))
         proc = subprocess.Popen(cancel_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (out, err) = proc.communicate()
         logger.info(out.decode())
         logger.debug('cancel_job ended. UUID={} JobID={}'.format(
             manifest[MANIFEST_PARAMS.UUID.value],
             manifest[MANIFEST_PARAMS.JOB_ID.value]))
+        logger.info('cancel job (slurm): succeeded. UUID={} JobID={}'.format(
+            manifest[MANIFEST_PARAMS.UUID.value],
+            manifest[MANIFEST_PARAMS.JOB_ID.value]))
         return manifest
 
     def get_job_log(self, manifest: dict, error: bool) -> dict:
         '''It saves a job log.
 
         Args:
             manifest (dict): a job manifest.
```

## cloudq/aws/__init__.py

```diff
@@ -1,10 +1,10 @@
 # cloudq.aws: CloudQ builder for AWS
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## cloudq/aws/cloudqaws.py

```diff
@@ -1,10 +1,10 @@
 # cloudqaws: cloudq builder for AWS
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -21,14 +21,15 @@
 from functools import cmp_to_key
 import configparser
 from enum import Enum
 import logging
 import tempfile
 import time
 import traceback
+import shutil
 
 from .utils import Utils
 
 PROCESS_NAME = 'CloudQ Builder for AWS'
 '''Name of this process.
 '''
 LOG_FILE = 'cloudqaws.log'
@@ -46,26 +47,30 @@
 CONFIG_FILE_ENCODING = 'utf-8'
 '''Encoding of configuration file.
 '''
 
 CONFIG_PARAMS = [
     {'section': 'default',  'key': 'stack_check_interval',
      'type': int,   'mandatory': True,    'min': 1},
+    {'section': 'default',  'key': 'log_level',
+     'type': str, 'mandatory': False,  'default': 'INFO'},
 ]
 '''Definition of mandatory configuration parameters.
 '''
 
 
 class MESSAGES(Enum):
     ''' List of console messages.
     '''
 
     # success
     CREATE_COMPLETED = 'AWS compute cluster ({}) has been created.'
     DELETE_COMPLETED = 'AWS compute cluster ({}) has been deleted.'
+    PRESET_COMPLETED = 'Preset ({}) has been created.'
+    INFORMATION_PRESET_AFTER = 'Please change the contents of the preset according to your computing environment.'
 
     # success
     STACK_CREATING = 'The stack ({}) is creating. Please wait a minute.'
     STACK_DELETING = 'The stack ({}) is deleting. Please wait a minute.'
 
     # error
     CONFIG_PARAM_NOT_SPECIFIED = 'Mandatory configuration parameter is not specified: [{}] {}'
@@ -73,14 +78,18 @@
     CLUSTER_NAME_NOT_SPECIFIED = 'Cluster name is not specified.'
     KEY_PAIR_NOT_SPECIFIED = 'EC2 Key-pair file is not specified.'
     KEY_PAIR_NOT_FOUND = 'The EC2 Key-pair file is not found: {}'
     PROFILE_NOT_SPECIFIED = 'AWS profile is not specified.'
     ENDPOINT_NOT_SPECIFIED = 'Endpoint URL is not specified.'
     BUCKET_NOT_SPECIFIED = 'Bucket name is not specified.'
     NO_CONFIG_FILE = 'The configuration file is not found: {}'
+    INVALID_PRESET_NAME = 'Invalid specified preset name.'
+    ERROR_MESSAGE_PRESET = 'Failed to create Preset.'
+    ERROR_MESSAGE_CREATE = 'Failed to create AWS compute cluster.'
+    ERROR_MESSAGE_DELETE = 'Failed to delete AWS compute cluster.'
 
 
 def create_cluster(config: configparser.ConfigParser, args: argparse.Namespace):
     '''It creates a AWS compute cluster.
 
     Args:
         config (configparser.ConfigParser): CloudQ Builder for AWS configuration.
@@ -105,31 +114,42 @@
     cs_aws_info = Utils().get_aws_info(args.cs_profile)
 
     if args.zone:
         zone = args.zone
     else:
         zone = Utils().get_availability_zone()
 
-    cf_stack_info = Utils().create_cloud_formation_stack(args.name, zone)
+    if args.preset_name:
+        preset_data = args.preset_name
+    else:
+        preset_data = 'default'
+
+    cf_stack_info = Utils().create_cloud_formation_stack(args.name, zone, preset_data)
     while not Utils().is_stack_created(cf_stack_info, True):
         logger.info(MESSAGES.STACK_CREATING.value.format(cf_stack_info['StackName']))
         time.sleep(config.getint('default', 'stack_check_interval'))
 
     with tempfile.TemporaryDirectory() as temp_dir_path:
         cluster_config_path = Utils().create_cluster_config(
-            temp_dir_path, default_aws_info, cs_aws_info, cf_stack_info, args.keypair)
+            temp_dir_path, default_aws_info, cs_aws_info, cf_stack_info, args.keypair, preset_data)
         cloudq_config_path = Utils().create_cloudq_config(
             args.name, temp_dir_path, args.cs_endpoint, args.cs_bucket)
+        cloudq_autoexec_path = Utils().create_autoexec_config(temp_dir_path, log_level, preset_data)
+
         Utils().upload_setup_files([
             cloudq_config_path,
-            os.path.join(Utils().get_data_dir_path(), 'on-head-node-start.sh'),
-            os.path.join(Utils().get_data_dir_path(), 'on-compute-node-start.sh'),
-            os.path.join(Utils().get_data_dir_path(), 'add_log.py'),
-            os.path.join(Utils().get_data_dir_path(), 'autoexec.sh'),
-            os.path.join(Utils().get_data_dir_path(), 'cloudq.service'),
+            os.path.join(os.path.expanduser(
+                '~/.cloudq/aws/'), preset_data, 'on-head-node-start.sh'),
+            os.path.join(os.path.expanduser(
+                '~/.cloudq/aws/'), preset_data, 'on-compute-node-start.sh'),
+            os.path.join(os.path.expanduser(
+                '~/.cloudq/aws/'), preset_data, 'add_log.py'),
+            cloudq_autoexec_path,
+            os.path.join(os.path.expanduser(
+                '~/.cloudq/aws/'), preset_data, 'cloudq.service'),
         ], cf_stack_info['BucketName'])
         pc_stack_info = Utils().create_parallel_cluster_stack(args.name, cluster_config_path)
         while not Utils().is_stack_created(pc_stack_info):
             logger.info(MESSAGES.STACK_CREATING.value.format(pc_stack_info['StackName']))
             time.sleep(config.getint('default', 'stack_check_interval'))
 
     logger.info(MESSAGES.CREATE_COMPLETED.value.format(args.name))
@@ -209,14 +229,40 @@
         logger.info('  '.join([cluster['ClusterName'].ljust(name_len, ' '),
                                cluster['Status'].ljust(9, ' '),
                                creation_time]))
 
     logger.debug('list_clusters ended.')
 
 
+def preset_cluster(config: configparser.ConfigParser, args: argparse.Namespace):
+    '''It creates a preset.
+
+    Args:
+        config (configparser.ConfigParser): Preset configuration.
+        args (argparse.Namespace): Arguments for directory name.
+            Used arguments are ``preset_name``.
+    '''
+    logger.debug('preset_cluster start.')
+    try:
+        if args.preset_name:
+            preset_dir_name = args.preset_name
+            path = os.path.join(os.path.expanduser('~/.cloudq/aws/'), args.preset_name)
+            if not os.path.isdir(path):
+                dir_default = os.path.join(os.path.dirname(__file__), 'data', 'default')
+                shutil.copytree(dir_default, path)
+        else:
+            preset_dir_name = 'default'
+    except Exception:
+        raise Exception(MESSAGES.INVALID_PRESET_NAME.value)
+
+    logger.info(MESSAGES.PRESET_COMPLETED.value.format(preset_dir_name))
+    logger.info(MESSAGES.INFORMATION_PRESET_AFTER.value)
+    logger.debug('preset_cluster ended.')
+
+
 def _check_config(config: configparser.ConfigParser) -> None:
     '''It checks configuration parameters.
 
     Args:
         config (configparser.ConfigParser): CloudQ CLI configuration.
     '''
     for param in CONFIG_PARAMS:
@@ -246,14 +292,32 @@
                 raise Exception(MESSAGES.CONFIG_PARAM_NOT_SPECIFIED.value.format(
                     param['section'], param['key']))
             else:
                 # if this parameter is optional, set detault value.
                 config[param['section']][param['key']] = param['default']
 
 
+def show_config(config: configparser.ConfigParser) -> None:
+    '''It checks configuration parameters.
+
+    Args:
+        config (configparser.ConfigParser): CloudQ CLI configuration.
+    '''
+    for param in CONFIG_PARAMS:
+        try:
+            logger.info('section={}, key={}, value={}'.format(
+                param['section'], param['key'],
+                config.get(param['section'], param['key'])
+            ))
+        except configparser.NoOptionError:
+            logger.info('section={}, key={}, value=None'.format(
+                param['section'], param['key']
+            ))
+
+
 def _construct_argparser() -> argparse.ArgumentParser:
     '''It returns arguemnt parser.
 
     Returns:
         (argparse.ArgumentParser): the argument parser of CloudQ client.
     '''
     parser = argparse.ArgumentParser(description='CloudQ Builder for AWS', add_help=True)
@@ -272,75 +336,136 @@
         help='specify AWS profile to access an object storage that stores CloudQ jobs.')
     parser_create.add_argument(
         '--cs_endpoint',
         help='specify the endpoint URL of an object storage that stores CloudQ jobs.')
     parser_create.add_argument(
         '--cs_bucket',
         help='specify the name of the bucket where CloudQ jobs are stored.')
+    parser_create.add_argument('--preset_name', help='specify preset name. ')
+    parser_create.add_argument('--log_level', help='specify log level. ')
     parser_create.set_defaults(func=create_cluster)
 
     # delete
     help_message_delete = 'Delete a AWS compute cluster'
     parser_delete = subparsers.add_parser('delete', help=help_message_delete,
                                           description=help_message_delete)
     parser_delete.add_argument('--name', help='specify cluster name.')
+    parser_delete.add_argument('--log_level', help='specify log level. ')
     parser_delete.set_defaults(func=delete_cluster)
 
     # list
     help_message_list = 'Show list of AWS compute clusters'
     parser_list = subparsers.add_parser('list', help=help_message_list,
                                         description=help_message_list)
+    parser_list.add_argument('--log_level', help='specify log level. ')
     parser_list.set_defaults(func=list_clusters)
 
+    # preset
+    help_message_preset = 'Create a preset'
+    parser_preset = subparsers.add_parser('preset', help=help_message_preset,
+                                          description=help_message_preset)
+    parser_preset.add_argument('--preset_name', help='specify preset name. ')
+    parser_preset.add_argument('--log_level', help='specify log level. ')
+    parser_preset.set_defaults(func=preset_cluster)
+
     return parser
 
 
-def init_logger() -> None:
+def init_logger(args: argparse.Namespace, config: configparser.ConfigParser) -> None:
     '''It setups logger object.
     '''
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setFormatter(logging.Formatter(LOG_STDOUT_FORMAT))
     handlers = [stdout_handler]
 
     # If you want to output the log to both stdout and file, remove following commments.
     # file_handler = logging.FileHandler(filename=LOG_FILE)
     # file_handler.setFormatter(logging.Formatter(LOG_FILE_FORMAT))
     # handlers = [file_handler, stdout_handler]
 
     logging.basicConfig(handlers=handlers)
 
+    global log_level
+
+    if args.log_level == 'INFO' or args.log_level == 'DEBUG':
+        log_level = args.log_level
+    else:
+        log_level = config['default']['log_level']
+
     global logger
     logger = logging.getLogger(PROCESS_NAME)
-    logger.setLevel(logging.INFO)
+    logger.setLevel(log_level)
+
+
+def create_default_config() -> str:
+    '''It creates default configuration files in home directory.
+
+    Returns:
+        str: configration file path.
+    '''
+    data_dir = os.path.expanduser('~/.cloudq/aws')
+    default_dir = os.path.join(os.path.dirname(__file__), 'data')
+    config_path = os.path.join(data_dir, CONFIG_FILE)
+
+    if not os.path.isdir(data_dir):
+        shutil.copytree(default_dir, data_dir)
+
+    if not os.path.isfile(config_path):
+        config_path = os.path.join(default_dir, CONFIG_FILE)
+
+    return config_path
+
+
+def create_error_message(subcommand: str) -> str:
+    '''It creates of error messages for each subcommand.
+
+    Args:
+        subcommand (str): subcommand arguments
+    Returns:
+        str: error message.
+    '''
+    message = ''
+    if subcommand == 'preset':
+        message = MESSAGES.ERROR_MESSAGE_PRESET.value
+    elif subcommand == 'create':
+        message = MESSAGES.ERROR_MESSAGE_CREATE.value
+    elif subcommand == 'delete':
+        message = MESSAGES.ERROR_MESSAGE_DELETE.value
+
+    return message
 
 
 def main():
     '''the entry point.
     '''
-    init_logger()
 
     try:
-        config_path = os.path.join(Utils().get_data_dir_path(), CONFIG_FILE)
+        config_path = create_default_config()
         if not os.path.isfile(config_path):
             raise Exception(MESSAGES.NO_CONFIG_FILE.value.format(CONFIG_FILE))
 
-        config = configparser.ConfigParser()
-        config.read(config_path, encoding=CONFIG_FILE_ENCODING)
-
         parser = _construct_argparser()
         args = parser.parse_args()
 
+        config = configparser.ConfigParser()
+        config.read(config_path, encoding=CONFIG_FILE_ENCODING)
+
         _check_config(config)
+        init_logger(args, config)
+        logger.info('=================== config ====================')
+        show_config(config)
+        logger.info('===============================================')
 
         start_time = time.perf_counter()
         args.func(config, args)
         elapsed_time = time.perf_counter() - start_time
         logger.debug('Process completed. {:.2f} seconds elapsed.'.format(elapsed_time))
     except Exception as e:
-        logger.error('Error: {}\n\n'.format(e))
-        logger.debug(traceback.format_exc())
+        message = create_error_message(args.subcommand)
+        logger.error('Error: {}\n {}\n\n'.format(message, e))
+        logger.error(traceback.format_exc())
         if 'parser' in locals():
             parser.print_help()
 
 
 if __name__ == '__main__':
     main()
```

## cloudq/aws/utils.py

```diff
@@ -1,10 +1,10 @@
 # util: cloudq builder for AWS utilities
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -69,21 +69,21 @@
     '''
 
     def __init__(self) -> None:
         '''Initialize.
         '''
         pass
 
-    def get_data_dir_path(self) -> list:
+    def get_data_dir_path(self, preset_data: str) -> list:
         '''It returns path of data directory.
 
         Returns:
             list(dict): path of data directory.
         '''
-        return os.path.join(os.path.dirname(__file__), 'data')
+        return os.path.join(os.path.expanduser('~/.cloudq/aws/'), preset_data)
 
     def get_aws_info(self, profile: str = None) -> dict:
         '''It returns profile of AWS CLI.
 
         Args:
             profile (str):  the name of AWS profile.
         Returns:
@@ -98,32 +98,33 @@
                 command.append('--profile={}'.format(profile))
             command.append(key)
             result = self.exec_command(command)
             if len(result):
                 aws_info[key] = result
         return aws_info
 
-    def create_cloud_formation_stack(self, cluster_name: str, zone: str) -> dict:
+    def create_cloud_formation_stack(self, cluster_name: str, zone: str, preset_data: str) -> dict:
         '''It creates Cloud Formation stack.
 
         Args:
             cluster_name (str): Name of AWS compute cluster.
             zone (str): Availability zone.
+            preset_data (str): Name of preset data.
         Returns:
             dict: Informations of cloud formation stack.
         '''
         stack_info = {
             'StackName': '{}-vpc'.format(cluster_name),
             'BucketName': '{}-{}'.format(cluster_name, self.get_random_value()),
         }
 
         command = ['aws', 'cloudformation', 'create-stack']
         command += ['--stack-name', stack_info['StackName']]
-        command += ['--template-body', 'file://{}'.format(
-            os.path.join(self.get_data_dir_path(), 'cloud-stack.yaml'))]
+        command += ['--template-body', 'file://{}'.format(os.path.join(
+            os.path.expanduser('~/.cloudq/aws/'), preset_data, 'cloud-stack.yaml'))]
         command += ['--parameters']
         command += ['ParameterKey=PublicCIDR,ParameterValue=10.0.0.0/24']
         command += ['ParameterKey=PrivateCIDR,ParameterValue=10.0.16.0/24']
         command += ['ParameterKey=AvailabilityZone,ParameterValue={}'.format(zone)]
         command += ['ParameterKey=InternetGatewayId,ParameterValue=']
         command += ['ParameterKey=BucketName,ParameterValue={}'.format(stack_info['BucketName'])]
 
@@ -190,27 +191,27 @@
             else:
                 raise Exception(result)
         if is_created is None:
             raise Exception('Stack is missing. StackId:{}'.format(stack_info['StackID']))
         return is_created
 
     def create_cluster_config(self, output_dir_path: str, default_aws_info: dict, cs_aws_info: dict,
-                              stack_info: dict, keypair: str) -> str:
+                              stack_info: dict, keypair: str, preset_data: str) -> str:
         '''It creates cluster config file
 
         Args:
             output_dir_path (str): Path of output directory.
             default_aws_info (dict):  default profile of AWS CLI.
             cs_aws_info (dict):  profile of AWS CLI to accessing cloud object storage.
             stack_info (dict): Informations of cloud formation stack.
             keypair (str): the name of EC2 key-pair.
         Returns:
             str: Path of Parallel Cluster configuretion file
         '''
-        with open(os.path.join(self.get_data_dir_path(), 'cluster-config.yaml')) as fp:
+        with open(os.path.join(self.get_data_dir_path(preset_data), 'cluster-config.yaml')) as fp:
             config = yaml.safe_load(fp)
 
         head_script = 's3://{}/on-head-node-start.sh'.format(stack_info['BucketName'])
         compute_script = 's3://{}/on-compute-node-start.sh'.format(stack_info['BucketName'])
 
         cloudq_version = self.get_cloudq_version()
 
@@ -271,14 +272,58 @@
 
         dst_path = os.path.join(output_dir_path, 'config.ini')
         with open(dst_path, 'w') as file:
             config.write(file)
 
         return dst_path
 
+    def create_autoexec_config(self, output_dir_path: str, log_level: str, preset_data: str) -> str:
+        '''It creates script file for CloudQ Agent.
+
+        Args:
+            output_dir_path (str): Path of output directory.
+            log_level (str): Specify the log level.
+        Returns:
+            str: Path of CloudQ Agent script file.
+        '''
+        src_path = os.path.join(os.path.expanduser('~/.cloudq/aws/'), preset_data, 'autoexec.sh')
+
+        with open(src_path, 'r') as file:
+            tmp_list = []
+            is_target = False
+            for row in file:
+                if not row.startswith('#') and 'cloudqd' in row:
+                    is_target = True
+                    split_list = row.split()
+                    if '--log_level' in split_list:
+                        x = split_list.index('--log_level') + 1
+                        if len(split_list) > x:
+                            split_list[x] = log_level
+                            split_list = " ".join(split_list)
+                            tmp_list.append(split_list + '\n')
+                        else:
+                            split_list = " ".join(split_list)
+                            tmp_list.append(split_list + ' ' + log_level + '\n')
+                    else:
+                        split_list.append('--log_level')
+                        split_list.append(log_level)
+                        split_list = " ".join(split_list)
+                        tmp_list.append(split_list + '\n')
+                else:
+                    tmp_list.append(row)
+            if is_target is False:
+                raise Exception('Failed to set log level.')
+
+        dst_path = os.path.join(output_dir_path, 'autoexec.sh')
+        with open(dst_path, 'w', newline="\n") as file:
+            for i in range(len(tmp_list)):
+                file.write(tmp_list[i])
+
+        return dst_path
+
     def upload_setup_files(self, upload_files: list, bucket_name: str) -> None:
         '''It uploads setup files to S3_bucket.
 
         Args:
             upload_files (list(str)): List of upload file path.
             bucket_name (str): Name of S3 bucket.
         '''
```

## cloudq/aws/data/config.ini

```diff
@@ -1,2 +1,3 @@
 [default]
 stack_check_interval = 10
+log_level = INFO
```

## cloudq/data/config.ini

```diff
@@ -2,14 +2,16 @@
 name = your_system_name
 
 aws_profile = default
 
 cloudq_endpoint_url = https://s3.abci.ai
 cloudq_bucket = cloudq
 
+log_level = INFO
+
 [agent]
 type = abci
 num_procs = 8
 daemon_interval = 5
 cloudq_directory = ~/.cloudq
 
 [client]
```

## cloudq/example/ljob_array.abci.sh

```diff
@@ -1,14 +1,14 @@
 #!/bin/sh
 #$ -l rt_G.small=1
 #$ -cwd
 #$-l h_rt=01:00:00
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -26,15 +26,15 @@
 #                    --submit_opt '-g YOUR_GROUP -t 1-4'
 #
 # $ cloudqcli submit --script ljob_array.abci.sh --submit_to abci \
 #                    --submit_opt '-g YOUR_GROUP' --array_tid 1-4
 
 source /etc/profile
 source /etc/profile.d/modules.sh
-module load singularitypro/3.7
+module load singularitypro/3.9
 
 export TMPDIR=$SGE_LOCALDIR
 
 SIGIMG=docker://nvcr.io/nvidia/pytorch:20.12-py3
 
 IDX=$((SGE_TASK_ID-1))
 TASKSETS=(
@@ -47,9 +47,9 @@
 echo "Array Job Configuration"
 echo "  SGE_TASK_ID:       ": $SGE_TASK_ID
 echo "  SGE_TASK_FIRST:    ": $SGE_TASK_FIRST
 echo "  SGE_TASK_LAST:     ": $SGE_TASK_LAST
 echo "  SGE_TASK_STEPSIZE: ": $SGE_TASK_STEPSIZE
 echo "  Train parameter:   ": ${TASKSETS[$IDX]}
 
-wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/master/mnist/main.py
+wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/0f0c9131ca5c79d1332dce1f4c06fe942fbdc665/mnist/main.py
 singularity exec --nv $SIGIMG python cnn_mnist.py ${TASKSETS[$IDX]}
```

## cloudq/example/ljob_pt_mnist.abci.sh

```diff
@@ -1,14 +1,14 @@
 #!/bin/sh
 #$ -l rt_G.small=1
 #$ -cwd
 #$-l h_rt=01:00:00
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -23,19 +23,19 @@
 #
 # Submission Example
 # $ cloudqcli submit --script ljob_pt_mnist.abci.sh --submit_to abci \
 #                    --submit_opt '-g YOUR_GROUP'
 
 source /etc/profile
 source /etc/profile.d/modules.sh
-module load singularitypro/3.7
+module load singularitypro/3.9
 
 export TMPDIR=$SGE_LOCALDIR
 
 SIGURL=docker://nvcr.io/nvidia/pytorch:20.12-py3
 SIGFILE=pytorch-20.12-py3.img
 
 singularity pull $SIGFILE $SIGURL
-wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/master/mnist/main.py
+wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/0f0c9131ca5c79d1332dce1f4c06fe942fbdc665/mnist/main.py
 singularity exec --nv $SIGFILE python cnn_mnist.py
 
 rm $SIGFILE
```

## cloudq/example/ljob_tf_mnist.abci.sh

```diff
@@ -1,14 +1,14 @@
 #!/bin/sh
 #$ -l rt_G.small=1
 #$ -cwd
 #$-l h_rt=01:00:00
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -23,15 +23,15 @@
 #
 # Submission Example
 # $ cloudqcli submit --script ljob_tf_mnist.abci.sh --submit_to abci \
 #                    --submit_opt '-g YOUR_GROUP'
 
 source /etc/profile
 source /etc/profile.d/modules.sh
-module load singularitypro/3.7
+module load singularitypro/3.9
 
 export TMPDIR=$SGE_LOCALDIR
 
 SIGURL=docker://nvcr.io/nvidia/tensorflow:19.07-py3
 SIGFILE=tensorflow-19.07-py3.img
 
 singularity pull $SIGFILE $SIGURL
```

## cloudq/example/mjob_array.sh

```diff
@@ -1,17 +1,17 @@
-#$ run_on:        ABCI
+#$ run_on:        abci
 #$ project:       project001
 #$ resource:      resource001
 #$ n_resource:    1
 #$ walltime:      1:00:00
 #$ other_opts:    -p -400
 #$ container_img: docker://nvcr.io/nvidia/pytorch:20.12-py3
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -38,9 +38,9 @@
 echo "Array Job Configuration"
 echo "  ARY_TASK_ID:       ": $ARY_TASK_ID
 echo "  ARY_TASK_FIRST:    ": $ARY_TASK_FIRST
 echo "  ARY_TASK_LAST:     ": $ARY_TASK_LAST
 echo "  ARY_TASK_STEPSIZE: ": $ARY_TASK_STEPSIZE
 echo "  Train parameter:   ": ${TASKSETS[$IDX]}
 
-wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/master/mnist/main.py
+wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/0f0c9131ca5c79d1332dce1f4c06fe942fbdc665/mnist/main.py
 cq_container_run $CONTAINER_IMG0 python cnn_mnist.py ${TASKSETS[$IDX]}
```

## cloudq/example/mjob_pt_mnist.sh

```diff
@@ -1,17 +1,17 @@
-#$ run_on:        ABCI
+#$ run_on:        abci
 #$ project:       project001
 #$ resource:      resource001
 #$ n_resource:    1
 #$ walltime:      1:00:00
 #$ other_opts:    -p -400
 #$ container_img: docker://nvcr.io/nvidia/pytorch:20.12-py3
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -23,9 +23,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #======================================================================================
 #
 # Submission Example
 # $ cloudqcli submit --script cloudq/example/mjob_pt_mnist.sh
 
-wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/master/mnist/main.py
+wget -O cnn_mnist.py https://raw.githubusercontent.com/pytorch/examples/0f0c9131ca5c79d1332dce1f4c06fe942fbdc665/mnist/main.py
 cq_container_run $CONTAINER_IMG0 python cnn_mnist.py
```

## cloudq/example/mjob_tf_mnist.sh

```diff
@@ -1,17 +1,17 @@
-#$ run_on:        ABCI
+#$ run_on:        abci
 #$ project:       project001
 #$ resource:      resource001
 #$ n_resource:    1
 #$ walltime:      1:00:00
 #$ other_opts:    -p -400
 #$ container_img: docker://nvcr.io/nvidia/tensorflow:19.07-py3
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## Comparing `cloudq/aws/data/add_log.py` & `cloudq/aws/data/default/add_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # add_logs: Add head node logs to Amazon CloudWatch Logs
 #
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## Comparing `cloudq/aws/data/autoexec.sh` & `cloudq/aws/data/default/autoexec.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## Comparing `cloudq/aws/data/cloud-stack.yaml` & `cloudq/aws/data/default/cloud-stack.yaml`

 * *Files identical despite different names*

## Comparing `cloudq/aws/data/cluster-config.yaml` & `cloudq/aws/data/default/cluster-config.yaml`

 * *Files identical despite different names*

## Comparing `cloudq/aws/data/on-compute-node-start.sh` & `cloudq/aws/data/default/on-compute-node-start.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## Comparing `cloudq/aws/data/on-head-node-start.sh` & `cloudq/aws/data/default/on-head-node-start.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 #
 #======================================================================================
-# Copyright 2022
+# Copyright 2022-2023
 #   National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 #   Hitachi, Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

## Comparing `cloudq-1.1.1.dist-info/LICENSE.txt` & `cloudq-1.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cloudq-1.1.1.dist-info/METADATA` & `cloudq-1.2.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudq
-Version: 1.1.1
+Version: 1.2.0
 Summary: A cloud storage-based meta scheduler.
 Home-page: https://github.com/aistairc/cloudq
 Author: Shinichiro Takizawa, AIST
 Author-email: shinichiro.takizawa@aist.go.jp
 License: Apache License, Version 2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3.6
@@ -15,21 +15,22 @@
 License-File: LICENSE.txt
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: pathos
 Provides-Extra: abci
 Provides-Extra: aws
 Requires-Dist: pyyaml ; extra == 'aws'
+Requires-Dist: Flask ; extra == 'aws'
 Requires-Dist: aws-parallelcluster ; extra == 'aws'
 
 # CloudQ
 
 Cloud storage-based meta scheduler
 
-Copyright 2022 National Institute of Advanced Industrial Science and Technology (AIST), Japan and
+Copyright 2022-2023 National Institute of Advanced Industrial Science and Technology (AIST), Japan and
 Hitachi, Ltd.
 
 This program is licensed under the Apache License, Version2.0.
 
 
 ## Overview
 
@@ -64,26 +65,26 @@
 CloudQ Builder for AWS creates clusters using Slurm as their job scheduler.
 It installs CloudQ Agent on cluster's head node.
 
 ## Requirements
 
 CloudQ Client
 - OS: Linux, MacOS and Windows
-- Python: 3.8 or newer (Tested on Python 3.8.7)
-- AWS CLI: 2.1.30 or newer (Tested on AWS CLI 2.1.30)
+- Python: 3.8 or newer (Tested on Python 3.8.16)
+- AWS CLI: 2.1.30 or newer (Tested on AWS CLI 2.9.16)
 
 CloudQ Agent
 - OS: Linux compatible OS (Tested on CentOS 7.5 and Amazon Linux 2)
-- Python: 3.8 or newer (Tested on Python 3.8.7)
-- AWS CLI: 2.1.30 or newer (Tested on AWS CLI 2.1.30)
+- Python: 3.8 or newer (Tested on Python 3.8.16)
+- AWS CLI: 2.1.30 or newer (Tested on AWS CLI 2.9.16)
 
 CloudQ Builder for AWS
 - OS: Linux, MacOS and Windows
-- Python: 3.8 or newer (Tested on Python 3.8.7)
-- AWS CLI: 2.1.30 or newer (Tested on AWS CLI 2.1.30)
+- Python: 3.8 or newer (Tested on Python 3.8.16)
+- AWS CLI: 2.1.30 or newer (Tested on AWS CLI 2.9.16)
 - AWS ParallelCluster: 3.0.3
 
 
 ## Installation
 
 [Installation Guide](/docs/INSTALLATION_GUIDE.md) describes how to install and configure CloudQ.
 
@@ -307,86 +308,21 @@
 ```console
 $ cloudqaws delete --name your-cluster-name
 The stack (your-cluster-name-nodes) is deleting. Please wait a minute.
 The stack (your-cluster-name-vpc) is deleting. Please wait a minute.
 AWS compute cluster (your-cluster-name) has been deleted.
 ```
 
+### Change log level of CloudQ
 
-## Meta Jobscript
-
-Meta jobscript is introduced to write a jobscript that runs on any systems CloudQ supports.
-A jobscript written in Meta jobscript is converted to a local jobscript by a CloudQ agent when it receives a job.
-Meta jobscript can use the following directives, functions and environment variables.
-
-### Directives
-
-|  Name  |  Explanation  | ABCI | AWS Compute Cluster |
-| ---- | ---- | ---- | ---- |
-|  run_on  |  [Optional] Name of a system that runs the job. If not specified, the job will be executed on the earliest scheduled system.  | Available | Available |
-|  project  |  [Mandatory] Name of a research project.  It can be used for charge on some systems.  | Available | Unavailable |
-|  resource  |  [Mandatory] Name of resource type used to run the job.  | Available | Available |
-|  n_resource  |  [Mandatory] Number of resources used to run the job.  | Available | Available |
-|  walltime  |  [Optional] Walltime requested.  If not specified, the default walltime on the system is applied.  | Available | Available |
-|  other_opts  |  [Optional] Options to the job submission command appended when the job is submitted.  | Available | Available |
-|  container_img  |  [Optional] URL of container image used in the job.  It can be specified multiple times.  | Available | Unavailable |
-
-### Functions
-
-#### Launch Container
-
-```shell
-cq_container_run IMG [CMD]
-```
-
-It launchs a container using the specified image.
-The container runtime the system supports is used.
-
-Arguments
-- IMG:	Path of a container image.
-- CMD:	A command and its options executed in the container.
-
-Availability
-- ABCI: Available
-- AWS Compute Cluster: Unavailable
+Commands CloudQ Client、Agent and Builder can change the log level by the respective `config.ini` setting or `--log_level` option.
+Log levels can be specified from `INFO` or `DEBUG`.
+The value specified with the `--log_level` option takes precedence.
+If neither is specified, `INFO` is applied as the default log level.
 
-#### Copy Cloud Storage Object
-
-```shell
-abci_cs_cp SRC DST [ENDPOINT [PROFILE]]
-```
-
-It copies files and objects between cloud storage and local filesystem.
-
-Arguments
-- SRC:	URL of source files/objects.
-- DST:	URL of destination files/objects.
-- ENDPOINT:	 URL of cloud storage endpoint.  It not specified, the endpoint URL specified in configuration file is used.
-- PROFILE:	Name of AWS profile. If not specified, the AWS profile specified in configuration file is used.
-
-Availability
-- ABCI: Available
-- AWS Compute Cluster: Available
-
-### Environment Variables
-
-|  Name  |  Explanation  | ABCI | AWS Compute Cluster |
-| ---- | ---- | ---- | ---- |
-|  SYSTEM  |  Name of a system that runs the job.  | Available | Available |
-|  CONTAINER_IMG#  |  File name of a container image.  # will be replaced by a serial number starting with 0.  | Available | Unavailable |
-|  ARY_TASK_ID  |  Task ID of an array job.  | Available | Available |
-|  ARY_TASK_FIRST  |  Task ID of the first task of an array job.  | Available | Available |
-|  ARY_TASK_LAST  |  Task ID of the last task of an array job.  | Available | Available |
-|  ARY_TASK_STEPSIZE  |  Step size of IDs of an array job.  | Available | Available |
-
-### Example
-
-Example meta jobscripts can be found in `cloudq/example` directory.
+## Meta Jobscript
 
-- mjob_array.sh
-  - Array job example
-- mjob_pt_mnist.sh
-  - Download container image from NGC and then train MNIST using PyTorch on a singularity container
-- mjob_tf_mnist.sh
-  - Download container image from NGC and then train MNIST using TensorFlow on a singularity container
+[Meta Jobscript Description](/docs/META_JOBSCRIPT_DESCRIPTION.md) describes how to use Meta jobscript.
 
+## Publications
 
+- Shinichiro Takizawa Masaaki Shimizu, Hidemoto Nakada, Toshiya Matsuba, and Ryousei Takano, "CloudQ: A Secure AI / HPC Cloud Bursting System,"  9th International Workshop on HPC User Support Tools (HUST22), November 2022.
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

