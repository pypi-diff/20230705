# Comparing `tmp/pymetastore-0.2.0.tar.gz` & `tmp/pymetastore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetastore-0.2.0.tar", last modified: Wed Jun 28 16:31:22 2023, max compression
+gzip compressed data, was "pymetastore-0.3.0.tar", last modified: Wed Jul  5 17:53:16 2023, max compression
```

## Comparing `pymetastore-0.2.0.tar` & `pymetastore-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-06-22 19:20:51.055689 pymetastore-0.2.0/LICENSE
--rw-r--r--   0        0        0     1064 2023-06-26 15:39:01.814661 pymetastore-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-22 19:20:51.056280 pymetastore-0.2.0/pymetastore/__init__.py
--rwxr-xr-x   0        0        0    62034 2023-06-22 19:20:51.056609 pymetastore-0.2.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote
--rw-r--r--   0        0        0  1715657 2023-06-22 19:20:51.059532 pymetastore-0.2.0/pymetastore/hive_metastore/ThriftHiveMetastore.py
--rw-r--r--   0        0        0       57 2023-06-22 19:20:51.059681 pymetastore-0.2.0/pymetastore/hive_metastore/__init__.py
--rw-r--r--   0        0        0     1387 2023-06-22 19:20:51.059785 pymetastore-0.2.0/pymetastore/hive_metastore/constants.py
--rw-r--r--   0        0        0   839918 2023-06-22 19:20:51.061341 pymetastore-0.2.0/pymetastore/hive_metastore/ttypes.py
--rw-r--r--   0        0        0    15768 2023-06-22 19:20:51.061556 pymetastore-0.2.0/pymetastore/htypes.py
--rw-r--r--   0        0        0    21854 2023-06-25 22:31:40.537299 pymetastore-0.2.0/pymetastore/metastore.py
--rw-r--r--   0        0        0     1393 2023-06-28 16:31:22.135518 pymetastore-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    20384 2023-06-28 16:30:14.633596 pymetastore-0.2.0/tests/integration/test_metastore.py
--rw-r--r--   0        0        0    16099 2023-06-22 19:20:51.062181 pymetastore-0.2.0/tests/unit/test_htypes.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 pymetastore-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-22 19:20:51.055689 pymetastore-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1064 2023-06-26 15:39:01.814661 pymetastore-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 19:20:51.056280 pymetastore-0.3.0/pymetastore/__init__.py
+-rwxr-xr-x   0        0        0    62034 2023-06-22 19:20:51.056609 pymetastore-0.3.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote
+-rw-r--r--   0        0        0  1715657 2023-06-22 19:20:51.059532 pymetastore-0.3.0/pymetastore/hive_metastore/ThriftHiveMetastore.py
+-rw-r--r--   0        0        0       57 2023-06-22 19:20:51.059681 pymetastore-0.3.0/pymetastore/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     1387 2023-06-22 19:20:51.059785 pymetastore-0.3.0/pymetastore/hive_metastore/constants.py
+-rw-r--r--   0        0        0   839918 2023-06-22 19:20:51.061341 pymetastore-0.3.0/pymetastore/hive_metastore/ttypes.py
+-rw-r--r--   0        0        0    19260 2023-06-29 00:42:02.585443 pymetastore-0.3.0/pymetastore/htypes.py
+-rw-r--r--   0        0        0    25863 2023-06-30 15:55:18.493216 pymetastore-0.3.0/pymetastore/metastore.py
+-rw-r--r--   0        0        0     3266 2023-06-30 15:36:42.940073 pymetastore-0.3.0/pymetastore/stats.py
+-rw-r--r--   0        0        0     1393 2023-07-05 17:53:16.701437 pymetastore-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22253 2023-06-30 15:55:18.493675 pymetastore-0.3.0/tests/integration/test_metastore.py
+-rw-r--r--   0        0        0    19596 2023-06-29 00:42:02.587038 pymetastore-0.3.0/tests/unit/test_htypes.py
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 pymetastore-0.3.0/PKG-INFO
```

### Comparing `pymetastore-0.2.0/LICENSE` & `pymetastore-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetastore-0.2.0/README.md` & `pymetastore-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pymetastore-0.2.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote` & `pymetastore-0.3.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote`

 * *Files identical despite different names*

### Comparing `pymetastore-0.2.0/pymetastore/hive_metastore/ThriftHiveMetastore.py` & `pymetastore-0.3.0/pymetastore/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.2.0/pymetastore/hive_metastore/constants.py` & `pymetastore-0.3.0/pymetastore/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.2.0/pymetastore/hive_metastore/ttypes.py` & `pymetastore-0.3.0/pymetastore/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.2.0/pymetastore/htypes.py` & `pymetastore-0.3.0/pymetastore/htypes.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,84 +34,198 @@
 
 
 class HType:
     def __init__(self, name: str, category: HTypeCategory):
         self.name = name
         self.category = category
 
+    def __str__(self):
+        return f"{self.__class__.__name__}(name={self.name}, category={self.category})"
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{self.name}', {self.category})"
+
+    def __eq__(self, other):
+        if isinstance(other, HType):
+            return (self.name == other.name) and (self.category == other.category)
+        else:
+            return False
+
 
 class HPrimitiveType(HType):
     def __init__(self, primitive_type: PrimitiveCategory):
         super().__init__(primitive_type.value, HTypeCategory.PRIMITIVE)
         self.primitive_type = primitive_type
 
+    def __str__(self):
+        return f"{self.__class__.__name__}(name={self.name}, category={self.category})"
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}({self.primitive_type})"
+
 
 class HMapType(HType):
     def __init__(self, key_type: HType, value_type: HType):
         super().__init__("MAP", HTypeCategory.MAP)
         self.key_type = key_type
         self.value_type = value_type
 
+    def __str__(self):
+        return f"{super().__str__()}, key_type={str(self.key_type)}, value_type={str(self.value_type)})"
+
+    def __repr__(self):
+        return f"HMapType({repr(self.key_type)}, {repr(self.value_type)})"
+
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return (
+                super().__eq__(other)
+                and (self.key_type == other.key_type)
+                and (self.value_type == other.value_type)
+            )
+        else:
+            return False
+
 
 class HListType(HType):
     def __init__(self, element_type: HType):
         super().__init__("LIST", HTypeCategory.LIST)
         self.element_type = element_type
 
+    def __str__(self):
+        return f"{super().__str__()}, element_type={str(self.element_type)})"
+
+    def __repr__(self):
+        return f"HListType({repr(self.element_type)})"
+
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return super().__eq__(other) and (self.element_type == other.element_type)
+        else:
+            return False
+
 
 class HUnionType(HType):
     def __init__(self, types: List[HType]):
         super().__init__("UNION", HTypeCategory.UNION)
         self.types = types
 
+    def __str__(self):
+        return f"{super().__str__()}, types={str(self.types)})"
+
+    def __repr__(self):
+        return f"HUnionType({repr(self.types)})"
+
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return super().__eq__(other) and (self.types == other.types)
+        else:
+            return False
+
 
 class HVarcharType(HType):
     def __init__(self, length: int):
         MAX_VARCHAR_LENGTH = 65535
         if length > MAX_VARCHAR_LENGTH:
             raise ValueError("Varchar length cannot exceed 65535")
         super().__init__("VARCHAR", HTypeCategory.PRIMITIVE)
         self.length = length
 
+    def __str__(self):
+        return f"HVarcharType(length={self.length})"
+
+    def __repr__(self):
+        return f"HVarcharType({self.length})"
+
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return super().__eq__(other) and (self.length == other.length)
+        else:
+            return False
+
 
 class HCharType(HType):
     def __init__(self, length: int):
         MAX_CHAR_LENGTH = 255
         if length > MAX_CHAR_LENGTH:
             raise ValueError("Char length cannot exceed 255")
         super().__init__("CHAR", HTypeCategory.PRIMITIVE)
         self.length = length
 
+    def __str__(self):
+        return f"HCharType(length={self.length})"
+
+    def __repr__(self):
+        return f"HCharType({self.length})"
+
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return super().__eq__(other) and (self.length == other.length)
+        else:
+            return False
+
 
 class HDecimalType(HType):
     def __init__(self, precision: int, scale: int):
         MAX_PRECISION = 38
         MAX_SCALE = 38
         if precision > MAX_PRECISION:
             raise ValueError("Decimal precision cannot exceed 38")
         if scale > MAX_SCALE:
             raise ValueError("Decimal scale cannot exceed 38")
         super().__init__("DECIMAL", HTypeCategory.PRIMITIVE)
         self.precision = precision
         self.scale = scale
 
+    def __str__(self):
+        return f"HDecimalType(precision={self.precision}, scale={self.scale})"
+
+    def __repr__(self):
+        return f"HDecimalType({self.precision}, {self.scale})"
+
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return (
+                super().__eq__(other)
+                and (self.precision == other.precision)
+                and (self.scale == other.scale)
+            )
+        else:
+            return False
+
 
 class HStructType(HType):
     def __init__(self, names: List[str], types: List[HType]):
         if len(names) != len(types):
             raise ValueError("mismatched size of names and types.")
         if None in names:
             raise ValueError("names cannot contain None")
         if None in types:
             raise ValueError("types cannot contain None")
 
         super().__init__("STRUCT", HTypeCategory.STRUCT)
         self.names = names
         self.types = types
 
+    def __str__(self):
+        return f"{super().__str__()}, names={self.names}, types={self.types})"
+
+    def __repr__(self):
+        return f"HStructType({self.names}, {self.types})"
+
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return (
+                super().__eq__(other)
+                and (self.names == other.names)
+                and (self.types == other.types)
+            )
+        else:
+            return False
+
 
 # We need to maintain a list of the expected serialized type names.
 # Thrift will return the type in string format and we will have to parse it to get the type.
 class SerdeTypeNameConstants(Enum):
     # Primitive types
     VOID = "void"
     BOOLEAN = "boolean"
```

### Comparing `pymetastore-0.2.0/pymetastore/metastore.py` & `pymetastore-0.3.0/pymetastore/metastore.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,24 @@
     Partition,
     PrincipalType,
     SerDeInfo,
     StorageDescriptor,
     Table,
 )
 from .htypes import HType, TypeParser
+from .stats import (
+    BinaryTypeStats,
+    BooleanTypeStats,
+    ColumnStats,
+    DateTypeStats,
+    DecimalTypeStats,
+    DoubleTypeStats,
+    LongTypeStats,
+    StringTypeStats,
+)
 
 
 class HPrincipalType(Enum):
     ROLE = "ROLE"
     USER = "USER"
     GROUP = "GROUP"
 
@@ -616,14 +626,116 @@
             params,
             table.viewOriginalText,
             table.viewExpandedText,
             table.writeId,
             table.owner,
         )
 
+    def get_table_stats(
+        self,
+        table: HTable,
+        columns: List[HColumn],
+    ) -> List[ColumnStats]:
+        assert isinstance(table, HTable)
+        assert isinstance(columns, list)
+
+        if len(columns) > 0:
+            assert all(isinstance(column, HColumn) for column in columns)
+
+        assert table.name is not None
+        assert table.database_name is not None
+        assert table.columns is not None
+        assert len(table.columns) > 0
+
+        if len(columns) == 0:
+            columns = table.columns
+
+        column_names = [column.name for column in columns]
+        results = []
+
+        for column in column_names:
+            res = self.client.get_table_column_statistics(
+                table.database_name,
+                table.name,
+                column,
+            )
+            results.append(res)
+
+        result_columns = []
+        for col in results:
+            for obj in col.statsObj:
+                name = obj.colName
+                col_type = obj.colType
+                stats = obj.statsData
+
+                if stats.booleanStats is not None:
+                    c_stats = BooleanTypeStats(
+                        stats.booleanStats.numTrues,
+                        stats.booleanStats.numFalses,
+                        stats.booleanStats.numNulls,
+                    )
+                elif stats.longStats is not None:
+                    c_stats = LongTypeStats(
+                        stats.longStats.lowValue,
+                        stats.longStats.highValue,
+                        stats.longStats.numNulls,
+                        stats.longStats.numDVs,
+                    )
+                elif stats.doubleStats is not None:
+                    c_stats = DoubleTypeStats(
+                        stats.doubleStats.lowValue,
+                        stats.doubleStats.highValue,
+                        stats.doubleStats.numNulls,
+                    )
+                elif stats.stringStats is not None:
+                    c_stats = StringTypeStats(
+                        stats.stringStats.avgColLen,
+                        stats.stringStats.maxColLen,
+                        stats.stringStats.numDVs,
+                        stats.stringStats.numNulls,
+                    )
+                elif stats.binaryStats is not None:
+                    c_stats = BinaryTypeStats(
+                        stats.binaryStats.avgColLen,
+                        stats.binaryStats.maxColLen,
+                        stats.binaryStats.numNulls,
+                    )
+                elif stats.decimalStats is not None:
+                    c_stats = DecimalTypeStats(
+                        stats.decimalStats.lowValue,
+                        stats.decimalStats.highValue,
+                        stats.decimalStats.numNulls,
+                        stats.decimalStats.numDVs,
+                    )
+                elif stats.dateStats is not None:
+                    c_stats = DateTypeStats(
+                        stats.dateStats.numDVs,
+                        stats.dateStats.lowValue,
+                        stats.dateStats.highValue,
+                        stats.dateStats.numNulls,
+                    )
+                else:
+                    c_stats = None
+
+                result = ColumnStats(
+                    catName=col.statsDesc.catName,
+                    dbName=col.statsDesc.dbName,
+                    tableName=col.statsDesc.tableName,
+                    partName=col.statsDesc.partName,
+                    isTblLevel=col.statsDesc.isTblLevel,
+                    lastAnalyzed=col.statsDesc.lastAnalyzed,
+                    columnName=name,
+                    columnType=col_type,
+                    stats=c_stats,
+                )
+
+                result_columns.append(result)
+
+        return result_columns
+
 
 class _HMSConnection:
     def __init__(self, host, port):
         self.host = host
         self.port = port
         self.transport = None
```

### Comparing `pymetastore-0.2.0/pyproject.toml` & `pymetastore-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymetastore"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python client for the Thrift interface to Hive Metastore"
 authors = [
     { name = "Chris Riccomini", email = "criccomini@apache.org" },
     { name = "Kostas Pardalis" },
 ]
 dependencies = [
     "thrift>=0.16.0",
```

### Comparing `pymetastore-0.2.0/tests/integration/test_metastore.py` & `pymetastore-0.3.0/tests/integration/test_metastore.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     HDatabase,
     HPartition,
     HStorage,
     HTable,
     HiveBucketProperty,
     StorageFormat,
 )
+from pymetastore.stats import BooleanTypeStats
 
 
 @pytest.fixture(scope="module")
 def hive_client():
     host = os.environ.get("HMS_HOST", "localhost")
     port = int(os.environ.get("HMS_PORT", 9083))
     transport = TSocket.TSocket(host, port)
@@ -193,14 +194,54 @@
         tableType="EXTERNAL_TABLE",
     )
 
     if "test_table3" in hive_client.get_all_tables("test_db"):
         hive_client.drop_table("test_db", "test_table3", True)
     hive_client.create_table(table)
 
+    cols4 = [ttypes.FieldSchema(name="col4", type="boolean", comment="c4")]
+
+    storageDesc = ttypes.StorageDescriptor(
+        location="/tmp/test_db/test_table4",
+        cols=cols4,
+        inputFormat="org.apache.hadoop.mapred.TextInputFormat",
+        outputFormat="org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
+        compressed=False,
+        numBuckets=-1,
+        serdeInfo=serde_info,
+        bucketCols=[],
+    )
+
+    table = ttypes.Table(
+        tableName="test_table4",
+        dbName="test_db",
+        owner="owner",
+        createTime=0,
+        lastAccessTime=0,
+        retention=0,
+        sd=storageDesc,
+        partitionKeys=partitionKeys,
+        parameters={},
+        tableType="EXTERNAL_TABLE",
+    )
+
+    if "test_table4" in hive_client.get_all_tables("test_db"):
+        hive_client.drop_table("test_db", "test_table4", True)
+    hive_client.create_table(table)
+
+    stats_desc = ttypes.ColumnStatisticsDesc(True, "test_db", "test_table4", "col4")
+
+    stats = ttypes.BooleanColumnStatsData(10, 10, 0)
+    stats_obj = ttypes.ColumnStatisticsObj(
+        "col4", "boolean", ttypes.ColumnStatisticsData(stats)
+    )
+    col_stats = ttypes.ColumnStatistics(stats_desc, [stats_obj])
+
+    hive_client.update_table_column_statistics(col_stats)
+
 
 def test_list_databases(hive_client):
     assert "test_db" in HMS(hive_client).list_databases()
 
 
 def test_get_database(hive_client):
     hms = HMS(hive_client)
@@ -548,7 +589,23 @@
     assert len(columns[6].type.types) == 2
     assert isinstance(columns[6].type.types[0], HType)
     assert isinstance(columns[6].type.types[0], HPrimitiveType)
     assert columns[6].type.types[0].name == "INT"
     assert isinstance(columns[6].type.types[1], HType)
     assert isinstance(columns[6].type.types[1], HPrimitiveType)
     assert columns[6].type.types[1].name == "STRING"
+
+
+def test_table_stats(hive_client):
+    hms = HMS(hive_client)
+    table = hms.get_table("test_db", "test_table4")
+
+    statistics = hms.get_table_stats(table, [])
+
+    assert len(statistics) == 1
+    assert statistics[0].tableName == "test_table4"
+    assert statistics[0].dbName == "test_db"
+    assert statistics[0].stats is not None
+    assert isinstance(statistics[0].stats, BooleanTypeStats)
+    assert statistics[0].stats.numTrues == 10
+    assert statistics[0].stats.numFalses == 10
+    assert statistics[0].stats.numNulls == 0
```

### Comparing `pymetastore-0.2.0/tests/unit/test_htypes.py` & `pymetastore-0.3.0/tests/unit/test_htypes.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pymetastore.htypes import (
     HCharType,
     HDecimalType,
     HListType,
     HMapType,
     HPrimitiveType,
     HStructType,
+    HType,
     HTypeCategory,
     HUnionType,
     HVarcharType,
     PrimitiveCategory,
     SerdeTypeNameConstants,
     Token,
     TypeParser,
@@ -480,7 +481,120 @@
     parser = TypeParser("uniontype<int,string>")
     ptype = parser.parse_type()
     assert isinstance(ptype, HUnionType)
     assert ptype.types[0].name == "INT"
     assert ptype.types[0].category == HPrimitiveType(PrimitiveCategory.INT).category
     assert ptype.types[1].name == "STRING"
     assert ptype.types[1].category == HPrimitiveType(PrimitiveCategory.STRING).category
+
+
+def test_htype_str_repr():
+    ex = HType("int", PrimitiveCategory.INT)
+    assert str(ex) == "HType(name=int, category=PrimitiveCategory.INT)"
+    assert repr(ex) == "HType('int', PrimitiveCategory.INT)"
+    clone = eval(repr(ex))
+    assert clone == ex
+
+
+def test_hmap_type_str_repr_and_eq():
+    typ = HMapType(
+        HPrimitiveType(PrimitiveCategory.STRING), HPrimitiveType(PrimitiveCategory.INT)
+    )
+    assert isinstance(typ, HMapType)
+    assert (
+        str(typ)
+        == "HMapType(name=MAP, category=HTypeCategory.MAP), key_type=HPrimitiveType(name=STRING, category=HTypeCategory.PRIMITIVE), value_type=HPrimitiveType(name=INT, category=HTypeCategory.PRIMITIVE))"
+    )
+    assert (
+        repr(typ)
+        == "HMapType(HPrimitiveType(PrimitiveCategory.STRING), HPrimitiveType(PrimitiveCategory.INT))"
+    )
+
+    clone = eval(repr(typ))
+    assert clone == typ
+
+
+def test_hlist_type_str_repr_and_eq():
+    _type = HListType(HPrimitiveType(PrimitiveCategory.INT))
+    assert isinstance(_type, HListType)
+    assert (
+        str(_type)
+        == "HListType(name=LIST, category=HTypeCategory.LIST), element_type=HPrimitiveType(name=INT, category=HTypeCategory.PRIMITIVE))"
+    )
+    assert repr(_type) == "HListType(HPrimitiveType(PrimitiveCategory.INT))"
+
+    clone = eval(repr(_type))
+    assert clone == _type
+
+
+def test_hunion_type_str_repr_and_eq():
+    _type = HUnionType(
+        [
+            HPrimitiveType(PrimitiveCategory.INT),
+            HPrimitiveType(PrimitiveCategory.STRING),
+        ]
+    )
+    assert isinstance(_type, HUnionType)
+    assert (
+        str(_type)
+        == "HUnionType(name=UNION, category=HTypeCategory.UNION), types=[HPrimitiveType(PrimitiveCategory.INT), HPrimitiveType(PrimitiveCategory.STRING)])"
+    )
+    assert (
+        repr(_type)
+        == "HUnionType([HPrimitiveType(PrimitiveCategory.INT), HPrimitiveType(PrimitiveCategory.STRING)])"
+    )
+
+    clone = eval(repr(_type))
+    assert clone == _type
+
+
+def test_hvarchar_type_str_repr_and_eq():
+    _type = HVarcharType(10)
+    assert isinstance(_type, HVarcharType)
+    assert str(_type) == "HVarcharType(length=10)"
+    assert repr(_type) == "HVarcharType(10)"
+
+    clone = eval(repr(_type))
+    assert clone == _type
+
+
+def test_hchar_type_str_repr_and_eq():
+    _type = HCharType(10)
+    assert isinstance(_type, HCharType)
+    assert str(_type) == "HCharType(length=10)"
+    assert repr(_type) == "HCharType(10)"
+
+    clone = eval(repr(_type))
+    assert clone == _type
+
+
+def test_hdecimal_type_str_repr_and_eq():
+    _type = HDecimalType(10, 2)
+    assert isinstance(_type, HDecimalType)
+    assert str(_type) == "HDecimalType(precision=10, scale=2)"
+    assert repr(_type) == "HDecimalType(10, 2)"
+
+    clone = eval(repr(_type))
+    assert clone == _type
+
+
+def test_hstruct_type_str_repr_and_eq():
+    _type = HStructType(
+        ["name", "age"],
+        [
+            HPrimitiveType(PrimitiveCategory.STRING),
+            HPrimitiveType(PrimitiveCategory.INT),
+        ],
+    )
+    assert isinstance(_type, HStructType)
+
+    assert (
+        str(_type)
+        == "HStructType(name=STRUCT, category=HTypeCategory.STRUCT), names=['name', 'age'], types=[HPrimitiveType(PrimitiveCategory.STRING), HPrimitiveType(PrimitiveCategory.INT)])"
+    )
+    assert (
+        repr(_type)
+        == "HStructType(['name', 'age'], [HPrimitiveType(PrimitiveCategory.STRING), HPrimitiveType(PrimitiveCategory.INT)])"
+    )
+
+    clone = eval(repr(_type))
+    assert clone == _type
```

### Comparing `pymetastore-0.2.0/PKG-INFO` & `pymetastore-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetastore
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python client for the Thrift interface to Hive Metastore
 Author: Kostas Pardalis
 Author-Email: Chris Riccomini <criccomini@apache.org>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: thrift>=0.16.0
 Description-Content-Type: text/markdown
```

