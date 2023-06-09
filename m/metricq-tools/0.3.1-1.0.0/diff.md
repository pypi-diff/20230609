# Comparing `tmp/metricq_tools-0.3.1-py3-none-any.whl.zip` & `tmp/metricq_tools-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,21 @@
-Zip file size: 34230 bytes, number of entries: 16
--rw-r--r--  2.0 unx     1037 b- defN 22-Dec-01 14:51 metricq_tools/__init__.py
--rw-r--r--  2.0 unx     2017 b- defN 22-Dec-01 14:51 metricq_tools/check.py
--rw-r--r--  2.0 unx    12150 b- defN 22-Dec-01 14:51 metricq_tools/discover.py
--rw-r--r--  2.0 unx     8051 b- defN 22-Dec-01 14:51 metricq_tools/inspect.py
--rw-r--r--  2.0 unx     1965 b- defN 22-Dec-01 14:51 metricq_tools/logging.py
--rw-r--r--  2.0 unx     3164 b- defN 22-Dec-01 14:51 metricq_tools/send.py
--rw-r--r--  2.0 unx     5665 b- defN 22-Dec-01 14:51 metricq_tools/spy.py
--rw-r--r--  2.0 unx     9774 b- defN 22-Dec-01 14:51 metricq_tools/summary.py
--rw-r--r--  2.0 unx     4343 b- defN 22-Dec-01 14:51 metricq_tools/utils.py
--rw-r--r--  2.0 unx      142 b- defN 22-Dec-01 14:51 metricq_tools/version.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Dec-01 14:51 metricq_tools-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7578 b- defN 22-Dec-01 14:51 metricq_tools-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-01 14:51 metricq_tools-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      272 b- defN 22-Dec-01 14:51 metricq_tools-0.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 22-Dec-01 14:51 metricq_tools-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1320 b- defN 22-Dec-01 14:51 metricq_tools-0.3.1.dist-info/RECORD
-16 files, 92733 bytes uncompressed, 32060 bytes compressed:  65.4%
+Zip file size: 34820 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-09 13:28 metricq_tools/__init__.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-Jun-09 13:28 metricq_tools/check.py
+-rw-r--r--  2.0 unx     1716 b- defN 23-Jun-09 13:28 metricq_tools/csv.py
+-rw-r--r--  2.0 unx    10743 b- defN 23-Jun-09 13:28 metricq_tools/discover.py
+-rw-r--r--  2.0 unx     3499 b- defN 23-Jun-09 13:28 metricq_tools/energy.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-Jun-09 13:28 metricq_tools/inspect.py
+-rw-r--r--  2.0 unx      397 b- defN 23-Jun-09 13:28 metricq_tools/logging.py
+-rw-r--r--  2.0 unx     1236 b- defN 23-Jun-09 13:28 metricq_tools/send.py
+-rw-r--r--  2.0 unx     5207 b- defN 23-Jun-09 13:28 metricq_tools/slurm.py
+-rw-r--r--  2.0 unx     3870 b- defN 23-Jun-09 13:28 metricq_tools/spy.py
+-rw-r--r--  2.0 unx     7675 b- defN 23-Jun-09 13:28 metricq_tools/summary.py
+-rw-r--r--  2.0 unx     8892 b- defN 23-Jun-09 13:28 metricq_tools/utils.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-09 13:28 metricq_tools/version.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-09 13:28 metricq_tools-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8140 b- defN 23-Jun-09 13:28 metricq_tools-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 13:28 metricq_tools-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      393 b- defN 23-Jun-09 13:28 metricq_tools-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-09 13:28 metricq_tools-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1554 b- defN 23-Jun-09 13:28 metricq_tools-1.0.0.dist-info/RECORD
+19 files, 97615 bytes uncompressed, 32292 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,49 +1,58 @@
 Filename: metricq_tools/__init__.py
 Comment: 
 
 Filename: metricq_tools/check.py
 Comment: 
 
+Filename: metricq_tools/csv.py
+Comment: 
+
 Filename: metricq_tools/discover.py
 Comment: 
 
+Filename: metricq_tools/energy.py
+Comment: 
+
 Filename: metricq_tools/inspect.py
 Comment: 
 
 Filename: metricq_tools/logging.py
 Comment: 
 
 Filename: metricq_tools/send.py
 Comment: 
 
+Filename: metricq_tools/slurm.py
+Comment: 
+
 Filename: metricq_tools/spy.py
 Comment: 
 
 Filename: metricq_tools/summary.py
 Comment: 
 
 Filename: metricq_tools/utils.py
 Comment: 
 
 Filename: metricq_tools/version.py
 Comment: 
 
-Filename: metricq_tools-0.3.1.dist-info/LICENSE
+Filename: metricq_tools-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: metricq_tools-0.3.1.dist-info/METADATA
+Filename: metricq_tools-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: metricq_tools-0.3.1.dist-info/WHEEL
+Filename: metricq_tools-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: metricq_tools-0.3.1.dist-info/entry_points.txt
+Filename: metricq_tools-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: metricq_tools-0.3.1.dist-info/top_level.txt
+Filename: metricq_tools-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: metricq_tools-0.3.1.dist-info/RECORD
+Filename: metricq_tools-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metricq_tools/__init__.py

```diff
@@ -1,29 +1,7 @@
-# metricq-tools
-# Copyright (C) 2021 ZIH, Technische Universitaet Dresden, Federal Republic of Germany
-#
-# All rights reserved.
-#
-# This file is part of metricq.
-#
-# metricq is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# metricq is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with metricq.  If not, see <http://www.gnu.org/licenses/>.
-
-# pylint: disable=logging-fstring-interpolation,logging-format-interpolation
-
 from . import discover, inspect, send, spy
 from .version import version as __version__
 
 __all__ = [
     "__version__",
     "discover",
     "inspect",
```

## metricq_tools/check.py

```diff
@@ -1,34 +1,28 @@
 import asyncio
 import math
 
 import click
-import click_completion
-import click_log
 import metricq
 
-from .logging import get_root_logger
-from .utils import metricq_server_option
+from .logging import logger
+from .utils import metricq_command
 from .version import version as client_version
 
-logger = get_root_logger()
 
-click_completion.init()
-
-
-async def check_for_non_finite(client):
+async def check_for_non_finite(client: metricq.HistoryClient) -> None:
     logger.info("Connecting...")
     await client.connect()
 
     start_time = metricq.Timestamp.from_iso8601("2010-01-01T00:00:00.0Z")
     end_time = metricq.Timestamp.from_now(metricq.Timedelta.from_string("7d"))
 
     bad_metrics = {}
 
-    async def check_metric(metric):
+    async def check_metric(metric: str) -> None:
         try:
             result = await client.history_aggregate(
                 metric, start_time=start_time, end_time=end_time
             )
             if not math.isfinite(result.minimum) or not math.isfinite(result.maximum):
                 bad_metrics[metric] = result
         except asyncio.TimeoutError:
@@ -48,24 +42,18 @@
             await request
             bar.update(1)
 
     for metric, aggregate in sorted(bad_metrics.items()):
         print(metric, aggregate)
 
 
-@click.command()
-@click_log.simple_verbosity_option(logger, default="warning")
-@metricq_server_option()
-def main(server):
-    """Check metrics for non-finite values."""
+@metricq_command(default_token="history-$USER-tool-check")
+def main(server: str, token: str) -> None:
+    """Check all historic metrics for non-finite values."""
     client = metricq.HistoryClient(
-        token="tool-check",
-        management_url=server,
+        token=token,
+        url=server,
         client_version=client_version,
         add_uuid=True,
     )
 
     asyncio.run(check_for_non_finite(client))
-
-
-if __name__ == "__main__":
-    main()
```

## metricq_tools/discover.py

```diff
@@ -1,77 +1,52 @@
-#!/usr/bin/env python3
-# Copyright (c) 2020, ZIH, Technische Universitaet Dresden, Federal Republic of Germany
-#
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#     * Redistributions of source code must retain the above copyright notice,
-#       this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above copyright notice,
-#       this list of conditions and the following disclaimer in the documentation
-#       and/or other materials provided with the distribution.
-#     * Neither the name of metricq nor the names of its contributors
-#       may be used to endorse or promote products derived from this software
-#       without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-# LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-# NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 import asyncio
 import datetime
 import json
 from asyncio import CancelledError, Queue
 from contextlib import asynccontextmanager
 from enum import Enum
 from enum import auto as enum_auto
-from typing import IO, Any, AsyncGenerator, Dict, List, Optional, Set, Tuple
+from typing import (
+    IO,
+    Any,
+    AsyncGenerator,
+    AsyncIterator,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Set,
+    Tuple,
+)
 
 import aio_pika
 import async_timeout
 import click
-import click_completion
-import click_log
-import humanize
+import humanize  # type: ignore
 import metricq
 from dateutil.parser import isoparse as parse_iso_datetime
 from dateutil.tz import tzlocal
-from metricq.types import Timedelta
+from metricq import Timedelta
 
-from .logging import get_root_logger
+from .logging import logger
 from .utils import (
     ChoiceParam,
     CommandLineChoice,
     DurationParam,
     OutputFormat,
-    metricq_server_option,
+    metricq_command,
     output_format_option,
 )
-from .version import version as client_version
-
-logger = get_root_logger()
-
-click_completion.init()
 
 
 class IgnoredEvent(CommandLineChoice, Enum):
     ErrorResponses = enum_auto()
 
     @classmethod
-    def default(cls):
+    def default(cls) -> "IgnoredEvent":
         return cls.ErrorResponses
 
 
 IGNORED_EVENT = ChoiceParam(IgnoredEvent, "ignored")
 
 TIMEOUT = DurationParam(default=None)
 
@@ -128,26 +103,26 @@
             metricq_version=response.get("metricqVersion"),
             client_version=response.get("version"),
             python_version=response.get("pythonVersion"),
             hostname=response.get("hostname"),
         )
 
     @classmethod
-    def _parse_datetime(cls, iso_string) -> Optional[datetime.datetime]:
+    def _parse_datetime(cls, iso_string: Optional[str]) -> Optional[datetime.datetime]:
         if iso_string is None:
             return None
         else:
             try:
                 dt = parse_iso_datetime(iso_string)
                 return dt.astimezone(tzlocal()).replace(tzinfo=None)
             except (AttributeError, ValueError, TypeError, OverflowError) as e:
                 logger.warning("Failed to parse ISO datestring ({}): {}", iso_string, e)
                 return None
 
-    def _fmt_parts(self):
+    def _fmt_parts(self) -> Iterable[str]:
         unknown_color = "bright_white"
 
         if self.error is not None:
             yield click.style(f"error: {self.error}", fg="bright_red")
             return
 
         alive = "alive" if self.alive else click.style("dead", fg="bright_red")
@@ -173,48 +148,51 @@
 
         if self.metricq_version:
             yield f"running {self.metricq_version}"
 
         if self.hostname:
             yield f"on {self.hostname}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return " ".join(self._fmt_parts())
 
 
 class Status(Enum):
     Ok = enum_auto()
     Warning = enum_auto()
     Error = enum_auto()
 
 
-def echo_status(status: Status, token: str, msg: str):
+def echo_status(status: Status, token: str, msg: str) -> None:
     style_status = {
         Status.Ok: {"text": "✔️", "fg": "green"},
         Status.Warning: {"text": "⚠", "fg": "yellow"},
         Status.Error: {"text": "❌", "fg": "red"},
     }
 
     status_prefix = click.style(**style_status[status])  # type: ignore
 
     click.echo(f'{status_prefix} {click.style(token, fg="cyan")}: {msg}')
 
 
 class MetricQDiscover(metricq.Agent):
-    def __init__(self, server):
-        super().__init__("discover", server, add_uuid=True)
-        self._response_queue: Queue[Tuple[str, dict]] = Queue()
+    _response_queue: Queue[Tuple[str, dict[str, Any]]]
+
+    def __init__(self, token: str, server: str) -> None:
+        super().__init__(token=token, url=server, add_uuid=True)
+        self._response_queue = Queue()
 
     async def discover(
         self,
         timeout: Optional[Timedelta],
-    ) -> AsyncGenerator[Tuple[str, dict], None]:
+    ) -> AsyncGenerator[Tuple[str, dict[str, Any]], None]:
         await self.connect()
         await self.rpc_consume()
 
+        assert self._management_channel is not None
         self._management_broadcast_exchange = (
             await self._management_channel.declare_exchange(
                 name=self._management_broadcast_exchange_name,
                 type=aio_pika.ExchangeType.FANOUT,
                 durable=True,
             )
         )
@@ -225,35 +203,35 @@
             response_callback=self.on_discover,
             function="discover",
             cleanup_on_response=False,
         )
 
         return self.responses(timeout)
 
-    def on_discover(self, from_token, **response):
+    def on_discover(self, from_token: str, **response: Any) -> None:
         logger.debug("response: {}", response)
         self._response_queue.put_nowait((from_token, response))
 
     async def responses(
         self, timeout: Optional[Timedelta]
-    ) -> AsyncGenerator[Tuple[str, dict], None]:
+    ) -> AsyncGenerator[Tuple[str, dict[str, Any]], None]:
         timeout_sec = timeout.s if timeout is not None else None
         async with async_timeout.timeout(timeout_sec):
             while True:
                 try:
                     yield await self._response_queue.get()
                 except CancelledError:
                     return
 
 
 def print_diff(
-    previous: Dict[str, dict],
-    current: Dict[str, dict],
+    previous: Dict[str, dict[str, Any]],
+    current: Dict[str, dict[str, Any]],
     format: OutputFormat,
-):
+) -> None:
     previous_clients = set(previous.keys())
     current_clients = set(current.keys())
 
     missing = previous_clients - current_clients
     additional = current_clients - previous_clients
     # reconnected = {
     #     client_token
@@ -269,15 +247,15 @@
                     "missing": {tok: previous[tok] for tok in missing},
                     "additional": {tok: current[tok] for tok in additional},
                 }
             )
         )
     elif format is OutputFormat.Pretty:
 
-        def print_list(heading: str, clients: set[str], bullet="*"):
+        def print_list(heading: str, clients: set[str], bullet: str = "*") -> None:
             if clients:
                 click.echo(heading)
                 for client_token in sorted(clients):
                     click.echo(f"{bullet} {client_token}")
 
         print_list(
             f"{click.style('Missing', fg='bright_red')} clients:",
@@ -288,60 +266,59 @@
             f"{click.style('Additional', fg='bright_green')} clients:",
             additional,
             bullet="+",
         )
 
 
 @asynccontextmanager
-async def stopping(client: MetricQDiscover):
+async def stopping(client: MetricQDiscover) -> AsyncIterator[MetricQDiscover]:
     try:
         yield client
     finally:
         await client.stop()
 
 
 async def discover(
+    *,
+    token: str,
     server: str,
-    diff: Optional[IO],
+    diff: Optional[IO[str]],
     timeout: Optional[Timedelta],
     ignored_events: Set[IgnoredEvent],
     format: OutputFormat,
-):
-    async with stopping(MetricQDiscover(server)) as discoverer:
+) -> None:
+    async with stopping(MetricQDiscover(token=token, server=server)) as discoverer:
         responses = await discoverer.discover(timeout=timeout)
 
         if diff:
             previous = json.load(diff)
             current = {
                 from_token: response async for (from_token, response) in responses
             }
 
             print_diff(previous=previous, current=current, format=format)
             return
 
         if format is OutputFormat.Json:
-
-            responses = {
+            responses_dict = {
                 from_token: response async for (from_token, response) in responses
             }
-            print(json.dumps(responses))
+            print(json.dumps(responses_dict))
 
         elif format is OutputFormat.Pretty:
             async for (from_token, response) in responses:
-                response = DiscoverResponse.parse(response)
-                if not response.error:
-                    status = Status.Ok if response.alive else Status.Warning
+                response_parsed = DiscoverResponse.parse(response)
+                if not response_parsed.error:
+                    status = Status.Ok if response_parsed.alive else Status.Warning
                     echo_status(status, from_token, str(response))
                 elif IgnoredEvent.ErrorResponses not in ignored_events:
                     echo_status(Status.Error, from_token, str(response))
 
 
-@click.command()
-@click.version_option(version=client_version)
-@metricq_server_option()
+@metricq_command(default_token="agent-$USER-tool-discover")
 @click.option(
     "-d",
     "--diff",
     type=click.File(encoding="utf-8"),
     metavar="JSON_FILE",
     help="Show a diff to a list of previously discovered clients (produced with --format=json)",
 )
@@ -350,30 +327,27 @@
     "--timeout",
     type=TIMEOUT,
     default=TIMEOUT.default,
     help="Wait at most this long for replies.",
 )
 @output_format_option()
 @click.option("--ignore", type=IGNORED_EVENT, multiple=True, help="Messages to ignore.")
-@click_log.simple_verbosity_option(logger, default="warning")
 def main(
     server: str,
-    diff: Optional[IO],
+    token: str,
+    diff: Optional[IO[str]],
     timeout: Optional[Timedelta],
     format: OutputFormat,
     ignore: List[IgnoredEvent],
-):
+) -> None:
     """Send an RPC broadcast on the MetricQ network and wait for replies from online clients."""
 
     asyncio.run(
         discover(
+            token=token,
             server=server,
             diff=diff,
             timeout=timeout,
             format=format,
             ignored_events=set(event for event in ignore),
         )
     )
-
-
-if __name__ == "__main__":
-    main()
```

## metricq_tools/inspect.py

```diff
@@ -1,67 +1,39 @@
-#!/usr/bin/env python3
-# Copyright (c) 2019, ZIH, Technische Universitaet Dresden, Federal Republic of Germany
-#
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#     * Redistributions of source code must retain the above copyright notice,
-#       this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above copyright notice,
-#       this list of conditions and the following disclaimer in the documentation
-#       and/or other materials provided with the distribution.
-#     * Neither the name of metricq nor the names of its contributors
-#       may be used to endorse or promote products derived from this software
-#       without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-# LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-# NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 from contextlib import suppress
+from typing import Any, Optional
 
 import aio_pika
 import click
-import click_completion
-import click_log
 import metricq
 import numpy as np
-import termplotlib as tpl
+import termplotlib as tpl  # type: ignore
 from metricq.datachunk_pb2 import DataChunk
 
-from metricq_tools.utils import metricq_server_option, metricq_token_option
-
-from .logging import get_root_logger
+from .logging import logger
+from .utils import metricq_command
 from .version import version as client_version
 
-logger = get_root_logger()
-
-click_completion.init()
-
 
 class InspectSink(metricq.Sink):
+    tokens: dict[Optional[str], int]
+    timestamps: list[float]
+    last_timestamp: Optional[float]
+    intervals: list[float]
+    values: list[float]
+    chunk_sizes: list[int]
+
     def __init__(
         self,
         metric: str,
         intervals_histogram: bool,
         chunk_sizes_histogram: bool,
         values_histogram: bool,
         print_data: bool,
-        *args,
-        **kwargs,
+        *args: Any,
+        **kwargs: Any,
     ):
         self._metric = metric
         self.tokens = {}
 
         self.print_intervals = intervals_histogram
         self.print_chunk_sizes = chunk_sizes_histogram
         self.print_values = values_histogram
@@ -70,57 +42,67 @@
         self.timestamps = []
         self.last_timestamp = None
         self.intervals = []
         self.values = []
         self.chunk_sizes = []
         super().__init__(*args, client_version=client_version, **kwargs)
 
-    async def connect(self):
+    async def connect(self) -> None:
         await super().connect()
 
         await self.subscribe([self._metric])
 
         click.echo(
             click.style(
                 f"Inspecting the metric '{self._metric}'... (Hit ctrl+C to stop)",
                 fg="green",
             )
         )
 
-    async def _on_data_message(self, message: aio_pika.IncomingMessage):
+    async def _on_data_message(
+        self, message: aio_pika.abc.AbstractIncomingMessage
+    ) -> None:
         async with message.process(requeue=True):
             body = message.body
             from_token = None
             with suppress(AttributeError):
-                from_token = message.client_id
+                # This probably doesn't ever work, but I'm just fixing the typing now, so I have to ignore
+                from_token = message.client_id  # type: ignore[attr-defined]
             metric = message.routing_key
+            if metric is None:
+                logger.warning(
+                    "received data message without routing key from {}", from_token
+                )
+                return
 
             if from_token not in self.tokens:
                 self.tokens[from_token] = 0
 
             self.tokens[from_token] += 1
 
             data_response = DataChunk()
             data_response.ParseFromString(body)
 
             self.chunk_sizes.append(len(data_response.value))
 
             await self._on_data_chunk(metric, data_response)
 
-    async def on_data(self, metric: str, timestamp: metricq.Timestamp, value: float):
+    async def on_data(
+        self, metric: str, timestamp: metricq.Timestamp, value: float
+    ) -> None:
         if self.print_data:
             click.echo(click.style("{}: {}".format(timestamp, value), fg="bright_blue"))
 
         self.timestamps.append(timestamp.posix)
         if self.last_timestamp:
             self.intervals.append(timestamp.posix - self.last_timestamp)
         self.last_timestamp = timestamp.posix
         self.values.append(value)
 
-    def on_signal(self, signal):
+    def on_signal(self, signal: str) -> None:
         try:
             click.echo()
             click.echo(
                 click.style(
                     "Received messages from: ",
                     fg="bright_red",
                 )
@@ -136,79 +118,77 @@
 
             click.echo()
 
             self.print_histograms()
         finally:
             super().on_signal(signal)
 
-    def print_histogram(self, values):
+    def print_histogram(self, values: list[float] | list[int]) -> None:
         counts, bin_edges = np.histogram(values, bins="doane")
         fig = tpl.figure()
         labels = [
             "[{:#.6g} - {:#.6g})".format(bin_edges[k], bin_edges[k + 1])
             for k in range(len(bin_edges) - 2)
         ]
         labels.append(
             "[{:#.6g} - {:#.6g}]".format(
                 bin_edges[len(bin_edges) - 2], bin_edges[len(bin_edges) - 1]
             )
         )
         fig.barh(counts, labels=labels)
         fig.show()
 
-    def print_chunk_sizes_histogram(self):
+    def print_chunk_sizes_histogram(self) -> None:
         click.echo(
             click.style(
                 "Distribution of the chunk sizes",
                 fg="yellow",
             )
         )
         click.echo()
 
         self.print_histogram(self.chunk_sizes)
 
         click.echo()
         click.echo()
 
-    def print_intervals_histogram(self):
+    def print_intervals_histogram(self) -> None:
         click.echo(
             click.style(
                 "Distribution of the duration between consecutive data points in seconds",
                 fg="yellow",
             )
         )
         click.echo()
 
         self.print_histogram(self.intervals)
 
         click.echo()
         click.echo()
 
-    def print_values_histogram(self):
+    def print_values_histogram(self) -> None:
         click.echo(
             click.style("Distribution of the values of the data points", fg="yellow")
         )
         click.echo()
 
         self.print_histogram(self.values)
 
-    def print_histograms(self):
+    def print_histograms(self) -> None:
         if self.print_chunk_sizes:
             self.print_chunk_sizes_histogram()
 
         if self.print_intervals and self.last_timestamp:
             self.print_intervals_histogram()
 
         if self.print_values:
             self.print_values_histogram()
 
 
-@click.command()
-@metricq_server_option()
-@metricq_token_option(default="metricq-inspect")
+@metricq_command(default_token="agent-$USER-tool-inspect")
 @click.option(
     "--intervals-histogram/--no-intervals-histogram",
     "-i/-I",
     default=True,
     help="Show an histogram of the observed distribution of durations between data points.",
 )
 @click.option(
@@ -221,37 +201,31 @@
     "--chunk-sizes-histogram/--no-chunk-sizes-histogram",
     "-c/-C",
     default=False,
     help="Show an histogram of the observed chunk sizes of all messages received.",
 )
 @click.option("--print-data-points/--no-print-data-points", "-d/-D", default=False)
 @click.argument("metric", required=True, nargs=1)
-@click_log.simple_verbosity_option(logger, default="WARNING")
-@click.version_option(version=client_version)
 def main(
-    server,
-    token,
-    metric,
-    intervals_histogram,
-    values_histogram,
-    chunk_sizes_histogram,
-    print_data_points,
-):
+    server: str,
+    token: str,
+    metric: str,
+    intervals_histogram: bool,
+    values_histogram: bool,
+    chunk_sizes_histogram: bool,
+    print_data_points: bool,
+) -> None:
     """Live metric data analysis and inspection on the MetricQ network.
 
     Consumes new data points for the given metric as they are submitted to the
     network, prints a statistical overview on exit.
     """
     sink = InspectSink(
         metric=metric,
         token=token,
-        management_url=server,
+        url=server,
         intervals_histogram=intervals_histogram,
         chunk_sizes_histogram=chunk_sizes_histogram,
         values_histogram=values_histogram,
         print_data=print_data_points,
     )
     sink.run()
-
-
-if __name__ == "__main__":
-    main()
```

## metricq_tools/logging.py

```diff
@@ -1,44 +1,18 @@
-#!/usr/bin/env python3
-# Copyright (c) 2021, ZIH, Technische Universitaet Dresden, Federal Republic of Germany
-#
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#     * Redistributions of source code must retain the above copyright notice,
-#       this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above copyright notice,
-#       this list of conditions and the following disclaimer in the documentation
-#       and/or other materials provided with the distribution.
-#     * Neither the name of metricq nor the names of its contributors
-#       may be used to endorse or promote products derived from this software
-#       without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-# LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-# NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 import logging
 
-import click_log
+import click_log  # type: ignore
 import metricq
 
 
-def get_root_logger():
+def get_root_logger() -> logging.Logger:
     logger = metricq.get_logger()
-    logger.setLevel(logging.WARN)
+    logger.setLevel(logging.WARNING)
     click_log.basic_config(logger)
     # logger.handlers[0].formatter = logging.Formatter(
     #     fmt="%(asctime)s [%(levelname)-8s] [%(name)-20s] %(message)s"
     # )
 
     return logger
+
+
+logger = get_root_logger()
```

## metricq_tools/send.py

```diff
@@ -1,86 +1,46 @@
-#!/usr/bin/env python3
-# Copyright (c) 2020, ZIH, Technische Universitaet Dresden, Federal Republic of Germany
-#
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#     * Redistributions of source code must retain the above copyright notice,
-#       this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above copyright notice,
-#       this list of conditions and the following disclaimer in the documentation
-#       and/or other materials provided with the distribution.
-#     * Neither the name of metricq nor the names of its contributors
-#       may be used to endorse or promote products derived from this software
-#       without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-# LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-# NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+from typing import Any
 
 import click
-import click_completion
-import click_log
-from metricq import Source, Timestamp
-from metricq.types import Metric
+from metricq import Metric, Source, Timestamp
 
-from metricq_tools.utils import TIMESTAMP, metricq_server_option, metricq_token_option
-
-from .logging import get_root_logger
+from .utils import TIMESTAMP, metricq_command
 from .version import version as client_version
 
-logger = get_root_logger()
-
-click_completion.init()
-
 
 class MetricQSend(Source):
-    def __init__(self, metric, timestamp, value, *args, **kwargs):
+    def __init__(
+        self, metric: str, timestamp: Timestamp, value: float, *args: Any, **kwargs: Any
+    ):
         super().__init__(*args, client_version=client_version, **kwargs)
         self.metric = metric
         self.timestamp = timestamp
         self.value = value
 
-    async def task(self):
+    async def task(self) -> None:
         await self.send(self.metric, time=self.timestamp, value=self.value)
         await self.stop()
 
 
-@click.command()
-@click_log.simple_verbosity_option(logger, default="warning")
-@click.version_option(version=client_version)
-@metricq_server_option()
-@metricq_token_option(default="source-send")
+@metricq_command(default_token="source-$USER-tool-send")
 @click.option(
     "--timestamp",
     type=TIMESTAMP,
     default=Timestamp.now(),
     show_default="now",
     help="Timestamp to send.",
 )
 @click.argument("metric", required=True)
 @click.argument("value", required=True, type=float)
-def main(server: str, token: str, timestamp: Timestamp, metric: Metric, value: float):
+def main(
+    server: str, token: str, timestamp: Timestamp, metric: Metric, value: float
+) -> None:
     """Send a single time-value pair for the given metric."""
     send = MetricQSend(
         token=token,
-        management_url=server,
+        url=server,
         metric=metric,
         timestamp=timestamp,
         value=value,
     )
 
     send.run()
-
-
-if __name__ == "__main__":
-    main()
```

## metricq_tools/spy.py

```diff
@@ -1,80 +1,46 @@
-#!/usr/bin/env python3
-# Copyright (c) 2020, ZIH, Technische Universitaet Dresden, Federal Republic of Germany
-#
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#     * Redistributions of source code must retain the above copyright notice,
-#       this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above copyright notice,
-#       this list of conditions and the following disclaimer in the documentation
-#       and/or other materials provided with the distribution.
-#     * Neither the name of metricq nor the names of its contributors
-#       may be used to endorse or promote products derived from this software
-#       without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-# LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-# NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 import asyncio
 from contextlib import suppress
 from typing import Any, Dict, Optional, TypedDict
 
 import aio_pika
 import click
-import click_completion
-import click_log
 import metricq
-from metricq.types import Metric
+from metricq import Metric
 
-from .logging import get_root_logger
-from .utils import OutputFormat, metricq_server_option, output_format_option
+from .utils import OutputFormat, metricq_command, output_format_option
 from .version import version as client_version
 
-logger = get_root_logger()
-
-click_completion.init()
-
 Database = str
 
 
 class SpyResults(TypedDict):
     location: Optional[Database]
     metadata: Dict[str, Any]
 
 
 class MetricQSpy(metricq.HistoryClient):
-    def __init__(self, server) -> None:
-        super().__init__("spy", server, client_version=client_version, add_uuid=True)
+    def __init__(self, token: str, url: str) -> None:
+        super().__init__(
+            token=token, url=url, client_version=client_version, add_uuid=True
+        )
         self._data_locations: Optional[asyncio.Queue[Database]] = None
 
-    async def spy(self, patterns, *, output_format: OutputFormat) -> None:
+    async def spy(self, patterns: list[str], *, output_format: OutputFormat) -> None:
         self._data_locations = asyncio.Queue()
         await self.connect()
 
         results: Dict[Metric, SpyResults] = dict()
 
         for pattern in patterns:
             result: Dict[Metric, Dict[str, Any]] = await self.get_metrics(
                 selector=pattern,
                 metadata=True,
                 historic=None,
-            )  # type: ignore # This is a bug in the type annotations for get_metrics
+            )
 
             assert isinstance(result, dict), "No metadata in result of get_metrics"
 
             now = metricq.Timestamp.now()
             window = metricq.Timedelta.from_s(60)
             for metric, metadata in result.items():
                 database: Optional[str] = None
@@ -115,30 +81,27 @@
 
         if output_format is OutputFormat.Json:
             import json
 
             click.echo(json.dumps(results, sort_keys=True, indent=None))
         await self.stop()
 
-    async def _on_history_response(self, message: aio_pika.IncomingMessage) -> None:
+    async def _on_history_response(
+        self, message: aio_pika.abc.AbstractIncomingMessage
+    ) -> None:
         database = message.app_id
+        if database is None:
+            database = "(unknown)"
         assert self._data_locations
         self._data_locations.put_nowait(database)
 
         await super()._on_history_response(message)
 
 
-@click.command()
-@click_log.simple_verbosity_option(logger, default="warning")
-@metricq_server_option()
+@metricq_command(default_token="agent-$USER-tool-spy")
 @output_format_option()
-@click.version_option(version=client_version)
 @click.argument("metrics", required=True, nargs=-1)
-def main(server, format: OutputFormat, metrics) -> None:
+def main(server: str, token: str, format: OutputFormat, metrics: list[str]) -> None:
     """Obtain metadata and storage location for a set of metrics."""
-    spy = MetricQSpy(server)
+    spy = MetricQSpy(token=token, url=server)
 
     asyncio.run(spy.spy(metrics, output_format=format))
-
-
-if __name__ == "__main__":
-    main()
```

## metricq_tools/summary.py

```diff
@@ -1,60 +1,28 @@
-#!/usr/bin/env python3
-# Copyright (c) 2021, ZIH, Technische Universitaet Dresden, Federal Republic of Germany
-#
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#     * Redistributions of source code must retain the above copyright notice,
-#       this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above copyright notice,
-#       this list of conditions and the following disclaimer in the documentation
-#       and/or other materials provided with the distribution.
-#     * Neither the name of metricq nor the names of its contributors
-#       may be used to endorse or promote products derived from this software
-#       without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-# LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-# NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
 import asyncio
 from sys import exit
+from typing import Any, Optional
 
 import click
-import click_completion
-import click_log
 import metricq
 import numpy as np
-import termplotlib as tpl
+import termplotlib as tpl  # type: ignore
 from metricq import Subscriber
 from tabulate import tabulate
 
-from metricq_tools.utils import metricq_server_option, metricq_token_option
-
-from .logging import get_root_logger
+from .utils import TemplateStringParam, metricq_command, run_cmd
 from .version import version as client_version
 
-logger = get_root_logger()
-
-click_completion.init()
-
 
 class Summary:
+    timestamps: dict[str, list[float]]
+    last_timestamp: dict[str, Optional[float]]
+    intervals: dict[str, list[float]]
+    values: dict[str, list[float]]
+
     def __init__(
         self,
         metrics: list[str],
         intervals_histogram: bool,
         values_histogram: bool,
         print_stats: bool,
         print_data: bool,
@@ -62,78 +30,79 @@
         self._metrics = metrics
 
         self.print_intervals = intervals_histogram
         self.print_values = values_histogram
         self.print_stats = print_stats
         self.print_data = print_data
 
-        self.timestamps = dict[str, list]()
-        self.last_timestamp = dict[str]()
-        self.intervals = dict[str, list]()
-        self.values = dict[str, list]()
+        self.timestamps = {}
+        self.last_timestamp = {}
+        self.intervals = {}
+        self.values = {}
 
         for metric in metrics:
-            self.timestamps[metric] = list()
+            self.timestamps[metric] = []
             self.last_timestamp[metric] = None
-            self.intervals[metric] = list()
-            self.values[metric] = list()
+            self.intervals[metric] = []
+            self.values[metric] = []
 
-    async def add_data(self, metric: str, timestamp: metricq.Timestamp, value: float):
+    async def add_data(
+        self, metric: str, timestamp: metricq.Timestamp, value: float
+    ) -> None:
         if self.print_data:
             click.echo(click.style("{}: {}".format(timestamp, value), fg="bright_blue"))
 
         self.timestamps[metric].append(timestamp.posix)
-        if self.last_timestamp[metric]:
-            self.intervals[metric].append(timestamp.posix - self.last_timestamp[metric])
+        if (last_timestamp := self.last_timestamp[metric]) is not None:
+            self.intervals[metric].append(timestamp.posix - last_timestamp)
         self.last_timestamp[metric] = timestamp.posix
         self.values[metric].append(value)
 
-    def _print_histogram(self, values):
+    def _print_histogram(self, values: list[float]) -> None:
         counts, bin_edges = np.histogram(values, bins="doane")
         fig = tpl.figure()
         labels = [
             "[{:#.6g} - {:#.6g})".format(bin_edges[k], bin_edges[k + 1])
             for k in range(len(bin_edges) - 2)
         ]
         labels.append(
             "[{:#.6g} - {:#.6g}]".format(
                 bin_edges[len(bin_edges) - 2], bin_edges[len(bin_edges) - 1]
             )
         )
         fig.barh(counts, labels=labels)
         fig.show()
 
-    def _print_intervals_histogram(self, intervals):
+    def _print_intervals_histogram(self, intervals: list[float]) -> None:
         click.echo(
             click.style(
                 "Distribution of the duration between consecutive data points in seconds",
                 fg="yellow",
             )
         )
         click.echo()
 
         self._print_histogram(intervals)
 
         click.echo()
         click.echo()
 
-    def _print_values_histogram(self, values):
+    def _print_values_histogram(self, values: list[float]) -> None:
         click.echo(
             click.style("Distribution of the values of the data points", fg="yellow")
         )
         click.echo()
 
         self._print_histogram(values)
 
         click.echo()
         click.echo()
 
-    def print(self):
+    def print(self) -> None:
         for metric in self._metrics:
-
             if self.values[metric]:
                 click.echo()
                 click.echo(click.style(f"Statistics of metric {metric!r}:", fg="green"))
                 click.echo()
 
                 if self.print_intervals and self.last_timestamp[metric]:
                     self._print_intervals_histogram(self.intervals[metric])
@@ -146,37 +115,37 @@
                     click.style(f"No Data for metric {metric!r} received!", fg="red")
                 )
                 click.echo()
 
         if self.print_stats:
             self._print_statistics()
 
-    def _print_statistics(self):
+    def _print_statistics(self) -> None:
         click.echo(
             click.style(
                 "Statistics",
                 fg="yellow",
             )
         )
         click.echo()
 
-        table = list[list]()
-
         headers = [
             "Metric",
             "Minimum",
             "Maximum",
             "Average",
             "Median",
             "Standard deviation",
             "Arithmetic mean",
             "Variance",
             "Count",
         ]
 
+        table: list[list[Any]] = [[] for _ in headers]
+
         for metric in self._metrics:
             if self.values[metric]:
                 table[0].append(metric)
                 table[1].append(np.amin(self.values[metric]))
                 table[2].append(np.amax(self.values[metric]))
                 table[3].append(np.average(self.values[metric]))
                 table[4].append(np.median(self.values[metric]))
@@ -197,102 +166,78 @@
 
         click.echo(tabulate(table, headers=headers, tablefmt="fancy_grid"))
 
         click.echo()
         click.echo()
 
 
-async def run_cmd(command):
-    logger.debug("Running command: {!r}", command)
-
-    proc = await asyncio.create_subprocess_shell(
-        command, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
-    )
-
-    stdout, stderr = await proc.communicate()
-
-    if stdout:
-        click.echo(stdout.decode())
-    if stderr:
-        click.echo(click.style(stderr.decode(), fg="red"))
-
-    if proc.returncode == 0:
-        logger.info("{!r} exited with {}", command, proc.returncode)
-    else:
-        logger.error("{!r} exited with {}", command, proc.returncode)
-
-    return proc.returncode
-
-
 async def async_main(
-    server,
-    token,
-    metric,
-    intervals_histogram,
-    values_histogram,
-    print_data_points,
-    print_statistics,
-    command,
-):
-    command_str = " ".join(command)
+    server: str,
+    token: str,
+    metric: list[str],
+    intervals_histogram: bool,
+    values_histogram: bool,
+    print_data_points: bool,
+    print_statistics: bool,
+    command: list[str],
+) -> Optional[int]:
     summary = Summary(
         intervals_histogram=intervals_histogram,
         values_histogram=values_histogram,
         print_data=print_data_points,
         print_stats=print_statistics,
         metrics=metric,
     )
     async with Subscriber(
         token=token,
-        management_url=server,
+        url=server,
         metrics=metric,
+        expires=3600,
+        client_version=client_version,
     ) as subscription:
-
-        returncode = await run_cmd(command_str)
+        returncode = await run_cmd(command)
 
         async with subscription.drain() as drain:
-            async for metric, timestamp, value in drain:
-                await summary.add_data(metric, timestamp, value)
+            async for m, timestamp, value in drain:
+                await summary.add_data(m, timestamp, value)
 
         summary.print()
 
         return returncode
 
 
-@click.command()
-@click_log.simple_verbosity_option(logger, default="WARNING")
-@metricq_server_option()
-@metricq_token_option(default="metricq-summary")
+@metricq_command(default_token="sink-$USER-tool-summary")
 @click.option(
     "--intervals-histogram/--no-intervals-histogram",
     "-i/-I",
     default=False,
     help="Show an histogram of the observed distribution of durations between data points.",
 )
 @click.option(
     "--values-histogram/--no-values-histogram",
     "-h/-H",
     default=False,
     help="Show an histogram of the observed metric values.",
 )
 @click.option("--print-data-points/--no-print-data-points", "-d/-D", default=False)
 @click.option("--print-statistics/--no-print-statistics", "-s/-S", default=True)
-@click.option("-m", "--metric", required=True, multiple=True)
-@click.version_option(version=client_version)
+@click.option(
+    "-m", "--metric", type=TemplateStringParam(), required=True, multiple=True
+)
 @click.argument("command", required=True, nargs=-1)
 def main(
-    server,
-    token,
-    metric,
-    intervals_histogram,
-    values_histogram,
-    print_data_points,
-    print_statistics,
-    command,
-):
+    server: str,
+    token: str,
+    metric: list[str],
+    intervals_histogram: bool,
+    values_histogram: bool,
+    print_data_points: bool,
+    print_statistics: bool,
+    command: list[str],
+) -> None:
     """Live metric data analysis and inspection on the MetricQ network.
 
     Consumes new data points for the given metric as they are submitted to the
     network, prints a statistical overview on exit.
     """
 
     returncode = asyncio.run(
@@ -305,11 +250,7 @@
             print_data_points,
             print_statistics,
             command,
         )
     )
 
     exit(returncode)
-
-
-if __name__ == "__main__":
-    main()
```

## metricq_tools/utils.py

```diff
@@ -1,16 +1,36 @@
+import asyncio
 import re
+from contextlib import suppress
 from enum import Enum, auto
-from typing import Any, Generic, List, Optional, Type, TypeVar, Union
+from getpass import getuser
+from socket import gethostname
+from string import Template
+from typing import Any, Callable, Generic, List, Optional, Type, TypeVar, Union, cast
 
+import click
+import click_log  # type: ignore
 from click import Context, Parameter, ParamType, option
-from metricq.types import Timedelta, Timestamp
+from dotenv import find_dotenv, load_dotenv
+from metricq import Timedelta, Timestamp
+
+from .logging import logger
+from .version import version as client_version
 
 _C = TypeVar("_C", covariant=True)
 
+# We do not interpolate (i.e. replace ${VAR} with corresponding environment variables).
+# That is because we want to be able to interpolate ourselves for metrics and tokens
+# using the same syntax. If it was only ${USER} for the token, we could use the
+# override functionality, but most unfortunately there is no standard environment
+# variable for the hostname. Even $HOST on zsh is not actually part of the environment.
+# ``override=false`` just means that environment variables have priority over the
+# env files.
+load_dotenv(dotenv_path=find_dotenv(".metricq"), interpolate=False, override=False)
+
 
 def camelcase_to_kebabcase(camelcase: str) -> str:
     # Match empty string preceeding uppercase character, but not at the start
     # of the word. Replace with '-' and make lowercase to get kebab-case word.
     return re.sub(r"(?<!^)(?=[A-Z])", "-", camelcase).lower()
 
 
@@ -31,15 +51,15 @@
     @classmethod
     def default(cls: Type[_C]) -> Optional[_C]:
         return None
 
     @classmethod
     def from_choice(cls: Type[_C], option: str) -> _C:
         member_name = kebabcase_to_camelcase(option.lower())
-        return getattr(cls, "__members__")[member_name]
+        return cast(_C, getattr(cls, "__members__")[member_name])
 
 
 ChoiceType = TypeVar("ChoiceType", bound=CommandLineChoice)
 
 
 class ChoiceParam(Generic[ChoiceType], ParamType):
     def __init__(self, cls: Type[ChoiceType], name: str):
@@ -72,22 +92,24 @@
 
 
 class OutputFormat(CommandLineChoice, Enum):
     Pretty = auto()
     Json = auto()
 
     @classmethod
-    def default(cls):
+    def default(cls) -> "OutputFormat":
         return OutputFormat.Pretty
 
 
 FORMAT = ChoiceParam(OutputFormat, "format")
 
+FC = TypeVar("FC", bound=Union[Callable[..., Any], click.Command])
 
-def output_format_option():
+
+def output_format_option() -> Callable[[FC], FC]:
     return option(
         "--format",
         type=FORMAT,
         default=OutputFormat.default(),
         show_default=OutputFormat.default().as_choice(),
         help="Print results in this format",
     )
@@ -117,48 +139,150 @@
                     ctx=ctx,
                 )
         else:
             return value
 
 
 class TimestampParam(ParamType):
+    """
+    Convert strings to ``metricq.Timestamp`` objects.
+
+    Accepts the following string inputs
+    - ISO-8601 timestamp (with timezone)
+    - Past Duration, e.g., '-10h' from now
+    - Posix timestamp, float seconds since 1.1.1970 midnight. (UTC)
+    - 'now'
+    - 'epoch', i.e., 1.1.1970 midnight
+    """
+
     name = "timestamp"
 
+    @staticmethod
+    def _convert(value: str) -> Timestamp:
+        if value == "now":
+            return Timestamp.now()
+        if value == "epoch":
+            return Timestamp.from_posix_seconds(0)
+        if value.startswith("-"):
+            # Plus because the minus makes negative timedelta
+            return Timestamp.now() + Timedelta.from_string(value)
+        with suppress(ValueError):
+            return Timestamp.from_posix_seconds(float(value))
+
+        return Timestamp.from_iso8601(value)
+
     def convert(
-        self, value: str, param: Optional[Parameter], ctx: Optional[Context]
-    ) -> Any:
+        self, value: Any, param: Optional[Parameter], ctx: Optional[Context]
+    ) -> Optional[Timestamp]:
         if value is None:
             return None
+        elif isinstance(value, Timestamp):
+            return value
         elif isinstance(value, str):
             try:
-                return Timestamp.from_iso8601(value)
+                return self._convert(value)
             except ValueError:
                 self.fail(
-                    "expected an ISO-8601 timestamp (e.g. 2012-12-21T00:00:00Z)",
+                    "expected an ISO-8601 timestamp (e.g. '2012-12-21T00:00:00Z'), "
+                    "POSIX timestamp, 'now', 'epoch', or a past duration (e.g. '-10h')",
                     param=param,
                     ctx=ctx,
                 )
         else:
-            return value
+            self.fail("unexpected type to convert to TimeStamp", param=param, ctx=ctx)
 
 
 TIMESTAMP = TimestampParam()
 
 
-def metricq_server_option():
+class TemplateStringParam(ParamType):
+    name = "text"
+    mapping: dict[str, str]
+
+    def __init__(self) -> None:
+        self.mapping = {}
+        with suppress(Exception):
+            self.mapping["USER"] = getuser()
+        with suppress(Exception):
+            self.mapping["HOST"] = gethostname()
+
+    def convert(
+        self, value: Any, param: Optional[Parameter], ctx: Optional[Context]
+    ) -> str:
+        if not isinstance(value, str):
+            raise TypeError("expected a string type for TemplateStringParam")
+        return Template(value).safe_substitute(self.mapping)
+
+
+def metricq_server_option() -> Callable[[FC], FC]:
     return option(
         "--server",
+        type=TemplateStringParam(),
         metavar="URL",
-        default="amqp://localhost/",
-        show_default=True,
+        required=True,
         help="MetricQ server URL.",
     )
 
 
-def metricq_token_option(default: str):
+def metricq_token_option(default: str) -> Callable[[FC], FC]:
     return option(
         "--token",
+        type=TemplateStringParam(),
         metavar="CLIENT_TOKEN",
         default=default,
         show_default=True,
         help="A token to identify this client on the MetricQ network.",
     )
+
+
+def metricq_command(default_token: str) -> Callable[[FC], click.Command]:
+    log_decorator = cast(
+        Callable[[FC], FC], click_log.simple_verbosity_option(logger, default="warning")
+    )
+    context_settings = {"auto_envvar_prefix": "METRICQ"}
+    epilog = (
+        "All options can be passed as environment variables prefixed with 'METRICQ_'."
+        "I.e., 'METRICQ_SERVER=amqps://...'.\n"
+        "\n"
+        "You can also create a '.metricq' file in the current or home directory that "
+        "contains environment variable settings in the same format.\n"
+        "\n"
+        "Some options, including server and token, can contain placeholders for $USER "
+        "and $HOST."
+    )
+
+    def decorator(func: FC) -> click.Command:
+        return click.version_option(version=client_version)(
+            log_decorator(
+                metricq_token_option(default_token)(
+                    metricq_server_option()(
+                        click.command(context_settings=context_settings, epilog=epilog)(
+                            func
+                        )
+                    )
+                )
+            )
+        )
+
+    return decorator
+
+
+async def run_cmd(command: list[str]) -> Optional[int]:
+    logger.debug("Running command: {!r}", command)
+
+    proc = await asyncio.create_subprocess_exec(
+        *command, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
+    )
+
+    stdout, stderr = await proc.communicate()
+
+    if stdout:
+        click.echo(stdout.decode())
+    if stderr:
+        click.echo(click.style(stderr.decode(), fg="red"))
+
+    if proc.returncode == 0:
+        logger.info("{!r} exited with {}", command, proc.returncode)
+    else:
+        logger.error("{!r} exited with {}", command, proc.returncode)
+
+    return proc.returncode
```

## metricq_tools/version.py

```diff
@@ -1,5 +1,5 @@
 # coding: utf-8
 # file generated by setuptools_scm
 # don't change, don't track in version control
-version = '0.3.1'
-version_tuple = (0, 3, 1)
+version = '1.0.0'
+version_tuple = (1, 0, 0)
```

## Comparing `metricq_tools-0.3.1.dist-info/LICENSE` & `metricq_tools-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `metricq_tools-0.3.1.dist-info/METADATA` & `metricq_tools-1.0.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,191 @@
 Metadata-Version: 2.1
 Name: metricq-tools
-Version: 0.3.1
+Version: 1.0.0
 Summary: Useful scripts to manage and inspect a MetricQ instance
 Home-page: https://github.com/metricq/metricq-tools
 Author: TU Dresden
 License: GPL3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: metricq (~=4.0)
+Requires-Dist: metricq (~=5.1)
 Requires-Dist: click
 Requires-Dist: click-log
-Requires-Dist: click-completion
 Requires-Dist: async-timeout (~=3.0)
 Requires-Dist: humanize (~=2.5)
 Requires-Dist: python-dateutil (~=2.8)
+Requires-Dist: python-dotenv (~=1.0.0)
+Requires-Dist: python-hostlist
 Requires-Dist: numpy
 Requires-Dist: termplotlib
 Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: black (==22.10.0) ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
 Requires-Dist: isort (~=5.0) ; extra == 'dev'
 Requires-Dist: check-manifest ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
+Requires-Dist: mypy (>=1.2.0) ; extra == 'dev'
+Requires-Dist: types-tabulate ; extra == 'dev'
+Requires-Dist: types-python-dateutil ; extra == 'dev'
 Requires-Dist: tox ; extra == 'dev'
 Provides-Extra: lint
 Requires-Dist: black (==22.10.0) ; extra == 'lint'
 Requires-Dist: flake8 ; extra == 'lint'
 Requires-Dist: isort (~=5.0) ; extra == 'lint'
 Requires-Dist: check-manifest ; extra == 'lint'
 Requires-Dist: pre-commit ; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
+Provides-Extra: typing
+Requires-Dist: mypy (>=1.2.0) ; extra == 'typing'
+Requires-Dist: types-tabulate ; extra == 'typing'
+Requires-Dist: types-python-dateutil ; extra == 'typing'
+Requires-Dist: pytest ; extra == 'typing'
 
 MetricQ Tools
 =============
 
 ![License: GPLv3](https://img.shields.io/badge/License-GPLv3-yellow)
 [![Build](https://github.com/metricq/metricq-tools/actions/workflows/package.yml/badge.svg)](https://github.com/metricq/metricq-tools/actions/workflows/package.yml)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![PyPI](https://img.shields.io/pypi/v/metricq-tools)](https://pypi.org/project/metricq-tools/)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/metricq-tools)
 
-Tools and utility scripts to monitor and administrate a MetricQ network.
+Tools and utility scripts to utilize, monitor, and administrate a MetricQ network.
 
-This repository includes a Python package that installs the following
-executables:
+
+Common command line options
+---------------------------
+
+```
+  --server URL          MetricQ server URL.  [required]
+  --token CLIENT_TOKEN  A token to identify this client on the MetricQ
+                        network.  [default: depends on the tool]
+  -v, --verbosity LVL   Either CRITICAL, ERROR, WARNING, INFO or DEBUG
+  --version             Show the version and exit.
+  --help                Show this message and exit.
+```
+
+All options for these tools can be passed as environment variables prefixed with `METRICQ_`,
+i.e., `METRICQ_SERVER=amqps://...`.
+You can also create a `.metricq` file in the current or home directory that contains environment variable settings in the same format.
+Some options, including server and token, can contain placeholders for `$USER` and `$HOST`.
+
+
+User tools
+----------
+
+`metricq-energy`
+----------------
+
+Run a command and calculate the energy consumption of a metric during this execution.
+
+```
+Usage: metricq-energy [OPTIONS] COMMAND...
+
+  Get a single energy value for a metric during the execution of the given
+  command. This value is just the integral of the metric over the time the
+  command was running.
+
+  The integral is calculated as the product of the arithmetic mean of all
+  values times the runtime of the given command. For the result to be
+  accurate, the metric should have updates in regular intervals and there
+  should be a sufficient number of values for the duration of the command.
+
+Options:
+  -m, --metric TEXT     [required]
+  --expires INTEGER     Queue expiration time in seconds. Set this value to
+                        the maximum time the command is expected to run.
+```
+
+`metricq-slurm`
+---------------
+
+Get the energy consumption for SLURM jobs.
+
+```
+Usage: metricq-slurm [OPTIONS]
+
+  Get an energy value for a slurm job given its job id.
+
+  This only works for exclusive jobs.
+
+Options:
+  -m, --metric TEXT     Pattern for per-metric power consumption. $HOST will
+                        be replaced with the host(s) running the job. The
+                        metric is assumed to be in W (watts).  [required]
+  -j, --jobs TEXT       job(.step) or list of job(.steps) as per sacct
+                        [required]
+```
+
+`metricq-summary`
+-----------------
+
+Run a command and collect statistics about a given metric during this execution.
+
+```
+Usage: metricq-summary [OPTIONS] COMMAND...
+
+  Live metric data analysis and inspection on the MetricQ network.
+
+  Consumes new data points for the given metric as they are submitted to the
+  network, prints a statistical overview on exit.
+
+Options:
+  -i, --intervals-histogram / -I, --no-intervals-histogram
+                                  Show an histogram of the observed
+                                  distribution of durations between data
+                                  points.
+  -h, --values-histogram / -H, --no-values-histogram
+                                  Show an histogram of the observed metric
+                                  values.
+  -d, --print-data-points / -D, --no-print-data-points
+  -s, --print-statistics / -S, --no-print-statistics
+  -m, --metric TEXT               [required]
+```
+
+Administrator tools
+-------------------
+
+These tools are intended for debugging and monitoring MetricQ networks.
 
 `metricq-check`
 ---------------
 
 Uses the aggregation of persisted metric values to quickly check, if it contains non-finite values like +/-inf and NaN.
 
 ```
 Usage: metricq-check [OPTIONS]
 
   Check metrics for non-finite values.
-
-Options:
-  -v, --verbosity LVL  Either CRITICAL, ERROR, WARNING, INFO or DEBUG
-  --server URL         MetricQ server URL.  [default: amqp://localhost/]
-  --help               Show this message and exit.
 ```
 
 `metricq-discover`
 ------------------
 
 Send an RPC broadcast on the MetricQ network and wait for replies from clients that are currently online.
 
 ```
 Usage: metricq-discover [OPTIONS]
 
   Send an RPC broadcast on the MetricQ network and wait for replies from online
   clients.
 
 Options:
-  --version                   Show the version and exit.
-  --server URL                MetricQ server URL.  [default:
-                              amqp://localhost/]
   -d, --diff JSON_FILE        Show a diff to a list of previously discovered
                               clients (produced with --format=json)
   -t, --timeout DURATION      Wait at most this long for replies.
   --format (pretty|json)      Print results in this format  [default:
                               (pretty)]
   --ignore (error-responses)  Messages to ignore.
-  -v, --verbosity LVL         Either CRITICAL, ERROR, WARNING, INFO or DEBUG
-  --help                      Show this message and exit.
 ```
 
 `metricq-inspect`
 -----------------
 
 Consumes new data points for the given metric as they are submitted to the network, prints a statistical overview on exit.
 
@@ -102,98 +194,48 @@
 
   Live metric data analysis and inspection on the MetricQ network.
 
   Consumes new data points for the given metric as they are submitted to the
   network, prints a statistical overview on exit.
 
 Options:
-  --server URL                    MetricQ server URL.  [default:
-                                  amqp://localhost/]
-  --token CLIENT_TOKEN            A token to identify this client on the
-                                  MetricQ network.  [default: metricq-inspect]
   -i, --intervals-histogram / -I, --no-intervals-histogram
                                   Show an histogram of the observed
                                   distribution of durations between data
                                   points.
   -h, --values-histogram / -H, --no-values-histogram
                                   Show an histogram of the observed metric
                                   values.
   -c, --chunk-sizes-histogram / -C, --no-chunk-sizes-histogram
                                   Show an histogram of the observed chunk
                                   sizes of all messages received.
   -d, --print-data-points / -D, --no-print-data-points
-  -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
-                                  DEBUG
-  --version                       Show the version and exit.
-  --help                          Show this message and exit.
 ```
 
 `metricq-send`
 --------------
 
 Send a single time-value pair for the given metric.
 
 ```
 Usage: metricq-send [OPTIONS] METRIC VALUE
 
   Send a single time-value pair for the given metric.
 
 Options:
-  -v, --verbosity LVL    Either CRITICAL, ERROR, WARNING, INFO or DEBUG
-  --version              Show the version and exit.
-  --server URL           MetricQ server URL.  [default: amqp://localhost/]
-  --token CLIENT_TOKEN   A token to identify this client on the MetricQ
-                         network.  [default: source-send]
   --timestamp TIMESTAMP  Timestamp to send.  [default: (now)]
-  --help                 Show this message and exit.
 ```
 
 `metricq-spy`
 -------------
 
 Obtain metadata and storage location for a set of metrics.
 
 ```
 Usage: metricq-spy [OPTIONS] METRICS...
 
   Obtain metadata and storage location for a set of metrics.
 
 Options:
-  -v, --verbosity LVL     Either CRITICAL, ERROR, WARNING, INFO or DEBUG
-  --server URL            MetricQ server URL.  [default: amqp://localhost/]
   --format (pretty|json)  Print results in this format  [default: (pretty)]
-  --help                  Show this message and exit.
 ```
 
-`metricq-summary`
------------------
-
-Live metric data analysis and inspection on the MetricQ network.
-
-```
-Usage: metricq-summary [OPTIONS] COMMAND...
-
-  Live metric data analysis and inspection on the MetricQ network.
-
-  Consumes new data points for the given metric as they are submitted to the
-  network, prints a statistical overview on exit.
-
-Options:
-  -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
-                                  DEBUG
-  --server URL                    MetricQ server URL.  [default:
-                                  amqp://localhost/]
-  --token CLIENT_TOKEN            A token to identify this client on the
-                                  MetricQ network.  [default: metricq-summary]
-  -i, --intervals-histogram / -I, --no-intervals-histogram
-                                  Show an histogram of the observed
-                                  distribution of durations between data
-                                  points.
-  -h, --values-histogram / -H, --no-values-histogram
-                                  Show an histogram of the observed metric
-                                  values.
-  -d, --print-data-points / -D, --no-print-data-points
-  -s, --print-statistics / -S, --no-print-statistics
-  -m, --metric TEXT               [required]
-  --version                       Show the version and exit.
-  --help                          Show this message and exit.
-```
```

