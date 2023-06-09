# Comparing `tmp/pandoc_pdf-0.1.8.tar.gz` & `tmp/pandoc_pdf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_pdf-0.1.8.tar", max compression
+gzip compressed data, was "pandoc_pdf-0.1.9.tar", max compression
```

## Comparing `pandoc_pdf-0.1.8.tar` & `pandoc_pdf-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1060 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/LICENSE
--rw-r--r--   0        0        0      691 2023-06-08 16:04:16.565677 pandoc_pdf-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf/__init__.py
--rw-r--r--   0        0        0     2777 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf/main.py
--rw-r--r--   0        0        0      802 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/deeplists.tex
--rw-r--r--   0        0        0      773 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/defaults.yml
--rw-r--r--   0        0        0      670 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/header.tex
--rw-r--r--   0        0        0      179 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/setting.yml
--rw-r--r--   0        0        0      184 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/env.py
--rw-r--r--   0        0        0     4105 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/functions.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.8/setup.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/LICENSE
+-rw-r--r--   0        0        0      691 2023-06-08 23:54:38.787035 pandoc_pdf-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf/__init__.py
+-rw-r--r--   0        0        0     2741 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf/main.py
+-rw-r--r--   0        0        0      802 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf_utils/default_config/deeplists.tex
+-rw-r--r--   0        0        0      773 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf_utils/default_config/defaults.yml
+-rw-r--r--   0        0        0      670 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf_utils/default_config/header.tex
+-rw-r--r--   0        0        0      179 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf_utils/default_config/setting.yml
+-rw-r--r--   0        0        0      184 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf_utils/env.py
+-rw-r--r--   0        0        0     4184 2023-06-08 23:54:22.942954 pandoc_pdf-0.1.9/src/pandoc_pdf_utils/functions.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.9/setup.py
+-rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.9/PKG-INFO
```

### Comparing `pandoc_pdf-0.1.8/LICENSE` & `pandoc_pdf-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.8/pyproject.toml` & `pandoc_pdf-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Command to generate pdf easily with pandoc."
 license = "MIT"
 name = "pandoc_pdf"
 packages = [
   {include = "pandoc_pdf", from = "src"},
   {include = "pandoc_pdf_utils", from = "src"},
 ]
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 PyYAML = "^6.0"
 click = "^8.1.3"
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `pandoc_pdf-0.1.8/src/pandoc_pdf/main.py` & `pandoc_pdf-0.1.9/src/pandoc_pdf/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,97 @@
-from asyncio import subprocess
-from pandoc_pdf_utils.functions import \
-    init_config, init_setting, init_cache, generate_command_docker, generate_command_pandoc
+from pandoc_pdf_utils.functions import (
+    init_config,
+    init_setting,
+    init_cache,
+    generate_command_docker,
+    generate_command_pandoc,
+)
 from pandoc_pdf_utils.env import CACHE_DIR, CONFIG_DIR
 from pathlib import Path
 import subprocess
 import click
 import yaml
 from copy import deepcopy
-from pprint import pprint
 
 init_config()
-with open(CONFIG_DIR / 'defaults.yml') as f:
+with open(CONFIG_DIR / "defaults.yml") as f:
     presets = [key_i for key_i in yaml.safe_load(f)]
 
 
 @click.command()
+@click.option("--debug", is_flag=True)
+@click.option("-D", "--docker", type=str)
 @click.option(
-    '--debug',
-    is_flag=True
-)
-@click.option(
-    '-D', '--docker',
-    type=str
-)
-@click.option(
-    '-v', '--volume',
+    "-v",
+    "--volume",
     type=str,
     multiple=True,
 )
+@click.option("-V", "--variable", type=str, multiple=True)
+@click.option("-M", "--metadata", type=str, multiple=True)
+@click.option("-p", "--preset", type=click.Choice(presets), default="latex")
 @click.option(
-    '-V', '--variable',
-    type=str,
-    multiple=True
-)
-@click.option(
-    '-M', '--metadata',
-    type=str,
-    multiple=True
-)
-@click.option(
-    '-p', '--preset',
-    type=click.Choice(presets),
-    default="latex"
-)
-@click.option(
-    '-o', '--output',
+    "-o",
+    "--output",
     type=click.Path(path_type=Path),
-    default='NULL',
+    default="NULL",
 )
 @click.argument(
-    'input_file',
+    "input_file",
     type=click.Path(exists=True, path_type=Path),
 )
-def pandoc_pdf(input_file: Path, debug: bool, docker, volume, metadata, variable, preset, output):
+def pandoc_pdf(
+    input_file: Path, debug: bool, docker, volume, metadata, variable, preset, output
+):
     """Command to generate pdf easily with pandoc."""
     output_file = deepcopy(output)
     volumes = deepcopy(volume)
     variables = deepcopy(variable)
     metadatas = deepcopy(metadata)
     del output
     del volume
     del variable
     del metadata
-    if str(output_file) == 'NULL':
+    if str(output_file) == "NULL":
         output_file = Path(f"{input_file.parent / input_file.stem}.pdf")
     init_cache()
     setting_obj = init_setting(docker, volumes)
-    if setting_obj['docker']['use_docker']:
-        defaults_file = Path(f'/cache/defaults_{preset}.yml')
+    if setting_obj["docker"]["use_docker"]:
+        defaults_file = Path(f"/cache/defaults_{preset}.yml")
     else:
-        defaults_file = CACHE_DIR / f'defaults_{preset}.yml'
+        defaults_file = CACHE_DIR / f"defaults_{preset}.yml"
 
     # * ---Execute command
     args_docker = generate_command_docker(setting_obj)
     args_pandoc = generate_command_pandoc(
-        setting_obj, defaults_file, input_file, output_file, preset, variables, metadatas
+        setting_obj,
+        defaults_file,
+        input_file,
+        output_file,
+        preset,
+        variables,
+        metadatas,
     )
-    if setting_obj['docker']['use_docker'] == True:
-        args = ' '.join(args_docker) + f" \"{' '.join(args_pandoc)}\""
+    if setting_obj["docker"]["use_docker"] == True:
+        args = " ".join(args_docker) + f" \"{' '.join(args_pandoc)}\""
     else:
-        args = ' '.join(args_pandoc)
+        args = " ".join(args_pandoc)
     result = subprocess.run(args, shell=True)
-    result_status = 'Succeeded' if result.returncode == 0 else 'Failed'
-    result_color = '' if result.returncode == 0 else 'red'
+    result_status = "Succeeded" if result.returncode == 0 else "Failed"
+    result_color = "" if result.returncode == 0 else "red"
     click.secho(
-        f'{result_status} to generate {str(output_file)} from {str(input_file)} by {preset}.',
+        f"{result_status} to generate {str(output_file)} from {str(input_file)} by {preset}.",
         fg=result_color,
-        bold=True
+        bold=True,
     )
 
     if debug:
-        click.secho('\n---< DEBUG >---', fg='red')
-        click.secho('Executed command:')
-        click.secho(f'  {result.args}', bold=True)
+        click.secho("\n---< DEBUG >---", fg="red")
+        click.secho("Executed command:")
+        click.secho(f"  {result.args}", bold=True)
 
     if result.returncode == 0:
         return 0
     else:
         return 1
```

### Comparing `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/deeplists.tex` & `pandoc_pdf-0.1.9/src/pandoc_pdf_utils/default_config/deeplists.tex`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/defaults.yml` & `pandoc_pdf-0.1.9/src/pandoc_pdf_utils/default_config/defaults.yml`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/header.tex` & `pandoc_pdf-0.1.9/src/pandoc_pdf_utils/default_config/header.tex`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/functions.py` & `pandoc_pdf-0.1.9/src/pandoc_pdf_utils/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,122 @@
 from .env import CONFIG_DIR, DEFAULT_CONFIG_DIR, CACHE_DIR
 import yaml
 from pathlib import Path
 import shutil
 
 
 def init_config() -> None:
-    """genegete default config files to CACHE_DIR and CONFIG_DIR if the cofig files don't exist.
-    """
+    """genegete default config files to CACHE_DIR and CONFIG_DIR if the cofig files don't exist."""
     if not CONFIG_DIR.exists():
         shutil.copytree(DEFAULT_CONFIG_DIR, CONFIG_DIR, dirs_exist_ok=False)
 
 
 def init_cache() -> None:
-    """Copy the CONFIG_DIR folder to CACHE_DIR recursively. Generate the defaults_{preset}.yml separeted by preset.
-    """
+    """Copy the CONFIG_DIR folder to CACHE_DIR recursively. Generate the defaults_{preset}.yml separeted by preset."""
     if not CACHE_DIR.exists():
         CACHE_DIR.mkdir()
     shutil.copytree(CONFIG_DIR, CACHE_DIR, dirs_exist_ok=True)
-    with open(CONFIG_DIR / 'defaults.yml') as f:
+    with open(CONFIG_DIR / "defaults.yml") as f:
         defaults_obj: dict = yaml.safe_load(f)
     for preset_i in defaults_obj:
-        defaults_by_preset: Path = CACHE_DIR / f'defaults_{preset_i}.yml'
+        defaults_by_preset: Path = CACHE_DIR / f"defaults_{preset_i}.yml"
         if not defaults_by_preset.exists():
             defaults_by_preset.touch()
-        with open(defaults_by_preset, 'w') as f:
-            yaml.dump(defaults_obj[preset_i], f,
-                      encoding='utf-8', allow_unicode=True)
+        with open(defaults_by_preset, "w") as f:
+            yaml.dump(defaults_obj[preset_i], f, encoding="utf-8", allow_unicode=True)
 
 
 def init_setting(opt_docker, opt_volumes) -> dict:
     """Load setting.yml and apply the command's options to the loaded object.
 
     Args:
         opt_docker (str): docker image name
         opt_volumes (str): the volume to mount to docker container
 
     Returns:
         dict: ~/.config/setting.yml object
     """
-    setting_file_path = CONFIG_DIR / 'setting.yml'
-    with open(setting_file_path, 'r') as f:
+    setting_file_path = CONFIG_DIR / "setting.yml"
+    with open(setting_file_path, "r") as f:
         setting_obj = yaml.safe_load(f)
 
-    setting_obj['docker'].setdefault('volumes', [])
-    setting_obj['docker'].setdefault('other_option', "")
+    setting_obj["docker"].setdefault("volumes", [])
+    setting_obj["docker"].setdefault("other_option", "")
     if opt_docker:
-        setting_obj['docker']['use_docker'] = True
-        setting_obj['docker']['docker_image'] = opt_docker
+        setting_obj["docker"]["use_docker"] = True
+        setting_obj["docker"]["docker_image"] = opt_docker
     if opt_volumes:
         if opt_docker:
-            setting_obj['docker']['volumes'] = opt_volumes
+            setting_obj["docker"]["volumes"] = opt_volumes
         else:
-            setting_obj['docker']['volumes'].extend(opt_volumes)
+            setting_obj["docker"]["volumes"].extend(opt_volumes)
 
     return setting_obj
 
 
 def generate_command_docker(setting_obj) -> list[str]:
     """Generate docker commands from the given settings.
 
     Args:
         setting_obj (dict): Object of pandoc_pdf command settings (~/.config/setting.yml)
 
     Returns:
         list[str]: docker command with arguments
     """
-    setting_obj['docker'].setdefault('volumes', [])
-    setting_obj['docker'].setdefault('other_option', "")
-    args_docker = ['docker', 'run', '--rm', '--volume',
-                   f'{CACHE_DIR}:/cache', '--entrypoint', '/bin/bash']
-    if setting_obj['docker']['use_docker'] == True:
-        for volume_i in setting_obj['docker']['volumes']:
-            args_docker.extend(['--volume', volume_i])
-        args_docker.append(setting_obj['docker']['other_option'])
-        args_docker.append(setting_obj['docker']['docker_image'])
-        args_docker.append('-c')
+    setting_obj["docker"].setdefault("volumes", [])
+    setting_obj["docker"].setdefault("other_option", "")
+    args_docker = [
+        "docker",
+        "run",
+        "--rm",
+        "--volume",
+        f"{CACHE_DIR}:/cache",
+        "--entrypoint",
+        "/bin/bash",
+    ]
+    if setting_obj["docker"]["use_docker"] == True:
+        for volume_i in setting_obj["docker"]["volumes"]:
+            args_docker.extend(["--volume", volume_i])
+        args_docker.append(setting_obj["docker"]["other_option"])
+        args_docker.append(setting_obj["docker"]["docker_image"])
+        args_docker.append("-c")
     else:
         args_docker = []
     return args_docker
 
 
-def generate_command_pandoc(setting_obj, defaults_file, input_file, output_file, opt_preset, opt_variables, opt_metadatas) -> list[str]:
+def generate_command_pandoc(
+    setting_obj,
+    defaults_file,
+    input_file,
+    output_file,
+    opt_preset,
+    opt_variables,
+    opt_metadatas,
+) -> list[str]:
     """Generate pandoc commands from the given defaults_file's object and options of pandoc_pdf command.
 
     Args:
         setting_obj (dict): Object of pandoc_pdf command settings.
         defaults_file (Path): Path to the pandoc defaults file (defaults.yml) generated for each preset.
         input_file (Path): Path to the file to be converted to PDF, given as an argument to the pandoc_pdf command.
         output_file (Path): Path of the file to output to. Value of --output option.
         opt_preset (str): Preset name to be used. By default, html5 and latex are set.
         opt_variables ([str]): Arguments for LaTeX files.
         opt_metadatas ([str]): A set of keys and values to be registered as metadata.
 
     Returns:
         list[str]: pandoc command with arguments
     """
-    args_pandoc = ['pandoc', str(input_file), '-o',
-                   str(output_file), '-d', str(defaults_file)]
+    args_pandoc = [
+        "pandoc",
+        str(input_file),
+        "-o",
+        str(output_file),
+        "-d",
+        str(defaults_file),
+    ]
     for variable in opt_variables:
-        args_pandoc.extend(['-V', variable])
+        args_pandoc.extend(["-V", variable])
     for metadata in opt_metadatas:
-        args_pandoc.extend(['-M', metadata])
+        args_pandoc.extend(["-M", metadata])
     return args_pandoc
```

### Comparing `pandoc_pdf-0.1.8/setup.py` & `pandoc_pdf-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['PyYAML>=6.0,<7.0', 'click>=8.1.3,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['pandoc_pdf = pandoc_pdf.main:pandoc_pdf']}
 
 setup_kwargs = {
     'name': 'pandoc-pdf',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Command to generate pdf easily with pandoc.',
     'long_description': 'None',
     'author': 'rai',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

