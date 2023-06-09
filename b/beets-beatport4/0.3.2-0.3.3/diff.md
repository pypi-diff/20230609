# Comparing `tmp/beets-beatport4-0.3.2.tar.gz` & `tmp/beets-beatport4-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beets-beatport4-0.3.2.tar", last modified: Wed Jan 18 14:00:01 2023, max compression
+gzip compressed data, was "dist\beets-beatport4-0.3.3.tar", last modified: Fri Jun  9 07:12:33 2023, max compression
```

## Comparing `beets-beatport4-0.3.2.tar` & `beets-beatport4-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 samik     (1000) samik     (1000)        0 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/
-drwxrwxrwx   0 samik     (1000) samik     (1000)        0 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/beetsplug/
--rwxrwxrwx   0 samik     (1000) samik     (1000)    28509 2023-01-18 13:54:05.000000 beets-beatport4-0.3.2/beetsplug/beatport4.py
--rwxrwxrwx   0 samik     (1000) samik     (1000)       74 2023-01-13 00:47:16.000000 beets-beatport4-0.3.2/beetsplug/__init__.py
-drwxrwxrwx   0 samik     (1000) samik     (1000)        0 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/beets_beatport4.egg-info/
--rwxrwxrwx   0 samik     (1000) samik     (1000)        1 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/beets_beatport4.egg-info/dependency_links.txt
--rwxrwxrwx   0 samik     (1000) samik     (1000)     7945 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/beets_beatport4.egg-info/PKG-INFO
--rwxrwxrwx   0 samik     (1000) samik     (1000)       30 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/beets_beatport4.egg-info/requires.txt
--rwxrwxrwx   0 samik     (1000) samik     (1000)      278 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/beets_beatport4.egg-info/SOURCES.txt
--rwxrwxrwx   0 samik     (1000) samik     (1000)       10 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/beets_beatport4.egg-info/top_level.txt
--rwxrwxrwx   0 samik     (1000) samik     (1000)     1079 2023-01-13 00:46:33.000000 beets-beatport4-0.3.2/LICENSE
--rwxrwxrwx   0 samik     (1000) samik     (1000)       26 2022-12-14 12:06:23.000000 beets-beatport4-0.3.2/MANIFEST.in
--rwxrwxrwx   0 samik     (1000) samik     (1000)     7945 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/PKG-INFO
--rwxrwxrwx   0 samik     (1000) samik     (1000)     5824 2023-01-13 12:12:26.000000 beets-beatport4-0.3.2/README.rst
--rwxrwxrwx   0 samik     (1000) samik     (1000)       38 2023-01-18 14:00:01.000000 beets-beatport4-0.3.2/setup.cfg
--rwxrwxrwx   0 samik     (1000) samik     (1000)     1253 2023-01-18 13:59:36.000000 beets-beatport4-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:12:33.440652 beets-beatport4-0.3.3/
+-rw-rw-rw-   0        0        0     1079 2023-01-13 00:46:33.000000 beets-beatport4-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2022-12-14 12:06:23.000000 beets-beatport4-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8108 2023-06-09 07:12:33.439651 beets-beatport4-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5824 2023-01-13 12:12:26.000000 beets-beatport4-0.3.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 07:12:33.435677 beets-beatport4-0.3.3/beets_beatport4.egg-info/
+-rw-rw-rw-   0        0        0     8108 2023-06-09 07:12:33.000000 beets-beatport4-0.3.3/beets_beatport4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-09 07:12:33.000000 beets-beatport4-0.3.3/beets_beatport4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 07:12:33.000000 beets-beatport4-0.3.3/beets_beatport4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-09 07:12:33.000000 beets-beatport4-0.3.3/beets_beatport4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 07:12:33.000000 beets-beatport4-0.3.3/beets_beatport4.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 07:12:33.438653 beets-beatport4-0.3.3/beetsplug/
+-rw-rw-rw-   0        0        0       74 2023-01-13 00:47:16.000000 beets-beatport4-0.3.3/beetsplug/__init__.py
+-rw-rw-rw-   0        0        0    28775 2023-06-09 06:40:42.000000 beets-beatport4-0.3.3/beetsplug/beatport4.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 07:12:33.440652 beets-beatport4-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2023-06-09 06:40:42.000000 beets-beatport4-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `beets-beatport4-0.3.2/beetsplug/beatport4.py` & `beets-beatport4-0.3.3/beetsplug/beatport4.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
     def __init__(self, data):
         self.id = str(data['id'])
         self.name = str(data['name'])
         self.artists = []
         self.tracks = []
         self.type = None
         if 'artists' in data:
-            self.artists = [BeatportArtist(x) for x in data['artists']]
+            self.artists = [BeatportArtist(x) for x in data['artists'] if
+                            x is not None]
         if 'label' in data:
             self.label = BeatportLabel(data['label'])
         if 'catalog_number' in data:
             self.catalog_number = str(data['catalog_number'])
         if 'slug' in data:
             self.url = "https://beatport.com/release/{}/{}" \
                 .format(data['slug'], data['id'])
@@ -124,15 +125,16 @@
         return str(self)
 
 
 class BeatportTrack:
     def __init__(self, data):
         self.id = str(data['id'])
         self.name = str(data['name'])
-        self.artists = [BeatportArtist(x) for x in data['artists']]
+        self.artists = [BeatportArtist(x) for x in data['artists'] if
+                        x is not None]
         self.length = timedelta(milliseconds=data.get('length_ms', 0) or 0)
         self.number = None
         self.initial_key = None
         self.url = None
         self.bpm = None
         self.genre = None
         self.image_url = None
@@ -383,15 +385,15 @@
         try:
             response = self._get(f'/catalog/releases/{beatport_id}/tracks/',
                                  per_page=100)
         except BeatportAPIError as e:
             self._log.debug((str(e)))
             return []
         # we are not using BeatportTrack(t) because "number" field is missing
-        return [self.get_track(t['id']) for t in response]
+        return [self.get_track(t['id']) for t in response if t is not None]
 
     def get_track(self, beatport_id):
         """ Get information about a single track.
 
         :param beatport_id:     Beatport ID of the track
         :returns:               The matching track
         :rtype:                 :py:class:`BeatportTrack`
@@ -467,15 +469,15 @@
                                     params=kwargs,
                                     headers=headers)
         except Exception as e:
             raise BeatportAPIError(
                 "Error connecting to Beatport API: {}"
                 .format(e)
             )
-        if not response:
+        if not response or response.status_code >= 400:
             raise BeatportAPIError(
                 "Error {0.status_code} for '{0.request.path_url}"
                 .format(response)
             )
 
         json_response = response.json()
 
@@ -523,15 +525,15 @@
         """
         beatport_token = None
         # Get the OAuth token from a file
         try:
             with open(self._tokenfile()) as f:
                 beatport_token = BeatportOAuthToken(json.load(f))
 
-        except (OSError, AttributeError, JSONDecodeError):
+        except (OSError, AttributeError, JSONDecodeError, KeyError):
             # File does not exist, or has invalid format
             pass
 
         try:
             self.client = Beatport4Client(
                 log=self._log,
                 client_id=self.config['client_id'].get(),
@@ -701,19 +703,21 @@
         return albums
 
     def _get_album_info(self, release):
         """Returns an AlbumInfo object for a Beatport Release object.
         """
         va = len(release.artists) > 3
         artist, artist_id = self._get_artist(
-            ((artist.id, artist.name) for artist in release.artists)
+            ((artist.id, artist.name) for artist in release.artists if
+             artist is not None)
         )
         if va:
             artist = "Various Artists"
-        tracks = [self._get_track_info(x) for x in release.tracks]
+        tracks = [self._get_track_info(x) for x in release.tracks if
+                  x is not None]
 
         return AlbumInfo(album=release.name, album_id=release.id,
                          artist=artist, artist_id=artist_id, tracks=tracks,
                          albumtype=release.type, va=va,
                          year=release.publish_date.year,
                          month=release.publish_date.month,
                          day=release.publish_date.day,
@@ -725,15 +729,16 @@
     def _get_track_info(self, track):
         """Returns a TrackInfo object for a Beatport Track object.
         """
         title = track.name
         if track.mix_name != "Original Mix":
             title += f" ({track.mix_name})"
         artist, artist_id = self._get_artist(
-            ((artist.id, artist.name) for artist in track.artists)
+            ((artist.id, artist.name) for artist in track.artists if
+             artist is not None)
         )
         length = track.length.total_seconds()
         return TrackInfo(title=title, track_id=track.id,
                          artist=artist, artist_id=artist_id,
                          length=length, index=track.number,
                          medium_index=track.number,
                          data_source=self.data_source, data_url=track.url,
@@ -748,9 +753,9 @@
             artists=artists, id_key=0, name_key=1
         )
 
     def _get_tracks(self, query):
         """Returns a list of TrackInfo objects for a Beatport query.
         """
         bp_tracks = self.client.search(query, model='tracks')
-        tracks = [self._get_track_info(x) for x in bp_tracks]
+        tracks = [self._get_track_info(x) for x in bp_tracks if x is not None]
         return tracks
```

### Comparing `beets-beatport4-0.3.2/beets_beatport4.egg-info/PKG-INFO` & `beets-beatport4-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-Metadata-Version: 1.1
-Name: beets-beatport4
-Version: 0.3.2
-Summary: Plugin for beets (http://beets.io) to replace stock beatport plugin which is not yet compatible with Beatport API v4.
-Home-page: https://github.com/Samik081/beets-beatport4
-Author: Szymon "Samik" Tarasinski
-Author-email: st.samik@gmail.com
-License: MIT
-Download-URL: https://github.com/Samik081/beets-beatport4/releases/download/v0.3.2/beets-beatport4-0.3.2.tar.gz
-Description: **beets Beatport API v4 compatible plugin**
-        ==================================================
-        
-        .. image:: http://img.shields.io/pypi/v/beets-beatport4.svg
-            :target: https://pypi.python.org/pypi/beets-beatport4
-        
-        Plugin for `beets <https://github.com/beetbox/beets>`_ to replace stock beatport plugin and use Beatport API v4 as an
-        autotagger source.
-        
-        As Beatport had killed their API v3, the stock beatport plugin does not work anymore. It is also currently not possible to request the access to the API "normal" way (by using your client credentials or API token generated by Beatport), so I have found workaround that uses public API client id used for `Beatport docs frontend <https://api.beatport.com/v4/docs/>`_ and updated the code to use the new specification.
-        
-        For more info, see the discussion on this issue: https://github.com/beetbox/beets/issues/3862
-        
-        I have also opened a pull request in the official beets repository (https://github.com/beetbox/beets/pull/4477), so if it gets merged, I am probably going to take down this plugin.
-        
-        Installation
-        ------------
-        
-        Install this plugin with
-        
-        ..
-        
-           $ pip install beets-beatport4
-        
-        and add ``beatport4`` to the ``plugins`` list in your beets config file.
-        
-        Beatport Authorization
-        ----------------------
-        There are two ways of acquiring user access token to the Beatport v4 API using
-        this plugin.
-        
-        Method 1: username and password
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        This method is fully automatic and relies on holding your Beatport username
-        and password inside your beets config file.
-        It will authorize to the Beatport API using ``authorization_code`` grant type
-        and ``client_id`` provided by beatport for the sake of their ``swagger-ui``
-        frontend in which you can test their API: https://api.beatport.com/v4/docs/
-        By default, ``client_id`` is scrapped automatically from the above URL.
-        Alternatively, you can also pass it via plugin configuration.
-        
-        Steps:
-        
-        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
-        2. Add below configuration and fill your credentials
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-                art_overwrite: no
-                username: <YOUR_BEATPORT_USERNAME>
-                password: <YOUR_BEATPORT_PASSWORD>
-        
-        
-        Method 2. copy token from the browser
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        You will probably want to use this method if you don't want to store your
-        credentials unencrypted within the config file. Also, it will be helpful if
-        for any reason something goes wrong during the username/password authorization
-        process.
-        
-        This is also a fallback method if you provide wrong credentials in the config.
-        
-        Steps:
-        
-        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
-        2. When the first import with plugin enabled happens, you will be prompted to paste the access token JSON
-        3. Visit https://api.beatport.com/v4/docs/
-        4. Open Network tab in your browser and start capturing the traffic
-        5. Login with your Beatport account
-        6. Search for the following request: ``https://api.beatport.com/v4/auth/o/token/``
-        7. Copy the response (whole JSON structure)
-        8. Paste it to the terminal (or `beatport_token.json` file next to your ``beets/config.yaml`` - you can check the path by running ``beet config --paths`` command)
-        9. If the token expires, you will be prompted again and required to repeat above steps
-        
-        Fetching and embedding an art
-        -----------------------------
-        Additionally, this plugin has implemented separate art fetching and embedding.
-        Unlike
-        `fetchart plugin <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_,
-        it handles both singletons, but it will not work if you choose candidate source
-        other than Beatport.
-        Also, it does not require enabling
-        `fetchart <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_ or
-        `embedart <https://beets.readthedocs.io/en/stable/plugins/embedart.html>`_
-        plugins, as it uses
-        `beets.art module <https://github.com/beetbox/beets/blob/master/beets/art.py>`_
-        shipped with the core library.
-        
-        Under the hood, it uses image URL for the track's release,
-        exposed by the Beatport API.
-        
-        You can enable this feature via configuration (**it is disabled by default**):
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-        
-        By default, if a track already contains an art, it will not be overwritten.
-        Again, you can force such behaviour via configuration:
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-                art_overwrite: yes
-        
-        Image size
-        ^^^^^^^^^^
-        Original images from Beatport might have big resolution and size, but thanks to
-        Beatport's dynamic image URIs, it is possible to fetch image already resized by
-        Beatport backend, saving the bandwidth and resources on resizing images locally.
-        To specify the dynamic width and height, just pass it via configuration:
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-                art_width: 250 # don't specify or 0 to disable
-                art_height: 250 # don't specify or 0 to disable
-        
-        - if you specify just one dimension, the other will be set to the same value, so the aspect ratio is 1:1
-        - if you don't specify any dimension, original art will be downloaded
-        - if you specify both dimensions, they will be used in the dynamic URI, but they usually (always?) return images in 1:1 aspect ratio using lower dimension anyway
-        
-        
-        Plugin configuration
-        --------------------
-        .. code-block:: yaml
-        
-            beatport4:
-                art: no
-                art_overwrite: no
-                art_width: <WIDTH_PX>
-                art_height: <HEIGHT_PX>
-                username: <YOUR_BEATPORT_USERNAME>
-                password: <YOUR_BEATPORT_PASSWORD>
-                client_id: <BEATPORT_API_CLIENT_ID> # optional, you can set it, but it should be scrapped automatically from the docs
-        
-        Apart from the above, plugin should work exactly the same way as the stock one, so please refer to the `official documentation <https://beets.readthedocs.io/en/v1.6.0/plugins/beatport.html>`_
-Platform: ALL
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Metadata-Version: 1.1
+Name: beets-beatport4
+Version: 0.3.3
+Summary: Plugin for beets (http://beets.io) to replace stock beatport plugin which is not yet compatible with Beatport API v4.
+Home-page: https://github.com/Samik081/beets-beatport4
+Author: Szymon "Samik" Tarasinski
+Author-email: st.samik@gmail.com
+License: MIT
+Download-URL: https://github.com/Samik081/beets-beatport4/releases/download/v0.3.3/beets-beatport4-0.3.3.tar.gz
+Description: **beets Beatport API v4 compatible plugin**
+        ==================================================
+        
+        .. image:: http://img.shields.io/pypi/v/beets-beatport4.svg
+            :target: https://pypi.python.org/pypi/beets-beatport4
+        
+        Plugin for `beets <https://github.com/beetbox/beets>`_ to replace stock beatport plugin and use Beatport API v4 as an
+        autotagger source.
+        
+        As Beatport had killed their API v3, the stock beatport plugin does not work anymore. It is also currently not possible to request the access to the API "normal" way (by using your client credentials or API token generated by Beatport), so I have found workaround that uses public API client id used for `Beatport docs frontend <https://api.beatport.com/v4/docs/>`_ and updated the code to use the new specification.
+        
+        For more info, see the discussion on this issue: https://github.com/beetbox/beets/issues/3862
+        
+        I have also opened a pull request in the official beets repository (https://github.com/beetbox/beets/pull/4477), so if it gets merged, I am probably going to take down this plugin.
+        
+        Installation
+        ------------
+        
+        Install this plugin with
+        
+        ..
+        
+           $ pip install beets-beatport4
+        
+        and add ``beatport4`` to the ``plugins`` list in your beets config file.
+        
+        Beatport Authorization
+        ----------------------
+        There are two ways of acquiring user access token to the Beatport v4 API using
+        this plugin.
+        
+        Method 1: username and password
+        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        This method is fully automatic and relies on holding your Beatport username
+        and password inside your beets config file.
+        It will authorize to the Beatport API using ``authorization_code`` grant type
+        and ``client_id`` provided by beatport for the sake of their ``swagger-ui``
+        frontend in which you can test their API: https://api.beatport.com/v4/docs/
+        By default, ``client_id`` is scrapped automatically from the above URL.
+        Alternatively, you can also pass it via plugin configuration.
+        
+        Steps:
+        
+        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
+        2. Add below configuration and fill your credentials
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+                art_overwrite: no
+                username: <YOUR_BEATPORT_USERNAME>
+                password: <YOUR_BEATPORT_PASSWORD>
+        
+        
+        Method 2. copy token from the browser
+        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        You will probably want to use this method if you don't want to store your
+        credentials unencrypted within the config file. Also, it will be helpful if
+        for any reason something goes wrong during the username/password authorization
+        process.
+        
+        This is also a fallback method if you provide wrong credentials in the config.
+        
+        Steps:
+        
+        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
+        2. When the first import with plugin enabled happens, you will be prompted to paste the access token JSON
+        3. Visit https://api.beatport.com/v4/docs/
+        4. Open Network tab in your browser and start capturing the traffic
+        5. Login with your Beatport account
+        6. Search for the following request: ``https://api.beatport.com/v4/auth/o/token/``
+        7. Copy the response (whole JSON structure)
+        8. Paste it to the terminal (or `beatport_token.json` file next to your ``beets/config.yaml`` - you can check the path by running ``beet config --paths`` command)
+        9. If the token expires, you will be prompted again and required to repeat above steps
+        
+        Fetching and embedding an art
+        -----------------------------
+        Additionally, this plugin has implemented separate art fetching and embedding.
+        Unlike
+        `fetchart plugin <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_,
+        it handles both singletons, but it will not work if you choose candidate source
+        other than Beatport.
+        Also, it does not require enabling
+        `fetchart <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_ or
+        `embedart <https://beets.readthedocs.io/en/stable/plugins/embedart.html>`_
+        plugins, as it uses
+        `beets.art module <https://github.com/beetbox/beets/blob/master/beets/art.py>`_
+        shipped with the core library.
+        
+        Under the hood, it uses image URL for the track's release,
+        exposed by the Beatport API.
+        
+        You can enable this feature via configuration (**it is disabled by default**):
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+        
+        By default, if a track already contains an art, it will not be overwritten.
+        Again, you can force such behaviour via configuration:
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+                art_overwrite: yes
+        
+        Image size
+        ^^^^^^^^^^
+        Original images from Beatport might have big resolution and size, but thanks to
+        Beatport's dynamic image URIs, it is possible to fetch image already resized by
+        Beatport backend, saving the bandwidth and resources on resizing images locally.
+        To specify the dynamic width and height, just pass it via configuration:
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+                art_width: 250 # don't specify or 0 to disable
+                art_height: 250 # don't specify or 0 to disable
+        
+        - if you specify just one dimension, the other will be set to the same value, so the aspect ratio is 1:1
+        - if you don't specify any dimension, original art will be downloaded
+        - if you specify both dimensions, they will be used in the dynamic URI, but they usually (always?) return images in 1:1 aspect ratio using lower dimension anyway
+        
+        
+        Plugin configuration
+        --------------------
+        .. code-block:: yaml
+        
+            beatport4:
+                art: no
+                art_overwrite: no
+                art_width: <WIDTH_PX>
+                art_height: <HEIGHT_PX>
+                username: <YOUR_BEATPORT_USERNAME>
+                password: <YOUR_BEATPORT_PASSWORD>
+                client_id: <BEATPORT_API_CLIENT_ID> # optional, you can set it, but it should be scrapped automatically from the docs
+        
+        Apart from the above, plugin should work exactly the same way as the stock one, so please refer to the `official documentation <https://beets.readthedocs.io/en/v1.6.0/plugins/beatport.html>`_
+Platform: ALL
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `beets-beatport4-0.3.2/LICENSE` & `beets-beatport4-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beets-beatport4-0.3.2/PKG-INFO` & `beets-beatport4-0.3.3/beets_beatport4.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-Metadata-Version: 1.1
-Name: beets-beatport4
-Version: 0.3.2
-Summary: Plugin for beets (http://beets.io) to replace stock beatport plugin which is not yet compatible with Beatport API v4.
-Home-page: https://github.com/Samik081/beets-beatport4
-Author: Szymon "Samik" Tarasinski
-Author-email: st.samik@gmail.com
-License: MIT
-Download-URL: https://github.com/Samik081/beets-beatport4/releases/download/v0.3.2/beets-beatport4-0.3.2.tar.gz
-Description: **beets Beatport API v4 compatible plugin**
-        ==================================================
-        
-        .. image:: http://img.shields.io/pypi/v/beets-beatport4.svg
-            :target: https://pypi.python.org/pypi/beets-beatport4
-        
-        Plugin for `beets <https://github.com/beetbox/beets>`_ to replace stock beatport plugin and use Beatport API v4 as an
-        autotagger source.
-        
-        As Beatport had killed their API v3, the stock beatport plugin does not work anymore. It is also currently not possible to request the access to the API "normal" way (by using your client credentials or API token generated by Beatport), so I have found workaround that uses public API client id used for `Beatport docs frontend <https://api.beatport.com/v4/docs/>`_ and updated the code to use the new specification.
-        
-        For more info, see the discussion on this issue: https://github.com/beetbox/beets/issues/3862
-        
-        I have also opened a pull request in the official beets repository (https://github.com/beetbox/beets/pull/4477), so if it gets merged, I am probably going to take down this plugin.
-        
-        Installation
-        ------------
-        
-        Install this plugin with
-        
-        ..
-        
-           $ pip install beets-beatport4
-        
-        and add ``beatport4`` to the ``plugins`` list in your beets config file.
-        
-        Beatport Authorization
-        ----------------------
-        There are two ways of acquiring user access token to the Beatport v4 API using
-        this plugin.
-        
-        Method 1: username and password
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        This method is fully automatic and relies on holding your Beatport username
-        and password inside your beets config file.
-        It will authorize to the Beatport API using ``authorization_code`` grant type
-        and ``client_id`` provided by beatport for the sake of their ``swagger-ui``
-        frontend in which you can test their API: https://api.beatport.com/v4/docs/
-        By default, ``client_id`` is scrapped automatically from the above URL.
-        Alternatively, you can also pass it via plugin configuration.
-        
-        Steps:
-        
-        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
-        2. Add below configuration and fill your credentials
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-                art_overwrite: no
-                username: <YOUR_BEATPORT_USERNAME>
-                password: <YOUR_BEATPORT_PASSWORD>
-        
-        
-        Method 2. copy token from the browser
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        You will probably want to use this method if you don't want to store your
-        credentials unencrypted within the config file. Also, it will be helpful if
-        for any reason something goes wrong during the username/password authorization
-        process.
-        
-        This is also a fallback method if you provide wrong credentials in the config.
-        
-        Steps:
-        
-        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
-        2. When the first import with plugin enabled happens, you will be prompted to paste the access token JSON
-        3. Visit https://api.beatport.com/v4/docs/
-        4. Open Network tab in your browser and start capturing the traffic
-        5. Login with your Beatport account
-        6. Search for the following request: ``https://api.beatport.com/v4/auth/o/token/``
-        7. Copy the response (whole JSON structure)
-        8. Paste it to the terminal (or `beatport_token.json` file next to your ``beets/config.yaml`` - you can check the path by running ``beet config --paths`` command)
-        9. If the token expires, you will be prompted again and required to repeat above steps
-        
-        Fetching and embedding an art
-        -----------------------------
-        Additionally, this plugin has implemented separate art fetching and embedding.
-        Unlike
-        `fetchart plugin <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_,
-        it handles both singletons, but it will not work if you choose candidate source
-        other than Beatport.
-        Also, it does not require enabling
-        `fetchart <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_ or
-        `embedart <https://beets.readthedocs.io/en/stable/plugins/embedart.html>`_
-        plugins, as it uses
-        `beets.art module <https://github.com/beetbox/beets/blob/master/beets/art.py>`_
-        shipped with the core library.
-        
-        Under the hood, it uses image URL for the track's release,
-        exposed by the Beatport API.
-        
-        You can enable this feature via configuration (**it is disabled by default**):
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-        
-        By default, if a track already contains an art, it will not be overwritten.
-        Again, you can force such behaviour via configuration:
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-                art_overwrite: yes
-        
-        Image size
-        ^^^^^^^^^^
-        Original images from Beatport might have big resolution and size, but thanks to
-        Beatport's dynamic image URIs, it is possible to fetch image already resized by
-        Beatport backend, saving the bandwidth and resources on resizing images locally.
-        To specify the dynamic width and height, just pass it via configuration:
-        
-        .. code-block:: yaml
-        
-            beatport4:
-                art: yes
-                art_width: 250 # don't specify or 0 to disable
-                art_height: 250 # don't specify or 0 to disable
-        
-        - if you specify just one dimension, the other will be set to the same value, so the aspect ratio is 1:1
-        - if you don't specify any dimension, original art will be downloaded
-        - if you specify both dimensions, they will be used in the dynamic URI, but they usually (always?) return images in 1:1 aspect ratio using lower dimension anyway
-        
-        
-        Plugin configuration
-        --------------------
-        .. code-block:: yaml
-        
-            beatport4:
-                art: no
-                art_overwrite: no
-                art_width: <WIDTH_PX>
-                art_height: <HEIGHT_PX>
-                username: <YOUR_BEATPORT_USERNAME>
-                password: <YOUR_BEATPORT_PASSWORD>
-                client_id: <BEATPORT_API_CLIENT_ID> # optional, you can set it, but it should be scrapped automatically from the docs
-        
-        Apart from the above, plugin should work exactly the same way as the stock one, so please refer to the `official documentation <https://beets.readthedocs.io/en/v1.6.0/plugins/beatport.html>`_
-Platform: ALL
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Metadata-Version: 1.1
+Name: beets-beatport4
+Version: 0.3.3
+Summary: Plugin for beets (http://beets.io) to replace stock beatport plugin which is not yet compatible with Beatport API v4.
+Home-page: https://github.com/Samik081/beets-beatport4
+Author: Szymon "Samik" Tarasinski
+Author-email: st.samik@gmail.com
+License: MIT
+Download-URL: https://github.com/Samik081/beets-beatport4/releases/download/v0.3.3/beets-beatport4-0.3.3.tar.gz
+Description: **beets Beatport API v4 compatible plugin**
+        ==================================================
+        
+        .. image:: http://img.shields.io/pypi/v/beets-beatport4.svg
+            :target: https://pypi.python.org/pypi/beets-beatport4
+        
+        Plugin for `beets <https://github.com/beetbox/beets>`_ to replace stock beatport plugin and use Beatport API v4 as an
+        autotagger source.
+        
+        As Beatport had killed their API v3, the stock beatport plugin does not work anymore. It is also currently not possible to request the access to the API "normal" way (by using your client credentials or API token generated by Beatport), so I have found workaround that uses public API client id used for `Beatport docs frontend <https://api.beatport.com/v4/docs/>`_ and updated the code to use the new specification.
+        
+        For more info, see the discussion on this issue: https://github.com/beetbox/beets/issues/3862
+        
+        I have also opened a pull request in the official beets repository (https://github.com/beetbox/beets/pull/4477), so if it gets merged, I am probably going to take down this plugin.
+        
+        Installation
+        ------------
+        
+        Install this plugin with
+        
+        ..
+        
+           $ pip install beets-beatport4
+        
+        and add ``beatport4`` to the ``plugins`` list in your beets config file.
+        
+        Beatport Authorization
+        ----------------------
+        There are two ways of acquiring user access token to the Beatport v4 API using
+        this plugin.
+        
+        Method 1: username and password
+        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        This method is fully automatic and relies on holding your Beatport username
+        and password inside your beets config file.
+        It will authorize to the Beatport API using ``authorization_code`` grant type
+        and ``client_id`` provided by beatport for the sake of their ``swagger-ui``
+        frontend in which you can test their API: https://api.beatport.com/v4/docs/
+        By default, ``client_id`` is scrapped automatically from the above URL.
+        Alternatively, you can also pass it via plugin configuration.
+        
+        Steps:
+        
+        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
+        2. Add below configuration and fill your credentials
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+                art_overwrite: no
+                username: <YOUR_BEATPORT_USERNAME>
+                password: <YOUR_BEATPORT_PASSWORD>
+        
+        
+        Method 2. copy token from the browser
+        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        You will probably want to use this method if you don't want to store your
+        credentials unencrypted within the config file. Also, it will be helpful if
+        for any reason something goes wrong during the username/password authorization
+        process.
+        
+        This is also a fallback method if you provide wrong credentials in the config.
+        
+        Steps:
+        
+        1. Add ``beatport4`` plugin to your ``beets/config.yaml`` plugins list
+        2. When the first import with plugin enabled happens, you will be prompted to paste the access token JSON
+        3. Visit https://api.beatport.com/v4/docs/
+        4. Open Network tab in your browser and start capturing the traffic
+        5. Login with your Beatport account
+        6. Search for the following request: ``https://api.beatport.com/v4/auth/o/token/``
+        7. Copy the response (whole JSON structure)
+        8. Paste it to the terminal (or `beatport_token.json` file next to your ``beets/config.yaml`` - you can check the path by running ``beet config --paths`` command)
+        9. If the token expires, you will be prompted again and required to repeat above steps
+        
+        Fetching and embedding an art
+        -----------------------------
+        Additionally, this plugin has implemented separate art fetching and embedding.
+        Unlike
+        `fetchart plugin <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_,
+        it handles both singletons, but it will not work if you choose candidate source
+        other than Beatport.
+        Also, it does not require enabling
+        `fetchart <https://beets.readthedocs.io/en/stable/plugins/fetchart.html>`_ or
+        `embedart <https://beets.readthedocs.io/en/stable/plugins/embedart.html>`_
+        plugins, as it uses
+        `beets.art module <https://github.com/beetbox/beets/blob/master/beets/art.py>`_
+        shipped with the core library.
+        
+        Under the hood, it uses image URL for the track's release,
+        exposed by the Beatport API.
+        
+        You can enable this feature via configuration (**it is disabled by default**):
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+        
+        By default, if a track already contains an art, it will not be overwritten.
+        Again, you can force such behaviour via configuration:
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+                art_overwrite: yes
+        
+        Image size
+        ^^^^^^^^^^
+        Original images from Beatport might have big resolution and size, but thanks to
+        Beatport's dynamic image URIs, it is possible to fetch image already resized by
+        Beatport backend, saving the bandwidth and resources on resizing images locally.
+        To specify the dynamic width and height, just pass it via configuration:
+        
+        .. code-block:: yaml
+        
+            beatport4:
+                art: yes
+                art_width: 250 # don't specify or 0 to disable
+                art_height: 250 # don't specify or 0 to disable
+        
+        - if you specify just one dimension, the other will be set to the same value, so the aspect ratio is 1:1
+        - if you don't specify any dimension, original art will be downloaded
+        - if you specify both dimensions, they will be used in the dynamic URI, but they usually (always?) return images in 1:1 aspect ratio using lower dimension anyway
+        
+        
+        Plugin configuration
+        --------------------
+        .. code-block:: yaml
+        
+            beatport4:
+                art: no
+                art_overwrite: no
+                art_width: <WIDTH_PX>
+                art_height: <HEIGHT_PX>
+                username: <YOUR_BEATPORT_USERNAME>
+                password: <YOUR_BEATPORT_PASSWORD>
+                client_id: <BEATPORT_API_CLIENT_ID> # optional, you can set it, but it should be scrapped automatically from the docs
+        
+        Apart from the above, plugin should work exactly the same way as the stock one, so please refer to the `official documentation <https://beets.readthedocs.io/en/v1.6.0/plugins/beatport.html>`_
+Platform: ALL
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `beets-beatport4-0.3.2/README.rst` & `beets-beatport4-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `beets-beatport4-0.3.2/setup.py` & `beets-beatport4-0.3.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='beets-beatport4',
-    version='0.3.2',
+    version='0.3.3',
     description='Plugin for beets (http://beets.io) to replace stock beatport plugin which is not yet compatible '
                 'with Beatport API v4.',
     long_description=open('README.rst').read(),
     author='Szymon "Samik" Tarasinski',
     author_email='st.samik@gmail.com',
     url='https://github.com/Samik081/beets-beatport4',
-    download_url='https://github.com/Samik081/beets-beatport4/releases/download/v0.3.2/beets-beatport4-0.3.2.tar.gz',
+    download_url='https://github.com/Samik081/beets-beatport4/releases/download/v0.3.3/beets-beatport4-0.3.3.tar.gz',
     license='MIT',
     platforms='ALL',
 
     packages=['beetsplug'],
 
     install_requires=[
         'beets>=1.6.0',
```

