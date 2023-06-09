# Comparing `tmp/expenvelope-0.7.0rc1-py3-none-any.whl.zip` & `tmp/expenvelope-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 40473 bytes, number of entries: 10
--rw-rw-r--  2.0 unx     2056 b- defN 20-Aug-20 16:39 expenvelope/__init__.py
--rw-rw-r--  2.0 unx    17408 b- defN 22-Jan-06 06:45 expenvelope/_utilities.py
--rw-rw-r--  2.0 unx    57333 b- defN 22-Apr-21 18:39 expenvelope/envelope.py
--rw-rw-r--  2.0 unx    23261 b- defN 21-Nov-12 05:17 expenvelope/envelope_segment.py
--rw-rw-r--  2.0 unx     7158 b- defN 22-Apr-06 02:00 expenvelope/json_serializer.py
--rw-rw-r--  2.0 unx    35147 b- defN 22-May-05 03:42 expenvelope-0.7.0rc1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2001 b- defN 22-May-05 03:42 expenvelope-0.7.0rc1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-May-05 03:42 expenvelope-0.7.0rc1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 22-May-05 03:42 expenvelope-0.7.0rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      842 b- defN 22-May-05 03:42 expenvelope-0.7.0rc1.dist-info/RECORD
-10 files, 145310 bytes uncompressed, 39039 bytes compressed:  73.1%
+Zip file size: 40760 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx     2205 b- defN 23-Jun-09 20:32 expenvelope/__init__.py
+-rw-rw-r--  2.0 unx    18698 b- defN 22-Nov-18 04:36 expenvelope/_utilities.py
+-rw-rw-r--  2.0 unx    57091 b- defN 23-May-26 18:28 expenvelope/envelope.py
+-rw-rw-r--  2.0 unx    23284 b- defN 23-May-26 18:28 expenvelope/envelope_segment.py
+-rw-rw-r--  2.0 unx     7158 b- defN 23-Apr-29 18:06 expenvelope/json_serializer.py
+-rw-rw-r--  2.0 unx    35147 b- defN 23-Jun-09 20:36 expenvelope-0.7.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2057 b- defN 23-Jun-09 20:36 expenvelope-0.7.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 20:36 expenvelope-0.7.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jun-09 20:36 expenvelope-0.7.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      827 b- defN 23-Jun-09 20:36 expenvelope-0.7.2.dist-info/RECORD
+10 files, 146571 bytes uncompressed, 39356 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: expenvelope/envelope_segment.py
 Comment: 
 
 Filename: expenvelope/json_serializer.py
 Comment: 
 
-Filename: expenvelope-0.7.0rc1.dist-info/LICENSE
+Filename: expenvelope-0.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: expenvelope-0.7.0rc1.dist-info/METADATA
+Filename: expenvelope-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: expenvelope-0.7.0rc1.dist-info/WHEEL
+Filename: expenvelope-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: expenvelope-0.7.0rc1.dist-info/top_level.txt
+Filename: expenvelope-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: expenvelope-0.7.0rc1.dist-info/RECORD
+Filename: expenvelope-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## expenvelope/__init__.py

```diff
@@ -20,7 +20,11 @@
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
 from .envelope import Envelope
 from .envelope_segment import EnvelopeSegment
+import importlib.metadata
+
+__version__ = importlib.metadata.version('expenvelope')
+__author__ = importlib.metadata.metadata('expenvelope')['Author']
```

## expenvelope/_utilities.py

```diff
@@ -12,17 +12,14 @@
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
 import math
 import bisect
-from abc import ABC, abstractmethod
-from typing import TypeVar, Type
-import json
 
 
 def _make_envelope_segments_from_function(function, domain_start, domain_end, scanning_step_size=0.05,
                                           keypoint_resolution_multiple=1, slope_change_threshold=0.1,
                                           iterations=5, min_key_point_distance=1e-7, check_for_discontinuities=True):
     """
     Makes a list of EnvelopeSegments from the given function
@@ -48,27 +45,36 @@
 
     discontinuities = _get_discontinuities_and_undifferentiable_points(
         function, domain_start, domain_end, scanning_step_size,
         slope_change_threshold=slope_change_threshold, iterations=iterations
     ) if check_for_discontinuities else ()
 
     if len(discontinuities) > 0:
-        # discontinuities is always even in length, containing a point right before and right after each jump/knee
-        discontinuities = [domain_start] + discontinuities + [domain_end]
-        for i in range(0, len(discontinuities), 2):
-            section_start, section_end = discontinuities[i], discontinuities[i + 1]
+        discontinuities.sort()  # just in case
+        x = domain_start
+        for discontinuity_l, discontinuity_r in discontinuities:
+            if discontinuity_l > x:
+                segments.extend(_make_envelope_segments_from_function(
+                    function, x, discontinuity_l, scanning_step_size=scanning_step_size,
+                    keypoint_resolution_multiple=keypoint_resolution_multiple,
+                    slope_change_threshold=slope_change_threshold, iterations=iterations,
+                    min_key_point_distance=min_key_point_distance, check_for_discontinuities=False
+                ))
+            segments.append(EnvelopeSegment(discontinuity_l, discontinuity_r,
+                                            function(discontinuity_l), function(discontinuity_r), 0))
+            x = discontinuity_r
+
+        if x < domain_end:
             segments.extend(_make_envelope_segments_from_function(
-                function, section_start, section_end, scanning_step_size=scanning_step_size,
+                function, x, domain_end, scanning_step_size=scanning_step_size,
                 keypoint_resolution_multiple=keypoint_resolution_multiple,
                 slope_change_threshold=slope_change_threshold, iterations=iterations,
                 min_key_point_distance=min_key_point_distance, check_for_discontinuities=False
             ))
-            if section_end != domain_end:
-                segments.append(EnvelopeSegment(section_end, discontinuities[i + 2], function(section_end),
-                                                function(discontinuities[i + 2]), 0))
+
         return segments
     else:
         key_points = _get_extrema_and_inflection_points(function, domain_start, domain_end,
                                                         scanning_step_size=scanning_step_size, iterations=iterations)
         if keypoint_resolution_multiple > 1:
             key_points = [left + k * (right - left) / keypoint_resolution_multiple
                           for left, right in zip(key_points[:-1], key_points[1:])
@@ -110,51 +116,64 @@
 
         return segments
 
 
 def _get_discontinuities_and_undifferentiable_points(function, domain_start, domain_end, scanning_step_size,
                                                      iterations, slope_change_threshold):
     """
-    Finds jump discontinuities and points where the function is not differentiable, and returns a list of points right
-    before and right after each of these discontinuities.
+    Finds jump discontinuities and points where the function is not differentiable, and returns a list of points to
+    before and right after each of these discontinuities. These take the form of tuples of (location, "l"/"r") where
+    "l" or "r" specifies whether it's to the left or right of the discontinuity.
 
     :param function: a function of one variable
     :param domain_start: where to start in the domain
     :param domain_end: where to end in the domain
     :param scanning_step_size: the step size to use when scanning the function
-    :param iterations: How many iterations of zooming in and bumping the slope_change_threshold to do.
+    :param iterations: How many iterations of zooming in to do. (Decreases by one with each recursive call)
     :param slope_change_threshold: a discontinuity or undifferentiable point is found by looking for a sudden change in
         slope between small scanning steps. If the slope changes by more than this value between successive steps,
         we repeatedly zoom in to that step, cut the scanning_step_size by a factor of 10, and see if this jump remains.
         If it's differentiable, it should become linear and the change of slope should fall below the threshold with
         enough iterations. If it's non-differentiable, the change of slope should remain the same. If it's not even
         continuous, the change of slope should approach infinity, which will definitely be over the threshold.
     """
-    x = domain_start
+    # discontinuity_lower_bound keeps track of the farthest back point that a discontinuity could have occured that
+    # we haven't accounted for yet
+    x = discontinuity_lower_bound = domain_start
     last_f_x = function(domain_start)
     last_slope = None
     discontinuities = []
     while x < domain_end:
         x += scanning_step_size
         f_x = function(x)
         slope = (f_x - last_f_x) / scanning_step_size
         if last_slope is not None and abs(slope - last_slope) > slope_change_threshold:
             # a slope that is suddenly greater or less than the previous slope
+            # if we're only two scanning steps in, then it could have happened at any point since the domain start,
+            # since this was the first opportunity for a sudden slope change. After that point, it has to have happened
+            # in the last scanning step.
+            discontinuity_bounds = (discontinuity_lower_bound, x)
             if iterations <= 0:
-                discontinuities.extend([x - scanning_step_size, x])
+                # no more iterations of zooming in are left, and the slope is still changing suddenly. This means that
+                # this represent an undifferentiable or discontinuous point.
+                discontinuities.append(discontinuity_bounds)
             else:
-                new_bounds = max(domain_start, x - scanning_step_size * 1.1), \
-                             min(domain_end, x + scanning_step_size * 0.1)
+                # Otherwise, we zoom in by a factor of 10
                 discontinuities.extend(_get_discontinuities_and_undifferentiable_points(
-                    function, *new_bounds, scanning_step_size/10, iterations - 1, slope_change_threshold
+                    function, *discontinuity_bounds, scanning_step_size/10, iterations - 1, slope_change_threshold
                 ))
             # if we find a discontinuity, we need to reset last_slope to 0, otherwise it will register both
             # going into the discontinuity and leaving it
             last_slope = None
+            discontinuity_lower_bound = x
         else:
+            if last_slope is not None:
+                # only reset the discontinuity_lower_bound if we've had a chance to compare two slopes
+                # on the very first iteration, we don't have a last slope to compare to
+                discontinuity_lower_bound = x
             last_slope = slope
         last_f_x = f_x
     discontinuities.sort()
     return discontinuities
 
 
 def _get_extrema_and_inflection_points(function, domain_start, domain_end, scanning_step_size=0.01, iterations=5,
```

## expenvelope/envelope.py

```diff
@@ -19,21 +19,22 @@
 #  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;     #
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
-from itertools import zip_longest
 
+from __future__ import annotations
+from itertools import zip_longest
 from ._utilities import _make_envelope_segments_from_function, _curve_shape_from_start_mid_and_end_levels
 from .json_serializer import SavesToJSON
 from .envelope_segment import EnvelopeSegment
 import numbers
-from typing import Sequence, Union, Callable, Tuple, TypeVar
+from typing import Sequence, Callable, TypeVar
 
 
 T = TypeVar('T', bound='Envelope')
 
 
 class Envelope(SavesToJSON):
 
@@ -53,15 +54,15 @@
         in for the variable "exp".
     :param offset: starts curve from somewhere other than zero
     :ivar segments: list of :class:`~expenvelope.envelope_segment.EnvelopeSegment`\ s representing the pieces of this
         envelope.
     """
 
     def __init__(self, levels: Sequence = (0,), durations: Sequence[float] = (),
-                 curve_shapes: Sequence[Union[float, str]] = None, offset: float = 0):
+                 curve_shapes: Sequence[float | str] = None, offset: float = 0):
         if not hasattr(levels, "__len__"):
             levels = (levels,)
         try:
             assert hasattr(levels, "__len__") and hasattr(durations, "__len__") \
                    and (curve_shapes is None or hasattr(curve_shapes, "__len__"))
             assert len(levels) > 0 and len(durations) == len(levels) - 1
             if len(levels) == 1:
@@ -72,15 +73,15 @@
         except AssertionError:
             raise ValueError("Bad arguments for envelope construction; there must be one fewer durations (and "
                              "curve shapes, if not None) than levels.")
         self.segments = Envelope._construct_segments_list(levels, durations, curve_shapes, offset)
 
     @staticmethod
     def _construct_segments_list(levels: Sequence = (0, 0), durations: Sequence[float] = (0,),
-                                 curve_shapes: Sequence[Union[float, str]] = None, offset: float = 0):
+                                 curve_shapes: Sequence[float | str] = None, offset: float = 0):
         segments = []
         t = offset
         for i in range(len(levels) - 1):
             segments.append(EnvelopeSegment(t, t + durations[i], levels[i], levels[i + 1], curve_shapes[i]))
             t += durations[i]
         return segments
 
@@ -96,15 +97,15 @@
         out = cls()
         assert all(isinstance(x, EnvelopeSegment) for x in segments)
         out.segments = segments
         return out
 
     @classmethod
     def from_levels_and_durations(cls, levels: Sequence, durations: Sequence[float],
-                                  curve_shapes: Sequence[Union[float, str]] = None, offset: float = 0) -> T:
+                                  curve_shapes: Sequence[float | str] = None, offset: float = 0) -> T:
         """
         Construct an Envelope from levels, durations, and optionally curve shapes.
 
         :param levels: the levels of the curve. These can be anything that acts like a number. For instance, one could
             even use numpy arrays as levels.
         :param durations: the durations of the curve segments. (Should have length one less than levels.)
         :param curve_shapes: the curve shape values (optional, should have length one less than levels). Generally these
@@ -196,29 +197,29 @@
         if len(extra) > 0:
             curve_shapes = extra[0][:-1] if len(extra[0]) == len(times) else extra[0]
         else:
             curve_shapes = None
         return levels, durations, curve_shapes, offset
 
     @classmethod
-    def release(cls, duration: float, start_level=1, curve_shape: Union[float, str] = None) -> T:
+    def release(cls, duration: float, start_level=1, curve_shape: float | str = None) -> T:
         """
         Construct an simple decaying envelope
         
         :param duration: total decay length
         :param start_level: level decayed from
         :param curve_shape: shape of the curve (see documentation for :func:`Envelope.from_levels_and_durations`)
         :return: an Envelope constructed accordingly
         """
         curve_shapes = (curve_shape,) if curve_shape is not None else None
         return cls.from_levels_and_durations((start_level, 0), (duration,), curve_shapes=curve_shapes)
 
     @classmethod
     def ar(cls, attack_length: float, release_length: float, peak_level=1,
-            attack_shape: Union[float, str] = None, release_shape: Union[float, str] = None) -> T:
+            attack_shape: float | str = None, release_shape: float | str = None) -> T:
         """
         Construct an attack/release envelope
 
         :param attack_length: rise time
         :param release_length: release time
         :param peak_level: level reached after attack and before release (see documentation for
             :func:`Envelope.from_levels_and_durations`)
@@ -231,15 +232,15 @@
         curve_shapes = None if attack_shape is release_shape is None else \
             (0 if attack_shape is None else attack_shape, 0 if release_shape is None else release_shape)
         return cls.from_levels_and_durations((0, peak_level, 0), (attack_length, release_length),
                                              curve_shapes=curve_shapes)
 
     @classmethod
     def asr(cls, attack_length: float, sustain_level, sustain_length: float, release_length: float,
-            attack_shape: Union[float, str] = None, release_shape: Union[float, str] = None) -> T:
+            attack_shape: float | str = None, release_shape: float | str = None) -> T:
         """
         Construct an attack/sustain/release envelope
 
         :param attack_length: rise time
         :param sustain_level: sustain level reached after attack and before release
         :param sustain_length: length of sustain portion of curve
         :param release_length: release time
@@ -253,16 +254,16 @@
             (0 if attack_shape is None else attack_shape, 0, 0 if release_shape is None else release_shape)
         return cls.from_levels_and_durations((0, sustain_level, sustain_level, 0),
                                              (attack_length, sustain_length, release_length),
                                              curve_shapes=curve_shapes)
 
     @classmethod
     def adsr(cls, attack_length: float, attack_level, decay_length: float, sustain_level, sustain_length: float,
-             release_length: float, attack_shape: Union[float, str] = None, decay_shape: Union[float, str] = None,
-             release_shape: Union[float, str] = None) -> T:
+             release_length: float, attack_shape: float | str = None, decay_shape: float | str = None,
+             release_shape: float | str = None) -> T:
         """
         Construct a standard attack/decay/sustain/release envelope
 
         :param attack_length: rise time
         :param attack_level: level reached after attack before decay
         :param decay_length: length of decay portion of the curve
         :param sustain_level: sustain level reached after decay and before release
@@ -282,35 +283,40 @@
         return cls.from_levels_and_durations((0, attack_level, sustain_level, sustain_level, 0),
                                              (attack_length, decay_length, sustain_length, release_length),
                                              curve_shapes=curve_shapes)
 
     @classmethod
     def from_function(cls, function: Callable[[float], float], domain_start: float = 0, domain_end: float = 1,
                       scanning_step_size: float = 0.05, key_point_resolution_multiple: int = 2,
-                      iterations: int = 6, min_key_point_distance: float = 1e-7) -> T:
+                      iterations: int = 6, min_key_point_distance: float = 1e-7, start_from_zero=True) -> T:
         """
         Constructs an Envelope that approximates an arbitrary function. By default, the function is split at local
         extrema and inflection points found through a pretty unsophisticated numerical process.
 
         :param function: a function from time to level (often a lambda function)
         :param domain_start: the beginning of the function domain range to capture
         :param domain_end: the end of the function domain range to capture
         :param scanning_step_size: when analyzing the function for discontinuities, maxima and minima, inflection
             points, etc., use this step size for the initial pass.
         :param key_point_resolution_multiple: factor by which we add extra key points between the extrema and
             inflection points to improve the curve fit.
         :param iterations: when a potential key point is found, we zoom in and scan again in the viscinity of the point.
             This determines how many iterations of zooming we do.
         :param min_key_point_distance: after scanning for key points, any that are closer than this distance are merged.
+        :param start_from_zero: if true, the envelope is shifted so that it starts at time zero. Otherwise, it will
+            have an offset equal to `domain_start`
         :return: an Envelope constructed accordingly
         """
-        return cls.from_segments(_make_envelope_segments_from_function(
+        function_env = cls.from_segments(_make_envelope_segments_from_function(
             function, domain_start, domain_end, scanning_step_size=scanning_step_size,
             keypoint_resolution_multiple=key_point_resolution_multiple, iterations=iterations,
             min_key_point_distance=min_key_point_distance))
+        if start_from_zero:
+            function_env.shift_horizontal(-function_env.start_time())
+        return function_env
 
     # ---------------------------- Various Properties --------------------------------
 
     def length(self) -> float:
         """
         The length of the domain on which this Envelope is defined (end time minus start time).
         """
@@ -338,33 +344,33 @@
 
     def end_level(self):
         """
         Ending value of the Envelope
         """
         return self.segments[-1].end_level
 
-    def max_level(self, t_range: Tuple[float, float] = None):
+    def max_level(self, t_range: tuple[float, float] = None):
         """
         Returns the highest value that the Envelope takes over the given range.
 
         :param t_range: tuple defining the start and end time of the interval to check. If None, return the max level
             reached over the entire Envelope.
         """
         return self._get_extremum(t_range, max)
 
-    def min_level(self, t_range: Tuple[float, float] = None):
+    def min_level(self, t_range: tuple[float, float] = None):
         """
         Returns the lowest value that the Envelope takes over the given range.
 
         :param t_range: tuple defining the start and end time of the interval to check. If None, return the max level
             reached over the entire Envelope.
         """
         return self._get_extremum(t_range, min)
 
-    def _get_extremum(self, t_range: Tuple[float, float] = None, func=max):
+    def _get_extremum(self, t_range: tuple[float, float] = None, func=max):
         if t_range is None:
             # checking over the entire range, so that's easy
             return func(segment.max_level() if func is max else segment.min_level() for segment in self.segments)
         else:
             # checking over the range (t1, t2), so look at the values at those endpoints and any anchor points between
             assert hasattr(t_range, "__len__") and len(t_range) == 2 and t_range[0] < t_range[1]
             t1, t2 = t_range
@@ -375,15 +381,15 @@
                     points_to_check.append(segment.start_level)
                 if t1 <= segment.end_time <= t2:
                     points_to_check.append(segment.end_level)
                 if segment.end_time > t2:
                     break
             return func(points_to_check)
 
-    def average_level(self, t_range: Tuple[float, float] = None):
+    def average_level(self, t_range: tuple[float, float] = None):
         """
         Returns the average value that the Envelope takes over the given range.
 
         :param t_range: tuple defining the start and end time of the interval to check. If None, return the average
             level reached over the entire Envelope.
         """
         if t_range is None:
@@ -417,15 +423,15 @@
     def times(self) -> Sequence[float]:
         """
         Tuple of all the segment start times.
         """
         return tuple(segment.start_time for segment in self.segments) + (self.end_time(),)
 
     @property
-    def curve_shapes(self) -> Sequence[Union[float, str]]:
+    def curve_shapes(self) -> Sequence[float | str]:
         """
         Tuple of all the segment curve shapes.
         """
         return tuple(segment.curve_shape for segment in self.segments)
 
     @property
     def offset(self) -> float:
@@ -635,30 +641,30 @@
             # (could do this for non-linear, but it's probably not worth the effort)
             self.segments[0].start_time = self.start_time() - duration
             self.segments[0].start_level = level
         else:
             self.segments.insert(0, EnvelopeSegment(self.start_time() - duration, self.start_time(),
                                                     level, self.start_level(), curve_shape))
 
-    def pop_segment(self) -> Union[EnvelopeSegment, None]:
+    def pop_segment(self) -> EnvelopeSegment | None:
         """
         Remove and return the last segment of this Envelope.
         If there is only one segment, reduce it to length zero and return None.
         """
         if len(self.segments) == 1:
             if self.segments[0].end_time != self.segments[0].start_time or \
                     self.segments[0].end_level != self.segments[0].start_level:
                 self.segments[0].end_time = self.segments[0].start_time
                 self.segments[0].end_level = self.segments[0].start_level
                 return
             else:
                 raise IndexError("Cannot pop from empty Envelope")
         return self.segments.pop()
 
-    def pop_segment_from_start(self) -> Union[EnvelopeSegment, None]:
+    def pop_segment_from_start(self) -> EnvelopeSegment | None:
         """
         Remove and return the first segment of this Envelope.
         If there is only one segment, reduce it to length zero and return None.
         """
         if len(self.segments) == 1:
             if self.segments[0].end_time != self.segments[0].start_time or \
                     self.segments[0].end_level != self.segments[0].start_level:
@@ -758,21 +764,27 @@
         Get the definite integral under this Envelope from t1 to t2
 
         :param t1: lower bound of integration
         :param t2: upper bound of integration
         """
         if t1 == t2:
             return 0
-        if t2 < t1:
+        elif t2 < t1:
             return -self.integrate_interval(t2, t1)
-        if t1 < self.start_time():
-            return (self.start_time() - t1) * self.segments[0].start_level + \
-                   self.integrate_interval(self.start_time(), t2)
+        elif t1 < t2 <= self.start_time():
+            return (t2 - t1) * self.start_level()
+        elif self.end_time() <= t1 < t2:
+            return (t2 - t1) * self.end_level()
+        elif t1 < self.start_time():
+            # ... but t2 > start time
+            return (self.start_time() - t1) * self.start_level() + self.integrate_interval(self.start_time(), t2)
         if t2 > self.end_time():
+            # ... but t1 < end time
             return (t2 - self.end_time()) * self.end_level() + self.integrate_interval(t1, self.end_time())
+
         # now that the edge conditions are covered, we just add up the segment integrals
         integral = 0
 
         for segment in self.segments[self._get_index_of_segment_at(t1):]:
             if t1 < segment.start_time:
                 if t2 > segment.start_time:
                     if t2 <= segment.end_time:
@@ -789,45 +801,33 @@
                     integral += segment.integrate_segment(t1, t2)
                     break
                 else:
                     # this is the first segment in our integration interval
                     integral += segment.integrate_segment(t1, segment.end_time)
         return integral
 
-    def get_upper_integration_bound(self, t1: float, desired_area: float, max_error: float = 0.001) -> float:
+    def get_upper_integration_bound(self, t1: float, desired_area: float, max_error: float = 1e-10) -> float:
         """
         Given a lower integration bound, find the upper bound that will result in the desired integral
 
         :param t1: lower bound of integration
         :param desired_area: desired value of the integral.
         :param max_error: the upper bound is found through a process of successive approximation; once we get within
             this error, the approximation is considered good enough.
         """
-        if desired_area < max_error:
-            return t1
         t1_level = self.value_at(t1)
         t2_guess = desired_area / t1_level + t1
         area = self.integrate_interval(t1, t2_guess)
-        if area <= desired_area:
-            if desired_area - area < max_error:
-                # we hit it almost perfectly and didn't go over
-                return t2_guess
-            else:
-                # we undershot, so start from where we left off.
-                # Eventually we will get close enough that we're below the max_error
-                return self.get_upper_integration_bound(t2_guess, desired_area - area, max_error=max_error)
+        if abs(desired_area - area) < max_error:
+            # we hit it almost perfectly and didn't go over
+            return t2_guess
         else:
-            # we overshot, so we need to back up to a point below the upper integration bound
-            # try going half as far, and if that fails, half again, etc.
-            trial_width = (t2_guess - t1) / 2
-            while (partial_area := self.integrate_interval(t1, t1 + trial_width)) > desired_area:
-                trial_width /= 2
-            # once we've found a step forward we can take that doesn't overshoot, try getting the
-            # upper integration bound from there, using the remaining area
-            return self.get_upper_integration_bound(t1 + trial_width, desired_area - partial_area, max_error=max_error)
+            # we undershot, so start from where we left off.
+            # Eventually we will get close enough that we're below the max_error
+            return self.get_upper_integration_bound(t2_guess, desired_area - area, max_error=max_error)
 
     # -------------------------------- Utilities --------------------------------
 
     def normalize_to_duration(self, desired_duration: float, in_place: bool = True) -> T:
         """
         Stretch or squeeze the segments of this Envelope so that it has the desired total duration.
 
@@ -864,15 +864,15 @@
                     local_extrema.append(segment.start_time)
             if last_direction * direction < 0 and segment.start_time not in local_extrema:
                 # we changed sign, since
                 local_extrema.append(segment.start_time)
             last_direction = direction
         return local_extrema
 
-    def split_at(self, t: Union[float, Sequence[float]], change_original: bool = False,
+    def split_at(self, t: float | Sequence[float], change_original: bool = False,
                      zero_out_offsets: bool = True) -> Sequence[T]:
         """
         Splits the Envelope at one or several points and returns a tuple of the pieces
 
         :param t: either the time t or a tuple/list of times t at which to split the curve
         :param change_original: if true, the original Envelope gets turned into the first of the returned tuple
         :param zero_out_offsets: if true, each new piece is shifted to start at zero
@@ -998,15 +998,15 @@
                 resolution=resolution, endpoint=(i == len(self.segments) - 1)
             )
             x_values.extend(segment_x_values)
             y_values.extend(segment_y_values)
         return x_values, y_values
 
     def show_plot(self, title: str = None, resolution: int = 25, show_segment_divisions: bool = True,
-                  x_range: Tuple[float, float] = None, y_range: Tuple[float, float] = None) -> None:
+                  x_range: tuple[float, float] = None, y_range: tuple[float, float] = None) -> None:
         """
         Shows a plot of this Envelope using matplotlib.
 
         :param title: A title to give the plot.
         :param resolution: number of points to use per envelope segment
         :param show_segment_divisions: Whether or not to place dots at the division points between envelope segments
         :param x_range: min and max value shown on the x-axis
@@ -1076,14 +1076,16 @@
         return Envelope.from_segments([segment._reciprocal() for segment in self.segments])
 
     def __eq__(self, other):
         if not isinstance(other, Envelope):
             return False
         return all(this_segment == other_segment for this_segment, other_segment in zip(self.segments, other.segments))
 
+    __hash__ = object.__hash__
+
     def __add__(self, other):
         if isinstance(other, numbers.Number):
             return Envelope.from_segments([segment + other for segment in self.segments])
         elif isinstance(other, Envelope):
             return Envelope._apply_binary_operation_to_pair(self, other, lambda a, b: a + b)
         else:
             raise ValueError("Envelope can only be added to a constant or another envelope")
@@ -1094,15 +1096,15 @@
     def __neg__(self):
         return Envelope.from_segments([-segment for segment in self.segments])
 
     def __sub__(self, other):
         return self.__add__(-other)
 
     def __rsub__(self, other):
-        return self.__radd__(-other)
+        return self.__neg__().__add__(other)
 
     def __mul__(self, other):
         if isinstance(other, numbers.Number):
             return Envelope.from_segments([segment * other for segment in self.segments])
         elif isinstance(other, Envelope):
             return Envelope._apply_binary_operation_to_pair(self, other, lambda a, b: a * b)
         else:
```

## expenvelope/envelope_segment.py

```diff
@@ -20,19 +20,20 @@
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
+from __future__ import annotations
 from ._utilities import _make_envelope_segments_from_function, _curve_shape_from_start_mid_and_end_levels, \
     _get_curvature_from_filled_amount
 import numbers
 import math
-from typing import Union, Tuple, TypeVar
+from typing import TypeVar
 
 
 T = TypeVar('T', bound='EnvelopeSegment')
 
 
 class EnvelopeSegment:
 
@@ -47,15 +48,15 @@
     :param end_level: the level of the envelope segment at the end.
     :param curve_shape: 0 is linear, > 0 changes late, < 0 changes early. Also, string expressions involving "exp"
         can be given, where "exp" stands for the shape that will produce constant proportional change per unit time.
     :ivar start_time: the start time of the segment
     :ivar end_time: the end time of the segment
     """
 
-    def __init__(self, start_time: float, end_time: float, start_level, end_level, curve_shape: Union[float, str]):
+    def __init__(self, start_time: float, end_time: float, start_level, end_level, curve_shape: float | str):
         # note that start_level, end_level, and curvature are properties, since we want
         # to recalculate the constants that we use internally if they are changed.
         self.start_time = start_time
         self.end_time = end_time
         self._start_level = start_level
         self._end_level = end_level
         if isinstance(curve_shape, str):
@@ -285,15 +286,15 @@
             raise ValueError("Desired integral out of adjustable range.")
         if self.end_level > self.start_level:
             self._curve_shape = _get_curvature_from_filled_amount((desired_integral - low) / (high - low))
         else:
             self._curve_shape = _get_curvature_from_filled_amount(1 - (desired_integral - low) / (high - low))
         self._calculate_coefficients()
 
-    def split_at(self, t: float) -> Tuple[T, T]:
+    def split_at(self, t: float) -> tuple[T, T]:
         """
         Split this segment into two EnvelopeSegment's without altering the curve shape and return them.
         This segment is altered in the process.
 
         :param t: where to split it (t is absolute time)
         :return: a tuple of this segment modified to be only the first part, and a new segment for the second part
         """
@@ -436,15 +437,15 @@
     def __radd__(self, other):
         return self.__add__(other)
 
     def __sub__(self, other):
         return self.__add__(-other)
 
     def __rsub__(self, other):
-        return self.__radd__(-other)
+        return self.__neg__().__add__(other)
 
     def __mul__(self, other):
         from .envelope import Envelope
         if isinstance(other, numbers.Number):
             out = self.clone()
             out.scale_vertical(other)
             return out
```

## Comparing `expenvelope-0.7.0rc1.dist-info/LICENSE` & `expenvelope-0.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `expenvelope-0.7.0rc1.dist-info/METADATA` & `expenvelope-0.7.2.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: expenvelope
-Version: 0.7.0rc1
+Version: 0.7.2
 Summary: Piecewise-exponential curves designed for musical expressiveness.
 Home-page: https://git.sr.ht/~marcevanstein/expenvelope
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
+License-File: LICENSE
 
 # expenvelope
 
 _expenvelope_ is a python library for managing piecewise exponential curves, original intended as a tool for algorithmic music composition. Curves are simple to make, expressive, and useful for controlling dynamics, tempo, and other higher-level parameters. 
 
 The central `Envelope` class bears some relation to SuperCollider's [_Env_](http://doc.sccode.org/Classes/Env.html) object, and is represented behind the scenes as a contiguous set of `EnvelopeSegments`. There are a number of different class methods available for constructing envelopes, including:
```

## Comparing `expenvelope-0.7.0rc1.dist-info/RECORD` & `expenvelope-0.7.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-expenvelope/__init__.py,sha256=yGqaRcCDgZ2SGqmMFtGLM4Zq6eer_hI1AtkmumcYQ0A,2056
-expenvelope/_utilities.py,sha256=AyKwrldwza8g3xeB_K3x_zAG-C_-6SlXDhJ1UiuqOu8,17408
-expenvelope/envelope.py,sha256=aa3JxwdbBc-SOWfNoBcfjo5jahuhwjmAJyxnS2px1-k,57333
-expenvelope/envelope_segment.py,sha256=KkSBZJ3dGZLF5LPyn0neef1GTQJ5y69l2Ob2M2KbhcA,23261
+expenvelope/__init__.py,sha256=WAxRlltGJhVmCFoMJRwFdQrNuJ2SnhsRs-1JKPw94sI,2205
+expenvelope/_utilities.py,sha256=hpeyXBVSSEoRCp1vOeVjGnngF0EIwh9YLIJrDA16eNo,18698
+expenvelope/envelope.py,sha256=vGQd3pBy0_jxThOf-nQk-mSAOwr09WHiKjUKHh4Uvac,57091
+expenvelope/envelope_segment.py,sha256=SkuPkdYOM9heoc7Vo_KigOSDcXQrmUJrBI5z5IUNBcA,23284
 expenvelope/json_serializer.py,sha256=LKD4LxnrEu3ckdPAvD1M7xXreRE9_hlRlFj_USwWtek,7158
-expenvelope-0.7.0rc1.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-expenvelope-0.7.0rc1.dist-info/METADATA,sha256=MwV-vn-5jVRtNkoAKoSHI2rW7WYYgtvi6ZjiwJzwDu0,2001
-expenvelope-0.7.0rc1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-expenvelope-0.7.0rc1.dist-info/top_level.txt,sha256=HYfuvoXyR_rJT9wM5F6ZGwsBQ-OfN6jljQvo7hdn0UY,12
-expenvelope-0.7.0rc1.dist-info/RECORD,,
+expenvelope-0.7.2.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+expenvelope-0.7.2.dist-info/METADATA,sha256=7t7H17P00FcRTE_GzNg1qGwuBbXBoYp55Pp0P6DFWtk,2057
+expenvelope-0.7.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+expenvelope-0.7.2.dist-info/top_level.txt,sha256=HYfuvoXyR_rJT9wM5F6ZGwsBQ-OfN6jljQvo7hdn0UY,12
+expenvelope-0.7.2.dist-info/RECORD,,
```

