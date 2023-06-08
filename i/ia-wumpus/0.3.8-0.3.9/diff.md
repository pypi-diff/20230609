# Comparing `tmp/ia_wumpus-0.3.8.tar.gz` & `tmp/ia_wumpus-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.8.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.9.tar", max compression
```

## Comparing `ia_wumpus-0.3.8.tar` & `ia_wumpus-0.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.8/LICENSE
--rw-r--r--   0        0        0     4260 2023-05-31 03:35:24.780713 ia_wumpus-0.3.8/README.md
--rw-r--r--   0        0        0      636 2023-05-29 00:49:09.138275 ia_wumpus-0.3.8/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     8583 2023-05-31 03:35:25.048720 ia_wumpus-0.3.8/ia_wumpus/agente_reativo_v1.py
--rw-r--r--   0        0        0     8960 2023-05-29 00:49:09.162276 ia_wumpus-0.3.8/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.8/ia_wumpus/dinamica_agente_ambiente.py
--rw-r--r--   0        0        0      511 2023-05-31 03:35:25.108722 ia_wumpus-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4914 1970-01-01 00:00:00.000000 ia_wumpus-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4260 2023-05-31 03:35:24.780713 ia_wumpus-0.3.9/README.md
+-rw-r--r--   0        0        0      636 2023-05-29 00:49:09.138275 ia_wumpus-0.3.9/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     8670 2023-06-08 03:02:20.786412 ia_wumpus-0.3.9/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0     8960 2023-05-29 00:49:09.162276 ia_wumpus-0.3.9/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.9/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      513 2023-06-08 23:06:42.508627 ia_wumpus-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 ia_wumpus-0.3.9/PKG-INFO
```

### Comparing `ia_wumpus-0.3.8/LICENSE` & `ia_wumpus-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.8/README.md` & `ia_wumpus-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.8/ia_wumpus/__init__.py` & `ia_wumpus-0.3.9/ia_wumpus/__init__.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.8/ia_wumpus/agente_reativo_v1.py` & `ia_wumpus-0.3.9/ia_wumpus/agente_reativo_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,17 @@
         for i in pos_wumpus:
             for j in pos_agente:
                 if i == j:
                     # self.amb.clear()
                     console.print("\nWumpus Matou o Agente!", style="danger")
                     console.print(" \n============= Fim de Jogo =============",
                                   style="danger")
-                    console.print("          DERROTA DO AGENTE ",
-                                  style="danger")
+                    console.print(
+                        f"[blink][b]{' '*10}DERROTA DO AGENTE [/b][/blink]",
+                        style="danger")
                     console.print("=======================================\n",
                                   style="danger")
                     self.morreu = True
 
     def verificar_morte_agente_poco(self) -> None:
         """
         Método responsável por verificar se o agente moveu ao cair em um
@@ -108,16 +109,17 @@
             for j in pos_agente:
                 if i == j:
                     # self.amb.clear()
                     console.print("Agente caiu no poço e morreu!",
                                   style="danger")
                     console.print(" \n============= Fim de Jogo =============",
                                   style="danger")
-                    console.print("          DERROTA DO AGENTE ",
-                                  style="danger")
+                    console.print(
+                        f"[blink][b]{' '*10}DERROTA DO AGENTE [/b][/blink]",
+                        style="danger")
                     console.print("=======================================\n",
                                   style="danger")
                     self.morreu = True
 
     def pegar_outro(self) -> None:
         """
         Método usado para o agente pegar o ouro caso esteja na mesma posição
@@ -176,15 +178,15 @@
         return self.vitoria
 
     def ganhou_jogo(self) -> None:
         if self.pegou_ouro:
             if self.amb.get_pos_objetos()["agente"][0] == (0, 0):
                 console.print("\n============== Fim de Jogo ==============",
                               style="info")
-                console.print("          VITÓRIA DO AGENTE",
+                console.print(f"[blink]{' '*10}VITÓRIA DO AGENTE [/blink]",
                               style="info_bold")
                 console.print("=========================================\n",
                               style="info")
 
     def get_opcoes_mov_agente(self) -> List:
         return self.__list_opc_mov_ag
```

### Comparing `ia_wumpus-0.3.8/ia_wumpus/ambiente.py` & `ia_wumpus-0.3.9/ia_wumpus/ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.8/ia_wumpus/dinamica_agente_ambiente.py` & `ia_wumpus-0.3.9/ia_wumpus/dinamica_agente_ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.8/PKG-INFO` & `ia_wumpus-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3.8
+Version: 0.3.9
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: numpy (>=1.24.3)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Mundo do Wumpus - Intelegência Computacional
 
 Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
```

