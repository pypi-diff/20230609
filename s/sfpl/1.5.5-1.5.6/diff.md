# Comparing `tmp/sfpl-1.5.5-py3-none-any.whl.zip` & `tmp/sfpl-1.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11427 bytes, number of entries: 8
+Zip file size: 11565 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      781 b- defN 23-Jun-06 22:54 sfpl/__init__.py
 -rw-r--r--  2.0 unx     2215 b- defN 23-Jun-06 22:54 sfpl/exceptions.py
--rw-r--r--  2.0 unx    30612 b- defN 23-Jun-07 03:39 sfpl/sfpl.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     4212 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/RECORD
-8 files, 39575 bytes uncompressed, 10411 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx    31284 b- defN 23-Jun-09 03:53 sfpl/sfpl.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-09 03:54 sfpl-1.5.6.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     4212 b- defN 23-Jun-09 03:54 sfpl-1.5.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 03:54 sfpl-1.5.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-09 03:54 sfpl-1.5.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-09 03:54 sfpl-1.5.6.dist-info/RECORD
+8 files, 40247 bytes uncompressed, 10549 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: sfpl/exceptions.py
 Comment: 
 
 Filename: sfpl/sfpl.py
 Comment: 
 
-Filename: sfpl-1.5.5.dist-info/LICENSE.md
+Filename: sfpl-1.5.6.dist-info/LICENSE.md
 Comment: 
 
-Filename: sfpl-1.5.5.dist-info/METADATA
+Filename: sfpl-1.5.6.dist-info/METADATA
 Comment: 
 
-Filename: sfpl-1.5.5.dist-info/WHEEL
+Filename: sfpl-1.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: sfpl-1.5.5.dist-info/top_level.txt
+Filename: sfpl-1.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: sfpl-1.5.5.dist-info/RECORD
+Filename: sfpl-1.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sfpl/sfpl.py

```diff
@@ -9,16 +9,16 @@
 
 from bs4 import BeautifulSoup
 from . import exceptions
 
 # Regex Patterns
 
 id_regex = 'https://sfpl.bibliocommons.com/.+/(\d+)'
-book_page_regex = '[\d,]+ to [\d,]+ of ([\d,]+) results'
-list_page_regex = '[\d,]+ - [\d,]+ of ([\d,]+) items'
+book_page_regex = '[\d,]+ to [\d,]+ of ([\d,]+) results?'
+list_page_regex = '[\d,]+ - [\d,]+ of ([\d,]+) items?'
 
 
 class User:
     """A library user account.
 
     Attributes:
         name (str): the account's username.
@@ -531,29 +531,44 @@
             pages(int): Number of pages to get.
 
         Yields:
             list: A list of books or lists on the page.
         """
         if self._type in ['keyword', 'title', 'author', 'subject', 'tag']:
             for x in range(1, pages + 1):
-                resp = requests.get('https://sfpl.bibliocommons.com/v2/search?pagination_page={}&query={}&searchType={}'.format(
-                    x, '+'.join(self.term.split()), self._type))
-
+                query = '+'.join(self.term.split())
+                url = f'https://sfpl.bibliocommons.com/v2/search?page={x}&query={query}&searchType={self._type}'
+                resp = requests.get(url)
                 soup = BeautifulSoup(resp.text, 'lxml')
+                pages_element = soup.find(string=re.compile(book_page_regex))
+
+                if not pages_element:
+                    raise StopIteration
 
-                if math.ceil(int(re.match(book_page_regex, soup.find(string=re.compile(book_page_regex))).group(1).replace(',', '')) / 10) < x:
+                pages = re.match(book_page_regex, pages_element).group(1).replace(',', '')
+
+                if math.ceil(int(pages) / 10) < x:
                     raise StopIteration
 
                 bib_data = json.loads(
                     soup.find(type='application/json').text)['entities']['bibs']
 
-                yield [Book({'title': bib_data[book]['briefInfo']['title'],
-                             'author': bib_data[book]['briefInfo']['authors'][0],
-                             'subtitle': bib_data[book]['briefInfo']['subtitle'],
-                             '_id': Book.metaDataIdToId(book)}) for book in bib_data]
+                books = []
+
+                for book in bib_data:
+                    authors = bib_data[book]['briefInfo']['authors']
+                    b = Book({
+                        'title': bib_data[book]['briefInfo']['title'],
+                        'author': authors[0] if authors else None,
+                        'subtitle': bib_data[book]['briefInfo']['subtitle'],
+                        '_id': Book.metaDataIdToId(book),
+                    })
+                    books.append(b)
+
+                yield books
 
         elif self._type == 'list':
             for x in range(1, pages + 1):
                 resp = requests.get(
                     'https://sfpl.bibliocommons.com/search?page={}&q={}&search_category=userlist&t=userlist'.format(x, self.term))
 
                 soup = BeautifulSoup(resp.text, 'lxml')
@@ -639,28 +654,43 @@
             >>> search = sfpl.AdvancedSearch(includeauthor='J. K. Rowling', excludekeyword='Harry Potter')
             >>> stream = search.getResults(pages=2)
             >>> next(stream)
             [Fantastic Beasts and Where to Find Them by Rowling, J. K., Fantastic Beasts and Where to Find Them : The Original Screenplay by Rowling, J. K., The Casual Vacancy by Rowling, J. K., Very Good Lives by Rowling, J. K., Animales fantásticos y dónde encontrarlos by Rowling, J. K.]
         """
         for x in range(1, pages + 1):
             resp = requests.get(
-                "https://sfpl.bibliocommons.com/v2/search?pagination_page={}&query={}&searchType=bl".format(x, self.query))
+                "https://sfpl.bibliocommons.com/v2/search?page={}&query={}&searchType=bl".format(x, self.query))
 
             soup = BeautifulSoup(resp.text, 'lxml')
+            pages_element = soup.find(string=re.compile(book_page_regex))
 
-            if math.ceil(int(re.match(book_page_regex, soup.find(string=re.compile(book_page_regex))).group(1).replace(',', '')) / 10) < x:
+            if not pages_element:
+                raise StopIteration
+
+            pages = re.match(book_page_regex, pages_element).group(1).replace(',', '')
+
+            if math.ceil(int(pages) / 10) < x:
                 raise StopIteration
 
             bib_data = json.loads(
                     soup.find(type='application/json').text)['entities']['bibs']
 
-            yield [Book({'title': bib_data[book]['briefInfo']['title'],
-                         'author': bib_data[book]['briefInfo']['authors'][0],
-                         'subtitle': bib_data[book]['briefInfo']['subtitle'],
-                         '_id': Book.metaDataIdToId(book)}) for book in bib_data]
+            books = []
+
+            for book in bib_data:
+                authors = bib_data[book]['briefInfo']['authors']
+                b = Book({
+                    'title': bib_data[book]['briefInfo']['title'],
+                    'author': authors[0] if authors else None,
+                    'subtitle': bib_data[book]['briefInfo']['subtitle'],
+                    '_id': Book.metaDataIdToId(book),
+                })
+                books.append(b)
+
+            yield books
 
     def __str__(self):
         return self.query
 
     def __repr__(self):
         return self.query
```

## Comparing `sfpl-1.5.5.dist-info/LICENSE.md` & `sfpl-1.5.6.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `sfpl-1.5.5.dist-info/METADATA` & `sfpl-1.5.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfpl
-Version: 1.5.5
+Version: 1.5.6
 Summary: Unofficial Python API for SFPL
 Home-page: https://github.com/kajchang/sfpl-scraper
 Author: Kai Chang
 Author-email: kaijchang@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

## Comparing `sfpl-1.5.5.dist-info/RECORD` & `sfpl-1.5.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 sfpl/__init__.py,sha256=cNLOiHrCoKKGzi_48XTPv5BYuWxDXv1yMSICpxiy_I0,781
 sfpl/exceptions.py,sha256=7bB-fFq0csIX8o2NDcqbDWyVDxNe8Nrl_CsVfCkEdWI,2215
-sfpl/sfpl.py,sha256=3y7IbvJqj_nmoLRbwJdl4lg2Rp1Daf_ikYkw4_9bBls,30612
-sfpl-1.5.5.dist-info/LICENSE.md,sha256=HYCE756ol-xGLObA5Tj5eWeJRpmqxlyTOAQGJxTTMwo,1068
-sfpl-1.5.5.dist-info/METADATA,sha256=mq5fb4g38qxX3OTTfdLE7zJw7v8ECuFijWqOGVbU30Q,4212
-sfpl-1.5.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sfpl-1.5.5.dist-info/top_level.txt,sha256=kp0tw-a9exZiW9jwktkLGfoLuuKzrbJlr_7WSZlvU10,5
-sfpl-1.5.5.dist-info/RECORD,,
+sfpl/sfpl.py,sha256=d7WhiAOCJ2TZkyHpvTzTi_ftgydutcYMtxciAhkXRak,31284
+sfpl-1.5.6.dist-info/LICENSE.md,sha256=HYCE756ol-xGLObA5Tj5eWeJRpmqxlyTOAQGJxTTMwo,1068
+sfpl-1.5.6.dist-info/METADATA,sha256=bP7Sb2ddvVtHgTqW5UaL1y0GowzKcr22MqAqp_WayQs,4212
+sfpl-1.5.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sfpl-1.5.6.dist-info/top_level.txt,sha256=kp0tw-a9exZiW9jwktkLGfoLuuKzrbJlr_7WSZlvU10,5
+sfpl-1.5.6.dist-info/RECORD,,
```

