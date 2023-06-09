# Comparing `tmp/gregory_online-0.2.7.tar.gz` & `tmp/gregory_online-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.2.7.tar", last modified: Wed Jun  7 09:59:02 2023, max compression
+gzip compressed data, was "gregory_online-0.2.9.tar", last modified: Fri Jun  9 15:16:54 2023, max compression
```

## Comparing `gregory_online-0.2.7.tar` & `gregory_online-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,39 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-07 09:59:02.364765 gregory_online-0.2.7/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-07 09:58:51.000000 gregory_online-0.2.7/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    52156 2023-06-07 09:58:54.000000 gregory_online-0.2.7/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.7/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.7/gregory_online/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12513 2023-06-05 13:30:27.000000 gregory_online-0.2.7/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.7/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:39:44.000000 gregory_online-0.2.7/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-06 11:16:18.000000 gregory_online-0.2.7/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.7/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:29:49.000000 gregory_online-0.2.7/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.7/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.7/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.7/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3279 2023-06-06 11:50:54.000000 gregory_online-0.2.7/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-07 09:59:02.364765 gregory_online-0.2.7/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-07 09:59:02.000000 gregory_online-0.2.7/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-07 09:59:02.364765 gregory_online-0.2.7/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-01 12:16:03.000000 gregory_online-0.2.7/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-09 15:16:54.394400 gregory_online-0.2.9/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-09 15:16:51.000000 gregory_online-0.2.9/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.390401 gregory_online-0.2.9/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    54874 2023-06-09 15:15:39.000000 gregory_online-0.2.9/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.9/gregory_online/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/gregory_online/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Am241.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Cm247.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Np237.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Pa231.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Pu239.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Th232.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/U235.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/U238.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-09 11:53:23.000000 gregory_online-0.2.9/gregory_online/data/decay_lara.parquet
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2022-12-08 12:00:24.000000 gregory_online-0.2.9/gregory_online/data/testrebin.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3764 2023-06-09 14:40:20.000000 gregory_online-0.2.9/gregory_online/decay_db.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-09 14:56:20.000000 gregory_online-0.2.9/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.9/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:39:44.000000 gregory_online-0.2.9/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-06 11:16:18.000000 gregory_online-0.2.9/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.9/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:29:49.000000 gregory_online-0.2.9/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.9/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.9/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-09 14:10:12.000000 gregory_online-0.2.9/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      926 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       80 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-09 15:16:54.394400 gregory_online-0.2.9/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1217 2023-06-09 15:16:22.000000 gregory_online-0.2.9/setup.py
```

### Comparing `gregory_online-0.2.7/PKG-INFO` & `gregory_online-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gregory_online
-Version: 0.2.7
+Version: 0.2.9
 Summary: Online watching HTTP server of ROOT on port 9009
 Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gregory_online-0.2.7/README.md` & `gregory_online-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/bin/gregory_online` & `gregory_online-0.2.9/bin/gregory_online`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     histo_zoombins, histo_unzoom, histo_area, bin2ene, ene2bin, \
     get_calib_coefs, histo_fit, get_ene_range
 
 from  gregory_online.histo_io import save_hist_txt, select_histo_to_load, load_hist_txt
 
 
 from  gregory_online.histo_displ import display_h_name, display_np, refresh_canvases
+from  gregory_online.decay_db import decay_candidates
 
 
 import threading
 import time
 import datetime as dt
 
 
@@ -102,14 +103,16 @@
 
 
 deadt = 0 #  for influx
 deadtavg = [0,0] #  long term dt for histosave # NOT USED
 deadttot = 0
 # global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
 
+LOCAL_GLOB_NONE_CALIB = 1 # global normally
+INFLUX = True
 
 
 # def udpsend(message):
 #     """
 #     send to local seread running instance
 #     """
 #     UDP_IP = "127.0.0.1"
@@ -258,14 +261,16 @@
 
     # ---------------- container stuff
     global histograms, canvases, range_and_peaks
     global gregory_started
     global last_fit_res
     global ECALIB, ECALIBa, ECALIBb # calibrations
     global deadtavg, deadt, deadttot # avg not used; tot from h1np
+    global LOCAL_GLOB_NONE_CALIB
+    global INFLUX
     #
     # --------------    other stuff
     #global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt
     global h1np,h1np_diff,h1np_old,h1np_last_interval,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
 
     cmd = "" # no key command
 
@@ -384,15 +389,23 @@
             if d_last_interval/h1np_last_interval>0.01:
                 # print(f"{fg.cyan}i...                    delta in age={d_last_interval:.2f} s, demanded age={h1np_old_age} s{fg.default}")
                 warn_del = f"{fg.white}{bg.red}"
             else:
                 warn_del = f"{fg.default}{bg.default}"
             unwarn_del = f"{fg.default}{bg.blue}"
 
-            limits_calib = b0c01.get_limits_calib()
+            if LOCAL_GLOB_NONE_CALIB == 1:
+                limits_calib = b0c01.get_limits_calib()
+            if LOCAL_GLOB_NONE_CALIB == 2:
+                limits_calib = b0c01.get_limits_bins() # None calib
+            if LOCAL_GLOB_NONE_CALIB == 0:
+                binrange = b0c01.get_limits_bins()
+                limits_calib = 0*ECALIBa + ECALIBb,binrange[1]*ECALIBa + ECALIBb
+
+            #print( "D... calibration: ",limits_calib)
 
             rate= h1np_diff.sum()/deltat # does sum contain underflow? ->Integral() doesnot
             # I like to have underflow there...
             # deadtavg  is on the line 444
 
             # print(h1np_diff[0], h1np_diff[1]) # underflow and 1st bin #1
             #------------------------- ending the small calc
@@ -451,15 +464,14 @@
             deadttot = 0
             if  just_spesum !=0:
                 # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
                 deadttot = h1np[0]/just_spesum*100
             #deadtavg[0]+=deadt
             #deadtavg[1]+=1
 
-            INFLUX = True
             if INFLUX and len(h1np_diff)>2:
                 # # just_spesum = h1np_diff[1:-1].sum()
                 # just_spesum = h1np_diff.sum()
                 # # print("D... just_spesum==",just_spesum, h1np_diff, h1np)
                 # deadt = 0
                 # if  just_spesum !=0:
                 #     # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
@@ -698,21 +710,30 @@
                     res = histo_fit( histograms[thisname],  canvas = "fitresult")
                     if res is not None:
                         last_fit_res = res
                         for i in res.keys():
                             if i.find("E")>=0: print( f"          {i:10s} {res[i]:.4f} ")
                             if i.find("area")>=0: print( f"          {i:10s} {res[i]:.4f} ")
 
+                        # test to database - not here
+                        #if "E" in res:
+                        #    decay_candidates( res["E"] )
+
 
         elif cmd == "c":   # ***CMD***  CALIB =======
             print(f"i... c: {arg}       datalen= {len(ECALIB)} _______________________" )
             print("i...    c Ene     channel")
             print("i...    c Isotope channel")
             print("i...    c [Isotope|Ene]   f    ... for fit result as the bin")
             print("i...    c r  ....  reset calibration data")
+            print("i...    c l  ....  override calibration to LOCAL")
+            print("i...    c g  ....  override calibration to GLOBAL")
+            print("i...    c n  ....  override calibration to NONE")
+            print("i...    c f  ....   search database for last fit E")
+            print("i...    c f de ....  search database for last fit E with dE")
             for ik in ECALIBdb.keys():
                 print(f"i...         | {ik:7s} | {ECALIBdb[ik]:8.2f} |")
             print( "             _________________________________")
 
             if len(arg)>0:
                 eline = None # energy of the line
                 bline = None # bin of the line
@@ -721,43 +742,68 @@
                     print(f"X... {fg.red} give me {bg.white}'c  ene bin'{bg.default} OR 'c  reset' ==  'c r'{fg.default}")
                     # break
                 elif arg.split()[0]=="reset" or arg.split()[0]=="r" :  # ** reset **
                     ECALIB = []
                     ECALIBa = 1
                     ECALIBb = 0
                     print("i... {fg.yellow} RESET! e-calibration done{fg.default} ")
+                elif arg.split()[0]=="local" or arg.split()[0]=="l" :  # **
+                    LOCAL_GLOB_NONE_CALIB = 0
+                    print("i... {fg.yellow} LOCAL! e-calibration NOW{fg.default} ")
+                elif arg.split()[0]=="global" or arg.split()[0]=="g" :  # **
+                    LOCAL_GLOB_NONE_CALIB = 1
+                    print("i... {fg.yellow} GLOBAL! e-calibration NOW{fg.default} ")
+                elif arg.split()[0]=="none" or arg.split()[0]=="n" :  # **
+                    LOCAL_GLOB_NONE_CALIB = 2
+                    print("i... {fg.yellow} NONE! e-calibration NOW{fg.default} ")
+
                 # decompose the arguments....
                 else:
                     ok = True
                     eline, bline = None,None
                     if is_float(arg.split()[0]):   # ** energy was given **
                         eline = float(arg.split()[0])
                     elif arg.split()[0].upper() in ECALIBdb.keys(): #** 40K was given **
                         eline = ECALIBdb[arg.split()[0].upper()]
+
+                    elif arg.split()[0].upper() == "F":
+                        print("i... search in database:")
+                        if "channel" in last_fit_res:
+                            eline = last_fit_res["E"]
+                            deline = last_fit_res["dE"]
+                            deline = 3*deline # 3sigma
+                            print(f"i... LAST FITTED PEAK ENE = {eline:.2f} +- {deline:.2f}")
+                        if len(arg.split())>1 and  is_float(arg.split()[1]):
+                            deline = float(arg.split()[1])
+                            print(f"i... LAST FITTED PEAK ENE = {eline:.2f} +- {deline:.2f}")
+
+                        decay_candidates( eline, deline*3 )#deline*3 )
+                        ok = False
+
                     else: # ** something else happened**
-                        print("X... problem if not float nor in DB",arg.split() )
+                        print("X... problem if not float nor in LIST",arg.split() )
                         ok = False
                     #print(f"D... ... eline {eline}")
 
-                    print(arg.split(), arg.split()[1], is_float(arg.split()[1]))
+                    #print(arg.split(), arg.split()[1], is_float(arg.split()[1]))
                     # BIN to be decoded
                     if len(arg.split())>1 and is_float(arg.split()[1]):   # ** bin **
                         bline = float(arg.split()[1])
                         #print(f"D... bline={bline}")
                     # taking from fit....
                     elif len(arg.split())>1 and arg.split()[1]=="f":      # ** f=fitted bin **
                         if "channel" in last_fit_res:
                             bline = last_fit_res["channel"]
                             dbline = last_fit_res["dchannel"]
                             print("i... GETTING LAST FITTED PEAK for calibration bin", bline)
                         else:
                             ok = False
                             print("X... no fit result stored to get bin from there...")
                     else:
-                        print("X... problem")
+                        print("X... some problem, bin not given (nor 'f') ")
                         ok = False
                     if ok:
                         ECALIB.append( [ eline, bline, dbline ] ) # energy, channel, dchannel
                         print(ECALIB)
             ECALIBa, ECALIBb = ecalibration(ECALIB)
             print(f"i...  calculated energy calibration is {fg.green} E = {ECALIBa:.6f}*k + {ECALIBb:.3f} {fg.default}")
             print(f"i... {fg.blue} REMEMBER!: spectra energy calibration comes from detector (for now)...  {fg.default}")
@@ -1236,15 +1282,18 @@
         # prima = str(dt.datetime.now())[:-5]
         if OFFLINE:
             prima = f"{bg.green}{fg.white}{fx.bold}OFFLINE{fg.default}{bg.blue}"
         else:
             prima = f"{bg.green}{fg.white}{fx.bold}{spectrumname}{fg.default}{bg.blue}"
 
 
-        top.print_to( 0, f" {prima} {fg.white}{fx.bold} dt={deltat:.2f} sec. {fg.yellow} rate={rate:7.1f} {fg.white} RUN={rditime} MEM={lenhistos:4}  D[{h1np_last_interval:.0f}s]={warn_del} {d_last_interval:.2f} {unwarn_del} {fg.default}" )
+        if LOCAL_GLOB_NONE_CALIB==0:LOCAL_GLOB_NONE_CALIBname="loca"
+        if LOCAL_GLOB_NONE_CALIB==1:LOCAL_GLOB_NONE_CALIBname="glob"
+        if LOCAL_GLOB_NONE_CALIB==2:LOCAL_GLOB_NONE_CALIBname="none"
+        top.print_to( 0, f" {prima} {fg.white}{fx.bold} dt={deltat:.2f} sec. {fg.yellow} rate={rate:7.1f} {fg.white} RUN={rditime} MEM={lenhistos:4}  D[{h1np_last_interval:.0f}s]={warn_del} {d_last_interval:.2f} {unwarn_del} {fg.default} : INFL={INFLUX} : CAL:{LOCAL_GLOB_NONE_CALIBname}" )
 
         if len(key)==0:
             top2.print_to( 0, f"{fg.cyan}{bg.black}{' '*80}{bg.black}")
         else:
             top2.print_to( 0, f"{fg.white}{bg.red} > {fx.bold}{a_abc}{fg.yellow}_{fg.white}{b_abc}{fx.default}{fg.default}{bg.default} ")
         #top.place()
```

### Comparing `gregory_online-0.2.7/gregory_online/config.py` & `gregory_online-0.2.9/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/fetchnp.py` & `gregory_online-0.2.9/gregory_online/fetchnp.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,17 @@
     #i keep all the history histos here in this object
     def get_lenhistos(self):
         return len(self.histos)
 
     def get_limits_calib(self):
         return self.xmin,self.xmax
 
+    def get_limits_bins(self):
+        return 0,self.size
+
 
     def get_partial_time_histo(self, age):
         ele=None
         dist=999999
         #print(f"D... demanded age = {age}")
         for k in self.histos.keys():
             if ele is None: ele = k
@@ -199,14 +202,15 @@
 
         grp = re.search(r'rt=([\d\.]+)$',jhis["fTitle"])  # rt=3600 at the END of title ...
         # print(grp)
         if grp is not None and len(grp.groups())>0:
             self.realtime = float(grp.groups()[0].split("=")[-1])
             #print( f" realtime from title grp ={self.realtime}" )
 
+        # THIS STEERS CALIBRATION ..... limits_calib
         self.xmin = jhis['fXaxis']['fXmin']
         self.xmax = jhis['fXaxis']['fXmax']
 
         #print( jhis.keys() )
         helem = jhis['fArray']
 
         # print("D... helem in fetch: len,0,1 ...", len(helem) , helem[0], helem[-1] )
```

### Comparing `gregory_online-0.2.7/gregory_online/histo_analyze.py` & `gregory_online-0.2.9/gregory_online/histo_analyze.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/histo_displ.py` & `gregory_online-0.2.9/gregory_online/histo_displ.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/histo_global_cont.py` & `gregory_online-0.2.9/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/histo_io.py` & `gregory_online-0.2.9/gregory_online/histo_io.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/histo_np_ops.py` & `gregory_online-0.2.9/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/key_enter.py` & `gregory_online-0.2.9/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/topbar.py` & `gregory_online-0.2.9/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.7/gregory_online/utils.py` & `gregory_online-0.2.9/gregory_online/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def is_float(n):
     try:
         float_n = float(n)
         #print(n, float_n)
     except ValueError:
-        print(f"X... not float /{n}/")
+        print(f"X... not float /{n}/ ... false ret")
         return False
     else:
         #print("true block", n)
         if n is None:
             print("X... isfloat ... NONE")
             return False
```

### Comparing `gregory_online-0.2.7/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.2.9/gregory_online.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gregory-online
-Version: 0.2.7
+Version: 0.2.9
 Summary: Online watching HTTP server of ROOT on port 9009
 Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gregory_online-0.2.7/setup.py` & `gregory_online-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     license="GPL2",
     version=get_version("gregory_online/version.py"),
     packages=['gregory_online'],
     package_data={'gregory_online': ['data/*']},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/gregory_online'],
-    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers','sshkeyboard'],
+    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers','sshkeyboard','terminaltables'],
 )
```

