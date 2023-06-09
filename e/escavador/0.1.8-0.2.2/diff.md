# Comparing `tmp/escavador-0.1.8.tar.gz` & `tmp/escavador-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escavador-0.1.8.tar", max compression
+gzip compressed data, was "escavador-0.2.2.tar", max compression
```

## Comparing `escavador-0.1.8.tar` & `escavador-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,38 @@
--rw-r--r--   0        0        0     1065 2023-04-14 19:57:07.301640 escavador-0.1.8/LICENSE
--rw-r--r--   0        0        0     3791 2023-04-14 19:57:07.301640 escavador-0.1.8/README.md
--rw-r--r--   0        0        0      230 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/__init__.py
--rw-r--r--   0        0        0     1675 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/api.py
--rw-r--r--   0        0        0       52 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/exceptions.py
--rw-r--r--   0        0        0      528 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/method.py
--rw-r--r--   0        0        0      704 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/__init__.py
--rw-r--r--   0        0        0     1060 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/busca.py
--rw-r--r--   0        0        0      570 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/busca_assincrona.py
--rw-r--r--   0        0        0     1973 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/callback.py
--rw-r--r--   0        0        0     1518 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/diario_oficial.py
--rw-r--r--   0        0        0        0 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/__init__.py
--rw-r--r--   0        0        0      842 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/documento.py
--rw-r--r--   0        0        0      119 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/endpoint.py
--rw-r--r--   0        0        0      721 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/enums.py
--rw-r--r--   0        0        0     1567 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/instituicao.py
--rw-r--r--   0        0        0     3237 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/jurisprudencia.py
--rw-r--r--   0        0        0     2357 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/legislacao.py
--rw-r--r--   0        0        0     4144 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/monitoramento_diario.py
--rw-r--r--   0        0        0     2411 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/monitoramento_tribunal.py
--rw-r--r--   0        0        0      393 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/movimentacao.py
--rw-r--r--   0        0        0      938 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/pessoa.py
--rw-r--r--   0        0        0    10603 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/processo.py
--rw-r--r--   0        0        0      296 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/saldo.py
--rw-r--r--   0        0        0      602 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/tribunal.py
--rw-r--r--   0        0        0      693 2023-04-14 19:57:07.301640 escavador-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 escavador-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-09 19:18:32.316446 escavador-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8335 2023-06-09 19:18:32.316446 escavador-0.2.2/README.md
+-rw-r--r--   0        0        0      724 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/__init__.py
+-rw-r--r--   0        0        0     3180 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/api.py
+-rw-r--r--   0        0        0     1444 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/exceptions.py
+-rw-r--r--   0        0        0     3037 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/method.py
+-rw-r--r--   0        0        0      449 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/helpers/__init__.py
+-rw-r--r--   0        0        0     1301 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/helpers/consume_cursor.py
+-rw-r--r--   0        0        0      774 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/helpers/documento.py
+-rw-r--r--   0        0        0     1193 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/helpers/endpoint.py
+-rw-r--r--   0        0        0       47 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/helpers/enums.py
+-rw-r--r--   0        0        0      721 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/helpers/enums_v1.py
+-rw-r--r--   0        0        0     2314 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/resources/helpers/enums_v2.py
+-rw-r--r--   0        0        0      664 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:18:32.316446 escavador-0.2.2/escavador/v1/resources/__init__.py
+-rw-r--r--   0        0        0     1131 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/busca.py
+-rw-r--r--   0        0        0      657 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/busca_assincrona.py
+-rw-r--r--   0        0        0     2074 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/callback.py
+-rw-r--r--   0        0        0     1614 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/diario_oficial.py
+-rw-r--r--   0        0        0     1668 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/instituicao.py
+-rw-r--r--   0        0        0     3352 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/jurisprudencia.py
+-rw-r--r--   0        0        0     2473 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/legislacao.py
+-rw-r--r--   0        0        0     4325 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/monitoramento_diario.py
+-rw-r--r--   0        0        0     2545 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/monitoramento_tribunal.py
+-rw-r--r--   0        0        0      464 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/movimentacao.py
+-rw-r--r--   0        0        0     1024 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/pessoa.py
+-rw-r--r--   0        0        0    10785 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/processo.py
+-rw-r--r--   0        0        0      368 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/saldo.py
+-rw-r--r--   0        0        0      689 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v1/resources/tribunal.py
+-rw-r--r--   0        0        0      174 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v2/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v2/resources/__init__.py
+-rw-r--r--   0        0        0     6873 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v2/resources/envolvido.py
+-rw-r--r--   0        0        0     4579 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v2/resources/movimentacao.py
+-rw-r--r--   0        0        0    23070 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v2/resources/processo.py
+-rw-r--r--   0        0        0      978 2023-06-09 19:18:32.320446 escavador-0.2.2/escavador/v2/resources/tribunal.py
+-rw-r--r--   0        0        0      743 2023-06-09 19:18:32.320446 escavador-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9420 1970-01-01 00:00:00.000000 escavador-0.2.2/PKG-INFO
```

### Comparing `escavador-0.1.8/LICENSE` & `escavador-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `escavador-0.1.8/escavador/resources/busca.py` & `escavador-0.2.2/escavador/v1/resources/busca.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from typing import Optional, Dict
 from escavador.resources.helpers.enums import TiposTermo
 
 
-class Busca(Endpoint):
+class Busca(EndpointV1):
 
-    def busca_termo(self, termo: str, tipo_termo: TiposTermo, *, limit: Optional[int] = None,
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def busca_termo(cls, termo: str, tipo_termo: TiposTermo, *, limit: Optional[int] = None,
                     page: Optional[int] = None) -> Dict:
         """
         Pesquisa um termo no escavador
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :param termo: o termo a ser pesquisado
         :param tipo_termo: Tipo da entidade a ser pesquisada(
@@ -24,8 +28,8 @@
 
         data = {
             'q': termo,
             'qo': tipo_termo.value,
             'limit': limit,
             'page': page
         }
-        return self.methods.get("busca", data=data)
+        return cls.methods.get("busca", data=data)
```

### Comparing `escavador-0.1.8/escavador/resources/callback.py` & `escavador-0.2.2/escavador/v1/resources/callback.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from datetime import datetime
 
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from typing import Optional, List, Dict
 
 from escavador.resources.helpers.enums import StatusCallback
 
 
-class Callback(Endpoint):
+class Callback(EndpointV1):
 
-    def callbacks(self, *, data_maxima: Optional[datetime] = None, data_minima: Optional[datetime] = None,
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def callbacks(cls, *, data_maxima: Optional[datetime] = None, data_minima: Optional[datetime] = None,
             evento: Optional[str] = None, item_tipo: Optional[str] = None, item_id: Optional[int] = None,
             status: Optional[StatusCallback]) -> Dict:
         """
         Retorna todos os callbacks, de acordo com os filtros enviados
         :param item_id:o id do item do callback, obrigatório se o item_tipo foi enviado
         :param item_tipo: o tipo do item do callback e.g: busca_assincrona, monitoramento_tribunal, monitoramento_diario
         :param evento: o evento do callback
@@ -27,30 +31,32 @@
             "data_minima": data_minima.strftime("%Y-%m-%d %H:%M:%S") if data_minima else None,
             "evento": evento,
             "item_tipo": item_tipo,
             "item_id": item_id,
             "status": status.value
         }
 
-        return self.methods.get('callbacks', data=data)
+        return cls.methods.get('callbacks', data=data)
 
-    def marcarRecebido(self, ids: List) -> Dict:
+    @classmethod
+    def marcarRecebido(cls, ids: List) -> Dict:
         """
         Marca callbacks como recebidos
-        :param ids:lista com ids dos callbacks que serão marcardos como recebidos
+        :param ids:lista com ids dos callbacks que serão marcados como recebidos
         :return: Dict
         """
 
         data = {
             'ids': ids
         }
 
-        return self.methods.post('callbacks/marcar-recebidos',data=data)
+        return cls.methods.post('callbacks/marcar-recebidos', data=data)
 
-    def reenviar(self, id: int) -> Dict:
+    @classmethod
+    def reenviar(cls, id: int) -> Dict:
         """
         Reenvia uma callback
         :param id: id do callback
         :return: Dict
         """
 
-        return self.methods.post(f'callbacks/{id}/reenviar')
+        return cls.methods.post(f'callbacks/{id}/reenviar')
```

### Comparing `escavador-0.1.8/escavador/resources/diario_oficial.py` & `escavador-0.2.2/escavador/v1/resources/diario_oficial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from escavador.resources.helpers.documento import Documento
 from typing import Optional, Dict
 
 
-class DiarioOficial(Endpoint):
+class DiarioOficial(EndpointV1):
 
-    def origens(self) -> Dict:
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def origens(cls) -> Dict:
         """
         Retorna as origens de todos os diários disponiveis no Escavador.
         :return: Dict
         """
-        return self.methods.get("origens")
+        return cls.methods.get("origens")
 
-    def pagina(self, id_diario: int, *, page: Optional[int] = None) -> Dict:
+    @classmethod
+    def pagina(cls, id_diario: int, *, page: Optional[int] = None) -> Dict:
         """
         Retorna uma página específica do Diário Oficial pelo seu identificador no Escavador.
         :param id_diario: o ID do diario oficial
         :param page: número da página do diário oficial
         :return: Dict
         """
         data = {
             "page": page
         }
 
-        return self.methods.get(f"diarios/{id_diario}", data=data)
+        return cls.methods.get(f"diarios/{id_diario}", data=data)
 
-    def download_pdf_pagina(self, id_diario: int, page: int, path: str, nome_arquivo: str) -> Dict:
+    @classmethod
+    def download_pdf_pagina(cls, id_diario: int, page: int, path: str, nome_arquivo: str) -> Dict:
         """
         Retorna em formato PDF, uma página do Diário Oficial pelo seu identificador
         :param nome_arquivo:nome para o arquivo baixado
         :param path: diretorio onde o arquivo será salvo
         :param id_diario: o ID do diario oficial
         :param page: número da página do diário oficial
         :return: Dict
         """
-        conteudo = self.methods.get(f"diarios/{id_diario}/pdf/pagina/{page}/baixar")
+        conteudo = cls.methods.get(f"diarios/{id_diario}/pdf/pagina/{page}/baixar")
 
-        if conteudo['sucesso'] is True:
-            return Documento.get_pdf(conteudo, path, nome_arquivo)
-        else:
+        if type(conteudo) is dict:
             return conteudo
+        else:
+            return Documento.get_pdf(conteudo, path, nome_arquivo)
```

### Comparing `escavador-0.1.8/escavador/resources/helpers/documento.py` & `escavador-0.2.2/escavador/resources/helpers/documento.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,13 +13,10 @@
         :param path: caminho onde o pdf será salvo
         :return: dict
         """
         real_path = Path(path) / f"{nome_arquivo}.pdf"
         try:
             with open(real_path, "xb+") as arquivo:
                 arquivo.write(conteudo)
-        except FileExistsError as error:
+        except (FileExistsError, FileNotFoundError) as error:
             return {"error": error.strerror}
-        except FileNotFoundError as error:
-            return {"error": error.strerror}
-
         return {"path": real_path}
```

### Comparing `escavador-0.1.8/escavador/resources/helpers/enums.py` & `escavador-0.2.2/escavador/resources/helpers/enums_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,32 +7,32 @@
     INSTITUICOES = "i"
     PATENTES = "pa"
     DIARIOS_OFICIAIS = "d"
     ENVOLVIDOS = "en"
 
 
 class TiposBusca(Enum):
-    BUSCA_POR_OAB = 'busca_por_oab'
-    BUSCA_POR_DOCUMENTO = 'busca_por_documento'
-    BUSCA_POR_NOME = 'busca_por_nome'
+    BUSCA_POR_OAB = "busca_por_oab"
+    BUSCA_POR_DOCUMENTO = "busca_por_documento"
+    BUSCA_POR_NOME = "busca_por_nome"
 
 
 class TiposMonitoramentosTribunal(Enum):
-    UNICO = 'UNICO'
-    NUMERO_DOCUMENTO = 'NUMDOC'
-    NOME = 'NOME'
+    UNICO = "UNICO"
+    NUMERO_DOCUMENTO = "NUMDOC"
+    NOME = "NOME"
 
 
 class TiposMonitoramentosDiario(Enum):
-    PROCESSO = 'processo'
-    TERMO = 'termo'
+    PROCESSO = "processo"
+    TERMO = "termo"
 
 
 class FrequenciaMonitoramentoTribunal(Enum):
-    DIARIA = 'DIARIA'
-    SEMANAL = 'SEMANAL'
+    DIARIA = "DIARIA"
+    SEMANAL = "SEMANAL"
 
 
 class StatusCallback(Enum):
     SUCESSO = "sucesso"
     EM_TENTATIVA = "em_tentativa"
     ERRO = "erro"
```

### Comparing `escavador-0.1.8/escavador/resources/jurisprudencia.py` & `escavador-0.2.2/escavador/v1/resources/jurisprudencia.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from escavador.resources.helpers.documento import Documento
 from typing import Optional, Dict, List
-from datetime import  datetime
+from datetime import datetime
 
 
-class Jurisprudencia(Endpoint):
+class Jurisprudencia(EndpointV1):
 
-    def filtros_busca_jurisprudencia(self) -> Dict:
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def filtros_busca_jurisprudencia(cls) -> Dict:
         """
         Lista de filtros disponíveis para a busca de jurisprudências,
         Para cada item da lista de filtros, o campo filtro representa a chave (key) da query.
         No campo opcoes, listamos todas as opções de valor para aquele filtro, e, para cada opção,
          o campo valor representa o valor (value) da query.
         :return: Dict
         """
-        return self.methods.get("jurisprudencias")
+        return cls.methods.get("jurisprudencias")
 
-    def busca_por_jurisprudencias(self, termo: str, *, ordena_por: Optional[str] = None, de_data: Optional[datetime] = None,
+    @classmethod
+    def busca_por_jurisprudencias(cls, termo: str, *, ordena_por: Optional[str] = None, de_data: Optional[datetime] = None,
                                   ate_data: Optional[datetime] = None, pagina: Optional[int] = None,
                                   filtros: Optional[List[Dict]] = None) -> Dict:
         """
         Traz a lista paginada dos itens encontrados na busca.
         :param filtros: filtros listados pelo método filtros_busca_jurisprudencia()
         :param pagina: lista os itens de uma página
         :param ate_data: filtra os resultados com data de julgamento limite até a data informada
@@ -38,37 +43,39 @@
             'pagina': pagina,
         }
 
         if filtros:
             for filtro in filtros:
                 data.update(filtro)
 
-        return self.methods.get('jurisprudencias/busca', data=data)
+        return cls.methods.get('jurisprudencias/busca', data=data)
 
-    def get_documento_jurisprudencia(self, tipo_documento: str, id_documento: int) -> Dict:
+    @classmethod
+    def get_documento_jurisprudencia(cls, tipo_documento: str, id_documento: int) -> Dict:
         """
         Traz informações sobre um documento de Jurisprudência em específico
         :param tipo_documento: o tipo de documento
         :param id_documento: o ID do documento
         :return Dict
         """
 
-        return self.methods.get(f"jurisprudencias/documento/{tipo_documento}/{id_documento}")
+        return cls.methods.get(f"jurisprudencias/documento/{tipo_documento}/{id_documento}")
 
-    def download_documento_jurisprudencia(self, tipo_documento: str, id_documento: int, id_arquivo: str, path: str,
+    @classmethod
+    def download_documento_jurisprudencia(cls, tipo_documento: str, id_documento: int, id_arquivo: str, path: str,
                                           nome_arquivo: str) -> Dict:
         """
         Retorna, em formato PDF, um documento de jurisprudência
          :param tipo_documento: o tipo de documento
         :param id_documento: o ID do documento
         :param id_arquivo: o ID do arquivo do documento
         :param path: caminho onde o pdf será salvo
         :param nome_arquivo: nome do arquivo a ser criado
         :return: Dict
         """
 
-        conteudo = self.methods.get(f"jurisprudencias/pdf/{tipo_documento}/{id_documento}/{id_arquivo}")
+        conteudo = cls.methods.get(f"jurisprudencias/pdf/{tipo_documento}/{id_documento}/{id_arquivo}")
 
         if conteudo['sucesso'] is True:
             return Documento.get_pdf(conteudo, path, nome_arquivo)
         else:
             return conteudo
```

### Comparing `escavador-0.1.8/escavador/resources/legislacao.py` & `escavador-0.2.2/escavador/v1/resources/legislacao.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from typing import Optional, Dict
 from datetime import datetime
 
 
-class Legislacao(Endpoint):
+class Legislacao(EndpointV1):
 
-    def filtros_busca_legislacao(self) -> Dict:
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def filtros_busca_legislacao(cls) -> Dict:
         """
         Lista de filtros disponíveis para a busca de Legislação
         :return: Dict
         """
-        return self.methods.get("legislacoes")
+        return cls.methods.get("legislacoes")
 
-    def busca_por_legislacao(self, termo: str, *, ordena_por: Optional[str] = None, de_data: Optional[datetime] = None,
+    @classmethod
+    def busca_por_legislacao(cls, termo: str, *, ordena_por: Optional[str] = None, de_data: Optional[datetime] = None,
                              ate_data: Optional[datetime] = None, pagina: Optional[int] = None,
                              filtro: Optional[str] = None) -> Dict:
         """
         Traz a lista paginada dos itens encontrados na busca.
         :param filtro: Um dos filtros listados pelo método filtros_busca_jurisprudencia()
         :param pagina: lista os itens de uma página
         :param ate_data: filtra os resultados com data de julgamento limite até a data informada
@@ -31,28 +36,30 @@
             'ordena_por': ordena_por,
             'de_data': de_data.strftime("%Y%m%d") if de_data else None,
             'ate_data': ate_data.strftime("%Y%m%d") if ate_data else None,
             'pagina': pagina,
             'filtro': filtro
         }
 
-        return self.methods.get('legislacoes/busca', data=data)
+        return cls.methods.get('legislacoes/busca', data=data)
 
-    def get_documento_legislacao(self, tipo_documento: str, id_documento: int) -> Dict:
+    @classmethod
+    def get_documento_legislacao(cls, tipo_documento: str, id_documento: int) -> Dict:
         """
         Traz informações sobre um documento de Legislação
         :param tipo_documento: O tipo do Documento
         :param id_documento: O ID do documento
         :return Dict
         """
 
-        return self.methods.get(f"legislacoes/documento/{tipo_documento}/{id_documento}")
+        return cls.methods.get(f"legislacoes/documento/{tipo_documento}/{id_documento}")
 
-    def fragmentos_texto_legislacao(self, tipo_documento: str, id_documento: int) -> Dict:
+    @classmethod
+    def fragmentos_texto_legislacao(cls, tipo_documento: str, id_documento: int) -> Dict:
         """
         Traz os fragmentos de uma legislação paginados.
         :param tipo_documento: O tipo do Documento
         :param id_documento: O ID do documento
         :return: Dict
         """
 
-        return self.methods.get(f"legislacoes/pdf/{tipo_documento}/{id_documento}/fragmentos")
+        return cls.methods.get(f"legislacoes/pdf/{tipo_documento}/{id_documento}/fragmentos")
```

### Comparing `escavador-0.1.8/escavador/resources/monitoramento_diario.py` & `escavador-0.2.2/escavador/v1/resources/monitoramento_diario.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from typing import Optional, List, Dict
-from escavador.resources.helpers.enums import TiposMonitoramentosDiario
+from escavador.resources.helpers.enums_v1 import TiposMonitoramentosDiario
 
-class MonitoramentoDiario(Endpoint):
 
-    def origens(self, id_monitoramento: int) -> Dict:
+class MonitoramentoDiario(EndpointV1):
+
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def origens(cls, id_monitoramento: int) -> Dict:
         """
         Retorna os diários oficiais de um monitoramento
         :param id_monitoramento: o ID do monitoramento
         :return: Dict
         """
 
-        return self.methods.get(f"monitoramentos/{id_monitoramento}/origens")
+        return cls.methods.get(f"monitoramentos/{id_monitoramento}/origens")
 
-    def criar(self, tipo_monitoramento: TiposMonitoramentosDiario, *, termo: Optional[str] = None,
+    @classmethod
+    def criar(cls, tipo_monitoramento: TiposMonitoramentosDiario, *, termo: Optional[str] = None,
                             origens_ids: Optional[List[int]] = None, processo_id: Optional[int] = None,
                             variacoes: Optional[List[str]] = None, termos_auxiliares: Optional[List[str]] = None
                             ) -> Dict:
         """
         Cria um novo monitoramento para termos ou processos
         :param termos_auxiliares: Array de array de strings com termos e condições
         :param variacoes: array de strings com as variações do termo monitorado.
@@ -33,72 +39,78 @@
             'termo': termo,
             'origens_ids': origens_ids,
             'processo_id': processo_id,
             'variacoes': variacoes,
             'termos_auxiliares': termos_auxiliares
         }
 
-        return self.methods.post("monitoramentos", data=data)
+        return cls.methods.post("monitoramentos", data=data)
 
-    def monitoramentos(self) -> Dict:
+    @classmethod
+    def monitoramentos(cls) -> Dict:
         """
         Retorna todos os monitoramentos de diários oficiais do usuário
         :return: Dict
         """
 
-        return self.methods.get("monitoramentos")
+        return cls.methods.get("monitoramentos")
 
-    def por_id(self, id_monitoramento: int) -> Dict:
+    @classmethod
+    def por_id(cls, id_monitoramento: int) -> Dict:
         """
         Retorna um monitoramento de diários oficiais de acordo com seu ID
         :param id_monitoramento o ID do monitoramento
         :return: Dict
         """
 
-        return self.methods.get(f"monitoramentos/{id_monitoramento}")
+        return cls.methods.get(f"monitoramentos/{id_monitoramento}")
 
-    def editar(self, id_monitoramento: int, *, variacoes: Optional[List[str]] = None,
+    @classmethod
+    def editar(cls, id_monitoramento: int, *, variacoes: Optional[List[str]] = None,
                              origens_ids: Optional[List[str]] = None) -> Dict:
         """
         Edita os diários oficiais e as variações do termo do monitoramento
         :param id_monitoramento: o ID do monitoramento
         :param origens_ids: array de ids dos diarios que deseja monitorar
         :param variacoes: array de strings com as variações do termo monitorado.
         :return: Dict
         """
         data = {
             'variacoes': variacoes,
             'origens_ids': origens_ids
         }
 
-        return self.methods.put(f"monitoramentos/{id_monitoramento}", data=data)
+        return cls.methods.put(f"monitoramentos/{id_monitoramento}", data=data)
 
-    def remover(self, id_monitoramento: int) -> Dict:
+    @classmethod
+    def remover(cls, id_monitoramento: int) -> Dict:
         """
         Remove um monitoramento de acordo com seu ID
         :param id_monitoramento: o ID do monitoramento
         :return: Dict
         """
 
-        return self.methods.delete(f"monitoramentos/{id_monitoramento}")
+        return cls.methods.delete(f"monitoramentos/{id_monitoramento}")
 
-    def aparicoes(self, id_monitoramento: int) -> Dict:
+    @classmethod
+    def aparicoes(cls, id_monitoramento: int) -> Dict:
         """
         Retorna as aparições de um monitoramento pelo identificador do monitoramento.
         :param id_monitoramento: O ID do monitoramento
         :return: Dict
         """
 
-        return self.methods.get(f"monitoramentos/{id_monitoramento}/aparicoes")
+        return cls.methods.get(f"monitoramentos/{id_monitoramento}/aparicoes")
 
-    def test_callback_monitoramento(self, callback_url: str, *, tipo: Optional[str] = None) -> Dict:
+    @classmethod
+    def test_callback_monitoramento(cls, callback_url: str, *, tipo: Optional[str] = None) -> Dict:
         """
         Testa se a ulr de callback do usuário pode receber callbacks com resultados de monitoramentos
         :param callback_url: a url que o callback será enviado
         :param tipo o tipo de objeto do callback (movimentacao ou diario)
         :return: Dict
         """
         data = {
             'callback_url': callback_url,
             'tipo': tipo
         }
-        return self.methods.post("monitoramentos/testcallback", data=data)
+        return cls.methods.post("monitoramentos/testcallback", data=data)
```

### Comparing `escavador-0.1.8/escavador/resources/monitoramento_tribunal.py` & `escavador-0.2.2/escavador/v1/resources/monitoramento_tribunal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from typing import Optional, Dict
-from escavador.resources.helpers.enums import TiposMonitoramentosTribunal, FrequenciaMonitoramentoTribunal
+from escavador.resources.helpers.enums_v1 import TiposMonitoramentosTribunal, FrequenciaMonitoramentoTribunal
 
 
-class MonitoramentoTribunal(Endpoint):
+class MonitoramentoTribunal(EndpointV1):
 
-    def monitoramentos(self) -> Dict:
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def monitoramentos(cls) -> Dict:
         """
         Retorna todos os monitoramentos de tribunal do usuário
         :return: Dict
         """
 
-        return self.methods.get("monitoramentos-tribunal")
+        return cls.methods.get("monitoramentos-tribunal")
 
-    def por_id(self, id_monitoramento: int) -> Dict:
+    @classmethod
+    def por_id(cls, id_monitoramento: int) -> Dict:
         """
         Retorna um monitoramento do usuário, de acordo com seu ID
         :param id_monitoramento: o ID do monitoramento
         :return: Dict
         """
 
-        return self.methods.get(f"monitoramentos-tribunal/{id_monitoramento}")
+        return cls.methods.get(f"monitoramentos-tribunal/{id_monitoramento}")
 
-    def editar(self, id_monitoramento: int, *, frequencia: Optional[str] = None) -> Dict:
+    @classmethod
+    def editar(cls, id_monitoramento: int, *, frequencia: Optional[str] = None) -> Dict:
         """
         Edita a frequencia de um monitoramento, de acordo com seu ID
         :param frequencia: a frequencia na qual o processo será monitorado
         :param id_monitoramento:  o ID do monitoramento
         :return: Dict
         """
         data = {
             'frequencia': frequencia
         }
-        return self.methods.put(f"monitoramentos-tribunal/{id_monitoramento}", data=data)
+        return cls.methods.put(f"monitoramentos-tribunal/{id_monitoramento}", data=data)
 
-    def criar(self, tipo_monitoramento: TiposMonitoramentosTribunal, valor: str, *,
+    @classmethod
+    def criar(cls, tipo_monitoramento: TiposMonitoramentosTribunal, valor: str, *,
                             frequencia: Optional[FrequenciaMonitoramentoTribunal] = None,
                             tribunal: Optional[str] = None) -> Dict:
         """
         Cria um monitoramento de tribunal
         :param tribunal: o tribunal a ser pesquisado
         :param frequencia: a frequencia na qual o processo será monitorado
         :param tipo_monitoramento: o tipo de monitoramento, opções disponiveis: UNICO, NUMDOC ,NOME
@@ -49,17 +56,18 @@
         data = {
             'tipo': tipo_monitoramento.value,
             'valor': valor,
             'tribunal': tribunal,
             'frequencia': frequencia.value
         }
 
-        return self.methods.post("monitoramento-tribunal", data=data)
+        return cls.methods.post("monitoramento-tribunal", data=data)
 
-    def remover(self, id_monitoramento: int) -> Dict:
+    @classmethod
+    def remover(cls, id_monitoramento: int) -> Dict:
         """
         Remove um monitoramento de acordo com seu ID
         :param id_monitoramento: o ID do monitoramento
         :return: Dict
         """
 
-        return self.methods.delete(f"monitoramentos-tribunal/{id_monitoramento}")
+        return cls.methods.delete(f"monitoramentos-tribunal/{id_monitoramento}")
```

### Comparing `escavador-0.1.8/escavador/resources/pessoa.py` & `escavador-0.2.2/escavador/v1/resources/pessoa.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from typing import Optional, Dict
 
 
-class Pessoa(Endpoint):
+class Pessoa(EndpointV1):
 
-    def por_id(self, id_pessoa: int) -> Dict:
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def por_id(cls, id_pessoa: int) -> Dict:
         """
         Retorna dados relacionados a uma pessoa pelo seu identificador.
         :param id_pessoa: o ID da pessoa
         :return: Dict
         """
-        return self.methods.get(f"pessoas/{id_pessoa}")
+        return cls.methods.get(f"pessoas/{id_pessoa}")
 
-    def processos(self, id_pessoa: int, *, limit: Optional[int] = None,
+    @classmethod
+    def processos(cls, id_pessoa: int, *, limit: Optional[int] = None,
                              page: Optional[int] = None) -> Dict:
         """
         Retorna os processos de uma pessoa baseado no ID da pessoa.
         :param id_pessoa: o ID da pessoa
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :return: Dict
         """
         data = {
             'limit': limit,
             'page': page
         }
 
-        return self.methods.get(f"pessoas/{id_pessoa}/processos", data=data)
+        return cls.methods.get(f"pessoas/{id_pessoa}/processos", data=data)
```

### Comparing `escavador-0.1.8/escavador/resources/processo.py` & `escavador-0.2.2/escavador/v1/resources/processo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-# from __future__ import annotations
-from escavador.resources.helpers.endpoint import Endpoint
-from escavador.resources.helpers.enums import TiposBusca
+from escavador.resources.helpers.endpoint import EndpointV1
+from escavador.resources.helpers.enums_v1 import TiposBusca
 from escavador.resources.helpers.documento import Documento
 from typing import Optional, List, Dict, Union
 
 
-class Processo(Endpoint):
+class Processo(EndpointV1):
 
-    def informacoes_no_tribunal(self, numero_unico: str, *, send_callback: Optional[bool] = None,
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def informacoes_no_tribunal(cls, numero_unico: str, *, send_callback: Optional[bool] = None,
                            wait: Optional[bool] = None,
                            autos: Optional[bool] = None, documentos_publicos:  Optional[bool] = None,
                            usuario: Optional[str] = None, senha: Optional[str] = None,
                            origem: Optional[str] = None, tipo_numero: Optional[str] = None,
                            tentativas:Optional[int] = None) -> Dict:
         """
         Cria uma busca assíncrona com o numero único, e busca por ele em todos os tribunais
@@ -37,17 +40,18 @@
             'usuario': usuario,
             'senha': senha,
             'origem': origem,
             'tipo_numero': tipo_numero,
             'tentativas': tentativas
         }
 
-        return self.methods.post(f"processo-tribunal/{numero_unico}/async", data=data)
+        return cls.methods.post(f"processo-tribunal/{numero_unico}/async", data=data)
 
-    def processos_por_nome_no_tribunal(self, origem: str, nome: str, *, send_callback: Optional[bool] = None,
+    @classmethod
+    def processos_por_nome_no_tribunal(cls, origem: str, nome: str, *, send_callback: Optional[bool] = None,
                               wait: Optional[bool] = None, permitir_parcial: Optional[bool] = None,
                               tentativas: Optional[int] = None) -> Dict:
         """
         Cria uma busca assíncrona no tribunal de origem baseada no nome enviado
         :param permitir_parcial: opção para não fazer a busca em todos os sistemas de um tribunal
         :param wait:  opção para esperar pelo resultado, espera no máximo 1 minuto
         :param send_callback: opção para mandar um callback com o resultado da busca
@@ -61,17 +65,18 @@
             'nome': nome,
             'permitir_parcial': permitir_parcial,
             'send_callback': send_callback,
             'wait': wait,
             'tentativas': tentativas
         }
 
-        return self.methods.post(f"tribunal/{origem.upper()}/busca-por-nome/async", data=data)
+        return cls.methods.post(f"tribunal/{origem.upper()}/busca-por-nome/async", data=data)
 
-    def processos_por_documento_no_tribunal(self, origem: str, numero_documento: str, *, send_callback: Optional[bool] = None,
+    @classmethod
+    def processos_por_documento_no_tribunal(cls, origem: str, numero_documento: str, *, send_callback: Optional[bool] = None,
                                    wait: Optional[bool] = None, permitir_parcial: Optional[bool] = None,
                                    tentativas: Optional[int] = None) -> Dict:
         """
         Cria uma busca assíncrona no tribunal de origem baseada no numero de documento enviado
         :param permitir_parcial: opção para não fazer a busca em todos os sistemas de um tribunal
         :param wait:  opção para esperar pelo resultado, espera no máximo 1 minuto
         :param send_callback: opção para mandar um callback com o resultado da busca
@@ -85,17 +90,18 @@
             'numero_documento': numero_documento,
             'permitir_parcial': permitir_parcial,
             'send_callback': send_callback,
             'wait': wait,
             'tentativas': tentativas
         }
 
-        return self.methods.post(f"tribunal/{origem.upper()}/busca-por-documento/async", data=data)
+        return cls.methods.post(f"tribunal/{origem.upper()}/busca-por-documento/async", data=data)
 
-    def processos_por_oab_no_tribunal(self, origem: str, numero_oab: str, estado_oab: str, *,
+    @classmethod
+    def processos_por_oab_no_tribunal(cls, origem: str, numero_oab: str, estado_oab: str, *,
                                    send_callback: Optional[bool] = None, wait: Optional[bool] = None,
                                    permitir_parcial: Optional[bool] = None,
                                    tentativas: Optional[int] = None) -> Dict:
         """
         Cria uma busca assíncrona no tribunal de origem baseada nos dados de oab enviados
         :param permitir_parcial: opção para não fazer a busca em todos os sistemas de um tribunal
         :param wait:  opção para esperar pelo resultado, espera no máximo 1 minuto
@@ -112,17 +118,18 @@
             'estado_oab': estado_oab,
             'permitir_parcial': permitir_parcial,
             'send_callback': send_callback,
             'wait': wait,
             'tentativas': tentativas
         }
 
-        return self.methods.post(f"tribunal/{origem.upper()}/busca-por-oab/async", data=data)
+        return cls.methods.post(f"tribunal/{origem.upper()}/busca-por-oab/async", data=data)
 
-    def busca_em_lote_no_tribunal(self, tipo_busca: TiposBusca, origens: List[str], *, send_callback: Optional[bool] = None,
+    @classmethod
+    def busca_em_lote_no_tribunal(cls, tipo_busca: TiposBusca, origens: List[str], *, send_callback: Optional[bool] = None,
                       numero_oab: Union[str, int, None] = None, estado_oab: Optional[str] = None,
                       numero_documento: Optional[str] = None, nome: Optional[str] = None) -> Dict:
         """
         Cria buscas do mesmo tipo para todos os tribunais enviados
         :param nome: o nome que será pesquisado
         :param numero_documento: o documento que será pesquisado
         :param estado_oab:  o estado da oab enviada
@@ -141,95 +148,101 @@
             'nome': nome,
             'numero_documento': numero_documento,
             'numero_oab': numero_oab,
             'estado_oab': estado_oab,
             'send_callback': send_callback
         }
 
-        return self.methods.post("tribunal/async/lote", data=data)
+        return cls.methods.post("tribunal/async/lote", data=data)
 
-    def processos_por_oab_em_diarios(self, estado_oab: str, numero_oab: Union[str, int], *, page: Optional[int] = None) -> Dict:
+    @classmethod
+    def processos_por_oab_em_diarios(cls, estado_oab: str, numero_oab: Union[str, int], *, page: Optional[int] = None) -> Dict:
         """
         Busca processos que estão nos Diários Oficiais do Escavador que estão relacionados ao OAB informado
         :param page: número da página
         :param estado_oab: sigla do estado da OAB
         :param numero_oab: número da OAB
         :return: Dict
         """
 
         data = {
             'page': page
         }
 
-        return self.methods.get(f"oab/{estado_oab}/{numero_oab}/processos", data=data)
+        return cls.methods.get(f"oab/{estado_oab}/{numero_oab}/processos", data=data)
 
-    def por_id_em_diarios(self, id_processo: int) -> Dict:
+    @classmethod
+    def por_id_em_diarios(cls, id_processo: int) -> Dict:
         """
         Retorna um processo pelo seu identificador no Escavador.
         :param id_processo: o ID do processo
         :return: Dict
         """
 
-        return self.methods.get(f"processos/{id_processo}")
+        return cls.methods.get(f"processos/{id_processo}")
 
-    def movimentacoes_diario_oficial(self, id_processo: int, *, limit: Optional[int] = None,
+    @classmethod
+    def movimentacoes_diario_oficial(cls, id_processo: int, *, limit: Optional[int] = None,
                                   page: Optional[int] = None) -> Dict:
         """
         Retorna as movimentações de um Processo pelo identificador do processo no Escavador.
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :param id_processo:  o ID do processo
         :return: Dict
         """
 
         data = {
             'limit': limit,
             'page': page
         }
 
-        return self.methods.get(f"processos/{id_processo}/movimentacoes", data=data)
+        return cls.methods.get(f"processos/{id_processo}/movimentacoes", data=data)
 
-    def processo_por_numero_em_diarios(self, numero_unico: str, *, match_exato: Optional[bool] = None) -> Dict:
+    @classmethod
+    def processo_por_numero_em_diarios(cls, numero_unico: str, *, match_exato: Optional[bool] = None) -> Dict:
         """
         Busca processos que estão nos Diários Oficiais do Escavador. e contenham o número único informado.
         :param match_exato: a busca será feita pelo número inteiro do processo pesquisado.
         :param numero_unico: número único do processo
         :return: Dict
         """
 
         data = {
             'match_exato': match_exato
         }
 
-        return self.methods.get(f"processos/numero/{numero_unico}", data=data)
+        return cls.methods.get(f"processos/numero/{numero_unico}", data=data)
 
-    def get_envolvidos_processo(self, id_processo: int, *, limit: Optional[int] = None,
+    @classmethod
+    def get_envolvidos_processo(cls, id_processo: int, *, limit: Optional[int] = None,
                                 page: Optional[int] = None) -> Dict:
         """
        Retorna os envolvidos de um Processo pelo identificador do processo no Escavador.
         :param id_processo:  o ID do processo
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :return: Dict
         """
 
         data = {
             'limit': limit,
             'page': page
         }
 
-        return self.methods.get(f"processos/{id_processo}/envolvidos", data=data)
+        return cls.methods.get(f"processos/{id_processo}/envolvidos", data=data)
 
-    def get_pdf(self, link_pdf: str, path: str, nome_arquivo: str) -> Dict:
+    @classmethod
+    def get_pdf(cls, link_pdf: str, path: str, nome_arquivo: str) -> Dict:
         """
         Baixa um pdf de autos de acordo com seu link e salva no caminho enviado, com o nome enviado
         :param nome_arquivo: nome do arquivo a ser criado
         :param link_pdf: link do documento
         :param path: caminho onde o pdf será salvo
         :return: Dict
         """
-        conteudo = self.methods.get(link_pdf)
+        conteudo = cls.methods.get(link_pdf)
 
-        if conteudo['sucesso'] is True:
-            return Documento.get_pdf(conteudo, path, nome_arquivo)
-        else:
+        if type(conteudo) is dict:
             return conteudo
+        else:
+            return Documento.get_pdf(conteudo, path, nome_arquivo)
```

### Comparing `escavador-0.1.8/escavador/resources/tribunal.py` & `escavador-0.2.2/escavador/v1/resources/tribunal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from escavador.resources.helpers.endpoint import Endpoint
+from escavador.resources.helpers.endpoint import EndpointV1
 from typing import Dict
 
-class Tribunal(Endpoint):
 
-    def sistemas_disponiveis(self) -> Dict:
+class Tribunal(EndpointV1):
+
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def sistemas_disponiveis(cls) -> Dict:
         """
         Retorna todos os sistemas de tribunais disponiveis
         :return: Dict
         """
-        return self.methods.get("tribunal/origens")
+        return cls.methods.get("tribunal/origens")
 
-    def detalhes(self, sigla_tribunal: str) -> Dict:
+    @classmethod
+    def detalhes(cls, sigla_tribunal: str) -> Dict:
         """
         Retorna os detalhes do tribunal enviado
         :param sigla_tribunal: A sigla do sistema de tribunal pesquisado
         :return: Dict
         """
-        return self.methods.get(f"tribunal/origens/{sigla_tribunal}")
+        return cls.methods.get(f"tribunal/origens/{sigla_tribunal}")
```

### Comparing `escavador-0.1.8/pyproject.toml` & `escavador-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "escavador"
-version = "0.1.8"
+version = "0.2.2"
 description = "A library to  interact with Escavador API"
 authors = [
     "Rafael <rafaelcampos@escavador.com>",
     "Gabriel <gabriel@escavador.com>"
 ]
 readme = "README.md"
 homepage = "https://www.escavador.com"
@@ -14,14 +14,17 @@
 keywords = ["escavador", "api", "python"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 requests = "^2.27.1"
 cchardet = "^2.1.7"
 python-dotenv = "^0.19.2"
+ratelimit = "*"
+dataclasses = "*"
+importlib = "*"
 importlib_metadata = "*"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

