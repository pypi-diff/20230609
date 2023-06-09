# Comparing `tmp/tool_server_generator-0.3.3.tar.gz` & `tmp/tool_server_generator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_server_generator-0.3.3.tar", last modified: Thu Jun  8 20:14:51 2023, max compression
+gzip compressed data, was "tool_server_generator-0.4.tar", last modified: Fri Jun  9 17:29:39 2023, max compression
```

## Comparing `tool_server_generator-0.3.3.tar` & `tool_server_generator-0.4.tar`

### file list

```diff
@@ -1,22 +1,28 @@
--rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.3.3/LICENSE
--rwxr-xr-x   0        0        0      669 2023-06-07 18:45:05.137872 tool_server_generator-0.3.3/config_server.txt
--rwxr-xr-x   0        0        0      526 2023-06-08 17:49:02.430745 tool_server_generator-0.3.3/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-05 17:15:32.717658 tool_server_generator-0.3.3/readme.md
--rwxr-xr-x   0        0        0     2760 2023-06-08 20:11:27.406406 tool_server_generator-0.3.3/tool_server_generator/__init__.py
--rwxr-xr-x   0        0        0      669 2023-06-07 18:37:38.465184 tool_server_generator-0.3.3/tool_server_generator/config_server.txt
--rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.3.3/tool_server_generator/model/app.js
--rwxr-xr-x   0        0        0     1524 2023-06-06 13:59:55.077587 tool_server_generator-0.3.3/tool_server_generator/model/bin/www
--rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.3.3/tool_server_generator/model/package-lock.json
--rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.3.3/tool_server_generator/model/package.json
--rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.3.3/tool_server_generator/model/public/stylesheets/w3.css
--rwxr-xr-x   0        0        0     1982 2023-06-08 16:18:55.637309 tool_server_generator-0.3.3/tool_server_generator/model/routes/index.js
--rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.3.3/tool_server_generator/model/views/error.pug
--rwxr-xr-x   0        0        0       66 2023-06-05 14:49:43.488782 tool_server_generator-0.3.3/tool_server_generator/model/views/index.pug
--rwxr-xr-x   0        0        0      129 2023-06-05 19:35:26.231973 tool_server_generator-0.3.3/tool_server_generator/model/views/layout.pug
--rwxr-xr-x   0        0        0     1147 2023-06-07 21:08:08.603638 tool_server_generator-0.3.3/tool_server_generator/model/views/requests.pug
--rwxr-xr-x   0        0        0     1312 2023-06-08 15:55:11.225309 tool_server_generator-0.3.3/tool_server_generator/model/workers/process_command.js
--rwxr-xr-x   0        0        0     3799 2023-06-08 16:08:07.456282 tool_server_generator-0.3.3/tool_server_generator/model/workers/request_listener.js
--rwxr-xr-x   0        0        0    11115 2023-06-08 17:25:13.811785 tool_server_generator-0.3.3/tool_server_generator/utils/config_parser.py
--rwxr-xr-x   0        0        0     8718 2023-06-08 17:31:14.438812 tool_server_generator-0.3.3/tool_server_generator/utils/config_server.py
--rwxr-xr-x   0        0        0      843 2023-06-08 17:45:14.500144 tool_server_generator-0.3.3/tool_server_generator/utils/utils.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 tool_server_generator-0.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.4/LICENSE
+-rwxr-xr-x   0        0        0      653 2023-06-08 22:39:34.183032 tool_server_generator-0.4/config_server.txt
+-rwxr-xr-x   0        0        0      526 2023-06-08 17:49:02.430745 tool_server_generator-0.4/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-05 17:15:32.717658 tool_server_generator-0.4/readme.md
+-rwxr-xr-x   0        0        0     3773 2023-06-09 17:21:38.772292 tool_server_generator-0.4/tool_server_generator/__init__.py
+-rwxr-xr-x   0        0        0      874 2023-06-09 17:06:31.629489 tool_server_generator-0.4/tool_server_generator/config_server.txt
+-rwxr-xr-x   0        0        0      990 2023-06-09 13:32:47.222267 tool_server_generator-0.4/tool_server_generator/examples/config_server.json
+-rwxr-xr-x   0        0        0      653 2023-06-08 22:39:31.488290 tool_server_generator-0.4/tool_server_generator/examples/config_server.txt
+-rwxr-xr-x   0        0        0      984 2023-06-09 13:33:25.461589 tool_server_generator-0.4/tool_server_generator/examples/config_server2.txt
+-rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.4/tool_server_generator/model/app.js
+-rwxr-xr-x   0        0        0     1524 2023-06-06 13:59:55.077587 tool_server_generator-0.4/tool_server_generator/model/bin/www
+-rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.4/tool_server_generator/model/package-lock.json
+-rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.4/tool_server_generator/model/package.json
+-rwxr-xr-x   0        0        0      318 2023-06-09 13:30:36.974342 tool_server_generator-0.4/tool_server_generator/model/public/images/favicon.ico
+-rwxr-xr-x   0        0        0      940 2023-06-09 17:03:39.505128 tool_server_generator-0.4/tool_server_generator/model/public/javascripts/jquery.js
+-rwxr-xr-x   0        0        0      998 2023-06-09 17:03:59.407667 tool_server_generator-0.4/tool_server_generator/model/public/javascripts/requests.js
+-rwxr-xr-x   0        0        0      421 2023-06-09 17:15:12.284029 tool_server_generator-0.4/tool_server_generator/model/public/stylesheets/color.css
+-rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.4/tool_server_generator/model/public/stylesheets/w3.css
+-rwxr-xr-x   0        0        0     2755 2023-06-09 17:13:40.296604 tool_server_generator-0.4/tool_server_generator/model/routes/index.js
+-rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.4/tool_server_generator/model/views/error.pug
+-rwxr-xr-x   0        0        0     1046 2023-06-09 17:09:04.085388 tool_server_generator-0.4/tool_server_generator/model/views/layout.pug
+-rwxr-xr-x   0        0        0     1950 2023-06-09 17:16:28.853886 tool_server_generator-0.4/tool_server_generator/model/views/requests.pug
+-rwxr-xr-x   0        0        0     1899 2023-06-09 17:04:43.374738 tool_server_generator-0.4/tool_server_generator/model/workers/process_command.js
+-rwxr-xr-x   0        0        0     6296 2023-06-09 17:04:43.379737 tool_server_generator-0.4/tool_server_generator/model/workers/request_listener.js
+-rwxr-xr-x   0        0        0    18259 2023-06-09 17:19:08.649664 tool_server_generator-0.4/tool_server_generator/utils/config_parser.py
+-rwxr-xr-x   0        0        0     9573 2023-06-09 17:04:43.390737 tool_server_generator-0.4/tool_server_generator/utils/config_server.py
+-rwxr-xr-x   0        0        0      824 2023-06-08 22:05:58.703064 tool_server_generator-0.4/tool_server_generator/utils/utils.py
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 tool_server_generator-0.4/PKG-INFO
```

### Comparing `tool_server_generator-0.3.3/LICENSE` & `tool_server_generator-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.3/config_server.txt` & `tool_server_generator-0.4/config_server.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 * Servidor
 - Nome: Servidor
 - Diretoria: "teste"
-- IP: 127.0.0.1
 - Porta: 15213
 * Ferramentas
 --
 - Família:Grep
 - Título: "Grep"
 - Descrição: "grep  searches  for  PATTERNS in each FILE.  PATTERNS is one or more patterns separated by newline characters,
 and grep prints each line that matches a pattern.  Typically PATTERNS should be quoted when grep is used in  a
```

### Comparing `tool_server_generator-0.3.3/pyproject.toml` & `tool_server_generator-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.3/tool_server_generator/__init__.py` & `tool_server_generator-0.4/tool_server_generator/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #! /usr/bin/env python3
 """Module to create tools server
 """
 
 import os
 import shutil
 import subprocess
+import json
 from pyngrok import ngrok
 from .utils.utils import *
 from .utils.config_parser import *
 from .utils.config_server import *
 
-__version__ = '0.3.3'
+__version__ = '0.4'
 project_dir = os.path.dirname(os.path.realpath(__file__))
 model_server = f'{project_dir}/model'
 tunnel = None
 
 def start_ngrok(config):
     '''Tenta expor a porta do servidor utilizando o ngrok'''
     global tunnel
     try:
         print(ngrok.get_tunnels())
         print('Exposing port using ngrok')
         tunnel = ngrok.connect(config['porta'],'http')
-        print('Port exposed',tunnel)
-        print('Public URL',tunnel.public_url)
+        print('Public URL: ',tunnel.public_url)
     except Exception as e:
         print(e)
         print('Error: Could not expose port using ngrok.')
         tunnel = None
 
 
 def start_server(server_dir,config):
@@ -37,51 +37,81 @@
     dependencies = ['express','http-errors','adm-zip']
 
     # multer apenas se ferramentas levarem ficheiros como input
     if has_file_input(config['ferramentas']):
         dependencies += ['multer']
         
     dependencies = ' '.join(dependencies)
-    print(f'Installing server dependencies: [{dependencies}]')
-    p = subprocess.call(f'npm i {dependencies} -s', cwd=server_path,shell=True)
-    print('Dependencies installed')
-    print('Starting server')
-    p = subprocess.call(f'npm start', cwd=server_path,shell=True)
-    print('Server closed')
-    # desconectar ngrok
-    if tunnel:
-        print('Closing ngrok')
-        ngrok.disconnect(tunnel.public_url)
+    try:
+        print(f'Installing server dependencies: [{dependencies}]')
+        p = subprocess.call(f'npm i {dependencies} -s', cwd=server_path,shell=True)
+        print('Dependencies installed')
+        print('Starting server')
+        p = subprocess.call(f'npm start', cwd=server_path,shell=True)
+    except Exception as e:
+        print('Server closed')
+        # desconectar ngrok
+        if tunnel:
+            print('Closing ngrok')
+            ngrok.disconnect(tunnel.public_url)
 
 def tool_server():
     args = parse_arguments(__version__)
-    config_file = args.config_file
-    config = parse_config(config_file[0])
+    config_file = args.config_file[0]
+    file = open(config_file,'r',encoding='utf-8')
+    json_config = False
+    # ficheiro json
+    if config_file.endswith('.json'):
+        json_config = True
+        config = dict(json.load(file))
+        file.close()
+    # outro tipo
+    else:
+        config = parse_config(file)
 
-    if config_valid(config):
+    if not json_config or config_valid(config):
         #Copiar o modelo do servidor para a diretoria desejada
         destino = config['diretoria'] + '/' + config['nome']
         origem = model_server
         try:
             shutil.copytree(origem, destino)
         except FileNotFoundError:
-            print("Servidor modelo não encontrado!")
+            print("Model Server not found!")
             exit(-1)
         except FileExistsError:
-            print("A diretoria de destino já existe.")
+            print("Directory already exists.")
             exit(-1)
         except Exception as e:
-            print(f"Erro ao copiar o modelo do servidor: {e}")
+            print(f"Error copying the model server: {e}")
             exit(-1)
+        
         # alterar configuracoes do servidor
         config_server(destino,config)
 
-        # expor porta de ngrok
-        if args.ngrok:
-            start_ngrok(config)
-
+        if config['visuais']['favicon'] != '':
+            favicon = config['visuais']['favicon']
+            old_favicon = destino + '/public/images/favicon.ico'
+            destino_favicon = destino + '/public/images/favicon.ico'
+
+            #remover favicon default que vem do model
+            os.remove(old_favicon)
+            
+            #colocar o dado
+            try:
+                shutil.copy(favicon,destino_favicon)
+            except FileNotFoundError:
+                print("Favicon not found!")
+                exit(-1)
+            except Exception as e:
+                print(f"Error copying the favicon: {e}")
+                exit(-1)
+                
         #iniciar servidor
         if args.start_server:
+            # expor porta de ngrok
+            if args.ngrok:
+                start_ngrok(config)
+
             start_server(destino,config)
     else:
-        print('Erro no ficheiro de configuração')
+        print('Error on the configuration file.')
         exit(-1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tool_server_generator-0.3.3/tool_server_generator/config_server.txt` & `tool_server_generator-0.4/tool_server_generator/examples/config_server.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 * Servidor
 - Nome: Servidor
 - Diretoria: "teste"
-- IP: 127.0.0.1
 - Porta: 15213
 * Ferramentas
 --
 - Família:Grep
 - Título: "Grep"
 - Descrição: "grep  searches  for  PATTERNS in each FILE.  PATTERNS is one or more patterns separated by newline characters,
 and grep prints each line that matches a pattern.  Typically PATTERNS should be quoted when grep is used in  a
```

### Comparing `tool_server_generator-0.3.3/tool_server_generator/model/app.js` & `tool_server_generator-0.4/tool_server_generator/model/app.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.3/tool_server_generator/model/bin/www` & `tool_server_generator-0.4/tool_server_generator/model/bin/www`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.3/tool_server_generator/model/package-lock.json` & `tool_server_generator-0.4/tool_server_generator/model/package-lock.json`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.3/tool_server_generator/model/public/stylesheets/w3.css` & `tool_server_generator-0.4/tool_server_generator/model/public/stylesheets/w3.css`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.3/tool_server_generator/model/workers/process_command.js` & `tool_server_generator-0.4/tool_server_generator/model/workers/process_command.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -12,42 +12,61 @@
 const fs = require('fs')
 const path = require('path')
 
 parentPort.on('message', (msg) => {
     if (msg === 'start') {
         run_command()
         message = 'Work Done'
-        request_id = request.id
+        request_id = request.number
+        // avisar parent que terminou de processar a request
         parentPort.postMessage({
             id,
             message,
             request_id
         })
         return
     }
     throw new Error(`Unknown message: ${msg}`)
 })
 
+function datesEqual(a, b) {
+    return a.getTime() === b.getTime();
+}
+
 /**
  * Funcao para correr um comando
  */
 function run_command() {
     request_path = request.path
     command = request.command
-    console.log('Running command: ' + command)
+    console.log('Worker ' + id + ' with request ' + request.number + 'running command: ' + command)
     try {
+        // executar comando
         out = execSync(command, {
             cwd: request_path
         })
         console.log(out.toString());
         // Escrever ficheiros com output de terminal na pasta da request
-        out_file = path.join(request_path, `request_${request.id}_${Date.parse(request.date)}_stdout.txt`)
+        out_file = path.join(request_path, `request_${request.number}_${Date.parse(request.date)}_stdout.txt`)
         fs.writeFileSync(out_file, out.toString())
     } catch (err) {
         error = err.stderr.toString()
         console.log('Error:' + err);
         console.log('Stderr:' + error);
-        err_file = path.join(request_path, `request_${request.id}_${Date.parse(request.date)}_stderr.txt`)
+        err_file = path.join(request_path, `request_${request.number}_${Date.parse(request.date)}_stderr.txt`)
         fs.writeFileSync(err_file, error)
     }
+
+    //verifico se os ficheiros de inputs foram alterados, caso não são eliminados
+    files_times = request.files_times
+    for (filepath in files_times) {
+        old_mtime = files_times[filepath]
+        stats = fs.statSync(filepath)
+        new_mtime = stats.mtime
+
+        if (datesEqual(old_mtime, new_mtime)) {
+            fs.unlinkSync(filepath) //elimino o input
+        }
+    }
+
     console.log('Worker ' + id + ' done')
 }
```

### Comparing `tool_server_generator-0.3.3/tool_server_generator/utils/config_server.py` & `tool_server_generator-0.4/tool_server_generator/utils/config_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,94 +12,74 @@
 
 def config_server(server_dir,config_file):
     '''Modificar configuracoes do servidor'''
 
     # www file (ip and port changed)
     __www_file(f'{server_dir}/bin/www',config_file['ip'],config_file['porta'])
 
-    # layout.pug file (alterar titulo do layout)
-    __layout_pug_file(f'{server_dir}/views/layout.pug',config_file['nome'])
 
     #nome das ferramentas organizado por familias
     ferramentas = config_file['ferramentas']
     families = {family:list(tools.keys()) for family,tools in ferramentas.items()}
     #TODO: se calhar deviamos ordenar este dicionario por familia e a lista de nome de tools
     # ou deixamos pela ordem que ele meteu na config (que é a que está), podes escolher Braz
 
+    # layout.pug file (alterar titulo do layout)
+    __layout_pug_file(f'{server_dir}/views/layout.pug',config_file['nome'],families)
+
     # index.pug file (criar a view inicial do servidor com botoes para as ferramentas)
-    __index_pug_file(f'{server_dir}/views/index.pug',config_file['nome'],families)
+    #__index_pug_file(f'{server_dir}/views/index.pug',config_file['nome'],families)
 
     # {family}_{tool}.pug file (criar uma view para cada conjunto de ferramentas)
     __tool_pug_file(f'{server_dir}/views', config_file)
 
     # criar rota para cada familia e ferramenta
     __server_create_routes(f'{server_dir}/routes/index.js',config_file)
 
+    # alterar cores do css
+    __css_color_file(f'{server_dir}/public/stylesheets/color.css',config_file['visuais']['colors'])
+
 
 def __www_file(www_path,ip,porta):
     '''Modificar configuracoes do servidor, porta e ip'''
     www_file = open(www_path,'r')
     www = www_file.read()
     www_file.close()
     www = re.sub(r'\$ip',f'\"{ip}\"',www)
     www = re.sub(r'\$port',f'\"{porta}\"',www)
     www_file = open(www_path,'w')
     www_file.write(www)
     www_file.close()
 
-def __layout_pug_file(layout_path,nome):
+
+def __sidebar_tools(families):
+    sidebar = ""
+    for family,tools in families.items():
+        sidebar += f"""button.w3-button.w3-block.w3-left-align(onclick="open_tools('{family}')") {family} 
+            i.fa.fa-caret-down
+      .w3-hide(id="Grep")"""
+        for tool in tools:
+            sidebar += f"""
+        a.w3-bar-item.w3-button(href="/{family}/{tool}") {tool}"""
+    return sidebar
+
+def __layout_pug_file(layout_path,nome,families):
     '''Modificar configuracoes do layout, titulo'''
     layout_file = open(layout_path,'r')
     layout = layout_file.read()
     layout_file.close()
-    layout = re.sub(r'title=(.*)',f'title {nome}',layout)
+    layout = re.sub(r'\$title',f'{nome}',layout)
+    layout = re.sub(r'\$tools',__sidebar_tools(families),layout)
     layout_file = open(layout_path,'w')
     layout_file.write(layout)
     layout_file.close()
 
 
-def __index_pug_add_family(family,tools):
-    '''Retorna o pug do container de uma familia e das suas ferramentas para o index'''
-    index = ''
-    index += f"""
-        .w3-container
-            h2 {family}"""
-    for tool in tools:
-        tool_re = tool.replace(' ','_')
-        index += f'''
-            button.w3-btn
-                a(href="/{family}/{tool_re}") {tool}'''
-    return index
-
-def __index_pug_file(index_path, name, families):
-    '''Criar o index do servidor. '''
-    index_file = open(index_path,'w+')
-
-    # header
-    index = f"""extends layout
-
-block content
-    .w3-container.w3-indigo
-        h1 {name}
-    .w3-container"""
-
-    # adicionar familias e tools
-    for family,tools in families.items():
-        index += __index_pug_add_family(family,tools)
-        
-    # footer
-    index += f"""
-    .w3-container.w3-indigo
-        h3 Generated by Tools Server in 2023"""
-
-    index_file.write(index)
-    index_file.close()
-
 def __pug_input_field(type,id):
-    return f'''input.w3-input.w3-round(type="{html_types[type]}" name="{id}")'''
+    return f'''input.w3-input.w3-round.w3-border.border_color.primary_bg_color.primary_text_color(type="{html_types[type]}" name="{id}")'''
 
 
 def __tool_pug_file_desc(descricao):
     '''Retorna o pug da descricao de uma ferramenta'''
     pug = ''
     for line in descricao.splitlines():
                 pug += f'''
@@ -107,32 +87,49 @@
     return pug
 
 def __tool_pug_file_form(config):
     '''Retorna o pug do form de uma ferramenta'''
     inputs = config['inputs']
     pug =''
     pug +='''
-    form.w3-container.w3-indigo(method="post"'''
+            form.w3-container.w3-border.border_color(method="post"'''
     # permite upload de ficheiros se for o caso
     if config['n_files'] > 0:
-        pug += ',enctype="multipart/form-data"'
-    pug+=''')
-        fieldset
-            legend Inputs'''
+        pug += ',enctype="multipart/form-data",style="overflow: hidden;"'
+    pug+=''')'''
+
+    if len(inputs)>0:
+        pug+='''
+                h3 Inputs'''
     # botao para cada input
-    for id,input_dict in inputs:
+    for input in inputs:
+        id = input['id']
+        input_dict = input['opcoes']
         nome = input_dict['nome'] if input_dict['nome'] else id
         input_type = input_dict['tipo']
+        pug += '''
+                label.w3-left.label_color'''
+        if ('descricao' in input_dict):
+            descricao = input_dict['descricao']
+            pug += f'''
+                    p.w3-tooltip
+                        b {nome} 
+                        span.w3-text {descricao}'''
+        else:
+            pug += f'''
+                    b {nome}'''
         pug += f'''
-            label {nome}
-            {__pug_input_field(input_type,id)}
-'''
+                {__pug_input_field(input_type,id)}
+                br'''
     pug += f'''
-            input(type="hidden" name="command" value="{config['comando']}")
-        button.w3-btn.w3-purple.w3-mb-2(type="submit") Submit
+                input(type="hidden" name="command" value="{config['comando']}")
+                br
+                button.w3-button.secondary_bg_color.secondary_text_color.w3-mb-2(type="submit") Submit
+                br
+                br
 '''
     return pug
 
 
 def __tool_pug_file(path, server_config):
     ferramentas = server_config['ferramentas']
     base_route = server_config['rota']
@@ -141,39 +138,47 @@
         for tool,config in tools.items():
             tool_re = tool.replace(' ','_')
             descricao = config['descricao']
             # header
             pug = f'''
 extends layout
 block content
-    .w3-container.w3-indigo
-        h1 {tool}
+    .w3-container
+        h3 Description
 '''         
             # descricao
             pug += __tool_pug_file_desc(descricao)
-            
+
+            pug += """
+    .w3-container.secondary_bg_color.secondary_text_color
+        p
+    .w3-container
+        br
+        .w3-container(style="width:40%;margin:auto;")
+"""
             # form
             pug += __tool_pug_file_form(config)
             
-            # footer
             pug += f'''
-    .w3-container.w3-indigo
-        h3 Generated by Tools Server in 2023 - [#[a(href="{base_route}") Return]]    
+    br
 '''
             
             tool_file = open(f'{path}/{family}_{tool_re}.pug','w+')
             tool_file.write(pug)
             tool_file.close()
 
 
 def __server_create_routes_multer():
     '''Retorna o js necessario para a preparacao do multer'''
     index = ''
     index += '''
 const multer = require("multer")
+// criar pasta de uploads se nao houver
+if(!fs.existsSync(path.join('uploads')))
+    fs.mkdirSync(path.join('uploads'))
 const storageEngine = multer.diskStorage({
   destination: (req, file, cb) => { cb(null, './uploads') },
   filename: (req, file, cb) => { cb(null, Date.now() + '_' + file.originalname) }, })
         '''
     return index
 
 
@@ -181,18 +186,20 @@
     '''Retorna o js da rota de post para uma ferramenta que receba ficheiros de input'''
     tool_re = tool.replace(' ','_')
     index = ''
     # middleware para processamento dos inputs ficheiros
     index += f'''
 const upload_{family}_{tool_re} = multer({'{'} storage: storageEngine {'}'}).fields(['''
     # adicioanr field para cada input ficheiro
-    for input,opcoes in config['inputs']:
+    for input in config['inputs']:
+        id = input['id']
+        opcoes = input['opcoes']
         if opcoes['tipo'] == 'FILE':
             index +=f'''
-    {'{'} name: '{input}', maxCount: 1 {'}'},
+    {'{'} name: '{id}', maxCount: 1 {'}'},
                 '''
     index = index[:-1] # retirar ultima ','
     index += '''
     ]);
     '''
     # rota com middleware
     index += f'''
@@ -263,7 +270,22 @@
     # adicionar ultima linha (module.exports = router;)
     index += f'''
 {export_router}'''
     file = open(index_path,'w')
     file.write(index)
     file.close()
 
+
+def __change_color(css, tag, color):
+    return css.replace(tag,color)
+
+def __css_color_file(css_path,colors):
+    file = open(css_path, 'r')
+    css = file.read()
+    file.close()
+
+    for tag in colors:
+        css = __change_color(css,f'${tag}',colors[tag])
+
+    file = open(css_path,'w')
+    file.write(css)
+    file.close()
```

### Comparing `tool_server_generator-0.3.3/tool_server_generator/utils/utils.py` & `tool_server_generator-0.4/tool_server_generator/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,12 +6,12 @@
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawTextHelpFormatter,
         description=f'''
     --------------------------------------------------------------------
                         **Tool Server**
     --------------------------------------------------------------------'''
     )
-    parser.add_argument('config_file',metavar='filename',type=argparse.FileType('r'),nargs=1,help='configure file')
+    parser.add_argument('config_file',metavar='filename',type=str,nargs=1,help='configure file')
     parser.add_argument('-s','--start_server'   ,action='store_true'      ,help='starts server automatically')
     parser.add_argument('-ng','--ngrok'   ,action='store_true'      ,help='uses ngrok to expose port. Please make sure to have ngrok installed and authenticated.')
     return parser.parse_args()
```

