# Comparing `tmp/whitebox_adversarial_toolbox-0.0.1-py3-none-any.whl.zip` & `tmp/whitebox_adversarial_toolbox-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,68 @@
-Zip file size: 3811 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      493 b- defN 21-Dec-01 15:17 what/__init__.py
--rw-rw-rw-  2.0 fat       91 b- defN 21-Dec-01 15:23 what/attacks/__init__.py
--rw-rw-rw-  2.0 fat       73 b- defN 21-Dec-01 15:24 what/models/__init__.py
--rw-rw-rw-  2.0 fat       38 b- defN 21-Dec-01 15:24 what/utils/__init__.py
--rw-rw-rw-  2.0 fat     1084 b- defN 21-Dec-01 16:02 whitebox_adversarial_toolbox-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2018 b- defN 21-Dec-01 16:02 whitebox_adversarial_toolbox-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 21-Dec-01 16:02 whitebox_adversarial_toolbox-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 21-Dec-01 16:02 whitebox_adversarial_toolbox-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      796 b- defN 21-Dec-01 16:02 whitebox_adversarial_toolbox-0.0.1.dist-info/RECORD
-9 files, 4695 bytes uncompressed, 2407 bytes compressed:  48.7%
+Zip file size: 59857 bytes, number of entries: 66
+-rw-rw-r--  2.0 unx     4966 b- defN 23-Jun-09 13:12 what/__init__.py
+-rw-rw-r--  2.0 unx       31 b- defN 23-Jun-01 14:11 what/__main__.py
+-rw-rw-r--  2.0 unx     4345 b- defN 23-Jun-09 13:01 what/_main.py
+-rw-rw-r--  2.0 unx      634 b- defN 23-Jun-09 14:08 what/attacks/__init__.py
+-rw-rw-r--  2.0 unx      119 b- defN 23-Jun-09 14:09 what/attacks/detection/__init__.py
+-rw-rw-r--  2.0 unx     3470 b- defN 23-Jun-01 13:53 what/attacks/detection/yolo/PCB.py
+-rw-rw-r--  2.0 unx     3518 b- defN 23-Jun-01 13:55 what/attacks/detection/yolo/TOG.py
+-rw-rw-r--  2.0 unx      399 b- defN 23-Jun-09 14:10 what/attacks/detection/yolo/__init__.py
+-rw-rw-r--  2.0 unx     1562 b- defN 23-Jun-09 14:14 what/examples/__init__.py
+-rw-rw-r--  2.0 unx     2723 b- defN 23-Jun-08 16:13 what/examples/faster_rcnn_demo.py
+-rw-rw-r--  2.0 unx     3237 b- defN 23-Jun-08 16:20 what/examples/mobilenet_ssd_demo.py
+-rw-rw-r--  2.0 unx     3027 b- defN 23-Jun-08 15:58 what/examples/yolov3_demo.py
+-rw-rw-r--  2.0 unx     4183 b- defN 23-Jun-08 19:16 what/examples/yolov3_pcb_attack_demo.py
+-rw-rw-r--  2.0 unx     4063 b- defN 23-Jun-08 19:16 what/examples/yolov3_tog_attack_demo.py
+-rw-rw-r--  2.0 unx     2999 b- defN 23-Jun-08 19:48 what/examples/yolov4_demo.py
+-rw-rw-r--  2.0 unx     1298 b- defN 23-Jun-09 14:03 what/models/__init__.py
+-rw-rw-r--  2.0 unx      310 b- defN 23-Jun-09 14:15 what/models/detection/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-09 16:07 what/models/detection/datasets/__init__.py
+-rw-rw-r--  2.0 unx     2466 b- defN 22-Jun-09 16:07 what/models/detection/datasets/coco.py
+-rw-rw-r--  2.0 unx     2664 b- defN 22-Jun-09 16:07 what/models/detection/datasets/fiftyone.py
+-rw-rw-r--  2.0 unx     4823 b- defN 22-Jun-09 16:07 what/models/detection/datasets/open_images.py
+-rw-rw-r--  2.0 unx     5154 b- defN 22-Jun-09 16:07 what/models/detection/datasets/voc.py
+-rw-rw-r--  2.0 unx      186 b- defN 23-Jun-09 14:19 what/models/detection/frcnn/__init__.py
+-rw-rw-r--  2.0 unx    10797 b- defN 22-Jun-09 16:07 what/models/detection/frcnn/faster_rcnn.py
+-rw-rw-r--  2.0 unx       95 b- defN 22-Jun-09 16:07 what/models/detection/frcnn/meter/__init__.py
+-rw-rw-r--  2.0 unx     1188 b- defN 22-Jun-09 16:07 what/models/detection/frcnn/meter/averagevalue_meter.py
+-rw-rw-r--  2.0 unx     3353 b- defN 22-Jun-09 16:07 what/models/detection/frcnn/meter/confusion_meter.py
+-rw-rw-r--  2.0 unx      544 b- defN 22-Jun-09 16:07 what/models/detection/frcnn/meter/meter.py
+-rw-rw-r--  2.0 unx      317 b- defN 23-Jun-09 14:19 what/models/detection/ssd/__init__.py
+-rw-rw-r--  2.0 unx     8042 b- defN 22-Jun-09 16:07 what/models/detection/ssd/mobilenet_v1_ssd.py
+-rw-rw-r--  2.0 unx     8112 b- defN 22-Jun-09 16:07 what/models/detection/ssd/mobilenet_v2_ssd_lite.py
+-rw-rw-r--  2.0 unx       62 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/__init__.py
+-rw-rw-r--  2.0 unx      648 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/mobilenet_ssd_config.py
+-rw-rw-r--  2.0 unx     3182 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py
+-rw-rw-r--  2.0 unx     3606 b- defN 23-Jun-01 14:09 what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py
+-rw-rw-r--  2.0 unx     3601 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py
+-rw-rw-r--  2.0 unx     5319 b- defN 23-Jun-01 14:09 what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py
+-rw-rw-r--  2.0 unx     1966 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/multibox_loss.py
+-rw-rw-r--  2.0 unx     3150 b- defN 22-Jun-20 18:22 what/models/detection/ssd/ssd/predictor.py
+-rw-rw-r--  2.0 unx     1773 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/preprocessing.py
+-rw-rw-r--  2.0 unx      617 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/squeezenet_ssd_config.py
+-rw-rw-r--  2.0 unx     3817 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py
+-rw-rw-r--  2.0 unx     7027 b- defN 22-Jun-09 16:07 what/models/detection/ssd/ssd/ssd.py
+-rw-rw-r--  2.0 unx       20 b- defN 22-Jun-09 16:07 what/models/detection/ssd/utils/__init__.py
+-rw-rw-r--  2.0 unx    10937 b- defN 22-Jun-09 16:07 what/models/detection/ssd/utils/box_utils.py
+-rw-rw-r--  2.0 unx      535 b- defN 22-Jun-09 16:07 what/models/detection/ssd/utils/misc.py
+-rw-rw-r--  2.0 unx      153 b- defN 22-Jun-09 16:07 what/models/detection/utils/__init__.py
+-rw-rw-r--  2.0 unx      589 b- defN 22-Jun-09 16:07 what/models/detection/utils/array_utils.py
+-rw-rw-r--  2.0 unx     1233 b- defN 22-Jun-20 17:46 what/models/detection/utils/box_utils.py
+-rw-rw-r--  2.0 unx      403 b- defN 22-Jun-09 16:07 what/models/detection/utils/time_utils.py
+-rw-rw-r--  2.0 unx      462 b- defN 23-Jun-09 14:19 what/models/detection/yolo/__init__.py
+-rw-rw-r--  2.0 unx      896 b- defN 22-Jun-09 16:07 what/models/detection/yolo/yolov3.py
+-rw-rw-r--  2.0 unx      911 b- defN 22-Jun-09 16:07 what/models/detection/yolo/yolov3_tiny.py
+-rw-rw-r--  2.0 unx     1040 b- defN 22-Jun-09 16:07 what/models/detection/yolo/yolov4.py
+-rw-rw-r--  2.0 unx     1101 b- defN 23-Jun-06 15:51 what/models/detection/yolo/yolov4_tiny.py
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jun-09 15:06 what/utils/__init__.py
+-rw-rw-r--  2.0 unx     2329 b- defN 23-Jun-05 20:33 what/utils/file.py
+-rw-rw-r--  2.0 unx     3522 b- defN 22-Jun-30 13:51 what/utils/logger.py
+-rw-rw-r--  2.0 unx      477 b- defN 22-Jun-21 20:00 what/utils/proj_lp.py
+-rw-rw-r--  2.0 unx     1054 b- defN 22-Jun-21 19:32 what/utils/resize.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-Jun-09 16:27 whitebox_adversarial_toolbox-0.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4583 b- defN 23-Jun-09 16:27 whitebox_adversarial_toolbox-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 16:27 whitebox_adversarial_toolbox-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       41 b- defN 23-Jun-09 16:27 whitebox_adversarial_toolbox-0.1.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-09 16:27 whitebox_adversarial_toolbox-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6300 b- defN 23-Jun-09 16:27 whitebox_adversarial_toolbox-0.1.0.dist-info/RECORD
+66 files, 161412 bytes uncompressed, 49567 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,28 +1,199 @@
 Filename: what/__init__.py
 Comment: 
 
+Filename: what/__main__.py
+Comment: 
+
+Filename: what/_main.py
+Comment: 
+
 Filename: what/attacks/__init__.py
 Comment: 
 
+Filename: what/attacks/detection/__init__.py
+Comment: 
+
+Filename: what/attacks/detection/yolo/PCB.py
+Comment: 
+
+Filename: what/attacks/detection/yolo/TOG.py
+Comment: 
+
+Filename: what/attacks/detection/yolo/__init__.py
+Comment: 
+
+Filename: what/examples/__init__.py
+Comment: 
+
+Filename: what/examples/faster_rcnn_demo.py
+Comment: 
+
+Filename: what/examples/mobilenet_ssd_demo.py
+Comment: 
+
+Filename: what/examples/yolov3_demo.py
+Comment: 
+
+Filename: what/examples/yolov3_pcb_attack_demo.py
+Comment: 
+
+Filename: what/examples/yolov3_tog_attack_demo.py
+Comment: 
+
+Filename: what/examples/yolov4_demo.py
+Comment: 
+
 Filename: what/models/__init__.py
 Comment: 
 
+Filename: what/models/detection/__init__.py
+Comment: 
+
+Filename: what/models/detection/datasets/__init__.py
+Comment: 
+
+Filename: what/models/detection/datasets/coco.py
+Comment: 
+
+Filename: what/models/detection/datasets/fiftyone.py
+Comment: 
+
+Filename: what/models/detection/datasets/open_images.py
+Comment: 
+
+Filename: what/models/detection/datasets/voc.py
+Comment: 
+
+Filename: what/models/detection/frcnn/__init__.py
+Comment: 
+
+Filename: what/models/detection/frcnn/faster_rcnn.py
+Comment: 
+
+Filename: what/models/detection/frcnn/meter/__init__.py
+Comment: 
+
+Filename: what/models/detection/frcnn/meter/averagevalue_meter.py
+Comment: 
+
+Filename: what/models/detection/frcnn/meter/confusion_meter.py
+Comment: 
+
+Filename: what/models/detection/frcnn/meter/meter.py
+Comment: 
+
+Filename: what/models/detection/ssd/__init__.py
+Comment: 
+
+Filename: what/models/detection/ssd/mobilenet_v1_ssd.py
+Comment: 
+
+Filename: what/models/detection/ssd/mobilenet_v2_ssd_lite.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/__init__.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/mobilenet_ssd_config.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/multibox_loss.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/predictor.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/preprocessing.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/squeezenet_ssd_config.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py
+Comment: 
+
+Filename: what/models/detection/ssd/ssd/ssd.py
+Comment: 
+
+Filename: what/models/detection/ssd/utils/__init__.py
+Comment: 
+
+Filename: what/models/detection/ssd/utils/box_utils.py
+Comment: 
+
+Filename: what/models/detection/ssd/utils/misc.py
+Comment: 
+
+Filename: what/models/detection/utils/__init__.py
+Comment: 
+
+Filename: what/models/detection/utils/array_utils.py
+Comment: 
+
+Filename: what/models/detection/utils/box_utils.py
+Comment: 
+
+Filename: what/models/detection/utils/time_utils.py
+Comment: 
+
+Filename: what/models/detection/yolo/__init__.py
+Comment: 
+
+Filename: what/models/detection/yolo/yolov3.py
+Comment: 
+
+Filename: what/models/detection/yolo/yolov3_tiny.py
+Comment: 
+
+Filename: what/models/detection/yolo/yolov4.py
+Comment: 
+
+Filename: what/models/detection/yolo/yolov4_tiny.py
+Comment: 
+
 Filename: what/utils/__init__.py
 Comment: 
 
-Filename: whitebox_adversarial_toolbox-0.0.1.dist-info/LICENSE
+Filename: what/utils/file.py
+Comment: 
+
+Filename: what/utils/logger.py
+Comment: 
+
+Filename: what/utils/proj_lp.py
+Comment: 
+
+Filename: what/utils/resize.py
+Comment: 
+
+Filename: whitebox_adversarial_toolbox-0.1.0.dist-info/LICENSE
+Comment: 
+
+Filename: whitebox_adversarial_toolbox-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: whitebox_adversarial_toolbox-0.0.1.dist-info/METADATA
+Filename: whitebox_adversarial_toolbox-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: whitebox_adversarial_toolbox-0.0.1.dist-info/WHEEL
+Filename: whitebox_adversarial_toolbox-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: whitebox_adversarial_toolbox-0.0.1.dist-info/top_level.txt
+Filename: whitebox_adversarial_toolbox-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: whitebox_adversarial_toolbox-0.0.1.dist-info/RECORD
+Filename: whitebox_adversarial_toolbox-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## what/__init__.py

```diff
@@ -1,16 +1,128 @@
-r'''
-WHite-box Adversarial Toolbox (WHAT) is a python library for Deep Learning Security that focuses on realtime white-box attacks.
-## what.models
-This module implements several object detection models.
-## what.attacks
-This module implements several white-box attacks against Deep Learning models.
-## what.utils
-This module implements several utility functions.
-'''
-
-# Project Imports
-from what import models
-from what import attacks
-
-# Semantic Version
-__version__ = "0.0.1"
+r'''
+WHite-box Adversarial Toolbox (WHAT) is a python library for Deep Learning Security that focuses on realtime white-box attacks.
+
+## Installation
+
+```
+pip install whitebox-adversarial-toolbox
+```
+
+Then you can use the cli tool `what` to try real-time adversarial attacks.
+
+```
+sage: what [OPTIONS] COMMAND [ARGS]...
+
+  The CLI tool for WHite-box Adversarial Toolbox (WHAT).
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  attack   Manage Attacks
+  example  Manage Examples
+  model    Manage Deep Learning Models
+```
+
+<br />
+
+## what.models
+
+Use `what model list` to list available models:
+
+```
+                Model                      Model Type           Description
+----------------------------------------------------------------------------------------------------
+[ ] 1 : YOLOv3      (    Darknet    )   Object Detection        YOLOv3 pretrained on MS COCO dataset.
+[ ] 2 : YOLOv3      (   Mobilenet   )   Object Detection        YOLOv3 pretrained on MS COCO dataset.
+[ ] 3 : YOLOv3 Tiny (    Darknet    )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
+[ ] 4 : YOLOv3 Tiny (   MobileNet   )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
+[ ] 5 : YOLOv4      (    Darknet    )   Object Detection        YOLOv4 pretrained on MS COCO dataset.
+[ ] 6 : YOLOv4 Tiny (    Darknet    )   Object Detection        YOLOv4 Tiny pretrained on MS COCO dataset.
+[ ] 7 : SSD         ( MobileNet  v1 )   Object Detection        SSD pretrained on VOC-2012 dataset.
+[ ] 8 : SSD         ( MobileNet  v2 )   Object Detection        SSD pretrained on VOC-2012 dataset.
+[ ] 9 : FasterRCNN  (     VGG16     )   Object Detection        Faster-RCNN pretrained on VOC-2012 dataset.
+```
+
+Use `what model download` to download pre-trained models:
+
+```
+                Model                      Model Type           Description
+----------------------------------------------------------------------------------------------------
+[x] 1 : YOLOv3      (    Darknet    )   Object Detection        YOLOv3 pretrained on MS COCO dataset.
+[x] 2 : YOLOv3      (   Mobilenet   )   Object Detection        YOLOv3 pretrained on MS COCO dataset.
+[x] 3 : YOLOv3 Tiny (    Darknet    )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
+[x] 4 : YOLOv3 Tiny (   MobileNet   )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
+[x] 5 : YOLOv4      (    Darknet    )   Object Detection        YOLOv4 pretrained on MS COCO dataset.
+[x] 6 : YOLOv4 Tiny (    Darknet    )   Object Detection        YOLOv4 Tiny pretrained on MS COCO dataset.
+[x] 7 : SSD         ( MobileNet  v1 )   Object Detection        SSD pretrained on VOC-2012 dataset.
+[x] 8 : SSD         ( MobileNet  v2 )   Object Detection        SSD pretrained on VOC-2012 dataset.
+[x] 9 : FasterRCNN  (     VGG16     )   Object Detection        Faster-RCNN pretrained on VOC-2012 dataset.
+
+Please input the model index: 
+```
+
+<br />
+
+## what.attacks
+
+Use `what attack list` to list available attacks:
+
+```
+1 : TOG Attack  Object Detection
+2 : PCB Attack  Object Detection
+```
+
+Related Papers:
+
+- [Adversarial Objectness Gradient Attacks in Real-time Object Detection Systems](https://ieeexplore.ieee.org/document/9325397).
+- [A Man-in-the-Middle Attack against Object Detection Systems](https://arxiv.org/abs/2208.07174).
+
+<br />
+
+## what.examples
+
+Use `what example list` to list available examples:
+
+```
+           Demo                Type             Description
+--------------------------------------------------------------------------------
+1 :     Yolov3 Demo      Model Inference        Yolov3 Object Detection.
+2 :     Yolov4 Demo      Model Inference        Yolov4 Object Detection.
+3 :   FasterRCNN Demo    Model Inference        FRCNN Object Detection.
+4 : MobileNet SSD Demo   Model Inference        MobileNet SSD Object Detection.
+5 :  TOG Attack Demo    Adversarial Attack      Real-time TOG Attack against Yolov3 Tiny.
+6 :  PCB Attack Demo    Adversarial Attack      Real-time PCB Attack against Yolov3 Tiny.
+```
+
+Use `what example run` to run examples.
+
+```
+           Demo                Type             Description
+--------------------------------------------------------------------------------
+1 :     Yolov3 Demo      Model Inference        Yolov3 Object Detection.
+2 :     Yolov4 Demo      Model Inference        Yolov4 Object Detection.
+3 :   FasterRCNN Demo    Model Inference        FRCNN Object Detection.
+4 : MobileNet SSD Demo   Model Inference        MobileNet SSD Object Detection.
+5 :  TOG Attack Demo    Adversarial Attack      Real-time TOG Attack against Yolov3 Tiny.
+6 :  PCB Attack Demo    Adversarial Attack      Real-time PCB Attack against Yolov3 Tiny.
+
+Please input the example index: 
+```
+
+<br />
+
+## what.utils
+
+This module implements several utility functions.
+
+<br />
+
+'''
+
+# Project Imports
+from what import models
+from what import attacks
+from what import utils
+
+# Semantic Version
+__version__ = "0.1.0"
```

## what/attacks/__init__.py

```diff
@@ -1,3 +1,24 @@
-r'''
-This module implements several white-box attacks against Deep Learning models.
-'''
+r'''
+This module implements several white-box attacks against Deep Learning models.
+
+Use `what attack list` to list available attacks:
+
+```
+1 : TOG Attack  Object Detection
+2 : PCB Attack  Object Detection
+```
+
+<br />
+
+## what.attacks.detection.yolo.PCB
+
+- [A Man-in-the-Middle Attack against Object Detection Systems](https://arxiv.org/abs/2208.07174).
+
+## what.attacks.detection.yolo.TOG
+
+- [Adversarial Objectness Gradient Attacks in Real-time Object Detection Systems](https://ieeexplore.ieee.org/document/9325397).
+
+'''
+
+from what.attacks.detection.yolo.PCB import PCBAttack
+from what.attacks.detection.yolo.TOG import TOGAttack
```

## what/models/__init__.py

```diff
@@ -1,4 +1,25 @@
-r'''
-This module implements several object detection models.
-```
-'''
+r'''
+This module implements several object detection models.
+
+
+Use `what model list` to list available models:
+
+```
+                Model                      Model Type           Description
+----------------------------------------------------------------------------------------------------
+[ ] 1 : YOLOv3      (    Darknet    )   Object Detection        YOLOv3 pretrained on MS COCO dataset.
+[ ] 2 : YOLOv3      (   Mobilenet   )   Object Detection        YOLOv3 pretrained on MS COCO dataset.
+[ ] 3 : YOLOv3 Tiny (    Darknet    )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
+[ ] 4 : YOLOv3 Tiny (   MobileNet   )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
+[ ] 5 : YOLOv4      (    Darknet    )   Object Detection        YOLOv4 pretrained on MS COCO dataset.
+[ ] 6 : YOLOv4 Tiny (    Darknet    )   Object Detection        YOLOv4 Tiny pretrained on MS COCO dataset.
+[ ] 7 : SSD         ( MobileNet  v1 )   Object Detection        SSD pretrained on VOC-2012 dataset.
+[ ] 8 : SSD         ( MobileNet  v2 )   Object Detection        SSD pretrained on VOC-2012 dataset.
+[ ] 9 : FasterRCNN  (     VGG16     )   Object Detection        Faster-RCNN pretrained on VOC-2012 dataset.
+```
+
+## what.models.detection
+
+'''
+
+from what.models import detection
```

## what/utils/__init__.py

```diff
@@ -1,3 +1,14 @@
-r'''
-Utility functions for WHAT.
-'''
+r'''
+Utility functions for WHAT.
+
+<br />
+
+## what.utils.logger.get_logger
+## what.utils.resize.bilinear_resize
+## what.utils.proj_lp.proj_lp
+
+'''
+
+from what.utils.logger import get_logger
+from what.utils.resize import bilinear_resize
+from what.utils.proj_lp import proj_lp
```

## Comparing `whitebox_adversarial_toolbox-0.0.1.dist-info/LICENSE` & `whitebox_adversarial_toolbox-0.1.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Wu Han
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Wu Han
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

