# Comparing `tmp/clockblocks-0.6.7rc1-py3-none-any.whl.zip` & `tmp/clockblocks-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54415 bytes, number of entries: 11
--rw-rw-r--  2.0 unx     2480 b- defN 21-Dec-07 01:48 clockblocks/__init__.py
--rw-rw-r--  2.0 unx    92195 b- defN 22-Mar-15 23:43 clockblocks/clock.py
--rw-rw-r--  2.0 unx     6179 b- defN 20-Aug-20 16:39 clockblocks/debug.py
--rw-rw-r--  2.0 unx     2178 b- defN 22-Jan-06 06:46 clockblocks/settings.py
--rw-rw-r--  2.0 unx    63811 b- defN 22-Mar-20 20:24 clockblocks/tempo_envelope.py
--rw-rw-r--  2.0 unx     8447 b- defN 22-Mar-24 06:00 clockblocks/utilities.py
--rw-rw-r--  2.0 unx    35147 b- defN 22-May-05 03:43 clockblocks-0.6.7rc1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2662 b- defN 22-May-05 03:43 clockblocks-0.6.7rc1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-May-05 03:43 clockblocks-0.6.7rc1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 22-May-05 03:43 clockblocks-0.6.7rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      905 b- defN 22-May-05 03:43 clockblocks-0.6.7rc1.dist-info/RECORD
-11 files, 214108 bytes uncompressed, 52891 bytes compressed:  75.3%
+Zip file size: 54542 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx     2629 b- defN 23-Jun-09 20:32 clockblocks/__init__.py
+-rw-rw-r--  2.0 unx    92690 b- defN 23-May-26 18:17 clockblocks/clock.py
+-rw-rw-r--  2.0 unx     6179 b- defN 22-Sep-24 17:32 clockblocks/debug.py
+-rw-rw-r--  2.0 unx     2178 b- defN 22-Sep-24 17:32 clockblocks/settings.py
+-rw-rw-r--  2.0 unx    63707 b- defN 23-Jun-05 17:35 clockblocks/tempo_envelope.py
+-rw-rw-r--  2.0 unx     8493 b- defN 23-Jun-05 17:35 clockblocks/utilities.py
+-rw-rw-r--  2.0 unx    35147 b- defN 23-Jun-09 20:37 clockblocks-0.6.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2720 b- defN 23-Jun-09 20:37 clockblocks-0.6.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 20:37 clockblocks-0.6.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jun-09 20:37 clockblocks-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      890 b- defN 23-Jun-09 20:37 clockblocks-0.6.9.dist-info/RECORD
+11 files, 214737 bytes uncompressed, 53048 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: clockblocks/tempo_envelope.py
 Comment: 
 
 Filename: clockblocks/utilities.py
 Comment: 
 
-Filename: clockblocks-0.6.7rc1.dist-info/LICENSE
+Filename: clockblocks-0.6.9.dist-info/LICENSE
 Comment: 
 
-Filename: clockblocks-0.6.7rc1.dist-info/METADATA
+Filename: clockblocks-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: clockblocks-0.6.7rc1.dist-info/WHEEL
+Filename: clockblocks-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: clockblocks-0.6.7rc1.dist-info/top_level.txt
+Filename: clockblocks-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: clockblocks-0.6.7rc1.dist-info/RECORD
+Filename: clockblocks-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clockblocks/__init__.py

```diff
@@ -24,7 +24,11 @@
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
 from .clock import Clock, TimeStamp, DeadClockError, ClockKilledError
 from .tempo_envelope import TempoEnvelope, TempoHistory, MetricPhaseTarget
 from .utilities import sleep_precisely, sleep_precisely_until, current_clock, wait, fork, fork_unsynchronized, \
     wait_forever, wait_for_children_to_finish
+import importlib.metadata
+
+__version__ = importlib.metadata.version('clockblocks')
+__author__ = importlib.metadata.metadata('clockblocks')['Author']
```

## clockblocks/clock.py

```diff
@@ -14,29 +14,30 @@
 #  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;     #
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
-import itertools
 
+from __future__ import annotations
+import itertools
 from .tempo_envelope import MetricPhaseTarget, TempoEnvelope, TempoHistory
 from expenvelope._utilities import _get_extrema_and_inflection_points
 from collections import namedtuple
 from multiprocessing.pool import ThreadPool
 from threading import Lock
 import logging
 from copy import deepcopy
 import inspect
 from .utilities import sleep_precisely_until, current_clock, _PrintColors
 from .debug import _print_and_clear_debug_calc_times
 from functools import total_ordering, wraps
 import textwrap
-from typing import Union, Sequence, Iterator, Tuple, Callable, TypeVar
+from typing import Sequence, Iterator, Callable, TypeVar
 import time
 import threading
 from .settings import catching_up_child_clocks_threshold_min, catching_up_child_clocks_threshold_max, \
     running_behind_warning_threshold_long, running_behind_warning_threshold_short
 from numbers import Real
 
 
@@ -130,17 +131,17 @@
     :param pool_size: the size of the process pool for unsynchronized forks, which are used for playing notes. Only
         has an effect if this is the master clock.
     :ivar name: the name of this clock (string)
     :ivar parent: the parent Clock to which this clock belongs (Clock, or None if master clock)
     :ivar tempo_history: TempoHistory describing how this clock has changed or will change tempo
     """
 
-    def __init__(self, name: str = None, parent: 'Clock' = None, initial_rate: float = None,
+    def __init__(self, name: str = None, parent: Clock = None, initial_rate: float = None,
                  initial_tempo: float = None, initial_beat_length: float = None,
-                 timing_policy: Union[str, float] = 0.98, synchronization_policy: str = None, pool_size: int = 200):
+                 timing_policy: str | float = 0.98, synchronization_policy: str = None, pool_size: int = 200):
 
         self.name = name
         self.parent = parent
         if self.parent is not None and self not in self.parent._children:
             self.parent._children.append(self)
         self._children = []
 
@@ -213,101 +214,101 @@
         self.priority = 0 if self.is_master() else next(self.parent._priority_counter)
 
     ##################################################################################################################
     #                                                  Family Matters
     ##################################################################################################################
 
     @property
-    def master(self) -> 'Clock':
+    def master(self) -> Clock:
         """
         The master clock under which this clock operates (possibly itself)
         """
         return self if self.is_master() else self.parent.master
 
     def is_master(self) -> bool:
         """
         Check if this is the master clock
 
         :return: True if this is the master clock, False otherwise
         """
         return self.parent is None
 
-    def children(self) -> Sequence['Clock']:
+    def children(self) -> Sequence[Clock]:
         """
         Get all direct child clocks forked by this clock.
 
         :return: tuple of all child clocks of this clock
         """
         return tuple(self._children)
 
-    def iterate_inheritance(self, include_self: bool = True) -> Iterator['Clock']:
+    def iterate_inheritance(self, include_self: bool = True) -> Iterator[Clock]:
         """
         Iterate through parent, grandparent, etc. of this clock up until the master clock
 
         :param include_self: whether or not to include this clock in the iterator or start with the parent
         :return: iterator going up the clock family tree up to the master clock
         """
 
         clock = self
         if include_self:
             yield clock
         while clock.parent is not None:
             clock = clock.parent
             yield clock
 
-    def inheritance(self, include_self: bool = True) -> Sequence['Clock']:
+    def inheritance(self, include_self: bool = True) -> Sequence[Clock]:
         """
         Get all parent, grandparent, etc. of this clock up until the master clock
 
         :param include_self: whether or not to include this clock in the iterator or start with the parent
         :return: tuple containing the clock's inheritance
         """
         return tuple(self.iterate_inheritance(include_self))
 
-    def iterate_all_relatives(self, include_self: bool = False) -> Iterator['Clock']:
+    def iterate_all_relatives(self, include_self: bool = False) -> Iterator[Clock]:
         """
         Iterate through all related clocks to this clock.
 
         :param include_self: whether or not to include this clock in the iterator
         :return: iterator going through all clocks in the family tree, starting with the master
         """
         if include_self:
             return self.master.iterate_descendants(True)
         else:
             return (c for c in self.master.iterate_descendants(True) if c is not self)
 
-    def iterate_descendants(self, include_self: bool = False) -> Iterator['Clock']:
+    def iterate_descendants(self, include_self: bool = False) -> Iterator[Clock]:
         """
         Iterate through all children, grandchildren, etc. of this clock
 
         :param include_self: whether or not to include this clock in the iterator
         :return: iterator going through all descendants
         """
         if include_self:
             yield self
         for child_clock in self._children:
             yield child_clock
             for descendant_of_child in child_clock.iterate_descendants():
                 yield descendant_of_child
 
-    def descendants(self) -> Sequence['Clock']:
+    def descendants(self) -> Sequence[Clock]:
         """
         Get all children, grandchildren, etc. of this clock
 
         :return: tuple of all descendants
         """
         return tuple(self.iterate_descendants())
 
     def print_family_tree(self) -> None:
         """
         Print a hierarchical representation of this clock's family tree.
         """
         print(self.master._child_tree_string(self))
 
-    def _child_tree_string(self, highlight_clock: 'Clock' = None) -> str:
+    def _child_tree_string(self, highlight_clock: Clock = None) -> str:
         name_text = self.name if self.name is not None else "(UNNAMED)"
         if highlight_clock is self:
             name_text = _PrintColors.BOLD + name_text + _PrintColors.END
         children = self.children()
         if len(children) == 0:
             return name_text
         return "{}:\n{}".format(
@@ -342,15 +343,15 @@
     def _resolve_synchronization_policy(self):
         # resolves a value of "inherit" if necessary
         for clock in self.iterate_inheritance():
             if clock.synchronization_policy != "inherit":
                 return clock.synchronization_policy
 
     @property
-    def timing_policy(self) -> Union[str, float]:
+    def timing_policy(self) -> str | float:
         """
         Determines how this clock should respond to getting behind.
         Allowable values are "absolute", "relative" or a float between 0 and 1 representing a balance between
         absolute and relative.
         """
         return self._timing_policy
 
@@ -481,15 +482,15 @@
 
     ##################################################################################################################
     #                                                  Tempo Changes
     ##################################################################################################################
 
     @tempo_modification
     def set_beat_length_target(self, beat_length_target: float, duration: float, curve_shape: float = 0,
-                               metric_phase_target: Union[float, MetricPhaseTarget, Tuple] = None,
+                               metric_phase_target: float | MetricPhaseTarget | tuple = None,
                                duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Set a target beat length for this clock to reach in duration beats/seconds (with the unit defined by
         duration_units).
 
         :param beat_length_target: The beat length we want to reach
         :param duration: How long until we reach that beat length
@@ -503,15 +504,15 @@
         :param truncate: Whether or not to delete all future tempo plans before setting this goal.
         """
         self.tempo_history.set_beat_length_target(beat_length_target, duration, curve_shape, metric_phase_target,
                                                   duration_units, truncate)
 
     @tempo_modification
     def set_rate_target(self, rate_target: float, duration: float, curve_shape: float = 0,
-                        metric_phase_target: Union[float, MetricPhaseTarget, Tuple] = None,
+                        metric_phase_target: float | MetricPhaseTarget | tuple = None,
                         duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Set a target rate for this clock to reach in duration beats/seconds (with the unit defined by duration_units)
 
         :param rate_target: The rate we want to reach
         :param duration: How long until we reach that tempo
         :param curve_shape: > 0 makes change happen later, < 0 makes change happen sooner
@@ -524,15 +525,15 @@
         :param truncate: Whether or not to delete all future tempo plans before setting this goal.
         """
         self.tempo_history.set_rate_target(rate_target, duration, curve_shape, metric_phase_target,
                                            duration_units, truncate)
 
     @tempo_modification
     def set_tempo_target(self, tempo_target: float, duration: float, curve_shape: float = 0,
-                         metric_phase_target: Union[float, MetricPhaseTarget, Tuple] = None,
+                         metric_phase_target: float | MetricPhaseTarget | tuple = None,
                          duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Set a target tempo for this clock to reach in duration beats/seconds (with the unit defined by duration_units)
 
         :param tempo_target: The tempo we want to reach
         :param duration: How long until we reach that tempo
         :param curve_shape: > 0 makes change happen later, < 0 makes change happen sooner
@@ -546,15 +547,15 @@
         """
         self.tempo_history.set_tempo_target(tempo_target, duration, curve_shape, metric_phase_target,
                                             duration_units, truncate)
 
     @tempo_modification
     def set_beat_length_targets(self, beat_length_targets: Sequence[float], durations: Sequence[float],
                                 curve_shapes: Sequence[float] = None,
-                                metric_phase_targets: Sequence[Union[float, MetricPhaseTarget, Tuple]] = None,
+                                metric_phase_targets: Sequence[float | MetricPhaseTarget | tuple] = None,
                                 duration_units: str = "beats", truncate: bool = True, loop: bool = False) -> None:
         """
         Same as set_beat_length_target, except that you can set multiple targets at once by providing lists to each
         of the arguments.
 
         :param beat_length_targets: list of the target beat_lengths
         :param durations: list of segment durations (in beats or seconds, as defined by duration_units)
@@ -578,15 +579,15 @@
             [s.curve_shape for s in segments_to_loop],
             units="beatlength"
         )
 
     @tempo_modification
     def set_rate_targets(self, rate_targets: Sequence[float], durations: Sequence[float],
                          curve_shapes: Sequence[float] = None,
-                         metric_phase_targets: Sequence[Union[float, MetricPhaseTarget, Tuple]] = None,
+                         metric_phase_targets: Sequence[float | MetricPhaseTarget | tuple] = None,
                          duration_units: str = "beats", truncate: bool = True, loop: bool = False) -> None:
         """
         Same as set_rate_target, except that you can set multiple targets at once by providing lists to each
         of the arguments.
 
         :param rate_targets: list of the target rates
         :param durations: list of segment durations (in beats or seconds, as defined by duration_units)
@@ -602,15 +603,15 @@
                                             duration_units, truncate)
         if loop:
             self._loop_segments(self.tempo_history.segments[-len(rate_targets):])
 
     @tempo_modification
     def set_tempo_targets(self, tempo_targets: Sequence[float], durations: Sequence[float],
                           curve_shapes: Sequence[float] = None,
-                          metric_phase_targets: Sequence[Union[float, MetricPhaseTarget, Tuple]] = None,
+                          metric_phase_targets: Sequence[float | MetricPhaseTarget | tuple] = None,
                           duration_units: str = "beats", truncate: bool = True, loop: bool = False) -> None:
         """
         Same as set_tempo_target, except that you can set multiple targets at once by providing lists to each
         of the arguments.
 
         :param tempo_targets: list of the target tempos
         :param durations: list of segment durations (in beats or seconds, as defined by duration_units)
@@ -791,15 +792,15 @@
         else:
             logging.warning("Ran out of threads in the master clock's ThreadPool; small thread creation delays may "
                             "result. You can increase the number of threads in the pool to avoid this.")
             threading.Thread(target=target, args=args, kwargs=kwargs, daemon=True).start()
 
     def fork(self, process_function: Callable, args: Sequence = (), kwargs: dict = None, name: str = None,
              initial_rate: float = None, initial_tempo: float = None, initial_beat_length: float = None,
-             schedule_at: Union[float, MetricPhaseTarget] = None, done_callback: Callable = None) -> 'Clock':
+             schedule_at: float | MetricPhaseTarget = None, done_callback: Callable = None) -> Clock:
         """
         Spawns a parallel process running on a child clock.
 
         :param process_function: function defining the process to be spawned
         :param args: arguments to be passed to the process function. One subtlety to note here: if the number of
             arguments passed is one fewer than the number taken by the function, the clock on which the process is
             forked will be passed as the first argument, followed by the arguments given. For instance, if we define
@@ -1184,15 +1185,15 @@
         self._queue.remove(next_wake_up_call)
         self._advance_tempo_map_to_beat(wake_up_beat)
         # tell the process of the clock being woken to go ahead and do it's thing
         next_wake_up_call.clock._dormant = False  # this flag tells us when that process hits a new wait
         next_wake_up_call.clock._wait_event.set()
         self._wait_for_child_to_finish_processing(next_wake_up_call.clock)
 
-    def _wait_for_child_to_finish_processing(self, child_clock: 'Clock') -> None:
+    def _wait_for_child_to_finish_processing(self, child_clock: Clock) -> None:
         # wait for the child clock that we woke up either to finish completely or to finish processing
         while child_clock in self._children and not child_clock._dormant:
             # note that sleeping a tiny amount is better than a straight while loop,
             # which slows down the other threads with its greediness
             time.sleep(0.000001)
 
     def _complete_timestamp_data(self):
@@ -1337,15 +1338,15 @@
         """
         while True:
             try:
                 self.wait(1.0)
             except DeadClockError:
                 break
 
-    def rouse_and_hold(self, holding_clock: 'Clock' = None) -> None:
+    def rouse_and_hold(self, holding_clock: Clock = None) -> None:
         """
         Rouse this clock if it is dormant, but keep it suspended until release_from_suspension is called.
         Generally this would not be called by the user, but it is useful for callback functions operating outside
         of the clock system, since they can wake up the clock of interest, carry out what they need to carry out
         and then release the clock from suspension.
 
         :param holding_clock: when rouse_and_hold is called on a child clock, all parents/grandparents/etc. must also
@@ -1369,15 +1370,15 @@
 
         while not self._wait_keeper.being_held:
             time.sleep(0.000001)
 
         if not self.is_master() and self.parent._dormant:
             self.parent.rouse_and_hold(holding_clock)
 
-    def release_from_suspension(self, releasing_clock: 'Clock' = None) -> None:
+    def release_from_suspension(self, releasing_clock: Clock = None) -> None:
         """
         Called after "rouse_and_hold" to release the roused clock.
 
         :param releasing_clock: the clock providing the initial impetus to release from suspension. Just like
             rouse_and_hold, a release propagates up the family tree, but we need to keep track of the initial clock
             from which it propagates. (Again, this is an implementation detail.
         """
@@ -1387,46 +1388,60 @@
         if not self.is_master():
             self.parent.release_from_suspension(releasing_clock)
 
     ##################################################################################################################
     #                                                 Fast-forwarding
     ##################################################################################################################
 
+    def fast_forward(self, on_or_off=True) -> None:
+        """
+        Set fast-forwarding of the clock; when fast-forwarding, all waiting is instantaneous.
+        (Only available on the master clock.)
+
+        :param on_or_off: if True, start fast-forwarding; if False, stop fast-forwarding.
+        """
+        if not self.is_master():
+            raise ValueError("Only the master clock can be fast-forwarded.")
+        if on_or_off:
+            self._fast_forward_goal = float("inf")
+        else:
+            self._fast_forward_goal = None
+
     def fast_forward_to_time(self, t: float) -> None:
         """
-        Fast forward clock, skipping instantaneously to the time of t seconds. (Only available on the master clock.)
+        Fast-forward clock, skipping instantaneously to the time of t seconds. (Only available on the master clock.)
 
         :param t: time to fast forward to
         """
         if not self.is_master():
             raise ValueError("Only the master clock can be fast-forwarded.")
         if t < self.time():
             raise ValueError("Cannot fast-forward to a time in the past.")
         self._fast_forward_goal = t
 
     def fast_forward_in_time(self, t: float) -> None:
         """
-        Fast forward clock, skipping ahead instantaneously by t seconds. (Only available on the master clock.)
+        Fast-forward clock, skipping ahead instantaneously by t seconds. (Only available on the master clock.)
 
         :param t: number of seconds to fast forward by
         """
         self.fast_forward_to_time(self.time() + t)
 
     def fast_forward_to_beat(self, b: float) -> None:
         """
-        Fast forward clock, skipping instantaneously to beat b. (Only available on the master clock.)
+        Fast-forward clock, skipping instantaneously to beat b. (Only available on the master clock.)
 
         :param b: beat to fast forward to
         """
         assert b > self.beat(), "Cannot fast-forward to a beat in the past."
         self.fast_forward_in_beats(b - self.beat())
 
     def fast_forward_in_beats(self, b: float) -> None:
         """
-        Fast forward clock, skipping ahead instantaneously by b beats. (Only available on the master clock.)
+        Fast-forward clock, skipping ahead instantaneously by b beats. (Only available on the master clock.)
 
         :param b: number of beats to fast forward by
         """
         self.fast_forward_in_time(self.tempo_history.get_wait_time(b))
 
     def is_fast_forwarding(self) -> bool:
         """
```

## clockblocks/tempo_envelope.py

```diff
@@ -16,20 +16,21 @@
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
+from __future__ import annotations
 from expenvelope import Envelope, EnvelopeSegment
 from copy import deepcopy
 from .utilities import snap_float_to_nice_decimal, current_clock
 import logging
 import math
-from typing import Union, Sequence, Tuple
+from typing import Sequence
 
 
 class TempoEnvelope(Envelope):
     r"""
     A subclass of :class:`~expenvelope.envelope.Envelope` that is specifically designed for representing changing tempo
     curves. The underlying envelope represents beat length as a function of the current beat, which means that the
     area under the curve represents how much time should pass from one beat to the next (beats * sec/beat = sec).
@@ -40,15 +41,15 @@
     :param durations: durations of the curve segments in the units specified by the `duration_units` argument
     :param curve_shapes: see :func:`~expenvelope.envelope.Envelope.from_levels_and_durations`
     :param units: one of "tempo", "rate" or "beat length", determining how we interpret the levels given
     :param duration_units: either "beats" or "time", determining how we interpret the durations given
     """
 
     def __init__(self, levels: Sequence = (60,), durations: Sequence[float] = (),
-                 curve_shapes: Sequence[Union[float, str]] = None,
+                 curve_shapes: Sequence[float | str] = None,
                  units: str = "tempo", duration_units: str = "beats"):
         units = units.lower().replace(" ", "")
         if units not in ("tempo", "rate", "beatlength"):
             raise ValueError("Units must be either \"tempo\" or \"rate\" or \"beatlength\".")
         if duration_units not in ("beats", "time"):
             raise ValueError("Duration units must be either \"beats\" or \"time\".")
 
@@ -62,31 +63,31 @@
 
     ##################################################################################################################
     #                                                Class Methods
     ##################################################################################################################
 
     @classmethod
     def from_levels_and_durations(cls, levels: Sequence = (0, 0), durations: Sequence[float] = (0,),
-                                  curve_shapes: Sequence[Union[float, str]] = None,
-                                  units: str = "tempo", duration_units: str = "beats") -> 'TempoEnvelope':
+                                  curve_shapes: Sequence[float | str] = None,
+                                  units: str = "tempo", duration_units: str = "beats") -> TempoEnvelope:
         """
         Constructs a TempoEnvelope from the given levels, durations and curve shapes, using the specified units.
 
         :param levels: levels of the curve segments (i.e. tempo values) in the units specified by the `units` argument
         :param durations: durations of the curve segments in the units specified by the `duration_units` argument
         :param curve_shapes: see :func:`~expenvelope.envelope.Envelope.from_levels_and_durations`
         :param units: one of "tempo", "rate" or "beat length", determining how we interpret the levels given
         :param duration_units: either "beats" or "time", determining how we interpret the durations given
         :return: a TempoEnvelope, constructed accordingly
         """
         return cls(levels, durations, curve_shapes, units=units, duration_units=duration_units)
 
     @classmethod
     def from_levels(cls, levels: Sequence[float], length: float = 1.0, units: str = "tempo",
-                    duration_units: str = "beats") -> 'TempoEnvelope':
+                    duration_units: str = "beats") -> TempoEnvelope:
         """
         Constructs a TempoEnvelope from the given levels and total length, using the specified units.
 
         :param levels: levels of the curve segments (i.e. tempo values) in the units specified by the `units` argument
         :param length: total length of the tempo curve, in the units specified by the `duration_units` argument
         :param units: one of "tempo", "rate" or "beat length", determining how we interpret the levels given
         :param duration_units: either "beats" or "time", determining how we interpret the durations given
@@ -96,15 +97,15 @@
         return cls(
             *TempoEnvelope._levels_and_length_to_levels_durations_and_curves(levels, length),
             units=units, duration_units=duration_units
         )
 
     @classmethod
     def from_list(cls, constructor_list: Sequence, units: str = "tempo",
-                  duration_units: str = "beats") -> 'TempoEnvelope':
+                  duration_units: str = "beats") -> TempoEnvelope:
         """
         Construct a TempoEnvelope from a list that can take a number of formats
 
         :param constructor_list: see :func:`~expenvelope.envelope.Envelope.from_list`
         :param units: one of "tempo", "rate" or "beat length", determining how we interpret the levels given
         :param duration_units: either "beats" or "time", determining how we interpret the durations given
         :return: a TempoEnvelope, constructed accordingly
@@ -127,15 +128,15 @@
                 return cls.from_levels_and_durations(constructor_list[0], constructor_list[1], constructor_list[2],
                                                      units=units, duration_units=duration_units)
         else:
             # just given levels
             return cls.from_levels(constructor_list, units=units, duration_units=duration_units)
 
     @classmethod
-    def from_points(cls, *points, units: str = "tempo", duration_units: str = "beats") -> 'TempoEnvelope':
+    def from_points(cls, *points, units: str = "tempo", duration_units: str = "beats") -> TempoEnvelope:
         """
         Construct an envelope from a list of (beat/time, tempo/rate/beat length) pairs. Units are defined by the
         `units` and `duration_units` parameters.
 
         :param points: list of points, each of which is of the form (time, value) or (time, value, curve_shape)
         :param units: one of "tempo", "rate" or "beat length", determining how we interpret the tempo values
         :param duration_units: either "beats" or "time", determining how we interpret the time values
@@ -146,15 +147,15 @@
             raise ValueError("TempoEnvelope must start from beat/time zero; when constructing from points, the "
                              "first point must be of the form (0, [start tempo], [optional curve shape]).")
         return cls(levels, durations, curve_shapes, units=units, duration_units=duration_units)
 
     @classmethod
     def from_function(cls, function, domain_start=0, domain_end=1, units: str = "tempo", duration_units: str = "beats",
                       scanning_step_size: float = 0.05, key_point_resolution_multiple: int = 2, iterations: int = 6,
-                      min_key_point_distance: float = 1e-7) -> 'TempoEnvelope':
+                      min_key_point_distance: float = 1e-7) -> TempoEnvelope:
         """
         Constructs a TempoEnvelope that approximates an arbitrary function. The domain of the function is in units
         defined by the `duration_units` parameter, and the range is in units defined by the `units` parameter.
 
         :param function: A function from beat/time to tempo/rate/beat length, as defined by the `duration_units` and
             `units` parameters.
         :param domain_start: see :func:`~expenvelope.envelope.Envelope.from_function`
@@ -212,24 +213,24 @@
         return the tempo after the jump, though this can be overridden with the `from_left` argument.
 
         :param beat: the beat at which to get the tempo
         :param from_left: whether to evaluate from the right or left-hand side of the beat in question
         """
         return self.rate_at(beat, from_left) * 60
 
-    def extend_to(self, beat: float) -> 'TempoEnvelope':
+    def extend_to(self, beat: float) -> TempoEnvelope:
         """
         Extends the end of this TempoEnvelope to the given beat (if needed) by adding a constant segment at the end.
         """
         if self.length() < beat:
             # no explicit segments have been made for a while, insert a constant segment to bring us up to date
             self.append_segment(self.end_level(), beat - self.length())
         return self
 
-    def truncate_at(self, beat: float) -> 'TempoEnvelope':
+    def truncate_at(self, beat: float) -> TempoEnvelope:
         """
         Removes all segments after the given beat and adds a constant segment if necessary to bring us up to that beat.
 
         :param beat: the beat that we are truncating the tempo envelope after
         :return: self, for chaining purposes
         """
         self.remove_segments_after(beat)
@@ -243,16 +244,16 @@
         return self.get_upper_integration_bound(0, t, max_error=0.00000001)
 
     ##################################################################################################################
     #                                             Conversion Utilities
     ##################################################################################################################
 
     @staticmethod
-    def convert_units(values: Union[float, Sequence[float]], input_units: str,
-                      output_units: str) -> Union[float, Sequence[float]]:
+    def convert_units(values: float | Sequence[float], input_units: str,
+                      output_units: str) -> float | Sequence[float]:
         """
         Utility method to convert values between unites of tempo, rate and beat length.
 
         :param values: value or list of values in terms of the input_units
         :param input_units: current units of the given values (either "tempo", "rate", or "beat length")
         :param output_units: desired units to convert to (either "tempo", "rate", or "beat length")
         :return: the list of values, converted to output units
@@ -370,15 +371,15 @@
     :param curve_shapes: see :class:`TempoEnvelope`
     :param units: see :class:`TempoEnvelope`
     :param duration_units: see :class:`TempoEnvelope`
     :param beat: Where to set the current beat
     """
 
     def __init__(self, levels: Sequence = (60,), durations: Sequence[float] = (),
-                 curve_shapes: Sequence[Union[float, str]] = None,
+                 curve_shapes: Sequence[float | str] = None,
                  units: str = "tempo", duration_units: str = "beats", beat: float = 0.0):
         super().__init__(levels, durations, curve_shapes, units, duration_units)
         self.go_to_beat(beat)
 
     ##################################################################################################################
     #                                                 Basic Properties
     ##################################################################################################################
@@ -434,15 +435,15 @@
         self.rate = tempo / 60
 
     ##################################################################################################################
     #                                                Tempo Changes
     ##################################################################################################################
 
     def set_beat_length_target(self, beat_length_target: float, duration: float, curve_shape: float = 0,
-                               metric_phase_target: Union[float, 'MetricPhaseTarget', Tuple] = None,
+                               metric_phase_target: float | MetricPhaseTarget | tuple = None,
                                duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Set a target beat length for this TempoEnvelope to reach in duration beats/seconds (with the unit defined by
         duration_units).
 
         :param beat_length_target: The beat length we want to reach
         :param duration: How long until we reach that beat length
@@ -464,15 +465,15 @@
             self.remove_segments_after(self.beat())
         # add a flat segment up to the current beat if needed
         self.extend_to(self.beat())
 
         self._add_segment(beat_length_target, duration, curve_shape, metric_phase_target, duration_units)
 
     def _add_segment(self, beat_length_target: float, duration: float, curve_shape: float = 0,
-                     metric_phase_target: Union[float, 'MetricPhaseTarget', Tuple] = None,
+                     metric_phase_target: float | MetricPhaseTarget | tuple = None,
                      duration_units: str = "beats") -> None:
         """
         The guts of adding a new segment, minus argument checking and truncating/bringing up to date.
         """
         if duration_units == "beats":
             extension_into_future = self.length() - self.beat()
             if duration < extension_into_future:
@@ -495,15 +496,15 @@
             self.append_segment(beat_length_target, desired_curve_length / normalized_time, curve_shape)
             if metric_phase_target is not None:
                 if not self._adjust_segment_end_beat_to_metric_phase_target(self.segments[-1], metric_phase_target):
                     logging.warning("Metric phase target {} was not reachable".format(metric_phase_target))
 
     def set_beat_length_targets(self, beat_length_targets: Sequence[float], durations: Sequence[float],
                                 curve_shapes: Sequence[float] = None,
-                                metric_phase_targets: Sequence[Union[float, 'MetricPhaseTarget', Tuple]] = None,
+                                metric_phase_targets: Sequence[float | MetricPhaseTarget | tuple] = None,
                                 duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Same as set_beat_length_target, except that you can set multiple targets at once by providing lists to each
         of the arguments.
 
         :param beat_length_targets: list of the target beat_lengths
         :param durations: list of segment durations (in beats or seconds, as defined by duration_units)
@@ -615,15 +616,15 @@
                         # segments that we just adjusted, since they would get messed up.
                         segments_to_adjust.clear()
                         # also reset the group start and end beat/time
                         current_group_start_beat = current_group_end_beat
                         current_group_start_time = current_group_end_time
 
     def set_rate_target(self, rate_target: float, duration: float, curve_shape: float = 0,
-                        metric_phase_target: Union[float, 'MetricPhaseTarget', Tuple] = None,
+                        metric_phase_target: float | MetricPhaseTarget | tuple = None,
                         duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Set a target beat rate for this TempoEnvelope to reach in duration beats/seconds (with the unit defined by
         duration_units).
 
         :param rate_target: The beat rate we want to reach
         :param duration: How long until we reach that beat rate
@@ -636,15 +637,15 @@
         :param truncate: Whether or not to truncate this TempoEnvelope to the current beat before setting this target.
         """
         self.set_beat_length_target(1 / rate_target, duration, curve_shape, metric_phase_target,
                                     duration_units, truncate)
 
     def set_rate_targets(self, rate_targets: Sequence[float], durations: Sequence[float],
                          curve_shapes: Sequence[float] = None,
-                         metric_phase_targets: Sequence[Union[float, 'MetricPhaseTarget', Tuple]] = None,
+                         metric_phase_targets: Sequence[float | MetricPhaseTarget | tuple] = None,
                          duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Same as set_rate_target, except that you can set multiple targets at once by providing lists to each
         of the arguments.
 
         :param rate_targets: list of the target beat rates
         :param durations: list of segment durations (in beats or seconds, as defined by duration_units)
@@ -654,15 +655,15 @@
             seconds/parent beats.
         :param truncate: Whether or not to truncate this TempoEnvelope to the current beat before setting these targets.
         """
         self.set_beat_length_targets([1 / x for x in rate_targets], durations, curve_shapes, metric_phase_targets,
                                      duration_units, truncate)
 
     def set_tempo_target(self, tempo_target: float, duration: float, curve_shape: float = 0,
-                         metric_phase_target: Union[float, 'MetricPhaseTarget', Tuple] = None,
+                         metric_phase_target: float | MetricPhaseTarget | tuple = None,
                          duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Set a target tempo for this TempoEnvelope to reach in duration beats/seconds (with the unit defined by
         duration_units).
 
         :param tempo_target: The tempo we want to reach
         :param duration: How long until we reach that tempo
@@ -675,15 +676,15 @@
         :param truncate: Whether or not to truncate this TempoEnvelope to the current beat before setting this target.
         """
         self.set_beat_length_target(60 / tempo_target, duration, curve_shape, metric_phase_target,
                                     duration_units, truncate)
 
     def set_tempo_targets(self, tempo_targets: Sequence[float], durations: Sequence[float],
                           curve_shapes: Sequence[float] = None,
-                          metric_phase_targets: Sequence[Union[float, 'MetricPhaseTarget', Tuple]] = None,
+                          metric_phase_targets: Sequence[float | MetricPhaseTarget | tuple] = None,
                           duration_units: str = "beats", truncate: bool = True) -> None:
         """
         Same as set_tempo_target, except that you can set multiple targets at once by providing lists to each
         of the arguments.
 
         :param tempo_targets: list of the target tempos
         :param durations: list of segment durations (in beats or seconds, as defined by duration_units)
@@ -727,15 +728,15 @@
             except ValueError:
                 pass
         return False
 
     # These methods are used when we want to adjust the metric phase at the end of a group of segments.
 
     def adjust_metric_phase_at_beat(self, beat: float,
-                                    metric_phase_target: Union[float, 'MetricPhaseTarget', Tuple]) -> bool:
+                                    metric_phase_target: float | MetricPhaseTarget | tuple) -> bool:
         """
         Sets the goal (time) metric phase at the given beat. So, for instance, if we called
         ``adjust_metric_phase_at_beat(5, 0.5)``, this would mean that we want to be at time 1.5, 2.5, 3.5 etc. at
         beat 5. If we called ``adjust_metric_phase_at_beat(7, 1.25, 3)``, this would mean that at beat 7, we would
         want to be at time 1.25, 4.25, 7.25, etc.
 
         :param beat: The beat at which to have the given phase in time
@@ -838,15 +839,15 @@
         weightings_sum = sum(weightings)
         segment_adjustments = [weighting / weightings_sum * delta_time for weighting in weightings]
         for segment, segment_time, segment_adjustment in zip(which_segments, segment_times, segment_adjustments):
             segment.set_curvature_to_desired_integral(segment_time + segment_adjustment)
         return True
 
     def adjust_metric_phase_at_time(self, target_time: float,
-                                    metric_phase_target: Union[float, 'MetricPhaseTarget', Tuple]) -> bool:
+                                    metric_phase_target: float | MetricPhaseTarget | tuple) -> bool:
         """
         Sets the goal (beat) metric phase at the given time. So, for instance, if we called
         ``adjust_metric_phase_at_time(5, 0.5)``, this would mean that at time 5 we want to be at beat 1.5, 2.5, 3.5
         etc. If we called ``adjust_metric_phase_at_time(7, 1.25, 3)``, this would mean that at time 7, we would want
         to be at beat 1.25, 4.25, 7.25, etc.
 
         :param target_time: The time at which to have the given phase in beat
@@ -930,15 +931,15 @@
         in the TempoEnvelope.
 
         :param beats: how many beats to wait
         :return: how much time that will take
         """
         return self.integrate_interval(self._beat, self._beat + beats)
 
-    def advance(self, beats: float) -> Tuple[float, float]:
+    def advance(self, beats: float) -> tuple[float, float]:
         """
         Advance the current beat/time in the envelope by the given number of beats.
 
         :param beats: how many beats to advance by
         :return: tuple of delta beats, delta time
         """
         wait_time = self.get_wait_time(beats)
@@ -964,30 +965,30 @@
         :param seconds: how many seconds to advance by
         :return: tuple of delta beats, delta time
         """
         beats = self.get_beat_wait_from_time_wait(seconds)
         self.advance(beats)
         return beats, seconds
 
-    def go_to_beat(self, b: float) -> 'TempoEnvelope':
+    def go_to_beat(self, b: float) -> TempoEnvelope:
         """
         Jump straight to the given beat in this TempoEnvelope
 
         :param b: the beat to jump to
         :return: self, for chaining purposes
         """
         self._beat = snap_float_to_nice_decimal(b)
         self._t = snap_float_to_nice_decimal(self.integrate_interval(0, b))
         return self
 
     ##################################################################################################################
     #                                                   Utilities
     ##################################################################################################################
 
-    def truncate(self) -> 'TempoEnvelope':
+    def truncate(self) -> TempoEnvelope:
         """
         Removes all segments after the current beat.
 
         :return: self, for chaining purposes
         """
         return self.truncate_at(self._beat)
 
@@ -1018,23 +1019,23 @@
 
     :param phase_or_phases: Where we are in the cycle.
     :param divisor: Length of the cycle (defaults to one beat, meaning that this specifies where we are in the beat)
     :param relative: Whether or not the start of the cycle is measured relative to the current beat/time or to the
         start of the clock.
     """
 
-    def __init__(self, phase_or_phases: Union[float, Sequence[float]], divisor: float = 1, relative: bool = False):
+    def __init__(self, phase_or_phases: float | Sequence[float], divisor: float = 1, relative: bool = False):
         self.phases = (phase_or_phases, ) if not hasattr(phase_or_phases, "__len__") else phase_or_phases
         if not all(0 <= x < divisor for x in self.phases):
             raise ValueError("One or more phases out of range for divisor.")
         self.divisor = divisor
         self.relative = relative
 
     @classmethod
-    def interpret(cls, value: Union[float, Sequence]) -> 'MetricPhaseTarget':
+    def interpret(cls, value: float | Sequence) -> MetricPhaseTarget:
         """
         Interpret a tuple or just a number as a MetricPhaseTarget. E.g. we want the user to be able to hand in a tuple
         like (0.5, 3) and have it get interpreted as a target of 0.5 with divisor 3.
 
         :param value: either a tuple (which becomes the constructor arguments), a MetricPhaseTarget (which
             is passed through unchanged), or a number which is treated as the phase with other args as defaults.
         :return: A MetricPhaseTarget, interpreted from the argument
@@ -1042,15 +1043,15 @@
         if isinstance(value, MetricPhaseTarget):
             return value
         elif hasattr(value, "__len__"):
             return MetricPhaseTarget(*value)
         else:
             return MetricPhaseTarget(value)
 
-    def _get_nearest_matches(self, t: float, offset: float = 0) -> Tuple[float, float]:
+    def _get_nearest_matches(self, t: float, offset: float = 0) -> tuple[float, float]:
         floored_value = math.floor(t / self.divisor) * self.divisor
         closest_below = None
         closest_above = None
         min_dist_below = float("inf")
         min_dist_above = float("inf")
         for base_multiple in (floored_value - self.divisor, floored_value, floored_value + self.divisor):
             for remainder in self.phases:
@@ -1061,27 +1062,27 @@
                     min_dist_below = t - this_value
                 elif this_value >= t and this_value - t < min_dist_above:
                     closest_above = this_value
                     min_dist_above = this_value - t
         # return the closest above and below in order of closeness
         return (closest_below, closest_above) if min_dist_below <= min_dist_above else (closest_above, closest_below)
 
-    def get_nearest_matching_beats(self, beat: float) -> Tuple[float, float]:
+    def get_nearest_matching_beats(self, beat: float) -> tuple[float, float]:
         """
         Get the nearest beats below and above the given beat with the correct metric phase
 
         :param beat: the beat to search around
         :return: tuple of nearest beat below, nearest beat above
         """
         if self.relative:
             return self._get_nearest_matches(beat, current_clock().beat())
         else:
             return self._get_nearest_matches(beat)
 
-    def get_nearest_matching_times(self, time: float) -> Tuple[float, float]:
+    def get_nearest_matching_times(self, time: float) -> tuple[float, float]:
         """
         Get the nearest times below and above the given time with the correct metric phase
 
         :param time: the time to search around
         :return: tuple of nearest time below, nearest time above
         """
         if self.relative:
```

## clockblocks/utilities.py

```diff
@@ -15,18 +15,20 @@
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
+from __future__ import annotations
 import threading
 import time
 from threading import Event
-from . import clock as clock_module
+from . import clock
+from . import tempo_envelope
 from typing import Sequence, Callable, Union
 
 
 def sleep_precisely_until(stop_time: float, interruption_event: Event = None) -> None:
     """
     High-precision sleep until stop_time. Sleeps repeatedly by half of the remaining time until there are fewer than
     500 microseconds left, at which point it implements a busy wait.
@@ -57,15 +59,15 @@
 
     :param secs: sleep duration
     :param interruption_event: see :func:`sleep_precisely_until`
     """
     sleep_precisely_until(time.time() + secs, interruption_event)
 
 
-def current_clock() -> Union['clock_module.Clock', None]:
+def current_clock() -> clock.Clock | None:
     """
     Get the :class:`~clockblocks.clock.Clock` active on the current thread (or None if none is active)
     """
     # utility for getting the clock we are currently using (we attach it to the thread when it's started)
     current_thread = threading.current_thread()
     if not hasattr(current_thread, '__clock__'):
         return None
@@ -110,15 +112,16 @@
     c = current_clock()
     if c is not None:
         current_clock().wait_for_children_to_finish()
 
 
 def fork(process_function: Callable, args: Sequence = (), kwargs: dict = None, name: str = None,
          initial_rate: float = None, initial_tempo: float = None, initial_beat_length: float = None,
-         schedule_at: Union[float, 'MetricPhaseTarget'] = None, done_callback: Callable = None) -> 'clock_module.Clock':
+         schedule_at: Union[float, tempo_envelope.MetricPhaseTarget] = None,
+         done_callback: Callable = None) -> clock.Clock:
 
     """
     Spawns a parallel process running on a child clock of the currently active clock.
 
     :param process_function: see :func:`~clockblocks.clock.Clock.fork`
     :param name: see :func:`~clockblocks.clock.Clock.fork`
     :param initial_rate: see :func:`~clockblocks.clock.Clock.fork`
```

## Comparing `clockblocks-0.6.7rc1.dist-info/LICENSE` & `clockblocks-0.6.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clockblocks-0.6.7rc1.dist-info/METADATA` & `clockblocks-0.6.9.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: clockblocks
-Version: 0.6.7rc1
-Summary: A python library for controlling the flow of musical time.
+Version: 0.6.9
+Summary: A python library for controlling the flow of musical time..
 Home-page: https://git.sr.ht/~marcevanstein/clockblocks
 Author: Marc Evanstein
 Author-email: marc@marcevanstein.com
-License: UNKNOWN
+License: GNU GPL Version 3
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: expenvelope (>=0.7.0)
+License-File: LICENSE
+Requires-Dist: expenvelope (>=0.7.2)
 
 # clockblocks
 
 _clockblocks_ is a python library for controlling the flow of time, designed with musical applications in mind. In particular, it is a central component of [scamp](https://sr.ht/~marcevanstein/scamp/), a Suite for Computer-Assisted Music in Python. It is described in detail [in this paper](marcevanstein.com/Writings/Clockblocks.pdf).
 
 A `Clock` acts like thread, but with the advantage that when multiple clocks are coordinated under the same master clock they remain precisely coordinated and do not experience drift. Furthermore, processing time is taken into account when "wait" is called in a given Clock. For example, the following program:
 
@@ -30,15 +32,15 @@
 while True:
     print("Current time: {}".format(round(time.time() - start, 4)))
     # do some pointless and time-consuming calculations
     for i in range(1000000):
         math.log((i+1)**0.7)
     clock.wait(2)
 ```
-
+ 
 ... generates the output:
 
 ```console
 Current time: 0.0
 Current time: 2.0001
 Current time: 4.0001
 Current time: 6.0
```

## Comparing `clockblocks-0.6.7rc1.dist-info/RECORD` & `clockblocks-0.6.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-clockblocks/__init__.py,sha256=exOea5F8TRnKct9rj5N3M_tWRh9m-eT95wnVMnRia0w,2480
-clockblocks/clock.py,sha256=dohDLrPbqmLCsSwrpFFDLqG5DHeH3l4hyHOgjPAKHWE,92195
+clockblocks/__init__.py,sha256=7jX_eBmFV6_s8fhzB7DH1B8I7KMGeQNC9Vs8zkZjo40,2629
+clockblocks/clock.py,sha256=a22jTvy9LwIArNSN4FcEBgJx7c8xyJ4bl9rHj2J64WI,92690
 clockblocks/debug.py,sha256=haYgFZj_lNT12X8ozglpQKWKt4b0JU-F85BAAF5M9k4,6179
 clockblocks/settings.py,sha256=_TPJr24-jPoN_2FDSAsBd_JCGRpv-6XvZ4ATR8n1X74,2178
-clockblocks/tempo_envelope.py,sha256=PP6xWqw9fwXJcheHz8Uy-FwruHrNPBLRHyKdayaTPgE,63811
-clockblocks/utilities.py,sha256=pqJT9gJTriHZQ9uRVF2Tc0MLYQ5bsIDbFOtY_ZQ624U,8447
-clockblocks-0.6.7rc1.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-clockblocks-0.6.7rc1.dist-info/METADATA,sha256=i9fm8qqcTojQao2YvyIO2xE8ie45c5CDG4AdGrj0Y5s,2662
-clockblocks-0.6.7rc1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-clockblocks-0.6.7rc1.dist-info/top_level.txt,sha256=X1i_RMiJpXmbgDd7-gFVhGMIyeyO34pFTr7SwBYjxfU,12
-clockblocks-0.6.7rc1.dist-info/RECORD,,
+clockblocks/tempo_envelope.py,sha256=Y7OMXWGd6jOGKcSLIv8iBKyOpmUSlaaPUCJIIUfKAAA,63707
+clockblocks/utilities.py,sha256=8BKy_fzPRmZ6L2a5aL_uQbHKhsbZREmtPZNo0lNbmoE,8493
+clockblocks-0.6.9.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+clockblocks-0.6.9.dist-info/METADATA,sha256=C4cZolC7EvZIkZ-WkN9IzlzHWuBDiyy-aXHjJnYjAY8,2720
+clockblocks-0.6.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+clockblocks-0.6.9.dist-info/top_level.txt,sha256=X1i_RMiJpXmbgDd7-gFVhGMIyeyO34pFTr7SwBYjxfU,12
+clockblocks-0.6.9.dist-info/RECORD,,
```

