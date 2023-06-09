# Comparing `tmp/pretext-1.6.1.dev20230608.tar.gz` & `tmp/pretext-1.6.1.dev20230609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230608.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230609.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230608.tar` & `pretext-1.6.1.dev20230609.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-08 06:21:35.347831 pretext-1.6.1.dev20230608/LICENSE
--rw-r--r--   0        0        0     9664 2023-06-08 06:21:35.347831 pretext-1.6.1.dev20230608/README.md
--rw-r--r--   0        0        0     1901 2023-06-08 06:22:04.779763 pretext-1.6.1.dev20230608/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/__main__.py
--rw-r--r--   0        0        0     8170 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/build.py
--rw-r--r--   0        0        0    22798 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-08 06:22:09.759752 pretext-1.6.1.dev20230608/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/core/resources.py
--rw-r--r--   0        0        0  1033652 2023-06-08 06:22:09.759752 pretext-1.6.1.dev20230608/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/generate.py
--rw-r--r--   0        0        0    24666 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/project.py
--rw-r--r--   0        0        0      516 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-08 06:22:09.823751 pretext-1.6.1.dev20230608/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-08 06:22:09.823751 pretext-1.6.1.dev20230608/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160064 2023-06-08 06:22:09.803752 pretext-1.6.1.dev20230608/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7570 2023-06-08 06:22:09.803752 pretext-1.6.1.dev20230608/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173263 2023-06-08 06:22:09.819751 pretext-1.6.1.dev20230608/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-06-08 06:22:09.823751 pretext-1.6.1.dev20230608/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4611 2023-06-08 06:22:09.823751 pretext-1.6.1.dev20230608/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-08 06:22:09.823751 pretext-1.6.1.dev20230608/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-08 06:22:09.823751 pretext-1.6.1.dev20230608/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8346 2023-06-08 06:22:09.823751 pretext-1.6.1.dev20230608/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18416 2023-06-08 06:21:35.351832 pretext-1.6.1.dev20230608/pretext/utils.py
--rw-r--r--   0        0        0     1143 2023-06-08 06:22:04.779763 pretext-1.6.1.dev20230608/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230608/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/LICENSE
+-rw-r--r--   0        0        0     9664 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/README.md
+-rw-r--r--   0        0        0     1901 2023-06-09 06:19:26.460978 pretext-1.6.1.dev20230609/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/__main__.py
+-rw-r--r--   0        0        0     8170 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/build.py
+-rw-r--r--   0        0        0    22798 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-09 06:19:31.393049 pretext-1.6.1.dev20230609/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/core/resources.py
+-rw-r--r--   0        0        0  1034862 2023-06-09 06:19:31.393049 pretext-1.6.1.dev20230609/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/generate.py
+-rw-r--r--   0        0        0    24666 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-09 06:19:31.461050 pretext-1.6.1.dev20230609/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-09 06:19:31.461050 pretext-1.6.1.dev20230609/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160064 2023-06-09 06:19:31.437049 pretext-1.6.1.dev20230609/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7570 2023-06-09 06:19:31.441049 pretext-1.6.1.dev20230609/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173263 2023-06-09 06:19:31.453050 pretext-1.6.1.dev20230609/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-06-09 06:19:31.461050 pretext-1.6.1.dev20230609/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4611 2023-06-09 06:19:31.457049 pretext-1.6.1.dev20230609/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-09 06:19:31.461050 pretext-1.6.1.dev20230609/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-09 06:19:31.461050 pretext-1.6.1.dev20230609/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8346 2023-06-09 06:19:31.461050 pretext-1.6.1.dev20230609/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18416 2023-06-09 06:18:53.416498 pretext-1.6.1.dev20230609/pretext/utils.py
+-rw-r--r--   0        0        0     1143 2023-06-09 06:19:26.460978 pretext-1.6.1.dev20230609/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230609/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230608/LICENSE` & `pretext-1.6.1.dev20230609/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/README.md` & `pretext-1.6.1.dev20230609/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/__init__.py` & `pretext-1.6.1.dev20230609/pretext/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '2f932ee34147145972432708f337a8a4102fc2d9'
+CORE_COMMIT = '390bd871cc5f84c3704b02ddf52b82239d09d000'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230608/pretext/build.py` & `pretext-1.6.1.dev20230609/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/cli.py` & `pretext-1.6.1.dev20230609/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/codechat.py` & `pretext-1.6.1.dev20230609/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230609/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/core/pretext.py` & `pretext-1.6.1.dev20230609/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/core/resources.py` & `pretext-1.6.1.dev20230609/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/core/resources.zip` & `pretext-1.6.1.dev20230609/pretext/core/resources.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,143 +1,143 @@
-Zip file size: 1033652 bytes, number of entries: 141
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 xsl/utilities/
--rw-r--r--  2.0 unx   230275 b- defN 23-Jun-08 06:22 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   609407 b- defN 23-Jun-08 06:22 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-08 06:22 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-08 06:22 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-08 06:22 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-08 06:22 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-08 06:22 xsl/entities.ent
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-08 06:22 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-08 06:22 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-08 06:22 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-08 06:22 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-08 06:22 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-08 06:22 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-08 06:22 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-Jun-08 06:22 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-08 06:22 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-08 06:22 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-08 06:22 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-08 06:22 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-08 06:22 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-08 06:22 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-08 06:22 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-08 06:22 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-08 06:22 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-08 06:22 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-08 06:22 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-08 06:22 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx   103793 b- defN 23-Jun-08 06:22 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-08 06:22 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-08 06:22 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-08 06:22 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-08 06:22 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-08 06:22 xsl/README.md
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-08 06:22 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-08 06:22 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-08 06:22 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-08 06:22 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-08 06:22 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-08 06:22 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-08 06:22 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-08 06:22 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-08 06:22 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-08 06:22 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-08 06:22 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-08 06:22 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 xsl/support/play-button/
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-08 06:22 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-08 06:22 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-08 06:22 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-08 06:22 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-08 06:22 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-08 06:22 xsl/support/README.md
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-08 06:22 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-08 06:22 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-08 06:22 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-08 06:22 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-08 06:22 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-08 06:22 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-08 06:22 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-08 06:22 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-08 06:22 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-08 06:22 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-08 06:22 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-08 06:22 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-08 06:22 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-08 06:22 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-08 06:22 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-08 06:22 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-08 06:22 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-08 06:22 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-08 06:22 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-08 06:22 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-08 06:22 xsl/localizations/README.md
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-08 06:22 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-08 06:22 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-08 06:22 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-08 06:22 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-08 06:22 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-08 06:22 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-08 06:22 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-08 06:22 css/kindle.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-08 06:22 css/update_css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-08 06:22 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-08 06:22 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-08 06:22 css/colors_default.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-08 06:22 css/colors_red_blue.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-08 06:22 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-08 06:22 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-08 06:22 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-08 06:22 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-08 06:22 css/colors_blue_green.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-08 06:22 css/mathbook-content.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-08 06:22 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-08 06:22 css/pretext.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-08 06:22 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-08 06:22 css/epub.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-08 06:22 css/mathbook-add-on.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-08 06:22 css/setcolors.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-08 06:22 css/pretext_add_on.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-08 06:22 css/mathbook-3.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-08 06:22 css/colors_green_plum.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-08 06:22 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-08 06:22 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-08 06:22 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-08 06:22 css/README.md
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-08 06:22 css/style_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-08 06:22 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-08 06:22 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 06:22 pretext/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-08 06:22 pretext/pretext.cfg
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-08 06:22 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-08 06:22 pretext/module-test.py
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-08 06:22 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-08 06:22 pretext/README.md
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-08 06:22 schema/xml.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-08 06:22 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-08 06:22 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-08 06:22 schema/pretext.xml
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-08 06:22 schema/pretext.rnc
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-08 06:22 schema/pretext.rng
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-08 06:22 schema/pretext-dev.rng
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-08 06:22 schema/build.sh
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-08 06:22 schema/pretext.xsd
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-08 06:22 schema/README.md
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-08 06:22 schema/pretext-validation-plus.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 script/mjsre/
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-08 06:22 script/mbx
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-08 06:22 script/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 06:22 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-08 06:22 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-08 06:22 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-08 06:22 script/mjsre/mj-sre-page.js
-141 files, 4804380 bytes uncompressed, 1016210 bytes compressed:  78.9%
+Zip file size: 1034862 bytes, number of entries: 141
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 xsl/utilities/
+-rw-r--r--  2.0 unx   231248 b- defN 23-Jun-09 06:19 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   611192 b- defN 23-Jun-09 06:19 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-09 06:19 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-09 06:19 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-09 06:19 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-09 06:19 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-09 06:19 xsl/entities.ent
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-09 06:19 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-09 06:19 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-09 06:19 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-09 06:19 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-09 06:19 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-09 06:19 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-09 06:19 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   111931 b- defN 23-Jun-09 06:19 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-09 06:19 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-09 06:19 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-09 06:19 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-09 06:19 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-09 06:19 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-09 06:19 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-09 06:19 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-09 06:19 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-09 06:19 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-09 06:19 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-09 06:19 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-09 06:19 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx   106649 b- defN 23-Jun-09 06:19 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-09 06:19 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-09 06:19 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-09 06:19 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-09 06:19 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-09 06:19 xsl/README.md
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-09 06:19 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-09 06:19 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-09 06:19 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-09 06:19 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-09 06:19 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-09 06:19 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-09 06:19 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-09 06:19 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-09 06:19 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-09 06:19 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-09 06:19 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-09 06:19 xsl/utilities/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 xsl/support/play-button/
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-09 06:19 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-09 06:19 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-09 06:19 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-09 06:19 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-09 06:19 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-09 06:19 xsl/support/README.md
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-09 06:19 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-09 06:19 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-09 06:19 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-09 06:19 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-09 06:19 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-09 06:19 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-09 06:19 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-09 06:19 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-09 06:19 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-09 06:19 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-09 06:19 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-09 06:19 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-09 06:19 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-09 06:19 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-09 06:19 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-09 06:19 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-09 06:19 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-09 06:19 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-09 06:19 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-09 06:19 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-09 06:19 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-09 06:19 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-09 06:19 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-09 06:19 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-09 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-09 06:19 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-09 06:19 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-09 06:19 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-09 06:19 css/kindle.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-09 06:19 css/update_css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-09 06:19 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-09 06:19 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-09 06:19 css/colors_default.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-09 06:19 css/colors_red_blue.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-09 06:19 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-09 06:19 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-09 06:19 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-09 06:19 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-09 06:19 css/colors_blue_green.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-09 06:19 css/mathbook-content.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-09 06:19 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-09 06:19 css/pretext.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-09 06:19 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-09 06:19 css/epub.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-09 06:19 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-09 06:19 css/setcolors.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-09 06:19 css/pretext_add_on.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-09 06:19 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-09 06:19 css/colors_green_plum.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-09 06:19 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-09 06:19 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-09 06:19 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-09 06:19 css/README.md
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-09 06:19 css/style_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-09 06:19 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-09 06:19 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 06:19 pretext/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-09 06:19 pretext/pretext.cfg
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-09 06:19 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-09 06:19 pretext/module-test.py
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-09 06:19 pretext/pretext.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-09 06:19 pretext/README.md
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-09 06:19 schema/xml.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-09 06:19 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-09 06:19 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-09 06:19 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-09 06:19 schema/pretext.rnc
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-09 06:19 schema/pretext.rng
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-09 06:19 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-09 06:19 schema/build.sh
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-09 06:19 schema/pretext.xsd
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-09 06:19 schema/README.md
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-09 06:19 schema/pretext-validation-plus.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 script/mjsre/
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-09 06:19 script/mbx
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-09 06:19 script/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 06:19 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-09 06:19 script/mjsre/package.json
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-09 06:19 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-09 06:19 script/mjsre/mj-sre-page.js
+141 files, 4810372 bytes uncompressed, 1017420 bytes compressed:  78.9%
```

#### xsl/publisher-variables.xsl

##### xsl/publisher-variables.xsl

```diff
@@ -2215,14 +2215,28 @@
   </xsl:variable>
   <xsl:variable name="knowl-exercise-worksheet">
     <xsl:apply-templates select="$publisher-attribute-options/html/knowl/pi:pub-attribute[@name='exercise-worksheet']" mode="set-pubfile-variable"/>
   </xsl:variable>
   <xsl:variable name="knowl-exercise-readingquestion">
     <xsl:apply-templates select="$publisher-attribute-options/html/knowl/pi:pub-attribute[@name='exercise-readingquestion']" mode="set-pubfile-variable"/>
   </xsl:variable>
+  <!--                   -->
+  <!-- HTML Tabbed Tasks -->
+  <!--                   -->
+  <!-- Presentational choice for exercises and projects that are  -->
+  <!-- structured by task.  Value is a list of possible types,    -->
+  <!-- seen in creation of four boolean variables.  Never for the -->
+  <!-- fifth type: "exercise" inside a "worksheet".               -->
+  <xsl:variable name="html-tabbed-tasks" select="str:tokenize($publication/html/exercises/@tabbed-tasks, ' ,')"/>
+  <!-- A string is equal to a node-set (the result of tokenize()) -->
+  <!-- if it is equal to *one* child's text value.                -->
+  <xsl:variable name="b-html-tabbed-tasks-divisional" select="'divisional' = $html-tabbed-tasks"/>
+  <xsl:variable name="b-html-tabbed-tasks-inline" select="'inline' = $html-tabbed-tasks"/>
+  <xsl:variable name="b-html-tabbed-tasks-reading" select="'reading' = $html-tabbed-tasks"/>
+  <xsl:variable name="b-html-tabbed-tasks-project" select="'project' = $html-tabbed-tasks"/>
   <!--               -->
   <!-- HTML Base URL -->
   <!--               -->
   <!-- This is used to build/reference standalone pages.    -->
   <!-- Specified as a property of the HTML conversion, it   -->
   <!-- actually gets used in the LaTeX conversion to form   -->
   <!-- QR codes and make links to HTML versions of          -->
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -3915,18 +3915,31 @@
         <xsl:apply-templates select="introduction|myopenmath|conclusion">
           <xsl:with-param name="b-original" select="$b-original"/>
         </xsl:apply-templates>
       </xsl:when>
       <!-- structured by "task" so let templates for tasks work -->
       <!-- down to terminal task with SOLUTION-LIKE appendages  -->
       <xsl:when test="task">
-        <xsl:apply-templates select="introduction|task|conclusion">
-          <xsl:with-param name="b-original" select="$b-original"/>
-          <xsl:with-param name="block-type" select="$block-type"/>
-        </xsl:apply-templates>
+        <!-- An "exercise" structured by task may electively be presented  -->
+        <!-- by a "tabbed" interface from Runestone components.            -->
+        <!-- *  Never for a "worksheet" - too messy for printing           -->
+        <!-- *  Not hitting PROJECT-LIKE here, see elsewhere               -->
+        <xsl:variable name="b-tabbed-tasks" select="                 (@exercise-customization = 'divisional' and $b-html-tabbed-tasks-divisional) or                 (@exercise-customization = 'inline' and $b-html-tabbed-tasks-inline) or                 (@exercise-customization = 'reading' and $b-html-tabbed-tasks-reading)"/>
+        <xsl:choose>
+          <xsl:when test="$b-tabbed-tasks">
+            <!-- Use tabbed viewer from Runestone Components -->
+            <xsl:apply-templates select="." mode="tabbed-tasks"/>
+          </xsl:when>
+          <xsl:otherwise>
+            <xsl:apply-templates select="introduction|task|conclusion">
+              <xsl:with-param name="b-original" select="$b-original"/>
+              <xsl:with-param name="block-type" select="$block-type"/>
+            </xsl:apply-templates>
+          </xsl:otherwise>
+        </xsl:choose>
       </xsl:when>
       <!--  -->
       <!-- structured with "statement" and SOLUTION-LIKE, -->
       <!-- or just bare content for a statement           -->
       <!--  -->
       <!-- inline                                        -->
       <!-- only possibility to be knowled, so only time  -->
@@ -4021,18 +4034,31 @@
       <!-- webwork case -->
       <xsl:when test="webwork-reps">
         <xsl:apply-templates select="." mode="webwork-core">
           <xsl:with-param name="b-original" select="$b-original"/>
         </xsl:apply-templates>
       </xsl:when>
       <xsl:when test="task">
-        <xsl:apply-templates select="introduction|task|conclusion">
-          <xsl:with-param name="b-original" select="$b-original"/>
-          <xsl:with-param name="block-type" select="$block-type"/>
-        </xsl:apply-templates>
+        <!-- An "PROJECT-LIKE" structured by task may electively  -->
+        <!-- be presented by a "tabbed" interface from Runestone  -->
+        <!-- components. Note: this test is simpler than for  -->
+        <!-- "exercise" since we know we have a PROJECT-LIKE and  -->
+        <!-- do not need to consult @exercise-customization. -->
+        <xsl:choose>
+          <xsl:when test="$b-html-tabbed-tasks-project">
+            <!-- Use tabbed viewer from Runestone Components -->
+            <xsl:apply-templates select="." mode="tabbed-tasks"/>
+          </xsl:when>
+          <xsl:otherwise>
+            <xsl:apply-templates select="introduction|task|conclusion">
+              <xsl:with-param name="b-original" select="$b-original"/>
+              <xsl:with-param name="block-type" select="$block-type"/>
+            </xsl:apply-templates>
+          </xsl:otherwise>
+        </xsl:choose>
       </xsl:when>
       <xsl:otherwise>
         <xsl:apply-templates select="." mode="exercise-components">
           <xsl:with-param name="b-original" select="$b-original"/>
           <xsl:with-param name="block-type" select="$block-type"/>
           <xsl:with-param name="b-has-statement" select="true()"/>
           <xsl:with-param name="b-has-hint" select="$b-has-project-hint"/>
```

#### xsl/pretext-assembly.xsl

##### xsl/pretext-assembly.xsl

```diff
@@ -705,71 +705,74 @@
   <!-- documentation) we take care to not annotate these elements which  have -->
   <!-- no source to show.                                                     -->
   <xsl:template match="url[node()]|dataurl[node()]" mode="enrichment">
     <xsl:copy>
       <!-- we drop the @visual attribute, a decision we might revisit -->
       <xsl:apply-templates select="node()|@*[not(local-name(.) = 'visual')]" mode="enrichment"/>
     </xsl:copy>
-    <!-- manufacture a footnote with (private) attribute -->
-    <!-- as a signal to conversions as to its origin     -->
-    <xsl:choose>
-      <!-- explicitly opt-out, so no footnote -->
-      <xsl:when test="@visual = ''"/>
-      <!-- go for it, as requested by author -->
-      <xsl:when test="@visual">
-        <fn pi:url="{@visual}"/>
-      </xsl:when>
-      <xsl:otherwise>
-        <!-- When an author has not made an effort to provide a visual   -->
-        <!-- alternative, then attempt some obvious clean-up of the      -->
-        <!-- default, and if not possible, settle for an ugly visual URL -->
-        <!--                                                             -->
-        <!-- We get a candidate visual URI from the @href attribute      -->
-        <!-- link/reference/location may be external -->
-        <!-- (@href) or internal (dataurl[@source]) -->
-        <xsl:variable name="uri">
-          <xsl:choose>
-            <!-- "url" and "dataurl" both support external @href -->
-            <xsl:when test="@href">
-              <xsl:value-of select="@href"/>
-            </xsl:when>
-            <!-- a "dataurl" might be local, @source is         -->
-            <!-- indication, so prefix with a base URL,         -->
-            <!-- add "external" directory, via template useful  -->
-            <!-- also for visual URL formulation in -assembly   -->
-            <!-- N.B. we are using the base URL, since this is  -->
-            <!-- the most likely need by employing conversions. -->
-            <!-- It would eem duplicative in a conversion to    -->
-            <!-- HTML, so could perhaps be killed in that case. -->
-            <!-- But it is what we want for LaTeX, and perhaps  -->
-            <!-- for EPUB, etc.                                 -->
-            <xsl:when test="self::dataurl and @source">
-              <xsl:apply-templates select="." mode="static-url"/>
-            </xsl:when>
-            <!-- empty will be non-functional -->
-            <xsl:otherwise/>
-          </xsl:choose>
-        </xsl:variable>
-        <!-- And clean-up automatically in the prevalent cases -->
-        <xsl:variable name="truncated-href">
-          <xsl:choose>
-            <xsl:when test="substring(@href, 1, 8) = 'https://'">
-              <xsl:value-of select="substring($uri, 9)"/>
-            </xsl:when>
-            <xsl:when test="substring(@href, 1, 7) = 'http://'">
-              <xsl:value-of select="substring($uri, 8)"/>
-            </xsl:when>
-            <xsl:otherwise>
-              <xsl:value-of select="$uri"/>
-            </xsl:otherwise>
-          </xsl:choose>
-        </xsl:variable>
-        <fn pi:url="{$truncated-href}"/>
-      </xsl:otherwise>
-    </xsl:choose>
+    <!-- Now make footnote, as long as we don't create a footnote in a footnote -->
+    <xsl:if test="not(self::url and ancestor::fn)">
+      <!-- manufacture a footnote with (private) attribute -->
+      <!-- as a signal to conversions as to its origin     -->
+      <xsl:choose>
+        <!-- explicitly opt-out, so no footnote -->
+        <xsl:when test="@visual = ''"/>
+        <!-- go for it, as requested by author -->
+        <xsl:when test="@visual">
+          <fn pi:url="{@visual}"/>
+        </xsl:when>
+        <xsl:otherwise>
+          <!-- When an author has not made an effort to provide a visual   -->
+          <!-- alternative, then attempt some obvious clean-up of the      -->
+          <!-- default, and if not possible, settle for an ugly visual URL -->
+          <!--                                                             -->
+          <!-- We get a candidate visual URI from the @href attribute      -->
+          <!-- link/reference/location may be external -->
+          <!-- (@href) or internal (dataurl[@source]) -->
+          <xsl:variable name="uri">
+            <xsl:choose>
+              <!-- "url" and "dataurl" both support external @href -->
+              <xsl:when test="@href">
+                <xsl:value-of select="@href"/>
+              </xsl:when>
+              <!-- a "dataurl" might be local, @source is         -->
+              <!-- indication, so prefix with a base URL,         -->
+              <!-- add "external" directory, via template useful  -->
+              <!-- also for visual URL formulation in -assembly   -->
+              <!-- N.B. we are using the base URL, since this is  -->
+              <!-- the most likely need by employing conversions. -->
+              <!-- It would eem duplicative in a conversion to    -->
+              <!-- HTML, so could perhaps be killed in that case. -->
+              <!-- But it is what we want for LaTeX, and perhaps  -->
+              <!-- for EPUB, etc.                                 -->
+              <xsl:when test="self::dataurl and @source">
+                <xsl:apply-templates select="." mode="static-url"/>
+              </xsl:when>
+              <!-- empty will be non-functional -->
+              <xsl:otherwise/>
+            </xsl:choose>
+          </xsl:variable>
+          <!-- And clean-up automatically in the prevalent cases -->
+          <xsl:variable name="truncated-href">
+            <xsl:choose>
+              <xsl:when test="substring(@href, 1, 8) = 'https://'">
+                <xsl:value-of select="substring($uri, 9)"/>
+              </xsl:when>
+              <xsl:when test="substring(@href, 1, 7) = 'http://'">
+                <xsl:value-of select="substring($uri, 8)"/>
+              </xsl:when>
+              <xsl:otherwise>
+                <xsl:value-of select="$uri"/>
+              </xsl:otherwise>
+            </xsl:choose>
+          </xsl:variable>
+          <fn pi:url="{$truncated-href}"/>
+        </xsl:otherwise>
+      </xsl:choose>
+    </xsl:if>
   </xsl:template>
   <!-- ############# -->
   <!-- Source Repair -->
   <!-- ############# -->
   <!-- We unilaterally make various changes to an author's source -->
   <!-- so a conversion (every conversion?) can assume more        -->
   <!-- accurately that the source has certain characteristics.    -->
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -1892,14 +1892,68 @@
           </xsl:element>
         </xsl:when>
         <!-- no other source/PTX element is supported , bail out-->
         <xsl:otherwise/>
       </xsl:choose>
     </div>
   </xsl:template>
+  <!-- ############# -->
+  <!-- Tabbed Viewer -->
+  <!-- ############# -->
+  <!-- Strictly a presentational device, but useful in certain situations  -->
+  <!-- as a pedogogical device.  But we start with presentation.  An       -->
+  <!-- "exercise" or PROJECT-LIKE, structured by "task" can have each      -->
+  <!-- top-level task go into a tab, along with tabs for "introduction"    -->
+  <!-- and "conclusion".  We *never* do this for worksheets, to avoid      -->
+  <!-- gumming up printing and spacing.  And WeBWorK problems manage       -->
+  <!-- their own tasks.  The "match" here is pretty selective for          -->
+  <!-- "exercise", should perhaps be tighter for PROJECT-LIKE.  Of course, -->
+  <!-- Runestone Components play nicely with this device, along with more  -->
+  <!-- boring exercises.                                                   -->
+  <xsl:template match="exercise[task and not(@exercise-customization = 'worksheet')]|" mode="tabbed-tasks">
+    <div class="ptx-runestone-container">
+      <div class="runestone">
+        <div data-component="tabbedStuff">
+          <xsl:apply-templates select="." mode="runestone-id-attribute"/>
+          <xsl:if test="introduction">
+            <xsl:variable name="the-intro">
+              <xsl:apply-templates select="." mode="type-name">
+                <xsl:with-param name="string-id" select="'introduction'"/>
+              </xsl:apply-templates>
+            </xsl:variable>
+            <div data-component="tab" data-tabname="{$the-intro}">
+              <xsl:apply-templates select="introduction"/>
+            </div>
+          </xsl:if>
+          <!--  -->
+          <xsl:for-each select="task">
+            <xsl:variable name="the-task-number">
+              <xsl:text>(</xsl:text>
+              <xsl:apply-templates select="." mode="serial-number"/>
+              <xsl:text>)</xsl:text>
+            </xsl:variable>
+            <div data-component="tab" data-tabname="{$the-task-number}">
+              <xsl:apply-templates select="."/>
+            </div>
+          </xsl:for-each>
+          <!--  -->
+          <xsl:if test="conclusion">
+            <xsl:variable name="the-outro">
+              <xsl:apply-templates select="." mode="type-name">
+                <xsl:with-param name="string-id" select="'conclusion'"/>
+              </xsl:apply-templates>
+            </xsl:variable>
+            <div data-component="tab" data-tabname="{$the-outro}">
+              <xsl:apply-templates select="conclusion"/>
+            </div>
+          </xsl:if>
+        </div>
+      </div>
+    </div>
+  </xsl:template>
   <!-- ######### -->
   <!-- Utilities -->
   <!-- ######### -->
   <!-- Runestone components, such as data files and select questions,  -->
   <!-- frequently point to other Runestone components in the database. -->
   <!--   * Authors point in their source with @xml:id                  -->
   <!--     values in a space- or comma- separated list                 -->
```

### Comparing `pretext-1.6.1.dev20230608/pretext/generate.py` & `pretext-1.6.1.dev20230609/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/project.py` & `pretext-1.6.1.dev20230609/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230609/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230609/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230609/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160064 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-08 06:22 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-08 06:22 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-08 06:22 project.ptx
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-08 06:21 README.md
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-08 06:21 assets/frog.jpg
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-08 06:21 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-08 06:21 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-08 06:21 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-08 06:21 source/section-2.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-08 06:22 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-09 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-09 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-09 06:19 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-09 06:18 README.md
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-09 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-09 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-09 06:18 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-09 06:18 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-09 06:18 source/section-2.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-09 06:19 .devcontainer/devcontainer.json
 14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
```

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230609/pretext/templates/resources/book.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7570 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-08 06:22 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-08 06:22 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-08 06:22 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-08 06:21 README.md
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-08 06:21 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-08 06:21 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-08 06:22 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-09 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-09 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-09 06:19 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-09 06:18 README.md
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-09 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-09 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-09 06:19 .devcontainer/devcontainer.json
 10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230609/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173263 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-08 06:22 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-08 06:22 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-08 06:22 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-08 06:21 README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-08 06:21 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-08 06:21 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-08 06:21 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 source/images/
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-08 06:21 source/sec-features.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-08 06:21 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-08 06:21 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-08 06:21 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-08 06:21 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-08 06:21 source/main.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-08 06:21 source/ch-generate.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-08 06:21 source/backmatter.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-08 06:21 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-08 06:21 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-08 06:21 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-08 06:21 source/ch-features.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-08 06:21 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-08 06:21 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-08 06:21 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-08 06:21 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-08 06:21 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-08 06:21 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-08 06:21 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-08 06:21 source/images/cflag.asy
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-08 06:22 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-09 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-09 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-09 06:19 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-09 06:18 README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-09 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-09 06:18 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-09 06:18 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 source/images/
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-09 06:18 source/sec-features.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-09 06:18 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-09 06:18 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-09 06:18 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-09 06:18 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-09 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-09 06:18 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-09 06:18 source/backmatter.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-09 06:18 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-09 06:18 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-09 06:18 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-09 06:18 source/ch-features.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-09 06:18 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-09 06:18 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-09 06:18 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-09 06:18 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-09 06:18 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-09 06:18 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-09 06:18 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-09 06:18 source/images/cflag.asy
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-09 06:19 .devcontainer/devcontainer.json
 34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230609/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230609/pretext/templates/resources/hello.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4611 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-08 06:22 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-08 06:22 codechat_config.yaml
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-08 06:21 project.ptx
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-08 06:21 README.md
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-08 06:21 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-08 06:21 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-08 06:22 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-09 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-09 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-09 06:18 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-09 06:18 README.md
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-09 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-09 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-09 06:19 .devcontainer/devcontainer.json
 10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
```

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230609/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230609/pretext/templates/resources/slideshow.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8346 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:22 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-08 06:21 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-08 06:22 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-08 06:22 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-08 06:21 project.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-08 06:21 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-08 06:21 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-08 06:21 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-08 06:22 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 06:18 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-09 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-09 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-09 06:18 project.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-09 06:18 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-09 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-09 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-09 06:19 .devcontainer/devcontainer.json
 11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230608/pretext/utils.py` & `pretext-1.6.1.dev20230609/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230608/pyproject.toml` & `pretext-1.6.1.dev20230609/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230608"
+version = "1.6.1.dev20230609"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230608/PKG-INFO` & `pretext-1.6.1.dev20230609/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230608
+Version: 1.6.1.dev20230609
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

