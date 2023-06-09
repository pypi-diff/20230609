# Comparing `tmp/metalo-0.5.1.tar.gz` & `tmp/metalo-0.5.2.tar.gz`

## Comparing `metalo-0.5.1.tar` & `metalo-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 metalo-0.5.1/metalo/__init__.py
--rwxr-xr-x   0        0        0    11679 2020-02-02 00:00:00.000000 metalo-0.5.1/metalo/metalo.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 metalo-0.5.1/.gitignore
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 metalo-0.5.1/.hgignore -> .dotfiles/hg/.hgignore
--rw-r--r--   0        0        0    32473 2020-02-02 00:00:00.000000 metalo-0.5.1/LICENSE
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 metalo-0.5.1/README.rst
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 metalo-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 metalo-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 metalo-0.5.2/metalo/__init__.py
+-rwxr-xr-x   0        0        0    11679 2020-02-02 00:00:00.000000 metalo-0.5.2/metalo/metalo.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 metalo-0.5.2/.gitignore
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 metalo-0.5.2/.hgignore -> .dotfiles/hg/.hgignore
+-rw-r--r--   0        0        0    32473 2020-02-02 00:00:00.000000 metalo-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 metalo-0.5.2/README.rst
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 metalo-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 metalo-0.5.2/PKG-INFO
```

### Comparing `metalo-0.5.1/metalo/__init__.py` & `metalo-0.5.2/metalo/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-version = "0.5.1"
+version = "0.5.2"
```

### Comparing `metalo-0.5.1/metalo/metalo.py` & `metalo-0.5.2/metalo/metalo.py`

 * *Files identical despite different names*

### Comparing `metalo-0.5.1/LICENSE` & `metalo-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metalo-0.5.1/README.rst` & `metalo-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `metalo-0.5.1/pyproject.toml` & `metalo-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metalo-0.5.1/PKG-INFO` & `metalo-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalo
-Version: 0.5.1
+Version: 0.5.2
 Summary: Metabolic analysis of Logical models extracted from maps
 Project-URL: Code, https://gitlab.inria.fr/soliman/metalo
 Author-email: Sahar Aghakhani <Sahar.Aghakhani@inria.fr>, Sylvain Soliman <Sylvain.Soliman@inria.fr>
 License-Expression: GPL-3.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

