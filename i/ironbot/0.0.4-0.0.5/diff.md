# Comparing `tmp/ironbot-0.0.4.tar.gz` & `tmp/ironbot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironbot-0.0.4.tar", max compression
+gzip compressed data, was "ironbot-0.0.5.tar", max compression
```

## Comparing `ironbot-0.0.4.tar` & `ironbot-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.4/LICENSE
--rw-r--r--   0        0        0     1939 2023-06-05 22:40:55.330531 ironbot-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-03 00:02:15.086424 ironbot-0.0.4/ironbot/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-03 00:04:34.846656 ironbot-0.0.4/ironbot/__main__.py
--rw-r--r--   0        0        0     2110 2023-06-05 22:46:37.886279 ironbot-0.0.4/ironbot/models.py
--rw-r--r--   0        0        0     2083 2023-06-03 00:01:27.405671 ironbot-0.0.4/ironbot/scrappers.py
--rw-r--r--   0        0        0     1555 2023-06-05 22:47:43.195292 ironbot-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ironbot-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1939 2023-06-05 22:40:55.330531 ironbot-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 00:02:15.086424 ironbot-0.0.5/ironbot/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-03 00:04:34.846656 ironbot-0.0.5/ironbot/__main__.py
+-rw-r--r--   0        0        0     2654 2023-06-09 04:39:25.712529 ironbot-0.0.5/ironbot/models.py
+-rw-r--r--   0        0        0     1069 2023-06-09 05:41:45.789123 ironbot-0.0.5/ironbot/parsers.py
+-rw-r--r--   0        0        0     2070 2023-06-09 05:43:22.012933 ironbot-0.0.5/ironbot/scrappers.py
+-rw-r--r--   0        0        0     1616 2023-06-09 05:46:40.642018 ironbot-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 ironbot-0.0.5/PKG-INFO
```

### Comparing `ironbot-0.0.4/LICENSE` & `ironbot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.4/README.md` & `ironbot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.4/ironbot/__main__.py` & `ironbot-0.0.5/ironbot/__main__.py`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.4/ironbot/models.py` & `ironbot-0.0.5/ironbot/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,74 @@
-from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from re import match
 from typing import Iterator
 
-from camelot import read_pdf  # type: ignore
+from sqlalchemy import Column, Integer, String, Date
+from sqlalchemy.orm import DeclarativeBase
 
 
 CATEGORY = r"^[MWF](PRO)?$"
 
 
 class Title(Enum):
     CALENDAR: str = "PRO Event Calendar"
     START_LIST: str = "Start Lists"
 
     def __eq__(self, other) -> bool:
         return self.value.lower() == other.strip().lower()
 
 
-@dataclass
-class Event:
-    when: str
-    name: str
-    prize: str
-    slots: str
-    registration: str
-    deadline: str
+class Base(DeclarativeBase):
+    pass
 
-    def __post_init__(self) -> None:
-        self.date = datetime.strptime(self.when, "%m/%d/%Y").date()
+
+class Event(Base):
+    __tablename__ = "events"
+
+    id = Column(Integer, primary_key=True)
+    name = Column(String)
+    when = Column(Date)
+    prize = Column(String)
+    slots = Column(String)
+    registration = Column(String)
+    deadline = Column(String)
+
+    def __init__(self, *args, **kwargs):
+        kwargs["when"] = datetime.strptime(kwargs["when"], "%m/%d/%Y").date()
+        return super().__init__(*args, **kwargs)
 
     def __str__(self) -> str:
         fields = (
-            self.date.strftime("%Y-%m-%d"),
+            self.when.strftime("%Y-%m-%d"),
             self.name,
             self.prize,
             self.slots,
             self.registration,
             self.deadline,
         )
-        return "\t".join(fields)
+        return "\t".join(str(field) for field in fields)
+
+    def __repr__(self) -> str:
+        return str(self)
 
 
-@dataclass
-class Athlete:
-    bib: str
-    first_name: str
-    last_name: str
-    country: str
-    category: str
+class Athlete(Base):
+    __tablename__ = "athletes"
+
+    id = Column(Integer, primary_key=True)
+    bib = Column(String)
+    first_name = Column(String)
+    last_name = Column(String)
+    country = Column(String)
+    category = Column(String)
 
     @classmethod
     def from_row(cls, row: Iterator[str]) -> "Athlete":
-        fields = {key: "" for key in cls.__annotations__}
+        fields = {column.name: "" for column in cls.__table__.columns}
 
         for field in (field.strip() for field in row):
             if field.isnumeric() and not fields["bib"]:
                 fields["bib"] = field
             elif match(CATEGORY, field.upper()) and not fields["category"]:
                 fields["category"] = field
             elif not fields["last_name"]:
@@ -73,8 +85,11 @@
 
     @property
     def name(self) -> str:
         return f"{self.first_name} {self.last_name}"
 
     def __str__(self) -> str:
         fields = (self.bib, self.category, self.name, self.country)
-        return "\t".join(field for field in fields if field)
+        return "\t".join(str(field) for field in fields if field)
+
+    def __repr__(self) -> str:
+        return str(self)
```

### Comparing `ironbot-0.0.4/ironbot/scrappers.py` & `ironbot-0.0.5/ironbot/scrappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from importlib.metadata import version
 from os import path
 from tempfile import TemporaryDirectory
-from typing import Iterable, Iterator
+from typing import Iterable, Iterator, Optional
 from urllib.request import Request, urlopen, urlretrieve
 
 from camelot import read_pdf  # type: ignore
 from bs4 import BeautifulSoup
 
 from ironbot.models import Athlete, Event, Title
+from ironbot.parsers import EventParser
 
 
 URL = "https://www.ironman.com/pro-athletes"
 CALENDAR = "PRO Schedule".lower()
 HEADERS = {"User-Agent": f"ironbot/{version('ironbot')}", "Accept": "*/*"}
 
 
@@ -43,18 +44,15 @@
 
 def events(data: BeautifulSoup) -> Iterable[Event]:
     for a in data.find_all("a"):
         if a.text.strip().lower() != CALENDAR:
             continue
 
         for row in pdf_table_rows(a["href"]):
-            try:
-                yield Event(*row)
-            except ValueError:
-                pass
+            yield from EventParser(row)
 
         return
 
     raise RuntimeError("Calendar URL not found")
 
 
 def event_names(data: BeautifulSoup) -> Iterable[str]:
```

### Comparing `ironbot-0.0.4/pyproject.toml` & `ironbot-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ironbot"
-version = "0.0.4"
+version = "0.0.5"
 description = "CLI to get information about Ironman professional races"
 authors = ["Eduardo Cuducos <4732915+cuducos@users.noreply.github.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/cuducos/ironbot/"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -26,32 +26,35 @@
     ]
 
 [tool.poetry.scripts]
 ironbot = "ironbot.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
+alembic = "^1.11.1"
 beautifulsoup4 = "^4.12.2"
 camelot-py = "^0.11.0"
+sqlalchemy = "^2.0.15"
 typer = "^0.9.0"
 
 # we could use camelot-py[base] but that would inject problematic pdftopng, so
 # let's add the other base packages manually. See, for example:
 # https://github.com/vinayak-mehta/pdftopng/issues/11
 # https://github.com/vinayak-mehta/pdftopng/issues/8
 ghostscript = "^0.7"
 opencv-python = "^4.7.0.72"
 
 [tool.poetry.group.dev.dependencies]
+ipdb = "^0.13.13"
 ipython = "^8.13.2"
 pytest = "^7.3.1"
 pytest-black = "^0.3.12"
 pytest-mypy = "^0.10.3"
-types-beautifulsoup4 = "^4.12.0.5"
 pytest-watch = "^4.2.0"
+types-beautifulsoup4 = "^4.12.0.5"
 
 [tool.pytest.ini_options]
 addopts = "--black --mypy"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ironbot-0.0.4/PKG-INFO` & `ironbot-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI to get information about Ironman professional races
 Home-page: https://github.com/cuducos/ironbot/
 License: GPLv3
 Keywords: triathlon,Ironamn,Professional triathletes,Professional triathlon races
 Author: Eduardo Cuducos
 Author-email: 4732915+cuducos@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -16,18 +16,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
+Requires-Dist: alembic (>=1.11.1,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: camelot-py (>=0.11.0,<0.12.0)
 Requires-Dist: ghostscript (>=0.7,<0.8)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
+Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/cuducos/ironbot/
 Description-Content-Type: text/markdown
 
 # `ironbot` [![Tests](https://github.com/cuducos/ironbot/actions/workflows/tests.yml/badge.svg)](https://github.com/cuducos/ironbot/actions/workflows/tests.yml)
 
 ## Requirements
```

