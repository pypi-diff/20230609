# Comparing `tmp/coge-0.1.8-py2.py3-none-any.whl.zip` & `tmp/coge-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11159 bytes, number of entries: 15
--rw-r--r--  2.0 unx      143 b- defN 21-Aug-24 17:59 coge/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 21-Aug-24 17:59 coge/__main__.py
--rw-r--r--  2.0 unx    11862 b- defN 22-Nov-21 06:42 coge/coge.py
--rw-r--r--  2.0 unx       36 b- defN 21-Aug-30 04:34 coge/binaryornot/__init__.py
--rw-r--r--  2.0 unx     1335 b- defN 21-Aug-30 04:32 coge/binaryornot/check.py
--rw-r--r--  2.0 unx     4814 b- defN 21-Aug-30 04:32 coge/binaryornot/helpers.py
--rw-r--r--  2.0 unx      101 b- defN 21-Aug-24 17:59 coge/logx/__init__.py
--rw-r--r--  2.0 unx      750 b- defN 21-Aug-24 17:59 coge/logx/colored_handler.py
--rw-r--r--  2.0 unx      641 b- defN 21-Aug-30 05:27 coge/logx/logging.yaml
--rw-r--r--  2.0 unx      851 b- defN 21-Aug-24 17:59 coge/logx/setup_logging.py
--rw-r--r--  2.0 unx     3168 b- defN 22-Nov-21 14:08 coge-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Nov-21 14:08 coge-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 22-Nov-21 14:08 coge-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 22-Nov-21 14:08 coge-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1161 b- defN 22-Nov-21 14:08 coge-0.1.8.dist-info/RECORD
-15 files, 25096 bytes uncompressed, 9249 bytes compressed:  63.1%
+Zip file size: 11664 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 03:58 coge/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 22-Feb-10 04:53 coge/__main__.py
+-rw-r--r--  2.0 unx    13172 b- defN 23-Jun-09 10:49 coge/coge.py
+-rw-r--r--  2.0 unx       36 b- defN 22-Feb-10 04:53 coge/binaryornot/__init__.py
+-rw-r--r--  2.0 unx     1335 b- defN 22-Feb-10 04:53 coge/binaryornot/check.py
+-rw-r--r--  2.0 unx     4814 b- defN 22-Feb-10 04:53 coge/binaryornot/helpers.py
+-rw-r--r--  2.0 unx      101 b- defN 22-Feb-10 04:53 coge/logx/__init__.py
+-rw-r--r--  2.0 unx      750 b- defN 22-Feb-10 04:53 coge/logx/colored_handler.py
+-rw-r--r--  2.0 unx      641 b- defN 22-Feb-10 04:53 coge/logx/logging.yaml
+-rw-r--r--  2.0 unx      851 b- defN 22-Feb-10 04:53 coge/logx/setup_logging.py
+-rw-r--r--  2.0 unx     3767 b- defN 23-Jun-09 10:49 coge-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-09 10:49 coge-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-09 10:49 coge-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-09 10:49 coge-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1161 b- defN 23-Jun-09 10:49 coge-0.1.9.dist-info/RECORD
+15 files, 27008 bytes uncompressed, 9754 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: coge/logx/logging.yaml
 Comment: 
 
 Filename: coge/logx/setup_logging.py
 Comment: 
 
-Filename: coge-0.1.8.dist-info/METADATA
+Filename: coge-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: coge-0.1.8.dist-info/WHEEL
+Filename: coge-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: coge-0.1.8.dist-info/entry_points.txt
+Filename: coge-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: coge-0.1.8.dist-info/top_level.txt
+Filename: coge-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: coge-0.1.8.dist-info/RECORD
+Filename: coge-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coge/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .coge import (entry_point,
                      main,
-                     createParse)
+                     create_parser)
 
 
-__all__ = ['entry_point','createParse', 'main']
+__all__ = ['entry_point','create_parser', 'main']
```

## coge/coge.py

```diff
@@ -4,42 +4,47 @@
 
 # don`t remove this line
 import logging
 setup_logging()
 logger = logging.getLogger(__name__)
 
 import argparse
-import sys
 import os
 from os.path import join, isfile,basename
 from pathlib import Path
 from distutils.dir_util import copy_tree
 import re
 import subprocess
 import shutil
 
+COGE_CONFIG_FILE = ".coge.json"
+COGE_HISTORY_FILE = ".coge.history"
+
 common_ignore=[".DS_Store",'.pyc',".o",".obj",".class","Pods"]
 
-def isGitFolder(src):
+def is_git_folder(src):
     try:
-        subprocess.check_output(f"cd {src}  && git status ", shell=True).splitlines()
+        if not os.path.isfile(src):
+            subprocess.check_output(f"cd {src}  && git status ", shell=True).splitlines()
+        else:
+            return False
     except Exception as e:
         return False
     return True
 
 # this command will respect .gitignore
-def isGitFolderClean(src):
+def is_git_folder_clean(src):
     list_of_files =[]
     try:
         list_of_files = subprocess.check_output(f"cd {src}  && git status -s", shell=True).splitlines()
     except Exception as e:
         pass
     return len(list_of_files) == 0
 
-def gitLsFiles(src):
+def git_ls_files(src):
     before_script=join(src,".coge.before.py")
     list_of_files = subprocess.check_output(f"cd {src}  && git ls-files", shell=True).splitlines()
     return list_of_files
 
 def before_copy(src,dest):
     before_py_script=join(src,".coge.before.py")
     if os.path.isfile(before_py_script):
@@ -63,22 +68,18 @@
     after_sh_script=join(src,".coge.after.sh")
     if os.path.isfile(after_sh_script):
         logger.warning(f'----------------.coge.after.sh----------------------')
         subprocess.Popen(["bash" ,after_sh_script],cwd=dest).communicate()
         logger.warning(f'-----------------------------------------------------')
 
 def copying(src,dest):
-    if isGitFolder(src):
-        #  if not allow_git_dirty and not isGitFolderClean(src):
+    print(src,dest)
+    if is_git_folder(src):
         logger.critical(f"if {src} is not clean, commit your changes or git reset. or it will ignore the file changes")
-        #      sys.exit(0);
-
-
-        gitfiles = gitLsFiles(src)
-
+        gitfiles = git_ls_files(src)
         logger.info(f'{src} is git repo')
 
         if len(gitfiles)==0:
             logger.warning(f'maybe you should commit your chagnes if you use -w, Nothing found with git ls-files in {src}')
         for f in gitfiles:
             try:
                 f = f.decode('utf8')
@@ -91,39 +92,41 @@
             isbreak= False
             for ci in common_ignore:
                 if f.endswith(ci):
                     isbreak = True
                     break
             if isbreak:
                 continue
-            
 
             try:
                 shutil.copy(join(src,f), join(dest,f),follow_symlinks=False)
                 logger.info("coge --> "+join(dest,f))
             except Exception as e:
                 logger.error("coge --> "+join(dest,f))
                 pass
     else:
         logger.critical("Not a git repo,full copy!")
-        copy_tree(src, dest)
-        logger.warning(f'copy done -------------------------------------------')
+        if os.path.isfile(src):
+            shutil.copyfile(src,dest)
+        else:
+            copy_tree(src, dest)
+            logger.warning(f'copy done -------------------------------------------')
 
 
-def replaceWithCase(content,before,after):
+def replace_with_case(content,before,after):
     regex = re.compile(re.escape(before), re.I)
     partial= regex.sub(lambda x: ''.join(d.upper() if c.isupper() else d.lower()
         for c,d in zip(x.group()+after[len(x.group()):], after)), content)
     return partial
 
-def fullReplace(root,oldKey,newKey):
+def full_repalcement(code_template_folder,oldKey,newKey):
     if oldKey == newKey or len(newKey)==0:
         return
 
-    for dname, dirs, files in os.walk(root,topdown=False):
+    for dname, dirs, files in os.walk(code_template_folder,topdown=False):
         dirs[:] = [d for d in dirs if not d == '.git']
         for filename in files:
 
             # this is evil file from MAC
             isbreak= False
             for ci in common_ignore:
                 if filename.endswith(ci):
@@ -131,195 +134,230 @@
                     break
 
             if isbreak:
                 continue
 
             oldfile = join(dname,filename)
             if is_binary(oldfile):
-                logger.critical(oldfile + " is binary!")
+                logger.info(oldfile + " is binary!")
                 continue
 
             contents = ""
             try:
                 contents = str(Path(oldfile).read_text())
             except Exception as e:
                 print(f"{oldfile} error: pass", e)
                 continue
 
-            contents = replaceWithCase(contents,oldKey,newKey)
+            contents = replace_with_case(contents,oldKey,newKey)
             with open(oldfile,"w") as f:
                 f.write(contents)
 
             if isfile(oldfile):
                 if oldKey.upper() in filename.upper():
-                    newfile = join(dname,replaceWithCase(filename,oldKey,newKey))
+                    newfile = join(dname,replace_with_case(filename,oldKey,newKey))
                     os.rename(oldfile,newfile)
 
         #  rename folder
-        if oldKey.lower() in basename(dname).lower() and (dname != root):
-            destfolder = join(Path(dname).parent,replaceWithCase(basename(dname),oldKey,newKey))
+        if oldKey.lower() in basename(dname).lower() and (dname != code_template_folder):
+            destfolder = join(Path(dname).parent,replace_with_case(basename(dname),oldKey,newKey))
             os.rename(dname,destfolder)
 
-def main(root,args):
-    keypairs={}
-    prefix = args.arg_prefix or "COGE_ARG_"
+def get_coge_config(code_template_folder):
+    # Check if the file exists
+    target = join(code_template_folder,COGE_CONFIG_FILE)
+    if os.path.isfile(target):
+        print("The file exists.")
+        import json
+        with open(target) as file:
+            # Load the contents of the file
+            data = json.load(file)
+            return data
+    else:
+        return []
 
-    idx = 0
+def main(args):
+    code_template_folder = get_code_template_folder()
+    targets = code_template_folder
+    keypairs={}
 
-    target_foldername = "app"
+    target_name = "app"
     for m in args.magic:
-        if ":" not in m:
-            root = join(root,m)
+        if "." == m:
+            pass
+        elif ":" not in m:
+            print("m",m)
+            targets = join(targets,m)
+            if os.path.isfile(targets):
+                target_name = m
         else:
             ms = m.split(":")
             key = ms[0]
             val = ms[1]
             if key == val:
                 print(f"keypair: {key}:{val} must not be the same!")
-                return 
+                return
             if key=="@":
-                target_foldername=val
+                target_name=val
                 continue
-            if len(key.strip()) == 0:
-                key = prefix +str(idx)
-                idx+=1
             keypairs[key] = val
 
+    coge_config =  get_coge_config(targets)
+    for o in coge_config:
+        key  = o
+        desc = ""
+        if type(o) == dict:
+            key = o["key"]
+            desc = o["desc"]
+        if key not in keypairs:
+            if type(key) == str:
+                v = input(f'Need key [{key}]: ')
+                keypairs[key] = v
+            else:
+                v = input(f'Need key [{key}], {desc}: ')
+                keypairs[key] = v
+
+
     if args.cmd or len(args.magic)==0:
-        listCmd(root,args.depth)
-        return 
+        list_commands(targets,args.depth)
+        return
 
     if args.list or len(args.magic)==0:
-        listTarget(root,args.depth)
-        return 
+        list_target(targets,args.depth)
+        return
 
     cwd = os.getcwd()
-    dest = join(cwd,target_foldername)
+    dest = join(cwd,target_name)
     if os.path.isdir(dest):
         logger.critical(f"{dest} exists. rm it first!")
-        return 
-    #  allow_git_dirty = args.allow_git_dirty
+        return
 
     tempalte_name = args.magic[0]
     is_from_net=tempalte_name.startswith("http://") or tempalte_name.startswith("https://") or tempalte_name.startswith("file://") or tempalte_name.startswith("git@")
 
 
     if is_from_net and args.script_from_net:
         logger.critical(f"template is from net! Script will run cause you use -s option! BE CAUTION!")
     if not is_from_net or args.script_from_net:
-        before_copy(root,dest)
+        before_copy(code_template_folder,dest)
     else:
         logger.warn(f'before script will not run')
 
     if is_from_net:
-        # -b opencv-2.4 --single-branch
         subprocess.Popen(["git","clone","--depth=1","-b",args.branch, "--single-branch",tempalte_name,dest]).communicate()
     else:
-        copying(root,dest)
+        copying(targets,dest)
 
-    for key, val in keypairs.items(): 
-        fullReplace(dest,key,val)
+    for key, val in keypairs.items():
+        full_repalcement(dest,key,val)
 
     if not is_from_net or args.script_from_net:
-        after_copy(root,dest)
+        after_copy(targets,dest)
     else:
         logger.warn(f'after script will not run')
 
 
-
-def listTarget(root,depth):
-    stuff = os.path.abspath(os.path.expanduser(os.path.expandvars(root)))
+def list_target(code_template_folder,depth):
+    stuff = os.path.abspath(os.path.expanduser(os.path.expandvars(code_template_folder)))
 
     for dname,dirs,files in os.walk(stuff, followlinks=True):
         dirs[:] = [d for d in dirs if not d == '.git']
         cdepth = dname[len(stuff):].count(os.sep)
         if basename(dname).startswith(".") or ".git" in dname or "__pycache__" in dname:
             continue
         if  cdepth < depth:
             print("     "*(cdepth-1) , basename(dname))
 
-def listCmd(root,depth):
-    stuff = os.path.abspath(os.path.expanduser(os.path.expandvars(root)))
-    
+def list_commands(code_template_folder,depth):
+    stuff = os.path.abspath(os.path.expanduser(os.path.expandvars(code_template_folder)))
+
     for dname,dirs,files in os.walk(stuff, followlinks=True):
         dirs[:] = [d for d in dirs if not d == '.git']
         cdepth = dname[len(stuff):].count(os.sep)
         if basename(dname).startswith(".") or ".git" in dname or "__pycache__" in dname:
             continue
         if  cdepth < depth:
-            print("coge",re.sub("/"," ",re.sub(root,"",dname)),"@:app")
-        olddepth = cdepth 
+            print("coge",re.sub("/"," ",re.sub(code_template_folder,"",dname)),"@:app")
 
 
 
-def get_root():
+def get_code_template_folder():
     env_root = os.environ.get("COGE_TMPLS") or os.environ.get("CG_TMPLS")
-    root  = env_root or os.path.expanduser("~/.config/.code_template")
-    return env_root,root
+    if env_root is None:
+        fallbackdir= os.path.expanduser("~/.config/.code_template")
+        Path(fallbackdir).mkdir(parents=True, exist_ok=True)
+        logger.warning(f"env COGE_TMPLS is not definded! use default tmplts location: {fallbackdir}")
+
+    code_template_folder  = env_root or os.path.expanduser("~/.config/.code_template")
+    return code_template_folder
 
 def entry_point():
-    parser = createParse()
+    parser = create_parser()
     mainArgs=parser.parse_args()
-    env_root,root = get_root()
     if(mainArgs.version):
         import pkg_resources  # part of setuptools
         version = pkg_resources.require("coge")[0].version
         print(version)
-        return 
-    if env_root is None:
-        fallbackdir= os.path.expanduser("~/.config/.code_template")
-        Path(fallbackdir).mkdir(parents=True, exist_ok=True)
-        logger.warning(f"env COGE_TMPLS is not definded! use default tmplts location: {fallbackdir}")
+        return
 
-    
-    if mainArgs.link_tplt:
-        link()
-        return 
-
-    if mainArgs.unlink_tplt:
-        unlink()
-        return 
+    if mainArgs.link_target:
+        t = mainArgs.link_target
+        apath = os.path.abspath(t)
+        link(apath)
+        return
 
-    main(root,mainArgs)
+    if mainArgs.unlink_target:
+        t = mainArgs.unlink_target
+        unlink(t)
+        return
+
+    main(mainArgs)
 
-def link():
-    _ ,root = get_root()
+def link(apath):
+    code_template_folder = get_code_template_folder()
+    print(code_template_folder)
     cwd = os.getcwd()
     dest_name = basename(cwd)
-    dest_tmpl = f"{root}/{dest_name}"
-    if not os.path.isdir(dest_tmpl):
-        subprocess.check_output(f"ln  -s $PWD {root}", shell=True)
-        logger.info(f'link:{cwd} --> {root}/{dest_name}')
+    dest_tmpl = f"{code_template_folder}/{dest_name}"
+
+    if not os.path.exists(dest_tmpl):
+        logger.info(f'link:{apath} --> {code_template_folder}/{dest_name}')
     else:
-        logger.warning(f"template {dest_tmpl} exits! Just use it. if you want to unlink it, use coge -R in your source folder")
+        logger.warning(f"target {dest_tmpl} exits! Just use it. if you want to unlink it, use coge -R in your source folder or file")
+        exit()
 
-def unlink():
-    _ ,root = get_root()
-    cwd = os.getcwd()
-    dest_name = basename(cwd)
-    dest_tmpl = f"{root}/{dest_name}"
-    if os.path.isdir(dest_tmpl):
-        subprocess.check_output(f"rm -f  {dest_tmpl}", shell=True)
-        logger.info(f'unlink:{cwd} -x- {root}/{dest_name}')
+    if os.path.isfile(apath):
+        subprocess.check_output(f"ln  -s {apath} {code_template_folder}", shell=True)
+    else:
+        subprocess.check_output(f"ln  -s {apath} {code_template_folder}", shell=True)
+
+def unlink(dest_name):
+    code_template_folder = get_code_template_folder()
+    dest_tmpl = f"{code_template_folder}/{dest_name}"
+    print(dest_tmpl)
+    if os.path.exists(dest_tmpl):
+        logger.info(f'Removed. {dest_tmpl}')
     else:
-        logger.warning(f"template {dest_tmpl} dose not exits!")
+        logger.warning(f"target {dest_tmpl} does not exits!")
+        exit()
+    subprocess.check_output(f"rm -f  {dest_tmpl}", shell=True)
 
-def createParse():
+def create_parser():
     parser = argparse.ArgumentParser( formatter_class=argparse.RawTextHelpFormatter, description="""
-       make template link : cd x-engine-module-template && coge -r 
-             use template : coge x-engine-module-template xxxx:camera @:x-engine-module-camera  
-use git template from net : coge https://www.github.com/vitejs/vite \\bvite\\b:your_vite @:your_vite  
+       make template link : cd x-engine-module-template && coge -r
+             use template : coge x-engine-module-template xxxx:camera @:x-engine-module-camera
+use git template from net : coge https://www.github.com/vitejs/vite \\bvite\\b:your_vite @:your_vite
     """)
 
-    parser.add_argument('-b', '--branch',type=str,required=False, help='branch', default="master")  
-    parser.add_argument('-a', '--arg_prefix',type=str,required=False, help='ex: COGE_ARG_', default="COGE_ARG_")  
-    parser.add_argument('-l', '--list', help='list folders', default=False, action='store_true' ,) 
-    parser.add_argument('-c', '--cmd', help='cmd', default=False, action='store_true' ,) 
-    parser.add_argument('-r', '--link_tplt', help='link `cwd` to $COGE_TMPLS', default=False, action='store_true' ) 
-    parser.add_argument('-R', '--unlink_tplt', help='unlink `cwd`', default=False, action='store_true' ) 
-    #  parser.add_argument('-w', '--allow_git_dirty', help='alllow git dirty, still, file not commited will not copy!', default=False, action='store_true' )
-    parser.add_argument('-s', '--script_from_net', help='alllow script from net', default=False, action='store_true' ) 
-    parser.add_argument('-d', '--depth',type=int,required=False, help='list depth', default=3)  
-    parser.add_argument('-v', '--version', help='version', default=False, action='store_true' ) 
-    parser.add_argument('magic', metavar="magic", type=str, nargs='*', 
+    parser.add_argument('-b', '--branch',type=str,required=False, help='branch', default="master")
+    parser.add_argument('-l', '--list', help='list folders', default=False, action='store_true' ,)
+    parser.add_argument('-c', '--cmd', help='cmd', default=False, action='store_true' ,)
+    parser.add_argument('-r', '--link_target',type=str,required=False, help='link target to $COGE_TMPLS, target must be a relative folder / file', default="")
+    parser.add_argument('-R', '--unlink_target',type=str,required=False, help='unlink target to $COGE_TMPLS, target must be a relative folder / file', default="")
+
+    parser.add_argument('-s', '--script_from_net', help='alllow script from net', default=False, action='store_true' )
+    parser.add_argument('-d', '--depth',type=int,required=False, help='list depth', default=3)
+    parser.add_argument('-v', '--version', help='version', default=False, action='store_true' )
+
+    parser.add_argument('magic', metavar="magic", type=str, nargs='*',
             help='newkey:oldkey or @:folder_name')
     return parser
```

## Comparing `coge-0.1.8.dist-info/METADATA` & `coge-0.1.9.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,77 @@
 Metadata-Version: 2.1
 Name: coge
-Version: 0.1.8
+Version: 0.1.9
 Summary: this is a description
 Home-page: https://github.com/zk4/coge
+Download-URL: https://github.com/zk4/coge/archive/master.zip
 Author: zk
 Author-email: liuzq7@gmail.com
 License: BSD
-Download-URL: https://github.com/zk4/coge/archive/master.zip
 Keywords: best practice for python project
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Requires-Python: >3.0.0
 Description-Content-Type: text/markdown
-Requires-Dist: PyYAML (==5.3.1)
 Requires-Dist: binaryornot (==0.4.4)
+Requires-Dist: chardet (==5.1.0)
+Requires-Dist: PyYAML (==5.3.1)
 
-![image-20210312140113821](https://raw.githubusercontent.com/zk4/image_backup/main/img/image-20210312140113821.png)
-
+> How I reuse a existing project as a template effectively? 
 
+![image-20210312140113821](https://raw.githubusercontent.com/zk4/image_backup/main/img/image-20210312140113821.png)
 
 Simple yet powerful code generator.
 Make use of existing tool as possiable as we can.
 
-Compare to hygen, yo.
-- yo is way too slow and complicated.
-- hygen pollutes all template files, and only support ejs.
-
-**What I only need:**
+**Small features:**
 1. template is runable as normal prj. No more %placehold% stuff.
-2. instinct command with the power of fzf.
-4. quick project to template and vice versa.
 3. respect .gitignore.
 3. support github.com repo.
 5. plugin in any language only if you can run it in shell.
 7. respect Old keyword case. 
 
 # install
 ```
 pip3 install coge
 ```
 
 # usage
+put this line in your `~/.bash_profile`, and change the `your_template_folder` to  the folder where you put your templates.
 ```
 export COGE_TMPLS="<your_template_folder>"
 ```
 
-## 1
+## demo 1
 ``` bash
 coge js react oldkey:newkey :newkey0 :newkey1 @:destname 
-```
-What coge does:
 
-- copy $COGE_TMPLS/js/react to $PWD/destname
-- change all names from oldkey to newkey,  from  COGE_ARG_0 to newkey0 ,from  COGE_ARG_1 to newkey1
+# What coge does:
+# - copy $COGE_TMPLS/js/react to $PWD/destname
+# - change all names from oldkey to newkey,  from  COGE_ARG_0 to newkey0 ,from  COGE_ARG_1 to newkey1
 
-## 2
+```
+## demo 2
 ``` bash
 coge js react
+# What coge does:
+# - Just copy $COGE_TMPLS/js/react to $PWD/app
 ```
-What coge does:
-- Just copy $COGE_TMPLS/js/react to $PWD/app
 
 
-# work with fzf
+# advanced tricks (optional)
+
+## work with fzf
 ``` 
 cg () {
 	eval `coge -c $@ | fzf --preview= --bind 'enter:execute-silent(pbcopy <<< {})+abort' ` && pbpaste
 }
 ```
 call cg from terminal. and paste it.
-
-
-# timing script 
+## hook script
 you can put .coge.after.sh in you template folder. 
 
 It will execute after copy, which is very handy.
 
 For Safety reason. Template from network would need to use -s option to enforcing script executing, only if you know the script is safe.
 
 Supported timing and language:
@@ -92,14 +87,33 @@
 put .coge.after.sh in your source template
 ```
 #!/bin/bash
 echo "init your git repo"
 git init 
 ```
 
+## .coge.json 
+Sometimes we do not remember what the string we should repalce,
+put a `.coge.json` in your template project.
+coge would respect this json file to verify all replacements. 
+It is just a array with two types, map or string.
+all elements in the array must be fullfilled when doing the replacements.
+If some strings to be replaced are missed in the command line. Coge would automatically prompt up for user to supply.
+
+I think the configuration explains for itself.
+``` json
+[
+  {
+   "key": "cli",
+   "desc": "this is blala"
+  },
+  "projectname"
+]
+```
+
 
 # help
 ```
 usage: coge [-h] [-a ARG_PREFIX] [-l] [-c] [-r] [-R] [-s] [-d DEPTH] [-v]
             [magic ...]
 
        make template link : cd x-engine-module-template && coge -r 
@@ -120,8 +134,7 @@
   -R, --unlink_tplt     unlink `cwd`
   -s, --script_from_net
                         alllow script from net
   -d DEPTH, --depth DEPTH
                         list depth
   -v, --version         version
 ```
-
```

