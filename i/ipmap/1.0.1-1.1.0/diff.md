# Comparing `tmp/ipmap-1.0.1.tar.gz` & `tmp/ipmap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipmap-1.0.1.tar", max compression
+gzip compressed data, was "ipmap-1.1.0.tar", max compression
```

## Comparing `ipmap-1.0.1.tar` & `ipmap-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1500 2023-06-07 01:28:04.587199 ipmap-1.0.1/LICENSE
--rw-r--r--   0        0        0     5752 2023-06-07 01:28:04.591199 ipmap-1.0.1/README.md
--rw-r--r--   0        0        0     1508 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/__init__.py
--rw-r--r--   0        0        0     4655 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/config.py
--rw-r--r--   0        0        0      735 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/data/settings.json
--rw-r--r--   0        0        0     2215 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/data/templates/map.html
--rw-r--r--   0        0        0     4364 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/ipmap.py
--rw-r--r--   0        0        0     1197 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/main.py
--rw-r--r--   0        0        0     1533 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/utils.py
--rw-r--r--   0        0        0      920 2023-06-07 01:28:04.591199 ipmap-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6702 1970-01-01 00:00:00.000000 ipmap-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-06-08 23:34:29.022267 ipmap-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5274 2023-06-08 23:34:29.026267 ipmap-1.1.0/README.md
+-rw-r--r--   0        0        0     1508 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/__init__.py
+-rw-r--r--   0        0        0     4441 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/config.py
+-rw-r--r--   0        0        0      735 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/data/settings.json
+-rw-r--r--   0        0        0     2215 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/data/templates/map.html
+-rw-r--r--   0        0        0     4699 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/ipmap.py
+-rw-r--r--   0        0        0     1036 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/main.py
+-rw-r--r--   0        0        0     2263 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/utils.py
+-rw-r--r--   0        0        0      904 2023-06-08 23:34:29.026267 ipmap-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6200 1970-01-01 00:00:00.000000 ipmap-1.1.0/PKG-INFO
```

### Comparing `ipmap-1.0.1/LICENSE` & `ipmap-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.1/ipmap/__init__.py` & `ipmap-1.1.0/ipmap/__init__.py`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.1/ipmap/config.py` & `ipmap-1.1.0/ipmap/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,15 @@
         self.patch = settings()["program"]["version"]["patch"]
         self.suffix = settings()["program"]["version"]["suffix"]
 
     def full_version(self) -> str:
         """
         Returns the full version string composed of the version components.
 
-        Returns:
-            str: The complete version string in the format "major.minor.patch.suffix".
+        :return: The complete version string in the format "major.minor.patch.suffix".
         """
         return f"{self.major}.{self.minor}.{self.patch}{self.suffix}"
 
 
 class Colours:
     def __init__(self):
         self.RED = self.get_colour("RED")
@@ -32,23 +31,23 @@
 
     @staticmethod
     def get_colour(colour_name: str) -> str:
         """
         Retrieves the value of the specified colour from the settings.
 
         :param: colour_name (str): The name of the colour to retrieve.
-
         :return: The value of the specified colour.
         """
         return settings()["colours"][colour_name]
 
 
 def settings() -> dict:
     """
     Loads the program's settings from /data/settings.json
+
     :return: Dictionary (JSON) containing program settings
     """
     # Get the absolute path of the current file
     current_dir = os.path.dirname(os.path.abspath(__file__))
 
     # Construct the path to the settings.json file
     settings_path = os.path.join(current_dir, "data", "settings.json")
@@ -59,14 +58,15 @@
 
     return data
 
 
 def format_map_name(defined_name) -> str:
     """
     Formats the output map name
+
     :param defined_name: User-defined name for the map
     :return: Formatted/Reconstructed name of the map
     """
     dt_now = datetime.now()
     if os.name == "nt":
         map_name = dt_now.strftime(f"{defined_name}_%d-%m-%Y %I-%M-%S%p")
     else:
@@ -74,14 +74,15 @@
 
     return map_name
 
 
 def create_ip_table(title: str, ip_data: list) -> Table:
     """
     Creates a table with the IP geolocation data.
+
     :param title: Table title
     :param ip_data: List of lists containing the geolocation data of IP Addresses
     :return: Table object containing the IP geolocation data
     """
     column_headers = [
         "IP",
         "Organization",
@@ -106,36 +107,35 @@
     return table
 
 
 def usage():
     return """
     Geolocate IP Address(es) (with an interactive map)
     --------------------------------------------------
-    ipmap map --ip <ip/file_containing_ip_addresses>
+    ipmap map --ip <ip>
 
     Open Google Earth on the given coordinates
     --------------------------------------------
-    ipmap earth --coordinates <latitude> <longitude>
+    ipmap earth --ip <ip>
 
     Lookup IP Address(es) (same as map but without an interactive map)
     ------------------------------------------------------------------
-    ipmap lookup --ip <ip/file_containing_ip_addresses>
+    ipmap lookup --ip <ip>
 
 
 modes:
     map - creates an interactive map and pin points the locations of the specified ip address(es) on it.
-    earth - opens google earth on the specified coordinates
+    earth - opens google earth on the location of the given ip address.
     lookup - looks up the specified ip address(es)' information.
     """
 
 
 def create_parser():
     parser = argparse.ArgumentParser(description=f"{settings()['program']['name']}" 
                                                  f" — by {settings()['program']['developer']['name']}" 
                                                  f" ({settings()['program']['developer']['about']})",
                                      epilog=settings()['program']['about'], usage=usage())
     parser.add_argument("mode", help="init mode", choices=["earth", "lookup", "map"])
-    parser.add_argument("-i", "--ip", help="an ip address or a file containing ip addresses")
-    parser.add_argument("-o", "--output", help="map output name", default="ipmap")
-    parser.add_argument("-c", "--coordinates", help="space separated latitude and longitude", nargs=2)
+    parser.add_argument("-i", "--ip", help="ip")
+    parser.add_argument("-o", "--output", help="map output name (default %(default)s)", default="ipmap")
     parser.add_argument("-v", "--version", action="version", version=Version().full_version())
     return parser
```

### Comparing `ipmap-1.0.1/ipmap/data/settings.json` & `ipmap-1.1.0/ipmap/data/settings.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99375%*

 * *Differences: {"'program'": "{'version': {'minor': '1', 'patch': '0'}}"}*

```diff
@@ -19,13 +19,13 @@
             "name": "Richard Mwewa",
             "twitter": "https://twitter.com/rly0nheart"
         },
         "license": "BDS-3 Clause",
         "name": "IPMap (IP Mapper)",
         "version": {
             "major": "1",
-            "minor": "0",
-            "patch": "1",
+            "minor": "1",
+            "patch": "0",
             "suffix": ""
         }
     }
 }
```

### Comparing `ipmap-1.0.1/ipmap/data/templates/map.html` & `ipmap-1.1.0/ipmap/data/templates/map.html`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.1/ipmap/ipmap.py` & `ipmap-1.1.0/ipmap/ipmap.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 colour = Colours()
 
 
 def get_ip_data(ip_address: str) -> list:
     """
     Gets the geolocation information of given IP Addresses.
+
     :param ip_address: IP Addresses to look up
     :return: A list of lists containing IP Addresses' data.
+
     The returned list is used in the leaflet map template to pinpoint the location(s)
     of IPs by using the coordinates.
     """
     # process input to get list of IPs
     ips = process_user_input(user_input=ip_address)
 
     # create an empty list to store ip data that will be used in the map
@@ -40,25 +42,26 @@
         ]
 
         # get the selected ip data from the response and append it to the ip_data_for_map list
         ip_data_for_map.append(ip_data)
 
     # create the IP geolocation data table
     # the table gets displayed on the terminal
-    table = create_ip_table(title=f"IP Geolocation Data: {ip_address}", ip_data=ip_data_for_map)
+    table = create_ip_table(title=f"\nIP Geolocation Data: {ip_address}", ip_data=ip_data_for_map)
     xprint(table)
 
     # return a list of lists containing ip data
     # this returned list will be used in the map template
     return ip_data_for_map
 
 
 def process_user_input(user_input: str) -> list:
     """
     Processes input from user to determine the type, and how to return the results
+
     :param user_input: IP; could be a single IP or a text file containing IP Addresses
     :return: A list of IP Addresses
     """
     if os.path.isfile(user_input):
         # if user_input is a file, read the contents of the file and return a list of IP addresses
         with open(user_input, 'r') as file:
             xprint(f"Loaded IP Addresses: '{file.name}'")
@@ -68,37 +71,46 @@
     else:
         return [user_input]
 
 
 def create_map(coordinates: list, output_file: str) -> str:
     """
     Uses the map template to create a new map with the geolocation data returned from the get_ip_data function
+
     :param coordinates: List of lists containing the geolocation data of each IP Address
     :param output_file: Output filename of the generated map
     :return: An interactive map in default browser (with pins pointing on the areas that correspond the IPs coordinates)
     """
+    # Construct path to the user's home directory
+    home_directory = os.path.expanduser("~")
+
     # Get the absolute path of the current file
-    current_dir = os.path.dirname(os.path.abspath(__file__))
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+
+    # Construct the path to the maps directory
+    maps_directory = os.path.join(home_directory, "maps")
+
     # Construct the path to the map template
-    html_path = os.path.join(current_dir, "data", "templates", "map.html")
+    html_path = os.path.join(current_directory, "data", "templates", "map.html")
     with open(html_path, "r") as html_file:
         html_content = html_file.read()
 
     updated_html_content = html_content.format(output_file, coordinates)
 
-    with open(f"{output_file}.html", "w") as created_map:
+    with open(os.path.join(maps_directory, f"{output_file}.html"), "w") as created_map:
         created_map.write(updated_html_content)
 
     return created_map.name
 
 
-def open_google_earth(coordinates: list) -> None:
+def open_google_earth(ip_data: list) -> None:
     """
     Opens Google Earth with the specified coordinates.
-    :param coordinates: A list of two item; latitude and longitude
+
+    :param ip_data: A list of lists from get_ip_data containing data of an ip
     :return: None
     """
     # Construct the URL with the coordinates
     google_earth_url = "https://earth.google.com/web/"
     """
     I honestly don't know what the below units are, 
     but I do know that 'data=KAI' makes the view tilt in a almost 360 view of the location.
@@ -107,14 +119,17 @@
     - 12094.0505788d
     - 1y
     - 1.97597436h
     - 60t
     - -0r
     - /data=KAI
     """
-    latitude, longitude = coordinates
-    google_earth_url += f"@{latitude},{longitude}," \
-                        f"89.06331136a,12094.0505788d,1y,1.97597436h,60t,-0r/data=KAI"
-
-    # Open the URL in the default web browser
-    xprint(f"{coordinates} Opening Google Earth...")
-    webbrowser.open(google_earth_url)
+
+    for data in ip_data:
+        latitude = data[9]
+        longitude = data[10]
+        google_earth_url += f"@{latitude},{longitude}," \
+                            f"89.06331136a,12094.0505788d,1y,1.97597436h,60t,-0r/data=KAI"
+
+        # Open the URL in the default web browser
+        xprint(f"({latitude}, {longitude}) Opening Google Earth...")
+        webbrowser.open(google_earth_url)
```

### Comparing `ipmap-1.0.1/ipmap/main.py` & `ipmap-1.1.0/ipmap/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 def run():
     clear_screen()
     xprint(f"Starting {settings()['program']['name']} v{Version().full_version()} at {time.asctime()}")
     path_finder(["maps"])
     check_updates()
     try:
         if args.mode == "earth":
-            open_google_earth(args.coordinates)
+            open_google_earth(get_ip_data(args.ip))
         elif args.mode == "lookup":
             get_ip_data(args.ip)
         elif args.mode == "map":
-            generated_map = create_map(get_ip_data(args.ip), os.path.join("maps", format_map_name(args.output)))
+            generated_map = create_map(get_ip_data(args.ip), format_map_name(args.output))
             xprint(f"Opening map: {generated_map}")
             webbrowser.open(generated_map)
     except KeyboardInterrupt:
         xprint(f"\nUser interruption detected ({colour.YELLOW}Ctrl+C{colour.RESET}).")
-    except FileNotFoundError as file_not_found_error:
-        xprint(f"File Not Found: {colour.YELLOW}{file_not_found_error}{colour.RESET}")
     except Exception as error:
-        xprint(f"Error: {colour.RESET}{error}{colour.RESET}")
+        xprint(f"Error: {colour.RED}{error}{colour.RESET}")
```

### Comparing `ipmap-1.0.1/pyproject.toml` & `ipmap-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 include = [
     {path = "ipmap/data/templates/map.html"},
     {path = "ipmap/data/settings.json"}
 ]
 name = "ipmap"
-version = "1.0.1"
+version = "1.1.0"
 description = "A cross-platform easy-to-use ip geolocation & mapping tool."
 authors = ["Richard Mwewa <rly0nheart@duck.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://github.com/rly0nheart/ipmap"
 repository = "https://github.com/rly0nheart/ipmap"
 keywords = ["mapping", "geolocation", "ip-address-geolocation", "ip-address-lookup", "ip-mapping"]
@@ -23,12 +23,10 @@
     "Operating System :: OS Independent",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "*"
-requests = "*"
-
 
 [tool.poetry.scripts]
 ipmap = "ipmap.main:run"
```

