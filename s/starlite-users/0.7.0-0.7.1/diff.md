# Comparing `tmp/starlite_users-0.7.0.tar.gz` & `tmp/starlite_users-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlite_users-0.7.0.tar", max compression
+gzip compressed data, was "starlite_users-0.7.1.tar", max compression
```

## Comparing `starlite_users-0.7.0.tar` & `starlite_users-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-05-15 08:50:32.380055 starlite_users-0.7.0/LICENSE
--rw-r--r--   0        0        0      809 2023-05-15 08:50:32.380055 starlite_users-0.7.0/README.md
--rw-r--r--   0        0        0     4317 2023-05-15 08:50:32.384055 starlite_users-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      124 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/__init__.py
--rw-r--r--   0        0        0     1522 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/guid.py
--rw-r--r--   0        0        0     1517 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/mixins.py
--rw-r--r--   0        0        0     8141 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/repository.py
--rw-r--r--   0        0        0    13032 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/config.py
--rw-r--r--   0        0        0     2660 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/dependencies.py
--rw-r--r--   0        0        0     2830 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/exceptions.py
--rw-r--r--   0        0        0     5046 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/generics.py
--rw-r--r--   0        0        0     1485 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/guards.py
--rw-r--r--   0        0        0     6734 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/main.py
--rw-r--r--   0        0        0     1350 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/password.py
--rw-r--r--   0        0        0    14243 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/route_handlers.py
--rw-r--r--   0        0        0     2356 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/schema.py
--rw-r--r--   0        0        0    15727 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/service.py
--rw-r--r--   0        0        0     3354 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/user_handlers.py
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 starlite_users-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 08:27:17.411144 starlite_users-0.7.1/LICENSE
+-rw-r--r--   0        0        0      809 2023-06-09 08:27:17.411144 starlite_users-0.7.1/README.md
+-rw-r--r--   0        0        0     4317 2023-06-09 08:27:17.411144 starlite_users-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/__init__.py
+-rw-r--r--   0        0        0     1522 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/guid.py
+-rw-r--r--   0        0        0     1517 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0     8141 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/repository.py
+-rw-r--r--   0        0        0    13032 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/config.py
+-rw-r--r--   0        0        0     2660 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/dependencies.py
+-rw-r--r--   0        0        0     2830 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/exceptions.py
+-rw-r--r--   0        0        0     5046 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/generics.py
+-rw-r--r--   0        0        0     1485 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/guards.py
+-rw-r--r--   0        0        0     6734 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/main.py
+-rw-r--r--   0        0        0     1350 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/password.py
+-rw-r--r--   0        0        0    14243 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/route_handlers.py
+-rw-r--r--   0        0        0     2356 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/schema.py
+-rw-r--r--   0        0        0    15754 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/service.py
+-rw-r--r--   0        0        0     3354 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/user_handlers.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 starlite_users-0.7.1/PKG-INFO
```

### Comparing `starlite_users-0.7.0/LICENSE` & `starlite_users-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/README.md` & `starlite_users-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/pyproject.toml` & `starlite_users-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starlite-users"
-version = "0.7.0"
+version = "0.7.1"
 description = "Authentication and user management for Starlite"
 authors = ["Michael Bosch <michael@lonelyviking.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "starlite_users"}]
 
 [tool.poetry.dependencies]
```

### Comparing `starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/guid.py` & `starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/guid.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/mixins.py` & `starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/repository.py` & `starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/config.py` & `starlite_users-0.7.1/starlite_users/config.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/dependencies.py` & `starlite_users-0.7.1/starlite_users/dependencies.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/exceptions.py` & `starlite_users-0.7.1/starlite_users/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/generics.py` & `starlite_users-0.7.1/starlite_users/generics.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/guards.py` & `starlite_users-0.7.1/starlite_users/guards.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/main.py` & `starlite_users-0.7.1/starlite_users/main.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/password.py` & `starlite_users-0.7.1/starlite_users/password.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/route_handlers.py` & `starlite_users-0.7.1/starlite_users/route_handlers.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/schema.py` & `starlite_users-0.7.1/starlite_users/schema.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/starlite_users/service.py` & `starlite_users-0.7.1/starlite_users/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     user_model: type[UserModelType]
     """A subclass of the `User` ORM model."""
 
     def __init__(
         self,
         repository: SQLAlchemyUserRepository[UserModelType, RoleModelType],
         secret: SecretStr,
-        hash_schemes: Sequence[str] | None,
+        hash_schemes: Sequence[str] | None = None,
     ) -> None:
         """User service constructor.
 
         Args:
             repository: A `UserRepository` instance
             secret: Secret string for securely signing tokens.
             hash_schemes: Schemes to use for password encryption.
@@ -74,15 +74,15 @@
         try:
             existing_user = await self.get_user_by(email=data.email)
             if existing_user:
                 raise RepositoryConflictException("email already associated with an account")
         except RepositoryNotFoundException:
             pass
 
-        user_dict = data.dict(exclude={"password"})
+        user_dict = data.dict(exclude={"password"}, exclude_unset=True)
         user_dict["password_hash"] = self.password_manager.hash(data.password)
         if not process_unsafe_fields:
             user_dict["is_verified"] = False
             user_dict["is_active"] = True
 
         return await self.repository.add_user(self.user_model(**user_dict))  # pyright: ignore
```

### Comparing `starlite_users-0.7.0/starlite_users/user_handlers.py` & `starlite_users-0.7.1/starlite_users/user_handlers.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.0/PKG-INFO` & `starlite_users-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlite-users
-Version: 0.7.0
+Version: 0.7.1
 Summary: Authentication and user management for Starlite
 License: MIT
 Author: Michael Bosch
 Author-email: michael@lonelyviking.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

