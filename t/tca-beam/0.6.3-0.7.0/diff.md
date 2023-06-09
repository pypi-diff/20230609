# Comparing `tmp/tca_beam-0.6.3.tar.gz` & `tmp/tca_beam-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tca_beam-0.6.3.tar", max compression
+gzip compressed data, was "tca_beam-0.7.0.tar", max compression
```

## Comparing `tca_beam-0.6.3.tar` & `tca_beam-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.6.3/README.md
--rw-r--r--   0        0        0      467 2023-06-08 20:48:33.893211 tca_beam-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      173 2023-06-08 15:05:54.275604 tca_beam-0.6.3/tca_beam/__init__.py
--rw-r--r--   0        0        0     2310 2023-06-08 19:47:14.919545 tca_beam-0.6.3/tca_beam/config.py
--rw-r--r--   0        0        0      391 2023-06-08 19:32:23.316107 tca_beam-0.6.3/tca_beam/helpers.py
--rw-r--r--   0        0        0     3417 2023-06-08 20:45:36.192946 tca_beam-0.6.3/tca_beam/run.py
--rw-r--r--   0        0        0     2393 2023-06-08 20:35:35.090566 tca_beam-0.6.3/tca_beam/settings.py
--rw-r--r--   0        0        0     3404 2023-06-08 19:20:03.772655 tca_beam-0.6.3/tca_beam/tca_beam.py
--rw-r--r--   0        0        0     1618 2023-06-08 19:32:34.191285 tca_beam-0.6.3/tca_beam/template_rendering.py
--rw-r--r--   0        0        0      285 2023-06-08 20:48:19.000000 tca_beam-0.6.3/tca_beam/templates/.beam-settings.toml
--rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.6.3/tca_beam/templates/AllPreviews.swift
--rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.6.3/tca_beam/templates/OneFile.swift
--rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.6.3/tca_beam/templates/TwoFile_ReducerPart.swift
--rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.6.3/tca_beam/templates/TwoFile_ViewPart.swift
--rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.6.3/tca_beam/templates/View.swift
--rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.6.3/tca_beam/templates/ViewFeature.swift
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.6.3/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.7.0/README.md
+-rw-r--r--   0        0        0      467 2023-06-09 10:22:48.802718 tca_beam-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      173 2023-06-08 15:05:54.275604 tca_beam-0.7.0/tca_beam/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-09 09:30:00.770572 tca_beam-0.7.0/tca_beam/config.py
+-rw-r--r--   0        0        0      391 2023-06-08 19:32:23.316107 tca_beam-0.7.0/tca_beam/helpers.py
+-rw-r--r--   0        0        0     5003 2023-06-09 10:23:16.388535 tca_beam-0.7.0/tca_beam/run.py
+-rw-r--r--   0        0        0     2393 2023-06-08 20:35:35.090566 tca_beam-0.7.0/tca_beam/settings.py
+-rw-r--r--   0        0        0     3654 2023-06-09 09:30:00.847921 tca_beam-0.7.0/tca_beam/tca_beam.py
+-rw-r--r--   0        0        0     1618 2023-06-08 19:32:34.191285 tca_beam-0.7.0/tca_beam/template_rendering.py
+-rw-r--r--   0        0        0      285 2023-06-09 06:43:44.049680 tca_beam-0.7.0/tca_beam/templates/.beam-settings.toml
+-rw-r--r--   0        0        0      630 2023-06-09 09:59:36.113175 tca_beam-0.7.0/tca_beam/templates/AllPreviews.swift
+-rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.7.0/tca_beam/templates/OneFile.swift
+-rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.7.0/tca_beam/templates/TwoFile_ReducerPart.swift
+-rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.7.0/tca_beam/templates/TwoFile_ViewPart.swift
+-rw-r--r--   0        0        0     1031 2023-06-09 09:30:00.841537 tca_beam-0.7.0/tca_beam/templates/View.swift
+-rw-r--r--   0        0        0     1996 2023-06-09 09:30:00.845043 tca_beam-0.7.0/tca_beam/templates/ViewFeature.swift
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.7.0/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.7.0/PKG-INFO
```

### Comparing `tca_beam-0.6.3/tca_beam/config.py` & `tca_beam-0.7.0/tca_beam/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,11 +63,12 @@
     permanent_settings: PermanentSettings
     script_dir: str
     target_dir: str
     jinja_env: Environment
     two_files: bool
     sub_dirs: bool
     preview_all: bool
+    make_hor: bool
     output_dir: str
     force_overwrite: bool
     dry_run: bool
     feature_names: [str]
```

### Comparing `tca_beam-0.6.3/tca_beam/settings.py` & `tca_beam-0.7.0/tca_beam/settings.py`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.3/tca_beam/tca_beam.py` & `tca_beam-0.7.0/tca_beam/tca_beam.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,44 +9,46 @@
 try:
     from tca_beam import __version__
     beam_version = __version__
 except ImportError:
     pass
 
 # TODO:
-# [x] try trogon/textualize on tca-beam -- see results in my main TW -- might have to make explicit tca-beam 'make' command
-# -[x] upload to main pyPi
+# -[ ] add --suppress-views (implies two-files style but only makes the reducers)
 # -[ ] make bbtests
+# -[x] try trogon/textualize on tca-beam -- see results in my main TW -- might have to make explicit tca-beam 'make' command
+# -[x] upload to main pyPi
 # -[x] option for preview-all
 # -[x] impl two files
 # -[x] flags for 'features in sub_dirs'
 # -[x] make script use abs path to the templates, no chdir!
 # -[x] --dry-run
-
 # For docs:
 #  tca-beam won't complain if the output_dir already exists, regardless of force_overwrite flag (which only applies to files).
 #
 
+
 # When you're testing and playing with beam, it might be tempting to set up a host xcode project with a _link_ to a folder
 # where you are generating the files with beam.
 # However, Xcode however won't add these files to any target (it's how linked folders work), so you're probably better off
 # just adding a folder group to your project (in the usual way) after you've generated the files with beam.
 
 
 @click.command(no_args_is_help=True)
 @click.option('--two-files', is_flag=True, help="Put view and reducer into separate files")
 @click.option('--sub-dirs', is_flag=True, help="Put each feature in a sub-directory")
 @click.option('--preview-all', is_flag=True, help="Generate a single View that previews all feature Views")
+@click.option('--make-hor', is_flag=True, help="Make first feature name a higher order reducer that scopes in the remaining ones as sub-reducers")
 @click.option('--output-dir', default='.', help="Output directory (defaults to current dir)")
 @click.option('--force-overwrite', is_flag=True, help="Force overwriting any existing files")
 @click.option('--dry-run', is_flag=True, help="Don't generate files, just preview any actions")
 @click.option('--customise-settings', is_flag=True, help="Generate a user-editable file to tweak file naming settings.")
 @click.option('--version', is_flag=True, help="Print version and exit")
 @click.argument('feature_names', nargs=-1)
-def start(two_files, sub_dirs, preview_all, output_dir, force_overwrite, dry_run, customise_settings, version, feature_names):
+def start(two_files, sub_dirs, preview_all, make_hor, output_dir, force_overwrite, dry_run, customise_settings, version, feature_names):
 
     if customise_settings:
         personalize_permanent_settings()
         sys.exit(0)
 
     permanent_settings = load_permanent_settings()
     dbg(f"Settings: {permanent_settings}")
@@ -58,15 +60,15 @@
     script_dir = os.path.abspath(os.path.dirname(__file__))
 
     templates_path = make_abs_path('templates')
     file_loader = FileSystemLoader(templates_path)
     jinja_env = Environment(loader=file_loader)
 
     config = BeamConfig(PermanentSettings(permanent_settings), script_dir, output_dir, jinja_env, two_files, sub_dirs, preview_all,
-                        output_dir, force_overwrite, dry_run, feature_names)
+                        make_hor, output_dir, force_overwrite, dry_run, feature_names)
 
     if len(feature_names) < 1:
         p()
         p("Please give one or more feature name arguments (after any option flags).")
         p()
 
         echo = click.echo
```

### Comparing `tca_beam-0.6.3/tca_beam/template_rendering.py` & `tca_beam-0.7.0/tca_beam/template_rendering.py`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.3/tca_beam/templates/AllPreviews.swift` & `tca_beam-0.7.0/tca_beam/templates/AllPreviews.swift`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 // MARK: - Preview all feature Views in a VStack
 
 public struct AllPreviews_Preview: PreviewProvider {
 
     public static var previews: some View {
         VStack {
             Spacer()
-{% for feature in allFeatures %}
+{%- for feature in allFeatures %}
             {{ feature.viewName }}(store: StoreOf<{{ feature.featureName }}>(
                 initialState: .init()) {
                     {{ feature.featureName }}()
                 }
 //                 withDependencies: {
 //                     $0.someDependency = something
 //                 }
             )
             Spacer()
-{% endfor %}
+{%- endfor %}
        }
     }
 }
```

### Comparing `tca_beam-0.6.3/setup.py` & `tca_beam-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tca-beam = tca_beam.tca_beam:start']}
 
 setup_kwargs = {
     'name': 'tca-beam',
-    'version': '0.6.3',
+    'version': '0.7.0',
     'description': 'Feature stub generation for The Composable Architecture',
     'long_description': 'TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.\n\nhttps://github.com/alexhunsley/tca-beam\n\n',
     'author': 'Alex Hunsley',
     'author_email': 'alex.hunsley@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tca_beam-0.6.3/PKG-INFO` & `tca_beam-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tca-beam
-Version: 0.6.3
+Version: 0.7.0
 Summary: Feature stub generation for The Composable Architecture
 Author: Alex Hunsley
 Author-email: alex.hunsley@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

