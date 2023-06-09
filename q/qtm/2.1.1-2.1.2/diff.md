# Comparing `tmp/qtm-2.1.1-py3-none-any.whl.zip` & `tmp/qtm-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 3108738 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      670 b- defN 21-Dec-02 09:57 qtm/__init__.py
--rw-rw-rw-  2.0 fat      651 b- defN 21-Dec-02 09:57 qtm/control.py
--rw-rw-rw-  2.0 fat     2893 b- defN 21-Dec-02 09:57 qtm/discovery.py
--rw-rw-rw-  2.0 fat    23488 b- defN 21-Dec-02 09:57 qtm/packet.py
--rw-rw-rw-  2.0 fat     5606 b- defN 21-Dec-02 09:57 qtm/protocol.py
--rw-rw-rw-  2.0 fat    13209 b- defN 21-Dec-02 09:57 qtm/qrt.py
--rw-rw-rw-  2.0 fat      890 b- defN 21-Dec-02 09:57 qtm/reboot.py
--rw-rw-rw-  2.0 fat     1507 b- defN 21-Dec-02 09:57 qtm/receiver.py
--rw-rw-rw-  2.0 fat  4259840 b- defN 21-Dec-02 09:57 qtm/data/demo.qtm
--rw-rw-rw-  2.0 fat     1080 b- defN 21-Dec-02 10:03 qtm-2.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      739 b- defN 21-Dec-02 10:03 qtm-2.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 21-Dec-02 10:03 qtm-2.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 21-Dec-02 10:03 qtm-2.1.1.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 21-Dec-02 10:03 qtm-2.1.1.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1089 b- defN 21-Dec-02 10:03 qtm-2.1.1.dist-info/RECORD
-15 files, 4311760 bytes uncompressed, 3106986 bytes compressed:  27.9%
+Zip file size: 3108915 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat      700 b- defN 23-Jun-09 15:07 qtm/__init__.py
+-rw-rw-rw-  2.0 fat      674 b- defN 23-Jun-09 15:07 qtm/control.py
+-rw-rw-rw-  2.0 fat     2991 b- defN 23-Jun-09 15:07 qtm/discovery.py
+-rw-rw-rw-  2.0 fat    24138 b- defN 23-Jun-09 15:07 qtm/packet.py
+-rw-rw-rw-  2.0 fat     5970 b- defN 23-Jun-09 15:07 qtm/protocol.py
+-rw-rw-rw-  2.0 fat    13609 b- defN 23-Jun-09 15:07 qtm/qrt.py
+-rw-rw-rw-  2.0 fat      925 b- defN 23-Jun-09 15:07 qtm/reboot.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-Jun-09 15:07 qtm/receiver.py
+-rw-rw-rw-  2.0 fat  4259840 b- defN 23-Jun-09 15:07 qtm/data/demo.qtm
+-rw-rw-rw-  2.0 fat     1101 b- defN 23-Jun-09 15:10 qtm-2.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      792 b- defN 23-Jun-09 15:10 qtm-2.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-09 15:10 qtm-2.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-09 15:10 qtm-2.1.2.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-09 15:09 qtm-2.1.2.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1089 b- defN 23-Jun-09 15:10 qtm-2.1.2.dist-info/RECORD
+15 files, 4313485 bytes uncompressed, 3107163 bytes compressed:  28.0%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: qtm/receiver.py
 Comment: 
 
 Filename: qtm/data/demo.qtm
 Comment: 
 
-Filename: qtm-2.1.1.dist-info/LICENSE
+Filename: qtm-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: qtm-2.1.1.dist-info/METADATA
+Filename: qtm-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: qtm-2.1.1.dist-info/WHEEL
+Filename: qtm-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: qtm-2.1.1.dist-info/top_level.txt
+Filename: qtm-2.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: qtm-2.1.1.dist-info/zip-safe
+Filename: qtm-2.1.2.dist-info/zip-safe
 Comment: 
 
-Filename: qtm-2.1.1.dist-info/RECORD
+Filename: qtm-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qtm/__init__.py

 * *Ordering differences only*

```diff
@@ -1,30 +1,30 @@
-""" Python SDK for QTM """
-
-import logging
-import sys
-import os
-
-PYTHON3 = sys.version_info.major == 3
-
-if PYTHON3:
-    from .discovery import Discover
-    from .reboot import reboot
-    from .qrt import connect, QRTConnection
-    from .protocol import QRTCommandException
-    from .control import TakeControl
-
-from .packet import QRTPacket, QRTEvent
-from .receiver import Receiver
-
-# pylint: disable=C0330
-
-LOG = logging.getLogger("qtm")
-LOG_LEVEL = os.getenv("QTM_LOGGING", None)
-
-LEVEL = logging.DEBUG if LOG_LEVEL == "debug" else logging.INFO
-logging.basicConfig(
-    level=LEVEL, format="%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-)
-
-
-__author__ = "mge"
+""" Python SDK for QTM """
+
+import logging
+import sys
+import os
+
+PYTHON3 = sys.version_info.major == 3
+
+if PYTHON3:
+    from .discovery import Discover
+    from .reboot import reboot
+    from .qrt import connect, QRTConnection
+    from .protocol import QRTCommandException
+    from .control import TakeControl
+
+from .packet import QRTPacket, QRTEvent
+from .receiver import Receiver
+
+# pylint: disable=C0330
+
+LOG = logging.getLogger("qtm")
+LOG_LEVEL = os.getenv("QTM_LOGGING", None)
+
+LEVEL = logging.DEBUG if LOG_LEVEL == "debug" else logging.INFO
+logging.basicConfig(
+    level=LEVEL, format="%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+)
+
+
+__author__ = "mge"
```

## qtm/control.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-import asyncio
-import logging
-
-from .qrt import QRTConnection
-
-LOG = logging.getLogger("qtm")
-
-
-class TakeControl:
-    """ Context manager for taking control and releasing control of QTM """
-
-    def __init__(self, connection: QRTConnection, password: str):
-        self.connection = connection
-        self.password = password
-
-    async def __aenter__(self):
-        await self.connection.take_control(self.password)
-        LOG.info("Took control")
-
-    async def __aexit__(self, exc_type, exc, _):
-        if self.connection.has_transport() is not None:
-            await self.connection.release_control()
-            LOG.info("Released control")
+import asyncio
+import logging
+
+from .qrt import QRTConnection
+
+LOG = logging.getLogger("qtm")
+
+
+class TakeControl:
+    """ Context manager for taking control and releasing control of QTM """
+
+    def __init__(self, connection: QRTConnection, password: str):
+        self.connection = connection
+        self.password = password
+
+    async def __aenter__(self):
+        await self.connection.take_control(self.password)
+        LOG.info("Took control")
+
+    async def __aexit__(self, exc_type, exc, _):
+        if self.connection.has_transport() is not None:
+            await self.connection.release_control()
+            LOG.info("Released control")
```

## qtm/discovery.py

 * *Ordering differences only*

```diff
@@ -1,98 +1,98 @@
-""" Implementation of QTM discovery protocol """
-
-import struct
-import asyncio
-from collections import namedtuple
-import logging
-
-from .protocol import RTheader, QRTPacketType
-
-# pylint: disable=C0103
-
-LOG = logging.getLogger("qtm")
-
-QRTDiscoveryP1 = struct.Struct("<II")
-QRTDiscoveryP2 = struct.Struct(">H")
-QRTDiscoveryPacketSize = QRTDiscoveryP1.size + QRTDiscoveryP2.size
-QRTDiscoveryBasePort = struct.Struct(">H")
-
-QRTDiscoveryResponse = namedtuple("QRTDiscoveryResponse", "info host port")
-
-class QRTDiscoveryProtocol:
-    """ Oqus/Miqus/Arqus discovery protocol implementation"""
-
-    def __init__(self, receiver=None):
-        self.port = None
-        self.receiver = receiver
-        self.transport = None
-
-    def connection_made(self, transport):
-        """ On socket creation """
-        self.transport = transport
-
-        sock = transport.get_extra_info("socket")
-        self.port = sock.getsockname()[1]
-
-    def datagram_received(self, datagram, address):
-        """ Parse response from QTM instances """
-        size, _ = RTheader.unpack_from(datagram, 0)
-        info, = struct.unpack_from("{0}s".format(size - 3 - 8), datagram, RTheader.size)
-        base_port, = QRTDiscoveryBasePort.unpack_from(datagram, size - 2)
-
-        if self.receiver is not None:
-            self.receiver(QRTDiscoveryResponse(info, address[0], base_port))
-
-    def send_discovery_packet(self):
-        """ Send discovery packet for QTM to respond to """
-        if self.port is None:
-            return
-
-        self.transport.sendto(
-            QRTDiscoveryP1.pack(
-                QRTDiscoveryPacketSize, QRTPacketType.PacketDiscover.value
-            )
-            + QRTDiscoveryP2.pack(self.port),
-            ("<broadcast>", 22226),
-        )
-
-class Discover:
-    """async discovery of qtm instances"""
-
-    def __init__(self, ip_address):
-        self.ip_address = ip_address
-        self.queue = asyncio.Queue()
-        self.first = True
-
-    def __aiter__(self):
-        return self
-
-    async def __anext__(self) -> QRTDiscoveryResponse:
-
-        loop = asyncio.get_event_loop()
-        if self.first:
-
-            protocol_factory = lambda: QRTDiscoveryProtocol(
-                receiver=self.queue.put_nowait
-            )
-
-            _, protocol = await loop.create_datagram_endpoint(
-                protocol_factory,
-                local_addr=(self.ip_address, 0),
-                allow_broadcast=True,
-            )
-
-            LOG.debug("Sending discovery packet on %s", self.ip_address)
-            protocol.send_discovery_packet()
-            self.first = False
-
-        call_handle = loop.call_later(0.2, lambda: self.queue.put_nowait(None))
-        result = await self.queue.get()
-        if result is None:
-            LOG.debug("Discovery timed out")
-            raise StopAsyncIteration
-
-        LOG.debug(result)
-        call_handle.cancel()
-        return result
-
-
+""" Implementation of QTM discovery protocol """
+
+import struct
+import asyncio
+from collections import namedtuple
+import logging
+
+from .protocol import RTheader, QRTPacketType
+
+# pylint: disable=C0103
+
+LOG = logging.getLogger("qtm")
+
+QRTDiscoveryP1 = struct.Struct("<II")
+QRTDiscoveryP2 = struct.Struct(">H")
+QRTDiscoveryPacketSize = QRTDiscoveryP1.size + QRTDiscoveryP2.size
+QRTDiscoveryBasePort = struct.Struct(">H")
+
+QRTDiscoveryResponse = namedtuple("QRTDiscoveryResponse", "info host port")
+
+class QRTDiscoveryProtocol:
+    """ Oqus/Miqus/Arqus discovery protocol implementation"""
+
+    def __init__(self, receiver=None):
+        self.port = None
+        self.receiver = receiver
+        self.transport = None
+
+    def connection_made(self, transport):
+        """ On socket creation """
+        self.transport = transport
+
+        sock = transport.get_extra_info("socket")
+        self.port = sock.getsockname()[1]
+
+    def datagram_received(self, datagram, address):
+        """ Parse response from QTM instances """
+        size, _ = RTheader.unpack_from(datagram, 0)
+        info, = struct.unpack_from("{0}s".format(size - 3 - 8), datagram, RTheader.size)
+        base_port, = QRTDiscoveryBasePort.unpack_from(datagram, size - 2)
+
+        if self.receiver is not None:
+            self.receiver(QRTDiscoveryResponse(info, address[0], base_port))
+
+    def send_discovery_packet(self):
+        """ Send discovery packet for QTM to respond to """
+        if self.port is None:
+            return
+
+        self.transport.sendto(
+            QRTDiscoveryP1.pack(
+                QRTDiscoveryPacketSize, QRTPacketType.PacketDiscover.value
+            )
+            + QRTDiscoveryP2.pack(self.port),
+            ("<broadcast>", 22226),
+        )
+
+class Discover:
+    """async discovery of qtm instances"""
+
+    def __init__(self, ip_address):
+        self.ip_address = ip_address
+        self.queue = asyncio.Queue()
+        self.first = True
+
+    def __aiter__(self):
+        return self
+
+    async def __anext__(self) -> QRTDiscoveryResponse:
+
+        loop = asyncio.get_event_loop()
+        if self.first:
+
+            protocol_factory = lambda: QRTDiscoveryProtocol(
+                receiver=self.queue.put_nowait
+            )
+
+            _, protocol = await loop.create_datagram_endpoint(
+                protocol_factory,
+                local_addr=(self.ip_address, 0),
+                allow_broadcast=True,
+            )
+
+            LOG.debug("Sending discovery packet on %s", self.ip_address)
+            protocol.send_discovery_packet()
+            self.first = False
+
+        call_handle = loop.call_later(0.2, lambda: self.queue.put_nowait(None))
+        result = await self.queue.get()
+        if result is None:
+            LOG.debug("Discovery timed out")
+            raise StopAsyncIteration
+
+        LOG.debug(result)
+        call_handle.cancel()
+        return result
+
+
```

## qtm/packet.py

 * *Ordering differences only*

```diff
@@ -1,650 +1,650 @@
-""" Definition of packets and binary formats from QTM """
-
-from collections import namedtuple
-from functools import wraps
-import struct
-
-from enum import Enum
-
-# pylint: disable=C0103, C0330, E1101, W0212
-
-# Used in protocol
-RTheader = struct.Struct("<II")
-RTEvent = struct.Struct("<c")
-
-RTCommand = "<II%dsc"
-
-# Base
-RTDataQRTPacket = struct.Struct("<qII")
-RTComponentData = struct.Struct("<II")
-
-# 2D
-RT2DComponent = namedtuple("RT2DComponent", "camera_count drop_rate out_of_sync_rate")
-RT2DComponent.format = struct.Struct("<Ihh")
-
-RT2DCamera = namedtuple("RT2DCamera", "marker_count status_flag")
-RT2DCamera.format = struct.Struct("<ic")
-
-RT2DMarker = namedtuple("RT2DMarker", "x y d_x d_y")
-RT2DMarker.format = struct.Struct("<iihh")
-
-# 3D
-RT3DComponent = namedtuple("RT3DComponent", "marker_count drop_rate out_of_sync_rate")
-RT3DComponent.format = struct.Struct("<Ihh")
-
-RT3DMarkerPosition = namedtuple("RT3DMarkerPosition", "x y z")
-RT3DMarkerPosition.format = struct.Struct("<3f")
-
-RT3DMarkerPositionResidual = namedtuple("RT3DMarkerPositionResidual", "x y z residual")
-RT3DMarkerPositionResidual.format = struct.Struct("<4f")
-
-RT3DMarkerPositionNoLabel = namedtuple("RT3DMarkerPositionNoLabel", "x y z id")
-RT3DMarkerPositionNoLabel.format = struct.Struct("<3fi")
-
-RT3DMarkerPositionNoLabelResidual = namedtuple(
-    "RT3DMarkerPositionNoLabelResidual", "x y z id residual"
-)
-RT3DMarkerPositionNoLabelResidual.format = struct.Struct("<3fif")
-
-# 6D
-RT6DComponent = namedtuple("RT6DComponent", "body_count drop_rate out_of_sync_rate")
-RT6DComponent.format = struct.Struct("<ihh")
-
-RT6DBodyPosition = namedtuple("RT6DBodyPosition", "x y z")
-RT6DBodyPosition.format = struct.Struct("<3f")
-
-RT6DBodyRotation = namedtuple("RT6DBodyRotation", "matrix")
-RT6DBodyRotation.format = struct.Struct("<9f")
-
-RT6DBodyResidual = namedtuple("RT6DBodyResidual", "residual")
-RT6DBodyResidual.format = struct.Struct("<f")
-
-RT6DBodyEuler = namedtuple("RT6DBodyEuler", "a1 a2 a3")
-RT6DBodyEuler.format = struct.Struct("<3f")
-
-# Analog
-RTAnalogComponent = namedtuple("RTAnalogComponent", "device_count")
-RTAnalogComponent.format = struct.Struct("<i")
-
-RTAnalogDevice = namedtuple("RTAnalogDevice", "id channel_count sample_count")
-RTAnalogDevice.format = struct.Struct("<iii")
-
-RTSampleNumber = namedtuple("RTSampleNumber", "sample_number")
-RTSampleNumber.format = struct.Struct("<i")
-
-RTAnalogChannel = namedtuple("RTAnalogChannel", "samples")
-RTAnalogChannel.format_str = "<%df"
-
-RTAnalogDeviceSingle = namedtuple("RTAnalogDeviceSingle", "id channel_count")
-RTAnalogDeviceSingle.format = struct.Struct("<ii")
-
-RTAnalogDeviceSamples = namedtuple("RTAnalogDeviceSamples", "samples")
-RTAnalogDeviceSamples.format_str = "<%df"
-
-# Force
-RTForceComponent = namedtuple("RTForceComponent", "plate_count")
-RTForceComponent.format = struct.Struct("<i")
-
-RTForcePlate = namedtuple("RTForcePlate", "id force_count force_number")
-RTForcePlate.format = struct.Struct("<iii")
-
-RTForcePlateSingle = namedtuple("RTForcePlateSingle", "id")
-RTForcePlateSingle.format = struct.Struct("<i")
-
-RTForce = namedtuple("RTForce", "x y z x_m y_m z_m x_a y_a z_a")
-RTForce.format = struct.Struct("<9f")
-
-# GazeVector
-RTGazeVectorComponent = namedtuple("RTGazeVectorComponent", "vector_count")
-RTGazeVectorComponent.format = struct.Struct("<i")
-
-RTGazeVectorInfo = namedtuple("RTGazeVectorInfo", "sample_count sample_number")
-RTGazeVectorInfo.format = struct.Struct("<ii")
-
-RTGazeVectorUnitVector = namedtuple("RTGazeVectorUnitVector", "x y z")
-RTGazeVectorUnitVector.format = struct.Struct("<3f")
-
-RTGazeVectorPosition = namedtuple("RTGazeVectorPosition", "x y z")
-RTGazeVectorPosition.format = struct.Struct("<3f")
-
-# EyeTracker
-RTEyeTrackerComponent = namedtuple("RTEyeTrackerComponent", "eye_tracker_count")
-RTEyeTrackerComponent.format = struct.Struct("<i")
-
-RTEyeTrackerInfo = namedtuple("RTEyeTrackerInfo", "sample_count sample_number")
-RTEyeTrackerInfo.format = struct.Struct("<ii")
-
-RTEyeTrackerDiameter = namedtuple("RTEyeTrackerDiameter", "left right")
-RTEyeTrackerDiameter.format = struct.Struct("<ff")
-
-# Image
-RTImageComponent = namedtuple("RTImageComponent", "image_count")
-RTImageComponent.format = struct.Struct("<i")
-
-# Skeleton
-RTSkeletonComponent = namedtuple("RTSkeletonComponent", "skeleton_count")
-RTSkeletonComponent.format = struct.Struct("<i")
-
-RTSegmentCount = namedtuple("RTSegmentCount", "segment_count")
-RTSegmentCount.format = struct.Struct("<i")
-
-RTSegmentId = namedtuple("RTSegmentId", "id")
-RTSegmentId.format = struct.Struct("<i")
-
-RTSegmentPosition = namedtuple("RTSegmentPosition", "x y z")
-RTSegmentPosition.format = struct.Struct("<3f")
-
-RTSegmentRotation = namedtuple("RTSegmentRotation", "x y z w")
-RTSegmentRotation.format = struct.Struct("<4f")
-
-RTImage = namedtuple(
-    "RTImage",
-    "id format width height left_crop top_crop right_crop bottom_crop image_size",
-)
-RTImage.format = struct.Struct("<iiiiffffi")
-
-# Time
-
-RTTimeComponent = namedtuple("RTTimeComponent", "timecode_count")
-RTTimeComponent.format = struct.Struct("<i")
-
-RTTime = namedtuple("RTTime", "type hi lo")
-RTTime.format = struct.Struct("<iII")
-
-
-class QRTPacketType(Enum):
-    """ Packet types """
-
-    PacketError = 0
-    PacketCommand = 1
-    PacketXML = 2
-    PacketData = 3
-    PacketNoMoreData = 4
-    PacketC3DFile = 5
-    PacketEvent = 6
-    PacketDiscover = 7
-    PacketQTMFile = 8
-    PacketNone = 9
-
-
-class QRTComponentType(Enum):
-    """ QTM Component types """
-
-    Component3d = 1
-    Component3dNoLabels = 2
-    ComponentAnalog = 3
-    ComponentForce = 4
-    Component6d = 5
-    Component6dEuler = 6
-    Component2d = 7
-    Component2dLin = 8
-    Component3dRes = 9
-    Component3dNoLabelsRes = 10
-    Component6dRes = 11
-    Component6dEulerRes = 12
-    ComponentAnalogSingle = 13
-    ComponentImage = 14
-    ComponentForceSingle = 15
-    ComponentGazeVector = 16
-    ComponentTimecode = 17
-    ComponentSkeleton = 18
-    ComponentEyeTracker = 19
-
-
-class QRTImageFormat(Enum):
-    """ QTM Image formats """
-
-    FormatRawGrayscale = 0
-    FormatRawBGR = 1
-    FormatJPG = 2
-    FormatPNG = 3
-
-
-class QRTEvent(Enum):
-    """ QTM Event types """
-
-    EventConnected = 1
-    EventConnectionClosed = 2
-    EventCaptureStarted = 3
-    EventCaptureStopped = 4
-    EventCaptureFetchingFinished = 5  # Not used in version 1.10 and later
-    EventCalibrationStarted = 6
-    EventCalibrationStopped = 7
-    EventRTfromFileStarted = 8
-    EventRTfromFileStopped = 9
-    EventWaitingForTrigger = 10
-    EventCameraSettingsChanged = 11
-    EventQTMShuttingDown = 12
-    EventCaptureSaved = 13
-    EventReprocessingStarted = 14
-    EventReprocessingStopped = 15
-    EventTrigger = 16
-    EventNone = (
-        17
-    )  # Must be the last. Not actually an event. Just used to count number of events.
-
-
-class ComponentGetter(object):
-    """ Helper decorator for extracting correct packet data based on type """
-
-    def __init__(self, component_enum, base_component):
-        self.component_enum = component_enum
-        self.base_component = base_component
-
-    def __call__(self, function):
-        @wraps(function)
-        def wrapper(*args, **kwargs):
-            calling_object = args[0]
-            component_position = calling_object.components.get(
-                self.component_enum, None
-            )
-            if component_position is None:
-                return None
-
-            component_position, component_info = QRTPacket._get_exact(
-                self.base_component, calling_object.data, component_position
-            )
-
-            return (
-                component_info,
-                function(
-                    *args,
-                    component_info=component_info,
-                    data=calling_object.data,
-                    component_position=component_position,
-                    **kwargs
-                ),
-            )
-
-        return wrapper
-
-
-# noinspection PyTypeChecker
-class QRTPacket(object):
-    """Packet containing data measured with QTM.
-
-    Too check for existence of a specific component in a packet:
-
-    ::
-
-        from qtm.packet import QRTComponentType
-        if QRTComponentType.Component3d in packet.components:
-            header, markers = packet.get_3d_markers()
-
-    Component retriever functions will return None if a component is not in the packet.
-
-    """
-
-    def __init__(self, data):
-        self.data = data
-
-        self.timestamp, self.framenumber, component_count = RTDataQRTPacket.unpack_from(
-            data, 0
-        )
-
-        self.components = {}
-        position = RTDataQRTPacket.size
-        for _ in range(component_count):
-            c_size, c_type = RTComponentData.unpack_from(data, position)
-            self.components[QRTComponentType(c_type)] = position + RTComponentData.size
-            position += c_size
-
-    @staticmethod
-    def _get_exact(component_type, data, position):
-        value = component_type._make(component_type.format.unpack_from(data, position))
-        position += component_type.format.size
-        return position, value
-
-    @staticmethod
-    def _get_tuple(component_type, data, position):
-        value = component_type._make(
-            [component_type.format.unpack_from(data, position)]
-        )
-        position += component_type.format.size
-        return position, value
-
-    @staticmethod
-    def _get_2d_markers(data, component_info, component_position, index=None):
-        components = []
-        append_components = components.append
-        for camera in range(component_info.camera_count):
-            component_position, camera_info = QRTPacket._get_exact(
-                RT2DCamera, data, component_position
-            )
-
-            if index is None or index == camera:
-                marker_list = []
-                append_marker = marker_list.append
-                append_components(marker_list)
-
-                for _ in range(camera_info.marker_count):
-                    component_position, marker = QRTPacket._get_exact(
-                        RT2DMarker, data, component_position
-                    )
-                    append_marker(marker)
-            else:
-                component_position += RT2DMarker.format.size * camera_info.marker_count
-
-        return components
-
-    @staticmethod
-    def _get_3d_markers(type_, component_info, data, component_position):
-        components = []
-        append_components = components.append
-        for _ in range(component_info.marker_count):
-            component_position, position = QRTPacket._get_exact(
-                type_, data, component_position
-            )
-            append_components(position)
-
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentTimecode, RTTimeComponent)
-    def get_timecode(self, component_info=None, data=None, component_position=None):
-        components = []
-        append_components = components.append
-        for _ in range(component_info.timecode_count):
-            time_component, timecode = QRTPacket._get_exact(
-                RTTime, data, component_position)
-            append_components(timecode)
-
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentAnalog, RTAnalogComponent)
-    def get_analog(self, component_info=None, data=None, component_position=None):
-        """Get analog data."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.device_count):
-            component_position, device = QRTPacket._get_exact(
-                RTAnalogDevice, data, component_position
-            )
-            if device.sample_count > 0:
-                component_position, sample_number = QRTPacket._get_exact(
-                    RTSampleNumber, data, component_position
-                )
-
-                RTAnalogChannel.format = struct.Struct(
-                    RTAnalogChannel.format_str % device.sample_count
-                )
-                for _ in range(device.channel_count):
-                    component_position, channel = QRTPacket._get_tuple(
-                        RTAnalogChannel, data, component_position
-                    )
-                    append_components((device, sample_number, channel))
-
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentAnalogSingle, RTAnalogComponent)
-    def get_analog_single(
-        self, component_info=None, data=None, component_position=None
-    ):
-        """Get a single analog data channel."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.device_count):
-            component_position, device = QRTPacket._get_exact(
-                RTAnalogDeviceSingle, data, component_position
-            )
-
-            RTAnalogDeviceSamples.format = struct.Struct(
-                RTAnalogDeviceSamples.format_str % device.channel_count
-            )
-            component_position, sample = QRTPacket._get_tuple(
-                RTAnalogDeviceSamples, data, component_position
-            )
-            append_components((device, sample))
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentForce, RTForceComponent)
-    def get_force(self, component_info=None, data=None, component_position=None):
-        """Get force data."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.plate_count):
-            component_position, plate = QRTPacket._get_exact(
-                RTForcePlate, data, component_position
-            )
-            force_list = []
-            for _ in range(plate.force_count):
-                component_position, force = QRTPacket._get_exact(
-                    RTForce, data, component_position
-                )
-                force_list.append(force)
-            append_components((plate, force_list))
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentForceSingle, RTForceComponent)
-    def get_force_single(self, component_info=None, data=None, component_position=None):
-        """Get a single force data channel."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.plate_count):
-            component_position, plate = QRTPacket._get_exact(
-                RTForcePlateSingle, data, component_position
-            )
-            component_position, force = QRTPacket._get_exact(
-                RTForce, data, component_position
-            )
-            append_components((plate, force))
-        return components
-
-    @ComponentGetter(QRTComponentType.Component6d, RT6DComponent)
-    def get_6d(self, component_info=None, data=None, component_position=None):
-        """Get 6D data."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.body_count):
-            component_position, position = QRTPacket._get_exact(
-                RT6DBodyPosition, data, component_position
-            )
-            component_position, matrix = QRTPacket._get_tuple(
-                RT6DBodyRotation, data, component_position
-            )
-            append_components((position, matrix))
-        return components
-
-    @ComponentGetter(QRTComponentType.Component6dRes, RT6DComponent)
-    def get_6d_residual(self, component_info=None, data=None, component_position=None):
-        """Get 6D data with residual."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.body_count):
-            component_position, position = QRTPacket._get_exact(
-                RT6DBodyPosition, data, component_position
-            )
-            component_position, matrix = QRTPacket._get_tuple(
-                RT6DBodyRotation, data, component_position
-            )
-            component_position, residual = QRTPacket._get_exact(
-                RT6DBodyResidual, data, component_position
-            )
-            append_components((position, matrix, residual))
-        return components
-
-    @ComponentGetter(QRTComponentType.Component6dEuler, RT6DComponent)
-    def get_6d_euler(self, component_info=None, data=None, component_position=None):
-        """Get 6D data with euler rotations."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.body_count):
-            component_position, position = QRTPacket._get_exact(
-                RT6DBodyPosition, data, component_position
-            )
-            component_position, euler = QRTPacket._get_exact(
-                RT6DBodyEuler, data, component_position
-            )
-            append_components((position, euler))
-        return components
-
-    @ComponentGetter(QRTComponentType.Component6dEulerRes, RT6DComponent)
-    def get_6d_euler_residual(
-        self, component_info=None, data=None, component_position=None
-    ):
-        """Get 6D data with residuals and euler rotations."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.body_count):
-            component_position, position = QRTPacket._get_exact(
-                RT6DBodyPosition, data, component_position
-            )
-            component_position, euler = QRTPacket._get_exact(
-                RT6DBodyEuler, data, component_position
-            )
-            component_position, residual = QRTPacket._get_exact(
-                RT6DBodyResidual, data, component_position
-            )
-            append_components((position, euler, residual))
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentImage, RTImageComponent)
-    def get_image(self, component_info=None, data=None, component_position=None):
-        """Get image."""
-        components = []
-        append_components = components.append
-        for _ in range(component_info.image_count):
-            component_position, image_info = QRTPacket._get_exact(
-                RTImage, data, component_position
-            )
-            append_components((image_info, data[component_position:component_position + image_info.image_size]))
-            component_position += image_info.image_size
-        return components
-
-    @ComponentGetter(QRTComponentType.Component3d, RT3DComponent)
-    def get_3d_markers(self, component_info=None, data=None, component_position=None):
-        """Get 3D markers."""
-        return self._get_3d_markers(
-            RT3DMarkerPosition, component_info, data, component_position
-        )
-
-    @ComponentGetter(QRTComponentType.Component3dRes, RT3DComponent)
-    def get_3d_markers_residual(
-        self, component_info=None, data=None, component_position=None
-    ):
-        """Get 3D markers with residual."""
-        return self._get_3d_markers(
-            RT3DMarkerPositionResidual, component_info, data, component_position
-        )
-
-    @ComponentGetter(QRTComponentType.Component3dNoLabels, RT3DComponent)
-    def get_3d_markers_no_label(
-        self, component_info=None, data=None, component_position=None
-    ):
-        """Get 3D markers without label."""
-        return self._get_3d_markers(
-            RT3DMarkerPositionNoLabel, component_info, data, component_position
-        )
-
-    @ComponentGetter(QRTComponentType.Component3dNoLabelsRes, RT3DComponent)
-    def get_3d_markers_no_label_residual(
-        self, component_info=None, data=None, component_position=None
-    ):
-        """Get 3D markers without label with residual."""
-        return self._get_3d_markers(
-            RT3DMarkerPositionNoLabelResidual, component_info, data, component_position
-        )
-
-    @ComponentGetter(QRTComponentType.Component2d, RT2DComponent)
-    def get_2d_markers(
-        self, component_info=None, data=None, component_position=None, index=None
-    ):
-        """Get 2D markers.
-
-        :param index: Specify which camera to get 2D from, will be returned as
-                      first entry in the returned array.
-        """
-        return self._get_2d_markers(
-            data, component_info, component_position, index=index
-        )
-
-    @ComponentGetter(QRTComponentType.Component2dLin, RT2DComponent)
-    def get_2d_markers_linearized(
-        self, component_info=None, data=None, component_position=None, index=None
-    ):
-        """Get 2D linearized markers.
-
-        :param index: Specify which camera to get 2D from, will be returned as
-                      first entry in the returned array.
-        """
-
-        return self._get_2d_markers(
-            data, component_info, component_position, index=index
-        )
-
-    @ComponentGetter(QRTComponentType.ComponentSkeleton, RTSkeletonComponent)
-    def get_skeletons(self, component_info=None, data=None, component_position=None):
-        """Get skeletons
-        """
-
-        components = []
-        append_components = components.append
-        for _ in range(component_info.skeleton_count):
-            component_position, info = QRTPacket._get_exact(
-                RTSegmentCount, data, component_position
-            )
-
-            segments = []
-            for __ in range(info.segment_count):
-                component_position, segment = QRTPacket._get_exact(
-                    RTSegmentId, data, component_position
-                )
-                component_position, position = QRTPacket._get_exact(
-                    RTSegmentPosition, data, component_position
-                )
-                component_position, rotation = QRTPacket._get_exact(
-                    RTSegmentRotation, data, component_position
-                )
-
-                segments.append((segment.id, position, rotation))
-            append_components(segments)
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentGazeVector, RTGazeVectorComponent)
-    def get_gaze_vectors(self, component_info=None, data=None, component_position=None):
-        """Get gaze vectors
-        """
-        
-        components = []
-        append_components = components.append
-        for _ in range(component_info.vector_count):
-            component_position, info = QRTPacket._get_exact(
-                RTGazeVectorInfo, data, component_position)
-            
-            samples = []
-            if info.sample_count > 0:
-                for _ in range(info.sample_count):
-                    component_position, unit_vector = QRTPacket._get_exact(
-                        RTGazeVectorUnitVector, data, component_position)
-
-                    component_position, position = QRTPacket._get_exact(
-                        RTGazeVectorPosition, data, component_position)
-
-                    samples.append((unit_vector, position))
-
-            append_components((info, samples))
-
-        return components
-
-    @ComponentGetter(QRTComponentType.ComponentEyeTracker, RTEyeTrackerComponent)
-    def get_eye_trackers(self, component_info=None, data=None, component_position=None):
-        """Get eye trackers
-        """
-
-        components = []
-        append_components = components.append
-        for _ in range(component_info.eye_tracker_count):
-            component_position, info = QRTPacket._get_exact(
-                RTEyeTrackerInfo, data, component_position)
-            
-            samples = []
-            if info.sample_count > 0:
-                for _ in range(info.sample_count):
-                    component_position, diameter = QRTPacket._get_exact(
-                        RTEyeTrackerDiameter, data, component_position
-                    )
-                    samples.append(diameter)
-
-            append_components((info, samples))
-
-        return components
-
+""" Definition of packets and binary formats from QTM """
+
+from collections import namedtuple
+from functools import wraps
+import struct
+
+from enum import Enum
+
+# pylint: disable=C0103, C0330, E1101, W0212
+
+# Used in protocol
+RTheader = struct.Struct("<II")
+RTEvent = struct.Struct("<c")
+
+RTCommand = "<II%dsc"
+
+# Base
+RTDataQRTPacket = struct.Struct("<qII")
+RTComponentData = struct.Struct("<II")
+
+# 2D
+RT2DComponent = namedtuple("RT2DComponent", "camera_count drop_rate out_of_sync_rate")
+RT2DComponent.format = struct.Struct("<Ihh")
+
+RT2DCamera = namedtuple("RT2DCamera", "marker_count status_flag")
+RT2DCamera.format = struct.Struct("<ic")
+
+RT2DMarker = namedtuple("RT2DMarker", "x y d_x d_y")
+RT2DMarker.format = struct.Struct("<iihh")
+
+# 3D
+RT3DComponent = namedtuple("RT3DComponent", "marker_count drop_rate out_of_sync_rate")
+RT3DComponent.format = struct.Struct("<Ihh")
+
+RT3DMarkerPosition = namedtuple("RT3DMarkerPosition", "x y z")
+RT3DMarkerPosition.format = struct.Struct("<3f")
+
+RT3DMarkerPositionResidual = namedtuple("RT3DMarkerPositionResidual", "x y z residual")
+RT3DMarkerPositionResidual.format = struct.Struct("<4f")
+
+RT3DMarkerPositionNoLabel = namedtuple("RT3DMarkerPositionNoLabel", "x y z id")
+RT3DMarkerPositionNoLabel.format = struct.Struct("<3fi")
+
+RT3DMarkerPositionNoLabelResidual = namedtuple(
+    "RT3DMarkerPositionNoLabelResidual", "x y z id residual"
+)
+RT3DMarkerPositionNoLabelResidual.format = struct.Struct("<3fif")
+
+# 6D
+RT6DComponent = namedtuple("RT6DComponent", "body_count drop_rate out_of_sync_rate")
+RT6DComponent.format = struct.Struct("<ihh")
+
+RT6DBodyPosition = namedtuple("RT6DBodyPosition", "x y z")
+RT6DBodyPosition.format = struct.Struct("<3f")
+
+RT6DBodyRotation = namedtuple("RT6DBodyRotation", "matrix")
+RT6DBodyRotation.format = struct.Struct("<9f")
+
+RT6DBodyResidual = namedtuple("RT6DBodyResidual", "residual")
+RT6DBodyResidual.format = struct.Struct("<f")
+
+RT6DBodyEuler = namedtuple("RT6DBodyEuler", "a1 a2 a3")
+RT6DBodyEuler.format = struct.Struct("<3f")
+
+# Analog
+RTAnalogComponent = namedtuple("RTAnalogComponent", "device_count")
+RTAnalogComponent.format = struct.Struct("<i")
+
+RTAnalogDevice = namedtuple("RTAnalogDevice", "id channel_count sample_count")
+RTAnalogDevice.format = struct.Struct("<iii")
+
+RTSampleNumber = namedtuple("RTSampleNumber", "sample_number")
+RTSampleNumber.format = struct.Struct("<i")
+
+RTAnalogChannel = namedtuple("RTAnalogChannel", "samples")
+RTAnalogChannel.format_str = "<%df"
+
+RTAnalogDeviceSingle = namedtuple("RTAnalogDeviceSingle", "id channel_count")
+RTAnalogDeviceSingle.format = struct.Struct("<ii")
+
+RTAnalogDeviceSamples = namedtuple("RTAnalogDeviceSamples", "samples")
+RTAnalogDeviceSamples.format_str = "<%df"
+
+# Force
+RTForceComponent = namedtuple("RTForceComponent", "plate_count")
+RTForceComponent.format = struct.Struct("<i")
+
+RTForcePlate = namedtuple("RTForcePlate", "id force_count force_number")
+RTForcePlate.format = struct.Struct("<iii")
+
+RTForcePlateSingle = namedtuple("RTForcePlateSingle", "id")
+RTForcePlateSingle.format = struct.Struct("<i")
+
+RTForce = namedtuple("RTForce", "x y z x_m y_m z_m x_a y_a z_a")
+RTForce.format = struct.Struct("<9f")
+
+# GazeVector
+RTGazeVectorComponent = namedtuple("RTGazeVectorComponent", "vector_count")
+RTGazeVectorComponent.format = struct.Struct("<i")
+
+RTGazeVectorInfo = namedtuple("RTGazeVectorInfo", "sample_count sample_number")
+RTGazeVectorInfo.format = struct.Struct("<ii")
+
+RTGazeVectorUnitVector = namedtuple("RTGazeVectorUnitVector", "x y z")
+RTGazeVectorUnitVector.format = struct.Struct("<3f")
+
+RTGazeVectorPosition = namedtuple("RTGazeVectorPosition", "x y z")
+RTGazeVectorPosition.format = struct.Struct("<3f")
+
+# EyeTracker
+RTEyeTrackerComponent = namedtuple("RTEyeTrackerComponent", "eye_tracker_count")
+RTEyeTrackerComponent.format = struct.Struct("<i")
+
+RTEyeTrackerInfo = namedtuple("RTEyeTrackerInfo", "sample_count sample_number")
+RTEyeTrackerInfo.format = struct.Struct("<ii")
+
+RTEyeTrackerDiameter = namedtuple("RTEyeTrackerDiameter", "left right")
+RTEyeTrackerDiameter.format = struct.Struct("<ff")
+
+# Image
+RTImageComponent = namedtuple("RTImageComponent", "image_count")
+RTImageComponent.format = struct.Struct("<i")
+
+# Skeleton
+RTSkeletonComponent = namedtuple("RTSkeletonComponent", "skeleton_count")
+RTSkeletonComponent.format = struct.Struct("<i")
+
+RTSegmentCount = namedtuple("RTSegmentCount", "segment_count")
+RTSegmentCount.format = struct.Struct("<i")
+
+RTSegmentId = namedtuple("RTSegmentId", "id")
+RTSegmentId.format = struct.Struct("<i")
+
+RTSegmentPosition = namedtuple("RTSegmentPosition", "x y z")
+RTSegmentPosition.format = struct.Struct("<3f")
+
+RTSegmentRotation = namedtuple("RTSegmentRotation", "x y z w")
+RTSegmentRotation.format = struct.Struct("<4f")
+
+RTImage = namedtuple(
+    "RTImage",
+    "id format width height left_crop top_crop right_crop bottom_crop image_size",
+)
+RTImage.format = struct.Struct("<iiiiffffi")
+
+# Time
+
+RTTimeComponent = namedtuple("RTTimeComponent", "timecode_count")
+RTTimeComponent.format = struct.Struct("<i")
+
+RTTime = namedtuple("RTTime", "type hi lo")
+RTTime.format = struct.Struct("<iII")
+
+
+class QRTPacketType(Enum):
+    """ Packet types """
+
+    PacketError = 0
+    PacketCommand = 1
+    PacketXML = 2
+    PacketData = 3
+    PacketNoMoreData = 4
+    PacketC3DFile = 5
+    PacketEvent = 6
+    PacketDiscover = 7
+    PacketQTMFile = 8
+    PacketNone = 9
+
+
+class QRTComponentType(Enum):
+    """ QTM Component types """
+
+    Component3d = 1
+    Component3dNoLabels = 2
+    ComponentAnalog = 3
+    ComponentForce = 4
+    Component6d = 5
+    Component6dEuler = 6
+    Component2d = 7
+    Component2dLin = 8
+    Component3dRes = 9
+    Component3dNoLabelsRes = 10
+    Component6dRes = 11
+    Component6dEulerRes = 12
+    ComponentAnalogSingle = 13
+    ComponentImage = 14
+    ComponentForceSingle = 15
+    ComponentGazeVector = 16
+    ComponentTimecode = 17
+    ComponentSkeleton = 18
+    ComponentEyeTracker = 19
+
+
+class QRTImageFormat(Enum):
+    """ QTM Image formats """
+
+    FormatRawGrayscale = 0
+    FormatRawBGR = 1
+    FormatJPG = 2
+    FormatPNG = 3
+
+
+class QRTEvent(Enum):
+    """ QTM Event types """
+
+    EventConnected = 1
+    EventConnectionClosed = 2
+    EventCaptureStarted = 3
+    EventCaptureStopped = 4
+    EventCaptureFetchingFinished = 5  # Not used in version 1.10 and later
+    EventCalibrationStarted = 6
+    EventCalibrationStopped = 7
+    EventRTfromFileStarted = 8
+    EventRTfromFileStopped = 9
+    EventWaitingForTrigger = 10
+    EventCameraSettingsChanged = 11
+    EventQTMShuttingDown = 12
+    EventCaptureSaved = 13
+    EventReprocessingStarted = 14
+    EventReprocessingStopped = 15
+    EventTrigger = 16
+    EventNone = (
+        17
+    )  # Must be the last. Not actually an event. Just used to count number of events.
+
+
+class ComponentGetter(object):
+    """ Helper decorator for extracting correct packet data based on type """
+
+    def __init__(self, component_enum, base_component):
+        self.component_enum = component_enum
+        self.base_component = base_component
+
+    def __call__(self, function):
+        @wraps(function)
+        def wrapper(*args, **kwargs):
+            calling_object = args[0]
+            component_position = calling_object.components.get(
+                self.component_enum, None
+            )
+            if component_position is None:
+                return None
+
+            component_position, component_info = QRTPacket._get_exact(
+                self.base_component, calling_object.data, component_position
+            )
+
+            return (
+                component_info,
+                function(
+                    *args,
+                    component_info=component_info,
+                    data=calling_object.data,
+                    component_position=component_position,
+                    **kwargs
+                ),
+            )
+
+        return wrapper
+
+
+# noinspection PyTypeChecker
+class QRTPacket(object):
+    """Packet containing data measured with QTM.
+
+    Too check for existence of a specific component in a packet:
+
+    ::
+
+        from qtm.packet import QRTComponentType
+        if QRTComponentType.Component3d in packet.components:
+            header, markers = packet.get_3d_markers()
+
+    Component retriever functions will return None if a component is not in the packet.
+
+    """
+
+    def __init__(self, data):
+        self.data = data
+
+        self.timestamp, self.framenumber, component_count = RTDataQRTPacket.unpack_from(
+            data, 0
+        )
+
+        self.components = {}
+        position = RTDataQRTPacket.size
+        for _ in range(component_count):
+            c_size, c_type = RTComponentData.unpack_from(data, position)
+            self.components[QRTComponentType(c_type)] = position + RTComponentData.size
+            position += c_size
+
+    @staticmethod
+    def _get_exact(component_type, data, position):
+        value = component_type._make(component_type.format.unpack_from(data, position))
+        position += component_type.format.size
+        return position, value
+
+    @staticmethod
+    def _get_tuple(component_type, data, position):
+        value = component_type._make(
+            [component_type.format.unpack_from(data, position)]
+        )
+        position += component_type.format.size
+        return position, value
+
+    @staticmethod
+    def _get_2d_markers(data, component_info, component_position, index=None):
+        components = []
+        append_components = components.append
+        for camera in range(component_info.camera_count):
+            component_position, camera_info = QRTPacket._get_exact(
+                RT2DCamera, data, component_position
+            )
+
+            if index is None or index == camera:
+                marker_list = []
+                append_marker = marker_list.append
+                append_components(marker_list)
+
+                for _ in range(camera_info.marker_count):
+                    component_position, marker = QRTPacket._get_exact(
+                        RT2DMarker, data, component_position
+                    )
+                    append_marker(marker)
+            else:
+                component_position += RT2DMarker.format.size * camera_info.marker_count
+
+        return components
+
+    @staticmethod
+    def _get_3d_markers(type_, component_info, data, component_position):
+        components = []
+        append_components = components.append
+        for _ in range(component_info.marker_count):
+            component_position, position = QRTPacket._get_exact(
+                type_, data, component_position
+            )
+            append_components(position)
+
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentTimecode, RTTimeComponent)
+    def get_timecode(self, component_info=None, data=None, component_position=None):
+        components = []
+        append_components = components.append
+        for _ in range(component_info.timecode_count):
+            time_component, timecode = QRTPacket._get_exact(
+                RTTime, data, component_position)
+            append_components(timecode)
+
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentAnalog, RTAnalogComponent)
+    def get_analog(self, component_info=None, data=None, component_position=None):
+        """Get analog data."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.device_count):
+            component_position, device = QRTPacket._get_exact(
+                RTAnalogDevice, data, component_position
+            )
+            if device.sample_count > 0:
+                component_position, sample_number = QRTPacket._get_exact(
+                    RTSampleNumber, data, component_position
+                )
+
+                RTAnalogChannel.format = struct.Struct(
+                    RTAnalogChannel.format_str % device.sample_count
+                )
+                for _ in range(device.channel_count):
+                    component_position, channel = QRTPacket._get_tuple(
+                        RTAnalogChannel, data, component_position
+                    )
+                    append_components((device, sample_number, channel))
+
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentAnalogSingle, RTAnalogComponent)
+    def get_analog_single(
+        self, component_info=None, data=None, component_position=None
+    ):
+        """Get a single analog data channel."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.device_count):
+            component_position, device = QRTPacket._get_exact(
+                RTAnalogDeviceSingle, data, component_position
+            )
+
+            RTAnalogDeviceSamples.format = struct.Struct(
+                RTAnalogDeviceSamples.format_str % device.channel_count
+            )
+            component_position, sample = QRTPacket._get_tuple(
+                RTAnalogDeviceSamples, data, component_position
+            )
+            append_components((device, sample))
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentForce, RTForceComponent)
+    def get_force(self, component_info=None, data=None, component_position=None):
+        """Get force data."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.plate_count):
+            component_position, plate = QRTPacket._get_exact(
+                RTForcePlate, data, component_position
+            )
+            force_list = []
+            for _ in range(plate.force_count):
+                component_position, force = QRTPacket._get_exact(
+                    RTForce, data, component_position
+                )
+                force_list.append(force)
+            append_components((plate, force_list))
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentForceSingle, RTForceComponent)
+    def get_force_single(self, component_info=None, data=None, component_position=None):
+        """Get a single force data channel."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.plate_count):
+            component_position, plate = QRTPacket._get_exact(
+                RTForcePlateSingle, data, component_position
+            )
+            component_position, force = QRTPacket._get_exact(
+                RTForce, data, component_position
+            )
+            append_components((plate, force))
+        return components
+
+    @ComponentGetter(QRTComponentType.Component6d, RT6DComponent)
+    def get_6d(self, component_info=None, data=None, component_position=None):
+        """Get 6D data."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.body_count):
+            component_position, position = QRTPacket._get_exact(
+                RT6DBodyPosition, data, component_position
+            )
+            component_position, matrix = QRTPacket._get_tuple(
+                RT6DBodyRotation, data, component_position
+            )
+            append_components((position, matrix))
+        return components
+
+    @ComponentGetter(QRTComponentType.Component6dRes, RT6DComponent)
+    def get_6d_residual(self, component_info=None, data=None, component_position=None):
+        """Get 6D data with residual."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.body_count):
+            component_position, position = QRTPacket._get_exact(
+                RT6DBodyPosition, data, component_position
+            )
+            component_position, matrix = QRTPacket._get_tuple(
+                RT6DBodyRotation, data, component_position
+            )
+            component_position, residual = QRTPacket._get_exact(
+                RT6DBodyResidual, data, component_position
+            )
+            append_components((position, matrix, residual))
+        return components
+
+    @ComponentGetter(QRTComponentType.Component6dEuler, RT6DComponent)
+    def get_6d_euler(self, component_info=None, data=None, component_position=None):
+        """Get 6D data with euler rotations."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.body_count):
+            component_position, position = QRTPacket._get_exact(
+                RT6DBodyPosition, data, component_position
+            )
+            component_position, euler = QRTPacket._get_exact(
+                RT6DBodyEuler, data, component_position
+            )
+            append_components((position, euler))
+        return components
+
+    @ComponentGetter(QRTComponentType.Component6dEulerRes, RT6DComponent)
+    def get_6d_euler_residual(
+        self, component_info=None, data=None, component_position=None
+    ):
+        """Get 6D data with residuals and euler rotations."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.body_count):
+            component_position, position = QRTPacket._get_exact(
+                RT6DBodyPosition, data, component_position
+            )
+            component_position, euler = QRTPacket._get_exact(
+                RT6DBodyEuler, data, component_position
+            )
+            component_position, residual = QRTPacket._get_exact(
+                RT6DBodyResidual, data, component_position
+            )
+            append_components((position, euler, residual))
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentImage, RTImageComponent)
+    def get_image(self, component_info=None, data=None, component_position=None):
+        """Get image."""
+        components = []
+        append_components = components.append
+        for _ in range(component_info.image_count):
+            component_position, image_info = QRTPacket._get_exact(
+                RTImage, data, component_position
+            )
+            append_components((image_info, data[component_position:component_position + image_info.image_size]))
+            component_position += image_info.image_size
+        return components
+
+    @ComponentGetter(QRTComponentType.Component3d, RT3DComponent)
+    def get_3d_markers(self, component_info=None, data=None, component_position=None):
+        """Get 3D markers."""
+        return self._get_3d_markers(
+            RT3DMarkerPosition, component_info, data, component_position
+        )
+
+    @ComponentGetter(QRTComponentType.Component3dRes, RT3DComponent)
+    def get_3d_markers_residual(
+        self, component_info=None, data=None, component_position=None
+    ):
+        """Get 3D markers with residual."""
+        return self._get_3d_markers(
+            RT3DMarkerPositionResidual, component_info, data, component_position
+        )
+
+    @ComponentGetter(QRTComponentType.Component3dNoLabels, RT3DComponent)
+    def get_3d_markers_no_label(
+        self, component_info=None, data=None, component_position=None
+    ):
+        """Get 3D markers without label."""
+        return self._get_3d_markers(
+            RT3DMarkerPositionNoLabel, component_info, data, component_position
+        )
+
+    @ComponentGetter(QRTComponentType.Component3dNoLabelsRes, RT3DComponent)
+    def get_3d_markers_no_label_residual(
+        self, component_info=None, data=None, component_position=None
+    ):
+        """Get 3D markers without label with residual."""
+        return self._get_3d_markers(
+            RT3DMarkerPositionNoLabelResidual, component_info, data, component_position
+        )
+
+    @ComponentGetter(QRTComponentType.Component2d, RT2DComponent)
+    def get_2d_markers(
+        self, component_info=None, data=None, component_position=None, index=None
+    ):
+        """Get 2D markers.
+
+        :param index: Specify which camera to get 2D from, will be returned as
+                      first entry in the returned array.
+        """
+        return self._get_2d_markers(
+            data, component_info, component_position, index=index
+        )
+
+    @ComponentGetter(QRTComponentType.Component2dLin, RT2DComponent)
+    def get_2d_markers_linearized(
+        self, component_info=None, data=None, component_position=None, index=None
+    ):
+        """Get 2D linearized markers.
+
+        :param index: Specify which camera to get 2D from, will be returned as
+                      first entry in the returned array.
+        """
+
+        return self._get_2d_markers(
+            data, component_info, component_position, index=index
+        )
+
+    @ComponentGetter(QRTComponentType.ComponentSkeleton, RTSkeletonComponent)
+    def get_skeletons(self, component_info=None, data=None, component_position=None):
+        """Get skeletons
+        """
+
+        components = []
+        append_components = components.append
+        for _ in range(component_info.skeleton_count):
+            component_position, info = QRTPacket._get_exact(
+                RTSegmentCount, data, component_position
+            )
+
+            segments = []
+            for __ in range(info.segment_count):
+                component_position, segment = QRTPacket._get_exact(
+                    RTSegmentId, data, component_position
+                )
+                component_position, position = QRTPacket._get_exact(
+                    RTSegmentPosition, data, component_position
+                )
+                component_position, rotation = QRTPacket._get_exact(
+                    RTSegmentRotation, data, component_position
+                )
+
+                segments.append((segment.id, position, rotation))
+            append_components(segments)
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentGazeVector, RTGazeVectorComponent)
+    def get_gaze_vectors(self, component_info=None, data=None, component_position=None):
+        """Get gaze vectors
+        """
+        
+        components = []
+        append_components = components.append
+        for _ in range(component_info.vector_count):
+            component_position, info = QRTPacket._get_exact(
+                RTGazeVectorInfo, data, component_position)
+            
+            samples = []
+            if info.sample_count > 0:
+                for _ in range(info.sample_count):
+                    component_position, unit_vector = QRTPacket._get_exact(
+                        RTGazeVectorUnitVector, data, component_position)
+
+                    component_position, position = QRTPacket._get_exact(
+                        RTGazeVectorPosition, data, component_position)
+
+                    samples.append((unit_vector, position))
+
+            append_components((info, samples))
+
+        return components
+
+    @ComponentGetter(QRTComponentType.ComponentEyeTracker, RTEyeTrackerComponent)
+    def get_eye_trackers(self, component_info=None, data=None, component_position=None):
+        """Get eye trackers
+        """
+
+        components = []
+        append_components = components.append
+        for _ in range(component_info.eye_tracker_count):
+            component_position, info = QRTPacket._get_exact(
+                RTEyeTrackerInfo, data, component_position)
+            
+            samples = []
+            if info.sample_count > 0:
+                for _ in range(info.sample_count):
+                    component_position, diameter = QRTPacket._get_exact(
+                        RTEyeTrackerDiameter, data, component_position
+                    )
+                    samples.append(diameter)
+
+            append_components((info, samples))
+
+        return components
+
```

## qtm/protocol.py

```diff
@@ -1,188 +1,193 @@
-"""
-    QTM RT Protocol implementation
-"""
-
-import asyncio
-import struct
-import collections
-import logging
-
-from qtm.packet import QRTPacketType
-from qtm.packet import QRTPacket, QRTEvent
-from qtm.packet import RTheader, RTEvent, RTCommand
-from qtm.receiver import Receiver
-
-# pylint: disable=C0330
-
-LOG = logging.getLogger("qtm")
-
-
-class QRTCommandException(Exception):
-    """
-        Basic RT Command Exception
-    """
-
-    def __init__(self, value):
-        super(QRTCommandException, self).__init__()
-        self.value = value
-
-    def __str__(self):
-        return repr(self.value)
-
-
-class QTMProtocol(asyncio.Protocol):
-    """
-        QTM RT Protocol implementation
-        Should be constructed by ::qrt.connect
-    """
-
-    def __init__(self, *, loop=None, on_disconnect=None, on_event=None):
-        self._received_data = b""
-
-        self.on_disconnect = on_disconnect
-        self.on_event = on_event
-        self.on_packet = None
-
-        self.request_queue = collections.deque()
-        self.event_future = None
-        self._start_streaming = False
-
-        self.loop = loop or asyncio.get_event_loop()
-        self.transport = None
-
-        self._handlers = {
-            QRTPacketType.PacketError: self._on_error,
-            QRTPacketType.PacketData: self._on_data,
-            QRTPacketType.PacketCommand: self._on_command,
-            QRTPacketType.PacketEvent: self._on_event,
-            QRTPacketType.PacketXML: self._on_xml,
-            QRTPacketType.PacketNoMoreData: lambda _: LOG.debug(
-                QRTPacketType.PacketNoMoreData
-            ),
-        }
-
-        self._receiver = Receiver(self._handlers)
-
-    async def set_version(self, version):
-        """ Set version of RT protocol used to communicate with QTM """
-        version_cmd = "version %s" % version
-        # No need to check response, will throw if error
-        await self.send_command(version_cmd)
-
-    async def _wait_loop(self, event):
-        while True:
-            self.event_future = self.event_future or self.loop.create_future()
-            result = await self.event_future
-
-            if event is None or event == result:
-                break
-        return result
-
-    async def await_event(self, event=None, timeout=None):
-        """ Wait for any or specified event """
-        if self.event_future is not None:
-            raise Exception("Can't wait on multiple events!")
-
-        result = await asyncio.wait_for(self._wait_loop(event), timeout)
-        return result
-
-    def send_command(
-        self, command, callback=True, command_type=QRTPacketType.PacketCommand
-    ):
-        """ Sends commands to QTM """
-        if self.transport is not None:
-            cmd_length = len(command)
-            LOG.debug("S: %s", command)
-            self.transport.write(
-                struct.pack(
-                    RTCommand % cmd_length,
-                    RTheader.size + cmd_length + 1,
-                    command_type.value,
-                    command.encode(),
-                    b"\0",
-                )
-            )
-
-            future = self.loop.create_future()
-            if callback:
-                self.request_queue.append(future)
-            else:
-                future.set_result(None)
-            return future
-
-        raise QRTCommandException("Not connected!")
-
-    def receive_response(self):
-        """ Sends commands to QTM """
-        if self.transport is not None:
-            future = self.loop.create_future()
-            self.request_queue.append(future)
-            return future
-
-        raise QRTCommandException("Not connected!")
-
-    def connection_made(self, transport):
-        LOG.info("Connected")
-        self.transport = transport
-
-    def set_on_packet(self, on_packet):
-        """ Set callback to use when packet arrives """
-        self.on_packet = on_packet
-        self._start_streaming = on_packet is not None
-
-    def data_received(self, data):
-        """ Received from QTM and route accordingly """
-        self._receiver.data_received(data)
-
-    def _deliver_promise(self, data):
-        try:
-            future = self.request_queue.pop()
-            future.set_result(data)
-        except IndexError:
-            pass
-
-    def _on_data(self, packet):
-        if self.on_packet is not None:
-            if self._start_streaming:
-                self._deliver_promise(b"Ok")
-                self._start_streaming = False
-
-            self.on_packet(packet)
-        else:
-            self._deliver_promise(packet)
-        return
-
-    def _on_event(self, event):
-        LOG.info(event)
-
-        if self.event_future is not None:
-            future, self.event_future = self.event_future, None
-            future.set_result(event)
-
-        if self.on_event:
-            self.on_event(event)
-
-    def _on_error(self, response):
-        LOG.debug("Error: %s", response)
-        if self._start_streaming:
-            self.set_on_packet(None)
-        try:
-            future = self.request_queue.pop()
-            future.set_exception(QRTCommandException(response))
-        except IndexError:
-            raise QRTCommandException(response)
-
-    def _on_xml(self, response):
-        LOG.debug("XML: %s ...", response[: min(len(response), 70)])
-        self._deliver_promise(response)
-
-    def _on_command(self, response):
-        LOG.debug("R: %s", response)
-        if response != b"QTM RT Interface connected":
-            self._deliver_promise(response)
-
-    def connection_lost(self, exc):
-        self.transport = None
-        LOG.info("Disconnected")
-        if self.on_disconnect is not None:
-            self.on_disconnect(exc)
+"""
+    QTM RT Protocol implementation
+"""
+
+import asyncio
+import struct
+import collections
+import logging
+
+from qtm.packet import QRTPacketType
+from qtm.packet import QRTPacket, QRTEvent
+from qtm.packet import RTheader, RTEvent, RTCommand
+from qtm.receiver import Receiver
+
+# pylint: disable=C0330
+
+LOG = logging.getLogger("qtm")
+
+
+class QRTCommandException(Exception):
+    """
+        Basic RT Command Exception
+    """
+
+    def __init__(self, value):
+        super(QRTCommandException, self).__init__()
+        self.value = value
+
+    def __str__(self):
+        return repr(self.value)
+
+
+class QTMProtocol(asyncio.Protocol):
+    """
+        QTM RT Protocol implementation
+        Should be constructed by ::qrt.connect
+    """
+
+    def __init__(self, *, loop=None, on_disconnect=None, on_event=None):
+        self._received_data = b""
+
+        self.on_disconnect = on_disconnect
+        self.on_event = on_event
+        self.on_packet = None
+
+        self.request_queue = collections.deque()
+        self.event_future = None
+        self._start_streaming = False
+
+        self.loop = loop or asyncio.get_event_loop()
+        self.transport = None
+
+        self._handlers = {
+            QRTPacketType.PacketError: self._on_error,
+            QRTPacketType.PacketData: self._on_data,
+            QRTPacketType.PacketCommand: self._on_command,
+            QRTPacketType.PacketEvent: self._on_event,
+            QRTPacketType.PacketXML: self._on_xml,
+            QRTPacketType.PacketNoMoreData: self._on_no_more_data
+        }
+
+        self._receiver = Receiver(self._handlers)
+
+    async def set_version(self, version):
+        """ Set version of RT protocol used to communicate with QTM """
+        version_cmd = "version %s" % version
+        # No need to check response, will throw if error
+        await self.send_command(version_cmd)
+
+    async def _wait_loop(self, event):
+        while True:
+            self.event_future = self.event_future or self.loop.create_future()
+            result = await self.event_future
+
+            if event is None or event == result:
+                break
+        return result
+
+    async def await_event(self, event=None, timeout=None):
+        """ Wait for any or specified event """
+        if self.event_future is not None:
+            raise Exception("Can't wait on multiple events!")
+
+        result = await asyncio.wait_for(self._wait_loop(event), timeout)
+        return result
+
+    def send_command(
+        self, command, callback=True, command_type=QRTPacketType.PacketCommand
+    ):
+        """ Sends commands to QTM """
+        if self.transport is not None:
+            cmd_length = len(command)
+            LOG.debug("S: %s", command)
+            self.transport.write(
+                struct.pack(
+                    RTCommand % cmd_length,
+                    RTheader.size + cmd_length + 1,
+                    command_type.value,
+                    command.encode(),
+                    b"\0",
+                )
+            )
+
+            future = self.loop.create_future()
+            if callback:
+                self.request_queue.append(future)
+            else:
+                future.set_result(None)
+            return future
+
+        raise QRTCommandException("Not connected!")
+
+    def receive_response(self):
+        """ Sends commands to QTM """
+        if self.transport is not None:
+            future = self.loop.create_future()
+            self.request_queue.append(future)
+            return future
+
+        raise QRTCommandException("Not connected!")
+
+    def connection_made(self, transport):
+        LOG.info("Connected")
+        self.transport = transport
+
+    def set_on_packet(self, on_packet):
+        """ Set callback to use when packet arrives """
+        self.on_packet = on_packet
+        self._start_streaming = on_packet is not None
+
+    def data_received(self, data):
+        """ Received from QTM and route accordingly """
+        self._receiver.data_received(data)
+
+    def _deliver_promise(self, data):
+        try:
+            future = self.request_queue.pop()
+            future.set_result(data)
+        except IndexError:
+            pass
+
+    def _on_data(self, packet):
+        if self.on_packet is not None:
+            if self._start_streaming:
+                self._deliver_promise(b"Ok")
+                self._start_streaming = False
+
+            self.on_packet(packet)
+        else:
+            self._deliver_promise(packet)
+        return
+    
+    def _on_no_more_data(self, packet):
+        if self.on_packet is not None:
+            if self._start_streaming:
+                self._deliver_promise(b"Ok")
+                self._start_streaming = False
+        return
+    
+    def _on_event(self, event):
+        LOG.info(event)
+
+        if self.event_future is not None:
+            future, self.event_future = self.event_future, None
+            future.set_result(event)
+
+        if self.on_event:
+            self.on_event(event)
+
+    def _on_error(self, response):
+        LOG.debug("Error: %s", response)
+        if self._start_streaming:
+            self.set_on_packet(None)
+        try:
+            future = self.request_queue.pop()
+            future.set_exception(QRTCommandException(response))
+        except IndexError:
+            raise QRTCommandException(response)
+
+    def _on_xml(self, response):
+        LOG.debug("XML: %s ...", response[: min(len(response), 70)])
+        self._deliver_promise(response)
+
+    def _on_command(self, response):
+        LOG.debug("R: %s", response)
+        if response != b"QTM RT Interface connected":
+            self._deliver_promise(response)
+
+    def connection_lost(self, exc):
+        self.transport = None
+        LOG.info("Disconnected")
+        if self.on_disconnect is not None:
+            self.on_disconnect(exc)
```

## qtm/qrt.py

```diff
@@ -1,400 +1,400 @@
-""" QTM RT protocol implementation """
-
-import asyncio
-import logging
-from functools import wraps
-
-from qtm.packet import QRTPacketType, QRTPacket
-from qtm.protocol import QTMProtocol, QRTCommandException
-
-# pylint: disable=C0330
-
-LOG = logging.getLogger("qtm")  # pylint: disable C0103
-
-
-def validate_response(expected_responses):
-    """ Decorator to validate responses from QTM """
-
-    def internal_decorator(function):
-        @wraps(function)
-        async def wrapper(*args, **kwargs):
-
-            response = await function(*args, **kwargs)
-
-            for expected_response in expected_responses:
-                if response.startswith(expected_response):
-                    return response
-
-            raise QRTCommandException(
-                "Expected %s but got %s" % (expected_responses, response)
-            )
-
-        return wrapper
-
-    return internal_decorator
-
-
-class QRTConnection(object):
-    """Represent a connection to QTM.
-
-        Returned by :func:`~qtm.connect` when successfuly connected to QTM.
-    """
-
-    def __init__(self, protocol: QTMProtocol, timeout):
-        super(QRTConnection, self).__init__()
-        self._protocol = protocol
-        self._timeout = timeout
-
-    def disconnect(self):
-        """Disconnect from QTM."""
-        self._protocol.transport.close()
-
-    def has_transport(self):
-        """ Check if connected to QTM """
-        return self._protocol.transport is not None
-
-    async def qtm_version(self):
-        """Get the QTM version.
-        """
-        return await asyncio.wait_for(
-            self._protocol.send_command("qtmversion"), timeout=self._timeout
-        )
-
-    async def byte_order(self):
-        """Get the byte order used when communicating
-            (should only ever be little endian using this library).
-        """
-        return await asyncio.wait_for(
-            self._protocol.send_command("byteorder"), timeout=self._timeout
-        )
-
-    async def get_state(self):
-        """Get the latest state change of QTM. If the :func:`~qtm.connect` on_event
-        callback was set the callback will be called as well.
-
-        :rtype: A :class:`qtm.QRTEvent`
-        """
-        await self._protocol.send_command("getstate", callback=False)
-        return await self._protocol.await_event()
-
-    async def await_event(self, event=None, timeout=30):
-        """Wait for an event from QTM.
-
-        :param event: A :class:`qtm.QRTEvent`
-            to wait for a specific event. Otherwise wait for any event.
-
-        :param timeout: Max time to wait for event.
-
-        :rtype: A :class:`qtm.QRTEvent`
-        """
-        return await self._protocol.await_event(event, timeout=timeout)
-
-    async def get_parameters(self, parameters=None):
-        """Get the settings for the requested component(s) of QTM in XML format.
-
-        :param parameters: A list of parameters to request.
-            Could be 'all' or any combination
-            of 'general', '3d', '6d', 'analog', 'force', 'gazevector', 'eyetracker', 'image',
-            'skeleton', 'skeleton:global', 'calibration'.
-        :rtype: An XML string containing the requested settings.
-            See QTM RT Documentation for details.
-        """
-
-        if parameters is None:
-            parameters = ["all"]
-        else:
-            for parameter in parameters:
-                if not parameter in [
-                    "all",
-                    "general",
-                    "3d",
-                    "6d",
-                    "analog",
-                    "force",
-                    "gazevector",
-                    "eyetracker",
-                    "image",
-                    "skeleton",
-                    "skeleton:global",
-                    "calibration",
-                ]:
-                    raise QRTCommandException("%s is not a valid parameter" % parameter)
-
-        cmd = "getparameters %s" % " ".join(parameters)
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    async def get_current_frame(self, components=None) -> QRTPacket:
-        """Get measured values from QTM for a single frame.
-
-        :param components: A list of components to receive, could be any combination of
-                '2d', '2dlin', '3d', '3dres', '3dnolabels',
-                '3dnolabelsres', 'analog', 'analogsingle', 'force', 'forcesingle', '6d', '6dres',
-                '6deuler', '6deulerres', 'gazevector', 'eyetracker', 'image', 'timecode',
-                'skeleton', 'skeleton:global'
-
-        :rtype: A :class:`qtm.QRTPacket` containing requested components
-        """
-
-        _validate_components(components)
-
-        cmd = "getcurrentframe %s" % " ".join(components)
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    async def stream_frames(self, frames="allframes", components=None, on_packet=None):
-        """Stream measured frames from QTM until :func:`~qtm.QRTConnection.stream_frames_stop`
-           is called.
-
-
-        :param frames: Which frames to receive, possible values are 'allframes',
-            'frequency:n' or 'frequencydivisor:n' where n should be desired value.
-        :param components: A list of components to receive, could be any combination of
-                '2d', '2dlin', '3d', '3dres', '3dnolabels',
-                '3dnolabelsres', 'analog', 'analogsingle', 'force', 'forcesingle', '6d', '6dres',
-                '6deuler', '6deulerres', 'gazevector', 'eyetracker', 'image', 'timecode',
-                'skeleton', 'skeleton:global'
-
-        :rtype: The string 'Ok' if successful
-        """
-
-        _validate_components(components)
-
-        self._protocol.set_on_packet(on_packet)
-
-        cmd = "streamframes %s %s" % (frames, " ".join(components))
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    async def stream_frames_stop(self):
-        """Stop streaming frames."""
-
-        self._protocol.set_on_packet(None)
-
-        cmd = "streamframes stop"
-        await self._protocol.send_command(cmd, callback=False)
-
-    @validate_response([b"You are now master"])
-    async def take_control(self, password):
-        """Take control of QTM.
-
-        :param password: Password as entered in QTM.
-        """
-        cmd = "takecontrol %s" % password
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"You are now a regular client"])
-    async def release_control(self):
-        """Release control of QTM.
-        """
-
-        cmd = "releasecontrol"
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Creating new connection", b"Already connected"])
-    async def new(self):
-        """Create a new measurement.
-        """
-        cmd = "new"
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response(
-        [
-            b"Closing connection",
-            b"File closed",
-            b"Closing file",
-            b"No connection to close",
-        ]
-    )
-    async def close(self):
-        """Close a measurement
-        """
-        cmd = "close"
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Starting measurement", b"Starting RT from file"])
-    async def start(self, rtfromfile=False):
-        """Start RT from file. You need to be in control of QTM to be able to do this.
-        """
-        cmd = "start" + (" rtfromfile" if rtfromfile else "")
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Stopping measurement"])
-    async def stop(self):
-        """Stop RT from file."""
-        cmd = "stop"
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Measurement loaded"])
-    async def load(self, filename):
-        """Load a measurement.
-
-        :param filename: Path to measurement you want to load.
-        """
-        cmd = "load %s" % filename
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Measurement saved"])
-    async def save(self, filename, overwrite=False):
-        """Save a measurement.
-
-        :param filename: Filename you wish to save as.
-        :param overwrite: If QTM should overwrite existing measurement.
-        """
-        cmd = "save %s%s" % (filename, " overwrite" if overwrite else "")
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Project loaded"])
-    async def load_project(self, project_path):
-        """Load a project.
-
-        :param project_path: Path to project you want to load.
-        """
-        cmd = "loadproject %s" % project_path
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Trig ok"])
-    async def trig(self):
-        """Trigger QTM, only possible when QTM is configured to use Software/Wireless trigger"""
-        cmd = "trig"
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    @validate_response([b"Event set"])
-    async def set_qtm_event(self, event=None):
-        """Set event in QTM."""
-        cmd = "event%s" % ("" if event is None else " " + event)
-        return await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout
-        )
-
-    async def send_xml(self, xml):
-        """Used to update QTM settings, see QTM RT protocol for more information.
-
-        :param xml: XML document as a str. See QTM RT Documentation for details.
-        """
-        return await asyncio.wait_for(
-            self._protocol.send_command(xml, command_type=QRTPacketType.PacketXML),
-            timeout=self._timeout,
-        )
-
-    async def calibrate(self, timeout=600):  # Timeout 10 min.
-        """Start calibration and return calibration result.
-
-        :param timeout_: Calibration timeout.
-
-        :rtype: An XML string containing the calibration result.
-            See QTM RT Documentation for details.
-        """
-        cmd = "calibrate"
-        response = await asyncio.wait_for(
-            self._protocol.send_command(cmd), timeout=self._timeout)
-
-        if response != b"Starting calibration":
-            raise QRTCommandException(response) 
-        
-        return await asyncio.wait_for(
-            self._protocol.receive_response(), timeout=timeout)
-
-
-
-# TODO GetCaptureC3D
-# TODO GetCaptureQTM
-
-
-async def connect(
-    host,
-    port=22223,
-    version="1.23",
-    on_event=None,
-    on_disconnect=None,
-    timeout=5,
-    loop=None,
-) -> QRTConnection:
-    """Async function to connect to QTM
-
-    :param host: Address of the computer running QTM.
-    :param port: Port number to connect to, should be the port configured for little endian.
-    :param version: Version of the rt protocol to use. Default is the latest version.
-        The Qualisys Python sdk does not support versions older than 1.8.
-    :param on_disconnect: Function to be called when a disconnect from QTM occurs.
-    :param on_event: Function to be called when there's an event from QTM.
-    :param timeout: The default timeout time for calls to QTM.
-    :param loop: Alternative event loop, will use asyncio default if None.
-
-    :rtype: A :class:`.QRTConnection`
-    """
-    loop = loop or asyncio.get_event_loop()
-
-    try:
-        _, protocol = await loop.create_connection(
-            lambda: QTMProtocol(
-                loop=loop, on_event=on_event, on_disconnect=on_disconnect
-            ),
-            host,
-            port,
-        )
-    except (ConnectionRefusedError, TimeoutError, OSError) as exception:
-        LOG.error(exception)
-        return None
-
-    try:
-        await protocol.set_version(version)
-    except QRTCommandException as exception:
-        LOG.error(exception)
-        return None
-    except TypeError as exception:  # TODO: fix test requiring this (test_connect_set_version)
-        LOG.error(exception)
-        return None
-
-    return QRTConnection(protocol, timeout=timeout)
-
-
-def _validate_components(components):
-    for component in components:
-        if not component.lower() in [
-            "2d",
-            "2dlin",
-            "3d",
-            "3dres",
-            "3dnolabels",
-            "3dnolabelsres",
-            "analog",
-            "analogsingle",
-            "force",
-            "forcesingle",
-            "6d",
-            "6dres",
-            "6deuler",
-            "6deulerres",
-            "gazevector",
-            "eyetracker",
-            "image",
-            "timecode",
-            "skeleton",
-            "skeleton:global",
-        ]:
-            raise QRTCommandException("%s is not a valid component" % component)
-
+""" QTM RT protocol implementation """
+
+import asyncio
+import logging
+from functools import wraps
+
+from qtm.packet import QRTPacketType, QRTPacket
+from qtm.protocol import QTMProtocol, QRTCommandException
+
+# pylint: disable=C0330
+
+LOG = logging.getLogger("qtm")  # pylint: disable C0103
+
+
+def validate_response(expected_responses):
+    """ Decorator to validate responses from QTM """
+
+    def internal_decorator(function):
+        @wraps(function)
+        async def wrapper(*args, **kwargs):
+
+            response = await function(*args, **kwargs)
+
+            for expected_response in expected_responses:
+                if response.startswith(expected_response):
+                    return response
+
+            raise QRTCommandException(
+                "Expected %s but got %s" % (expected_responses, response)
+            )
+
+        return wrapper
+
+    return internal_decorator
+
+
+class QRTConnection(object):
+    """Represent a connection to QTM.
+
+        Returned by :func:`~qtm.connect` when successfuly connected to QTM.
+    """
+
+    def __init__(self, protocol: QTMProtocol, timeout):
+        super(QRTConnection, self).__init__()
+        self._protocol = protocol
+        self._timeout = timeout
+
+    def disconnect(self):
+        """Disconnect from QTM."""
+        self._protocol.transport.close()
+
+    def has_transport(self):
+        """ Check if connected to QTM """
+        return self._protocol.transport is not None
+
+    async def qtm_version(self):
+        """Get the QTM version.
+        """
+        return await asyncio.wait_for(
+            self._protocol.send_command("qtmversion"), timeout=self._timeout
+        )
+
+    async def byte_order(self):
+        """Get the byte order used when communicating
+            (should only ever be little endian using this library).
+        """
+        return await asyncio.wait_for(
+            self._protocol.send_command("byteorder"), timeout=self._timeout
+        )
+
+    async def get_state(self):
+        """Get the latest state change of QTM. If the :func:`~qtm.connect` on_event
+        callback was set the callback will be called as well.
+
+        :rtype: A :class:`qtm.QRTEvent`
+        """
+        await self._protocol.send_command("getstate", callback=False)
+        return await self._protocol.await_event()
+
+    async def await_event(self, event=None, timeout=30):
+        """Wait for an event from QTM.
+
+        :param event: A :class:`qtm.QRTEvent`
+            to wait for a specific event. Otherwise wait for any event.
+
+        :param timeout: Max time to wait for event.
+
+        :rtype: A :class:`qtm.QRTEvent`
+        """
+        return await self._protocol.await_event(event, timeout=timeout)
+
+    async def get_parameters(self, parameters=None):
+        """Get the settings for the requested component(s) of QTM in XML format.
+
+        :param parameters: A list of parameters to request.
+            Could be 'all' or any combination
+            of 'general', '3d', '6d', 'analog', 'force', 'gazevector', 'eyetracker', 'image',
+            'skeleton', 'skeleton:global', 'calibration'.
+        :rtype: An XML string containing the requested settings.
+            See QTM RT Documentation for details.
+        """
+
+        if parameters is None:
+            parameters = ["all"]
+        else:
+            for parameter in parameters:
+                if not parameter in [
+                    "all",
+                    "general",
+                    "3d",
+                    "6d",
+                    "analog",
+                    "force",
+                    "gazevector",
+                    "eyetracker",
+                    "image",
+                    "skeleton",
+                    "skeleton:global",
+                    "calibration",
+                ]:
+                    raise QRTCommandException("%s is not a valid parameter" % parameter)
+
+        cmd = "getparameters %s" % " ".join(parameters)
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    async def get_current_frame(self, components=None) -> QRTPacket:
+        """Get measured values from QTM for a single frame.
+
+        :param components: A list of components to receive, could be any combination of
+                '2d', '2dlin', '3d', '3dres', '3dnolabels',
+                '3dnolabelsres', 'analog', 'analogsingle', 'force', 'forcesingle', '6d', '6dres',
+                '6deuler', '6deulerres', 'gazevector', 'eyetracker', 'image', 'timecode',
+                'skeleton', 'skeleton:global'
+
+        :rtype: A :class:`qtm.QRTPacket` containing requested components
+        """
+
+        _validate_components(components)
+
+        cmd = "getcurrentframe %s" % " ".join(components)
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    async def stream_frames(self, frames="allframes", components=None, on_packet=None):
+        """Stream measured frames from QTM until :func:`~qtm.QRTConnection.stream_frames_stop`
+           is called.
+
+
+        :param frames: Which frames to receive, possible values are 'allframes',
+            'frequency:n' or 'frequencydivisor:n' where n should be desired value.
+        :param components: A list of components to receive, could be any combination of
+                '2d', '2dlin', '3d', '3dres', '3dnolabels',
+                '3dnolabelsres', 'analog', 'analogsingle', 'force', 'forcesingle', '6d', '6dres',
+                '6deuler', '6deulerres', 'gazevector', 'eyetracker', 'image', 'timecode',
+                'skeleton', 'skeleton:global'
+
+        :rtype: The string 'Ok' if successful
+        """
+
+        _validate_components(components)
+
+        self._protocol.set_on_packet(on_packet)
+
+        cmd = "streamframes %s %s" % (frames, " ".join(components))
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    async def stream_frames_stop(self):
+        """Stop streaming frames."""
+
+        self._protocol.set_on_packet(None)
+
+        cmd = "streamframes stop"
+        await self._protocol.send_command(cmd, callback=False)
+
+    @validate_response([b"You are now master"])
+    async def take_control(self, password):
+        """Take control of QTM.
+
+        :param password: Password as entered in QTM.
+        """
+        cmd = "takecontrol %s" % password
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"You are now a regular client"])
+    async def release_control(self):
+        """Release control of QTM.
+        """
+
+        cmd = "releasecontrol"
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Creating new connection", b"Already connected"])
+    async def new(self):
+        """Create a new measurement.
+        """
+        cmd = "new"
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response(
+        [
+            b"Closing connection",
+            b"File closed",
+            b"Closing file",
+            b"No connection to close",
+        ]
+    )
+    async def close(self):
+        """Close a measurement
+        """
+        cmd = "close"
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Starting measurement", b"Starting RT from file"])
+    async def start(self, rtfromfile=False):
+        """Start RT from file. You need to be in control of QTM to be able to do this.
+        """
+        cmd = "start" + (" rtfromfile" if rtfromfile else "")
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Stopping measurement"])
+    async def stop(self):
+        """Stop RT from file."""
+        cmd = "stop"
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Measurement loaded"])
+    async def load(self, filename):
+        """Load a measurement.
+
+        :param filename: Path to measurement you want to load.
+        """
+        cmd = "load %s" % filename
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Measurement saved"])
+    async def save(self, filename, overwrite=False):
+        """Save a measurement.
+
+        :param filename: Filename you wish to save as.
+        :param overwrite: If QTM should overwrite existing measurement.
+        """
+        cmd = "save %s%s" % (filename, " overwrite" if overwrite else "")
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Project loaded"])
+    async def load_project(self, project_path):
+        """Load a project.
+
+        :param project_path: Path to project you want to load.
+        """
+        cmd = "loadproject %s" % project_path
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Trig ok"])
+    async def trig(self):
+        """Trigger QTM, only possible when QTM is configured to use Software/Wireless trigger"""
+        cmd = "trig"
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    @validate_response([b"Event set"])
+    async def set_qtm_event(self, event=None):
+        """Set event in QTM."""
+        cmd = "event%s" % ("" if event is None else " " + event)
+        return await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout
+        )
+
+    async def send_xml(self, xml):
+        """Used to update QTM settings, see QTM RT protocol for more information.
+
+        :param xml: XML document as a str. See QTM RT Documentation for details.
+        """
+        return await asyncio.wait_for(
+            self._protocol.send_command(xml, command_type=QRTPacketType.PacketXML),
+            timeout=self._timeout,
+        )
+
+    async def calibrate(self, timeout=600):  # Timeout 10 min.
+        """Start calibration and return calibration result.
+
+        :param timeout_: Calibration timeout.
+
+        :rtype: An XML string containing the calibration result.
+            See QTM RT Documentation for details.
+        """
+        cmd = "calibrate"
+        response = await asyncio.wait_for(
+            self._protocol.send_command(cmd), timeout=self._timeout)
+
+        if response != b"Starting calibration":
+            raise QRTCommandException(response) 
+        
+        return await asyncio.wait_for(
+            self._protocol.receive_response(), timeout=timeout)
+
+
+
+# TODO GetCaptureC3D
+# TODO GetCaptureQTM
+
+
+async def connect(
+    host,
+    port=22223,
+    version="1.24",
+    on_event=None,
+    on_disconnect=None,
+    timeout=5,
+    loop=None,
+) -> QRTConnection:
+    """Async function to connect to QTM
+
+    :param host: Address of the computer running QTM.
+    :param port: Port number to connect to, should be the port configured for little endian.
+    :param version: Version of the rt protocol to use. Default is the latest version.
+        The Qualisys Python sdk does not support versions older than 1.8.
+    :param on_disconnect: Function to be called when a disconnect from QTM occurs.
+    :param on_event: Function to be called when there's an event from QTM.
+    :param timeout: The default timeout time for calls to QTM.
+    :param loop: Alternative event loop, will use asyncio default if None.
+
+    :rtype: A :class:`.QRTConnection`
+    """
+    loop = loop or asyncio.get_event_loop()
+
+    try:
+        _, protocol = await loop.create_connection(
+            lambda: QTMProtocol(
+                loop=loop, on_event=on_event, on_disconnect=on_disconnect
+            ),
+            host,
+            port,
+        )
+    except (ConnectionRefusedError, TimeoutError, OSError) as exception:
+        LOG.error(exception)
+        return None
+
+    try:
+        await protocol.set_version(version)
+    except QRTCommandException as exception:
+        LOG.error(exception)
+        return None
+    except TypeError as exception:  # TODO: fix test requiring this (test_connect_set_version)
+        LOG.error(exception)
+        return None
+
+    return QRTConnection(protocol, timeout=timeout)
+
+
+def _validate_components(components):
+    for component in components:
+        if not component.lower() in [
+            "2d",
+            "2dlin",
+            "3d",
+            "3dres",
+            "3dnolabels",
+            "3dnolabelsres",
+            "analog",
+            "analogsingle",
+            "force",
+            "forcesingle",
+            "6d",
+            "6dres",
+            "6deuler",
+            "6deulerres",
+            "gazevector",
+            "eyetracker",
+            "image",
+            "timecode",
+            "skeleton",
+            "skeleton:global",
+        ]:
+            raise QRTCommandException("%s is not a valid component" % component)
+
```

## qtm/reboot.py

 * *Ordering differences only*

```diff
@@ -1,35 +1,35 @@
-""" Implementation of QTM cameras reboot protocol """
-
-import asyncio
-import logging
-
-LOG = logging.getLogger("qtm")
-
-DEFAULT_DISCOVERY_PORT = 9930
-
-
-async def reboot(ip_address):
-    """ async function to reboot QTM cameras """
-    _, protocol = await asyncio.get_event_loop().create_datagram_endpoint(
-        QRebootProtocol,
-        local_addr=(ip_address, 0),
-        allow_broadcast=True,
-    )
-
-    LOG.info("Sending reboot on %s", ip_address)
-    protocol.send_reboot()
-
-
-class QRebootProtocol:
-    """ Oqus/Miqus/Arqus discovery protocol implementation"""
-
-    def __init__(self):
-        self.transport = None
-
-    def connection_made(self, transport):
-        """ On socket creation """
-        self.transport = transport
-
-    def send_reboot(self):
-        """ Sends reboot package broadcast """
-        self.transport.sendto(b"reboot", ("<broadcast>", DEFAULT_DISCOVERY_PORT))
+""" Implementation of QTM cameras reboot protocol """
+
+import asyncio
+import logging
+
+LOG = logging.getLogger("qtm")
+
+DEFAULT_DISCOVERY_PORT = 9930
+
+
+async def reboot(ip_address):
+    """ async function to reboot QTM cameras """
+    _, protocol = await asyncio.get_event_loop().create_datagram_endpoint(
+        QRebootProtocol,
+        local_addr=(ip_address, 0),
+        allow_broadcast=True,
+    )
+
+    LOG.info("Sending reboot on %s", ip_address)
+    protocol.send_reboot()
+
+
+class QRebootProtocol:
+    """ Oqus/Miqus/Arqus discovery protocol implementation"""
+
+    def __init__(self):
+        self.transport = None
+
+    def connection_made(self, transport):
+        """ On socket creation """
+        self.transport = transport
+
+    def send_reboot(self):
+        """ Sends reboot package broadcast """
+        self.transport.sendto(b"reboot", ("<broadcast>", DEFAULT_DISCOVERY_PORT))
```

## qtm/receiver.py

 * *Ordering differences only*

```diff
@@ -1,51 +1,51 @@
-import logging
-
-from qtm.packet import QRTPacketType
-from qtm.packet import QRTPacket, QRTEvent
-from qtm.packet import RTheader, RTEvent, RTCommand
-
-LOG = logging.getLogger("qtm")
-
-
-class Receiver(object):
-    def __init__(self, handlers):
-        self._handlers = handlers
-        self._received_data = b""
-
-    def data_received(self, data):
-        """ Received from QTM and route accordingly """
-        self._received_data += data
-        h_size = RTheader.size
-        data = self._received_data
-        data_len = len(data);
-
-        while data_len >= h_size:
-            size, type_ = RTheader.unpack_from(data, 0)
-            if data_len >= size:
-                self._parse_received(data[h_size:size], type_)
-                data = data[size:]
-                data_len = len(data);
-            else:
-                break;
-
-        self._received_data = data
-
-    def _parse_received(self, data, type_):
-        type_ = QRTPacketType(type_)
-
-        if (
-            type_ == QRTPacketType.PacketError
-            or type_ == QRTPacketType.PacketCommand
-            or type_ == QRTPacketType.PacketXML
-        ):
-            data = data[:-1]
-        elif type_ == QRTPacketType.PacketData:
-            data = QRTPacket(data)
-        elif type_ == QRTPacketType.PacketEvent:
-            event, = RTEvent.unpack(data)
-            data = QRTEvent(ord(event))
-
-        try:
-            self._handlers[type_](data)
-        except KeyError:
-            LOG.error("Non handled packet type! - %s", type_)
+import logging
+
+from qtm.packet import QRTPacketType
+from qtm.packet import QRTPacket, QRTEvent
+from qtm.packet import RTheader, RTEvent, RTCommand
+
+LOG = logging.getLogger("qtm")
+
+
+class Receiver(object):
+    def __init__(self, handlers):
+        self._handlers = handlers
+        self._received_data = b""
+
+    def data_received(self, data):
+        """ Received from QTM and route accordingly """
+        self._received_data += data
+        h_size = RTheader.size
+        data = self._received_data
+        data_len = len(data);
+
+        while data_len >= h_size:
+            size, type_ = RTheader.unpack_from(data, 0)
+            if data_len >= size:
+                self._parse_received(data[h_size:size], type_)
+                data = data[size:]
+                data_len = len(data);
+            else:
+                break;
+
+        self._received_data = data
+
+    def _parse_received(self, data, type_):
+        type_ = QRTPacketType(type_)
+
+        if (
+            type_ == QRTPacketType.PacketError
+            or type_ == QRTPacketType.PacketCommand
+            or type_ == QRTPacketType.PacketXML
+        ):
+            data = data[:-1]
+        elif type_ == QRTPacketType.PacketData:
+            data = QRTPacket(data)
+        elif type_ == QRTPacketType.PacketEvent:
+            event, = RTEvent.unpack(data)
+            data = QRTEvent(ord(event))
+
+        try:
+            self._handlers[type_](data)
+        except KeyError:
+            LOG.error("Non handled packet type! - %s", type_)
```

## Comparing `qtm-2.1.1.dist-info/METADATA` & `qtm-2.1.2.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qtm
-Version: 2.1.1
-Summary: QTM Python SDK
+Version: 2.1.2
+Summary: DEPRECATED
 Home-page: https://github.com/qualisys/qualisys_python_sdk
 Author: Martin Gejke
 Author-email: support@qualisys.com
 License: MIT
-Download-URL: https://github.com/qualisys/qualisys_python_sdk/tarball/2.1.1
+Download-URL: https://github.com/qualisys/qualisys_python_sdk/tarball/2.1.2
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5.3
 
-UNKNOWN
+Future versions of this package will go under the name "qtm-rt".
```

## Comparing `qtm-2.1.1.dist-info/RECORD` & `qtm-2.1.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-qtm/__init__.py,sha256=mU-JPQQTDl5_Kp8zDIc-82VGl1zyBzKWYdAXaEv1OI0,670
-qtm/control.py,sha256=d9sh2zIW18l2D1hQ-pj1upOmQSi4dFgHiVALJ61VaTU,651
-qtm/discovery.py,sha256=hisBaOeb38jU__-8tN_YOHr8zAg5sBUq7zDfuE4cx24,2893
-qtm/packet.py,sha256=SbVvuVwqvWv-1P_JLYzl-V-fOIPGzPZy68G0DDvnTlI,23488
-qtm/protocol.py,sha256=Uy9c1vjd4okWRym0ESP9QtpnJYH8KsBiGYQ-XHjko04,5606
-qtm/qrt.py,sha256=32oBv0iL8qpJTqvFB7WjRwSqH-pMzdNVyfaj_-cgVSc,13209
-qtm/reboot.py,sha256=Wa74XluiGT8vzA52wb_bqBFZiYVNsooIt6BdeCnXl_g,890
-qtm/receiver.py,sha256=82EIF-XTW5Ekf-0y0-1JMHTflSfHk0lrMB0j7mwfSTE,1507
+qtm/__init__.py,sha256=2pk2etWC8JeDwqQneLc_vci6MWruiA1J1y6yOAEkAw4,700
+qtm/control.py,sha256=xWD-llnOR2eOUpMaaMSAKgXtBQPkYqHkfSAx7zSLWhI,674
+qtm/discovery.py,sha256=BnKjojNm27vrCVRqWUmmRgyLYITCP4Eh2jCZseSfeDk,2991
+qtm/packet.py,sha256=ltEQee549rd8np39fpcklR4bjO7SjZoc8mPAyYarpjo,24138
+qtm/protocol.py,sha256=fJnhKz6aXROxjzzzYv6qfj1wZaOFIdg0ymEGkcJXqx0,5970
+qtm/qrt.py,sha256=m9JiU1fVTyAsGrBMUJ3cJ58iRzJEZWlTh3xCTxOC-bs,13609
+qtm/reboot.py,sha256=00wvNPNoic4XymsjGJkOjYj-0Hkg6ETwWM9P2k_SMI0,925
+qtm/receiver.py,sha256=1JY-G4EGscksPxzFieZpSuVlnYyU-my3G_iliZ43bgM,1558
 qtm/data/demo.qtm,sha256=sYOMHapSu1WyN88VFiZup2t12AlR1ObR_gd_D7eNL4s,4259840
-qtm-2.1.1.dist-info/LICENSE,sha256=fugD2gcW8ghT4A9w-jjYNoxWUK2AMvwHhzrWm6EXTH4,1080
-qtm-2.1.1.dist-info/METADATA,sha256=QvIx_XBc6jSpqOKn71zSp6KRowlcN6NDITlhuaoN6NE,739
-qtm-2.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-qtm-2.1.1.dist-info/top_level.txt,sha256=jYib1OZ8W-GnMzlBVvPZ08k-2aJUW_K-3Je2_LPtkOs,4
-qtm-2.1.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-qtm-2.1.1.dist-info/RECORD,,
+qtm-2.1.2.dist-info/LICENSE,sha256=kJwS4jkbWBWIO7Fa5CpKY-42ShVC2K-z9kDhOclXTQ4,1101
+qtm-2.1.2.dist-info/METADATA,sha256=dshOAmERCWVKIwctDYyDb-V22ShRG8i7ulaO_kyawfc,792
+qtm-2.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+qtm-2.1.2.dist-info/top_level.txt,sha256=jYib1OZ8W-GnMzlBVvPZ08k-2aJUW_K-3Je2_LPtkOs,4
+qtm-2.1.2.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+qtm-2.1.2.dist-info/RECORD,,
```

