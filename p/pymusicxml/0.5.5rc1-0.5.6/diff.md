# Comparing `tmp/pymusicxml-0.5.5rc1-py3-none-any.whl.zip` & `tmp/pymusicxml-0.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 47370 bytes, number of entries: 12
--rw-rw-r--  2.0 unx     3026 b- defN 22-May-04 15:12 pymusicxml/__init__.py
--rw-rw-r--  2.0 unx     3767 b- defN 21-Jul-03 04:44 pymusicxml/_utilities.py
--rw-rw-r--  2.0 unx     5991 b- defN 21-Jul-03 04:44 pymusicxml/directions.py
--rw-rw-r--  2.0 unx     2204 b- defN 21-Jul-03 04:44 pymusicxml/enums.py
--rw-rw-r--  2.0 unx    10035 b- defN 22-May-04 15:12 pymusicxml/notations.py
--rw-rw-r--  2.0 unx    98814 b- defN 22-May-04 15:12 pymusicxml/score_components.py
--rw-rw-r--  2.0 unx    20532 b- defN 22-May-04 15:12 pymusicxml/spanners.py
--rw-rw-r--  2.0 unx    35147 b- defN 22-May-05 03:42 pymusicxml-0.5.5rc1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1178 b- defN 22-May-05 03:42 pymusicxml-0.5.5rc1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-May-05 03:42 pymusicxml-0.5.5rc1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 22-May-05 03:42 pymusicxml-0.5.5rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      983 b- defN 22-May-05 03:42 pymusicxml-0.5.5rc1.dist-info/RECORD
-12 files, 181780 bytes uncompressed, 45730 bytes compressed:  74.8%
+Zip file size: 48181 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx     3190 b- defN 23-Jun-09 20:32 pymusicxml/__init__.py
+-rw-rw-r--  2.0 unx     3767 b- defN 22-Sep-24 17:32 pymusicxml/_utilities.py
+-rw-rw-r--  2.0 unx     9011 b- defN 23-May-26 18:35 pymusicxml/directions.py
+-rw-rw-r--  2.0 unx     2204 b- defN 22-Sep-24 17:32 pymusicxml/enums.py
+-rw-rw-r--  2.0 unx    10007 b- defN 23-May-26 18:35 pymusicxml/notations.py
+-rw-rw-r--  2.0 unx    98635 b- defN 23-May-26 18:35 pymusicxml/score_components.py
+-rw-rw-r--  2.0 unx    20440 b- defN 23-May-26 18:35 pymusicxml/spanners.py
+-rw-rw-r--  2.0 unx    35147 b- defN 23-Jun-09 20:35 pymusicxml-0.5.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1235 b- defN 23-Jun-09 20:35 pymusicxml-0.5.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 20:35 pymusicxml-0.5.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-09 20:35 pymusicxml-0.5.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      968 b- defN 23-Jun-09 20:35 pymusicxml-0.5.6.dist-info/RECORD
+12 files, 184707 bytes uncompressed, 46571 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pymusicxml/score_components.py
 Comment: 
 
 Filename: pymusicxml/spanners.py
 Comment: 
 
-Filename: pymusicxml-0.5.5rc1.dist-info/LICENSE
+Filename: pymusicxml-0.5.6.dist-info/LICENSE
 Comment: 
 
-Filename: pymusicxml-0.5.5rc1.dist-info/METADATA
+Filename: pymusicxml-0.5.6.dist-info/METADATA
 Comment: 
 
-Filename: pymusicxml-0.5.5rc1.dist-info/WHEEL
+Filename: pymusicxml-0.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: pymusicxml-0.5.5rc1.dist-info/top_level.txt
+Filename: pymusicxml-0.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pymusicxml-0.5.5rc1.dist-info/RECORD
+Filename: pymusicxml-0.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymusicxml/__init__.py

```diff
@@ -27,11 +27,15 @@
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
 from .score_components import Pitch, Duration, BarRestDuration, Note, Rest, BarRest, Chord, GraceNote, GraceChord, \
     BeamedGroup, Tuplet, Clef, Transpose, Measure, Part, PartGroup, Score, Notehead, Notation, Direction
 from pymusicxml.notations import StartGliss, StopGliss, StartMultiGliss, StopMultiGliss, Fermata, Arpeggiate, \
     NonArpeggiate, Technical, UpBow, DownBow, OpenString, Harmonic, Stopped, SnapPizzicato, Ornament, Mordent, Turn, \
     TrillMark, Schleifer, Tremolo
-from pymusicxml.directions import MetronomeMark, TextAnnotation, Dynamic
+from pymusicxml.directions import Harmony, Degree, MetronomeMark, TextAnnotation, Dynamic
 from pymusicxml.spanners import StopBracket, StartBracket, StopDashes, StartDashes, StopTrill, StartTrill, StopPedal, \
     ChangePedal, StartPedal, StopHairpin, StartHairpin, StopSlur, StartSlur
 from pymusicxml.enums import *
+import importlib.metadata
+
+__version__ = importlib.metadata.version('pymusicxml')
+__author__ = importlib.metadata.metadata('pymusicxml')['Author']
```

## pymusicxml/directions.py

```diff
@@ -14,15 +14,16 @@
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
-from typing import Union, Sequence
+from __future__ import annotations
+from typing import Sequence
 from xml.etree import ElementTree
 from pymusicxml.enums import StaffPlacement
 from pymusicxml.score_components import Duration, Direction
 
 
 class MetronomeMark(Direction):
 
@@ -34,15 +35,15 @@
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     :param placement: Where to place the direction in relation to the staff ("above" or "below")
     :param other_attributes: any other attributes to assign to the metronome mark, e.g. parentheses="yes" or
         font_size="5"
     """
 
-    def __init__(self, beat_length: float, bpm: float, placement: Union[str, StaffPlacement] = "above",
+    def __init__(self, beat_length: float, bpm: float, placement: str | StaffPlacement = "above",
                  voice: int = 1, staff: int = None, **other_attributes):
         super().__init__(placement, voice, staff)
         try:
             self.beat_unit = Duration.from_written_length(beat_length)
         except ValueError:
             # fall back to quarter note tempo if the beat length is not expressible as a single notehead
             self.beat_unit = Duration.from_written_length(1.0)
@@ -69,15 +70,15 @@
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     :param kwargs: any extra properties of the musicXML "words" tag aside from font-size and italics can be
         passed to kwargs
     """
 
     def __init__(self, text: str, font_size: float = None, italic: bool = False, bold: bool = False,
-                 placement: Union[str, StaffPlacement] = "above", voice: int = 1, staff: int = None, **kwargs):
+                 placement: str | StaffPlacement = "above", voice: int = 1, staff: int = None, **kwargs):
         super().__init__(placement, voice, staff)
         self.text = text
         self.text_properties = kwargs
         if font_size is not None:
             self.text_properties["font-size"] = font_size
         if italic:
             self.text_properties["font-style"] = "italic"
@@ -98,20 +99,85 @@
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     """
 
     STANDARD_TYPES = ("f", "ff", "fff", "ffff", "fffff", "ffffff", "fp", "fz", "mf", "mp", "p", "pp", "ppp", "pppp",
                       "ppppp", "pppppp", "rf", "rfz", "sf", "sffz", "sfp", "sfpp", "sfz")
 
-    def __init__(self, dynamic_text: str, placement: Union[str, StaffPlacement] = "below",
+    def __init__(self, dynamic_text: str, placement: str | StaffPlacement = "below",
                  voice: int = 1, staff: int = None):
         self.dynamic_text = dynamic_text
         super().__init__(placement, voice, staff)
 
     def render_direction_type(self) -> Sequence[ElementTree.Element]:
         type_el = ElementTree.Element("direction-type")
         dynamics_el = ElementTree.SubElement(type_el, "dynamics")
         if self.dynamic_text in Dynamic.STANDARD_TYPES:
             ElementTree.SubElement(dynamics_el, self.dynamic_text)
         else:
             ElementTree.SubElement(dynamics_el, "other-dynamics").text = self.dynamic_text
         return type_el,
+
+
+class Harmony(Direction):
+    """
+    Class representing harmonic notation.
+    """
+    KINDS = ("augmented", "augmented-seventh", "diminished",
+            "diminished-seventh", "dominant", "dominant-11th", "dominant-13th",
+            "dominant-ninth", "French", "German", "half-diminished", "Italian",
+            "major", "major-11th", "major-13th", "major-minor", "major-ninth",
+            "major-seventh", "major-sixth", "minor", "minor-11th", "minor-13th",
+            "minor-ninth", "minor-seventh", "minor-sixth", "Neapolitan", "none",
+            "other", "pedal", "power", "suspended-fourth", "suspended-second",
+            "Tristan")
+
+    def __init__(self, root_letter: str, root_alter: int, kind: str,
+                 use_symbols: bool = False, degrees: Sequence[Degree] = (),
+                 placement: str | StaffPlacement = "above"):
+        if kind not in self.KINDS:
+            raise ValueError(f"Chord {kind} of invalid kind. Allowed values: {self.KINDS}")
+        self.root_letter = root_letter
+        self.root_alter = root_alter
+        self.kind = kind
+        self.use_symbols = use_symbols
+        self.degrees = list(degrees)
+        super().__init__(placement, 1, None)
+
+    def render(self) -> Sequence[ElementTree.Element]:
+        harmony_el = ElementTree.Element("harmony")
+        root_el = ElementTree.SubElement(harmony_el, "root")
+        ElementTree.SubElement(root_el, "root-step").text = str(self.root_letter)
+        ElementTree.SubElement(root_el, "root-alter").text = str(self.root_alter)
+        ElementTree.SubElement(harmony_el, "kind").text = str(self.kind)
+        for d in self.degrees:
+            harmony_el.extend(d.render())
+        return harmony_el,
+
+    def render_direction_type(self) -> Sequence[ElementTree.Element]:
+        return self.render(),
+
+
+class Degree:
+    """
+    The <degree> element is used to add, alter, or subtract individual notes in the chord.
+
+    :param value: The number of the degree, a positive integer.
+    :param alter: An integer meaning alteration by semitones.
+    :param degree_type: Type of alteration. A positive alter + 'subtract' = semitone down.
+    :param print_object: Whether to print the degree or not.
+    """
+    DEGREE_TYPES = ("add", "alter", "subtract")
+
+    def __init__(self, value: int, alter: int, degree_type: str = "alter", print_object: bool = True):
+        assert degree_type in self.DEGREE_TYPES
+        self.value = value
+        self.alter = alter
+        self.degree_type = degree_type
+        self.print_object = print_object
+
+    def render(self) -> Sequence[ElementTree.Element]:
+        degree_element = ElementTree.Element("degree", {"print-object": "yes" if self.print_object else "no"})
+        ElementTree.SubElement(degree_element, "degree-value").text = str(self.value)
+        ElementTree.SubElement(degree_element, "degree-alter").text = str(self.alter)
+        ElementTree.SubElement(degree_element, "degree-type").text = str(self.degree_type)
+        return degree_element,
```

## pymusicxml/notations.py

```diff
@@ -14,18 +14,19 @@
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
+from __future__ import annotations
 from abc import abstractmethod, ABC
-from typing import Sequence, Union
+from typing import Sequence
 from xml.etree import ElementTree
-from pymusicxml.score_components import MusicXMLComponent, Note, Notation, MultiGliss
+from pymusicxml.score_components import Notation, MultiGliss
 from pymusicxml.enums import StaffPlacement, ArpeggiationDirection
 
 
 class StartGliss(Notation):
     """
     Notation to attach to a note that starts a glissando
 
@@ -100,15 +101,15 @@
 class Arpeggiate(Notation):
     """
     Chord arpeggiation notation.
 
     :param direction: "up" or "down"
     """
 
-    def __init__(self, direction: Union[str, ArpeggiationDirection] = None):
+    def __init__(self, direction: str | ArpeggiationDirection = None):
         self.direction = ArpeggiationDirection(direction) if isinstance(direction, str) else direction
 
     def render(self) -> Sequence[ElementTree.Element]:
         if self.direction is None:
             return ElementTree.Element("arpeggiate"),
         else:
             return ElementTree.Element("arpeggiate", {"direction": self.direction.value}),
@@ -205,15 +206,15 @@
 class Mordent(Ornament):
     """
     Mordent ornament.
 
     :param inverted: if true, an inverted mordent
     :param placement: "above" or "below"
     """
-    def __init__(self, inverted: bool = False, placement: Union[str, StaffPlacement] = "above"):
+    def __init__(self, inverted: bool = False, placement: str | StaffPlacement = "above"):
         self.placement = StaffPlacement(placement) if isinstance(placement, str) else placement
         self.inverted = inverted
 
     def render_ornament(self) -> Sequence[ElementTree.Element]:
         return ElementTree.Element("inverted-mordent" if self.inverted else "mordent",
                                    {"placement": self.placement.value}),
 
@@ -222,15 +223,15 @@
     """
     Turn ornament.
 
     :param inverted: if true, an inverted turn
     :param delayed: if true, a turn which is delayed until the end of the note
     :param placement: "above" or "below"
     """
-    def __init__(self, inverted: bool = False, delayed: bool = False, placement: Union[str, StaffPlacement] = "above"):
+    def __init__(self, inverted: bool = False, delayed: bool = False, placement: str | StaffPlacement = "above"):
         self.placement = StaffPlacement(placement) if isinstance(placement, str) else placement
         self.inverted = inverted
         self.delayed = delayed
 
     def render_ornament(self) -> Sequence[ElementTree.Element]:
 
         return ElementTree.Element("delayed-" if self.delayed else "" + "inverted-" if self.inverted else "" + "turn",
@@ -240,30 +241,29 @@
 class TrillMark(Ornament):
     """
     Trill mark on a single note (without wavy line).
 
     :param placement: "above" or "below"
     """
 
-    def __init__(self, placement: Union[str, StaffPlacement] = "above"):
+    def __init__(self, placement: str | StaffPlacement = "above"):
         self.placement = StaffPlacement(placement) if isinstance(placement, str) else placement
 
     def render_ornament(self) -> Sequence[ElementTree.Element]:
         return ElementTree.Element("trill-mark", {"placement": self.placement.value}),
 
 
-
 class Schleifer(Ornament):
     """
     Schleifer mark.
 
     :param placement: "above" or "below"
     """
 
-    def __init__(self, placement: Union[str, StaffPlacement] = "above"):
+    def __init__(self, placement: str | StaffPlacement = "above"):
         self.placement = StaffPlacement(placement) if isinstance(placement, str) else placement
 
     def render_ornament(self) -> Sequence[ElementTree.Element]:
         return ElementTree.Element("schleifer", {"placement": self.placement.value}),
 
 
 class Tremolo(Ornament):
```

## pymusicxml/score_components.py

```diff
@@ -14,18 +14,17 @@
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
-from typing import MutableSequence, Sequence, Tuple, Type, Union, Optional, Iterator, Any
-
+from __future__ import annotations
+from typing import MutableSequence, Sequence, Type, Iterator, Any
 from pymusicxml.enums import StaffPlacement
-
 from ._utilities import _least_common_multiple, _is_power_of_two, _escape_split, get_average_square_correlation
 from xml.etree import ElementTree
 from abc import ABC, abstractmethod
 from fractions import Fraction
 from numbers import Real
 import math
 import datetime
@@ -88,15 +87,15 @@
         Renders this component to a tuple of ElementTree.Element. (The reason for making it a tuple is that musical
         objects like chords are represented by several notes side by side, with all but the first containing
         a </chord> tag.)
         """
         pass
 
     @abstractmethod
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         """
         Wraps this component in a :class:`Score` so that it can be exported and viewed
         """
         pass
 
     def to_xml(self, pretty_print: bool = False) -> str:
         """
@@ -161,15 +160,15 @@
     :param allowed_types: Allowable types for objects contained within this object
     :ivar contents: Musical objects contained within this object
     :ivar allowed_types: Allowable types for objects contained within this object
     """
 
     def __init__(self, contents: Sequence[MusicXMLComponent], allowed_types: Sequence[Type]):
         contents = [] if contents is None else contents
-        self.allowed_types = tuple(allowed_types) if not isinstance(allowed_types, Tuple) else allowed_types
+        self.allowed_types = tuple(allowed_types) if not isinstance(allowed_types, tuple) else allowed_types
         if not all(isinstance(x, self.allowed_types) for x in contents):
             raise ValueError("Contents not of correct type.")
         self.contents = list(contents)
 
     def insert(self, i, o) -> None:
         """
         Insert the given object before the given index.
@@ -306,15 +305,15 @@
         octave_el = ElementTree.Element("octave")
         octave_el.text = str(self.octave)
         pitch_element.append(step_el)
         pitch_element.append(alter_el)
         pitch_element.append(octave_el)
         return pitch_element,
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Note(self, 1.0).wrap_as_score()
 
     def __eq__(self, other):
         if not isinstance(other, Pitch):
             return False
         return self.step == other.step and self.octave == other.octave and self.alteration == other.alteration
 
@@ -367,15 +366,15 @@
         "64th": 4,
         "128th": 5,
         "256th": 6,
         "512th": 7,
         "1024th": 8
     }
 
-    def __init__(self, note_type: str, num_dots: int = 0, tuplet_ratio: Tuple = None):
+    def __init__(self, note_type: str, num_dots: int = 0, tuplet_ratio: tuple = None):
         assert note_type in Duration._length_to_note_type.values()
         self.note_type = note_type
         self.num_dots = num_dots
         assert isinstance(tuplet_ratio, (type(None), tuple))
         self.tuplet_ratio = tuplet_ratio
         self._divisions = Fraction(self.true_length).limit_denominator().denominator
 
@@ -474,15 +473,15 @@
             divisor = int(duration_string)
             assert divisor in Duration._valid_divisors
         except (ValueError, AssertionError):
             raise ValueError("Bad duration string.")
         return cls.from_divisor(divisor, num_dots=num_dots)
 
     @staticmethod
-    def get_note_type_and_number_of_dots(length: float, max_dots_allowed: int = 4) -> Tuple[str, int]:
+    def get_note_type_and_number_of_dots(length: float, max_dots_allowed: int = 4) -> tuple[str, int]:
         """
         Given a length in quarter notes, get the note type and number of dots.
 
         :param length: length in quarter notes
         :param max_dots_allowed: maximum number of dots to allow
         :raise: ValueError if the given note length is impossible with max_dots_allowed dots or fewer
         :return: tuple of (note type string, number of dots)
@@ -532,15 +531,15 @@
         beat_unit_el = ElementTree.Element("beat-unit")
         beat_unit_el.text = self.note_type
         out = (beat_unit_el, )
         for _ in range(self.num_dots):
             out += (ElementTree.Element("beat-unit-dot"), )
         return out
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Note("c4", self).wrap_as_score()
 
     def __repr__(self):
         return "Duration(\"{}\", {}{})".format(
             self.note_type, self.num_dots, ", {}".format(self.tuplet_ratio) if self.tuplet_ratio is not None else ""
         )
 
@@ -581,15 +580,15 @@
         return self.length
 
     def render(self) -> Sequence[ElementTree.Element]:
         duration_el = ElementTree.Element("duration")
         duration_el.text = str(int(round(self.length * self.divisions)))
         return duration_el,
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return BarRest(self).wrap_as_score()
 
 
 # ---------------------------------------- Note class and all it variations -----------------------------------------
 
 
 class _XMLNote(DurationalObject):
@@ -782,15 +781,15 @@
                     else:
                         articulations_el.append(ElementTree.Element(articulation))
             note_element.append(notations_el)
 
         # place any text annotations before the note so that they show up at the same time as the note start
         return sum((direction.render() for direction in self.directions), ()) + (note_element,)
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         if isinstance(self, BarRest):
             duration_as_fraction = Fraction(self.true_length).limit_denominator()
             assert _is_power_of_two(duration_as_fraction.denominator)
             time_signature = (duration_as_fraction.numerator, duration_as_fraction.denominator * 4)
             return Measure([self], time_signature=time_signature).wrap_as_score()
         else:
             measure_length = 4 if self.true_length <= 4 else int(self.true_length) + 1
@@ -816,17 +815,17 @@
         represents an ordinary notehead.
     :param directions: either a single direction, or a list of directions (e.g. :class:`TextAnnotation`,
         :class:`MetronomeMark`) to populate the musicXML "directions" tag.
     :param stemless: boolean for whether to render the note with no stem.
     :param velocity: a note velocity (0-127) which gets passed along and used for playback by many applications
     """
 
-    def __init__(self, pitch: Union[Pitch, str], duration: Union[Duration, str, float], ties: str = None,
-                 notations=(), articulations=(), notehead: Union['Notehead', str] = None,
-                 directions: Sequence['Direction'] = (), stemless: bool = False, velocity: int = None):
+    def __init__(self, pitch: Pitch | str, duration: Duration | str | float, ties: str = None,
+                 notations=(), articulations=(), notehead: Notehead | str = None,
+                 directions: Sequence[Direction] = (), stemless: bool = False, velocity: int = None):
 
         if isinstance(pitch, str):
             pitch = Pitch.from_string(pitch)
         assert isinstance(pitch, Pitch)
 
         if isinstance(duration, str):
             duration = Duration.from_string(duration)
@@ -914,15 +913,15 @@
         self.filled = "yes" if filled in ("yes", True) else "no" if filled in ("no", False) else None
 
     def render(self) -> Sequence[ElementTree.Element]:
         notehead_el = ElementTree.Element("notehead", {"filled": self.filled} if self.filled is not None else {})
         notehead_el.text = self.notehead_name
         return notehead_el,
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Note("c5", 1, notehead=self).wrap_as_score()
 
     def __repr__(self):
         return "Notehead({}{})".format(self.notehead_name,
                                        ", {}".format(self.filled) if self.filled is not None else "")
 
 
@@ -933,17 +932,17 @@
 
     :param duration: either a :class:`Duration` object, a string to parse as a duration (see
         :func:`Duration.from_string`), or a number of quarter notes.
     :param notations: see :class:`Note`
     :param directions: see :class:`Note`
     """
 
-    def __init__(self, duration: Union[Duration, str, float],
-                 notations: Sequence[Union['Notation', str, ElementTree.Element]] = (),
-                 directions: Sequence['Direction'] = ()):
+    def __init__(self, duration: Duration | str | float,
+                 notations: Sequence[Notation | str | ElementTree.Element] = (),
+                 directions: Sequence[Direction] = ()):
         if isinstance(duration, str):
             duration = Duration.from_string(duration)
         elif isinstance(duration, Real):
             duration = Duration.from_written_length(duration)
 
         assert isinstance(duration, Duration)
         super().__init__(None, duration, notations=notations, directions=directions)
@@ -963,15 +962,15 @@
 
     :param bar_length: length of this bar, either as a number, :class:`Duration`, or :class:`BarRestDuration`. Bar rest
         durations are a little special, since they can be lengths (like 2.5 beats) that are otherwise note notatable
         in a single note or rest object.
     :param directions: see :class:`Note`
     """
 
-    def __init__(self, bar_length: Union[float, Duration, BarRestDuration], directions: Sequence['Direction'] = ()):
+    def __init__(self, bar_length: float | Duration | BarRestDuration, directions: Sequence[Direction] = ()):
         duration = BarRestDuration(bar_length) if isinstance(bar_length, Real) \
             else BarRestDuration(bar_length.true_length) if isinstance(bar_length, Duration) else bar_length
         super().__init__("bar rest", duration, directions=directions)
 
     def __repr__(self):
         return "BarRest({}{})".format(
             self.duration,
@@ -1001,16 +1000,16 @@
         chord being the same; the latter results in different noteheads for each chord member. Note that the default
         of None represents ordinary noteheads.
     :param directions: a direction or list of directions like that passed to a :class:`Note` object.
     :param stemless: boolean for whether to render the chord with no stem.
     :param velocity: a note velocity (0-127) which gets passed along and used for playback by many applications
     """
 
-    def __init__(self, pitches: Sequence[Union[Pitch, str]], duration: Union[Duration, str, float],
-                 ties: Union[str, Sequence[Optional[str]]] = None, notations=(), articulations=(),
+    def __init__(self, pitches: Sequence[Pitch | str], duration: Duration | str | float,
+                 ties: str | Sequence[str | None] = None, notations=(), articulations=(),
                  noteheads=None, directions=(), stemless: bool = False, velocity: int = None):
         assert isinstance(pitches, (list, tuple)) and len(pitches) > 1, "Chord should have multiple notes."
         pitches = [Pitch.from_string(pitch) if isinstance(pitch, str) else pitch for pitch in pitches]
         assert all(isinstance(pitch, Pitch) for pitch in pitches)
 
         if isinstance(duration, str):
             duration = Duration.from_string(duration)
@@ -1081,15 +1080,15 @@
         return self.notes[0].written_length
 
     @property
     def length_in_divisions(self) -> int:
         return self.notes[0].length_in_divisions
 
     @property
-    def notations(self) -> Sequence['Notation']:
+    def notations(self) -> Sequence[Notation]:
         """
         Notations attached to this chord.
         """
         return self.notes[0].notations
 
     @property
     def articulations(self) :
@@ -1172,15 +1171,15 @@
 
     def min_denominator(self) -> int:
         return self.notes[0].min_denominator()
 
     def render(self) -> Sequence[ElementTree.Element]:
         return sum((note.render() for note in self.notes), ())
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         measure_length = 4 if self.true_length <= 4 else int(self.true_length) + 1
         return Measure(pad_with_rests(self, measure_length), (measure_length, 4)).wrap_as_score()
 
     def __repr__(self):
         noteheads = None if all(n.notehead is None for n in self.notes) else tuple(n.notehead for n in self.notes)
         return "Chord({}, {}{}{}{}{})".format(
             tuple(note.pitch for note in self.notes), self.duration,
@@ -1210,17 +1209,17 @@
     :param articulations: see :class:`Note`
     :param notehead: see :class:`Note`
     :param directions: see :class:`Note`
     :param stemless: see :class:`Note`
     :param slashed: whether or not this grace note is rendered with a slash.
     :param velocity: a note velocity (0-127) which gets passed along and used for playback by many applications
     """
-    def __init__(self, pitch: Union[Pitch, str], duration: Union[Duration, str, float], ties: str = None,
-                 notations=(), articulations=(), notehead: Union['Notehead', str] = None,
-                 directions: Sequence['Direction'] = (), stemless: bool = False, slashed=False, velocity: int = None):
+    def __init__(self, pitch: Pitch | str, duration: Duration | str | float, ties: str = None,
+                 notations=(), articulations=(), notehead: Notehead | str = None,
+                 directions: Sequence[Direction] = (), stemless: bool = False, slashed=False, velocity: int = None):
         super().__init__(pitch,  duration, ties=ties, notations=notations, articulations=articulations,
                          notehead=notehead, directions=directions, stemless=stemless, velocity=velocity)
         self.is_grace = True
         self.slashed = slashed
 
     def __repr__(self):
         return "Grace" + super().__repr__()
@@ -1241,16 +1240,16 @@
     :param noteheads: see :class:`Chord`
     :param directions: see :class:`Chord`
     :param stemless: see :class:`Chord`
     :param slashed: whether or not this grace chord is rendered with a slash.
     :param velocity: a note velocity (0-127) which gets passed along and used for playback by many applications
     """
 
-    def __init__(self, pitches: Sequence[Union[Pitch, str]], duration: Union[Duration, str, float],
-                 ties: Union[str, Sequence[Optional[str]]] = None, notations=(), articulations=(),
+    def __init__(self, pitches: Sequence[Pitch | str], duration: Duration | str | float,
+                 ties: str | Sequence[str | None] = None, notations=(), articulations=(),
                  noteheads=None, directions=(), stemless: bool = False, slashed=False, velocity: int = None):
         super().__init__(pitches, duration, ties=ties, notations=notations, articulations=articulations,
                          noteheads=noteheads, directions=directions, stemless=stemless, velocity=velocity)
         for note in self.notes:
             note.is_grace = True
             note.slashed = slashed
 
@@ -1326,28 +1325,28 @@
     def min_denominator(self) -> int:
         return _least_common_multiple(*[n.min_denominator() for n in self.contents])
 
     def render(self) -> Sequence[ElementTree.Element]:
         self.render_contents_beaming()
         return sum((leaf.render() for leaf in self.contents), ())
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         measure_length = 4 if self.true_length <= 4 else int(math.ceil(self.true_length))
         return Measure(pad_with_rests(self, measure_length), (measure_length, 4)).wrap_as_score()
 
 
 class Tuplet(BeamedGroup):
     """
     Represents a tuplet; same as a BeamedGroup, but with a particular time ratio associated with it.
 
     :param contents: a list of notes, chords and rests contained in this group.
     :param ratio: a tuple representing the tuplet ratio (as described in :class:`Duration`)
     """
 
-    def __init__(self, contents: Sequence[MusicXMLComponent], ratio: Tuple):
+    def __init__(self, contents: Sequence[MusicXMLComponent], ratio: tuple):
         super().__init__(contents)
         self.ratio = ratio
         self._set_tuplet_info_for_contents(ratio)
 
     def _set_tuplet_info_for_contents(self, ratio):
         self.contents[0].tuplet_bracket = "start"
         # it would be stupid to have a tuplet that has only one note in it, but we'll cover that case anyway
@@ -1418,15 +1417,15 @@
         clef_element = ElementTree.Element("clef")
         ElementTree.SubElement(clef_element, "sign").text = self.sign
         ElementTree.SubElement(clef_element, "line").text = self.line
         if self.octaves_transposition != 0:
             ElementTree.SubElement(clef_element, "clef-octave-change").text = str(self.octaves_transposition)
         return clef_element,
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Measure([BarRest(4)], time_signature=(4, 4), clef=self).wrap_as_score()
 
 
 class Transpose(MusicXMLComponent):
     """
     Class representing transposition. Used for instruments like guitar or bass
     which transpose by an octave down.
@@ -1435,29 +1434,29 @@
     get a correct sounding pitch. It is used for encoding parts for transposing
     instruments that are in written vs. concert pitch.
 
     :param chromatic: Chromatic transposition
     :param diatonic: Diatonic transposition (optional)
     :param octave: Octave change (optional)
     """
-    def __init__(self, chromatic: int, diatonic: int, octave: int = 0):
+    def __init__(self, chromatic: int, diatonic: int = None, octave: int = None):
         self.chromatic = chromatic
         self.diatonic = diatonic
         self.octave = octave
 
     def render(self) -> Sequence[ElementTree.Element]:
         transpose_element = ElementTree.Element("transpose")
-        ElementTree.SubElement(transpose_element, "chromatic").text = str(self.chromatic)
-        if self.diatonic != 0:
+        if self.diatonic is not None:
             ElementTree.SubElement(transpose_element, "diatonic").text = str(self.diatonic)
-        if self.octave != 0:
+        ElementTree.SubElement(transpose_element, "chromatic").text = str(self.chromatic)
+        if self.octave is not None:
             ElementTree.SubElement(transpose_element, "octave-change").text = str(self.octave)
         return transpose_element,
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Measure([BarRest(4)], time_signature=(4, 4), transpose=self).wrap_as_score()
 
 
 class KeySignature(MusicXMLComponent):
 
     """
     Abstract base class for traditional and non-traditional key signatures.
@@ -1509,15 +1508,15 @@
         "aeolian": -3,
         "minor": -3,
         "locrian": -4,
         None: 0
     }
 
     @staticmethod
-    def parse(interpretable_as_key_signature: Union['KeySignature', int, str]) -> 'KeySignature':
+    def parse(interpretable_as_key_signature: KeySignature | int | str) -> KeySignature:
         """
         Parses several kinds of input into a TraditionalKeySignature or NonTraditionalKeySignature object.
 
         :param interpretable_as_key_signature: either a KeySignature object, an integer representing the number of
             sharps (or flats if negative), or a string to be parsed into a key signature, such as "G major",
             "F# lydian", or "C#, Ab" (which produces a non-traditional key-signature), etc.
         """
@@ -1548,15 +1547,15 @@
         else:
             raise ValueError("Key signature not understood.")
 
     @abstractmethod
     def render(self) -> Sequence[ElementTree.Element]:
         pass
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Measure([BarRest(4)], time_signature=(4, 4), clef="treble", key=self).wrap_as_score()
 
 
 class TraditionalKeySignature(KeySignature):
 
     """
     A traditional key signature. See https://www.w3.org/2021/06/musicxml40/musicxml-reference/elements/key/.
@@ -1639,20 +1638,20 @@
         "heavy-light": "heavy-light",
         "heavy-heavy": "heavy-heavy",
         "tick": "tick",
         "short": "short",
         "none": "none"
     }
 
-    def __init__(self, contents: Union[Sequence[DurationalObject], Sequence[Sequence[DurationalObject]]] = None,
-                 time_signature: Tuple = None, key: Union[KeySignature, str, int] = None,
-                 clef: Union[Clef, str, Tuple] = None, barline: str = None,
+    def __init__(self, contents: Sequence[DurationalObject] | Sequence[Sequence[DurationalObject]] = None,
+                 time_signature: tuple = None, key: KeySignature | str | int = None,
+                 clef: Clef | str | tuple = None, barline: str = None,
                  staves: str = None, number: int = 1,
-                 directions_with_displacements: Sequence[Tuple['Direction', float]] = (),
-                 transpose: Optional[Transpose] = None):
+                 directions_with_displacements: Sequence[tuple[Direction, float]] = (),
+                 transpose: Transpose | None = None):
         super().__init__(contents=contents, allowed_types=(Note, Rest, Chord, BarRest, BeamedGroup,
                                                            Tuplet, type(None), Sequence))
         assert hasattr(self.contents, '__len__') and all(
             isinstance(x, (Note, Rest, Chord, BarRest, BeamedGroup, Tuplet, type(None))) or
             hasattr(x, '__len__') and all(isinstance(y, (Note, Rest, Chord, BarRest, BeamedGroup, Tuplet)) for y in x)
             for x in self.contents
         )
@@ -1669,21 +1668,21 @@
         self.barline = barline
         self.staves = staves
         self.transpose = transpose
 
         self.directions_with_displacements = directions_with_displacements
 
     @property
-    def voices(self) -> Tuple[Sequence[MusicXMLComponent]]:
+    def voices(self) -> tuple[Sequence[MusicXMLComponent]]:
         """
         Returns a tuple of the voices in this Measure
         """
         return (self.contents, ) if not isinstance(self.contents[0], (tuple, list, type(None))) else self.contents
 
-    def iter_leaves(self, which_voices=None) -> Iterator[Tuple[Union[Note, Chord, Rest], float]]:
+    def iter_leaves(self, which_voices=None) -> Iterator[tuple[Note | Chord | Rest, float]]:
         """
         Iterates through the Notes/Chords/Rests in this measure, expanding out any tuplets or beam groups. The
         notes/chords/rests draw from the specified voices.
 
         :param which_voices: List of voices to return notes from (numbered 0, 1, 2, 3). The default value of None
             returns notes from all voices.
 
@@ -1707,25 +1706,25 @@
             popped_note = voice_list_copy[voice_to_pop].pop(0)
             yield popped_note, next_note_beats[voice_to_pop]
             next_note_beats[voice_to_pop] += popped_note.true_length
             if len(voice_list_copy[voice_to_pop]) == 0:
                 voice_list_copy.pop(voice_to_pop)
                 next_note_beats.pop(voice_to_pop)
 
-    def leaves(self, which_voices=None) -> Sequence[Union[Note, Chord, Rest]]:
+    def leaves(self, which_voices=None) -> Sequence[Note | Chord | Rest]:
         """
         Returns a tuple of all to the Notes/Chords/Rests in this measure, expanding out any tuplets or beam groups. The
         notes/chords/rests and draw from the specified voices, and are returned in order within the measure.
 
         :param which_voices: List of voices to return notes from (numbered 0, 1, 2, 3). The default value of None
             returns notes from all voices.
         """
         return tuple(leaf for leaf, _ in self.iter_leaves(which_voices))
 
-    def iter_directions(self) -> Iterator[Tuple['Direction', float]]:
+    def iter_directions(self) -> Iterator[tuple[Direction, float]]:
         """
         Iterates through the Directions in this measure, both those attached to notes and those passed to the
         directions_with_displacements constructor argument.
 
         :return tuples of (Direction, beat within measure)
         """
         # directions_with_displacements is a list of (Direction, beat_within_measure) tuples
@@ -1733,32 +1732,32 @@
         # self.iter_leaves() gives (Note/Chord/Rest, beat_within_measure) tuples, so we unpack the leaf's directions
         directions_with_displacements.extend((direction, beat_within_measure)
                                              for leaf, beat_within_measure in self.iter_leaves()
                                              for direction in leaf.directions)
         directions_with_displacements.sort(key=lambda x: (x[1], isinstance(x, Direction)))
         yield from directions_with_displacements
 
-    def iter_notations(self) -> Iterator[Tuple['Notation', float]]:
+    def iter_notations(self) -> Iterator[tuple[Notation, float]]:
         """
         Iterates through the Notations in this measure, in order.
 
         :return tuples of (Notation, beat_within_measure)
         """
         for leaf, beat_within_measure in self.iter_leaves():
             for notation in leaf.notations:
                 yield notation, beat_within_measure
 
-    def directions(self) -> Sequence['Direction']:
+    def directions(self) -> Sequence[Direction]:
         """
         Returns a tuple of all to the Diections in this measure, both those attached to notes and those passed to the
         directions_with_displacements constructor argument. Returned in order within the measure.
         """
         return tuple(direction for direction, _ in self.iter_directions())
 
-    def notations(self) -> Sequence['Notation']:
+    def notations(self) -> Sequence[Notation]:
         """
         Returns a tuple of all to the Notation in this measure, returned in order within the measure.
         """
         return tuple(notation for notation, _ in self.iter_notations())
 
     def _set_leaf_voices(self):
         for i, voice in enumerate(self.voices):
@@ -1858,15 +1857,15 @@
 
         if self.barline is not None:
             barline_el = ElementTree.SubElement(measure_element, "barline", {"location": "right"})
             ElementTree.SubElement(barline_el, "bar-style").text = Measure._barline_xml_names[self.barline.lower()]
 
         return measure_element,
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Part("", [self]).wrap_as_score()
 
 
 # -------------------------------------------- Part, PartGroup, and Score ------------------------------------------
 
 
 class Part(MusicXMLComponent, MusicXMLContainer):
@@ -1920,44 +1919,44 @@
         self.part_id = part_id
         super().__init__(contents=measures, allowed_types=(Measure,))
         self.part_name = part_name
         self.instrument_name = instrument_name
         self.midi_program = midi_program_num
 
     @property
-    def measures(self) -> Sequence['Measure']:
+    def measures(self) -> Sequence[Measure]:
         """
         List of the measures in this Part.
         """
         return self.contents
 
-    def iter_leaves(self, which_voices=None) -> Iterator[Union[Note, Chord, Rest]]:
+    def iter_leaves(self, which_voices=None) -> Iterator[Note | Chord | Rest]:
         """
         Iterates through the Notes/Chords/Rests in this part, expanding out any measures, tuplets and beam groups. The
         notes/chords/rests are ordered in time, and draw from the specified voices.
 
         :param which_voices: List of voices to return notes from (numbered 0, 1, 2, 3). The default value of None
             returns notes from all voices.
         """
         for measure in self.measures:
             for leaf, _ in measure.iter_leaves(which_voices):
                 yield leaf
 
-    def iter_directions(self, direction_type=None) -> Iterator['Direction']:
+    def iter_directions(self, direction_type=None) -> Iterator[Direction]:
         """
         Iterates through all directions, or all directions of a certain type, in this Part.
 
         :param direction_type: the type of direction to filter for, if any
         """
         for measure in self.measures:
             for direction, _ in measure.iter_directions():
                 if direction_type is None or isinstance(direction, direction_type):
                     yield direction
 
-    def iter_notations(self, notation_type=None) -> Iterator['Notation']:
+    def iter_notations(self, notation_type=None) -> Iterator[Notation]:
         """
         Iterates through all notations, or all notations of a certain type, in this Part.
 
         :param notation_type: the type of notation to filter for, if any
         """
         for measure in self.measures:
             for notation, _ in measure.iter_notations():
@@ -1970,15 +1969,15 @@
         part_element = ElementTree.Element("part", {"id": "P{}".format(part_copy.part_id)})
         for i, measure in enumerate(part_copy.measures):
             measure.number = i + 1
             part_element.extend(measure.render())
         return part_element,
 
     @staticmethod
-    def _validate_spanner_numbers(part: 'Part'):
+    def _validate_spanner_numbers(part: Part):
         """
         Redoes all the spanner numbers so that they are integers from 1-6 in accordance with the MusicXML number-level
         type. We want to be able to assign any number to the spanner (since keeping track of which numbers are available
         is a pain), and then adapt the numbers on export.
 
         :param part: the part whose spanners numbers to validate
         """
@@ -2054,15 +2053,15 @@
         if best_preset_score > 1.5:
             # threshold for a close enough name match
             return best_preset_match, Part.general_midi_preset_nums[best_preset_match]
         else:
             # no good match
             return None, None
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Score([self])
 
 
 class PartGroup(MusicXMLComponent, MusicXMLContainer):
     """
     Represents a part group (a group of related parts, possible connected by a bracket)
 
@@ -2103,29 +2102,29 @@
         ElementTree.SubElement(start_element, "group-barline").text = "yes" if self.has_group_bar_line else "no"
         return start_element
 
     @staticmethod
     def _render_stop_element():
         return ElementTree.Element("part-group", {"type": "stop"})
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Score([self])
 
 
 class Score(MusicXMLComponent, MusicXMLContainer):
 
     """
     Class representing a full musical score
 
     :param contents: list of parts and part groups included in this score
     :param title: title of the score
     :param composer: name of the composer
     """
 
-    def __init__(self, contents: Sequence[Union[Part, PartGroup]] = None, title: str = None, composer: str = None):
+    def __init__(self, contents: Sequence[Part | PartGroup] = None, title: str = None, composer: str = None):
         super().__init__(contents=contents, allowed_types=(Part, PartGroup))
         self.title = title
         self.composer = composer
 
     @property
     def parts(self) -> Sequence[Part]:
         """
@@ -2154,15 +2153,15 @@
         ElementTree.SubElement(encoding_el, "software").text = "pymusicxml"
         part_list_el = ElementTree.SubElement(score_element, "part-list")
         for part_or_part_group in self.contents:
             part_list_el.extend(part_or_part_group.render_part_list_entry())
             score_element.extend(part_or_part_group.render())
         return score_element,
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return self
 
 
 class NumberedSpanner(ABC):
     """Abstract base class for part of a Direction or Notation that spans multiple time-points."""
 
     def __init__(self, label: Any = 1):
@@ -2192,25 +2191,25 @@
 
     """Abstract base class for MusicXML Notations (glissandi, slurs)."""
 
     @abstractmethod
     def render(self) -> Sequence[ElementTree.Element]:
         pass
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Note("c5", 1, notations=(self, )).wrap_as_score()
 
 
 class Direction(MusicXMLComponent, ABC):
 
     """
     Abstract base class for musical directions, such as text and metronome marks.
     """
 
-    def __init__(self, placement: Union[str, StaffPlacement] = "above", voice: int = 1, staff: int = None):
+    def __init__(self, placement: str | StaffPlacement = "above", voice: int = 1, staff: int = None):
         self.placement = StaffPlacement(placement) if isinstance(placement, str) else placement
         self.voice = voice
         self.staff = staff
 
     def render(self) -> Sequence[ElementTree.Element]:
         direction_element = ElementTree.Element("direction", {"placement": self.placement.value})
         direction_element.extend(self.render_direction_type())
@@ -2222,15 +2221,15 @@
     @abstractmethod
     def render_direction_type(self) -> Sequence[ElementTree.Element]:
         """
         Renders the <direction-type> element that constitutes the main substance of a <direction> element.
         """
         pass
 
-    def wrap_as_score(self) -> 'Score':
+    def wrap_as_score(self) -> Score:
         return Measure([BarRest(4, directions=(self, ))], time_signature=(4, 4)).wrap_as_score()
 
 
 class MultiGliss(Notation):
     """Abstract base class for start and stop multi glisses"""
 
     def __init__(self, numbers: Sequence[int] = (1,)):
```

## pymusicxml/spanners.py

```diff
@@ -15,28 +15,29 @@
 #  without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.     #
 #  See the GNU General Public License for more details.                                          #
 #                                                                                                #
 #  You should have received a copy of the GNU General Public License along with this program.    #
 #  If not, see <http://www.gnu.org/licenses/>.                                                   #
 #  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++  #
 
+from __future__ import annotations
 from numbers import Real
-from typing import Any, Sequence, Union
+from typing import Any, Sequence
 from xml.etree import ElementTree
 from .enums import LineEnd, LineType, AccidentalType, HairpinType, StaffPlacement
 from .score_components import StopNumberedSpanner, MidNumberedSpanner, StartNumberedSpanner
 from .notations import Notation
 from .directions import TextAnnotation
 from pymusicxml import Direction
 
 
 class StopBracket(Direction, StopNumberedSpanner):
 
-    def __init__(self, label: Any = 1, line_end: Union[str, LineEnd] = None, end_length: Real = None,
-                 text: Union[str, TextAnnotation] = None, placement: Union[str, StaffPlacement] = "above",
+    def __init__(self, label: Any = 1, line_end: str | LineEnd = None, end_length: Real = None,
+                 text: str | TextAnnotation = None, placement: str | StaffPlacement = "above",
                  voice: int = 1, staff: int = None):
         """
         End of a bracket spanner.
 
         :param label: this should correspond to the label of the associated :class:`StartBracket`
         :param line_end: Type of hook/arrow at the end of this bracket
         :param end_length: Length of the hock at the end of this bracket
@@ -88,17 +89,17 @@
     :param placement: Where to place the direction in relation to the staff ("above" or "below")
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     """
 
     STOP_TYPE = StopBracket
 
-    def __init__(self, label: Any = 1, line_type: Union[str, LineType] = "dashed", line_end: Union[str, LineEnd] = None,
-                 end_length: Real = None, text: Union[str, TextAnnotation] = None,
-                 placement: Union[str, StaffPlacement] = "above", voice: int = 1, staff: int = None):
+    def __init__(self, label: Any = 1, line_type: str | LineType = "dashed", line_end: str | LineEnd = None,
+                 end_length: Real = None, text: str | TextAnnotation = None,
+                 placement: str | StaffPlacement = "above", voice: int = 1, staff: int = None):
         StartNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.line_type = LineType(line_type) if isinstance(line_type, str) else line_type
         self.line_end = LineEnd(line_end) if isinstance(line_end, str) else line_end
         self.end_length = end_length
         self.text = TextAnnotation(text) if isinstance(text, str) else text
         if self.line_end is None:
@@ -136,16 +137,16 @@
     :param label: this should correspond to the label of the associated :class:`StartDashes`
     :param text: Any text to attach to the end of this dashed spanner
     :param placement: Where to place the direction in relation to the staff ("above" or "below")
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     """
 
-    def __init__(self, label: Any = 1, text: Union[str, TextAnnotation] = None,
-                 placement: Union[str, StaffPlacement] = "above", voice: int = 1, staff: int = None):
+    def __init__(self, label: Any = 1, text: str | TextAnnotation = None,
+                 placement: str | StaffPlacement = "above", voice: int = 1, staff: int = None):
 
         StopNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.text = TextAnnotation(text) if isinstance(text, str) else text
 
     def render_direction_type(self) -> Sequence[ElementTree.Element]:
         direction_type_el = ElementTree.Element("direction-type")
@@ -173,15 +174,15 @@
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     """
 
     STOP_TYPE = StopDashes
 
     def __init__(self, label: Any = 1, dash_length: Real = None, space_length: Real = None,
-                 text: Union[str, TextAnnotation] = None, placement: Union[str, StaffPlacement] = "above",
+                 text: str | TextAnnotation = None, placement: str | StaffPlacement = "above",
                  voice: int = 1, staff: int = None):
         StartNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.text = TextAnnotation(text) if isinstance(text, str) else text
         self.dash_length = dash_length
         self.space_length = space_length
 
@@ -206,15 +207,15 @@
     """
     Stops a trill spanner with a wavy line.
 
     :param label: this should correspond to the label of the associated :class:`StartTrill`
     :param placement: Where to place the direction in relation to the staff ("above" or "below")
     """
 
-    def __init__(self, label: Any = 1, placement: Union[StaffPlacement, str] = "above"):
+    def __init__(self, label: Any = 1, placement: StaffPlacement | str = "above"):
         self.placement = StaffPlacement(placement) if isinstance(placement, str) else placement
         super().__init__(label)
 
     def render(self) -> Sequence[ElementTree.Element]:
         ornaments_el = ElementTree.Element("ornaments")
         ElementTree.SubElement(ornaments_el, "wavy-line",
                                {"type": "stop", "placement": self.placement.value, "number": str(self.label)})
@@ -231,16 +232,16 @@
     :param placement: Where to place the direction in relation to the staff ("above" or "below")
     :param accidental: Accidental annotation to go on the trill ("flat-flat", "flat", "natural", "sharp",
         or "double-sharp")
     """
 
     STOP_TYPE = StopTrill
 
-    def __init__(self, label: Any = 1, placement: Union[StaffPlacement, str] = "above",
-                 accidental: Union[AccidentalType, str] = None):
+    def __init__(self, label: Any = 1, placement: StaffPlacement | str = "above",
+                 accidental: AccidentalType | str = None):
         self.placement = StaffPlacement(placement) if isinstance(placement, str) else placement
         self.accidental = AccidentalType(accidental)if isinstance(accidental, str) else accidental
         super().__init__(label)
 
     def render(self) -> Sequence[ElementTree.Element]:
         ornaments_el = ElementTree.Element("ornaments")
         ElementTree.SubElement(ornaments_el, "trill-mark")
@@ -261,15 +262,15 @@
     :param line: whether or not to use a line in the pedal marking
     :param placement: Where to place the direction in relation to the staff ("above" or "below")
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     """
 
     def __init__(self, label: Any = 1, sign: bool = False, line: bool = True,
-                 placement: Union[str, StaffPlacement] = "below", voice: int = 1, staff: int = None):
+                 placement: str | StaffPlacement = "below", voice: int = 1, staff: int = None):
         StartNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.sign = sign
         self.line = line
 
     def render_direction_type(self) -> Sequence[ElementTree.Element]:
         direction_type_el = ElementTree.Element("direction-type")
@@ -288,15 +289,15 @@
     :param line: whether or not to use a line in the pedal marking
     :param placement: Where to place the direction in relation to the staff ("above" or "below")
     :param voice: Which voice to attach to
     :param staff: Which staff to attach to if the part has multiple staves
     """
 
     def __init__(self, label: Any = 1, sign: bool = True, line: bool = True,
-                 placement: Union[str, StaffPlacement] = "below", voice: int = 1, staff: int = None):
+                 placement: str | StaffPlacement = "below", voice: int = 1, staff: int = None):
         StartNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.sign = sign
         self.line = line
 
     def render_direction_type(self) -> Sequence[ElementTree.Element]:
         direction_type_el = ElementTree.Element("direction-type")
@@ -320,15 +321,15 @@
     :param staff: Which staff to attach to if the part has multiple staves
     """
 
     STOP_TYPE = StopPedal
     MID_TYPES = (ChangePedal, )
 
     def __init__(self, label: Any = 1, sign: bool = True, line: bool = True,
-                 placement: Union[str, StaffPlacement] = "below", voice: int = 1, staff: int = None):
+                 placement: str | StaffPlacement = "below", voice: int = 1, staff: int = None):
         StartNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.sign = sign
         self.line = line
 
     def render_direction_type(self) -> Sequence[ElementTree.Element]:
         direction_type_el = ElementTree.Element("direction-type")
@@ -341,15 +342,15 @@
 class StopHairpin(Direction, StopNumberedSpanner):
     """
     Notation to attach to a note that ends a hairpin
 
     :param label: this should correspond to the label of the associated :class:`StartHairpin`
     """
 
-    def __init__(self, label: Any = 1, spread: Real = None, placement: Union[str, StaffPlacement] = "below",
+    def __init__(self, label: Any = 1, spread: Real = None, placement: str | StaffPlacement = "below",
                  voice: int = 1, staff: int = None):
         StopNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.spread = spread
 
     def render_direction_type(self) -> Sequence[ElementTree.Element]:
         direction_type_el = ElementTree.Element("direction-type")
@@ -368,16 +369,16 @@
     :param label: each spanner is given an label to distinguish it from other spanners of the same type. In the MusicXML
         standard, this is a number from 1 to 6, but in pymusicxml it is allowed to be anything (including, for instance,
         a string). These labels are then converted to numbers on export.
     """
 
     STOP_TYPE = StopHairpin
 
-    def __init__(self, hairpin_type: Union[str, HairpinType], label: Any = 1, spread: Real = None,
-                 placement: Union[str, StaffPlacement] = "below", niente: bool = False, voice: int = 1,
+    def __init__(self, hairpin_type: str | HairpinType, label: Any = 1, spread: Real = None,
+                 placement: str | StaffPlacement = "below", niente: bool = False, voice: int = 1,
                  staff: int = None):
         StopNumberedSpanner.__init__(self, label)
         Direction.__init__(self, placement, voice, staff)
         self.hairpin_type = HairpinType(hairpin_type) if isinstance(hairpin_type, str) else hairpin_type
         self.spread = spread
         self.niente = niente
```

## Comparing `pymusicxml-0.5.5rc1.dist-info/LICENSE` & `pymusicxml-0.5.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymusicxml-0.5.5rc1.dist-info/METADATA` & `pymusicxml-0.5.6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pymusicxml
-Version: 0.5.5rc1
-Summary: A simple python library for exporting MusicXML
+Version: 0.5.6
+Summary: A simple python library for exporting MusicXML.
 Home-page: https://git.sr.ht/~marcevanstein/pymusicxml
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
 
 # pymusicxml
 
 _pymusicxml_ is a simple python library for exporting (and perhaps in the future, importing) MusicXML files, modelling 
 them in a hierarchical and musically logical way. Although MusicXML can simply be created using `xml.etree.ElementTree`,
 it is a confusing process: for instance, objects like tuplets and chords are created using note attributes in the 
 MusicXML standard. In _pymusicxml_, they are modelled as containers.
```

## Comparing `pymusicxml-0.5.5rc1.dist-info/RECORD` & `pymusicxml-0.5.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-pymusicxml/__init__.py,sha256=YpsAUtxeeoEDE2UXgfjEc_fP8lUD8OfHwPqF4lkrFck,3026
+pymusicxml/__init__.py,sha256=JQyHoTNivDIOaNbrWsblxPzeixJuLiRKwzfq_k9I3cs,3190
 pymusicxml/_utilities.py,sha256=WWxybqb2GOhLBtuvcdoUfcXSC75FQoQZrDX7rKfJBTk,3767
-pymusicxml/directions.py,sha256=51tWabpbmw8a2Ue-5e5hbBquSITnmZUvht2mt6sACg4,5991
+pymusicxml/directions.py,sha256=woGbN_7tRRSVDFwc1jHMSlGJzfR2U0LMiMb8HaFDlP8,9011
 pymusicxml/enums.py,sha256=l7YrgnK0PoAv9o0pgmEF3LbxALCyG8JmXWRyjumpFHQ,2204
-pymusicxml/notations.py,sha256=VvgYK0ZKca5uauV9ZHyema9LwvRx4ZgJUmCdu2J0yOM,10035
-pymusicxml/score_components.py,sha256=oPPbS7Knpu0uRHogbka_1WbOu2Yr5v41eOkCCwSIPdk,98814
-pymusicxml/spanners.py,sha256=q4WdpmwmzrWCcTVBdqcKwvbzhDvi1bcYaUMPl1DL9ds,20532
-pymusicxml-0.5.5rc1.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-pymusicxml-0.5.5rc1.dist-info/METADATA,sha256=6JyCT-PSZmGAFGWbD-fWeI7_ZT_rh4Wgn1IB4NFo3eM,1178
-pymusicxml-0.5.5rc1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pymusicxml-0.5.5rc1.dist-info/top_level.txt,sha256=Ykt-p0mZHHwVqyG4txe4wfb7hsqZFkQdCsNaQ3VCLYU,11
-pymusicxml-0.5.5rc1.dist-info/RECORD,,
+pymusicxml/notations.py,sha256=3fSoN6pqCfUzs0SghaktB6AnKP6N2bvtAoeMFktl-c8,10007
+pymusicxml/score_components.py,sha256=7328Ds3dFEmZp0rU6wPa-qhPebvfscDprvjVacktKM0,98635
+pymusicxml/spanners.py,sha256=f_dxu3xAXpvphSPRGvCuxMUYBxfJ-uJ6OF7ck0KMg1g,20440
+pymusicxml-0.5.6.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+pymusicxml-0.5.6.dist-info/METADATA,sha256=GpH3nWRo4u8x3PY7DgltA-zxjrnYUk4UhxuHuyUGHOU,1235
+pymusicxml-0.5.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pymusicxml-0.5.6.dist-info/top_level.txt,sha256=Ykt-p0mZHHwVqyG4txe4wfb7hsqZFkQdCsNaQ3VCLYU,11
+pymusicxml-0.5.6.dist-info/RECORD,,
```

