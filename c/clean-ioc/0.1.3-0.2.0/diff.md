# Comparing `tmp/clean_ioc-0.1.3.tar.gz` & `tmp/clean_ioc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.1.3.tar", max compression
+gzip compressed data, was "clean_ioc-0.2.0.tar", max compression
```

## Comparing `clean_ioc-0.1.3.tar` & `clean_ioc-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/LICENSE
--rw-r--r--   0        0        0    15650 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/README.md
--rw-r--r--   0        0        0    32533 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/clean_ioc/__init__.py
--rw-r--r--   0        0        0      674 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0     1811 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6569 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1125 2023-06-20 21:25:32.652480 clean_ioc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    16897 1970-01-01 00:00:00.000000 clean_ioc-0.1.3/setup.py
--rw-r--r--   0        0        0    16290 1970-01-01 00:00:00.000000 clean_ioc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/LICENSE
+-rw-r--r--   0        0        0    16473 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/README.md
+-rw-r--r--   0        0        0    33608 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     1320 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0     1959 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      587 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6569 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1125 2023-07-05 17:51:44.915057 clean_ioc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17746 1970-01-01 00:00:00.000000 clean_ioc-0.2.0/setup.py
+-rw-r--r--   0        0        0    17113 1970-01-01 00:00:00.000000 clean_ioc-0.2.0/PKG-INFO
```

### Comparing `clean_ioc-0.1.3/LICENSE` & `clean_ioc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.3/README.md` & `clean_ioc-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     type(root.child) # returns DecoratorTwo
     type(root.child.child) # returns Concrete
 ```
 
 
 ## Subclasses registration
 
-This feature allows registartion of all subclasses of a giveb type
+This feature allows registration of all subclasses of a giveb type
 
 ```python
 class Client(abc.ABC)
     @abc.abstractmethod
     def get_number(self):
         pass
 
@@ -398,74 +398,74 @@
 
 with container.get_scope() as scope:
     scope.register(int, instance=10)
     scoped_client = scope.resolve(Client)
     scoped_client.get_number() # returns 10
 ```
 
-## Named registartions & Registartion filters
+## Named registrations & Registration filters
 
-By default the last registration is what the container will return when resolve is called as below.
+By default the last unnamed registration is what the container will return when resolve is called as below.
 
 ```python
 
 container = Container()
 container.register(int, instance=1)
 container.register(int, instance=2)
 container.register(int, instance=3)
 
 number = container.resolve(int) # returns 3
 
 ```
-To be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.
+To be more selective of what we return we can add a name to the registration and apply a registration filter when we resolve.
 
-A registartion filter is simply function that receives a **Registartion** and returns a **bool**
+A registration filter is simply function that receives a **Registration** and returns a **bool**
 
 For example if we wanted to get the int named **"One"** we do the following
 
 ```python
 container = Container()
 container.register(int, instance=1, name="One")
 container.register(int, instance=2, name="Two")
 container.register(int, instance=3, name="Three")
 
 number = container.resolve(int, filter=lambda r: r.name == "One") # returns 1
 ```
 
-Clean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)
+Clean IOC comes with a set of in built registration filters that can be found [here](./clean_ioc/registration_filters.py)
 
 We can get the desired behaviour as above
 ```python
-from clean_ioc.registartion_filters import with_name
+from clean_ioc.registration_filters import with_name
 
 container = Container()
 container.register(int, instance=1, name="One")
 container.register(int, instance=2, name="Two")
 container.register(int, instance=3, name="Three")
 
 number = container.resolve(int, filter=with_name("One")) # returns 1
 ```
 
 ## Dependency Settings
 
-Dependency settings are defined at registartion and allow you to define the selection or setting dependencies
+Dependency settings are defined at registration and allow you to define the selection or setting dependencies
 
 
 ```python
 class Client
     def __init__(self, number=10)
         self.number = number
 
     def get_number(self):
         return self.number
 
 container = Container()
 
 container.register(int, instance=1, name="One")
-container.register(int, instance=2, name="Two")
+container.register(int, instance=2)
 
 container.register(
     Client,
     name="SetsValue",
     dependency_config={"number": DependencySettings(value=50)}
 )
 container.register(
@@ -475,22 +475,22 @@
 container.register(
     Client,
     name="IgnoresDefaultParameterValue",
     dependency_config={"number": DependencySettings(use_default_paramater=False)}
 )
 container.register(
     Client,
-    name="UsesRegistartionFilter",
+    name="UsesRegistrationFilter",
     dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}
 )
 
 client1 = container.resolve(Client, filter=with_name("SetsValue"))
 client2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))
 client3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))
-client4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))
+client4 = container.resolve(Client, filter=with_name("UsesRegistrationFilter"))
 
 
 client1.get_number() # returns 50
 client2.get_number() # returns 10
 client3.get_number() # returns 2
 client4.get_number() # returns 1
 ```
@@ -506,16 +506,42 @@
     def __init__(self, number=10)
         self.number = number
     ```
     If you don't want to use the default parameter value you can set it to false in the dependency setting
     ```python
     DependencySettings(use_default_paramater=False)
     ```
-3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.
+3. Going to the container registry to find a registration using the registration filter if, if there is a default value on the dependant paramater you must explicity set.
+
+
+## Tags
+
+Tags can be added to registrations in order to support filtering. This can be useful as a means to filter registrations when resolving lists of a particular type
+
+```python
+class A:
+    pass
+
+a1 = A()
+a2 = A()
+a3 = A()
 
+container = Container()
+
+container.register(A, instance=a1, tags=[Tag("a", "a1")])
+container.register(A, instance=a2, tags=[Tag("a")])
+container.register(A, instance=a3)
+
+ar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1
+al1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]
+al2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]
+al3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]
+al4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]
+al5 = container.resolve(list[A]) # returns [a3, a2, a1]
+```
 ## Accessing the Container, Scope and Resolver within dependencies
 
 Accessing container directly
 
 ```python
 class Client
     def __init__(self, container: Container)
@@ -571,15 +597,15 @@
 with container.get_scope() as scope:
     scope.register(int, instance=10)
     scoped_client = scope.resolve(Client)
     scoped_client.get_number() # returns 10
 ```
 
 
-## Modules (BETA feature)
+## Modules
 
 
 A module is a just a function that accepts a container, it can be used to set up common elements on the container
 
 ```python
 class ClientDependency
     def get_int(self):
```

### Comparing `clean_ioc-0.1.3/clean_ioc/__init__.py` & `clean_ioc-0.2.0/clean_ioc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 from __future__ import annotations
 import abc
 from collections import defaultdict, deque
 from dataclasses import dataclass
 import types
 from enum import IntEnum
-from typing import Any, Sequence, Type, get_type_hints
+from typing import Any, Type, get_type_hints
 from collections.abc import Callable
 from typing import _GenericAlias  # type: ignore
 from uuid import uuid4
 from .functional_utils import constant, fn_and, fn_not
 from .type_filters import is_abstract
 from .typing_utils import (
     get_generic_bases,
@@ -47,15 +47,22 @@
     for name, param in signature.parameters.items():
         if "*" in str(param):
             continue
         d[name] = ArgInfo(name=name, arg_type=args[name], default_value=param.default)
     return d
 
 
-_all_registartions = constant(True)
+def _default_registration_filter(r: Registration) -> bool:
+    return not r.is_named
+
+
+@dataclass
+class Tag:
+    name: str
+    value: str | None = None
 
 
 class Lifespan(IntEnum):
     transient = 0
     once_per_graph = 1
     scoped = 2
     singleton = 3
@@ -332,15 +339,15 @@
 
 
 class PreConfiguration:
     def __init__(
         self,
         service_type: type,
         pre_configuration: Callable[..., None],
-        registration_filter: RegistartionFilter,
+        registration_filter: RegistrationFilter,
         dependency_config: dict[str, DependencySettings],
     ):
         self.service_type = service_type
         self.configuration_fn = pre_configuration
         self.filter = registration_filter
         self.dependency_config = dependency_config
 
@@ -357,27 +364,27 @@
 
 
 class Decorator:
     def __init__(
         self,
         service_type: type,
         decorator_type: type,
-        filter: RegistartionFilter,
+        filter: RegistrationFilter,
         decorated_arg: str | None,
         dependency_config: dict[str, DependencySettings] = {},
     ):
         self.service_type = service_type
         self.decorator_type = decorator_type
         self.creator = DecoratorCreator(
             service_type=service_type,
             decorator_type=decorator_type,
             decorated_arg=decorated_arg,
             dependency_config=dependency_config,
         )
-        self.registartion_filter = filter
+        self.registration_filter = filter
 
     def decorate(
         self,
         instance: Any,
         context: ResolvingContext,
         dependency_node: DependencyNode,
     ):
@@ -390,29 +397,37 @@
     def __init__(
         self,
         service_type: type,
         implementation: Callable,
         lifespan: Lifespan,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
+        tags: list[Tag] | None = None,
     ):
         self.service_type = service_type
         self.implementation = implementation
         self.creator = ImplementationCreator(
             creator_function=implementation, dependency_config=dependency_config
         )
         self.lifespan = lifespan
         self.name = name
+        self.tags = tuple(tags) if tags else tuple()
         self._id = str(uuid4())
         self.generic_mapping = get_typevar_to_type_mapping(self.service_type)
 
     @property
     def is_named(self):
         return self.name is not None
 
+    def has_tag(self, name: str, value: str | None):
+        if value is not None:
+            return any(t.name == name and t.value == value for t in self.tags)
+
+        return any(t.name == name for t in self.tags)
+
     def build(self, context: ResolvingContext, parent_node: DependencyNode):
         my_node = DependencyNode(
             service_type=self.service_type,
             implementation=self.implementation,
             lifespan=self.lifespan,
         )
 
@@ -455,42 +470,42 @@
         self._decorators: dict[type, deque[Decorator]] = defaultdict(deque)
         self._pre_configurations: dict[type, deque[PreConfiguration]] = defaultdict(
             deque
         )
         self._singletons: dict[str, Any] = {}
         self._run_preconfigurations: list[str] = []
 
-    def add_registration(self, registartion: Registration):
-        self._registrations[registartion.service_type].appendleft(registartion)
+    def add_registration(self, registration: Registration):
+        self._registrations[registration.service_type].appendleft(registration)
 
     def add_decorator(self, decorator: Decorator):
         self._decorators[decorator.service_type].appendleft(decorator)
 
     def add_pre_configuration(self, pre_configuration: PreConfiguration):
         self._pre_configurations[pre_configuration.service_type].appendleft(
             pre_configuration
         )
 
-    def add_singleton_instance(self, registartion_id: str, instance: Any):
-        self._singletons[registartion_id] = instance
+    def add_singleton_instance(self, registration_id: str, instance: Any):
+        self._singletons[registration_id] = instance
 
     def mark_pre_configuration_as_run(self, pre_configuration_id):
         self._run_preconfigurations.append(pre_configuration_id)
 
-    def get_registartions(self, service_type: type):
+    def get_registrations(self, service_type: type):
         return self._registrations[service_type]
 
     def get_pre_configurations(self, service_type: type):
         return self._pre_configurations[service_type]
 
     def get_decorators(self, service_type: type):
         return self._decorators[service_type]
 
-    def get_singleton(self, registartion_id):
-        return self._singletons.get(registartion_id)
+    def get_singleton(self, registration_id):
+        return self._singletons.get(registration_id)
 
     @property
     def singletons(self):
         return self._singletons
 
     @property
     def run_pre_configurations(self):
@@ -535,15 +550,17 @@
 class ResolvingContext:
     def __init__(self, registry: Registry, scope: Scope):
         self.registry = registry
         self.scope = scope
         self._cache = DependencyCache(registry=registry, scope=scope)
 
     def try_generic_fallback(self, service_type: _GenericAlias):
-        return self.find_registration(service_type.__origin__, _all_registartions)
+        return self.find_registration(
+            service_type.__origin__, _default_registration_filter
+        )
 
     def find_registration(
         self, service_type: type, registration_finder: Callable
     ) -> Registration:
         regs = self.find_registrations(service_type, registration_finder)
         reg = next(iter(regs), None)
 
@@ -556,29 +573,29 @@
         return reg
 
     def find_registrations(
         self, service_type: type, registration_filter: Callable[[Registration], bool]
     ) -> list[Registration]:
         scoped_registrations = [
             r
-            for r in self.scope.get_registartions(service_type)
+            for r in self.scope.get_registrations(service_type)
             if registration_filter(r)
         ]
         container_registrations = [
             r
-            for r in self.registry.get_registartions(service_type)
+            for r in self.registry.get_registrations(service_type)
             if registration_filter(r)
         ]
         return scoped_registrations + container_registrations
 
     def find_decorators_that_apply(self, registration: Registration):
         return [
             d
             for d in self.registry.get_decorators(registration.service_type)
-            if d.registartion_filter(registration)
+            if d.registration_filter(registration)
         ]
 
     def find_pre_configurations_that_apply(self, registration: Registration):
         return [
             c
             for c in self.registry.get_pre_configurations(registration.service_type)
             if c.id not in self.registry.run_pre_configurations
@@ -596,15 +613,15 @@
 
 
 class Resolver(abc.ABC):
     @abc.abstractmethod
     def resolve(
         self,
         cls: type,
-        filter: RegistartionFilter = _all_registartions,
+        filter: RegistrationFilter = _default_registration_filter,
         *args,
         **kwargs,
     ) -> Any:
         pass
 
 
 class Scope(Resolver):
@@ -632,15 +649,15 @@
         factory: Callable | None = None,
         instance: Any | None = None,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
     ):
         pass
 
-    def get_registartions(self, service_tyep):
+    def get_registrations(self, service_tyep):
         return self._registrations[service_tyep]
 
     @property
     def scoped_instances(self):
         return self._scoped_instances
 
 
@@ -657,52 +674,57 @@
         self,
         service_type: type,
         impl_type: type | None = None,
         factory: Callable | None = None,
         instance: Any | None = None,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
+        tags: list[Tag] | None = None,
     ):
         if instance is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=lambda: instance,
                     lifespan=Lifespan.scoped,
                     name=name,
+                    tags=tags,
                 )
             )
         elif factory is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=factory,
                     lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
+                    tags=tags,
                 )
             )
         elif impl_type is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=impl_type,
                     lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
+                    tags=tags,
                 )
             )
         else:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=service_type,
                     lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
+                    tags=tags,
                 )
             )
 
     def _before_start(self):
         pass
 
     def _after_finish(self):
@@ -711,24 +733,24 @@
     def __enter__(self):
         self._before_start()
         return self
 
     def __exit__(self, *args, **kwargs):
         self._after_finish()
 
-    def get_registartions(self, service_tyep):
+    def get_registrations(self, service_tyep):
         return self._registrations[service_tyep]
 
     def add_scoped_instance(self, registration_id: str, instance: Any):
         self._scoped_instances[registration_id] = instance
 
     def resolve(
         self,
         service_type: type,
-        filter: RegistartionFilter = _all_registartions,
+        filter: RegistrationFilter = _default_registration_filter,
     ):
         return self._container.resolve(
             service_type=service_type, filter=filter, scope=self
         )
 
 
 class EmptyContainerScope(Scope):
@@ -768,15 +790,15 @@
         self.register(Container, instance=self)
         self.register(Resolver, instance=self)
 
     def pre_configure(
         self,
         service_type: type,
         configuration_function: Callable[..., None],
-        registration_filter: RegistartionFilter = _all_registartions,
+        registration_filter: RegistrationFilter = _default_registration_filter,
         dependency_config: dict[str, DependencySettings] = {},
     ):
         self.registry.add_pre_configuration(
             PreConfiguration(
                 service_type=service_type,
                 pre_configuration=configuration_function,
                 registration_filter=registration_filter,
@@ -789,75 +811,83 @@
         service_type: type,
         impl_type: type | None = None,
         factory: Callable | None = None,
         instance: Any | None = None,
         lifespan: Lifespan = Lifespan.once_per_graph,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
+        tags: list[Tag] | None = None,
     ):
         if instance is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=lambda: instance,
                     dependency_config=dependency_config,
                     lifespan=Lifespan.singleton,
                     name=name,
+                    tags=tags,
                 )
             )
         elif factory is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=factory,
                     dependency_config=dependency_config,
                     lifespan=lifespan,
                     name=name,
+                    tags=tags,
                 )
             )
         elif impl_type is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=impl_type,
                     dependency_config=dependency_config,
                     lifespan=lifespan,
                     name=name,
+                    tags=tags,
                 )
             )
         else:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=service_type,
                     dependency_config=dependency_config,
                     lifespan=lifespan,
                     name=name,
+                    tags=tags,
                 )
             )
 
     def register_subclasses(
         self,
         base_type: type,
         lifespan: Lifespan = Lifespan.once_per_graph,
         subclass_type_filter: Callable[[type], bool] = constant(True),
         get_registration_name: Callable[[type], str | None] = constant(None),
+        tags: list[Tag] | None = None,
     ):
         full_type_filter = fn_and(fn_not(is_abstract), subclass_type_filter)
         subclasses = get_subclasses(base_type, full_type_filter)
         for sc in subclasses:
             name = get_registration_name(sc)
-            self.register(base_type, sc, lifespan=lifespan, name=name)
-            self.register(sc, lifespan=lifespan)
+            self.register(base_type, sc, lifespan=lifespan, name=name, tags=tags)
+            self.register(sc, lifespan=lifespan, tags=tags)
 
     def register_decorator(
         self,
         service_type: type,
         decorator_type: type,
-        registration_filter: Callable[[Registration], bool] = _all_registartions,
+        registration_filter: Callable[
+            [Registration], bool
+        ] = _default_registration_filter,
         decorated_arg: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
     ):
         self.registry.add_decorator(
             Decorator(
                 service_type=service_type,
                 decorator_type=decorator_type,
@@ -884,33 +914,39 @@
         self,
         generic_service_type: type,
         fallback_type: type | None = None,
         fallback_name: str | None = None,
         lifespan: Lifespan = Lifespan.once_per_graph,
         subclass_type_filter: Callable[[type], bool] = constant(True),
         get_registration_name: Callable[[type], str | None] = constant(None),
+        tags: list[Tag] | None = None,
     ):
         full_type_filter = fn_and(fn_not(is_abstract), subclass_type_filter)
         subclasses = get_subclasses(generic_service_type, full_type_filter)
         for subclass in subclasses:
             name = get_registration_name(subclass)
             target_generic_base = self._get_target_generic_base(
                 generic_service_type, subclass
             )
             if target_generic_base:
                 self.register(
-                    target_generic_base, subclass, lifespan=lifespan, name=name
+                    target_generic_base,
+                    subclass,
+                    lifespan=lifespan,
+                    name=name,
+                    tags=tags,
                 )
 
         if fallback_type:
             self.register(
                 generic_service_type,
                 fallback_type,
                 lifespan=lifespan,
                 name=fallback_name,
+                tags=tags,
             )
 
     def register_open_generic_decorator(
         self,
         generic_service_type: type,
         generic_decorator_type: type,
         subclass_type_filter: Callable[[type], bool] = constant(True),
@@ -949,15 +985,15 @@
                         decorated_arg=decorated_arg,
                         dependency_config=dependency_config,
                     )
 
     def resolve(
         self,
         service_type,
-        filter: RegistartionFilter = _all_registartions,
+        filter: RegistrationFilter = _default_registration_filter,
         scope: Scope = EmptyContainerScope(),
     ) -> Any:
         d = RootDependency(service_type, DependencySettings(filter=filter))
         context = ResolvingContext(self.registry, scope)
         return d.resolve_instance(context)
 
     def new_scope(
@@ -971,19 +1007,19 @@
             factory=type_expected_to_be_scoped(service_type, name),
             name=name,
         )
 
     def apply_module(self, module_fn: Callable[[Container], None]):
         module_fn(self)
 
-    def has_registartion(self, service_type):
-        return len(self.registry.get_registartions(service_type)) > 0
+    def has_registration(self, service_type):
+        return len(self.registry.get_registrations(service_type)) > 0
 
 
 @dataclass(kw_only=True)
 class DependencySettings:
     value: Any = _empty
     use_default_paramater: bool = True
-    filter: RegistartionFilter = _all_registartions
+    filter: RegistrationFilter = _default_registration_filter
 
 
-RegistartionFilter = Callable[[Registration], bool]
+RegistrationFilter = Callable[[Registration], bool]
```

### Comparing `clean_ioc-0.1.3/clean_ioc/factories.py` & `clean_ioc-0.2.0/clean_ioc/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from . import Resolver, RegistartionFilter
+from . import Resolver, RegistrationFilter
 from .registration_filters import all_registrations
 from typing import Any, Callable, TypeVar
 
 
-def use_registered(cls: type, filter: RegistartionFilter = all_registrations):
+def use_registered(cls: type, filter: RegistrationFilter = all_registrations):
     def factory(resolver: Resolver):
         return resolver.resolve(cls, filter=filter)
 
     return factory
 
 
 T = TypeVar("T")
 
 
 def create_type_mapping(
     service_type: type[T],
     key_getter: Callable[[T], Any],
-    filter: RegistartionFilter = all_registrations,
+    filter: RegistrationFilter = all_registrations,
 ):
     def factory(resolver: Resolver):
         items = resolver.resolve(list[service_type], filter=filter)
         return {key_getter(item): item for item in items}
 
     return factory
```

### Comparing `clean_ioc-0.1.3/clean_ioc/functional_utils.py` & `clean_ioc-0.2.0/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.3/clean_ioc/registration_filters.py` & `clean_ioc-0.2.0/clean_ioc/registration_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,73 +2,73 @@
 from .functional_utils import constant, fn_not
 
 all_registrations = constant(True)
 
 
 def with_name(name: str | None):
     """
-    Filter registartions equal the name
+    Filter registrations equal the name
     """
 
     def predicate(r: Registration):
         return r.name == name
 
     return predicate
 
 
 def name_starts_with(prefix: str):
     """
-    Filter registartions where the name starts the prefix
+    Filter registrations where the name starts the prefix
     """
 
     def predicate(r: Registration):
         if r.name is not None:
             return r.name.startswith(prefix)
         return False
 
     return predicate
 
 
 def name_ends_with(suffix: str):
     """
-    Filter registartions where the name ends the suffix
+    Filter registrations where the name ends the suffix
     """
 
     def predicate(r: Registration):
         if r.name is not None:
             return r.name.endswith(suffix)
         return False
 
     return predicate
 
 
 def is_named(r: Registration):
     """
-    Filter registartions that have a name
+    Filter registrations that have a name
     """
     return r.is_named
 
 
 is_not_named = with_name(None)
 
 
 def with_implementation(implementation: type):
     """
-    Filter to registartions that have the implementation
+    Filter to registrations that have the implementation
     """
 
     def predicate(r: Registration):
         return r.implementation == implementation
 
     return predicate
 
 
 def has_generic_args_matching(pair: tuple[type, type]):
     """
-    Filter registartions where generic type arg matches
+    Filter registrations where generic type arg matches
     >>> TBar = TypeVar("TBar")
     >>> class Foo(Generic[TBar]):
     ...    pass
     >>> class IntFoo(Foo[int]):
     ...    pass
     >>> class StringFoo(Foo[str]):
     ...    pass
@@ -77,7 +77,14 @@
     >>> container.resolve(Foo, filter=has_generic_args_matching((TBar, int))) # returns instance of IntFoo
     """
 
     def predicate(r: Registration):
         return r.generic_mapping.get(pair[0]) == pair[1]
 
     return predicate
+
+
+def has_tag(name: str, value: str | None = None):
+    def predicate(r: Registration):
+        return r.has_tag(name, value)
+
+    return predicate
```

### Comparing `clean_ioc-0.1.3/clean_ioc/type_filters.py` & `clean_ioc-0.2.0/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.3/clean_ioc/typing_utils.py` & `clean_ioc-0.2.0/clean_ioc/typing_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.3/pyproject.toml` & `clean_ioc-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "0.1.3"
+version = "0.2.0"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://github.com/peter-daly/clean_ioc"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://github.com/peter-daly/clean_ioc"
 readme = "README.md"
```

### Comparing `clean_ioc-0.1.3/setup.py` & `clean_ioc-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['clean_ioc']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'clean-ioc',
-    'version': '0.1.3',
+    'version': '0.2.0',
     'description': 'An IOC Container for Python 3.10+',
-    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registartion of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registartions & Registartion filters\n\nBy default the last registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.\n\nA registartion filter is simply function that receives a **Registartion** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registartion_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registartion and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistartionFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules (BETA feature)\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\nclient = container.resolve(Client)\n\n\n```\n\n\n## Pre-configurations\n\nPre configurations run a side-effect for a type before the type gets resolved.\nThis is useful if some python modules have some sort of module level functions that need to be called before the object get created\n\n```python\nimport logging\n\nclass Client\n    def __init__(self, logger: logging.Logger)\n        self.logger = logger\n\n    def do_a_thing(self):\n        self.logger.info(\'Doing a thing\')\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return logging.getLogger(module)\n\ndef configuring_logging():\n    logging.basicConfig()\n\n\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(logging.Logger, factory=logger_fac)\ncontainer.pre_configure(logging.Logger, configuring_logging)\n\nclient = container.resolve(Client)\n\n\n```',
+    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registration of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registrations & Registration filters\n\nBy default the last unnamed registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registration filter when we resolve.\n\nA registration filter is simply function that receives a **Registration** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registration filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registration_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registration and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2)\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistrationFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistrationFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registration using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n\n## Tags\n\nTags can be added to registrations in order to support filtering. This can be useful as a means to filter registrations when resolving lists of a particular type\n\n```python\nclass A:\n    pass\n\na1 = A()\na2 = A()\na3 = A()\n\ncontainer = Container()\n\ncontainer.register(A, instance=a1, tags=[Tag("a", "a1")])\ncontainer.register(A, instance=a2, tags=[Tag("a")])\ncontainer.register(A, instance=a3)\n\nar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1\nal1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]\nal2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]\nal3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]\nal4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]\nal5 = container.resolve(list[A]) # returns [a3, a2, a1]\n```\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\nclient = container.resolve(Client)\n\n\n```\n\n\n## Pre-configurations\n\nPre configurations run a side-effect for a type before the type gets resolved.\nThis is useful if some python modules have some sort of module level functions that need to be called before the object get created\n\n```python\nimport logging\n\nclass Client\n    def __init__(self, logger: logging.Logger)\n        self.logger = logger\n\n    def do_a_thing(self):\n        self.logger.info(\'Doing a thing\')\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return logging.getLogger(module)\n\ndef configuring_logging():\n    logging.basicConfig()\n\n\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(logging.Logger, factory=logger_fac)\ncontainer.pre_configure(logging.Logger, configuring_logging)\n\nclient = container.resolve(Client)\n\n\n```',
     'author': 'Peter Daly',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/peter-daly/clean_ioc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clean_ioc-0.1.3/PKG-INFO` & `clean_ioc-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-ioc
-Version: 0.1.3
+Version: 0.2.0
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -235,15 +235,15 @@
     type(root.child) # returns DecoratorTwo
     type(root.child.child) # returns Concrete
 ```
 
 
 ## Subclasses registration
 
-This feature allows registartion of all subclasses of a giveb type
+This feature allows registration of all subclasses of a giveb type
 
 ```python
 class Client(abc.ABC)
     @abc.abstractmethod
     def get_number(self):
         pass
 
@@ -415,74 +415,74 @@
 
 with container.get_scope() as scope:
     scope.register(int, instance=10)
     scoped_client = scope.resolve(Client)
     scoped_client.get_number() # returns 10
 ```
 
-## Named registartions & Registartion filters
+## Named registrations & Registration filters
 
-By default the last registration is what the container will return when resolve is called as below.
+By default the last unnamed registration is what the container will return when resolve is called as below.
 
 ```python
 
 container = Container()
 container.register(int, instance=1)
 container.register(int, instance=2)
 container.register(int, instance=3)
 
 number = container.resolve(int) # returns 3
 
 ```
-To be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.
+To be more selective of what we return we can add a name to the registration and apply a registration filter when we resolve.
 
-A registartion filter is simply function that receives a **Registartion** and returns a **bool**
+A registration filter is simply function that receives a **Registration** and returns a **bool**
 
 For example if we wanted to get the int named **"One"** we do the following
 
 ```python
 container = Container()
 container.register(int, instance=1, name="One")
 container.register(int, instance=2, name="Two")
 container.register(int, instance=3, name="Three")
 
 number = container.resolve(int, filter=lambda r: r.name == "One") # returns 1
 ```
 
-Clean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)
+Clean IOC comes with a set of in built registration filters that can be found [here](./clean_ioc/registration_filters.py)
 
 We can get the desired behaviour as above
 ```python
-from clean_ioc.registartion_filters import with_name
+from clean_ioc.registration_filters import with_name
 
 container = Container()
 container.register(int, instance=1, name="One")
 container.register(int, instance=2, name="Two")
 container.register(int, instance=3, name="Three")
 
 number = container.resolve(int, filter=with_name("One")) # returns 1
 ```
 
 ## Dependency Settings
 
-Dependency settings are defined at registartion and allow you to define the selection or setting dependencies
+Dependency settings are defined at registration and allow you to define the selection or setting dependencies
 
 
 ```python
 class Client
     def __init__(self, number=10)
         self.number = number
 
     def get_number(self):
         return self.number
 
 container = Container()
 
 container.register(int, instance=1, name="One")
-container.register(int, instance=2, name="Two")
+container.register(int, instance=2)
 
 container.register(
     Client,
     name="SetsValue",
     dependency_config={"number": DependencySettings(value=50)}
 )
 container.register(
@@ -492,22 +492,22 @@
 container.register(
     Client,
     name="IgnoresDefaultParameterValue",
     dependency_config={"number": DependencySettings(use_default_paramater=False)}
 )
 container.register(
     Client,
-    name="UsesRegistartionFilter",
+    name="UsesRegistrationFilter",
     dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}
 )
 
 client1 = container.resolve(Client, filter=with_name("SetsValue"))
 client2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))
 client3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))
-client4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))
+client4 = container.resolve(Client, filter=with_name("UsesRegistrationFilter"))
 
 
 client1.get_number() # returns 50
 client2.get_number() # returns 10
 client3.get_number() # returns 2
 client4.get_number() # returns 1
 ```
@@ -523,16 +523,42 @@
     def __init__(self, number=10)
         self.number = number
     ```
     If you don't want to use the default parameter value you can set it to false in the dependency setting
     ```python
     DependencySettings(use_default_paramater=False)
     ```
-3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.
+3. Going to the container registry to find a registration using the registration filter if, if there is a default value on the dependant paramater you must explicity set.
+
+
+## Tags
+
+Tags can be added to registrations in order to support filtering. This can be useful as a means to filter registrations when resolving lists of a particular type
+
+```python
+class A:
+    pass
+
+a1 = A()
+a2 = A()
+a3 = A()
 
+container = Container()
+
+container.register(A, instance=a1, tags=[Tag("a", "a1")])
+container.register(A, instance=a2, tags=[Tag("a")])
+container.register(A, instance=a3)
+
+ar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1
+al1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]
+al2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]
+al3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]
+al4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]
+al5 = container.resolve(list[A]) # returns [a3, a2, a1]
+```
 ## Accessing the Container, Scope and Resolver within dependencies
 
 Accessing container directly
 
 ```python
 class Client
     def __init__(self, container: Container)
@@ -588,15 +614,15 @@
 with container.get_scope() as scope:
     scope.register(int, instance=10)
     scoped_client = scope.resolve(Client)
     scoped_client.get_number() # returns 10
 ```
 
 
-## Modules (BETA feature)
+## Modules
 
 
 A module is a just a function that accepts a container, it can be used to set up common elements on the container
 
 ```python
 class ClientDependency
     def get_int(self):
```

