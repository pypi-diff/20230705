# Comparing `tmp/hipal_mixin_scrud-1.0.6.tar.gz` & `tmp/hipal_mixin_scrud-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hipal_mixin_scrud-1.0.6.tar", last modified: Tue Jun 27 19:56:23 2023, max compression
+gzip compressed data, was "dist\hipal_mixin_scrud-1.0.7.tar", last modified: Wed Jul  5 20:23:57 2023, max compression
```

## Comparing `hipal_mixin_scrud-1.0.6.tar` & `hipal_mixin_scrud-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.535277 hipal_mixin_scrud-1.0.6/
--rw-rw-rw-   0        0        0     4285 2023-06-27 19:56:23.534279 hipal_mixin_scrud-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3860 2023-06-27 19:42:51.000000 hipal_mixin_scrud-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.481278 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.514279 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/crud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/crud/__init__.py
--rw-rw-rw-   0        0        0     5704 2023-06-27 19:54:12.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/crud/generator.py
--rw-rw-rw-   0        0        0     3504 2023-06-27 19:54:11.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/crud/mixin_list.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.519280 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/enums/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/enums/__init__.py
--rw-rw-rw-   0        0        0      255 2023-06-22 17:45:04.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/enums/operators.py
--rw-rw-rw-   0        0        0       82 2023-06-22 17:45:06.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/enums/sorts.py
--rw-rw-rw-   0        0        0     5053 2023-06-27 19:54:13.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/mixin.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.525279 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/schemas/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/schemas/__init__.py
--rw-rw-rw-   0        0        0      295 2023-06-27 19:55:29.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/schemas/paginate_params.py
--rw-rw-rw-   0        0        0      364 2023-06-27 19:40:37.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/schemas/pagination_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.528279 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/
--rw-rw-rw-   0        0        0        0 2023-06-23 18:53:11.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.532277 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/factory_test/
--rw-rw-rw-   0        0        0        0 2023-06-23 18:57:52.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/factory_test/__init__.py
--rw-rw-rw-   0        0        0     1001 2023-06-27 19:40:44.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/factory_test/person.py
--rw-rw-rw-   0        0        0     4608 2023-06-27 19:55:32.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/test_mixin_paginate.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:56:23.508279 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/
--rw-rw-rw-   0        0        0     4285 2023-06-27 19:56:23.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-06-27 19:56:23.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 19:56:23.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-27 19:56:23.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-27 19:56:23.000000 hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 19:56:23.535277 hipal_mixin_scrud-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-06-27 19:56:11.000000 hipal_mixin_scrud-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.388429 hipal_mixin_scrud-1.0.7/
+-rw-rw-rw-   0        0        0     4285 2023-07-05 20:23:57.386431 hipal_mixin_scrud-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3860 2023-06-27 19:42:51.000000 hipal_mixin_scrud-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.339429 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.361432 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/crud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/crud/__init__.py
+-rw-rw-rw-   0        0        0     5707 2023-07-05 20:11:58.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/crud/generator.py
+-rw-rw-rw-   0        0        0     3504 2023-07-05 20:13:57.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/crud/mixin_list.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.366429 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/enums/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/enums/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-06-22 17:45:04.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/enums/operators.py
+-rw-rw-rw-   0        0        0       82 2023-06-22 17:45:06.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/enums/sorts.py
+-rw-rw-rw-   0        0        0     5057 2023-07-05 20:12:24.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/mixin.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.373430 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/schemas/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/schemas/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-07-05 20:11:58.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/schemas/paginate_params.py
+-rw-rw-rw-   0        0        0      364 2023-07-05 20:13:50.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/schemas/pagination_base.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.379429 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-23 18:53:11.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.384431 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/factory_test/
+-rw-rw-rw-   0        0        0        0 2023-06-23 18:57:52.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/factory_test/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-07-05 20:13:38.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/factory_test/person.py
+-rw-rw-rw-   0        0        0     4592 2023-07-05 20:13:32.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/test_mixin_paginate.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:57.355430 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/
+-rw-rw-rw-   0        0        0     4285 2023-07-05 20:23:57.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-07-05 20:23:57.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 20:23:57.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-05 20:23:57.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-05 20:23:57.000000 hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 20:23:57.388429 hipal_mixin_scrud-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-07-05 20:23:55.000000 hipal_mixin_scrud-1.0.7/setup.py
```

### Comparing `hipal_mixin_scrud-1.0.6/PKG-INFO` & `hipal_mixin_scrud-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipal_mixin_scrud
-Version: 1.0.6
+Version: 1.0.7
 Summary: Libreria para crud basica.
 Home-page: http://git.hipal.com.co/libraries/ms-mixins/-/tree/feature/mixins
 Author: Hipal
 Author-email: desarrollo@hipal.com.co
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `hipal_mixin_scrud-1.0.6/README.md` & `hipal_mixin_scrud-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/crud/generator.py` & `hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/crud/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         has_get_one: bool = True,
         has_delete_one: bool = True,
         **kwargs: Any,
     ) -> None:
         self.model = model
         self.db_session = db_session
         self.schema = schema
-        self._pk: str = self._pk if hasattr(self, "_pk") else "id"
+        self._pk = [c.key for c in self.model.__table__.c if c.primary_key][0]
         self.create_schema = (
             create_schema
             if create_schema
             else self.schema_factory(self.schema, pk_field_name=self._pk, name="Create")
         )
         self.update_schema = (
             update_schema
@@ -104,35 +104,35 @@
                 response_model=self.schema,
                 summary="Create One",
                 dependencies=[],
             )
 
         if has_get_one:
             self._add_api_route(
-                "/{item_id}",
+                "/{item}",
                 self._get_one(),
                 methods=["GET"],
                 response_model=self.schema,
                 summary="Get One",
                 dependencies=[],
             )
 
         if has_update:
             self._add_api_route(
-                "/{item_id}",
+                "/{item}",
                 self._update(),
                 methods=["PUT"],
                 response_model=self.schema,
                 summary="Update One",
                 dependencies=[],
             )
 
         if has_delete_one:
             self._add_api_route(
-                "/{item_id}",
+                "/{item}",
                 self._delete_one(),
                 methods=["DELETE"],
                 summary="Delete One",
                 dependencies=[],
             )
 
     def _add_api_route(
```

### Comparing `hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/crud/mixin_list.py` & `hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/crud/mixin_list.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/mixin.py` & `hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,109 +60,108 @@
             has_create=has_create,
             has_get_one=has_get_one,
             has_delete_one=has_delete_one,
             **kwargs,
         )
 
     def get_message(self, http_code):
-        
-        error_mesages = self.error_messages if self.error_messages else {
-            "not_found": "Recurso no encontrado.",
-            "already_exists": "El dato ya existe.",
-        }
-        
+        error_mesages = (
+            self.error_messages
+            if self.error_messages
+            else {
+                "not_found": "Recurso no encontrado.",
+                "already_exists": "El dato ya existe.",
+            }
+        )
+
         return error_mesages.get(http_code)
-    
+
     def _fk_fields(self, model: Model):
         foreign_keys = [c.key for c in model.__table__.c if c.foreign_keys]
         return foreign_keys
 
     def _get_one_db(self, item_id, query: Query = None):
         item = (
             query.filter(getattr(self.model, self._pk) == item_id).first()
             if self.query
             else self.db_session.query(self.model)
             .filter(getattr(self.model, self._pk) == item_id)
             .first()
         )
-        
+
         msg_response = self.get_message("not_found")
 
         if not item:
             raise HTTPException(404, msg_response)
 
         return item
 
     def _get_paginate(self, *args: Any, **kwargs: Any):
         def route(
             request: Request,
             paginate_params: PaginateParams = Depends(),
         ):
-
             query = None
 
             if self.query:
                 query = self.query(request)
 
             path = request.url._url.split("?")[0]
             return self.paginate(
                 db_session=self.db_session,
                 model=self.model,
                 paginate_params=paginate_params,
                 squema=self.schema,
                 path=path,
                 query_model=query,
             )
-    
 
         return route
 
     def _get_one(self, *args: Any, **kwargs: Any):
-        def route(request: Request, item_id):
+        def route(request: Request, item):
             query = None
             if self.query:
                 query = self.query(request)
-            return self._get_one_db(item_id, query)
+            return self._get_one_db(item, query)
 
         return route
 
     def _create(self, *args: Any, **kwargs: Any):
         def route(model: self.create_schema):
-
             db_model = self.model(**model.dict())
             self.db_session.add(db_model)
             self.db_session.commit()
             self.db_session.refresh(db_model)
 
             return db_model
 
         return route
 
     def _update(self, *args: Any, **kwargs: Any):
         def route(
-            item_id,
+            item,
             model: self.update_schema,
         ):
-
-            db_model = self._get_one_db(item_id)
+            db_model = self._get_one_db(item)
 
             for key, value in model.dict(exclude={self._pk}).items():
                 if hasattr(db_model, key):
                     setattr(db_model, key, value)
 
             self.db_session.commit()
             self.db_session.refresh(db_model)
             return db_model
 
         return route
 
     def _delete_one(self, *args: Any, **kwargs: Any):
-        def route(request: Request, item_id):
+        def route(request: Request, item):
             query = None
             if self.query:
                 query = self.query(request)
-            db_model = self._get_one_db(item_id, query)
+            db_model = self._get_one_db(item, query)
             self.db_session.delete(db_model)
             self.db_session.commit()
             return Response(status_code=204)
 
         return route
```

### Comparing `hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/factory_test/person.py` & `hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/factory_test/person.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.6/hipal_mixin_scrud/tests/test_mixin_paginate.py` & `hipal_mixin_scrud-1.0.7/hipal_mixin_scrud/tests/test_mixin_paginate.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # unittest
 from unittest.mock import MagicMock
 from unittest.mock import patch
 import unittest
 
 # fast api
 from fastapi.testclient import TestClient
-from fastapi import FastAPI
+from fastapi import FastAPI, status
 
 # sqlalchemy
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session
 
 # app
@@ -20,129 +20,127 @@
 from hipal_mixin_scrud.tests.factory_test.person import PersonSchema
 from hipal_mixin_scrud.tests.factory_test.person import PersonModel
 from hipal_mixin_scrud.crud.mixin_list import ListModelMixin
 from hipal_mixin_scrud.mixin import MixinCrud
 
 
 class TestMixin(unittest.TestCase):
-    
     def factory_list_to_dict(self, list_to_dict: list):
-        return [{k:v for k ,v in item.__dict__.items() if k != '_sa_instance_state'} for item in list_to_dict]
+        return [
+            {k: v for k, v in item.__dict__.items() if k != "_sa_instance_state"}
+            for item in list_to_dict
+        ]
 
     def factory_obj_to_dict(self, obj: object):
-        return {k:v for k ,v in obj.__dict__.items() if k != '_sa_instance_state'}
+        return {k: v for k, v in obj.__dict__.items() if k != "_sa_instance_state"}
 
-    @patch('crud.mixin_list.ListModelMixin.paginate')
+    @patch("hipal_mixin_scrud.crud.mixin_list.ListModelMixin.paginate")
     def test_success_paginate(self, mocker):
-        
         mock_db_session = Session()
-        
+
         persons: list[PersonFactory] = PersonFactory.create_batch(10)
-        
-        obj =  {
-            "pagination":{
+
+        obj = {
+            "pagination": {
                 "offset": 0,
                 "limit": 10,
                 "total": 10,
                 "total_pages": 1,
                 "links": {
-                    "first":'localhost',
-                    "prev": 'localhost',
-                    "next": 'localhost',
-                    "last": 'localhost',
+                    "first": "localhost",
+                    "prev": "localhost",
+                    "next": "localhost",
+                    "last": "localhost",
                 },
             },
-            "data": self.factory_list_to_dict(persons)
-        }        
-        
+            "data": self.factory_list_to_dict(persons),
+        }
+
         mocker.return_value = obj
 
         list_model_mixin = ListModelMixin()
         result = list_model_mixin.paginate(
             db_session=mock_db_session,
             model=PersonModel,
             squema=PersonSchema,
-            path='localhost',
+            path="localhost",
         )
 
         assert result == obj
 
     def session(self):
         engine = create_engine(
-            'postgresql://user:pass@db:5432/db',
-        )
-        Session = sessionmaker(
-            bind=engine,
-            autocommit=False,
-            autoflush=False
+            "postgresql://user:pass@db:5432/db",
         )
-        
+        Session = sessionmaker(bind=engine, autocommit=False, autoflush=False)
+
         db_session = Session()
-        
-        return db_session
 
+        return db_session
 
     def mock_refresh(self, model):
-        person_refresh: PersonFactory = PersonFactory.create(id=2)
+        person_refresh: PersonFactory = PersonFactory.create()
         model.name_1 = person_refresh.name_1
         model.name_2 = person_refresh.name_2
         model.last_name_1 = person_refresh.last_name_1
         model.last_name_2 = person_refresh.last_name_2
         model.rh = person_refresh.rh
 
-
     def test_routes(self):
-        
         mock_session = MagicMock()
-        mock_session = self.session().create_session = MagicMock(return_value=mock_session)
-        
+        mock_session = self.session().create_session = MagicMock(
+            return_value=mock_session
+        )
+
         mock_model = MagicMock(spec=PersonModel)
         persons: list[PersonFactory] = PersonFactory.create_batch(10)
         person1: PersonFactory = PersonFactory.create(id=1)
         person2: PersonFactory = PersonFactory.create(id=2)
-        
-        mock_session.query.return_value.order_by.return_value.limit.return_value.offset.return_value.all.return_value = persons
+
+        mock_session.query.return_value.order_by.return_value.limit.return_value.offset.return_value.all.return_value = (
+            persons
+        )
         mock_session.query.return_value.filter.return_value.first.return_value = person1
         mock_session.refresh = self.mock_refresh
 
-        url = 'api/v1/items'
+        url = "api/v1/items"
 
         mixin_route = MixinCrud(
             schema=PersonSchema,
             db_session=mock_session,
             model=mock_model,
             prefix=url,
         )
-        
-        app = FastAPI(title='items')
+
+        app = FastAPI(title="items")
         app.include_router(mixin_route)
 
         client = TestClient(app)
 
         item_url = f"{url}/1"
 
         actions = [
-            ('get', url, {}),
-            ('get', item_url, {}),
-            ('post', url, self.factory_obj_to_dict(person2)),
-            ('put', item_url, self.factory_obj_to_dict(person2)),
-            ('delete', item_url, {}),
+            ("get", url, {}),
+            ("get", item_url, {}),
+            ("post", url, self.factory_obj_to_dict(person2)),
+            ("put", item_url, self.factory_obj_to_dict(person2)),
+            ("delete", item_url, {}),
         ]
-        
+
         success_codes = []
 
         for method, url, data in actions:
-
             request = client.request(
                 method,
-                url, 
-                headers = {'Content-Type': 'application/json'},
-                data=json.dumps(data)
+                url,
+                headers={"Content-Type": "application/json"},
+                data=json.dumps(data),
             )
             status_code = request.status_code
-            assert 200 <= status_code <= 226
+            assert status.HTTP_200_OK <= status_code <= status.HTTP_226_IM_USED
             success_codes.append(status_code)
-    
+
         assert len(success_codes) == len(actions)
 
-if __name__ == '__main__':
-    unittest.main()
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/PKG-INFO` & `hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipal-mixin-scrud
-Version: 1.0.6
+Version: 1.0.7
 Summary: Libreria para crud basica.
 Home-page: http://git.hipal.com.co/libraries/ms-mixins/-/tree/feature/mixins
 Author: Hipal
 Author-email: desarrollo@hipal.com.co
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `hipal_mixin_scrud-1.0.6/hipal_mixin_scrud.egg-info/SOURCES.txt` & `hipal_mixin_scrud-1.0.7/hipal_mixin_scrud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.6/setup.py` & `hipal_mixin_scrud-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Lee el contenido del archivo README.md
 readme_path = Path(__file__).parent / "README.md"
 with open(readme_path, "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name="hipal_mixin_scrud",
-    version="1.0.6",
+    version="1.0.7",
     description="Libreria para crud basica.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.9",
     install_requires=[
         "pydantic==1.10.7",
```

