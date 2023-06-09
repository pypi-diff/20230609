# Comparing `tmp/pyved-0.0.5.tar.gz` & `tmp/pyved-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-0.0.5.tar", last modified: Mon May  1 19:29:00 2023, max compression
+gzip compressed data, was "pyved-0.0.6.tar", last modified: Fri Jun  9 10:12:29 2023, max compression
```

## Comparing `pyved-0.0.5.tar` & `pyved-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.052037 pyved-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-01 19:28:48.000000 pyved-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-01 19:29:00.052037 pyved-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-01 19:28:48.000000 pyved-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:29:00.052037 pyved-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-01 19:28:48.000000 pyved-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.048037 pyved-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.052037 pyved-0.0.5/src/pyved/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/menu_bar_ev_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/menu_bar_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/test.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/ver_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.052037 pyved-0.0.5/src/pyved.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.480497 pyved-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-09 10:12:15.000000 pyved-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-09 10:12:29.476497 pyved-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-09 10:12:15.000000 pyved-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:12:29.480497 pyved-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-09 10:12:15.000000 pyved-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.476497 pyved-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.476497 pyved-0.0.6/src/pyved/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/_ecs_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/menu_bar_ev_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/menu_bar_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-09 10:12:15.000000 pyved-0.0.6/src/pyved/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:12:29.476497 pyved-0.0.6/src/pyved.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 10:12:29.000000 pyved-0.0.6/src/pyved.egg-info/top_level.txt
```

### Comparing `pyved-0.0.5/LICENSE` & `pyved-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyved-0.0.5/src/pyved/__main__.py` & `pyved-0.0.6/src/pyved/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,101 +1,104 @@
 import argparse
-from pathlib import Path
 import os
-from .ver_info import version_num as pyved_ver_num
+from pathlib import Path
+from . import utils
 
 
 parser = argparse.ArgumentParser(
     prog='pyved',
     description='runs PYVED and opens a new/existing project',
-    epilog="pyved (=PY Visual Editor) is a new toolbox for easy game development. For more information, please visit https://github.com/wktab/gamedev-pyved/"
+    epilog="pyved (=PY Visual Editor) is a new toolbox for easy game development. For more information, please visit "
+           "https://github.com/wktab/gamedev-pyved/"
 )
 # configuration --
 # besoin d'utiliser des sub parsers car on a plusieurs cmd
 subparser = parser.add_subparsers(dest='command', required=True)
 new = subparser.add_parser('new')
-new.add_argument('project', type=str)#, required=True)
-
+new.add_argument('project', type=str)  # , required=True)
 register = subparser.add_parser('open')
-register.add_argument('filepath', type=str)#, required=True)
-
+register.add_argument('filepath', type=str)  # , required=True)
 cmd = subparser.add_parser('version')
 # -- fin configuration
 
 
 # definition implem {{
-def create_new_project(pname):
+def create_new_project(pname, tool_ver):
     target_dir = Path(pname)
     if target_dir.exists():
         print(f"ERROR: folder {target_dir} already exists")
     else:
         os.mkdir(target_dir)
         print(f" +Initializing a new project named \"{target_dir}\"...")
         DB_QT = '"'
         with open(os.path.join(target_dir, 'pyved.json'), 'w') as fout:
             fout.write("{\n")
-            fout.write(' '*4 + '"tag":'+DB_QT+'pyved'+pyved_ver_num+DB_QT+",\n")
-            fout.write(' '*4 + '"project":'+DB_QT+pname+DB_QT+",\n")
+            fout.write(' ' * 4 + '"tag":' + DB_QT + 'pyved' + tool_ver + DB_QT + ",\n")
+            fout.write(' ' * 4 + '"project":' + DB_QT + pname + DB_QT + ",\n")
             fout.write("}")
 
         # main source-code file
         with open(os.path.join(target_dir, 'main.py'), 'w') as fout:
             fout.write("import katagames_engine as kengi")
             fout.write("\n")
             fout.write("kengi.init()")
 
 
 def open_project(desc_ptr, dirname):
-    print('*'*32)
+    print('*' * 32)
     print(' Welcome to PYVED')
-    print('*'*32)
+    print('*' * 32)
 
     print()
     print(desc_ptr.read())
     print('---')
 
     print('Listing files:')
-    
+
     t_dir = Path(dirname)
     has_main = False
     for entry in t_dir.iterdir():
         print(entry.name)
         if 'main.py' == entry.name:
             has_main = True
     if not has_main:
         raise Exception('invalid project format! main.py not found in the project folder')
 
     # ouverture projet avec format valide ds l'editor
     from . import editor
     editor.target_dir = dirname
     editor.target_file = 'main.py'
     editor.run_editor()
+
+
 # }} definition implem
 
 
 # ------
 #  main chunk of code
 # -----
 def main():
+    # tool_version = pyved.__version__
+    tool_ver = utils.get_version()
+
     args = parser.parse_args()
     if args.command == 'new':
-        create_new_project(args.project)
+        create_new_project(args.project, tool_ver)
 
     elif args.command == 'open':
         filepath = os.path.abspath(args.filepath)
         dirname = os.path.dirname(filepath)
         if not os.path.isfile(os.path.join(dirname, filepath)):
             print(f"ERROR: cannot read the file {filepath}, please provide a valid pyved.json FILE")
         else:
             fptr = open(filepath, 'r')
             open_project(fptr, dirname)
             fptr.close()
 
     elif args.command == 'version':
-        print(f"PYVED - version {pyved_ver_num}")
-
+        print(f"PYVED - version {tool_ver}")
     else:
         print(f"ERROR: command {args.command} is not a valid command!")
 
 
-if __name__=='__main__':
+if __name__ == '__main__':
     main()
```

### Comparing `pyved-0.0.5/src/pyved/editor.py` & `pyved-0.0.6/src/pyved/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # from pygame_gui.ui_manager import UIManager
 # from pygame_gui.elements.ui_window import UIWindow
 from pygame_gui.elements.ui_image import UIImage
 from pygame_gui import UIManager, UI_TEXT_ENTRY_CHANGED
 from pygame_gui.elements import UIWindow, UITextEntryBox, UITextBox
 from .menu_bar_gui import UIMenuBar, menu_data
+
 from . import menu_bar_ev_handler
 
 from .pong.pong import PongGame
 import os  # so i can open file to read src code!
 import pathlib
 
 PONG_WINDOW_SELECTED = pygame.event.custom_type()
@@ -72,20 +73,20 @@
 def gen_edition_title(file, project_name):
     return file+f"({project_name}) source-code"
 
 
 class MiniGamesApp:
     def __init__(self):
         pygame.init()
-
+        pygame.display.set_caption('Pyved: game creation toolbox')
         self.root_window_surface = pygame.display.set_mode((APP_W, APP_H))
 
         self.background_surface = pygame.Surface((APP_W, APP_H)).convert()
         self.background_surface.fill(pygame.Color('#505050'))
-        self.ui_manager = UIManager((APP_W, APP_H), 'data/ui_theme.json')
+        self.ui_manager = UIManager((APP_W, APP_H), os.path.join(os.path.dirname(__file__),'gui-rel-data/ui_theme.json'))
         self.clock = pygame.time.Clock()
         self.is_running = True
 
         self.pong_window_1 = GamePreview(
             'Pong demo',
             POS_PREVIEW,
             self.ui_manager
@@ -96,15 +97,15 @@
         # --------- text edition related stuff -------------
         if target_dir is not None:
             path = pathlib.PurePath(target_dir)
             pure_dir = path.name
         else:
             pure_dir = '??'
         self.notepad_window = UIWindow(pygame.Rect(50, 20, 380, 400), window_display_title=gen_edition_title(target_file, pure_dir))
-        output_window = UIWindow(pygame.Rect(440, 20, 380, 400), window_display_title="Pygame GUI Formatted Text")
+        output_window = UIWindow(pygame.Rect(440, 20, 380, 400), window_display_title="Score")
 
         self.text_entry_box = UITextEntryBox(  # swap to editable text box
                 relative_rect=pygame.Rect((0, 0), self.notepad_window.get_container().get_size()),
                 initial_text="",
                 container=self.notepad_window)
 
         self.text_output_box = UITextBox(
```

### Comparing `pyved-0.0.5/src/pyved/menu_bar_ev_handler.py` & `pyved-0.0.6/src/pyved/menu_bar_ev_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 from pathlib import Path
 
 import pygame
 
 from pygame_gui.windows import UIFileDialog, UIMessageWindow
 from pygame_gui import UI_BUTTON_START_PRESS, UI_WINDOW_MOVED_TO_FRONT, UI_WINDOW_CLOSE
 from pygame_gui import UI_FILE_DIALOG_PATH_PICKED
-from .ver_info import version_num as pyved_ver_num
+
+from . import utils
+
+
+
 # from ui.ui_canvas_window import CanvasWindow
 # from ui.ui_new_canvas_dialog import UINewCanvasDialog
 # from tools.undo_record import UndoRecord
 
 ABOUT_MSG = '<b>Pyved for Game Development</b><br>'\
             '********<br>' \
             '<b>Authors: </b>moonb3ndr et al.<br>' \
-            f"<b>Version: </b>{pyved_ver_num}<br>"\
+            f"<b>Version: </b>{utils.get_version()}<br>"\
             '<b>License: </b>Gnu LGPL v3.0<br>'
 
 
 class MenuBarEventHandler:
     def __init__(self, window_surface, ui_manger):
 
         self.window_surface = window_surface
```

### Comparing `pyved-0.0.5/src/pyved/menu_bar_gui.py` & `pyved-0.0.6/src/pyved/menu_bar_gui.py`

 * *Files identical despite different names*

