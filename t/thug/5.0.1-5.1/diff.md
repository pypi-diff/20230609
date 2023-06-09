# Comparing `tmp/thug-5.0.1.tar.gz` & `tmp/thug-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thug-5.0.1.tar", last modified: Wed May 24 07:31:49 2023, max compression
+gzip compressed data, was "thug-5.1.tar", last modified: Fri Jun  9 06:55:31 2023, max compression
```

## Comparing `thug-5.0.1.tar` & `thug-5.1.tar`

### file list

```diff
@@ -1,524 +1,518 @@
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.272548 thug-5.0.1/
--rw-r--r--   0 buffer    (1000) buffer    (1000)    17987 2022-11-28 09:02:06.000000 thug-5.0.1/LICENSE.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      130 2023-01-12 15:47:27.000000 thug-5.0.1/MANIFEST.in
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3950 2023-05-24 07:31:49.271548 thug-5.0.1/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2676 2023-01-12 15:47:27.000000 thug-5.0.1/README.rst
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3485 2023-05-24 07:31:15.000000 thug-5.0.1/pyproject.toml
--rw-r--r--   0 buffer    (1000) buffer    (1000)      339 2023-05-24 07:31:15.000000 thug-5.0.1/requirements.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       38 2023-05-24 07:31:49.272548 thug-5.0.1/setup.cfg
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1346 2023-01-12 15:47:27.000000 thug-5.0.1/setup.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.047541 thug-5.0.1/thug/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.050541 thug-5.0.1/thug/ActiveX/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     7598 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/ActiveX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    64018 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/CLSID.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.104543 thug-5.0.1/thug/ActiveX/modules/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      400 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/AOLAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1119 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/AcroPDF.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      610 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/AdodbRecordset.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2573 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/AdodbStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1482 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/AnswerWorks.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1086 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/AolAmpX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      979 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/AolICQ.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      801 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/BaiduBar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      567 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/BitDefender.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      421 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/CABrightStor.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      600 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/CGAgent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      726 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Comodo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      720 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ConnectAndEnterRoom.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      307 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/CreativeSoftAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      445 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/DLinkMPEG.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      673 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/DPClient.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      447 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/DVRHOSTWeb.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      625 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/DirectShow.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      404 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/DivX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1857 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Domino.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1500 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/EnjoySAP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      825 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/FacebookPhotoUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3049 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/File.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      478 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/FileUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2221 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Folder.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      496 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/GLIEDown2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      656 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/GatewayWeblaunch.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      420 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Gogago.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      561 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/GomWeb.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4119 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/HPInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      443 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ICQToolbar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      945 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/IMWebControl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      672 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/InternetCleverSuite.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1964 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/JavaDeploymentToolkit.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1197 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      405 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Kingsoft.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/MSRICHTXT.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      601 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/MSVFP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      535 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/MSXML2DOMDocument.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4390 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/MacrovisionFlexNet.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/MicrosoftWorks7Attack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2048 2023-01-19 12:08:02.000000 thug-5.0.1/thug/ActiveX/modules/MicrosoftXMLDOM.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8006 2023-01-12 15:47:27.000000 thug-5.0.1/thug/ActiveX/modules/MicrosoftXMLHTTP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      466 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Move.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      438 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/MyspaceUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      589 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/NCTAudioFile2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1259 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/NamoInstaller.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      616 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/NeoTracePro.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3311 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/NessusScanCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1175 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/OfficeOCX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1057 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/OurgameGLWorld.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1201 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/PPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      498 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/PTZCamPanel.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      494 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/QuantumStreaming.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      484 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/QvodCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      973 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/RDSDataSpace.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2335 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/RealPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      348 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/RediffBolDownloaderAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      831 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/RegistryPro.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      361 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/RisingScanner.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      449 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/RtspVaPgCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1116 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/SSReaderPdg2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1027 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ScriptingDictionary.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ScriptingEncoder.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5185 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ScriptingFileSystemObject.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1527 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ShellApplication.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      361 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Shockwave.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      394 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ShockwaveFlash10.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      394 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ShockwaveFlash11.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      394 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ShockwaveFlash12.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      394 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ShockwaveFlash9.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      273 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/SilverLight.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      921 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/SinaDLoader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1472 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/SnapshotViewer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      715 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      906 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Spreadsheet.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      677 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/StormConfig.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2436 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/StormMps.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      516 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/StreamAudioChainCast.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1061 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/SymantecAppStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2224 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/SymantecBackupExec.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4772 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/TextStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      787 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/Toshiba.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      391 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/UUSeeUpdate.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      691 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/UniversalUpload.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1763 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/VLC.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      719 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/VisualStudioDTE80.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      699 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/VsaIDEDTE.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      699 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/VsmIDEDTE.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      796 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WMEncProfileManager.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      132 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WMP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WScriptCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1280 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WScriptExec.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1689 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WScriptNetwork.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8980 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WScriptShell.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      213 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WScriptShortcut.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      645 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WebViewFolderIcon.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1373 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WinNTSystemInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      599 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WinZip.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      145 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/WindowsMediaPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      942 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/XMLDOMParseError.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1026 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/XUpload.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1159 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/YahooJukebox.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      688 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/YahooMessengerCyft.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1077 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/YahooMessengerYVerInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1244 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/YahooMessengerYwcvwr.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1932 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2870 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ActiveX/modules/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.105543 thug-5.0.1/thug/Analysis/
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.105543 thug-5.0.1/thug/Analysis/awis/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3224 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/awis/AWIS.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/awis/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.106543 thug-5.0.1/thug/Analysis/context/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1554 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/context/ContextAnalyzer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/context/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.107543 thug-5.0.1/thug/Analysis/honeyagent/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4000 2022-12-06 12:21:07.000000 thug-5.0.1/thug/Analysis/honeyagent/HoneyAgent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/honeyagent/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.108543 thug-5.0.1/thug/Analysis/screenshot/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1333 2023-03-20 08:16:52.000000 thug-5.0.1/thug/Analysis/screenshot/Screenshot.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/screenshot/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.108543 thug-5.0.1/thug/Analysis/shellcode/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8069 2023-01-19 12:08:02.000000 thug-5.0.1/thug/Analysis/shellcode/Shellcode.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Analysis/shellcode/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.113543 thug-5.0.1/thug/Classifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5017 2023-04-10 08:29:36.000000 thug-5.0.1/thug/Classifier/BaseClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2106 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/CookieClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2159 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/HTMLClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2070 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/ImageClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2008 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/JSClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2243 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/SampleClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2082 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/TextClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2330 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/URLClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2014 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/VBSClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Classifier/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.134544 thug-5.0.1/thug/DOM/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2534 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Alexa.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2289 2023-04-10 08:29:36.000000 thug-5.0.1/thug/DOM/AsyncPrefetcher.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2254 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/CCInterpreter.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Chrome.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1304 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/ClipboardData.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      817 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Components.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5901 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Console.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1112 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Crypto.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    54541 2023-03-20 08:16:52.000000 thug-5.0.1/thug/DOM/DFT.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3602 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/External.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2776 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/HTMLInspector.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9866 2023-03-20 08:16:52.000000 thug-5.0.1/thug/DOM/HTTPSession.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      932 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/HTTPSessionException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3593 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/History.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3506 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/JSClass.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     7824 2023-01-12 15:47:27.000000 thug-5.0.1/thug/DOM/JSEngine.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4502 2022-12-06 12:21:07.000000 thug-5.0.1/thug/DOM/JSInspector.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5959 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/JScriptEncode.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      752 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/LocalStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4661 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/Location.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19549 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/MIMEHandler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      762 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Map.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1197 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/MimeType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5282 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/MimeTypes.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/MozConnection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    13340 2023-03-20 08:16:52.000000 thug-5.0.1/thug/DOM/Navigator.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4056 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Personality.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1233 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Plugin.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1471 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Plugins.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1069 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/SchemeHandler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     6150 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Screen.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      756 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/SessionStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1750 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Sidebar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3502 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Storage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3216 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/UserProfile.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/Utils.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.137544 thug-5.0.1/thug/DOM/W3C/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.148544 thug-5.0.1/thug/DOM/W3C/Core/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2138 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/Attr.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      265 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/CDATASection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1241 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/CharacterData.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3531 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/ClassList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      564 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/Comment.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1910 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/DOMException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5765 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/DOMImplementation.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8868 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/Document.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2412 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/DocumentFragment.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1513 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/DocumentType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9544 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/Element.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      457 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/Entity.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      501 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/EntityReference.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1293 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/NamedNodeMap.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    14464 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/Node.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      569 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/NodeList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      474 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/NodeType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      485 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/Notation.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      510 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/ProcessingInstruction.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      803 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/Text.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1051 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Core/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      337 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Core/abstractmethod.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/DOMParser.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1454 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/DOMTokenList.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.155544 thug-5.0.1/thug/DOM/W3C/Events/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      868 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/DocumentEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4120 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/Event.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      525 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/EventException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      272 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/EventListener.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9134 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/EventTarget.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      484 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/HTMLEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1206 2023-01-12 15:47:27.000000 thug-5.0.1/thug/DOM/W3C/Events/MessageEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2198 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/MouseEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1575 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/MutationEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1105 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/StorageEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      636 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Events/UIEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      691 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/Events/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.157544 thug-5.0.1/thug/DOM/W3C/File/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2433 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/File/Blob.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1381 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/File/File.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       85 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/File/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.192546 thug-5.0.1/thug/DOM/W3C/HTML/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      194 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/AudioTrackList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      610 2022-11-28 09:03:52.000000 thug-5.0.1/thug/DOM/W3C/HTML/Dataset.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      374 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLAllCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1922 2022-11-28 09:03:52.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLAnchorElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      654 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLAppletElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLAudioElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      252 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLBRElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      291 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLBaseElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      331 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1486 2023-05-10 07:54:25.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLBodyElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      582 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLButtonElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1281 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      265 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLDListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      263 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLDivElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    15982 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLDocument.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      955 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      412 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4141 2022-11-28 09:03:52.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      336 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      322 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLFontElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1742 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLFormElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      978 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLFrameElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      289 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      407 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLHRElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLHeadElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLHeadingElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLHtmlElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1300 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLIFrameElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1302 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLImageElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1466 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLInputElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      277 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      291 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLLIElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      373 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLLabelElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      376 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLLegendElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      558 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLLinkElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4216 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLMediaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      264 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLMenuElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      667 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLMetaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      296 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLModElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      378 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLOListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2595 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLObjectElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      343 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      720 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLOptionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      227 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      259 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLParagraphElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      378 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLParamElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLPreElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLQuoteElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      988 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLScriptElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1636 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLSelectElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      177 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLSpanElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      316 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLStyleElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      262 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      917 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableCellElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      445 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableColElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4711 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2800 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableRowElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2091 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1031 2023-01-12 15:47:27.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLTitleElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      336 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/HTMLUListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1105 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/TAnimateColor.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      280 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/TextTrackList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      681 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/TimeRanges.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5132 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      442 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/attr_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      426 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/bool_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      436 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/HTML/form_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      806 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/HTML/text_property.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.193546 thug-5.0.1/thug/DOM/W3C/Style/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.194546 thug-5.0.1/thug/DOM/W3C/Style/CSS/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1293 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      425 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Style/CSS/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Style/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.195546 thug-5.0.1/thug/DOM/W3C/URL/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4843 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/URL/URL.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2710 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/URL/URLSearchParams.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      115 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/URL/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.197546 thug-5.0.1/thug/DOM/W3C/Views/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      217 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Views/AbstractView.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      211 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Views/DocumentView.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/Views/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       56 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/W3C/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      367 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/W3C/w3c.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      829 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/WebStore.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    35015 2023-01-19 12:08:02.000000 thug-5.0.1/thug/DOM/Window.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/DOM/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     7624 2023-01-12 15:47:27.000000 thug-5.0.1/thug/DOM/w3c_bindings.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.198546 thug-5.0.1/thug/Encoding/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      877 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Encoding/Encoding.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Encoding/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.199546 thug-5.0.1/thug/Java/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1114 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Java/System.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Java/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      763 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Java/java.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      771 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Java/lang.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.203546 thug-5.0.1/thug/Logging/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2454 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/BaseLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3893 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/Features.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      920 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/LoggingModules.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5106 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/SampleLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    14604 2023-01-12 15:47:27.000000 thug-5.0.1/thug/Logging/ThugLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.207546 thug-5.0.1/thug/Logging/modules/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2565 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/modules/ElasticSearch.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1301 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/modules/ExploitGraph.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    14581 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/modules/JSON.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    10438 2022-12-06 12:21:07.000000 thug-5.0.1/thug/Logging/modules/Mapper.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16889 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/modules/MongoDB.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       83 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Logging/modules/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.208546 thug-5.0.1/thug/Magic/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1593 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Magic/Magic.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Magic/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.209546 thug-5.0.1/thug/OS/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4912 2022-11-28 09:02:06.000000 thug-5.0.1/thug/OS/Windows.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/OS/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.210546 thug-5.0.1/thug/Plugins/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      956 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Plugins/IPlugin.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3401 2023-01-12 15:47:27.000000 thug-5.0.1/thug/Plugins/ThugPlugins.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Plugins/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.210546 thug-5.0.1/thug/Plugins/plugins/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.211546 thug-5.0.1/thug/Plugins/plugins/POST-TestPlugin-999/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.212546 thug-5.0.1/thug/Plugins/plugins/PRE-TestPlugin-999/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/Plugins/plugins/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.216546 thug-5.0.1/thug/ThugAPI/
--rw-r--r--   0 buffer    (1000) buffer    (1000)    18741 2023-03-20 08:16:52.000000 thug-5.0.1/thug/ThugAPI/IThugAPI.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      787 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ThugAPI/OpaqueFilter.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16007 2023-03-20 08:16:52.000000 thug-5.0.1/thug/ThugAPI/ThugAPI.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9649 2023-03-20 08:16:52.000000 thug-5.0.1/thug/ThugAPI/ThugOpts.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4203 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ThugAPI/ThugVulnModules.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1642 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ThugAPI/Watchdog.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ThugAPI/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      317 2022-11-28 09:02:06.000000 thug-5.0.1/thug/ThugAPI/abstractmethod.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.218546 thug-5.0.1/thug/WebTracking/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3206 2022-11-28 09:02:06.000000 thug-5.0.1/thug/WebTracking/Cookies.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1176 2022-11-28 09:02:06.000000 thug-5.0.1/thug/WebTracking/WebStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1596 2022-11-28 09:02:06.000000 thug-5.0.1/thug/WebTracking/WebTracking.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-5.0.1/thug/WebTracking/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2026 2023-05-24 07:31:15.000000 thug-5.0.1/thug/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.219546 thug-5.0.1/thug/conf/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.219546 thug-5.0.1/thug/conf/hooks/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       45 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/hooks/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)      174 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/inspector.json
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.241547 thug-5.0.1/thug/conf/personalities/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/galaxy2chrome18.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/galaxy2chrome25.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      743 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/galaxy2chrome29.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      793 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome33.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome35.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome37.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome38.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome39.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome45.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome46.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      729 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadchrome47.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      692 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadsafari7.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      688 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadsafari8.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      680 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/ipadsafari9.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/linuxchrome26.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/linuxchrome30.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/linuxchrome44.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/linuxchrome54.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/linuxchrome98.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/linuxfirefox19.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/linuxfirefox40.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      748 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/nexuschrome18.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/osx10chrome19.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      690 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/osx10chrome80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/osx10chrome97.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/osx10safari5.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      682 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/osx11safari14.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      396 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/prefix_allocation.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2851 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win10edge20.json.review
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3826 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win10ie110.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win2kie60.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      915 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win2kie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7chrome20.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7chrome40.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7chrome45.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7chrome49.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      579 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7firefox3.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3769 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7ie100.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3800 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7ie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3820 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7ie90.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      678 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/win7safari5.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      674 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/winxpchrome20.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      564 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/winxpfirefox12.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2876 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/winxpie60.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2896 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/winxpie61.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2871 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/winxpie70.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2968 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/winxpie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      666 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/personalities/winxpsafari5.json
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.241547 thug-5.0.1/thug/conf/plugins/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       47 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/plugins/README
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.247547 thug-5.0.1/thug/conf/rules/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.247547 thug-5.0.1/thug/conf/rules/cookieclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/cookieclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/cookieclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.247547 thug-5.0.1/thug/conf/rules/cookiefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/cookiefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/cookiefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.248547 thug-5.0.1/thug/conf/rules/htmlclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/htmlclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/htmlclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.248547 thug-5.0.1/thug/conf/rules/htmlfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/htmlfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/htmlfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.249548 thug-5.0.1/thug/conf/rules/imageclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      115 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/imageclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/imageclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.249548 thug-5.0.1/thug/conf/rules/imagefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      103 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/imagefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/imagefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.250548 thug-5.0.1/thug/conf/rules/jsclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      245 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/jsclassifier/plugindetect.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/jsclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.250548 thug-5.0.1/thug/conf/rules/jsfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       97 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/jsfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/jsfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.251548 thug-5.0.1/thug/conf/rules/sampleclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/sampleclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/sampleclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.251548 thug-5.0.1/thug/conf/rules/samplefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/samplefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/samplefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.252548 thug-5.0.1/thug/conf/rules/textclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/textclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/textclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.253548 thug-5.0.1/thug/conf/rules/textfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/textfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/textfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.262548 thug-5.0.1/thug/conf/rules/urlclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3005 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/blackhole.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      418 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/cool.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/crimeboss.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      641 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/critxpack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1000 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/fiesta.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      870 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/g01pack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      387 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/impact.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      808 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/neutrino.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      612 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/nuclear.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      969 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/popads.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      765 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/redkit.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      427 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/safepack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      176 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/sakura.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      478 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/sofosfo.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2400 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/styx.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      849 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/sweetorange.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      340 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier/tds.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.263548 thug-5.0.1/thug/conf/rules/urlfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/urlfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.263548 thug-5.0.1/thug/conf/rules/vbsclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/vbsclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/vbsclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.264548 thug-5.0.1/thug/conf/rules/vbsfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/vbsfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/rules/vbsfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.266548 thug-5.0.1/thug/conf/scripts/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       69 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/scripts/date.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      197 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/scripts/eval.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)       87 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/scripts/message-event.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/scripts/storage.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      753 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/scripts/thug.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      205 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/scripts/write.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      325 2023-01-12 15:47:27.000000 thug-5.0.1/thug/conf/thug.conf
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.270548 thug-5.0.1/thug/thug.egg-info/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4017 2022-12-08 08:47:59.000000 thug-5.0.1/thug/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19264 2022-12-08 08:47:59.000000 thug-5.0.1/thug/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-08 08:47:59.000000 thug-5.0.1/thug/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2022-12-08 08:47:59.000000 thug-5.0.1/thug/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      486 2022-12-08 08:47:59.000000 thug-5.0.1/thug/thug.egg-info/requires.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       91 2022-12-08 08:47:59.000000 thug-5.0.1/thug/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-07 11:50:03.000000 thug-5.0.1/thug/thug.egg-info/zip-safe
--rw-r--r--   0 buffer    (1000) buffer    (1000)    17085 2023-03-20 08:16:52.000000 thug-5.0.1/thug/thug.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2023-05-24 07:31:49.048541 thug-5.0.1/thug.egg-info/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3950 2023-05-24 07:31:48.000000 thug-5.0.1/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16006 2023-05-24 07:31:49.000000 thug-5.0.1/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2023-05-24 07:31:48.000000 thug-5.0.1/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2023-05-24 07:31:48.000000 thug-5.0.1/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      507 2023-05-24 07:31:48.000000 thug-5.0.1/thug.egg-info/requires.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        5 2023-05-24 07:31:48.000000 thug-5.0.1/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2023-05-24 07:31:48.000000 thug-5.0.1/thug.egg-info/zip-safe
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.330650 thug-5.1/
+-rw-r--r--   0 buffer     (502) staff       (20)    17987 2022-12-28 14:31:40.000000 thug-5.1/LICENSE.txt
+-rw-r--r--   0 buffer     (502) staff       (20)      130 2023-01-03 13:39:45.000000 thug-5.1/MANIFEST.in
+-rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-06-09 06:55:31.330016 thug-5.1/PKG-INFO
+-rw-r--r--   0 buffer     (502) staff       (20)     2676 2023-01-17 09:44:55.000000 thug-5.1/README.rst
+-rw-r--r--   0 buffer     (502) staff       (20)     3485 2023-05-23 10:28:15.000000 thug-5.1/pyproject.toml
+-rw-r--r--   0 buffer     (502) staff       (20)      339 2023-05-23 10:28:25.000000 thug-5.1/requirements.txt
+-rw-r--r--   0 buffer     (502) staff       (20)       38 2023-06-09 06:55:31.330985 thug-5.1/setup.cfg
+-rw-r--r--   0 buffer     (502) staff       (20)     1346 2023-01-03 12:33:41.000000 thug-5.1/setup.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:30.910521 thug-5.1/thug/
+-rw-r--r--   0 buffer     (502) staff       (20)     8196 2022-11-04 15:21:57.000000 thug-5.1/thug/.DS_Store
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:30.918889 thug-5.1/thug/ActiveX/
+-rw-r--r--   0 buffer     (502) staff       (20)     7598 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/ActiveX.py
+-rw-r--r--   0 buffer     (502) staff       (20)    64018 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/CLSID.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.013098 thug-5.1/thug/ActiveX/modules/
+-rw-r--r--   0 buffer     (502) staff       (20)      400 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/AOLAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1119 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/AcroPDF.py
+-rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/AdodbRecordset.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2573 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/AdodbStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1482 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/AnswerWorks.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1086 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/AolAmpX.py
+-rw-r--r--   0 buffer     (502) staff       (20)      979 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/AolICQ.py
+-rw-r--r--   0 buffer     (502) staff       (20)      801 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/BaiduBar.py
+-rw-r--r--   0 buffer     (502) staff       (20)      567 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/BitDefender.py
+-rw-r--r--   0 buffer     (502) staff       (20)      421 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/CABrightStor.py
+-rw-r--r--   0 buffer     (502) staff       (20)      600 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/CGAgent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      726 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Comodo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ConnectAndEnterRoom.py
+-rw-r--r--   0 buffer     (502) staff       (20)      307 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/CreativeSoftAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/DLinkMPEG.py
+-rw-r--r--   0 buffer     (502) staff       (20)      673 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/DPClient.py
+-rw-r--r--   0 buffer     (502) staff       (20)      447 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/DVRHOSTWeb.py
+-rw-r--r--   0 buffer     (502) staff       (20)      625 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/DirectShow.py
+-rw-r--r--   0 buffer     (502) staff       (20)      404 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/DivX.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1857 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Domino.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1500 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/EnjoySAP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      825 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/FacebookPhotoUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3049 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/File.py
+-rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/FileUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2221 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Folder.py
+-rw-r--r--   0 buffer     (502) staff       (20)      496 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/GLIEDown2.py
+-rw-r--r--   0 buffer     (502) staff       (20)      656 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/GatewayWeblaunch.py
+-rw-r--r--   0 buffer     (502) staff       (20)      420 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Gogago.py
+-rw-r--r--   0 buffer     (502) staff       (20)      561 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/GomWeb.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4119 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/HPInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      443 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ICQToolbar.py
+-rw-r--r--   0 buffer     (502) staff       (20)      945 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/IMWebControl.py
+-rw-r--r--   0 buffer     (502) staff       (20)      672 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/InternetCleverSuite.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1964 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/JavaDeploymentToolkit.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
+-rw-r--r--   0 buffer     (502) staff       (20)      405 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Kingsoft.py
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/MSRICHTXT.py
+-rw-r--r--   0 buffer     (502) staff       (20)      601 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/MSVFP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      535 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/MSXML2DOMDocument.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4390 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/MacrovisionFlexNet.py
+-rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/MicrosoftWorks7Attack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2048 2023-01-13 08:09:32.000000 thug-5.1/thug/ActiveX/modules/MicrosoftXMLDOM.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8006 2023-01-06 14:50:41.000000 thug-5.1/thug/ActiveX/modules/MicrosoftXMLHTTP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      466 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Move.py
+-rw-r--r--   0 buffer     (502) staff       (20)      438 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/MyspaceUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)      589 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/NCTAudioFile2.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1259 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/NamoInstaller.py
+-rw-r--r--   0 buffer     (502) staff       (20)      616 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/NeoTracePro.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3311 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/NessusScanCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1175 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/OfficeOCX.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1057 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/OurgameGLWorld.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1201 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/PPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      498 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/PTZCamPanel.py
+-rw-r--r--   0 buffer     (502) staff       (20)      494 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/QuantumStreaming.py
+-rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/QvodCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)      973 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/RDSDataSpace.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2335 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/RealPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      348 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/RediffBolDownloaderAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)      831 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/RegistryPro.py
+-rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/RisingScanner.py
+-rw-r--r--   0 buffer     (502) staff       (20)      449 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/RtspVaPgCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1116 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/SSReaderPdg2.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1027 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ScriptingDictionary.py
+-rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ScriptingEncoder.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5185 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ScriptingFileSystemObject.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1527 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ShellApplication.py
+-rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Shockwave.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ShockwaveFlash10.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ShockwaveFlash11.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ShockwaveFlash12.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ShockwaveFlash9.py
+-rw-r--r--   0 buffer     (502) staff       (20)      273 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/SilverLight.py
+-rw-r--r--   0 buffer     (502) staff       (20)      921 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/SinaDLoader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1472 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/SnapshotViewer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      715 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
+-rw-r--r--   0 buffer     (502) staff       (20)      906 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Spreadsheet.py
+-rw-r--r--   0 buffer     (502) staff       (20)      677 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/StormConfig.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2436 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/StormMps.py
+-rw-r--r--   0 buffer     (502) staff       (20)      516 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/StreamAudioChainCast.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1061 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/SymantecAppStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2224 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/SymantecBackupExec.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4772 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/TextStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/Toshiba.py
+-rw-r--r--   0 buffer     (502) staff       (20)      391 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/UUSeeUpdate.py
+-rw-r--r--   0 buffer     (502) staff       (20)      691 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/UniversalUpload.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1763 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/VLC.py
+-rw-r--r--   0 buffer     (502) staff       (20)      719 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/VisualStudioDTE80.py
+-rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/VsaIDEDTE.py
+-rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/VsmIDEDTE.py
+-rw-r--r--   0 buffer     (502) staff       (20)      796 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WMEncProfileManager.py
+-rw-r--r--   0 buffer     (502) staff       (20)      132 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WMP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WScriptCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1280 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WScriptExec.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1689 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WScriptNetwork.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8980 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WScriptShell.py
+-rw-r--r--   0 buffer     (502) staff       (20)      213 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WScriptShortcut.py
+-rw-r--r--   0 buffer     (502) staff       (20)      645 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WebViewFolderIcon.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1373 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WinNTSystemInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      599 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WinZip.py
+-rw-r--r--   0 buffer     (502) staff       (20)      145 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/WindowsMediaPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      942 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/XMLDOMParseError.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1026 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/XUpload.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1159 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/YahooJukebox.py
+-rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/YahooMessengerCyft.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1077 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/YahooMessengerYVerInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1244 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/YahooMessengerYwcvwr.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1932 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2870 2022-12-28 14:31:40.000000 thug-5.1/thug/ActiveX/modules/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.013695 thug-5.1/thug/Analysis/
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.014594 thug-5.1/thug/Analysis/awis/
+-rw-r--r--   0 buffer     (502) staff       (20)     3224 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/awis/AWIS.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/awis/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.015491 thug-5.1/thug/Analysis/context/
+-rw-r--r--   0 buffer     (502) staff       (20)     1554 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/context/ContextAnalyzer.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/context/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.016378 thug-5.1/thug/Analysis/honeyagent/
+-rw-r--r--   0 buffer     (502) staff       (20)     4000 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/honeyagent/HoneyAgent.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/honeyagent/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.017251 thug-5.1/thug/Analysis/screenshot/
+-rw-r--r--   0 buffer     (502) staff       (20)     1333 2023-03-07 14:57:11.000000 thug-5.1/thug/Analysis/screenshot/Screenshot.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/screenshot/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.018321 thug-5.1/thug/Analysis/shellcode/
+-rw-r--r--   0 buffer     (502) staff       (20)     8069 2023-01-13 08:09:32.000000 thug-5.1/thug/Analysis/shellcode/Shellcode.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Analysis/shellcode/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.024828 thug-5.1/thug/Classifier/
+-rw-r--r--   0 buffer     (502) staff       (20)     5017 2023-03-28 13:07:55.000000 thug-5.1/thug/Classifier/BaseClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2106 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/CookieClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2159 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/HTMLClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2070 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/ImageClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2008 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/JSClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2243 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/SampleClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2082 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/TextClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2330 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/URLClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2014 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/VBSClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Classifier/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.054166 thug-5.1/thug/DOM/
+-rw-r--r--   0 buffer     (502) staff       (20)     2534 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Alexa.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2289 2023-03-28 10:08:11.000000 thug-5.1/thug/DOM/AsyncPrefetcher.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2254 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/CCInterpreter.py
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Chrome.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1304 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/ClipboardData.py
+-rw-r--r--   0 buffer     (502) staff       (20)      817 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Components.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5901 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Console.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1112 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Crypto.py
+-rw-r--r--   0 buffer     (502) staff       (20)    54541 2023-03-01 08:10:57.000000 thug-5.1/thug/DOM/DFT.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3602 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/External.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2776 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/HTMLInspector.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9866 2023-03-07 14:57:11.000000 thug-5.1/thug/DOM/HTTPSession.py
+-rw-r--r--   0 buffer     (502) staff       (20)      932 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/HTTPSessionException.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3593 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/History.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3506 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/JSClass.py
+-rw-r--r--   0 buffer     (502) staff       (20)     7824 2023-01-06 16:11:13.000000 thug-5.1/thug/DOM/JSEngine.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4502 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/JSInspector.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5959 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/JScriptEncode.py
+-rw-r--r--   0 buffer     (502) staff       (20)      752 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/LocalStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4661 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/Location.py
+-rw-r--r--   0 buffer     (502) staff       (20)    19549 2023-02-27 08:54:28.000000 thug-5.1/thug/DOM/MIMEHandler.py
+-rw-r--r--   0 buffer     (502) staff       (20)      762 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Map.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/MimeType.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5282 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/MimeTypes.py
+-rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/MozConnection.py
+-rw-r--r--   0 buffer     (502) staff       (20)    13340 2023-03-07 14:57:11.000000 thug-5.1/thug/DOM/Navigator.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4056 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Personality.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1233 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Plugin.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1471 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Plugins.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1069 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/SchemeHandler.py
+-rw-r--r--   0 buffer     (502) staff       (20)     6150 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Screen.py
+-rw-r--r--   0 buffer     (502) staff       (20)      756 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/SessionStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1750 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Sidebar.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3502 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Storage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3216 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/UserProfile.py
+-rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/Utils.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.060274 thug-5.1/thug/DOM/W3C/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.141323 thug-5.1/thug/DOM/W3C/Core/
+-rw-r--r--   0 buffer     (502) staff       (20)     2138 2023-01-06 12:37:35.000000 thug-5.1/thug/DOM/W3C/Core/Attr.py
+-rw-r--r--   0 buffer     (502) staff       (20)      265 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/CDATASection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1241 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Core/CharacterData.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3531 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Core/ClassList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      564 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/Comment.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1910 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Core/DOMException.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5765 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/DOMImplementation.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8868 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/Document.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2412 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/DocumentFragment.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1513 2023-01-06 12:31:24.000000 thug-5.1/thug/DOM/W3C/Core/DocumentType.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9544 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/Element.py
+-rw-r--r--   0 buffer     (502) staff       (20)      457 2023-01-06 12:38:21.000000 thug-5.1/thug/DOM/W3C/Core/Entity.py
+-rw-r--r--   0 buffer     (502) staff       (20)      501 2023-01-06 12:38:52.000000 thug-5.1/thug/DOM/W3C/Core/EntityReference.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Core/NamedNodeMap.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14464 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/Node.py
+-rw-r--r--   0 buffer     (502) staff       (20)      569 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/NodeList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      474 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/NodeType.py
+-rw-r--r--   0 buffer     (502) staff       (20)      485 2023-01-06 12:34:08.000000 thug-5.1/thug/DOM/W3C/Core/Notation.py
+-rw-r--r--   0 buffer     (502) staff       (20)      510 2023-01-06 12:34:27.000000 thug-5.1/thug/DOM/W3C/Core/ProcessingInstruction.py
+-rw-r--r--   0 buffer     (502) staff       (20)      803 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/Text.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1051 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Core/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      337 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Core/abstractmethod.py
+-rw-r--r--   0 buffer     (502) staff       (20)      274 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/DOMParser.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1454 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/DOMTokenList.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.162648 thug-5.1/thug/DOM/W3C/Events/
+-rw-r--r--   0 buffer     (502) staff       (20)      868 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/DocumentEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4120 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/Event.py
+-rw-r--r--   0 buffer     (502) staff       (20)      525 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/EventException.py
+-rw-r--r--   0 buffer     (502) staff       (20)      272 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/EventListener.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9134 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/EventTarget.py
+-rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/HTMLEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1206 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/MessageEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2198 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/MouseEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1575 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/MutationEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/StorageEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      636 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Events/UIEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      691 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/Events/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.168322 thug-5.1/thug/DOM/W3C/File/
+-rw-r--r--   0 buffer     (502) staff       (20)     2433 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/File/Blob.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1381 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/File/File.py
+-rw-r--r--   0 buffer     (502) staff       (20)       85 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/File/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.219448 thug-5.1/thug/DOM/W3C/HTML/
+-rw-r--r--   0 buffer     (502) staff       (20)      194 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/AudioTrackList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/Dataset.py
+-rw-r--r--   0 buffer     (502) staff       (20)      374 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLAllCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1922 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLAnchorElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      654 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLAppletElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLAudioElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      252 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLBRElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLBaseElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      331 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1486 2023-04-11 09:54:20.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLBodyElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      582 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLButtonElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1281 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)      265 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLDListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      263 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLDivElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)    15982 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLDocument.py
+-rw-r--r--   0 buffer     (502) staff       (20)      955 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      412 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4141 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      322 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLFontElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1742 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLFormElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      978 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLFrameElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      289 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      407 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLHRElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLHeadElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLHeadingElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLHtmlElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1300 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLIFrameElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1302 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLImageElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1466 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLInputElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      277 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLLIElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      373 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLLabelElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      376 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLLegendElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      558 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLLinkElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4216 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLMediaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      264 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLMenuElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      667 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLMetaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      296 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLModElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLOListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2595 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLObjectElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      343 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLOptionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      227 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)      259 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLParagraphElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLParamElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLPreElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLQuoteElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      988 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLScriptElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1636 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLSelectElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      177 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLSpanElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      316 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLStyleElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      262 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      917 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTableCellElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTableColElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4711 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTableElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2800 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTableRowElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2091 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1031 2022-12-30 12:26:43.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLTitleElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/HTMLUListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/TAnimateColor.py
+-rw-r--r--   0 buffer     (502) staff       (20)      280 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/TextTrackList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      681 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/TimeRanges.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5132 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      442 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/attr_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      426 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/bool_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      436 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/HTML/form_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      806 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/HTML/text_property.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.219945 thug-5.1/thug/DOM/W3C/Style/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.221882 thug-5.1/thug/DOM/W3C/Style/CSS/
+-rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
+-rw-r--r--   0 buffer     (502) staff       (20)      425 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Style/CSS/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Style/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.223482 thug-5.1/thug/DOM/W3C/URL/
+-rw-r--r--   0 buffer     (502) staff       (20)     4843 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/URL/URL.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2710 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/URL/URLSearchParams.py
+-rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/URL/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.226693 thug-5.1/thug/DOM/W3C/Views/
+-rw-r--r--   0 buffer     (502) staff       (20)      217 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Views/AbstractView.py
+-rw-r--r--   0 buffer     (502) staff       (20)      211 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Views/DocumentView.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/Views/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)       56 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/W3C/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      367 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/W3C/w3c.py
+-rw-r--r--   0 buffer     (502) staff       (20)      829 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/WebStore.py
+-rw-r--r--   0 buffer     (502) staff       (20)    35015 2023-01-13 08:09:32.000000 thug-5.1/thug/DOM/Window.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)     7624 2022-12-28 14:31:40.000000 thug-5.1/thug/DOM/w3c_bindings.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.227858 thug-5.1/thug/Encoding/
+-rw-r--r--   0 buffer     (502) staff       (20)      877 2022-12-28 14:31:40.000000 thug-5.1/thug/Encoding/Encoding.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Encoding/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.230350 thug-5.1/thug/Java/
+-rw-r--r--   0 buffer     (502) staff       (20)     1114 2022-12-28 14:31:40.000000 thug-5.1/thug/Java/System.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Java/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      763 2022-12-28 14:31:40.000000 thug-5.1/thug/Java/java.py
+-rw-r--r--   0 buffer     (502) staff       (20)      771 2022-12-28 14:31:40.000000 thug-5.1/thug/Java/lang.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.236735 thug-5.1/thug/Logging/
+-rw-r--r--   0 buffer     (502) staff       (20)     2454 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/BaseLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3893 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/Features.py
+-rw-r--r--   0 buffer     (502) staff       (20)      920 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/LoggingModules.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5106 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/SampleLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14604 2023-01-03 10:16:05.000000 thug-5.1/thug/Logging/ThugLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.241036 thug-5.1/thug/Logging/modules/
+-rw-r--r--   0 buffer     (502) staff       (20)     2565 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/modules/ElasticSearch.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1301 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/modules/ExploitGraph.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14581 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/modules/JSON.py
+-rw-r--r--   0 buffer     (502) staff       (20)    10438 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/modules/Mapper.py
+-rw-r--r--   0 buffer     (502) staff       (20)    16889 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/modules/MongoDB.py
+-rw-r--r--   0 buffer     (502) staff       (20)       83 2022-12-28 14:31:40.000000 thug-5.1/thug/Logging/modules/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.242813 thug-5.1/thug/Magic/
+-rw-r--r--   0 buffer     (502) staff       (20)     1593 2022-12-28 14:31:40.000000 thug-5.1/thug/Magic/Magic.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Magic/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.244252 thug-5.1/thug/OS/
+-rw-r--r--   0 buffer     (502) staff       (20)     4912 2022-12-28 14:31:40.000000 thug-5.1/thug/OS/Windows.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/OS/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.245960 thug-5.1/thug/Plugins/
+-rw-r--r--   0 buffer     (502) staff       (20)      956 2022-12-28 14:31:40.000000 thug-5.1/thug/Plugins/IPlugin.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3401 2023-01-03 10:15:59.000000 thug-5.1/thug/Plugins/ThugPlugins.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Plugins/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.252224 thug-5.1/thug/Plugins/plugins/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.254167 thug-5.1/thug/Plugins/plugins/POST-TestPlugin-999/
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.1/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.255196 thug-5.1/thug/Plugins/plugins/PRE-TestPlugin-999/
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.1/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/Plugins/plugins/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.261190 thug-5.1/thug/ThugAPI/
+-rw-r--r--   0 buffer     (502) staff       (20)    18741 2023-03-07 14:57:11.000000 thug-5.1/thug/ThugAPI/IThugAPI.py
+-rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.1/thug/ThugAPI/OpaqueFilter.py
+-rw-r--r--   0 buffer     (502) staff       (20)    16007 2023-03-07 14:57:11.000000 thug-5.1/thug/ThugAPI/ThugAPI.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9649 2023-03-07 14:57:11.000000 thug-5.1/thug/ThugAPI/ThugOpts.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4203 2022-12-28 14:31:40.000000 thug-5.1/thug/ThugAPI/ThugVulnModules.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1642 2022-12-28 14:31:40.000000 thug-5.1/thug/ThugAPI/Watchdog.py
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.1/thug/ThugAPI/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      317 2022-12-28 14:31:40.000000 thug-5.1/thug/ThugAPI/abstractmethod.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.265041 thug-5.1/thug/WebTracking/
+-rw-r--r--   0 buffer     (502) staff       (20)     3206 2022-12-28 14:31:40.000000 thug-5.1/thug/WebTracking/Cookies.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1176 2022-12-28 14:31:40.000000 thug-5.1/thug/WebTracking/WebStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1596 2022-12-28 14:31:40.000000 thug-5.1/thug/WebTracking/WebTracking.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/WebTracking/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2024 2023-06-09 06:51:58.000000 thug-5.1/thug/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.266766 thug-5.1/thug/conf/
+-rw-r--r--   0 buffer     (502) staff       (20)     6148 2022-11-04 15:21:57.000000 thug-5.1/thug/conf/.DS_Store
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.267242 thug-5.1/thug/conf/hooks/
+-rw-r--r--   0 buffer     (502) staff       (20)       45 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/hooks/README
+-rw-r--r--   0 buffer     (502) staff       (20)      174 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/inspector.json
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.296571 thug-5.1/thug/conf/personalities/
+-rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/galaxy2chrome18.json
+-rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/galaxy2chrome25.json
+-rw-r--r--   0 buffer     (502) staff       (20)      743 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/galaxy2chrome29.json
+-rw-r--r--   0 buffer     (502) staff       (20)      793 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome33.json
+-rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome35.json
+-rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome37.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome38.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome39.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome45.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome46.json
+-rw-r--r--   0 buffer     (502) staff       (20)      729 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadchrome47.json
+-rw-r--r--   0 buffer     (502) staff       (20)      692 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadsafari7.json
+-rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadsafari8.json
+-rw-r--r--   0 buffer     (502) staff       (20)      680 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/ipadsafari9.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/linuxchrome26.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/linuxchrome30.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/linuxchrome44.json
+-rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/linuxchrome54.json
+-rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/linuxchrome98.json
+-rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/linuxfirefox19.json
+-rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/linuxfirefox40.json
+-rw-r--r--   0 buffer     (502) staff       (20)      748 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/nexuschrome18.json
+-rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/osx10chrome19.json
+-rw-r--r--   0 buffer     (502) staff       (20)      690 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/osx10chrome80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/osx10chrome97.json
+-rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/osx10safari5.json
+-rw-r--r--   0 buffer     (502) staff       (20)      682 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/osx11safari14.json
+-rw-r--r--   0 buffer     (502) staff       (20)      396 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/prefix_allocation.txt
+-rw-r--r--   0 buffer     (502) staff       (20)     2851 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win10edge20.json.review
+-rw-r--r--   0 buffer     (502) staff       (20)     3826 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win10ie110.json
+-rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win2kie60.json
+-rw-r--r--   0 buffer     (502) staff       (20)      915 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win2kie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7chrome20.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7chrome40.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7chrome45.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7chrome49.json
+-rw-r--r--   0 buffer     (502) staff       (20)      579 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7firefox3.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3769 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7ie100.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3800 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7ie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3820 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7ie90.json
+-rw-r--r--   0 buffer     (502) staff       (20)      678 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/win7safari5.json
+-rw-r--r--   0 buffer     (502) staff       (20)      674 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/winxpchrome20.json
+-rw-r--r--   0 buffer     (502) staff       (20)      564 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/winxpfirefox12.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2876 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/winxpie60.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2896 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/winxpie61.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2871 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/winxpie70.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2968 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/winxpie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      666 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/personalities/winxpsafari5.json
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.297119 thug-5.1/thug/conf/plugins/
+-rw-r--r--   0 buffer     (502) staff       (20)       47 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/plugins/README
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.304369 thug-5.1/thug/conf/rules/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.304894 thug-5.1/thug/conf/rules/cookieclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/cookieclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/cookieclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.305478 thug-5.1/thug/conf/rules/cookiefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/cookiefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/cookiefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.306164 thug-5.1/thug/conf/rules/htmlclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/htmlclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/htmlclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.306874 thug-5.1/thug/conf/rules/htmlfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/htmlfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/htmlfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.307670 thug-5.1/thug/conf/rules/imageclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/imageclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/imageclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.308497 thug-5.1/thug/conf/rules/imagefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      103 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/imagefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/imagefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.309203 thug-5.1/thug/conf/rules/jsclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      245 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/jsclassifier/plugindetect.yar
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/jsclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.309805 thug-5.1/thug/conf/rules/jsfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       97 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/jsfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/jsfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.310452 thug-5.1/thug/conf/rules/sampleclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/sampleclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/sampleclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.311171 thug-5.1/thug/conf/rules/samplefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/samplefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/samplefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.311835 thug-5.1/thug/conf/rules/textclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/textclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/textclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.312513 thug-5.1/thug/conf/rules/textfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/textfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/textfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.322864 thug-5.1/thug/conf/rules/urlclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)     3005 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/blackhole.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      418 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/cool.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/crimeboss.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      641 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/critxpack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)     1000 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/fiesta.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      870 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/g01pack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      387 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/impact.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      808 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/neutrino.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      612 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/nuclear.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      969 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/popads.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      765 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/redkit.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      427 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/safepack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      176 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/sakura.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/sofosfo.yar
+-rw-r--r--   0 buffer     (502) staff       (20)     2400 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/styx.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      849 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/sweetorange.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      340 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier/tds.yar
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.323361 thug-5.1/thug/conf/rules/urlfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/urlfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.324513 thug-5.1/thug/conf/rules/vbsclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/vbsclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/vbsclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.325351 thug-5.1/thug/conf/rules/vbsfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/vbsfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/rules/vbsfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:31.329320 thug-5.1/thug/conf/scripts/
+-rw-r--r--   0 buffer     (502) staff       (20)       69 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/scripts/date.js
+-rw-r--r--   0 buffer     (502) staff       (20)      197 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/scripts/eval.js
+-rw-r--r--   0 buffer     (502) staff       (20)       87 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/scripts/message-event.js
+-rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/scripts/storage.js
+-rw-r--r--   0 buffer     (502) staff       (20)      753 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/scripts/thug.js
+-rw-r--r--   0 buffer     (502) staff       (20)      205 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/scripts/write.js
+-rw-r--r--   0 buffer     (502) staff       (20)      325 2022-12-28 14:31:40.000000 thug-5.1/thug/conf/thug.conf
+-rw-r--r--   0 buffer     (502) staff       (20)    17085 2023-03-07 14:57:11.000000 thug-5.1/thug/thug.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-09 06:55:30.916742 thug-5.1/thug.egg-info/
+-rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-06-09 06:55:30.000000 thug-5.1/thug.egg-info/PKG-INFO
+-rw-r--r--   0 buffer     (502) staff       (20)    15813 2023-06-09 06:55:30.000000 thug-5.1/thug.egg-info/SOURCES.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        1 2023-06-09 06:55:30.000000 thug-5.1/thug.egg-info/dependency_links.txt
+-rw-r--r--   0 buffer     (502) staff       (20)       40 2023-06-09 06:55:30.000000 thug-5.1/thug.egg-info/entry_points.txt
+-rw-r--r--   0 buffer     (502) staff       (20)      507 2023-06-09 06:55:30.000000 thug-5.1/thug.egg-info/requires.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        5 2023-06-09 06:55:30.000000 thug-5.1/thug.egg-info/top_level.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        1 2023-06-09 06:55:30.000000 thug-5.1/thug.egg-info/zip-safe
```

### Comparing `thug-5.0.1/LICENSE.txt` & `thug-5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/PKG-INFO` & `thug-5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 5.0.1
+Version: 5.1
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
```

### Comparing `thug-5.0.1/README.rst` & `thug-5.1/README.rst`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/pyproject.toml` & `thug-5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/setup.py` & `thug-5.1/setup.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/ActiveX.py` & `thug-5.1/thug/ActiveX/ActiveX.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/CLSID.py` & `thug-5.1/thug/ActiveX/CLSID.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/AcroPDF.py` & `thug-5.1/thug/ActiveX/modules/AcroPDF.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/AdodbRecordset.py` & `thug-5.1/thug/ActiveX/modules/AdodbRecordset.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/AdodbStream.py` & `thug-5.1/thug/ActiveX/modules/AdodbStream.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/AnswerWorks.py` & `thug-5.1/thug/ActiveX/modules/AnswerWorks.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/AolAmpX.py` & `thug-5.1/thug/ActiveX/modules/AolAmpX.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/AolICQ.py` & `thug-5.1/thug/ActiveX/modules/AolICQ.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/BaiduBar.py` & `thug-5.1/thug/ActiveX/modules/BaiduBar.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/BitDefender.py` & `thug-5.1/thug/ActiveX/modules/BitDefender.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/CGAgent.py` & `thug-5.1/thug/ActiveX/modules/CGAgent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/Comodo.py` & `thug-5.1/thug/ActiveX/modules/Comodo.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/ConnectAndEnterRoom.py` & `thug-5.1/thug/ActiveX/modules/ConnectAndEnterRoom.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/DPClient.py` & `thug-5.1/thug/ActiveX/modules/DPClient.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/DirectShow.py` & `thug-5.1/thug/ActiveX/modules/DirectShow.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/Domino.py` & `thug-5.1/thug/ActiveX/modules/Domino.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/EnjoySAP.py` & `thug-5.1/thug/ActiveX/modules/EnjoySAP.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/FacebookPhotoUploader.py` & `thug-5.1/thug/ActiveX/modules/FacebookPhotoUploader.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/File.py` & `thug-5.1/thug/ActiveX/modules/File.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/Folder.py` & `thug-5.1/thug/ActiveX/modules/Folder.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/GatewayWeblaunch.py` & `thug-5.1/thug/ActiveX/modules/GatewayWeblaunch.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/GomWeb.py` & `thug-5.1/thug/ActiveX/modules/GomWeb.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/HPInfo.py` & `thug-5.1/thug/ActiveX/modules/HPInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/IMWebControl.py` & `thug-5.1/thug/ActiveX/modules/IMWebControl.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/InternetCleverSuite.py` & `thug-5.1/thug/ActiveX/modules/InternetCleverSuite.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/JavaDeploymentToolkit.py` & `thug-5.1/thug/ActiveX/modules/JavaDeploymentToolkit.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py` & `thug-5.1/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/MSRICHTXT.py` & `thug-5.1/thug/ActiveX/modules/MSRICHTXT.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/MSVFP.py` & `thug-5.1/thug/ActiveX/modules/MSVFP.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/MSXML2DOMDocument.py` & `thug-5.1/thug/ActiveX/modules/MSXML2DOMDocument.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/MacrovisionFlexNet.py` & `thug-5.1/thug/ActiveX/modules/MacrovisionFlexNet.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/MicrosoftXMLDOM.py` & `thug-5.1/thug/ActiveX/modules/MicrosoftXMLDOM.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/MicrosoftXMLHTTP.py` & `thug-5.1/thug/ActiveX/modules/MicrosoftXMLHTTP.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/NCTAudioFile2.py` & `thug-5.1/thug/ActiveX/modules/NCTAudioFile2.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/NamoInstaller.py` & `thug-5.1/thug/ActiveX/modules/NamoInstaller.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/NeoTracePro.py` & `thug-5.1/thug/ActiveX/modules/NeoTracePro.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/NessusScanCtrl.py` & `thug-5.1/thug/ActiveX/modules/NessusScanCtrl.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/OfficeOCX.py` & `thug-5.1/thug/ActiveX/modules/OfficeOCX.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/OurgameGLWorld.py` & `thug-5.1/thug/ActiveX/modules/OurgameGLWorld.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/PPlayer.py` & `thug-5.1/thug/ActiveX/modules/PPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/RDSDataSpace.py` & `thug-5.1/thug/ActiveX/modules/RDSDataSpace.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/RealPlayer.py` & `thug-5.1/thug/ActiveX/modules/RealPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/RegistryPro.py` & `thug-5.1/thug/ActiveX/modules/RegistryPro.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/SSReaderPdg2.py` & `thug-5.1/thug/ActiveX/modules/SSReaderPdg2.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/ScriptingDictionary.py` & `thug-5.1/thug/ActiveX/modules/ScriptingDictionary.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/ScriptingFileSystemObject.py` & `thug-5.1/thug/ActiveX/modules/ScriptingFileSystemObject.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/ShellApplication.py` & `thug-5.1/thug/ActiveX/modules/ShellApplication.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/SinaDLoader.py` & `thug-5.1/thug/ActiveX/modules/SinaDLoader.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/SnapshotViewer.py` & `thug-5.1/thug/ActiveX/modules/SnapshotViewer.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py` & `thug-5.1/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/Spreadsheet.py` & `thug-5.1/thug/ActiveX/modules/Spreadsheet.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/StormConfig.py` & `thug-5.1/thug/ActiveX/modules/StormConfig.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/StormMps.py` & `thug-5.1/thug/ActiveX/modules/StormMps.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/StreamAudioChainCast.py` & `thug-5.1/thug/ActiveX/modules/StreamAudioChainCast.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/SymantecAppStream.py` & `thug-5.1/thug/ActiveX/modules/SymantecAppStream.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/SymantecBackupExec.py` & `thug-5.1/thug/ActiveX/modules/SymantecBackupExec.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/TextStream.py` & `thug-5.1/thug/ActiveX/modules/TextStream.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/Toshiba.py` & `thug-5.1/thug/ActiveX/modules/Toshiba.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/UniversalUpload.py` & `thug-5.1/thug/ActiveX/modules/UniversalUpload.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/VLC.py` & `thug-5.1/thug/ActiveX/modules/VLC.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/VisualStudioDTE80.py` & `thug-5.1/thug/ActiveX/modules/VisualStudioDTE80.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/VsaIDEDTE.py` & `thug-5.1/thug/ActiveX/modules/VsaIDEDTE.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/VsmIDEDTE.py` & `thug-5.1/thug/ActiveX/modules/VsmIDEDTE.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/WMEncProfileManager.py` & `thug-5.1/thug/ActiveX/modules/WMEncProfileManager.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/WScriptExec.py` & `thug-5.1/thug/ActiveX/modules/WScriptExec.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/WScriptNetwork.py` & `thug-5.1/thug/ActiveX/modules/WScriptNetwork.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/WScriptShell.py` & `thug-5.1/thug/ActiveX/modules/WScriptShell.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/WebViewFolderIcon.py` & `thug-5.1/thug/ActiveX/modules/WebViewFolderIcon.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/WinNTSystemInfo.py` & `thug-5.1/thug/ActiveX/modules/WinNTSystemInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/WinZip.py` & `thug-5.1/thug/ActiveX/modules/WinZip.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/XMLDOMParseError.py` & `thug-5.1/thug/ActiveX/modules/XMLDOMParseError.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/XUpload.py` & `thug-5.1/thug/ActiveX/modules/XUpload.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/YahooJukebox.py` & `thug-5.1/thug/ActiveX/modules/YahooJukebox.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/YahooMessengerCyft.py` & `thug-5.1/thug/ActiveX/modules/YahooMessengerCyft.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/YahooMessengerYVerInfo.py` & `thug-5.1/thug/ActiveX/modules/YahooMessengerYVerInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/YahooMessengerYwcvwr.py` & `thug-5.1/thug/ActiveX/modules/YahooMessengerYwcvwr.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py` & `thug-5.1/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ActiveX/modules/__init__.py` & `thug-5.1/thug/ActiveX/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Analysis/awis/AWIS.py` & `thug-5.1/thug/Analysis/awis/AWIS.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Analysis/context/ContextAnalyzer.py` & `thug-5.1/thug/Analysis/context/ContextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Analysis/honeyagent/HoneyAgent.py` & `thug-5.1/thug/Analysis/honeyagent/HoneyAgent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Analysis/screenshot/Screenshot.py` & `thug-5.1/thug/Analysis/screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Analysis/shellcode/Shellcode.py` & `thug-5.1/thug/Analysis/shellcode/Shellcode.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/BaseClassifier.py` & `thug-5.1/thug/Classifier/BaseClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/CookieClassifier.py` & `thug-5.1/thug/Classifier/CookieClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/HTMLClassifier.py` & `thug-5.1/thug/Classifier/HTMLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/ImageClassifier.py` & `thug-5.1/thug/Classifier/ImageClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/JSClassifier.py` & `thug-5.1/thug/Classifier/JSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/SampleClassifier.py` & `thug-5.1/thug/Classifier/SampleClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/TextClassifier.py` & `thug-5.1/thug/Classifier/TextClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/URLClassifier.py` & `thug-5.1/thug/Classifier/URLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Classifier/VBSClassifier.py` & `thug-5.1/thug/Classifier/VBSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Alexa.py` & `thug-5.1/thug/DOM/Alexa.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/AsyncPrefetcher.py` & `thug-5.1/thug/DOM/AsyncPrefetcher.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/CCInterpreter.py` & `thug-5.1/thug/DOM/CCInterpreter.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Chrome.py` & `thug-5.1/thug/DOM/Chrome.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/ClipboardData.py` & `thug-5.1/thug/DOM/ClipboardData.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Components.py` & `thug-5.1/thug/DOM/Components.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Console.py` & `thug-5.1/thug/DOM/Console.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Crypto.py` & `thug-5.1/thug/DOM/Crypto.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/DFT.py` & `thug-5.1/thug/DOM/DFT.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/External.py` & `thug-5.1/thug/DOM/External.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/HTMLInspector.py` & `thug-5.1/thug/DOM/HTMLInspector.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/HTTPSession.py` & `thug-5.1/thug/DOM/HTTPSession.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/HTTPSessionException.py` & `thug-5.1/thug/DOM/HTTPSessionException.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/History.py` & `thug-5.1/thug/DOM/History.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/JSClass.py` & `thug-5.1/thug/DOM/JSClass.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/JSEngine.py` & `thug-5.1/thug/DOM/JSEngine.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/JSInspector.py` & `thug-5.1/thug/DOM/JSInspector.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/JScriptEncode.py` & `thug-5.1/thug/DOM/JScriptEncode.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/LocalStorage.py` & `thug-5.1/thug/DOM/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Location.py` & `thug-5.1/thug/DOM/Location.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/MIMEHandler.py` & `thug-5.1/thug/DOM/MIMEHandler.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Map.py` & `thug-5.1/thug/DOM/Map.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/MimeType.py` & `thug-5.1/thug/DOM/MimeType.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/MimeTypes.py` & `thug-5.1/thug/DOM/MimeTypes.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/MozConnection.py` & `thug-5.1/thug/DOM/MozConnection.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Navigator.py` & `thug-5.1/thug/DOM/Navigator.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Personality.py` & `thug-5.1/thug/DOM/Personality.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Plugin.py` & `thug-5.1/thug/DOM/Plugin.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Plugins.py` & `thug-5.1/thug/DOM/Plugins.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/SchemeHandler.py` & `thug-5.1/thug/DOM/SchemeHandler.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Screen.py` & `thug-5.1/thug/DOM/Screen.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/SessionStorage.py` & `thug-5.1/thug/DOM/SessionStorage.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Sidebar.py` & `thug-5.1/thug/DOM/Sidebar.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Storage.py` & `thug-5.1/thug/DOM/Storage.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/UserProfile.py` & `thug-5.1/thug/DOM/UserProfile.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Utils.py` & `thug-5.1/thug/DOM/Utils.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/Attr.py` & `thug-5.1/thug/DOM/W3C/Core/Attr.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/CharacterData.py` & `thug-5.1/thug/DOM/W3C/Core/CharacterData.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/ClassList.py` & `thug-5.1/thug/DOM/W3C/Core/ClassList.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/Comment.py` & `thug-5.1/thug/DOM/W3C/Core/Comment.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/DOMException.py` & `thug-5.1/thug/DOM/W3C/Core/DOMException.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/DOMImplementation.py` & `thug-5.1/thug/DOM/W3C/Core/DOMImplementation.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/Document.py` & `thug-5.1/thug/DOM/W3C/Core/Document.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/DocumentFragment.py` & `thug-5.1/thug/DOM/W3C/Core/DocumentFragment.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/DocumentType.py` & `thug-5.1/thug/DOM/W3C/Core/DocumentType.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/Element.py` & `thug-5.1/thug/DOM/W3C/Core/Element.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/NamedNodeMap.py` & `thug-5.1/thug/DOM/W3C/Core/NamedNodeMap.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/Node.py` & `thug-5.1/thug/DOM/W3C/Core/Node.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/NodeList.py` & `thug-5.1/thug/DOM/W3C/Core/NodeList.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/Text.py` & `thug-5.1/thug/DOM/W3C/Core/Text.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Core/__init__.py` & `thug-5.1/thug/DOM/W3C/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/DOMTokenList.py` & `thug-5.1/thug/DOM/W3C/DOMTokenList.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/DocumentEvent.py` & `thug-5.1/thug/DOM/W3C/Events/DocumentEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/Event.py` & `thug-5.1/thug/DOM/W3C/Events/Event.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/EventException.py` & `thug-5.1/thug/DOM/W3C/Events/EventException.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/EventTarget.py` & `thug-5.1/thug/DOM/W3C/Events/EventTarget.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/MessageEvent.py` & `thug-5.1/thug/DOM/W3C/Events/MessageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/MouseEvent.py` & `thug-5.1/thug/DOM/W3C/Events/MouseEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/MutationEvent.py` & `thug-5.1/thug/DOM/W3C/Events/MutationEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/StorageEvent.py` & `thug-5.1/thug/DOM/W3C/Events/StorageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/UIEvent.py` & `thug-5.1/thug/DOM/W3C/Events/UIEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Events/__init__.py` & `thug-5.1/thug/DOM/W3C/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/File/Blob.py` & `thug-5.1/thug/DOM/W3C/File/Blob.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/File/File.py` & `thug-5.1/thug/DOM/W3C/File/File.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/Dataset.py` & `thug-5.1/thug/DOM/W3C/HTML/Dataset.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLAnchorElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLAnchorElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLAppletElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLAppletElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLBodyElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLBodyElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLButtonElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLButtonElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLCollection.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLCollection.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLDocument.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLFormElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLFormElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLFrameElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLIFrameElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLIFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLImageElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLImageElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLInputElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLInputElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLLinkElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLLinkElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLMediaElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLMediaElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLMetaElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLMetaElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLObjectElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLObjectElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLOptionElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLOptionElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLScriptElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLScriptElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLSelectElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLSelectElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableCellElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLTableCellElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLTableElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableRowElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLTableRowElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLTableSectionElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLTableSectionElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/HTMLTextAreaElement.py` & `thug-5.1/thug/DOM/W3C/HTML/HTMLTextAreaElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/TAnimateColor.py` & `thug-5.1/thug/DOM/W3C/HTML/TAnimateColor.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/TimeRanges.py` & `thug-5.1/thug/DOM/W3C/HTML/TimeRanges.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/__init__.py` & `thug-5.1/thug/DOM/W3C/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/HTML/text_property.py` & `thug-5.1/thug/DOM/W3C/HTML/text_property.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py` & `thug-5.1/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/URL/URL.py` & `thug-5.1/thug/DOM/W3C/URL/URL.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/W3C/URL/URLSearchParams.py` & `thug-5.1/thug/DOM/W3C/URL/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/WebStore.py` & `thug-5.1/thug/DOM/WebStore.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/Window.py` & `thug-5.1/thug/DOM/Window.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/DOM/w3c_bindings.py` & `thug-5.1/thug/DOM/w3c_bindings.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Encoding/Encoding.py` & `thug-5.1/thug/Encoding/Encoding.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Java/System.py` & `thug-5.1/thug/Java/System.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Java/java.py` & `thug-5.1/thug/Java/java.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Java/lang.py` & `thug-5.1/thug/Java/lang.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/BaseLogging.py` & `thug-5.1/thug/Logging/BaseLogging.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/Features.py` & `thug-5.1/thug/Logging/Features.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/LoggingModules.py` & `thug-5.1/thug/Logging/LoggingModules.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/SampleLogging.py` & `thug-5.1/thug/Logging/SampleLogging.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/ThugLogging.py` & `thug-5.1/thug/Logging/ThugLogging.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/modules/ElasticSearch.py` & `thug-5.1/thug/Logging/modules/ElasticSearch.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/modules/ExploitGraph.py` & `thug-5.1/thug/Logging/modules/ExploitGraph.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/modules/JSON.py` & `thug-5.1/thug/Logging/modules/JSON.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/modules/Mapper.py` & `thug-5.1/thug/Logging/modules/Mapper.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Logging/modules/MongoDB.py` & `thug-5.1/thug/Logging/modules/MongoDB.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Magic/Magic.py` & `thug-5.1/thug/Magic/Magic.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/OS/Windows.py` & `thug-5.1/thug/OS/Windows.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Plugins/IPlugin.py` & `thug-5.1/thug/Plugins/IPlugin.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Plugins/ThugPlugins.py` & `thug-5.1/thug/Plugins/ThugPlugins.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py` & `thug-5.1/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py` & `thug-5.1/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ThugAPI/IThugAPI.py` & `thug-5.1/thug/ThugAPI/IThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ThugAPI/OpaqueFilter.py` & `thug-5.1/thug/ThugAPI/OpaqueFilter.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ThugAPI/ThugAPI.py` & `thug-5.1/thug/ThugAPI/ThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ThugAPI/ThugOpts.py` & `thug-5.1/thug/ThugAPI/ThugOpts.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ThugAPI/ThugVulnModules.py` & `thug-5.1/thug/ThugAPI/ThugVulnModules.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/ThugAPI/Watchdog.py` & `thug-5.1/thug/ThugAPI/Watchdog.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/WebTracking/Cookies.py` & `thug-5.1/thug/WebTracking/Cookies.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/WebTracking/WebStorage.py` & `thug-5.1/thug/WebTracking/WebStorage.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/WebTracking/WebTracking.py` & `thug-5.1/thug/WebTracking/WebTracking.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/__init__.py` & `thug-5.1/thug/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import appdirs
 
-__version__            = "5.0.1"
+__version__            = "5.1"
 __jsengine__           = ""
 __jsengine_version__   = ""
 
 __global_configuration_path__ = "/etc/thug"
 if os.path.exists(__global_configuration_path__):
     __configuration_path__ = __global_configuration_path__
 else:
```

### Comparing `thug-5.0.1/thug/conf/personalities/galaxy2chrome18.json` & `thug-5.1/thug/conf/personalities/galaxy2chrome18.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/galaxy2chrome25.json` & `thug-5.1/thug/conf/personalities/galaxy2chrome25.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/galaxy2chrome29.json` & `thug-5.1/thug/conf/personalities/galaxy2chrome29.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome33.json` & `thug-5.1/thug/conf/personalities/ipadchrome33.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome35.json` & `thug-5.1/thug/conf/personalities/ipadchrome35.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome37.json` & `thug-5.1/thug/conf/personalities/ipadchrome37.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome38.json` & `thug-5.1/thug/conf/personalities/ipadchrome38.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome39.json` & `thug-5.1/thug/conf/personalities/ipadchrome39.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome45.json` & `thug-5.1/thug/conf/personalities/ipadchrome45.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome46.json` & `thug-5.1/thug/conf/personalities/ipadchrome46.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadchrome47.json` & `thug-5.1/thug/conf/personalities/ipadchrome47.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadsafari7.json` & `thug-5.1/thug/conf/personalities/ipadsafari7.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadsafari8.json` & `thug-5.1/thug/conf/personalities/ipadsafari8.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/ipadsafari9.json` & `thug-5.1/thug/conf/personalities/ipadsafari9.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/linuxchrome26.json` & `thug-5.1/thug/conf/personalities/linuxchrome26.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/linuxchrome30.json` & `thug-5.1/thug/conf/personalities/linuxchrome30.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/linuxchrome44.json` & `thug-5.1/thug/conf/personalities/linuxchrome44.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/linuxchrome54.json` & `thug-5.1/thug/conf/personalities/linuxchrome54.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/linuxchrome98.json` & `thug-5.1/thug/conf/personalities/linuxchrome98.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/linuxfirefox19.json` & `thug-5.1/thug/conf/personalities/linuxfirefox19.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/linuxfirefox40.json` & `thug-5.1/thug/conf/personalities/linuxfirefox40.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/nexuschrome18.json` & `thug-5.1/thug/conf/personalities/nexuschrome18.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/osx10chrome19.json` & `thug-5.1/thug/conf/personalities/osx10chrome19.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/osx10chrome80.json` & `thug-5.1/thug/conf/personalities/osx10chrome80.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/osx10chrome97.json` & `thug-5.1/thug/conf/personalities/osx10chrome97.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/osx10safari5.json` & `thug-5.1/thug/conf/personalities/osx10safari5.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/osx11safari14.json` & `thug-5.1/thug/conf/personalities/osx11safari14.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win10edge20.json.review` & `thug-5.1/thug/conf/personalities/win10edge20.json.review`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win10ie110.json` & `thug-5.1/thug/conf/personalities/win10ie110.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win2kie60.json` & `thug-5.1/thug/conf/personalities/win2kie60.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win2kie80.json` & `thug-5.1/thug/conf/personalities/win2kie80.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7chrome20.json` & `thug-5.1/thug/conf/personalities/win7chrome20.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7chrome40.json` & `thug-5.1/thug/conf/personalities/win7chrome40.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7chrome45.json` & `thug-5.1/thug/conf/personalities/win7chrome45.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7chrome49.json` & `thug-5.1/thug/conf/personalities/win7chrome49.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7firefox3.json` & `thug-5.1/thug/conf/personalities/win7firefox3.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7ie100.json` & `thug-5.1/thug/conf/personalities/win7ie100.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7ie80.json` & `thug-5.1/thug/conf/personalities/win7ie80.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7ie90.json` & `thug-5.1/thug/conf/personalities/win7ie90.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/win7safari5.json` & `thug-5.1/thug/conf/personalities/win7safari5.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/winxpchrome20.json` & `thug-5.1/thug/conf/personalities/winxpchrome20.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/winxpfirefox12.json` & `thug-5.1/thug/conf/personalities/winxpfirefox12.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/winxpie60.json` & `thug-5.1/thug/conf/personalities/winxpie60.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/winxpie61.json` & `thug-5.1/thug/conf/personalities/winxpie61.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/winxpie70.json` & `thug-5.1/thug/conf/personalities/winxpie70.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/winxpie80.json` & `thug-5.1/thug/conf/personalities/winxpie80.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/personalities/winxpsafari5.json` & `thug-5.1/thug/conf/personalities/winxpsafari5.json`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/blackhole.yar` & `thug-5.1/thug/conf/rules/urlclassifier/blackhole.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/crimeboss.yar` & `thug-5.1/thug/conf/rules/urlclassifier/crimeboss.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/critxpack.yar` & `thug-5.1/thug/conf/rules/urlclassifier/critxpack.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/fiesta.yar` & `thug-5.1/thug/conf/rules/urlclassifier/fiesta.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/g01pack.yar` & `thug-5.1/thug/conf/rules/urlclassifier/g01pack.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/neutrino.yar` & `thug-5.1/thug/conf/rules/urlclassifier/neutrino.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/nuclear.yar` & `thug-5.1/thug/conf/rules/urlclassifier/nuclear.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/popads.yar` & `thug-5.1/thug/conf/rules/urlclassifier/popads.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/redkit.yar` & `thug-5.1/thug/conf/rules/urlclassifier/redkit.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/styx.yar` & `thug-5.1/thug/conf/rules/urlclassifier/styx.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/rules/urlclassifier/sweetorange.yar` & `thug-5.1/thug/conf/rules/urlclassifier/sweetorange.yar`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/conf/scripts/thug.js` & `thug-5.1/thug/conf/scripts/thug.js`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug/thug.egg-info/PKG-INFO` & `thug-5.1/thug.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 4.5
+Version: 5.1
 Summary: Low-interaction honeyclient Thug
-Home-page: http://buffer.github.io/thug/
-Download-URL: https://github.com/buffer/thug/
-Author: Angelo Dell'Aera
-Author-email: angelo.dellaera@honeynet.org
+Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
+Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
-Project-URL: Docs, https://thug-honeyclient.readthedocs.io/en/latest/
-Project-URL: Bugs, https://github.com/buffer/thug/issues
-Project-URL: Funding, https://buffer.github.io/thug/
-Platform: Linux
-Platform: Darwin
+Project-URL: homepage, https://github.com/buffer/thug
+Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
+Project-URL: bugs, https://github.com/buffer/thug/issues
+Project-URL: funding, https://buffer.github.io/thug/
+Keywords: honeyclient,low-interaction,client-honeypot,security-tools
+Platform: linux
+Platform: darwin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
-Requires-Python: <4,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Thug
 ====
 
-|version badge| |github badge| |lgtm badge| |codefactor badge| |codecov badge| |bandit badge|
+|version badge| |github badge| |codefactor badge| |codecov badge| |bandit badge|
 
 The number of client-side attacks has grown significantly in the past few years
 shifting focus on poorly protected vulnerable clients. Just as the most known
 honeypot technologies enable research into server-side attacks, honeyclients
 allow the study of client-side attacks.
 
 A complement to honeypots, a honeyclient is a tool designed to mimic the behavior
@@ -81,25 +81,23 @@
 
     pytest --cov thug
 
 
 License information
 -------------------
 
-Copyright (C) 2011-2022 Angelo Dell'Aera <angelo.dellaera@honeynet.org>
+Copyright (C) 2011-2023 Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 
 License: GNU General Public License, version 2
 
 
 .. |version badge| image:: https://img.shields.io/pypi/v/thug.svg
    :target: https://pypi.python.org/pypi/thug/
 .. |github badge| image:: https://github.com/buffer/thug/workflows/Build/badge.svg
    :target: https://github.com/buffer/thug
-.. |lgtm badge| image:: https://img.shields.io/lgtm/grade/python/g/buffer/thug.svg?logo=lgtm&logoWidth=18
-   :target: https://lgtm.com/projects/g/buffer/thug
 .. |codefactor badge| image:: https://www.codefactor.io/repository/github/buffer/thug/badge
    :target: https://www.codefactor.io/repository/github/buffer/thug
 .. |codecov badge| image:: https://codecov.io/gh/buffer/thug/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/buffer/thug
 .. |bandit badge| image:: https://img.shields.io/badge/security-bandit-yellow.svg
    :target: https://github.com/PyCQA/bandit
 .. |docs badge| image:: https://readthedocs.org/projects/thug-honeyclient/badge/?version=latest
```

### Comparing `thug-5.0.1/thug/thug.py` & `thug-5.1/thug/thug.py`

 * *Files identical despite different names*

### Comparing `thug-5.0.1/thug.egg-info/SOURCES.txt` & `thug-5.1/thug.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 setup.py
+thug/.DS_Store
 thug/__init__.py
 thug/thug.py
 thug.egg-info/PKG-INFO
 thug.egg-info/SOURCES.txt
 thug.egg-info/dependency_links.txt
 thug.egg-info/entry_points.txt
 thug.egg-info/requires.txt
@@ -345,14 +346,15 @@
 thug/ThugAPI/Watchdog.py
 thug/ThugAPI/__init__.py
 thug/ThugAPI/abstractmethod.py
 thug/WebTracking/Cookies.py
 thug/WebTracking/WebStorage.py
 thug/WebTracking/WebTracking.py
 thug/WebTracking/__init__.py
+thug/conf/.DS_Store
 thug/conf/inspector.json
 thug/conf/thug.conf
 thug/conf/hooks/README
 thug/conf/personalities/galaxy2chrome18.json
 thug/conf/personalities/galaxy2chrome25.json
 thug/conf/personalities/galaxy2chrome29.json
 thug/conf/personalities/ipadchrome33.json
@@ -451,15 +453,8 @@
 thug/conf/rules/vbsclassifier/README
 thug/conf/rules/vbsfilter/README
 thug/conf/scripts/date.js
 thug/conf/scripts/eval.js
 thug/conf/scripts/message-event.js
 thug/conf/scripts/storage.js
 thug/conf/scripts/thug.js
-thug/conf/scripts/write.js
-thug/thug.egg-info/PKG-INFO
-thug/thug.egg-info/SOURCES.txt
-thug/thug.egg-info/dependency_links.txt
-thug/thug.egg-info/entry_points.txt
-thug/thug.egg-info/requires.txt
-thug/thug.egg-info/top_level.txt
-thug/thug.egg-info/zip-safe
+thug/conf/scripts/write.js
```

