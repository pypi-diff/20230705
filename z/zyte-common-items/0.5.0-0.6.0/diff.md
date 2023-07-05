# Comparing `tmp/zyte-common-items-0.5.0.tar.gz` & `tmp/zyte-common-items-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-common-items-0.5.0.tar", last modified: Wed May 10 13:31:58 2023, max compression
+gzip compressed data, was "zyte-common-items-0.6.0.tar", last modified: Wed Jul  5 10:33:14 2023, max compression
```

## Comparing `zyte-common-items-0.5.0.tar` & `zyte-common-items-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:58.242227 zyte-common-items-0.5.0/zyte_common_items/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/zyte_common_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/zyte_common_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30046 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-05 10:33:03.000000 zyte-common-items-0.6.0/zyte_common_items/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:33:14.447446 zyte-common-items-0.6.0/zyte_common_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 10:33:14.000000 zyte-common-items-0.6.0/zyte_common_items.egg-info/top_level.txt
```

### Comparing `zyte-common-items-0.5.0/LICENSE` & `zyte-common-items-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.5.0/PKG-INFO` & `zyte-common-items-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.5.0
+Version: 0.6.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =================
 zyte-common-items
 =================
 
@@ -38,15 +38,15 @@
 
 .. image:: https://codecov.io/github/zytedata/zyte-common-items/coverage.svg?branch=master
    :target: https://codecov.io/gh/zytedata/zyte-common-items
    :alt: Coverage report
 
 .. description starts
 
-``zyte-common-items`` is a Python 3.7+ library of item_ and `page object`_
+``zyte-common-items`` is a Python 3.8+ library of item_ and `page object`_
 classes for web data extraction that we use at Zyte_ to maximize opportunities
 for code reuse.
 
 .. _item: https://docs.scrapy.org/en/latest/topics/items.html
 .. _page object: https://web-poet.readthedocs.io/en/stable/
 .. _Zyte: https://www.zyte.com/
```

### Comparing `zyte-common-items-0.5.0/README.rst` & `zyte-common-items-0.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 .. image:: https://codecov.io/github/zytedata/zyte-common-items/coverage.svg?branch=master
    :target: https://codecov.io/gh/zytedata/zyte-common-items
    :alt: Coverage report
 
 .. description starts
 
-``zyte-common-items`` is a Python 3.7+ library of item_ and `page object`_
+``zyte-common-items`` is a Python 3.8+ library of item_ and `page object`_
 classes for web data extraction that we use at Zyte_ to maximize opportunities
 for code reuse.
 
 .. _item: https://docs.scrapy.org/en/latest/topics/items.html
 .. _page object: https://web-poet.readthedocs.io/en/stable/
 .. _Zyte: https://www.zyte.com/
```

### Comparing `zyte-common-items-0.5.0/setup.py` & `zyte-common-items-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

### Comparing `zyte-common-items-0.5.0/zyte_common_items/adapter.py` & `zyte-common-items-0.6.0/zyte_common_items/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     It can be :ref:`configured <configuration>` into itemadapter_ to improve
     interaction with :ref:`items <items>` for itemadapter users like Scrapy_.
 
     In extends AttrsAdapter_ with the following features:
 
     -   Allows interaction and serialization of fields from
-        :attr:`~zyte_common_items.base.Item._unknown_fields_dict` as if they
+        :attr:`~zyte_common_items.Item._unknown_fields_dict` as if they
         were regular item fields.
 
     -   Removes keys with empty values from the output of
         `ItemAdapter.asdict()`_, for a cleaner output.
 
     .. _AttrsAdapter: https://github.com/scrapy/itemadapter#built-in-adapters
     .. _itemadapter: https://github.com/scrapy/itemadapter#itemadapter
```

### Comparing `zyte-common-items-0.5.0/zyte_common_items/base.py` & `zyte-common-items-0.6.0/zyte_common_items/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 """The ``Item`` class should be used as the parent class for data containers."""
 
 from collections import ChainMap
-
-try:
-    from typing import get_args
-except ImportError:
-    # Compliance with python 3.7
-    from .util import get_args
-
-try:
-    from typing import get_origin
-except ImportError:
-    # Compliance with python 3.7
-    from .util import get_origin
-
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, get_args, get_origin
 
 import attrs
 
 from .util import split_in_unknown_and_known_fields
 
 _Trail = Optional[str]
```

### Comparing `zyte-common-items-0.5.0/zyte_common_items/components.py` & `zyte-common-items-0.6.0/zyte_common_items/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,32 @@
 import attrs
 
 from zyte_common_items.base import Item
 from zyte_common_items.util import url_to_str
 
 
 @attrs.define
+class _Media(Item):
+    #: URL.
+    #:
+    #: When multiple URLs exist for a given media element, pointing to
+    #: different-quality versions, the highest-quality URL should be used.
+    #:
+    #: `Data URIs`_ are not allowed in this attribute.
+    #:
+    #: .. _Data URIs: https://en.wikipedia.org/wiki/Data_URI_scheme
+    url: str = attrs.field(converter=url_to_str)
+
+
+@attrs.define
 class AdditionalProperty(Item):
     """A name-value pair.
 
     See :attr:`Product.additionalProperties
-    <zyte_common_items.items.Product.additionalProperties>`.
+    <zyte_common_items.Product.additionalProperties>`.
     """
 
     #: Name.
     name: str
 
     #: Value.
     value: str
@@ -25,44 +38,75 @@
 @attrs.define(kw_only=True)
 class AggregateRating(Item):
     """Aggregate data about reviews and ratings.
 
     At least one of :attr:`ratingValue` or :attr:`reviewCount` is required.
 
     See :attr:`Product.aggregateRating
-    <zyte_common_items.items.Product.aggregateRating>`.
+    <zyte_common_items.Product.aggregateRating>`.
     """
 
     #: Maximum value of the rating system.
     bestRating: Optional[float] = None
 
     #: Average value of all ratings.
     ratingValue: Optional[float] = None
 
     #: Review count.
     reviewCount: Optional[int] = None
 
 
 @attrs.define
+class Audio(_Media):
+    """Audio.
+
+    See :class:`Article.audios <zyte_common_items.Article.audios>`.
+    """
+
+
+@attrs.define(kw_only=True)
+class Author(Item):
+    """Author of an article.
+
+    See :attr:`Article.authors <zyte_common_items.Article.authors>`.
+    """
+
+    #: Email.
+    email: Optional[str] = None
+
+    #: URL of the details page of the author.
+    url: Optional[str] = attrs.field(
+        default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
+    )
+
+    #: Full name.
+    name: Optional[str] = None
+
+    #: Text from which :attr:`~zyte_common_items.Author.name` was
+    #: extracted.
+    nameRaw: Optional[str] = None
+
+
+@attrs.define
 class Brand(Item):
     """Brand.
 
-    See :attr:`Product.brand <zyte_common_items.items.Product.brand`.
+    See :attr:`Product.brand <zyte_common_items.Product.brand>`.
     """
 
     #: Name as it appears on the source webpage (no post-processing).
     name: str
 
 
 @attrs.define(kw_only=True)
 class Breadcrumb(Item):
     """A breadcrumb from the `breadcrumb trail`_ of a webpage.
 
     See :attr:`Product.breadcrumbs
-    <zyte_common_items.items.Product.breadcrumbs>`.
+    <zyte_common_items.Product.breadcrumbs>`.
 
     .. _breadcrumb trail: https://en.wikipedia.org/wiki/Breadcrumb_navigation
     """
 
     #: Displayed name.
     name: Optional[str] = None
 
@@ -72,15 +116,15 @@
     )
 
 
 @attrs.define
 class Gtin(Item):
     """GTIN_ type-value pair.
 
-    See :class:`Product.gtin <zyte_common_items.items.Product.gtin>`.
+    See :class:`Product.gtin <zyte_common_items.Product.gtin>`.
 
     .. _GTIN: https://en.wikipedia.org/wiki/Global_Trade_Item_Number
     """
 
     #: Identifier of the GTIN format of ``value``.
     #:
     #: One of: ``"gtin13"``, ``"gtin8"``, ``"gtin14"``, ``"isbn10"``,
@@ -90,32 +134,22 @@
     #: Value.
     #:
     #: It should only contain digits.
     value: str
 
 
 @attrs.define
-class Image(Item):
+class Image(_Media):
     """Image.
 
-    See :class:`Product.images <zyte_common_items.items.Product.images>` and
-    :class:`Product.mainImage <zyte_common_items.items.Product.mainImage>`.
+    See for example
+    :class:`Product.images <zyte_common_items.Product.images>` and
+    :class:`Product.mainImage <zyte_common_items.Product.mainImage>`.
     """
 
-    #: URL.
-    #:
-    #: When multiple URLs exist for a given image, and those URLs point to
-    #: image files that are different-quality versions of that image, the URL
-    #: of the highest-quality image file should be used.
-    #:
-    #: `Data URIs`_ are not allowed in this attribute.
-    #:
-    #: .. _Data URIs: https://en.wikipedia.org/wiki/Data_URI_scheme
-    url: str = attrs.field(converter=url_to_str)
-
 
 @attrs.define(kw_only=True)
 class Link(Item):
     """A link from a webpage to another webpage."""
 
     #: Displayed text.
     text: Optional[str] = None
@@ -136,24 +170,28 @@
     #: Target URL.
     url: Optional[str] = attrs.field(
         default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
     )
 
 
 @attrs.define(kw_only=True)
-class Metadata(Item):
-    """Data extraction process metadata.
+class DateDownloadedMetadata(Item):
+    """Data extraction process metadata that only indicates the download date.
 
-    See :class:`Product.metadata <zyte_common_items.items.Product.metadata>`.
+    See
+    :class:`ArticleList.metadata <zyte_common_items.ArticleList.metadata>`.
     """
 
     #: Date and time when the product data was downloaded, in UTC timezone and
     #: the following format: ``YYYY-MM-DDThh:mm:ssZ``.
     dateDownloaded: Optional[str] = None
 
+
+@attrs.define(kw_only=True)
+class Metadata(DateDownloadedMetadata):
     #: The probability (0 for 0%, 1 for 100%) that the webpage features the
     #: requested data type.
     #:
     #: For example, if the extraction of a product from a given URL is
     #: requested, and that URL points to the webpage of a product with complete
     #: certainty, the value should be `1`. If with complete certainty the
     #: webpage features a job listing instead of a product, the value should be
@@ -162,15 +200,15 @@
     probability: Optional[float] = None
 
 
 @attrs.define(kw_only=True)
 class BusinessPlaceMetadata(Metadata):
     """Data extraction process metadata.
 
-    See :class:`BusinessPlace.metadata <zyte_common_items.items.BusinessPlace.metadata>`.
+    See :class:`BusinessPlace.metadata <zyte_common_items.BusinessPlace.metadata>`.
     """
 
     #: The search text the place was found with.
     searchText: Optional[str] = None
 
 
 @attrs.define(kw_only=True)
@@ -281,7 +319,15 @@
     unitCode: str
 
     #: Type of area, one of: LOT, FLOOR
     areaType: Optional[str] = None
 
     #: Area in the raw format, as it appears on the website.
     raw: str
+
+
+@attrs.define
+class Video(_Media):
+    """Video.
+
+    See :class:`Article.videos <zyte_common_items.Article.videos>`.
+    """
```

### Comparing `zyte-common-items-0.5.0/zyte_common_items/items.py` & `zyte-common-items-0.6.0/zyte_common_items/items.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,30 +4,241 @@
 
 from zyte_common_items.base import Item
 from zyte_common_items.components import (
     AdditionalProperty,
     Address,
     AggregateRating,
     Amenity,
+    Audio,
+    Author,
     Brand,
     Breadcrumb,
     BusinessPlaceMetadata,
+    DateDownloadedMetadata,
     Gtin,
     Image,
     Link,
     Metadata,
     NamedLink,
     OpeningHoursItem,
     ParentPlace,
     RealEstateArea,
     StarRating,
+    Video,
 )
 from zyte_common_items.util import url_to_str
 
 
+@attrs.define(slots=True, kw_only=True)
+class ArticleFromList(Item):
+    """Article from an article list from an article listing page.
+
+    See :class:`ArticleList`.
+    """
+
+    #: Clean text of the article, including sub-headings, with newline
+    #: separators.
+    #:
+    #: Format:
+    #:
+    #: - trimmed (no whitespace at the beginning or the end of the body
+    #:   string),
+    #: - line breaks included,
+    #: - no length limit,
+    #: - no normalization of Unicode characters.
+    articleBody: Optional[str] = None
+
+    #: All authors of the article.
+    authors: Optional[List[Author]] = None
+
+    #: Publication date of the article.
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ" or
+    #: "YYYY-MM-DDThh:mm:ss±zz:zz".
+    #:
+    #: With timezone, if available.
+    #:
+    #: If the actual publication date is not found, the date of the last
+    #: modification is used instead.
+    datePublished: Optional[str] = None
+
+    #: Same date as
+    #: :attr:`~zyte_common_items.ArticleFromList.datePublished`, but
+    #: :before parsing/normalization, i.e. as it appears on the website.
+    datePublishedRaw: Optional[str] = None
+
+    #: Headline or title.
+    headline: Optional[str] = None
+
+    #: Language of the article, as an ISO 639-1 language code.
+    #:
+    #: Sometimes the article language is not the same as the web page overall
+    #: language.
+    inLanguage: Optional[str] = None
+
+    #: Main image.
+    mainImage: Optional[Image] = None
+
+    #: All images.
+    images: Optional[List[Image]] = None
+
+    #: The probability (0 for 0%, 1 for 100%) that this record represents an
+    #: actual article.
+    probability: Optional[float] = None
+
+    #: Main URL.
+    url: Optional[str] = attrs.field(
+        default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
+    )
+
+
+@attrs.define(kw_only=True)
+class Article(Item):
+    #: Headline or title.
+    headline: Optional[str] = None
+
+    #: Publication date of the article.
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ" or
+    #: "YYYY-MM-DDThh:mm:ss±zz:zz".
+    #:
+    #: With timezone, if available.
+    #:
+    #: If the actual publication date is not found, the value of
+    #: :attr:`~zyte_common_items.Article.dateModified` is used instead.
+    datePublished: Optional[str] = None
+
+    #: Same date as
+    #: :attr:`~zyte_common_items.Article.datePublished`, but
+    #: :before parsing/normalization, i.e. as it appears on the website.
+    datePublishedRaw: Optional[str] = None
+
+    #: Date when the article was most recently modified.
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ" or
+    #: "YYYY-MM-DDThh:mm:ss±zz:zz".
+    #:
+    #: With timezone, if available.
+    dateModified: Optional[str] = None
+
+    #: Same date as
+    #: :attr:`~zyte_common_items.Article.dateModified`, but
+    #: :before parsing/normalization, i.e. as it appears on the website.
+    dateModifiedRaw: Optional[str] = None
+
+    #: All authors of the article.
+    authors: Optional[List[Author]] = None
+
+    #: Webpage `breadcrumb trail`_.
+    #:
+    #: .. _Breadcrumb trail: https://en.wikipedia.org/wiki/Breadcrumb_navigation
+    breadcrumbs: Optional[List[Breadcrumb]] = None
+
+    #: Language of the article, as an ISO 639-1 language code.
+    #:
+    #: Sometimes the article language is not the same as the web page overall
+    #: language.
+    inLanguage: Optional[str] = None
+
+    #: Main image.
+    mainImage: Optional[Image] = None
+
+    #: All images.
+    images: Optional[List[Image]] = None
+
+    #: A short summary of the article.
+    #:
+    #: It can be either human-provided (if available), or auto-generated.
+    description: Optional[str] = None
+
+    #: Clean text of the article, including sub-headings, with newline
+    #: separators.
+    #:
+    #: Format:
+    #:
+    #: - trimmed (no whitespace at the beginning or the end of the body
+    #:   string),
+    #: - line breaks included,
+    #: - no length limit,
+    #: - no normalization of Unicode characters.
+    articleBody: Optional[str] = None
+
+    #: Simplified and standardized HTML of the article, including sub-headings,
+    #: image captions and embedded content (videos, tweets, etc.).
+    #:
+    #: Format: HTML string normalized in a consistent way.
+    articleBodyHtml: Optional[str] = None
+
+    #: All videos.
+    videos: Optional[List[Video]] = None
+
+    #: All audios.
+    audios: Optional[List[Audio]] = None
+
+    #: Canonical form of the URL, as indicated by the website.
+    #:
+    #: See also ``url``.
+    canonicalUrl: Optional[str] = attrs.field(
+        default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
+    )
+
+    #: The main URL of the article page.
+    #:
+    #: The URL of the final response, after any redirects.
+    #:
+    #: Required attribute.
+    #:
+    #: In case there is no article data on the page or the page was not
+    #: reached, the returned "empty" item would still contain this URL field.
+    url: str = attrs.field(converter=url_to_str)
+
+    #: Data extraction process metadata.
+    metadata: Optional[DateDownloadedMetadata] = None
+
+
+@attrs.define(slots=True, kw_only=True)
+class ArticleList(Item):
+    """Article list from an article listing page.
+
+    The :attr:`url` attribute is the only required attribute, all other fields
+    are optional.
+    """
+
+    #: The main URL of the article list.
+    #:
+    #: The URL of the final response, after any redirects.
+    #:
+    #: Required attribute.
+    #:
+    #: In case there is no article list data on the page or the page was not
+    #: reached, the returned item still contain this URL field and all the
+    #: other available datapoints.
+    url: str = attrs.field(converter=url_to_str)
+
+    #: Canonical form of the URL, as indicated by the website.
+    #:
+    #: See also ``url``.
+    canonicalUrl: Optional[str] = attrs.field(
+        default=None, converter=attrs.converters.optional(url_to_str), kw_only=True
+    )
+
+    #: List of article details found on the page.
+    #:
+    #: The order of the articles reflects their position on the page.
+    articles: Optional[List[ArticleFromList]] = None
+
+    #: Webpage `breadcrumb trail`_.
+    #:
+    #: .. _Breadcrumb trail: https://en.wikipedia.org/wiki/Breadcrumb_navigation
+    breadcrumbs: Optional[List[Breadcrumb]] = None
+
+    #: Data extraction process metadata.
+    metadata: Optional[DateDownloadedMetadata] = None
+
+
 @attrs.define(kw_only=True)
 class ProductVariant(Item):
     """:class:`Product` variant.
 
     See :attr:`Product.variants`.
     """
 
@@ -485,20 +696,17 @@
     #: For example, if the webpage is one of the pages of the Robots category,
     #: ``categoryName`` is ``'Robots'``.
     categoryName: Optional[str] = None
 
     #: Data extraction process metadata.
     metadata: Optional[Metadata] = None
 
-    #: Number of the current page.
-    #:
-    #: It should only be extracted if the webpage shows a page number.
+    #: Current page number, if displayed explicitly on the list page.
     #:
-    #: It must be 1-based. For example, if the first page of a listing is
-    #: numbered as 0 on the website, it should be extracted as `1` nonetheless.
+    #: Numeration starts with 1.
     pageNumber: Optional[int] = None
 
     #: Link to the next page.
     paginationNext: Optional[Link] = None
 
     #: List of products.
     #:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zyte-common-items-0.5.0/zyte_common_items/pages.py` & `zyte-common-items-0.6.0/zyte_common_items/pages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 
 import attrs
 from web_poet import ItemPage, RequestUrl, Returns, WebPage, field
 from web_poet.pages import ItemT
 
 from .components import Metadata
-from .items import BusinessPlace, Product, ProductList, RealEstate
+from .items import Article, ArticleList, BusinessPlace, Product, ProductList, RealEstate
 from .util import format_datetime
 
 
 def _date_downloaded_now():
     return format_datetime(datetime.utcnow())
 
 
@@ -38,44 +38,60 @@
     request_url: RequestUrl
 
     @field
     def url(self) -> str:
         return str(self.request_url)
 
 
-class BaseProductPage(BasePage, Returns[Product]):
+class BaseArticlePage(BasePage, Returns[Article]):
     pass
 
 
-class BaseProductListPage(BasePage, Returns[ProductList]):
+class BaseArticleListPage(BasePage, Returns[ArticleList]):
     pass
 
 
 class BaseBusinessPlacePage(BasePage, Returns[BusinessPlace]):
     pass
 
 
+class BaseProductPage(BasePage, Returns[Product]):
+    pass
+
+
+class BaseProductListPage(BasePage, Returns[ProductList]):
+    pass
+
+
 class BaseRealEstatePage(BasePage, Returns[RealEstate]):
     pass
 
 
 @attrs.define
 class Page(_BasePage, WebPage):
     @field
     def url(self) -> str:
         return str(self.response.url)
 
 
-class ProductPage(Page, Returns[Product]):
+class ArticlePage(Page, Returns[Article]):
     pass
 
 
-class ProductListPage(Page, Returns[ProductList]):
+class ArticleListPage(Page, Returns[ArticleList]):
     pass
 
 
 class BusinessPlacePage(Page, Returns[BusinessPlace]):
     pass
 
 
+class ProductPage(Page, Returns[Product]):
+    pass
+
+
+class ProductListPage(Page, Returns[ProductList]):
+    pass
+
+
 class RealEstatePage(Page, Returns[RealEstate]):
     pass
```

### Comparing `zyte-common-items-0.5.0/zyte_common_items/util.py` & `zyte-common-items-0.6.0/zyte_common_items/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,28 +41,14 @@
         if key_pred(k):
             yes[k] = v
         else:
             no[k] = v
     return (no, yes)
 
 
-def get_args(tp) -> Tuple:
-    """Offers backward compatibility for Python 3.7 since
-    typing.get_args(tp) is only available startingo on 3.8.
-    """
-    return getattr(tp, "__args__", ())
-
-
-def get_origin(tp) -> Tuple:
-    """Offers backward compatibility for Python 3.7 since
-    typing.get_origin(tp) is only available startingo on 3.8.
-    """
-    return getattr(tp, "__origin__", ())
-
-
 def url_to_str(url: Union[str, _Url]) -> str:
     if not isinstance(url, (str, _Url)):
         raise ValueError(
             f"{url!r} is neither a string nor an instance of RequestURL or ResponseURL."
         )
     return str(url)
```

### Comparing `zyte-common-items-0.5.0/zyte_common_items.egg-info/PKG-INFO` & `zyte-common-items-0.6.0/zyte_common_items.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.5.0
+Version: 0.6.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =================
 zyte-common-items
 =================
 
@@ -38,15 +38,15 @@
 
 .. image:: https://codecov.io/github/zytedata/zyte-common-items/coverage.svg?branch=master
    :target: https://codecov.io/gh/zytedata/zyte-common-items
    :alt: Coverage report
 
 .. description starts
 
-``zyte-common-items`` is a Python 3.7+ library of item_ and `page object`_
+``zyte-common-items`` is a Python 3.8+ library of item_ and `page object`_
 classes for web data extraction that we use at Zyte_ to maximize opportunities
 for code reuse.
 
 .. _item: https://docs.scrapy.org/en/latest/topics/items.html
 .. _page object: https://web-poet.readthedocs.io/en/stable/
 .. _Zyte: https://www.zyte.com/
```

