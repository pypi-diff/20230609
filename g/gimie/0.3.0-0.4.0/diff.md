# Comparing `tmp/gimie-0.3.0.tar.gz` & `tmp/gimie-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimie-0.3.0.tar", max compression
+gzip compressed data, was "gimie-0.4.0.tar", max compression
```

## Comparing `gimie-0.3.0.tar` & `gimie-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-02-24 10:35:50.363298 gimie-0.3.0/LICENSE
--rw-r--r--   0        0        0     4470 2023-02-24 10:35:50.363298 gimie-0.3.0/README.md
--rw-r--r--   0        0        0      916 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/__init__.py
--rw-r--r--   0        0        0     2392 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/cli.py
--rw-r--r--   0        0        0      973 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/graph/namespaces.py
--rw-r--r--   0        0        0     1074 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/graph/operations.py
--rw-r--r--   0        0        0     3631 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/models.py
--rw-r--r--   0        0        0     3938 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/project.py
--rw-r--r--   0        0        0     1208 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/sources/__init__.py
--rw-r--r--   0        0        0     1774 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/sources/abstract.py
--rw-r--r--   0        0        0     4341 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/sources/git.py
--rw-r--r--   0        0        0     7050 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/sources/github.py
--rw-r--r--   0        0        0      357 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/sources/gitlab.py
--rw-r--r--   0        0        0     1460 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/sources/helpers.py
--rw-r--r--   0        0        0     3580 2023-02-24 10:35:50.363298 gimie-0.3.0/gimie/utils.py
--rw-r--r--   0        0        0     1457 2023-02-24 10:35:50.363298 gimie-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5598 1970-01-01 00:00:00.000000 gimie-0.3.0/setup.py
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 gimie-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 13:34:21.959745 gimie-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5072 2023-06-09 13:34:21.959745 gimie-0.4.0/README.md
+-rw-r--r--   0        0        0      917 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/__init__.py
+-rw-r--r--   0        0        0     2575 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/cli.py
+-rw-r--r--   0        0        0     1028 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/graph/namespaces.py
+-rw-r--r--   0        0        0     1074 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/graph/operations.py
+-rw-r--r--   0        0        0     2946 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/models.py
+-rw-r--r--   0        0        0     6723 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/project.py
+-rw-r--r--   0        0        0     1391 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/__init__.py
+-rw-r--r--   0        0        0     1849 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/abstract.py
+-rw-r--r--   0        0        0     1544 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/common/license.py
+-rw-r--r--   0        0        0      929 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/common/queries.py
+-rw-r--r--   0        0        0     4708 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/git.py
+-rw-r--r--   0        0        0    10671 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/github.py
+-rw-r--r--   0        0        0    10741 2023-06-09 13:34:21.963745 gimie-0.4.0/gimie/sources/gitlab.py
+-rw-r--r--   0        0        0     1832 2023-06-09 13:34:21.963745 gimie-0.4.0/gimie/utils.py
+-rw-r--r--   0        0        0     3131 2023-06-09 13:34:21.963745 gimie-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6263 1970-01-01 00:00:00.000000 gimie-0.4.0/PKG-INFO
```

### Comparing `gimie-0.3.0/LICENSE` & `gimie-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gimie-0.3.0/README.md` & `gimie-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-# Gimie
+[![gimie](docs/logo.svg)](https://github.com/SDSC-ORD/gimie)
 
-[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml)
+[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml) [![docs](https://github.com/SDSC-ORD/gimie/actions/workflows/sphinx-docs.yml/badge.svg)](https://sdsc-ord.github.io/gimie)
 
 Gimie (GIt Meta Information Extractor) is a python library and command line tool to extract structured metadata from git repositories.
 
-:warning: Gimie is at an early development stage. It is not yet functional.
 
 ## Context
-Scientific code repositories contain valuable metadata which can be used to enrich existing catalogues, platforms or databases. This tool aims to easily extract structured metadata from a generic git repositories. The following sources of information are used:
-
-* [x] Github API
-* [ ] Gitlab API
-* [ ] Local Git metadata
-* [ ] License text
-* [ ] Free text in README
-* [ ] Renku project metadata
+Scientific code repositories contain valuable metadata which can be used to enrich existing catalogues, platforms or databases. This tool aims to easily extract structured metadata from a generic git repositories. It can extract extract metadata from the Git provider (GitHub or GitLab) or from the git index itself.
 
 ## Installation
 
 To install the stable version on PyPI:
 
 ```shell
 pip install gimie
@@ -57,20 +49,26 @@
 
 run checks:
 
 ```shell
 make check
 ```
 
+build documentation:
+
+```shell
+make doc
+```
+
 ## Usage
 
 ### Set your github credentials
 
 In order to avoid rate limits with the github api, you need to provide your github
-username and a github token: see
+username and a github token with the `read:org` scope: see
 [here ](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
 on how to generate a github token.
 
 There are 2 options for setting up your github token in your local environment:
 
 **Option 1:**
 
@@ -108,30 +106,36 @@
 
 # To retrieve the serialized graph
 proj.serialize(format='ttl')
 ```
 
 Or to extract only from a specific source:
 ```python
-from gimie.sources.remote import GithubExtractor
+from gimie.sources.github import GithubExtractor
 gh = GithubExtractor('https://github.com/SDSC-ORD/gimie')
 gh.extract()
 
 # To retrieve the rdflib.Graph object
 g = gh.to_graph()
 
 # To retrieve the serialized graph
 gh.serialize(format='ttl')
 ```
+[For a GitLab project, replace `gimie.sources.github` by `gimie.sources.gitlab`, `GithubExtractor` by `GitlabExtractor`, as well as the URL to the GitLab project.]
 
 ## Outputs
 
 The default output is JSON-ld, a JSON serialization of the [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) data model. We follow the schema recommended by [codemeta](https://codemeta.github.io/).
 Supported formats are json-ld, turtle and n-triples.
 
+### Limitations
+
+* Currently, gimie will only the first 100 contributors of a repository (in arbitrary order), and for each users, at most 100 affiliations.
+* If a Github repository is owned by an organization, all "mentionable users" are reported as contributors. This will include all members of the organization in addition to contributors.
+
 ## Contributing
 
 All contributions are welcome. New functions and classes should have associated tests and docstrings following the [numpy style guide](https://numpydoc.readthedocs.io/en/latest/format.html).
 
 The code formatting standard we use is [black](https://github.com/psf/black), with `--line-length=79` to follow [PEP8](https://peps.python.org/pep-0008/) recommendations. We use [pytest](https://docs.pytest.org/en/7.2.x/) as our testing framework. This project uses [pyproject.toml](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) to define package information, requirements and tooling configuration.
 
 ## Releases and Publishing on Pypi
```

### Comparing `gimie-0.3.0/gimie/__init__.py` & `gimie-0.4.0/gimie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 import logging
 
 import importlib.metadata as importlib_metadata
 
 __version__ = importlib_metadata.version(__name__)
 
 logger = logging.getLogger()
```

### Comparing `gimie-0.3.0/gimie/cli.py` & `gimie-0.4.0/gimie/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,68 +14,79 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Command line interface to the gimie package."""
 from enum import Enum
 from typing import Optional
 from gimie import __version__
+import click
 import typer
 
 from gimie.project import Project
 
 app = typer.Typer(add_completion=False)
 
+# Used to autogenerate docs with sphinx-click
+@click.group()
+def cli():
+    """Command line group"""
+    pass
+
 
 class SerializationFormat(str, Enum):
+    """Enumeration of valid RDF serialization formats for project graphs"""
+
     ttl = "ttl"
     jsonld = "json-ld"
     nt = "nt"
 
 
 def version_callback(value: bool):
     if value:
         print(f"gimie {__version__}")
         # Exits successfully
         raise typer.Exit()
 
 
 @app.command()
 def data(
-    path: str,
-    only: str = typer.Option(False, "--only", help="Only use these sources."),
-    exclude: str = typer.Option(
-        False, "--exclude", help="Do not use these sources."
-    ),
+    url: str,
     format: SerializationFormat = typer.Option(
-        SerializationFormat.ttl,
+        "ttl",
         "--format",
         show_choices=True,
         help="Output serialization format for the RDF graph.",
     ),
     version: Optional[bool] = typer.Option(
         None,
         "--version",
         help="Display version and exit",
         callback=version_callback,
     ),
 ):
-    """Extract metadata from a Git repository at the target PATH."""
-    proj = Project(path)
+    """Extract linked metadata from a Git repository at the target URL.
+
+    The output is sent to stdout, and turtle is used as the default serialization format."""
+    proj = Project(url)
     print(proj.serialize(format=format))
-    proj.cleanup()
 
 
 @app.command()
-def advice(path: str):
+def advice(url: str):
     """Show a metadata completion report for a Git repository
-    at the target PATH."""
+    at the target URL.
+
+    NOTE: Not implemented yet"""
     ...
     raise typer.Exit()
 
 
+typer_cli = typer.main.get_command(app)
+cli.add_command(typer_cli, "cli")
+
 # This callback is triggered when gimie is called without subcommand
 @app.callback()
 def callback(
     version: Optional[bool] = typer.Option(
         None, "--version", callback=version_callback
     )
 ):
```

### Comparing `gimie-0.3.0/gimie/graph/namespaces.py` & `gimie-0.4.0/gimie/graph/namespaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 # limitations under the License.
 from rdflib.namespace import Namespace
 
 SDO = Namespace("http://schema.org/")
 COD = Namespace("https://doi.org/10.5063/schema/codemeta-2.0/")
 SD = Namespace("https://w3id.org/okn/o/sd/1.9.0/")
 BIO = Namespace("https://bioschemas.org/")
+GIMIE = Namespace("https://sdsc-ord.github.io/gimie/")
```

### Comparing `gimie-0.3.0/gimie/graph/operations.py` & `gimie-0.4.0/gimie/graph/operations.py`

 * *Files identical despite different names*

### Comparing `gimie-0.3.0/gimie/models.py` & `gimie-0.4.0/gimie/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,35 +22,14 @@
 
 from calamus.schema import JsonLDSchema
 from calamus import fields
 
 from gimie.graph.namespaces import SDO
 
 
-class IRI(fields.String):
-    """An external IRI reference.
-    NOTE: This is a temporary solution until calamus correctly serializes IRI fields."""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def _serialize(self, value, attr, obj, **kwargs):
-        if self.parent.opts.add_value_types or self.add_value_types:
-            return {"@id": value}
-
-        value = super()._serialize(value, attr, obj, **kwargs)
-        if value:
-            return {"@id": value}
-
-    def _deserialize(self, value, attr, data, **kwargs):
-        if "@id" in value:
-            value = value["@id"]
-        return super()._deserialize(value, attr, data, **kwargs)
-
-
 @dataclass(order=True)
 class Release:
     """
     This class represents a release of a repository.
 
     Parameters
     ----------
@@ -81,15 +60,15 @@
 
 class OrganizationSchema(JsonLDSchema):
     _id = fields.Id()
     name = fields.String(SDO.name)
     legal_name = fields.String(SDO.legalName)
     email = fields.String(SDO.email)
     description = fields.String(SDO.description)
-    logo = IRI(SDO.logo)
+    logo = fields.IRI(SDO.logo)
 
     class Meta:
         rdf_type = SDO.Organization
         model = Organization
 
 
 @dataclass
```

### Comparing `gimie-0.3.0/gimie/sources/abstract.py` & `gimie-0.4.0/gimie/sources/abstract.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 
     All subclasses must implement extract() and to_graph() methods
     they are free to override the default serialize() and jsonld()
     """
 
     def __init__(self, path: str, _id: Optional[str] = None):
         self.path = path
+        if _id is not None:
+            self._id = _id
 
     @abstractmethod
     def extract(self):
         """Extract metadata"""
         ...
 
     @abstractmethod
     def to_graph(self) -> Graph:
         """Generate an RDF graph from the instance"""
         return Graph()
 
-    def serialize(self, format: str = "ttl") -> str:
+    def serialize(self, format: str = "ttl", **kwargs) -> str:
         """Serialize the RDF graph representing the instance."""
-        return self.to_graph().serialize(format=format)  # type: ignore
+        return self.to_graph().serialize(format=format, **kwargs)  # type: ignore
 
     def jsonld(self) -> str:
         """Alias for jsonld serialization."""
         return self.serialize(format="json-ld")
```

### Comparing `gimie-0.3.0/gimie/sources/github.py` & `gimie-0.4.0/gimie/sources/gitlab.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,206 +1,301 @@
-# Gimie
-# Copyright 2022 - Swiss Data Science Center (SDSC)
-# A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
-# Eidgenössische Technische Hochschule Zürich (ETHZ).
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 from __future__ import annotations
-
 from dataclasses import dataclass
-from datetime import datetime
-import requests
 import os
-from typing import Any, Dict, List, Optional, Union, Tuple
+import requests
+from datetime import datetime
+from typing import Any, Dict, List, Optional, Union
 from urllib.parse import urlparse
-from dotenv import load_dotenv
 
+from dotenv import load_dotenv
 from calamus import fields
 from calamus.schema import JsonLDSchema
 from rdflib import Graph
 
 from gimie.sources.abstract import Extractor
 from gimie.models import (
     Organization,
     OrganizationSchema,
     Person,
     PersonSchema,
-    IRI,
 )
 from gimie.graph.namespaces import SDO
-from gimie.utils import get_spdx_url
+from gimie.sources.common.queries import send_graphql_query, send_rest_query
 
-GH_API = "https://api.github.com"
+GL_API_REST = "https://gitlab.com/api/v4/"
+GL_API_GRAPHQL = "https://gitlab.com/api"
 load_dotenv()
 
 
 @dataclass
-class GithubExtractor(Extractor):
+class GitlabExtractor(Extractor):
+    """Extractor for Gitlab repositories. Uses the Gitlab GraphQL API to
+    extract metadata into linked data."""
+
     path: str
-    github_token: Optional[str] = None
+    _id: Optional[str] = None
+    token: Optional[str] = None
 
     name: Optional[str] = None
-    author: Optional[Union[Organization, Person]] = None
+    identifier: Optional[str] = None
+    author: Optional[List[Union[Organization, Person]]] = None
     contributors: Optional[List[Person]] = None
     prog_langs: Optional[List[str]] = None
-    download_url: Optional[str] = None
     description: Optional[str] = None
     date_created: Optional[datetime] = None
     date_modified: Optional[datetime] = None
+    version: Optional[str] = None
     keywords: Optional[List[str]] = None
-    license: Optional[str] = None
-    software_version: Optional[str] = None
+    source_organization: Optional[Organization] = None
+    download_url: Optional[str] = None
+    # license: Optional[str] = None
 
     def to_graph(self) -> Graph:
-        jd = GithubExtractorSchema().dumps(self)
+        """Convert repository to RDF graph."""
+        jd = GitlabExtractorSchema().dumps(self)
         g: Graph = Graph().parse(format="json-ld", data=str(jd))
         g.bind("schema", SDO)
         return g
 
     def extract(self):
-        self._id = self.path
+        """Extract metadata from target Gitlab repository."""
+        if self._id is None:
+            self._id = self.path
         self.name = urlparse(self.path).path.strip("/")
 
-        data = self._request(f"repos/{self.name}")
-        self.author = self._get_owner(
-            data["owner"]["login"], data["owner"]["type"]
-        )
-        self.contributors = self._get_contributors()
-        self.download_url = data["archive_url"][:-6].format(
-            archive_format="tarball"
-        )
+        # fetch metadata
+        data = self._fetch_repo_data(self.name)
+
+        # Each Gitlab project has a unique identifier (integer)
+        self.identifier = urlparse(data["id"]).path.split("/")[2]
+        # at the moment, Gimie fetches only the group directly related to the project
+        # the group name will take the form: parent/subgroup
+        self.source_organization = self._safe_extract_group(data)
         self.description = data["description"]
-        self.date_created = datetime.fromisoformat(data["created_at"][:-1])
-        self.date_modified = datetime.fromisoformat(data["updated_at"][:-1])
-        # If license is available, convert to standard SPDX URL
-        if data["license"]["url"]:
-            self.license = get_spdx_url(data["license"]["spdx_id"])
-        self.prog_langs = self._get_prog_langs()
+        self.prog_langs = [lang["name"] for lang in data["languages"]]
+        self.date_created = datetime.fromisoformat(data["createdAt"][:-1])
+        self.date_modified = datetime.fromisoformat(
+            data["lastActivityAt"][:-1]
+        )
         self.keywords = data["topics"]
-        self.version = self._get_last_release()
+
+        # Get contributors as the project members that are not owners and those that have written merge requests
+        # owners are either multiple individuals or a group, if not user is marked as owner
+        self.author = self._safe_extract_author(data)
+        # contributors are project members or merge request authors
+        self.contributors = self._safe_extract_contributors(data)
+
+        if data["releases"] and (len(data["releases"]["edges"]) > 0):
+            # go into releases and take the name from the first node (most recent)
+            self.version = data["releases"]["edges"][0]["node"]["name"]
+            self.download_url = f"{self.path}/-/archive/{self.version}/{self.name.split('/')[-1]}-{self.version}.tar.gz"
+
+        # for the license, we need to query the rest API
+        # the code below does not work, returns - if you have permission- the GitLab specific licence
+        # resp = requests.get(url=f"{GL_API_rest}/license/{self.identifier}")
+        # if resp.status_code == 200:
+        #     self.license = resp.json()
+
+    def _safe_extract_group(
+        self, repo: Dict[str, Any]
+    ) -> Optional[Organization]:
+        """Extract the group from a GraphQL repository node if it has one."""
+        if (self.name is not None) and (repo["group"] is not None):
+            repo["group"]["name"] = "/".join(self.name.split("/")[0:-1])
+            return self._get_organization(repo["group"])
+        return None
+
+    def _safe_extract_author(
+        self, repo: Dict[str, Any]
+    ) -> List[Union[Person, Organization]]:
+        """Extract the author from a GraphQL repository node.
+        projectMembers is used if available, otherwise the author
+        is inferred from the project url."""
+        members = repo["projectMembers"]["edges"]
+        if len(members) > 0:
+            owners = filter(
+                lambda m: m["node"]["accessLevel"]["stringValue"] == "OWNER",
+                members,
+            )
+            return [
+                self._get_author(owner["node"]["user"]) for owner in owners
+            ]
+
+        if repo["group"] is not None:
+            return [self._get_author(repo["group"])]
+
+        # If the author is absent from the GraphQL response (permission bug),
+        # fallback to the REST API
+        return [self._user_from_rest(self.name.split("/")[0])]
+
+    def _safe_extract_contributors(
+        self, repo: dict[str, Any]
+    ) -> list[Person] | None:
+        members = [
+            user["node"]["user"]
+            for user in repo["projectMembers"]["edges"]
+            if user["node"]["accessLevel"]["stringValue"] != "OWNER"
+        ]
+        merge_request_authors = [
+            author["node"]["author"]
+            for author in repo["mergeRequests"]["edges"]
+        ]
+        contributors = members + merge_request_authors
+        # Drop duplicate (unhashable) dicts by "id" key
+        uniq_contrib = list({c["id"]: c for c in contributors}.values())
+        return [self._get_user(contrib) for contrib in uniq_contrib]
+
+    def _fetch_repo_data(self, path: str) -> Dict[str, Any]:
+        """Fetch repository metadata from GraphQL endpoint."""
+        data = {"path": path}
+        project_query = """
+        query project_query($path: ID!) {
+            project(fullPath: $path) {
+                name
+                id
+                description
+                createdAt
+                lastActivityAt
+                group {
+                    id
+                    name
+                    description
+                    avatarUrl
+                    webUrl
+                }
+                languages {
+                    name
+                    share
+                }
+                topics
+                projectMembers {
+                    edges {
+                        node {
+                        id
+                        accessLevel {
+                            stringValue
+                        }
+                        user {
+                            id
+                            name
+                            username
+                            publicEmail
+                            webUrl
+                        }
+                        }
+                    }
+                }
+                mergeRequests{
+                    edges {
+                    node {
+                        author {
+                        id
+                        name
+                        username
+                        publicEmail
+                        webUrl
+                        }
+                    }
+                    }
+                }
+                releases {
+                    edges {
+                    node {
+                        name
+                    }
+                    }
+                }
+        }
+        }
+        """
+        response = send_graphql_query(
+            GL_API_GRAPHQL, project_query, data, self._set_auth()
+        )
+        if "errors" in response:
+            raise ValueError(response["errors"])
+
+        return response["data"]["project"]
 
     def _set_auth(self) -> Any:
+        """Set authentication headers for Gitlab API requests."""
         try:
-            if not self.github_token:
-                self.github_token = os.environ.get("ACCESS_TOKEN")
-                assert self.github_token
-            headers = {"Authorization": f"token {self.github_token}"}
+            if not self.token:
+                self.token = os.environ.get("GITLAB_TOKEN")
+                assert self.token
+            headers = {"Authorization": f"token {self.token}"}
 
-            login = requests.get(
-                "https://api.github.com/user", headers=headers
-            )
+            login = requests.get(f"{GL_API_REST}/user", headers=headers)
             assert login.json().get("login")
         except AssertionError:
             return {}
         else:
             return headers
 
-    def _request(self, query_path: str) -> Any:
-        """Wrapper to query github api and return
-        a dictionary of the json response.
-
-        Parameters
-        ----------
-        query_path:
-            The query, without the base path.
+    def _get_author(self, node: Dict[str, Any]) -> Union[Organization, Person]:
+        """Given the GraphQL node for a repository owner,
+        return the author as a Person or Organization object."""
+        # Is this the best test?
+        if "username" in node:
+            return self._get_user(node)
+        return self._get_organization(node)
 
-        """
-        resp = requests.get(
-            f"{GH_API}/{query_path.lstrip('/')}", headers=self._set_auth()
-        )
-        # If the query fails, explain why
-        if resp.status_code != 200:
-            raise ConnectionError(resp.json()["message"])
-        return resp.json()
-
-    def _get_contributors(self) -> List[Person]:
-        """Specialized API query to get list of contributors names."""
-        conts = self._request(f"repos/{self.name}/contributors")
-        return [self._get_user(cont["login"]) for cont in conts]
-
-    def _get_last_release(self) -> Optional[str]:
-        resp: List[Dict[str, Any]] = self._request(
-            f"repos/{self.name}/releases"
+    def _get_organization(self, node: Dict[str, Any]) -> Organization:
+        """Extract details from a GraphQL organization node."""
+        return Organization(
+            _id=node["webUrl"],
+            name=node["name"],
+            description=node.get("description"),
+            logo=node.get("avatarUrl"),
         )
-        if len(resp):
-            return resp[0]["name"]
-        return None
 
-    def _get_organization(self, name: str) -> Organization:
-        resp = self._request(f"orgs/{name}")
-        return Organization(
-            _id=resp["url"],
-            name=resp["login"],
-            description=resp["description"],
-            legal_name=resp["name"],
-            logo=resp["avatar_url"],
+    def _get_user(self, node: Dict[str, Any]) -> Person:
+        """Extract details from a GraphQL user node."""
+        return Person(
+            _id=node["webUrl"],
+            identifier=node["username"],
+            name=node.get("name"),
+            email=node.get("publicEmail"),
         )
 
-    def _get_owner(
-        self, name: str, owner_type: str
-    ) -> Union[Organization, Person]:
-        """Set the person or organization who owns the repository."""
-        if owner_type == "User":
-            return self._get_user(name)
-        elif owner_type == "Organization":
-            return self._get_organization(name)
-        else:
-            raise ValueError(f"Unknown Github owner type: {owner_type}.")
+    def _user_from_rest(self, username: str) -> Person:
+        """Given a username, use the REST API to retrieve the Person object."""
+
+        author = send_rest_query(
+            GL_API_REST,
+            f"/users?username={username}",
+            self._set_auth(),
+        )
+        if isinstance(author, list):
+            author = author[0]
 
-    def _get_prog_langs(self) -> List[str]:
-        """Get the list of programming languages used."""
-        resp = self._request(f"repos/{self.name}/languages")
-        return [lang for lang in resp.keys()]
-
-    def _get_user(self, name: str) -> Person:
-        """Specialized API query to get user details."""
-        user = self._request(f"users/{name}")
-        # Get user's affiliations
-        orgs = self._request(f"users/{name}/orgs")
-        orgs = [
-            Organization(
-                _id=org["url"],
-                name=org["login"],
-                description=org["description"],
-            )
-            for org in orgs
-        ]
         return Person(
-            _id=user["url"],
-            identifier=user["login"],
-            name=user["name"],
-            email=user["email"],
-            affiliations=orgs,
+            _id=author["web_url"],
+            identifier=author["username"],
+            name=author.get("name"),
         )
 
 
-class GithubExtractorSchema(JsonLDSchema):
+class GitlabExtractorSchema(JsonLDSchema):
     """This defines the schema used for json-ld serialization."""
 
     _id = fields.Id()
     name = fields.String(SDO.name)
-    author = fields.Nested(SDO.author, [PersonSchema, OrganizationSchema])
+    identifier = fields.String(SDO.identifier)
+    source_organization = fields.Nested(SDO.isPartOf, OrganizationSchema)
+    author = fields.Nested(
+        SDO.author, [PersonSchema, OrganizationSchema], many=True
+    )
     contributors = fields.Nested(SDO.contributor, PersonSchema, many=True)
     prog_langs = fields.List(SDO.programmingLanguage, fields.String)
     download_url = fields.Raw(SDO.downloadUrl)
     description = fields.String(SDO.description)
     date_created = fields.Date(SDO.dateCreated)
     date_modified = fields.Date(SDO.dateModified)
-    license = IRI(SDO.license)
-    path = IRI(SDO.CodeRepository)
+    # license = IRI(SDO.license)
+    path = fields.IRI(SDO.CodeRepository)
     keywords = fields.List(SDO.keywords, fields.String)
     version = fields.String(SDO.version)
 
     class Meta:
         rdf_type = SDO.SoftwareSourceCode
-        model = GithubExtractor
+        model = GitlabExtractor
         add_value_types = False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gimie-0.3.0/setup.py` & `gimie-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,178 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gimie
+Version: 0.4.0
+Summary: Extract structured metadata from git repositories.
+Home-page: https://github.com/SDSC-ORD/gimie
+License: Apache-2.0
+Keywords: metadata,git,extraction,linked-data
+Author: Swiss Data Science Center
+Author-email: contact@datascience.ch
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyDriller (>=2.3,<3.0)
+Requires-Dist: calamus (>=0.4.2,<0.5.0)
+Requires-Dist: importlib (>=1.0.4,<2.0.0)
+Requires-Dist: pre-commit (>=3.0.0,<4.0.0)
+Requires-Dist: pyshacl (>=0.20.0,<0.21.0)
+Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['gimie', 'gimie.graph', 'gimie.sources']
+[![gimie](docs/logo.svg)](https://github.com/SDSC-ORD/gimie)
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml) [![docs](https://github.com/SDSC-ORD/gimie/actions/workflows/sphinx-docs.yml/badge.svg)](https://sdsc-ord.github.io/gimie)
 
-install_requires = \
-['PyDriller>=2.3,<3.0',
- 'calamus>=0.4.1,<0.5.0',
- 'pre-commit>=3.0.0,<4.0.0',
- 'pyshacl>=0.20.0,<0.21.0',
- 'python-dotenv>=0.21.1,<0.22.0',
- 'requests>=2.28.2,<3.0.0',
- 'typer>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['gimie = gimie.cli:app']}
-
-setup_kwargs = {
-    'name': 'gimie',
-    'version': '0.3.0',
-    'description': 'Extract structured metadata from git repositories.',
-    'long_description': '# Gimie\n\n[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml)\n\nGimie (GIt Meta Information Extractor) is a python library and command line tool to extract structured metadata from git repositories.\n\n:warning: Gimie is at an early development stage. It is not yet functional.\n\n## Context\nScientific code repositories contain valuable metadata which can be used to enrich existing catalogues, platforms or databases. This tool aims to easily extract structured metadata from a generic git repositories. The following sources of information are used:\n\n* [x] Github API\n* [ ] Gitlab API\n* [ ] Local Git metadata\n* [ ] License text\n* [ ] Free text in README\n* [ ] Renku project metadata\n\n## Installation\n\nTo install the stable version on PyPI:\n\n```shell\npip install gimie\n```\n\nTo install the dev version from github:\n\n```shell\npip install git+https://github.com/SDSC-ORD/gimie.git@main#egg=gimie\n```\n\nGimie is also available as a docker container hosted on the [Github container registry](https://github.com/SDSC-ORD/gimie/pkgs/container/gimie):\n\n```shell\ndocker pull ghcr.io/sdsc-ord/gimie:latest\n\n# The access token can be provided as an environment variable\ndocker run -e ACCESS_TOKEN=$ACCESS_TOKEN ghcr.io/sdsc-ord/gimie:latest gimie data <repo>\n```\n\n\n### For development:\n\nactivate a conda or virtual environment with Python 3.8 or higher\n\n```shell\ngit clone https://github.com/SDSC-ORD/gimie && cd gimie\nmake install\n```\n\nrun tests:\n\n```shell\nmake test\n```\n\nrun checks:\n\n```shell\nmake check\n```\n\n## Usage\n\n### Set your github credentials\n\nIn order to avoid rate limits with the github api, you need to provide your github\nusername and a github token: see\n[here ](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)\non how to generate a github token.\n\nThere are 2 options for setting up your github token in your local environment:\n\n**Option 1:**\n\n```\ncp .env.dist .env\n```\n\nAnd then edit the `.env` file and put your github token in.\n\n**Option 2:**\n\nAdd your github token in your terminal:\n\n```bash\nexport ACCESS_TOKEN=\n```\n\nAfter the github token has been added, you can run the command without running into an github api limit.\nOtherwise you can still run the command, but might hit that limit after running the command several times.\n\n### Run the command\n\nAs a command line tool:\n```shell\ngimie data https://github.com/numpy/numpy\n```\nAs a python library:\n\n```python\nfrom gimie.project import Project\nproj = Project("https://github.com/numpy/numpy)\n\n# To retrieve the rdflib.Graph object\ng = proj.to_graph()\n\n# To retrieve the serialized graph\nproj.serialize(format=\'ttl\')\n```\n\nOr to extract only from a specific source:\n```python\nfrom gimie.sources.remote import GithubExtractor\ngh = GithubExtractor(\'https://github.com/SDSC-ORD/gimie\')\ngh.extract()\n\n# To retrieve the rdflib.Graph object\ng = gh.to_graph()\n\n# To retrieve the serialized graph\ngh.serialize(format=\'ttl\')\n```\n\n## Outputs\n\nThe default output is JSON-ld, a JSON serialization of the [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) data model. We follow the schema recommended by [codemeta](https://codemeta.github.io/).\nSupported formats are json-ld, turtle and n-triples.\n\n## Contributing\n\nAll contributions are welcome. New functions and classes should have associated tests and docstrings following the [numpy style guide](https://numpydoc.readthedocs.io/en/latest/format.html).\n\nThe code formatting standard we use is [black](https://github.com/psf/black), with `--line-length=79` to follow [PEP8](https://peps.python.org/pep-0008/) recommendations. We use [pytest](https://docs.pytest.org/en/7.2.x/) as our testing framework. This project uses [pyproject.toml](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) to define package information, requirements and tooling configuration.\n\n## Releases and Publishing on Pypi\n\nReleases are done via github release\n\n- a release will trigger a github workflow to publish the package on Pypi\n- Make sure to update to a new version in `pyproject.toml` before making the release\n- It is possible to test the publishing on Pypi.test by running a manual workflow: go to github actions and run the Workflow: \'Publish on Pypi Test\'\n',
-    'author': 'Swiss Data Science Center',
-    'author_email': 'contact@datascience.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/SDSC-ORD/gimie',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Gimie (GIt Meta Information Extractor) is a python library and command line tool to extract structured metadata from git repositories.
 
 
-setup(**setup_kwargs)
+## Context
+Scientific code repositories contain valuable metadata which can be used to enrich existing catalogues, platforms or databases. This tool aims to easily extract structured metadata from a generic git repositories. It can extract extract metadata from the Git provider (GitHub or GitLab) or from the git index itself.
+
+## Installation
+
+To install the stable version on PyPI:
+
+```shell
+pip install gimie
+```
+
+To install the dev version from github:
+
+```shell
+pip install git+https://github.com/SDSC-ORD/gimie.git@main#egg=gimie
+```
+
+Gimie is also available as a docker container hosted on the [Github container registry](https://github.com/SDSC-ORD/gimie/pkgs/container/gimie):
+
+```shell
+docker pull ghcr.io/sdsc-ord/gimie:latest
+
+# The access token can be provided as an environment variable
+docker run -e ACCESS_TOKEN=$ACCESS_TOKEN ghcr.io/sdsc-ord/gimie:latest gimie data <repo>
+```
+
+
+### For development:
+
+activate a conda or virtual environment with Python 3.8 or higher
+
+```shell
+git clone https://github.com/SDSC-ORD/gimie && cd gimie
+make install
+```
+
+run tests:
+
+```shell
+make test
+```
+
+run checks:
+
+```shell
+make check
+```
+
+build documentation:
+
+```shell
+make doc
+```
+
+## Usage
+
+### Set your github credentials
+
+In order to avoid rate limits with the github api, you need to provide your github
+username and a github token with the `read:org` scope: see
+[here ](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
+on how to generate a github token.
+
+There are 2 options for setting up your github token in your local environment:
+
+**Option 1:**
+
+```
+cp .env.dist .env
+```
+
+And then edit the `.env` file and put your github token in.
+
+**Option 2:**
+
+Add your github token in your terminal:
+
+```bash
+export ACCESS_TOKEN=
+```
+
+After the github token has been added, you can run the command without running into an github api limit.
+Otherwise you can still run the command, but might hit that limit after running the command several times.
+
+### Run the command
+
+As a command line tool:
+```shell
+gimie data https://github.com/numpy/numpy
+```
+As a python library:
+
+```python
+from gimie.project import Project
+proj = Project("https://github.com/numpy/numpy)
+
+# To retrieve the rdflib.Graph object
+g = proj.to_graph()
+
+# To retrieve the serialized graph
+proj.serialize(format='ttl')
+```
+
+Or to extract only from a specific source:
+```python
+from gimie.sources.github import GithubExtractor
+gh = GithubExtractor('https://github.com/SDSC-ORD/gimie')
+gh.extract()
+
+# To retrieve the rdflib.Graph object
+g = gh.to_graph()
+
+# To retrieve the serialized graph
+gh.serialize(format='ttl')
+```
+[For a GitLab project, replace `gimie.sources.github` by `gimie.sources.gitlab`, `GithubExtractor` by `GitlabExtractor`, as well as the URL to the GitLab project.]
+
+## Outputs
+
+The default output is JSON-ld, a JSON serialization of the [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) data model. We follow the schema recommended by [codemeta](https://codemeta.github.io/).
+Supported formats are json-ld, turtle and n-triples.
+
+### Limitations
+
+* Currently, gimie will only the first 100 contributors of a repository (in arbitrary order), and for each users, at most 100 affiliations.
+* If a Github repository is owned by an organization, all "mentionable users" are reported as contributors. This will include all members of the organization in addition to contributors.
+
+## Contributing
+
+All contributions are welcome. New functions and classes should have associated tests and docstrings following the [numpy style guide](https://numpydoc.readthedocs.io/en/latest/format.html).
+
+The code formatting standard we use is [black](https://github.com/psf/black), with `--line-length=79` to follow [PEP8](https://peps.python.org/pep-0008/) recommendations. We use [pytest](https://docs.pytest.org/en/7.2.x/) as our testing framework. This project uses [pyproject.toml](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) to define package information, requirements and tooling configuration.
+
+## Releases and Publishing on Pypi
+
+Releases are done via github release
+
+- a release will trigger a github workflow to publish the package on Pypi
+- Make sure to update to a new version in `pyproject.toml` before making the release
+- It is possible to test the publishing on Pypi.test by running a manual workflow: go to github actions and run the Workflow: 'Publish on Pypi Test'
+
```

