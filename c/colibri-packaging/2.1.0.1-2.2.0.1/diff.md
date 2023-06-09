# Comparing `tmp/colibri-packaging-2.1.0.1.tar.gz` & `tmp/colibri-packaging-2.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\colibri-packaging-2.1.0.1.tar", last modified: Tue Feb 22 13:22:01 2022, max compression
+gzip compressed data, was "colibri-packaging-2.2.0.1.tar", last modified: Fri Jun  9 14:14:18 2023, max compression
```

## Comparing `colibri-packaging-2.1.0.1.tar` & `colibri-packaging-2.2.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-02-22 13:22:01.000000 colibri-packaging-2.1.0.1/
--rw-rw-rw-   0        0        0     1191 2018-08-14 12:50:16.000000 colibri-packaging-2.1.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0      546 2022-02-22 13:22:01.000000 colibri-packaging-2.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      344 2020-07-31 18:07:08.000000 colibri-packaging-2.1.0.1/README.rst
--rw-rw-rw-   0        0        0       18 2022-02-22 13:21:39.000000 colibri-packaging-2.1.0.1/__buildnumber__.py
--rw-rw-rw-   0        0        0       35 2022-02-22 13:14:28.000000 colibri-packaging-2.1.0.1/__version__.py
-drwxrwxrwx   0        0        0        0 2022-02-22 13:22:01.000000 colibri-packaging-2.1.0.1/colibri_packaging/
--rwxrwxrwx   0        0        0   587776 2018-08-14 12:50:16.000000 colibri-packaging-2.1.0.1/colibri_packaging/7za.exe
--rw-rw-rw-   0        0        0       97 2018-08-14 13:03:48.000000 colibri-packaging-2.1.0.1/colibri_packaging/__init__.py
--rw-rw-rw-   0        0        0     1936 2020-07-31 18:07:08.000000 colibri-packaging-2.1.0.1/colibri_packaging/__main__.py
--rw-rw-rw-   0        0        0     8887 2022-02-22 13:10:06.000000 colibri-packaging-2.1.0.1/colibri_packaging/empacotar.py
-drwxrwxrwx   0        0        0        0 2022-02-22 13:22:01.000000 colibri-packaging-2.1.0.1/colibri_packaging.egg-info/
--rw-rw-rw-   0        0        0      546 2022-02-22 13:21:59.000000 colibri-packaging-2.1.0.1/colibri_packaging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2022-02-22 13:21:59.000000 colibri-packaging-2.1.0.1/colibri_packaging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-22 13:21:59.000000 colibri-packaging-2.1.0.1/colibri_packaging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-02-22 13:21:59.000000 colibri-packaging-2.1.0.1/colibri_packaging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-22 13:22:01.000000 colibri-packaging-2.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1064 2018-08-14 12:50:16.000000 colibri-packaging-2.1.0.1/setup.py
--rw-rw-rw-   0        0        0      491 2018-08-14 12:50:16.000000 colibri-packaging-2.1.0.1/versao.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:14:18.448128 colibri-packaging-2.2.0.1/
+-rw-rw-rw-   0        0        0     1191 2018-08-14 12:50:16.000000 colibri-packaging-2.2.0.1/LICENCE.txt
+-rw-rw-rw-   0        0        0      771 2023-06-09 14:14:18.447128 colibri-packaging-2.2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-06-09 14:08:45.000000 colibri-packaging-2.2.0.1/README.rst
+-rw-rw-rw-   0        0        0       18 2023-06-09 14:14:17.000000 colibri-packaging-2.2.0.1/__buildnumber__.py
+-rw-rw-rw-   0        0        0       35 2023-06-08 14:51:49.000000 colibri-packaging-2.2.0.1/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:14:18.425615 colibri-packaging-2.2.0.1/colibri_packaging/
+-rwxrwxrwx   0        0        0   587776 2018-08-14 12:50:16.000000 colibri-packaging-2.2.0.1/colibri_packaging/7za.exe
+-rw-rw-rw-   0        0        0       97 2018-08-14 13:03:48.000000 colibri-packaging-2.2.0.1/colibri_packaging/__init__.py
+-rw-rw-rw-   0        0        0     1936 2020-07-31 18:07:08.000000 colibri-packaging-2.2.0.1/colibri_packaging/__main__.py
+-rw-rw-rw-   0        0        0     8899 2023-06-08 19:23:27.000000 colibri-packaging-2.2.0.1/colibri_packaging/empacotar.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:14:18.438611 colibri-packaging-2.2.0.1/colibri_packaging.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-06-09 14:14:18.000000 colibri-packaging-2.2.0.1/colibri_packaging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-06-09 14:14:18.000000 colibri-packaging-2.2.0.1/colibri_packaging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:14:18.000000 colibri-packaging-2.2.0.1/colibri_packaging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-09 14:14:18.000000 colibri-packaging-2.2.0.1/colibri_packaging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 14:14:18.449126 colibri-packaging-2.2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-06-09 13:51:14.000000 colibri-packaging-2.2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:14:18.442127 colibri-packaging-2.2.0.1/tests/
+-rw-rw-rw-   0        0        0     8361 2022-02-22 04:11:47.000000 colibri-packaging-2.2.0.1/tests/test_obter_arquivos.py
+-rw-rw-rw-   0        0        0      491 2018-08-14 12:50:16.000000 colibri-packaging-2.2.0.1/versao.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `colibri-packaging-2.1.0.1/LICENCE.txt` & `colibri-packaging-2.2.0.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `colibri-packaging-2.1.0.1/colibri_packaging/7za.exe` & `colibri-packaging-2.2.0.1/colibri_packaging/7za.exe`

 * *Files identical despite different names*

### Comparing `colibri-packaging-2.1.0.1/colibri_packaging/__main__.py` & `colibri-packaging-2.2.0.1/colibri_packaging/__main__.py`

 * *Files identical despite different names*

### Comparing `colibri-packaging-2.1.0.1/colibri_packaging/empacotar.py` & `colibri-packaging-2.2.0.1/colibri_packaging/empacotar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 # coding: utf-8
-from __future__ import print_function
 import json
 import logging
 import os
 import subprocess
 import re
-import sys
 import shutil
+from functools import cmp_to_key
 try:
     from scripts.versao_banco import obter_versao_db_scripts
 except ImportError:
     obter_versao_db_scripts = None
 
-PY3 = sys.version_info > (3,)
-if PY3:
-    from functools import cmp_to_key
 CAM_7ZA = os.path.join(os.path.split(__file__)[0] or os.getcwd(), '7za.exe')
 MANIFESTO_SERVER = 'manifesto.server'
 MANIFESTO_LOCAL = 'manifesto.local'
 MANIFESTO = 'manifesto.dat'
 EXTENSAO_PACOTE = '.cmpkg'
 RE_ARQ_SCRIPT = re.compile(r'_scripts(\d{0,2})(\S+)?\.zip')
 EXTENSAO_ARQ_SCRIPT = '.zip'
@@ -84,33 +80,33 @@
         if arq.endswith(EXTENSAO_PACOTE) and arq.startswith(prefixo):
             try:
                 os.unlink(os.path.join(pasta, arq))
             except Exception:
                 logger.exception('Falha ao remover cmpkg anterior: ' + arq)
 
 
-def obter_arquivos(pasta, configs, lista_no_diretorio):
+def obter_arquivos(pasta, manifesto_dat, lista_no_diretorio):
     lista_zip = list((os.path.join(pasta, MANIFESTO),))
-    lista_anterior = configs.get(ARQUIVOS, list())
+    lista_anterior = manifesto_dat.get(ARQUIVOS, list())
 
-    configs[ARQUIVOS] = list()
+    manifesto_dat[ARQUIVOS] = list()
 
     def criar_arq_(arq, chaves=None):
         dictarq = dict(
             nome=arq
         )
 
         if chaves is not None:
             dictarq.update(_obter_chaves_arquivo(chaves))
 
         if dictarq.get('destino') is None:
             dictarq['destino'] = _acha_tipo(arq)
 
         if dictarq.get('destino'):
-            configs[ARQUIVOS].append(dictarq)
+            manifesto_dat[ARQUIVOS].append(dictarq)
             completo = os.path.join(pasta, arq)
             if completo not in lista_zip:
                 lista_zip.append(completo)
         elif arq.lower().endswith('.exe'):
             raise RuntimeError(
                 f"Arquivo executável desconhecido na pasta de empacotamento: {arq}"
             )
@@ -148,128 +144,136 @@
                 f"Pattern de nome arquivo não foi encontrado: {a['_pattern_nome']}"
             )
         elif 'nome' in a and "__count" not in a:
             raise RuntimeError(
                 f"Nome arquivo não foi encontrado: {a['nome']}"
             )
 
-    if PY3:
-        configs[ARQUIVOS].sort(
-            key=cmp_to_key(
-                lambda arq1, arq2: _acha_ordem(arq1) - _acha_ordem(arq2)
-            )
-        )
-    else:
-        configs[ARQUIVOS].sort(
-            cmp=lambda arq1, arq2: _acha_ordem(arq1) - _acha_ordem(arq2)
+    manifesto_dat[ARQUIVOS].sort(
+        key=cmp_to_key(
+            lambda arq1, arq2: _acha_ordem(arq1) - _acha_ordem(arq2)
         )
+    )
     return lista_zip
 
 
-def obter_versoes_bases(configs, kwargs):
+def _atualizar_versoes_bases(manifesto_dat, kwargs):
     OBTER = '_obter_versao_do_json'
     versoes_bases = [
         dict(schema=a[0], versao=a[1]) for a in kwargs.pop('versoes_bases', [])
     ]
     schemas = [a[SCHEMA] for a in versoes_bases]
 
-    for base in configs.get(BASES_COMPATIVEIS, []):
+    for base in manifesto_dat.get(BASES_COMPATIVEIS, []):
         obter = base.get(OBTER)
         if obter:
             if obter_versao_db_scripts is None:
                 raise RuntimeError('Biblioteca de scripts indisponivel')
             schema, versao = obter_versao_db_scripts(obter)
             base[SCHEMA] = schema
             base[VERSAO] = versao
             del base[OBTER]
         if base.get(SCHEMA) and base.get(SCHEMA) not in schemas:
             versoes_bases.append(base)
 
     if len(versoes_bases):
-        configs[BASES_COMPATIVEIS] = versoes_bases
+        manifesto_dat[BASES_COMPATIVEIS] = versoes_bases
 
 
-def empacotar(pasta, pasta_saida, senha, **kwargs):
+def _obter_manifesto_do_template(pasta):
+    manifesto_usado = os.path.join(pasta, MANIFESTO_SERVER)
     try:
-        manifesto_usado = os.path.join(pasta, MANIFESTO_SERVER)
         with open(manifesto_usado, 'r', encoding='utf-8-sig') as arq:
-            configs = json.load(arq)
+            manifesto_dat = json.load(arq)
             logger.info('usando ' + MANIFESTO_SERVER)
     except IOError:
         try:
             manifesto_usado = os.path.join(pasta, MANIFESTO_LOCAL)
             with open(manifesto_usado, 'r', encoding='utf-8-sig') as arq:
-                configs = json.load(arq)
+                manifesto_dat = json.load(arq)
                 logger.info('usando ' + MANIFESTO_LOCAL)
         except IOError:
             logger.info(u'template de manifesto não encontrado. gerando...')
-            configs = DEFAULTS_PACOTE.copy()
+            manifesto_dat = DEFAULTS_PACOTE.copy()
     except Exception as e:
-        logger.exception('Erro ao processar manifesto %s', manifesto_usado)
+        logger.exception(f'Erro ao processar manifesto {manifesto_usado}')
         print('Erro ao processar: ' + manifesto_usado)
         print(e)
         raise
+    return manifesto_dat
+
+
+def empacotar(pasta, pasta_saida, senha, **kwargs):
+    manifesto_dat = _obter_manifesto_do_template(pasta)
 
     # Atualizo o manifesto com o que foi passado pela linha de comando
-    obter_versoes_bases(configs, kwargs)
-    configs.update(kwargs)
+    _atualizar_versoes_bases(manifesto_dat, kwargs)
+    manifesto_dat.update(kwargs)
 
-    arquivos = obter_arquivos(pasta, configs, os.listdir(pasta))
+    arquivos = obter_arquivos(pasta, manifesto_dat, os.listdir(pasta))
 
     with open(os.path.join(pasta, MANIFESTO), 'w') as manifile:
-        json.dump(configs, manifile, indent=2)
+        json.dump(manifesto_dat, manifile, indent=2)
 
-    prefixo = configs[PACOTE].replace(' ', '') + '_'
+    prefixo = manifesto_dat[PACOTE].replace(' ', '') + '_'
     nome_cmpkg = prefixo + \
-        configs[VERSAO].replace(' ', '').replace('.', '_') + \
+        manifesto_dat[VERSAO].replace(' ', '').replace('.', '_') + \
         EXTENSAO_PACOTE
     saida = os.path.join(pasta_saida, nome_cmpkg)
 
     _excluir_com_prefixo(pasta_saida, prefixo)
     zipar(saida, arquivos=arquivos, senha=senha)
     arquivo_cmpkg = os.path.join(os.getcwd(), saida)
 
     # Suporte a uma pasta para os QAs
-    if os.environ.get('QA', '').lower() == 'true':
-        if os.environ.get('ALOHA', '').lower() == 'true':
-            logger.error('Arquivo não será gerado na pasta de QA pois ALOHA=true')
-            return
-        pasta_QA = os.environ.get('PASTA_QA', PASTA_QA)
-        if not os.path.exists(pasta_QA):
-            logger.error(f'PASTA_QA nao encontrada: {pasta_QA}')
-        else:
-            _excluir_com_prefixo(pasta_QA, prefixo)
-            try:
-                print(f'Copiando para pasta de QA: {pasta_QA}')
-                shutil.copyfile(saida, os.path.join(pasta_QA, nome_cmpkg))
-            except Exception:
-                logger.exception(
-                    f'Falha ao copiar arquivo {saida} para a pasta {pasta_QA}'
-                )
+    _copiar_para_qa(nome_cmpkg, prefixo, saida)
 
     return arquivo_cmpkg
 
 
+def _copiar_para_qa(nome_cmpkg, prefixo, saida):
+    if os.environ.get('QA', '').lower() != 'true':
+        return
+
+    if os.environ.get('ALOHA', '').lower() == 'true':
+        logger.info('Arquivo não será gerado na pasta de QA pois ALOHA=true')
+        return
+
+    pasta_QA = os.environ.get('PASTA_QA', PASTA_QA)
+    if not os.path.exists(pasta_QA):
+        logger.error(f'PASTA_QA nao encontrada: {pasta_QA}')
+        return
+
+    _excluir_com_prefixo(pasta_QA, prefixo)
+    try:
+        print(f'Copiando para pasta de QA: {pasta_QA}')
+        shutil.copyfile(saida, os.path.join(pasta_QA, nome_cmpkg))
+    except Exception:
+        logger.exception(
+            f'Falha ao copiar arquivo {saida} para a pasta {pasta_QA}'
+        )
+
+
 def zipar(destino, arquivos=None, pasta=None, senha=''):
     destino = os.path.join(os.getcwd(), destino)
 
     cmdline = [
         CAM_7ZA,
         'a',
         '-tzip',
         '-mx9',
         '-y'
     ]
     if senha:
         cmdline.append('-p' + senha)
     cmdline.append(destino)
 
+    prevdir = None
     if arquivos:
         cmdline = cmdline + arquivos
-        prevdir = None
     elif pasta:
         prevdir = os.getcwd()
         pasta = os.path.join(os.getcwd(), pasta)
         os.chdir(pasta)
 
     logger.debug('comando gerado: "{}"'.format(cmdline))
     subprocess.call(cmdline)
```

