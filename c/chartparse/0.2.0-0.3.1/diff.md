# Comparing `tmp/chartparse-0.2.0.tar.gz` & `tmp/chartparse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartparse-0.2.0.tar", last modified: Sat Jul  9 07:47:41 2022, max compression
+gzip compressed data, was "chartparse-0.3.1.tar", last modified: Tue Apr 11 06:34:23 2023, max compression
```

## Comparing `chartparse-0.2.0.tar` & `chartparse-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 07:47:41.602425 chartparse-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-07-09 07:47:34.000000 chartparse-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-07-09 07:47:41.602425 chartparse-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-07-09 07:47:34.000000 chartparse-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 07:47:41.602425 chartparse-0.2.0/chartparse/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16395 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/chart.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/globalevents.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)    19438 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/instrument.py
--rw-r--r--   0 runner    (1001) docker     (121)    14166 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     8118 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/tick.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/track.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-07-09 07:47:34.000000 chartparse-0.2.0/chartparse/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 07:47:41.602425 chartparse-0.2.0/chartparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-07-09 07:47:41.000000 chartparse-0.2.0/chartparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-07-09 07:47:41.000000 chartparse-0.2.0/chartparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-09 07:47:41.000000 chartparse-0.2.0/chartparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-09 07:47:41.000000 chartparse-0.2.0/chartparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-07-09 07:47:41.000000 chartparse-0.2.0/chartparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-09 07:47:41.000000 chartparse-0.2.0/chartparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-09 07:47:41.602425 chartparse-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-07-09 07:47:34.000000 chartparse-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:34:23.742505 chartparse-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-11 06:34:10.000000 chartparse-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 06:34:23.742505 chartparse-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 06:34:10.000000 chartparse-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:34:23.738505 chartparse-0.3.1/chartparse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/globalevents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31567 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 06:34:10.000000 chartparse-0.3.1/chartparse/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:34:23.738505 chartparse-0.3.1/chartparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 06:34:23.000000 chartparse-0.3.1/chartparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-11 06:34:23.000000 chartparse-0.3.1/chartparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:34:23.000000 chartparse-0.3.1/chartparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 06:34:23.000000 chartparse-0.3.1/chartparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 06:34:23.000000 chartparse-0.3.1/chartparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 06:34:23.000000 chartparse-0.3.1/chartparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 06:34:23.742505 chartparse-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 06:34:10.000000 chartparse-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:34:23.734504 chartparse-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:34:23.742505 chartparse-0.3.1/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/fruit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/globalevents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-11 06:34:10.000000 chartparse-0.3.1/tests/helpers/unsafe.py
```

### Comparing `chartparse-0.2.0/LICENSE` & `chartparse-0.3.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 Andrew Conant
+Copyright 2022 emptyset
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `chartparse-0.2.0/PKG-INFO` & `chartparse-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: chartparse
-Version: 0.2.0
+Version: 0.3.1
 Summary: A library for parsing Guitar Hero .chart files.
 Home-page: https://github.com/AWConant/chartparse/
 Author: AWConant
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ---
 # chartparse
 
@@ -26,31 +24,33 @@
 
 ```py
 from chartparse.chart import Chart
 from chartparse.instrument import Instrument, Difficulty
 
 c = Chart.from_filepath("/path/to/file.chart")
 
-# the first 7 BPM changes
+# the first 7 BPM changes (including the initial one)
 c.sync_track.bpm_events[:7]
 
-# the first 8 time signature changes
+# the first 8 time signature changes (including the initial one)
 c.sync_track.time_signature_events[:8]
 
-expert_guitar = c.instrument_tracks[Instrument.GUITAR][Difficulty.EXPERT]
+expert_guitar = c[Instrument.GUITAR][Difficulty.EXPERT]
 
 # the first 10 notes of the expert guitar chart
 expert_guitar.note_events[:10]
 
 # the first 3 star power phrases of the expert guitar chart
 expert_guitar.star_power_events[:3]
 ```
 
+See the [documentation](https://chartparse-gh.readthedocs.io/en/latest/) for more detailed
+guidance.
+
 Note: this software is tested only with .chart files that are written by
 [Moonscraper](https://github.com/FireFox2000000/Moonscraper-Chart-Editor).
 Files written by other editors or are handwritten may produce undefined
 behavior.
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
```

### Comparing `chartparse-0.2.0/README.md` & `chartparse-0.3.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -14,29 +14,32 @@
 
 ```py
 from chartparse.chart import Chart
 from chartparse.instrument import Instrument, Difficulty
 
 c = Chart.from_filepath("/path/to/file.chart")
 
-# the first 7 BPM changes
+# the first 7 BPM changes (including the initial one)
 c.sync_track.bpm_events[:7]
 
-# the first 8 time signature changes
+# the first 8 time signature changes (including the initial one)
 c.sync_track.time_signature_events[:8]
 
-expert_guitar = c.instrument_tracks[Instrument.GUITAR][Difficulty.EXPERT]
+expert_guitar = c[Instrument.GUITAR][Difficulty.EXPERT]
 
 # the first 10 notes of the expert guitar chart
 expert_guitar.note_events[:10]
 
 # the first 3 star power phrases of the expert guitar chart
 expert_guitar.star_power_events[:3]
 ```
 
+See the [documentation](https://chartparse-gh.readthedocs.io/en/latest/) for more detailed
+guidance.
+
 Note: this software is tested only with .chart files that are written by
 [Moonscraper](https://github.com/FireFox2000000/Moonscraper-Chart-Editor).
 Files written by other editors or are handwritten may produce undefined
 behavior.
 
 ## Development
```

### Comparing `chartparse-0.2.0/chartparse/chart.py` & `chartparse-0.3.1/chartparse/sync.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,370 +1,501 @@
-# TODO: Add module docstrings everywhere.
+"""For representing the data related to tempo and meter.
+
+You should not need to create any of this module's objects manually; please instead create a
+:class:`~chartparse.chart.Chart` and inspect its attributes via that object.
+
+.. _Google Python Style Guide:
+    http://google.github.io/styleguide/pyguide.html
+
+"""
 
 from __future__ import annotations
 
-import collections
-import datetime
-import itertools
+import dataclasses
+import logging
 import re
-import typing
-from collections.abc import Callable, Iterable, Iterator, Sequence
-from pathlib import Path
-from typing import Optional, TextIO
-
+import typing as typ
+from collections.abc import Sequence
+from datetime import timedelta
+
+import chartparse.tick
+import chartparse.time
+import chartparse.track
 from chartparse.event import Event
 from chartparse.exceptions import RegexNotMatchError
-from chartparse.globalevents import GlobalEventsTrack
-from chartparse.hints import T
-from chartparse.instrument import Difficulty, Instrument, InstrumentTrack, NoteEvent
-from chartparse.metadata import Metadata
-from chartparse.sync import SyncTrack
-from chartparse.util import DictPropertiesEqMixin, DictReprTruncatedSequencesMixin
-
-_max_timedelta = datetime.datetime.max - datetime.datetime.min
-
-
-class Chart(DictPropertiesEqMixin, DictReprTruncatedSequencesMixin):
-    """A Clone Hero / Moonscraper chart and its relevant gameplay data.
-
-    While it is possible to create this with its initializer, as a user, you will most likely have
-    a ``.chart`` file and not the constituent objects necessary to use ``__init__``. To initialize
-    a ``Chart`` from a file, you should instead use :meth:`~chartparse.chart.Chart.from_file`.
-    """
+from chartparse.tick import Tick, Ticks
+from chartparse.time import Timestamp
+from chartparse.util import DictPropertiesEqMixin, DictReprMixin, DictReprTruncatedSequencesMixin
 
-    metadata: Metadata
-    """The chart's metadata, such as song title or charter name."""
+if typ.TYPE_CHECKING:  # pragma: no cover
+    from collections.abc import Iterable
 
-    global_events_track: GlobalEventsTrack
-    """Contains the chart's :class:`~chartparse.globalevents.GlobalEvent` objects"""
+logger = logging.getLogger(__name__)
 
-    sync_track: SyncTrack
-    """Contains the chart's sync-related events."""
 
-    instrument_tracks: dict[Instrument, dict[Difficulty, InstrumentTrack]]
-    """Contains all of the chart's :class:`~chartparse.instrument.InstrumentTrack` objects."""
-
-    def __init__(
-        self,
-        metadata: Metadata,
-        global_events_track: GlobalEventsTrack,
-        sync_track: SyncTrack,
-        instrument_tracks: dict[Instrument, dict[Difficulty, InstrumentTrack]],
-    ) -> None:
-        """Instantiates all instance attributes and populates timestamps & note HOPO states."""
-
-        self.metadata = metadata
-        self.global_events_track = global_events_track
-        self.sync_track = sync_track
-        self.instrument_tracks = instrument_tracks
-
-        self._populate_bpm_event_timestamps()
-        self._populate_event_timestamps(self.sync_track.time_signature_events)
-        self._populate_event_timestamps(self.global_events_track.text_events)
-        self._populate_event_timestamps(self.global_events_track.section_events)
-        self._populate_event_timestamps(self.global_events_track.lyric_events)
-        for instrument, difficulties in self.instrument_tracks.items():
-            for difficulty, track in difficulties.items():
-                self._populate_event_timestamps(track.note_events)
-                self._populate_event_timestamps(track.star_power_events)
-                self._populate_note_event_hopo_states(track.note_events)
-
-    _required_sections = ("Song", "SyncTrack")
-    _instrument_track_name_to_instrument_difficulty_pair = {
-        d + i: (Instrument(i), Difficulty(d))
-        for i, d in typing.cast(
-            Iterable[tuple[str, str]],
-            itertools.product(Instrument.all_values(), Difficulty.all_values()),
-        )
-    }
+@typ.final
+@dataclasses.dataclass(frozen=True, kw_only=True)
+class SyncTrack(DictPropertiesEqMixin, DictReprTruncatedSequencesMixin):
+    """All of a :class:`~chartparse.chart.Chart` object's tempo-mapping related events."""
+
+    Self = typ.TypeVar("Self", bound="SyncTrack")
+
+    header_tag: typ.ClassVar[str] = "SyncTrack"
+    """The name of this track's data section in a ``.chart`` file."""
+
+    time_signature_events: Sequence[TimeSignatureEvent]
+
+    bpm_events: BPMEvents
+
+    anchor_events: Sequence[AnchorEvent]
+
+    def __post_init__(self) -> None:
+        """Validates all instance attributes.
+
+        Raises:
+            ValueError: If ``time_signature_events`` or ``bpm_events`` is empty, or if either of
+                their first elements has a ``tick`` value of ``0``, or if ``resolution`` is not
+                positive.
+        """
+        if not self.time_signature_events:
+            raise ValueError("time_signature_events must not be empty")
+        if self.time_signature_events[0].tick != 0:
+            raise ValueError(
+                f"first TimeSignatureEvent {self.time_signature_events[0]} must have tick 0"
+            )
 
     @classmethod
-    def from_filepath(cls, path: Path) -> Chart:
-        """Given a path, parses the contents of its file and returns a new Chart.
+    def from_chart_lines(
+        cls: type[Self],
+        resolution: Ticks,
+        lines: Iterable[str],
+    ) -> Self:
+        """Initializes instance attributes by parsing an iterable of strings.
 
         Args:
-            path: A ``Path`` object that points to a ``.chart`` file written by Moonscraper. Must
-                have a ``[Song]`` section and a ``[SyncTrack]`` section.
+            resolution: The number of ticks in a quarter note.
+            lines: An iterable of strings obtained from a Moonscraper ``.chart`` file.
 
         Returns:
-            A ``Chart`` object, initialized with data parsed from ``path``.
+            A ``SyncTrack`` parsed from ``lines``.
         """
-        with open(path, "r", encoding="utf-8-sig") as f:
-            return Chart.from_file(f)
+
+        time_signature_data, bpm_data, anchor_data = cls._parse_data_from_chart_lines(lines)
+
+        bpm_events = chartparse.track.build_events_from_data(BPMEvent, bpm_data, resolution)
+
+        time_signature_events = chartparse.track.build_events_from_data(
+            TimeSignatureEvent, time_signature_data, bpm_events
+        )
+
+        anchor_events = chartparse.track.build_events_from_data(AnchorEvent, anchor_data)
+
+        return cls(
+            time_signature_events=time_signature_events,
+            bpm_events=bpm_events,
+            anchor_events=anchor_events,
+        )
 
     @classmethod
-    def from_file(cls, fp: TextIO) -> Chart:
-        """Given a file object, parses its contents and returns a new Chart.
+    def _parse_data_from_chart_lines(
+        cls: type[Self],
+        lines: Iterable[str],
+    ) -> tuple[
+        list[TimeSignatureEvent.ParsedData],
+        list[BPMEvent.ParsedData],
+        list[AnchorEvent.ParsedData],
+    ]:
+        parsed_data = chartparse.track.parse_data_from_chart_lines(
+            (BPMEvent.ParsedData, TimeSignatureEvent.ParsedData, AnchorEvent.ParsedData), lines
+        )
+        return (
+            parsed_data[TimeSignatureEvent.ParsedData],
+            parsed_data[BPMEvent.ParsedData],
+            parsed_data[AnchorEvent.ParsedData],
+        )
+
+
+@typ.final
+@dataclasses.dataclass(kw_only=True, frozen=True)
+class TimeSignatureEvent(Event):
+    """An event representing a time signature change at a particular tick.
+
+    The first ``TimeSignatureEvent`` sets the initial time signature.
+    """
+
+    Self = typ.TypeVar("Self", bound="TimeSignatureEvent")
+
+    upper_numeral: int
+    """The number indicating how many beats constitute a bar."""
+
+    lower_numeral: int
+    """The number indicating the note value that represents one beat."""
+
+    _default_lower_numeral: typ.ClassVar[int] = 4
+    """If ``from_parsed_data``\\'s input lacks ``lower``, we assume the true lower numeral is 4."""
+
+    @classmethod
+    def from_parsed_data(
+        cls: type[Self],
+        data: TimeSignatureEvent.ParsedData,
+        prev_event: Self | None,
+        bpm_events: BPMEvents,
+    ) -> Self:
+        """Obtain an instance of this object from parsed data.
 
         Args:
-            fp: A file object that allows reading from a .chart file written by Moonscraper.  Must
-                have a ``[Song]`` section and a ``[SyncTrack]`` section.
+            data: The data necessary to create an event.
+
+            prev_event: The event of this type with the greatest ``tick`` value less than that of
+                this event. If this is ``None``, then this must be the tick-wise first event of
+                this type.
+
+            bpm_events: An object that can be used to get a timestamp at a particular tick.
 
         Returns:
-            A ``Chart`` object, initialized with data parsed from ``fp``.
+            An an instance of this object initialized from ``data``.
         """
-        lines = fp.read().splitlines()
-        sections = cls._find_sections(lines)
-        if not all(section in sections for section in cls._required_sections):
-            raise ValueError(
-                f"parsed section list {list(sections.keys())} does not contain all "
-                f"required sections {cls._required_sections}"
-            )
 
-        instrument_tracks: collections.defaultdict[
-            Instrument, dict[Difficulty, InstrumentTrack]
-        ] = collections.defaultdict(dict)
-        for section_name, iterator_getter in sections.items():
-            if section_name == Metadata.section_name:
-                metadata = Metadata.from_chart_lines(iterator_getter)
-            elif section_name == GlobalEventsTrack.section_name:
-                global_events_track = GlobalEventsTrack.from_chart_lines(iterator_getter)
-            elif section_name == SyncTrack.section_name:
-                sync_track = SyncTrack.from_chart_lines(iterator_getter)
-            elif section_name in cls._instrument_track_name_to_instrument_difficulty_pair:
-                instrument, difficulty = cls._instrument_track_name_to_instrument_difficulty_pair[
-                    section_name
-                ]
-                track = InstrumentTrack.from_chart_lines(instrument, difficulty, iterator_getter)
-                instrument_tracks[instrument][difficulty] = track
-            # TODO: [Logging] Log unhandled sections.
+        # The lower number is written by Moonscraper as the log2 of the true value.
+        lower_numeral = 2**data.lower if data.lower is not None else cls._default_lower_numeral
+        timestamp, proximal_bpm_event_index = bpm_events.timestamp_at_tick(
+            data.tick,
+            start_iteration_index=prev_event._proximal_bpm_event_index if prev_event else 0,
+        )
+        return cls(
+            tick=data.tick,
+            timestamp=timestamp,
+            upper_numeral=data.upper,
+            lower_numeral=lower_numeral,
+            _proximal_bpm_event_index=proximal_bpm_event_index,
+        )
 
-        return cls(metadata, global_events_track, sync_track, instrument_tracks)
+    def __str__(self) -> str:
+        to_join = [super().__str__()]
+        to_join.append(f": {self.upper_numeral}/{self.lower_numeral}")
+        return "".join(to_join)
+
+    @typ.final
+    @dataclasses.dataclass(kw_only=True, frozen=True, repr=False)
+    class ParsedData(Event.ParsedData, DictReprMixin):
+        """The data on a single chart line associated with a ``TimeSignatureEvent``."""
+
+        Self = typ.TypeVar("Self", bound="TimeSignatureEvent.ParsedData")
+
+        upper: int
+        """The number indicating how many beats constitute a bar."""
+
+        lower: int | None
+        """The log (base 2) of the number indicating the note value that represents one beat."""
+
+        # Match 1: Tick
+        # Match 2: Upper numeral
+        # Match 3: Lower numeral (optional)
+        _regex: typ.Final[str] = r"^\s*?(\d+?) = TS (\d+?)(?: (\d+?))?\s*?$"
+        _regex_prog: typ.Final[typ.Pattern[str]] = re.compile(_regex)
+
+        @classmethod
+        def from_chart_line(cls: type[Self], line: str) -> Self:
+            """Attempt to construct this object from a ``.chart`` line.
+
+            Returns:
+                An an instance of this object initialized from ``line``.
+
+            Raises:
+                RegexNotMatchError: If the mixed-into class' ``_regex`` does not match ``line``.
+            """
+            m = cls._regex_prog.match(line)
+            if not m:
+                raise RegexNotMatchError(cls._regex, line)
+            raw_tick, raw_upper, raw_lower = m.groups()
+            try:
+                lower = int(raw_lower)
+            except TypeError:
+                lower = None
+            return cls(tick=Tick(int(raw_tick)), upper=int(raw_upper), lower=lower)
+
+
+@typ.final
+@dataclasses.dataclass(kw_only=True, frozen=True)
+class BPMEvent(Event):
+    """An event representing a BPM (beats per minute) change at a particular tick.
 
-    _section_name_regex = r"^\[(.+?)\]$"
-    _section_name_regex_prog = re.compile(_section_name_regex)
+    The first ``BPMEvent`` sets the initial BPM.
+    """
+
+    Self = typ.TypeVar("Self", bound="BPMEvent")
+
+    bpm: float
+    """The beats per minute value. Must not have more than 3 decimal places."""
+
+    def __post_init__(self) -> None:
+        """Validate instance attributes.
+
+        Raises:
+            ValueError: If ``bpm`` has more than 3 decimal places.
+        """
+        if round(self.bpm, 3) != self.bpm:
+            raise ValueError(f"bpm {self.bpm} must not have more than 3 decimal places.")
 
     @classmethod
-    def _find_sections(cls, lines: Iterable[str]) -> dict[str, Callable[[], Iterable[str]]]:
-        sections: dict[str, Callable[[], Iterable[str]]] = dict()
-        curr_section_name = None
-        curr_first_line_idx = None
-        curr_last_line_idx = None
-        for i, line in enumerate(lines):
-            if curr_section_name is None:
-                m = cls._section_name_regex_prog.match(line)
-                if not m:
-                    raise RegexNotMatchError(cls._section_name_regex, line)
-                curr_section_name = m.group(1)
-            elif line == "{":
-                curr_first_line_idx = i + 1
-            elif line == "}":
-                curr_last_line_idx = i - 1
-                # Set default values for x and y so their current values are
-                # captured, rather than references to these local variables.
-                iterator_getter = (
-                    lambda x=curr_first_line_idx, y=curr_last_line_idx: itertools.islice(
-                        lines, x, y + 1
-                    )
+    def from_parsed_data(
+        cls: type[Self],
+        data: BPMEvent.ParsedData,
+        prev_event: Self | None,
+        resolution: Ticks,
+    ) -> Self:
+        """Obtain an instance of this object from parsed data.
+
+        Args:
+            data: The data necessary to create an event.
+
+            prev_event: The event of this type with the greatest ``tick`` value less than that of
+                this event. If this is ``None``, then this must be the tick-wise first event of
+                this type.
+
+            resolution: The number of ticks for which a quarter note lasts.
+
+        Returns:
+            An an instance of this object initialized from ``data``.
+
+        Raises:
+            ValueError: If ``prev_event.tick`` is not less than the tick value parsed from
+                ``line``.
+        """
+
+        bpm_whole_part_str, bpm_decimal_part_str = data.raw_bpm[:-3], data.raw_bpm[-3:]
+        bpm_whole_part = int(bpm_whole_part_str) if bpm_whole_part_str != "" else 0
+        bpm_decimal_part = int(bpm_decimal_part_str) / 1000
+        bpm = bpm_whole_part + bpm_decimal_part
+
+        if prev_event is None:
+            timestamp, proximal_bpm_event_index = Timestamp(timedelta(0)), 0
+        else:
+            if data.tick <= prev_event.tick:
+                raise ValueError(
+                    f"{cls.__name__} at tick {data.tick} does not occur after previous "
+                    f"{cls.__name__} at tick {prev_event.tick}; tick values of "
+                    f"{cls.__name__} must be strictly increasing."
                 )
-                sections[curr_section_name] = iterator_getter
-                curr_section_name = None
-                curr_first_line_idx = None
-                curr_last_line_idx = None
-        return sections
-
-    def _populate_bpm_event_timestamps(self) -> None:
-        self.sync_track.bpm_events[0].timestamp = datetime.timedelta(0)
-        for i, cur_event in enumerate(
-            _iterate_from_second_elem(self.sync_track.bpm_events), start=1
-        ):
-            prev_event = self.sync_track.bpm_events[i - 1]
-            assert prev_event.timestamp is not None
-            ticks_since_prev = cur_event.tick - prev_event.tick
-            seconds_since_prev = self._seconds_from_ticks_at_bpm(ticks_since_prev, prev_event.bpm)
-            cur_event.timestamp = prev_event.timestamp + datetime.timedelta(
-                seconds=seconds_since_prev
+            ticks_since_prev = chartparse.tick.between(prev_event.tick, data.tick)
+            seconds_since_prev = chartparse.tick.seconds_from_ticks_at_bpm(
+                ticks_since_prev, prev_event.bpm, resolution
             )
-
-    def _populate_event_timestamps(self, events: Iterable[Event]) -> None:
-        proximal_bpm_event_idx = 0
-        for i, event in enumerate(events):
-            timestamp, proximal_bpm_event_idx = self._timestamp_at_tick(
-                event.tick,
-                start_bpm_event_index=proximal_bpm_event_idx,
+            timestamp = chartparse.time.add(
+                prev_event.timestamp, timedelta(seconds=seconds_since_prev)
             )
-            event.timestamp = timestamp
+            proximal_bpm_event_index = prev_event._proximal_bpm_event_index + 1
 
-    def _populate_note_event_hopo_states(self, events: Sequence[NoteEvent]) -> None:
-        if not events:
-            return
-
-        for i, cur_event in enumerate(events):
-            previous_event = events[i - 1] if i > 0 else None
-            cur_event._populate_hopo_state(self.metadata.resolution, previous_event)
-
-    def _timestamp_at_tick(
-        self, tick: int, start_bpm_event_index: int = 0
-    ) -> tuple[datetime.timedelta, int]:
-        proximal_bpm_event_idx = self.sync_track.idx_of_proximal_bpm_event(
-            tick, start_idx=start_bpm_event_index
+        return cls(
+            tick=data.tick,
+            timestamp=timestamp,
+            bpm=bpm,
+            _proximal_bpm_event_index=proximal_bpm_event_index,
         )
-        proximal_bpm_event = self.sync_track.bpm_events[proximal_bpm_event_idx]
-        assert proximal_bpm_event.timestamp is not None
-        ticks_since_proximal_bpm_event = tick - proximal_bpm_event.tick
-        seconds_since_proximal_bpm_event = self._seconds_from_ticks_at_bpm(
-            ticks_since_proximal_bpm_event, proximal_bpm_event.bpm
-        )
-        timedelta_since_proximal_bpm_event = datetime.timedelta(
-            seconds=seconds_since_proximal_bpm_event
-        )
-        timestamp = proximal_bpm_event.timestamp + timedelta_since_proximal_bpm_event
-        return timestamp, proximal_bpm_event_idx
 
-    def _seconds_from_ticks_at_bpm(self, ticks: int, bpm: float) -> float:
-        if bpm <= 0:
-            raise ValueError(f"bpm {bpm} must be positive")
-        ticks_per_minute = bpm * self.metadata.resolution
-        ticks_per_second = ticks_per_minute / 60
-        seconds_per_tick = 1 / ticks_per_second
-        return ticks * seconds_per_tick
-
-    # TODO: Calculate this over the actual interval, not the interval formed by the first and last
-    # notes.
-    def notes_per_second(
-        self,
-        instrument: Instrument,
-        difficulty: Difficulty,
-        start_time: Optional[datetime.timedelta] = None,
-        end_time: Optional[datetime.timedelta] = None,
-        start_tick: Optional[int] = None,
-        end_tick: Optional[int] = None,
-        start_seconds: Optional[float] = None,
-        end_seconds: Optional[float] = None,
-    ) -> float:
-        """Returns the average notes per second from the first and last note in the interval.
-
-        More specifically, this calculates the number of :class:`~chartparse.instrument.NoteEvent`
-        objects per second. Chords do not count as multiple "notes" in one instant.
-
-        The interval is always a closed interval.
-
-        You may pass one or zero of ``start_time``, ``start_tick``, and ``start_seconds``, or else
-        ``ValueError`` will be raised.  If none of ``start_time``, ``start_tick``, and
-        ``start_seconds`` are passed, the beginning of the track will be treated as the start of
-        the interval.  If none of ``end_time``, ``end_tick``, and ``end_seconds`` are passed, the
-        end of the track will be treated as the end of the interval.
+    def __str__(self) -> str:
+        to_join = [super().__str__()]
+        to_join.append(f": {self.bpm} BPM")
+        return "".join(to_join)
+
+    @typ.final
+    @dataclasses.dataclass(kw_only=True, frozen=True, repr=False)
+    class ParsedData(Event.ParsedData, DictReprMixin):
+        """The data on a single chart line associated with a ``BPMEvent``."""
+
+        Self = typ.TypeVar("Self", bound="BPMEvent.ParsedData")
+
+        raw_bpm: str
+
+        # Match 1: Tick
+        # Match 2: BPM (the last 3 digits are the decimal places)
+        _regex: typ.Final[str] = r"^\s*?(\d+?) = B (\d+?)\s*?$"
+        _regex_prog: typ.Final[typ.Pattern[str]] = re.compile(_regex)
+
+        @classmethod
+        def from_chart_line(cls: type[Self], line: str) -> Self:
+            """Attempt to construct this object from a ``.chart`` line.
+
+            Args:
+                line: A string, obtained from a Moonscraper ``.chart`` file.
+
+            Returns:
+                An an instance of this object initialized from ``line``.
+
+            Raises:
+                RegexNotMatchError: If the mixed-into class' ``_regex`` does not match ``line``.
+            """
+            m = cls._regex_prog.match(line)
+            if not m:
+                raise RegexNotMatchError(cls._regex, line)
+            raw_tick, raw_bpm = m.groups()
+            return cls(tick=Tick(int(raw_tick)), raw_bpm=raw_bpm)
+
+
+@typ.final
+@dataclasses.dataclass(kw_only=True, frozen=True)
+class BPMEvents(Sequence[BPMEvent]):
+    """The chart's ``BPMEvent``\\s, wrapped with the chart's resolution.
+
+    This exists solely to allow ``timestamp_at_tick`` to be called the moment all requisite data is
+    accessible. If the resolution and BPM events were instead bundled into ``SyncTrack`` and
+    ``timestamp_at_tick`` were attached to ``SyncTrack``, is would be irksome to call
+    ``timestamp_at_tick`` while initializing ``TimeSignatureEvents``.
+    """
 
-        Args:
-            instrument: The instrument for which the
-                :class:`~chartparse.instrument.InstrumentTrack` should be looked up.
-            difficulty: The instrument for which the
-                :class:`~chartparse.instrument.InstrumentTrack` should be looked up.
-            start_time: The beginning of the interval.
-            end_time: The end of the interval.
-            start_tick: The beginning of the interval.
-            end_tick: The end of the interval.
-            start_seconds: The beginning of the interval.
-            end_seconds: The end of the interval.
+    events: Sequence[BPMEvent]
+    """The chart's ``BPMEvent``\\s."""
 
-        Returns:
-            The average notes per second value over the interval formed by the first and last note.
+    resolution: Ticks
+    """The number of ticks in a quarter note."""
+
+    def __post_init__(self) -> None:
+        """Validates all instance attributes.
 
         Raises:
-            ValueError: If more than one of ``start_time``, ``start_tick``, and ``start_seconds``
-                is ``None``.
-            ValueError: If there is no :class:`~chartparse.instrument.InstrumentTrack`
-                corresponding to ``instrument`` and ``difficulty``.
-            ValueError: If there are fewer than two :class:`~chartparse.instrument.NoteEvent`
-                objects within the indicated interval.
+            ValueError: If ``bpm_events`` is empty, or if its first element has a ``tick`` value of
+                ``0``, or if ``resolution`` is not positive.
         """
+        if self.resolution <= 0:
+            raise ValueError(f"resolution ({self.resolution}) must be positive")
+        if not self.events:
+            raise ValueError("events must not be empty")
+        if self.events[0].tick != 0:
+            raise ValueError(f"first BPMEvent {self.events[0]} must have tick 0")
+
+    def __len__(self) -> int:
+        return len(self.events)
+
+    @typ.overload
+    def __getitem__(self, index: int) -> BPMEvent:
+        ...  # pragma: no cover
+
+    @typ.overload
+    def __getitem__(self, index: slice) -> Sequence[BPMEvent]:
+        ...  # pragma: no cover
+
+    def __getitem__(self, index: int | slice) -> BPMEvent | Sequence[BPMEvent]:
+        return self.events[index]
+
+    # TODO(P2): Figure out why kwargs docstring is ugly in Sphinx.
+    def timestamp_at_tick_no_optimize_return(self, tick: Tick) -> Timestamp:
+        """Returns the timestamp at the input tick.
 
-        start_args = (start_time, start_seconds, start_tick)
-        num_of_start_args_none = start_args.count(None)
-        if num_of_start_args_none < 2:
-            raise ValueError(
-                f"no more than one of start_time {start_time}, start_seconds {start_seconds}, "
-                f"and start_tick {start_tick} can be non-None"
-            )
-        all_start_args_none = num_of_start_args_none == len(start_args)
+        Args:
+            tick: The tick at which the timestamp should be calculated.
 
-        def event_is_eligible_by_tick(note: NoteEvent) -> bool:
-            lower_bound: int = start_tick if start_tick is not None else 0
-            upper_bound: float = end_tick if end_tick is not None else float("inf")
-            return lower_bound <= note.tick <= upper_bound
-
-        def event_is_eligible_by_time(note: NoteEvent) -> bool:
-            assert note.timestamp is not None
-            lower_bound: datetime.timedelta = (
-                start_time if start_time is not None else datetime.timedelta(0)
-            )
-            upper_bound: datetime.timedelta = end_time if end_time is not None else _max_timedelta
-            return lower_bound <= note.timestamp <= upper_bound
+        Returns:
+            The timestamp at the input tick.
+        """
+        timestamp, _ = self.timestamp_at_tick(tick)
+        return timestamp
 
-        def event_is_eligible_by_seconds(note: NoteEvent) -> bool:
-            assert note.timestamp is not None
-            lower_bound: datetime.timedelta = (
-                datetime.timedelta(seconds=start_seconds)
-                if start_seconds is not None
-                else datetime.timedelta(0)
-            )
-            upper_bound: datetime.timedelta = (
-                datetime.timedelta(seconds=end_seconds)
-                if end_seconds is not None
-                else _max_timedelta
-            )
-            return lower_bound <= note.timestamp <= upper_bound
+    def timestamp_at_tick(
+        self, tick: Tick, *, start_iteration_index: int = 0
+    ) -> tuple[Timestamp, int]:
+        """Returns the timestamp at the input tick, and an optimizing value.
 
-        if (start_tick is not None) or all_start_args_none:
-            event_is_eligible_fn = event_is_eligible_by_tick
-        elif start_time is not None:
-            event_is_eligible_fn = event_is_eligible_by_time
-        elif start_seconds is not None:
-            event_is_eligible_fn = event_is_eligible_by_seconds
-        else:
-            raise RuntimeError(
-                "unhandled input combination; should be impossible"
-            )  # pragma: no cover
-
-        try:
-            track = self.instrument_tracks[instrument][difficulty]
-        except KeyError:
+        Args:
+            tick: The tick at which the timestamp should be calculated.
+
+        Kwargs:
+            start_iteration_index: An optional optimizing input that allows this function to start
+                iterating over BPM events at a later index. Only pass this if you are certain that
+                the event that should be proximal to tick is _not_ before this index. Not passing
+                this kwarg results only in slower execution.
+
+        Returns:
+            The timestamp at the input tick, plus the index of the ``BPMEvent`` proximal to the
+            input tick. This index can be passed to successive calls to this function via
+            ``start_iteration_index`` as an optimization.
+        """
+        proximal_bpm_event_index = self._index_of_proximal_event(
+            tick, start_iteration_index=start_iteration_index
+        )
+        proximal_bpm_event = self.events[proximal_bpm_event_index]
+        ticks_since_proximal_bpm_event = chartparse.tick.between(proximal_bpm_event.tick, tick)
+        seconds_since_proximal_bpm_event = chartparse.tick.seconds_from_ticks_at_bpm(
+            ticks_since_proximal_bpm_event,
+            proximal_bpm_event.bpm,
+            self.resolution,
+        )
+        timestamp = chartparse.time.add(
+            proximal_bpm_event.timestamp, seconds_since_proximal_bpm_event
+        )
+        return timestamp, proximal_bpm_event_index
+
+    def _index_of_proximal_event(self, tick: Tick, start_iteration_index: int = 0) -> int:
+        index_of_last_event = len(self) - 1
+        if start_iteration_index > index_of_last_event:
             raise ValueError(
-                f"no instrument track for difficulty {difficulty} instrument {instrument}"
+                f"there are no BPMEvents at or after index {start_iteration_index} in bpm_events"
             )
-        events_to_consider = list(filter(event_is_eligible_fn, track.note_events))
-        if len(events_to_consider) < 2:
+
+        first_event = self[start_iteration_index]
+        if first_event.tick > tick:
             raise ValueError(
-                "cannot determine average notes per second value of phrase with fewer than 2 "
-                f"Events: {events_to_consider}"
+                f"input tick {tick} precedes tick value of first BPMEvent ({first_event.tick})"
             )
 
-        return self._notes_per_second_from_events(events_to_consider)
+        # Do NOT iterate over last BPMEvent, since it has no next event.
+        for index in range(start_iteration_index, index_of_last_event):
+            if self[index + 1].tick > tick:
+                return index
+
+        # If none of the previous BPMEvents are proximal, the last event is proximal by
+        # definition.
+        return index_of_last_event
+
+
+@typ.final
+@dataclasses.dataclass(kw_only=True, frozen=True)
+class AnchorEvent(Event):
+    """An event representing a tick "locked" to a particular timestamp."""
 
-    @staticmethod
-    def _notes_per_second_from_events(events: Sequence[NoteEvent]) -> float:
-        first_event = events[0]
-        last_event = events[-1]
-        assert first_event.timestamp is not None
-        assert last_event.timestamp is not None
-        phrase_duration_seconds = (last_event.timestamp - first_event.timestamp).total_seconds()
-        return len(events) / phrase_duration_seconds
-
-    def __str__(self) -> str:  # pragma: no cover
-        items = []
-        if hasattr(self, "metadata"):
-            items.append(f"{self.metadata}")
-        if hasattr(self, "global_events_track"):
-            items.append(f"{self.global_events_track}")
-        if hasattr(self, "sync_track"):
-            items.append(f"{self.sync_track}")
-        if hasattr(self, "instrument_tracks"):
-            for _, difficulty_dict in self.instrument_tracks.items():
-                for _, track in difficulty_dict.items():
-                    items.append(f"{track}")
-
-        item_string = ",\n  ".join(items)
-        return f"{type(self).__name__}(\n  {item_string})"
+    Self = typ.TypeVar("Self", bound="AnchorEvent")
 
+    @classmethod
+    def from_parsed_data(cls: type[Self], data: AnchorEvent.ParsedData) -> Self:
+        """Obtain an instance of this object from parsed data.
 
-def _iterate_from_second_elem(xs: Sequence[T]) -> Iterator[T]:
-    """Given an iterable ``xs``, return an iterator that skips ``xs[0]``.
+        Args:
+            data: The data necessary to create an event.
 
-    Args:
-        xs: Any non-exhausted iterable.
+        Returns:
+            An an instance of this object initialized from ``data``.
+        """
 
-    Returns:
-        A iterator that iterates over ``xs``, ignoring the first element.
-    """
-    it = iter(xs)
-    next(it)
-    yield from it
+        timestamp = Timestamp(timedelta(microseconds=data.microseconds))
+        return cls(tick=data.tick, timestamp=timestamp)
+
+    @typ.final
+    @dataclasses.dataclass(kw_only=True, frozen=True, repr=False)
+    class ParsedData(Event.ParsedData, DictReprMixin):
+        """The data on a single chart line associated with an ``AnchorEvent``."""
+
+        Self = typ.TypeVar("Self", bound="AnchorEvent.ParsedData")
+
+        microseconds: int
+
+        # Match 1: Tick
+        # Match 2: Microseconds
+        _regex: typ.Final[str] = r"^\s*?(\d+?) = A (\d+?)$"
+        _regex_prog: typ.Final[typ.Pattern[str]] = re.compile(_regex)
+
+        @classmethod
+        def from_chart_line(cls: type[Self], line: str) -> Self:
+            """Attempt to construct this object from a ``.chart`` line.
+
+            Args:
+                line: A string, obtained from a Moonscraper ``.chart`` file.
+
+            Returns:
+                An an instance of this object initialized from ``line``.
+
+            Raises:
+                RegexNotMatchError: If the mixed-into class' ``_regex`` does not match ``line``.
+            """
+            m = cls._regex_prog.match(line)
+            if not m:
+                raise RegexNotMatchError(cls._regex, line)
+            raw_tick, raw_microseconds = m.groups()
+            return cls(tick=Tick(int(raw_tick)), microseconds=int(raw_microseconds))
```

### Comparing `chartparse-0.2.0/chartparse/event.py` & `chartparse-0.3.1/chartparse/event.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,62 @@
+"""For functionality useful for all event objects.
+
+.. _Google Python Style Guide:
+    http://google.github.io/styleguide/pyguide.html
+
+"""
+
 from __future__ import annotations
 
-import datetime
-from typing import Optional, TypeVar
+import abc
+import dataclasses
+import typing as typ
 
+from chartparse.tick import Tick
+from chartparse.time import Timestamp
 from chartparse.util import DictPropertiesEqMixin, DictReprMixin
 
-EventT = TypeVar("EventT", bound="Event")
 
-
-# TODO: Should this be an abstract base class?
+@dataclasses.dataclass(kw_only=True, frozen=True)
 class Event(DictPropertiesEqMixin, DictReprMixin):
-    """An event that occurs at a specific tick in an :class:`~chartparse.track.EventTrack`.
+    """An event that occurs at a tick and timestamp in an event track.
 
     This is typically used only as a base class for more specialized subclasses. It implements an
     attractive ``__str__`` representation.
     """
 
-    tick: int
+    tick: Tick
     """The tick at which this event occurs."""
 
-    # TODO: Figure out a way for ``timestamp`` to not be Optional.
-    timestamp: Optional[datetime.timedelta]
-    """The timestamp when this event occurs.
+    timestamp: Timestamp
+    """The timestamp when this event occurs."""
 
-    Optional, as it may need to be calculated later.
-    """
+    _proximal_bpm_event_index: int = 0
 
-    def __init__(self, tick: int, timestamp: Optional[datetime.timedelta] = None) -> None:
-        self.tick = tick
-        self.timestamp = timestamp
-
-    # TODO: Figure out a way for the final closing parenthesis to wrap _around_ any additional info
-    # added by subclass __str__ implementations.
-    def __str__(self) -> str:  # pragma: no cover
-        to_join = [f"{type(self).__name__}(t@{self.tick:07}"]
-        if self.timestamp is not None:
-            as_str = (
-                str(self.timestamp)
-                if self.timestamp.total_seconds() > 0
-                else f"{self.timestamp}.000000"
-            )
-            to_join.append(f" {as_str}")
-        to_join.append(")")
+    # TODO(P3): Figure out a way for the final closing parenthesis to wrap _around_ any additional
+    # info added by subclass __str__ implementations.
+    def __str__(self) -> str:
+        to_join = [f"{type(self).__name__}(t@{self.tick:07})"]
+        as_str = (
+            str(self.timestamp)
+            # This normally converts to str with six decimal digits, but for integral timedeltas,
+            # it prints with no decimal places. Manually force decimals to be included so
+            # everything lines up prettily.
+            if not self.timestamp.total_seconds().is_integer()
+            else f"{self.timestamp}.000000"
+        )
+        to_join.append(f": {as_str}")
         return "".join(to_join)
+
+    @dataclasses.dataclass(kw_only=True, frozen=True)
+    class ParsedData(abc.ABC):
+        """The data on a single chart line associated with an ``Event``."""
+
+        tick: Tick
+        """The tick at which the event represented by this data occurs."""
+
+        Self = typ.TypeVar("Self", bound="Event.ParsedData")
+
+        @classmethod
+        @abc.abstractmethod
+        def from_chart_line(cls: type[Self], line: str) -> Self:
+            ...  # pragma: no cover
```

### Comparing `chartparse-0.2.0/chartparse/exceptions.py` & `chartparse-0.3.1/chartparse/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,80 @@
+"""For custom exceptions raised in this package.
+
+.. _Google Python Style Guide:
+    http://google.github.io/styleguide/pyguide.html
+
+"""
+
 from __future__ import annotations
 
+import typing as typ
 from collections.abc import Collection
-from typing import Union, overload
 
 
 def raise_(ex: Exception) -> None:
     """Raises ``ex``.
 
     Can be used to raise an exception from within a lambda.
     """
 
     raise ex
 
 
+@typ.final
 class MissingRequiredField(Exception):
     """Raised when a required :class:`~chartparse.metadata.Metadata` could not be parsed."""
 
-    field_name: str
-    message: str
+    field_name: typ.Final[str]
+    message: typ.Final[str]
 
     def __init__(self, field_name: str) -> None:
         self.field_name = field_name
         self.message = f"unable to find a chart line matching required field '{field_name}'"
         super().__init__(self.message)
 
 
+@typ.final
 class RegexNotMatchError(Exception):
     """Raised when a regex failed to match."""
 
-    regex: str
-    message: str
+    regex: typ.Final[str]
+    message: typ.Final[str]
 
-    @overload
+    # TODO(P2): How do you document overloads with Sphinx?
+    @typ.overload
     def __init__(self, regex: str) -> None:
         ...  # pragma: no cover
 
-    @overload
+    @typ.overload
     def __init__(self, regex: str, s: str) -> None:
         ...  # pragma: no cover
 
-    @overload
+    @typ.overload
     def __init__(self, regex: str, s: Collection[str]) -> None:
         ...  # pragma: no cover
 
-    def __init__(self, regex: str, s: Union[None, str, Collection[str]] = None) -> None:
-        self.regex = regex
+    def __init__(self, regex: str, s: typ.Union[None, str, Collection[str]] = None) -> None:
         if s is None:
-            self.message = f"regex '{regex}' failed to match"
+            message = f"regex '{regex}' failed to match"
         elif isinstance(s, str):
-            self.message = f"string '{s}' failed to match regex '{regex}'"
+            message = f"string '{s}' failed to match regex '{regex}'"
         else:
-            self.message = f"none of {len(s)} strings matched regex '{regex}'"
-        super().__init__(self.message)
+            message = f"none of {len(s)} strings matched regex '{regex}'"
+        super().__init__(message)
+        self.regex = regex
+        self.message = message
+
+
+@typ.final
+class UnreachableError(Exception):
+    """Raised in branches that should be unreachable.
+
+    Oftentimes, these branches must exist to satisfy mypy. If this error is raised, it indicates
+    a fundamental issue with the code that should have been caught during review.
+    """
+
+    message: typ.Final[str]
+
+    def __init__(self, reason: str) -> None:
+        super().__init__(reason)
+        self.message = reason
```

### Comparing `chartparse-0.2.0/chartparse/metadata.py` & `chartparse-0.3.1/chartparse/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+"""For representing a chart's metadata, such as musical artist.
+
+You should not need to create any of this module's objects manually; please instead create a
+:class:`~chartparse.chart.Chart` and inspect its attributes via that object.
+
+.. _Google Python Style Guide:
+    http://google.github.io/styleguide/pyguide.html
+
+"""
+
 from __future__ import annotations
 
+import dataclasses
 import enum
 import re
-from collections.abc import Callable, Iterable
-from typing import Literal, Optional, Pattern, Type, TypedDict, TypeVar, Union
+import typing as typ
+from collections.abc import Callable
 
 from chartparse.exceptions import MissingRequiredField, RegexNotMatchError, raise_
-from chartparse.track import HasSectionNameMixin
+from chartparse.tick import Ticks
 from chartparse.util import DictPropertiesEqMixin, DictReprMixin
 
-SnakeCaseFieldNameT = Literal[
+if typ.TYPE_CHECKING:  # pragma: no cover
+    from collections.abc import Iterable
+
+SnakeCaseFieldName = typ.Literal[
     "resolution",
     "offset",
     "player2",
     "difficulty",
     "preview_start",
     "preview_end",
     "genre",
@@ -32,15 +46,15 @@
     "drum3_stream",
     "drum4_stream",
     "vocal_stream",
     "keys_stream",
     "crowd_stream",
 ]
 
-PascalCaseFieldNameT = Literal[
+PascalCaseFieldName = typ.Literal[
     "Resolution",
     "Offset",
     "Player2",
     "Difficulty",
     "PreviewStart",
     "PreviewEnd",
     "Genre",
@@ -59,29 +73,32 @@
     "Drum3Stream",
     "Drum4Stream",
     "VocalStream",
     "KeysStream",
     "CrowdStream",
 ]
 
-FieldValueT = Union[int, str, "Player2Instrument"]
-
-FieldValueParserT = Callable[[str], FieldValueT]
-
 
 @enum.unique
 class Player2Instrument(enum.Enum):
     """The instrument type of the co-op guitar chart in Guitar Hero 3."""
 
     BASS = "bass"
     RHYTHM = "rhythm"
 
 
-class _FieldValuesDict(TypedDict, total=False):
-    resolution: int
+FieldValue = Ticks | int | str | Player2Instrument
+
+FieldValueParser = Callable[[str], FieldValue]
+
+
+class _FieldValuesDict(typ.TypedDict, total=False):
+    # TODO(P2): Should resolution even be here? I think it is technically part of this part of the
+    # chart, but it is much more useful coupled to BPMEvents.
+    resolution: Ticks
     offset: int
     player2: Player2Instrument
     difficulty: int
     preview_start: int
     preview_end: int
     genre: str
     media_type: str
@@ -103,71 +120,75 @@
     crowd_stream: str
 
 
 class _FieldParsingSpec(object):
     """A bundle of data necessary to parse a field from a ``.chart`` file."""
 
     regex: str
-    regex_prog: Pattern[str]
+    regex_prog: typ.Pattern[str]
 
-    # Cannot actually be annotated as an instance attribute directly due to longstanding mypy bug:
-    # https://github.com/python/mypy/issues/708.
-    # processing_fn: FieldValueParserT
+    processing_fn: FieldValueParser
 
-    def __init__(self, regex: str, processing_fn: FieldValueParserT) -> None:
+    def __init__(self, regex: str, processing_fn: FieldValueParser) -> None:
         self.regex = regex
         self.regex_prog = re.compile(self.regex)
         self.processing_fn = processing_fn
 
     @staticmethod
-    def make_field_regex(
-        field_name: PascalCaseFieldNameT, value_regex: str, is_value_quoted: bool
-    ) -> str:
-        to_join = [rf"^\s*?{field_name} = "]
-        if is_value_quoted:
-            to_join.append(r'"')
-        to_join.append(rf"({value_regex})")
-        if is_value_quoted:
-            to_join.append(r'"')
-        to_join.append(r"\s*?$")
-        return "".join(to_join)
+    def make_field_regex(field_name: PascalCaseFieldName, value_regex: str) -> str:
+        """Returns a regex for parsing a particular field.
+
+        Args:
+            field_name: The name of the field to be parsed.
 
+            value_regex: The regex that parses the field's value. This should _not_ contain ^ or $,
+                as this will be interpolated within another regex pattern that does have those.
 
+        Returns:
+            A regex capable of extracting a particular field's value from a chart line containing a
+            a definition for that field.
+        """
+        return rf"^\s*?{field_name} = \"?({value_regex})\"?\s*?$"
+
+
+@typ.final
 class _IntFieldSpec(_FieldParsingSpec):
-    def __init__(self, field_name: PascalCaseFieldNameT) -> None:
+    def __init__(self, field_name: PascalCaseFieldName) -> None:
         super().__init__(self.make_int_field_regex(field_name), int)
 
     @staticmethod
-    def make_int_field_regex(field_name: PascalCaseFieldNameT) -> str:
-        return _FieldParsingSpec.make_field_regex(field_name, r"\d+?", False)
+    def make_int_field_regex(field_name: PascalCaseFieldName) -> str:
+        return _FieldParsingSpec.make_field_regex(field_name, r"\d+?")
 
 
+@typ.final
 class _MultiwordStrFieldSpec(_FieldParsingSpec):
-    def __init__(self, field_name: PascalCaseFieldNameT) -> None:
+    def __init__(self, field_name: PascalCaseFieldName) -> None:
         super().__init__(self.make_multiword_str_field_regex(field_name), str)
 
     @staticmethod
-    def make_multiword_str_field_regex(field_name: PascalCaseFieldNameT) -> str:
-        return _FieldParsingSpec.make_field_regex(field_name, r".+?", True)
+    def make_multiword_str_field_regex(field_name: PascalCaseFieldName) -> str:
+        return _FieldParsingSpec.make_field_regex(field_name, r".+?")
 
 
+@typ.final
 class _QuotelessStrFieldSpec(_FieldParsingSpec):
     def __init__(
         self,
-        field_name: PascalCaseFieldNameT,
-        processing_fn: FieldValueParserT,
+        field_name: PascalCaseFieldName,
+        processing_fn: FieldValueParser,
     ) -> None:
         super().__init__(self.make_quoteless_str_field_regex(field_name), processing_fn)
 
     @staticmethod
-    def make_quoteless_str_field_regex(field_name: PascalCaseFieldNameT) -> str:
-        return _FieldParsingSpec.make_field_regex(field_name, r'[^"]+?', False)
+    def make_quoteless_str_field_regex(field_name: PascalCaseFieldName) -> str:
+        return _FieldParsingSpec.make_field_regex(field_name, r'[^"]+?')
 
 
-class _FieldParsingSpecDict(TypedDict):
+class _FieldParsingSpecDict(typ.TypedDict):
     resolution: _FieldParsingSpec
     offset: _FieldParsingSpec
     player2: _FieldParsingSpec
     difficulty: _FieldParsingSpec
     preview_start: _FieldParsingSpec
     preview_end: _FieldParsingSpec
     genre: _FieldParsingSpec
@@ -213,218 +234,149 @@
     "drum3_stream": _MultiwordStrFieldSpec("Drum3Stream"),
     "drum4_stream": _MultiwordStrFieldSpec("Drum4Stream"),
     "vocal_stream": _MultiwordStrFieldSpec("VocalStream"),
     "keys_stream": _MultiwordStrFieldSpec("KeysStream"),
     "crowd_stream": _MultiwordStrFieldSpec("CrowdStream"),
 }
 
-MetadataT = TypeVar("MetadataT", bound="Metadata")
 
-
-class Metadata(HasSectionNameMixin, DictPropertiesEqMixin, DictReprMixin):
+@typ.final
+@dataclasses.dataclass(frozen=True, kw_only=True)
+class Metadata(DictPropertiesEqMixin, DictReprMixin):
     """All of a :class:`~chartparse.chart.Chart` object's metadata."""
 
-    section_name = "Song"
+    Self = typ.TypeVar("Self", bound="Metadata")
+
+    header_tag: typ.ClassVar[str] = "Song"
+    """The name of this track's data section in a ``.chart`` file."""
 
-    resolution: int
+    resolution: Ticks
     """The number of ticks for which a quarter note lasts."""
 
-    offset: int
+    offset: int = 0
     """The number of seconds in time before tick 0 is reached.
 
     This is a legacy field and should most likely be ignored.
     """
 
-    player2: Player2Instrument
+    player2: Player2Instrument = Player2Instrument.BASS
     """The instrument type of the co-op guitar chart in Guitar Hero 3."""
 
-    difficulty: int
+    difficulty: int = 0
     """The perceived difficulty to play the chart.
 
-    This is often referred to as "intensity".
+    This is often referred to as "intensity" in modern Guitar Hero.
     """
 
-    preview_start: int
+    preview_start: int = 0
     """The number of seconds into the song at which the song preview should start.
 
     Might not actually be seconds. Typically, ``preview_start_time`` in ``song.ini`` is respected
     for Clone Hero instead.
     """
 
-    preview_end: int
+    preview_end: int = 0
     """The number of seconds into the song at which the song preview should end.
 
     Might not actually be seconds. Clone Hero just plays a preview of a particular length starting
     at ``preview_start_time`` in ``song.ini``, so this is unlikely to ever do anything in modern
     Guitar Hero.
     """
 
-    genre: str
+    genre: str = "rock"
     """The genre of the chart's song."""
 
-    media_type: str
+    media_type: str = "cd"
     """The type of media from which the chart's song originates."""
 
-    name: str
+    name: str | None = None
     """The name of the chart's song."""
 
-    artist: str
+    artist: str | None = None
     """The name of the chart's song's artist."""
 
-    charter: str
+    charter: str | None = None
     """The user who made this chart."""
 
-    album: str
+    album: str | None = None
     """The name of the chart's song's album."""
 
-    year: str
+    year: str | None = None
     """The year the chart's song came out.
 
-    This is formatted as, e.g. ", 2018" because it saved time when importing into GHTCP (Guitar
-    Hero Three Control Panel).
+    This is formatted as, e.g. ", 2018" because it historically saved time when importing into
+    GHTCP (Guitar Hero Three Control Panel).
     """
 
-    music_stream: str
+    music_stream: str | None = None
     """The filename of the main music audio file."""
 
-    guitar_stream: str
+    guitar_stream: str | None = None
     """The filename of the guitar audio file."""
 
-    rhythm_stream: str
+    rhythm_stream: str | None = None
     """The filename of the rhythm audio file."""
 
-    bass_stream: str
+    bass_stream: str | None = None
     """The filename of the bass audio file."""
 
-    drum_stream: str
+    drum_stream: str | None = None
     """The filename of the drum audio file."""
 
-    drum2_stream: str
+    drum2_stream: str | None = None
     """The filename of the drum2 audio file."""
 
-    drum3_stream: str
+    drum3_stream: str | None = None
     """The filename of the drum3 audio file."""
 
-    drum4_stream: str
+    drum4_stream: str | None = None
     """The filename of the drum4 audio file."""
 
-    vocal_stream: str
+    vocal_stream: str | None = None
     """The filename of the vocal audio file."""
 
-    keys_stream: str
+    keys_stream: str | None = None
     """The filename of the keys audio file."""
 
-    crowd_stream: str
+    crowd_stream: str | None = None
     """The filename of the crowd audio file."""
 
-    def __init__(
-        self,
-        resolution: int,
-        offset: int = 0,
-        player2: Player2Instrument = Player2Instrument.BASS,
-        difficulty: int = 0,
-        preview_start: int = 0,
-        preview_end: int = 0,
-        genre: str = "rock",
-        media_type: str = "cd",
-        name: Optional[str] = None,
-        artist: Optional[str] = None,
-        charter: Optional[str] = None,
-        album: Optional[str] = None,
-        year: Optional[str] = None,
-        music_stream: Optional[str] = None,
-        guitar_stream: Optional[str] = None,
-        rhythm_stream: Optional[str] = None,
-        bass_stream: Optional[str] = None,
-        drum_stream: Optional[str] = None,
-        drum2_stream: Optional[str] = None,
-        drum3_stream: Optional[str] = None,
-        drum4_stream: Optional[str] = None,
-        vocal_stream: Optional[str] = None,
-        keys_stream: Optional[str] = None,
-        crowd_stream: Optional[str] = None,
-    ) -> None:
-        """Initializes all instance attributes."""
-
-        self.resolution = resolution
-        self.offset = offset
-        self.player2 = player2
-        self.difficulty = difficulty
-        self.preview_start = preview_start
-        self.preview_end = preview_end
-        self.genre = genre
-        self.media_type = media_type
-        if name is not None:
-            self.name = name
-        if artist is not None:
-            self.artist = artist
-        if charter is not None:
-            self.charter = charter
-        if album is not None:
-            self.album = album
-        if year is not None:
-            self.year = year
-        if music_stream is not None:
-            self.music_stream = music_stream
-        if guitar_stream is not None:
-            self.guitar_stream = guitar_stream
-        if rhythm_stream is not None:
-            self.rhythm_stream = rhythm_stream
-        if bass_stream is not None:
-            self.bass_stream = bass_stream
-        if drum_stream is not None:
-            self.drum_stream = drum_stream
-        if drum2_stream is not None:
-            self.drum2_stream = drum2_stream
-        if drum3_stream is not None:
-            self.drum3_stream = drum3_stream
-        if drum4_stream is not None:
-            self.drum4_stream = drum4_stream
-        if vocal_stream is not None:
-            self.vocal_stream = vocal_stream
-        if keys_stream is not None:
-            self.keys_stream = keys_stream
-        if crowd_stream is not None:
-            self.crowd_stream = crowd_stream
-
     @classmethod
-    def from_chart_lines(
-        cls: Type[MetadataT], iterator_getter: Callable[[], Iterable[str]]
-    ) -> MetadataT:
+    def from_chart_lines(cls: type[Self], lines_iter: Iterable[str]) -> Self:
         """Initializes instance attributes by parsing an iterable of strings.
 
         Args:
-            iterator_getter: The iterable of strings returned by this is most likely from a
-                Moonscraper ``.chart``. Must be a function so the strings can be iterated over
-                multiple times, if necessary.
+            lines_iter: An iterable of strings obtained from a Moonscraper ``.chart`` file.
         """
         kwargs: _FieldValuesDict = dict()
 
+        lines = list(lines_iter)
+
         def set_kwarg(
-            field_name: SnakeCaseFieldNameT,
-            regex_not_match_callback: Optional[Callable[[], None]] = None,
+            field_name: SnakeCaseFieldName,
+            regex_not_match_callback: Callable[[], None] | None = None,
         ) -> None:
             maybe_set_kwarg(
                 field_name,
                 regex_not_match_callback=lambda: raise_(MissingRequiredField(field_name)),
             )
 
         def maybe_set_kwarg(
-            field_name: SnakeCaseFieldNameT,
-            regex_not_match_callback: Optional[Callable[[], None]] = None,
+            field_name: SnakeCaseFieldName,
+            regex_not_match_callback: Callable[[], None] | None = None,
         ) -> None:
             try:
                 kwargs[field_name] = parse_all_lines_for_field(field_name)
             except RegexNotMatchError:
                 if regex_not_match_callback is not None:
                     regex_not_match_callback()
 
-        def parse_all_lines_for_field(field_name: SnakeCaseFieldNameT) -> FieldValueT:
+        def parse_all_lines_for_field(field_name: SnakeCaseFieldName) -> FieldValue:
             regex_prog = _field_parsing_specs[field_name].regex_prog
-            for line in iterator_getter():
+            for line in lines:
                 m = regex_prog.match(line)
                 if m:
                     return _field_parsing_specs[field_name].processing_fn(m.group(1))
             raise RegexNotMatchError(_field_parsing_specs[field_name].regex)
 
         set_kwarg("resolution")
         maybe_set_kwarg("offset")
```

### Comparing `chartparse-0.2.0/chartparse/util.py` & `chartparse-0.3.1/chartparse/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,71 @@
+"""For various utilities useful throughout ``chartparse``.
+
+.. _Google Python Style Guide:
+    http://google.github.io/styleguide/pyguide.html
+
+"""
+
 from __future__ import annotations
 
 import enum
 from collections.abc import Sequence
 
-from chartparse.datastructures import ImmutableList
 from chartparse.hints import T
 
 
 class DictPropertiesEqMixin(object):
-    """A mixin that implements ``__eq__`` via ``__dict__().__eq__``."""
+    """A mixin that implements ``__eq__`` via ``__dict__().__eq__``.
+
+    An object with this mixed in will equate to other objects that share this mixin and have equal
+    ``__dict__``\\s.
+    """
 
     def __eq__(self, other: object) -> bool:
         if not issubclass(other.__class__, DictPropertiesEqMixin):
             return NotImplemented
         return self.__dict__ == other.__dict__
 
 
 class DictReprMixin(object):
-    """A mixin implementing ``__repr__`` by dumping ``__dict__()``."""
+    """A mixin implementing ``__repr__`` by dumping ``__dict__()``.
+
+    Additionally, this ignores class attributes, since they (typically) do not change and are
+    therefore uninteresting.
+    """
 
-    def __repr__(self) -> str:  # pragma: no cover
-        return f"{type(self).__name__}({str(self.__dict__)[1:-1]})"
+    def __repr__(self) -> str:
+        instance_attrs = {k: v for k, v in self.__dict__.items() if not hasattr(self.__class__, k)}
+        return f"{type(self).__name__}({str(instance_attrs)[1:-1]})"
 
 
+# TODO(P2): this (and DictReprMixin) probably needs to handle missing values somehow? The repr of
+# bare test objects raises an exception for missing attributes, but I guess it expects them to be
+# there because they are dataclasses?
 class DictReprTruncatedSequencesMixin(object):
-    """A mixin implementing ``__repr__`` by dumping ``__dict__()`` with truncated sequences."""
+    """A mixin implementing ``__repr__`` by dumping ``__dict__()`` with truncated sequences.
+
+    Specifically, any instance attribute of type `Sequence
+    <https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence>`_ with
+    more than 1 element will be represented as such::
+
+        ["foo", ... 4 more elements]
+
+    Additionally, this ignores class attributes, since they (typically) do not change and are
+    therefore uninteresting.
+    """
+
+    def __repr__(self) -> str:
+        # TODO(P2): This doesn't work if dataclasses were created in the "bare" manner, since it
+        # thinks all of the dataclass' fields should be set, and crashes when they aren't. Possible
+        # solution is to migrate all usage of "bare" to "minimal".
+        instance_attrs = {k: v for k, v in self.__dict__.items() if not hasattr(self.__class__, k)}
 
-    def __repr__(self) -> str:  # pragma: no cover
         items = []
-        for k, v in self.__dict__.items():
+        for k, v in instance_attrs.items():
             item = f"'{k}': "
             if isinstance(v, Sequence) and len(v) > 1:
                 item += f"[{v[0]}, ... {len(v)-1} more elements]"
             else:
                 item += f"{v}"
             items.append(item)
 
@@ -40,14 +73,14 @@
         return f"{type(self).__name__}({item_string})"
 
 
 class AllValuesGettableEnum(enum.Enum):
     """A wrapper for ``Enum`` that adds a method for returning all enum values."""
 
     @classmethod
-    def all_values(cls) -> ImmutableList[T]:
+    def all_values(cls) -> Sequence[T]:
         """Returns all Enum values.
 
         Returns:
-            An :class:`~chartparse.datastructures.ImmutableList` containing all Enum values.
+            A Sequence containing all Enum values.
         """
-        return ImmutableList([c.value for c in cls])
+        return [c.value for c in cls]
```

### Comparing `chartparse-0.2.0/chartparse.egg-info/PKG-INFO` & `chartparse-0.3.1/chartparse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: chartparse
-Version: 0.2.0
+Version: 0.3.1
 Summary: A library for parsing Guitar Hero .chart files.
 Home-page: https://github.com/AWConant/chartparse/
 Author: AWConant
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ---
 # chartparse
 
@@ -26,31 +24,33 @@
 
 ```py
 from chartparse.chart import Chart
 from chartparse.instrument import Instrument, Difficulty
 
 c = Chart.from_filepath("/path/to/file.chart")
 
-# the first 7 BPM changes
+# the first 7 BPM changes (including the initial one)
 c.sync_track.bpm_events[:7]
 
-# the first 8 time signature changes
+# the first 8 time signature changes (including the initial one)
 c.sync_track.time_signature_events[:8]
 
-expert_guitar = c.instrument_tracks[Instrument.GUITAR][Difficulty.EXPERT]
+expert_guitar = c[Instrument.GUITAR][Difficulty.EXPERT]
 
 # the first 10 notes of the expert guitar chart
 expert_guitar.note_events[:10]
 
 # the first 3 star power phrases of the expert guitar chart
 expert_guitar.star_power_events[:3]
 ```
 
+See the [documentation](https://chartparse-gh.readthedocs.io/en/latest/) for more detailed
+guidance.
+
 Note: this software is tested only with .chart files that are written by
 [Moonscraper](https://github.com/FireFox2000000/Moonscraper-Chart-Editor).
 Files written by other editors or are handwritten may produce undefined
 behavior.
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
```

### Comparing `chartparse-0.2.0/setup.py` & `chartparse-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Python setup.py for chartparse package"""
 import io
 import os
+
 from setuptools import find_packages, setup
 
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
     >>> read("README.md")
     ...
```

