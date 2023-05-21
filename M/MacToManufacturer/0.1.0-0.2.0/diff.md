# Comparing `tmp/MacToManufacturer-0.1.0.tar.gz` & `tmp/MacToManufacturer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MacToManufacturer-0.1.0.tar", last modified: Thu Oct 27 03:03:35 2022, max compression
+gzip compressed data, was "MacToManufacturer-0.2.0.tar", last modified: Sun May 21 20:36:41 2023, max compression
```

## Comparing `MacToManufacturer-0.1.0.tar` & `MacToManufacturer-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 03:03:35.085099 MacToManufacturer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-10-27 03:03:35.085099 MacToManufacturer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-10-27 03:03:25.000000 MacToManufacturer-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 03:03:35.085099 MacToManufacturer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-10-27 03:03:25.000000 MacToManufacturer-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 03:03:35.077098 MacToManufacturer-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 03:03:35.081099 MacToManufacturer-0.1.0/src/MacToManufacturer/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-27 03:03:25.000000 MacToManufacturer-0.1.0/src/MacToManufacturer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 03:03:35.081099 MacToManufacturer-0.1.0/src/MacToManufacturer/data/
--rw-r--r--   0 runner    (1001) docker     (121)  2133397 2022-10-27 03:03:26.000000 MacToManufacturer-0.1.0/src/MacToManufacturer/data/manuf.csv
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-10-27 03:03:26.000000 MacToManufacturer-0.1.0/src/MacToManufacturer/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 03:03:35.081099 MacToManufacturer-0.1.0/src/MacToManufacturer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-10-27 03:03:34.000000 MacToManufacturer-0.1.0/src/MacToManufacturer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-27 03:03:35.000000 MacToManufacturer-0.1.0/src/MacToManufacturer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 03:03:34.000000 MacToManufacturer-0.1.0/src/MacToManufacturer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-27 03:03:34.000000 MacToManufacturer-0.1.0/src/MacToManufacturer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:36:41.118493 MacToManufacturer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 20:36:35.000000 MacToManufacturer-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-21 20:36:41.118493 MacToManufacturer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-21 20:36:35.000000 MacToManufacturer-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 20:36:41.118493 MacToManufacturer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-21 20:36:35.000000 MacToManufacturer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:36:41.114493 MacToManufacturer-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:36:41.114493 MacToManufacturer-0.2.0/src/MacToManufacturer/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 20:36:35.000000 MacToManufacturer-0.2.0/src/MacToManufacturer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:36:41.114493 MacToManufacturer-0.2.0/src/MacToManufacturer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2215514 2023-05-21 20:36:35.000000 MacToManufacturer-0.2.0/src/MacToManufacturer/data/manuf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-21 20:36:35.000000 MacToManufacturer-0.2.0/src/MacToManufacturer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:36:41.114493 MacToManufacturer-0.2.0/src/MacToManufacturer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-21 20:36:41.000000 MacToManufacturer-0.2.0/src/MacToManufacturer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-21 20:36:41.000000 MacToManufacturer-0.2.0/src/MacToManufacturer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:36:41.000000 MacToManufacturer-0.2.0/src/MacToManufacturer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 20:36:41.000000 MacToManufacturer-0.2.0/src/MacToManufacturer.egg-info/top_level.txt
```

### Comparing `MacToManufacturer-0.1.0/README.md` & `MacToManufacturer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `MacToManufacturer-0.1.0/setup.py` & `MacToManufacturer-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MacToManufacturer",
-    version="0.1.0",
+    version="0.2.0",
     author="Nishant Bhandari",
     author_email="getrooted0019@hotmail.com",
     description="Library to find manufacturer of a device using macaddress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/n1snt/MacToManufacturer",
     project_urls={
```

### Comparing `MacToManufacturer-0.1.0/src/MacToManufacturer/data/manuf.csv` & `MacToManufacturer-0.2.0/src/MacToManufacturer/data/manuf.csv`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
 00:01:40,Sendtek Sendtek Corporation
 00:01:41,CablePri Cable Print
 00:01:42,"Cisco Cisco Systems, Inc"
 00:01:43,Ieee802  IEEE 802
 00:01:44,DellEMC Dell EMC
 00:01:45,"Winsyste Winsystems, Inc."
 00:01:46,"TescoCon Tesco Controls, Inc."
-00:01:47,ZhoneTec Zhone Technologies
+00:01:47,DZS DZS Inc.
 00:01:48,X-traWeb X-traWeb Inc.
 00:01:49,Tdt Tdt Ag
 00:01:4A,Sony Sony Corporation
 00:01:4B,"Ennovate Ennovate Networks, Inc."
 00:01:4C,Berkeley Berkeley Process Control
 00:01:4D,"ShinKinE Shin Kin Enterprises Co., Ltd"
 00:01:4E,"WINEnter WIN Enterprises, Inc."
@@ -619,15 +619,15 @@
 00:02:6A,"CocessTe Cocess Telecom Co., Ltd."
 00:02:6B,"BCMCompu BCM Computers Co., Ltd."
 00:02:6C,PhilipsC Philips CFT
 00:02:6D,AdeptTel Adept Telecom
 00:02:6E,"NeGeNAcc NeGeN Access, Inc."
 00:02:6F,"SenaoInt Senao International Co., Ltd."
 00:02:70,"Crewave Crewave Co., Ltd."
-00:02:71,ZhoneTec Zhone Technologies
+00:02:71,DZS DZS Inc.
 00:02:72,"CC&CTech CC&C Technologies, Inc."
 00:02:73,Coriolis Coriolis Networks
 00:02:74,TommyTec Tommy Technologies Corp.
 00:02:75,"SMARTTec SMART Technologies, Inc."
 00:02:76,PrimaxEl Primax Electronics Ltd.
 00:02:77,CashSyst Cash Systemes Industrie
 00:02:78,"SamsungE Samsung Electro Mechanics Co., Ltd."
@@ -843,20 +843,20 @@
 00:03:4A,RIAS RIAS Corporation
 00:03:4B,NortelNe Nortel Networks
 00:03:4C,"Shanghai Shanghai DigiVision Technology Co., Ltd."
 00:03:4D,"ChiaroNe Chiaro Networks, Ltd."
 00:03:4E,"PosData Pos Data Company, Ltd."
 00:03:4F,Sur-Gard Sur-Gard Security
 00:03:50,Bticino Bticino Spa
-00:03:51,"Diebold Diebold, Inc."
+00:03:51,DieboldN Diebold Nixdorf
 00:03:52,Colubris Colubris Networks
 00:03:53,"Mitac Mitac, Inc."
 00:03:54,FiberLog Fiber Logic Communications
 00:03:55,TeraBeam TeraBeam Internet Systems
-00:03:56,WincorNi Wincor Nixdorf International GmbH
+00:03:56,DieboldN Diebold Nixdorf
 00:03:57,"Intervoi Intervoice-Brite, Inc."
 00:03:58,HanyangD Hanyang Digitech Co.Ltd
 00:03:59,DigitalS DigitalSis
 00:03:5A,Photron Photron Limited
 00:03:5B,BridgeWa BridgeWave Communications
 00:03:5C,SaintSon Saint Song Corp.
 00:03:5D,"BosungHi Bosung Hi-Net Co., Ltd."
@@ -2200,15 +2200,15 @@
 00:08:B2,"Shenzhen Shenzhen Compass Technology Development Co.,Ltd"
 00:08:B3,Fastwel
 00:08:B4,Syspol
 00:08:B5,"TaiGuenE Tai Guen Enterprise Co., Ltd"
 00:08:B6,"RouteFre RouteFree, Inc."
 00:08:B7,HIT HIT Incorporated
 00:08:B8,EFJohnso E.F. Johnson
-00:08:B9,"Kaonmedi Kaonmedia CO., LTD."
+00:08:B9,"KaonGrou Kaon Group Co., Ltd."
 00:08:BA,Erskine Erskine Systems Ltd
 00:08:BB,NetExcel NetExcell
 00:08:BC,Ilevo Ilevo AB
 00:08:BD,Tepg-Us
 00:08:BE,XENPAKMS XENPAK MSA Group
 00:08:BF,AptusEle Aptus Elektronik AB
 00:08:C0,Asa Asa Systems
@@ -3274,15 +3274,15 @@
 00:0C:E5,"ARRISGro ARRIS Group, Inc."
 00:0C:E6,"Fortinet Fortinet, Inc."
 00:0C:E7,MediaTek MediaTek Inc.
 00:0C:E8,"GuangZho GuangZhou AnJuBao Co., Ltd"
 00:0C:E9,Bloomber Bloomberg L.P.
 00:0C:EA,aphonaKo aphona Kommunikationssysteme
 00:0C:EB,"CNMPNetw CNMP Networks, Inc."
-00:0C:EC,OroliaUS Orolia USA
+00:0C:EC,SafranTr Safran Trusted 4D Inc.
 00:0C:ED,RealDigi Real Digital Media
 00:0C:EE,jp-embed jp-embedded
 00:0C:EF,OpenNetw Open Networks Engineering Ltd
 00:0C:F0,MN M & N GmbH
 00:0C:F1,Intel Intel Corporation
 00:0C:F2,GAMESAEó GAMESA Eólica
 00:0C:F3,CallImag Call Image Sa
@@ -3351,15 +3351,15 @@
 00:0D:32,"Dispense DispenseSource, Inc."
 00:0D:33,Prediwav Prediwave Corp.
 00:0D:34,"ShellInt Shell International Exploration and Production, Inc."
 00:0D:35,PACInter PAC International Ltd
 00:0D:36,"WuHanRou Wu Han Routon Electronic Co., Ltd"
 00:0D:37,Wiplug
 00:0D:38,Nissin Nissin Inc.
-00:0D:39,NetworkE Network Electronics
+00:0D:39,Nevion
 00:0D:3A,Microsof Microsoft Corp.
 00:0D:3B,Microele Microelectronics Technology Inc.
 00:0D:3C,iTechDyn i.Tech Dynamic Ltd
 00:0D:3D,"Hammerhe Hammerhead Systems, Inc."
 00:0D:3E,APLUXCom APLUX Communications Ltd.
 00:0D:3F,VTIInstr VTI Instruments Corporation
 00:0D:40,VerintLo Verint Loronix Video Solutions
@@ -3631,15 +3631,15 @@
 00:0E:4A,"Changchu Changchun Huayu WEBPAD Co.,LTD"
 00:0E:4B,atriumca atrium c and i
 00:0E:4C,Bermai Bermai Inc.
 00:0E:4D,Numesa Numesa Inc.
 00:0E:4E,"Waveplus Waveplus Technology Co., Ltd."
 00:0E:4F,Trajet Trajet GmbH
 00:0E:50,ThomsonT Thomson Telecom Belgium
-00:0E:51,tecnaele tecna elettronica srl
+00:0E:51,TECNA TECNA SpA
 00:0E:52,Optium Optium Corporation
 00:0E:53,AvTech Av Tech Corporation
 00:0E:54,AlphaCel AlphaCell Wireless Ltd.
 00:0E:55,Auvitran
 00:0E:56,4G 4G Systems GmbH & Co. KG
 00:0E:57,"IworldNe Iworld Networking, Inc."
 00:0E:58,"Sonos Sonos, Inc."
@@ -4487,15 +4487,15 @@
 00:11:A2,Manufact Manufacturing Technology Inc
 00:11:A3,LanReady LanReady Technologies Inc.
 00:11:A4,JStreamT JStream Technologies Inc.
 00:11:A5,FortunaE Fortuna Electronic Corp.
 00:11:A6,SypixxNe Sypixx Networks
 00:11:A7,InfilcoD Infilco Degremont Inc.
 00:11:A8,QuestTec Quest Technologies
-00:11:A9,"MOIMSTON MOIMSTONE Co., LTD"
+00:11:A9,"Nurivoic Nurivoice Co., Ltd"
 00:11:AA,"Uniclass Uniclass Technology, Co., LTD"
 00:11:AB,"Trustabl Trustable Technology Co.,Ltd."
 00:11:AC,SimtecEl Simtec Electronics
 00:11:AD,Shanghai Shanghai Ruijie Technology
 00:11:AE,"ARRISGro ARRIS Group, Inc."
 00:11:AF,"Medialin Medialink-i,Inc"
 00:11:B0,Fortelin Fortelink Inc.
@@ -5173,15 +5173,15 @@
 00:14:50,Heim Heim Systems GmbH
 00:14:51,"Apple Apple, Inc."
 00:14:52,"Calculex Calculex,Inc."
 00:14:53,"Advantec Advantech Technologies Co.,Ltd"
 00:14:54,Symwave
 00:14:55,CoderEle Coder Electronics Corporation
 00:14:56,EdgeProd Edge Products
-00:14:57,T-VipsAs T-Vips As
+00:14:57,Nevion
 00:14:58,HSAutoma HS Automatic ApS
 00:14:59,"Moram Moram Co., Ltd."
 00:14:5A,Westermo Westermo Neratec AG
 00:14:5B,SeekerNe SeekerNet Inc.
 00:14:5C,Intronic Intronics B.V.
 00:14:5D,"WJCommun WJ Communications, Inc."
 00:14:5E,IBM IBM Corp
@@ -5231,15 +5231,15 @@
 00:14:8A,ElinEbgT Elin Ebg Traction Gmbh
 00:14:8B,GloboEle Globo Electronic GmbH & Co. KG
 00:14:8C,GeneralD General Dynamics Mission Systems
 00:14:8D,CubicDef Cubic Defense Simulation Systems
 00:14:8E,TelePowe Tele Power Inc.
 00:14:8F,Protroni Protronic (Far East) Ltd.
 00:14:90,ASP ASP Corporation
-00:14:91,DanielsE Daniels Electronics Ltd. dbo Codan Rado Communications
+00:14:91,DanielsE Daniels Electronics Ltd. dba Codan Radio Communications
 00:14:92,"LiteonMo Liteon, Mobile Media Solution SBU"
 00:14:93,Systimax Systimax Solutions
 00:14:94,Esu Esu Ag
 00:14:95,2Wire 2Wire Inc
 00:14:96,Phonic Phonic Corp.
 00:14:97,"ZHIYUANE ZHIYUAN Eletronics co.,ltd."
 00:14:98,VikingDe Viking Design Technology
@@ -5451,15 +5451,15 @@
 00:15:66,"A-FirstT A-First Technology Co., Ltd."
 00:15:67,RADWIN RADWIN Inc.
 00:15:68,Dilithiu Dilithium Networks
 00:15:69,"PECOII PECO II, Inc."
 00:15:6A,DG2LTech DG2L Technologies Pvt. Ltd.
 00:15:6B,Perfisan Perfisans Networks Corp.
 00:15:6C,"SaneSyst Sane System Co., Ltd"
-00:15:6D,Ubiquiti Ubiquiti Networks Inc.
+00:15:6D,Ubiquiti Ubiquiti Inc
 00:15:6E,AWCommun A. W. Communication Systems Ltd
 00:15:6F,XiranetC Xiranet Communications GmbH
 00:15:70,ZebraTec Zebra Technologies Inc
 00:15:71,Nolan Nolan Systems
 00:15:72,Red-Lemo Red-Lemon
 00:15:73,NewSoftT NewSoft Technology Corporation
 00:15:74,HorizonS Horizon Semiconductors Ltd.
@@ -5620,15 +5620,15 @@
 00:16:0F,BadgerMe Badger Meter Inc
 00:16:10,CarinaTe Carina Technology
 00:16:11,Altecon Altecon Srl
 00:16:12,"OtsukaEl Otsuka Electronics Co., Ltd."
 00:16:13,LibreStr LibreStream Technologies Inc.
 00:16:14,Picoseco Picosecond Pulse Labs
 00:16:15,"Nittan Nittan Company, Limited"
-00:16:16,BrowanCo Browan Communication Inc.
+00:16:16,BrowanCo Browan Communications Incorporation
 00:16:17,Msi
 00:16:18,"HIVION HIVION Co., Ltd."
 00:16:19,Lancelan Lancelan Technologies S.L.
 00:16:1A,Dametric Dametric AB
 00:16:1B,Micronet Micronet Corporation
 00:16:1C,ecue e:cue
 00:16:1D,"Innovati Innovative Wireless Technologies, Inc."
@@ -5844,15 +5844,15 @@
 00:16:EF,"KokoFitn Koko Fitness, Inc."
 00:16:F0,Dell
 00:16:F1,"OmniSens OmniSense, LLC"
 00:16:F2,"DmobileS Dmobile System Co., Ltd."
 00:16:F3,"CASTInfo CAST Information Co., Ltd"
 00:16:F4,"Eidicom Eidicom Co., Ltd."
 00:16:F5,"DalianGo Dalian Golden Hualu Digital Technology Co.,Ltd"
-00:16:F6,VideoPro Video Products Group
+00:16:F6,Nevion
 00:16:F7,"L-3Commu L-3 Communications, Aviation Recorders"
 00:16:F8,"Aviqtech Aviqtech Technology Co., Ltd."
 00:16:F9,"CETRTAPO CETRTA POT, d.o.o., Kranj"
 00:16:FA,ECITelec ECI Telecom Ltd.
 00:16:FB,Shenzhen Shenzhen Mtc Co Ltd
 00:16:FC,"Tohken Tohken Co.,Ltd."
 00:16:FD,JatyElec Jaty Electronics
@@ -6122,15 +6122,15 @@
 00:18:05,"BeijingI Beijing InHand Networking Technology Co.,Ltd."
 00:18:06,"HokkeiIn Hokkei Industries Co., Ltd."
 00:18:07,Fanstel Fanstel Corp.
 00:18:08,"SightLog SightLogix, Inc."
 00:18:09,Cresyn
 00:18:0A,CiscoMer Cisco Meraki
 00:18:0B,Brillian Brilliant Telecommunications
-00:18:0C,Optelian Optelian Access Networks
+00:18:0C,DZS DZS Inc.
 00:18:0D,Terabyte Terabytes Server Storage Tech Corp
 00:18:0E,Avega Avega Systems
 00:18:0F,NokiaDan Nokia Danmark A/S
 00:18:10,IPTrade IPTrade S.A.
 00:18:11,"NeurosTe Neuros Technology International, LLC."
 00:18:12,"BeijingX Beijing Xinwei Telecom Technology Co., Ltd."
 00:18:13,Sony Sony Corporation
@@ -6138,15 +6138,15 @@
 00:18:15,"GZTechno GZ Technologies, Inc."
 00:18:16,"Ubixon Ubixon Co., Ltd."
 00:18:17,"DEShawRe D. E. Shaw Research, LLC"
 00:18:18,"Cisco Cisco Systems, Inc"
 00:18:19,"Cisco Cisco Systems, Inc"
 00:18:1A,AVerMedi AVerMedia Information Inc.
 00:18:1B,"TaiJinMe TaiJin Metal Co., Ltd."
-00:18:1C,Exterity Exterity Limited
+00:18:1C,Vitec
 00:18:1D,"AsiaElec Asia Electronics Co.,Ltd"
 00:18:1E,GDXTechn GDX Technologies Ltd.
 00:18:1F,Palmmicr Palmmicro Communications
 00:18:20,w5networ w5networks
 00:18:21,Sindoric Sindoricoh
 00:18:22,"CecTelec Cec Telecom Co.,Ltd."
 00:18:23,"DeltaEle Delta Electronics, Inc."
@@ -6283,15 +6283,15 @@
 00:18:A6,"Persiste Persistent Systems, LLC"
 00:18:A7,YoggieSe Yoggie Security Systems LTD.
 00:18:A8,AnNealTe AnNeal Technology Inc.
 00:18:A9,Ethernet Ethernet Direct Corporation
 00:18:AA,ProtecFi Protec Fire Detection plc
 00:18:AB,BeijingL Beijing Lhwt Microelectronics Inc.
 00:18:AC,Shanghai Shanghai Jiao Da HISYS Technology Co. Ltd.
-00:18:AD,NidecSan Nidec Sankyo Corporation
+00:18:AD,NidecIns Nidec Instruments Corporation
 00:18:AE,"Tvt Tvt Co.,Ltd"
 00:18:AF,"SamsungE Samsung Electronics Co.,Ltd"
 00:18:B0,NortelNe Nortel Networks
 00:18:B1,IBM IBM Corp
 00:18:B2,AdeunisR Adeunis Rf
 00:18:B3,"TECWizHo TEC WizHome Co., Ltd."
 00:18:B4,DawonMed Dawon Media Inc.
@@ -6496,15 +6496,15 @@
 00:19:7B,Picotest Picotest Corp.
 00:19:7C,RiedelCo Riedel Communications GmbH
 00:19:7D,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 00:19:7E,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 00:19:7F,"Plantron Plantronics, Inc."
 00:19:80,Gridpoin Gridpoint Systems
 00:19:81,Vivox Vivox Inc
-00:19:82,SmarDTV
+00:19:82,SmarDTV SmarDTV Corporation
 00:19:83,CCTR&D CCT R&D Limited
 00:19:84,ESTIC ESTIC Corporation
 00:19:85,"ITWatchd IT Watchdogs, Inc"
 00:19:86,ChengHon Cheng Hongjian
 00:19:87,"Panasoni Panasonic Mobile Communications Co.,Ltd."
 00:19:88,"Wi2Wi Wi2Wi, Inc"
 00:19:89,Sonitrol Sonitrol Corporation
@@ -6606,15 +6606,15 @@
 00:19:E9,"S-Inform S-Information Technolgy, Co., Ltd."
 00:19:EA,"TeraMage TeraMage Technologies Co., Ltd."
 00:19:EB,Pyronix Pyronix Ltd
 00:19:EC,"Sagamore Sagamore Systems, Inc."
 00:19:ED,Axesstel Axesstel Inc.
 00:19:EE,CARLOGAV CARLO GAVAZZI CONTROLS SPA-Controls Division
 00:19:EF,"Shenzhen Shenzhen Linnking Electronics Co.,Ltd"
-00:19:F0,"Unionman Unionman Technology Co.,Ltd"
+00:19:F0,"UnionMan Union Man Technology Co.,Ltd"
 00:19:F1,"StarComm Star Communication Network Technology Co.,Ltd"
 00:19:F2,Teradyne Teradyne K.K.
 00:19:F3,"Cetis Cetis, Inc"
 00:19:F4,Converge Convergens Oy Ltd
 00:19:F5,Imaginat Imagination Technologies Ltd
 00:19:F6,AcconetP Acconet (PTE) Ltd
 00:19:F7,OnsetCom Onset Computer Corporation
@@ -6788,15 +6788,15 @@
 00:1A:9F,A-Link A-Link Ltd
 00:1A:A0,Dell Dell Inc.
 00:1A:A1,"Cisco Cisco Systems, Inc"
 00:1A:A2,"Cisco Cisco Systems, Inc"
 00:1A:A3,Delorme
 00:1A:A4,FutureUn Future University-Hakodate
 00:1A:A5,BRNPhoen BRN Phoenix
-00:1A:A6,Telefunk Telefunken Radio Communication Systems GmbH &CO.KG
+00:1A:A6,ElbitDeu Elbit Systems Deutschland GmbH & Co. KG
 00:1A:A7,TorianWi Torian Wireless
 00:1A:A8,"MamiyaDi Mamiya Digital Imaging Co., Ltd."
 00:1A:A9,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 00:1A:AA,Analogic Analogic Corp.
 00:1A:AB,eWings eWings s.r.l.
 00:1A:AC,Corelatu Corelatus AB
 00:1A:AD,"ARRISGro ARRIS Group, Inc."
@@ -6909,15 +6909,15 @@
 00:1B:18,"TsukenEl Tsuken Electric Ind. Co.,Ltd"
 00:1B:19,IEEEI&MS IEEE I&M Society TC9
 00:1B:1A,"e-treesJ e-trees Japan, Inc."
 00:1B:1B,"Siemens Siemens AG,"
 00:1B:1C,Coherent
 00:1B:1D,"PhoenixI Phoenix International Co., Ltd"
 00:1B:1E,HARTComm HART Communication Foundation
-00:1B:1F,"DELTA-Da DELTA - Danish Electronics, Light & Acoustics"
+00:1B:1F,FORCETec FORCE Technology
 00:1B:20,TPineTec TPine Technology
 00:1B:21,IntelCor Intel Corporate
 00:1B:22,PalitMic Palit Microsystems ( H.K.) Ltd.
 00:1B:23,SimpleCo SimpleComTools
 00:1B:24,QuantaCo Quanta Computer Inc.
 00:1B:25,NortelNe Nortel Networks
 00:1B:26,RON-Tele RON-Telecom ZAO
@@ -8611,15 +8611,15 @@
 00:20:F5,Pandatel Pandatel Ag
 00:20:F6,NetTekKa Net Tek & Karlnet Inc
 00:20:F7,Cyberdat Cyberdata Corporation
 00:20:F8,"CarreraC Carrera Computers, Inc."
 00:20:F9,"Paralink Paralink Networks, Inc."
 00:20:FA,"Gde Gde Systems, Inc."
 00:20:FB,OctelCom Octel Communications Corp.
-00:20:FC,Matrox
+00:20:FC,MatroxCe Matrox Central Services Inc
 00:20:FD,"ItvTechn Itv Technologies, Inc."
 00:20:FE,TopwareG Topware Inc. / Grand Computer
 00:20:FF,Symmetri Symmetrical Technologies
 00:21:00,"GemtekTe Gemtek Technology Co., Ltd."
 00:21:01,Aplicaci Aplicaciones Electronicas Quasar (AEQ)
 00:21:02,UpdateLo UpdateLogic Inc.
 00:21:03,"GHIElect GHI Electronics, LLC"
@@ -9326,15 +9326,15 @@
 00:23:C0,Broadway Broadway Networks
 00:23:C1,Securita Securitas Direct AB
 00:23:C2,SAMSUNGE SAMSUNG Electronics. Co. LTD
 00:23:C3,"LogMeIn LogMeIn, Inc."
 00:23:C4,LuxLumen Lux Lumen
 00:23:C5,Radiatio Radiation Safety and Control Services Inc
 00:23:C6,SMC SMC Corporation
-00:23:C7,AVSystem
+00:23:C7,AVSystem AVSystem sp. z o. o.
 00:23:C8,Team-R
 00:23:C9,"SichuanT Sichuan Tianyi Information Science & Technology Stock CO.,LTD"
 00:23:CA,"BehindSe Behind The Set, LLC"
 00:23:CB,"Shenzhen Shenzhen Full-join Technology Co.,Ltd"
 00:23:CC,"Nintendo Nintendo Co., Ltd."
 00:23:CD,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 00:23:CE,KitaDens Kita Denshi Corporation
@@ -10177,26 +10177,27 @@
 00:27:1B,AlecSich Alec Sicherheitssysteme GmbH
 00:27:1C,Mercury Mercury Corporation
 00:27:1D,CombaTel Comba Telecom Systems (China) Ltd.
 00:27:1E,XagylCom Xagyl Communications
 00:27:1F,"MIPROEle MIPRO Electronics Co., Ltd"
 00:27:20,New-SolC New-Sol Com
 00:27:21,"Shenzhen Shenzhen Baoan Fenda Industrial Co., Ltd"
-00:27:22,Ubiquiti Ubiquiti Networks Inc.
+00:27:22,Ubiquiti Ubiquiti Inc
 00:27:90,"Cisco Cisco Systems, Inc"
 00:27:E3,"Cisco Cisco Systems, Inc"
 00:27:F8,BrocadeC Brocade Communications Systems LLC
 00:28:9F,"Semptian Semptian Co., Ltd."
 00:28:F8,IntelCor Intel Corporate
 00:29:26,"AppliedO Applied Optoelectronics, Inc Taiwan Branch"
 00:29:C2,"Cisco Cisco Systems, Inc"
 00:2A:10,"Cisco Cisco Systems, Inc"
 00:2A:6A,"Cisco Cisco Systems, Inc"
 00:2A:AF,LARsys-A LARsys-Automation GmbH
 00:2B:67,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
+00:2B:F5,Buffalo Buffalo.Inc
 00:2C:C8,"Cisco Cisco Systems, Inc"
 00:2D:76,TITECH TITECH GmbH
 00:2D:B3,"AMPAKTec AMPAK Technology,Inc."
 00:2E:C7,"HuaweiTe Huawei Technologies Co.,Ltd"
 00:2F:5C,"Cisco Cisco Systems, Inc"
 00:2F:D9,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 00:30:00,AllwellT Allwell Technology Corp.
@@ -10238,15 +10239,15 @@
 00:30:24,"Cisco Cisco Systems, Inc"
 00:30:25,"Checkout Checkout Computer Systems, Ltd"
 00:30:26,HeiTelDi HeiTel Digital Video GmbH
 00:30:27,"Kerbango Kerbango, Inc."
 00:30:28,FASESald FASE Saldatura srl
 00:30:29,Opicom
 00:30:2A,Southern Southern Information
-00:30:2B,"InalpNet Inalp Networks, Inc."
+00:30:2B,InalpSol Inalp Solutions AG
 00:30:2C,Sylantro Sylantro Systems Corporation
 00:30:2D,QuantumB Quantum Bridge Communications
 00:30:2E,HoftWess Hoft & Wessel AG
 00:30:2F,GEAviati GE Aviation System
 00:30:30,Harmonix Harmonix Corporation
 00:30:31,"Lightwav Lightwave Communications, Inc."
 00:30:32,"MagicRam MagicRam, Inc."
@@ -10277,15 +10278,15 @@
 00:30:4B,"Orbacom Orbacom Systems, Inc."
 00:30:4C,"AppianCo Appian Communications, Inc."
 00:30:4D,Esi
 00:30:4E,BustecPr Bustec Production Ltd.
 00:30:4F,PLANETTe PLANET Technology Corporation
 00:30:50,VersaTec Versa Technology
 00:30:51,OrbitAvi Orbit Avionic & Communication
-00:30:52,ElasticN Elastic Networks
+00:30:52,DZS DZS Inc.
 00:30:53,Basler Basler AG
 00:30:54,Castlene Castlenet Technology Inc.
 00:30:55,"RenesasT Renesas Technology America, Inc."
 00:30:56,HMSIndus HMS Industrial Networks
 00:30:57,"QTelNet QTelNet, Inc."
 00:30:58,ApiMotio Api Motion
 00:30:59,KontronE Kontron Europe GmbH
@@ -10467,19 +10468,21 @@
 00:34:FE,"HuaweiTe Huawei Technologies Co.,Ltd"
 00:35:1A,"Cisco Cisco Systems, Inc"
 00:35:32,Electro- Electro-Metrics Corporation
 00:35:60,RosenAvi Rosen Aviation
 00:35:FF,TexasIns Texas Instruments
 00:36:76,"ARRISGro ARRIS Group, Inc."
 00:36:BE,Northwes Northwest Towers
+00:36:D7,KeltronI Keltron IOT Corp.
 00:36:F8,ContiTem Conti Temic microelectronic GmbH
 00:36:FE,SuperVis SuperVision
 00:37:6D,"MurataMa Murata Manufacturing Co., Ltd."
 00:37:B7,Sagemcom Sagemcom Broadband SAS
 00:38:DF,"Cisco Cisco Systems, Inc"
+00:39:69,Air-Weig Air-Weigh Incorporated
 00:3A:7D,"Cisco Cisco Systems, Inc"
 00:3A:98,"Cisco Cisco Systems, Inc"
 00:3A:99,"Cisco Cisco Systems, Inc"
 00:3A:9A,"Cisco Cisco Systems, Inc"
 00:3A:9B,"Cisco Cisco Systems, Inc"
 00:3A:9C,"Cisco Cisco Systems, Inc"
 00:3A:9D,"NECPlatf NEC Platforms, Ltd."
@@ -11711,15 +11714,15 @@
 00:50:C2:2F:30:00/36,"Crossbow Crossbow Technology, Inc."
 00:50:C2:2F:40:00/36,Efficien Efficient Channel Coding
 00:50:C2:2F:50:00/36,ADChips
 00:50:C2:2F:60:00/36,Clifford Clifford Chance LLP
 00:50:C2:2F:70:00/36,Gillam-F Gillam-Fei S.A.
 00:50:C2:2F:80:00/36,SavvyCor SavvyCorp.com Ltd
 00:50:C2:2F:90:00/36,Digilent Digilent Inc.
-00:50:C2:2F:A0:00/36,"TornadoM Tornado Modular Systems, Ltd"
+00:50:C2:2F:A0:00/36,TornadoM Tornado Modular Systems
 00:50:C2:2F:B0:00/36,"ArthurIn Arthur Industries Inc., dba On Hold Media Group"
 00:50:C2:2F:C0:00/36,Blacklin Blackline Systems Corporation
 00:50:C2:2F:D0:00/36,"American American Microsystems, Ltd."
 00:50:C2:2F:E0:00/36,Saab Saab AB
 00:50:C2:2F:F0:00/36,PatriaAd Patria Advanced Solutions
 00:50:C2:30:00:00/36,SoredexI Soredex Instrumentarium Oyj
 00:50:C2:30:10:00/36,"DelphiDi Delphi Display Systems, Inc."
@@ -11937,15 +11940,15 @@
 00:50:C2:3D:50:00/36,"FlukeBio Fluke Biomedical, Radiation Management Services"
 00:50:C2:3D:60:00/36,Comlab Comlab Inc.
 00:50:C2:3D:70:00/36,TTCTELEK TTC TELEKOMUNIKACE Ltd
 00:50:C2:3D:80:00/36,"Key Key Systems , Inc."
 00:50:C2:3D:90:00/36,BavariaD Bavaria Digital Technik GmbH
 00:50:C2:3D:A0:00/36,M5Data M5 Data Limited
 00:50:C2:3D:B0:00/36,Osmetech Osmetech Inc.
-00:50:C2:3D:C0:00/36,3Dpercep 3D perception
+00:50:C2:3D:C0:00/36,3Dpercep 3D perception AS
 00:50:C2:3D:D0:00/36,ELMIC ELMIC GmbH
 00:50:C2:3D:E0:00/36,ABBPower ABB Power Technologies S.p.A. Unità Operativa SACE (PTMV)
 00:50:C2:3D:F0:00/36,BiODE BiODE Inc.
 00:50:C2:3E:00:00/36,Stinghor Oy Stinghorn Ltd
 00:50:C2:3E:10:00/36,NeuLion NeuLion Incorporated
 00:50:C2:3E:20:00/36,SysNova
 00:50:C2:3E:30:00/36,CSIRO-Di CSIRO - Division of Exploration and Mining
@@ -11960,15 +11963,15 @@
 00:50:C2:3E:C0:00/36,Teneros
 00:50:C2:3E:D0:00/36,BoardRoo The Board Room Inc.
 00:50:C2:3E:E0:00/36,"Commoca Commoca, Inc"
 00:50:C2:3E:F0:00/36,"PATIndus PAT Industries, DBA Pacific Advanced Technology"
 00:50:C2:3F:00:00/36,megatece megatec electronic GmbH
 00:50:C2:3F:10:00/36,SallandE Salland Electronics Holding BV
 00:50:C2:3F:20:00/36,STL STL GmbH
-00:50:C2:3F:30:00/36,HitachiE Hitachi Energy
+00:50:C2:3F:30:00/36,HitachiE Hitachi Energy Germany AG
 00:50:C2:3F:40:00/36,MCTECHNO MC TECHNOLOGY GmbH
 00:50:C2:3F:50:00/36,Phaedrus Phaedrus Limited
 00:50:C2:3F:60:00/36,dAFTdATA dAFTdATA Limited
 00:50:C2:3F:70:00/36,Advantag Advantage R&D
 00:50:C2:3F:80:00/36,Superna Superna Ltd
 00:50:C2:3F:90:00/36,Sintium Sintium Ltd
 00:50:C2:3F:A0:00/36,Tumsan
@@ -12078,15 +12081,15 @@
 00:50:C2:46:20:00/36,CT CT Company
 00:50:C2:46:30:00/36,"Codem Codem Systems, Inc."
 00:50:C2:46:40:00/36,XYTACsys XYTAC system technologies
 00:50:C2:46:50:00/36,PDTS PDTS GmbH
 00:50:C2:46:60:00/36,LONAP LONAP Limited
 00:50:C2:46:70:00/36,UnitedWe United Western Technologies
 00:50:C2:46:80:00/36,NetworkI Network I/O
-00:50:C2:46:90:00/36,"BiPOMEle BiPOM Electronics, Inc."
+00:50:C2:46:90:00/36,"BipomEle Bipom Electronics, Inc."
 00:50:C2:46:A0:00/36,ISE ISE GmbH
 00:50:C2:46:B0:00/36,EASYTECH EASYTECH GmbH
 00:50:C2:46:C0:00/36,CAMCO CAMCO GmbH
 00:50:C2:46:D0:00/36,PaulSche Paul Scherrer Institut (PSI)
 00:50:C2:46:E0:00/36,AvenirTe Avenir Technologies Inc.
 00:50:C2:46:F0:00/36,Neurowar Neuroware
 00:50:C2:47:00:00/36,Cybectec Cybectec inc.
@@ -12622,15 +12625,15 @@
 00:50:C2:68:20:00/36,Commet Commet AB
 00:50:C2:68:30:00/36,MEGGITTS MEGGITT Safety System
 00:50:C2:68:40:00/36,REASONTe REASON Tecnologia S.A.
 00:50:C2:68:50:00/36,Datamars Datamars SA
 00:50:C2:68:60:00/36,ANNAXAnz ANNAX Anzeigesysteme GmbH
 00:50:C2:68:70:00/36,"AccessSp Access Specialties, Inc"
 00:50:C2:68:80:00/36,ElkProdu Elk Products
-00:50:C2:68:90:00/36,"RFCode RF Code, Inc."
+00:50:C2:68:90:00/36,RFCode RF Code
 00:50:C2:68:A0:00/36,"ZhuhaiJi Zhuhai Jiahe Electronics Co.,LTD"
 00:50:C2:68:B0:00/36,Simtek Simtek Inc.
 00:50:C2:68:C0:00/36,Isochron Isochron Inc
 00:50:C2:68:D0:00/36,CXRLarus CXR Larus Corporation
 00:50:C2:68:E0:00/36,Selco
 00:50:C2:68:F0:00/36,Bertroni Bertronic Srl
 00:50:C2:69:00:00/36,GHLBerha GHL Systems Berhad
@@ -13312,15 +13315,15 @@
 00:50:C2:93:40:00/36,Xilar Xilar Corp.
 00:50:C2:93:50:00/36,ImageVid Image Video
 00:50:C2:93:60:00/36,Margarit Margaritis Engineering
 00:50:C2:93:70:00/36,BigBear
 00:50:C2:93:80:00/36,PostecDa Postec Data Systems Ltd
 00:50:C2:93:90:00/36,MosaicDy Mosaic Dynamic Solutions
 00:50:C2:93:A0:00/36,ALPHATRO ALPHATRONICS nv
-00:50:C2:93:B0:00/36,Reliatro Reliatronics Inc.
+00:50:C2:93:B0:00/36,"Cleavela Cleaveland/Price, Inc."
 00:50:C2:93:C0:00/36,Fracture FractureCode Corporation
 00:50:C2:93:D0:00/36,Lighting Lighting Science Group
 00:50:C2:93:E0:00/36,RCSCommu RCS Communication Test Systems Ltd.
 00:50:C2:93:F0:00/36,TSBSolut TSB Solutions Inc.
 00:50:C2:94:00:00/36,Phitek Phitek Systems Ltd.
 00:50:C2:94:10:00/36,Rolbit
 00:50:C2:94:20:00/36,KeithKoe Keith & Koep GmbH
@@ -13769,15 +13772,15 @@
 00:50:C2:AF:D0:00/36,"HomeScen HomeScenario, Inc."
 00:50:C2:AF:E0:00/36,Trolex Trolex Limited
 00:50:C2:AF:F0:00/36,XoByte XoByte LLC
 00:50:C2:B0:00:00/36,Saia-Bur Saia-Burgess Controls AG
 00:50:C2:B0:10:00/36,HSRHaral HSR Harald L. Reuter
 00:50:C2:B0:20:00/36,Master Master Co Ltd
 00:50:C2:B0:30:00/36,SpiderTe Spider Tecnologia Ind. e Com. Ltda.
-00:50:C2:B0:40:00/36,Ubiquiti Ubiquiti Networks Inc.
+00:50:C2:B0:40:00/36,Ubiquiti Ubiquiti Inc
 00:50:C2:B0:50:00/36,POLA POLA s.r.l.
 00:50:C2:B0:60:00/36,"CompuDes CompuDesigns, Inc."
 00:50:C2:B0:70:00/36,Fareco
 00:50:C2:B0:80:00/36,Goerlitz Goerlitz AG
 00:50:C2:B0:90:00/36,HarperCh Harper Chalice Group Limited
 00:50:C2:B0:A0:00/36,Induther Indutherm Giesstechnologie GmbH
 00:50:C2:B0:B0:00/36,Honeywel Honeywell
@@ -13856,15 +13859,15 @@
 00:50:C2:B5:40:00/36,"APGCashD APG Cash Drawer, LLC"
 00:50:C2:B5:50:00/36,"SanyoEle Sanyo Electronic Industries Co.,Ltd"
 00:50:C2:B5:60:00/36,Sinovia Sinovia Sa
 00:50:C2:B5:70:00/36,PhytecMe Phytec Messtechnik GmbH
 00:50:C2:B5:80:00/36,"RealD RealD, Inc."
 00:50:C2:B5:90:00/36,SLICANsp SLICAN sp. z o.o.
 00:50:C2:B5:A0:00/36,GREENCen GREEN Center s.r.o.
-00:50:C2:B5:B0:00/36,Timberli Timberline Mfg Company
+00:50:C2:B5:B0:00/36,Timberli Timberline Manufacturing
 00:50:C2:B5:C0:00/36,ADIVideo ADI Video Technologies
 00:50:C2:B5:D0:00/36,PlitronM Plitron Manufacturing Inc.
 00:50:C2:B5:E0:00/36,"Palgiken Palgiken Co.,Ltd."
 00:50:C2:B5:F0:00/36,NorthBri North Bridge Technologies
 00:50:C2:B6:00:00/36,NpfAtis Ooo Npf Atis
 00:50:C2:B6:10:00/36,Nayos Nayos LTD
 00:50:C2:B6:20:00/36,Measurem Measurement Technology NW
@@ -13993,15 +13996,15 @@
 00:50:C2:BD:E0:00/36,Evo-Tehd Evo-Teh d.o.o.
 00:50:C2:BD:F0:00/36,Euro-Kon Euro-Konsult Sp. z o.o.
 00:50:C2:BE:00:00/36,Phaedrus Phaedrus Limited
 00:50:C2:BE:10:00/36,Tattile Tattile srl
 00:50:C2:BE:20:00/36,Converge Convergent Bioscience Ltd.
 00:50:C2:BE:30:00/36,Jiskoot Jiskoot Ltd
 00:50:C2:BE:40:00/36,GrupoEpe Grupo Epelsa S.L.
-00:50:C2:BE:50:00/36,"RFCode RF Code, Inc"
+00:50:C2:BE:50:00/36,RFCode RF Code
 00:50:C2:BE:60:00/36,Docobo Docobo Ltd
 00:50:C2:BE:70:00/36,Genetec Genetec Inc.
 00:50:C2:BE:80:00/36,"VehicleT Vehicle Testing Equipment, S.L."
 00:50:C2:BE:90:00/36,Zucchett Zucchetti Spa
 00:50:C2:BE:A0:00/36,Daeyoung Daeyoung inc.
 00:50:C2:BE:B0:00/36,PeekTraf Peek Traffic Corporation
 00:50:C2:BE:C0:00/36,DRSLarue DRS Laruel Technologies
@@ -14451,15 +14454,15 @@
 00:50:C2:DA:A0:00/36,"MPaul M & Paul, Inc"
 00:50:C2:DA:B0:00/36,AplexTec Aplex Technology Inc.
 00:50:C2:DA:C0:00/36,"RFLElect RFL Electronics, Inc."
 00:50:C2:DA:D0:00/36,KeithKoe Keith & Koep GmbH
 00:50:C2:DA:E0:00/36,SpangPow Spang Power Electronics
 00:50:C2:DA:F0:00/36,eumigind eumig industrie-tv GmbH
 00:50:C2:DB:00:00/36,IMAGOTec IMAGO Technologies GmbH
-00:50:C2:DB:10:00/36,"RFCode RF Code, Inc"
+00:50:C2:DB:10:00/36,RFCode RF Code
 00:50:C2:DB:20:00/36,Software SoftwareCannery
 00:50:C2:DB:30:00/36,LaudaDrR Lauda Dr. R. Wobser Gmbh & Co. Kg
 00:50:C2:DB:40:00/36,"NPCKompj ZAO NPC ""Kompjuternie Technologii"""
 00:50:C2:DB:50:00/36,DspDesig Dsp Design Ltd
 00:50:C2:DB:60:00/36,Prosoft Prosoft-Systems Ltd
 00:50:C2:DB:70:00/36,SORELMik SOREL GmbH Mikroelektronik
 00:50:C2:DB:80:00/36,ComsatVe Comsat VertriebsgmbH
@@ -14897,15 +14900,15 @@
 00:50:C2:F6:A0:00/36,OFIdba2D OFI Inc. (dba 2D2C)
 00:50:C2:F6:B0:00/36,AlgodueE Algodue Elettronica Srl
 00:50:C2:F6:C0:00/36,ProDesig Pro Design Electronic GmbH
 00:50:C2:F6:D0:00/36,ProDesig Pro Design Electronic GmbH
 00:50:C2:F6:E0:00/36,"SmithMet Smith Meter, Inc."
 00:50:C2:F6:F0:00/36,AplexTec Aplex Technology Inc.
 00:50:C2:F7:00:00/36,NoraltaT Noralta Technologies Inc
-00:50:C2:F7:10:00/36,"RFCode RF Code, Inc"
+00:50:C2:F7:10:00/36,RFCode RF Code
 00:50:C2:F7:20:00/36,MaxDeTec MaxDeTec AG
 00:50:C2:F7:30:00/36,Deltacas Deltacast.Tv
 00:50:C2:F7:40:00/36,ThorTech Thor Technologies Pty Ltd
 00:50:C2:F7:50:00/36,PumpWell PumpWell Solutions Ltd.
 00:50:C2:F7:60:00/36,"RongJieF Rong Jie(FuZhou)Electronics Co.,Ltd"
 00:50:C2:F7:70:00/36,SYSTEMTE SYSTEMTECHNIK GmbH
 00:50:C2:F7:80:00/36,GetsMSS Gets MSS S.A.
@@ -15045,15 +15048,15 @@
 00:50:C2:FF:F0:00/36,MSR-Solu MSR-Solutions GmbH
 00:50:C4,Imd
 00:50:C5,"ADSTechn ADS Technologies, Inc"
 00:50:C6,"LoopTele Loop Telecommunication International, Inc."
 00:50:C7,Private
 00:50:C8,"Addonics Addonics Technologies, Inc."
 00:50:C9,MasproDe Maspro Denkoh Corp.
-00:50:CA,NetToNet Net To Net Technologies
+00:50:CA,DZS DZS Inc.
 00:50:CB,Jetter
 00:50:CC,SeagateC Seagate Cloud Systems Inc
 00:50:CD,Digiansw Digianswer A/S
 00:50:CE,LgIntern Lg International Corp.
 00:50:CF,VanlinkC Vanlink Communication Technology Research Institute
 00:50:D0,Minerva Minerva Systems
 00:50:D1,"Cisco Cisco Systems, Inc"
@@ -15122,17 +15125,19 @@
 00:55:DA:A0:00:00/28,Speechla Speechlab
 00:55:DA:B0:00:00/28,Interaxo Interaxon Inc
 00:55:DA:C0:00:00/28,"DonguanW Donguan WideLink Communication Technology Co.,Ltd."
 00:55:DA:D0:00:00/28,"ArrowEle Arrow Electronics,Inc."
 00:55:DA:E0:00:00/28,Victorsu Victorsure Limited
 00:55:DA:F0:00:00/28,Private
 00:56:2B,"Cisco Cisco Systems, Inc"
+00:56:6D,"HuaweiDe Huawei Device Co., Ltd."
 00:56:CD,"Apple Apple, Inc."
 00:57:C1,LGElectr LG Electronics (Mobile Communications)
 00:57:D2,"Cisco Cisco Systems, Inc"
+00:58:28,AxonNetw Axon Networks Inc.
 00:58:3F,PCAquari PC Aquarius
 00:59:07,"LenovoEM LenovoEMC Products USA, LLC"
 00:59:79,Networke Networked Energy Services
 00:59:AC,Kpn Kpn. B.V.
 00:59:DC,"Cisco Cisco Systems, Inc"
 00:5A:13,"HuaweiTe Huawei Technologies Co.,Ltd"
 00:5A:39,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
@@ -15407,14 +15412,15 @@
 00:61:71,"Apple Apple, Inc."
 00:62:0B,Broadcom Broadcom Limited
 00:62:EC,"Cisco Cisco Systems, Inc"
 00:63:DE,"Cloudwal Cloudwalk Technology Co.,Ltd"
 00:64:40,"Cisco Cisco Systems, Inc"
 00:64:A6,MaquetCa Maquet CardioVascular
 00:64:AF,DishTech Dish Technologies Corp
+00:65:1E,AmcrestT Amcrest Technologies
 00:66:19,"HuaweiDe Huawei Device Co., Ltd."
 00:66:4B,"HuaweiTe Huawei Technologies Co.,Ltd"
 00:67:62,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 00:68:2B,"HuaweiDe Huawei Device Co., Ltd."
 00:68:EB,HP HP Inc.
 00:69:2D,SunnovoI Sunnovo International Limited
 00:69:67,IEEERegi IEEE Registration Authority
@@ -15654,15 +15660,15 @@
 00:80:B1,Softcom Softcom A/S
 00:80:B2,NetNetwo NET (Network Equipment Technologies)
 00:80:B3,AvalData Aval Data Corporation
 00:80:B4,Sophia Sophia Systems
 00:80:B5,UnitedNe United Networks Inc.
 00:80:B6,Themis  Themis corporation
 00:80:B7,StellarC Stellar Computer
-00:80:B8,"DmgMoriB Dmg Mori B.U.G. Co., Ltd."
+00:80:B8,"DMGMORID DMG MORI Digital Co., LTD"
 00:80:B9,ArcheTec Arche Technoligies Inc.
 00:80:BA,"Speciali Specialix (Asia) Pte, Ltd"
 00:80:BB,HughesLa Hughes Lan Systems
 00:80:BC,"HitachiE Hitachi Engineering Co., Ltd"
 00:80:BD,"Furukawa The Furukawa Electric Co., Ltd"
 00:80:BE,AriesRes Aries Research
 00:80:BF,TakaokaE Takaoka Electric Mfg. Co. Ltd.
@@ -16010,14 +16016,15 @@
 00:90:FE,"ElecomLa Elecom Co., Ltd. (Laneed Div.)"
 00:90:FF,TellusTe Tellus Technology Inc.
 00:91:9E,IntelCor Intel Corporate
 00:91:D6,"CrystalG Crystal Group, Inc."
 00:91:EB,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 00:91:FA,SynapseP Synapse Product Development
 00:92:7D,"FicosaIn Ficosa Internationa(Taicang) C0.,Ltd."
+00:92:A5,LGInnote LG Innotek
 00:92:FA,"Shenzhen Shenzhen Wisky Technology Co.,Ltd"
 00:93:37,IntelCor Intel Corporate
 00:93:63,"Uni-Link Uni-Link Technology Co., Ltd."
 00:94:A1,"F5Networ F5 Networks, Inc."
 00:94:EC,"HuaweiDe Huawei Device Co., Ltd."
 00:95:69,"LSDScien LSD Science and Technology Co.,Ltd."
 00:97:FF,HeimannS Heimann Sensor GmbH
@@ -16053,15 +16060,15 @@
 00:A0:14,Csir
 00:A0:15,Wyle
 00:A0:16,Micropol Micropolis Corp.
 00:A0:17,JBM J B M Corporation
 00:A0:18,"Creative Creative Controllers, Inc."
 00:A0:19,"NebulaCo Nebula Consultants, Inc."
 00:A0:1A,BinarEle Binar Elektronik Ab
-00:A0:1B,"Premisys Premisys Communications, Inc."
+00:A0:1B,DZS DZS Inc.
 00:A0:1C,NascentN Nascent Networks Corporation
 00:A0:1D,"RedLionC Red Lion Controls, LP"
 00:A0:1E,Est Est Corporation
 00:A0:1F,"Tricord Tricord Systems, Inc."
 00:A0:20,Citicorp Citicorp/Tti
 00:A0:21,GeneralD General Dynamics Mission Systems
 00:A0:22,CentreFo Centre For Development Of Advanced Computing
@@ -16239,15 +16246,15 @@
 00:A0:CE,Ecessa
 00:A0:CF,"Sotas Sotas, Inc."
 00:A0:D0,"TenXTech Ten X Technology, Inc."
 00:A0:D1,Inventec Inventec Corporation
 00:A0:D2,AlliedTe Allied Telesyn
 00:A0:D3,"InstemCo Instem Computer Systems, Ltd."
 00:A0:D4,"Radiolan Radiolan, Inc."
-00:A0:D5,SierraWi Sierra Wireless
+00:A0:D5,"SierraWi Sierra Wireless, ULC"
 00:A0:D6,"SBE SBE, Inc."
 00:A0:D7,KastenCh Kasten Chase Applied Research
 00:A0:D8,Spectra- Spectra - Tek
 00:A0:D9,ConvexCo Convex Computer Corporation
 00:A0:DA,"INTEGRAT INTEGRATED SYSTEMS Technology, Inc."
 00:A0:DB,FisherPa Fisher & Paykel Production
 00:A0:DC,"ONElectr O.N. Electronic Co., Ltd."
@@ -16450,15 +16457,15 @@
 00:C0:33,Telebit  Telebit Corporation
 00:C0:34,Transact Transaction Network
 00:C0:35,Quintar Quintar Company
 00:C0:36,RaytechE Raytech Electronic Corp.
 00:C0:37,Dynatem
 00:C0:38,RasterIm Raster Image Processing System
 00:C0:39,Teridian Teridian Semiconductor Corporation
-00:C0:3A,Men-Mikr Men-Mikro Elektronik Gmbh
+00:C0:3A,duagonGe duagon Germany GmbH
 00:C0:3B,Multiacc Multiaccess Computing Corp.
 00:C0:3C,TowerTec Tower Tech S.R.L.
 00:C0:3D,Wieseman Wiesemann & Theis Gmbh
 00:C0:3E,FaGebrHe Fa. Gebr. Heller Gmbh
 00:C0:3F,"StoresAu Stores Automated Systems, Inc."
 00:C0:40,Ecci
 00:C0:41,DigitalT Digital Transmission Systems
@@ -16660,19 +16667,20 @@
 00:C3:0A,XiaomiCo Xiaomi Communications Co Ltd
 00:C3:43,E-T-ACir E-T-A Circuit Breakers Ltd
 00:C3:F4,"SamsungE Samsung Electronics Co.,Ltd"
 00:C5:2C,JuniperN Juniper Networks
 00:C5:85,"Apple Apple, Inc."
 00:C5:DB,Datatech Datatech Sistemas Digitales Avanzados SL
 00:C6:10,"Apple Apple, Inc."
+00:C7:11,ItelMobi Itel Mobile Limited
 00:C8:8B,"Cisco Cisco Systems, Inc"
 00:CA:E5,"Cisco Cisco Systems, Inc"
 00:CB:00,Private
 00:CB:51,Sagemcom Sagemcom Broadband SAS
-00:CB:7A,Technico Technicolor CH USA Inc.
+00:CB:7A,VantivaU Vantiva USA LLC
 00:CB:B4,"Shenzhen Shenzhen Ateko Photoelectricity Co.,Ltd"
 00:CB:BD,Cambridg Cambridge Broadband Networks Group
 00:CC:34,JuniperN Juniper Networks
 00:CC:3F,"Universa Universal Electronics, Inc."
 00:CC:FC,"Cisco Cisco Systems, Inc"
 00:CD:90,MASElekt MAS Elektronik AG
 00:CD:FE,"Apple Apple, Inc."
@@ -16799,15 +16807,15 @@
 00:D0:75,"AlarisMe Alaris Medical Systems, Inc."
 00:D0:76,BankAmer Bank of America
 00:D0:77,LucentTe Lucent Technologies
 00:D0:78,EltexSwe Eltex of Sweden AB
 00:D0:79,"Cisco Cisco Systems, Inc"
 00:D0:7A,Amaquest Amaquest Computer Corp.
 00:D0:7B,ComcamIn Comcam International Inc
-00:D0:7C,"KoyoElec Koyo Electronics Inc. Co.,Ltd."
+00:D0:7C,JtektEle Jtekt Electronics Corporation
 00:D0:7D,CosineCo Cosine Communications
 00:D0:7E,Keycorp Keycorp Ltd.
 00:D0:7F,"Strategy Strategy & Technology, Limited"
 00:D0:80,Exabyte Exabyte Corporation
 00:D0:81,"RTDEmbed RTD Embedded Technologies, Inc."
 00:D0:82,Iowave Iowave Inc.
 00:D0:83,"Invertex Invertex, Inc."
@@ -16998,15 +17006,15 @@
 00:E0:15,Heiwa Heiwa Corporation
 00:E0:16,Rapid-Ci rapid-city (now a part of bay networks)
 00:E0:17,EXXACT EXXACT GmbH
 00:E0:18,AsustekI Asustek
 00:E0:19,IngGiord Ing. Giordano Elettronica
 00:E0:1A,"Comtec Comtec Systems. Co., Ltd."
 00:E0:1B,"SphereCo Sphere Communications, Inc."
-00:E0:1C,"Cradlepo Cradlepoint, Inc"
+00:E0:1C,"CradlePo CradlePoint, Inc"
 00:E0:1D,"WebTVNET WebTV NETWORKS, INC."
 00:E0:1E,"Cisco Cisco Systems, Inc"
 00:E0:1F,"AVIDIA AVIDIA Systems, Inc."
 00:E0:20,Tecnomen Tecnomen Oy
 00:E0:21,Freegate Freegate Corp.
 00:E0:22,"AnalogDe Analog Devices, Inc."
 00:E0:23,Telrad
@@ -17193,15 +17201,15 @@
 00:E0:D8,"LANBitCo LANBit Computer, Inc."
 00:E0:D9,"Tazmo Tazmo Co., Ltd."
 00:E0:DA,Alcatel- Alcatel-Lucent Enterprise
 00:E0:DB,"ViaVideo ViaVideo Communications, Inc."
 00:E0:DC,Nexware Nexware Corp.
 00:E0:DD,ZenithEl Zenith Electronics Corporation
 00:E0:DE,Datax Datax Nv
-00:E0:DF,DZS DZS GmbH
+00:E0:DF,DZS DZS Inc.
 00:E0:E0,"SiElectr Si Electronics, Ltd."
 00:E0:E1,"G2Networ G2 Networks, Inc."
 00:E0:E2,Innova Innova Corp.
 00:E0:E3,Sk-Elekt Sk-Elektronik Gmbh
 00:E0:E4,"FANUCROB FANUC ROBOTICS NORTH AMERICA, Inc."
 00:E0:E5,"CincoNet Cinco Networks, Inc."
 00:E0:E6,INCAACom INCAA Computers
@@ -17236,26 +17244,29 @@
 00:E2:2C,"ChinaMob China Mobile Group Device Co.,Ltd."
 00:E3:B2,"SamsungE Samsung Electronics Co.,Ltd"
 00:E4:00,SichuanC Sichuan Changhong Electric Ltd.
 00:E4:06,"HuaweiTe Huawei Technologies Co.,Ltd"
 00:E4:21,SonyInte Sony Interactive Entertainment Inc.
 00:E5:E4,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 00:E5:F1,Buffalo Buffalo.Inc
+00:E6:0E,"ExtremeN Extreme Networks, Inc."
+00:E6:3A,RuckusWi Ruckus Wireless
 00:E6:66,ARIMACom ARIMA Communications Corp.
 00:E6:D3,NixdorfC Nixdorf Computer Corp.
 00:E6:E8,"NetzinTe Netzin Technology Corporation,.Ltd."
 00:E7:E3,zte zte corporation
 00:E8:AB,"MeggittT Meggitt Training Systems, Inc."
 00:E9:3A,AzureWav AzureWave Technology Inc.
 00:EA:BD,"Cisco Cisco Systems, Inc"
 00:EB:2D,Sony Sony Corporation
 00:EB:D5,"Cisco Cisco Systems, Inc"
 00:EB:D8,"Mercusys Mercusys Technologies Co., Ltd."
 00:EC:0A,XiaomiCo Xiaomi Communications Co Ltd
 00:ED:B8,KYOCERA KYOCERA Corporation
+00:EE:01,Enablers Enablers Solucoes e Consultoria em Dispositivos
 00:EE:AB,"Cisco Cisco Systems, Inc"
 00:EE:BD,HTC HTC Corporation
 00:F0:51,KWB KWB Gmbh
 00:F2:2C,"Shanghai Shanghai B-star Technology Co.,Ltd."
 00:F2:8B,"Cisco Cisco Systems, Inc"
 00:F3:61,AmazonTe Amazon Technologies Inc.
 00:F3:9F,"Apple Apple, Inc."
@@ -17310,14 +17321,15 @@
 04:03:12,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 04:03:D6,"Nintendo Nintendo Co.,Ltd"
 04:04:B8,"ChinaHua China Hualu Panasonic AVC Networks Co., LTD."
 04:04:EA,ValensSe Valens Semiconductor Ltd.
 04:05:DD,"Shenzhen Shenzhen Cultraview Digital Technology Co., Ltd"
 04:07:2E,VTechEle VTech Electronics Ltd.
 04:09:73,HewlettP Hewlett Packard Enterprise
+04:09:86,Arcadyan Arcadyan Corporation
 04:09:A5,"HFR HFR, Inc."
 04:0A:83,Alcatel- Alcatel-Lucent
 04:0A:E0,XmitComp Xmit Ag Computer Networks
 04:0C:CE,"Apple Apple, Inc."
 04:0D:84,SiliconL Silicon Laboratories
 04:0E:3C,HP HP Inc.
 04:0E:C2,ViewSoni ViewSonic Mobile China Limited
@@ -17340,15 +17352,15 @@
 04:11:19:E0:00:00/28,Julida Julida Limited
 04:15:52,"Apple Apple, Inc."
 04:15:D9,Viwone
 04:17:B6,SmartInn Smart Innovation LLC
 04:18:0F,"SamsungE Samsung Electronics Co.,Ltd"
 04:18:92,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:18:B6,Private
-04:18:D6,Ubiquiti Ubiquiti Networks Inc.
+04:18:D6,Ubiquiti Ubiquiti Inc
 04:19:7F,Graspher Grasphere Japan
 04:1A:04,WaveIP
 04:1B:6D,LGElectr LG Electronics (Mobile Communications)
 04:1B:94,HostMobi Host Mobility AB
 04:1B:BA,"SamsungE Samsung Electronics Co.,Ltd"
 04:1D:10,DreamWar Dream Ware Inc.
 04:1D:C7,zte zte corporation
@@ -17370,39 +17382,44 @@
 04:29:2E,"SamsungE Samsung Electronics Co.,Ltd"
 04:2A:E2,"Cisco Cisco Systems, Inc"
 04:2B:58,"Shenzhen Shenzhen Hanzsung Technology Co.,Ltd"
 04:2B:BB,"PicoCELA PicoCELA, Inc."
 04:2D:B4,"FirstPro First Property (Beijing) Co., Ltd Modern MOMA Branch"
 04:2F:56,ATOCSShe ATOCS (Shenzhen) LTD
 04:31:10,"InspurGr Inspur Group Co., Ltd."
+04:32:01,Broadcom Broadcom Limited
 04:32:F4,Partron
 04:33:1F,"HuaweiDe Huawei Device Co., Ltd."
 04:33:85,"Nanchang Nanchang BlackShark Co.,Ltd."
 04:33:89,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:33:C2,IntelCor Intel Corporate
 04:34:F6,"Motorola Motorola (Wuhan) Mobility Technologies Communication Co., Ltd."
 04:36:04,Gyeyoung Gyeyoung I&T
+04:36:B8,I&CTechn I&C Technology
 04:38:55,ScopusIn Scopus International-Belgium
+04:38:DC,"ChinaUni China Unicom Online Information Technology Co.,Ltd"
 04:39:26,ChinaDra China Dragon Technology Limited
 04:3A:0D,SMOptics SM Optics S.r.l.
 04:3C:E8,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 04:3D:98,"ChongQin ChongQing QingJia Electronics CO.,LTD"
 04:3F:72,"Mellanox Mellanox Technologies, Inc."
 04:40:A9,"NewH3CTe New H3C Technologies Co., Ltd"
 04:41:69,GoPro
 04:42:1A,ASUSTekC ASUSTek COMPUTER INC.
 04:43:FD,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 04:44:A1,"TeleconG Telecon Galicia,S.A."
 04:45:62,ANDRASpz ANDRA Sp. z o. o.
 04:45:A1,"NIRIT-Xi NIRIT- Xinwei Telecom Technology Co., Ltd."
 04:46:65,"MurataMa Murata Manufacturing Co., Ltd."
 04:46:CF,"BeijingV Beijing Venustech Cybervision Co.,Ltd."
+04:47:2A,PaloAlto Palo Alto Networks
 04:48:9A,"Apple Apple, Inc."
 04:49:5D,"HuaweiDe Huawei Device Co., Ltd."
 04:4A:50,RamaxelT Ramaxel Technology (Shenzhen) limited company
+04:4A:6A,"niliwina niliwi nanjing big data Co,.Ltd"
 04:4A:6C,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:4A:C6,"AiponEle Aipon Electronics Co., Ltd"
 04:4B:A5,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 04:4B:ED,"Apple Apple, Inc."
 04:4B:FF,"GuangZho GuangZhou Hedy Digital Technology Co., Ltd"
 04:4C:EF,"FujianSa Fujian Sanao Technology Co.,Ltd"
 04:4E:06,Ericsson Ericsson AB
@@ -17447,14 +17464,15 @@
 04:6B:1B,"SYSDINE SYSDINE Co., Ltd."
 04:6B:25,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 04:6C:59,IntelCor Intel Corporate
 04:6C:9D,"Cisco Cisco Systems, Inc"
 04:6D:42,Bryston Bryston Ltd.
 04:6E:02,OpenRTLS OpenRTLS Group
 04:6E:49,"TaiYearE TaiYear Electronic Technology (Suzhou) Co., Ltd"
+04:70:56,Arcadyan Arcadyan Corporation
 04:70:BC,Globalst Globalstar Inc.
 04:71:4B,IEEERegi IEEE Registration Authority
 04:71:4B:00:00:00/28,NeurioTe Neurio Technology Inc.
 04:71:4B:10:00:00/28,uAvionix uAvionix Corporation
 04:71:4B:20:00:00/28,"Shenzhen Shenzhen WayOS Technology Crop., Ltd."
 04:71:4B:30:00:00/28,Griesser Griesser Electronic AG
 04:71:4B:40:00:00/28,Apparate Apparatebau Gauting GmbH
@@ -17485,18 +17503,20 @@
 04:7B:CB,"Universa Universal Global Scientific Industrial Co., Ltd."
 04:7C:16,"Micro-St Micro-Star INTL CO., LTD."
 04:7D:50,Shenzhen Shenzhen Kang Ying Technology Co.Ltd.
 04:7D:7B,QuantaCo Quanta Computer Inc.
 04:7E:23,ChinaMob China Mobile IOT Company Limited
 04:7E:4A,"moobox moobox CO., Ltd."
 04:7F:0E,"BarrotTe Barrot Technology Co.,LTD"
+04:80:A7,ShenZhen ShenZhen TianGang Micro Technology CO.LTD
 04:81:9B,SkyUk Sky Uk Limited
 04:81:AE,Clack Clack Corporation
 04:84:8A,7InovaTe 7Inova Technology Limited
 04:86:80,"QuectelW Quectel Wireless Solutions Co.,Ltd."
+04:87:27,SiliconL Silicon Laboratories
 04:88:45,BayNetwo Bay Networks
 04:88:5F,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:88:8C,Eifelwer Eifelwerk Butler Systeme GmbH
 04:88:E2,BeatsEle Beats Electronics LLC
 04:8A:15,Avaya Avaya Inc
 04:8A:E1,"Flextron Flextronics Manufacturing(Zhuhai)Co.,Ltd."
 04:8B:42,Skspruce Skspruce Technologies
@@ -17516,36 +17536,41 @@
 04:97:90,Lartecht Lartech telecom LLC
 04:98:F3,"Alpsalpi Alpsalpine Co,.Ltd"
 04:99:B9,"Apple Apple, Inc."
 04:99:BB,"Apple Apple, Inc."
 04:99:E6,"Shenzhen Shenzhen Yoostar Technology Co., Ltd"
 04:9B:9C,"Eadingco Eadingcore Intelligent Technology Co., Ltd."
 04:9C:62,BMTMedic BMT Medical Technology s.r.o.
+04:9D:05,"Apple Apple, Inc."
 04:9D:FE,Hivesyst Hivesystem
 04:9F:06,"Smobile Smobile Co., Ltd."
 04:9F:15,Humane
 04:9F:81,Netscout Netscout Systems Inc
 04:9F:CA,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:A1:51,Netgear
 04:A2:22,Arcadyan Arcadyan Corporation
 04:A2:F3,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 04:A3:16,TexasIns Texas Instruments
 04:A3:F3,Emicon
+04:A5:26,Nokia
 04:A7:41,"Cisco Cisco Systems, Inc"
+04:A8:1C,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:A8:2A,Nokia Nokia Corporation
 04:AA:E1,"BeijingM Beijing Microvision Technology Co.,Ltd"
+04:AB:08,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 04:AB:18,"Elecom Elecom Co.,Ltd."
 04:AB:6A,"Chun-il Chun-il Co.,Ltd."
 04:AC:44,HoltekSe Holtek Semiconductor Inc.
 04:B0:E7,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:B1:67,XiaomiCo Xiaomi Communications Co Ltd
 04:B1:A1,"SamsungE Samsung Electronics Co.,Ltd"
 04:B3:B6,SeamapUK Seamap (UK) Ltd
 04:B4:29,"SamsungE Samsung Electronics Co.,Ltd"
 04:B4:66,"BSP BSP Co., Ltd."
+04:B4:FE,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 04:B6:48,Zenner
 04:B6:BE,CigShang Cig Shanghai Co Ltd
 04:B8:6A,SkyUk Sky Uk Limited
 04:B9:7D,"AiVISItd AiVIS Co., Itd."
 04:B9:E3,"SamsungE Samsung Electronics Co.,Ltd"
 04:BA:1C,"HuaweiDe Huawei Device Co., Ltd."
 04:BA:36,LiSengTe Li Seng Technology Ltd
@@ -17634,14 +17659,15 @@
 04:D6:AA,SamsungE Samsung Electro-Mechanics(Thailand)
 04:D6:F4,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 04:D7:83,"Y&HE&C Y&H E&C Co.,LTD."
 04:D7:A5,"NewH3CTe New H3C Technologies Co., Ltd"
 04:D9:21,Occuspac Occuspace
 04:D9:C8,"HonHaiPr Hon Hai Precision Industry Co., Ltd."
 04:D9:F5,ASUSTekC ASUSTek COMPUTER INC.
+04:DA:28,"Chongqin Chongqing Zhouhai Intelligent Technology Co., Ltd"
 04:DA:D2,"Cisco Cisco Systems, Inc"
 04:DB:56,"Apple Apple, Inc."
 04:DB:8A,SuntechI Suntech International Ltd.
 04:DD:4C,Velocyte Velocytech
 04:DE:DB,Rockport Rockport Networks Inc
 04:DE:F2,Shenzhen Shenzhen ECOM Technology Co. Ltd
 04:DF:69,CarConne Car Connectivity Consortium
@@ -17693,14 +17719,15 @@
 04:F1:28,HMDGloba HMD Global Oy
 04:F1:3E,"Apple Apple, Inc."
 04:F1:69,"HuaweiDe Huawei Device Co., Ltd."
 04:F1:7D,TaranaWi Tarana Wireless
 04:F3:52,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:F4:BC,XenaNetw Xena Networks
 04:F5:F4,ProximWi Proxim Wireless
+04:F7:78,SonyInte Sony Interactive Entertainment Inc.
 04:F7:E4,"Apple Apple, Inc."
 04:F8:C2,"Flaircom Flaircomm Microelectronics, Inc."
 04:F8:F8,Edgecore Edgecore Networks Corporation
 04:F9:38,"HuaweiTe Huawei Technologies Co.,Ltd"
 04:F9:93,Infinixm Infinix mobility limited
 04:F9:D9,"SpeakerE Speaker Electronic(Jiashan) Co.,Ltd"
 04:F9:F8,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
@@ -17855,14 +17882,15 @@
 08:00:8F,Chipcom Chipcom Corporation
 08:00:90,Sonoma Sonoma Systems
 08:01:0F,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 08:02:05,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:02:8E,Netgear
 08:03:42,PaloAlto Palo Alto Networks
 08:03:71,KrgCorpo Krg Corporate
+08:04:B4,TexasIns Texas Instruments
 08:05:81,"Roku Roku, Inc."
 08:05:CD,DongGuan DongGuang EnMai Electronic Product Co.Ltd.
 08:05:E2,JuniperN Juniper Networks
 08:08:5C,LunaProd Luna Products
 08:08:C2,"SamsungE Samsung Electronics Co.,Ltd"
 08:08:EA,Amsc
 08:09:B6,Masimo Masimo Corp
@@ -17875,14 +17903,15 @@
 08:0F:FA,Ksp Ksp Inc.
 08:10:86,"NECPlatf NEC Platforms, Ltd."
 08:11:5E,"Bitel Bitel Co., Ltd."
 08:11:96,IntelCor Intel Corporate
 08:12:A5,AmazonTe Amazon Technologies Inc.
 08:14:43,Unibrain Unibrain S.A.
 08:15:2F,"SamsungE Samsung Electronics Co., Ltd. ARTIK"
+08:15:AE,"ChinaMob China Mobile Group Device Co.,Ltd."
 08:16:05,Vodafone Vodafone Italia S.p.A.
 08:16:51,"Shenzhen Shenzhen Sea Star Technology Co.,Ltd"
 08:16:D5,Goertek Goertek Inc.
 08:17:35,"Cisco Cisco Systems, Inc"
 08:17:F4,IBM IBM Corp
 08:18:1A,zte zte corporation
 08:18:4C,"Thomas A. S. Thomas, Inc."
@@ -17894,14 +17923,15 @@
 08:1D:FB,"Shanghai Shanghai Mexon Communication Technology Co.,Ltd"
 08:1F:3F,WondaLin WondaLink Inc.
 08:1F:71,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 08:1F:EB,BinCube
 08:1F:F3,"Cisco Cisco Systems, Inc"
 08:21:EF,"SamsungE Samsung Electronics Co.,Ltd"
 08:23:B2,"vivoMobi vivo Mobile Communication Co., Ltd."
+08:23:C6,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:25:22,Advansee
 08:25:25,XiaomiCo Xiaomi Communications Co Ltd
 08:25:73,"Apple Apple, Inc."
 08:26:97,ZyxelCom Zyxel Communications Corporation
 08:26:AE,IEEERegi IEEE Registration Authority
 08:26:AE:00:00:00/28,"WuhanTia Wuhan Tianyu Information Industry Co., Ltd."
 08:26:AE:10:00:00/28,"BeijingS Beijing Silion Technology Corp.,Ltd."
@@ -17916,25 +17946,27 @@
 08:26:AE:A0:00:00/28,Flextron Flextronics International Kft
 08:26:AE:B0:00:00/28,F-PlusMo F-Plus Mobile LLC
 08:26:AE:C0:00:00/28,Brannstr Brannstrom Sweden AB
 08:26:AE:D0:00:00/28,VethProp Veth Propulsion bv
 08:26:AE:E0:00:00/28,MassElec Mass Electronics Pty Ltd
 08:27:19,APSelect APS systems/electronic AG
 08:27:CE,"NaganoKe Nagano Keiki Co., Ltd."
+08:28:02,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 08:2A:D0,SRDInnov SRD Innovations Inc.
 08:2C:B0,NetworkI Network Instruments
 08:2C:B6,"Apple Apple, Inc."
 08:2C:ED,Technity Technity Solutions Inc.
 08:2E:36,"HuaweiDe Huawei Device Co., Ltd."
 08:2E:5F,HewlettP Hewlett Packard
 08:2F:E9,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:30:6B,PaloAlto Palo Alto Networks
 08:30:CE,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 08:31:8B,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:31:A4,"HuaweiDe Huawei Device Co., Ltd."
+08:33:ED,AskeyCom Askey Computer Corp
 08:35:1B,"Shenzhen Shenzhen Jialihua Electronic Technology Co., Ltd"
 08:35:71,CASwell CASwell INC.
 08:35:B2,"CoreEdge CoreEdge Networks Co., Ltd"
 08:36:C9,Netgear
 08:37:3D,"SamsungE Samsung Electronics Co.,Ltd"
 08:37:9C,Topaz Topaz Co. LTD.
 08:38:69,HongKong Hong Kong AMobile Intelligent Corp. Limited Taiwan Branch
@@ -17952,14 +17984,15 @@
 08:3E:5D,Sagemcom Sagemcom Broadband SAS
 08:3E:8E,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 08:3F:3E,WSH WSH GmbH
 08:3F:76,"Intellia Intellian Technologies, Inc."
 08:3F:BC,zte zte corporation
 08:40:27,Gridstor Gridstore Inc.
 08:40:F3,"TendaTec Tenda Technology Co.,Ltd.Dongguan branch"
+08:42:18,Asyril Asyril SA
 08:42:96,MobileTe Mobile Technology Solutions LLC
 08:45:D1,"Cisco Cisco Systems, Inc"
 08:46:56,Veo-Labs
 08:46:C7,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 08:47:4C,Nokia
 08:47:D0,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 08:48:2C,"RaycoreT Raycore Taiwan Co., LTD."
@@ -18006,31 +18039,33 @@
 08:6B:D1,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 08:6B:D7,SiliconL Silicon Laboratories
 08:6D:41,"Apple Apple, Inc."
 08:6D:F2,"Shenzhen Shenzhen MIMOWAVE Technology Co.,Ltd"
 08:6E:9C,"HuaweiDe Huawei Device Co., Ltd."
 08:6F:48,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 08:70:45,"Apple Apple, Inc."
+08:70:73,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:71:90,IntelCor Intel Corporate
 08:74:02,"Apple Apple, Inc."
+08:74:58,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 08:74:F6,Winterha Winterhalter Gastronom GmbH
 08:75:72,Obelux Obelux Oy
 08:76:18,ViETechn ViE Technologies Sdn. Bhd.
 08:76:95,"AutoIndu Auto Industrial Co., Ltd."
 08:76:FF,ThomsonT Thomson Telecom Belgium
 08:78:08,"SamsungE Samsung Electronics Co.,Ltd"
 08:79:8C,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:79:99,AIM AIM GmbH
 08:7A:4C,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:7B:12,Sagemcom Sagemcom Broadband SAS
 08:7B:AA,"Svyazkom Svyazkomplektservice, Llc"
 08:7C:39,AmazonTe Amazon Technologies Inc.
 08:7C:BE,Quintic Quintic Corp.
 08:7D:21,Altasect Altasec technology corporation
-08:7E:64,Technico Technicolor CH USA Inc.
+08:7E:64,VantivaU Vantiva USA LLC
 08:7F:98,"vivoMobi vivo Mobile Communication Co., Ltd."
 08:80:39,CiscoSPV Cisco SPVTG
 08:81:B2,"Logitech Logitech (China) Technology Co., Ltd"
 08:81:BC,"HongKong HongKong Ipro Technology Co., Limited"
 08:81:F4,JuniperN Juniper Networks
 08:84:66,Novartis Novartis Pharma AG
 08:84:9D,AmazonTe Amazon Technologies Inc.
@@ -18041,20 +18076,22 @@
 08:87:C7,"Apple Apple, Inc."
 08:8C:2C,"SamsungE Samsung Electronics Co.,Ltd"
 08:8D:C8,"RyowaEle Ryowa Electronics Co.,Ltd"
 08:8E:4F,SFSoftwa SF Software Solutions
 08:8E:90,IntelCor Intel Corporate
 08:8E:DC,"Apple Apple, Inc."
 08:8F:2C,AmberTec Amber Technology Ltd.
+08:8F:C3,"CompalIn Compal Information (Kunshan) Co., Ltd."
 08:90:BA,Danlaw Danlaw Inc
 08:91:15,AmazonTe Amazon Technologies Inc.
+08:91:A3,AmazonTe Amazon Technologies Inc.
 08:92:04,Dell Dell Inc.
 08:93:56,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:94:EF,WistronI Wistron Infocomm (Zhongshan) Corporation
-08:95:2A,Technico Technicolor CH USA Inc.
+08:95:2A,VantivaU Vantiva USA LLC
 08:95:42,"Apple Apple, Inc."
 08:96:AD,"Cisco Cisco Systems, Inc"
 08:96:D7,AVM AVM GmbH
 08:97:34,HewlettP Hewlett Packard Enterprise
 08:97:58,"Shenzhen Shenzhen Strong Rising Electronics Co.,Ltd DongGuan Subsidiary"
 08:97:98,"CompalIn Compal Information (Kunshan) Co., Ltd."
 08:99:E8,KEMAS KEMAS GmbH
@@ -18068,15 +18105,15 @@
 08:9E:08,"Google Google, Inc."
 08:9E:84,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:9F:97,LeroyAut Leroy Automation
 08:A1:2B,"ShenZhen ShenZhen EZL Technology Co., Ltd"
 08:A1:89,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 08:A5:C8,SunnovoI Sunnovo International Limited
 08:A6:BC,AmazonTe Amazon Technologies Inc.
-08:A7:C0,Technico Technicolor CH USA Inc.
+08:A7:C0,VantivaU Vantiva USA LLC
 08:A8:42,"HuaweiDe Huawei Device Co., Ltd."
 08:A8:A1,"Cyclotro Cyclotronics Power Concepts, Inc"
 08:A9:5A,AzureWav AzureWave Technology Inc.
 08:AA:55,"Motorola Motorola Mobility LLC, a Lenovo Company"
 08:AA:89,zte zte corporation
 08:AC:A5,"BenuVide Benu Video, Inc."
 08:AC:C4,FMTech
@@ -18099,30 +18136,33 @@
 08:BB:CC,AK-NORDE AK-NORD EDV VERTRIEBSGES. mbH
 08:BC:20,"Hangzhou Hangzhou Royal Cloud Technology Co., Ltd"
 08:BD:43,Netgear
 08:BE:09,AstrolEl Astrol Electronic AG
 08:BE:77,GreenEle Green Electronics
 08:BE:AC,EdimaxTe Edimax Technology Co. Ltd.
 08:BF:A0,"SamsungE Samsung Electronics Co.,Ltd"
+08:BF:B8,ASUSTekC ASUSTek COMPUTER INC.
 08:C0:21,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:C0:6C,"HuaweiDe Huawei Device Co., Ltd."
 08:C0:EB,"Mellanox Mellanox Technologies, Inc."
 08:C3:B3,"TCLKingE TCL King Electrical Appliances(Huizhou)Co.,Ltd"
 08:C5:E1,SamsungE Samsung Electro-Mechanics(Thailand)
 08:C6:B3,Qtech Qtech Llc
 08:C7:29,"Apple Apple, Inc."
 08:C8:C2,GNAudio GN Audio A/S
 08:CA:45,"ToyouFei Toyou Feiji Electronics Co., Ltd."
 08:CB:E5,R3Soluti R3 Solutions GmbH
 08:CC:27,"Motorola Motorola Mobility LLC, a Lenovo Company"
 08:CC:68,"Cisco Cisco Systems, Inc"
+08:CC:81,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 08:CC:A7,"Cisco Cisco Systems, Inc"
 08:CD:9B,samtecau samtec automotive electronics & software GmbH
 08:D0:9F,"Cisco Cisco Systems, Inc"
 08:D0:B7,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
+08:D1:F9,Espressi Espressif Inc.
 08:D2:3E,IntelCor Intel Corporate
 08:D2:9A,Proforma Proformatique
 08:D3:4B,"TechmanE Techman Electronics (Changshu) Co., Ltd."
 08:D4:0C,IntelCor Intel Corporate
 08:D4:2B,"SamsungE Samsung Electronics Co.,Ltd"
 08:D4:6A,LGElectr LG Electronics (Mobile Communications)
 08:D5:9D,Sagemcom Sagemcom Broadband SAS
@@ -18132,14 +18172,15 @@
 08:DF:CB,Systrome Systrome Networks
 08:E0:21,"HonorDev Honor Device Co., Ltd."
 08:E4:DF,"Shenzhen Shenzhen Sande Dacom Electronics Co., Ltd"
 08:E5:DA,"NanjingF Nanjing Fujitsu Computer Products Co.,Ltd."
 08:E6:3B,zte zte corporation
 08:E6:72,"JebseeEl Jebsee Electronics Co.,Ltd."
 08:E6:89,"Apple Apple, Inc."
+08:E6:C9,Business Business-intelligence of Oriental Nations Corporation Ltd.
 08:E7:E5,"HuaweiDe Huawei Device Co., Ltd."
 08:E8:4F,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:E9:F6,"AMPAKTec AMPAK Technology,Inc."
 08:EA:40,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 08:EA:44,"ExtremeN Extreme Networks, Inc."
 08:EB:29,"JiangsuH Jiangsu Huitong Group Co.,Ltd."
 08:EB:74,"HUMAX HUMAX Co., Ltd."
@@ -18165,14 +18206,15 @@
 08:ED:02:E0:00:00/28,Telstra Telstra Corporation Limited
 08:ED:9D,TecnoMob Tecno Mobile Limited
 08:ED:B9,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 08:ED:ED,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 08:EE:8B,"SamsungE Samsung Electronics Co.,Ltd"
 08:EF:3B,MCSLogic MCS Logic Inc.
 08:EF:AB,SaymeWir Sayme Wireless Sensor Network
+08:F0:1E,eero eero inc.
 08:F1:B3,CiscoMer Cisco Meraki
 08:F1:B7,Towerstr Towerstream Corpration
 08:F1:EA,HewlettP Hewlett Packard Enterprise
 08:F2:F4,"NetOnePa Net One Partners Co.,Ltd."
 08:F3:FB,"Cisco Cisco Systems, Inc"
 08:F4:58,"HuaweiDe Huawei Device Co., Ltd."
 08:F4:AB,"Apple Apple, Inc."
@@ -18181,42 +18223,50 @@
 08:F6:F8,GETEngin GET Engineering
 08:F7:28,GLOBOMul GLOBO Multimedia Sp. z o.o. Sp.k.
 08:F7:E9,HRCPRese HRCP Research and Development Partnership
 08:F8:0D,IEEERegi IEEE Registration Authority
 08:F8:0D:00:00:00/28,"Huizhouc Huizhou changfei Optoelectruonics Technology Co.,Ltd"
 08:F8:0D:10:00:00/28,"Shenzhen Shenzhen DophiGo IoT Technology Co.,Ltd"
 08:F8:0D:20:00:00/28,"Shanghai Shanghai Mininglamp AI Group Co.,Ltd"
+08:F8:0D:30:00:00/28,Annapurn Annapurna labs
 08:F8:0D:40:00:00/28,FG-Lab FG-Lab Inc.
 08:F8:0D:50:00:00/28,"Zhejiang Zhejiang Luci Technology Co., Ltd"
 08:F8:0D:60:00:00/28,"SedaChem Seda Chemical Products Co., Ltd."
 08:F8:0D:70:00:00/28,HANGZHOU HANGZHOU YILI Communication Equipment Ltd
 08:F8:0D:80:00:00/28,OpenYard OpenYard LLC
 08:F8:0D:90:00:00/28,Benelink Benelink Technology Inc.
 08:F8:0D:A0:00:00/28,"MickeyIn Mickey Industry,Ltd."
 08:F8:0D:B0:00:00/28,VontInno Vont Innovations
+08:F8:0D:C0:00:00/28,ZmbiziAp Zmbizi App Llc
+08:F8:0D:D0:00:00/28,"Zhejiang Zhejiang Ev-Tech.,Ltd"
+08:F8:0D:E0:00:00/28,"SuzhouSi Suzhou Sidi Information Technology Co., Ltd."
 08:F8:BC,"Apple Apple, Inc."
+08:F9:E0,Espressi Espressif Inc.
 08:FA:28,"HuaweiTe Huawei Technologies Co.,Ltd"
 08:FA:79,"vivoMobi vivo Mobile Communication Co., Ltd."
 08:FA:E0,FohhnAud Fohhn Audio AG
 08:FB:EA,"AMPAKTec AMPAK Technology,Inc."
 08:FC:52,OpenXS OpenXS BV
 08:FC:88,"SamsungE Samsung Electronics Co.,Ltd"
 08:FD:0E,"SamsungE Samsung Electronics Co.,Ltd"
 08:FF:24,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 08:FF:44,"Apple Apple, Inc."
 09:00:6A,AT&T
 0A:2A:33,Digistor
 0A:36:1C,Smardii
 0A:87:36,IEEE1901 IEEE 1901 Working Group
 0A:8E:62,DeltaSol Delta Solutions LLC
+0A:A2:3B,Vitex Vitex LLC
 0A:CD:8F,CiscoNor Cisco Systems Norway
 0A:D9:C4,"CraftDes Craft Designs, Inc"
 0A:E4:71,Caterpil Caterpillar Inc.
+0C:01:4B,zte zte corporation
+0C:01:C8,"DENSO DENSO Co.,Ltd"
 0C:01:DB,Infinixm Infinix mobility limited
-0C:02:27,Technico Technicolor CH USA Inc.
+0C:02:27,VantivaU Vantiva USA LLC
 0C:02:BD,"SamsungE Samsung Electronics Co.,Ltd"
 0C:04:00,Jantardo Jantar d.o.o.
 0C:05:35,Juniper Juniper Systems
 0C:08:B4,"HUMAX HUMAX Co., Ltd."
 0C:0E:76,D-LinkIn D-Link International
 0C:11:05,"AkuvoxXi Akuvox (Xiamen) Networks Co., Ltd"
 0C:11:67,"Cisco Cisco Systems, Inc"
@@ -18241,20 +18291,22 @@
 0C:20:26,noaxTech noax Technologies AG
 0C:20:D3,"vivoMobi vivo Mobile Communication Co., Ltd."
 0C:21:38,Hengstle Hengstler GmbH
 0C:23:69,Honeywel Honeywell SPS
 0C:25:76,Longchee Longcheer Telecommunication Limited
 0C:27:24,"Cisco Cisco Systems, Inc"
 0C:27:55,Valuable Valuable Techologies Limited
+0C:29:8F,"Tesla Tesla,Inc."
 0C:29:EF,Dell Dell Inc.
 0C:2A:69,"electric electric imp, incorporated"
 0C:2A:86,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 0C:2A:E7,BeijingG Beijing General Research Institute of Mining and Metallurgy
 0C:2C:54,"HuaweiTe Huawei Technologies Co.,Ltd"
 0C:2D:89,QiiQComm QiiQ Communications Inc.
+0C:2E:57,"HuaweiTe Huawei Technologies Co.,Ltd"
 0C:2F:B0,"SamsungE Samsung Electronics Co.,Ltd"
 0C:30:21,"Apple Apple, Inc."
 0C:31:DC,"HuaweiTe Huawei Technologies Co.,Ltd"
 0C:35:26,Microsof Microsoft Corporation
 0C:35:4F,Nokia
 0C:35:FE,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 0C:37:47,zte zte corporation
@@ -18308,37 +18360,40 @@
 0C:5C:B5:40:00:00/28,Annapurn Annapurna labs
 0C:5C:B5:50:00:00/28,Raymond The Raymond Corporation
 0C:5C:B5:60:00:00/28,S2C S2C limited
 0C:5C:B5:70:00:00/28,Energybo Energybox Limited
 0C:5C:B5:80:00:00/28,"Shenzhen Shenzhen C & D Electronics Co., Ltd."
 0C:5C:B5:90:00:00/28,Colordev Colordeve International
 0C:5C:B5:A0:00:00/28,"Zhengzho Zhengzhou coal machinery hydraulic electric control Co.,Ltd"
-0C:5C:B5:B0:00:00/28,Adi
+0C:5C:B5:B0:00:00/28,ADIGloba ADI Global Distribution
 0C:5C:B5:C0:00:00/28,"HunanNew Hunan Newman Car NetworKing Technology Co.,Ltd"
 0C:5C:B5:D0:00:00/28,BSU BSU Inc
 0C:5C:B5:E0:00:00/28,MuntersE Munters Europe AB
 0C:5C:D8,DOLIElek DOLI Elektronik GmbH
 0C:5F:35,NiagaraV Niagara Video Corporation
 0C:60:46,"vivoMobi vivo Mobile Communication Co., Ltd."
 0C:60:76,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 0C:61:11,AndaTech Anda Technologies SAC
 0C:61:27,"Actionte Actiontec Electronics, Inc"
 0C:61:CF,TexasIns Texas Instruments
 0C:62:A6,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 0C:63:FC,"NanjingS Nanjing Signway Technology Co., Ltd"
 0C:64:22,"BeijingW Beijing Wiseasy Technology Co.,Ltd."
+0C:67:14,SernetSu Sernet (Suzhou) Technologies Corporation
 0C:68:03,"Cisco Cisco Systems, Inc"
 0C:6A:BC,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 0C:6A:E6,StanleyS Stanley Security Solutions
 0C:6E:4F,"PrimeVOL PrimeVOLT Co., Ltd."
 0C:6F:9C,ShawComm Shaw Communications Inc.
+0C:70:43,SonyInte Sony Interactive Entertainment Inc.
 0C:70:4A,"HuaweiTe Huawei Technologies Co.,Ltd"
 0C:71:5D,"SamsungE Samsung Electronics Co.,Ltd"
 0C:71:8C,TCTmobil TCT mobile ltd
 0C:72:2C,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
+0C:72:74,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 0C:72:D9,zte zte corporation
 0C:73:29,Sercomm Sercomm Corporation.
 0C:73:BE,"Dongguan Dongguan Haimai Electronie Technology Co.,Ltd"
 0C:73:EB,IEEERegi IEEE Registration Authority
 0C:73:EB:00:00:00/28,GeminiDa Gemini Data Loggers (UK) Limited
 0C:73:EB:10:00:00/28,EversecT Eversec Technology Corporation
 0C:73:EB:20:00:00/28,"Deltapat Deltapath, Inc."
@@ -18355,14 +18410,15 @@
 0C:73:EB:D0:00:00/28,D-Link（S D-Link （Shanghai）Limited Corp.
 0C:73:EB:E0:00:00/28,"TaiwanPu Taiwan Pulse Motion Co., Ltd."
 0C:74:C2,"Apple Apple, Inc."
 0C:75:12,"Shenzhen Shenzhen Kunlun TongTai Technology Co.,Ltd."
 0C:75:23,"BeijingG Beijing Gehua Catv Network Co.,Ltd"
 0C:75:6C,"AnarenMi Anaren Microwave, Inc."
 0C:75:BD,"Cisco Cisco Systems, Inc"
+0C:75:D2,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 0C:77:1A,"Apple Apple, Inc."
 0C:7A:15,IntelCor Intel Corporate
 0C:7B:C8,CiscoMer Cisco Meraki
 0C:7C:28,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 0C:7D:7C,"KexiangI Kexiang Information Technology Co, Ltd."
 0C:7F:B2,"ARRISGro ARRIS Group, Inc."
 0C:7F:ED,IEEERegi IEEE Registration Authority
@@ -18410,14 +18466,15 @@
 0C:86:29:90:00:00/28,Hongkong Hongkong Saint Tech Industrial Limited
 0C:86:29:A0:00:00/28,"Nipron Nipron Co.,Ltd"
 0C:86:29:B0:00:00/28,Akribis Akribis Systems
 0C:86:29:C0:00:00/28,"Shenzhen Shenzhen Yingmu Technology.,Ltd"
 0C:86:29:D0:00:00/28,"BeijingB Beijing Beibianzhida Technology Co.,Ltd"
 0C:86:29:E0:00:00/28,FxTechno Fx Technology Limited
 0C:86:C7,JabilCir Jabil Circuit (Guangzhou) Limited
+0C:87:72,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 0C:89:10,"SamsungE Samsung Electronics Co.,Ltd"
 0C:8A:87,"AgLogica AgLogica Holdings, Inc"
 0C:8B:7D,"Vizio Vizio, Inc"
 0C:8B:95,Espressi Espressif Inc.
 0C:8B:D3,ItelMobi Itel Mobile Limited
 0C:8B:FD,IntelCor Intel Corporate
 0C:8C:24,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
@@ -18432,14 +18489,15 @@
 0C:90:43,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 0C:91:60,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 0C:91:92,IntelCor Intel Corporate
 0C:92:4E,RiceLake Rice Lake Weighing Systems
 0C:93:01,PTPrasim PT. Prasimax Inovasi Teknologi
 0C:93:8F,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 0C:93:FB,BNSSolut BNS Solutions
+0C:95:05,"Chamberl The Chamberlain Group, Inc"
 0C:95:41,ChipseaT Chipsea Technologies (Shenzhen) Corp.
 0C:96:BF,"HuaweiTe Huawei Technologies Co.,Ltd"
 0C:96:CD,Mercury Mercury Corporation
 0C:96:E6,CloudNet Cloud Network Technology (Samoa) Limited
 0C:97:5F,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 0C:98:38,XiaomiCo Xiaomi Communications Co Ltd
 0C:9A:3C,IntelCor Intel Corporate
@@ -18455,14 +18513,15 @@
 0C:A4:02,Alcatel- Alcatel-Lucent IPD
 0C:A4:2A,"OBTeleco OB Telecom Electronic Technology Co., Ltd"
 0C:A6:94,"SunitecE Sunitec Enterprise Co.,Ltd"
 0C:A8:A7,"SamsungE Samsung Electronics Co.,Ltd"
 0C:AA:EE,"AnsjerEl Ansjer Electronics Co., Ltd."
 0C:AC:05,UnitendT Unitend Technologies Inc.
 0C:AC:8A,Sagemcom Sagemcom Broadband SAS
+0C:AE:5F,SiliconL Silicon Laboratories
 0C:AE:7D,TexasIns Texas Instruments
 0C:AE:BD,EdifierI Edifier International
 0C:AF:31,"Cisco Cisco Systems, Inc"
 0C:AF:5A,GenusPow Genus Power Infrastructures Limited
 0C:B0:88,AITeleco AITelecom
 0C:B2:B7,TexasIns Texas Instruments
 0C:B3:19,"SamsungE Samsung Electronics Co.,Ltd"
@@ -18477,14 +18536,15 @@
 0C:B7:89,"HonorDev Honor Device Co., Ltd."
 0C:B8:15,Espressi Espressif Inc.
 0C:B8:E8,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 0C:B9:12,JM-DATA JM-DATA GmbH
 0C:B9:37,"UbeeInte Ubee Interactive Co., Limited"
 0C:BC:9F,"Apple Apple, Inc."
 0C:BD:51,TCTmobil TCT mobile ltd
+0C:BD:75,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 0C:BE:F1,"HuaweiDe Huawei Device Co., Ltd."
 0C:BF:15,Genetec Genetec Inc.
 0C:BF:3F,"Shenzhen Shenzhen Lencotion Technology Co.,Ltd"
 0C:BF:74,MorseMic Morse Micro
 0C:C0:C0,MagnetiM Magneti Marelli Sistemas Electronicos Mexico
 0C:C3:A7,Meritec
 0C:C4:13,"Google Google, Inc."
@@ -18530,14 +18590,15 @@
 0C:D2:B5,Binatone Binatone Telecommunication Pvt. Ltd
 0C:D5:02,WestellT Westell Technologies Inc.
 0C:D6:96,Amimon Amimon Ltd
 0C:D6:BD,"HuaweiTe Huawei Technologies Co.,Ltd"
 0C:D7:46,"Apple Apple, Inc."
 0C:D7:C2,"AxiumTec Axium Technologies, Inc."
 0C:D8:6C,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
+0C:D9:23,GOCLOUDN GOCLOUD Networks(GAOKE Networks)
 0C:D9:96,"Cisco Cisco Systems, Inc"
 0C:D9:C1,Visteon Visteon Corporation
 0C:DA:41,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 0C:DC:7E,Espressi Espressif Inc.
 0C:DC:CC,InalaTec Inala Technologies
 0C:DD:24,IntelCor Intel Corporate
 0C:DD:EF,Nokia Nokia Corporation
@@ -18662,31 +18723,35 @@
 10:10:81,zte zte corporation
 10:10:B6,McCain McCain Inc
 10:12:12,VivoInte Vivo International Corporation Pty Ltd
 10:12:18,Korins Korins Inc.
 10:12:48,"ITG ITG, Inc."
 10:12:50,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 10:12:B4,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
+10:12:D0,zte zte corporation
 10:12:FB,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 10:13:31,Technico Technicolor Delivery Technologies Belgium NV
 10:13:EE,JustecIn Justec International Technology INC.
+10:15:C1,"ZhanzuoB Zhanzuo (Beijing) Technology Co., Ltd."
+10:18:49,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 10:18:9E,ElmoMoti Elmo Motion Control
 10:19:65,"NewH3CTe New H3C Technologies Co., Ltd"
 10:1B:54,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:1C:0C,"Apple Apple, Inc."
 10:1D:51,8MeshNet 8Mesh Networks Limited
 10:1D:C0,"SamsungE Samsung Electronics Co.,Ltd"
 10:1E:DA,Ingenico Ingenico Terminals Sas
 10:1F:74,HewlettP Hewlett Packard
 10:22:79,"ZeroDesk ZeroDesktop, Inc."
 10:24:07,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:27:79,Sadel Sadel S.p.A.
 10:27:BE,Tvip
 10:27:F5,TP-Link TP-Link Corporation Limited
 10:28:31,Morion Morion Inc.
+10:28:34,SALZAuto SALZ Automation GmbH
 10:29:59,"Apple Apple, Inc."
 10:29:AB,"SamsungE Samsung Electronics Co.,Ltd"
 10:2A:B3,XiaomiCo Xiaomi Communications Co Ltd
 10:2B:41,"SamsungE Samsung Electronics Co.,Ltd"
 10:2C:6B,"AMPAKTec AMPAK Technology, Inc."
 10:2C:83,Ximea
 10:2C:8D,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
@@ -18700,15 +18765,15 @@
 10:2F:A3,Shenzhen Shenzhen Uvision-tech Technology Co.Ltd
 10:30:25,"Apple Apple, Inc."
 10:30:34,Cara Cara Systems
 10:30:47,"SamsungE Samsung Electronics Co.,Ltd"
 10:32:1D,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:32:7E,"HuaweiDe Huawei Device Co., Ltd."
 10:33:78,"FLECTRON FLECTRON Co., LTD"
-10:33:BF,Technico Technicolor CH USA Inc.
+10:33:BF,VantivaU Vantiva USA LLC
 10:34:1B,Spacelin Spacelink
 10:36:4A,BostonDy Boston Dynamics
 10:37:11,NorbitIt Norbit Its
 10:38:1F,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 10:39:17,"SamsungE Samsung Electronics Co.,Ltd"
 10:39:4E,"Hisenseb Hisense broadband multimedia technology Co.,Ltd"
 10:39:E9,JuniperN Juniper Networks
@@ -18776,15 +18841,15 @@
 10:5D:DC,"HuaweiDe Huawei Device Co., Ltd."
 10:5F:02,Private
 10:5F:06,"Actionte Actiontec Electronics, Inc"
 10:5F:49,CiscoSPV Cisco SPVTG
 10:5F:D4,Tendyron Tendyron Corporation
 10:60:4B,HewlettP Hewlett Packard
 10:62:C9,Adatis Adatis GmbH & Co. KG
-10:62:D0,Technico Technicolor CH USA Inc.
+10:62:D0,VantivaU Vantiva USA LLC
 10:62:E5,HewlettP Hewlett Packard
 10:62:EB,D-LinkIn D-Link International
 10:63:4B,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 10:63:C8,LiteonTe Liteon Technology Corporation
 10:64:E2,ADFwebco ADFweb.com s.r.l.
 10:65:30,Dell Dell Inc.
 10:65:A3,Panamax Panamax LLC
@@ -18796,28 +18861,30 @@
 10:6F:3F,Buffalo Buffalo.Inc
 10:6F:D9,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 10:6F:EF,Ad-SolNi Ad-Sol Nissin Corp
 10:70:FD,"Mellanox Mellanox Technologies, Inc."
 10:71:00,"HuaweiDe Huawei Device Co., Ltd."
 10:71:B3,ZyxelCom Zyxel Communications Corporation
 10:71:F9,"CloudTel Cloud Telecomputers, LLC"
+10:71:FA,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 10:72:23,Tellesco Tellescom Industria E Comercio Em Telecomunicacao
 10:73:EB,Infiniti Infiniti Electro-Optics
 10:74:6F,Motorola Motorola Solutions Malaysia Sdn. Bhd.
 10:76:36,EardaTec Earda Technologies co Ltd
 10:76:8A,EoCell
 10:77:17,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 10:77:B0,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 10:77:B1,"SamsungE Samsung Electronics Co.,Ltd"
 10:78:5B,"Actionte Actiontec Electronics, Inc"
 10:78:73,"Shenzhen Shenzhen Jinkeyi Communication Co., Ltd."
 10:78:CE,"HanvitSI Hanvit SI, Inc."
 10:78:D2,"Elitegro Elitegroup Computer Systems Co.,Ltd."
 10:7A:86,U&UEngin U&U Engineering Inc.
 10:7B:44,ASUSTekC ASUSTek COMPUTER INC.
+10:7B:93,"ZhenShiI Zhen Shi Information Technology (Shanghai) Co., Ltd."
 10:7B:A4,"OliveDov Olive & Dove Co.,Ltd."
 10:7B:CE,Nokia
 10:7B:EF,ZyxelCom Zyxel Communications Corporation
 10:7D:1A,Dell Dell Inc.
 10:81:B4,"HunanGre Hunan Greatwall Galaxy Science and Technology Co.,Ltd."
 10:82:3D,"RuijieNe Ruijie Networks Co.,LTD"
 10:82:86,"Luxshare Luxshare Precision Industry Co.,Ltd"
@@ -18830,14 +18897,15 @@
 10:8A:1B,RAONIX RAONIX Inc.
 10:8B:6A,"Antailiy Antailiye Technology Co.,Ltd"
 10:8C:CF,"Cisco Cisco Systems, Inc"
 10:8E:BA,Molekule
 10:8E:E0,"SamsungE Samsung Electronics Co.,Ltd"
 10:8F:FE,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:91:A8,Espressi Espressif Inc.
+10:91:D1,IntelCor Intel Corporate
 10:92:66,"SamsungE Samsung Electronics Co.,Ltd"
 10:93:97,"ARRISGro ARRIS Group, Inc."
 10:93:E9,"Apple Apple, Inc."
 10:94:97,Logitech Logitech Hong Kong
 10:94:BB,"Apple Apple, Inc."
 10:95:4B,Megabyte Megabyte Ltd.
 10:96:1A,ChipseaT Chipsea Technologies (Shenzhen) Corp.
@@ -18846,82 +18914,91 @@
 10:98:26,Nokia
 10:98:36,Dell Dell Inc.
 10:98:C3,"MurataMa Murata Manufacturing Co., Ltd."
 10:9A:B9,Tosibox Tosibox Oy
 10:9A:DD,"Apple Apple, Inc."
 10:9C:70,PrusaRes Prusa Research s.r.o.
 10:9D:7A,"HuaweiDe Huawei Device Co., Ltd."
+10:9D:9C,EMMicroe EM Microelectronic
 10:9E:3A,"Zhejiang Zhejiang Tmall Technology Co., Ltd."
+10:9F:41,"Apple Apple, Inc."
 10:9F:4F,"NewH3CIn New H3C Intelligence Terminal Co., Ltd."
 10:9F:A9,"Actionte Actiontec Electronics, Inc"
 10:A1:3B,Fujikura Fujikura Rubber Ltd.
 10:A2:4E,"Gold3Lin Gold3Link Electronics Co., Ltd"
 10:A3:B8,Iskratel Iskratel d.o.o.
 10:A4:B9,"BaiduOnl Baidu Online Network Technology (Beijing) Co., Ltd"
 10:A4:BE,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 10:A4:DA,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:A5:1D,IntelCor Intel Corporate
 10:A5:62,ItonTech Iton Technology Corp.
 10:A5:D0,"MurataMa Murata Manufacturing Co., Ltd."
 10:A6:59,"MobileCr Mobile Create Co.,Ltd."
 10:A7:43,SKMtek SK Mtek Limited
+10:A7:93,VantivaU Vantiva USA LLC
 10:A8:29,"Cisco Cisco Systems, Inc"
 10:A9:32,"BeijingC Beijing Cyber Cloud Technology Co. ,Ltd."
 10:AE:60,AmazonTe Amazon Technologies Inc.
 10:AE:A5,Duskrise Duskrise inc.
 10:AF:78,"Shenzhen Shenzhen ATUE Technology Co., Ltd"
 10:B1:DF,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 10:B1:F8,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:B2:32,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
 10:B2:6B,"base base Co.,Ltd."
 10:B3:6F,BoweiTec Bowei Technology Company Limited
 10:B3:C6,"Cisco Cisco Systems, Inc"
 10:B3:D5,"Cisco Cisco Systems, Inc"
 10:B3:D6,"Cisco Cisco Systems, Inc"
+10:B5:88,"Apple Apple, Inc."
 10:B7:13,Private
 10:B7:A8,CableFre CableFree Networks Limited
 10:B7:F6,Plastofo Plastoform Industries Ltd.
 10:B9:C4,"Apple Apple, Inc."
 10:B9:F7,Niko-Ser Niko-Servodan
 10:B9:FE,Lika Lika srl
 10:BA:A5,"GanaI&C Gana I&C Co., Ltd"
 10:BB:F3,HunanFn- Hunan Fn-Link Technology Limited
 10:BC:97,"vivoMobi vivo Mobile Communication Co., Ltd."
 10:BD:18,"Cisco Cisco Systems, Inc"
+10:BD:3A,"Apple Apple, Inc."
 10:BD:55,Q-Lab Q-Lab Corporation
+10:BE:99,Netberg
 10:BE:F5,D-LinkIn D-Link International
 10:BF:48,ASUSTekC ASUSTek COMPUTER INC.
 10:BF:67,AmazonTe Amazon Technologies Inc.
 10:C0:7C,Blu-rayD Blu-ray Disc Association
 10:C1:72,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:C2:2F,"ChinaEnt China Entropy Co., Ltd."
-10:C2:5A,Technico Technicolor CH USA Inc.
+10:C2:5A,VantivaU Vantiva USA LLC
 10:C2:BA,"UTT UTT Co., Ltd."
 10:C3:7B,ASUSTekC ASUSTek COMPUTER INC.
 10:C3:AB,"HuaweiTe Huawei Technologies Co.,Ltd"
+10:C4:CA,"HUMAX HUMAX Co., Ltd."
 10:C5:86,"BioSound Bio Sound Lab Co., Ltd."
 10:C5:95,Lenovo
 10:C6:0C,DominoUK Domino UK Ltd
 10:C6:1F,"HuaweiTe Huawei Technologies Co.,Ltd"
 10:C6:5E,Adapt-IP
 10:C6:7E,"Shenzhen Shenzhen Juchin Technology Co., Ltd"
 10:C6:FC,GarminIn Garmin International
 10:C7:3F,MidasKla Midas Klark Teknik Ltd
 10:C7:53,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
 10:C9:CA,AceTechn Ace Technology Corp.
 10:CA:81,Precia
+10:CA:BF,TexasIns Texas Instruments
 10:CC:1B,"Liverock Liverock technologies,INC"
 10:CC:DB,AximumPr Aximum Produits Electroniques
 10:CD:6E,Fisys
 10:CD:AE,Avaya Avaya Inc
 10:CD:B6,"Essentia Essential Products, Inc."
 10:CE:02,AmazonTe Amazon Technologies Inc.
 10:CE:45,Miromico Miromico AG
 10:CE:A9,TexasIns Texas Instruments
 10:CE:E9,"Apple Apple, Inc."
+10:CF:0F,"Apple Apple, Inc."
 10:D0:7A,"AMPAKTec AMPAK Technology, Inc."
 10:D0:AB,zte zte corporation
 10:D1:DC,INSTARDe INSTAR Deutschland GmbH
 10:D3:8A,"SamsungE Samsung Electronics Co.,Ltd"
 10:D5:42,"SamsungE Samsung Electronics Co.,Ltd"
 10:D5:61,TuyaSmar Tuya Smart Inc.
 10:D6:80,Tendyron Tendyron Corporation
@@ -18938,23 +19015,24 @@
 10:DC:B6:50:00:00/28,Milesigh Milesight Taiwan
 10:DC:B6:60:00:00/28,ProlanZr Prolan Zrt.
 10:DC:B6:70:00:00/28,"MoyaComm Moya Commumication Technology (Shenzhen) Co.,Ltd."
 10:DC:B6:80:00:00/28,"SanofiBe Sanofi (Beijing) Pharmaceutical Co., Ltd."
 10:DC:B6:90:00:00/28,"FuzhouRo Fuzhou Rockchip Electronics Co.,Ltd"
 10:DC:B6:A0:00:00/28,Pickerin Pickering Interfaces Ltd
 10:DC:B6:B0:00:00/28,EyeballF Eyeball Fintech Company
-10:DC:B6:C0:00:00/28,BBPOSInt BBPOS International Limited
+10:DC:B6:C0:00:00/28,BBPOS BBPOS Limited
 10:DC:B6:D0:00:00/28,LeoLabs
 10:DC:B6:E0:00:00/28,"Shenzhen Shenzhen Sunwoda intelligent hardware Co.,Ltd"
 10:DD:B1,"Apple Apple, Inc."
 10:DD:F4,"MaxwayEl Maxway Electronics CO.,LTD"
 10:DE:E4,automati automationNEXT GmbH
 10:DF:8B,"Shenzhen Shenzhen CareDear Communication Technology Co.,Ltd"
 10:DF:FC,Siemens Siemens AG
 10:E1:77,"ARRISGro ARRIS Group, Inc."
+10:E2:C9,"Apple Apple, Inc."
 10:E2:D5,QiHardwa Qi Hardware Inc.
 10:E3:C7,SeohwaTe Seohwa Telecom
 10:E4:AF,"Apr Apr, Llc"
 10:E4:C2,"SamsungE Samsung Electronics Co.,Ltd"
 10:E6:8F,"Kwangsun Kwangsung Electronics Korea Co.,Ltd."
 10:E6:AE,"SourceTe Source Technologies, LLC"
 10:E7:7A,STMicrol STMicrolectronics International NV
@@ -19002,14 +19080,15 @@
 14:09:DC,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:0A:29,Tiinlab Tiinlab Corporation
 14:0A:C5,AmazonTe Amazon Technologies Inc.
 14:0C:5B,PLNetwor PLNetworks
 14:0C:76,FreeboxS Freebox Sas
 14:0D:4F,Flextron Flextronics International
 14:0F:42,Nokia
+14:0F:A6,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 14:10:9F,"Apple Apple, Inc."
 14:11:14,TecnoMob Tecno Mobile Limited
 14:11:5D,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 14:13:0B,GarminIn Garmin International
 14:13:30,Anakreon Anakreon UK LLP
 14:13:33,AzureWav AzureWave Technology Inc.
 14:13:46,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
@@ -19018,18 +19097,20 @@
 14:14:4B,"RuijieNe Ruijie Networks Co.,LTD"
 14:14:59,Vodafone Vodafone Italia S.p.A.
 14:14:E6,"NingboSa Ningbo Sanhe Digital Co.,Ltd"
 14:15:7C,"TokyoCos Tokyo Cosmos Electric Co.,Ltd."
 14:16:9D,"Cisco Cisco Systems, Inc"
 14:16:9E,Wingtech Wingtech Group (HongKong）Limited
 14:17:2A,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
+14:18:44,XenonSma Xenon Smart Teknoloji Ltd.
 14:18:77,Dell Dell Inc.
 14:18:C3,IntelCor Intel Corporate
 14:19:73,"BeijingY Beijing Yunyi Times Technology Co.,Ltd"
 14:1A:51,Treetech Treetech Sistemas Digitais
+14:1A:97,"Apple Apple, Inc."
 14:1A:A3,"Motorola Motorola Mobility LLC, a Lenovo Company"
 14:1A:AA,MetalWor Metal Work SpA
 14:1B:30,"Shenzhen Shenzhen Yipingfang Network Technology Co., Ltd."
 14:1B:BD,Volex Volex Inc.
 14:1B:F0,Intellim Intellimedia Systems Ltd
 14:1F:78,"SamsungE Samsung Electronics Co.,Ltd"
 14:1F:BA,IEEERegi IEEE Registration Authority
@@ -19061,25 +19142,28 @@
 14:28:82,MidicomE Midicom Electronics Co.Ltd
 14:29:71,NemoaEle Nemoa Electronics (Hk) Co. Ltd
 14:2A:14,"ShenZhen ShenZhen Selenview Digital Technology Co.,Ltd"
 14:2B:D2,Armtel Armtel Ltd.
 14:2B:D6,"Guangdon Guangdong Appscomm Co.,Ltd"
 14:2C:78,"GooWiWir GooWi Wireless Technology Co., Limited"
 14:2D:27,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+14:2D:41,SiliconL Silicon Laboratories
 14:2D:4D,"Apple Apple, Inc."
 14:2D:79,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 14:2D:8B,"IncipioT Incipio Technologies, Inc"
 14:2D:F5,Amphitec Amphitech
 14:2E:5E,Sercomm Sercomm Corporation.
 14:2F:FD,LtSecuri Lt Security Inc
 14:30:04,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:30:7A,Avermetr Avermetrics
 14:30:C6,"Motorola Motorola Mobility LLC, a Lenovo Company"
 14:32:D1,"SamsungE Samsung Electronics Co.,Ltd"
 14:33:65,TEMMobil TEM Mobile Limited
+14:33:75,ZyxelCom Zyxel Communications Corporation
+14:34:F6,LvSoluti Lv Solution Sdn. Bhd.
 14:35:8B,"Mediabri Mediabridge Products, LLC."
 14:35:B3,"FutureDe Future Designs, Inc."
 14:36:05,Nokia Nokia Corporation
 14:36:C6,LenovoMo Lenovo Mobile Communication Technology Ltd.
 14:37:19,PTPrakar PT Prakarsa Visi Valutama
 14:37:3B,PROCOM PROCOM Systems
 14:3A:EA,Dynapowe Dynapower Company LLC
@@ -19175,17 +19259,21 @@
 14:79:F3,"ChinaMob China Mobile Group Device Co.,Ltd."
 14:7B:AC,Nokia
 14:7D:05,SercommP Sercomm Philippines Inc
 14:7D:B3,"JoaTelec Joa Telecom.Co.,Ltd"
 14:7D:C5,"MurataMa Murata Manufacturing Co., Ltd."
 14:7D:DA,"Apple Apple, Inc."
 14:7E:A1,Britania Britania Eletrônicos S.A.
+14:7F:0F,TexasIns Texas Instruments
 14:82:5B,"HefeiRad Hefei Radio Communication Technology Co., Ltd"
 14:84:30,MitacCom Mitac Computing Technology Corporation
+14:84:73,"Cisco Cisco Systems, Inc"
+14:84:77,"NewH3CTe New H3C Technologies Co., Ltd"
 14:85:09,"Apple Apple, Inc."
+14:85:54,EardaTec Earda Technologies co Ltd
 14:85:7F,IntelCor Intel Corporate
 14:86:92,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 14:87:6A,"Apple Apple, Inc."
 14:88:E6,"Apple Apple, Inc."
 14:89:19,2bps
 14:89:3E,VixtelTe Vixtel Technologies Limted
 14:89:CB,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -19198,46 +19286,51 @@
 14:91:38,AmazonTe Amazon Technologies Inc.
 14:91:82,BelkinIn Belkin International Inc.
 14:93:46,PNIsenso PNI sensor corporation
 14:94:2F,"Usys Usys Co.,Ltd."
 14:94:48,BluCastl Blu Castle S.A.
 14:94:6C,"Apple Apple, Inc."
 14:95:CE,"Apple Apple, Inc."
+14:96:2D,"NewH3CTe New H3C Technologies Co., Ltd"
 14:96:E5,"SamsungE Samsung Electronics Co.,Ltd"
 14:98:77,"Apple Apple, Inc."
-14:98:7D,Technico Technicolor CH USA Inc.
+14:98:7D,VantivaU Vantiva USA LLC
+14:99:3E,XiaomiCo Xiaomi Communications Co Ltd
 14:99:E2,"Apple Apple, Inc."
 14:9A:10,Microsof Microsoft Corporation
 14:9B:2F,"JiangSuZ JiangSu ZhongXie Intelligent Technology co., LTD"
 14:9B:D7,"MuliMuwa Muli Muwai Furniture Qidong Co., Ltd"
 14:9B:F3,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+14:9C:EF,TexasIns Texas Instruments
 14:9D:09,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:9D:99,"Apple Apple, Inc."
 14:9E:5D,"IBReform JSC ""IB Reform"""
 14:9E:CF,Dell Dell Inc.
 14:9F:3C,"SamsungE Samsung Electronics Co.,Ltd"
 14:9F:43,CiscoMer Cisco Meraki
 14:9F:B6,"Guangdon Guangdong Genius Technology Co., Ltd."
 14:9F:E8,LenovoMo Lenovo Mobile Communication Technology Ltd.
 14:A0:F8,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:A1:BF,"ASSAABLO ASSA ABLOY Korea Co., Ltd Unilock"
 14:A2:A0,"Cisco Cisco Systems, Inc"
 14:A3:2F,"HuaweiDe Huawei Device Co., Ltd."
 14:A3:64,"SamsungE Samsung Electronics Co.,Ltd"
 14:A3:B4,"HuaweiDe Huawei Device Co., Ltd."
+14:A4:17,"Shenzhen Shenzhen Belon Technology CO.,LTD"
 14:A5:1A,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:A6:2C,SMDezac S.M. Dezac S.A.
 14:A7:2B,currento currentoptronics Pvt.Ltd
 14:A7:8B,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 14:A8:6B,"ShenZhen ShenZhen Telacom Science&Technology Co., Ltd"
 14:A9:D0,"F5Networ F5 Networks, Inc."
 14:A9:E3,Mst Mst Corporation
 14:AB:02,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:AB:56,"WuxiFuni Wuxi Funide Digital Co.,Ltd"
 14:AB:C5,IntelCor Intel Corporate
+14:AB:EC,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 14:AB:F0,"ARRISGro ARRIS Group, Inc."
 14:AC:60,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 14:AD:CA,ChinaMob China Mobile Iot Limited company
 14:AE:85,IEEERegi IEEE Registration Authority
 14:AE:85:00:00:00/28,Kayamati Kayamatics Limited
 14:AE:85:10:00:00/28,"HenfredT Henfred Technology Co., Ltd."
 14:AE:85:20:00:00/28,"Qingdaoi Qingdao iTechene Technologies Co., Ltd."
@@ -19259,27 +19352,29 @@
 14:B2:E5,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 14:B3:1F,Dell Dell Inc.
 14:B3:70,"GigasetD Gigaset Digital Technology (Shenzhen) Co., Ltd."
 14:B3:A1,JuniperN Juniper Networks
 14:B4:57,SiliconL Silicon Laboratories
 14:B4:84,"SamsungE Samsung Electronics Co.,Ltd"
 14:B7:3D,ARCHEANT ARCHEAN Technologies
-14:B7:F8,Technico Technicolor CH USA Inc.
+14:B7:F8,VantivaU Vantiva USA LLC
 14:B8:37,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 14:B9:68,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:BB:6E,"SamsungE Samsung Electronics Co.,Ltd"
 14:BD:61,"Apple Apple, Inc."
 14:C0:3E,"ARRISGro ARRIS Group, Inc."
+14:C0:50,"Guangdon Guangdong Genius Technology Co., Ltd."
 14:C0:89,DuneHd Dune Hd Ltd
 14:C0:A1,"UCloudTe UCloud Technology Co., Ltd."
 14:C1:26,Nokia Nokia Corporation
 14:C1:4E,"Google Google, Inc."
 14:C1:FF,"ShenZhen ShenZhen QianHai Comlan communication Co.,LTD"
 14:C2:13,"Apple Apple, Inc."
 14:C2:1D,SabtechI Sabtech Industries
+14:C3:5E,FibRSolG FibRSol Global Network Limited
 14:C3:C2,KASchmer K.A. Schmersal GmbH & Co. KG
 14:C6:97,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 14:C8:8B,"Apple Apple, Inc."
 14:C9:13,LGElectr LG Electronics
 14:C9:CF,Sigmasta Sigmastar Technology Ltd.
 14:CA:A0,Hu Hu&Co
 14:CB:19,HP HP Inc.
@@ -19293,18 +19388,20 @@
 14:D1:1F,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:D1:69,"HuaweiTe Huawei Technologies Co.,Ltd"
 14:D1:9E,"Apple Apple, Inc."
 14:D4:24,AzureWav AzureWave Technology Inc.
 14:D4:FE,"ARRISGro ARRIS Group, Inc."
 14:D6:4D,D-LinkIn D-Link International
 14:D7:6E,"CONCHELE CONCH ELECTRONIC Co.,Ltd"
+14:D8:64,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 14:DA:E9,ASUSTekC ASUSTek COMPUTER INC.
 14:DB:85,SNetMedi S Net Media
 14:DC:51,"XiamenCh Xiamen Cheerzing IOT Technology Co.,Ltd."
 14:DC:E2,THALESAV THALES AVS France
+14:DD:02,"Liangang Liangang Optoelectronic Technology CO., Ltd."
 14:DD:9C,"vivoMobi vivo Mobile Communication Co., Ltd."
 14:DD:A9,ASUSTekC ASUSTek COMPUTER INC.
 14:DD:E5,Mpmkvvcl
 14:DE:39,"HuaweiDe Huawei Device Co., Ltd."
 14:E4:EC,mLogic mLogic LLC
 14:E6:E4,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 14:E7:C8,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
@@ -19318,14 +19415,15 @@
 14:EE:9D,AirNav AirNav Systems LLC
 14:EF:CF,Schreder
 14:F0:C5,Xtremio Xtremio Ltd.
 14:F2:87,"Apple Apple, Inc."
 14:F2:8E,ShenYang ShenYang ZhongKe-Allwin Technology Co.LTD
 14:F4:2A,"SamsungE Samsung Electronics Co.,Ltd"
 14:F5:92,"Shenzhen Shenzhen SDG DONZHI Technology Co., Ltd"
+14:F5:F9,HunanFn- Hunan Fn-Link Technology Limited
 14:F6:5A,XiaomiCo Xiaomi Communications Co Ltd
 14:F6:D8,IntelCor Intel Corporate
 14:F8:93,"WuhanFib Wuhan FiberHome Digital Technology Co.,Ltd."
 14:FB:70,"HuaweiDe Huawei Device Co., Ltd."
 14:FE:AF,Sagittar Sagittar Limited
 14:FE:B5,Dell Dell Inc.
 18:00:2D,Sony Sony Corporation
@@ -19352,14 +19450,15 @@
 18:10:4E,Cedint-U Cedint-Upm
 18:11:71,"Guangzho Guangzhou Doctorpai Education & Technology Co.,Ltd"
 18:12:12,CeptonTe Cepton Technologies
 18:13:2D,zte zte corporation
 18:14:20,TebSas Teb Sas
 18:14:56,Nokia Nokia Corporation
 18:14:6C,"Zhejiang Zhejiang Tmall Technology Co., Ltd."
+18:14:AE,Nokia
 18:16:C9,"SamsungE Samsung Electronics Co.,Ltd"
 18:16:E8,"Siliconw Siliconware Precision Industries Co., Ltd."
 18:17:14,Daewoois
 18:17:25,"CameoCom Cameo Communications, Inc."
 18:18:8B,FcntLmit Fcnt Lmited
 18:19:3F,Tamtron Tamtron Oy
 18:19:D6,"SamsungE Samsung Electronics Co.,Ltd"
@@ -19372,14 +19471,15 @@
 18:20:32,"Apple Apple, Inc."
 18:20:4C,Kummler+ Kummler+Matter AG
 18:20:A6,"Sage Sage Co., Ltd."
 18:20:D5,"ARRISGro ARRIS Group, Inc."
 18:21:95,"SamsungE Samsung Electronics Co.,Ltd"
 18:22:7E,"SamsungE Samsung Electronics Co.,Ltd"
 18:26:49,IntelCor Intel Corporate
+18:26:54,"SamsungE Samsung Electronics Co.,Ltd"
 18:26:66,"SamsungE Samsung Electronics Co.,Ltd"
 18:28:61,AirTiesW AirTies Wireless Networks
 18:2A:44,HiroseEl Hirose Electronic System
 18:2A:57,"HuaweiTe Huawei Technologies Co.,Ltd"
 18:2A:7B,"Nintendo Nintendo Co., Ltd."
 18:2A:D3,JuniperN Juniper Networks
 18:2B:05,8DTechno 8D Technologies
@@ -19391,15 +19491,15 @@
 18:30:09,"WoojinIn Woojin Industrial Systems Co., Ltd."
 18:30:0C,"HisenseE Hisense Electric Co.,Ltd"
 18:31:BF,ASUSTekC ASUSTek COMPUTER INC.
 18:32:19,EMMicroe EM Microelectronic
 18:32:A2,"LaonTech Laon Technology Co., Ltd."
 18:33:9D,"Cisco Cisco Systems, Inc"
 18:34:51,"Apple Apple, Inc."
-18:34:AF,"Kaonmedi Kaonmedia CO., LTD."
+18:34:AF,"KaonGrou Kaon Group Co., Ltd."
 18:35:D1,"ARRISGro ARRIS Group, Inc."
 18:36:72,"Shaoxing Shaoxing ShunChuang Technology CO.,LTD"
 18:36:FC,ElecsysI Elecsys International Corporation
 18:38:25,"WuhanLin Wuhan Lingjiu High-tech Co.,Ltd."
 18:38:64,"Cap-Tech Cap-Tech International Co., Ltd."
 18:38:AE,ConspinS Conspin Solution
 18:39:19,Unicoi Unicoi Systems
@@ -19416,14 +19516,15 @@
 18:3F:47,"SamsungE Samsung Electronics Co.,Ltd"
 18:40:A4,"Shenzhen Shenzhen Trylong Smart Science and Technology Co., Ltd."
 18:41:FE,Digital1 Digital 14
 18:42:1D,Private
 18:42:2F,AlcatelL Alcatel Lucent
 18:42:D4,"WuhanHos Wuhan Hosan Telecommunication Technology Co.,Ltd"
 18:44:62,"RiavaNet Riava Networks, Inc."
+18:44:CF,B+LIndus B+L Industrial Measurements GmbH
 18:44:E6,zte zte corporation
 18:45:16,TexasIns Texas Instruments
 18:45:93,TaicangT Taicang T&W Electronics
 18:45:B3,IEEERegi IEEE Registration Authority
 18:45:B3:00:00:00/28,"leetopte leetop tech co.,ltd"
 18:45:B3:10:00:00/28,Pfannenb Pfannenberg GmbH
 18:45:B3:20:00:00/28,"Haierclo Haier cloud Health Technology (Qingdao) Co., Ltd"
@@ -19442,14 +19543,15 @@
 18:46:17,"SamsungE Samsung Electronics Co.,Ltd"
 18:46:44,HomeCont Home Control Singapore Pte Ltd
 18:47:3D,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 18:48:59,Castlene Castlenet Technology Inc.
 18:48:BE,AmazonTe Amazon Technologies Inc.
 18:48:CA,"MurataMa Murata Manufacturing Co., Ltd."
 18:48:D8,Fastback Fastback Networks
+18:4A:53,"Apple Apple, Inc."
 18:4A:6F,"Alcatel- Alcatel-Lucent Shanghai Bell Co., Ltd"
 18:4B:0D,RuckusWi Ruckus Wireless
 18:4B:DF,Caavo Caavo Inc
 18:4C:08,Rockwell Rockwell Automation
 18:4C:AE,Continen Continental
 18:4E:03,HMDGloba HMD Global Oy
 18:4E:16,"SamsungE Samsung Electronics Co.,Ltd"
@@ -19484,27 +19586,29 @@
 18:60:24,HewlettP Hewlett Packard
 18:61:C7,lemonbea lemonbeat GmbH
 18:62:2C,Sagemcom Sagemcom Broadband SAS
 18:62:E4,TexasIns Texas Instruments
 18:64:72,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 18:65:71,"TopVicto Top Victory Electronics (Taiwan) Co., Ltd."
 18:65:90,"Apple Apple, Inc."
+18:65:C7,Dongguan Dongguan YIMO Technology Co.LTD
 18:66:C7,"Shenzhen Shenzhen Libre Technology Co., Ltd"
 18:66:DA,Dell Dell Inc.
 18:66:E3,"Veros Veros Systems, Inc."
 18:66:F0,Jupiter Jupiter Systems
 18:67:3F,HanoverD Hanover Displays Limited
 18:67:51,KOMEGInd KOMEG Industrielle Messtechnik GmbH
 18:67:B0,"SamsungE Samsung Electronics Co.,Ltd"
 18:68:6A,zte zte corporation
 18:68:82,"BewardR& Beward R&D Co., Ltd."
 18:68:CB,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 18:69:D4,"SamsungE Samsung Electronics Co.,Ltd"
 18:69:D8,TuyaSmar Tuya Smart Inc.
 18:69:DA,"ChinaMob China Mobile Group Device Co.,Ltd."
+18:6A:81,Sagemcom Sagemcom Broadband SAS
 18:6D:99,Adanis Adanis Inc.
 18:6F:2D,Shenzhen Shenzhen Sundray Technologies Company Limited
 18:70:3B,"HuaweiDe Huawei Device Co., Ltd."
 18:71:17,etapluse eta plus electronic gmbh
 18:71:D5,"HazensAu Hazens Automotive Electronics(SZ)Co.,Ltd."
 18:74:2E,AmazonTe Amazon Technologies Inc.
 18:74:E2,IEEERegi IEEE Registration Authority
@@ -19528,25 +19632,27 @@
 18:78:D4,Verizon
 18:79:A2,GmjElect Gmj Electric Limited
 18:7A:3B,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 18:7A:3E,SiliconL Silicon Laboratories
 18:7A:93,AMICCOME AMICCOM Electronics Corporation
 18:7C:0B,RuckusWi Ruckus Wireless
 18:7C:81,ValeoVis Valeo Vision Systems
+18:7C:AA,"ChinaMob China Mobile Group Device Co.,Ltd."
 18:7E:B9,"Apple Apple, Inc."
 18:7E:D5,shenzhen shenzhen kaism technology Co. Ltd
 18:80:90,"Cisco Cisco Systems, Inc"
 18:80:CE,Barberry Barberry Solutions Ltd
 18:80:F5,"Alcatel- Alcatel-Lucent Shanghai Bell Co., Ltd"
 18:81:0E,"Apple Apple, Inc."
 18:82:19,AlibabaC Alibaba Cloud Computing Ltd.
 18:82:8C,Arcadyan Arcadyan Corporation
 18:83:31,"SamsungE Samsung Electronics Co.,Ltd"
 18:83:BF,Arcadyan Arcadyan Technology Corporation
 18:84:10,CoreTrus CoreTrust Inc.
+18:84:C1,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 18:86:3A,DigitalA Digital Art System
 18:86:AC,NokiaDan Nokia Danmark A/S
 18:87:40,XiaomiCo Xiaomi Communications Co Ltd
 18:87:96,HTC HTC Corporation
 18:88:57,BeijingJ Beijing Jinhong Xi-Dian Information Technology Corp.
 18:89:5B,"SamsungE Samsung Electronics Co.,Ltd"
 18:89:A0,"WuhanFun Wuhan Funshion Online Technologies Co.,Ltd"
@@ -19605,15 +19711,17 @@
 18:A5:9C:80:00:00/28,Residenc Residence Control Ltd
 18:A5:9C:90:00:00/28,"estunaut estun automation co.,ltd"
 18:A5:9C:A0:00:00/28,ErbaLach Erba Lachema s.r.o.
 18:A5:9C:B0:00:00/28,Cal-Comp Cal-Comp Industria E Comercio De Eletronicos E Informatica Ltda
 18:A5:9C:C0:00:00/28,BlueEyes BlueEyes Technology
 18:A5:9C:D0:00:00/28,Annapurn Annapurna labs
 18:A5:9C:E0:00:00/28,BMCMesss BMC Messsysteme GmbH
+18:A5:FF,Arcadyan Arcadyan Corporation
 18:A6:F7,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
+18:A7:88,Shenzhen Shenzhen MEK Intellisys Pte Ltd
 18:A7:F1,"QingdaoH Qingdao Haier Technology Co.,Ltd"
 18:A9:05,HewlettP Hewlett Packard
 18:A9:58,"Provisio Provision Thai Co., Ltd."
 18:A9:9B,Dell Dell Inc.
 18:A9:A6,Nebra Nebra Ltd
 18:AA:0F,"HuaweiDe Huawei Device Co., Ltd."
 18:AA:1E,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
@@ -19623,14 +19731,15 @@
 18:AB:F5,UltraEle Ultra Electronics Electrics
 18:AC:9E,ItelMobi Itel Mobile Limited
 18:AD:4D,Polostar Polostar Technology Corporation
 18:AE:BB,SiemensC Siemens Convergence Creators GmbH&Co.KG
 18:AF:61,"Apple Apple, Inc."
 18:AF:8F,"Apple Apple, Inc."
 18:AF:9F,DIGITRON DIGITRONIC Automationsanlagen GmbH
+18:AF:A1,"Shenzhen Shenzhen Yifang Network Technology Co., Ltd."
 18:B1:69,Sonicwal Sonicwall
 18:B1:85,"QiaoInfo Qiao Information Technology (Zhengzhou) Co., Ltd."
 18:B2:09,"TorreyPi Torrey Pines Logic, Inc"
 18:B3:BA,Netlogic Netlogic AB
 18:B4:30,NestLabs Nest Labs Inc.
 18:B5:91,I-Storm
 18:B6:CC,We We Corporation Inc.
@@ -19711,14 +19820,15 @@
 18:D7:93:D0:00:00/28,KrakenTe Kraken Technologies Ltd
 18:D7:93:E0:00:00/28,Teegarde Teegarden Applied Science Inc
 18:D9:49,"QvisLabs Qvis Labs, LLC"
 18:D9:8F,"HuaweiDe Huawei Device Co., Ltd."
 18:D9:EF,Shuttle Shuttle Inc.
 18:DB:F2,Dell Dell Inc.
 18:DC:56,"YulongCo Yulong Computer Telecommunication Scientific (Shenzhen) Co.,Ltd"
+18:DE:50,TuyaSmar Tuya Smart Inc.
 18:DE:D7,"HuaweiTe Huawei Technologies Co.,Ltd"
 18:DF:B4,"BosungPo Bosung Powertec Co.,Ltd."
 18:DF:C1,Aetheros
 18:E1:CA,wanze
 18:E1:DE,"ChengduC Chengdu ChipIntelli Technology Co., Ltd"
 18:E2:15,Nokia
 18:E2:88,STTCondi STT Condigi
@@ -19726,34 +19836,37 @@
 18:E2:C2,"SamsungE Samsung Electronics Co.,Ltd"
 18:E3:BC,TCTmobil TCT mobile ltd
 18:E7:28,"Cisco Cisco Systems, Inc"
 18:E7:77,"vivoMobi vivo Mobile Communication Co., Ltd."
 18:E7:B0,"Apple Apple, Inc."
 18:E7:F4,"Apple Apple, Inc."
 18:E8:0F,VikingEl Viking Electronics Inc.
-18:E8:29,Ubiquiti Ubiquiti Networks Inc.
+18:E8:29,Ubiquiti Ubiquiti Inc
 18:E8:DD,Modulete Moduletek
 18:E9:1D,"HuaweiTe Huawei Technologies Co.,Ltd"
 18:EC:E7,Buffalo Buffalo.Inc
 18:EE:69,"Apple Apple, Inc."
 18:EE:86,"NovatelW Novatel Wireless Solutions, Inc."
 18:EF:3A,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 18:EF:63,"Cisco Cisco Systems, Inc"
 18:F0:E4,XiaomiCo Xiaomi Communications Co Ltd
 18:F1:45,NetCommW NetComm Wireless Limited
 18:F1:8E,ChipERTe ChipER Technology co. ltd
 18:F1:D8,"Apple Apple, Inc."
 18:F2:2C,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 18:F2:92,Shannon Shannon Systems
 18:F4:6A,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+18:F4:6B,TelenorC Telenor Connexion AB
 18:F6:43,"Apple Apple, Inc."
 18:F6:50,Multimed Multimedia Pacific Limited
+18:F6:97,"AxiomMem Axiom Memory Solutions, Inc."
 18:F7:6B,"Zhejiang Zhejiang Winsight Technology CO.,LTD"
 18:F8:7A,i3Intern i3 International Inc.
 18:F8:7F,"WhaYuInd Wha Yu Industrial Co., Ltd."
+18:F9:35,"Cisco Cisco Systems, Inc"
 18:F9:C4,BAE BAE Systems
 18:FA:6F,ISCappli ISC applied systems corp
 18:FA:B7,"Apple Apple, Inc."
 18:FB:7B,Dell Dell Inc.
 18:FC:26,QorvoInt Qorvo International Pte. Ltd.
 18:FC:9F,"ChangheE Changhe Electronics Co., Ltd."
 18:FD:74,Routerbo Routerboard.com
@@ -19820,15 +19933,15 @@
 1C:21:D1:10:00:00/28,Ognios Ognios GmbH
 1C:21:D1:20:00:00/28,VaraaniW Varaani Works Oy
 1C:21:D1:30:00:00/28,"Microvie Microview Science and Technology Co.,Ltd"
 1C:21:D1:40:00:00/28,Scientif Scientific-Production Enterprise Dynamics
 1C:21:D1:50:00:00/28,B-Scada B-Scada Inc.
 1C:21:D1:60:00:00/28,"WuhanTie Wuhan TieChi Detection Technology Co., Ltd."
 1C:21:D1:70:00:00/28,Soundtra Soundtrack Your Brand Sweden AB
-1C:21:D1:80:00:00/28,Reliatro Reliatronics Inc.
+1C:21:D1:80:00:00/28,"Cleavela Cleaveland/Price, Inc."
 1C:21:D1:90:00:00/28,DynojetR Dynojet Research
 1C:21:D1:A0:00:00/28,LgCns Lg Cns
 1C:21:D1:B0:00:00/28,GlobalDe Global Design Solutions Ltd
 1C:21:D1:C0:00:00/28,Private
 1C:21:D1:D0:00:00/28,"Liscotec Liscotech System Co., Ltd."
 1C:21:D1:E0:00:00/28,p2-plus p2-plus inc.
 1C:21:D1:F0:00:00/28,Private
@@ -19839,14 +19952,15 @@
 1C:24:EB,Burlywoo Burlywood
 1C:25:E1,ChinaMob China Mobile IOT Company Limited
 1C:27:04,zte zte corporation
 1C:27:DD,"DatangGo Datang Gohighsec(zhejiang)Information Technology Co.,Ltd."
 1C:28:AF,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 1C:2A:8B,Nokia
 1C:2A:A3,"Shenzhen Shenzhen HongRui Optical Technology Co., Ltd."
+1C:2A:B0,"BeijingX Beijing Xiaomi Electronics Co.,Ltd"
 1C:2C:E0,Shanghai Shanghai Mountain View Silicon
 1C:2E:1B,"SuzhouTr Suzhou Tremenet Communication Technology Co., Ltd."
 1C:30:08,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 1C:32:83,"COMTTIIn COMTTI Intelligent Technology(Shenzhen) Co., Ltd."
 1C:33:0E,PernixDa PernixData
 1C:33:4D,ITSTelec ITS Telecom
 1C:34:77,Innovati Innovation Wireless
@@ -19857,14 +19971,15 @@
 1C:37:BF,Cloudium Cloudium Systems Ltd.
 1C:39:29,Ohsung
 1C:39:47,"CompalIn Compal Information (Kunshan) Co., Ltd."
 1C:39:8A,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 1C:3A:4F,"AccuSpec AccuSpec Electronics, LLC"
 1C:3A:60,RuckusWi Ruckus Wireless
 1C:3A:DE,"SamsungE Samsung Electronics Co.,Ltd"
+1C:3B:62,HMDGloba HMD Global Oy
 1C:3B:8F,Selve Selve GmbH & Co. KG
 1C:3B:F3,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 1C:3C:D4,"HuaweiTe Huawei Technologies Co.,Ltd"
 1C:3D:2F,"HuaweiTe Huawei Technologies Co.,Ltd"
 1C:3D:E7,"SigmaKok Sigma Koki Co.,Ltd."
 1C:3E:84,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 1C:40:24,Dell Dell Inc.
@@ -19942,21 +20057,23 @@
 1C:63:BF,"Shenzhen Shenzhen Broadtel Telecom Co.,Ltd"
 1C:64:99,Comtrend Comtrend Corporation
 1C:65:9D,LiteonTe Liteon Technology Corporation
 1C:66:6D,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 1C:66:AA,"SamsungE Samsung Electronics Co.,Ltd"
 1C:67:4A,zte zte corporation
 1C:67:58,"HuaweiTe Huawei Technologies Co.,Ltd"
+1C:67:60,Phonesui Phonesuite
 1C:68:7E,Shenzhen Shenzhen Qihu Intelligent Technology Company Limited
 1C:69:7A,"EliteGro EliteGroup Computer Systems Co., LTD"
 1C:69:A5,BlackBer BlackBerry RTS
 1C:6A:76,"Apple Apple, Inc."
 1C:6A:7A,"Cisco Cisco Systems, Inc"
 1C:6B:CA,"Mitsunam Mitsunami Co., Ltd."
 1C:6E:4C,"Logistic Logistic Service & Engineering Co.,Ltd"
+1C:6E:74,EnOceanE EnOcean Edge Inc.
 1C:6E:76,QuarionT Quarion Technology Inc
 1C:6E:E6,Nhnetwor Nhnetworks
 1C:6F:65,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 1C:70:22,"MurataMa Murata Manufacturing Co., Ltd."
 1C:70:C9,"JiangsuA Jiangsu Aisida Electronic Co., Ltd"
 1C:71:25,"Apple Apple, Inc."
 1C:72:1D,Dell Dell Inc.
@@ -19970,14 +20087,15 @@
 1C:77:F6,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 1C:78:39,"Shenzhen Shenzhen Tencent Computer System Co., Ltd."
 1C:78:4E,ChinaMob China Mobile Iot Limited company
 1C:7B:21,Sony Sony Corporation
 1C:7B:23,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
 1C:7C:11,Eid
 1C:7C:45,"VitekInd Vitek Industrial Video Products, Inc."
+1C:7C:98,"NECPlatf NEC Platforms, Ltd."
 1C:7C:C7,Coriant Coriant GmbH
 1C:7D:22,FUJIFILM FUJIFILM Business Innovation Corp.
 1C:7E:51,3bumenco 3bumen.com
 1C:7E:E5,D-LinkIn D-Link International
 1C:7F:2C,"HuaweiTe Huawei Technologies Co.,Ltd"
 1C:82:59,IEEERegi IEEE Registration Authority
 1C:82:59:00:00:00/28,"Shandong Shandong Luneng Intelligence Technology CO., Ltd"
@@ -19994,14 +20112,15 @@
 1C:82:59:B0:00:00/28,"KeyWestN KeyWest Networks, Inc"
 1C:82:59:C0:00:00/28,Evondos Evondos Oy
 1C:82:59:D0:00:00/28,"AppliedC Applied Concepts, Inc."
 1C:82:59:E0:00:00/28,Microtro Microtronics Engineering GmbH
 1C:83:41,HefeiBit Hefei Bitland Information Technology Co.Ltd
 1C:83:B0,LinkedIP Linked IP GmbH
 1C:84:64,FormosaW Formosa Wireless Communication Corp.
+1C:86:0B,"Guangdon Guangdong Taiying Technology Co.,Ltd"
 1C:86:82,"Apple Apple, Inc."
 1C:86:9A,"SamsungE Samsung Electronics Co.,Ltd"
 1C:86:AD,"Mct Mct Co., Ltd."
 1C:87:2C,ASUSTekC ASUSTek COMPUTER INC.
 1C:87:74:00:00:00/28,PhilipsP Philips Personal Health Solutions
 1C:87:74:10:00:00/28,Sigfox
 1C:87:74:20:00:00/28,Nichigak Nichigaku
@@ -20087,19 +20206,19 @@
 1C:98:C1,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 1C:98:EC,HewlettP Hewlett Packard Enterprise
 1C:99:4C,"MurataMa Murata Manufacturing Co., Ltd."
 1C:99:57,IntelCor Intel Corporate
 1C:9C:26,ZoovelTe Zoovel Technologies
 1C:9C:8C,JuniperN Juniper Networks
 1C:9D:3E,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
-1C:9D:72,Technico Technicolor CH USA Inc.
+1C:9D:72,VantivaU Vantiva USA LLC
 1C:9D:C2,Espressi Espressif Inc.
 1C:9E:46,"Apple Apple, Inc."
 1C:9E:CB,BeijingN Beijing Nari Smartchip Microelectronics Company Limited
-1C:9E:CC,Technico Technicolor CH USA Inc.
+1C:9E:CC,VantivaU Vantiva USA LLC
 1C:9F:4E,CooseaGr Coosea Group (Hk) Company Limited
 1C:A0:B8,"HonHaiPr Hon Hai Precision Industry Co., Ltd."
 1C:A0:D3,IEEERegi IEEE Registration Authority
 1C:A0:D3:00:00:00/28,Tekhnotr OOO Tekhnotronika
 1C:A0:D3:10:00:00/28,Jabilcir Jabil circuit italia srl
 1C:A0:D3:20:00:00/28,"NovTech NovTech, Inc."
 1C:A0:D3:30:00:00/28,Savelec
@@ -20202,14 +20321,16 @@
 1C:C1:BC,"YichipMi Yichip Microelectronics (Hangzhou) Co.,Ltd"
 1C:C1:DE,HewlettP Hewlett Packard
 1C:C3:16,"XiamenMi Xiamen Milesight IoT Co., Ltd."
 1C:C3:EB,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 1C:C5:86,Absolute Absolute Acoustics
 1C:C6:3C,Arcadyan Arcadyan Technology Corporation
 1C:C7:2D,"Shenzhen Shenzhen Huapu Digital CO.,Ltd"
+1C:C9:92,"HonorDev Honor Device Co., Ltd."
+1C:CA:41,Ao
 1C:CA:E3,IEEERegi IEEE Registration Authority
 1C:CA:E3:00:00:00/28,Private
 1C:CA:E3:10:00:00/28,PgaElect Pga Electronic
 1C:CA:E3:20:00:00/28,Insigma Insigma Inc
 1C:CA:E3:30:00:00/28,"Shenzhen Shenzhen Smart Device Technology Co.,LTD"
 1C:CA:E3:40:00:00/28,"SunrayMe Sunray Medical Apparatus Co.,Ltd."
 1C:CA:E3:50:00:00/28,TengFeng
@@ -20285,14 +20406,15 @@
 1C:FD:08:D0:00:00/28,"TianjinK Tianjin Keyvia Electric Co.,Ltd"
 1C:FD:08:E0:00:00/28,MeshboxF Meshbox Foundation Pte. Ltd.
 1C:FE:2B,AmazonTe Amazon Technologies Inc.
 1C:FE:A7,IDentyte IDentytech Solutins Ltd.
 1C:FF:59,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 20:01:4F,LineaRes Linea Research Ltd
 20:02:AF,"MurataMa Murata Manufacturing Co., Ltd."
+20:02:FE,"Hangzhou Hangzhou Dangbei Network Technology Co., Ltd"
 20:04:0F,Dell Dell Inc.
 20:04:F3,"HonorDev Honor Device Co., Ltd."
 20:05:05,RadmaxCo Radmax Communication Private Limited
 20:05:E8,InProMed OOO InProMedia
 20:08:89,zte zte corporation
 20:08:ED,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:0A:0D,IEEERegi IEEE Registration Authority
@@ -20309,50 +20431,56 @@
 20:0A:0D:A0:00:00/28,Irsap
 20:0A:0D:B0:00:00/28,AmazonTe Amazon Technologies Inc.
 20:0A:0D:C0:00:00/28,sehwa
 20:0A:0D:D0:00:00/28,BentlyEL Bently & EL Co. Ltd.
 20:0A:0D:E0:00:00/28,"HANGZHOU HANGZHOU DANGBEI NETWORK TECH.Co.,Ltd"
 20:0A:5E,"Xiangsha Xiangshan Giant Eagle Technology Developing Co., Ltd."
 20:0B:16,TexasIns Texas Instruments
+20:0B:C5,"Cisco Cisco Systems, Inc"
 20:0B:C7,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:0B:CF,"Nintendo Nintendo Co.,Ltd"
 20:0C:86,GXIndia GX India Pvt Ltd
 20:0C:C8,Netgear
 20:0D:B0,"Shenzhen Shenzhen Four Seas Global Link Network Technology Co., Ltd."
 20:0E:2B,"Apple Apple, Inc."
 20:0E:95,Iec–Tc9W Iec – Tc9 Wg43
 20:0F:70,Foxtech
 20:10:7A,"GemtekTe Gemtek Technology Co., Ltd."
 20:11:4E,MeteRSit MeteRSit S.R.L.
 20:12:57,MostLuck Most Lucky Trading Ltd
 20:12:D5,Scientec Scientech Materials Corporation
 20:13:E0,"SamsungE Samsung Electronics Co.,Ltd"
+20:15:82,"Apple Apple, Inc."
 20:16:3D,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 20:16:42,Microsof Microsoft Corporation
 20:16:B9,IntelCor Intel Corporate
 20:16:D8,LiteonTe Liteon Technology Corporation
 20:17:42,LGElectr LG Electronics
+20:17:46,"Paradrom Paradromics, Inc."
 20:18:0E,"Shenzhen Shenzhen Sunchip Technology Co., Ltd"
 20:1A:06,"CompalIn Compal Information (Kunshan) Co., Ltd."
 20:1A:94,"Apple Apple, Inc."
 20:1B:88,"Dongguan Dongguan Liesheng Electronic Co., Ltd."
 20:1B:C9,JuniperN Juniper Networks
+20:1C:3A,"Nintendo Nintendo Co.,Ltd"
 20:1D:03,Elatec Elatec GmbH
 20:1E:88,IntelCor Intel Corporate
 20:1F:31,IntenoBr Inteno Broadband Technology AB
 20:1F:3B,"Google Google, Inc."
 20:1F:54,"Raisecom Raisecom Technology CO., LTD"
 20:20:27,Shenzhen Shenzhen Sundray Technologies Company Limited
+20:21:41,Universa Universal Electronics BV
 20:21:A5,LGElectr LG Electronics (Mobile Communications)
 20:25:64,Pegatron Pegatron Corporation
 20:25:98,Teleview
 20:25:D2,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 20:26:81,TecnoMob Tecno Mobile Limited
 20:28:3E,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:28:BC,"Visionsc Visionscape Co,. Ltd."
+20:29:B9,"Ikotekte Ikotek technology SH Co., Ltd"
 20:2A:C5,Petite-E Petite-En
 20:2B:20,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 20:2B:C1,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:2C:B7,KongYueE Kong Yue Electronics & Information Industry (Xinhui) Ltd.
 20:2D:07,"SamsungE Samsung Electronics Co.,Ltd"
 20:2D:23,Collinea Collinear Networks Inc.
 20:2D:F8,DigitalM Digital Media Cartridge Ltd.
@@ -20368,14 +20496,15 @@
 20:36:D7,"Shanghai Shanghai Reacheng Communication Technology Co.,Ltd"
 20:37:06,"Cisco Cisco Systems, Inc"
 20:37:A5,"Apple Apple, Inc."
 20:37:BC,KuipersE Kuipers Electronic Engineering BV
 20:39:56,HMDGloba HMD Global Oy
 20:3A:07,"Cisco Cisco Systems, Inc"
 20:3A:43,IntelCor Intel Corporate
+20:3A:EB,zte zte corporation
 20:3A:EF,Sivantos Sivantos GmbH
 20:3B:69,"vivoMobi vivo Mobile Communication Co., Ltd."
 20:3C:AE,"Apple Apple, Inc."
 20:3C:C0,"BeijingT Beijing Tosee Technology Co., Ltd."
 20:3D:66,"ARRISGro ARRIS Group, Inc."
 20:3D:B2,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:3D:BD,LGInnote LG Innotek
@@ -20416,15 +20545,15 @@
 20:5B:2A,Private
 20:5B:5E,"Shenzhen Shenzhen Wonhe Technology Co., Ltd"
 20:5C:FA,"Yangzhou Yangzhou ChangLian Network Technology Co,ltd."
 20:5D:47,"vivoMobi vivo Mobile Communication Co., Ltd."
 20:5E:64,"HuaweiDe Huawei Device Co., Ltd."
 20:5E:97,Nokia
 20:5E:F7,"SamsungE Samsung Electronics Co.,Ltd"
-20:5F:3D,Cambridg Cambridge Communication Systems Ltd
+20:5F:3D,Adtran Adtran Inc
 20:62:74,Microsof Microsoft Corporation
 20:62:96,"Shenzhen Shenzhen Malio Technology Co.,Ltd"
 20:63:5F,Abeeway
 20:64:32,"SamsungE Samsung Electro Mechanics Co., Ltd."
 20:64:CB,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 20:64:DE,"SunitecE Sunitec Enterprise Co.,Ltd"
 20:65:8E,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -20440,14 +20569,15 @@
 20:6A:FF,AtlasEle Atlas Elektronik UK Limited
 20:6B:E7,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 20:6C:8A,"ExtremeN Extreme Networks, Inc."
 20:6D:31,Firewall Firewalla Inc
 20:6E:9C,"SamsungE Samsung Electronics Co.,Ltd"
 20:6F:EC,BraemacC Braemac CA LLC
 20:71:9E,"SFTechno SF Technology Co.,Ltd"
+20:72:A9,"BeijingX Beijing Xiaomi Electronics Co.,Ltd"
 20:73:55,"ARRISGro ARRIS Group, Inc."
 20:74:54,"vivoMobi vivo Mobile Communication Co., Ltd."
 20:74:CF,"Shenzhen Shenzhen Voxtech Co.,Ltd"
 20:76:00,"Actionte Actiontec Electronics, Inc"
 20:76:8F,"Apple Apple, Inc."
 20:76:93,LenovoBe Lenovo (Beijing) Limited.
 20:77:59,"OpticalN Optical Network Video Technologies (Shenzhen) Co., Ltd."
@@ -20482,28 +20612,31 @@
 20:85:93:B0:00:00/28,IOGProdu IOG Products LLC
 20:85:93:C0:00:00/28,Reglopla Regloplas AG
 20:85:93:D0:00:00/28,"Shanghai Shanghai Kenmyond Industrial Network Equipment Co.,Ltd"
 20:85:93:E0:00:00/28,Dynaudio
 20:87:56,Siemens Siemens Ag
 20:87:AC,AESmotom AES motomation
 20:87:EC,"HuaweiTe Huawei Technologies Co.,Ltd"
+20:88:10,Dell Dell Inc.
 20:89:6F,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 20:89:84,"CompalIn Compal Information (Kunshan) Co., Ltd."
 20:89:86,zte zte corporation
 20:89:8A,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 20:8B:37,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 20:8B:D1,NXPSemic NXP Semiconductor (Tianjin) LTD.
 20:8C:47,Tenstorr Tenstorrent Inc
 20:8C:86,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:90:6F,"Shenzhen Shenzhen Tencent Computer System Co., Ltd."
 20:91:48,TexasIns Texas Instruments
 20:91:8A,Profalux
 20:91:D9,IM I'M Spa
+20:91:DF,"Apple Apple, Inc."
 20:93:4D,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 20:96:8A,"ChinaMob China Mobile (Hangzhou) Information Technology Co., Ltd."
+20:97:27,Teltonik Teltonika Networks Uab
 20:98:D8,"Shenzhen Shenzhen Yingdakang Technology CO., LTD"
 20:9A:7D,Sagemcom Sagemcom Broadband SAS
 20:9A:E9,"Volacomm Volacomm Co., Ltd"
 20:9B:A5,"JIAXINGG JIAXING GLEAD Electronics Co.,Ltd"
 20:9B:CD,"Apple Apple, Inc."
 20:9B:E6,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 20:9C:B4,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
@@ -20533,16 +20666,19 @@
 20:B0:01,Technico Technicolor Delivery Technologies Belgium NV
 20:B0:F7,Enclustr Enclustra GmbH
 20:B3:99,Enterasy Enterasys
 20:B5:C6,MimosaNe Mimosa Networks
 20:B7:30,"TeconGro TeconGroup, Inc"
 20:B7:80,"ToshibaV Toshiba Visual Solutions Corporation Co.,Ltd"
 20:B7:C0,OMICRONe OMICRON electronics GmbH
+20:B8:2B,Sagemcom Sagemcom Broadband SAS
 20:B8:68,"Motorola Motorola Mobility LLC, a Lenovo Company"
+20:BA:36,u-blox u-blox AG
 20:BB:76,COLGIOVA COL GIOVANNI PAOLO SpA
+20:BB:BC,"Hangzhou Hangzhou Ezviz Software Co.,Ltd."
 20:BB:C0,"Cisco Cisco Systems, Inc"
 20:BB:C6,JabilCir Jabil Circuit Hungary Ltd.
 20:BE:CD,eero eero inc.
 20:BF:DB,Dvl
 20:C0:47,Verizon
 20:C0:6D,"Shenzhen Shenzhen Spacetek Technology Co.,Ltd"
 20:C1:9B,IntelCor Intel Corporate
@@ -20596,14 +20732,15 @@
 20:DE:88,ICRealti IC Realtime LLC
 20:DF:3F,"NanjingS Nanjing SAC Power Grid Automation Co., Ltd."
 20:DF:73,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:DF:B9,"Google Google, Inc."
 20:E0:9C,Nokia
 20:E2:A8,"Apple Apple, Inc."
 20:E4:07,Spark Spark srl
+20:E4:6F,"vivoMobi vivo Mobile Communication Co., Ltd."
 20:E5:2A,Netgear
 20:E5:64,"ARRISGro ARRIS Group, Inc."
 20:E6:DF,eero eero inc.
 20:E7:91,"SiemensH Siemens Healthcare Diagnostics, Inc"
 20:E7:B6,"Universa Universal Electronics, Inc."
 20:E8:74,"Apple Apple, Inc."
 20:E8:82,zte zte corporation
@@ -20619,14 +20756,15 @@
 20:F3:A3,"HuaweiTe Huawei Technologies Co.,Ltd"
 20:F4:1B,"Shenzhen Shenzhen Bilian electronic CO.,LTD"
 20:F4:4F,Nokia
 20:F4:52,Shanghai Shanghai IUV Software Development Co. Ltd
 20:F4:78,XiaomiCo Xiaomi Communications Co Ltd
 20:F5:10,CodexDig Codex Digital Limited
 20:F5:43,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
+20:F5:97,"Maasiv Maasiv, LLC"
 20:F7:7C,"vivoMobi vivo Mobile Communication Co., Ltd."
 20:F8:5E,DeltaEle Delta Electronics
 20:FA:BB,Cambridg Cambridge Executive Limited
 20:FA:DB,"HuahaoKu Huahao Kunpeng Technology (chengDu) Co.,Ltd."
 20:FD:F1,3ComEuro 3Com Europe Ltd
 20:FE:00,AmazonTe Amazon Technologies Inc.
 20:FE:CD,SystemIn System In Frontier Inc.
@@ -20671,15 +20809,15 @@
 24:15:10:10:00:00/28,SMaBiT SMaBiT GmbH
 24:15:10:20:00:00/28,NileGlob Nile Global Inc
 24:15:10:30:00:00/28,Kaiyun
 24:15:10:40:00:00/28,Annapurn Annapurna labs
 24:15:10:50:00:00/28,"GanzhouD Ganzhou Dehuida Technology Co., Ltd"
 24:15:10:60:00:00/28,Shandong Shandong Kehui Power Automation Co. Ltd.
 24:15:10:70:00:00/28,"SuZhouA- SuZhou A-rack Information Technology Co.,Ltd"
-24:15:10:80:00:00/28,Private
+24:15:10:80:00:00/28,"Medicomp Medicomp, Inc"
 24:15:10:90:00:00/28,TopgolfS Topgolf Sweden AB
 24:15:10:A0:00:00/28,"Unitronu Unitronux(Shenzhen) Intelligence Technology Co.,Ltd"
 24:15:10:B0:00:00/28,"Teknic Teknic, Inc."
 24:15:10:C0:00:00/28,"Shenzhen Shenzhen Xtooltech Co., Ltd"
 24:15:10:D0:00:00/28,HelenTro Helen of Troy
 24:15:10:E0:00:00/28,"Satellit Satellite Link Technology CO.,LTD"
 24:15:51,"HuaweiDe Huawei Device Co., Ltd."
@@ -20699,18 +20837,20 @@
 24:1E:EB,"Apple Apple, Inc."
 24:1F:2C,"Calsys Calsys, Inc."
 24:1F:A0,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:1F:BD,"ExtremeN Extreme Networks, Inc."
 24:20:C7,Sagemcom Sagemcom Broadband SAS
 24:21:24,Nokia
 24:21:AB,Sony Sony Corporation
+24:23:61,"vivoMobi vivo Mobile Communication Co., Ltd."
 24:24:0E,"Apple Apple, Inc."
 24:26:42,SHARP SHARP Corporation.
 24:26:BA,"Shenzhen Shenzhen Toptel Technology Co., Ltd."
 24:26:D6,"HuaweiTe Huawei Technologies Co.,Ltd"
+24:27:30,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 24:28:FD,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 24:29:34,"Google Google, Inc."
 24:29:FE,KYOCERA KYOCERA Corporation
 24:2A:04,"Cisco Cisco Systems, Inc"
 24:2C:FE,"Zhejiang Zhejiang Tmall Technology Co., Ltd."
 24:2E:02,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:2E:90,"PalitMic Palit Microsystems, Ltd"
@@ -20734,17 +20874,19 @@
 24:43:E2,DASANNet DASAN Network Solutions
 24:44:27,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:45:6B,"HuaweiDe Huawei Device Co., Ltd."
 24:45:97,GEMUEGeb GEMUE Gebr. Mueller Apparatebau
 24:46:C8,"Motorola Motorola Mobility LLC, a Lenovo Company"
 24:46:E4,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:47:0E,Pentroni PentronicAB
+24:48:45,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 24:49:7B,Innovati Innovative Converged Devices Inc
 24:4B:03,"SamsungE Samsung Electronics Co.,Ltd"
 24:4B:81,"SamsungE Samsung Electronics Co.,Ltd"
+24:4B:F1,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:4B:FE,ASUSTekC ASUSTek COMPUTER INC.
 24:4C:07,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:4C:AB,Espressi Espressif Inc.
 24:4C:E3,AmazonTe Amazon Technologies Inc.
 24:4E:7B,IEEERegi IEEE Registration Authority
 24:4E:7B:00:00:00/28,TekelekE Tekelek Europe Ltd
 24:4E:7B:10:00:00/28,sonoscap sonoscape
@@ -20763,15 +20905,15 @@
 24:4E:7B:E0:00:00/28,"WithWinT WithWin Technology ShenZhen CO.,LTD"
 24:4F:1D,iRule iRule LLC
 24:52:6A,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 24:53:BF,Enernet
 24:58:6E,zte zte corporation
 24:58:80,Vizeo
 24:59:0B,WhiteSky White Sky Inc. Limited
-24:5A:4C,Ubiquiti Ubiquiti Networks Inc.
+24:5A:4C,Ubiquiti Ubiquiti Inc
 24:5A:B5,"SamsungE Samsung Electronics Co.,Ltd"
 24:5B:83,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 24:5B:A7,"Apple Apple, Inc."
 24:5B:F0,"Liteon Liteon, Inc."
 24:5C:BF,Ncse
 24:5C:C5,"HuaweiDe Huawei Device Co., Ltd."
 24:5C:CB,"AXIeCons AXIe Consortium, Inc."
@@ -20808,28 +20950,30 @@
 24:69:3E,innodisk innodisk Corporation
 24:69:4A,Jasmine Jasmine Systems Inc.
 24:69:68,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 24:69:8E,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 24:69:A5,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:6A:AB,IT-ISInt IT-IS International
 24:6C:60,"HuaweiDe Huawei Device Co., Ltd."
+24:6C:84,"Cisco Cisco Systems, Inc"
 24:6C:8A,YUKAIEng YUKAI Engineering
 24:6E:96,Dell Dell Inc.
 24:6F:28,Espressi Espressif Inc.
 24:6F:8C,"HuaweiDe Huawei Device Co., Ltd."
 24:71:52,Dell Dell Inc.
 24:71:89,TexasIns Texas Instruments
 24:72:4A,NileGlob Nile Global Inc
 24:72:60,IOTTECH IOTTECH Corp
 24:74:F7,GoPro
 24:75:3A,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 24:76:25,TexasIns Texas Instruments
 24:76:56,"Shanghai Shanghai Net Miles Fiber Optics Technology Co., LTD."
 24:76:7D,CiscoSPV Cisco SPVTG
 24:77:03,IntelCor Intel Corporate
+24:78:23,"Panasoni Panasonic Entertainment & Communication Co., Ltd."
 24:79:2A,RuckusWi Ruckus Wireless
 24:79:EF,"Greenpac Greenpacket Berhad, Taiwan"
 24:79:F3,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 24:79:F8,KUPSONsp KUPSON spol. s r.o.
 24:7C:4C,HermanMi Herman Miller
 24:7D:4D,TexasIns Texas Instruments
 24:7E:12,"Cisco Cisco Systems, Inc"
@@ -20843,33 +20987,35 @@
 24:82:8A,ProwaveT Prowave Technologies Ltd.
 24:84:98,"BeijingJ Beijing Jiaoda Microunion Tech.Co.,Ltd."
 24:86:F4,"Ctek Ctek, Inc."
 24:87:07,SEnergy SEnergy Corporation
 24:88:94,shenzhen shenzhen lensun Communication Technology LTD
 24:8A:07,"Mellanox Mellanox Technologies, Inc."
 24:8B:E0,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
+24:90:38,Universa Universal Biosensors Pty Ltd
 24:91:BB,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:92:0E,"SamsungE Samsung Electronics Co.,Ltd"
 24:93:CA,Voxtroni Voxtronic Austria
 24:94:42,"OpenRoad Open Road Solutions , Inc."
 24:94:93,FibRSolG FibRSol Global Network Limited
 24:94:94,HongKong Hong Kong Bouffalo Lab Limited
 24:94:CB,"ARRISGro ARRIS Group, Inc."
 24:95:04,Sfr
+24:95:2F,"Google Google, Inc."
 24:97:45,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:97:ED,Techvisi Techvision Intelligent Technology Limited
 24:9A:C8,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 24:9A:D8,"YealinkX Yealink(Xiamen) Network Technology Co.,Ltd."
 24:9E:AB,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:9F:89,TexasIns Texas Instruments
 24:A0:74,"Apple Apple, Inc."
 24:A1:60,Espressi Espressif Inc.
 24:A2:E1,"Apple Apple, Inc."
-24:A4:2C,KOUKAAM KOUKAAM a.s.
-24:A4:3C,Ubiquiti Ubiquiti Networks Inc.
+24:A4:2C,NETIOpro NETIO products a.s.
+24:A4:3C,Ubiquiti Ubiquiti Inc
 24:A4:87,"HuaweiDe Huawei Device Co., Ltd."
 24:A4:95,ThalesCa Thales Canada Inc.
 24:A5:2C,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:A5:34,SynTrust SynTrust Tech International Ltd.
 24:A6:5E,zte zte corporation
 24:A6:FA,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 24:A7:99,"HuaweiDe Huawei Device Co., Ltd."
@@ -20889,19 +21035,20 @@
 24:B7:2A,ChinaDra China Dragon Technology Limited
 24:B7:DA,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 24:B8:8C,"Crenus Crenus Co.,Ltd."
 24:B8:D2,"OpzoonTe Opzoon Technology Co.,Ltd."
 24:BA:13,RisoKaga Riso Kagaku Corporation
 24:BA:30,"Technica Technical Consumer Products, Inc."
 24:BB:C1,Absolute Absolute Analysis
+24:BB:C9,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 24:BC:82,"DaliWire Dali Wireless, Inc."
 24:BC:F8,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:BE:05,HewlettP Hewlett Packard
 24:BE:18,Dadoutek Dadoutek Company Limited
-24:BF:74,Private
+24:BF:74,Hamamats Hamamatsu Photonics K.K.
 24:C0:B3,Rsf
 24:C1:7A,"BeijingI Beijing Iactive Network Co.,Ltd"
 24:C1:BD,"CrrcDali Crrc Dalian R&D Co.,Ltd."
 24:C3:F9,Securita Securitas Direct AB
 24:C4:2F,PhilipsL Philips Lifeline
 24:C4:4A,zte zte corporation
 24:C6:13,"SamsungE Samsung Electronics Co.,Ltd"
@@ -20916,14 +21063,15 @@
 24:CD:8D,"MurataMa Murata Manufacturing Co., Ltd."
 24:CE:33,AmazonTe Amazon Technologies Inc.
 24:CF:21,"Shenzhen Shenzhen State Micro Technology Co., Ltd"
 24:CF:24,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 24:D0:DF,"Apple Apple, Inc."
 24:D1:3F,"Mexus Mexus Co.,Ltd"
 24:D2:CC,SmartDri SmartDrive Systems Inc.
+24:D3:37,XiaomiCo Xiaomi Communications Co Ltd
 24:D3:F2,zte zte corporation
 24:D5:1C,"Zhongtia Zhongtian broadband technology co., LTD"
 24:D7:6B,Syntroni Syntronic AB
 24:D7:9C,"Cisco Cisco Systems, Inc"
 24:D7:EB,Espressi Espressif Inc.
 24:D8:1E,"MirWifiJ MirWifi,Joint-Stock Company"
 24:D9:04,"SichuanC Sichuan Changhong Network Technologies Co., Ltd."
@@ -20932,27 +21080,30 @@
 24:DA:33,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:DA:9B,"Motorola Motorola Mobility LLC, a Lenovo Company"
 24:DA:B6,Sistemas Sistemas de Gestión Energética S.A. de C.V
 24:DB:AC,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:DB:AD,ShopperT ShopperTrak RCT Corporation
 24:DB:ED,"SamsungE Samsung Electronics Co.,Ltd"
 24:DC:0F,"PhytiumT Phytium Technology Co.,Ltd."
+24:DC:C3,Espressi Espressif Inc.
 24:DE:C6,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 24:DF:6A,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:DF:A7,"Hangzhou Hangzhou BroadLink Technology Co.,Ltd"
 24:E1:24,"XiamenMi Xiamen Milesight IoT Co., Ltd."
 24:E2:71,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
 24:E3:14,"Apple Apple, Inc."
 24:E3:DE,"ChinaTel China Telecom Fufu Information Technology Co., Ltd."
 24:E4:3F,"WenzhouK Wenzhou Kunmei Communication Technology Co.,Ltd."
 24:E4:C8,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
+24:E4:CE,"KaonGrou Kaon Group Co., Ltd."
 24:E5:0F,"Google Google, Inc."
 24:E5:AA,"PhilipsO Philips Oral Healthcare, Inc."
 24:E6:BA,ZavodimK JSC Zavod im. Kozitsky
 24:E8:53,LGInnote LG Innotek
+24:E8:E5,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 24:E9:27,TomTomIn TomTom International BV
 24:E9:B3,"Cisco Cisco Systems, Inc"
 24:E9:CA,"HuaweiDe Huawei Device Co., Ltd."
 24:EA:40,Helmholz Helmholz GmbH & Co. KG
 24:EB:65,SAETIS SAET I.S. S.r.l.
 24:EB:ED,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:EC:51,ADFTechn ADF Technologies Sdn Bhd
@@ -20976,27 +21127,31 @@
 24:FA:F3,"Shanghai Shanghai Flexem Technology Co.,Ltd."
 24:FB:65,"HuaweiTe Huawei Technologies Co.,Ltd"
 24:FC:4E,JuniperN Juniper Networks
 24:FC:E5,"SamsungE Samsung Electronics Co.,Ltd"
 24:FD:0D,Intelbra Intelbras
 24:FD:52,LiteonTe Liteon Technology Corporation
 24:FD:5B,"SmartThi SmartThings, Inc."
+24:FD:FA,Private
+24:FE:9A,CyberTAN CyberTAN Technology Inc.
 28:01:1C,zte zte corporation
+28:02:2E,"Apple Apple, Inc."
 28:02:44,"Apple Apple, Inc."
 28:02:45,"KonzeSys Konze System Technology Co.,Ltd."
 28:02:D8,"SamsungE Samsung Electronics Co.,Ltd"
 28:04:C6,WananHon Wanan Hongsheng Electronic Co.Ltd
 28:04:E0,FermaxEl Fermax Electronica S.A.U.
 28:05:2E,Dematic Dematic Corp
 28:06:1E,"NingboGl Ningbo Global Useful Electric Co.,Ltd"
 28:06:8D,"Itl Itl, Llc"
 28:07:0D,"Guangzho Guangzhou Winsound Information Technology Co.,Ltd."
 28:0A:EE,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 28:0B:5C,"Apple Apple, Inc."
 28:0C:28,UnigenDa Unigen DataStorage Corporation
+28:0C:2D,"Qualvisi Qualvision Technology Co.,Ltd"
 28:0C:B8,Mikrosay Mikrosay Yazilim ve Elektronik A.S.
 28:0D:FC,SonyInte Sony Interactive Entertainment Inc.
 28:0E:8B,"BeijingS Beijing Spirit Technology Development Co., Ltd."
 28:0F:C5,"BeijingL Beijing Leadsec Technology Co., Ltd."
 28:0F:EB,LGInnote LG Innotek
 28:10:1B,MagnaCom
 28:10:7B,D-LinkIn D-Link International
@@ -21147,17 +21302,19 @@
 28:6B:35,IntelCor Intel Corporate
 28:6C:07,"XIAOMIEl XIAOMI Electronics,CO.,LTD"
 28:6D:97,"SAMJIN SAMJIN Co., Ltd."
 28:6D:CD,"BeijingW Beijing Winner Microelectronics Co.,Ltd."
 28:6E:D4,"HuaweiTe Huawei Technologies Co.,Ltd"
 28:6F:40,TonlyTec Tonly Technology Co. Ltd
 28:6F:7F,"Cisco Cisco Systems, Inc"
+28:70:4E,Ubiquiti Ubiquiti Inc
 28:71:84,SpirePay Spire Payments
 28:72:C5,Smartmat Smartmatic Corp
 28:72:F0,Athena
+28:73:F6,AmazonTe Amazon Technologies Inc.
 28:74:F5,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 28:75:D8,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 28:76:10,IgniteNe IgniteNet
 28:76:81,SiliconL Silicon Laboratories
 28:76:CD,"Funshion Funshion Online Technologies Co.,Ltd"
 28:77:77,zte zte corporation
 28:77:B1,Triplusg Tri plus grupa d.o.o.
@@ -21203,15 +21360,15 @@
 28:A0:2B,"Apple Apple, Inc."
 28:A1:83,"Alpsalpi Alpsalpine Co,.Ltd"
 28:A1:86,enblink
 28:A1:92,GERPSolu GERP Solution
 28:A1:EB,"EtekTech Etek Technology (Shenzhen) Co.,Ltd"
 28:A2:41,exlar exlar corp
 28:A2:4B,JuniperN Juniper Networks
-28:A3:31,SierraWi Sierra Wireless
+28:A3:31,"SierraWi Sierra Wireless, ULC"
 28:A5:3F,"vivoMobi vivo Mobile Communication Co., Ltd."
 28:A5:74,MillerEl Miller Electric Mfg. Co.
 28:A5:EE,"Shenzhen Shenzhen SDGI CATV Co., Ltd"
 28:A6:AC,seca seca gmbh & co. kg
 28:A6:DB,"HuaweiTe Huawei Technologies Co.,Ltd"
 28:AC:67,"MachPowe Mach Power, Rappresentanze Internazionali s.r.l."
 28:AC:9E,"Cisco Cisco Systems, Inc"
@@ -21222,14 +21379,15 @@
 28:B0:CC,Xenyadoo Xenya d.o.o.
 28:B1:33,"SHINEMAN SHINEMAN(SHENZHEN) Tech. Cor., Ltd."
 28:B2:BD,IntelCor Intel Corporate
 28:B3:71,RuckusWi Ruckus Wireless
 28:B3:AB,GenmarkA Genmark Automation
 28:B4:48,"HuaweiTe Huawei Technologies Co.,Ltd"
 28:B4:FB,"Sprocomm Sprocomm Technologies CO.,LTD."
+28:B5:E8,TexasIns Texas Instruments
 28:B7:7C,IEEERegi IEEE Registration Authority
 28:B7:7C:00:00:00/28,Shenzhen Shenzhen Eview Gps Technology
 28:B7:7C:10:00:00/28,SolarEdg SolarEdge Technologies
 28:B7:7C:20:00:00/28,"ZhuhaiRo Zhuhai RongBang Electronic Technology Co., Ltd."
 28:B7:7C:30:00:00/28,"BeijingK Beijing Kitten&Puppy Technology Co.,Ltd."
 28:B7:7C:40:00:00/28,Annapurn Annapurna labs
 28:B7:7C:50:00:00/28,GROTHE GROTHE GmbH
@@ -21249,19 +21407,21 @@
 28:BB:59,"RNETTech RNET Technologies, Inc."
 28:BC:05,BLUProdu BLU Products Inc
 28:BC:18,Sourcing SourcingOverseas Co. Ltd
 28:BC:56,"EMAC EMAC, Inc."
 28:BD:89,"Google Google, Inc."
 28:BE:03,TCTmobil TCT mobile ltd
 28:BE:43,"vivoMobi vivo Mobile Communication Co., Ltd."
-28:BE:9B,Technico Technicolor CH USA Inc.
+28:BE:9B,VantivaU Vantiva USA LLC
+28:BE:F3,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 28:BF:89,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 28:C0:1B,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 28:C0:DA,JuniperN Juniper Networks
 28:C1:3C,"HonHaiPr Hon Hai Precision Industry Co., Ltd."
+28:C1:A0,"Apple Apple, Inc."
 28:C2:1F,SamsungE Samsung Electro-Mechanics(Thailand)
 28:C2:DD,AzureWav AzureWave Technology Inc.
 28:C5:38,"Apple Apple, Inc."
 28:C5:D2,IntelCor Intel Corporate
 28:C6:3F,IntelCor Intel Corporate
 28:C6:71,YotaDevi Yota Devices OY
 28:C6:8E,Netgear
@@ -21282,15 +21442,15 @@
 28:CD:C1,Raspberr Raspberry Pi Trading Ltd
 28:CD:C4,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 28:CF:08,Essys
 28:CF:51,"Nintendo Nintendo Co.,Ltd"
 28:CF:DA,"Apple Apple, Inc."
 28:CF:E9,"Apple Apple, Inc."
 28:D0:44,Shenzhen Shenzhen Xinyin technology company
-28:D0:CB,Cambridg Cambridge Communication Systems Ltd
+28:D0:CB,Adtran Adtran Inc
 28:D0:EA,IntelCor Intel Corporate
 28:D0:F5,"RuijieNe Ruijie Networks Co.,LTD"
 28:D1:27,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 28:D1:AF,Nokia Nokia Corporation
 28:D1:B7,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 28:D2:44,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 28:D3:EA,"HuaweiDe Huawei Device Co., Ltd."
@@ -21316,15 +21476,19 @@
 28:E5:B0,"HuaweiTe Huawei Technologies Co.,Ltd"
 28:E6:08,Tokheim
 28:E6:E9,SISSatIn SIS Sat Internet Services GmbH
 28:E7:1D,AristaNe Arista Networks
 28:E7:94,Microtim Microtime Computer Inc.
 28:E7:CF,"Apple Apple, Inc."
 28:E9:8E,Mitsubis Mitsubishi Electric Corporation
+28:EA:0B,Microsof Microsoft Corporation
 28:EA:2D,"Apple Apple, Inc."
+28:EB:0A,RollingW Rolling Wireless S.a.r.l. Luxembourg
+28:EB:A6,Nex-T Nex-T LLC
+28:EC:22,eero eero inc.
 28:EC:95,"Apple Apple, Inc."
 28:EC:9A,TexasIns Texas Instruments
 28:ED:58,JAGJakob JAG Jakob AG
 28:ED:6A,"Apple Apple, Inc."
 28:ED:E0,"AMPAKTec AMPAK Technology, Inc."
 28:EE:2C,Frontlin Frontline Test Equipment
 28:EE:52,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
@@ -21381,20 +21545,22 @@
 28:FD:80:E0:00:00/28,T-RadioA T-Radio AS
 28:FD:80:F0:00:00/28,Private
 28:FE:65,"DongGuan DongGuan Siyoto Electronics Co., Ltd"
 28:FE:CD,"Lemobile Lemobile Information Technology (Beijing) Co., Ltd."
 28:FE:DE,"COMESTA COMESTA, Inc."
 28:FF:3C,"Apple Apple, Inc."
 28:FF:3E,zte zte corporation
+28:FF:5F,"HGGenuin HG Genuine Intelligent Terminal (Xiaogan) Co.,Ltd."
 28:FF:B2,Toshiba Toshiba Corp.
 2A:0B:B8,"xFusionD xFusion Digital Technologies Co., Limited"
 2A:A1:39,"Pointgua Pointguard, Llc"
 2A:AC:53,Wolfspyr Wolfspyre Labs
 2A:EA:15,TibitCom Tibit Communications
 2A:FD:6A,CharterC Charter Communications
+2C:00:2A,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 2C:00:2C,Unowhy
 2C:00:33,"EControl EControls, LLC"
 2C:00:AB,"ARRISGro ARRIS Group, Inc."
 2C:00:F7,Xos
 2C:01:0B,"NASCENTT NASCENT Technology, LLC - RemKon"
 2C:01:B5,"Cisco Cisco Systems, Inc"
 2C:02:9F,3ALogics
@@ -21517,28 +21683,31 @@
 2C:39:C1,Ciena Ciena Corporation
 2C:3A:28,FagorEle Fagor Electrónica
 2C:3A:91,"HuaweiDe Huawei Device Co., Ltd."
 2C:3A:E8,Espressi Espressif Inc.
 2C:3A:FD,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 2C:3B:70,AzureWav AzureWave Technology Inc.
 2C:3B:FD,"NetstorT Netstor Technology Co., Ltd."
+2C:3C:05,Marinesy Marinesync Corp
+2C:3E:BF,"HOSINGlo HOSIN Global Electronics Co., Ltd."
 2C:3E:CF,"Cisco Cisco Systems, Inc"
 2C:3F:0B,CiscoMer Cisco Meraki
 2C:3F:38,"Cisco Cisco Systems, Inc"
 2C:3F:3E,Alge-Tim Alge-Timing GmbH
 2C:40:2B,SmartiBl Smart iBlue Technology Limited
 2C:40:53,"SamsungE Samsung Electronics Co.,Ltd"
 2C:41:38,HewlettP Hewlett Packard
 2C:41:A1,Bose Bose Corporation
 2C:42:05,Lytx
 2C:43:1A,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 2C:43:BE,SunnovoI Sunnovo International Limited
 2C:44:01,"SamsungE Samsung Electronics Co.,Ltd"
 2C:44:1B,Spectrum Spectrum Medical Limited
 2C:44:FD,HewlettP Hewlett Packard
+2C:45:9A,DixonTec Dixon Technologies (India) Limited
 2C:47:59,BeijingM Beijing MEGA preponderance Science & Technology Co. Ltd
 2C:48:35,IEEERegi IEEE Registration Authority
 2C:48:35:00:00:00/28,"Progress Progress Rail Services, Inspection and Information Systems"
 2C:48:35:10:00:00/28,Advanced Advanced Electronics Company Ltd
 2C:48:35:20:00:00/28,RheonikM Rheonik Messtechnik GmbH
 2C:48:35:30:00:00/28,NewtraxT Newtrax Technologies Inc
 2C:48:35:40:00:00/28,Geartech Geartech Ltd
@@ -21550,14 +21719,15 @@
 2C:48:35:A0:00:00/28,Collatz+ Collatz+Trojan GmbH
 2C:48:35:B0:00:00/28,Shanghai Shanghai Visteon Automotive Electronics System CO. Ltd.
 2C:48:35:C0:00:00/28,Santec Santec Corporation
 2C:48:35:D0:00:00/28,PhasorSo Phasor Solutions Ltd
 2C:48:35:E0:00:00/28,"Irootech Irootech Technology Co.,Ltd"
 2C:48:81,"vivoMobi vivo Mobile Communication Co., Ltd."
 2C:4A:11,Ciena Ciena Corporation
+2C:4C:15,JuniperN Juniper Networks
 2C:4C:C6,"MurataMa Murata Manufacturing Co., Ltd."
 2C:4D:54,ASUSTekC ASUSTek COMPUTER INC.
 2C:4D:79,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 2C:4D:DE,TecnoMob Tecno Mobile Limited
 2C:4E:7D,Chunghua Chunghua Intelligent Network Equipment Inc.
 2C:4F:52,"Cisco Cisco Systems, Inc"
 2C:50:89,"Shenzhen Shenzhen Kaixuan Visual Technology Co.,Limited"
@@ -21592,15 +21762,17 @@
 2C:60:CD,"NrElectr Nr Electric Co., Ltd"
 2C:61:04,"Shenzhen Shenzhen Fenglian Technology Co., Ltd."
 2C:61:F6,"Apple Apple, Inc."
 2C:62:5A,"FinestSe Finest Security Systems Co., Ltd"
 2C:62:89,Regeners Regenersis (Glenrothes) Ltd
 2C:63:73,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 2C:64:1F,"Vizio Vizio, Inc"
+2C:64:F6,"WuQiTech Wu Qi Technologies,Inc."
 2C:67:98,InTalTec InTalTech Ltd.
+2C:67:AB,EzelinkT Ezelink Telecom
 2C:67:FB,"ShenZhen ShenZhen Zhengjili Electronics Co., LTD"
 2C:69:1D,IEEERegi IEEE Registration Authority
 2C:69:1D:00:00:00/28,"HunanXia Hunan Xiangjiang Kunpeng Information Technology Co., Ltd."
 2C:69:1D:10:00:00/28,KatekSe Katek Se
 2C:69:1D:20:00:00/28,Abode Abode Systems Inc
 2C:69:1D:30:00:00/28,"Sunsa Sunsa, Inc"
 2C:69:1D:40:00:00/28,Speedtec Speedtech Corp.
@@ -21636,14 +21808,15 @@
 2C:6B:7D,TexasIns Texas Instruments
 2C:6B:F5,JuniperN Juniper Networks
 2C:6D:C1,IntelCor Intel Corporate
 2C:6E:85,IntelCor Intel Corporate
 2C:6F:4E,"HubeiYua Hubei Yuan Times Technology Co.,Ltd."
 2C:6F:51,Herospee Herospeed Digital Technology Limited
 2C:6F:C9,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+2C:70:4F,zte zte corporation
 2C:71:55,HiveMoti HiveMotion
 2C:71:FF,AmazonTe Amazon Technologies Inc.
 2C:72:C3,Soundmat Soundmatters
 2C:73:60,EardaTec Earda Technologies co Ltd
 2C:73:A0,"Cisco Cisco Systems, Inc"
 2C:75:0F,Shanghai Shanghai Dongzhou-Lawton Communication Technology Co. Ltd.
 2C:75:CB,"Novitec Novitec Co., Ltd."
@@ -21673,18 +21846,21 @@
 2C:92:2C,"KishuGik Kishu Giken Kogyou Company Ltd,."
 2C:93:FB,SercommF Sercomm France Sarl
 2C:94:52,"HuaweiTe Huawei Technologies Co.,Ltd"
 2C:94:64,"Cincoze Cincoze Co., Ltd."
 2C:95:69,"ARRISGro ARRIS Group, Inc."
 2C:95:7F,zte zte corporation
 2C:96:62,Invenit Invenit BV
+2C:96:82,MitraSta MitraStar Technology Corp.
 2C:97:17,ICY I.C.Y. B.V.
 2C:97:B1,"HuaweiTe Huawei Technologies Co.,Ltd"
 2C:97:ED,SonyImag Sony Imaging Products & Solutions Inc.
+2C:98:11,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 2C:99:24,"ARRISGro ARRIS Group, Inc."
+2C:99:75,"SamsungE Samsung Electronics Co.,Ltd"
 2C:9A:A4,Eolo Eolo SpA
 2C:9D:1E,"HuaweiTe Huawei Technologies Co.,Ltd"
 2C:9D:65,"vivoMobi vivo Mobile Communication Co., Ltd."
 2C:9E:00,SonyInte Sony Interactive Entertainment Inc.
 2C:9E:5F,"ARRISGro ARRIS Group, Inc."
 2C:9E:EC,JabilCir Jabil Circuit Penang
 2C:9E:FC,Canon Canon Inc.
@@ -21725,21 +21901,25 @@
 2C:B6:C8,"Raisecom Raisecom Technology CO., LTD"
 2C:B8:ED,SonicWal SonicWall
 2C:BA:BA,"SamsungE Samsung Electronics Co.,Ltd"
 2C:BC:87,"Apple Apple, Inc."
 2C:BE:08,"Apple Apple, Inc."
 2C:BE:97,Ingenieu Ingenieurbuero Bickele und Buehler GmbH
 2C:BE:EB,NothingT Nothing Technology Limited
+2C:C2:53,"Apple Apple, Inc."
 2C:C2:60,Oracle Oracle Corporation
+2C:C3:E6,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 2C:C4:07,machineQ
 2C:C5:46,"HuaweiDe Huawei Device Co., Ltd."
 2C:C5:48,IAdea IAdea Corporation
 2C:C5:D3,RuckusWi Ruckus Wireless
+2C:C6:A0,Lumacron Lumacron Technology Ltd.
 2C:C8:1B,Routerbo Routerboard.com
 2C:CA:0C,WithusPl Withus Planet
+2C:CA:75,RobertBo Robert Bosch GmbH AnP
 2C:CC:15,Nokia Nokia Corporation
 2C:CC:44,SonyInte Sony Interactive Entertainment Inc.
 2C:CC:E6,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 2C:CD:27,Precor Precor Inc
 2C:CD:43,SummitTe Summit Technology Group
 2C:CD:69,Aqavicom Aqavi.com
 2C:CE:1E,Cloudtro Cloudtronics Pty Ltd
@@ -21760,19 +21940,21 @@
 2C:D1:41:90:00:00/28,"BeijingH Beijing Hexing Chuangxiang Technology Co., Ltd."
 2C:D1:41:A0:00:00/28,"Fiberroa Fiberroad Technology Co., Ltd."
 2C:D1:41:B0:00:00/28,ResusInd Resus Industries
 2C:D1:41:C0:00:00/28,"PINSHANG PIN SHANG LED Co., LTD."
 2C:D1:41:D0:00:00/28,Square Square Inc.
 2C:D1:41:E0:00:00/28,CitaSmar Cita Smart Solutions Ltd
 2C:D1:41:F0:00:00/28,Private
+2C:D1:C6,"MurataMa Murata Manufacturing Co., Ltd."
 2C:D1:DA,"Keysight Keysight Technologies, Inc."
 2C:D2:6B,Fn-LinkT Fn-Link Technology Limited
 2C:D2:E3,"Guangzho Guangzhou Aoshi Electronic Co.,Ltd"
 2C:D2:E7,Nokia Nokia Corporation
 2C:D4:44,Fujitsu Fujitsu Limited
+2C:D7:FF,LANCOM LANCOM Systems GmbH
 2C:D9:74,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 2C:DB:07,IntelCor Intel Corporate
 2C:DC:78,Descarte Descartes Systems (USA) LLC
 2C:DC:AD,WistronN Wistron Neweb Corporation
 2C:DC:D7,AzureWav AzureWave Technology Inc.
 2C:DD:0C,Discover Discovergy GmbH
 2C:DD:5F,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
@@ -21804,14 +21986,16 @@
 2C:FC:8B,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 2C:FC:E4,CTEKSwed CTEK Sweden AB
 2C:FD:37,"BlueCaly Blue Calypso, Inc."
 2C:FD:A1,ASUSTekC ASUSTek COMPUTER INC.
 2C:FD:AB,"Motorola Motorola (Wuhan) Mobility Technologies Communication Co., Ltd."
 2C:FD:B3,TonlyTec Tonly Technology Co. Ltd
 2C:FD:B4,"Shenzhen Shenzhen Jingxun Software Telecommunication Technology Co.,Ltd"
+2C:FE:4F,XiaomiCo Xiaomi Communications Co Ltd
+2C:FE:E2,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
 2C:FF:65,"OkiElect Oki Electric Industry Co., Ltd."
 2C:FF:EE,"vivoMobi vivo Mobile Communication Co., Ltd."
 2E:2E:2E,LaaLocal LAA (Locally Administered Address) for Meditech Systems
 30:03:C8,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 30:04:5C,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 30:05:05,IntelCor Intel Corporate
 30:05:3F,"JTI JTI Co.,Ltd."
@@ -21870,14 +22054,15 @@
 30:18:CF,DEOScont DEOS control systems GmbH
 30:19:66,"SamsungE Samsung Electronics Co.,Ltd"
 30:19:84,"HuaweiTe Huawei Technologies Co.,Ltd"
 30:1A:28,MakoNetw Mako Networks Ltd
 30:1A:30,MakoNetw Mako Networks Ltd
 30:1A:BA,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 30:1B:97,"LierdaSc Lierda Science & Technology Group Co.,Ltd"
+30:1D:49,FirmusTe Firmus Technologies Pty Ltd
 30:1F:48,zte zte corporation
 30:1F:9A,IEEERegi IEEE Registration Authority
 30:1F:9A:00:00:00/28,IlsanEle Ilsan Electronics
 30:1F:9A:10:00:00/28,Dewesoft Dewesoft d.o.o.
 30:1F:9A:20:00:00/28,"CHISONMe CHISON Medical Technologies Co., Ltd."
 30:1F:9A:30:00:00/28,"Micomsof Micomsoft Co.,Ltd."
 30:1F:9A:40:00:00/28,"NCMSuppl NCM Supplies, Inc."
@@ -21898,14 +22083,15 @@
 30:24:78,Sagemcom Sagemcom Broadband SAS
 30:24:A9,HP HP Inc.
 30:27:CF,CanopyGr Canopy Growth Corp
 30:29:52,Hillston Hillstone Networks Inc
 30:29:BE,"Shanghai Shanghai MRDcom Co.,Ltd"
 30:2B:DC,"Top-Unum Top-Unum Electronics Co., LTD"
 30:2D:E8,"JDAJDA JDA, LLC (JDA Systems)"
+30:2F:1E,Siemens Siemens Ag
 30:31:7D,Hosiden Hosiden Corporation
 30:31:80,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 30:32:35,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
 30:32:94,W-IE-NE- W-IE-NE-R Plein & Baus GmbH
 30:32:D4,"Hanilstm Hanilstm Co., Ltd."
 30:33:35,Boosty
 30:34:22,eero eero inc.
@@ -21939,14 +22125,15 @@
 30:3D:51:D0:00:00/28,XORUK XOR UK Corporation Limited
 30:3D:51:E0:00:00/28,Percentc Percent.com
 30:3E:A7,IntelCor Intel Corporate
 30:3E:AD,SonavoxC Sonavox Canada Inc
 30:3F:5D,PtHanSun Pt Han Sung Electoronics Indonesia
 30:3F:7B,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 30:3F:BB,HewlettP Hewlett Packard Enterprise
+30:40:74,zte zte corporation
 30:41:74,AltecLan Altec Lansing Llc
 30:42:25,Burg-Wäc Burg-Wächter Kg
 30:42:40,zte zte corporation
 30:42:A1,ilumisys ilumisys Inc. DBA Toggled
 30:43:D7,IEEERegi IEEE Registration Authority
 30:43:D7:00:00:00/28,Symes Symes Sa
 30:43:D7:10:00:00/28,"Shenzhen Shenzhen juduoping Technology Co.,Ltd"
@@ -21989,15 +22176,15 @@
 30:49:9E,"HuaweiTe Huawei Technologies Co.,Ltd"
 30:4A:26,"Shenzhen Shenzhen Trolink Technology CO, LTD"
 30:4B:07,"Motorola Motorola Mobility LLC, a Lenovo Company"
 30:4C:7E,"Panasoni Panasonic Electric Works Automation Controls Techno Co.,Ltd."
 30:4E:1B,"HuaweiDe Huawei Device Co., Ltd."
 30:4E:C3,"TianjinT Tianjin Techua Technology Co., Ltd."
 30:4F:00,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
-30:4F:75,DASANNet DASAN Network Solutions
+30:4F:75,DZS DZS Inc.
 30:50:75,GNAudio GN Audio A/S
 30:50:FD,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 30:51:F8,BYK-Gard BYK-Gardner GmbH
 30:52:5A,"NST NST Co., LTD"
 30:52:CB,LiteonTe Liteon Technology Corporation
 30:53:C1,Cresyn
 30:55:ED,TrexNetw Trex Network LLC
@@ -22010,14 +22197,15 @@
 30:59:5B,streamno streamnow AG
 30:59:B7,Microsof Microsoft
 30:5A:3A,ASUSTekC ASUSTek COMPUTER INC.
 30:5A:99,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 30:5D:38,Beissbar Beissbarth
 30:5D:A6,ADVALYSY ADVALY SYSTEM Inc.
 30:5F:77,"NewH3CTe New H3C Technologies Co., Ltd"
+30:60:0A,CigShang Cig Shanghai Co Ltd
 30:60:23,"ARRISGro ARRIS Group, Inc."
 30:61:12,PAV PAV GmbH
 30:61:18,Paradom Paradom Inc.
 30:63:6B,"Apple Apple, Inc."
 30:63:71,Shenzhen Shenzhenshi Xinzhongxin Technology Co.Ltd
 30:65:EC,WistronC Wistron (ChongQing)
 30:66:D0,"HuaweiDe Huawei Device Co., Ltd."
@@ -22034,14 +22222,15 @@
 30:75:12,Sony Sony Corporation
 30:76:6F,LGElectr LG Electronics (Mobile Communications)
 30:77:CB,"MaikeInd Maike Industry(Shenzhen)CO.,LTD"
 30:78:5C,PartowTa Partow Tamas Novin (Parman)
 30:78:6B,"TIANJING TIANJIN Golden Pentagon Electronics Co., Ltd."
 30:78:C2,Innowire Innowireless / QUCELL Networks
 30:78:D3,Virgilan Virgilant Technologies Ltd.
+30:7A:57,Accuener Accuenergy (CANADA) Inc
 30:7B:AC,"NewH3CTe New H3C Technologies Co., Ltd"
 30:7B:C9,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 30:7C:30,Rim
 30:7C:4A,"HuaweiDe Huawei Device Co., Ltd."
 30:7C:5E,JuniperN Juniper Networks
 30:7C:B2,AnovFran Anov France
 30:7E:CB,Sfr
@@ -22050,14 +22239,15 @@
 30:82:16,"Apple Apple, Inc."
 30:83:98,Espressi Espressif Inc.
 30:83:D2,"Motorola Motorola Mobility LLC, a Lenovo Company"
 30:84:54,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 30:85:A9,ASUSTekC ASUSTek COMPUTER INC.
 30:85:EB,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 30:86:2D,"AristaNe Arista Network, Inc."
+30:86:F1,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 30:87:30,"HuaweiTe Huawei Technologies Co.,Ltd"
 30:87:D9,RuckusWi Ruckus Wireless
 30:88:41,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 30:89:44,DEVABroa DEVA Broadcast Ltd.
 30:89:4A,IntelCor Intel Corporate
 30:89:76,"DalianLa Dalian Lamba Technology Co.,Ltd"
 30:89:99,"Guangdon Guangdong East Power Co.,"
@@ -22098,21 +22288,23 @@
 30:A9:DE,LGInnote LG Innotek
 30:AA:BD,"Shanghai Shanghai Reallytek Information Technology Co.,Ltd"
 30:AA:E4,"HuaweiDe Huawei Device Co., Ltd."
 30:AB:6A,SamsungE Samsung Electro-Mechanics(Thailand)
 30:AE:7B,"DeqingDu Deqing Dusun Electron CO., LTD"
 30:AE:A4,Espressi Espressif Inc.
 30:AE:F6,RadioMob Radio Mobile Access
+30:AF:7E,TexasIns Texas Instruments
 30:AF:CE,"vivoMobi vivo Mobile Communication Co., Ltd."
 30:B0:37,"NewH3CTe New H3C Technologies Co., Ltd"
 30:B0:EA,"Shenzhen Shenzhen Chuangxin Internet Communication Technology Co., Ltd"
 30:B1:64,PowerEle Power Electronics International Inc.
 30:B1:B5,Arcadyan Arcadyan Corporation
-30:B2:16,HitachiE Hitachi Energy
+30:B2:16,HitachiE Hitachi Energy Germany AG
 30:B2:37,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
+30:B2:9F,Evident Evident Corporation
 30:B3:46,CjscNors Cjsc Norsi-Trans
 30:B3:A2,"Shenzhen Shenzhen Heguang Measurement & Control Technology Co.,Ltd"
 30:B4:9E,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 30:B4:B8,LGElectr LG Electronics
 30:B5:C2,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 30:B5:F1,"AitexinT Aitexin Technology Co., Ltd"
 30:B6:2D,"MojoNetw Mojo Networks, Inc."
@@ -22151,16 +22343,18 @@
 30:D7:A1,"Apple Apple, Inc."
 30:D9:41,RaydiumS Raydium Semiconductor Corp.
 30:D9:D9,"Apple Apple, Inc."
 30:DE:4B,TP-Link TP-Link Corporation Limited
 30:DE:86,CedacSof Cedac Software S.r.l.
 30:DF:17,"Alpsalpi Alpsalpine Co,.Ltd"
 30:DF:8D,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
+30:E0:4F,"Apple Apple, Inc."
 30:E0:90,Genevisi Genevisio Ltd.
 30:E1:71,HewlettP Hewlett Packard
+30:E1:F1,Intelbra Intelbras
 30:E2:83,TexasIns Texas Instruments
 30:E3:7A,IntelCor Intel Corporate
 30:E3:96,"HuaweiDe Huawei Device Co., Ltd."
 30:E3:D6,SpotifyU Spotify USA Inc.
 30:E4:8E,Vodafone Vodafone UK
 30:E4:DB,"Cisco Cisco Systems, Inc"
 30:E7:BC,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -22239,14 +22433,15 @@
 34:0A:22,Top-Acce Top-Access Electronics Co Ltd
 34:0A:33,D-LinkIn D-Link International
 34:0A:98,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:0A:FF,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
 34:0B:40,MiosElet Mios Elettronica Srl
 34:0C:ED,Moduel Moduel AB
 34:0F:66,WebSensi Web Sensing LLC
+34:10:F4,SiliconL Silicon Laboratories
 34:12:90,"Treeview Treeview Co.,Ltd."
 34:12:98,"Apple Apple, Inc."
 34:12:F9,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:13:43,GELighti GE Lighting
 34:13:A8,Mediplan Mediplan Limited
 34:13:E8,IntelCor Intel Corporate
 34:14:5F,"SamsungE Samsung Electronics Co.,Ltd"
@@ -22320,14 +22515,15 @@
 34:40:B5,Ibm
 34:41:5D,IntelCor Intel Corporate
 34:41:A8,ER-Telec ER-Telecom
 34:42:62,"Apple Apple, Inc."
 34:46:6F,HiTEMEng HiTEM Engineering
 34:46:EC,"HuaweiDe Huawei Device Co., Ltd."
 34:47:9A,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+34:47:D4,"ChengduQ Chengdu Quanjing Intelligent Technology Co.,Ltd"
 34:48:ED,Dell Dell Inc.
 34:49:5B,Sagemcom Sagemcom Broadband SAS
 34:4A:C3,"HuNanZiK HuNan ZiKun Information Technology CO., Ltd"
 34:4B:3D,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 34:4B:50,zte zte corporation
 34:4C:A4,amazipoi amazipoint technology Ltd.
 34:4C:C8,Echodyne Echodyne Corp
@@ -22352,25 +22548,27 @@
 34:5B:11,EviHeat Evi Heat Ab
 34:5B:98,EMMicroe EM Microelectronic
 34:5B:BB,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 34:5C:40,CargtHol Cargt Holdings LLC
 34:5D:10,Wytek
 34:5D:9E,Sagemcom Sagemcom Broadband SAS
 34:5D:A8,"Cisco Cisco Systems, Inc"
+34:5E:08,"Roku Roku, Inc"
 34:60:F9,TP-Link TP-Link Corporation Limited
 34:61:78,Boeing The Boeing Company
 34:62:88,"Cisco Cisco Systems, Inc"
 34:62:B4,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 34:63:D4,BionixSu Bionix Supplychain Technologies Slu
 34:64:A9,HewlettP Hewlett Packard
 34:66:79,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:66:EA,VertuInt Vertu International Corporation Limited
 34:68:4A,"Terawork Teraworks Co., Ltd."
 34:68:93,Tecnovid Tecnovideo Srl
 34:68:95,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+34:68:B5,TexasIns Texas Instruments
 34:69:87,zte zte corporation
 34:6A:C2,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:6B:46,Sagemcom Sagemcom Broadband SAS
 34:6B:5B,"NewH3CTe New H3C Technologies Co., Ltd"
 34:6B:D3,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:6C:0F,PramodTe Pramod Telecom Pvt. Ltd
 34:6D:9C,Carrier Carrier Corporation
@@ -22389,14 +22587,15 @@
 34:76:C5,"I-ODataD I-O Data Device,Inc."
 34:78:39,zte zte corporation
 34:78:77,O-NetCom O-Net Communications (Shenzhen) Limited
 34:78:D7,"GioneeCo Gionee Communication Equipment Co.,Ltd."
 34:79:16,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:7A:60,"ARRISGro ARRIS Group, Inc."
 34:7C:25,"Apple Apple, Inc."
+34:7D:E4,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 34:7D:F6,IntelCor Intel Corporate
 34:7E:00,"HuaweiDe Huawei Device Co., Ltd."
 34:7E:39,NokiaDan Nokia Danmark A/S
 34:7E:5C,"Sonos Sonos, Inc."
 34:7E:CA,Nextwill
 34:80:0D,Cavium Cavium Inc
 34:80:B3,XiaomiCo Xiaomi Communications Co Ltd
@@ -22410,29 +22609,33 @@
 34:84:E4,TexasIns Texas Instruments
 34:85:11,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 34:85:18,Espressi Espressif Inc.
 34:85:84,"ExtremeN Extreme Networks, Inc."
 34:86:2A,HeinzLac Heinz Lackmann GmbH & Co KG
 34:86:5D,Espressi Espressif Inc.
 34:87:3D,"QuectelW Quectel Wireless Solutions Co.,Ltd."
+34:88:18,"Cisco Cisco Systems, Inc"
 34:88:5D,Logitech Logitech Far East
 34:8A:12,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 34:8A:7B,"SamsungE Samsung Electronics Co.,Ltd"
 34:8A:AE,Sagemcom Sagemcom Broadband SAS
 34:8B:75,LavaInte Lava International(H.K) Limited
+34:8C:5E,"Apple Apple, Inc."
+34:8D:52,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 34:8F:27,RuckusWi Ruckus Wireless
 34:91:6F,UserGate UserGate Ltd.
 34:92:C2,"SquareRo Square Route Co., Ltd."
 34:93:42,TTE TTE Corporation
 34:94:54,Espressi Espressif Inc.
 34:95:DB,Logitec Logitec Corporation
 34:96:72,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 34:97:6F,"Rootech Rootech, Inc."
 34:97:F6,ASUSTekC ASUSTek COMPUTER INC.
 34:97:FB,Advanced Advanced Rf Technologies Inc
+34:98:7A,Espressi Espressif Inc.
 34:98:B5,Netgear
 34:99:6F,VPIEngin VPI Engineering
 34:99:71,QuantaSt Quanta Storage Inc.
 34:99:D7,"Universa Universal Flow Monitors, Inc."
 34:9A:0D,ZBDDispl ZBD Displays Ltd
 34:9B:5B,Maquet Maquet GmbH
 34:9D:90,Heinzman Heinzmann GmbH & CO. KG
@@ -22457,21 +22660,23 @@
 34:AA:EE,Mikrovis Mikrovisatos Servisas UAB
 34:AB:37,"Apple Apple, Inc."
 34:AB:95,Espressi Espressif Inc.
 34:AC:11,"ChinaMob China Mobile Group Device Co.,Ltd."
 34:AD:61,Celestic Celestica Inc.
 34:AD:E4,"Shanghai Shanghai Chint Power Systems Co., Ltd."
 34:AF:2C,"Nintendo Nintendo Co., Ltd."
+34:AF:A3,Recogni Recogni Inc
 34:AF:B3,AmazonTe Amazon Technologies Inc.
 34:B1:F7,TexasIns Texas Instruments
 34:B2:0A,"HuaweiDe Huawei Device Co., Ltd."
 34:B3:54,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:B4:72,Espressi Espressif Inc.
 34:B5:71,Plds
 34:B5:A3,CigShang Cig Shanghai Co Ltd
+34:B7:DA,Espressi Espressif Inc.
 34:B7:FD,"Guangzho Guangzhou Younghead Electronic Technology Co.,Ltd"
 34:B8:83,"Cisco Cisco Systems, Inc"
 34:B9:8D,XiaomiCo Xiaomi Communications Co Ltd
 34:BA:38,PalMohan Pal Mohan Electronics Pvt Ltd
 34:BA:51,"Se-KureC Se-Kure Controls, Inc."
 34:BA:75,"EverestN Everest Networks, Inc"
 34:BA:9A,Asiatelc Asiatelco Technologies Co.
@@ -22492,14 +22697,15 @@
 34:C5:D0,Hagleitn Hagleitner Hygiene International GmbH
 34:C6:9A,Enecsys Enecsys Ltd
 34:C7:31,"Alpsalpi Alpsalpine Co,.Ltd"
 34:C8:03,Nokia Nokia Corporation
 34:C9:3D,IntelCor Intel Corporate
 34:C9:9D,EidolonC Eidolon Communications Technology Co. Ltd.
 34:C9:F0,LMTechno LM Technologies Ltd
+34:CA:81,"NewH3CIn New H3C Intelligence Terminal Co., Ltd."
 34:CB:1A,ProcterG Procter & Gamble Company
 34:CC:28,"Nexpring Nexpring Co. LTD.,"
 34:CD:6D,CommSkyT CommSky Technologies
 34:CD:BE,"HuaweiTe Huawei Technologies Co.,Ltd"
 34:CE:00,"XIAOMIEl XIAOMI Electronics,CO.,LTD"
 34:CE:69,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 34:CE:94,Parsec Parsec (Pty) Ltd
@@ -22521,24 +22727,27 @@
 34:D0:B8:B0:00:00/28,Orosound Orosound Sas
 34:D0:B8:C0:00:00/28,GloryMar Glory Mark Electronic Ltd. Taiwan Branch (B.V.I.)
 34:D0:B8:D0:00:00/28,NTXEmbed NTX Embedded
 34:D0:B8:E0:00:00/28,Kongqigu Kongqiguanjia (Beijing)Technology co.，ltd
 34:D2:62,"SzDjiTec Sz Dji Technology Co.,Ltd"
 34:D2:70,AmazonTe Amazon Technologies Inc.
 34:D2:C4,RENAPrin RENA GmbH Print Systeme
+34:D4:E3,"AtomPowe Atom Power, Inc."
 34:D6:93,"HuaweiDe Huawei Device Co., Ltd."
 34:D7:12,"Smartisa Smartisan Digital Co., Ltd"
 34:D7:37,IBGIndus IBG Industriebeteiligungsgesellschaft mbH &b Co. KG
 34:D7:72,"XiamenYu Xiamen Yudian Automation Technology Co., Ltd"
 34:D7:B4,"Tributar Tributary Systems, Inc."
+34:D8:56,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 34:D9:54,WiBotic WiBotic Inc.
 34:DA:B7,zte zte corporation
 34:DA:C1,"SAETechn SAE Technologies Development(Dongguan) Co., Ltd."
 34:DB:9C,Sagemcom Sagemcom Broadband SAS
 34:DB:FD,"Cisco Cisco Systems, Inc"
+34:DC:99,"NewH3CTe New H3C Technologies Co., Ltd"
 34:DD:04,Minut Minut AB
 34:DD:7E,"UmeoxInn Umeox Innovations Co.,Ltd"
 34:DE:1A,IntelCor Intel Corporate
 34:DE:34,zte zte corporation
 34:DF:20,"Shenzhen Shenzhen Comstar.Technology Co.,Ltd"
 34:DF:2A,"FujikonI Fujikon Industrial Co.,Limited"
 34:E0:CF,zte zte corporation
@@ -22570,20 +22779,22 @@
 34:E7:0B,"HANNetwo HAN Networks Co., Ltd"
 34:E7:1C,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 34:E8:94,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 34:E9:11,"vivoMobi vivo Mobile Communication Co., Ltd."
 34:E9:FE,"Metis Metis Co., Ltd."
 34:EA:34,"HangZhou HangZhou Gubei Electronics Technology Co.,Ltd"
 34:EA:E7,"Shanghai Shanghai High-Flying Electronics Technology Co., Ltd"
+34:EC:B6,PhyplusM Phyplus Microelectronics Limited
 34:ED:0B,"Shanghai Shanghai XZ-COM.CO.,Ltd."
 34:ED:1B,"Cisco Cisco Systems, Inc"
 34:EE:2A,ConMet
 34:EF:44,2Wire 2Wire Inc
 34:EF:8B,NTTCommu NTT Communications Corporation
 34:EF:B6,Edgecore Edgecore Networks Corporation
+34:F0:43,"SamsungE Samsung Electronics Co.,Ltd"
 34:F0:CA,"Shenzhen Shenzhen Linghangyuan Digital Technology Co.,Ltd."
 34:F1:50,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 34:F2:23,"FujianNe Fujian Newland Communication Science Technology Co.,Ltd."
 34:F3:9A,IntelCor Intel Corporate
 34:F3:9B,WizLAN WizLAN Ltd.
 34:F6:2D,SHARP SHARP Corporation
 34:F6:4B,IntelCor Intel Corporate
@@ -22609,38 +22820,42 @@
 38:01:95,"SamsungE Samsung Electronics Co.,Ltd"
 38:01:97,"TSSTGlob TSST Global,Inc"
 38:01:9F,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
 38:02:DE,Sercomm Sercomm Corporation.
 38:05:46,"FoctekPh Foctek Photonics, Inc."
 38:05:AC,PillerGr Piller Group GmbH
 38:06:B4,ADC A.D.C. GmbH
+38:07:16,FreeboxS Freebox Sas
 38:07:D4,Zeppelin Zeppelin Systems GmbH
 38:08:FD,Silca Silca Spa
 38:09:A4,FireflyI Firefly Integrations
 38:0A:0A,Sky-City Sky-City Communication and Electronics Limited Company
 38:0A:4F,PrachiEn Prachi Enterprises
 38:0A:94,"SamsungE Samsung Electronics Co.,Ltd"
 38:0A:AB,Formlabs
 38:0B:3C,TexasIns Texas Instruments
 38:0B:40,"SamsungE Samsung Electronics Co.,Ltd"
 38:0D:D4,PrimaxEl Primax Electronics Ltd.
 38:0E:4D,"Cisco Cisco Systems, Inc"
 38:0E:7B,"VPSThai V.P.S. Thai Co., Ltd"
 38:0F:4A,"Apple Apple, Inc."
+38:0F:AD,"HuaweiTe Huawei Technologies Co.,Ltd"
 38:0F:E4,Dedicate Dedicated Network Partners Oy
 38:10:D5,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 38:10:F0,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 38:12:7B,"CrenetLa Crenet Labs Co., Ltd."
+38:14:1B,SecureLe Secure Letter Inc.
 38:14:28,Dell Dell Inc.
 38:14:4E,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
+38:16:72,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 38:16:D1,"SamsungE Samsung Electronics Co.,Ltd"
 38:17:30,UlrichLi Ulrich Lippert GmbH & Co KG
 38:17:66,Promzaka Promzakaz Ltd.
 38:17:C3,HewlettP Hewlett Packard Enterprise
-38:17:E1,Technico Technicolor CH USA Inc.
+38:17:E1,VantivaU Vantiva USA LLC
 38:18:4C,SonyHome Sony Home Entertainment&Sound Products Inc
 38:19:2F,Nokia Nokia Corporation
 38:1A:52,SeikoEps Seiko Epson Corporation
 38:1C:1A,"Cisco Cisco Systems, Inc"
 38:1C:23,"HilanTec Hilan Technology CO.,LTD"
 38:1C:4A,"SIMComWi SIMCom Wireless Solutions Co.,Ltd."
 38:1D:14,Skydio Skydio Inc.
@@ -22680,19 +22895,22 @@
 38:29:DD,ONvocal ONvocal Inc
 38:2A:19,Technica Technica Engineering GmbH
 38:2B:78,"EcoPlugs Eco Plugs Enterprise Co., Ltd"
 38:2C:4A,ASUSTekC ASUSTek COMPUTER INC.
 38:2D:D1,"SamsungE Samsung Electronics Co.,Ltd"
 38:2D:E8,"SamsungE Samsung Electronics Co.,Ltd"
 38:30:F9,LGElectr LG Electronics (Mobile Communications)
+38:31:5A,Rinnai
 38:31:AC,Weg
 38:35:FB,Sagemcom Sagemcom Broadband SAS
 38:37:8B,"HuaweiTe Huawei Technologies Co.,Ltd"
 38:38:4B,"vivoMobi vivo Mobile Communication Co., Ltd."
 38:38:A6,AristaNe Arista Networks
+38:39:6C,"HuaweiDe Huawei Device Co., Ltd."
+38:39:8F,SiliconL Silicon Laboratories
 38:3A:21,IEEERegi IEEE Registration Authority
 38:3A:21:00:00:00/28,R3CInfor R3C Information(Shenzhen) Co.，Ltd.
 38:3A:21:10:00:00/28,HOBART HOBART GmbH
 38:3A:21:20:00:00/28,"Shenzhen Shenzhen HS Fiber Communication Equipment CO., LTD"
 38:3A:21:30:00:00/28,"Shanghai Shanghai Greatwall Safety System Co.,Ltd"
 38:3A:21:40:00:00/28,Dongguan Dongguan Innovation Technology Co Ltd
 38:3A:21:50:00:00/28,NPPUralt OOO NPP Uraltechnologiya
@@ -22706,15 +22924,15 @@
 38:3A:21:D0:00:00/28,Colooc Colooc AB
 38:3A:21:E0:00:00/28,"SDNwaret SDNware technology co.,LTD"
 38:3B:26,"JiangsuQ Jiangsu Qinheng Co., Ltd."
 38:3B:C8,2Wire 2Wire Inc
 38:3C:9C,"FujianNe Fujian Newland Payment Technology Co.,Ltd."
 38:3D:5B,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 38:3F:10,DBLTechn DBL Technology Ltd.
-38:3F:B3,Technico Technicolor CH USA Inc.
+38:3F:B3,VantivaU Vantiva USA LLC
 38:42:0B,"Sonos Sonos, Inc."
 38:42:33,Wildeboe Wildeboer Bauteile GmbH
 38:42:A6,Ingenieu Ingenieurbuero Stahlkopf
 38:43:69,PatrolPr Patrol Products Consortium LLC
 38:43:7D,"CompalBr Compal Broadband Networks, Inc."
 38:43:E5,Grotech Grotech Inc
 38:45:3B,RuckusWi Ruckus Wireless
@@ -22756,24 +22974,25 @@
 38:64:07,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
 38:65:04,"HonorDev Honor Device Co., Ltd."
 38:65:B2,"Apple Apple, Inc."
 38:66:45,"OOSICTec OOSIC Technology CO.,Ltd"
 38:66:F0,"Apple Apple, Inc."
 38:67:93,"AsiaOpti Asia Optical Co., Inc."
 38:68:93,IntelCor Intel Corporate
-38:68:A4,"SamsungE Samsung Electronics Co.,LTD"
+38:68:A4,"SamsungE Samsung Electronics Co.,Ltd"
 38:68:BE,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 38:68:DD,Inventec Inventec Corporation
 38:6A:77,"SamsungE Samsung Electronics Co.,Ltd"
 38:6B:1C,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 38:6B:BB,"ARRISGro ARRIS Group, Inc."
 38:6C:9B,IvyBiome Ivy Biomedical
 38:6E:21,WasionGr Wasion Group Ltd.
 38:6E:88,zte zte corporation
 38:6E:A2,"vivoMobi vivo Mobile Communication Co., Ltd."
+38:6F:6B,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 38:70:0C,"ARRISGro ARRIS Group, Inc."
 38:71:DE,"Apple Apple, Inc."
 38:72:C0,Comtrend Comtrend Corporation
 38:73:EA,IEEERegi IEEE Registration Authority
 38:73:EA:00:00:00/28,"L-3Commu L-3 Communications Mobile-Vision, Inc."
 38:73:EA:10:00:00/28,"KingWayI KingWay Information Co.,Ltd."
 38:73:EA:20:00:00/28,"Eyesight Eyesight(Shanghai)Communication Technology Co.,Ltd."
@@ -22804,50 +23023,53 @@
 38:86:02,Flexopti Flexoptix GmbH
 38:86:F7,"Google Google, Inc."
 38:87:D5,IntelCor Intel Corporate
 38:88:1E,"HuaweiTe Huawei Technologies Co.,Ltd"
 38:88:A4,"Apple Apple, Inc."
 38:89:2C,"Apple Apple, Inc."
 38:89:DC,OpticonS Opticon Sensors Europe B.V.
+38:8A:06,"SamsungE Samsung Electronics Co.,Ltd"
 38:8A:21,"UABTelto UAB ""Teltonika Telematics"""
 38:8A:B7,ITCNetwo ITC Networks
 38:8A:BE,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 38:8B:59,"Google Google, Inc."
 38:8C:50,LGElectr LG Electronics
 38:8E:7A,Autoit
 38:8E:E7,Fanhatta Fanhattan LLC
 38:8F:30,"SamsungE Samsung Electronics Co.,Ltd"
 38:90:52,"HuaweiTe Huawei Technologies Co.,Ltd"
 38:90:A5,"Cisco Cisco Systems, Inc"
 38:91:B7,"Cisco Cisco Systems, Inc"
 38:91:D5,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 38:91:FB,Xenox Xenox Holding BV
+38:92:2E,ArrayCom ArrayComm
 38:94:61,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 38:94:96,"SamsungE Samsung Electronics Co.,Ltd"
 38:94:E0,Syrotech Syrotech Networks. Ltd.
 38:94:ED,Netgear
 38:95:92,Tendyron Tendyron Corporation
 38:97:A4,"Elecom Elecom Co.,Ltd."
 38:97:D6,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 38:98:D8,"Meritech Meritech Co.,Ltd"
 38:98:E9,"HuaweiDe Huawei Device Co., Ltd."
 38:9A:F6,"SamsungE Samsung Electronics Co.,Ltd"
+38:9C:B2,"Apple Apple, Inc."
 38:9D:92,SeikoEps Seiko Epson Corporation
 38:9E:80,zte zte corporation
 38:9F:5A,C-KurTV C-Kur TV Inc.
 38:9F:83,OTN OTN Systems N.V.
 38:A0:67,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 38:A2:8C,"Shenzhen Shenzhen Rf-Link Technology Co.,Ltd."
 38:A4:4B,"HuaweiDe Huawei Device Co., Ltd."
 38:A4:ED,XiaomiCo Xiaomi Communications Co Ltd
 38:A5:3C,COMECERN COMECER Netherlands
 38:A5:B6,"Shenzhen Shenzhen Megmeet Electrical Co.,Ltd"
 38:A6:59,Sagemcom Sagemcom Broadband SAS
 38:A6:CE,SkyUk Sky Uk Limited
-38:A8:51,"MoogIng Moog, Ing"
+38:A8:51,"Quickset Quickset Defense Technologies, LLC"
 38:A8:6B,Orga Orga BV
 38:A8:9B,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 38:A8:CD,IEEERegi IEEE Registration Authority
 38:A8:CD:00:00:00/28,ACiiSTSm ACiiST Smart Networks Ltd.
 38:A8:CD:10:00:00/28,"FujicaSy Fujica System Co., ltd"
 38:A8:CD:20:00:00/28,"BeijingP Beijing Porient Technology Co., Ltd"
 38:A8:CD:30:00:00/28,"Dongguan Dongguan Fyrnetics Co., Ltd"
@@ -22862,14 +23084,15 @@
 38:A8:CD:C0:00:00/28,"BeijingA Beijing Aumiwalker technology CO.,LTD"
 38:A8:CD:D0:00:00/28,Annapurn Annapurna labs
 38:A8:CD:E0:00:00/28,Outform
 38:A9:1C,"NewH3CTe New H3C Technologies Co., Ltd"
 38:A9:5F,Actifio Actifio Inc
 38:A9:EA,"HkDapuEl Hk Dapu Electronic Technology Co., Limited"
 38:AA:3C,"SamsungE Samsung Electro Mechanics Co., Ltd."
+38:AB:16,NpoRtt Npo Rtt Llc
 38:AB:41,TexasIns Texas Instruments
 38:AC:3D,Nephos Nephos Inc
 38:AD:8E,"NewH3CTe New H3C Technologies Co., Ltd"
 38:AD:BE,"NewH3CTe New H3C Technologies Co., Ltd"
 38:AF:29,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 38:AF:D0,Nevro
 38:AF:D7,Fujitsu Fujitsu Limited
@@ -22891,14 +23114,15 @@
 38:B1:9E:D0:00:00/28,DallasDe Dallas Delta Corporation
 38:B1:9E:E0:00:00/28,ShenZhen ShenZhen ShuaiXian Electronic Equipment Co.Ltd
 38:B1:DB,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 38:B3:F7,"HuaweiDe Huawei Device Co., Ltd."
 38:B4:D3,BSHHausg BSH Hausgeraete GmbH
 38:B5:4D,"Apple Apple, Inc."
 38:B5:BD,EGOElekt E.G.O. Elektro-Ger
+38:B5:C9,IngramMi Ingram Micro Services
 38:B5:D3,SecuWork SecuWorks
 38:B7:25,WistronI Wistron Infocomm (Zhongshan) Corporation
 38:B7:4D,Fijowave Fijowave Limited
 38:B8:00,WistronN Wistron Neweb Corporation
 38:B8:EB,IEEERegi IEEE Registration Authority
 38:B8:EB:00:00:00/28,"BumjinC& Bumjin C&L Co., Ltd."
 38:B8:EB:10:00:00/28,1AConnec 1.A Connect GmbH
@@ -22907,15 +23131,15 @@
 38:B8:EB:40:00:00/28,Umlogics
 38:B8:EB:50:00:00/28,Dojo-Lab Dojo-Labs Ltd
 38:B8:EB:60:00:00/28,"Matrixst Matrixstream Technologies, Inc."
 38:B8:EB:70:00:00/28,SirinMob Sirin Mobile Technologies
 38:B8:EB:80:00:00/28,CeeNex CeeNex Inc
 38:B8:EB:90:00:00/28,NHSSiste NHS Sistemas de Energia
 38:B8:EB:A0:00:00/28,Secad Secad Sa
-38:B8:EB:B0:00:00/28,ExaScale ExaScaler Inc.
+38:B8:EB:B0:00:00/28,PEZYComp PEZY Computing K.K.
 38:B8:EB:C0:00:00/28,Ajax Ajax Systems Inc
 38:B8:EB:D0:00:00/28,"Yellowbr Yellowbrick Data, Inc."
 38:B8:EB:E0:00:00/28,WyresSAS Wyres SAS
 38:BA:B0,Broadcom
 38:BA:F8,IntelCor Intel Corporate
 38:BB:23,OzVision OzVision America LLC
 38:BB:3C,Avaya Avaya Inc
@@ -22982,14 +23206,16 @@
 38:F3:3F,Tatsuno Tatsuno Corporation
 38:F3:AB,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 38:F3:FB,Asperiq
 38:F5:54,"HisenseE Hisense Electric Co.,Ltd"
 38:F5:57,"Jolata Jolata, Inc."
 38:F5:97,home2net home2net GmbH
 38:F6:01,SolidSta Solid State Storage Technology Corporation
+38:F6:CF,zte zte corporation
+38:F6:ED,EVKDIKer EVK DI Kerschhaggl GmbH
 38:F7:08,"National National Resource Management, Inc."
 38:F7:3D,AmazonTe Amazon Technologies Inc.
 38:F7:B2,SeojunEl Seojun Electric
 38:F7:CD,IEEERegi IEEE Registration Authority
 38:F7:CD:00:00:00/28,PolskaFa Polska Fabryka Wodomierzy i Ciep?omierzy FILA
 38:F7:CD:10:00:00/28,NZIAConn NZIA Connect Inc
 38:F7:CD:20:00:00/28,"RIPower RIPower Co.,Ltd"
@@ -23010,14 +23236,15 @@
 38:F8:89,"HuaweiTe Huawei Technologies Co.,Ltd"
 38:F8:B7,V2ComPar V2Com Participacoes S.A.
 38:F8:CA,OWIN OWIN Inc.
 38:F8:F6,Adtran Adtran Inc
 38:F9:D3,"Apple Apple, Inc."
 38:FA:CA,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 38:FB:14,"HuaweiTe Huawei Technologies Co.,Ltd"
+38:FC:34,"HuaweiDe Huawei Device Co., Ltd."
 38:FC:98,IntelCor Intel Corporate
 38:FD:F5,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 38:FD:F8,"Cisco Cisco Systems, Inc"
 38:FD:FE,IEEERegi IEEE Registration Authority
 38:FD:FE:00:00:00/28,"EdgeI&D Edge I&D Co., Ltd."
 38:FD:FE:10:00:00/28,"WaytoneB Waytone (Beiijng) Communications Co.,Ltd"
 38:FD:FE:20:00:00/28,"SmartSol Smart Solution Technology, Inc"
@@ -23033,17 +23260,19 @@
 38:FD:FE:C0:00:00/28,"NewGarde New Garden Co., Ltd."
 38:FD:FE:D0:00:00/28,FUBAAuto FUBA Automotive Electronics GmbH
 38:FD:FE:E0:00:00/28,"iSmartel iSmart electronic technology co.,LTD"
 38:FE:C5,Ellips Ellips B.V.
 38:FF:13,"JointSto Joint Stock Company ""Research Instinite ""Masshtab"""
 38:FF:36,RuckusWi Ruckus Wireless
 3A:02:92,VideoEle Video Electronics Standards Association
+3A:0E:75,Kevcom Kevcom Llc
 3A:35:41,Raspberr Raspberry Pi (Trading) Ltd
 3A:5A:27,"Shenzhen Shenzhen Longsys Electronics Co.,Ltd."
 3A:5E:03,"CirrusDa Cirrus Data Solutions, Inc"
+3A:72:C2,"HuaweiTe Huawei Technologies Co.,Ltd"
 3A:76:5D,"NewCoSem NewCoSemi(Beijing) Technology Co., Ltd"
 3A:78:CA,SoundTal SoundTalks NV
 3A:79:6E,"LXSemico LX Semicon co.,Ltd."
 3A:A3:F8,IEEE8021 IEEE 802.1 Chair
 3A:BA:37,Cirrent
 3A:CF:C5,Quicklin Quickline AG
 3A:F5:21,SingleDi Single Digits
@@ -23058,20 +23287,22 @@
 3C:05:AB,ProductC Product Creation Studio
 3C:06:30,"Apple Apple, Inc."
 3C:06:64,"BeijingL Beijing Leagrid Technology Co.,Ltd."
 3C:06:A7,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 3C:07:54,"Apple Apple, Inc."
 3C:07:71,Sony Sony Corporation
 3C:08:1E,"BeijingY Beijing Yupont Electric Power Technology Co.,Ltd"
+3C:08:CD,JuniperN Juniper Networks
 3C:08:F6,"Cisco Cisco Systems, Inc"
 3C:09:6D,Powerhou Powerhouse Dynamics
 3C:0B:4F,YandexSe Yandex Services AG
 3C:0C:48,"Servergy Servergy, Inc."
 3C:0C:7D,TinyMesh Tiny Mesh AS
-3C:0C:DB,"Unionman Unionman Technology Co.,Ltd"
+3C:0C:DB,"UnionMan Union Man Technology Co.,Ltd"
+3C:0D:2C,Liquid-M Liquid-Markets GmbH
 3C:0E:23,"Cisco Cisco Systems, Inc"
 3C:0F:C1,KBCNetwo KBC Networks
 3C:10:40,daesungn daesung network
 3C:10:6F,Albahith Albahith Technologies
 3C:10:E6,PHAZR PHAZR Inc.
 3C:11:B2,Fraunhof Fraunhofer FIT
 3C:13:5A,XiaomiCo Xiaomi Communications Co Ltd
@@ -23082,22 +23313,24 @@
 3C:15:FB,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:17:10,Sagemcom Sagemcom Broadband SAS
 3C:18:9F,Nokia Nokia Corporation
 3C:18:A0,Luxshare Luxshare Precision Industry Company Limited
 3C:19:15,GFIChron GFI Chrono Time
 3C:19:5E,"SamsungE Samsung Electronics Co.,Ltd"
 3C:19:7D,Ericsson Ericsson AB
+3C:19:CB,TecnoMob Tecno Mobile Limited
 3C:1A:0F,ClearSky ClearSky Data
 3C:1A:57,Cardiopu Cardiopulmonary Corp
 3C:1A:79,"HuayuanT Huayuan Technology CO.,LTD"
 3C:1A:9E,VitalThi VitalThings AS
 3C:1B:F8,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 3C:1C:BE,Jadak Jadak Llc
 3C:1E:04,D-LinkIn D-Link International
 3C:1E:13,"Hangzhou Hangzhou Sunrise Technology Co., Ltd"
+3C:1E:B5,"Apple Apple, Inc."
 3C:20:93,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 3C:20:F6,"SamsungE Samsung Electronics Co.,Ltd"
 3C:21:9C,IntelCor Intel Corporate
 3C:22:FB,"Apple Apple, Inc."
 3C:24:F0,IEEERegi IEEE Registration Authority
 3C:24:F0:00:00:00/28,"Shenzhen Shenzhen Pinsida Technology Co.,Ltd."
 3C:24:F0:10:00:00/28,Abrites Abrites Ltd.
@@ -23121,22 +23354,26 @@
 3C:28:6D,"Google Google, Inc."
 3C:28:A6,Alcatel- Alcatel-Lucent Enterprise (China)
 3C:2A:F4,"BrotherI Brother Industries, LTD."
 3C:2C:30,Dell Dell Inc.
 3C:2C:94,"杭州德澜科技有限 杭州德澜科技有限公司（HangZhou Delan Technology Co.,Ltd）"
 3C:2C:99,Edgecore Edgecore Networks Corporation
 3C:2C:A6,"BeijingX Beijing Xiaomi Electronics Co.,Ltd"
+3C:2D:9E,Vantiva- Vantiva - Connected Home
 3C:2D:B7,TexasIns Texas Instruments
+3C:2E:F5,SiliconL Silicon Laboratories
 3C:2E:F9,"Apple Apple, Inc."
 3C:2E:FF,"Apple Apple, Inc."
 3C:2F:3A,SFORZATO SFORZATO Corp.
 3C:30:0C,DewarEle Dewar Electronics Pty Ltd
 3C:30:6F,"HuaweiTe Huawei Technologies Co.,Ltd"
+3C:31:74,"Google Google, Inc."
 3C:31:78,Qolsys Qolsys Inc.
 3C:33:00,"Shenzhen Shenzhen Bilian electronic CO.,LTD"
+3C:33:32,D-Link D-Link Corporation
 3C:35:56,Cognitec Cognitec Systems GmbH
 3C:36:3D,Nokia Nokia Corporation
 3C:36:E4,"ARRISGro ARRIS Group, Inc."
 3C:37:12,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 3C:37:86,Netgear
 3C:38:88,"ConnectQ ConnectQuest, llc"
 3C:38:F4,Sony Sony Corporation
@@ -23155,14 +23392,15 @@
 3C:39:E7:90:00:00/28,ZoneCont Zone Controls AB
 3C:39:E7:A0:00:00/28,iiM iiM AG
 3C:39:E7:B0:00:00/28,"chipsgui chipsguide technology Co.,LTD"
 3C:39:E7:C0:00:00/28,"Vanstone Vanstone Electronic (Beijing)Co,. Ltd."
 3C:39:E7:E0:00:00/28,Marposs Marposs Spa
 3C:39:E7:F0:00:00/28,Private
 3C:3A:73,Avaya Avaya Inc
+3C:3B:4D,"ToyoSeis Toyo Seisakusho Kaisha, Limited"
 3C:3B:99,ItelMobi Itel Mobile Limited
 3C:3F:51,2Crsi
 3C:40:4F,"Guangdon Guangdong Pisen Electronics Co.,Ltd"
 3C:41:0E,"Cisco Cisco Systems, Inc"
 3C:42:7E,IEEERegi IEEE Registration Authority
 3C:42:7E:00:00:00/28,Grandway Grandway Technology (Shenzhen) Limited
 3C:42:7E:10:00:00/28,"Dongguan Dongguan Taide Industrial Co.,Ltd."
@@ -23178,26 +23416,28 @@
 3C:42:7E:B0:00:00/28,CompalEl Compal Electronics INC.
 3C:42:7E:C0:00:00/28,PrivacyL Privacy Labs
 3C:42:7E:D0:00:00/28,"RoboxSma Robox Smart Motion (Wuhu) Co.,Ltd"
 3C:42:7E:E0:00:00/28,"Xiaoniun Xiaoniu network technology (Shanghai) Co., Ltd."
 3C:43:8E,"ARRISGro ARRIS Group, Inc."
 3C:45:7A,SkyUk Sky Uk Limited
 3C:46:45,"Shanghai Shanghai Infinity Wireless Technologies Co.,Ltd."
+3C:46:A1,RuckusWi Ruckus Wireless
 3C:46:D8,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 3C:47:11,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:47:9B,"Theissen Theissen Training Systems, Inc."
 3C:49:37,ASSMANNE ASSMANN Electronic GmbH
 3C:4A:92,HewlettP Hewlett Packard
 3C:4C:69,Infinity Infinity System S.L.
 3C:4C:D0,CeragonN Ceragon Networks
 3C:4D:BE,"Apple Apple, Inc."
 3C:4E:47,Etronic Etronic A/S
 3C:4E:56,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 3C:51:0E,"Cisco Cisco Systems, Inc"
 3C:52:82,HewlettP Hewlett Packard
+3C:52:A1,TP-Link TP-Link Corporation Limited
 3C:53:D7,Cedes Cedes Ag
 3C:54:47,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:55:76,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 3C:57:31,"Cisco Cisco Systems, Inc"
 3C:57:4F,"ChinaMob China Mobile Group Device Co.,Ltd."
 3C:57:6C,"SamsungE Samsung Electronics Co.,Ltd"
 3C:57:BD,KesslerC Kessler Crane Inc.
@@ -23242,35 +23482,37 @@
 3C:6A:48,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 3C:6A:7D,"NiigataP Niigata Power Systems Co., Ltd."
 3C:6A:9D,DexatekT Dexatek Technology LTD.
 3C:6A:A7,IntelCor Intel Corporate
 3C:6D:89,"Apple Apple, Inc."
 3C:6E:63,Mitron Mitron OY
 3C:6F:45,Fiberpro Fiberpro Inc.
+3C:6F:9B,zte zte corporation
 3C:6F:EA,Panasoni Panasonic India Pvt. Ltd.
 3C:6F:F7,"EnTek EnTek Systems, Inc."
 3C:70:59,MakerBot MakerBot Industries
 3C:71:BF,Espressi Espressif Inc.
 3C:74:37,Rim
 3C:75:4A,"ARRISGro ARRIS Group, Inc."
 3C:77:E6,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 3C:78:43,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:78:73,Airsonic Airsonics
+3C:79:2B,"Dongguan Dongguan Auklink TechnologyCo.,Ltd"
 3C:7A:8A,"ARRISGro ARRIS Group, Inc."
 3C:7A:AA,ChinaDra China Dragon Technology Limited
 3C:7A:C4,Chemtron Chemtronics
 3C:7A:F0,ItelMobi Itel Mobile Limited
 3C:7C:3F,ASUSTekC ASUSTek COMPUTER INC.
 3C:7D:0A,"Apple Apple, Inc."
 3C:7D:B1,TexasIns Texas Instruments
 3C:7F:6F,"Telechip Telechips, Inc."
 3C:80:6B,"HunanVoc Hunan Voc Acoustics Technology Co., Ltd."
 3C:80:AA,RansnetS Ransnet Singapore Pte Ltd
 3C:81:D8,Sagemcom Sagemcom Broadband SAS
-3C:82:C0,Technico Technicolor CH USA Inc.
+3C:82:C0,VantivaU Vantiva USA LLC
 3C:83:1E,CKD CKD Corporation
 3C:83:75,Microsof Microsoft Corporation
 3C:83:B5,AdvanceV Advance Vision Electronics Co. Ltd.
 3C:84:6A,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 3C:86:9A,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:86:A8,"Sangshin Sangshin elecom.co,, LTD"
 3C:86:D1,"vivoMobi vivo Mobile Communication Co., Ltd."
@@ -23297,16 +23539,17 @@
 3C:93:F4,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:94:D5,JuniperN Juniper Networks
 3C:95:09,LiteonTe Liteon Technology Corporation
 3C:97:0E,"WistronI Wistron InfoComm(Kunshan)Co.,Ltd."
 3C:97:7E,IPSTechn IPS Technology Limited
 3C:98:72,Sercomm Sercomm Corporation.
 3C:98:BF,"QuestCon Quest Controls, Inc."
+3C:99:8C,HouwaSys Houwa System Design Corp.
 3C:99:F7,Lansente Lansentechnology AB
-3C:9A:77,Technico Technicolor CH USA Inc.
+3C:9A:77,VantivaU Vantiva USA LLC
 3C:9B:C6,"HuaweiDe Huawei Device Co., Ltd."
 3C:9B:D6,"Vizio Vizio, Inc"
 3C:9C:0F,IntelCor Intel Corporate
 3C:9D:56,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:9E:C7,SkyUk Sky Uk Limited
 3C:9F:81,"Shenzhen Shenzhen CATIC Bit Communications Technology Co.,Ltd"
 3C:9F:C3,"BeijingS Beijing Sinead Technology Co., Ltd."
@@ -23335,35 +23578,37 @@
 3C:B0:7E,"AroundsI Arounds Intelligent Equipment Co., Ltd."
 3C:B1:5B,Avaya Avaya Inc
 3C:B1:7F,Wattwatc Wattwatchers Pty Ld
 3C:B2:33,"HuaweiDe Huawei Device Co., Ltd."
 3C:B5:3D,"HunanGok Hunan Goke Microelectronics Co.,Ltd"
 3C:B6:B7,"vivoMobi vivo Mobile Communication Co., Ltd."
 3C:B7:2B,PLUMgrid PLUMgrid Inc
-3C:B7:4B,Technico Technicolor CH USA Inc.
+3C:B7:4B,VantivaU Vantiva USA LLC
 3C:B7:92,"HitachiM Hitachi Maxell, Ltd., Optronics Division"
 3C:B8:7A,Private
 3C:B9:A6,BeldenDe Belden Deutschland GmbH
 3C:BB:73,"Shenzhen Shenzhen Xinguodu Technology Co., Ltd."
 3C:BB:FD,"SamsungE Samsung Electronics Co.,Ltd"
 3C:BC:D0,zte zte corporation
 3C:BD:3E,"BeijingX Beijing Xiaomi Electronics Co., Ltd."
 3C:BD:C5,Arcadyan Arcadyan Corporation
 3C:BD:D8,LgElectr Lg Electronics Inc
 3C:BE:E1,Nikon Nikon Corporation
 3C:BF:60,"Apple Apple, Inc."
+3C:C0:3E,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:C0:79,"Shenzhen Shenzhen One-Nine Intelligent Electronic Science and Technology Co., Ltd"
 3C:C0:C6,d&baudio d&b audiotechnik GmbH
 3C:C1:2C,AES AES Corporation
 3C:C1:F6,Melange Melange Systems Pvt. Ltd.
 3C:C2:43,Nokia Nokia Corporation
 3C:C2:E1,"XinhuaCo Xinhua Control Engineering Co.,Ltd"
 3C:C7:86,"Dongguan Dongguan Huarong Communication Technologies Co.,Ltd."
 3C:C9:9E,"HuiyangT Huiyang Technology Co., Ltd"
 3C:CA:87,Iders Iders Incorporated
+3C:CB:4D,"Avikus Avikus Co., Ltd"
 3C:CB:7C,TCTmobil TCT mobile ltd
 3C:CD:36,"Apple Apple, Inc."
 3C:CD:57,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 3C:CD:5A,Technisc Technische Alternative GmbH
 3C:CD:5D,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:CD:93,LgElectr Lg Electronics Inc
 3C:CE:0D,"Shenzhen Shenzhen juduoping Technology Co.,Ltd"
@@ -23381,14 +23626,15 @@
 3C:DA:2A,zte zte corporation
 3C:DA:6D,"TiandyTe Tiandy Technologies CO.,LTD"
 3C:DC:BC,"SamsungE Samsung Electronics Co.,Ltd"
 3C:DD:89,"SomoHold Somo Holdings & Tech. Co.,Ltd."
 3C:DF:1E,"Cisco Cisco Systems, Inc"
 3C:DF:A9,"ARRISGro ARRIS Group, Inc."
 3C:DF:BD,"HuaweiTe Huawei Technologies Co.,Ltd"
+3C:E0:02,TexasIns Texas Instruments
 3C:E0:38,Omnifi Omnifi Inc.
 3C:E0:64,TexasIns Texas Instruments
 3C:E0:72,"Apple Apple, Inc."
 3C:E1:A1,"Universa Universal Global Scientific Industrial Co., Ltd."
 3C:E3:6B,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 3C:E3:E7,"ChinaMob China Mobile Group Device Co.,Ltd."
 3C:E4:41,AmazonTe Amazon Technologies Inc.
@@ -23398,29 +23644,33 @@
 3C:E6:24,LGDispla LG Display
 3C:E8:24,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:E9:0E,Espressi Espressif Inc.
 3C:E9:F7,IntelCor Intel Corporate
 3C:EA:4F,2Wire 2Wire Inc
 3C:EA:F9,Jubixcol Jubixcoltd
 3C:EA:FB,Nse Nse Ag
+3C:EC:DE,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 3C:EC:EF,"SuperMic Super Micro Computer, Inc."
+3C:EF:42,TCTmobil TCT mobile ltd
 3C:EF:8C,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 3C:F0:11,IntelCor Intel Corporate
 3C:F3:92,Virtualt Virtualtek. Co. Ltd
 3C:F4:F9,Moda-Inn Moda-InnoChips
 3C:F5:2C,DSPECIAL DSPECIALISTS GmbH
 3C:F5:91,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 3C:F5:CC,"NewH3CTe New H3C Technologies Co., Ltd"
 3C:F6:52,zte zte corporation
+3C:F6:92,"HuaweiDe Huawei Device Co., Ltd."
 3C:F7:2A,Nokia Nokia Corporation
 3C:F7:48,"Shenzhen Shenzhen Linsn Technology Development Co.,Ltd"
 3C:F7:A4,"SamsungE Samsung Electronics Co.,Ltd"
 3C:F7:D1,OMRON OMRON Corporation
 3C:F8:08,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:F8:62,IntelCor Intel Corporate
+3C:F9:F0,zte zte corporation
 3C:FA:06,Microsof Microsoft Corporation
 3C:FA:43,"HuaweiTe Huawei Technologies Co.,Ltd"
 3C:FA:D3,IEEERegi IEEE Registration Authority
 3C:FA:D3:00:00:00/28,HomeCont Home Control AS
 3C:FA:D3:10:00:00/28,Annapurn Annapurna labs
 3C:FA:D3:20:00:00/28,NaruidaT Naruida Technology Ltd.
 3C:FA:D3:30:00:00/28,"HarmanCo Harman Connected Services, Inc."
@@ -23451,14 +23701,15 @@
 40:06:A0,TexasIns Texas Instruments
 40:06:D5,"Cisco Cisco Systems, Inc"
 40:07:C0,Railtec Railtec Systems GmbH
 40:0D:10,"ARRISGro ARRIS Group, Inc."
 40:0E:67,Tremol Tremol Ltd.
 40:0E:85,SamsungE Samsung Electro-Mechanics(Thailand)
 40:0E:F3,zte zte corporation
+40:0F:C1,VantivaU Vantiva USA LLC
 40:11:75,IEEERegi IEEE Registration Authority
 40:11:75:00:00:00/28,"LexiDevi Lexi Devices, Inc."
 40:11:75:10:00:00/28,"FujianKu Fujian Kuke3D Technology Co.,LTD"
 40:11:75:20:00:00/28,KandaKog Kanda Kogyo
 40:11:75:30:00:00/28,"BeijingH Beijing Hexinruitong Electric Power Technology Co., Ltd."
 40:11:75:40:00:00/28,TableTra Table Trac Inc
 40:11:75:50:00:00/28,MircElec Mirc Electronics Ltd
@@ -23471,14 +23722,15 @@
 40:11:75:C0:00:00/28,disguise disguise Technologies Limited
 40:11:75:D0:00:00/28,"NanJingH NanJing HuaStart Network Technology Co.,Ltd."
 40:11:75:E0:00:00/28,Nibble
 40:11:C3,"SamsungE Samsung Electronics Co.,Ltd"
 40:11:DC,Sonance
 40:12:E4,Compass- Compass-EOS
 40:13:D9,GlobalES Global ES
+40:14:82,"Cisco Cisco Systems, Inc"
 40:14:AD,"HuaweiDe Huawei Device Co., Ltd."
 40:15:97,"ProtectA Protect America, Inc."
 40:16:3B,"SamsungE Samsung Electronics Co.,Ltd"
 40:16:7E,ASUSTekC ASUSTek COMPUTER INC.
 40:16:9F,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 40:16:FA,EKMMeter EKM Metering
 40:17:E2,IntaiTec Intai Technology Corp.
@@ -23495,21 +23747,23 @@
 40:22:ED,DigitalP Digital Projection Ltd
 40:23:43,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 40:24:B2,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 40:25:C2,IntelCor Intel Corporate
 40:26:19,"Apple Apple, Inc."
 40:27:0B,"Mobileec Mobileeco Co., Ltd"
 40:28:14,RFIEngin RFI Engineering
+40:2A:8F,"Shanghai Shanghai High-Flying Electronics Technology Co., Ltd"
 40:2B:50,"ARRISGro ARRIS Group, Inc."
 40:2B:69,KumhoEle Kumho Electric Inc.
 40:2B:A1,Sony Sony Corporation
 40:2C:76,IEEERegi IEEE Registration Authority
 40:2C:76:00:00:00/28,Lista Lista AG
 40:2C:76:10:00:00/28,Shanghai Shanghai Dahua Scale Factory
 40:2C:76:20:00:00/28,Annapurn Annapurna labs
+40:2C:76:30:00:00/28,Embedded EmbeddedArt AB
 40:2C:76:40:00:00/28,"BeijingS Beijing Smarot Technology Co., Ltd."
 40:2C:76:50:00:00/28,BaumerBo Baumer Bourdon-Haenni
 40:2C:76:60:00:00/28,"Guangzho Guangzhou LANGO Electronics Technology Co., Ltd."
 40:2C:76:70:00:00/28,"Zhejiang Zhejiang Guoli Security Technology Co., Ltd."
 40:2C:76:80:00:00/28,"SutengIn Suteng Innovation Technology Co., Ltd."
 40:2C:76:90:00:00/28,Annapurn Annapurna labs
 40:2C:76:A0:00:00/28,NowTechn NowTechnologies Zrt
@@ -23536,17 +23790,19 @@
 40:3F:8C,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 40:40:22,Ziv
 40:40:28,Ziv
 40:40:6B,Icomera
 40:40:6C,Icomera
 40:40:A7,Sony Sony Corporation
 40:41:01,Rockwell Rockwell Automation
+40:41:0D,"HuaweiTe Huawei Technologies Co.,Ltd"
 40:42:29,"Layer3TV Layer3TV, Inc"
 40:42:44,"Cisco Cisco Systems, Inc"
 40:44:FD,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
+40:45:C4,"HuaweiTe Huawei Technologies Co.,Ltd"
 40:45:DA,"Spreadtr Spreadtrum Communications (Shanghai) Co., Ltd."
 40:47:5E,eero eero inc.
 40:47:6A,AstroGam Astro Gaming
 40:48:FD,IEEERegi IEEE Registration Authority
 40:48:FD:00:00:00/28,"BeijingC Beijing C&W Electronics(Group)Co.,Ltd"
 40:48:FD:10:00:00/28,FastProg Fast Programming
 40:48:FD:20:00:00/28,"MITHRAST MITHRAS Technology Co., LTD"
@@ -23564,18 +23820,20 @@
 40:48:FD:E0:00:00/28,SmartSen Smart Sensor Devices Ab
 40:49:0F,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 40:49:8A,Synaptic Synapticon GmbH
 40:4A:03,ZyxelCom Zyxel Communications Corporation
 40:4A:18,AddrekSm Addrek Smart Solutions
 40:4A:D4,Widex Widex A/S
 40:4C:77,"ARRISGro ARRIS Group, Inc."
+40:4C:CA,Espressi Espressif Inc.
 40:4D:7F,"Apple Apple, Inc."
 40:4D:8E,"HuaweiTe Huawei Technologies Co.,Ltd"
 40:4E:36,HTC HTC Corporation
 40:4E:EB,"HigherWa Higher Way Electronic Co., Ltd."
+40:4F:42,"HuaweiTe Huawei Technologies Co.,Ltd"
 40:50:B5,"Shenzhen Shenzhen New Species Technology Co., Ltd."
 40:50:E0,MiltonSe Milton Security Group LLC
 40:51:6C,GrandexI Grandex International Corporation
 40:52:0D,PicoTech Pico Technology
 40:54:E4,Wearsafe Wearsafe Labs Inc
 40:55:39,"Cisco Cisco Systems, Inc"
 40:55:82,Nokia
@@ -23611,52 +23869,58 @@
 40:70:09,"ARRISGro ARRIS Group, Inc."
 40:70:4A,PowerIde Power Idea Technology Limited
 40:70:74,"LifeTech Life Technology (China) Co., Ltd"
 40:70:F5,"Apple Apple, Inc."
 40:71:83,JuniperN Juniper Networks
 40:74:96,aFUNTECH aFUN TECHNOLOGY INC.
 40:74:E0,IntelCor Intel Corporate
-40:75:C3,Technico Technicolor CH USA Inc.
+40:75:C3,VantivaU Vantiva USA LLC
 40:76:A9,"HuaweiDe Huawei Device Co., Ltd."
 40:77:A9,"NewH3CTe New H3C Technologies Co., Ltd"
 40:78:6A,"Motorola Motorola Mobility LLC, a Lenovo Company"
 40:78:75,IMBEL-In IMBEL - Industria de Material Belico do Brasil
+40:79:12,TexasIns Texas Instruments
 40:7A:80,Nokia Nokia Corporation
 40:7B:1B,MettleNe Mettle Networks Inc.
 40:7C:7D,Nokia
 40:7D:0F,"HuaweiTe Huawei Technologies Co.,Ltd"
+40:7F:5F,JuniperN Juniper Networks
 40:7F:E0,GlorySta Glory Star Technics (ShenZhen) Limited
 40:82:56,Continen Continental Automotive GmbH
 40:83:1D,"Apple Apple, Inc."
 40:83:DE,ZebraTec Zebra Technologies Inc
+40:84:32,Microchi Microchip Technology Inc.
 40:84:93,Claviste Clavister AB
 40:86:2E,"JdmMobil Jdm Mobile Internet Solution Co., Ltd."
 40:88:05,"Motorola Motorola Mobility LLC, a Lenovo Company"
 40:88:2F,"ExtremeN Extreme Networks, Inc."
 40:88:E0,BeijingE Beijing Ereneben Information Technology Limited Shenzhen Branch
 40:89:A8,"WiredIQ WiredIQ, LLC"
 40:8A:9A,"TITENG TITENG CO., Ltd."
 40:8B:07,"Actionte Actiontec Electronics, Inc"
 40:8B:F6,"Shenzhen Shenzhen TCL New Technology Co., Ltd"
 40:8C:1F,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 40:8C:4C,"Shenzhen Shenzhen MiaoMing Intelligent Technology Co.,Ltd"
 40:8D:5C,"Giga-Byt Giga-Byte Technology Co.,Ltd."
+40:8E:2C,Microsof Microsoft Corporation
 40:8E:DF,"HuaweiDe Huawei Device Co., Ltd."
 40:8E:F6,Infinixm Infinix mobility limited
 40:8F:9D,JuniperN Juniper Networks
 40:91:51,Espressi Espressif Inc.
+40:92:1A,"Apple Apple, Inc."
 40:95:05,"AcoinfoT Acoinfo Technology Co.,Ltd"
 40:95:58,Aisino Aisino Corporation
 40:95:BD,"NTmore NTmore.Co.,Ltd"
 40:97:D1,BKElectr BK Electronics cc
 40:98:4C,CasacomS Casacom Solutions AG
 40:98:4E,TexasIns Texas Instruments
 40:98:7B,Aisino Aisino Corporation
 40:98:AD,"Apple Apple, Inc."
 40:99:22,AzureWav AzureWave Technology Inc.
+40:9A:30,TecnoMob Tecno Mobile Limited
 40:9B:0D,"Shenzhen Shenzhen Yourf Kwan Industrial Co., Ltd"
 40:9B:21,Nokia
 40:9B:CD,D-LinkIn D-Link International
 40:9C:28,"Apple Apple, Inc."
 40:9C:A6,Curvalux
 40:9F:38,AzureWav AzureWave Technology Inc.
 40:9F:87,JideTech Jide Technology (Hong Kong) Limited
@@ -23707,14 +23971,15 @@
 40:B4:F0,JuniperN Juniper Networks
 40:B5:C1,"Cisco Cisco Systems, Inc"
 40:B6:07,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 40:B6:88,LEGICIde LEGIC Identsystems AG
 40:B6:B1,"SUNGSAM SUNGSAM CO,.Ltd"
 40:B6:E7,"HuaweiDe Huawei Device Co., Ltd."
 40:B7:F3,"ARRISGro ARRIS Group, Inc."
+40:B7:FC,PhyplusM Phyplus Microelectronics Limited
 40:B8:37,Sony Sony Corporation
 40:B8:9A,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 40:B9:3C,HewlettP Hewlett Packard Enterprise
 40:BA:61,ARIMACom ARIMA Communications Corp.
 40:BC:60,"Apple Apple, Inc."
 40:BC:68,"WuhanFun Wuhan Funshion Online Technologies Co.,Ltd"
 40:BC:73,Cronopla Cronoplast S.L.
@@ -23745,15 +24010,17 @@
 40:D2:5F,ItelMobi Itel Mobile Limited
 40:D2:8A,"Nintendo Nintendo Co., Ltd."
 40:D3:2D,"Apple Apple, Inc."
 40:D3:57,"IsonTech Ison Technology Co., Ltd."
 40:D3:AE,"SamsungE Samsung Electronics Co.,Ltd"
 40:D4:0E,Biodata Biodata Ltd
 40:D4:BD,"SKNetwor SK Networks Service CO., LTD."
+40:D4:F6,"HonorDev Honor Device Co., Ltd."
 40:D5:59,MicroSER Micro S.E.R.I.
+40:D5:63,HANAElec HANA Electronics
 40:D6:3C,"Equitech Equitech Industrial(DongGuan)Co.,Ltd"
 40:D8:55,IEEERegi IEEE Registration Authority
 40:D8:55:00:00:00/36,Xronos Xronos.Inc
 40:D8:55:00:10:00/36,Vemotion
 40:D8:55:00:20:00/36,Hangzhou Hangzhou Chenxiao Technologies Co. Ltd.
 40:D8:55:00:30:00/36,AlphaNav AlphaNavigation coltd
 40:D8:55:00:40:00/36,"CRMagnet CR Magnetics, Inc."
@@ -24254,14 +24521,15 @@
 40:E6:4B,"Apple Apple, Inc."
 40:E7:30,"DEYStora DEY Storage Systems, Inc."
 40:E7:93,"Shenzhen Shenzhen Siviton Technology Co.,Ltd"
 40:E9:9B,SamsungE Samsung Electro-Mechanics(Thailand)
 40:EA:CE,"FounderB Founder Broadband Network Service Co.,Ltd"
 40:EC:99,IntelCor Intel Corporate
 40:EC:F8,Siemens Siemens AG
+40:ED:00,TP-Link TP-Link Corporation Limited
 40:ED:98,IEEERegi IEEE Registration Authority
 40:ED:98:00:00:00/28,"Tsinghua Tsinghua Tongfang Co., LTD"
 40:ED:98:10:00:00/28,"GuangZho GuangZhou FiiO Electronics Technology Co.,Ltd"
 40:ED:98:20:00:00/28,A-Iox A-Iox Inc.
 40:ED:98:30:00:00/28,Knox Knox Company
 40:ED:98:40:00:00/28,Kendrion Kendrion Kuhnke Automation GmbH
 40:ED:98:50:00:00/28,Cape
@@ -24279,15 +24547,15 @@
 40:EE:DD,"HuaweiTe Huawei Technologies Co.,Ltd"
 40:EF:4C,"Fihonest Fihonest communication co.,Ltd"
 40:F0:2F,LiteonTe Liteon Technology Corporation
 40:F0:4E,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 40:F0:78,"Cisco Cisco Systems, Inc"
 40:F1:4C,ISEEurop ISE Europe SPRL
 40:F2:01,Sagemcom Sagemcom Broadband SAS
-40:F2:1C,DASANZho DASAN Zhone Solutions
+40:F2:1C,DZS DZS Inc.
 40:F2:E9,Ibm
 40:F3:08,"MurataMa Murata Manufacturing Co., Ltd."
 40:F3:85,IEEERegi IEEE Registration Authority
 40:F3:85:00:00:00/28,SubPac
 40:F3:85:10:00:00/28,JohnsonM Johnson Matthey
 40:F3:85:20:00:00/28,BeijingZ Beijing Zongheng Electro-Mechanical Technology Development Co.
 40:F3:85:30:00:00/28,IntelliD IntelliDesign Pty Ltd
@@ -24298,30 +24566,33 @@
 40:F3:85:80:00:00/28,Teleepoc Teleepoch Ltd
 40:F3:85:90:00:00/28,FastPrec Fast Precision Technologies Co. Ltd.
 40:F3:85:A0:00:00/28,Creanord
 40:F3:85:B0:00:00/28,URMETHom URMET Home & Building Solutions Pty Ltd
 40:F3:85:C0:00:00/28,ClixxoBr Clixxo Broadband Private Limited
 40:F3:85:D0:00:00/28,DigitalB Digital Bros S.p.A.
 40:F3:85:E0:00:00/28,BBB BBB Inc.
+40:F3:B0,TexasIns Texas Instruments
 40:F4:07,"Nintendo Nintendo Co., Ltd."
 40:F4:13,Rubezh
 40:F4:20,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 40:F4:EC,"Cisco Cisco Systems, Inc"
-40:F4:FD,"Unionman Unionman Technology Co.,Ltd"
+40:F4:FD,"UnionMan Union Man Technology Co.,Ltd"
 40:F5:20,Espressi Espressif Inc.
 40:F5:2E,LeicaMic Leica Microsystems (Schweiz) AG
 40:F6:BC,AmazonTe Amazon Technologies Inc.
 40:F8:DF,Canon Canon Inc.
 40:F9:46,"Apple Apple, Inc."
 40:F9:D5,TecoreNe Tecore Networks
 40:FA:7F,PrehCarC Preh Car Connect GmbH
+40:FA:FE,"Motorola Motorola Mobility LLC, a Lenovo Company"
 40:FC:89,"ARRISGro ARRIS Group, Inc."
 40:FD:F3,"AMPAKTec AMPAK Technology,Inc."
 40:FE:0D,Maxio
 40:FE:95,"NewH3CTe New H3C Technologies Co., Ltd"
+40:FF:40,GloquadT GloquadTech
 44:00:10,"Apple Apple, Inc."
 44:00:49,AmazonTe Amazon Technologies Inc.
 44:00:4D,"HuaweiTe Huawei Technologies Co.,Ltd"
 44:01:BB,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 44:03:2C,IntelCor Intel Corporate
 44:03:77,IEEERegi IEEE Registration Authority
 44:03:77:00:00:00/28,"MusashiS Musashi Seimitsu Industry Co.,Ltd"
@@ -24337,14 +24608,15 @@
 44:03:77:A0:00:00/28,symplr
 44:03:77:B0:00:00/28,"Hangzhou Hangzhou Asia Infrastructure Tech. Co., Ltd."
 44:03:77:C0:00:00/28,"BIGClima BIG Climatic Manufacture, Co. LTD, Zhongshan Branch"
 44:03:77:D0:00:00/28,Omnisens Omnisense Systems Private Limited Taiwan Branch
 44:03:77:E0:00:00/28,"BolinTec Bolin Technology Co., Ltd"
 44:03:A7,"Cisco Cisco Systems, Inc"
 44:04:44,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+44:05:3F,Sagemcom Sagemcom Broadband SAS
 44:05:E8,twareLAB
 44:07:0B,"Google Google, Inc."
 44:09:B8,"SalcompS Salcomp (Shenzhen) CO., LTD."
 44:0C:EE,RobertBo Robert Bosch Elektronikai Kft.
 44:0C:FD,"NetMan NetMan Co., Ltd."
 44:10:FE,"HuizhouF Huizhou Foryou General Electronics Co., Ltd."
 44:11:02,EDMIEuro EDMI Europe Ltd
@@ -24356,23 +24628,25 @@
 44:16:22,Microsof Microsoft Corporation
 44:16:FA,"SamsungE Samsung Electronics Co.,Ltd"
 44:17:93,Espressi Espressif Inc.
 44:18:47,"HunanScr Hunan Scrown Electronic Information Tech.Co.,Ltd"
 44:18:4F,Fitview
 44:18:FD,"Apple Apple, Inc."
 44:19:B6,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
+44:1A:4C,"xFusionD xFusion Digital Technologies Co.,Ltd."
 44:1A:AC,Elektrik Elektrik Uretim AS EOS
 44:1A:FA,"NewH3CTe New H3C Technologies Co., Ltd"
 44:1B:88,"Apple Apple, Inc."
-44:1C:12,Technico Technicolor CH USA Inc.
+44:1C:12,VantivaU Vantiva USA LLC
 44:1C:7F,"Motorola Motorola Mobility LLC, a Lenovo Company"
 44:1C:A8,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 44:1E:91,"ARVIDAIn ARVIDA Intelligent Electronics Technology Co.,Ltd."
 44:1E:98,RuckusWi Ruckus Wireless
 44:1E:A1,HewlettP Hewlett Packard
+44:20:63,Continen Continental Automotive Technologies GmbH
 44:22:7C,"HuaweiTe Huawei Technologies Co.,Ltd"
 44:22:95,ChinaMob China Mobile Iot Limited company
 44:22:F1,"SFac S.Fac, Inc"
 44:23:7C,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 44:23:AA,"Farmage Farmage Co., Ltd."
 44:25:BB,BambooEn Bamboo Entertainment Corporation
 44:27:2E,"HuaweiDe Huawei Device Co., Ltd."
@@ -24384,15 +24658,15 @@
 44:2A:FF,"E3Techno E3 Technology, Inc."
 44:2B:03,"Cisco Cisco Systems, Inc"
 44:2C:05,"AMPAKTec AMPAK Technology, Inc."
 44:31:92,HewlettP Hewlett Packard
 44:32:2A,Avaya Avaya Inc
 44:32:62,zte zte corporation
 44:32:C2,"GOAL GOAL Co., Ltd."
-44:32:C8,Technico Technicolor CH USA Inc.
+44:32:C8,VantivaU Vantiva USA LLC
 44:33:4C,"Shenzhen Shenzhen Bilian electronic CO.,LTD"
 44:34:8F,MxtIndus Mxt Industrial Ltda
 44:34:A7,"ARRISGro ARRIS Group, Inc."
 44:35:6F,Neterix Neterix Ltd
 44:35:83,"Apple Apple, Inc."
 44:37:08,MRVComun MRV Comunications
 44:37:19,2SaveEne 2 Save Energy Ltd
@@ -24437,28 +24711,30 @@
 44:54:C0,Thompson Thompson Aerospace
 44:55:B1,"HuaweiTe Huawei Technologies Co.,Ltd"
 44:55:C4,"HuaweiDe Huawei Device Co., Ltd."
 44:56:8D,"PNCTechn PNC Technologies Co., Ltd."
 44:56:B7,"SpawnLab Spawn Labs, Inc"
 44:56:E2,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 44:58:29,CiscoSPV Cisco SPVTG
+44:59:25,Square Square Inc.
 44:59:43,zte zte corporation
 44:59:9F,"Criticar Criticare Systems, Inc"
 44:59:E3,"HuaweiTe Huawei Technologies Co.,Ltd"
 44:5A:DF,"Mikami Mikami & Co., Ltd."
 44:5B:ED,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 44:5C:E9,"SamsungE Samsung Electronics Co.,Ltd"
 44:5D:5E,"SHENZHEN SHENZHEN Coolkit Technology CO.,LTD"
 44:5E:CD,Razer Razer Inc
 44:5E:F3,Tonalite Tonalite Holding B.V.
 44:5F:7A,ShihlinE Shihlin Electric & Engineering Corp.
 44:5F:8C,Intercel Intercel Group Limited
 44:61:32,ecobee ecobee inc
 44:61:9C,FONsyste FONsystem co. ltd.
 44:62:46,Comat Comat AG
+44:63:70,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 44:64:3C,"Cisco Cisco Systems, Inc"
 44:65:0D,AmazonTe Amazon Technologies Inc.
 44:65:6A,"MegaVide Mega Video Electronic(HK) Industry Co., Ltd"
 44:65:7F,Calix Calix Inc.
 44:66:6E,Ip-Line
 44:66:FC,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 44:67:47,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -24536,14 +24812,15 @@
 44:9B:78,NowFacto The Now Factory
 44:9B:C1,"HuaweiTe Huawei Technologies Co.,Ltd"
 44:9C:B5,"Alcomp Alcomp, Inc"
 44:9E:F9,"vivoMobi vivo Mobile Communication Co., Ltd."
 44:9F:46,"HuaweiDe Huawei Device Co., Ltd."
 44:9F:7F,DataCore DataCore Software Corporation
 44:A1:91,"HuaweiTe Huawei Technologies Co.,Ltd"
+44:A3:C7,zte zte corporation
 44:A4:2D,TCTmobil TCT mobile ltd
 44:A4:66,GroupeLd Groupe Ldlc
 44:A5:4E,QorvoInt Qorvo International Pte. Ltd.
 44:A5:6E,Netgear
 44:A6:1E,IngramMi Ingram Micro Services
 44:A6:42,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 44:A6:89,PromaxEl Promax Electronica Sa
@@ -24582,14 +24859,15 @@
 44:B2:95,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 44:B3:2D,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 44:B3:82,Kuang-ch Kuang-chi Institute of Advanced Technology
 44:B4:12,Sius Sius Ag
 44:B4:33,"tide tide.co.,ltd"
 44:B4:62,Flextron Flextronics Tech.(Ind) Pvt Ltd
 44:B4:B2,AmazonTe Amazon Technologies Inc.
+44:B5:9C,TenetNet Tenet Networks Private Limited
 44:B6:BE,"Cisco Cisco Systems, Inc"
 44:B7:D0,Microchi Microchip Technology Inc.
 44:B9:94,DouglasL Douglas Lighting Controls
 44:BA:46,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 44:BB:3B,"Google Google, Inc."
 44:BD:DE,BHTC BHTC GmbH
 44:BF:E3,"Shenzhen Shenzhen Longtech Electronics Co.,Ltd"
@@ -24618,14 +24896,15 @@
 44:D3:CA,"Cisco Cisco Systems, Inc"
 44:D4:37,IntenoBr Inteno Broadband Technology AB
 44:D4:53,Sagemcom Sagemcom Broadband SAS
 44:D4:54,Sagemcom Sagemcom Broadband SAS
 44:D4:E0,Sony Sony Corporation
 44:D5:06,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 44:D5:A5,AddOnCom AddOn Computer
+44:D5:C1,EMMicroe EM Microelectronic
 44:D5:CC,AmazonTe Amazon Technologies Inc.
 44:D5:F2,IEEERegi IEEE Registration Authority
 44:D5:F2:00:00:00/28,TIBARese TIBA Research & Development (1986) LTD
 44:D5:F2:10:00:00/28,Simplere Simplered Technology Ltd.
 44:D5:F2:20:00:00/28,"Shenzhen Shenzhen Hebang Electronic Co., Ltd"
 44:D5:F2:30:00:00/28,Vuro Vuro Llc
 44:D5:F2:40:00:00/28,"Appotron Appotronics Co., Ltd"
@@ -24637,63 +24916,69 @@
 44:D5:F2:A0:00:00/28,SYSTECel SYS TEC electronic GmbH
 44:D5:F2:B0:00:00/28,"ValeoInt Valeo Interior Controls (Shenzhen) Co.,Ltd"
 44:D5:F2:C0:00:00/28,neocontr neocontrol soluções em automação
 44:D5:F2:D0:00:00/28,"Shenzhen Shenzhen Nation RFID Technology Co.,Ltd."
 44:D5:F2:E0:00:00/28,"Joint-St Joint-Stock Company Research and Development Center ""ELVEES"""
 44:D6:3D,TalariNe Talari Networks
 44:D6:E1,SnuzaInt Snuza International Pty. Ltd.
+44:D7:7E,RobertBo Robert Bosch GmbH
 44:D7:91,"HuaweiTe Huawei Technologies Co.,Ltd"
 44:D8:32,AzureWav AzureWave Technology Inc.
 44:D8:78,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 44:D8:84,"Apple Apple, Inc."
-44:D9:E7,Ubiquiti Ubiquiti Networks Inc.
+44:D9:E7,Ubiquiti Ubiquiti Inc
 44:DA:30,"Apple Apple, Inc."
 44:DB:60,"NanjingB Nanjing Baihezhengliu Technology Co., Ltd"
+44:DB:D2,"YealinkX Yealink(Xiamen) Network Technology Co.,Ltd."
 44:DC:4E,ItelMobi Itel Mobile Limited
 44:DC:91,PlanexCo Planex Communications Inc.
 44:DC:CB,Semindia Semindia Systems Pvt Ltd
+44:DF:65,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 44:E0:8E,CiscoSPV Cisco SPVTG
 44:E1:37,"ARRISGro ARRIS Group, Inc."
 44:E2:F1,"NewRadio NewRadio Technologies Co. , Ltd."
 44:E4:9A,Omnitron Omnitronics Pty Ltd
 44:E4:D9,"Cisco Cisco Systems, Inc"
 44:E4:EE,WistronN Wistron Neweb Corporation
 44:E5:17,IntelCor Intel Corporate
 44:E6:6E,"Apple Apple, Inc."
 44:E6:B0,ChinaMob China Mobile IOT Company Limited
+44:E7:61,Infinixm Infinix mobility limited
 44:E8:A5,MyrekaTe Myreka Technologies Sdn. Bhd.
 44:E9:68,"HuaweiTe Huawei Technologies Co.,Ltd"
 44:E9:DD,Sagemcom Sagemcom Broadband SAS
 44:EA:30,"SamsungE Samsung Electronics Co.,Ltd"
 44:EA:4B,Actlas Actlas Inc.
 44:EA:D8,TexasIns Texas Instruments
 44:EB:2E,"Alpsalpi Alpsalpine Co,.Ltd"
 44:EC:CE,JuniperN Juniper Networks
 44:ED:57,"Longicor Longicorn, inc."
 44:EE:02,MTI MTI Ltd.
+44:EE:14,TexasIns Texas Instruments
 44:EE:30,Budelman Budelmann Elektronik GmbH
 44:EF:BF,ChinaDra China Dragon Technology Limited
 44:EF:CF,UGENESOL UGENE SOLUTION inc.
-44:F0:34,"Kaonmedi Kaonmedia CO., LTD."
+44:F0:34,"KaonGrou Kaon Group Co., Ltd."
 44:F0:9E,"Apple Apple, Inc."
 44:F2:1B,"Apple Apple, Inc."
 44:F4:36,zte zte corporation
 44:F4:59,"SamsungE Samsung Electronics Co.,Ltd"
 44:F4:77,JuniperN Juniper Networks
 44:F4:E7,Cohesity Cohesity Inc
 44:F8:49,UnionPac Union Pacific Railroad
 44:F9:71,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
+44:FA:66,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 44:FB:42,"Apple Apple, Inc."
 44:FB:5A,zte zte corporation
 44:FD:A3,Everysig Everysight LTD.
 44:FE:3B,Arcadyan Arcadyan Corporation
 44:FF:BA,zte zte corporation
 47:54:43,GtcNotRe GTC (Not registered!)
 48:00:31,"HuaweiTe Huawei Technologies Co.,Ltd"
-48:00:33,Technico Technicolor CH USA Inc.
+48:00:33,VantivaU Vantiva USA LLC
 48:00:7D,DtsElekt Dts Elektronik San. Tic. Ltd. Sti.
 48:01:C5,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 48:02:2A,B-LinkEl B-Link Electronic Limited
 48:02:86,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 48:02:AF,TelitCom Telit Communication s.p.a
 48:03:62,"DesayEle Desay Electronics(Huizhou)Co.,Ltd"
 48:04:9F,"Elecom Elecom Co., Ltd"
@@ -24727,72 +25012,81 @@
 48:13:F3,"BbkEduca Bbk Educational Electronics Corp.,Ltd."
 48:16:93,Lear Lear Corporation GmbH
 48:17:4C,MicroPow MicroPower technologies
 48:18:42,Shanghai Shanghai Winaas Co. Equipment Co. Ltd.
 48:18:8D,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 48:18:FA,Nocsys
 48:1A:84,PointerT Pointer Telocation Ltd
-48:1B:40,Technico Technicolor CH USA Inc.
+48:1B:40,VantivaU Vantiva USA LLC
+48:1B:A4,"Cisco Cisco Systems, Inc"
 48:1B:D2,"IntronSc Intron Scientific co., ltd."
 48:1C:B9,"SzDjiTec Sz Dji Technology Co.,Ltd"
 48:1D:70,CiscoSPV Cisco SPVTG
 48:1F:2D,"Shenzhen Shenzhen Jie Shi Lian Industrial Co.,LTD"
 48:1F:66,"ChinaMob China Mobile Group Device Co.,Ltd."
 48:21:0B,Pegatron Pegatron Corporation
 48:21:6C,ChinaMob China Mobile IOT Company Limited
 48:22:18,"Shenzhen Shenzhen Yipingfang Network Technology Co., Ltd."
 48:22:54,TP-Link TP-Link Corporation Limited
 48:23:35,DialogSe Dialog Semiconductor Hellas SA
 48:25:67,Poly
+48:25:F3,"HuaweiDe Huawei Device Co., Ltd."
 48:26:2C,"Apple Apple, Inc."
 48:26:E8,"Tek-Air Tek-Air Systems, Inc."
 48:27:59,LevvenEl Levven Electronics Ltd.
 48:27:C5,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:27:E2,Espressi Espressif Inc.
 48:27:EA,"SamsungE Samsung Electronics Co.,Ltd"
 48:28:2F,zte zte corporation
 48:29:52,Sagemcom Sagemcom Broadband SAS
-48:29:E4,"AONPKRoT AO ""NPK RoTeK"""
+48:29:D6,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+48:29:E4,Ao
 48:2A:E3,"WistronI Wistron InfoComm(Kunshan)Co.,Ltd."
 48:2C:A0,XiaomiCo Xiaomi Communications Co Ltd
 48:2C:D0,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:2C:EA,Motorola Motorola Inc Business Light Radios
 48:2E:72,"Cisco Cisco Systems, Inc"
 48:2F:6B,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 48:2F:D7,"HuaweiTe Huawei Technologies Co.,Ltd"
+48:31:33,RobertBo Robert Bosch Elektronika Kft.
+48:31:77,"Nintendo Nintendo Co.,Ltd"
+48:31:B7,Espressi Espressif Inc.
+48:31:DB,"HuaweiDe Huawei Device Co., Ltd."
 48:33:DD,"ZennioAv Zennio Avance Y Tecnologia, S.L."
 48:34:3D,IEP IEP GmbH
 48:35:2B,"Apple Apple, Inc."
 48:35:2E,"Shenzhen Shenzhen Wolck Network Product Co.,LTD"
 48:36:5F,Wintecro Wintecronics Ltd.
 48:38:71,"HuaweiDe Huawei Device Co., Ltd."
+48:38:B6,"AuhuiTao Auhui Taoyun Technology Co., Ltd"
 48:39:74,"ProwareT Proware Technologies Co., Ltd."
 48:3B:38,"Apple Apple, Inc."
 48:3C:0C,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:3D:32,SyscorCo Syscor Controls & Automation
 48:3E:5E,SernetSu Sernet (Suzhou) Technologies Corporation
 48:3F:DA,Espressi Espressif Inc.
 48:3F:E9,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:43:5A,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:43:7C,"Apple Apple, Inc."
 48:43:DD,AmazonTe Amazon Technologies Inc.
 48:44:53,Hds???  HDS ???
 48:44:87,CiscoSPV Cisco SPVTG
 48:44:F7,"SamsungE Samsung Electronics Co.,Ltd"
 48:45:20,IntelCor Intel Corporate
+48:45:CF,"Proizvod LLC Proizvodstvennaya Kompania ""TransService"""
 48:46:8D,Zepcam Zepcam B.V.
 48:46:C1,Fn-LinkT Fn-Link Technology Limited
 48:46:F1,Uros Uros Oy
 48:46:FB,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:47:4B,"HuaweiDe Huawei Device Co., Ltd."
 48:49:C7,"SamsungE Samsung Electronics Co.,Ltd"
 48:4A:30,GeorgeRo George Robotics Limited
 48:4A:E9,HewlettP Hewlett Packard Enterprise
 48:4B:AA,"Apple Apple, Inc."
-48:4B:D4,Technico Technicolor CH USA Inc.
+48:4B:D4,VantivaU Vantiva USA LLC
 48:4C:00,NetworkS Network Solutions
 48:4C:29,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:4C:86,"HuaweiDe Huawei Device Co., Ltd."
 48:4D:7E,Dell Dell Inc.
 48:4E:FC,"ARRISGro ARRIS Group, Inc."
 48:50:73,Microsof Microsoft Corporation
 48:51:69,"SamsungE Samsung Electronics Co.,Ltd"
@@ -24800,32 +25094,35 @@
 48:51:C5,IntelCor Intel Corporate
 48:51:CF,Intelbra Intelbras
 48:51:D0,"JiangsuX Jiangsu Xinsheng Intelligent Technology Co., Ltd."
 48:52:61,Soreel
 48:54:15,NetRules Net Rules Tecnologia Eireli
 48:54:E8,Winbond?
 48:55:19,Espressi Espressif Inc.
+48:55:41,Iskratel Iskratel d.o.o.
 48:55:5C,"WuQiTech Wu Qi Technologies,Inc."
 48:55:5E,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 48:55:5F,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 48:57:02,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:57:D2,Broadcom Broadcom Limited
 48:57:DD,Facebook Facebook Inc
 48:59:29,LGElectr LG Electronics (Mobile Communications)
 48:59:A4,zte zte corporation
+48:5A:0D,JuniperN Juniper Networks
 48:5A:3F,Wisol
 48:5A:67,"ShaanxiR Shaanxi Ruixun Electronic Information Technology Co., Ltd"
 48:5A:B6,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 48:5A:EA,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 48:5B:39,ASUSTekC ASUSTek COMPUTER INC.
 48:5D:35,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 48:5D:36,Verizon
 48:5D:60,AzureWav AzureWave Technology Inc.
 48:5D:EB,JustAddP Just Add Power
 48:5D:ED,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
+48:5F:08,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 48:5F:99,CloudNet Cloud Network Technology (Samoa) Limited
 48:60:5F,LGElectr LG Electronics (Mobile Communications)
 48:60:BC,"Apple Apple, Inc."
 48:61:A3,"ConcernA Concern ""Axion"" JSC"
 48:61:EE,"SamsungE Samsung Electronics Co.,Ltd"
 48:62:76,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:65:EE,IEEERegi IEEE Registration Authority
@@ -24848,14 +25145,15 @@
 48:68:4A,IntelCor Intel Corporate
 48:6B:2C,"BbkEduca Bbk Educational Electronics Corp.,Ltd."
 48:6B:91,Fleetwoo Fleetwood Group Inc.
 48:6D:BB,VestelEl Vestel Elektronik San ve Tic. A.S.
 48:6E:70,"Zhejiang Zhejiang Tmall Technology Co., Ltd."
 48:6E:73,"Pica8 Pica8, Inc."
 48:6E:FB,"DavitSys Davit System Technology Co., Ltd."
+48:6F:33,"Kyungwoo Kyungwoo.System, Inc."
 48:6F:D2,StorSimp StorSimple Inc
 48:70:1E,TexasIns Texas Instruments
 48:70:6F,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:71:19,SgbGroup Sgb Group Ltd.
 48:73:10,JuniperN Juniper Networks
 48:73:97,"NewH3CTe New H3C Technologies Co., Ltd"
 48:73:CB,Tiinlab Tiinlab Corporation
@@ -24872,14 +25170,16 @@
 48:7A:DA,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 48:7A:F6,NcsElect Ncs Electrical Sdn Bhd
 48:7A:FF,Essys
 48:7B:5E,SmtTelec Smt Telecomm Hk
 48:7B:6B,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:7D:2E,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 48:7E:48,EardaTec Earda Technologies co Ltd
+48:81:4E,"E&MSOLUT E&M SOLUTION CO,.Ltd"
+48:81:D4,"RuijieNe Ruijie Networks Co.,LTD"
 48:82:44,LifeFitn Life Fitness / Div. of Brunswick
 48:82:F2,AppelEle Appel Elektronik GmbH
 48:83:B4,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 48:83:C7,Sagemcom Sagemcom Broadband SAS
 48:86:E8,Microsof Microsoft Corporation
 48:87:2D,"ShenZhen Shen Zhen Da Xia Long Que Technology Co.,Ltd"
 48:87:59,XiaomiCo Xiaomi Communications Co Ltd
@@ -24896,25 +25196,29 @@
 48:8D:36,Arcadyan Arcadyan Corporation
 48:8E:42,DIGALOG DIGALOG GmbH
 48:8E:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:8F:4C,"shenzhen shenzhen trolink Technology Co.,Ltd"
 48:8F:5A,Routerbo Routerboard.com
 48:90:2F,LGElectr LG Electronics (Mobile Communications)
 48:91:53,Weinmann Weinmann Geräte für Medizin GmbH + Co. KG
+48:91:D5,"Cisco Cisco Systems, Inc"
 48:91:F6,"Shenzhen Shenzhen Reach software technology CO.,LTD"
+48:93:DC,UniwayIn Uniway Infocom Pvt Ltd
 48:95:07,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 48:98:CA,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 48:9A:42,Technoma Technomate Ltd
 48:9B:D5,"ExtremeN Extreme Networks, Inc."
 48:9B:E0,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 48:9B:E2,SCIInnov SCI Innovations Ltd
 48:9D:18,Flashbay Flashbay Limited
 48:9D:24,BlackBer BlackBerry RTS
 48:9D:D1,"SamsungE Samsung Electronics Co.,Ltd"
+48:9E:9D,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 48:9E:BD,HP HP Inc.
+48:9E:CB,HewlettP Hewlett Packard Enterprise
 48:A0:F8,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 48:A1:95,"Apple Apple, Inc."
 48:A2:2D,"Shenzhen Shenzhen Huaxuchang Telecom Technology Co.,Ltd"
 48:A2:B7,Kodofon Kodofon JSC
 48:A2:B8,"ChengduV Chengdu Vision-Zenith Tech.Co,.Ltd"
 48:A2:E6,Resideo
 48:A3:80,"GioneeCo Gionee Communication Equipment Co.,Ltd."
@@ -24923,14 +25227,15 @@
 48:A5:16,"HuaweiDe Huawei Device Co., Ltd."
 48:A5:E7,"Nintendo Nintendo Co.,Ltd"
 48:A6:B8,"Sonos Sonos, Inc."
 48:A6:D2,"GJsunOpt GJsun Optical Science and Tech Co.,Ltd."
 48:A7:3C,"Sichuant Sichuan tianyi kanghe communications co., LTD"
 48:A7:4E,zte zte corporation
 48:A9:1C,"Apple Apple, Inc."
+48:A9:8A,Routerbo Routerboard.com
 48:A9:D2,WistronN Wistron Neweb Corporation
 48:AA:5D,StoreEle Store Electronic Systems
 48:AD:08,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:AD:9A,IntelCor Intel Corporate
 48:B0:2D,NVIDIA NVIDIA Corporation
 48:B2:53,Marketax Marketaxess Corporation
 48:B2:5D,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -24940,33 +25245,36 @@
 48:B6:20,ROLI ROLI Ltd.
 48:B8:A3,"Apple Apple, Inc."
 48:B8:DE,"Homewins Homewins Technology Co.,Ltd."
 48:B9:77,PulseOn PulseOn Oy
 48:B9:C2,Teletics Teletics Inc.
 48:BA:4E,HewlettP Hewlett Packard
 48:BC:A6,"​ASUNGTE ​ASUNG TECHNO CO.,Ltd"
+48:BC:E1,"SamsungE Samsung Electronics Co.,Ltd"
 48:BD:0E,QuantaSt Quanta Storage Inc.
 48:BD:3D,"NewH3CTe New H3C Technologies Co., Ltd"
 48:BD:4A,"HuaweiTe Huawei Technologies Co.,Ltd"
-48:BD:CE,Technico Technicolor CH USA Inc.
+48:BD:A7,"HonorDev Honor Device Co., Ltd."
+48:BD:CE,VantivaU Vantiva USA LLC
 48:BE:2D,Symanitr Symanitron
 48:BF:6B,"Apple Apple, Inc."
 48:BF:74,"Baicells Baicells Technologies Co.,LTD"
 48:C0:49,BroadTel Broad Telecom SA
 48:C0:93,"Xirrus Xirrus, Inc."
 48:C1:AC,"Plantron Plantronics, Inc."
 48:C1:EE,"HonorDev Honor Device Co., Ltd."
 48:C3:5A,"LenovoBe Lenovo(Beijing)Co., Ltd."
 48:C3:B0,Pharos Pharos Co.Ltd
+48:C4:61,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 48:C5:8D,Lear Lear Corporation GmbH
 48:C6:63,GTOAcces GTO Access Systems LLC
 48:C7:96,"SamsungE Samsung Electronics Co.,Ltd"
 48:C8:62,"SimoWire Simo Wireless,Inc."
 48:C8:B6,SysTec SysTec GmbH
-48:CA:C6,"Unionman Unionman Technology Co.,Ltd"
+48:CA:C6,"UnionMan Union Man Technology Co.,Ltd"
 48:CB:6E,CelloEle Cello Electronics (UK) Ltd
 48:CD:D3,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:D0:CF,"Universa Universal Electronics, Inc."
 48:D1:8E,"MetisCom Metis Communication Co.,Ltd"
 48:D2:24,LiteonTe Liteon Technology Corporation
 48:D2:4F,Sagemcom Sagemcom Broadband SAS
 48:D3:43,"ARRISGro ARRIS Group, Inc."
@@ -24986,14 +25294,15 @@
 48:DC:2D,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:DC:9D,"Grandpri Grandprint(Beijing) Technology Co., LTD."
 48:DC:FB,Nokia Nokia Corporation
 48:DD:0C,eero eero inc.
 48:DD:9D,ItelMobi Itel Mobile Limited
 48:DF:1C,WuhanNEC Wuhan NEC Fibre Optic Communications industry Co. Ltd
 48:DF:37,HewlettP Hewlett Packard Enterprise
+48:E1:5C,"Apple Apple, Inc."
 48:E1:AF,Vity
 48:E1:E9,"ChengduM Chengdu Meross Technology Co., Ltd."
 48:E2:44,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 48:E3:C3,JENOPTIK JENOPTIK Advanced Systems GmbH
 48:E6:95,Insigma Insigma Inc
 48:E6:C0,"SIMComWi SIMCom Wireless Solutions Co.,Ltd."
 48:E7:29,Espressi Espressif Inc.
@@ -25011,15 +25320,15 @@
 48:F0:27,"Chengdun Chengdu newifi Co.,Ltd"
 48:F0:7B,"Alpsalpi Alpsalpine Co,.Ltd"
 48:F1:7F,IntelCor Intel Corporate
 48:F2:30,"Ubizcore Ubizcore Co.,LTD"
 48:F3:17,Private
 48:F3:F3,"BaiduOnl Baidu Online Network Technology (Beijing) Co., Ltd"
 48:F4:7D,TechVisi TechVision Holding Internation Limited
-48:F7:C0,Technico Technicolor CH USA Inc.
+48:F7:C0,VantivaU Vantiva USA LLC
 48:F7:F1,Nokia
 48:F8:B3,"Cisco-Li Cisco-Linksys, LLC"
 48:F8:DB,"HuaweiTe Huawei Technologies Co.,Ltd"
 48:F8:E1,Nokia
 48:F8:FF,"ChengduK Chengdu Kt Electronic Hi-Tech Co.,Ltd"
 48:F9:25,Maestron Maestronic
 48:F9:7C,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
@@ -25030,14 +25339,15 @@
 48:FE:EA,Homa Homa B.V.
 4A:07:D6,IEEE8021 IEEE 802.1 Chair
 4A:15:40,sasdelaH sas de la Halle aux Fours
 4A:19:1B,ZigBeeAl ZigBee Alliance
 4A:5A:6F,AppliedM Applied Materials
 4A:5A:A9,GoCodeIT GoCodeIT Inc
 4A:67:04,Reliable Reliable Robotics Corporation
+4A:68:8D,"Shenzhen Shenzhen TCL New Technology Co., Ltd"
 4A:72:06,"CAIRE CAIRE, Inc."
 4A:7F:74,INTEC INTEC Inc.
 4A:AD:CE,CodanArg Codan Argus Ag
 4A:C0:3F,"WuhanHik Wuhan Hikstorage Technology Co.,Ltd"
 4A:CA:3E,Zeus
 4A:DA:10,EmotivaA Emotiva Audio Corp
 4A:E0:3F,ChengduS Chengdu Superxon communication Technology Co. Ltd.
@@ -25062,14 +25372,15 @@
 4C:0F:6E,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 4C:0F:C7,EardaTec Earda Technologies co Ltd
 4C:11:54,"Mobiwire Mobiwire Mobiles (NingBo) Co., LTD"
 4C:11:59,VisionIn Vision Information & Communications
 4C:11:AE,Espressi Espressif Inc.
 4C:11:BF,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 4C:12:65,"ARRISGro ARRIS Group, Inc."
+4C:12:E8,VietnamP Vietnam Post And Telecommunication Industry Technology Join Stock Company
 4C:13:65,EmplusTe Emplus Technologies
 4C:14:80,"Noregon Noregon Systems, Inc"
 4C:14:A3,"TCLTechn TCL Technoly Electronics (Huizhou) Co., Ltd."
 4C:16:94,"shenzhen shenzhen sibituo Technology Co., Ltd"
 4C:16:F1,zte zte corporation
 4C:16:FC,JuniperN Juniper Networks
 4C:17:44,AmazonTe Amazon Technologies Inc.
@@ -25085,14 +25396,15 @@
 4C:20:B8,"Apple Apple, Inc."
 4C:21:13,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 4C:21:8C,Panasoni Panasonic India Private limited
 4C:21:D0,Sony Sony Corporation
 4C:22:19,Yuanfuda Yuanfudao Hk Limted
 4C:22:58,"cozybit cozybit, Inc."
 4C:22:F3,Arcadyan Arcadyan Corporation
+4C:23:1A,"ExtremeN Extreme Networks, Inc."
 4C:24:98,TexasIns Texas Instruments
 4C:24:CE,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 4C:25:78,Nokia Nokia Corporation
 4C:26:E7,"Welgate Welgate Co., Ltd."
 4C:2C:80,"BeijingS Beijing Skyway Technologies Co.,Ltd"
 4C:2C:83,"Zhejiang Zhejiang KaNong Network Technology Co.,Ltd."
 4C:2E:5E,"SamsungE Samsung Electronics Co.,Ltd"
@@ -25122,14 +25434,15 @@
 4C:40:88,"SanshinE Sanshin Electronics Co.,Ltd."
 4C:42:1E,"Cisco Cisco Systems, Inc"
 4C:42:4C,Informat Information Modes software modified addresses (not registered?)
 4C:44:5B,IntelCor Intel Corporate
 4C:45:76,"ChinaMob China Mobile(Hangzhou) Information Technology Co.,Ltd."
 4C:48:DA,"BeijingA Beijing Autelan Technology Co.,Ltd"
 4C:49:4F,zte zte corporation
+4C:49:6C,IntelCor Intel Corporate
 4C:49:E3,XiaomiCo Xiaomi Communications Co Ltd
 4C:4B:68,"MobileDe Mobile Device, Inc."
 4C:4B:F9,IEEERegi IEEE Registration Authority
 4C:4B:F9:00:00:00/28,Multitek Multitek Elektronik Sanayi ve Ticaret A.S.
 4C:4B:F9:10:00:00/28,"Jiangsua Jiangsu acrel Co., Ltd."
 4C:4B:F9:20:00:00/28,"Shenzhen Shenzhen HommPro Technology Co.,Ltd"
 4C:4B:F9:30:00:00/28,"PowerAct Power Active Co., Ltd"
@@ -25163,20 +25476,22 @@
 4C:56:DF,TargusUS Targus US LLC
 4C:57:CA,"Apple Apple, Inc."
 4C:5B:B3,SiliconL Silicon Laboratories
 4C:5C:DF,ItelMobi Itel Mobile Limited
 4C:5D:3C,"Cisco Cisco Systems, Inc"
 4C:5D:CD,FinnishE Oy Finnish Electric Vehicle Technologies Ltd
 4C:5E:0C,Routerbo Routerboard.com
+4C:5E:D3,UnisyueT Unisyue Technologies Co; LTD.
 4C:5F:D2,Alcatel- Alcatel-Lucent
 4C:60:D5,airPoint airPointe of New Hampshire
 4C:60:DE,Netgear
 4C:61:7E,"HuaweiDe Huawei Device Co., Ltd."
 4C:62:55,Sanmina- Sanmina-Sci System De Mexico S.A. De C.V.
 4C:62:7B,SmartCow SmartCow AI Technologies Taiwan Ltd.
+4C:62:CD,Nokia
 4C:63:71,XiaomiCo Xiaomi Communications Co Ltd
 4C:63:AD,"HuaweiDe Huawei Device Co., Ltd."
 4C:63:EB,Applicat Application Solutions (Electronics and Vision) Ltd
 4C:64:D9,"Guangdon Guangdong Leawin Group Co., Ltd"
 4C:65:A8,IEEERegi IEEE Registration Authority
 4C:65:A8:00:00:00/28,WELT WELT Corporation
 4C:65:A8:10:00:00/28,BeijingB Beijing Bluehalo Internet Inc.
@@ -25190,20 +25505,22 @@
 4C:65:A8:90:00:00/28,"Shenzhen Shenzhen Lisaier Tronics Co.,Ltd"
 4C:65:A8:A0:00:00/28,"SuzhouEm Suzhou Embedded Electronic Technology Co., Ltd."
 4C:65:A8:B0:00:00/28,ZMINTech ZMIN Technologies
 4C:65:A8:C0:00:00/28,Fuse
 4C:65:A8:D0:00:00/28,"Qingping Qingping Technology (Beijing) Co., Ltd."
 4C:65:A8:E0:00:00/28,HighInfi High Infinity Germany
 4C:66:41,SamsungE Samsung Electro-Mechanics(Thailand)
+4C:66:A6,"SamsungE Samsung Electronics Co.,Ltd"
 4C:6A:F6,HMDGloba HMD Global Oy
 4C:6B:E8,"Apple Apple, Inc."
 4C:6C:13,IoTSoluc IoT Company Solucoes Tecnologicas Ltda
 4C:6D:58,JuniperN Juniper Networks
 4C:6E:6E,"ComnectT Comnect Technology CO.,LTD"
 4C:6F:9C,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+4C:70:CC,Blyott Blyott NV
 4C:71:0C,"Cisco Cisco Systems, Inc"
 4C:71:0D,"Cisco Cisco Systems, Inc"
 4C:71:67,PoLabsdo PoLabs d.o.o.
 4C:72:74,Shenzhen Shenzhenshi Xinzhongxin Technology Co.Ltd
 4C:72:B9,Pegatron Pegatron Corporation
 4C:73:4F,JuniperN Juniper Networks
 4C:73:67,GeniusBy Genius Bytes Software Solutions GmbH
@@ -25221,14 +25538,15 @@
 4C:74:A7:70:00:00/28,CoreipTe Coreip Technology Private Limited
 4C:74:A7:80:00:00/28,Annapurn Annapurna labs
 4C:74:A7:90:00:00/28,SuzhouXi Suzhou XiongLi Technology Inc.
 4C:74:A7:A0:00:00/28,Raonark
 4C:74:A7:B0:00:00/28,traplink traplinked Gmbh
 4C:74:A7:C0:00:00/28,N3com
 4C:74:A7:D0:00:00/28,ddcpersi ddcpersia
+4C:74:A7:E0:00:00/28,Kyocera Kyocera Corporation
 4C:74:BF,"Apple Apple, Inc."
 4C:75:25,Espressi Espressif Inc.
 4C:76:25,Dell Dell Inc.
 4C:77:13,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 4C:77:4F,Embedded Embedded Wireless Labs
 4C:77:66,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 4C:77:6D,"Cisco Cisco Systems, Inc"
@@ -25246,14 +25564,15 @@
 4C:80:93,IntelCor Intel Corporate
 4C:80:BA,"WuhanTia Wuhan Tianyu Information Industry Co., Ltd."
 4C:81:20,TaicangT Taicang T&W Electronics
 4C:82:A9,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 4C:82:CF,DishTech Dish Technologies Corp
 4C:83:DE,CiscoSPV Cisco SPVTG
 4C:87:5D,Bose Bose Corporation
+4C:88:9E,"HuaweiDe Huawei Device Co., Ltd."
 4C:8B:30,"Actionte Actiontec Electronics, Inc"
 4C:8B:55,GrupoDig Grupo Digicon
 4C:8B:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
 4C:8D:53,"HuaweiTe Huawei Technologies Co.,Ltd"
 4C:8D:79,"Apple Apple, Inc."
 4C:8E:CC,Silkan Silkan Sa
 4C:8F:A5,Jastec
@@ -25292,14 +25611,16 @@
 4C:93:A6:C0:00:00/28,"WuhanMai Wuhan Maiwe communication Co.,Ltd"
 4C:93:A6:D0:00:00/28,Cantroni Cantronic Systems (Canada) Inc
 4C:93:A6:E0:00:00/28,Celltron
 4C:96:14,JuniperN Juniper Networks
 4C:96:2D,Fresh Fresh AB
 4C:96:8A,"Wacom Wacom Co.,Ltd."
 4C:98:EF,Zeo
+4C:99:92,"vivoMobi vivo Mobile Communication Co., Ltd."
+4C:9B:63,LGInnote LG Innotek
 4C:9D:22,"ACES ACES Co.,Ltd"
 4C:9E:6C,BroadexT Broadex Technologies Co.Ltd
 4C:9E:80,"KYOKKOEL KYOKKO ELECTRIC Co., Ltd."
 4C:9E:E4,"HanyangN Hanyang Navicom Co.,Ltd."
 4C:9E:FF,ZyxelCom Zyxel Communications Corporation
 4C:A0:03,Vitec
 4C:A1:61,RainBird Rain Bird Corporation
@@ -25368,32 +25689,36 @@
 4C:BD:8F,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 4C:C0:0A,"vivoMobi vivo Mobile Communication Co., Ltd."
 4C:C2:06,Somfy
 4C:C4:49,Icotera Icotera A/S
 4C:C4:52,ShangHai Shang Hai Tyd. Electon Technology Ltd.
 4C:C5:3E,ZyxelCom Zyxel Communications Corporation
 4C:C6:02,"Radios Radios, Inc."
+4C:C6:4C,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 4C:C6:81,"Shenzhen Shenzhen Aisat Electronic Co., Ltd."
 4C:C7:D6,"Flextron Flextronics Manufacturing(Zhuhai)Co.,Ltd."
+4C:C8:44,"MaipuCom Maipu Communication Technology Co.,Ltd."
 4C:C8:A1,CiscoMer Cisco Meraki
 4C:C9:4F,Nokia
 4C:C9:5E,"SamsungE Samsung Electronics Co.,Ltd"
 4C:CA:53,"Skyera Skyera, Inc."
 4C:CB:F5,zte zte corporation
 4C:CC:34,Motorola Motorola Solutions Inc.
 4C:CC:6A,"Micro-St Micro-Star INTL CO., LTD."
 4C:CE:2D,Danlaw Danlaw Inc
 4C:D0:8A,"HUMAX HUMAX Co., Ltd."
 4C:D0:CB,"HuaweiTe Huawei Technologies Co.,Ltd"
 4C:D0:DD,"HuaweiTe Huawei Technologies Co.,Ltd"
 4C:D1:A1,"HuaweiTe Huawei Technologies Co.,Ltd"
+4C:D2:FB,"Unionman Unionman Technology Co.,Ltd"
 4C:D3:AF,HMDGloba HMD Global Oy
 4C:D5:77,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 4C:D6:29,"HuaweiTe Huawei Technologies Co.,Ltd"
 4C:D6:37,"QsonoEle Qsono Electronics Co., Ltd"
+4C:D7:17,Dell Dell Inc.
 4C:D7:B6,HelmerSc Helmer Scientific
 4C:D9:8F,Dell Dell Inc.
 4C:D9:C4,MagnetiM Magneti Marelli Automotive Electronics (Guangzhou) Co. Ltd
 4C:DC:0D,CoralTel Coral Telecom Limited
 4C:DD:31,"SamsungE Samsung Electronics Co.,Ltd"
 4C:DD:7D,LHPTelem LHP Telematics LLC
 4C:DF:3D,TeamEngi Team Engineers Advance Technologies India Pvt Ltd
@@ -25418,20 +25743,22 @@
 4C:E1:76,"Cisco Cisco Systems, Inc"
 4C:E1:9E,TecnoMob Tecno Mobile Limited
 4C:E1:BB,"ZhuhaiHi Zhuhai HiFocus Technology Co., Ltd."
 4C:E2:F1,Udino Udino srl
 4C:E5:AE,"TianjinB Tianjin Beebox Intelligent Technology Co.,Ltd."
 4C:E6:76,Buffalo Buffalo.Inc
 4C:E6:C0,"Apple Apple, Inc."
+4C:E7:05,"SiemensI Siemens Industrial Automation Products Ltd., Chengdu"
 4C:E9:33,"RailComm RailComm, LLC"
 4C:E9:E4,"NewH3CTe New H3C Technologies Co., Ltd"
 4C:EA:AE,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 4C:EB:42,IntelCor Intel Corporate
 4C:EB:BD,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 4C:EB:D6,Espressi Espressif Inc.
+4C:EC:0F,"Cisco Cisco Systems, Inc"
 4C:EC:EF,"Soraa Soraa, Inc."
 4C:ED:DE,AskeyCom Askey Computer Corp
 4C:ED:FB,ASUSTekC ASUSTek COMPUTER INC.
 4C:EE:B0,SHCNetzw SHC Netzwerktechnik GmbH
 4C:EF:56,Shenzhen Shenzhen Sundray Technologies Company Limited
 4C:EF:C0,AmazonTe Amazon Technologies Inc.
 4C:F0:2E,VifaDenm Vifa Denmark A/S
@@ -25453,21 +25780,22 @@
 4C:FE:2E,"DongGuan DongGuan Siyoto Electronics Co., Ltd"
 4C:FF:12,"FuzeEnte Fuze Entertainment Co., ltd"
 50:00:84,SiemensC Siemens Canada
 50:00:8C,HongKong Hong Kong Telecommunications (HKT) Limited
 50:01:6B,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:01:BB,"SamsungE Samsung Electronics Co.,Ltd"
 50:01:D9,"HuaweiTe Huawei Technologies Co.,Ltd"
+50:02:38,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 50:02:91,Espressi Espressif Inc.
 50:04:B8,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:05:3D,CyWeeGro CyWee Group Ltd
 50:06:04,"Cisco Cisco Systems, Inc"
 50:06:AB,"Cisco Cisco Systems, Inc"
 50:07:C3,AmazonTe Amazon Technologies Inc.
-50:09:59,Technico Technicolor CH USA Inc.
+50:09:59,VantivaU Vantiva USA LLC
 50:09:E5,"Drimsys Drimsys,Inc"
 50:0A:52,HuiwanTe Huiwan Technologies Co. Ltd
 50:0B:26,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:0B:32,"FoxdaTec Foxda Technology Industrial(ShenZhen)Co.,LTD"
 50:0B:91,IEEERegi IEEE Registration Authority
 50:0B:91:00:00:00/28,"Igor Igor, Inc."
 50:0B:91:10:00:00/28,SPDDevel SPD Development Company Ltd
@@ -25490,14 +25818,15 @@
 50:0F:F5,"TendaTec Tenda Technology Co.,Ltd.Dongguan branch"
 50:11:EB,SilverNe SilverNet Ltd
 50:13:95,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 50:14:08,AiNET
 50:14:79,iRobot iRobot Corporation
 50:14:B5,"RichfitI Richfit Information Technology Co., Ltd"
 50:14:C1,"HuaweiTe Huawei Technologies Co.,Ltd"
+50:16:F4,"Motorola Motorola Mobility LLC, a Lenovo Company"
 50:17:FF,"Cisco Cisco Systems, Inc"
 50:18:4C,Platina Platina Systems Inc.
 50:1A:A5,GNNetcom GN Netcom A/S
 50:1A:C5,Microsof Microsoft
 50:1B:32,TaicangT Taicang T&W Electronics
 50:1C:B0,"Cisco Cisco Systems, Inc"
 50:1C:BF,"Cisco Cisco Systems, Inc"
@@ -25529,14 +25858,15 @@
 50:2D:BB,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 50:2D:F4,PhytecMe Phytec Messtechnik GmbH
 50:2D:FB,"IGShare IGShare Co., Ltd."
 50:2E:5C,HTC HTC Corporation
 50:2E:CE,"AsahiEle Asahi Electronics Co.,Ltd"
 50:2F:9B,IntelCor Intel Corporate
 50:2F:A8,"Cisco Cisco Systems, Inc"
+50:30:F4,"Exascend Exascend, Inc."
 50:31:AD,ABBGloba ABB Global Industries and Services Private Limited
 50:32:37,"Apple Apple, Inc."
 50:32:5F,SiliconL Silicon Laboratories
 50:32:75,"SamsungE Samsung Electronics Co.,Ltd"
 50:33:8B,TexasIns Texas Instruments
 50:33:F0,YichenSh Yichen (Shenzhen) Technology Co.Ltd
 50:38:2F,ASEGroup ASE Group Chung-Li
@@ -25553,24 +25883,42 @@
 50:3D:EB,"Zhejiang Zhejiang Tmall Technology Co., Ltd."
 50:3E:7C,LeiShenI LeiShen Intelligent System Co.Ltd
 50:3E:AA,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 50:3F:50,"HuaweiDe Huawei Device Co., Ltd."
 50:3F:56,Syncmold Syncmold Enterprise Corp
 50:3F:98,Cmitech
 50:40:61,Nokia
+50:40:74,Alarmcom Alarm.com
 50:41:1C,"AMPAKTec AMPAK Technology,Inc."
 50:41:72,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:41:B9,"I-ODataD I-O Data Device,Inc."
 50:42:89,zte zte corporation
 50:43:48,ThingsMa ThingsMatrix Inc.
 50:43:B9,OktoInfo OktoInform RUS
+50:45:94,Radisys
 50:45:F7,LiuheInt Liuhe Intelligence Technology Ltd.
 50:46:4A,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:46:5D,ASUSTekC ASUSTek COMPUTER INC.
 50:46:AE,Mercury Mercury Corporation
+50:48:2C,IEEERegi IEEE Registration Authority
+50:48:2C:00:00:00/28,Landatel Landatel Comunicaciones SL
+50:48:2C:10:00:00/28,Annapurn Annapurna labs
+50:48:2C:20:00:00/28,BBPOS BBPOS Limited
+50:48:2C:30:00:00/28,Immunity Immunity Networks and Technologies Pvt Ltd
+50:48:2C:40:00:00/28,Hy-LineC Hy-Line Computer Components GmbH
+50:48:2C:50:00:00/28,BluefinI Bluefin International Inc
+50:48:2C:60:00:00/28,WIKAMobi WIKA Mobile Conrol GmbH&Co.KG
+50:48:2C:70:00:00/28,"OliverIQ Oliver IQ, Inc."
+50:48:2C:80:00:00/28,"Dongguan Dongguan Amdolla Electric & Light Material Manufacture Co., Ltd"
+50:48:2C:90:00:00/28,SoterTec Soter Technologies
+50:48:2C:A0:00:00/28,JungHo Jung Ho
+50:48:2C:B0:00:00/28,SLProces SL Process
+50:48:2C:C0:00:00/28,"TelecamT Telecam Technology Co.,Ltd"
+50:48:2C:D0:00:00/28,"KidoSpor Kido Sports Co., Ltd."
+50:48:2C:E0:00:00/28,"HarbinNo Harbin Nosean Tese And Control Technology Co.,Ltd"
 50:48:77,"HonorDev Honor Device Co., Ltd."
 50:48:EB,BeijingH Beijing Haihejinsheng Network Technology Co. Ltd.
 50:49:21,"Cisco Cisco Systems, Inc"
 50:49:B0,"SamsungE Samsung Electronics Co.,Ltd"
 50:4A:5E,Masimo Masimo Corporation
 50:4A:6E,Netgear
 50:4B:5B,CONTROLt CONTROLtronic GmbH
@@ -25628,14 +25976,15 @@
 50:62:55:E0:00:00/28,"Shinsoft Shinsoft Co., Ltd."
 50:63:13,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 50:63:91,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:64:2B,"XIAOMIEl XIAOMI Electronics,CO.,LTD"
 50:64:41,Greenlee
 50:65:83,TexasIns Texas Instruments
 50:65:F3,HewlettP Hewlett Packard
+50:66:E5,"HuaweiDe Huawei Device Co., Ltd."
 50:67:87,PlanetNe Planet Networks
 50:67:AE,"Cisco Cisco Systems, Inc"
 50:67:F0,ZyxelCom Zyxel Communications Corporation
 50:68:0A,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:68:AC,"HuaweiDe Huawei Device Co., Ltd."
 50:6A:03,Netgear
 50:6B:4B,"Mellanox Mellanox Technologies, Inc."
@@ -25675,20 +26024,22 @@
 50:87:B8,Nuvyyo Nuvyyo Inc
 50:89:65,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 50:89:D1,"HuaweiDe Huawei Device Co., Ltd."
 50:8A:06,TuyaSmar Tuya Smart Inc.
 50:8A:0F,"Shenzhen Shenzhen Fise Technology Holding Co.,Ltd."
 50:8A:42,"UptmateT Uptmate Technology Co., LTD"
 50:8A:CB,"Shenzhen Shenzhen Maxmade Technology Co., Ltd."
+50:8B:B9,TuyaSmar Tuya Smart Inc.
 50:8C:77,DIRMEIER DIRMEIER Schanktechnik GmbH &Co KG
 50:8C:B1,TexasIns Texas Instruments
 50:8C:F5,"ChinaMob China Mobile Group Device Co.,Ltd."
 50:8D:6F,CHAHOO CHAHOO Limited
 50:8E:49,XiaomiCo Xiaomi Communications Co Ltd
 50:8F:4C,XiaomiCo Xiaomi Communications Co Ltd
+50:91:E3,TP-Link TP-Link Corporation Limited
 50:92:B9,"SamsungE Samsung Electronics Co.,Ltd"
 50:93:4F,GradualT Gradual Tecnologia Ltda.
 50:95:51,"ARRISGro ARRIS Group, Inc."
 50:97:07,"XiamenPa Xiamen Paperang Technology Co.,Ltd."
 50:97:44,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 50:97:72,Westingh Westinghouse Digital
 50:98:39,XiaomiCo Xiaomi Communications Co Ltd
@@ -25699,14 +26050,15 @@
 50:9A:4C,Dell Dell Inc.
 50:9A:88,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:9E:A7,"SamsungE Samsung Electronics Co.,Ltd"
 50:9F:27,"HuaweiTe Huawei Technologies Co.,Ltd"
 50:9F:3B,"OiElectr Oi Electric Co.,Ltd"
 50:A0:09,XiaomiCo Xiaomi Communications Co Ltd
 50:A0:15,"Shenzhen Shenzhen Yipingfang Network Technology Co., Ltd."
+50:A0:30,IEEERegi IEEE Registration Authority
 50:A0:30:00:00:00/28,GopodGro Gopod Group Limited
 50:A0:30:10:00:00/28,XEPIC XEPIC Corporation Limited
 50:A0:30:20:00:00/28,Annapurn Annapurna labs
 50:A0:30:30:00:00/28,RealWear RealWear (Shanghai) Intelligent Technology Co. Ltd
 50:A0:30:40:00:00/28,AlertInn Alert Innovation
 50:A0:30:50:00:00/28,"JiangsuJ Jiangsu Jinshi Legend Technology Co.,Ltd"
 50:A0:30:60:00:00/28,AbacusRe Abacus Research AG
@@ -25785,28 +26137,30 @@
 50:CD:32,"NanJingC NanJing Chaoran Science & Technology Co.,Ltd."
 50:CE:75,"MeasyEle Measy Electronics Co., Ltd."
 50:CE:E3,Gigafirm Gigafirm.co.LTD
 50:D0:65,ESYLUX ESYLUX GmbH
 50:D2:13,CviLux CviLux Corporation
 50:D2:74,Steffes Steffes Corporation
 50:D2:F5,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
+50:D3:3B,cloudnin cloudnineinfo
 50:D3:7F,"YuFlyMik Yu Fly Mikly Way Science and Technology Co., Ltd."
 50:D4:5C,AmazonTe Amazon Technologies Inc.
 50:D4:F7,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 50:D5:9C,"ThaiHabe Thai Habel Industrial Co., Ltd."
 50:D6:D7,Takahata Takahata Precision
 50:D7:53,CONELCOM CONELCOM GmbH
 50:DA:00,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 50:DA:D6,XiaomiCo Xiaomi Communications Co Ltd
 50:DB:3F,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 50:DC:D0,"Observin Observint Technologies, Inc."
 50:DC:E7,AmazonTe Amazon Technologies Inc.
 50:DC:FC,Ecocom
 50:DD:4F,"Automati Automation Components, Inc"
 50:DE:06,"Apple Apple, Inc."
+50:DE:19,IEEERegi IEEE Registration Authority
 50:DE:19:00:00:00/28,Telic Telic AG
 50:DE:19:10:00:00/28,ClearFlo Clear Flow by Antiference
 50:DE:19:20:00:00/28,Spii Spii Spa
 50:DE:19:30:00:00/28,Traxens
 50:DE:19:40:00:00/28,"LangogoT Langogo Technology Co., Ltd."
 50:DE:19:50:00:00/28,Bliq Bliq B.V.
 50:DE:19:60:00:00/28,Oceancct Oceancctv Ltd
@@ -25821,14 +26175,16 @@
 50:DF:95,Lytx
 50:E0:39,ZyxelCom Zyxel Communications Corporation
 50:E0:85,IntelCor Intel Corporate
 50:E0:C7,TurContr TurControlSystme AG
 50:E0:EF,Nokia
 50:E1:4A,Private
 50:E2:4E,zte zte corporation
+50:E4:E0,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
+50:E5:38,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 50:E5:49,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 50:E6:36,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 50:E6:66,"Shenzhen Shenzhen Techtion Electronics Co., Ltd."
 50:E7:A0,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 50:E7:B7,"vivoMobi vivo Mobile Communication Co., Ltd."
 50:E9:71,"Jibo Jibo, Inc."
 50:E9:DF,"QuectelW Quectel Wireless Solutions Co.,Ltd."
@@ -25878,40 +26234,61 @@
 50:FF:99:C0:00:00/28,Goetting Goetting KG
 50:FF:99:D0:00:00/28,"Shenzhen Shenzhen Haipengxin Electronic Co., Ltd."
 50:FF:99:E0:00:00/28,Informa Informa LLC
 52:54:00,RealtekU Realtek (UpTech? also reported)
 52:54:4C,Novell20 Novell 2000
 52:54:AB,RealtekA REALTEK (a Realtek 8029 based PCI Card)
 54:02:37,Teltroni Teltronic AG
+54:02:95,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:03:84,"Hongkong Hongkong Nano IC Technologies Co., Ltd"
 54:03:F5,EBNTechn EBN Technology Corp.
 54:04:96,Gigawave Gigawave LTD
 54:04:A6,ASUSTekC ASUSTek COMPUTER INC.
 54:05:36,Vivago Vivago Oy
 54:05:5F,AlcatelL Alcatel Lucent
 54:05:93,"WOORIELE WOORI ELEC Co.,Ltd"
 54:05:DB,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 54:06:8B,NingboDe Ningbo Deli Kebei Technology Co.LTD
 54:07:64,"HuaweiDe Huawei Device Co., Ltd."
 54:07:7D,Netgear
+54:08:3B,IEEERegi IEEE Registration Authority
+54:08:3B:00:00:00/28,Shenzhen Shenzhen Liandian Communication Technology Co.LTD
+54:08:3B:10:00:00/28,Annapurn Annapurna labs
+54:08:3B:20:00:00/28,NavitusL Navitus Lt
+54:08:3B:30:00:00/28,"DhyanNet Dhyan Networks and Technologies, Inc"
+54:08:3B:40:00:00/28,TorayMed Toray Medical Company Limited
+54:08:3B:50:00:00/28,"shenzhen shenzhen HAIOT technology co.,ltd"
+54:08:3B:60:00:00/28,VectorAt Vector Atomic
+54:08:3B:70:00:00/28,ASCSSp ASCS Sp. z o.o.
+54:08:3B:80:00:00/28,Update Update Systems Inc.
+54:08:3B:90:00:00/28,"Unicompu Unicompute Technology Co.,Ltd."
+54:08:3B:A0:00:00/28,SilexIpa Silex Ipari Automatizálási Zrt.
+54:08:3B:B0:00:00/28,KoreaBus Korea Bus Broadcasting
+54:08:3B:C0:00:00/28,FairPhon FairPhone B.V.
+54:08:3B:D0:00:00/28,BHSCorru BHS Corrugated Maschinen- und Anlagenbau GmbH
+54:08:3B:E0:00:00/28,Sinclair Sinclair Technologies
 54:09:10,"Apple Apple, Inc."
 54:09:55,zte zte corporation
 54:09:8D,deistere deister electronic GmbH
 54:0D:F9,"HuaweiDe Huawei Device Co., Ltd."
 54:0E:2D,"vivoMobi vivo Mobile Communication Co., Ltd."
 54:0E:58,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 54:0F:57,SiliconL Silicon Laboratories
 54:10:2E,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:10:31,Smarto
 54:10:EC,Microchi Microchip Technology Inc.
 54:11:2F,SulzerPu Sulzer Pump Solutions Finland Oy
+54:11:49,"vivoMobi vivo Mobile Communication Co., Ltd."
+54:11:59,NettrixI Nettrix Information Industry co.LTD
 54:11:5F,Atamo Atamo Pty Ltd
+54:12:CB,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:13:10,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:13:79,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 54:14:73,Wingtech Wingtech Group (HongKong）Limited
+54:14:A7,"NanjingQ Nanjing Qinheng Microelectronics Co., Ltd."
 54:14:F3,IntelCor Intel Corporate
 54:14:FD,Orbbec3D Orbbec 3D Technology International
 54:15:89,MCSLogic MCS Logic Inc.
 54:16:51,"RuijieNe Ruijie Networks Co.,LTD"
 54:19:C8,"vivoMobi vivo Mobile Communication Co., Ltd."
 54:1B:5D,Techno-I Techno-Innov
 54:1D:61,"YEESTORM YEESTOR Microelectronics Co., Ltd"
@@ -25938,14 +26315,16 @@
 54:2B:DE,"NewH3CTe New H3C Technologies Co., Ltd"
 54:2C:EA,Protectr Protectron
 54:2F:04,"Shanghai Shanghai Longcheer Technology Co., Ltd."
 54:2F:89,"EuclidLa Euclid Laboratories, Inc."
 54:2F:8A,Tellesco Tellescom Industria E Comercio Em Telecomunicacao
 54:31:31,RasterVi Raster Vision Ltd
 54:31:D4,TGWMecha TGW Mechanics GmbH
+54:32:04,Espressi Espressif Inc.
+54:32:C7,"Apple Apple, Inc."
 54:33:CB,"Apple Apple, Inc."
 54:34:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:35:30,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 54:35:DF,Symeo Symeo GmbH
 54:36:9B,"1VergeIn 1Verge Internet Technology (Beijing) Co., Ltd."
 54:37:BB,TaicangT Taicang T&W Electronics
 54:39:68,Edgewate Edgewater Networks Inc
@@ -25955,42 +26334,47 @@
 54:3D:37,RuckusWi Ruckus Wireless
 54:3D:92,Wireless Wireless-Tek Technology Limited
 54:3E:64,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 54:40:AD,"SamsungE Samsung Electronics Co.,Ltd"
 54:42:49,Sony Sony Corporation
 54:43:B2,Espressi Espressif Inc.
 54:44:08,Nokia Nokia Corporation
+54:44:3B,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:44:A3,"SamsungE Samsung Electronics Co.,Ltd"
 54:45:38,TexasIns Texas Instruments
 54:46:17,zte zte corporation
 54:46:6B,"Shenzhen Shenzhen CZTIC Electronic Technology Co., Ltd"
 54:47:41,Xcheng Xcheng Holding
 54:47:CC,Sagemcom Sagemcom Broadband SAS
 54:47:D3,TsatAs Tsat As
 54:47:E8,Syrotech Syrotech Networks. Ltd.
 54:48:10,Dell Dell Inc.
 54:48:9C,Cdoubles Cdoubles Electronics Co. Ltd.
 54:48:E6,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 54:49:DF,"PelotonI Peloton Interactive, Inc"
+54:49:FC,"UbeeInte Ubee Interactive Co., Limited"
 54:4A:00,"Cisco Cisco Systems, Inc"
 54:4A:05,wenglors wenglor sensoric gmbh
 54:4A:16,TexasIns Texas Instruments
 54:4B:8C,JuniperN Juniper Networks
+54:4C:8A,Microsof Microsoft Corporation
 54:4E:45,Private
 54:4E:90,"Apple Apple, Inc."
 54:51:1B,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:51:46,AMG AMG Systems Ltd.
 54:51:DE,"Cisco Cisco Systems, Inc"
 54:52:84,"HuaweiDe Huawei Device Co., Ltd."
 54:53:ED,Sony Sony Corporation
 54:54:14,"DigitalR Digital RF Corea, Inc"
 54:54:CF,"Probedig Probedigital Co.,Ltd"
 54:55:D5,"HuaweiDe Huawei Device Co., Ltd."
 54:5A:A6,Espressi Espressif Inc.
+54:5D:D9,Edistec
 54:5E:BD,NLTechno NL Technologies
+54:5F:A7,"Jibaiyou Jibaiyou Technology Co.,Ltd."
 54:5F:A9,Teracom Teracom Limited
 54:60:09,"Google Google, Inc."
 54:61:72,ZodiacAe Zodiac Aerospace Sas
 54:61:EA,Zaplox Zaplox AB
 54:62:E2,"Apple Apple, Inc."
 54:64:D9,Sagemcom Sagemcom Broadband SAS
 54:64:DE,u-blox u-blox AG
@@ -26007,19 +26391,20 @@
 54:6C:0E,TexasIns Texas Instruments
 54:6C:EB,IntelCor Intel Corporate
 54:6D:52,TopviewO Topview Optronics Corp.
 54:6F:71,uAvionix uAvionix Corporation
 54:70:68,VTechCom VTech Communications Limited
 54:71:DD,"HuaweiDe Huawei Device Co., Ltd."
 54:72:4F,"Apple Apple, Inc."
-54:72:5E,"Unionman Unionman Technology Co.,Ltd"
+54:72:5E,"UnionMan Union Man Technology Co.,Ltd"
 54:73:98,ToyoElec Toyo Electronics Corporation
 54:74:E6,WebtechW Webtech Wireless
 54:75:95,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 54:75:D0,"Cisco Cisco Systems, Inc"
+54:76:B2,"Raisecom Raisecom Technology CO., LTD"
 54:77:87,EardaTec Earda Technologies co Ltd
 54:77:8A,HewlettP Hewlett Packard Enterprise
 54:78:1A,"Cisco Cisco Systems, Inc"
 54:78:C9,"AMPAKTec AMPAK Technology,Inc."
 54:79:75,Nokia Nokia Corporation
 54:7A:52,CTEInter CTE International srl
 54:7C:69,"Cisco Cisco Systems, Inc"
@@ -26034,17 +26419,19 @@
 54:81:AD,EagleRes Eagle Research Corporation
 54:83:3A,ZyxelCom Zyxel Communications Corporation
 54:84:7B,DigitalD Digital Devices GmbH
 54:84:DC,zte zte corporation
 54:86:BC,"Cisco Cisco Systems, Inc"
 54:88:0E,SamsungE Samsung Electro-Mechanics(Thailand)
 54:88:DE,"Cisco Cisco Systems, Inc"
+54:88:FE,"Xiaoniun Xiaoniu network technology (Shanghai) Co., Ltd."
 54:89:22,Zelfy Zelfy Inc
 54:89:98,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:8A:BA,"Cisco Cisco Systems, Inc"
+54:8C:81,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 54:8C:A0,LiteonTe Liteon Technology Corporation
 54:8D:5A,IntelCor Intel Corporate
 54:92:09,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:92:BE,"SamsungE Samsung Electronics Co.,Ltd"
 54:93:59,"Shenzhen Shenzhen Twowing Technologies Co.,Ltd."
 54:94:78,Silversh Silvershore Technology Partners
 54:99:63,"Apple Apple, Inc."
@@ -26097,15 +26484,15 @@
 54:A4:93:B0:00:00/28,Advice
 54:A4:93:C0:00:00/28,"BjCotyte Bj Cotytech Technology Co.,Ltd"
 54:A4:93:D0:00:00/28,"AssemTec Assem Technology Co.,Ltd."
 54:A4:93:E0:00:00/28,Nederman Nederman Holding AB
 54:A5:1B,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:A5:4B,NSCCommu NSC Communications Siberia Ltd
 54:A6:19,"Alcatel- Alcatel-Lucent Shanghai Bell Co., Ltd"
-54:A6:5C,Technico Technicolor CH USA Inc.
+54:A6:5C,VantivaU Vantiva USA LLC
 54:A6:DB,"HuaweiDe Huawei Device Co., Ltd."
 54:A7:03,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 54:A9:C8,HomeCont Home Control Singapore Pte Ltd
 54:A9:D4,Minibar Minibar Systems
 54:AB:3A,QuantaCo Quanta Computer Inc.
 54:AC:FC,LIZNApS LIZN ApS
 54:AE:27,"Apple Apple, Inc."
@@ -26113,14 +26500,15 @@
 54:AE:D2,CSLDualc CSL Dualcom Ltd
 54:AF:97,TP-Link TP-Link Corporation Limited
 54:B1:21,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:B2:03,Pegatron Pegatron Corporation
 54:B5:6C,"XianNova Xi'an NovaStar Tech Co., Ltd"
 54:B6:20,SUHDOLE& SUHDOL E&C Co.Ltd.
 54:B7:53,"HunanFen Hunan Fenghui Yinjia Science And Technology Co.,Ltd"
+54:B7:BD,Arcadyan Arcadyan Corporation
 54:B7:E5,"RaysonTe Rayson Technology Co., Ltd."
 54:B8:02,"SamsungE Samsung Electronics Co.,Ltd"
 54:B8:0A,D-LinkIn D-Link International
 54:BA:D6,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:BD:79,"SamsungE Samsung Electronics Co.,Ltd"
 54:BE:53,zte zte corporation
 54:BE:F7,Pegatron Pegatron Corporation
@@ -26178,27 +26566,29 @@
 54:E7:D5,SunCupid Sun Cupid Technology (HK) LTD
 54:EA:A8,"Apple Apple, Inc."
 54:EB:E9,"Apple Apple, Inc."
 54:EC:2F,RuckusWi Ruckus Wireless
 54:ED:A3,"Navdy Navdy, Inc."
 54:EE:75,"WistronI Wistron InfoComm(Kunshan)Co.,Ltd."
 54:EF:33,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
+54:EF:43,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:EF:44,"LumiUnit Lumi United Technology Co., Ltd"
 54:EF:92,"Shenzhen Shenzhen Elink Technology Co., LTD"
 54:EF:FE,"Fullpowe Fullpower Technologies, Inc."
 54:F1:5F,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 54:F2:01,"SamsungE Samsung Electronics Co.,Ltd"
 54:F2:94,"HuaweiDe Huawei Device Co., Ltd."
 54:F5:B6,Oriental Oriental Pacific International Limited
 54:F6:07,"HuaweiDe Huawei Device Co., Ltd."
 54:F6:66,Berthold Berthold Technologies GmbH and Co.KG
 54:F6:C5,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 54:F6:E2,"HuaweiTe Huawei Technologies Co.,Ltd"
 54:F8:2A,u-blox u-blox AG
 54:F8:76,Abb Abb Ag
+54:F8:F0,Tesla Tesla Inc
 54:FA:3E,"SamsungE Samsung Electronics Co.,Ltd"
 54:FA:96,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 54:FB:58,"WISEWARE WISEWARE, Lda"
 54:FC:F0,"SamsungE Samsung Electronics Co.,Ltd"
 54:FD:BF,ScheidtB Scheidt & Bachmann GmbH
 54:FF:82,DavitSol Davit Solution co.
 54:FF:CF,MopriaAl Mopria Alliance
@@ -26212,14 +26602,15 @@
 58:05:28,LabrisNe Labris Networks
 58:05:56,Elettron Elettronica GF S.r.L.
 58:08:FA,FiberOpt Fiber Optic & telecommunication INC.
 58:09:43,Private
 58:09:E5,Kivic Kivic Inc.
 58:0A:20,"Cisco Cisco Systems, Inc"
 58:0A:D4,"Apple Apple, Inc."
+58:10:31,"HonHaiPr Hon Hai Precision IND.CO.,LTD"
 58:10:8C,Intelbra Intelbras
 58:10:B7,Infinixm Infinix mobility limited
 58:11:22,ASUSTekC ASUSTek COMPUTER INC.
 58:12:43,AcSiPTec AcSiP Technology Corp.
 58:13:D3,"GemtekTe Gemtek Technology Co., Ltd."
 58:16:26,Avaya Avaya Inc
 58:16:D7,"Alpsalpi Alpsalpine Co,.Ltd"
@@ -26233,30 +26624,32 @@
 58:1F:67,Open-mte Open-m technology limited
 58:1F:AA,"Apple Apple, Inc."
 58:1F:EF,Tuttnaer Tuttnaer LTD
 58:20:59,XiaomiCo Xiaomi Communications Co Ltd
 58:20:71,"SamsungE Samsung Electronics Co.,Ltd"
 58:20:8A,IEEERegi IEEE Registration Authority
 58:20:8A:00:00:00/28,Annapurn Annapurna labs
+58:20:8A:10:00:00/28,BeijingS Beijing Senfetech Corporation Ltd.
 58:20:8A:20:00:00/28,"MarsDigi Mars Digi Tech Co.,Ltd"
 58:20:8A:30:00:00/28,"Aggregat Aggregate Co.,Ltd."
 58:20:8A:40:00:00/28,Tring
 58:20:8A:50:00:00/28,"JiaHuang Jia Huang Jhan Ye Co.,Ltd"
 58:20:8A:60:00:00/28,"Shangyin Shangyin Intelligence Technology Shandong Co.,Ltd"
 58:20:8A:70:00:00/28,pureLiFi pureLiFi Ltd
 58:20:8A:80:00:00/28,"SAMILCTS SAMIL CTS Co., Ltd."
 58:20:8A:90:00:00/28,SuzhouRu Suzhou Ruilisi Technology Ltd.
 58:20:8A:A0:00:00/28,Conducti Conductix-Wampfler
 58:20:8A:B0:00:00/28,InfodevE Infodev Electronic Designers Intl.
+58:20:8A:C0:00:00/28,JiangsuZ Jiangsu Zhonganzhixin Communication Technology Co.
 58:20:8A:D0:00:00/28,SamboHit Sambo Hitech
 58:20:8A:E0:00:00/28,"UPMTechn UPM Technology, Inc"
 58:20:B1,HewlettP Hewlett Packard
 58:21:36,"KMBsro KMB systems, s.r.o."
 58:21:E9,Twpi
-58:23:8C,Technico Technicolor CH USA Inc.
+58:23:8C,VantivaU Vantiva USA LLC
 58:24:29,"Google Google, Inc."
 58:25:75,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:27:8C,Buffalo Buffalo.Inc
 58:2A:F7,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:2B:0A,TexasIns Texas Instruments
 58:2B:DB,Pax Pax AB
 58:2D:34,"Qingping Qingping Electronics (Suzhou) Co., Ltd"
@@ -26268,31 +26661,35 @@
 58:31:12,Drust
 58:32:77,Reliance Reliance Communications LLC
 58:34:3B,GlovastT Glovast Technology Ltd.
 58:35:26,DeepletT Deeplet Technology Corp
 58:35:5D,"HuaweiDe Huawei Device Co., Ltd."
 58:35:6B,TecnoMob Tecno Mobile Limited
 58:35:D9,"Cisco Cisco Systems, Inc"
+58:36:53,"Apple Apple, Inc."
 58:38:79,"Ricoh Ricoh Company, Ltd."
 58:3B:D9,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 58:3C:C6,Omnealit Omneality Ltd.
 58:3F:54,LGElectr LG Electronics (Mobile Communications)
 58:40:4E,"Apple Apple, Inc."
 58:41:20,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 58:42:E4,BaxterIn Baxter International Inc
+58:43:AB,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 58:44:98,XiaomiCo Xiaomi Communications Co Ltd
 58:45:4C,Ericsson Ericsson AB
 58:46:8F,KoncarEl Koncar Electronics and Informatics
 58:46:E1,BaxterIn Baxter International Inc
 58:47:04,"Shenzhen Shenzhen Webridge Technology Co.,Ltd"
 58:47:CA,IEEERegi IEEE Registration Authority
 58:47:CA:00:00:00/28,LitumBil Litum Bilgi Teknolojileri San. Ve Tic. A.S.
 58:47:CA:10:00:00/28,HexagonM Hexagon Metrology Services Ltd.
 58:47:CA:20:00:00/28,OnawhimO Onawhim (Oaw) Inc.
+58:47:CA:30:00:00/28,"FujianHe Fujian Helios Technologies Co., Ltd."
 58:47:CA:40:00:00/28,FutureTe Future Tech Development FZC LLC
+58:47:CA:50:00:00/28,"HuizhouJ Huizhou Jiemeisi Technology Co., Ltd"
 58:47:CA:60:00:00/28,"Shenzhen Shenzhen C & D Electronics Co., Ltd."
 58:47:CA:70:00:00/28,"Shenzhen Shenzhen Meigao Electronic Equipment Co.,Ltd"
 58:47:CA:80:00:00/28,"BirgerEn Birger Engineering, Inc."
 58:47:CA:90:00:00/28,"KingnuoI Kingnuo Intelligent Technology (Jiaxing) Co., Ltd."
 58:47:CA:A0:00:00/28,"PowderWa Powder Watts, LLC"
 58:47:CA:B0:00:00/28,"SuzhouLa Suzhou Laisai Intelligence Technology Co.,Ltd"
 58:47:CA:C0:00:00/28,"SmsElect Sms Electric Co., Ltd Zhengzhou"
@@ -26326,14 +26723,15 @@
 58:50:AB,TLS TLS Corporation
 58:50:E6,BestBuy Best Buy Corporation
 58:50:ED,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 58:52:8A,Mitsubis Mitsubishi Electric Corporation
 58:53:C0,"BeijingG Beijing Guang Runtong Technology Development Company co.,Ltd"
 58:55:95,"Apple Apple, Inc."
 58:55:CA,"Apple Apple, Inc."
+58:56:9F,"Cisco Cisco Systems, Inc"
 58:56:C2,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:56:E8,"ARRISGro ARRIS Group, Inc."
 58:57:0D,DanfossS Danfoss Solar Inverters
 58:58:CD,"ExtremeN Extreme Networks, Inc."
 58:59:C2,"ExtremeN Extreme Networks, Inc."
 58:5B:69,"Tvt Tvt Co., Ltd"
 58:5F:F6,zte zte corporation
@@ -26344,14 +26742,15 @@
 58:63:9A,TplSyste Tpl Systemes
 58:64:C4,"Apple Apple, Inc."
 58:65:E6,infomark
 58:66:BA,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 58:67:1A,Barnes&N Barnes&Noble
 58:67:7F,ClareCon Clare Controls Inc.
 58:68:5D,TempoAus Tempo Australia Pty Ltd
+58:68:61,"Viasat Viasat, Incorporated"
 58:69:6C,"RuijieNe Ruijie Networks Co.,LTD"
 58:69:F9,FusionTr Fusion Transactive Ltd.
 58:6A:B1,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 58:6B:14,"Apple Apple, Inc."
 58:6C:25,IntelCor Intel Corporate
 58:6D:67,IntelCor Intel Corporate
 58:6D:8F,"Cisco-Li Cisco-Linksys, LLC"
@@ -26359,14 +26758,15 @@
 58:70:7F,Ericsson Ericsson AB
 58:70:C6,"Shanghai Shanghai Xiaoyi Technology Co., Ltd."
 58:73:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:73:D8,"Apple Apple, Inc."
 58:75:21,CJSCRTSo CJSC RTSoft
 58:76:75,"BeijingE Beijing ECHO Technologies Co.,Ltd"
 58:76:AC,SernetSu Sernet (Suzhou) Technologies Corporation
+58:76:B3,"UbeeInte Ubee Interactive Co., Limited"
 58:76:C5,DigiIS Digi I'S Ltd
 58:7A:4D,Stonesof Stonesoft Corporation
 58:7A:62,TexasIns Texas Instruments
 58:7A:6A,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 58:7B:E9,AirProTe AirPro Technology India Pvt. Ltd
 58:7D:B6,Northern Northern Data AG
 58:7E:61,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
@@ -26381,14 +26781,15 @@
 58:85:A2,RealmeCh Realme Chongqing MobileTelecommunications Corp Ltd
 58:85:E9,RealmeCh Realme Chongqing MobileTelecommunications Corp Ltd
 58:86:94,EFMNetwo EFM Networks
 58:87:4C,Lite-OnC Lite-On Clean Energy Technology Corp.
 58:87:9F,"HuaweiDe Huawei Device Co., Ltd."
 58:87:E2,"Shenzhen Shenzhen Coship Electronics Co., Ltd."
 58:8A:5A,Dell Dell Inc.
+58:8B:1C,"Cisco Cisco Systems, Inc"
 58:8B:F3,ZyxelCom Zyxel Communications Corporation
 58:8D:09,"Cisco Cisco Systems, Inc"
 58:8D:64,"XianClev Xi'an Clevbee Technology Co.,Ltd"
 58:8E:81,SiliconL Silicon Laboratories
 58:8F:CF,"Hangzhou Hangzhou Ezviz Software Co.,Ltd."
 58:90:43,Sagemcom Sagemcom Broadband SAS
 58:91:53,ChinaMob China Mobile IOT Company Limited
@@ -26416,34 +26817,36 @@
 58:95:D8:90:00:00/28,Loftie
 58:95:D8:A0:00:00/28,PeakComm Peak Communications Limited
 58:95:D8:B0:00:00/28,"SuZhouRu SuZhou Ruishengwei Intelligent Technology Co.,Ltd"
 58:95:D8:C0:00:00/28,LoctekEr Loctek Ergonomic Technology Corp.
 58:95:D8:D0:00:00/28,Alunos Alunos AG
 58:95:D8:E0:00:00/28,Gmvsiste Gmv sistemas SAU
 58:96:1D,IntelCor Intel Corporate
-58:96:30,Technico Technicolor CH USA Inc.
+58:96:30,VantivaU Vantiva USA LLC
 58:97:1E,"Cisco Cisco Systems, Inc"
 58:97:BD,"Cisco Cisco Systems, Inc"
 58:98:35,Technico Technicolor Delivery Technologies Belgium NV
 58:98:6F,Revoluti Revolution Display
 58:9A:3E,AmazonTe Amazon Technologies Inc.
 58:9B:0B,"Shineway Shineway Technologies, Inc."
 58:9B:4A,DWnetTec DWnet Technologies(Suzhou) Corporation
 58:9B:F7,"HefeiRad Hefei Radio Communication Technology Co., Ltd"
 58:9C:FC,FreeBSDF FreeBSD Foundation
 58:9E:C6,GigasetC Gigaset Communications GmbH
 58:A0:23,IntelCor Intel Corporate
 58:A0:CB,"TrackNet TrackNet, Inc"
+58:A1:5F,TexasIns Texas Instruments
 58:A2:B5,LGElectr LG Electronics (Mobile Communications)
 58:A4:8E,PixArtIm PixArt Imaging Inc.
 58:A6:39,"SamsungE Samsung Electronics Co.,Ltd"
 58:A7:6F,iD iD corporation
 58:A8:39,IntelCor Intel Corporate
 58:A8:7B,"Fitbit Fitbit, Inc."
 58:AC:78,"Cisco Cisco Systems, Inc"
+58:AD:12,"Apple Apple, Inc."
 58:AE:2B,"HuaweiDe Huawei Device Co., Ltd."
 58:AE:A8,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:AE:F1,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 58:B0:35,"Apple Apple, Inc."
 58:B0:3E,"Nintendo Nintendo Co.,Ltd"
 58:B0:D4,ZuniData ZuniData Systems Inc.
 58:B0:FE,TeamEPS Team EPS GmbH
@@ -26465,28 +26868,46 @@
 58:BE:72,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:BF:25,Espressi Espressif Inc.
 58:BF:EA,"Cisco Cisco Systems, Inc"
 58:C1:7A,CambiumN Cambium Networks Limited
 58:C2:32,NEC NEC Corporation
 58:C3:56,EMMicroe EM Microelectronic
 58:C3:8B,"SamsungE Samsung Electronics Co.,Ltd"
+58:C4:1E,IEEERegi IEEE Registration Authority
+58:C4:1E:00:00:00/28,"Guangzho Guangzhou TeleStar Communication Consulting Service Co., Ltd"
+58:C4:1E:10:00:00/28,"JLZTLink JLZTLink Industry ?Shen Zhen?Co., Ltd."
+58:C4:1E:20:00:00/28,Truesens Truesense Srl
+58:C4:1E:30:00:00/28,LemcoIKE Lemco IKE
+58:C4:1E:40:00:00/28,"BeijingF Beijing Fibrlink Communications Co.,Ltd."
+58:C4:1E:50:00:00/28,"Zhejiang Zhejiang Cainiao Supply Chain Management Co.,Ltd"
+58:C4:1E:70:00:00/28,HwaCom HwaCom Systems Inc.
+58:C4:1E:80:00:00/28,"XiaomiEV Xiaomi EV Technology Co., Ltd."
+58:C4:1E:90:00:00/28,"ShenZhen ShenZhen Heng Yue Industry Co.,Ltd"
+58:C4:1E:A0:00:00/28,GeBEElek GeBE Elektronik und Feinwerktechnik GmbH
+58:C4:1E:B0:00:00/28,PulseStr Pulse Structural Monitoring Ltd
+58:C4:1E:C0:00:00/28,"PQTELNet PQTEL Network Technology Co. , Ltd."
+58:C4:1E:D0:00:00/28,MunichEl Munich Electrification GmbH
+58:C4:1E:E0:00:00/28,"BeijingQ Beijing Qiangyun Innovation Technology Co.,Ltd"
 58:C5:7E,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 58:C5:83,ItelMobi Itel Mobile Limited
 58:C5:CB,"SamsungE Samsung Electronics Co.,Ltd"
 58:C6:F0,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 58:C7:AC,"NewH3CTe New H3C Technologies Co., Ltd"
 58:C8:76,"ChinaMob China Mobile (Hangzhou) Information Technology Co., Ltd."
-58:C9:35,"ChiunMai Chiun Mai Communication Systems, Inc"
+58:C9:35,"ChiunMai Chiun Mai Communication System, Inc"
 58:CB:52,"Google Google, Inc."
+58:CD:C9,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 58:CE:2A,IntelCor Intel Corporate
 58:CF:4B,LufkinIn Lufkin Industries
 58:CF:79,Espressi Espressif Inc.
 58:D0:61,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:D0:71,BWBroadc BW Broadcast
 58:D0:8F,IEEE1904 IEEE 1904.1 Working Group
+58:D2:37,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
+58:D3:12,zte zte corporation
 58:D3:49,"Apple Apple, Inc."
 58:D3:91,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 58:D5:0A,"MurataMa Murata Manufacturing Co., Ltd."
 58:D5:6E,D-LinkIn D-Link International
 58:D6:7A,TCPlink
 58:D6:97,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 58:D6:D3,DairyChe Dairy Cheq Inc
@@ -26499,14 +26920,15 @@
 58:E0:2C,MicroTec Micro Technic A/S
 58:E1:6C,"YingHuaI Ying Hua Information Technology (Shanghai)Co., LTD"
 58:E2:8F,"Apple Apple, Inc."
 58:E3:26,CompassT Compass Technologies Inc.
 58:E4:03,WistronN Wistron Neweb Corporation
 58:E4:34,JuniperN Juniper Networks
 58:E4:76,"CentronC Centron Communications Technologies Fujian Co.,Ltd"
+58:E4:88,AmazonTe Amazon Technologies Inc.
 58:E6:36,EVRsafeT EVRsafe Technologies
 58:E6:BA,"Apple Apple, Inc."
 58:E7:47,Deltanet Deltanet AG
 58:E8:08,Autonics Autonics Corporation
 58:E8:73,"HANGZHOU HANGZHOU DANGBEI NETWORK TECH.Co.,Ltd"
 58:E8:76,IEEERegi IEEE Registration Authority
 58:E8:76:00:00:00/28,"ZhuhaiRa Zhuhai Raysharp Technology Co.,Ltd"
@@ -26534,14 +26956,15 @@
 58:F2:FC,"HuaweiDe Huawei Device Co., Ltd."
 58:F3:87,Airios
 58:F3:9C,"Cisco Cisco Systems, Inc"
 58:F4:96,SourceCh Source Chain
 58:F6:7B,XiaMenUn Xia Men UnionCore Technology LTD.
 58:F6:BF,KyotoUni Kyoto University
 58:F8:5C,"Proizvod LLC Proizvodstvennaya Kompania ""TransService"""
+58:F8:D7,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:F9:87,"HuaweiTe Huawei Technologies Co.,Ltd"
 58:F9:8E,SECUDOS SECUDOS GmbH
 58:FB:84,IntelCor Intel Corporate
 58:FB:96,RuckusWi Ruckus Wireless
 58:FC:20,AlticeLa Altice Labs S.A.
 58:FC:73,"ArriaLiv Arria Live Media, Inc."
 58:FC:C6,Tozo Tozo Inc
@@ -26583,41 +27006,45 @@
 5C:0A:5B,"SamsungE Samsung Electro Mechanics Co., Ltd."
 5C:0B:CA,Tunstall Tunstall Nordic AB
 5C:0C:0E,GuizhouH Guizhou Huaxintong Semiconductor Technology Co Ltd
 5C:0C:BB,CELIZION CELIZION Inc.
 5C:0C:E6,"Nintendo Nintendo Co.,Ltd"
 5C:0E:8B,"ExtremeN Extreme Networks, Inc."
 5C:0F:FB,AminoCom Amino Communications Ltd
+5C:10:1E,zte zte corporation
 5C:10:C5,"SamsungE Samsung Electronics Co.,Ltd"
 5C:11:93,SealOne Seal One AG
 5C:14:37,Thyssenk Thyssenkrupp Aufzugswerke GmbH
 5C:15:15,Advan
 5C:15:E1,AidcTech Aidc Technology (S) Pte Ltd
+5C:16:48,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 5C:16:C7,AristaNe Arista Networks
 5C:17:20,"HuaweiDe Huawei Device Co., Ltd."
 5C:17:37,"I-ViewNo I-View Now, LLC."
 5C:17:CF,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 5C:17:D3,Lge
 5C:18:B5,TalonCom Talon Communications
 5C:1A:6F,"Cambridg Cambridge Industries(Group) Co.,Ltd."
 5C:1B:F4,"Apple Apple, Inc."
 5C:1C:B9,"vivoMobi vivo Mobile Communication Co., Ltd."
 5C:1D:D9,"Apple Apple, Inc."
 5C:20:D0,"AsoniCom Asoni Communication Co., Ltd."
 5C:21:67,Rockwell Rockwell Automation
 5C:22:C4,"DaeEunEl Dae Eun Eletronics Co., Ltd"
+5C:22:DA,VantivaU Vantiva USA LLC
 5C:23:16,Squirrel Squirrels Research Labs LLC
 5C:24:43,"O-SungTe O-Sung Telecom Co., Ltd."
 5C:24:79,Baltech Baltech AG
 5C:24:E2,"SuzhouDe Suzhou Denbom Electronic S&T Co., Ltd"
 5C:25:4C,AvireGlo Avire Global Pte Ltd
 5C:26:0A,Dell Dell Inc.
 5C:26:23,WaveLynx WaveLynx Technologies Corporation
 5C:27:63,ItibiaTe Itibia Technologies
 5C:27:D4,Shenzhen Shenzhen Qihu Intelligent Technology Company Limited
+5C:28:86,Inventec Inventec(Chongqing) Corporation
 5C:2A:EF,r2pAsia- r2p Asia-Pacific Pty Ltd
 5C:2B:F5,VivintWi Vivint Wireless Inc.
 5C:2E:59,"SamsungE Samsung Electronics Co.,Ltd"
 5C:2E:D2,"ABCXiShe ABC(XiSheng) Electronics Co.,Ltd"
 5C:2F:AF,HomeWiza HomeWizard B.V.
 5C:31:3E,TexasIns Texas Instruments
 5C:31:92,"Cisco Cisco Systems, Inc"
@@ -26647,14 +27074,15 @@
 5C:47:5E,Ring Ring LLC
 5C:49:79,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 5C:49:7D,"SamsungE Samsung Electronics Co.,Ltd"
 5C:49:FA,"Shenzhen Shenzhen Guowei Shidai Communication Equipement Co., Ltd"
 5C:4A:1F,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 5C:4A:26,EnguityT Enguity Technology Corp
 5C:4C:A9,"HuaweiTe Huawei Technologies Co.,Ltd"
+5C:4D:BF,zte zte corporation
 5C:50:15,"Cisco Cisco Systems, Inc"
 5C:50:D9,"Apple Apple, Inc."
 5C:51:4F,IntelCor Intel Corporate
 5C:51:81,"SamsungE Samsung Electronics Co.,Ltd"
 5C:51:88,"Motorola Motorola Mobility LLC, a Lenovo Company"
 5C:52:1E,"Nintendo Nintendo Co.,Ltd"
 5C:52:30,"Apple Apple, Inc."
@@ -26674,42 +27102,64 @@
 5C:5B:35,"Mist Mist Systems, Inc."
 5C:5B:C2,YIK YIK Corporation
 5C:5E:AB,JuniperN Juniper Networks
 5C:5F:67,IntelCor Intel Corporate
 5C:60:BA,HP HP Inc.
 5C:61:99,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 5C:62:5A,Canon Canon Inc.
+5C:62:8B,TP-Link TP-Link Corporation Limited
 5C:63:BF,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 5C:63:C9,Intellit Intellithings Ltd.
 5C:64:7A,"HuaweiTe Huawei Technologies Co.,Ltd"
 5C:64:8E,ZyxelCom Zyxel Communications Corporation
+5C:64:F1,"Cisco Cisco Systems, Inc"
 5C:64:F3,"sywinkey sywinkey HongKong Co,. Limited?"
 5C:66:6C,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 5C:67:76,IDSImagi IDS Imaging Development Systems GmbH
 5C:68:D0,AuroraIn Aurora Innovation Inc.
 5C:69:84,Nuvico
 5C:6A:7D,Kentkart Kentkart Ege Elektronik San. Ve Tic. Ltd. Sti.
 5C:6A:80,ZyxelCom Zyxel Communications Corporation
+5C:6A:EC,IEEERegi IEEE Registration Authority
+5C:6A:EC:00:00:00/28,AcuityBr Acuity Brands Lighting
+5C:6A:EC:10:00:00/28,"Shanghai Shanghai Smilembb Technology Co.,LTD"
+5C:6A:EC:20:00:00/28,"Shenzhen Shenzhen Mingyue Technology lnnovation Co.,Ltd"
+5C:6A:EC:30:00:00/28,"Shanghai Shanghai Yunsilicon Technology Co., Ltd."
+5C:6A:EC:40:00:00/28,GeneTouc GeneTouch Corp.
+5C:6A:EC:50:00:00/28,Exaterra Exaterra Ltd.
+5C:6A:EC:60:00:00/28,Femtocel Femtocell
+5C:6A:EC:70:00:00/28,"NipponPu Nippon Pulse Motor Co., Ltd."
+5C:6A:EC:80:00:00/28,OptiverS Optiver Services B.V.
+5C:6A:EC:90:00:00/28,"Shanghai Shanghai Alway Information Technology Co., Ltd"
+5C:6A:EC:A0:00:00/28,"Shenzhen Shenzhen Olax Technology CO.,Ltd"
+5C:6A:EC:B0:00:00/28,Shenzhen Shenzhen Anked vision Electronics Co.Ltd
+5C:6A:EC:C0:00:00/28,"SuzhouHu Suzhou Huaqi Intelligent Technology Co., Ltd."
+5C:6A:EC:D0:00:00/28,DarkVisi DarkVision Technologies Inc.
+5C:6A:EC:E0:00:00/28,SaabSeae Saab Seaeye Ltd
 5C:6B:32,TexasIns Texas Instruments
 5C:6B:4F,Hello Hello Inc.
 5C:6B:D7,FoshanVI Foshan VIOMI Electric Appliance Technology Co. Ltd.
 5C:6D:20,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 5C:6F:4F,Sistel S.A. Sistel
 5C:6F:69,Broadcom Broadcom Limited
 5C:70:17,"Apple Apple, Inc."
+5C:70:75,"HuaweiTe Huawei Technologies Co.,Ltd"
 5C:70:A3,LGElectr LG Electronics (Mobile Communications)
 5C:71:0D,"Cisco Cisco Systems, Inc"
+5C:75:45,"Wayties Wayties, Inc."
 5C:75:AF,"Fitbit Fitbit, Inc."
 5C:75:C6,"ChinaMob China Mobile Group Device Co.,Ltd."
-5C:76:95,Technico Technicolor CH USA Inc.
+5C:76:95,VantivaU Vantiva USA LLC
+5C:76:D5,Nokia
 5C:77:57,Haivisio Haivision Network Video
 5C:77:76,TCTmobil TCT mobile ltd
 5C:78:F8,"HuaweiDe Huawei Device Co., Ltd."
+5C:7B:5C,"Shenzhen Shenzhen SDMC Technology CO.,Ltd."
 5C:7D:5E,"HuaweiTe Huawei Technologies Co.,Ltd"
-5C:7D:7D,Technico Technicolor CH USA Inc.
+5C:7D:7D,VantivaU Vantiva USA LLC
 5C:80:B6,IntelCor Intel Corporate
 5C:81:A7,NetworkD Network Devices Pty Ltd
 5C:83:82,Nokia
 5C:83:8F,"Cisco Cisco Systems, Inc"
 5C:83:CD,Newplatf New platforms
 5C:84:3C,SonyInte Sony Interactive Entertainment Inc.
 5C:84:86,Brightso Brightsource Industries Israel LTD
@@ -26737,25 +27187,27 @@
 5C:87:30,"Apple Apple, Inc."
 5C:87:78,"Cybertel Cybertelbridge co.,ltd"
 5C:87:9C,IntelCor Intel Corporate
 5C:88:16,Rockwell Rockwell Automation
 5C:89:9A,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 5C:89:D4,"BeijingB Beijing Banner Electric Co.,Ltd"
 5C:8A:38,HewlettP Hewlett Packard
+5C:8B:6B,AmazonTe Amazon Technologies Inc.
 5C:8C:30,TaicangT Taicang T&W Electronics
 5C:8D:2D,"Shanghai Shanghai Wellpay Information Technology Co., Ltd"
 5C:8D:4E,"Apple Apple, Inc."
 5C:8E:8B,"Shenzhen Shenzhen Linghai Electronics Co.,Ltd"
 5C:8F:40,TecnoMob Tecno Mobile Limited
 5C:8F:E0,"ARRISGro ARRIS Group, Inc."
 5C:90:12,"OwlCyber Owl Cyber Defense Solutions, LLC"
 5C:91:57,"HuaweiTe Huawei Technologies Co.,Ltd"
 5C:91:FD,Jaewoncn Jaewoncnc
 5C:92:5E,ZioncomE Zioncom Electronics (Shenzhen) Ltd.
 5C:93:A2,LiteonTe Liteon Technology Corporation
+5C:94:62,"Shenzhen Shenzhen Jiuzhou Electric Co.,LTD"
 5C:95:AE,"Apple Apple, Inc."
 5C:96:56,AzureWav AzureWave Technology Inc.
 5C:96:66,SonyInte Sony Interactive Entertainment Inc.
 5C:96:6A,Rtnet
 5C:96:9D,"Apple Apple, Inc."
 5C:97:F3,"Apple Apple, Inc."
 5C:99:60,"SamsungE Samsung Electronics Co.,Ltd"
@@ -26853,21 +27305,24 @@
 5C:E2:86,NortelNe Nortel Networks
 5C:E2:8C,ZyxelCom Zyxel Communications Corporation
 5C:E2:F4,AcSiPTec AcSiP Technology Corp.
 5C:E3:0E,"ARRISGro ARRIS Group, Inc."
 5C:E3:B6,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 5C:E4:2A,IntelCor Intel Corporate
 5C:E5:0C,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
+5C:E6:88,VECOSEur VECOS Europe B.V.
 5C:E7:47,"HuaweiTe Huawei Technologies Co.,Ltd"
 5C:E7:A0,Nokia
 5C:E7:BF,"NewSingu New Singularity International Technical Development Co.,Ltd"
 5C:E8:83,"HuaweiTe Huawei Technologies Co.,Ltd"
 5C:E8:B7,OraimoTe Oraimo Technology Limited
+5C:E8:D3,"Signalin Signalinks Communication Technology Co., Ltd"
 5C:E8:EB,"SamsungE Samsung Electronics Co.,Ltd"
 5C:E9:1E,"Apple Apple, Inc."
+5C:E9:31,TP-Link TP-Link Corporation Limited
 5C:EA:1D,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 5C:EB:4E,RSTAHLHM R. STAHL HMI Systems GmbH
 5C:EB:68,"Cheersta Cheerstar Technology Co., Ltd"
 5C:ED:8C,HewlettP Hewlett Packard Enterprise
 5C:ED:F4,"SamsungE Samsung Electronics Co.,Ltd"
 5C:EE:79,GlobalDi Global Digitech Co LTD
 5C:F2:07,SpecoTec Speco Technologies
@@ -26913,14 +27368,15 @@
 5C:FF:35,Wistron Wistron Corporation
 5C:FF:FF,"Shenzhen Shenzhen Kezhonglong Optoelectronic Technology Co., Ltd"
 60:01:94,Espressi Espressif Inc.
 60:01:B1,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:02:92,Pegatron Pegatron Corporation
 60:02:B4,WistronN Wistron Neweb Corporation
 60:03:08,"Apple Apple, Inc."
+60:03:0C,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 60:03:47,BillionE Billion Electric Co. Ltd.
 60:03:A6,IntenoBr Inteno Broadband Technology AB
 60:04:17,"Posbank Posbank Co.,Ltd"
 60:05:8A,"HitachiM Hitachi Metals, Ltd."
 60:06:E3,"Apple Apple, Inc."
 60:07:7C,JalaGrou Jala Group
 60:07:C4,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -26934,22 +27390,24 @@
 60:11:99,Siama Siama Systems Inc
 60:12:3C,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:12:83,TsbRealT Tsb Real Time Location Systems S.L.
 60:12:8B,Canon Canon Inc.
 60:14:66,zte zte corporation
 60:14:B3,CyberTAN CyberTAN Technology Inc.
 60:15:21,RedarcEl Redarc Electronics
+60:15:2B,PaloAlto Palo Alto Networks
 60:15:92,IEEERegi IEEE Registration Authority
 60:15:92:00:00:00/28,SLabssp S Labs sp. z o.o.
 60:15:92:10:00:00/28,RTDSTech RTDS Technologies Inc.
 60:15:92:20:00:00/28,"EDATechn EDA Technology Co.,LTD"
 60:15:92:30:00:00/28,"OsiTechn Osi Technology Co.,Ltd."
 60:15:92:40:00:00/28,Zaptec
+60:15:92:50:00:00/28,ComfitHe Comfit HealthCare Devices Limited
 60:15:92:60:00:00/28,"BeijingK Beijing Kuangshi Technology Co., Ltd"
-60:15:92:70:00:00/28,FasterCZ Faster CZ spol. s r.o.
+60:15:92:70:00:00/28,UnipiTec Unipi Technology s.r.o.
 60:15:92:80:00:00/28,"Yangzhou Yangzhou Wanfang Electronic Technology,CO.,Ltd."
 60:15:92:90:00:00/28,"JiangsuS Jiangsu Sunfy Technologies Holding Co.,Ltd."
 60:15:92:A0:00:00/28,insensiv insensiv GmbH
 60:15:92:B0:00:00/28,Annapurn Annapurna labs
 60:15:92:C0:00:00/28,"PSS PSS Co., Ltd"
 60:15:92:D0:00:00/28,"Remowire Remowireless Communication International Co.,Limited"
 60:15:92:E0:00:00/28,Annapurn Annapurna labs
@@ -26959,32 +27417,35 @@
 60:18:3A,"HuaweiDe Huawei Device Co., Ltd."
 60:18:88,zte zte corporation
 60:18:95,Dell Dell Inc.
 60:19:0C,Rramac
 60:19:29,Voltroni Voltronic Power Technology(Shenzhen) Corp.
 60:19:70,"HuizhouQ Huizhou Qiaoxing Electronics Technology Co., Ltd."
 60:19:71,"ARRISGro ARRIS Group, Inc."
+60:1B:52,Vodafone Vodafone Italia S.p.A.
 60:1D:0F,MidniteS Midnite Solar
 60:1D:91,"Motorola Motorola Mobility LLC, a Lenovo Company"
 60:1D:9D,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 60:1E:02,EltexAla EltexAlatau
 60:1E:98,AxevastT Axevast Technology
 60:21:01,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 60:21:03,"I4Vine I4Vine, Inc"
 60:21:C0,"MurataMa Murata Manufacturing Co., Ltd."
-60:22:32,Ubiquiti Ubiquiti Networks Inc.
+60:22:32,Ubiquiti Ubiquiti Inc
 60:23:A4,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 60:24:C1,"JiangsuZ Jiangsu Zhongxun Electronic Technology Co., Ltd"
 60:26:AA,"Cisco Cisco Systems, Inc"
 60:26:EF,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 60:27:1C,VIDEOREH VIDEOR E. Hartig GmbH
 60:29:2B,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 60:29:D5,DAVOLINK DAVOLINK Inc.
+60:2A:1B,Jancus
 60:2A:54,CardioTe CardioTek B.V.
 60:2A:D0,CiscoSPV Cisco SPVTG
+60:2B:58,EMMicroe EM Microelectronic
 60:2E:20,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:30:D4,"Apple Apple, Inc."
 60:31:3B,SunnovoI Sunnovo International Limited
 60:31:97,ZyxelCom Zyxel Communications Corporation
 60:32:B1,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 60:32:F0,Mplustec Mplus technology
 60:33:4B,"Apple Apple, Inc."
@@ -26995,44 +27456,46 @@
 60:36:DD,IntelCor Intel Corporate
 60:38:0E,"Alpsalpi Alpsalpine Co,.Ltd"
 60:38:E0,BelkinIn Belkin International Inc.
 60:39:1F,ABB ABB Ltd
 60:3A:7C,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 60:3A:AF,"SamsungE Samsung Electronics Co.,Ltd"
 60:3C:EE,LGElectr LG Electronics (Mobile Communications)
-60:3D:26,Technico Technicolor CH USA Inc.
+60:3D:26,VantivaU Vantiva USA LLC
 60:3D:29,"HuaweiTe Huawei Technologies Co.,Ltd"
+60:3E:5F,"Apple Apple, Inc."
 60:3E:7B,"Gafachi Gafachi, Inc."
 60:3E:CA,Cambridg Cambridge Medical Robotics Ltd
 60:3F:C5,"Cox Cox Co., Ltd"
 60:42:7F,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 60:44:7A,Water-id Water-i.d. GmbH
 60:44:F5,EasyDigi Easy Digital Ltd.
 60:45:5E,Liptelsr Liptel s.r.o.
 60:45:BD,Microsof Microsoft
 60:45:CB,ASUSTekC ASUSTek COMPUTER INC.
 60:46:16,"XiamenVa Xiamen Vann Intelligent Co., Ltd"
 60:47:62,"BeijingS Beijing Sensoro Technology Co.,Ltd."
 60:47:D4,"FORICSEl FORICS Electronic Technology Co., Ltd."
 60:48:26,Newbridg Newbridge Technologies Int. Ltd.
+60:48:9C,"YippeeEl Yippee Electronics Co.,Limited"
 60:49:C1,Avaya Avaya Inc
 60:4A:1C,SUYIN SUYIN Corporation
 60:4B:AA,"MagicLea Magic Leap, Inc."
 60:4D:E1,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:4F:5B,"HuaweiDe Huawei Device Co., Ltd."
 60:50:C1,KinetekS Kinetek Sports
 60:51:2C,TCTmobil TCT mobile ltd
 60:52:D0,FACTSEng FACTS Engineering
 60:53:17,Sandston Sandstone Technologies
 60:53:75,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:54:64,EyedroGr Eyedro Green Solutions Inc.
 60:55:F9,Espressi Espressif Inc.
 60:56:61,IXECLOUD IXECLOUD Tech
 60:56:7D,"AMTeleco AM Telecom co., Ltd."
-60:56:99,MarelliM Marelli Morocco LLC SARL
+60:56:99,MAGNETIM MAGNETI MARELLI S.E. S.p.A.
 60:57:18,IntelCor Intel Corporate
 60:57:47,CigShang Cig Shanghai Co Ltd
 60:57:7D,eero eero inc.
 60:58:01,"Shandong Shandong ZTop Microelectronics Co., Ltd."
 60:5B:30,Dell Dell Inc.
 60:5B:B4,AzureWav AzureWave Technology Inc.
 60:5E:4F,"HuaweiDe Huawei Device Co., Ltd."
@@ -27063,25 +27526,28 @@
 60:70:6C,"Google Google, Inc."
 60:70:72,"Shenzhen Shenzhen Hongde Smart Link Technology Co., Ltd"
 60:70:C0,"Apple Apple, Inc."
 60:72:0B,BLUProdu BLU Products Inc
 60:73:5C,"Cisco Cisco Systems, Inc"
 60:73:BC,zte zte corporation
 60:74:8D,AtmacaEl Atmaca Elektronik
+60:74:F4,Private
+60:76:23,"Shenzhen Shenzhen E-Superlink Technology Co., Ltd"
 60:76:88,Velodyne
 60:77:71,TexasIns Texas Instruments
 60:77:E2,"SamsungE Samsung Electronics Co.,Ltd"
 60:7D:09,"Luxshare Luxshare Precision Industry Co., Ltd"
 60:7D:DD,"Shenzhen Shenzhen Shichuangyi Electronics Co.,Ltd"
 60:7E:A4,Shanghai Shanghai Imilab Technology Co.Ltd
 60:7E:C9,"Apple Apple, Inc."
 60:7E:CD,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:7E:DD,Microsof Microsoft Mobile Oy
 60:81:2B,Astronic Astronics Custom Control Concepts
 60:81:F9,"Helium Helium Systems, Inc"
+60:82:46,"Apple Apple, Inc."
 60:83:34,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:83:73,"Apple Apple, Inc."
 60:83:B2,GkWareeK GkWare e.K.
 60:84:3B,"Soladigm Soladigm, Inc."
 60:84:BD,Buffalo Buffalo.Inc
 60:86:45,"AveryWei Avery Weigh-Tronix, LLC"
 60:89:3C,ThermoFi Thermo Fisher Scientific P.O.A.
@@ -27099,14 +27565,15 @@
 60:8F:5C,"SamsungE Samsung Electronics Co.,Ltd"
 60:8F:A4,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 60:90:84,DSSD DSSD Inc
 60:91:F3,"vivoMobi vivo Mobile Communication Co., Ltd."
 60:92:17,"Apple Apple, Inc."
 60:92:F5,"ARRISGro ARRIS Group, Inc."
 60:93:16,"Apple Apple, Inc."
+60:95:32,ZebraTec Zebra Technologies Inc.
 60:95:BD,"Apple Apple, Inc."
 60:95:CE,IEEERegi IEEE Registration Authority
 60:95:CE:00:00:00/28,SiemaApp Siema Applications
 60:95:CE:10:00:00/28,PonoorEx Ponoor Experiments Inc.
 60:95:CE:20:00:00/28,"Q-SENTEC Q-SENTECH Co.,Ltd."
 60:95:CE:30:00:00/28,Robot Robot S.A.
 60:95:CE:40:00:00/28,"Untangle Untangle, Inc."
@@ -27117,14 +27584,15 @@
 60:95:CE:90:00:00/28,"Jlztlink Jlztlink Industry(ShenZhen)Co.,Ltd."
 60:95:CE:A0:00:00/28,UnManned (Un)Manned
 60:95:CE:B0:00:00/28,"BeijingS Beijing Sinomedisite Bio-tech Co.,Ltd"
 60:95:CE:C0:00:00/28,Synamedi Synamedia
 60:95:CE:D0:00:00/28,GovComm
 60:95:CE:E0:00:00/28,VNS VNS Inc.
 60:96:20,Private
+60:96:A4,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:97:DD,MicroSys MicroSys Electronics GmbH
 60:98:13,Shanghai Shanghai Visking Digital Technology Co. LTD
 60:98:66,TexasIns Texas Instruments
 60:99:D1,VuzixLen Vuzix / Lenovo
 60:9A:A4,GviSecur Gvi Security Inc.
 60:9A:C1,"Apple Apple, Inc."
 60:9B:2D,"JMACSJap JMACS Japan Co., Ltd."
@@ -27167,25 +27635,29 @@
 60:BA:18,nextLAP nextLAP GmbH
 60:BB:0C,"BeijingH Beijing HuaqinWorld Technology Co,Ltd"
 60:BC:4C,EWMHight EWM Hightec Welding GmbH
 60:BD:91,MoveInno Move Innovation
 60:BE:B4,"S-Bluete S-Bluetech co., limited"
 60:BE:B5,"Motorola Motorola Mobility LLC, a Lenovo Company"
 60:BE:C4,"Apple Apple, Inc."
+60:C0:1E,"V&GInfor V&G Information System Co.,Ltd"
 60:C0:BF,ONSemico ON Semiconductor
 60:C1:CB,"FujianGr Fujian Great Power PLC Equipment Co.,Ltd"
 60:C3:97,2Wire 2Wire Inc
 60:C5:47,"Apple Apple, Inc."
 60:C5:A8,"BeijingL Beijing LT Honway Technology Co.,Ltd"
 60:C5:AD,"SamsungE Samsung Electronics Co.,Ltd"
 60:C5:E6,Skullcan Skullcandy
 60:C6:58,"PHYTRONI PHYTRONIX Co.,Ltd."
+60:C7:27,Digiboar Digiboard Eletronica da Amazonia Ltda
+60:C7:8D,JuniperN Juniper Networks
 60:C7:98,Verifone
 60:C7:BE,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 60:C9:80,Trymus
+60:C9:AA,Nokia
 60:CB:FB,AirScape AirScape Inc.
 60:CD:A9,Abloomy
 60:CD:C5,"TaiwanCa Taiwan Carol Electronics., Ltd"
 60:CE:41,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:CE:86,Sercomm Sercomm Corporation.
 60:CE:92,RefinedI The Refined Industry Company Limited
 60:CF:69,meerecom meerecompany
@@ -27222,34 +27694,39 @@
 60:D9:A0,LenovoMo Lenovo Mobile Communication Technology Ltd.
 60:D9:C7,"Apple Apple, Inc."
 60:DA:23,"Estech Estech Co.,Ltd"
 60:DA:83,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 60:DB:15,"NewH3CTe New H3C Technologies Co., Ltd"
 60:DB:2A,Hns
 60:DB:98,Calix Calix Inc.
+60:DB:EF,UnifySof Unify Software and Solutions GmbH & Co. KG
+60:DC:81,AltoBeam AltoBeam Inc.
 60:DD:70,"Apple Apple, Inc."
 60:DD:8E,IntelCor Intel Corporate
 60:DE:35,"GITSN GITSN, Inc."
 60:DE:44,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:DE:F3,"HuaweiTe Huawei Technologies Co.,Ltd"
+60:DE:F4,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 60:E0:0E,ShinseiE Shinsei Electronics Co Ltd
 60:E3:27,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 60:E3:2B,IntelCor Intel Corporate
 60:E3:AC,LGElectr LG Electronics (Mobile Communications)
 60:E6:BC,"Sino-Tel Sino-Telecom Technology Co.,Ltd."
 60:E6:F0,WistronN Wistron Neweb Corporation
 60:E7:01,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:E7:8A,Unisem
 60:E8:5B,TexasIns Texas Instruments
 60:E9:56,"AylaNetw Ayla Networks, Inc"
 60:E9:AA,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 60:EB:5A,"Asterfus Asterfusion Data Technologies Co.,Ltd"
 60:EB:69,QuantaCo Quanta Computer Inc.
 60:EE:5C,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
+60:EF:AB,SiliconL Silicon Laboratories
 60:EF:C6,Shenzhen Shenzhen Chima Technologies Co Limited
+60:F0:4D,"HonorDev Honor Device Co., Ltd."
 60:F1:3D,JABLOCOM JABLOCOM s.r.o.
 60:F1:89,"MurataMa Murata Manufacturing Co., Ltd."
 60:F1:8A,"HuaweiTe Huawei Technologies Co.,Ltd"
 60:F2:62,IntelCor Intel Corporate
 60:F2:81,"TranwoTe Tranwo Technology Co., Ltd."
 60:F2:EF,"VisionVe VisionVera International Co., Ltd."
 60:F3:DA,LogicWay Logic Way GmbH
@@ -27258,27 +27735,30 @@
 60:F4:94,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 60:F5:9C,CRU-Data CRU-Dataport
 60:F6:73,Terumo Terumo Corporation
 60:F6:77,IntelCor Intel Corporate
 60:F8:1D,"Apple Apple, Inc."
 60:F8:F2,Synaptec
 60:FA:9D,"HuaweiTe Huawei Technologies Co.,Ltd"
+60:FA:B1,Kempower Kempower Oyj
 60:FA:CD,"Apple Apple, Inc."
 60:FB:00,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 60:FB:42,"Apple Apple, Inc."
 60:FC:F1,Private
 60:FD:56,"WOORISYS WOORISYSTEMS CO., Ltd"
+60:FD:A6,"Apple Apple, Inc."
 60:FE:1E,ChinaPal China Palms Telecom.Ltd
 60:FE:20,2Wire 2Wire Inc
 60:FE:C5,"Apple Apple, Inc."
 60:FE:F9,ThomasBe Thomas & Betts
 60:FF:12,"SamsungE Samsung Electronics Co.,Ltd"
 60:FF:DD,"CEElectr C.E. Electronics, Inc"
 64:00:2D,"Powerlin Powerlinq Co., LTD"
 64:00:6A,Dell Dell Inc.
+64:00:9C,Insulet Insulet Corporation
 64:00:F1,"Cisco Cisco Systems, Inc"
 64:01:FB,Landis+G Landis+Gyr GmbH
 64:02:CB,"ARRISGro ARRIS Group, Inc."
 64:03:7F,"SamsungE Samsung Electronics Co.,Ltd"
 64:05:BE,NewLight New Light Led
 64:05:E4,"Alpsalpi Alpsalpine Co,.Ltd"
 64:05:E9,"Shenzhen Shenzhen WayOS Technology Crop., Ltd."
@@ -27295,27 +27775,30 @@
 64:0E:6A,SECO-LAR SECO-LARM USA Inc
 64:0E:94,"Pluribus Pluribus Networks, Inc."
 64:0E:9B,"IshidaMe Ishida Medical Co., Ltd."
 64:0F:28,2Wire 2Wire Inc
 64:10:84,"HEXIUMTe HEXIUM Technical Development Co., Ltd."
 64:11:A4,"Motorola Motorola Mobility LLC, a Lenovo Company"
 64:12:25,"Cisco Cisco Systems, Inc"
-64:12:36,Technico Technicolor CH USA Inc.
+64:12:36,VantivaU Vantiva USA LLC
 64:12:69,"ARRISGro ARRIS Group, Inc."
 64:13:31,BoschCar Bosch Car Multimedia (Wuhu) Co. Ltd.
 64:13:5A,Itectra Itectra A/S
 64:13:6C,zte zte corporation
 64:13:AB,"HuaweiTe Huawei Technologies Co.,Ltd"
 64:16:66,NestLabs Nest Labs Inc.
 64:16:7F,Polycom
 64:16:8D,"Cisco Cisco Systems, Inc"
 64:16:F0,"HuaweiTe Huawei Technologies Co.,Ltd"
 64:17:59,"Intelliv Intellivision Holdings, LLC"
+64:17:CD,"SamsungE Samsung Electronics Co.,Ltd"
 64:1A:22,Heliospe Heliospectra AB
 64:1A:BA,DryadNet Dryad Networks GmbH
+64:1B:2F,"SamsungE Samsung Electronics Co.,Ltd"
+64:1C:10,TexasIns Texas Instruments
 64:1C:67,Digibras Digibras Industria Do Brasils/A
 64:1C:AE,"SamsungE Samsung Electronics Co.,Ltd"
 64:1C:B0,"SamsungE Samsung Electronics Co.,Ltd"
 64:1E:81,Dowslake Dowslake Microsystems
 64:20:0C,"Apple Apple, Inc."
 64:20:9F,Tilgin Tilgin AB
 64:20:E0,"T3Techno T3 Technology Co., Ltd."
@@ -27342,15 +27825,17 @@
 64:31:39:20:00:00/28,Smartplu Smartplus Inc.
 64:31:39:30:00:00/28,"Koangyow Koangyow Integration Machine Co., Ltd."
 64:31:39:40:00:00/28,ActiveBr Active Brains
 64:31:39:50:00:00/28,"Shenzhen Shenzhen He&e Technology Co.,Ltd."
 64:31:39:60:00:00/28,"HunanVoc Hunan Voc Acoustics Technology Co., Ltd."
 64:31:39:70:00:00/28,"Dongguan Dongguan Huili electroacoustic Industrial Co.,ltd"
 64:31:39:80:00:00/28,Shenzhen Shenzhen Huanyin Electronics Ltd.
+64:31:39:90:00:00/28,Honeywel Honeywell Analytics Ltd
 64:31:39:A0:00:00/28,"ProductD Product Development Associates, Inc."
+64:31:39:B0:00:00/28,Alphago Alphago GmbH
 64:31:39:C0:00:00/28,"SHENZHEN SHEN ZHEN FUCHANG TECHNOLOGY Co.,Ltd."
 64:31:39:D0:00:00/28,"Zhejiang Zhejiang Moorgen Intelligent Technology Co.,Ltd"
 64:31:39:E0:00:00/28,ATGUVTec ATG UV Technology
 64:31:50,HewlettP Hewlett Packard
 64:31:72,"Zhejiang Zhejiang Hising Technology Co.,Ltd"
 64:31:7E,Dexin Dexin Corporation
 64:32:16,"WeiduTec Weidu Technology (Beijing) Co., Ltd."
@@ -27373,14 +27858,15 @@
 64:33:B5:E0:00:00/28,Universi University of Texas at Austin
 64:33:DB,TexasIns Texas Instruments
 64:34:09,BITwaveP BITwave Pte Ltd
 64:35:1C,e-CONIND e-CON SYSTEMS INDIA PVT LTD
 64:37:A4,"Tokyoshu Tokyoshuha Co.,Ltd."
 64:3A:B1,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 64:3A:EA,"Cisco Cisco Systems, Inc"
+64:3E:0A,"HuaweiTe Huawei Technologies Co.,Ltd"
 64:3E:8C,"HuaweiTe Huawei Technologies Co.,Ltd"
 64:3F:5F,Exablaze
 64:42:12,"Shenzhen Shenzhen Water World Information Co.,Ltd."
 64:42:14,Swisscom Swisscom Energy Solutions AG
 64:43:46,"GuangDon GuangDong Quick Network Computer CO.,LTD"
 64:44:D5,TDTech TD Tech
 64:47:E0,"FeitianT Feitian Technologies Co., Ltd"
@@ -27391,14 +27877,15 @@
 64:4D:70,dSPACE dSPACE GmbH
 64:4F:42,"JETTER JETTER CO., Ltd."
 64:4F:74,"LENUS LENUS Co., Ltd."
 64:4F:B0,Hyunjinc Hyunjin.com
 64:50:D6,Liquidto Liquidtool Systems
 64:51:06,HewlettP Hewlett Packard
 64:51:7E,"LongBenD Long Ben (Dongguan) Electronic Technology Co.,Ltd."
+64:52:34,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 64:52:99,"Chamberl The Chamberlain Group, Inc"
 64:53:5D,Frausche Frauscher Sensortechnik
 64:54:22,EquinoxP Equinox Payments
 64:55:63,Inteligh Intelight Inc.
 64:55:7F,"NSFOCUSI NSFOCUS Information Technology Co., Ltd."
 64:55:B1,"ARRISGro ARRIS Group, Inc."
 64:56:01,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
@@ -27440,14 +27927,15 @@
 64:62:8A,evon evon GmbH
 64:64:4A,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 64:64:9B,JuniperN Juniper Networks
 64:65:C0,"Nuvon Nuvon, Inc"
 64:66:24,Sagemcom Sagemcom Broadband SAS
 64:66:B3,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 64:67:07,"BeijingO Beijing Omnific Technology, Ltd."
+64:67:CD,"HuaweiTe Huawei Technologies Co.,Ltd"
 64:68:0C,Comtrend Comtrend Corporation
 64:68:76,EdifierI Edifier International
 64:69:4E,TexasIns Texas Instruments
 64:69:BC,"HyteraCo Hytera Communications Co.,ltd"
 64:6A:52,Avaya Avaya Inc
 64:6A:74,"Auth-Ser Auth-Servers, Llc"
 64:6C:80,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
@@ -27486,24 +27974,26 @@
 64:87:88,JuniperN Juniper Networks
 64:87:D7,ADBBroad ADB Broadband Italia
 64:88:FF,SichuanC Sichuan Changhong Electric Ltd.
 64:89:9A,LGElectr LG Electronics (Mobile Communications)
 64:89:F1,"SamsungE Samsung Electronics Co.,Ltd"
 64:8C:BB,TexasIns Texas Instruments
 64:8D:9E,"IVTElect IVT Electronic Co.,Ltd"
+64:8F:3E,"Cisco Cisco Systems, Inc"
 64:90:C1,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 64:95:6C,LGElectr LG Electronics
 64:97:14,eero eero inc.
 64:98:29,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 64:98:9E,TrinnovA Trinnov Audio
 64:99:5D,Lge
 64:99:68,Elentec
 64:99:A0,Elektron AG Elektronik AB
 64:9A:08,"Shenzhen Shenzhen SuperElectron Technology Co.,LTD"
 64:9A:12,P2Mobile P2 Mobile Technologies Limited
+64:9A:63,Ring Ring LLC
 64:9A:BE,"Apple Apple, Inc."
 64:9B:24,"VTechnol V Technology Co., Ltd."
 64:9C:81,Qualcomm Qualcomm Inc.
 64:9C:8E,TexasIns Texas Instruments
 64:9D:99,FsCom Fs Com Inc
 64:9E:31,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 64:9E:F3,"Cisco Cisco Systems, Inc"
@@ -27525,22 +28015,24 @@
 64:A9:65,"Linkflow Linkflow Co., Ltd."
 64:AE:0C,"Cisco Cisco Systems, Inc"
 64:AE:88,Polytec Polytec GmbH
 64:AE:F1,"QingdaoH Qingdao Hisense Electronics Co.,Ltd."
 64:B0:A6,"Apple Apple, Inc."
 64:B0:E8,"HuaweiDe Huawei Device Co., Ltd."
 64:B2:1D,"ChengduP Chengdu Phycom Tech Co., Ltd."
+64:B2:B4,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 64:B3:10,"SamsungE Samsung Electronics Co.,Ltd"
 64:B3:70,PowerCom PowerComm Solutions LLC
-64:B3:79,Private
+64:B3:79,"JiangsuV Jiangsu Viscore Technologies Co.,Ltd"
 64:B4:73,XiaomiCo Xiaomi Communications Co Ltd
 64:B5:C6,"Nintendo Nintendo Co.,Ltd"
 64:B5:F2,"SamsungE Samsung Electronics Co.,Ltd"
 64:B6:23,SchrackS Schrack Seconet Care Communication GmbH
 64:B6:4A,"ViVOtech ViVOtech, Inc."
+64:B7:08,Espressi Espressif Inc.
 64:B8:53,"SamsungE Samsung Electronics Co.,Ltd"
 64:B9:4E,DellTech Dell Technologies
 64:B9:E8,"Apple Apple, Inc."
 64:BA:BD,"SDJTechn SDJ Technologies, Inc."
 64:BC:0C,LGElectr LG Electronics (Mobile Communications)
 64:BC:11,CombiQ CombiQ AB
 64:BC:58,IntelCor Intel Corporate
@@ -27562,15 +28054,15 @@
 64:C9:44,"LARKTech LARK Technologies, Inc"
 64:CB:5D,"SIATeleS SIA ""TeleSet"""
 64:CB:9F,TecnoMob Tecno Mobile Limited
 64:CB:A3,Pointmob Pointmobile
 64:CB:E9,LGInnote LG Innotek
 64:CC:22,Arcadyan Arcadyan Corporation
 64:CC:2E,XiaomiCo Xiaomi Communications Co Ltd
-64:CE:6E,SierraWi Sierra Wireless
+64:CE:6E,"SierraWi Sierra Wireless, ULC"
 64:CF:13,"WeigaoNi Weigao Nikkiso(Weihai)Dialysis Equipment Co.,Ltd"
 64:CF:D9,TexasIns Texas Instruments
 64:D0:2D,NextGene Next Generation Integration Limited (Ngi)
 64:D0:D6,"SamsungE Samsung Electronics Co.,Ltd"
 64:D1:54,Routerbo Routerboard.com
 64:D1:A3,SitecomE Sitecom Europe BV
 64:D2:41,KeithKoe Keith & Koep GmbH
@@ -27595,30 +28087,33 @@
 64:DC:01,StaticGr Static Systems Group PLC
 64:DC:DE,"ZheJiang ZheJiang FuChunJiang Information Technology Co.,Ltd"
 64:DD:E9,XiaomiCo Xiaomi Communications Co Ltd
 64:DE:1C,Kingneti Kingnetic Pte Ltd
 64:DF:10,JingLueS JingLue Semiconductor(SH) Ltd.
 64:DF:E9,Ateme
 64:E0:03,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
-64:E0:AB,"Unionman Unionman Technology Co.,Ltd"
+64:E0:AB,"UnionMan Union Man Technology Co.,Ltd"
 64:E1:61,DEP DEP Corp.
 64:E1:72,"Shenzhen Shenzhen Qihoo Intelligent Technology Co.,Ltd"
+64:E2:04,NTNTechn NTN Technical Service Corporation
 64:E2:20,Qisda Qisda Corporation
+64:E4:A5,LGElectr LG Electronics
 64:E5:99,EFMNetwo EFM Networks
 64:E6:25,"WoxuWire Woxu Wireless Co., Ltd"
 64:E6:82,"Apple Apple, Inc."
 64:E7:D8,"SamsungE Samsung Electronics Co.,Ltd"
 64:E8:33,Espressi Espressif Inc.
 64:E8:4F,Serialwa Serialway Communication Technology Co. Ltd
 64:E8:81,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 64:E8:92,"MorioDen Morio Denki Co., Ltd."
 64:E8:E6,globalmo global moisture management system
 64:E9:50,"Cisco Cisco Systems, Inc"
 64:EA:C5,"SiboTech SiboTech Automation Co., Ltd."
 64:EB:8C,SeikoEps Seiko Epson Corporation
+64:EC:65,"vivoMobi vivo Mobile Communication Co., Ltd."
 64:ED:57,"ARRISGro ARRIS Group, Inc."
 64:ED:62,"WOORI WOORI SYSTEMS Co., Ltd"
 64:EE:B7,NetcoreT Netcore Technology Inc
 64:F2:42,GerdesAk Gerdes Aktiengesellschaft
 64:F2:FB,"Hangzhou Hangzhou Ezviz Software Co.,Ltd."
 64:F5:0E,KinionTe Kinion Technology Company Limited
 64:F5:4E,EMMicroe EM Microelectronic
@@ -27628,14 +28123,15 @@
 64:F7:05,"HuaweiDe Huawei Device Co., Ltd."
 64:F8:1C,"HuaweiTe Huawei Technologies Co., Ltd."
 64:F8:8A,ChinaMob China Mobile IOT Company Limited
 64:F9:47,"Senscomm Senscomm Semiconductor Co., Ltd."
 64:F9:70,"KenadeEl Kenade Electronics Technology Co.,LTD."
 64:F9:87,Avvasi Avvasi Inc.
 64:F9:C0,AnalogDe Analog Devices
+64:FB:01,Zhongsha Zhongshan Camry Electronic Company Limited
 64:FB:50,"RoomRead RoomReady/Zdi, Inc."
 64:FB:81,IEEERegi IEEE Registration Authority
 64:FB:81:00:00:00/28,Shanghai Shanghai Simcom Limited
 64:FB:81:10:00:00/28,Narrativ Narrative AB
 64:FB:81:20:00:00/28,SevenSol Seven Solutions S.L
 64:FB:81:30:00:00/28,MOBILUS MOBILUS Inc.
 64:FB:81:40:00:00/28,Pricer Pricer AB
@@ -27663,42 +28159,47 @@
 68:09:27,"Apple Apple, Inc."
 68:0A:D7,"Yancheng Yancheng Kecheng Optoelectronic Technology Co., Ltd"
 68:0A:E2,SiliconL Silicon Laboratories
 68:12:2D,"SpecialI Special Instrument Development Co., Ltd."
 68:12:95,LupineLi Lupine Lighting Systems GmbH
 68:13:24,"HuaweiDe Huawei Device Co., Ltd."
 68:13:E2,EltexEnt Eltex Enterprise LTD
+68:13:F3,AmazonTe Amazon Technologies Inc.
 68:14:01,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 68:15:90,Sagemcom Sagemcom Broadband SAS
 68:15:D3,ZakladyE Zaklady Elektroniki i Mechaniki Precyzyjnej R&G S.A.
 68:16:05,AndElect Systems And Electronic Development FZCO
 68:17:29,IntelCor Intel Corporate
 68:18:D9,HillAFB- Hill AFB - CAPRE Group
 68:19:3F,DigitalA Digital Airways
 68:19:AC,"Guangzho Guangzhou Xianyou Intelligent Technogoly CO., LTD"
+68:1A:7C,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 68:1A:A4,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 68:1A:B2,zte zte corporation
 68:1B:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:1C:A2,Rosewill Rosewill Inc.
 68:1D:64,"SunwaveC Sunwave Communications Co., Ltd"
 68:1D:EF,"Shenzhen Shenzhen CYX Technology Co., Ltd."
 68:1E:8B,InfoSigh InfoSight Corporation
 68:1F:40,BluWirel Blu Wireless Technology Ltd
 68:1F:D8,"SiemensI Siemens Industry, Inc."
 68:21:5F,Edgecore Edgecore Networks Corporation
 68:22:8E,JuniperN Juniper Networks
 68:23:4B,NihonDen Nihon Dengyo Kousaku
+68:23:F4,"Shenzhen Shenzhen Jinlangxin Technology Co., Ltd"
 68:26:24,Ergatta
 68:26:2A,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 68:27:19,Microchi Microchip Technology Inc.
 68:27:37,"SamsungE Samsung Electronics Co.,Ltd"
 68:27:5F,zte zte corporation
 68:28:BA,Dejai
+68:28:CF,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 68:28:F6,"VubiqNet Vubiq Networks, Inc."
 68:29:DC,FicosaEl Ficosa Electronics S.L.U.
+68:2C:4F,leerang leerang corporation
 68:2C:7B,"Cisco Cisco Systems, Inc"
 68:2D:83,Shenzhen Shenzhen Dinghe Communication Company
 68:2D:DC,"WuhanCha Wuhan Changjiang Electro-Communication Equipment CO.,LTD"
 68:2F:67,"Apple Apple, Inc."
 68:31:FE,"Teladin Teladin Co.,Ltd."
 68:33:2C,KenstelN Kenstel Networks Limited
 68:34:89,LEAProfe LEA Professional
@@ -27719,66 +28220,73 @@
 68:3F:7D,IngramMi Ingram Micro Services
 68:40:3C,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 68:41:8F,"Telechip Telechips, Inc."
 68:43:52,Bhuu Bhuu Limited
 68:43:D7,Agilecom Agilecom Photonics Solutions Guangdong Limited
 68:45:71,"HuaweiDe Huawei Device Co., Ltd."
 68:45:F1,"ToshibaC Toshiba Client Solutions Co., Ltd."
+68:47:24,EMMicroe EM Microelectronic
 68:47:49,TexasIns Texas Instruments
 68:48:98,"SamsungE Samsung Electronics Co.,Ltd"
 68:49:92,CiscoMer Cisco Meraki
 68:49:B2,CarloGav Carlo Gavazzi Ltd
 68:4A:76,eero eero inc.
 68:4A:AE,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:4A:E9,"SamsungE Samsung Electronics Co.,Ltd"
 68:4B:88,Galtroni Galtronics Telemetry Inc.
 68:4C:A8,"Shenzhen Shenzhen Herotel Tech. Co., Ltd."
 68:4E:05,HunanFn- Hunan Fn-Link Technology Limited
 68:4F:64,Dell Dell Inc.
+68:50:5D,HaloTech Halo Technologies
 68:51:B7,"PowerClo PowerCloud Systems, Inc."
 68:52:D6,"UGameTec UGame Technology Co.,Ltd"
 68:53:6C,"SPnS SPnS Co.,Ltd"
 68:53:88,P&STechn P&S Technology
 68:53:9D,EMMicroe EM Microelectronic
 68:54:5A,IntelCor Intel Corporate
 68:54:C1,"ColorTok ColorTokens, Inc."
 68:54:ED,Alcatel- Alcatel-Lucent
 68:54:F5,enLighte enLighted Inc
 68:54:FD,AmazonTe Amazon Technologies Inc.
 68:57:2D,TuyaSmar Tuya Smart Inc.
 68:58:11,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 68:58:C5,ZFTRWAut ZF TRW Automotive
+68:59:32,"SunitecE Sunitec Enterprise Co.,Ltd"
 68:59:7F,AlcatelL Alcatel Lucent
 68:5A:CF,"SamsungE Samsung Electronics Co.,Ltd"
 68:5B:35,"Apple Apple, Inc."
 68:5B:36,"Powertec Powertech Industrial Co., Ltd."
 68:5D:43,IntelCor Intel Corporate
 68:5E:1C,TexasIns Texas Instruments
 68:5E:6B,"PowerRay PowerRay Co., Ltd."
 68:63:50,HellaInd Hella India Automotive Pvt Ltd
 68:63:59,Advanced Advanced Digital Broadcast SA
+68:63:72,"HuaweiDe Huawei Device Co., Ltd."
 68:64:4B,"Apple Apple, Inc."
 68:65:B7,"Zhishang Zhishang Chuanglian Technology Co., Ltd"
 68:67:25,Espressi Espressif Inc.
 68:69:2E,"Zycoo Zycoo Co.,Ltd"
 68:69:75,AnglerLa Angler Labs Inc
 68:69:CA,"Hitachi Hitachi, Ltd."
 68:69:F2,ComApsro ComAp s.r.o.
 68:6C:E6,Microsof Microsoft Corporation
 68:6D:BC,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 68:6E:23,Wi3 Wi3 Inc.
 68:6E:48,"ProphetE Prophet Electronic Technology Corp.,Ltd"
-68:72:51,Ubiquiti Ubiquiti Networks Inc.
+68:71:61,"Cisco Cisco Systems, Inc"
+68:72:51,Ubiquiti Ubiquiti Inc
 68:72:C3,"SamsungE Samsung Electronics Co.,Ltd"
 68:72:DC,CETORYTV CETORY.TV Company Limited
 68:76:27,"ZhuhaiDi Zhuhai Dingzhi Electronic Technology Co., Ltd"
 68:76:4F,Sony Sony Corporation
 68:77:24,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
+68:77:DA,zte zte corporation
 68:78:48,"Westunit Westunitis Co., Ltd."
 68:78:4C,NortelNe Nortel Networks
+68:79:09,"Cisco Cisco Systems, Inc"
 68:79:12,IEEERegi IEEE Registration Authority
 68:79:12:00:00:00/28,"PCTEL PCTEL, Inc."
 68:79:12:10:00:00/28,Annapurn Annapurna labs
 68:79:12:20:00:00/28,"Cndi Cndi Co.,Ltd"
 68:79:12:30:00:00/28,StephanE Stephan Electronics SARL
 68:79:12:40:00:00/28,McDonald McDonald's Corporation
 68:79:12:50:00:00/28,"CopperLa Copper Labs, Inc."
@@ -27788,14 +28296,15 @@
 68:79:12:90:00:00/28,LEAPSsro LEAPS s.r.o.
 68:79:12:A0:00:00/28,"Wingtech Wingtech Mobile Communications Co., Ltd."
 68:79:12:B0:00:00/28,Swisscom Swisscom Broadcast Ltd
 68:79:12:C0:00:00/28,GlobusIn Globus Infocom Limited
 68:79:12:D0:00:00/28,Neurolab
 68:79:12:E0:00:00/28,AmetekSo Ametek Solidstate Controls
 68:79:24,ELS ELS-GmbH & Co. KG
+68:79:DD,Omniples Omnipless Manufacturing (PTY) Ltd
 68:79:ED,SHARP SHARP Corporation
 68:7A:64,IntelCor Intel Corporate
 68:7C:C8,Measurem Measurement Systems S. de R.L.
 68:7C:D5,"YSoft Y Soft Corporation, a.s."
 68:7D:6B,"SamsungE Samsung Electronics Co.,Ltd"
 68:7D:B4,"Cisco Cisco Systems, Inc"
 68:7F:74,"Cisco-Li Cisco-Linksys, LLC"
@@ -27804,14 +28313,15 @@
 68:82:F2,grandcen grandcentrix GmbH
 68:83:1A,PandoraM Pandora Mobility Corporation
 68:83:CB,"Apple Apple, Inc."
 68:84:70,"eSSys eSSys Co.,Ltd"
 68:84:7E,Fujitsu Fujitsu Limited
 68:85:40,"IGIMobil IGI Mobile, Inc."
 68:85:6A,OuterLin OuterLink Corporation
+68:85:A4,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 68:86:A7,"Cisco Cisco Systems, Inc"
 68:86:E7,"Orbotix Orbotix, Inc."
 68:87:1C,"Motorola Motorola Mobility LLC, a Lenovo Company"
 68:87:6B,INQMobil INQ Mobile Limited
 68:87:C6,"Cisco Cisco Systems, Inc"
 68:88:A1,"Universa Universal Electronics, Inc."
 68:89:75,nuoxc
@@ -27846,29 +28356,32 @@
 68:96:2E,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:96:6A,Ohsung
 68:96:7B,"Apple Apple, Inc."
 68:97:4B,Shenzhen Shenzhen Costar Electronics Co. Ltd.
 68:97:E8,SocietyM Society of Motion Picture & Television Engineers
 68:98:61,Beacon Beacon Inc
 68:99:CD,"Cisco Cisco Systems, Inc"
+68:9A:21,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 68:9A:87,AmazonTe Amazon Technologies Inc.
 68:9A:B7,AtelierV Atelier Vision Corporation
 68:9C:5E,AcSiPTec AcSiP Technology Corp.
 68:9C:70,"Apple Apple, Inc."
 68:9C:E2,"Cisco Cisco Systems, Inc"
 68:9E:0B,"Cisco Cisco Systems, Inc"
 68:9E:19,TexasIns Texas Instruments
+68:9E:29,zte zte corporation
 68:9E:6A,"HuaweiDe Huawei Device Co., Ltd."
 68:9F:F0,zte zte corporation
 68:A0:3E,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:A0:F6,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:A1:B7,"HonghaoM Honghao Mingchuan Technology (Beijing) CO.,Ltd."
 68:A3:78,FreeboxS Freebox Sas
 68:A3:C4,LiteonTe Liteon Technology Corporation
 68:A4:0E,BSHHausg BSH Hausgeräte GmbH
+68:A4:6A,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:A4:7D,SunCupid Sun Cupid Technology (HK) LTD
 68:A6:82,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 68:A7:B4,"HonorDev Honor Device Co., Ltd."
 68:A8:28,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:A8:6D,"Apple Apple, Inc."
 68:A8:78,GeoWAN GeoWAN Pty Ltd
 68:A8:E1,"Wacom Wacom Co.,Ltd."
@@ -27910,33 +28423,52 @@
 68:D1:BA,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 68:D1:FD,"Shenzhen Shenzhen Trimax Technology Co.,Ltd"
 68:D2:47,Portalis Portalis LC
 68:D4:0C,Tellesco Tellescom Industria E Comercio Em Telecomunicacao
 68:D4:82,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 68:D4:8B,HailoTec Hailo Technologies Ltd.
 68:D6:ED,"GooWiWir GooWi Wireless Technology Co., Limited"
-68:D7:9A,Ubiquiti Ubiquiti Networks Inc.
+68:D7:9A,Ubiquiti Ubiquiti Inc
 68:D9:25,ProSysDe ProSys Development Services
 68:D9:27,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:D9:3C,"Apple Apple, Inc."
+68:DA:73,IEEERegi IEEE Registration Authority
+68:DA:73:00:00:00/28,Annapurn Annapurna labs
+68:DA:73:10:00:00/28,DTEN DTEN Inc.
+68:DA:73:20:00:00/28,"Shenzhen Shenzhen Alldocube Science And Technology Co., Ltd."
+68:DA:73:30:00:00/28,Softroni Softronics Ltd
+68:DA:73:40:00:00/28,Agramkow Agramkow A/S
+68:DA:73:50:00:00/28,"Shenzhen Shenzhen Xin hang xian Electronics Co., LTD"
+68:DA:73:60:00:00/28,"GlobalNe Global Networks ZEN-EI Co., Ltd"
+68:DA:73:70:00:00/28,HavenLig Haven Lighting
+68:DA:73:80:00:00/28,StelFibe Stel Fiber Electronics India Private Limited
+68:DA:73:90:00:00/28,"NadexMac Nadex Machinery(Shanghai) Co.,Ltd"
+68:DA:73:A0:00:00/28,"Shenzhen Shenzhen Haiyingzhilian Industrial Co., Ltd."
+68:DA:73:B0:00:00/28,Gamber-J Gamber-Johnson LLC
+68:DA:73:C0:00:00/28,DeltaSur Delta Surge Inc.
+68:DA:73:D0:00:00/28,SichuanG Sichuan GFS Information Technology Co.Ltd
+68:DA:73:E0:00:00/28,Synamedi Synamedia
 68:DB:54,"PhicommS Phicomm (Shanghai) Co., Ltd."
 68:DB:67,"NantongC Nantong Coship Electronics Co., Ltd."
 68:DB:96,"OPWILLTe OPWILL Technologies CO.,LTD"
 68:DB:CA,"Apple Apple, Inc."
 68:DB:F5,AmazonTe Amazon Technologies Inc.
 68:DC:E8,PacketSt PacketStorm Communications
 68:DD:26,"Shanghai Shanghai Focus Vision Security Technology Co.,Ltd"
+68:DD:B7,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 68:DD:D9,HMDGloba HMD Global Oy
+68:DE:CE,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 68:DF:DD,XiaomiCo Xiaomi Communications Co Ltd
 68:E1:54,SiMaai SiMa.ai
 68:E1:66,Private
 68:E1:DC,Buffalo Buffalo.Inc
 68:E2:09,"HuaweiTe Huawei Technologies Co.,Ltd"
 68:E4:1F,Unglaube Unglaube Identech GmbH
 68:E4:78,"QingdaoH Qingdao Haier Technology Co.,Ltd"
+68:E5:9E,"Cisco Cisco Systems, Inc"
 68:E7:4A,TexasIns Texas Instruments
 68:E7:C2,"SamsungE Samsung Electronics Co.,Ltd"
 68:E8:EB,"LinktelT Linktel Technologies Co.,Ltd"
 68:EB:AE,"SamsungE Samsung Electronics Co.,Ltd"
 68:EB:C5,Angstrem Angstrem Telecom
 68:EC:62,YODOTech YODO Technology Corp. Ltd.
 68:EC:8A,IKEASwed IKEA of Sweden AB
@@ -27945,19 +28477,21 @@
 68:ED:A4,"Shenzhen Shenzhen Seavo Technology Co.,Ltd"
 68:EE:4B,"Sharetro Sharetronic Data Technology Co.,Ltd"
 68:EE:88,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 68:EE:96,CiscoSPV Cisco SPVTG
 68:EF:43,"Apple Apple, Inc."
 68:EF:BD,"Cisco Cisco Systems, Inc"
 68:F0:6D,"AlongInd Along Industrial Co., Limited"
+68:F0:B5,"HonorDev Honor Device Co., Ltd."
 68:F0:BC,"Shenzhen Shenzhen LiWiFi Technology Co., Ltd"
 68:F0:D0,SkyBellT SkyBell Technologies Inc.
 68:F1:25,DataCont Data Controls Inc.
 68:F3:8E,JuniperN Juniper Networks
 68:F5:43,"HuaweiTe Huawei Technologies Co.,Ltd"
+68:F6:3B,AmazonTe Amazon Technologies Inc.
 68:F7:28,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 68:F8:95,Redflow Redflow Limited
 68:F9:56,Objetivo Objetivos y Servicio de Valor Añadido
 68:FB:7E,"Apple Apple, Inc."
 68:FB:95,Generalp Generalplus Technology Inc.
 68:FC:B3,"NextLeve Next Level Security Systems, Inc."
 68:FC:B6,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -27966,24 +28500,27 @@
 68:FE:F7,"Apple Apple, Inc."
 68:FF:7B,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 6A:0E:20,"GeoFrenz GeoFrenzy, Inc"
 6A:1F:6C,"iPass iPass, Inc."
 6A:40:65,OpenConn Open Connectivity Foundation
 6A:5C:35,Secrétar Secrétariat général de la défense et de la sécurité nationale
 6A:62:1E,DIFICons DIFI Consortium
+6A:71:E6,FuelClou FuelCloud
 6A:73:7D,25GEther 25G Ethernet Consortium
 6A:8E:AF,Waoo
 6A:9D:A4,GlobalRe Global Reach Technology
 6A:B6:F2,EliTechn Eli Technology Inc
 6A:E6:4A,S&OElect S&O Electronics (Malaysia) Sdn. Bhd.
 6A:E7:32,"UNIS-WDC UNIS-WDC Storage Co.,Ltd"
 6C:00:6B,"SamsungE Samsung Electronics Co.,Ltd"
 6C:02:73,"Shenzhen Shenzhen Jin Yun Video Equipment Co., Ltd."
 6C:02:E0,HP HP Inc.
 6C:03:09,"Cisco Cisco Systems, Inc"
+6C:03:70,"ExtremeN Extreme Networks, Inc."
+6C:03:B5,"Cisco Cisco Systems, Inc"
 6C:04:60,RBHAcces RBH Access Technologies Inc.
 6C:04:7A,"HuaweiTe Huawei Technologies Co.,Ltd"
 6C:05:D5,Ethertro Ethertronics Inc
 6C:06:D6,"HuaweiDe Huawei Device Co., Ltd."
 6C:08:31,Analog Analog Systems
 6C:09:0A,Gematica Gematica Srl
 6C:09:BF,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
@@ -28035,23 +28572,40 @@
 6C:1E:D7,"vivoMobi vivo Mobile Communication Co., Ltd."
 6C:20:56,"Cisco Cisco Systems, Inc"
 6C:21:A2,"AMPAKTec AMPAK Technology, Inc."
 6C:22:AB,Ainswort Ainsworth Game Technology
 6C:23:16,"TATUNGTe TATUNG Technology Inc.,"
 6C:23:B9,Sony Sony Corporation
 6C:23:CB,Wattty Wattty Corporation
-6C:24:08,"LCFCHefe LCFC(Hefei) Electronics Technology Co., Ltd"
+6C:24:08,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 6C:24:83,Microsof Microsoft Mobile Oy
 6C:24:A6,"vivoMobi vivo Mobile Communication Co., Ltd."
 6C:25:B9,"BbkEduca Bbk Educational Electronics Corp.,Ltd."
 6C:26:36,"HuaweiTe Huawei Technologies Co.,Ltd"
 6C:27:79,Microsof Microsoft Mobile Oy
 6C:29:90,WiZConne WiZ Connected Lighting Company Limited
 6C:29:95,IntelCor Intel Corporate
+6C:29:D2,"Cisco Cisco Systems, Inc"
 6C:2A:CB,PaxtonAc Paxton Access Ltd
+6C:2A:DF,IEEERegi IEEE Registration Authority
+6C:2A:DF:00:00:00/28,Ademcodb Ademco Inc. dba ADI Global Distribution
+6C:2A:DF:10:00:00/28,"XianXind Xi'an Xindian Equipment Engineering Center Co., Ltd"
+6C:2A:DF:20:00:00/28,"DaikoEle Daiko Electric Co.,Ltd"
+6C:2A:DF:30:00:00/28,"JohnsonC Johnson Controls IR, Sabroe Controls"
+6C:2A:DF:40:00:00/28,"Zhejiang Zhejiang Eternal Automation Sci-Tec Co., Ltd"
+6C:2A:DF:50:00:00/28,"Xinjiang Xinjiang Ying Sheng Information Technology Co., Ltd."
+6C:2A:DF:60:00:00/28,ITI ITI Limited
+6C:2A:DF:70:00:00/28,RootV
+6C:2A:DF:80:00:00/28,"BeijingY Beijing Yisheng Chuanqi Technology Co., Ltd."
+6C:2A:DF:90:00:00/28,Simplewa Simpleway Europe a.s.
+6C:2A:DF:A0:00:00/28,Jbf
+6C:2A:DF:B0:00:00/28,MOBAMobi MOBA Mobile Automation AG
+6C:2A:DF:C0:00:00/28,VnetsInf Vnets Information Technology Ltd.
+6C:2A:DF:D0:00:00/28,"SichuanH Sichuan Huidian Qiming Intelligent Technology Co.,Ltd"
+6C:2A:DF:E0:00:00/28,"WeatherF WeatherFlow-Tempest, Inc"
 6C:2B:59,Dell Dell Inc.
 6C:2C:06,NPPSyste OOO NPP Systemotechnika-NN
 6C:2C:DC,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 6C:2D:24,"ZhenShiI Zhen Shi Information Technology (Shanghai) Co., Ltd."
 6C:2E:33,"Accelink Accelink Technologies Co.,Ltd."
 6C:2E:72,B&BExpor B&B Exporting Limited
 6C:2E:85,Sagemcom Sagemcom Broadband SAS
@@ -28081,31 +28635,33 @@
 6C:41:6A,"Cisco Cisco Systems, Inc"
 6C:42:AB,"Subscrib Subscriber Networks, Inc."
 6C:43:3C,TecnoMob Tecno Mobile Limited
 6C:44:18,Zappware
 6C:44:2A,"HuaweiTe Huawei Technologies Co.,Ltd"
 6C:45:98,AntexEle Antex Electronic Corp.
 6C:47:60,"SunitecE Sunitec Enterprise Co.,Ltd"
+6C:48:A6,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 6C:49:C1,"o2ones o2ones Co., Ltd."
 6C:4A:39,Bita
 6C:4A:74,Aerodisk Aerodisk Llc
 6C:4A:85,"Apple Apple, Inc."
 6C:4B:7F,Vossloh- Vossloh-Schwabe Deutschland GmbH
 6C:4B:90,LiteON
 6C:4B:B4,"HUMAX HUMAX Co., Ltd."
+6C:4C:E2,IntelCor Intel Corporate
 6C:4D:51,"Shenzhen Shenzhen Ceres Technology Co., Ltd."
 6C:4D:73,"Apple Apple, Inc."
 6C:4E:86,ThirdMil Third Millennium Systems Ltd.
 6C:4E:F6,"Cisco Cisco Systems, Inc"
 6C:50:4D,"Cisco Cisco Systems, Inc"
 6C:51:BF,"HuaweiDe Huawei Device Co., Ltd."
 6C:54:CD,LampexEl Lampex Electronics Limited
 6C:55:63,"SamsungE Samsung Electronics Co.,Ltd"
 6C:55:8D,"HuaweiTe Huawei Technologies Co.,Ltd"
-6C:55:E8,Technico Technicolor CH USA Inc.
+6C:55:E8,VantivaU Vantiva USA LLC
 6C:56:40,BLUProdu BLU Products Inc
 6C:56:97,AmazonTe Amazon Technologies Inc.
 6C:57:79,"Aclima Aclima, Inc."
 6C:59:40,"MercuryC Mercury Communication Technologies Co.,Ltd."
 6C:59:76,"Shanghai Shanghai Tricheer Technology Co.,Ltd."
 6C:5A:34,"Shenzhen Shenzhen Haitianxiong Electronic Co., Ltd."
 6C:5A:B0,TP-Link TP-Link Corporation Limited
@@ -28135,22 +28691,25 @@
 6C:5E:7A,"Ubiquito Ubiquitous Internet Telecom Co., Ltd"
 6C:5F:1C,LenovoMo Lenovo Mobile Communication Technology Ltd.
 6C:60:D0,"HuaweiDe Huawei Device Co., Ltd."
 6C:60:EB,"ZhiYuanE Zhi Yuan Electronics Co., Limited"
 6C:61:26,RinicomH Rinicom Holdings
 6C:61:F4,Sfr
 6C:62:6D,"Micro-St Micro-Star INT'L CO., LTD"
+6C:62:86,Nokia
 6C:63:9C,"ARRISGro ARRIS Group, Inc."
 6C:64:1A,PenguinC Penguin Computing
 6C:65:67,BELIMOAu BELIMO Automation AG
 6C:67:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
+6C:68:A4,"Guangzho Guangzhou V-Solution Telecommunication Technology Co.,Ltd."
 6C:6A:77,IntelCor Intel Corporate
 6C:6C:0F,"HuaweiTe Huawei Technologies Co.,Ltd"
 6C:6C:D3,"Cisco Cisco Systems, Inc"
 6C:6D:09,"KyowaEle Kyowa Electronics Co.,Ltd."
+6C:6E:07,CeLink Ce Link Limited
 6C:6E:FE,CoreLogi Core Logic Inc.
 6C:6F:18,"Stereota Stereotaxis, Inc."
 6C:70:39,Novar Novar GmbH
 6C:70:9F,"Apple Apple, Inc."
 6C:70:CB,"SamsungE Samsung Electronics Co.,Ltd"
 6C:71:0D,"Cisco Cisco Systems, Inc"
 6C:71:BD,EzelinkT Ezelink Telecom
@@ -28173,14 +28732,15 @@
 6C:8A:EC,"NantongC Nantong Coship Electronics Co., Ltd."
 6C:8B:2F,zte zte corporation
 6C:8B:D3,"Cisco Cisco Systems, Inc"
 6C:8C:DB,OtusTech Otus Technologies Ltd
 6C:8D:65,"Wireless Wireless Glue Networks, Inc."
 6C:8D:77,"Cisco Cisco Systems, Inc"
 6C:8D:C1,"Apple Apple, Inc."
+6C:8F:4E,"Chongqin Chongqing Yipingfang Technology Co., Ltd."
 6C:8F:B5,Microsof Microsoft Mobile Oy
 6C:90:B1,SanLogic SanLogic Inc
 6C:91:06,KatenaCo Katena Computing Technologies
 6C:92:BF,"InspurEl Inspur Electronic Information Industry Co.,Ltd."
 6C:93:08,IEEERegi IEEE Registration Authority
 6C:93:08:00:00:00/28,Braums
 6C:93:08:10:00:00/28,Waterfor Waterford Consultants Llc
@@ -28213,14 +28773,15 @@
 6C:9B:02,Nokia Nokia Corporation
 6C:9B:C0,Chemopti Chemoptics Inc.
 6C:9C:E9,NimbleSt Nimble Storage
 6C:9C:ED,"Cisco Cisco Systems, Inc"
 6C:9E:7C,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 6C:A0:B4,SkyUk Sky Uk Limited
 6C:A1:00,IntelCor Intel Corporate
+6C:A3:67,Avlinkpr Avlinkpro
 6C:A4:01,essensys essensys plc
 6C:A4:D1,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 6C:A6:04,"ARRISGro ARRIS Group, Inc."
 6C:A6:82,EDAMinfo EDAM information & communications
 6C:A7:5F,zte zte corporation
 6C:A7:80,Nokia Nokia Corporation
 6C:A7:FA,YoungboE Youngbo Engineering Inc.
@@ -28231,14 +28792,15 @@
 6C:A9:36,DisplayL DisplayLink (UK) Ltd
 6C:A9:6F,TransPac TransPacket AS
 6C:AA:B3,RuckusWi Ruckus Wireless
 6C:AB:05,"Cisco Cisco Systems, Inc"
 6C:AB:31,"Apple Apple, Inc."
 6C:AB:4D,DigitalP Digital Payment Technologies
 6C:AC:60,Venetex Venetex Corp
+6C:AC:C2,"SamsungE Samsung Electronics Co.,Ltd"
 6C:AD:3F,"HubbellB Hubbell Building Automation, Inc."
 6C:AD:AD,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 6C:AD:EF,"KZBroadb KZ Broadband Technologies, Ltd."
 6C:AD:F8,AzureWav AzureWave Technology Inc.
 6C:AE:8B,IBM IBM Corporation
 6C:AE:E3,Nokia
 6C:AE:F6,eero eero inc.
@@ -28283,14 +28845,15 @@
 6C:D1:99,"vivoMobi vivo Mobile Communication Co., Ltd."
 6C:D1:B0,WingSing Wing Sing Electronics Hong Kong Limited
 6C:D1:E5,"HuaweiTe Huawei Technologies Co.,Ltd"
 6C:D2:BA,zte zte corporation
 6C:D3:EE,Zimi Zimi Corporation
 6C:D6:30,"RootousS Rootous System Co.,Ltd"
 6C:D6:8A,LGElectr LG Electronics (Mobile Communications)
+6C:D6:E3,"Cisco Cisco Systems, Inc"
 6C:D7:04,"HuaweiTe Huawei Technologies Co.,Ltd"
 6C:D7:19,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 6C:D7:1F,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 6C:D8:69,"Guangzho Guangzhou Sat Infrared Co.,LTD"
 6C:D9:4C,"vivoMobi vivo Mobile Communication Co., Ltd."
 6C:DC:6A,Promethe Promethean Limited
 6C:DD:30,"Cisco Cisco Systems, Inc"
@@ -28328,20 +28891,22 @@
 6C:E9:83,"Gastron Gastron Co., LTD."
 6C:EB:B2,"Dongguan Dongguan Sen DongLv Electronics Co.,Ltd"
 6C:EB:B6,"HuaweiTe Huawei Technologies Co.,Ltd"
 6C:EC:5A,"HonHaiPr Hon Hai Precision Ind. CO.,Ltd."
 6C:EC:A1,Shenzhen Shenzhen Clou Electronics Co. Ltd.
 6C:EC:EB,TexasIns Texas Instruments
 6C:ED:51,"NEXCONTR NEXCONTROL Co.,Ltd"
+6C:EE:F7,"shenzhen shenzhen scodeno technology co., Ltd."
 6C:EF:C6,"Shenzhen Shenzhen Twowing Technologies Co.,Ltd."
 6C:F0:49,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 6C:F1:7E,"Zhejiang Zhejiang Uniview Technologies Co.,Ltd."
 6C:F3:73,"SamsungE Samsung Electronics Co.,Ltd"
 6C:F3:7F,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 6C:F5:E8,Mooredol Mooredoll Inc.
+6C:F6:DA,IntelCor Intel Corporate
 6C:F7:12,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 6C:F7:84,XiaomiCo Xiaomi Communications Co Ltd
 6C:F9:7C,Nanoptix Nanoptix Inc.
 6C:F9:D2,"ChengduP Chengdu Povodo Electronic Technology Co., Ltd"
 6C:FA:58,Avaya Avaya Inc
 6C:FA:89,"Cisco Cisco Systems, Inc"
 6C:FA:A7,"AMPAKTec AMPAK Technology, Inc."
@@ -28349,19 +28914,35 @@
 6C:FE:54,IntelCor Intel Corporate
 6C:FF:BE,MPBCommu MPB Communications Inc.
 6C:FF:CE,Sagemcom Sagemcom Broadband SAS
 70:01:36,FATEKAut FATEK Automation Corporation
 70:01:B5,"Cisco Cisco Systems, Inc"
 70:02:58,01Db-Met 01Db-Metravib
 70:03:3F,"PimaxTec Pimax Technology(ShangHai)Co.,Ltd"
-70:03:7E,Technico Technicolor CH USA Inc.
+70:03:7E,VantivaU Vantiva USA LLC
 70:03:9F,Espressi Espressif Inc.
 70:04:1D,Espressi Espressif Inc.
 70:04:33,Californ California Things Inc.
 70:05:14,LGElectr LG Electronics (Mobile Communications)
+70:06:92,IEEERegi IEEE Registration Authority
+70:06:92:00:00:00/28,"Techolog Techology, LLC"
+70:06:92:10:00:00/28,"BeijingF Beijing Fortech Microsystems., Co., Ltd."
+70:06:92:20:00:00/28,"ScudFuji Scud (Fujian) Electronics Co.,Ltd"
+70:06:92:30:00:00/28,"Bosscctv Bosscctv Co., Ltd"
+70:06:92:40:00:00/28,Fusiosto Fusiostor Technologies Private Limited
+70:06:92:50:00:00/28,"CanaanCr Canaan Creative Co.,Ltd."
+70:06:92:60:00:00/28,Hangzhou Hangzhou Clounix Technology Limited
+70:06:92:70:00:00/28,DcnetSol Dcnet Solutions India Pvt Ltd
+70:06:92:80:00:00/28,JMAWirel JMA Wireless
+70:06:92:90:00:00/28,"Shenzhen Shenzhen Lingwei Technology Co., Ltd"
+70:06:92:A0:00:00/28,Munters
+70:06:92:B0:00:00/28,"SWITElec SWIT Electronics Co.,Ltd"
+70:06:92:C0:00:00/28,"ScoreBir ScoreBird, LLC"
+70:06:92:D0:00:00/28,SkywareP Skyware Protech Limited
+70:06:92:E0:00:00/28,Ganghsan Ganghsan Guanglian
 70:06:AC,"Eastcomp Eastcompeace Technology Co., Ltd"
 70:07:77,"OnTarget OnTarget Technologies, Inc"
 70:09:71,"SamsungE Samsung Electronics Co.,Ltd"
 70:0B:01,Sagemcom Sagemcom Broadband SAS
 70:0B:4F,"Cisco Cisco Systems, Inc"
 70:0B:C0,DewavTec Dewav Technology Company
 70:0F:6A,"Cisco Cisco Systems, Inc"
@@ -28372,14 +28953,15 @@
 70:11:0E,zte zte corporation
 70:11:24,"Apple Apple, Inc."
 70:11:35,"Livesecu Livesecu co., Ltd"
 70:11:AE,MusicLif Music Life LTD
 70:14:04,Liabilit Limited Liability Company
 70:14:A6,"Apple Apple, Inc."
 70:16:9F,EtherCAT EtherCAT Technology Group
+70:17:D7,"Shanghai Shanghai Enflame Technology Co., Ltd."
 70:18:8B,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 70:18:A7,"Cisco Cisco Systems, Inc"
 70:19:2F,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:1A:04,LiteonTe Liteon Technology Corporation
 70:1A:B8,IntelCor Intel Corporate
 70:1A:D5,"Openpath Openpath Security, Inc."
 70:1A:ED,"Advas Advas Co., Ltd."
@@ -28409,23 +28991,25 @@
 70:2D:84,i4CInnov i4C Innovations
 70:2D:D1,"NewingsC Newings Communication CO., LTD."
 70:2E:22,zte zte corporation
 70:2E:80,DIEHLCon DIEHL Connectivity Solutions
 70:2E:D9,"Guangzho Guangzhou Shiyuan Electronics Co., Ltd."
 70:2F:35,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:2F:4B,Steelcas Steelcase Inc.
+70:2F:86,Marquard Marquardt GmbH
 70:2F:97,AavaMobi Aava Mobile Oy
 70:30:18,Avaya Avaya Inc
 70:30:5D,Ubiquoss Ubiquoss Inc
 70:30:5E,"NanjingZ Nanjing Zhongke Menglian Information Technology Co.,LTD"
 70:31:7F,"Apple Apple, Inc."
 70:31:87,ACX ACX GmbH
 70:32:17,IntelCor Intel Corporate
 70:32:D5,AthenaWi Athena Wireless Communications Inc
 70:35:09,"Cisco Cisco Systems, Inc"
+70:36:B2,Focusai Focusai Corp
 70:38:11,SiemensM Siemens Mobility Limited
 70:38:B4,LowTechS Low Tech Solutions
 70:38:EE,Avaya Avaya Inc
 70:3A:0E,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 70:3A:2D,"Shenzhen Shenzhen V-Link Technology CO., LTD."
 70:3A:51,XiaomiCo Xiaomi Communications Co Ltd
 70:3A:73,Shenzhen Shenzhen Sundray Technologies Company Limited
@@ -28479,26 +29063,44 @@
 70:50:E7:C0:00:00/28,"shenzhen shenzhen newbridge communication equipment CO.,LTD"
 70:50:E7:D0:00:00/28,EtaCompu Eta Compute Inc.
 70:50:E7:E0:00:00/28,"KfbioKon Kfbio (Konfoong Bioinformation Tech Co.,Ltd)"
 70:52:C5,Avaya Avaya Inc
 70:52:D8,ItelMobi Itel Mobile Limited
 70:53:3F,AlfaInst Alfa Instrumentos Eletronicos Ltda.
 70:54:25,"ARRISGro ARRIS Group, Inc."
+70:54:64,SiliconL Silicon Laboratories
 70:54:B4,VestelEl Vestel Elektronik San ve Tic. A.S.
 70:54:D2,Pegatron Pegatron Corporation
 70:54:F5,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:55:F8,Cerebras Cerebras Systems Inc
 70:56:81,"Apple Apple, Inc."
 70:57:BF,"NewH3CTe New H3C Technologies Co., Ltd"
 70:58:12,Panasoni Panasonic Corporation AVC Networks Company
+70:58:46,TrigAvio Trig Avionics Limited
 70:58:96,InShowTe InShow Technology
 70:59:57,Medallio Medallion Instrumentation Systems
 70:59:86,Ttv Ooo Ttv
 70:5A:0F,HewlettP Hewlett Packard
-70:5A:9E,Technico Technicolor CH USA Inc.
+70:5A:6F,IEEERegi IEEE Registration Authority
+70:5A:6F:00:00:00/28,Thyracon Thyracont Vacuum Instruments GmbH
+70:5A:6F:10:00:00/28,BMRsro BMR s.r.o.
+70:5A:6F:20:00:00/28,Tyromoti Tyromotion GmbH
+70:5A:6F:30:00:00/28,WavelabT Wavelab Telecom Equipment (GZ) Ltd.
+70:5A:6F:40:00:00/28,"Vaiotik Vaiotik Co., Ltd"
+70:5A:6F:50:00:00/28,AcerConn Acer Connect
+70:5A:6F:60:00:00/28,EarfunTe Earfun Technology (HK) Limited
+70:5A:6F:70:00:00/28,WiBASEIn WiBASE Industrial Solutions Inc.
+70:5A:6F:80:00:00/28,"LUANIndu LUAN Industry and Commerce Co., Ltd"
+70:5A:6F:90:00:00/28,Annapurn Annapurna labs
+70:5A:6F:A0:00:00/28,Annapurn Annapurna labs
+70:5A:6F:B0:00:00/28,"Callidus Callidus trading, spol. s r.o."
+70:5A:6F:C0:00:00/28,CoolRGro CoolR Group Inc
+70:5A:6F:D0:00:00/28,PICadvan PICadvanced SA
+70:5A:6F:E0:00:00/28,HallTech Hall Technologies
+70:5A:9E,VantivaU Vantiva USA LLC
 70:5A:AC,"SamsungE Samsung Electronics Co.,Ltd"
 70:5A:B6,"CompalIn Compal Information (Kunshan) Co., Ltd."
 70:5B:2E,M2Commun M2Communication Inc.
 70:5C:AD,KonamiGa Konami Gaming Inc
 70:5D:CC,EFMNetwo EFM Networks
 70:5E:55,RealmeCh Realme Chongqing MobileTelecommunications Corp Ltd
 70:5E:AA,"ActionTa Action Target, Inc."
@@ -28511,14 +29113,15 @@
 70:62:B8,D-LinkIn D-Link International
 70:64:17,OrbisTec Orbis Tecnologia Electrica S.A.
 70:65:82,"SuzhouHa Suzhou Hanming Technologies Co., Ltd."
 70:65:A3,"Kandaoli Kandao lightforge Co., Ltd."
 70:66:1B,Sonova Sonova AG
 70:66:2A,SonyInte Sony Interactive Entertainment Inc.
 70:66:55,AzureWav AzureWave Technology Inc.
+70:66:B9,"HuaweiDe Huawei Device Co., Ltd."
 70:66:E1,dntInnov dnt Innovation GmbH
 70:68:79,"SaijoDen Saijo Denki International Co., Ltd."
 70:69:5A,"Cisco Cisco Systems, Inc"
 70:69:79,IEEERegi IEEE Registration Authority
 70:69:79:00:00:00/28,FullSolu Full Solution Telecom
 70:69:79:10:00:00/28,"LinksysT Linksys Telecom Shenzhen CO., LTD"
 70:69:79:20:00:00/28,Graphcor Graphcore Ltd
@@ -28545,33 +29148,36 @@
 70:70:AA,AmazonTe Amazon Technologies Inc.
 70:70:FC,Gold&Wat Gold&Water Industrial Limited
 70:71:B3,Brain Brain Corporation
 70:71:BC,Pegatron Pegatron Corporation
 70:72:0D,LenovoMo Lenovo Mobile Communication Technology Ltd.
 70:72:3C,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:72:CF,EdgeCore EdgeCore Networks
+70:72:FE,"Apple Apple, Inc."
 70:73:CB,"Apple Apple, Inc."
 70:74:14,"MurataMa Murata Manufacturing Co., Ltd."
 70:76:30,"ARRISGro ARRIS Group, Inc."
 70:76:DD,OxyGuard OxyGuard Internation A/S
 70:76:F0,LevelOne LevelOne Communications (India) Private Limited
 70:76:FF,Kerlink
 70:77:81,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 70:78:8B,"vivoMobi vivo Mobile Communication Co., Ltd."
 70:79:38,"WuxiZhan Wuxi Zhanrui Electronic Technology Co.,LTD"
 70:79:90,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:79:B3,"Cisco Cisco Systems, Inc"
 70:7B:E8,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:7C:18,"ADATATec ADATA Technology Co., Ltd"
 70:7C:69,Avaya Avaya Inc
+70:7C:E3,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:7D:95,Shenzhen Shenzhen City LinwlanTechnology Co. Ltd.
 70:7D:B9,"Cisco Cisco Systems, Inc"
 70:7E:43,"ARRISGro ARRIS Group, Inc."
 70:7E:DE,Nastec Nastec Ltd.
 70:81:05,"Cisco Cisco Systems, Inc"
+70:81:85,"NewH3CTe New H3C Technologies Co., Ltd"
 70:81:EB,"Apple Apple, Inc."
 70:82:0E,aselectr as electronics GmbH
 70:82:8E,OleumTec OleumTech Corporation
 70:85:40,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 70:85:C2,ASRockIn ASRock Incorporation
 70:85:C4,"RuijieNe Ruijie Networks Co.,LTD"
 70:85:C6,"ARRISGro ARRIS Group, Inc."
@@ -28601,17 +29207,19 @@
 70:8C:BB,Mimodisp Mimodisplaykorea
 70:8D:09,Nokia Nokia Corporation
 70:8F:47,"vivoMobi vivo Mobile Communication Co., Ltd."
 70:90:B7,"HuaweiDe Huawei Device Co., Ltd."
 70:91:8F,Weber-St Weber-Stephen Products LLC
 70:91:F3,"Universa Universal Electronics, Inc."
 70:93:83,"Intellig Intelligent Optical Network High Tech CO.,LTD."
+70:93:C1,eero eero inc.
 70:93:F8,"SpaceMon Space Monkey, Inc."
 70:97:41,Arcadyan Arcadyan Corporation
 70:97:56,"Happyele Happyelectronics Co.,Ltd"
+70:98:83,"Shenzhen Shenzhen Kayan Electronics., Ltd."
 70:99:1C,"Shenzhen Shenzhen Honesty Electronics Co.,Ltd"
 70:9A:0B,ItalianI Italian Institute of Technology
 70:9B:A5,"Shenzhen Shenzhen Y&D Electronics Co.,LTD."
 70:9B:FC,Bryton Bryton Inc.
 70:9C:45,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:9C:8F,Nero Nero AG
 70:9C:D1,IntelCor Intel Corporate
@@ -28622,15 +29230,15 @@
 70:A1:91,"Trendset Trendsetter Medical, LLC"
 70:A2:B3,"Apple Apple, Inc."
 70:A4:1C,Advanced Advanced Wireless Dynamics S.L.
 70:A5:6A,"Shenzhen Shenzhen C-Data Technology Co., Ltd."
 70:A6:6A,ProxDyna Prox Dynamics AS
 70:A6:BD,"HonorDev Honor Device Co., Ltd."
 70:A6:CC,IntelCor Intel Corporate
-70:A7:41,Ubiquiti Ubiquiti Networks Inc.
+70:A7:41,Ubiquiti Ubiquiti Inc
 70:A8:4C,"MONAD MONAD., Inc."
 70:A8:D3,IntelCor Intel Corporate
 70:A8:E3,"HuaweiTe Huawei Technologies Co.,Ltd"
 70:A9:83,"Cisco Cisco Systems, Inc"
 70:AA:B2,BlackBer BlackBerry RTS
 70:AC:08,SiliconL Silicon Laboratories
 70:AC:D7,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
@@ -29134,14 +29742,15 @@
 70:B3:D5:1E:50:00/36,VendNova VendNovation LLC
 70:B3:D5:1E:60:00/36,SanminaI Sanmina Israel
 70:B3:D5:1E:70:00/36,DogWatch DogWatch Inc
 70:B3:D5:1E:80:00/36,GogoBA Gogo BA
 70:B3:D5:1E:90:00/36,comtime comtime GmbH
 70:B3:D5:1E:A0:00/36,SenseFor Sense For Innovation
 70:B3:D5:1E:B0:00/36,Xavant
+70:B3:D5:1E:C0:00/36,"CherryLa Cherry Labs, Inc."
 70:B3:D5:1E:D0:00/36,SUS SUS Corporation
 70:B3:D5:1E:E0:00/36,Meggitt
 70:B3:D5:1E:F0:00/36,Adtek
 70:B3:D5:1F:00:00/36,Harmonic Harmonic Design GmbH
 70:B3:D5:1F:10:00/36,DIEHLCon DIEHL Connectivity Solutions
 70:B3:D5:1F:20:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
 70:B3:D5:1F:30:00/36,SmartEne Smart Energy Code Company Limited
@@ -29191,27 +29800,28 @@
 70:B3:D5:21:F0:00/36,Chronome Chronomedia
 70:B3:D5:22:00:00/36,Private
 70:B3:D5:22:10:00/36,LXDesign LX Design House
 70:B3:D5:22:20:00/36,Marioff Marioff Corporation Oy
 70:B3:D5:22:30:00/36,"Research Research Laboratory of Design Automation, Ltd."
 70:B3:D5:22:40:00/36,UrbanaSm Urbana Smart Solutions Pte Ltd
 70:B3:D5:22:50:00/36,RCDRadio RCD Radiokomunikace
-70:B3:D5:22:60:00/36,Yaviar
+70:B3:D5:22:60:00/36,Yaviar Yaviar LLC
 70:B3:D5:22:70:00/36,Montalvo
 70:B3:D5:22:80:00/36,Heitec Heitec Ag
 70:B3:D5:22:90:00/36,CONTROL CONTROL SYSTEMS Srl
 70:B3:D5:22:A0:00/36,"Shishido Shishido Electrostatic, Ltd."
 70:B3:D5:22:B0:00/36,Vitec
 70:B3:D5:22:C0:00/36,HiquelEl Hiquel Elektronik- und Anlagenbau GmbH
 70:B3:D5:22:D0:00/36,LederEle Leder Elektronik Design
 70:B3:D5:22:E0:00/36,Private
 70:B3:D5:22:F0:00/36,"Instec Instec, Inc."
 70:B3:D5:23:00:00/36,CT CT Company
 70:B3:D5:23:10:00/36,"DeltaTau Delta Tau Data Systems, Inc."
 70:B3:D5:23:20:00/36,Uconsys
+70:B3:D5:23:30:00/36,RCHVietn RCH Vietnam Limited Liability Company
 70:B3:D5:23:40:00/36,EDFelect EDFelectronics JRMM Sp z o.o. sp.k.
 70:B3:D5:23:50:00/36,Cameon Cameon S.A.
 70:B3:D5:23:60:00/36,Monnit Monnit Corporation
 70:B3:D5:23:70:00/36,SikomAS Sikom AS
 70:B3:D5:23:80:00/36,AreteAss Arete Associates
 70:B3:D5:23:90:00/36,AppliedS Applied Silver
 70:B3:D5:23:A0:00/36,"MesaLabs Mesa Labs, Inc."
@@ -29233,15 +29843,15 @@
 70:B3:D5:24:A0:00/36,UnmuktiT Unmukti Technology Pvt Ltd
 70:B3:D5:24:B0:00/36,ToseiEng Tosei Engineering Corp.
 70:B3:D5:24:C0:00/36,"Astronom Astronomical Research Cameras, Inc."
 70:B3:D5:24:D0:00/36,InfoCrea Info Creative (Hk) Ltd
 70:B3:D5:24:E0:00/36,"ChengduC Chengdu Cove Technology CO.,LTD"
 70:B3:D5:24:F0:00/36,ElbitBmd Elbit Systems Bmd And Land Ew - Elisra Ltd
 70:B3:D5:25:00:00/36,DatumEle Datum Electronics Limited
-70:B3:D5:25:10:00/36,PixelApp PixelApps s.r.o.
+70:B3:D5:25:10:00/36,"TapHomes Tap Home, s.r.o."
 70:B3:D5:25:20:00/36,SierraNe Sierra Nevada Corporation
 70:B3:D5:25:30:00/36,WimateTe Wimate Technology Solutions Private Limited
 70:B3:D5:25:40:00/36,Spectrum Spectrum Brands
 70:B3:D5:25:50:00/36,Asystems Asystems Corporation
 70:B3:D5:25:60:00/36,TelcoAnt Telco Antennas Pty Ltd
 70:B3:D5:25:70:00/36,LGElectr LG Electronics
 70:B3:D5:25:80:00/36,BAYKONEn BAYKON Endüstriyel Kontrol Sistemleri San. ve Tic. A.Ş.
@@ -29272,15 +29882,15 @@
 70:B3:D5:27:10:00/36,CodeBlue Code Blue Corporation
 70:B3:D5:27:20:00/36,TelecomS Telecom Sante
 70:B3:D5:27:30:00/36,WeVoTech WeVo Tech
 70:B3:D5:27:40:00/36,StercomP Stercom Power Solutions GmbH
 70:B3:D5:27:50:00/36,Internet Internet Protocolo Logica Sl
 70:B3:D5:27:60:00/36,TELLSoft TELL Software Hungaria Kft.
 70:B3:D5:27:70:00/36,Voltawar Voltaware Limited
-70:B3:D5:27:80:00/36,Private
+70:B3:D5:27:80:00/36,"Medicomp Medicomp, Inc"
 70:B3:D5:27:90:00/36,"Medicomp Medicomp, Inc"
 70:B3:D5:27:A0:00/36,TdEcophi Td Ecophisika
 70:B3:D5:27:B0:00/36,Dave Dave Srl
 70:B3:D5:27:C0:00/36,"MOTIONLI MOTION LIB,Inc."
 70:B3:D5:27:D0:00/36,TelenorC Telenor Connexion AB
 70:B3:D5:27:E0:00/36,MettlerT Mettler Toledo
 70:B3:D5:27:F0:00/36,STAerosp ST Aerospace Systems
@@ -29417,14 +30027,15 @@
 70:B3:D5:30:20:00/36,DogWatch DogWatch Inc
 70:B3:D5:30:30:00/36,"FuchuGik Fuchu Giken, Inc."
 70:B3:D5:30:40:00/36,Wartsila Wartsila Voyage Limited
 70:B3:D5:30:50:00/36,CAITRONI CAITRON Industrial Solutions GmbH
 70:B3:D5:30:60:00/36,"Lemz-T Lemz-T, Llc"
 70:B3:D5:30:70:00/36,Energiin Energi innovation Aps
 70:B3:D5:30:80:00/36,"DsdMicro Dsd Microtechnology,Inc."
+70:B3:D5:30:90:00/36,ABSAppli ABS Applied Biometric Systems GmbH
 70:B3:D5:30:A0:00/36,HongSeok HongSeok Ltd.
 70:B3:D5:30:B0:00/36,AshTechn Ash Technologies
 70:B3:D5:30:C0:00/36,Sicon Sicon srl
 70:B3:D5:30:D0:00/36,Fiberbas Fiberbase
 70:B3:D5:30:E0:00/36,Ecolonum Ecolonum Inc.
 70:B3:D5:30:F0:00/36,Cardinal Cardinal Scales Manufacturing Co
 70:B3:D5:31:00:00/36,ConservS Conserv Solutions
@@ -29514,14 +30125,15 @@
 70:B3:D5:36:40:00/36,ADAMCZEW ADAMCZEWSKI elektronische Messtechnik GmbH
 70:B3:D5:36:50:00/36,CircuitM CircuitMeter Inc.
 70:B3:D5:36:60:00/36,"Solarlyt Solarlytics, Inc."
 70:B3:D5:36:70:00/36,LivingWa Living Water
 70:B3:D5:36:80:00/36,WhiteMat White Matter LLC
 70:B3:D5:36:90:00/36,ALVATsro ALVAT s.r.o.
 70:B3:D5:36:A0:00/36,BectonDi Becton Dickinson
+70:B3:D5:36:B0:00/36,HuzElect Huz Electronics Ltd
 70:B3:D5:36:C0:00/36,Sicon Sicon srl
 70:B3:D5:36:D0:00/36,Cybertea Cyberteam Sp z o o
 70:B3:D5:36:E0:00/36,Electrón Electrónica Falcón S.A.U
 70:B3:D5:36:F0:00/36,BuddyGua BuddyGuard GmbH
 70:B3:D5:37:00:00/36,Inphi Inphi Corporation
 70:B3:D5:37:10:00/36,BEDEROV BEDEROV GmbH
 70:B3:D5:37:20:00/36,Matelex
@@ -29543,15 +30155,15 @@
 70:B3:D5:38:20:00/36,NavalGro Naval Group
 70:B3:D5:38:30:00/36,LPAExcil LPA Excil Electronics
 70:B3:D5:38:40:00/36,Sensohiv Sensohive Technologies
 70:B3:D5:38:50:00/36,"KamachoS Kamacho Scale Co., Ltd."
 70:B3:D5:38:60:00/36,GPSat GPSat Systems
 70:B3:D5:38:70:00/36,GWFMessS GWF MessSysteme AG
 70:B3:D5:38:80:00/36,Xitron
-70:B3:D5:38:90:00/36,Private
+70:B3:D5:38:90:00/36,2KLIC 2KLIC inc.
 70:B3:D5:38:A0:00/36,KSE KSE GmbH
 70:B3:D5:38:B0:00/36,LookmanE Lookman Electroplast Industries Ltd
 70:B3:D5:38:C0:00/36,"MiraeSig MiraeSignal Co., Ltd"
 70:B3:D5:38:D0:00/36,Imp-Tele Imp-Telekomunikacije Doo
 70:B3:D5:38:E0:00/36,"ChinaTel China Telecom Fufu Information Technology CO.,LTD"
 70:B3:D5:38:F0:00/36,Sorynory Sorynorydotcom Inc
 70:B3:D5:39:00:00/36,TexCompu Tex Computer Srl
@@ -29687,14 +30299,15 @@
 70:B3:D5:41:20:00/36,Tattile Tattile Srl
 70:B3:D5:41:30:00/36,Axess Axess AG
 70:B3:D5:41:40:00/36,"SmithMet Smith Meter, Inc."
 70:B3:D5:41:50:00/36,Idea Idea Spa
 70:B3:D5:41:60:00/36,Antlia Antlia Systems
 70:B3:D5:41:70:00/36,FigmentD Figment Design Laboratories
 70:B3:D5:41:80:00/36,DEVSyste DEV Systemtechnik GmbH& Co KG
+70:B3:D5:41:90:00/36,ProdataM Prodata Mobility Brasil SA
 70:B3:D5:41:A0:00/36,HYOSUNGH HYOSUNG Heavy Industries Corporation
 70:B3:D5:41:B0:00/36,SYSTECel SYS TEC electronic GmbH
 70:B3:D5:41:C0:00/36,"TwowayCo Twoway Communications, Inc."
 70:B3:D5:41:D0:00/36,AzmoonKe Azmoon Keifiat
 70:B3:D5:41:E0:00/36,RedlerCo Redler Computers
 70:B3:D5:41:F0:00/36,Orion Orion S.r.l.
 70:B3:D5:42:00:00/36,Ecoinet
@@ -29717,14 +30330,15 @@
 70:B3:D5:43:10:00/36,"PowerEle Power Electronics Espana, S.L."
 70:B3:D5:43:20:00/36,DEUTA-WE DEUTA-WERKE GmbH
 70:B3:D5:43:30:00/36,Flexsolu Flexsolution APS
 70:B3:D5:43:40:00/36,Witcom Wit.com Inc
 70:B3:D5:43:50:00/36,"WuhanXin Wuhan Xingtuxinke ELectronic Co.,Ltd"
 70:B3:D5:43:60:00/36,HenrichE Henrich Electronics Corporation
 70:B3:D5:43:70:00/36,DigitalW Digital Way
+70:B3:D5:43:80:00/36,HBIBissc HBI Bisscheroux bv
 70:B3:D5:43:90:00/36,TriLED
 70:B3:D5:43:A0:00/36,"ARKSEnte ARKS Enterprises, Inc."
 70:B3:D5:43:B0:00/36,Kalycito Kalycito Infotech Private Limited
 70:B3:D5:43:C0:00/36,Scenario Scenario Automation
 70:B3:D5:43:D0:00/36,VeryxTec Veryx Technologies Private Limited
 70:B3:D5:43:E0:00/36,PelotonT Peloton Technology
 70:B3:D5:43:F0:00/36,"biosilve biosilver.co.,ltd"
@@ -29877,15 +30491,15 @@
 70:B3:D5:4D:30:00/36,"HefeiSTA Hefei STAROT Technology Co.,Ltd"
 70:B3:D5:4D:40:00/36,NortekGl Nortek Global HVAC
 70:B3:D5:4D:50:00/36,MoogReko Moog Rekofa GmbH
 70:B3:D5:4D:60:00/36,Operatio Operational Technology Solutions
 70:B3:D5:4D:70:00/36,Technolo Technological Ray GmbH
 70:B3:D5:4D:80:00/36,Versilis Versilis Inc.
 70:B3:D5:4D:90:00/36,CodaOcto Coda Octopus Products Limited
-70:B3:D5:4D:A0:00/36,Private
+70:B3:D5:4D:A0:00/36,RADAElec RADA Electronics Industries Ltd.
 70:B3:D5:4D:B0:00/36,Temperat Temperature@lert
 70:B3:D5:4D:C0:00/36,JkDevice Jk Device Corporation
 70:B3:D5:4D:D0:00/36,Velvac Velvac Incorporated
 70:B3:D5:4D:E0:00/36,"OsoTechn Oso Technologies, Inc."
 70:B3:D5:4D:F0:00/36,NidecAvt Nidec Avtron Automation Corp
 70:B3:D5:4E:00:00/36,Microvid Microvideo
 70:B3:D5:4E:10:00/36,GrupoEpe Grupo Epelsa S.L.
@@ -30103,15 +30717,15 @@
 70:B3:D5:5B:50:00/36,LehighEl Lehigh Electric Products Co
 70:B3:D5:5B:60:00/36,EthicalL Ethical Lighting and Sensor Solutions Limited
 70:B3:D5:5B:70:00/36,on on-systems limited
 70:B3:D5:5B:80:00/36,HellaGut Hella Gutmann Solutions GmbH
 70:B3:D5:5B:90:00/36,EizoRugg Eizo Rugged Solutions
 70:B3:D5:5B:A0:00/36,Infrasaf Infrasafe/ Advantor Systems
 70:B3:D5:5B:B0:00/36,OlympusN Olympus NDT Canada
-70:B3:D5:5B:C0:00/36,LAMTECMe LAMTEC Meß- und Regeltechnik für Feuerungen GmbH & Co. KG
+70:B3:D5:5B:C0:00/36,LAMTECMe LAMTEC Mess- und Regeltechnik für Feuerungen GmbH & Co. KG
 70:B3:D5:5B:D0:00/36,nexgenwa nexgenwave
 70:B3:D5:5B:E0:00/36,Caswa
 70:B3:D5:5B:F0:00/36,Aton Aton srl
 70:B3:D5:5C:00:00/36,"Shenzhen Shenzhen Lianfaxun Electronic Technology Co., Ltd"
 70:B3:D5:5C:10:00/36,"Shanghai Shanghai JaWay Information Technology Co., Ltd."
 70:B3:D5:5C:20:00/36,Sono-Tek Sono-Tek Corporation
 70:B3:D5:5C:30:00/36,DIC DIC Corporation
@@ -30415,15 +31029,15 @@
 70:B3:D5:6E:D0:00/36,Wiingtec Wiingtech International Co. LTD.
 70:B3:D5:6E:E0:00/36,"HankookC Hankook Ctec Co,. Ltd."
 70:B3:D5:6E:F0:00/36,Beringar
 70:B3:D5:6F:00:00/36,iTelaSof iTelaSoft Pvt Ltd
 70:B3:D5:6F:10:00/36,Discover Discover Battery
 70:B3:D5:6F:20:00/36,P&CMicro P&C Micro's Pty Ltd
 70:B3:D5:6F:30:00/36,iungo
-70:B3:D5:6F:40:00/36,Private
+70:B3:D5:6F:40:00/36,WDIWiseD WDI Wise Device Inc.
 70:B3:D5:6F:50:00/36,"Cominfo Cominfo, Inc."
 70:B3:D5:6F:60:00/36,AccoBran Acco Brands Europe
 70:B3:D5:6F:70:00/36,Egicon Egicon Srl
 70:B3:D5:6F:80:00/36,SENSEON SENSEON Corporation
 70:B3:D5:6F:90:00/36,ENVItech ENVItech s.r.o.
 70:B3:D5:6F:A0:00/36,Datafort Dataforth Corporation
 70:B3:D5:6F:B0:00/36,Shachiha Shachihata Inc.
@@ -30532,14 +31146,15 @@
 70:B3:D5:76:20:00/36,"Transfor Transformational Security, LLC"
 70:B3:D5:76:30:00/36,"ATrapUSA A Trap, USA"
 70:B3:D5:76:40:00/36,SCHMIDel SCHMID electronic
 70:B3:D5:76:50:00/36,LGElectr LG Electronics
 70:B3:D5:76:60:00/36,Tirasoft Tirasoft Nederland
 70:B3:D5:76:70:00/36,Franklin Franklin France
 70:B3:D5:76:80:00/36,KazanNet Kazan Networks Corporation
+70:B3:D5:76:90:00/36,BarberCr Barber Creations LLC
 70:B3:D5:76:A0:00/36,Swiftnet Swiftnet SOC Ltd
 70:B3:D5:76:B0:00/36,EMPELOR EMPELOR GmbH
 70:B3:D5:76:C0:00/36,Aural Aural Ltd
 70:B3:D5:76:D0:00/36,Trimble
 70:B3:D5:76:E0:00/36,GrupoEpe Grupo Epelsa S.L.
 70:B3:D5:76:F0:00/36,Oti Oti Ltd
 70:B3:D5:77:00:00/36,Strega
@@ -30763,15 +31378,15 @@
 70:B3:D5:84:A0:00/36,MOGLabor MOG Laboratories Pty Ltd
 70:B3:D5:84:B0:00/36,"QuestHou QuestHouse, Inc."
 70:B3:D5:84:C0:00/36,CoreKine CoreKinect
 70:B3:D5:84:D0:00/36,QuantumD Quantum Design Inc.
 70:B3:D5:84:E0:00/36,"Chromalo Chromalox, Inc."
 70:B3:D5:84:F0:00/36,MettlerT Mettler Toledo
 70:B3:D5:85:00:00/36,Reo Reo Ag
-70:B3:D5:85:10:00/36,"EXASCEND EXASCEND (Wuhan) Co., Ltd"
+70:B3:D5:85:10:00/36,"Exascend Exascend, Inc."
 70:B3:D5:85:20:00/36,"NetBoxSC NetBoxSC, LLC"
 70:B3:D5:85:30:00/36,HghSyste Hgh Systemes Infrarouges
 70:B3:D5:85:40:00/36,AdimecAd Adimec Advanced Image Systems
 70:B3:D5:85:50:00/36,Crde
 70:B3:D5:85:60:00/36,Shanghai Shanghai Westwell Information and Technology Company Ltd
 70:B3:D5:85:70:00/36,RchItali Rch Italia Spa
 70:B3:D5:85:80:00/36,HubbellP Hubbell Power Systems
@@ -31459,14 +32074,15 @@
 70:B3:D5:B0:30:00/36,Sprintsh Sprintshield d.o.o.
 70:B3:D5:B0:40:00/36,Herrmann Herrmann Datensysteme GmbH
 70:B3:D5:B0:50:00/36,"E-PlusTe E-Plus Technology Co., Ltd"
 70:B3:D5:B0:60:00/36,Multivoi Multivoice Llc
 70:B3:D5:B0:70:00/36,Arrowval Arrowvale Electronics
 70:B3:D5:B0:80:00/36,Secuinfo Secuinfo Co. Ltd
 70:B3:D5:B0:90:00/36,FirstLig First Light Imaging
+70:B3:D5:B0:A0:00/36,Mitsubis Mitsubishi Electric India Pvt. Ltd.
 70:B3:D5:B0:B0:00/36,Internet Internet Protocolo Logica Sl
 70:B3:D5:B0:C0:00/36,Vigilate Vigilate srl
 70:B3:D5:B0:D0:00/36,Alfi
 70:B3:D5:B0:E0:00/36,Servotro Servotronix Motion Control
 70:B3:D5:B0:F0:00/36,merkurFu merkur Funksysteme AG
 70:B3:D5:B1:00:00/36,ZumbachE Zumbach Electronic AG
 70:B3:D5:B1:10:00/36,Cab Cab S.R.L.
@@ -31498,14 +32114,15 @@
 70:B3:D5:B2:B0:00/36,Vtron Vtron Pty Ltd
 70:B3:D5:B2:C0:00/36,Elman Elman srl
 70:B3:D5:B2:D0:00/36,Plexus
 70:B3:D5:B2:E0:00/36,GreenAcc Green Access Ltd
 70:B3:D5:B2:F0:00/36,HermannA Hermann Automation GmbH
 70:B3:D5:B3:00:00/36,SystoléH Systolé Hardware B.V.
 70:B3:D5:B3:10:00/36,Qwave Qwave Inc
+70:B3:D5:B3:20:00/36,GridBeyo GridBeyond
 70:B3:D5:B3:30:00/36,AplexTec Aplex Technology Inc.
 70:B3:D5:B3:40:00/36,Medtroni Medtronic
 70:B3:D5:B3:50:00/36,"Rexxam Rexxam Co.,Ltd."
 70:B3:D5:B3:60:00/36,Cetitec Cetitec GmbH
 70:B3:D5:B3:70:00/36,"CODEC CODEC Co., Ltd."
 70:B3:D5:B3:80:00/36,GoTrustI GoTrustID Inc.
 70:B3:D5:B3:90:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
@@ -31595,14 +32212,15 @@
 70:B3:D5:B8:E0:00/36,UrFog Ur Fog S.R.L.
 70:B3:D5:B8:F0:00/36,Assembly Assembly Contracts Ltd
 70:B3:D5:B9:00:00/36,Amico Amico Corporation
 70:B3:D5:B9:10:00/36,"Dynetics Dynetics, Inc."
 70:B3:D5:B9:20:00/36,NACommun N A Communications LLC
 70:B3:D5:B9:30:00/36,Internet Internet Protocolo Logica Sl
 70:B3:D5:B9:40:00/36,Cygnetic Cygnetic Technologies (Pty) Ltd
+70:B3:D5:B9:50:00/36,EPIImagi EPIImaging
 70:B3:D5:B9:60:00/36,Oculii
 70:B3:D5:B9:70:00/36,"CanamTec Canam Technology, Inc."
 70:B3:D5:B9:80:00/36,GSFPte GSF Corporation Pte Ltd
 70:B3:D5:B9:90:00/36,DomoSafe DomoSafety S.A.
 70:B3:D5:B9:A0:00/36,PotterEl Potter Electric Signal Co. LLC
 70:B3:D5:B9:B0:00/36,Elektron Elektronik Art
 70:B3:D5:B9:C0:00/36,EDCOTech EDCO Technology 1993 ltd
@@ -31730,15 +32348,15 @@
 70:B3:D5:C1:60:00/36,Southern Southern Innovation
 70:B3:D5:C1:70:00/36,PotterEl Potter Electric Signal Co. LLC
 70:B3:D5:C1:80:00/36,SanminaI Sanmina Israel
 70:B3:D5:C1:90:00/36,ZumbachE Zumbach Electronic AG
 70:B3:D5:C1:A0:00/36,Xylon
 70:B3:D5:C1:B0:00/36,Labinven Labinvent JSC
 70:B3:D5:C1:C0:00/36,DEM D.E.M. Spa
-70:B3:D5:C1:D0:00/36,KranzeTe Kranze Technology Solutions
+70:B3:D5:C1:D0:00/36,"KranzeTe Kranze Technology Solutions, Inc."
 70:B3:D5:C1:E0:00/36,KronMedi Kron Medidores
 70:B3:D5:C1:F0:00/36,BehrTech Behr Technologies Inc
 70:B3:D5:C2:00:00/36,Mipot Mipot S.p.a.
 70:B3:D5:C2:10:00/36,AplexTec Aplex Technology Inc.
 70:B3:D5:C2:20:00/36,Skyriver Skyriver Communications Inc.
 70:B3:D5:C2:30:00/36,"Sumitomo Sumitomo Heavy Industries, Ltd."
 70:B3:D5:C2:40:00/36,ElbitAme Elbit Systems of America
@@ -31818,15 +32436,15 @@
 70:B3:D5:C6:E0:00/36,"OrionTec Orion Technologies, LLC"
 70:B3:D5:C6:F0:00/36,nyantec nyantec GmbH
 70:B3:D5:C7:00:00/36,Magnetek
 70:B3:D5:C7:10:00/36,Engineer The Engineerix Group
 70:B3:D5:C7:20:00/36,ScharcoE Scharco Elektronik GmbH
 70:B3:D5:C7:30:00/36,CDN C.D.N.Corporation
 70:B3:D5:C7:40:00/36,Qtechnol Qtechnology A/S
-70:B3:D5:C7:50:00/36,PlanetIn Planet Innovation (Pi)
+70:B3:D5:C7:50:00/36,PlanetIn Planet Innovation Products Inc.
 70:B3:D5:C7:60:00/36,ElaInnov Ela Innovation
 70:B3:D5:C7:70:00/36,YönnetAk Yönnet Akıllı Bina ve Otomasyon Sistemleri
 70:B3:D5:C7:80:00/36,NETAElek NETA Elektronik AS
 70:B3:D5:C7:90:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 70:B3:D5:C7:A0:00/36,"ENTECEle ENTEC Electric & Electronic Co., LTD."
 70:B3:D5:C7:B0:00/36,EMClarit EM Clarity Pty Ltd
 70:B3:D5:C7:C0:00/36,"BeijingA Beijing Aumiwalker technology CO.,LTD"
@@ -32413,15 +33031,15 @@
 70:B3:D5:EC:10:00/36,XafaxNed Xafax Nederland bv
 70:B3:D5:EC:20:00/36,Lightsid Lightside Instruments AS
 70:B3:D5:EC:30:00/36,VirtualC Virtual Control Systems Ltd
 70:B3:D5:EC:40:00/36,hmttelem hmt telematik GmbH
 70:B3:D5:EC:50:00/36,Tattile Tattile Srl
 70:B3:D5:EC:60:00/36,Esii
 70:B3:D5:EC:70:00/36,Neoptix Neoptix Inc.
-70:B3:D5:EC:80:00/36,Panasoni Panasonic Life Solutions Elektri̇k Sanayi̇ Ve Ti̇care
+70:B3:D5:EC:80:00/36,Panasoni Panasonic Life Solutions Elektr?K Sanay? Ve T?Care
 70:B3:D5:EC:90:00/36,QlinxTec Qlinx Technologies
 70:B3:D5:EC:A0:00/36,Transtro Transtronic AB
 70:B3:D5:EC:B0:00/36,Re-Contr Re spa - Controlli Industriali - IT01782300154
 70:B3:D5:EC:C0:00/36,Digifocu Digifocus Technology Inc.
 70:B3:D5:EC:D0:00/36,SBS-Fein SBS-Feintechnik GmbH & Co. KG
 70:B3:D5:EC:E0:00/36,COMM-con COMM-connect A/S
 70:B3:D5:EC:F0:00/36,Ipitek
@@ -32501,14 +33119,15 @@
 70:B3:D5:F1:90:00/36,VitroTec Vitro Technology Corporation
 70:B3:D5:F1:A0:00/36,SatorCon Sator Controls s.r.o.
 70:B3:D5:F1:B0:00/36,IndiNatu IndiNatus (IndiNatus India Private Limited)
 70:B3:D5:F1:C0:00/36,BavariaD Bavaria Digital Technik GmbH
 70:B3:D5:F1:D0:00/36,Critical Critical Link LLC
 70:B3:D5:F1:E0:00/36,AtxNetwo Atx Networks Ltd
 70:B3:D5:F1:F0:00/36,HKCSecur HKC Security Ltd.
+70:B3:D5:F2:00:00/36,Ibercomp Ibercomp SA
 70:B3:D5:F2:10:00/36,dds
 70:B3:D5:F2:20:00/36,ShengliF Shengli Financial Software Development
 70:B3:D5:F2:30:00/36,LyseAS Lyse AS
 70:B3:D5:F2:40:00/36,Daavlin
 70:B3:D5:F2:50:00/36,"“Scienti JSC “Scientific Industrial Enterprise ""Rubin"""
 70:B3:D5:F2:60:00/36,"XjElectr Xj Electric Co., Ltd."
 70:B3:D5:F2:70:00/36,"NIRIT-Xi NIRIT- Xinwei Telecom Technology Co., Ltd."
@@ -32719,21 +33338,23 @@
 70:B3:D5:FF:40:00/36,Serveron Serveron Corporation
 70:B3:D5:FF:50:00/36,ProlanPr Prolan Process Control Co.
 70:B3:D5:FF:60:00/36,ElektroA Elektro Adrian
 70:B3:D5:FF:70:00/36,Cybercom Cybercom AB
 70:B3:D5:FF:80:00/36,"DutileGl Dutile, Glines and Higgins Corporation"
 70:B3:D5:FF:90:00/36,InOutCom InOut Communication Systems
 70:B3:D5:FF:A0:00/36,Barracud Barracuda Measurement Solutions
+70:B3:D5:FF:B0:00/36,"QuercusT Quercus Technologies, S.L."
 70:B3:D5:FF:C0:00/36,Symetric Symetrics Industries d.b.a. Extant Aerospace
 70:B3:D5:FF:D0:00/36,i2System i2Systems
 70:B3:D5:FF:E0:00/36,Private
 70:B3:D5:FF:F0:00/36,Private
 70:B5:99,Embedded Embedded Technologies s.r.o.
 70:B5:E8,Dell Dell Inc.
 70:B6:4F,"Guangzho Guangzhou V-SOLUTION Electronic Technology Co., Ltd."
+70:B6:51,EightSle Eight Sleep
 70:B7:AA,"vivoMobi vivo Mobile Communication Co., Ltd."
 70:B7:E2,"JiangsuM Jiangsu Miter Technology Co.,Ltd."
 70:B7:E4,Broadcom Broadcom Limited
 70:B8:F6,Espressi Espressif Inc.
 70:B9:21,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 70:B9:50,TexasIns Texas Instruments
 70:B9:BB,"Shenzhen Shenzhen Hankvision Technology CO.,LTD"
@@ -32763,14 +33384,15 @@
 70:D3:79,"Cisco Cisco Systems, Inc"
 70:D4:F2,Rim
 70:D5:7E,Scalar Scalar Corporation
 70:D5:E7,Wellcore Wellcore Corporation
 70:D6:B6,MetrumTe Metrum Technologies
 70:D8:23,IntelCor Intel Corporate
 70:D8:80,UposSyst Upos System sp. z o.o.
+70:D8:C2,IntelCor Intel Corporate
 70:D9:23,"vivoMobi vivo Mobile Communication Co., Ltd."
 70:D9:31,"Cambridg Cambridge Industries(Group) Co.,Ltd."
 70:DA:17,Austrian Austrian Audio GmbH
 70:DA:9C,Tecsen
 70:DB:98,"Cisco Cisco Systems, Inc"
 70:DD:A1,Tellabs
 70:DD:A8,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -32781,14 +33403,15 @@
 70:DF:F7,"ARRISGro ARRIS Group, Inc."
 70:E0:27,HongyuCo Hongyu Communication Technology Limited
 70:E1:39,3view 3view Ltd
 70:E1:FD,Flextron Flextronics
 70:E2:4C,SAEIT SAE IT-systems GmbH & Co. KG
 70:E2:84,WistronI Wistron Infocomm (Zhongshan) Corporation
 70:E4:22,"Cisco Cisco Systems, Inc"
+70:E4:6E,Lytx
 70:E5:6E,TexasIns Texas Instruments
 70:E7:2C,"Apple Apple, Inc."
 70:E8:43,"BeijingC Beijing C&W Optical Communication Technology Co.,Ltd."
 70:EA:1A,"Cisco Cisco Systems, Inc"
 70:EA:5A,"Apple Apple, Inc."
 70:EC:E4,"Apple Apple, Inc."
 70:EE:50,Netatmo
@@ -32803,14 +33426,15 @@
 70:F1:A1,LiteonTe Liteon Technology Corporation
 70:F1:E5,Xetawave Xetawave LLC
 70:F2:20,"Actionte Actiontec Electronics, Inc"
 70:F3:5A,"Cisco Cisco Systems, Inc"
 70:F3:95,"Universa Universal Global Scientific Industrial Co., Ltd."
 70:F7:54,"AMPAKTec AMPAK Technology,Inc."
 70:F8:2B,DWnetTec DWnet Technologies(Suzhou) Corporation
+70:F8:AE,Microsof Microsoft Corporation
 70:F8:E7,IEEERegi IEEE Registration Authority
 70:F8:E7:00:00:00/28,SHENZHEN SHENZHEN Xin JiuNing Electronics Co Ltd
 70:F8:E7:10:00:00/28,SystemLe System Level Solutions (India) Pvt.
 70:F8:E7:20:00:00/28,VOXXInte VOXX International
 70:F8:E7:30:00:00/28,DrSimonC Dr. Simon Consulting GmbH
 70:F8:E7:40:00:00/28,CLIP CLIP Inc.
 70:F8:E7:50:00:00/28,"BeijingE Beijing Eehuu Technology Co.,Ltd."
@@ -32847,14 +33471,15 @@
 74:11:B2,"Cisco Cisco Systems, Inc"
 74:12:B3,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 74:12:BB,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 74:13:EA,IntelCor Intel Corporate
 74:14:89,SRTWirel SRT Wireless
 74:15:75,XiaomiCo Xiaomi Communications Co Ltd
 74:15:E2,Tri-Sen Tri-Sen Systems Corporation
+74:15:F5,"Apple Apple, Inc."
 74:18:65,"Shanghai Shanghai DareGlobal Technologies Co.,Ltd"
 74:19:0A,"SamsungE Samsung Electronics Co.,Ltd"
 74:19:F8,IEEERegi IEEE Registration Authority
 74:19:F8:00:00:00/28,Marmitek
 74:19:F8:10:00:00/28,"Trend-te Trend-tech Technology Co., Limited"
 74:19:F8:20:00:00/28,SymtopIn Symtop Instrument Co.
 74:19:F8:30:00:00/28,Essentia Essential Trading Systems Corp
@@ -32893,42 +33518,45 @@
 74:1F:79,"Youngkoo Youngkook Electronics Co.,Ltd"
 74:22:BB,"HuaweiDe Huawei Device Co., Ltd."
 74:23:44,XiaomiCo Xiaomi Communications Co Ltd
 74:24:9F,TIBRO TIBRO Corp.
 74:25:8A,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 74:26:AC,"Cisco Cisco Systems, Inc"
 74:26:FF,zte zte corporation
+74:27:2C,"Advanced Advanced Micro Devices, Inc."
 74:27:3C,"ChangYan ChangYang Technology (Nanjing) Co., LTD"
 74:27:EA,"Elitegro Elitegroup Computer Systems Co.,Ltd."
 74:28:57,Mayfield Mayfield Robotics
 74:29:AF,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 74:2A:8A,"shenzhen shenzhen worldelite electronics co., LTD"
 74:2B:0F,Infinida Infinidat Ltd.
 74:2B:62,Fujitsu Fujitsu Limited
 74:2D:0A,NorfolkE Norfolk Elektronik AG
 74:2E:DB,Perinet Perinet GmbH
 74:2E:FC,"DirectPa DirectPacket Research, Inc,"
 74:2F:68,AzureWav AzureWave Technology Inc.
+74:30:AF,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 74:31:70,Arcadyan Arcadyan Technology Corporation
 74:31:74,"Apple Apple, Inc."
 74:32:56,NT-wareS NT-ware Systemprg GmbH
 74:32:C2,Kyolis
+74:33:57,"vivoMobi vivo Mobile Communication Co., Ltd."
 74:33:A6,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 74:34:00,"MTG MTG Co., Ltd."
 74:34:2B,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:34:AE,thisisen this is engineering Inc.
 74:36:6D,Vodafone Vodafone Italia S.p.A.
 74:37:2F,"Tongfang Tongfang Shenzhen Cloudcomputing Technology Co.,Ltd"
 74:37:3B,"UNINET UNINET Co.,Ltd."
 74:37:5F,SercommP Sercomm Philippines Inc
 74:38:89,ANNAXAnz ANNAX Anzeigesysteme GmbH
 74:38:B7,Canon Canon Inc.
 74:3A:20,"NewH3CTe New H3C Technologies Co., Ltd"
 74:3A:65,NEC NEC Corporation
-74:3A:EF,"Kaonmedi Kaonmedia CO., LTD."
+74:3A:EF,"KaonGrou Kaon Group Co., Ltd."
 74:3A:F4,IntelCor Intel Corporate
 74:3C:18,TaicangT Taicang T&W Electronics
 74:3E:2B,RuckusWi Ruckus Wireless
 74:3E:39,"YUSURTec YUSUR Technology Co., Ltd."
 74:3E:CB,Gentrice Gentrice tech
 74:3F:C2,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 74:40:BB,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
@@ -32938,25 +33566,27 @@
 74:44:01,Netgear
 74:45:2D,"HuaweiDe Huawei Device Co., Ltd."
 74:45:8A,"SamsungE Samsung Electronics Co.,Ltd"
 74:45:CE,Cresyn
 74:46:87,"Kingsign Kingsignal Technology Co., Ltd."
 74:46:A0,HewlettP Hewlett Packard
 74:46:B3,TexasIns Texas Instruments
+74:49:D2,"NewH3CTe New H3C Technologies Co., Ltd"
 74:4A:A4,zte zte corporation
 74:4B:E9,"Explorer Explorer Hypertech Co.,Ltd"
 74:4C:A1,LiteonTe Liteon Technology Corporation
 74:4D:28,Routerbo Routerboard.com
 74:4D:6D,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:4D:79,Arrive Arrive Systems Inc.
 74:50:4E,"NewH3CTe New H3C Technologies Co., Ltd"
 74:51:BA,XiaomiCo Xiaomi Communications Co Ltd
 74:53:27,"Commsen Commsen Co., Limited"
 74:53:A8,ACLAirsh ACL Airshop BV
 74:54:27,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
+74:54:6B,"hangzhou hangzhou zhiyi communication co., ltd"
 74:54:7D,CiscoSPV Cisco SPVTG
 74:56:12,"ARRISGro ARRIS Group, Inc."
 74:56:3C,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 74:57:98,TRUMPFLa TRUMPF Laser GmbH + Co. KG
 74:58:89,Multilas Multilaser Industrial S.A.
 74:58:F3,AmazonTe Amazon Technologies Inc.
 74:59:09,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -32977,21 +33607,22 @@
 74:5B:C5:B0:00:00/28,Smartipl Smartiply Inc.
 74:5B:C5:C0:00:00/28,ComNot
 74:5B:C5:D0:00:00/28,CelyssSa Celyss Sas
 74:5B:C5:E0:00:00/28,"QingdaoW Qingdao Wintec System Co., Ltd"
 74:5C:4B,GNAudio GN Audio A/S
 74:5C:9F,TCTmobil TCT mobile ltd
 74:5C:FA,"Shenzhen Shenzhen Shunrui Gaojie Technology Co., Ltd."
+74:5D:22,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 74:5D:43,BSHHausg BSH Hausgeraete GmbH
 74:5D:68,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 74:5E:1C,Pioneer Pioneer Corporation
 74:5F:00,SamsungS Samsung Semiconductor Inc.
 74:5F:90,LAMTechn LAM Technologies
 74:5F:AE,TslPpl Tsl Ppl
-74:60:4C,Røde
+74:60:4C,Rode
 74:60:FA,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:61:4B,"Chongqin Chongqing Huijiatong Information Technology Co., Ltd."
 74:63:C2,"HuaweiDe Huawei Device Co., Ltd."
 74:63:DF,VTS VTS GmbH
 74:65:0C,"Apple Apple, Inc."
 74:65:D1,Atlinks
 74:66:30,TmiYtti T:mi Ytti
@@ -33011,39 +33642,42 @@
 74:70:FD,IntelCor Intel Corporate
 74:71:8B,"Apple Apple, Inc."
 74:72:1E,EdisonLa Edison Labs Inc.
 74:72:B0,"Guangzho Guangzhou Shiyuan Electronics Co., Ltd."
 74:72:F2,"ChipsipT Chipsip Technology Co., Ltd."
 74:73:1D,ifmelect ifm electronic gmbh
 74:73:36,MICRODIG MICRODIGTAL Inc
+74:73:B4,"Apple Apple, Inc."
 74:74:46,"Google Google, Inc."
 74:75:48,AmazonTe Amazon Technologies Inc.
 74:76:5B,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 74:76:7D,"shenzhen shenzhen kexint technology co.,ltd"
 74:78:18,Jurumani Jurumani Solutions
 74:78:27,Dell Dell Inc.
+74:78:A6,"Fortinet Fortinet, Inc."
 74:7A:90,"MurataMa Murata Manufacturing Co., Ltd."
 74:7B:7A,ETH ETH Inc.
 74:7D:24,"PhicommS Phicomm (Shanghai) Co., Ltd."
 74:7D:B6,"AliweiCo Aliwei Communications, Inc"
 74:7E:1A,RedEmbed Red Embedded Design Limited
 74:7E:2D,BeijingT Beijing Thomson CITIC Digital Technology Co. LTD.
 74:80:3F,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 74:81:14,"Apple Apple, Inc."
 74:81:9A,PTHarton PT. Hartono Istana Teknologi
-74:83:C2,Ubiquiti Ubiquiti Networks Inc.
+74:83:C2,Ubiquiti Ubiquiti Inc
 74:83:EF,AristaNe Arista Networks
 74:84:69,"Nintendo Nintendo Co.,Ltd"
 74:84:E1,"Dongguan Dongguan Haoyuan Electronics Co.,Ltd"
 74:85:2A,Pegatron Pegatron Corporation
 74:85:C4,"NewH3CTe New H3C Technologies Co., Ltd"
 74:86:0B,"Cisco Cisco Systems, Inc"
 74:86:69,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 74:86:7A,Dell Dell Inc.
 74:86:E2,Dell Dell Inc.
+74:87:2E,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:87:A9,"OCTTechn OCT Technology Co., Ltd."
 74:87:BB,Ciena Ciena Corporation
 74:88:2A,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:88:8B,ADBBroad ADB Broadband Italia
 74:88:BB,"Cisco Cisco Systems, Inc"
 74:8A:0D,"ARRISGro ARRIS Group, Inc."
 74:8A:28,HMDGloba HMD Global Oy
@@ -33052,26 +33686,30 @@
 74:8B:34,"Shanghai Shanghai Smart System Technology Co., Ltd"
 74:8D:08,"Apple Apple, Inc."
 74:8E:08,Bestek Bestek Corp.
 74:8E:F8,BrocadeC Brocade Communications Systems LLC
 74:8F:1B,MasterIm MasterImage 3D
 74:8F:3C,"Apple Apple, Inc."
 74:8F:4D,duagonGe duagon Germany GmbH
+74:8F:C2,"Cisco Cisco Systems, Inc"
 74:90:1F,RagileNe Ragile Networks Inc.
 74:90:50,RenesasE Renesas Electronics Corporation
 74:91:1A,RuckusWi Ruckus Wireless
 74:91:BD,"Four Four systems Co.,Ltd."
+74:92:BA,Movesens Movesense Ltd
 74:93:A4,ZebraTec Zebra Technologies Corp.
 74:93:DA,AskeyCom Askey Computer Corp
 74:94:3D,AgJuncti AgJunction
 74:95:52,"XuzhouWI Xuzhou WIKA Electronics Control Technology Co., Ltd."
+74:95:A7,Keyence Keyence Corporation
 74:95:EC,"Alpsalpi Alpsalpine Co,.Ltd"
 74:96:37,"TodaairE Todaair Electronic Co., Ltd"
 74:97:79,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 74:97:81,zte zte corporation
+74:97:8E,NovaLabs Nova Labs
 74:99:75,IBM IBM Corporation
 74:9A:C0,"Cachengo Cachengo, Inc."
 74:9B:E8,HitronTe Hitron Technologies. Inc
 74:9C:52,"HuizhouD Huizhou Desay SV Automotive Co., Ltd."
 74:9C:E3,"KodaClou KodaCloud Canada, Inc"
 74:9D:79,Sercomm Sercomm Corporation.
 74:9D:8F,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -33083,45 +33721,48 @@
 74:A0:2F,"Cisco Cisco Systems, Inc"
 74:A0:63,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:A2:E6,"Cisco Cisco Systems, Inc"
 74:A3:4A,Zimi Zimi Corporation
 74:A4:A7,"QRSMusic QRS Music Technologies, Inc."
 74:A4:B5,Powerlea Powerleader Science and Technology Co. Ltd.
 74:A5:28,"HuaweiTe Huawei Technologies Co.,Ltd"
+74:A5:8C,TexasIns Texas Instruments
 74:A6:CD,"Apple Apple, Inc."
 74:A7:22,LGElectr LG Electronics (Mobile Communications)
 74:A7:8E,zte zte corporation
 74:A7:EA,AmazonTe Amazon Technologies Inc.
 74:AB:93,BlinkbyA Blink by Amazon
 74:AC:5F,"QikuInte Qiku Internet Network Scientific (Shenzhen) Co., Ltd."
-74:AC:B9,Ubiquiti Ubiquiti Networks Inc.
+74:AC:B9,Ubiquiti Ubiquiti Inc
 74:AD:98,"Cisco Cisco Systems, Inc"
 74:AD:B7,"ChinaMob China Mobile Group Device Co.,Ltd."
 74:AE:76,"iNovoBro iNovo Broadband, Inc."
 74:B0:0C,"NetworkV Network Video Technologies, Inc"
 74:B4:72,Ciesse
 74:B5:7E,zte zte corporation
 74:B5:87,"Apple Apple, Inc."
 74:B6:B6,eero eero inc.
 74:B7:25,"HuaweiDe Huawei Device Co., Ltd."
 74:B7:B3,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 74:B7:E6,Zegna-Da Zegna-Daidong Limited
+74:B8:0F,ZiplineI Zipline International Inc.
 74:B8:39,TexasIns Texas Instruments
 74:B9:1E,"NanjingB Nanjing Bestway Automation System Co., Ltd"
 74:B9:EB,"JinQianM JinQianMao Technology Co.,Ltd."
 74:BA:DB,"Longconn Longconn Electornics(shenzhen)Co.,Ltd"
 74:BB:D3,"Shenzhen Shenzhen xeme Communication Co., Ltd."
 74:BE:08,"ATEKProd ATEK Products, LLC"
 74:BF:A1,Hyunteck
 74:BF:B7,Nusoft Nusoft Corporation
 74:BF:C0,Canon Canon Inc.
 74:C1:4F,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:C1:7D,Infinixm Infinix mobility limited
 74:C2:46,AmazonTe Amazon Technologies Inc.
 74:C3:30,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
+74:C5:30,"vivoMobi vivo Mobile Communication Co., Ltd."
 74:C6:21,"Zhejiang Zhejiang Hite Renewable Energy Co.,LTD"
 74:C6:3B,AzureWav AzureWave Technology Inc.
 74:C9:29,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 74:C9:9A,Ericsson Ericsson AB
 74:C9:A3,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 74:CA:25,"Calxeda Calxeda, Inc."
 74:CB:F3,Lavainte Lava international limited
@@ -33132,21 +33773,23 @@
 74:D0:2B,ASUSTekC ASUSTek COMPUTER INC.
 74:D0:DC,Ericsson Ericsson AB
 74:D2:1D,"HuaweiTe Huawei Technologies Co.,Ltd"
 74:D2:85,TexasIns Texas Instruments
 74:D4:23,AmazonTe Amazon Technologies Inc.
 74:D4:35,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 74:D4:DD,QuantaCo Quanta Computer Inc.
+74:D5:58,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 74:D6:37,AmazonTe Amazon Technologies Inc.
 74:D6:54,Gint
 74:D6:75,WYMATecn WYMA Tecnologia
 74:D6:CB,"NewH3CTe New H3C Technologies Co., Ltd"
+74:D6:E5,"HuaweiDe Huawei Device Co., Ltd."
 74:D6:EA,TexasIns Texas Instruments
-74:D7:13,"HuaqinTe Huaqin Technology Co.,Ltd"
-74:D7:CA,Panasoni Panasonic Corporation Automotive
+74:D7:13,HuaqinTe Huaqin Technology Co. LTD
+74:D7:CA,"Panasoni Panasonic Automotive Systems Co.,Ltd"
 74:D8:3E,IntelCor Intel Corporate
 74:D8:50,Evrisko Evrisko Systems
 74:D8:73,"Guangdon Guangdong Genius Technology Co., Ltd."
 74:D9:EB,"PetabitS Petabit Scale, Inc."
 74:DA:38,EdimaxTe Edimax Technology Co. Ltd.
 74:DA:88,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 74:DA:DA,D-LinkIn D-Link International
@@ -33197,14 +33840,15 @@
 74:EA:CB,"NewH3CTe New H3C Technologies Co., Ltd"
 74:EA:E8,"ARRISGro ARRIS Group, Inc."
 74:EB:80,"SamsungE Samsung Electronics Co.,Ltd"
 74:EC:42,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 74:EC:B2,AmazonTe Amazon Technologies Inc.
 74:EC:F1,Acumen
 74:EE:2A,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
+74:EE:8D,"ApolloIn Apollo Intelligent Connectivity (Beijing) Technology Co., Ltd."
 74:EF:4B,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 74:F0:6D,AzureWav AzureWave Technology Inc.
 74:F0:7D,"BnCOM BnCOM Co.,Ltd"
 74:F1:02,"BeijingH Beijing HCHCOM Technology Co., Ltd"
 74:F2:FA,XiaomiCo Xiaomi Communications Co Ltd
 74:F4:13,MaxwellF Maxwell Forest
 74:F6:12,"ARRISGro ARRIS Group, Inc."
@@ -33305,19 +33949,21 @@
 78:24:AF,ASUSTekC ASUSTek COMPUTER INC.
 78:25:44,Omnima Omnima Limited
 78:25:7A,LEOInnov LEO Innovation Lab
 78:25:AD,"SamsungE Samsung Electronics Co.,Ltd"
 78:28:CA,"Sonos Sonos, Inc."
 78:29:ED,AskeyCom Askey Computer Corp
 78:2A:79,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
+78:2A:F8,"IethcomI Iethcom Information Technology Co., Ltd."
 78:2B:46,IntelCor Intel Corporate
 78:2B:64,Bose Bose Corporation
 78:2B:CB,Dell Dell Inc.
 78:2C:29,"NewH3CTe New H3C Technologies Co., Ltd"
 78:2D:7E,"TRENDnet TRENDnet, Inc."
+78:2D:AD,"HuaweiTe Huawei Technologies Co.,Ltd"
 78:2E:56,"ChinaMob China Mobile Group Device Co.,Ltd."
 78:2E:EF,Nokia Nokia Corporation
 78:2F:17,"Xlab Xlab Co.,Ltd"
 78:30:3B,"StephenT Stephen Technologies Co.,Limited"
 78:30:E1,"UltraCle UltraClenz, LLC"
 78:30:F5,TBT TBT Inc.
 78:31:2B,zte zte corporation
@@ -33339,18 +33985,19 @@
 78:3F:15,EasySYNC EasySYNC Ltd.
 78:40:E4,"SamsungE Samsung Electronics Co.,Ltd"
 78:44:05,"FUJITUHO FUJITU(HONG KONG) ELECTRONIC Co.,LTD."
 78:44:4A,"Shenzhen Shenzhen Aiwinn information Technology Co., Ltd."
 78:44:76,ZioncomE Zioncom Electronics (Shenzhen) Ltd.
 78:44:FD,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 78:45:01,Biamp Biamp Systems
-78:45:58,Ubiquiti Ubiquiti Networks Inc.
+78:45:58,Ubiquiti Ubiquiti Inc
 78:45:61,CyberTAN CyberTAN Technology Inc.
 78:45:B3,"HuaweiDe Huawei Device Co., Ltd."
 78:45:C4,Dell Dell Inc.
+78:46:5C,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 78:46:C4,DaehapHy Daehap Hyper-Tech
 78:46:D4,"SamsungE Samsung Electronics Co.,Ltd"
 78:47:1D,"SamsungE Samsung Electronics Co.,Ltd"
 78:47:E3,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 78:48:2C,"StartUsa Start Usa, Inc."
 78:48:59,HewlettP Hewlett Packard
 78:49:1D,Will-Bur The Will-Burt Company
@@ -33411,14 +34058,15 @@
 78:64:E6,GreenMot Green Motive Technology Limited
 78:65:3B,"Shaoxing Shaoxing Ourten Electronics Co., Ltd."
 78:65:59,Sagemcom Sagemcom Broadband SAS
 78:66:9D,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 78:66:AE,"ZTECInst ZTEC Instruments, Inc."
 78:67:0E,WistronN Wistron Neweb Corporation
 78:67:D7,"Apple Apple, Inc."
+78:68:29,eero eero inc.
 78:68:F7,"YSTenTec YSTen Technology Co.,Ltd"
 78:69:D4,Shenyang Shenyang Vibrotech Instruments Inc.
 78:6A:1F,"ARRISGro ARRIS Group, Inc."
 78:6A:89,"HuaweiTe Huawei Technologies Co.,Ltd"
 78:6C:1C,"Apple Apple, Inc."
 78:6C:84,AmazonTe Amazon Technologies Inc.
 78:6D:94,PaloAlto Palo Alto Networks
@@ -33460,20 +34108,22 @@
 78:84:EE,IndraEsp Indra Espacio S.A.
 78:85:F4,"HuaweiDe Huawei Device Co., Ltd."
 78:86:B6,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 78:87:0D,Unifiedg Unifiedgateways India Private Limited
 78:88:6D,"Apple Apple, Inc."
 78:88:8A,CDRSpSpk CDR Sp. z o.o. Sp. k.
 78:89:73,Cmc
-78:8A:20,Ubiquiti Ubiquiti Networks Inc.
+78:8A:20,Ubiquiti Ubiquiti Inc
+78:8A:86,ChinaDra China Dragon Technology Limited
 78:8B:2A,"ZhenShiI Zhen Shi Information Technology (Shanghai) Co., Ltd."
 78:8B:77,StandarT Standar Telecom
 78:8C:4D,"IndymeSo Indyme Solutions, LLC"
 78:8C:54,PingComm Ping Communication
 78:8C:77,"LexmarkI Lexmark International, Inc."
+78:8C:B5,TP-Link TP-Link Corporation Limited
 78:8D:F7,HitronTe Hitron Technologies. Inc
 78:8E:33,"JiangsuS Jiangsu SEUIC Technology Co.,Ltd"
 78:90:A2,zte zte corporation
 78:91:DE,"Guangdon Guangdong ACIGA Science&Technology Co.,Ltd"
 78:91:E9,"Raisecom Raisecom Technology CO.,LTD"
 78:92:3E,Nokia Nokia Corporation
 78:92:9C,IntelCor Intel Corporate
@@ -33488,14 +34138,15 @@
 78:98:FD,Q9Networ Q9 Networks Inc.
 78:99:5C,NationzT Nationz Technologies Inc
 78:99:66,"MusilabE Musilab Electronics (DongGuan)Co.,Ltd."
 78:99:8F,Mediline Mediline Italia Srl
 78:9C:85,"AugustHo August Home, Inc."
 78:9C:E7,"Shenzhen Shenzhen Aikede Technology Co., Ltd"
 78:9E:D0,"SamsungE Samsung Electronics Co.,Ltd"
+78:9F:38,"Shenzhen Shenzhen Feasycom Co., Ltd"
 78:9F:4C,HOERBIGE HOERBIGER Elektronik GmbH
 78:9F:70,"Apple Apple, Inc."
 78:9F:87,SiemensI Siemens AG I IA PP PRM
 78:9F:AA,"HuaweiDe Huawei Device Co., Ltd."
 78:A0:3F,AmazonTe Amazon Technologies Inc.
 78:A0:51,iiNetLab iiNet Labs Pty Ltd
 78:A1:06,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
@@ -33657,14 +34308,15 @@
 78:DB:2F,TexasIns Texas Instruments
 78:DD:08,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 78:DD:12,Arcadyan Arcadyan Corporation
 78:DD:33,"HuaweiTe Huawei Technologies Co.,Ltd"
 78:DD:D6,c-scape
 78:DD:D9,"Guangzho Guangzhou Shiyuan Electronics Co., Ltd."
 78:DE:E4,TexasIns Texas Instruments
+78:DF:72,Shanghai Shanghai Imilab Technology Co.Ltd
 78:E1:03,AmazonTe Amazon Technologies Inc.
 78:E2:2C,"HuaweiDe Huawei Device Co., Ltd."
 78:E2:BD,Vodafone Vodafone Automotive S.p.A.
 78:E3:6D,Espressi Espressif Inc.
 78:E3:B5,HewlettP Hewlett Packard
 78:E3:DE,"Apple Apple, Inc."
 78:E4:00,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
@@ -33737,14 +34389,15 @@
 7C:11:BE,"Apple Apple, Inc."
 7C:11:CB,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:11:CD,QianTang QianTang Technology
 7C:13:1D,SernetSu Sernet (Suzhou) Technologies Corporation
 7C:14:76,DamallTe Damall Technologies SAS
 7C:16:0D,Saia-Bur Saia-Burgess Controls AG
 7C:16:89,Sagemcom Sagemcom Broadband SAS
+7C:17:79,EMMicroe EM Microelectronic
 7C:18:CD,"E-TRON E-TRON Co.,Ltd."
 7C:1A:03,"8Locatio 8Locations Co., Ltd."
 7C:1A:C0,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:1A:FC,"DalianCo Dalian Co-Edifice Video Technology Co., Ltd"
 7C:1B:93,"HuaweiDe Huawei Device Co., Ltd."
 7C:1C:4E,LGInnote LG Innotek
 7C:1C:68,"SamsungE Samsung Electronics Co.,Ltd"
@@ -33763,26 +34416,28 @@
 7C:24:0C,"Telechip Telechips, Inc."
 7C:24:99,"Apple Apple, Inc."
 7C:25:86,JuniperN Juniper Networks
 7C:25:87,chaowifi chaowifi.com
 7C:25:DA,Fn-LinkT Fn-Link Technology Limited
 7C:26:34,"ARRISGro ARRIS Group, Inc."
 7C:26:64,Sagemcom Sagemcom Broadband SAS
+7C:27:3C,"Shenzhen Shenzhen Yunlink Technology Co., Ltd"
 7C:27:BC,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 7C:29:6F,"Apple Apple, Inc."
 7C:2A:31,IntelCor Intel Corporate
 7C:2A:CA,"Apple Apple, Inc."
 7C:2A:DB,XiaomiCo Xiaomi Communications Co Ltd
 7C:2B:E1,"Shenzhen Shenzhen Ferex Electrical Co.,Ltd"
 7C:2C:F3,SecureEl Secure Electrans Ltd
 7C:2E:0D,Blackmag Blackmagic Design
 7C:2E:BD,"Google Google, Inc."
 7C:2E:DD,"SamsungE Samsung Electronics Co.,Ltd"
 7C:2F:80,GigasetC Gigaset Communications GmbH
 7C:31:0E,"Cisco Cisco Systems, Inc"
+7C:31:80,SMK SMK corporation
 7C:33:6E,MEGElect MEG Electronics Inc.
 7C:33:F9,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:35:48,Transcen Transcend Information
 7C:35:F8,"Zhejiang Zhejiang Tmall Technology Co., Ltd."
 7C:38:66,TexasIns Texas Instruments
 7C:38:6C,RealTime Real Time Logic
 7C:38:AD,"SamsungE Samsung Electronics Co.,Ltd"
@@ -33794,14 +34449,30 @@
 7C:3D:2B,"HuaweiDe Huawei Device Co., Ltd."
 7C:3E:74,"HuaweiDe Huawei Device Co., Ltd."
 7C:3E:9D,Patech
 7C:41:A2,Nokia
 7C:43:8F,E-BandCo E-Band Communications Corp.
 7C:44:4C,"Entertai Entertainment Solutions, S.L."
 7C:45:D0,"Shenzhen Shenzhen Wewins Wireless Co., ltd"
+7C:45:F9,IEEERegi IEEE Registration Authority
+7C:45:F9:00:00:00/28,SENSeOR
+7C:45:F9:10:00:00/28,"HunanShe Hunan Shengyun Photoelectric Technology Co., LTD"
+7C:45:F9:20:00:00/28,"Dongguan Dongguan Boyye Industrial Co., Ltd"
+7C:45:F9:30:00:00/28,"Hangzhou Hangzhou LUXAR Technologies Co., Ltd"
+7C:45:F9:40:00:00/28,SPECSSur SPECS Surface Nano Analysis GmbH
+7C:45:F9:50:00:00/28,"Interact Interactive Technologies, Inc."
+7C:45:F9:60:00:00/28,"HankElec Hank Electronics Co., Ltd"
+7C:45:F9:70:00:00/28,GeorgFis Georg Fischer Piping Systems Ltd.
+7C:45:F9:80:00:00/28,Feller Feller AG
+7C:45:F9:90:00:00/28,Mij Mij Co Ltd
+7C:45:F9:A0:00:00/28,qiio qiio AG
+7C:45:F9:B0:00:00/28,"IngDanCh IngDan China-chip Electronic Technology(Wuxi) Co.,Ltd."
+7C:45:F9:C0:00:00/28,Xemex Xemex NV
+7C:45:F9:D0:00:00/28,Mobilari Mobilaris Industrial Solutions
+7C:45:F9:E0:00:00/28,ScaniaCV Scania CV AB
 7C:46:85,"Motorola Motorola (Wuhan) Mobility Technologies Communication Co., Ltd."
 7C:47:7C,IEEERegi IEEE Registration Authority
 7C:47:7C:00:00:00/28,BungBung BungBungame Inc
 7C:47:7C:10:00:00/28,Photosyn Photosynth Inc.
 7C:47:7C:20:00:00/28,Powerlan Powerland Limited
 7C:47:7C:30:00:00/28,EyeLock EyeLock LLC
 7C:47:7C:40:00:00/28,RLCElect RLC Electronics Systems
@@ -33819,14 +34490,15 @@
 7C:49:B9,PlexusMa Plexus Manufacturing Sdn Bhd
 7C:49:EB,"XIAOMIEl XIAOMI Electronics,CO.,LTD"
 7C:4A:82,Portsmit Portsmith LLC
 7C:4A:A8,MindTree MindTree Wireless PVT Ltd
 7C:4B:78,RedSunSy Red Sun Synthesis Pte Ltd
 7C:4C:58,"ScaleCom Scale Computing, Inc."
 7C:4C:A5,SkyUk Sky Uk Limited
+7C:4D:8F,HP HP Inc.
 7C:4E:09,"Shenzhen Shenzhen Skyworth Wireless Technology Co.,Ltd"
 7C:4F:7D,Sawwave
 7C:4F:B5,Arcadyan Arcadyan Technology Corporation
 7C:50:49,"Apple Apple, Inc."
 7C:50:79,IntelCor Intel Corporate
 7C:50:DA,EJWard E.J Ward
 7C:51:89,SGWirele SG Wireless Limited
@@ -33838,27 +34510,29 @@
 7C:57:4E,COBI COBI GmbH
 7C:57:58,HP HP Inc.
 7C:5A:1C,Sophos Sophos Ltd
 7C:5A:67,"JNC JNC Systems, Inc."
 7C:5C:F8,IntelCor Intel Corporate
 7C:60:4A,Avelon
 7C:60:97,"HuaweiTe Huawei Technologies Co.,Ltd"
+7C:61:30,"Apple Apple, Inc."
 7C:61:66,AmazonTe Amazon Technologies Inc.
 7C:61:93,HTC HTC Corporation
 7C:63:05,AmazonTe Amazon Technologies Inc.
 7C:64:56,"SamsungE Samsung Electronics Co.,Ltd"
 7C:64:6C,LGElectr LG Electronics
 7C:66:9A,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:66:9D,TexasIns Texas Instruments
 7C:66:EF,"HonHaiPr Hon Hai Precision IND.CO.,LTD"
 7C:67:A2,IntelCor Intel Corporate
 7C:67:AB,"Roku Roku, Inc"
 7C:69:6B,AtmosicT Atmosic Technologies
 7C:69:F6,"Cisco Cisco Systems, Inc"
 7C:6A:60,"ChinaMob China Mobile Group Device Co.,Ltd."
+7C:6A:8A,"SINOBOND SINOBONDER Technology Co., Ltd."
 7C:6A:B3,IbcTechn Ibc Technologies Inc.
 7C:6A:C3,"GatesAir GatesAir, Inc"
 7C:6A:DB,"SafeTone SafeTone Technology Co.,Ltd"
 7C:6A:F3,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 7C:6B:33,TenyuTec Tenyu Tech Co. Ltd.
 7C:6B:52,TigaroWi Tigaro Wireless
 7C:6B:9C,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -33898,14 +34572,15 @@
 7C:76:35,IntelCor Intel Corporate
 7C:76:68,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:76:73,ENMAS ENMAS GmbH
 7C:77:16,ZyxelCom Zyxel Communications Corporation
 7C:78:7E,"SamsungE Samsung Electronics Co.,Ltd"
 7C:78:B2,WyzeLabs Wyze Labs Inc
 7C:79:E8,PayRange PayRange Inc.
+7C:7A:3C,"NewH3CTe New H3C Technologies Co., Ltd"
 7C:7A:53,PhytrexT Phytrex Technology Corp.
 7C:7A:91,IntelCor Intel Corporate
 7C:7B:8B,"ControlC Control Concepts, Inc."
 7C:7B:E4,ZSedaiKe Z'Sedai Kenkyusho Corporation
 7C:7D:3D,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:7D:41,"JinmuyuE Jinmuyu Electronics Co., Ltd."
 7C:82:2D,Nortec
@@ -33926,14 +34601,15 @@
 7C:83:34:B0:00:00/28,"Shenzhen Shenzhen AZW Technology Co., Ltd."
 7C:83:34:C0:00:00/28,"HunanDat Hunan Datang Xianyi Technology Co.,Ltd"
 7C:83:34:D0:00:00/28,MSVelekt MSV elektronika s.r.o.
 7C:83:34:E0:00:00/28,Balter Balter GmbH
 7C:84:37,"ChinaPos China Post Communications Equipment Co., Ltd."
 7C:85:30,Nokia
 7C:87:CE,Espressi Espressif Inc.
+7C:89:31,"HuaweiDe Huawei Device Co., Ltd."
 7C:89:56,"SamsungE Samsung Electronics Co.,Ltd"
 7C:89:C1,PaloAlto Palo Alto Networks
 7C:8A:C0,EVBox EVBox BV
 7C:8A:E1,"CompalIn Compal Information (Kunshan) Co., Ltd."
 7C:8B:B5,"SamsungE Samsung Electronics Co.,Ltd"
 7C:8B:CA,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 7C:8D:91,"Shanghai Shanghai Hongzhuo Information Technology co.,LTD"
@@ -33945,15 +34621,15 @@
 7C:94:B2,PhilipsH Philips Healthcare PCCI
 7C:95:B1,"ExtremeN Extreme Networks, Inc."
 7C:95:F3,"Cisco Cisco Systems, Inc"
 7C:96:D2,"Fihonest Fihonest communication co.,Ltd"
 7C:97:63,Openmati Openmatics s.r.o.
 7C:97:E1,"HuaweiDe Huawei Device Co., Ltd."
 7C:9A:1D,"Apple Apple, Inc."
-7C:9A:54,Technico Technicolor CH USA Inc.
+7C:9A:54,VantivaU Vantiva USA LLC
 7C:9A:9B,VSEvalen VSE valencia smart energy
 7C:9E:BD,Espressi Espressif Inc.
 7C:9F:07,CigShang Cig Shanghai Co Ltd
 7C:A1:5D,GNReSoun GN ReSound A/S
 7C:A1:77,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:A1:AE,"Apple Apple, Inc."
 7C:A2:37,"KingSlid King Slide Technology CO., LTD."
@@ -34019,27 +34695,30 @@
 7C:BC:84:A0:00:00/28,Opnt Opnt Bv
 7C:BC:84:B0:00:00/28,Guangzho Guangzhou Puppyrobot Technology Co.Ltd Beijing Branch
 7C:BC:84:C0:00:00/28,TibitCom Tibit Communications
 7C:BC:84:D0:00:00/28,VantageI Vantage Integrated Security Solutions Pvt Ltd
 7C:BC:84:E0:00:00/28,"BeijingT Beijing Topnew Group Co., Ltd"
 7C:BD:06,AEREFUso AE REFUsol
 7C:BF:88,Mobilico Mobilicom LTD
+7C:BF:AE,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 7C:BF:B1,"ARRISGro ARRIS Group, Inc."
+7C:C0:6F,"Apple Apple, Inc."
 7C:C1:77,IngramMi Ingram Micro Services
 7C:C1:80,"Apple Apple, Inc."
 7C:C2:25,"SamsungE Samsung Electronics Co.,Ltd"
 7C:C2:55,"SuperMic Super Micro Computer, Inc."
 7C:C2:94,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 7C:C2:C6,TP-Link TP-Link Corporation Limited
 7C:C3:85,"HuaweiTe Huawei Technologies Co.,Ltd"
 7C:C3:A1,"Apple Apple, Inc."
 7C:C4:EF,Devialet
 7C:C5:37,"Apple Apple, Inc."
 7C:C6:C4,KolffCom Kolff Computer Supplies b.v.
 7C:C7:09,"Shenzhen Shenzhen Rf-Link Technology Co.,Ltd."
+7C:C7:4A,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 7C:C7:7E,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 7C:C8:AB,"AcroAsso Acro Associates, Inc."
 7C:C8:D0,"TianjinY Tianjin Yaan Technology Co., Ltd."
 7C:C8:D7,Damalisk
 7C:C9:26,"WuhanGre Wuhan GreeNet Information Service Co.,Ltd."
 7C:C9:5A,DellEMC Dell EMC
 7C:C9:5E,"Dongguan Dongguan Liesheng Electronic Co., Ltd."
@@ -34086,28 +34765,30 @@
 7C:DD:90,"Shenzhen Shenzhen Ogemray Technology Co., Ltd."
 7C:DD:E9,ATOMtech ATOM tech Inc.
 7C:DE:78,"NewH3CTe New H3C Technologies Co., Ltd"
 7C:DF:A1,Espressi Espressif Inc.
 7C:E0:44,NEON NEON Inc
 7C:E1:52,Goodyear The Goodyear Tire & Rubber Company
 7C:E1:FF,"Computer Computer Performance, Inc. DBA Digital Loggers, Inc."
+7C:E2:69,TexasIns Texas Instruments
 7C:E2:CA,JuniperN Juniper Networks
 7C:E4:AA,Private
 7C:E5:24,"Quirky Quirky, Inc."
 7C:E5:6B,"ESENOpto ESEN Optoelectronics Technology Co.,Ltd."
 7C:E8:7F,Sagemcom Sagemcom Broadband SAS
 7C:E9:7C,ItelMobi Itel Mobile Limited
 7C:E9:D3,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 7C:EB:7F,DmetProd Dmet Products Corp.
 7C:EB:AE,Ridgelin Ridgeline Instruments
 7C:EB:EA,Asct
 7C:EC:79,TexasIns Texas Instruments
 7C:EC:9B,"FuzhouTe Fuzhou Teraway Information Technology Co.,Ltd"
 7C:EC:B1,"Apple Apple, Inc."
 7C:ED:8D,Microsof Microsoft
+7C:ED:C6,AmazonTe Amazon Technologies Inc.
 7C:EF:18,Creative Creative Product Design Pty. Ltd.
 7C:EF:40,Nextorag Nextorage Corporation
 7C:EF:61,STRElekt STR Elektronik Josef Schlechtinger GmbH
 7C:EF:8A,InhonInt Inhon International Ltd.
 7C:F0:5F,"Apple Apple, Inc."
 7C:F0:98,"BeeBeans Bee Beans Technologies, Inc."
 7C:F0:BA,Linkwell Linkwell Telesystems Pvt Ltd
@@ -34155,14 +34836,15 @@
 80:02:F4:D0:00:00/28,"JiangsuV Jiangsu Vedkang Medicl Sclence and Technology Co.,Ltd"
 80:02:F4:E0:00:00/28,Alfred Alfred Systems Inc
 80:03:84,RuckusWi Ruckus Wireless
 80:04:5F,"Apple Apple, Inc."
 80:05:88,"RuijieNe Ruijie Networks Co.,LTD"
 80:05:DF,MontageT Montage Technology Group Limited
 80:07:1B,"Vsolutio Vsolution Telecommunication Technology Co.,Ltd."
+80:07:94,"SamsungE Samsung Electronics Co.,Ltd"
 80:07:A2,EssonTec Esson Technology Inc.
 80:09:02,"Keysight Keysight Technologies, Inc."
 80:0A:06,"COMTEC COMTEC co.,ltd"
 80:0A:80,IEEERegi IEEE Registration Authority
 80:0A:80:00:00:00/28,"GolanaTe Golana Technology (Shenzhen) Co., Ltd."
 80:0A:80:10:00:00/28,"Dongguan Dongguan I-Chime electrinics Co.,Ltd"
 80:0A:80:20:00:00/28,"Sumitomo Sumitomo Wiring Systems, Ltd."
@@ -34200,18 +34882,19 @@
 80:22:75,BeijingB Beijing Beny Wave Technology Co Ltd
 80:22:78,ChinaMob China Mobile IOT Company Limited
 80:22:A7,"NECPlatf NEC Platforms, Ltd."
 80:24:8F,"Cisco Cisco Systems, Inc"
 80:25:11,ItelMobi Itel Mobile Limited
 80:26:89,D-LinkIn D-Link International
 80:27:6C,"Cisco Cisco Systems, Inc"
-80:29:94,Technico Technicolor CH USA Inc.
-80:2A:A8,Ubiquiti Ubiquiti Networks Inc.
+80:29:94,VantivaU Vantiva USA LLC
+80:2A:A8,Ubiquiti Ubiquiti Inc
 80:2A:FA,Germanee Germaneers GmbH
 80:2B:F9,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+80:2D:1A,zte zte corporation
 80:2D:BF,"Cisco Cisco Systems, Inc"
 80:2D:E1,Solarbri Solarbridge Technologies
 80:2E:14,azetiNet azeti Networks AG
 80:2F:DE,ZurichIn Zurich Instruments AG
 80:30:49,LiteonTe Liteon Technology Corporation
 80:30:DC,TexasIns Texas Instruments
 80:30:E0,HewlettP Hewlett Packard Enterprise
@@ -34237,14 +34920,15 @@
 80:3C:20,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:3E:48,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 80:3F:5D,Winstars Winstars Technology Ltd
 80:3F:D6,bytesatw bytes at work AG
 80:41:26,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:41:4E,"BbkEduca Bbk Educational Electronics Corp.,Ltd."
 80:42:7C,AdolfTed Adolf Tedsen GmbH & Co. KG
+80:43:3F,JuniperN Juniper Networks
 80:44:FD,"ChinaMob China Mobile (Hangzhou) Information Technology Co., Ltd."
 80:45:DD,IntelCor Intel Corporate
 80:47:31,"PacketDe Packet Design, Inc."
 80:47:86,"SamsungE Samsung Electronics Co.,Ltd"
 80:48:A5,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 80:49:71,"Apple Apple, Inc."
 80:4A:14,"Apple Apple, Inc."
@@ -34268,14 +34952,15 @@
 80:58:F8,"Motorola Motorola Mobility LLC, a Lenovo Company"
 80:59:FD,Noviga
 80:5A:04,LGElectr LG Electronics (Mobile Communications)
 80:5B:65,LGInnote LG Innotek
 80:5E:0C,"YealinkX Yealink(Xiamen) Network Technology Co.,Ltd."
 80:5E:4F,Fn-LinkT Fn-Link Technology Limited
 80:5E:C0,"YealinkX Yealink(Xiamen) Network Technology Co.,Ltd."
+80:5F:8E,"HuizhouB Huizhou BYD Electronic Co., Ltd."
 80:5F:C5,"Apple Apple, Inc."
 80:60:07,Rim
 80:60:36,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:60:B7,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 80:61:5F,"BeijingS Beijing Sinead Technology Co., Ltd."
 80:61:6C,"NewH3CTe New H3C Technologies Co., Ltd"
 80:61:8F,"Shenzhen Shenzhen sangfei consumer communications co.,ltd"
@@ -34304,14 +34989,15 @@
 80:71:7A,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:72:15,SkyUk Sky Uk Limited
 80:72:64,"HuaweiDe Huawei Device Co., Ltd."
 80:73:9F,Kyocera Kyocera Corporation
 80:74:59,"Ks K's Co.,Ltd."
 80:74:84,ALLWinne ALL Winner (Hong Kong) Limited
 80:75:1F,SkyUk Sky Uk Limited
+80:76:77,"hangzhou hangzhou puwell cloud tech co., ltd."
 80:76:93,Newag Newag SA
 80:76:C2,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 80:77:A4,TecnoMob Tecno Mobile Limited
 80:78:71,AskeyCom Askey Computer Corp
 80:79:5D,Infinixm Infinix mobility limited
 80:79:AE,"ShanDong ShanDong Tecsunrise Co.,Ltd"
 80:7A:7F,"ABBGenwa ABB Genway Xiamen Electrical Equipment CO., LTD"
@@ -34331,43 +35017,46 @@
 80:7B:85:90:00:00/28,SmartEle Smart Electronics Nz Limited
 80:7B:85:A0:00:00/28,"Interpla Interplan Co., Ltd."
 80:7B:85:B0:00:00/28,Oliotalo Oliotalo Oy
 80:7B:85:C0:00:00/28,"SCALADig SCALA Digital Technology(Ningbo) CO, LTD"
 80:7B:85:D0:00:00/28,KaynesTe Kaynes Technology India Pvt Ltd
 80:7B:85:E0:00:00/28,Mersen
 80:7B:85:F0:00:00/28,Private
+80:7C:62,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 80:7D:14,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:7D:1B,Neosyste Neosystem Co. Ltd.
 80:7D:3A,Espressi Espressif Inc.
 80:7D:E3,Chongqin Chongqing Sichuan Instrument Microcircuit Co.LTD.
 80:7E:B4,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 80:7F:F8,JuniperN Juniper Networks
+80:80:2C,"Fortinet Fortinet, Inc."
 80:81:A5,"TONGQING TONGQING COMMUNICATION EQUIPMENT (SHENZHEN) Co.,Ltd"
 80:82:23,"Apple Apple, Inc."
 80:82:87,ATCOMTec ATCOM Technology Co.Ltd.
 80:82:F5,STMicrol STMicrolectronics International NV
 80:84:A9,oshkosh oshkosh Corporation
 80:86:98,Netronic Netronics Technologies Inc.
 80:86:D9,"SamsungE Samsung Electronics Co.,Ltd"
 80:86:F2,IntelCor Intel Corporate
 80:89:17,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 80:8A:8B,"vivoMobi vivo Mobile Communication Co., Ltd."
 80:8A:BD,"SamsungE Samsung Electronics Co.,Ltd"
 80:8A:F7,Nanoleaf
 80:8B:5C,"Shenzhen Shenzhen Runhuicheng Technology Co., Ltd"
-80:8C:97,"Kaonmedi Kaonmedia CO., LTD."
+80:8C:97,"KaonGrou Kaon Group Co., Ltd."
 80:8D:B7,HewlettP Hewlett Packard Enterprise
 80:8F:1D,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 80:8F:E8,Intelbra Intelbras
 80:91:2A,"LihRonge Lih Rong electronic Enterprise Co., Ltd."
 80:91:33,AzureWav AzureWave Technology Inc.
 80:91:C0,"AgileMes AgileMesh, Inc."
 80:92:9F,"Apple Apple, Inc."
 80:93:93,Xapt Xapt GmbH
 80:94:6C,TokyoRad Tokyo Radar Corporation
+80:95:62,"ExtremeN Extreme Networks, Inc."
 80:96:21,Lenovo
 80:96:B1,"ARRISGro ARRIS Group, Inc."
 80:96:CA,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 80:97:1B,"Altenerg Altenergy Power System,Inc."
 80:97:33,"Shenzhen Shenzhen Elebao Technology Co., Ltd"
 80:9B:20,IntelCor Intel Corporate
 80:9F:9B,"SichuanA Sichuan AI-Link Technology Co., Ltd."
@@ -34376,50 +35065,57 @@
 80:A0:36,"Shanghai Shanghai MXCHIP Information Technology Co., Ltd."
 80:A1:AB,Intellis Intellisis
 80:A1:D7,"Shanghai Shanghai DareGlobal Technologies Co.,Ltd"
 80:A2:35,Edgecore Edgecore Networks Corporation
 80:A5:89,AzureWav AzureWave Technology Inc.
 80:A7:96,Neuralin Neuralink Corp.
 80:A8:5D,Osterhou Osterhout Design Group
+80:A9:97,"Apple Apple, Inc."
 80:AA:A4,Usag
 80:AB:4D,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 80:AC:7C,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 80:AC:AC,JuniperN Juniper Networks
+80:AC:C8,PhyplusM Phyplus Microelectronics Limited
 80:AD:00,"CnetTech CNET Technology Inc. (Probably an error, see instead 0080AD)"
 80:AD:16,XiaomiCo Xiaomi Communications Co Ltd
 80:AD:67,KasdaNet Kasda Networks Inc
+80:AF:CA,"Shenzhen Shenzhen Cudy Technology Co., Ltd."
 80:B0:3D,"Apple Apple, Inc."
 80:B0:7B,zte zte corporation
 80:B2:19,Elektron Elektron Technology Uk Limited
-80:B2:34,Technico Technicolor CH USA Inc.
+80:B2:34,VantivaU Vantiva USA LLC
 80:B2:89,Forworld Forworld Electronics Ltd.
 80:B3:2A,UKGridSo UK Grid Solutions Ltd
 80:B5:75,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:B6:24,Ivs
 80:B6:55,IntelCor Intel Corporate
 80:B6:86,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:B7:08,"BlueDanu Blue Danube Systems, Inc"
 80:B7:09,"Viptela Viptela, Inc"
 80:B7:45,SilkTech The Silk Technologies ILC LTD
+80:B9:46,Nokia
 80:B9:5C,"ELFTECH ELFTECH Co., Ltd."
 80:B9:7A,eero eero inc.
+80:B9:89,"Apple Apple, Inc."
 80:BA:AC,TeleAdap TeleAdapt Ltd
 80:BA:E6,Neets
 80:BB:EB,Satmap Satmap Systems Ltd
 80:BC:37,RuckusWi Ruckus Wireless
 80:BE:05,"Apple Apple, Inc."
 80:BE:AF,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 80:C1:6E,HewlettP Hewlett Packard
 80:C3:BA,SonovaCo Sonova Consumer Hearing GmbH
+80:C4:1B,TexasIns Texas Instruments
+80:C4:5D,IPGLaser IPG Laser GmbH
 80:C5:01,OctoGate OctoGate IT Security Systems GmbH
 80:C5:48,"Shenzhen Shenzhen Zowee Technology Co.,Ltd"
 80:C5:E6,Microsof Microsoft Corporation
 80:C5:F2,AzureWav AzureWave Technology Inc.
 80:C6:3F,"RemecBro Remec Broadband Wireless , LLC"
-80:C6:AB,Technico Technicolor CH USA Inc.
+80:C6:AB,VantivaU Vantiva USA LLC
 80:C6:CA,Endian Endian s.r.l.
 80:C7:55,Panasoni Panasonic Appliances Company
 80:C7:C5,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 80:C8:62,"Openpeak Openpeak, Inc"
 80:C9:55,"RedpineS Redpine Signals, Inc."
 80:CA:4B,"Shenzhen Shenzhen Gongjin Electronics Co.,Ltd"
 80:CB:BC,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
@@ -34427,29 +35123,30 @@
 80:CC:9C,Netgear
 80:CE:62,HewlettP Hewlett Packard
 80:CE:B1,Theissen Theissen Training Systems GmbH
 80:CE:B9,"SamsungE Samsung Electronics Co.,Ltd"
 80:CF:41,LenovoMo Lenovo Mobile Communication Technology Ltd.
 80:CF:A2,"HuaweiDe Huawei Device Co., Ltd."
 80:D0:19,"Embed Embed, Inc"
-80:D0:4A,Technico Technicolor CH USA Inc.
+80:D0:4A,VantivaU Vantiva USA LLC
 80:D0:65,CKS CKS Corporation
 80:D0:9B,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:D1:60,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 80:D1:8B,"Hangzhou Hangzhou I'converge Technology Co.,Ltd"
 80:D2:1D,AzureWav AzureWave Technology Inc.
+80:D2:66,ScaleFlu ScaleFlux
 80:D2:E5,"Nintendo Nintendo Co.,Ltd"
 80:D3:36,Cern
 80:D4:33,LzLabs LzLabs GmbH
 80:D4:A5,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:D6:05,"Apple Apple, Inc."
 80:D7:33,"QSRAutom QSR Automations, Inc."
 80:DA:13,eero eero inc.
 80:DA:BC,Megafone Megafone Limited
-80:DA:C2,Technico Technicolor CH USA Inc.
+80:DA:C2,VantivaU Vantiva USA LLC
 80:DB:17,JuniperN Juniper Networks
 80:DB:31,"PowerQuo Power Quotient International Co., Ltd."
 80:DE:CC,"HYBE HYBE Co.,LTD"
 80:E0:1D,"Cisco Cisco Systems, Inc"
 80:E1:BF,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:E4:55,"NewH3CTe New H3C Technologies Co., Ltd"
 80:E4:DA,IEEERegi IEEE Registration Authority
@@ -34477,18 +35174,19 @@
 80:EA:23,WistronN Wistron Neweb Corporation
 80:EA:96,"Apple Apple, Inc."
 80:EA:CA,DialogSe Dialog Semiconductor Hellas SA
 80:EB:77,Wistron Wistron Corporation
 80:ED:2C,"Apple Apple, Inc."
 80:EE:25,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 80:EE:73,Shuttle Shuttle Inc.
+80:F0:CF,RuckusWi Ruckus Wireless
 80:F1:A4,"HuaweiTe Huawei Technologies Co.,Ltd"
 80:F1:F1,"Tech4hom Tech4home, Lda"
 80:F2:5E,Kyynel
-80:F3:EF,"Facebook Facebook Technologies, LLC"
+80:F3:EF,"MetaPlat Meta Platforms Technologies, LLC"
 80:F5:03,"ARRISGro ARRIS Group, Inc."
 80:F5:93,IRCOSist IRCO Sistemas de Telecomunicación S.A.
 80:F5:B5,TexasIns Texas Instruments
 80:F6:2E,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 80:F7:A6,"Shenzhen Shenzhen C-Data Technology Co., Ltd."
 80:F8:EB,RayTight
 80:FA:5B,Clevo Clevo Co.
@@ -34496,25 +35194,26 @@
 80:FB:F0,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 80:FB:F1,Freescal Freescale Semiconductor (China) Ltd.
 80:FD:7A,BLUProdu BLU Products Inc
 80:FD:7B,BLUProdu BLU Products Inc
 80:FF:A8,Unidis
 84:00:2D,Pegatron Pegatron Corporation
 84:00:D2,Sony Sony Corporation
-84:01:12,"Kaonmedi Kaonmedia CO., LTD."
+84:01:12,"KaonGrou Kaon Group Co., Ltd."
 84:01:A7,"Greyware Greyware Automation Products, Inc"
 84:02:83,"HUMAX HUMAX Co., Ltd."
 84:03:28,JuniperN Juniper Networks
 84:04:D2,KiraleTe Kirale Technologies SL
 84:06:FA,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 84:07:C4,Carrier Carrier Corporation
 84:0B:2D,"SamsungE Samsung Electro Mechanics Co., Ltd."
 84:0B:7C,HitronTe Hitron Technologies. Inc
 84:0B:BB,MitraSta MitraStar Technology Corp.
 84:0D:8E,Espressi Espressif Inc.
+84:0F:2A,"JiangxiR Jiangxi Risound Electronics Co., LTD"
 84:0F:45,"Shanghai Shanghai GMT Digital Technologies Co., Ltd"
 84:10:0D,"Motorola Motorola Mobility LLC, a Lenovo Company"
 84:11:9E,"SamsungE Samsung Electronics Co.,Ltd"
 84:11:C2,IEEERegi IEEE Registration Authority
 84:11:C2:00:00:00/28,Kazdream Kazdream Technologies LLP
 84:11:C2:10:00:00/28,"BeijingD Beijing Dayu Technology Co., Ltd."
 84:11:C2:20:00:00/28,Futureco Futurecom Systems Group
@@ -34533,15 +35232,15 @@
 84:13:9F,zte zte corporation
 84:14:4D,IntelCor Intel Corporate
 84:15:D3,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:16:0C,Broadcom Broadcom Limited
 84:16:F9,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 84:17:15,GPElectr GP Electronics (HK) Ltd.
 84:17:66,"WeifangG Weifang Goertek Electronics Co.,Ltd"
-84:17:EF,Technico Technicolor CH USA Inc.
+84:17:EF,VantivaU Vantiva USA LLC
 84:18:26,Osram Osram GmbH
 84:18:3A,RuckusWi Ruckus Wireless
 84:18:88,JuniperN Juniper Networks
 84:1B:38,"Shenzhen Shenzhen Excelsecu Data Technology Co.,Ltd"
 84:1B:5E,Netgear
 84:1B:77,IntelCor Intel Corporate
 84:1C:70,zte zte corporation
@@ -34560,34 +35259,37 @@
 84:25:DB,"SamsungE Samsung Electronics Co.,Ltd"
 84:26:15,ADBBroad ADB Broadband Italia
 84:26:2B,Nokia
 84:26:7A,"Guangdon Guangdong Taide Zhilian Technology Co.,Ltd"
 84:26:90,"BeijingT Beijing Thought Science Co.,Ltd."
 84:27:B6,ChinaMob China Mobile IOT Company Limited
 84:27:CE,Presidin Corporation of the Presiding Bishop of The Church of Jesus Christ of Latter-day Saints
+84:28:59,AmazonTe Amazon Technologies Inc.
 84:28:5A,SaffronS Saffron Solutions Inc
 84:29:14,EMPORIAT EMPORIA TELECOM Produktions- und VertriebsgesmbH & Co KG
 84:29:99,"Apple Apple, Inc."
 84:2A:FD,HP HP Inc.
 84:2B:2B,Dell Dell Inc.
 84:2B:50,"Huria Huria Co.,Ltd."
 84:2B:BC,Modellei Modelleisenbahn GmbH
 84:2C:80,SichuanC Sichuan Changhong Electric Ltd.
 84:2E:14,SiliconL Silicon Laboratories
 84:2E:27,"SamsungE Samsung Electronics Co.,Ltd"
 84:2F:75,InnokasG Innokas Group
 84:30:95,"HonHaiPr Hon Hai Precision IND.CO.,LTD"
+84:30:CE,"Shenzhen Shenzhen Jaguar Microsystems Co., Ltd"
 84:30:E5,"SkyHawke SkyHawke Technologies, LLC"
 84:32:6F,"Guangzho Guangzhou Ava Electronics Technology Co.,Ltd"
 84:32:EA,"AnhuiWan Anhui Wanzten P&T Co., Ltd"
 84:34:97,HewlettP Hewlett Packard
 84:36:11,hyungseu hyungseul publishing networks
 84:37:D5,"SamsungE Samsung Electronics Co.,Ltd"
 84:38:35,"Apple Apple, Inc."
 84:38:38,SamsungE Samsung Electro-Mechanics(Thailand)
+84:39:8F,"Fortinet Fortinet, Inc."
 84:39:BE:00:00:00/28,"HinoEngi Hino Engineering, Inc"
 84:39:BE:10:00:00/28,Guangzho Guangzhou Heygears Technology Ltd
 84:39:BE:20:00:00/28,ChengDuv Cheng Du virtual world Technology Limited.
 84:39:BE:30:00:00/28,"ShenZhen ShenZhen Fudeyu Technology co.,Ltd"
 84:39:BE:40:00:00/28,"Shenzhen Shenzhen Ramos Digital Technology Co,.Ltd."
 84:39:BE:50:00:00/28,Neat Neat S.r.l.
 84:39:BE:60:00:00/28,"Shenzhen Shenzhen IP3 Century Intelligent Technology Co., Ltd"
@@ -34597,48 +35299,54 @@
 84:39:BE:B0:00:00/28,"Shenzhen Shenzhen Horn Audio Co.,Ltd."
 84:39:BE:C0:00:00/28,EDCElect EDC Electronic Design Chemnitz GmbH
 84:39:BE:D0:00:00/28,"Shenzhen Shenzhen Lidaxun Digital Technology Co.,Ltd"
 84:3A:4B,IntelCor Intel Corporate
 84:3A:5B,Inventec Inventec(Chongqing) Corporation
 84:3B:10,Lvswitch Lvswitches Inc.
 84:3C:4C,RobertBo Robert Bosch SRL
+84:3C:99,zte zte corporation
 84:3D:C6,"Cisco Cisco Systems, Inc"
+84:3E:1D,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 84:3E:79,"Shenzhen Shenzhen Belon Technology CO.,LTD"
 84:3E:92,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:3F:4E,"Tri-Tech Tri-Tech Manufacturing, Inc."
 84:40:76,Drivenet Drivenets
 84:41:67,"Apple Apple, Inc."
 84:44:64,ServerU ServerU Inc
 84:44:AF,"Zhejiang Zhejiang Tmall Technology Co., Ltd."
+84:46:93,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 84:46:FE,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:47:09,"Shenzhen Shenzhen IP3 Century Intelligent Technology CO.,Ltd"
 84:47:65,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:48:23,WOXTERTE WOXTER TECHNOLOGY Co. Ltd
 84:49:15,"vArmourN vArmour Networks, Inc."
 84:4B:B7,"BeijingS Beijing Sankuai Online Technology Co.,Ltd"
 84:4B:F5,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+84:4D:BE,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 84:4F:03,Ablelink Ablelink Electronics Ltd
 84:50:9A,"EasySoft Easy Soft TV Co., Ltd"
 84:51:81,"SamsungE Samsung Electronics Co.,Ltd"
 84:54:DF,"HuaweiDe Huawei Device Co., Ltd."
 84:55:A5,"SamsungE Samsung Electronics Co.,Ltd"
 84:56:9C,"CohoData Coho Data, Inc.,"
 84:57:33,Microsof Microsoft Corporation
 84:57:87,"DVRC&C DVR C&C Co., Ltd."
+84:5A:3E,"Cisco Cisco Systems, Inc"
 84:5A:81,ffly4u
 84:5B:12,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:5C:93,Chabrier Chabrier Services
 84:5C:F3,IntelCor Intel Corporate
 84:5D:D7,"Shenzhen Shenzhen Netcom Electronics Co.,Ltd"
 84:5F:04,"SamsungE Samsung Electronics Co.,Ltd"
 84:60:82,"Hyperloo Hyperloop Technologies, Inc dba Virgin Hyperloop"
 84:61:A0,"ARRISGro ARRIS Group, Inc."
 84:62:23,"Shenzhen Shenzhen Coship Electronics Co., Ltd."
 84:62:A6,"EuroCBPh EuroCB (Phils), Inc."
 84:63:D6,Microsof Microsoft Corporation
+84:64:DD,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:65:69,"NewH3CTe New H3C Technologies Co., Ltd"
 84:68:3E,IntelCor Intel Corporate
 84:68:78,"Apple Apple, Inc."
 84:68:C8,Totolink Totolink Technology Int‘L Limited
 84:69:91,Nokia
 84:69:93,HP HP Inc.
 84:6A:66,"Sumitomo Sumitomo Kizai Co.,Ltd."
@@ -34646,26 +35354,28 @@
 84:6B:48,"ShenZhen ShenZhen EepuLink Co., Ltd."
 84:6E:B1,ParkAssi Park Assist LLC
 84:6F:CE,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 84:70:D7,eero eero inc.
 84:71:27,SiliconL Silicon Laboratories
 84:71:6A,"HuaweiDe Huawei Device Co., Ltd."
 84:72:07,I&CTechn I&C Technology
+84:72:93,TexasIns Texas Instruments
 84:73:03,LetvMobi Letv Mobile and Intelligent Information Technology (Beijing) Corporation Ltd.
 84:74:2A,zte zte corporation
 84:74:60,zte zte corporation
 84:76:16,Addatsro Addat s.r.o.
 84:76:37,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:77:78,Cochlear Cochlear Limited
 84:78:8B,"Apple Apple, Inc."
 84:78:AC,"Cisco Cisco Systems, Inc"
 84:79:33,profichi profichip GmbH
 84:79:73,"Shanghai Shanghai Baud Data Communication Co.,Ltd."
 84:7A:88,HTC HTC Corporation
 84:7A:B6,AltoBeam AltoBeam (China) Inc.
+84:7A:DF,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 84:7B:57,IntelCor Intel Corporate
 84:7B:EB,Dell Dell Inc.
 84:7C:9B,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 84:7D:50,HolleyMe Holley Metering Limited
 84:7E:40,TexasIns Texas Instruments
 84:7F:3D,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 84:80:2D,"Cisco Cisco Systems, Inc"
@@ -34676,15 +35386,17 @@
 84:83:36,Newrun
 84:83:71,Avaya Avaya Inc
 84:84:33,ParadoxE Paradox Engineering SA
 84:85:06,"Apple Apple, Inc."
 84:85:0A,HellaSon Hella Sonnen- und Wetterschutztechnik GmbH
 84:85:53,"BiznesSy Biznes Systema Telecom, LLC"
 84:85:E6,"Guangdon Guangdong Asano Technology CO.,Ltd."
+84:86:87,weiyuant weiyuantechnology
 84:86:F3,Greenvit Greenvity Communications
+84:88:E1,"Apple Apple, Inc."
 84:89:AD,"Apple Apple, Inc."
 84:89:EC,IEEERegi IEEE Registration Authority
 84:89:EC:00:00:00/28,SmartGia SmartGiant Technology
 84:89:EC:10:00:00/28,"Research Research Electronics International, LLC."
 84:89:EC:20:00:00/28,thousand thousand star tech LTD.
 84:89:EC:30:00:00/28,Aerionic Aerionics Inc.
 84:89:EC:40:00:00/28,VayyarIm Vayyar Imaging Ltd.
@@ -34694,14 +35406,15 @@
 84:89:EC:80:00:00/28,ArtsDigi Arts Digital Technology (HK) Ltd.
 84:89:EC:90:00:00/28,"Shenzhen Shenzhen Xtooltech Co., Ltd"
 84:89:EC:A0:00:00/28,NewellBr Newell Brands
 84:89:EC:B0:00:00/28,EPSaElek EPSa Elektronik & Präzisionsbau Saalfeld GmbH
 84:89:EC:C0:00:00/28,Shinkawa Shinkawa Ltd.
 84:89:EC:D0:00:00/28,PriceInd Price Industries Limited
 84:89:EC:E0:00:00/28,"Shenzhen Shenzhen Intellifusion Technologies Co., Ltd."
+84:8A:59,"Hisilico Hisilicon Technologies Co., Ltd"
 84:8A:8D,"Cisco Cisco Systems, Inc"
 84:8B:CD,IEEERegi IEEE Registration Authority
 84:8B:CD:00:00:00/28,SouXinCo SouXin Corporate
 84:8B:CD:10:00:00/28,Shenzhen Shenzhen LTIME In-Vehicle Entertainment System Company Limited
 84:8B:CD:20:00:00/28,CCXTechn CCX Technologies Inc.
 84:8B:CD:30:00:00/28,Annapurn Annapurna labs
 84:8B:CD:40:00:00/28,LogicSup Logic Supply
@@ -34756,14 +35469,15 @@
 84:A9:C4,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:A9:EA,CareerTe Career Technologies USA
 84:AA:9C,MitraSta MitraStar Technology Corp.
 84:AA:A4,SONoC SONoC Corp.
 84:AB:1A,"Apple Apple, Inc."
 84:AB:26,Tiinlab Tiinlab Corporation
 84:AC:16,"Apple Apple, Inc."
+84:AC:60,"GuangxiH Guangxi Hesheng Electronics Co., Ltd."
 84:AC:A4,"BeijingN Beijing Novel Super Digital TV Technology Co., Ltd"
 84:AC:FB,CrouzetA Crouzet Automatismes
 84:AD:58,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:AD:8D,"Apple Apple, Inc."
 84:AF:1F,"BeatSyst Beat System Service Co,. Ltd."
 84:AF:EC,Buffalo Buffalo.Inc
 84:B1:53,"Apple Apple, Inc."
@@ -34771,14 +35485,15 @@
 84:B2:61,"Cisco Cisco Systems, Inc"
 84:B3:1B,Kinexon Kinexon GmbH
 84:B3:86,IEEERegi IEEE Registration Authority
 84:B3:86:00:00:00/28,NanJingW Nan Jing WZX Technology Limited
 84:B3:86:10:00:00/28,"SichuanH Sichuan Huakun Zhenyu Intelligent Technology Co., Ltd"
 84:B3:86:20:00:00/28,Annapurn Annapurna labs
 84:B3:86:30:00:00/28,Phonesui Phonesuite
+84:B3:86:40:00:00/28,Cobham
 84:B3:86:50:00:00/28,Fusus
 84:B3:86:60:00:00/28,ALPHA ALPHA Corporation
 84:B3:86:70:00:00/28,"FOTILEGR FOTILE GROUP NINGBO FOTILE KITCHENWARE Co.,Ltd"
 84:B3:86:80:00:00/28,NetworX
 84:B3:86:90:00:00/28,WeissRob Weiss Robotics GmbH & Co. KG
 84:B3:86:A0:00:00/28,"VelocioN Velocio Networks, Inc."
 84:B3:86:B0:00:00/28,"Sinengel Sineng electric CO., Ltd"
@@ -34804,35 +35519,38 @@
 84:C5:A6,IntelCor Intel Corporate
 84:C6:92,TexasIns Texas Instruments
 84:C7:27,Gnodal Gnodal Ltd
 84:C7:8F,APSNetwo APS Networks GmbH
 84:C7:A9,C3Po C3Po S.A.
 84:C7:EA,Sony Sony Corporation
 84:C8:07,ADVAOpti ADVA Optical Networking Ltd.
+84:C8:A0,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 84:C8:B1,Incognit Incognito Software Systems Inc.
 84:C9:B2,D-LinkIn D-Link International
 84:C9:C6,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 84:CC:63,"HuaweiDe Huawei Device Co., Ltd."
 84:CC:A8,Espressi Espressif Inc.
 84:CD:62,"ShenZhen ShenZhen IDWELL Technology CO.,Ltd"
 84:CF:BF,Fairphon Fairphone
 84:D1:5A,TCTmobil TCT mobile ltd
+84:D3:28,"Apple Apple, Inc."
 84:D3:2A,Ieee1905 Ieee 1905.1
 84:D3:43,Calix Calix Inc.
+84:D3:52,TonlyTec Tonly Technology Co. Ltd
 84:D3:D5,"HuaweiDe Huawei Device Co., Ltd."
 84:D4:12,PaloAlto Palo Alto Networks
 84:D4:7E,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 84:D4:C8,Widex Widex A/S
 84:D6:08,"Wingtech Wingtech Mobile Communications Co., Ltd."
 84:D6:C5,SolarEdg SolarEdge Technologies
 84:D6:D0,AmazonTe Amazon Technologies Inc.
 84:D8:1B,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 84:D9:31,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 84:D9:C8,"Unipatte Unipattern Co.,"
-84:DB:2F,SierraWi Sierra Wireless
+84:DB:2F,"SierraWi Sierra Wireless, ULC"
 84:DB:9E,PinkNect Pink Nectarine Health AB
 84:DB:A4,"HuaweiDe Huawei Device Co., Ltd."
 84:DB:AC,"HuaweiTe Huawei Technologies Co.,Ltd"
 84:DB:FC,Nokia
 84:DD:20,TexasIns Texas Instruments
 84:DD:B7,CilagInt Cilag GmbH International
 84:DE:3D,CrystalV Crystal Vision Ltd
@@ -34872,14 +35590,15 @@
 84:EB:3E,VivintSm Vivint Smart Home
 84:EB:EF,"Cisco Cisco Systems, Inc"
 84:ED:33,"BBMC BBMC Co.,Ltd"
 84:EF:18,IntelCor Intel Corporate
 84:F1:17,Newseaso Newseason
 84:F1:29,Metrasca Metrascale Inc.
 84:F1:47,"Cisco Cisco Systems, Inc"
+84:F1:75,"JiangxiX Jiangxi Xunte Intelligent Terminal Co., Ltd"
 84:F1:D0,EhoomeIo Ehoome Iot Private Limited
 84:F3:EB,Espressi Espressif Inc.
 84:F4:4C,"Internat International Integrated Systems., Inc."
 84:F4:93,OMSspols OMS spol. s.r.o.
 84:F6:4C,CrossPoi Cross Point BV
 84:F6:FA,Miovisio Miovision Technologies Incorporated
 84:F7:03,Espressi Espressif Inc.
@@ -34895,19 +35614,22 @@
 88:01:18,BLT BLT Co
 88:01:F2,VitecSys Vitec System Engineering Inc.
 88:01:F9,TexasIns Texas Instruments
 88:03:4C,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 88:03:55,Arcadyan Arcadyan Technology Corporation
 88:03:E9,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 88:07:4B,LGElectr LG Electronics (Mobile Communications)
+88:08:94,Skullcan Skullcandy
 88:09:05,MTMCommu MTMCommunications
 88:09:07,MKTSyste MKT Systemtechnik GmbH & Co. KG
 88:09:AF,Masimo Masimo Corporation
 88:0A:A3,JuniperN Juniper Networks
+88:0C:E0,TexasIns Texas Instruments
 88:0F:10,"HuamiInf Huami Information Technology Co.,Ltd."
+88:0F:A2,Sagemcom Sagemcom Broadband SAS
 88:0F:B6,"JabilCir Jabil Circuits India Pvt Ltd,-EHTP unit"
 88:10:36,PanodicS Panodic(ShenZhen) Electronics Limted
 88:10:8F,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:11:96,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:12:3D,SuzhouAq Suzhou Aquila Solutions Inc.
 88:12:4E,Qualcomm Qualcomm Inc.
 88:12:AC,HunanFn- Hunan Fn-Link Technology Limited
@@ -34916,38 +35638,42 @@
 88:15:C5,"HuaweiDe Huawei Device Co., Ltd."
 88:17:A3,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 88:18:AE,"Tamron Tamron Co., Ltd"
 88:19:08,"Apple Apple, Inc."
 88:1B:99,Shenzhen Shenzhen Xin Fei Jia Electronic Co. Ltd.
 88:1C:95,ItelMobi Itel Mobile Limited
 88:1D:FC,"Cisco Cisco Systems, Inc"
+88:1E:59,Onion Onion Corporation
 88:1E:5A,"Apple Apple, Inc."
 88:1F:A1,"Apple Apple, Inc."
 88:20:0D,"Apple Apple, Inc."
 88:20:12,LMITechn LMI Technologies
 88:21:E3,"Nebusens Nebusens, S.L."
 88:22:B2,ChipseaT Chipsea Technologies (Shenzhen) Corp.
 88:23:1F,FibocomW Fibocom Wireless Inc.
 88:23:64,Watchnet Watchnet DVR Inc
 88:23:8C,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 88:23:FE,TTTechCo TTTech Computertechnik AG
+88:25:08,"MetaPlat Meta Platforms Technologies, LLC"
 88:25:10,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 88:25:2C,Arcadyan Arcadyan Technology Corporation
 88:25:93,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 88:28:7D,AltoBeam AltoBeam (China) Inc.
 88:28:B3,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:28:FB,JuniperN Juniper Networks
 88:29:49,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 88:29:50,"NetmoonT Netmoon Technology Co., Ltd"
 88:29:9C,"SamsungE Samsung Electronics Co.,Ltd"
 88:2A:5E,"NewH3CTe New H3C Technologies Co., Ltd"
 88:2B:94,"MADOKASY MADOKA SYSTEM Co.,Ltd."
 88:2B:D7,Addénerg Addénergie Technologies
 88:2D:53,"BaiduOnl Baidu Online Network Technology (Beijing) Co., Ltd."
 88:2E:5A,storONE
+88:2F:64,BCOMNetw BCOM Networks Limited
+88:30:37,JuniperN Juniper Networks
 88:30:8A,"MurataMa Murata Manufacturing Co., Ltd."
 88:32:9B,SamsungE Samsung Electro-Mechanics(Thailand)
 88:33:14,TexasIns Texas Instruments
 88:33:BE,"Ivenix Ivenix, Inc."
 88:34:FE,BoschAut Bosch Automotive Products (Suzhou) Co. Ltd
 88:35:4C,Transics
 88:35:C1,"OiElectr Oi Electric Co.,Ltd"
@@ -34955,14 +35681,15 @@
 88:36:5F,LGElectr LG Electronics (Mobile Communications)
 88:36:6C,EFMNetwo EFM Networks
 88:36:CF,"HuaweiDe Huawei Device Co., Ltd."
 88:3A:30,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 88:3B:8B,Cheering Cheering Connection Co. Ltd.
 88:3C:1C,Mercury Mercury Corporation
 88:3C:93,Alcatel- Alcatel-Lucent Enterprise
+88:3C:C5,IEEERegi IEEE Registration Authority
 88:3C:C5:00:00:00/28,"ChengduD Chengdu Data Sky Technology Co., Ltd."
 88:3C:C5:10:00:00/28,HanweiEl Hanwei Electronics Group Corporation
 88:3C:C5:20:00:00/28,NetgenHi Netgen Hitech Solutions Llp
 88:3C:C5:30:00:00/28,"shenzhen shenzhen Feng Jing Sheng Electronics Technology Co.,Ltd"
 88:3C:C5:40:00:00/28,SwabianI Swabian Instruments GmbH
 88:3C:C5:50:00:00/28,"Shanghai Shanghai Ucan Automation Equipment Co., Ltd."
 88:3C:C5:60:00:00/28,mfJebsen mfJebsen Electronics Ltd.
@@ -34972,14 +35699,15 @@
 88:3C:C5:A0:00:00/28,"Corigine Corigine,Inc."
 88:3C:C5:B0:00:00/28,"Shenzhen Shenzhen shijia chuangxin Technology Co., Ltd"
 88:3C:C5:C0:00:00/28,HDLdaAma HDL da Amazônia Industria Eletrônica Ltda
 88:3C:C5:D0:00:00/28,LenardEn Lenard Enterprises Inc
 88:3C:C5:E0:00:00/28,myUpTech myUpTech AB
 88:3D:24,"Google Google, Inc."
 88:3F:0C,"systemav system a.v. co., ltd."
+88:3F:37,"Uhtek Uhtek Co., Ltd."
 88:3F:4A,TexasIns Texas Instruments
 88:3F:99,Siemens Siemens AG
 88:3F:D3,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:40:33,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:40:3B,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:40:67,infomark
 88:41:57,"Shenzhen Shenzhen Atsmart Technology Co.,Ltd."
@@ -35005,14 +35733,15 @@
 88:53:2E,IntelCor Intel Corporate
 88:53:95,"Apple Apple, Inc."
 88:53:D4,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:54:1F,"Google Google, Inc."
 88:57:1D,SeongjiI Seongji Industry Company
 88:57:6D,XTAElect XTA Electronics Ltd
 88:57:EE,Buffalo Buffalo.Inc
+88:58:BE,kuosheng kuosheng.com
 88:5A:06,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 88:5A:85,WistronN Wistron Neweb Corporation
 88:5A:92,"Cisco Cisco Systems, Inc"
 88:5B:DD,"ExtremeN Extreme Networks, Inc."
 88:5C:47,AlcatelL Alcatel Lucent
 88:5D:90,IEEERegi IEEE Registration Authority
 88:5D:90:00:00:00/28,"FoshanHu Foshan Huaguo Optical Co.,Ltd"
@@ -35045,28 +35774,35 @@
 88:5F:E8:90:00:00/28,Sowee
 88:5F:E8:A0:00:00/28,LisleDes Lisle Design Ltd
 88:5F:E8:B0:00:00/28,"Shenzhen Shenzhen ORVIBO Technology Co., Ltd"
 88:5F:E8:C0:00:00/28,InorProc Inor Process AB
 88:5F:E8:D0:00:00/28,"zhejiang zhejiang yuanwang communication technolgy co.,ltd"
 88:5F:E8:E0:00:00/28,"UnicomGl Unicom Global, Inc."
 88:61:5A,SianoMob Siano Mobile Silicon Ltd.
+88:62:5D,"Bitnetwo Bitnetworks Co.,Ltd"
 88:63:DF,"Apple Apple, Inc."
 88:64:40,"Apple Apple, Inc."
 88:66:39,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:66:5A,"Apple Apple, Inc."
 88:66:A5,"Apple Apple, Inc."
+88:67:DC,"HuaweiTe Huawei Technologies Co.,Ltd"
+88:68:4B,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 88:68:5C,"Shenzhen Shenzhen ChuangDao & Perpetual Eternal Technology Co.,Ltd"
 88:69:3D,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:6A:B1,"vivoMobi vivo Mobile Communication Co., Ltd."
 88:6A:E3,AlphaNet Alpha Networks Inc.
 88:6B:0F,Bluegiga Bluegiga Technologies OY
 88:6B:44,SunnovoI Sunnovo International Limited
 88:6B:6E,"Apple Apple, Inc."
 88:6B:76,"ChinaHop China Hopeful Group Hopeful Electric Co.,Ltd"
+88:6C:60,XiaomiCo Xiaomi Communications Co Ltd
+88:6D:2D,"HuaweiDe Huawei Device Co., Ltd."
+88:6E:DD,"Micronet Micronet union Technology(Chengdu)Co., Ltd."
 88:6E:E1,ErbeElek Erbe Elektromedizin GmbH
+88:6E:EB,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:6F:29,Pocketbo Pocketbook International SA
 88:6F:D4,Dell Dell Inc.
 88:70:33,Hangzhou Hangzhou Silan Microelectronic Inc
 88:70:8C,LenovoMo Lenovo Mobile Communication Technology Ltd.
 88:70:EF,"SCProfes SC Professional Trading Co., Ltd."
 88:71:B1,"ARRISGro ARRIS Group, Inc."
 88:71:E5,AmazonTe Amazon Technologies Inc.
@@ -35076,16 +35812,18 @@
 88:75:56,"Cisco Cisco Systems, Inc"
 88:75:98,"SamsungE Samsung Electronics Co.,Ltd"
 88:78:73,IntelCor Intel Corporate
 88:78:9C,GameTech Game Technologies SA
 88:79:5B,"KonkaGro Konka Group Co., Ltd."
 88:79:7E,"Motorola Motorola Mobility LLC, a Lenovo Company"
 88:7A:31,Velankan Velankani Electronics Pvt. Ltd.
+88:7B:2C,zte zte corporation
 88:7E:25,"ExtremeN Extreme Networks, Inc."
 88:7F:03,ComperTe Comper Technology Investment Limited
+88:81:87,"UmeoxInn Umeox Innovations Co.,Ltd"
 88:81:B9,"HuaweiDe Huawei Device Co., Ltd."
 88:82:79,Shenzhen Shenzhen RB-LINK Intelligent Technology Co.Ltd
 88:83:22,"SamsungE Samsung Electronics Co.,Ltd"
 88:83:5D,Fn-LinkT Fn-Link Technology Limited
 88:86:03,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:86:A0,"SimtonTe Simton Technologies, Ltd."
 88:86:C2,STABILOI STABILO International GmbH
@@ -35094,14 +35832,15 @@
 88:89:14,AllCompo All Components Incorporated
 88:89:2F,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:89:64,GSIElect GSI Electronics Inc.
 88:8B:5D,StorageA Storage Appliance Corporation
 88:8C:19,BradyAsi Brady Corp Asia Pacific Ltd
 88:8E:68,"HuaweiDe Huawei Device Co., Ltd."
 88:8E:7F,Atop Atop Corporation
+88:8F:10,"Shenzhen Shenzhen Max Infinite Technology Co.,Ltd."
 88:8F:A4,"HuaweiDe Huawei Device Co., Ltd."
 88:90:09,JuniperN Juniper Networks
 88:90:8D,"Cisco Cisco Systems, Inc"
 88:91:66,Viewcoop Viewcooper Corp.
 88:91:DD,Racktivi Racktivity
 88:94:71,BrocadeC Brocade Communications Systems LLC
 88:94:7E,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
@@ -35119,26 +35858,26 @@
 88:97:DF,Entrypas Entrypass Corporation Sdn. Bhd.
 88:98:21,Teraon
 88:9B:39,"SamsungE Samsung Electronics Co.,Ltd"
 88:9C:A6,BTBKorea BTB Korea INC
 88:9C:AD,"Cisco Cisco Systems, Inc"
 88:9D:98,Allied-t Allied-telesisK.K.
 88:9E:33,TCTmobil TCT mobile ltd
-88:9E:68,Technico Technicolor CH USA Inc.
+88:9E:68,VantivaU Vantiva USA LLC
 88:9F:6F,"SamsungE Samsung Electronics Co.,Ltd"
 88:9F:AA,HellaGut Hella Gutmann Solutions GmbH
 88:9F:FA,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 88:A0:84,Formatio Formation Data Systems
 88:A0:BE,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:A2:5E,JuniperN Juniper Networks
 88:A2:D7,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:A3:03,"SamsungE Samsung Electronics Co.,Ltd"
 88:A3:CC,AmatisCo Amatis Controls
 88:A4:79,"Apple Apple, Inc."
-88:A4:C2,"LCFCHefe LCFC(Hefei) Electronics Technology Co., Ltd"
+88:A4:C2,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 88:A5:BD,Qpcom Qpcom Inc.
 88:A6:C6,Sagemcom Sagemcom Broadband SAS
 88:A7:3C,Ragentek Ragentek Technology Group
 88:A9:A7,IEEERegi IEEE Registration Authority
 88:A9:A7:00:00:00/28,Shenzhen Shenzhenshi kechuangzhixian technology Co.LTD
 88:A9:A7:10:00:00/28,Solaredg Solaredge LTD.
 88:A9:A7:20:00:00/28,Honeywel Honeywell spol. s.r.o. HTS CZ o.z.
@@ -35168,16 +35907,18 @@
 88:B1:68,DeltaCon Delta Control GmbH
 88:B1:E1,"MojoNetw Mojo Networks, Inc."
 88:B2:91,"Apple Apple, Inc."
 88:B3:62,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 88:B4:36,FUJIFILM FUJIFILM Corporation
 88:B4:A6,"Motorola Motorola Mobility LLC, a Lenovo Company"
 88:B4:BE,"HuaweiTe Huawei Technologies Co.,Ltd"
+88:B5:FF,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 88:B6:27,GembirdE Gembird Europe BV
 88:B6:6B,easynetw easynetworks
+88:B6:BD,"Flaircom Flaircomm Microelectronics, Inc."
 88:B6:EE,DishTech Dish Technologies Corp
 88:B8:63,"HisenseV Hisense Visual Technology Co.,Ltd"
 88:B8:6F,Infinixm Infinix mobility limited
 88:B8:D0,"Dongguan Dongguan Koppo Electronic Co.,Ltd"
 88:B9:45,"Apple Apple, Inc."
 88:BA:7F,"Qfiednet Qfiednet Co., Ltd."
 88:BC:C1,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -35192,26 +35933,27 @@
 88:C2:55,TexasIns Texas Instruments
 88:C3:6E,BeijingE Beijing Ereneben lnformation Technology Limited
 88:C3:97,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 88:C3:B3,Sovico
 88:C3:E5,BetopTec Betop Techonologies
 88:C6:26,"Logitech Logitech, Inc"
 88:C6:63,"Apple Apple, Inc."
+88:C6:E8,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:C9:B3,IEEERegi IEEE Registration Authority
 88:C9:B3:00:00:00/28,AdoptNet Adopt Nettech Pvt Ltd
 88:C9:B3:10:00:00/28,CervozTe Cervoz Technology Co; Ltd.
 88:C9:B3:20:00:00/28,"shenzhen shenzhen franklin ESS technology CO.,Ltd"
 88:C9:B3:30:00:00/28,"FortiveS Fortive Setra-ICG(Tianjin)Co.,Ltd"
 88:C9:B3:40:00:00/28,Hasbro Hasbro Inc
 88:C9:B3:50:00:00/28,"Brabende Brabender Technologie GmbH & Co, KG"
 88:C9:B3:60:00:00/28,HugoTech Hugo Techno
 88:C9:B3:70:00:00/28,RobertBo Robert Bosch JuP1
 88:C9:B3:80:00:00/28,Divelbis Divelbiss Corporation
 88:C9:B3:90:00:00/28,"Richbeam Richbeam (Beijing) Technology Co., Ltd."
-88:C9:B3:A0:00:00/28,GefranDr Gefran Drive & Motion srl
+88:C9:B3:A0:00:00/28,WegAutom Weg Automation Europe S.R.L.
 88:C9:B3:B0:00:00/28,"Shenzhen Shenzhen MMUI Co.,Ltd"
 88:C9:B3:C0:00:00/28,"Shenzhen Shenzhen Viewsmart Technology Co.,Ltd"
 88:C9:B3:D0:00:00/28,OriginsT Origins Technology Limited
 88:C9:B3:E0:00:00/28,Sercomm Sercomm Corporation.
 88:C9:D0,LGElectr LG Electronics (Mobile Communications)
 88:C9:E8,Sony Sony Corporation
 88:CB:87,"Apple Apple, Inc."
@@ -35264,36 +36006,39 @@
 88:F0:31,"Cisco Cisco Systems, Inc"
 88:F0:77,"Cisco Cisco Systems, Inc"
 88:F2:BD,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 88:F4:88,"cellonco cellon communications technology(shenzhen)Co.,Ltd."
 88:F4:90,Jetmobil Jetmobile Pte Ltd
 88:F5:6E,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:F7:BF,"vivoMobi vivo Mobile Communication Co., Ltd."
-88:F7:C7,Technico Technicolor CH USA Inc.
+88:F7:C7,VantivaU Vantiva USA LLC
 88:F8:72,"HuaweiTe Huawei Technologies Co.,Ltd"
 88:FC:5D,"Cisco Cisco Systems, Inc"
 88:FC:A6,devolo devolo AG
 88:FD:15,"Lineeye Lineeye Co., Ltd"
 88:FE:D6,"ShangHai ShangHai WangYong Software Co., Ltd."
 8A:00:B0,"Eoptolin Eoptolink Technology Inc. Ltd,"
+8A:07:75,LyotechL Lyotech Labs Llc
 8A:0A:F7,"MontageT Montage Technology Co,.LTD"
 8A:34:BC,Fiberwor Fiberworks AS
 8A:4F:8B,Irdeto
 8A:94:AD,Nexgen Nexgen A/S
 8A:A5:C1,RanovusU Ranovus USA
 8A:B3:DA,"HomePlug HomePlug Powerline Alliance, Inc."
 8A:C7:2E,"Roku Roku, Inc."
 8A:CB:A4,Resideo
+8A:D2:0F,ProOptix Pro Optix AB
 8A:D8:5E,"GigaIONe GigaIO Networks, Inc."
 8A:DA:26,Eleven Eleven Inc.
 8A:FB:16,"TeraByte TeraByte, Inc."
 8C:00:6D,"Apple Apple, Inc."
+8C:02:CD,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 8C:02:FA,COMMANDO COMMANDO Networks Limited
 8C:04:BA,Dell Dell Inc.
-8C:04:FF,Technico Technicolor CH USA Inc.
+8C:04:FF,VantivaU Vantiva USA LLC
 8C:05:51,Koubachi Koubachi AG
 8C:06:CB,Toradex Toradex AG
 8C:07:8C,FlowData Flow Data Inc
 8C:08:8B,RemoteSo Remote Solution
 8C:09:F4,"ARRISGro ARRIS Group, Inc."
 8C:0C:87,Nokia
 8C:0C:90,RuckusWi Ruckus Wireless
@@ -35346,14 +36091,15 @@
 8C:19:2D:A0:00:00/28,TeleAlar TeleAlarm SA
 8C:19:2D:B0:00:00/28,"AbsideNe Abside Networks, Inc."
 8C:19:2D:C0:00:00/28,"YouZheng You Zhengcheng co.,ltd"
 8C:19:2D:D0:00:00/28,PyrasTec Pyras Technology Inc.
 8C:19:2D:E0:00:00/28,Elcon Elcon AB
 8C:19:B5,Arcadyan Arcadyan Corporation
 8C:1A:BF,"SamsungE Samsung Electronics Co.,Ltd"
+8C:1A:F3,"Shenzhen Shenzhen Gooxi Information Security CO.,Ltd."
 8C:1C:DA,IEEERegi IEEE Registration Authority
 8C:1C:DA:00:00:00/28,CEOS CEOS Pty Ltd
 8C:1C:DA:10:00:00/28,GESAS GESAS GmbH
 8C:1C:DA:20:00:00/28,Geomc
 8C:1C:DA:30:00:00/28,Structur Structura Technology & Innovation
 8C:1C:DA:40:00:00/28,"Anntec（B Anntec （Beijing） Technology Co.,Ltd."
 8C:1C:DA:50:00:00/28,Septentr Septentrio NV
@@ -35374,821 +36120,1125 @@
 8C:1F:64:00:30:00/36,Brighten Brighten Controls LLP
 8C:1F:64:00:90:00/36,Convergi Converging Systems Inc.
 8C:1F:64:00:C0:00/36,"GuanShow Guan Show Technologe Co., Ltd."
 8C:1F:64:01:10:00/36,DEUTA-WE DEUTA-WERKE GmbH
 8C:1F:64:01:70:00/36,Farmote Farmote Limited
 8C:1F:64:01:A0:00/36,Paragraf
 8C:1F:64:01:E0:00/36,SCIREQSc SCIREQ Scientific Respiratory Equipment Inc
+8C:1F:64:02:00:00/36,Utthunga Utthunga Techologies Pvt Ltd
 8C:1F:64:02:40:00/36,"ShinNiho Shin Nihon Denshi Co., Ltd."
+8C:1F:64:02:50:00/36,SMITEC SMITEC S.p.A.
+8C:1F:64:02:90:00/36,"HunanShe Hunan Shengyun Photoelectric Technology Co.,LTD"
 8C:1F:64:02:F0:00/36,SOLIDpow SOLIDpower SpA
+8C:1F:64:03:30:00/36,IQHomeKf IQ Home Kft.
+8C:1F:64:03:C0:00/36,SonaBusi Sona Business B.V.
 8C:1F:64:04:30:00/36,"AperNet AperNet, LLC"
 8C:1F:64:04:50:00/36,Veilux Veilux Inc.
+8C:1F:64:04:60:00/36,American American Fullway Corp.
+8C:1F:64:05:10:00/36,CPcontec CP contech electronic GmbH
+8C:1F:64:05:60:00/36,DongGuan Dong Guan Yung Fu Electronics Ltd.
 8C:1F:64:05:90:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
+8C:1F:64:05:C0:00/36,tickIoT tickIoT Inc.
 8C:1F:64:05:F0:00/36,ESCADAUT ESCAD AUTOMATION GmbH
+8C:1F:64:06:10:00/36,Micron Micron Systems
+8C:1F:64:06:B0:00/36,SanwaSup Sanwa Supply Inc.
 8C:1F:64:06:D0:00/36,Monnit Monnit Corporation
 8C:1F:64:07:10:00/36,DorletSa Dorlet Sau
 8C:1F:64:07:70:00/36,EngageTe Engage Technologies
 8C:1F:64:07:A0:00/36,Flextron Flextronics International Kft
 8C:1F:64:07:E0:00/36,FLOYD FLOYD inc.
 8C:1F:64:08:00:00/36,Twinleaf Twinleaf LLC
+8C:1F:64:08:30:00/36,Avionica
 8C:1F:64:08:50:00/36,SorbEngi Sorb Engineering Llc
 8C:1F:64:08:60:00/36,WEPTECHe WEPTECH elektronik GmbH
 8C:1F:64:08:B0:00/36,"Shanghai Shanghai Shenxu Technology Co., Ltd"
+8C:1F:64:08:D0:00/36,NeetraSb Neetra Srl Sb
 8C:1F:64:08:E0:00/36,qiio qiio AG
 8C:1F:64:08:F0:00/36,AixContr AixControl GmbH
 8C:1F:64:09:20:00/36,GogoBA Gogo BA
+8C:1F:64:09:30:00/36,MAGAudio MAG Audio LLC
+8C:1F:64:09:70:00/36,FoMa FoMa Systems GmbH
 8C:1F:64:09:80:00/36,Agvoluti Agvolution GmbH
 8C:1F:64:09:90:00/36,Pantheru Pantherun Technologies Pvt Ltd
 8C:1F:64:09:B0:00/36,Taiv
+8C:1F:64:09:D0:00/36,Flextron Flextronics International Kft
+8C:1F:64:09:E0:00/36,IWSGloba IWS Global Pty Ltd
 8C:1F:64:09:F0:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
+8C:1F:64:0A:40:00/36,"DynamicR Dynamic Research, Inc."
 8C:1F:64:0A:80:00/36,SamabaNo SamabaNova Systems
+8C:1F:64:0A:A0:00/36,Di3Infot Di3 Infotech Llp
 8C:1F:64:0A:B0:00/36,NorbitOD Norbit ODM AS
 8C:1F:64:0A:C0:00/36,"PatchTec Patch Technologies, Inc."
 8C:1F:64:0A:F0:00/36,ForseePo Forsee Power
 8C:1F:64:0B:00:00/36,"BunkaShu Bunka Shutter Co., Ltd."
+8C:1F:64:0B:60:00/36,LukeGran Luke Granger-Brown
+8C:1F:64:0B:70:00/36,Tiama
 8C:1F:64:0B:80:00/36,Signatro Signatrol Ltd
+8C:1F:64:0B:B0:00/36,"InfraChe InfraChen Technology Co., Ltd."
 8C:1F:64:0B:E0:00/36,Bnb
+8C:1F:64:0B:F0:00/36,AuroraCo Aurora Communication Technologies Corp.
 8C:1F:64:0C:00:00/36,ActiveRe Active Research Limited
 8C:1F:64:0C:50:00/36,TechnipF TechnipFMC
+8C:1F:64:0C:A0:00/36,CLOUDTEL CLOUD TELECOM Inc.
 8C:1F:64:0D:50:00/36,"RealD RealD, Inc."
 8C:1F:64:0D:60:00/36,AvdInnov Avd Innovation Limited
+8C:1F:64:0D:80:00/36,"PowerEle Power Electronics Espana, S.L."
 8C:1F:64:0E:00:00/36,Autophar Autopharma
 8C:1F:64:0E:60:00/36,"Cleanwat Cleanwatts Digital, S.A."
 8C:1F:64:0E:A0:00/36,SmartSky SmartSky Networks LLC
 8C:1F:64:0E:E0:00/36,"RichSour Rich Source Precision IND., Co., LTD."
 8C:1F:64:0E:F0:00/36,Dave Dave Srl
 8C:1F:64:0F:00:00/36,Xylon
+8C:1F:64:0F:20:00/36,Graphime Graphimecc Group SRL
+8C:1F:64:0F:40:00/36,AW-SOMTe AW-SOM Technologies LLC
+8C:1F:64:0F:50:00/36,VishayNo Vishay Nobel AB
 8C:1F:64:0F:90:00/36,ikanInte ikan International LLC
+8C:1F:64:0F:E0:00/36,IndraHee Indra Heera Technology LLP
 8C:1F:64:10:10:00/36,ASW-ATI ASW-ATI Srl
 8C:1F:64:10:30:00/36,Kronotec Kronotech Srl
 8C:1F:64:11:10:00/36,Isac Isac Srl
+8C:1F:64:11:30:00/36,Timberli Timberline Manufacturing
 8C:1F:64:11:50:00/36,Neuralog Neuralog LP
 8C:1F:64:11:70:00/36,Grossenb Grossenbacher Systeme AG
 8C:1F:64:11:80:00/36,Automata Automata GmbH & Co. KG
 8C:1F:64:11:F0:00/36,NodeUDes NodeUDesign
 8C:1F:64:12:80:00/36,YulistaI Yulista Integrated Solution
 8C:1F:64:12:B0:00/36,"BeijingT Beijing Tongtech Technology Co., Ltd."
+8C:1F:64:12:E0:00/36,inomatic inomatic GmbH
 8C:1F:64:13:30:00/36,Vtron Vtron Pty Ltd
 8C:1F:64:13:50:00/36,YuvalFic Yuval Fichman
+8C:1F:64:13:80:00/36,Vissavis Vissavi sp. z o.o.
+8C:1F:64:13:F0:00/36,Elsist Elsist Srl
 8C:1F:64:14:40:00/36,"Langfang Langfang ENN lntelligent Technology Co.,Ltd."
 8C:1F:64:14:50:00/36,Spectrum Spectrum FiftyNine BV
+8C:1F:64:14:80:00/36,Carehawk
 8C:1F:64:14:B0:00/36,PotterEl Potter Electric Signal Company
+8C:1F:64:14:D0:00/36,VerteszE Vertesz Elektronika Kft.
 8C:1F:64:15:10:00/36,GogoBusi Gogo Business Aviation
+8C:1F:64:15:40:00/36,Flextron Flextronics International Kft
 8C:1F:64:15:C0:00/36,TronFutu Tron Future Tech Inc.
 8C:1F:64:15:E0:00/36,"Dynomoti Dynomotion, Inc"
 8C:1F:64:16:40:00/36,Revo-Tec Revo - Tec GmbH
 8C:1F:64:16:60:00/36,HikariAl Hikari Alphax Inc.
 8C:1F:64:16:D0:00/36,"XiamenRg Xiamen Rgblink Science & Technology Co., Ltd."
 8C:1F:64:16:E0:00/36,Benchmar Benchmark Electronics BV
 8C:1F:64:17:70:00/36,Emcom Emcom Systems
 8C:1F:64:17:90:00/36,Agrowtek Agrowtek Inc.
 8C:1F:64:17:C0:00/36,Zelp Zelp Ltd
 8C:1F:64:17:E0:00/36,MI MI Inc.
 8C:1F:64:18:70:00/36,Sicon Sicon srl
+8C:1F:64:18:B0:00/36,M-Pulse M-Pulse GmbH & Co.KG
 8C:1F:64:19:30:00/36,Sicon Sicon srl
 8C:1F:64:19:40:00/36,Tiflex
 8C:1F:64:19:70:00/36,"TEKVOX TEKVOX, Inc"
 8C:1F:64:19:B0:00/36,FeedFlo
 8C:1F:64:19:C0:00/36,Aton Aton srl
+8C:1F:64:1A:00:00/36,EngageTe Engage Technologies
 8C:1F:64:1A:50:00/36,Dialtron Dialtronics Systems Pvt Ltd
 8C:1F:64:1A:70:00/36,aelettro aelettronica group srl
+8C:1F:64:1A:D0:00/36,NexxtoSe Nexxto Servicos Em Tecnologia da Informacao SA
 8C:1F:64:1A:F0:00/36,EnviroNo EnviroNode IoT Solutions
+8C:1F:64:1B:20:00/36,Rapid-e- Rapid-e-Engineering Steffen Kramer
 8C:1F:64:1B:50:00/36,Xicato
 8C:1F:64:1B:60:00/36,RedSenso Red Sensors Limited
 8C:1F:64:1B:70:00/36,Rax-Tech Rax-Tech International
 8C:1F:64:1B:B0:00/36,"RenweiEl Renwei Electronics Technology (Shenzhen) Co.,LTD."
 8C:1F:64:1B:D0:00/36,DorletSa Dorlet Sau
 8C:1F:64:1B:F0:00/36,Ossia Ossia Inc
 8C:1F:64:1C:00:00/36,INVENTIA INVENTIA Sp. z o.o.
 8C:1F:64:1C:20:00/36,SolidInv Solid Invent Ltda.
 8C:1F:64:1C:B0:00/36,SASYSeK SASYS e.K.
+8C:1F:64:1C:E0:00/36,"Eiden Eiden Co.,Ltd."
 8C:1F:64:1D:00:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 8C:1F:64:1D:10:00/36,ASStrömu AS Strömungstechnik GmbH
+8C:1F:64:1D:60:00/36,Zhejiang Zhejiang Qian Information & Technologies
 8C:1F:64:1D:80:00/36,Mesomat Mesomat inc.
 8C:1F:64:1D:A0:00/36,"Chongqin Chongqing Huaxiu Technology Co.,Ltd"
 8C:1F:64:1E:10:00/36,VAF VAF Co.
 8C:1F:64:1E:30:00/36,WBNet
 8C:1F:64:1E:F0:00/36,Tantroni Tantronic AG
 8C:1F:64:1F:00:00/36,AVCOMMTe AVCOMM Technologies Inc
+8C:1F:64:1F:50:00/36,NanoThin NanoThings Inc.
 8C:1F:64:1F:E0:00/36,BurkTech Burk Technology
 8C:1F:64:20:40:00/36,castcore
 8C:1F:64:20:80:00/36,SichuanA Sichuan AnSphere Technology Co. Ltd.
+8C:1F:64:20:C0:00/36,"Shanghai Shanghai Stairmed Technology Co.,ltd"
+8C:1F:64:20:E0:00/36,AlphaBri Alpha Bridge Technologies Private Limited
+8C:1F:64:21:10:00/36,"BipomEle Bipom Electronics, Inc."
 8C:1F:64:21:90:00/36,"Guangzho Guangzhou Desam Audio Co.,Ltd"
 8C:1F:64:21:C0:00/36,"EMS-Expe LLC ""EMS-Expert"""
 8C:1F:64:22:40:00/36,PHBEletr PHB Eletronica Ltda.
 8C:1F:64:22:70:00/36,Digilens
 8C:1F:64:22:E0:00/36,JideCarR Jide Car Rastreamento e Monitoramento LTDA
+8C:1F:64:23:20:00/36,Monnit Monnit Corporation
 8C:1F:64:23:D0:00/36,MokilaNe Mokila Networks Pvt Ltd
 8C:1F:64:24:00:00/36,HuiTongi HuiTong intelligence Company
 8C:1F:64:24:20:00/36,Giordano Giordano Controls Spa
+8C:1F:64:24:C0:00/36,"Shenzhen Shenzhen Link-All Technolgy Co., Ltd"
+8C:1F:64:25:10:00/36,Watchdog Watchdog Systems
 8C:1F:64:25:20:00/36,"TYTElect TYT Electronics CO., LTD"
 8C:1F:64:25:40:00/36,ZhuhaiYu Zhuhai Yunzhou Intelligence Technology Ltd.
 8C:1F:64:25:60:00/36,Landinge Landinger
 8C:1F:64:25:A0:00/36,"WuhanXin Wuhan Xingtuxinke ELectronic Co.,Ltd"
 8C:1F:64:25:C0:00/36,TimeMach TimeMachines Inc.
 8C:1F:64:25:E0:00/36,"R2Sonic R2Sonic, LLC"
+8C:1F:64:26:30:00/36,EPCPower EPC Power Corporation
 8C:1F:64:26:40:00/36,BRVossIn BR. Voss Ingenjörsfirma AB
 8C:1F:64:26:80:00/36,AstroMac Astro Machine Corporation
 8C:1F:64:26:E0:00/36,KoizumiL Koizumi Lighting Technology Corp.
 8C:1F:64:27:00:00/36,"Xi‘anHan Xi‘an Hangguang Satellite and Control Technology Co.,Ltd"
 8C:1F:64:27:40:00/36,Invixium Invixium Access Inc
+8C:1F:64:28:10:00/36,NvpTeco Nvp Teco Ltd
+8C:1F:64:28:60:00/36,i2s
+8C:1F:64:28:90:00/36,Craft4Di Craft4 Digital GmbH
 8C:1F:64:28:A0:00/36,Arcopie
 8C:1F:64:28:C0:00/36,"SakuraSe Sakura Seiki Co.,Ltd."
 8C:1F:64:28:D0:00/36,AVAMonit AVA Monitoring AB
+8C:1F:64:29:20:00/36,GogoBusi Gogo Business Aviation
+8C:1F:64:29:30:00/36,Landis+G Landis+Gyr Equipamentos de Medição Ltda
 8C:1F:64:29:60:00/36,"Roogzhit Roog zhi tong Technology(Beijing) Co.,Ltd"
 8C:1F:64:29:80:00/36,MeggerGe Megger Germany GmbH
 8C:1F:64:29:F0:00/36,Nagtech Nagtech Llc
 8C:1F:64:2A:10:00/36,Pantheru Pantherun Technologies Pvt Ltd
 8C:1F:64:2A:50:00/36,Nonet Nonet Inc
 8C:1F:64:2A:90:00/36,"ElbitAme Elbit Systems of America, LLC"
 8C:1F:64:2B:60:00/36,StercomP Stercom Power Solutions GmbH
+8C:1F:64:2B:80:00/36,Veinland Veinland GmbH
 8C:1F:64:2B:B0:00/36,ChakraTe Chakra Technology Ltd
 8C:1F:64:2C:20:00/36,TexCompu Tex Computer Srl
 8C:1F:64:2C:30:00/36,TeraDiod TeraDiode / Panasonic
 8C:1F:64:2C:50:00/36,Sysn
 8C:1F:64:2C:60:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
+8C:1F:64:2C:70:00/36,Contralt Contralto Audio Srl
 8C:1F:64:2C:80:00/36,BRSSiste BRS Sistemas Eletrônicos
+8C:1F:64:2C:B0:00/36,SmartCom Smart Component Technologies Ltd
+8C:1F:64:2C:D0:00/36,TaiwanVt Taiwan Vtron
+8C:1F:64:2D:00:00/36,Cambridg Cambridge Research Systems Ltd
 8C:1F:64:2D:80:00/36,CONTROL CONTROL SYSTEMS Srl
 8C:1F:64:2E:20:00/36,MarkRobe Mark Roberts Motion Control
+8C:1F:64:2E:30:00/36,ErbaLach Erba Lachema s.r.o.
 8C:1F:64:2E:80:00/36,SonoraNe Sonora Network Solutions
 8C:1F:64:2E:F0:00/36,Invisens Invisense AB
+8C:1F:64:2F:00:00/36,"SwitchSc Switch Science, Inc."
 8C:1F:64:2F:50:00/36,FloridaR Florida R&D Associates LLC
 8C:1F:64:2F:B0:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 8C:1F:64:2F:C0:00/36,"Unimar Unimar, Inc."
 8C:1F:64:2F:D0:00/36,Enestone Enestone Corporation
 8C:1F:64:2F:E0:00/36,"VERSITRO VERSITRON, Inc."
 8C:1F:64:30:00:00/36,AbbottDi Abbott Diagnostics Technologies AS
 8C:1F:64:30:10:00/36,Agar Agar Corporation Inc.
 8C:1F:64:30:40:00/36,JemacSwe Jemac Sweden AB
 8C:1F:64:30:60:00/36,"Corigine Corigine,Inc."
 8C:1F:64:30:90:00/36,Mect Mect Srl
 8C:1F:64:30:A0:00/36,XCOMLabs XCOM Labs
 8C:1F:64:31:40:00/36,Cedel Cedel BV
 8C:1F:64:31:60:00/36,PotterEl Potter Electric Signal Company
+8C:1F:64:31:70:00/36,BacancyL Bacancy Systems LLP
 8C:1F:64:31:A0:00/36,Asiga Asiga Pty Ltd
+8C:1F:64:31:B0:00/36,jointana joint analytical systems GmbH
 8C:1F:64:32:40:00/36,KineticT Kinetic Technologies
 8C:1F:64:32:80:00/36,"ComVideo Com Video Security Systems Co., Ltd."
+8C:1F:64:32:90:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
+8C:1F:64:32:B0:00/36,"Shenyang Shenyang Taihua Technology Co., Ltd."
+8C:1F:64:32:C0:00/36,TaikoAud Taiko Audio B.V.
 8C:1F:64:32:F0:00/36,DEUTACon DEUTA Controls GmbH
 8C:1F:64:33:00:00/36,VisionSa Vision Systems Safety Tech
+8C:1F:64:33:40:00/36,OutdoorL OutdoorLink
+8C:1F:64:34:90:00/36,WavesSys Waves System
+8C:1F:64:34:C0:00/36,"KyushuKe Kyushu Keisokki Co.,Ltd."
 8C:1F:64:34:D0:00/36,"biosilve biosilver.co.,ltd"
+8C:1F:64:35:00:00/36,"biosilve biosilver.co.,ltd"
 8C:1F:64:35:40:00/36,PaulTagl Paul Tagliamonte
+8C:1F:64:35:80:00/36,DensoMan Denso Manufacturing Tennessee
 8C:1F:64:35:C0:00/36,OpgalOpt Opgal Optronic Industries ltd
 8C:1F:64:35:D0:00/36,Security Security&Best
+8C:1F:64:36:20:00/36,"PowerEle Power Electronics Espana, S.L."
 8C:1F:64:36:50:00/36,"VectorTe Vector Technologies, Llc"
 8C:1F:64:36:60:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
+8C:1F:64:36:70:00/36,LAMTECMe LAMTEC Mess- und Regeltechnik für Feuerungen GmbH & Co. KG
+8C:1F:64:36:90:00/36,OrbitalA Orbital Astronautics Ltd
+8C:1F:64:36:A0:00/36,INVENTIS INVENTIS S.r.l.
 8C:1F:64:37:00:00/36,WOLFAdva WOLF Advanced Technology
 8C:1F:64:37:20:00/36,WINKStre WINK Streaming
 8C:1F:64:37:60:00/36,DIASInfr DIAS Infrared GmbH
+8C:1F:64:37:F0:00/36,"ScarletT Scarlet Tech Co., Ltd."
 8C:1F:64:38:20:00/36,"Shenzhen Shenzhen ROLSTONE Technology Co., Ltd"
+8C:1F:64:38:30:00/36,Tristate Tristate Electronic Mfg
 8C:1F:64:38:50:00/36,Multilan Multilane Inc
 8C:1F:64:38:70:00/36,Omnivisi Omnivision
 8C:1F:64:38:B0:00/36,BorrellU Borrell USA Corp
+8C:1F:64:38:C0:00/36,"XiamenZh Xiamen Zhixiaojin Intelligent Technology Co., Ltd"
 8C:1F:64:38:D0:00/36,WilsonEl Wilson Electronics
 8C:1F:64:38:E0:00/36,Wartsila Wartsila Voyage Limited
 8C:1F:64:39:10:00/36,CpcUk Cpc (Uk)
 8C:1F:64:39:70:00/36,IntelCor Intel Corporate
 8C:1F:64:39:80:00/36,Software Software Systems Plus
 8C:1F:64:39:A0:00/36,GoldingA Golding Audio Ltd
 8C:1F:64:39:E0:00/36,AbbottDi Abbott Diagnostics Technologies AS
+8C:1F:64:3A:20:00/36,KronMedi Kron Medidores
 8C:1F:64:3A:40:00/36,QLMTechn QLM Technology Ltd
 8C:1F:64:3A:C0:00/36,BenisonT Benison Tech
 8C:1F:64:3A:D0:00/36,TowerIQ
+8C:1F:64:3A:F0:00/36,PSATechn PSA Technology Ltda.
 8C:1F:64:3B:00:00/36,Flextron Flextronics International Kft
 8C:1F:64:3B:20:00/36,RealDigi Real Digital
 8C:1F:64:3B:50:00/36,Svms
 8C:1F:64:3B:60:00/36,TexCompu Tex Computer Srl
 8C:1F:64:3B:70:00/36,Ai-Blox
+8C:1F:64:3B:B0:00/36,ClausalC Clausal Computing Oy
 8C:1F:64:3C:40:00/36,NavSysTe NavSys Technology Inc.
 8C:1F:64:3C:50:00/36,StratisI Stratis IOT
 8C:1F:64:3C:60:00/36,Wavestre Wavestream Corp
 8C:1F:64:3C:D0:00/36,Sejongse Sejong security system Cor.
+8C:1F:64:3D:00:00/36,Tripltek
 8C:1F:64:3D:10:00/36,EMIT EMIT GmbH
 8C:1F:64:3D:40:00/36,epgElett e.p.g. Elettronica s.r.l.
+8C:1F:64:3D:50:00/36,FRAKOKon FRAKO Kondensatoren- und Anlagenbau GmbH
 8C:1F:64:3E:00:00/36,YPP YPP Corporation
 8C:1F:64:3E:30:00/36,FMTec-Fu FMTec GmbH - Future Management Technologies
 8C:1F:64:3E:80:00/36,Ruichuan Ruichuangte
 8C:1F:64:3F:40:00/36,Actelser Actelser S.L.
 8C:1F:64:3F:C0:00/36,STVElect STV Electronic GmbH
 8C:1F:64:3F:E0:00/36,Plumsp Plum sp. z.o.o.
 8C:1F:64:3F:F0:00/36,UiseeSha Uisee(Shanghai) Automotive Technologies Ltd.
+8C:1F:64:40:20:00/36,Integerp Integer.pl S.A.
 8C:1F:64:40:60:00/36,AndaTele Anda Telecom Pvt Ltd
+8C:1F:64:40:80:00/36,techones techone system
 8C:1F:64:40:C0:00/36,SichuanA Sichuan Aiyijan Technology Company Ltd.
+8C:1F:64:40:D0:00/36,PROFITT PROFITT Ltd
 8C:1F:64:40:E0:00/36,BakerHug Baker Hughes EMEA
+8C:1F:64:41:20:00/36,Comercia Comercial Electronica Studio-2 s.l.
 8C:1F:64:41:40:00/36,INSEVIS INSEVIS GmbH
 8C:1F:64:41:70:00/36,Fracarro Fracarro srl
+8C:1F:64:41:C0:00/36,KSE KSE GmbH
 8C:1F:64:41:D0:00/36,AspenSpe Aspen Spectra Sdn Bhd
+8C:1F:64:42:30:00/36,HiwinMik Hiwin Mikrosystem Corp.
 8C:1F:64:42:60:00/36,eumigind eumig industrie-TV GmbH.
 8C:1F:64:42:90:00/36,AbbottDi Abbott Diagnostics Technologies AS
 8C:1F:64:42:B0:00/36,GamberJo Gamber Johnson-LLC
 8C:1F:64:43:80:00/36,Integerp Integer.pl S.A.
+8C:1F:64:43:90:00/36,Bornico
+8C:1F:64:43:D0:00/36,SolidSta Solid State Supplies Ltd
 8C:1F:64:44:50:00/36,FigmentD Figment Design Laboratories
 8C:1F:64:44:E0:00/36,"GVALight GVA Lighting, Inc."
 8C:1F:64:44:F0:00/36,"RealD RealD, Inc."
 8C:1F:64:45:40:00/36,KJKlimat KJ Klimateknik A/S
 8C:1F:64:45:B0:00/36,"BeijingA Beijing Aoxing Technology Co.,Ltd"
 8C:1F:64:45:D0:00/36,"FuzhouTu Fuzhou Tucsen Photonics Co.,Ltd"
 8C:1F:64:45:F0:00/36,Toshniwa Toshniwal Security Solutions Pvt Ltd
 8C:1F:64:46:00:00/36,Solace Solace Systems Inc.
+8C:1F:64:46:10:00/36,KaraPart Kara Partners LLC
 8C:1F:64:46:20:00/36,Reo Reo Ag
 8C:1F:64:46:60:00/36,Intamsys Intamsys Technology Co.Ltd
 8C:1F:64:46:A0:00/36,Pharsigh Pharsighted LLC
 8C:1F:64:47:20:00/36,"SurgeNet Surge Networks, Inc."
+8C:1F:64:47:50:00/36,AlpineQu Alpine Quantum Technologies GmbH
+8C:1F:64:47:60:00/36,ClairGlo Clair Global Corporation
 8C:1F:64:47:A0:00/36,"MissingL Missing Link Electronics, Inc."
+8C:1F:64:47:D0:00/36,EbNeuro Eb Neuro Spa
 8C:1F:64:48:90:00/36,Hupi
+8C:1F:64:48:F0:00/36,Mecos Mecos AG
 8C:1F:64:49:30:00/36,"Security Security Products International, LLC"
+8C:1F:64:49:50:00/36,Dave Dave Srl
 8C:1F:64:49:80:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
+8C:1F:64:49:90:00/36,Tiama
+8C:1F:64:49:B0:00/36,Wartsila Wartsila Voyage Limited
+8C:1F:64:4A:00:00/36,Tantec Tantec A/S
 8C:1F:64:4A:C0:00/36,Vekto
 8C:1F:64:4A:E0:00/36,"KCS KCS Co., Ltd."
+8C:1F:64:4A:F0:00/36,miniDSP
 8C:1F:64:4B:00:00/36,"U-Mei-Da U -Mei-Dah Int'L Enterprise Co.,Ltd."
 8C:1F:64:4B:B0:00/36,IWSGloba IWS Global Pty Ltd
 8C:1F:64:4C:10:00/36,Clock-O- Clock-O-Matic
 8C:1F:64:4C:70:00/36,SBS SBS SpA
 8C:1F:64:4C:D0:00/36,"GuanShow Guan Show Technologe Co., Ltd."
 8C:1F:64:4D:60:00/36,DanSmith Dan Smith LLC
+8C:1F:64:4D:90:00/36,Securico Securico Electronics India Ltd
 8C:1F:64:4D:A0:00/36,DTDSTech DTDS Technology Pte Ltd
 8C:1F:64:4D:B0:00/36,Private
+8C:1F:64:4D:C0:00/36,BESOsp BESO sp. z o.o.
 8C:1F:64:4D:D0:00/36,GriffynR Griffyn Robotech Private Limited
 8C:1F:64:4E:00:00/36,PuSund PuS GmbH und Co. KG
 8C:1F:64:4E:50:00/36,RenukasC Renukas Castle Hard- and Software
 8C:1F:64:4E:70:00/36,CircuitS Circuit Solutions
+8C:1F:64:4E:90:00/36,EersGlob Eers Global Technologies Inc.
 8C:1F:64:4E:C0:00/36,XORUK XOR UK Corporation Limited
 8C:1F:64:4F:00:00/36,TielineR Tieline Research Pty Ltd
+8C:1F:64:4F:70:00/36,SmartDTe SmartD Technologies Inc
 8C:1F:64:4F:90:00/36,Photonic Photonic Science and Engineering Ltd
 8C:1F:64:4F:A0:00/36,Sanskrut Sanskruti
 8C:1F:64:4F:B0:00/36,MesaTech Mesa Technologies Llc
+8C:1F:64:50:10:00/36,QUISS QUISS GmbH
+8C:1F:64:50:20:00/36,SamwellI Samwell International Inc
 8C:1F:64:50:40:00/36,EAElektr EA Elektroautomatik GmbH & Co. KG
+8C:1F:64:50:90:00/36,SeasonEl Season Electronics Ltd
 8C:1F:64:50:A0:00/36,BellcoTr Bellco Trading Company (Pvt) Ltd
 8C:1F:64:50:E0:00/36,Panorami Panoramic Power
-8C:1F:64:51:00:00/36,NovantaN Novanta Corp / Novanta IMS
+8C:1F:64:51:00:00/36,NovantaI Novanta IMS
 8C:1F:64:51:10:00/36,ControlA Control Aut Tecnologia em Automação LTDA
 8C:1F:64:51:20:00/36,BlikSens Blik Sensing B.V.
 8C:1F:64:51:70:00/36,"SmartRad Smart Radar System, Inc"
 8C:1F:64:51:80:00/36,WagnerGr Wagner Group GmbH
 8C:1F:64:52:10:00/36,MP-SENSO MP-SENSOR GmbH
 8C:1F:64:52:50:00/36,UnitedSt United States Technologies Inc.
+8C:1F:64:52:A0:00/36,HiwinMik Hiwin Mikrosystem Corp.
 8C:1F:64:52:D0:00/36,"CubicITS Cubic ITS, Inc. dba GRIDSMART Technologies"
+8C:1F:64:52:E0:00/36,CLOUDTEL CLOUD TELECOM Inc.
 8C:1F:64:53:40:00/36,SuryaEle Surya Electronics
 8C:1F:64:53:50:00/36,Columbus Columbus McKinnon
 8C:1F:64:53:60:00/36,"BeijingL Beijing Lxtv Technology Co.,Ltd"
 8C:1F:64:53:A0:00/36,TPVision TPVision Europe B.V
 8C:1F:64:53:B0:00/36,REFUStor REFU Storage System GmbH
 8C:1F:64:53:D0:00/36,Nexconte Nexcontech
 8C:1F:64:53:F0:00/36,Velvac Velvac Incorporated
 8C:1F:64:54:20:00/36,Landis+G Landis+Gyr Equipamentos de Medição Ltda
 8C:1F:64:54:40:00/36,Tinkerbe Tinkerbee Innovations Private Limited
 8C:1F:64:54:90:00/36,BradTech Brad Technology
 8C:1F:64:54:A0:00/36,BeldenIn Belden India Private Limited
 8C:1F:64:54:C0:00/36,GeminiEl Gemini Electronics B.V.
 8C:1F:64:54:F0:00/36,"Toolplan Toolplanet Co., Ltd."
+8C:1F:64:55:00:00/36,ard ard sa
 8C:1F:64:55:20:00/36,"Proterra Proterra, Inc"
 8C:1F:64:55:30:00/36,ENIGMASO ENIGMA SOI Sp. z o.o.
 8C:1F:64:55:60:00/36,BAE BAE Systems
 8C:1F:64:55:70:00/36,In-liteD In-lite Design BV
 8C:1F:64:55:E0:00/36,Hanateks Hanateksystem
+8C:1F:64:56:00:00/36,DexterLa Dexter Laundry Inc.
 8C:1F:64:56:C0:00/36,ELTEK ELTEK SpA
 8C:1F:64:56:D0:00/36,Acod
+8C:1F:64:56:F0:00/36,AdetecSa Adetec Sas
 8C:1F:64:57:20:00/36,ZmbiziAp Zmbizi App Llc
 8C:1F:64:57:30:00/36,Ingeniou Ingenious Technology LLC
 8C:1F:64:57:50:00/36,"Yu-HengE Yu-Heng Electric Co., LTD"
 8C:1F:64:57:A0:00/36,NPOECO-I NPO ECO-INTECH Ltd.
 8C:1F:64:57:B0:00/36,PotterEl Potter Electric Signal Company
+8C:1F:64:57:D0:00/36,ISDI ISDI Ltd
 8C:1F:64:58:10:00/36,"SpectraD SpectraDynamics, Inc."
 8C:1F:64:58:C0:00/36,EarMicro Ear Micro LLC
 8C:1F:64:58:E0:00/36,NovantaI Novanta IMS
+8C:1F:64:59:10:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
+8C:1F:64:59:30:00/36,"Brillian Brillian Network & Automation Integrated System Co., Ltd."
+8C:1F:64:59:60:00/36,RFCode RF Code
+8C:1F:64:59:A0:00/36,Primaluc Primalucelab isrl
 8C:1F:64:59:F0:00/36,DeltaCom Delta Computers LLC.
 8C:1F:64:5A:C0:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
 8C:1F:64:5A:E0:00/36,"SuzhouMo Suzhou Motorcomm Electronic Technology Co., Ltd"
 8C:1F:64:5A:F0:00/36,TeqDilig Teq Diligent Product Solutions Pvt. Ltd.
 8C:1F:64:5B:30:00/36,eumigind eumig industrie-TV GmbH.
 8C:1F:64:5B:C0:00/36,Heitec Heitec Ag
+8C:1F:64:5C:90:00/36,AbbottDi Abbott Diagnostics Technologies AS
 8C:1F:64:5C:B0:00/36,dinosys
+8C:1F:64:5C:D0:00/36,MahindrM Mahindr & Mahindra
+8C:1F:64:5C:E0:00/36,Packetal Packetalk LLC
 8C:1F:64:5D:30:00/36,EloyWate Eloy Water
 8C:1F:64:5D:60:00/36,"Portrait Portrait Displays, Inc."
+8C:1F:64:5D:90:00/36,Opdi-tex Opdi-tex GmbH
+8C:1F:64:5D:A0:00/36,White2ne White2net srl
 8C:1F:64:5D:B0:00/36,GlobalIn GlobalInvacom
+8C:1F:64:5E:30:00/36,Nixer Nixer Ltd
 8C:1F:64:5E:50:00/36,Telemetr Telemetrics Inc.
+8C:1F:64:5E:70:00/36,HOSCHGeb HOSCH Gebäude Automation Neue Produkte GmbH
 8C:1F:64:5E:A0:00/36,BTGInstr BTG Instruments AB
 8C:1F:64:5E:B0:00/36,Tiama
 8C:1F:64:5F:50:00/36,HongSeok HongSeok Ltd.
 8C:1F:64:5F:70:00/36,"EagleHar Eagle Harbor Technologies, Inc."
 8C:1F:64:5F:A0:00/36,PolCamSp PolCam Systems Sp. z o.o.
 8C:1F:64:60:00:00/36,"AnhuiCha Anhui Chaokun Testing Equipment Co., Ltd"
 8C:1F:64:60:10:00/36,Camius
 8C:1F:64:60:30:00/36,"FukuEner Fuku Energy Technology Co., Ltd."
+8C:1F:64:60:50:00/36,Xacti Xacti Corporation
 8C:1F:64:60:A0:00/36,"Rfengine Rfengine Co., Ltd."
 8C:1F:64:60:E0:00/36,ICTInter ICT International
 8C:1F:64:61:00:00/36,"BeijingZ Beijing Zhongzhi Huida Technology Co., Ltd"
 8C:1F:64:61:10:00/36,SiemensI Siemens Industry Software Inc.
 8C:1F:64:61:90:00/36,Labtrino Labtrino AB
 8C:1F:64:61:C0:00/36,Automata Automata GmbH & Co. KG
 8C:1F:64:61:F0:00/36,Lightwor Lightworks GmbH
+8C:1F:64:62:00:00/36,Solace Solace Systems Inc.
 8C:1F:64:62:20:00/36,LogicalP Logical Product
 8C:1F:64:62:50:00/36,Stresste Stresstech OY
 8C:1F:64:62:60:00/36,Csiro
+8C:1F:64:62:C0:00/36,"Hangzhou Hangzhou EasyXR Advanced Technology Co., Ltd."
+8C:1F:64:62:D0:00/36,Embeddde Embeddded Plus Plus
 8C:1F:64:63:40:00/36,Aml
+8C:1F:64:63:60:00/36,EuropeTr Europe Trade
 8C:1F:64:63:80:00/36,"ThunderD Thunder Data Taiwan Co., Ltd."
 8C:1F:64:63:B0:00/36,Tiama
 8C:1F:64:63:F0:00/36,PreoIndu Preo Industries Far East Ltd
 8C:1F:64:64:10:00/36,"biosilve biosilver.co.,ltd"
 8C:1F:64:64:70:00/36,SeniorGr Senior Group LLC
+8C:1F:64:64:E0:00/36,NilfiskF Nilfisk Food
 8C:1F:64:65:00:00/36,"Ltec L tec Co.,Ltd"
+8C:1F:64:65:30:00/36,P5
 8C:1F:64:65:50:00/36,"SEI S.E.I. Co.,Ltd."
 8C:1F:64:65:60:00/36,Optotune Optotune Switzerland AG
 8C:1F:64:65:D0:00/36,ActionSt Action Streamer LLC
 8C:1F:64:65:F0:00/36,"Astromet Astrometric Instruments, Inc."
 8C:1F:64:66:00:00/36,Ntpc Llc Ntpc
 8C:1F:64:66:20:00/36,"SuzhouLe Suzhou Leamore Optronics Co., Ltd."
 8C:1F:64:66:30:00/36,mal-tech mal-tech Technological Solutions Ltd/CRISP
 8C:1F:64:66:C0:00/36,"LineageP Lineage Power Pvt Ltd.,"
+8C:1F:64:66:D0:00/36,Vt100 Vt100 Srl
 8C:1F:64:66:F0:00/36,Elix Elix Systems SA
 8C:1F:64:67:20:00/36,Farmobil Farmobile LLC
 8C:1F:64:67:50:00/36,"TransitS Transit Solutions, LLC."
 8C:1F:64:67:60:00/36,sdtnet sdt.net AG
+8C:1F:64:67:70:00/36,FreySJ Frey S.J.
 8C:1F:64:67:A0:00/36,MG MG s.r.l.
 8C:1F:64:67:C0:00/36,EnstoPro Ensto Protrol AB
+8C:1F:64:67:E0:00/36,LDAAudio LDA Audiotech
 8C:1F:64:67:F0:00/36,Hamamats Hamamatsu Photonics K.K.
 8C:1F:64:68:30:00/36,Slat
 8C:1F:64:68:50:00/36,SancharC Sanchar Communication Systems
+8C:1F:64:69:10:00/36,WendeTan Wende Tan
 8C:1F:64:69:20:00/36,NexilisE Nexilis Electronics India Pvt Ltd (PICSYS)
 8C:1F:64:69:70:00/36,Sontay Sontay Ltd.
 8C:1F:64:69:80:00/36,Arcus-ED Arcus-EDS GmbH
 8C:1F:64:69:90:00/36,FIDICA FIDICA GmbH & Co. KG
 8C:1F:64:69:E0:00/36,AT-Autom AT-Automation Technology GmbH
 8C:1F:64:6A:00:00/36,Avionica
 8C:1F:64:6A:80:00/36,Bulwark
 8C:1F:64:6A:D0:00/36,PotterEl Potter Electric Signal Company
 8C:1F:64:6A:E0:00/36,BrayInte Bray International
+8C:1F:64:6B:10:00/36,Speciali Specialist Mechanical Engineers (PTY)LTD
 8C:1F:64:6B:30:00/36,Feritech Feritech Ltd.
 8C:1F:64:6B:50:00/36,O-NetCom O-Net Communications(Shenzhen)Limited
 8C:1F:64:6B:90:00/36,GSIndust GS Industrie-Elektronik GmbH
 8C:1F:64:6B:B0:00/36,SeasonEl Season Electronics Ltd
 8C:1F:64:6C:60:00/36,Fit
+8C:1F:64:6C:B0:00/36,GJDManuf GJD Manufacturing
 8C:1F:64:6C:D0:00/36,"WuhanXin Wuhan Xingtuxinke ELectronic Co.,Ltd"
 8C:1F:64:6C:F0:00/36,Italora
 8C:1F:64:6D:00:00/36,Abb
 8C:1F:64:6D:50:00/36,HTKHambu HTK Hamburg GmbH
+8C:1F:64:6D:90:00/36,Khimo
+8C:1F:64:6E:20:00/36,"SCU SCU Co., Ltd."
 8C:1F:64:6E:30:00/36,ViewSoni ViewSonic International Corporation
+8C:1F:64:6E:40:00/36,RABMicro RAB Microfluidics R&D Company Ltd
 8C:1F:64:6E:A0:00/36,KMtronic KMtronic ltd
 8C:1F:64:6E:C0:00/36,"BitTrade Bit Trade One, Ltd."
 8C:1F:64:6F:40:00/36,Elsist Elsist Srl
 8C:1F:64:6F:90:00/36,Anddoro Anddoro Llc
 8C:1F:64:6F:C0:00/36,HM HM Systems A/S
 8C:1F:64:70:00:00/36,Quantafl Quantaflow
 8C:1F:64:70:20:00/36,AIDirect AIDirections
 8C:1F:64:70:30:00/36,CalnexSo Calnex Solutions plc
 8C:1F:64:70:70:00/36,Oas Oas Ag
 8C:1F:64:70:80:00/36,Zuum
 8C:1F:64:70:E0:00/36,OvercomT OvercomTech
 8C:1F:64:71:20:00/36,NexionDa Nexion Data Systems P/L
+8C:1F:64:71:B0:00/36,Adasky Adasky Ltd.
 8C:1F:64:72:10:00/36,MSMilind M/S Milind Ramachandra Rajwade
+8C:1F:64:72:30:00/36,Celestic Celestica Inc.
 8C:1F:64:72:60:00/36,Dave Dave Srl
 8C:1F:64:72:A0:00/36,DorletSa Dorlet Sau
 8C:1F:64:72:C0:00/36,"Antaitec Antai technology Co.,Ltd"
 8C:1F:64:73:10:00/36,"ehoosys ehoosys Co.,LTD."
+8C:1F:64:73:30:00/36,VideoNet Video Network Security
 8C:1F:64:73:70:00/36,Vytahy-V Vytahy-Vymyslicky s.r.o.
 8C:1F:64:73:90:00/36,Monnit Monnit Corporation
 8C:1F:64:73:B0:00/36,FinkZeit Fink Zeitsysteme GmbH
 8C:1F:64:73:C0:00/36,Reo Reo Ag
 8C:1F:64:73:D0:00/36,NewAgeMi NewAgeMicro
 8C:1F:64:73:F0:00/36,Ubiscale
 8C:1F:64:74:00:00/36,"Norvento Norvento Tecnología, S.L."
 8C:1F:64:74:40:00/36,ChaseoCo Chaseo Connectome
 8C:1F:64:74:60:00/36,SensusHe Sensus Healthcare
 8C:1F:64:74:70:00/36,VisionTI VisionTIR Multispectral Technology
+8C:1F:64:74:E0:00/36,OpenPark OpenPark Technologies Kft
+8C:1F:64:75:60:00/36,StarInte Star Systems International Limited
 8C:1F:64:75:F0:00/36,ASTRACOM ASTRACOM Co. Ltd
 8C:1F:64:76:40:00/36,nanoTRON nanoTRONIX Computing Inc.
 8C:1F:64:76:50:00/36,MicroEle Micro Electroninc Products
 8C:1F:64:76:80:00/36,mapnagro mapna group
 8C:1F:64:77:40:00/36,navXperi navXperience GmbH
 8C:1F:64:77:50:00/36,BectonDi Becton Dickinson
+8C:1F:64:77:70:00/36,Sicon Sicon srl
+8C:1F:64:77:B0:00/36,DbSas Db Sas
 8C:1F:64:77:C0:00/36,OrangeTr Orange Tree Technologies Ltd
 8C:1F:64:77:E0:00/36,"Institut Institute of geophysics, China earthquake administration"
+8C:1F:64:77:F0:00/36,TargaSys TargaSystem S.r.L.
 8C:1F:64:78:00:00/36,"HME HME Co.,ltd"
 8C:1F:64:78:20:00/36,Atm Atm Llc
 8C:1F:64:78:70:00/36,Tabology
 8C:1F:64:78:F0:00/36,Connecti Connection Systems
+8C:1F:64:79:30:00/36,Aditec Aditec GmbH
+8C:1F:64:79:70:00/36,AlbanGia Alban Giacomo S.p.a.
 8C:1F:64:79:B0:00/36,Foerster Foerster-Technik GmbH
 8C:1F:64:79:D0:00/36,"MurataMa Murata Manufacturing Co., Ltd."
 8C:1F:64:79:E0:00/36,AccemicT Accemic Technologies GmbH
+8C:1F:64:79:F0:00/36,HiwinMik Hiwin Mikrosystem Corp.
 8C:1F:64:7A:10:00/36,Guardian Guardian Controls International Ltd
 8C:1F:64:7A:40:00/36,Hirotech Hirotech inc.
 8C:1F:64:7A:60:00/36,OTMetric
 8C:1F:64:7A:70:00/36,Timegate Timegate Instruments Ltd.
 8C:1F:64:7A:A0:00/36,XSENSORT XSENSOR Technology Corp.
+8C:1F:64:7A:E0:00/36,D-E-K D-E-K GmbH & Co.KG
 8C:1F:64:7A:F0:00/36,EVisionI E Vision India Pvt Ltd
 8C:1F:64:7B:00:00/36,AxidSyst Axid System
+8C:1F:64:7B:10:00/36,EAElektr EA Elektro-Automatik
 8C:1F:64:7B:50:00/36,"GuanShow Guan Show Technologe Co., Ltd."
 8C:1F:64:7B:60:00/36,Keyline Keyline S.P.A.
 8C:1F:64:7B:70:00/36,Weidmann Weidmann Tecnologia Electrica de Mexico
 8C:1F:64:7B:80:00/36,TimeMach TimeMachines Inc.
 8C:1F:64:7B:90:00/36,Devicero Deviceroy
 8C:1F:64:7B:C0:00/36,GOdevelo GO development GmbH
+8C:1F:64:7C:70:00/36,AsconTec Ascon Tecnologic S.r.l.
 8C:1F:64:7C:80:00/36,JacquetD Jacquet Dechaume
 8C:1F:64:7C:F0:00/36,Transdig Transdigital Pty Ltd
 8C:1F:64:7D:20:00/36,Enlaps
 8C:1F:64:7D:30:00/36,SuntechE Suntech Engineering
+8C:1F:64:7D:40:00/36,Penteon Penteon Corporation
 8C:1F:64:7D:60:00/36,AlgodueE Algodue Elettronica Srl
 8C:1F:64:7D:80:00/36,"HIROSAWA HIROSAWA ELECTRIC Co.,Ltd."
 8C:1F:64:7D:90:00/36,Noisewav Noisewave Corporation
+8C:1F:64:7D:C0:00/36,"LineageP Lineage Power Pvt Ltd.,"
 8C:1F:64:7D:D0:00/36,"TAKASAKI TAKASAKI KYODO COMPUTING CENTER Co.,LTD."
 8C:1F:64:7D:E0:00/36,SOCNOCAI SOCNOC AI Inc
 8C:1F:64:7E:00:00/36,"ColomboS Colombo Sales & Engineering, Inc."
 8C:1F:64:7E:20:00/36,AaronnEl Aaronn Electronic GmbH
 8C:1F:64:7E:70:00/36,robertju robert juliat
 8C:1F:64:7E:C0:00/36,Methods2 Methods2Business B.V.
 8C:1F:64:7E:E0:00/36,OrangePr Orange Precision Measurement LLC
 8C:1F:64:7F:10:00/36,AEMSinga AEM Singapore Pte Ltd
 8C:1F:64:80:10:00/36,"Zhejiang Zhejiang Laolan Information Technology Co., Ltd"
+8C:1F:64:80:30:00/36,MOSCAEle MOSCA Elektronik und Antriebstechnik GmbH
 8C:1F:64:80:70:00/36,Giordano Giordano Controls Spa
+8C:1F:64:81:00:00/36,Kymata Kymata Srl
+8C:1F:64:81:10:00/36,Panorami Panoramic Power
 8C:1F:64:81:70:00/36,nkemarin nke marine electronics
 8C:1F:64:81:A0:00/36,GeminiEl Gemini Electronics B.V.
 8C:1F:64:82:00:00/36,Tiama
 8C:1F:64:82:50:00/36,MTUAeroE MTU Aero Engines AG
+8C:1F:64:82:F0:00/36,AnySigna AnySignal
+8C:1F:64:83:00:00/36,Vtron Vtron Pty Ltd
 8C:1F:64:83:70:00/36,"runZero runZero, Inc"
+8C:1F:64:83:80:00/36,Drimaes Drimaes Inc.
 8C:1F:64:83:A0:00/36,Grossenb Grossenbacher Systeme AG
 8C:1F:64:83:C0:00/36,XtendTec Xtend Technologies Pvt Ltd
+8C:1F:64:83:D0:00/36,L-signat L-signature
 8C:1F:64:83:E0:00/36,Sicon Sicon srl
 8C:1F:64:84:20:00/36,PotterEl Potter Electric Signal Co. LLC
 8C:1F:64:84:80:00/36,Jena-Opt Jena-Optronik GmbH
+8C:1F:64:84:A0:00/36,Bitmappe Bitmapper Integration Technologies Private Limited
 8C:1F:64:84:C0:00/36,AvMapsrl AvMap srlu
 8C:1F:64:84:E0:00/36,"WestPhar West Pharmaceutical Services, Inc."
 8C:1F:64:85:20:00/36,Abb
 8C:1F:64:85:50:00/36,ekundens e.kundenservice Netz GmbH
 8C:1F:64:85:60:00/36,GartenAu Garten Automation
 8C:1F:64:85:B0:00/36,Atlantic Atlantic Pumps Ltd
+8C:1F:64:86:30:00/36,EngiNe EngiNe srl
 8C:1F:64:86:70:00/36,ForeverE Forever Engineering Systems Pvt. Ltd.
 8C:1F:64:86:A0:00/36,VisionTo VisionTools Bildanalyse Systeme GmbH
 8C:1F:64:87:80:00/36,GreenAcc Green Access Ltd
+8C:1F:64:87:90:00/36,ASHIDAEl ASHIDA Electronics Pvt. Ltd
+8C:1F:64:88:00:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 8C:1F:64:88:20:00/36,TmyTechn Tmy Technology Inc.
 8C:1F:64:88:30:00/36,DEUTA-WE DEUTA-WERKE GmbH
 8C:1F:64:88:B0:00/36,"TaiwanAu Taiwan Aulisa Medical Devices Technologies, Inc"
 8C:1F:64:88:D0:00/36,Pantheru Pantherun Technologies Pvt Ltd
+8C:1F:64:88:E0:00/36,"CubeWork CubeWorks, Inc."
 8C:1F:64:89:00:00/36,"WonATech WonATech Co., Ltd."
 8C:1F:64:89:20:00/36,MDIIndus MDI Industrial
+8C:1F:64:89:50:00/36,DacomWes Dacom West GmbH
+8C:1F:64:89:80:00/36,CopperCo Copper Connections Ltd
+8C:1F:64:89:90:00/36,American American Edge IP
 8C:1F:64:89:E0:00/36,Cinetix Cinetix Srl
 8C:1F:64:8A:40:00/36,GenesisT Genesis Technologies AG
+8C:1F:64:8A:80:00/36,Massachu Massachusetts Institute of Technology
 8C:1F:64:8A:90:00/36,"GuanShow Guan Show Technologe Co., Ltd."
 8C:1F:64:8A:A0:00/36,ForeverE Forever Engineering Systems Pvt. Ltd.
 8C:1F:64:8A:C0:00/36,"BOZHONPr BOZHON Precision Industry Technology Co.,Ltd"
 8C:1F:64:8A:E0:00/36,"Shenzhen Shenzhen Qunfang Technology Co., LTD."
 8C:1F:64:8A:F0:00/36,Ibeos
 8C:1F:64:8B:50:00/36,AshtonBe Ashton Bentley Collaboration Spaces
+8C:1F:64:8B:80:00/36,WienEner Wien Energie GmbH
 8C:1F:64:8B:90:00/36,ZynexMon Zynex Monitoring Solutions
 8C:1F:64:8C:20:00/36,"Cirrus Cirrus Systems, Inc."
 8C:1F:64:8C:40:00/36,HermesNe Hermes Network Inc
 8C:1F:64:8C:50:00/36,NextTMic NextT Microwave Inc
 8C:1F:64:8C:F0:00/36,Diffract Diffraction Limited
+8C:1F:64:8D:00:00/36,Enerthin Enerthing GmbH
 8C:1F:64:8D:10:00/36,OrlacoPr Orlaco Products B.V.
 8C:1F:64:8D:40:00/36,RecabSwe Recab Sweden AB
 8C:1F:64:8D:50:00/36,Agramkow Agramkow A/S
 8C:1F:64:8D:90:00/36,PietroFi Pietro Fiorentini Spa
+8C:1F:64:8D:A0:00/36,Dart Dart Systems Ltd
 8C:1F:64:8D:E0:00/36,IconetSe Iconet Services
+8C:1F:64:8D:F0:00/36,Grossenb Grossenbacher Systeme AG
 8C:1F:64:8E:20:00/36,ALPHA ALPHA Corporation
+8C:1F:64:8E:30:00/36,"UniTikTe UniTik Technology Co., Limited"
 8C:1F:64:8E:50:00/36,Druck Druck Ltd.
+8C:1F:64:8E:80:00/36,"Cominfo Cominfo, Inc."
 8C:1F:64:8E:90:00/36,Vesperix Vesperix Corporation
+8C:1F:64:8E:B0:00/36,NumaProd Numa Products LLC
 8C:1F:64:8E:E0:00/36,AbbottDi Abbott Diagnostics Technologies AS
 8C:1F:64:8F:40:00/36,Loadrite Loadrite (Auckland) Limited
+8C:1F:64:8F:60:00/36,IdneoTec Idneo Technologies S.A.U.
 8C:1F:64:8F:80:00/36,HIGHVOLT HIGHVOLT Prüftechnik
 8C:1F:64:90:30:00/36,"Portrait Portrait Displays, Inc."
 8C:1F:64:90:50:00/36,Qualitro Qualitrol LLC
+8C:1F:64:90:70:00/36,Sicon Sicon srl
 8C:1F:64:90:90:00/36,Matelex
+8C:1F:64:90:C0:00/36,CoolAir Cool Air Incorporated
 8C:1F:64:90:D0:00/36,AlgodueE Algodue Elettronica Srl
 8C:1F:64:90:E0:00/36,Xacti Xacti Corporation
 8C:1F:64:90:F0:00/36,BELIMOAu BELIMO Automation AG
 8C:1F:64:91:10:00/36,Eolane
 8C:1F:64:91:80:00/36,AbbottDi Abbott Diagnostics Technologies AS
 8C:1F:64:91:A0:00/36,Profcon Profcon AB
+8C:1F:64:91:B0:00/36,PotterEl Potter Electric Signal Co. LLC
 8C:1F:64:91:D0:00/36,enlighte enlighten
 8C:1F:64:92:30:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
+8C:1F:64:92:40:00/36,MagicsTe Magics Technologies
+8C:1F:64:92:80:00/36,ITG ITG Co.Ltd
 8C:1F:64:92:A0:00/36,ThermoOn Thermo Onix Ltd
 8C:1F:64:92:D0:00/36,"IVORInte IVOR Intelligent Electrical Appliance Co., Ltd"
 8C:1F:64:93:10:00/36,Noptel Noptel Oy
 8C:1F:64:93:90:00/36,"SPITTech SPIT Technology, Inc"
 8C:1F:64:94:30:00/36,Autark Autark GmbH
 8C:1F:64:94:60:00/36,"UniJet UniJet Co., Ltd."
 8C:1F:64:94:70:00/36,"TCVympel LLC ""TC ""Vympel"""
 8C:1F:64:94:90:00/36,tickIoT tickIoT Inc.
 8C:1F:64:94:C0:00/36,Bcmtech
 8C:1F:64:94:E0:00/36,Monnit Monnit Corporation
 8C:1F:64:95:60:00/36,Paulmann Paulmann Licht GmbH
 8C:1F:64:95:80:00/36,SancharT Sanchar Telesystems limited
 8C:1F:64:95:A0:00/36,"Shenzhen Shenzhen Longyun Lighting Electric Appliances Co., Ltd"
+8C:1F:64:96:30:00/36,GogoBusi Gogo Business Aviation
 8C:1F:64:96:70:00/36,Dave Dave Srl
 8C:1F:64:96:80:00/36,IavEngin Iav Engineering Sarl
 8C:1F:64:97:10:00/36,Infrasaf Infrasafe/ Advantor Systems
 8C:1F:64:97:30:00/36,DorsettT Dorsett Technologies Inc
+8C:1F:64:97:80:00/36,PlanetIn Planet Innovation Products Inc.
 8C:1F:64:97:C0:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 8C:1F:64:97:D0:00/36,KSE KSE GmbH
+8C:1F:64:97:F0:00/36,Talleres Talleres de Escoriaza SA
 8C:1F:64:98:40:00/36,AbacusPe Abacus Peripherals Pvt Ltd
+8C:1F:64:98:90:00/36,Phe-nX Phe-nX B.V.
+8C:1F:64:98:C0:00/36,PANBusin PAN Business & Consulting (ANYOS]
 8C:1F:64:98:F0:00/36,BreasMed Breas Medical AB
 8C:1F:64:99:10:00/36,DBSystel DB Systel GmbH
 8C:1F:64:99:80:00/36,EVLOStoc EVLO Stockage Énergie
+8C:1F:64:99:E0:00/36,EIDOS EIDOS s.r.l.
+8C:1F:64:9A:10:00/36,"PacificS Pacific Software Development Co., Ltd."
 8C:1F:64:9A:40:00/36,LabLogic LabLogic Systems
+8C:1F:64:9A:50:00/36,Xi‘anShe Xi‘an Shengxin Science& Technology Development Co.?Ltd.
 8C:1F:64:9A:60:00/36,"Institut Instituto De Gestão, Redes Tecnológicas E Nergias"
 8C:1F:64:9A:B0:00/36,Dave Dave Srl
 8C:1F:64:9B:20:00/36,EmersonR Emerson Rosemount Analytical
 8C:1F:64:9B:30:00/36,Böckelt Böckelt GmbH
 8C:1F:64:9B:60:00/36,GSElektr GS Elektromedizinsiche Geräte G. Stemple GmbH
 8C:1F:64:9B:A0:00/36,WintusSy Wintus System
 8C:1F:64:9B:D0:00/36,AtmSolut Atm Solutions
 8C:1F:64:9B:F0:00/36,ArgusEye ArgusEye TECH. INC
 8C:1F:64:9C:00:00/36,HeaderRh Header Rhyme
 8C:1F:64:9C:10:00/36,RealWear
 8C:1F:64:9C:30:00/36,CamozziA Camozzi Automation SpA
+8C:1F:64:9C:B0:00/36,"Shanghai Shanghai Sizhong Information Technology Co., Ltd"
 8C:1F:64:9C:E0:00/36,ExiFlowM Exi Flow Measurement Ltd
 8C:1F:64:9C:F0:00/36,ASAPElec ASAP Electronics GmbH
 8C:1F:64:9D:40:00/36,Wolfspyr Wolfspyre Labs
 8C:1F:64:9D:80:00/36,Integerp Integer.pl S.A.
+8C:1F:64:9E:00:00/36,Druck Druck Ltd.
+8C:1F:64:9E:20:00/36,Technolo Technology for Energy Corp
+8C:1F:64:9E:60:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 8C:1F:64:9E:80:00/36,GHMMesst GHM Messtechnik GmbH
+8C:1F:64:9E:C0:00/36,Speciali Specialized Communications Corp.
 8C:1F:64:9F:00:00/36,"ePlant ePlant, Inc."
 8C:1F:64:9F:20:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 8C:1F:64:9F:40:00/36,Grossenb Grossenbacher Systeme AG
+8C:1F:64:9F:50:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
+8C:1F:64:9F:60:00/36,VisionSa Vision Systems Safety Tech
 8C:1F:64:9F:A0:00/36,METRONA- METRONA-Union GmbH
+8C:1F:64:9F:B0:00/36,CiIsrael Ci Systems Israel Ltd
 8C:1F:64:9F:D0:00/36,VishayNo Vishay Nobel AB
 8C:1F:64:9F:E0:00/36,Metroval Metroval Controle de Fluidos Ltda
 8C:1F:64:9F:F0:00/36,Satelles Satelles Inc
 8C:1F:64:A0:00:00/36,BITECHNI BITECHNIK GmbH
 8C:1F:64:A0:10:00/36,"GuanShow Guan Show Technologe Co., Ltd."
 8C:1F:64:A0:70:00/36,GJDManuf GJD Manufacturing
 8C:1F:64:A0:A0:00/36,"Shanghai Shanghai Wise-Tech Intelligent Technology Co.,Ltd."
+8C:1F:64:A0:D0:00/36,Lumiplan Lumiplan Duhamel
 8C:1F:64:A1:B0:00/36,Zilica Zilica Limited
 8C:1F:64:A2:90:00/36,Ringtail Ringtail Security
 8C:1F:64:A2:B0:00/36,WENetVie WENet Vietnam Joint Stock company
 8C:1F:64:A2:D0:00/36,ACSL ACSL Ltd.
+8C:1F:64:A3:10:00/36,ZingComm Zing Communications Inc
 8C:1F:64:A3:20:00/36,Nautel Nautel LTD
+8C:1F:64:A3:40:00/36,PotterEl Potter Electric Signal Co. LLC
+8C:1F:64:A3:60:00/36,"Dongguan Dongguan Gago Electronics Co.,Ltd"
 8C:1F:64:A3:80:00/36,NuGridPo NuGrid Power
+8C:1F:64:A3:B0:00/36,"FujianSa Fujian Satlink Electronics Co., Ltd"
+8C:1F:64:A3:F0:00/36,ViewSoni ViewSonic Corp
 8C:1F:64:A4:20:00/36,RodgersI Rodgers Instruments US LLC
 8C:1F:64:A4:40:00/36,Rapidev Rapidev Pvt Ltd
 8C:1F:64:A4:C0:00/36,Flextron Flextronics International Kft
 8C:1F:64:A4:E0:00/36,SyscomIn Syscom Instruments SA
 8C:1F:64:A5:10:00/36,Babtel
+8C:1F:64:A5:60:00/36,Flextron Flextronics International Kft
 8C:1F:64:A5:70:00/36,EkspertS EkspertStroyProekt
 8C:1F:64:A5:C0:00/36,Prosys
 8C:1F:64:A5:D0:00/36,"Shenzhen Shenzhen zhushida Technology lnformation Co.,Ltd"
+8C:1F:64:A5:E0:00/36,XTIA XTIA Ltd.
 8C:1F:64:A6:00:00/36,"ActiveOp Active Optical Systems, LLC"
 8C:1F:64:A6:A0:00/36,SphereCo Sphere Com Services Pvt Ltd
 8C:1F:64:A6:D0:00/36,"CyberneX CyberneX Co., Ltd"
+8C:1F:64:A6:E0:00/36,"shenzhen shenzhen beswave co.,ltd"
+8C:1F:64:A7:00:00/36,V-teknik V-teknik Elektronik AB
 8C:1F:64:A7:60:00/36,DEUTA-WE DEUTA-WERKE GmbH
+8C:1F:64:A7:70:00/36,Rax-Tech Rax-Tech International
+8C:1F:64:A8:10:00/36,3Dpercep 3D perception AS
+8C:1F:64:A8:30:00/36,EkspertS EkspertStroyProekt
 8C:1F:64:A8:40:00/36,"BeijingW Beijing Wenrise Technology Co., Ltd."
+8C:1F:64:A9:10:00/36,Infiniti Infinitive Group Limited
 8C:1F:64:A9:40:00/36,Futurewa Future wave ultra tech Company
 8C:1F:64:A9:70:00/36,Integerp Integer.pl S.A.
 8C:1F:64:A9:A0:00/36,Signasys Signasystems Elektronik San. ve Tic. Ltd. Sti.
 8C:1F:64:A9:C0:00/36,UpstartP Upstart Power
 8C:1F:64:A9:E0:00/36,OptimumI Optimum Instruments Inc.
+8C:1F:64:AA:30:00/36,PeterHub Peter Huber Kaeltemaschinenbau AG
 8C:1F:64:AA:40:00/36,HEINENEL HEINEN ELEKTRONIK GmbH
 8C:1F:64:AA:80:00/36,axelife
+8C:1F:64:AA:A0:00/36,LederEle Leder Elektronik Design GmbH
 8C:1F:64:AA:B0:00/36,"BlueSwor BlueSword Intelligent Technology Co., Ltd."
 8C:1F:64:AB:40:00/36,"BeijingZ Beijing Zhongchen Microelectronics Co.,Ltd"
 8C:1F:64:AB:50:00/36,Justmorp Justmorph Pte. Ltd.
 8C:1F:64:AB:70:00/36,"MClavis MClavis Co.,Ltd."
 8C:1F:64:AC:00:00/36,AIQuatro
 8C:1F:64:AC:30:00/36,WavesSys Waves System
 8C:1F:64:AC:40:00/36,comelec
 8C:1F:64:AC:50:00/36,ForeverE Forever Engineering Systems Pvt. Ltd.
+8C:1F:64:AC:90:00/36,"ShenYang ShenYang LeShun Technology Co.,Ltd"
 8C:1F:64:AC:E0:00/36,RayhaanN Rayhaan Networks
+8C:1F:64:AD:00:00/36,Elektrot Elektrotechnik & Elektronik Oltmann GmbH
 8C:1F:64:AD:20:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
+8C:1F:64:AD:40:00/36,Flextron Flextronics International Kft
+8C:1F:64:AD:80:00/36,NovantaI Novanta IMS
 8C:1F:64:AE:10:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
+8C:1F:64:AE:50:00/36,"Ltec Ltec Co.,Ltd"
 8C:1F:64:AE:80:00/36,AdetecSa Adetec Sas
 8C:1F:64:AE:A0:00/36,"INHEMETE INHEMETER Co.,Ltd"
 8C:1F:64:AE:D0:00/36,MBconnec MB connect line GmbH Fernwartungssysteme
 8C:1F:64:AE:F0:00/36,Scenario Scenario Automation
 8C:1F:64:AF:00:00/36,MinebeaM MinebeaMitsumi Inc.
 8C:1F:64:AF:50:00/36,SanminaI Sanmina Israel Medical Systems Ltd
 8C:1F:64:AF:70:00/36,ard ard sa
 8C:1F:64:AF:D0:00/36,Universa Universal Robots A/S
+8C:1F:64:AF:F0:00/36,Qtechnol Qtechnology A/S
 8C:1F:64:B0:10:00/36,noah
 8C:1F:64:B0:30:00/36,"Shenzhen Shenzhen Pisoftware Technology Co.,Ltd."
 8C:1F:64:B0:80:00/36,CronusEl Cronus Electronics
 8C:1F:64:B0:C0:00/36,Barkodes Barkodes Bilgisayar Sistemleri Bilgi Iletisim ve Y
 8C:1F:64:B0:F0:00/36,HKCSecur HKC Security Ltd.
 8C:1F:64:B1:00:00/36,MTUAeroE MTU Aero Engines AG
 8C:1F:64:B1:30:00/36,Abode Abode Systems Inc
 8C:1F:64:B1:40:00/36,"MurataMa Murata Manufacturing CO., Ltd."
 8C:1F:64:B2:20:00/36,Blighter Blighter Surveillance Systems Ltd
 8C:1F:64:B2:B0:00/36,RhombusE Rhombus Europe
 8C:1F:64:B2:C0:00/36,SanminaI Sanmina Israel Medical Systems Ltd
+8C:1F:64:B2:F0:00/36,Mtechnol Mtechnology - Gamma Commerciale Srl
+8C:1F:64:B3:60:00/36,Pneumax Pneumax Spa
 8C:1F:64:B3:B0:00/36,Sicon Sicon srl
 8C:1F:64:B3:D0:00/36,"RealD RealD, Inc."
 8C:1F:64:B4:60:00/36,Phygital Phygitall Soluções Em Internet Das Coisas
 8C:1F:64:B4:C0:00/36,PicocomT Picocom Technology Ltd
 8C:1F:64:B5:50:00/36,SancharT Sanchar Telesystems limited
 8C:1F:64:B5:60:00/36,Arcvideo
 8C:1F:64:B6:40:00/36,GSPSprac GSP Sprachtechnologie GmbH
+8C:1F:64:B6:50:00/36,HomyHubS HomyHub SL
 8C:1F:64:B6:70:00/36,"M2Mcraft M2M craft Co., Ltd."
+8C:1F:64:B6:80:00/36,AllElect All-Systems Electronics Pty Ltd
 8C:1F:64:B6:90:00/36,"Quanxing Quanxing Tech Co.,LTD"
+8C:1F:64:B6:D0:00/36,Andy-L Andy-L Ltd
+8C:1F:64:B6:E0:00/36,LoopTech Loop Technologies
 8C:1F:64:B7:30:00/36,"Comm-enc Comm-ence, Inc."
 8C:1F:64:B7:70:00/36,Carestre Carestream Dental LLC
 8C:1F:64:B7:B0:00/36,Gateview Gateview Technologies
 8C:1F:64:B7:C0:00/36,"EvernetT Evernet Co,.Ltd Taiwan"
+8C:1F:64:B7:D0:00/36,Scheuric Scheurich GmbH
 8C:1F:64:B8:20:00/36,"SeedCore Seed Core Co., LTD."
 8C:1F:64:B8:40:00/36,SPXFlowT SPX Flow Technology
 8C:1F:64:B8:D0:00/36,"Tongyeln Tongye lnnovation Science and Technology (Shenzhen) Co.,Ltd"
 8C:1F:64:B9:20:00/36,Neurable
 8C:1F:64:B9:70:00/36,GeminiEl Gemini Electronics B.V.
 8C:1F:64:B9:A0:00/36,"QuercusT Quercus Technologies, S.L."
 8C:1F:64:B9:E0:00/36,"PowerEle Power Electronics Espana, S.L."
 8C:1F:64:BA:30:00/36,DEUTA-WE DEUTA-WERKE GmbH
+8C:1F:64:BB:30:00/36,ZarucTec Zaruc Tecnologia LTDA
+8C:1F:64:BB:C0:00/36,Liberato Liberator Pty Ltd
 8C:1F:64:BB:F0:00/36,Retency
 8C:1F:64:BC:00:00/36,GSElektr GS Elektromedizinsiche Geräte G. Stemple GmbH
+8C:1F:64:BC:10:00/36,"CominTec CominTech, LLC"
 8C:1F:64:BC:20:00/36,HuzElect Huz Electronics Ltd
 8C:1F:64:BC:30:00/36,FoxIoT FoxIoT OÜ
 8C:1F:64:BC:60:00/36,"ChengduZ Chengdu ZiChen Time&Frequency Technology Co.,Ltd"
+8C:1F:64:BC:90:00/36,"GlTech Gl Tech Co.,Ltd"
 8C:1F:64:BC:B0:00/36,A&T A&T Corporation
 8C:1F:64:BC:C0:00/36,SoundHea Sound Health Systems
 8C:1F:64:BD:30:00/36,IOMaster IO Master Technology
 8C:1F:64:BD:60:00/36,NOVAProd NOVA Products GmbH
 8C:1F:64:BD:70:00/36,UnionEle Union Electronic.
+8C:1F:64:BD:B0:00/36,Cardinal Cardinal Scales Manufacturing Co
 8C:1F:64:BE:80:00/36,Technolo Technologies Bacmove Inc.
 8C:1F:64:BE:E0:00/36,Sirius Sirius LLC
 8C:1F:64:BF:00:00/36,Newtec Newtec A/S
+8C:1F:64:BF:10:00/36,SohaJin Soha Jin
 8C:1F:64:BF:30:00/36,Alphatek Alphatek AS
 8C:1F:64:BF:40:00/36,FluidCom Fluid Components Intl
 8C:1F:64:BF:B0:00/36,TechArgo TechArgos
 8C:1F:64:C0:10:00/36,HoribaAb Horiba Abx Sas
 8C:1F:64:C0:30:00/36,AbimanEn Abiman Engineering
 8C:1F:64:C0:40:00/36,Sanwa Sanwa Corporation
 8C:1F:64:C0:50:00/36,SkyCell SkyCell AG
+8C:1F:64:C0:60:00/36,TardisTe Tardis Technology
 8C:1F:64:C0:70:00/36,HYOSUNGH HYOSUNG Heavy Industries Corporation
 8C:1F:64:C0:C0:00/36,Giordano Giordano Controls Spa
+8C:1F:64:C0:D0:00/36,AbbottDi Abbott Diagnostics Technologies AS
 8C:1F:64:C0:E0:00/36,Goodtech Goodtech AS dep Fredrikstad
 8C:1F:64:C1:20:00/36,PHYSEC PHYSEC GmbH
+8C:1F:64:C1:E0:00/36,VaSyd Va Syd
 8C:1F:64:C1:F0:00/36,Esys Esys Srl
 8C:1F:64:C2:40:00/36,Alifax Alifax S.r.l.
 8C:1F:64:C2:70:00/36,"LiftVent Lift Ventures, Inc"
 8C:1F:64:C2:80:00/36,TornadoS Tornado Spectral Systems Inc.
 8C:1F:64:C2:F0:00/36,"PowerEle Power Electronics Espana, S.L."
 8C:1F:64:C3:50:00/36,PeterHub Peter Huber Kaeltemaschinenbau AG
 8C:1F:64:C3:80:00/36,Eco-Adap Eco-Adapt
 8C:1F:64:C3:A0:00/36,"YUSURTec YUSUR Technology Co., Ltd."
 8C:1F:64:C4:00:00/36,Sciospec Sciospec Scientific Instruments GmbH
 8C:1F:64:C4:10:00/36,Katronic Katronic AG & Co. KG
+8C:1F:64:C4:20:00/36,SdOptics Sd Optics
 8C:1F:64:C4:40:00/36,SyprisEl Sypris Electronics
+8C:1F:64:C4:A0:00/36,SGiTechn SGi Technology Group Ltd.
 8C:1F:64:C4:C0:00/36,Lumiplan Lumiplan Duhamel
 8C:1F:64:C5:00:00/36,Spacee
 8C:1F:64:C5:10:00/36,EPCEnerg EPC Energy Inc
 8C:1F:64:C5:20:00/36,Invendis Invendis Technologies India Pvt Ltd
 8C:1F:64:C5:40:00/36,FirstMod First Mode
 8C:1F:64:C5:70:00/36,Strategi Strategic Robotic Systems
+8C:1F:64:C5:90:00/36,Tunstall Tunstall A/S
+8C:1F:64:C5:D0:00/36,AlfaProx Alfa Proxima d.o.o.
 8C:1F:64:C6:10:00/36,"BeijingC Beijing Ceresdate Technology Co.,LTD"
+8C:1F:64:C6:40:00/36,Ajeco Ajeco Oy
 8C:1F:64:C6:80:00/36,FibermeC Fiberme Communications Llc
+8C:1F:64:C6:A0:00/36,RedPhase Red Phase Technologies Limited
 8C:1F:64:C6:B0:00/36,Mediana
+8C:1F:64:C7:10:00/36,Yaviar Yaviar LLC
 8C:1F:64:C7:C0:00/36,MERKLESc MERKLE Schweissanlagen-Technik GmbH
 8C:1F:64:C8:00:00/36,VECOSEur VECOS Europe B.V.
 8C:1F:64:C8:10:00/36,TaolinkT Taolink Technologies Corporation
+8C:1F:64:C8:50:00/36,PotterEl Potter Electric Signal Co. LLC
 8C:1F:64:C8:F0:00/36,JWFroehl JW Froehlich Maschinenfabrik GmbH
 8C:1F:64:C9:10:00/36,SoehnleI Soehnle Industrial Solutions GmbH
 8C:1F:64:C9:70:00/36,Magnet-P Magnet-Physik Dr. Steingroever GmbH
 8C:1F:64:CA:10:00/36,Pantheru Pantherun Technologies Pvt Ltd
 8C:1F:64:CA:60:00/36,"ReliaSpe ReliaSpeak Information Technology Co., Ltd."
+8C:1F:64:CA:70:00/36,eumigind eumig industrie-TV GmbH.
+8C:1F:64:CA:B0:00/36,SpyderCo Spyder Controls Corp.
 8C:1F:64:CA:D0:00/36,GeneralM General Motors
 8C:1F:64:CA:F0:00/36,BRSSiste BRS Sistemas Eletrônicos
 8C:1F:64:CB:20:00/36,DyncirSo Dyncir Soluções Tecnológicas Ltda
+8C:1F:64:CB:50:00/36,Gamber-J Gamber-Johnson LLC
+8C:1F:64:CB:70:00/36,"ARKRAYKy ARKRAY,Inc.Kyoto Laboratory"
 8C:1F:64:CB:E0:00/36,CircaEnt Circa Enterprises Inc
 8C:1F:64:CC:10:00/36,VITREASm VITREA Smart Home Technologies Ltd.
+8C:1F:64:CC:20:00/36,"Toyogike Toyogiken Co.,Ltd."
+8C:1F:64:CC:50:00/36,PotterEl Potter Electric Signal Co. LLC
 8C:1F:64:CC:60:00/36,GeniusVi Genius Vision Digital Private Limited
 8C:1F:64:CC:B0:00/36,"suzhouyu suzhou yuecrown Electronic Technology Co.,LTD"
 8C:1F:64:CD:30:00/36,Pionierk Pionierkraft GmbH
 8C:1F:64:CD:60:00/36,USM USM Pty Ltd
 8C:1F:64:CD:80:00/36,GogoBusi Gogo Business Aviation
 8C:1F:64:CD:90:00/36,Fingoti Fingoti Limited
 8C:1F:64:CD:B0:00/36,European European Telecommunication International Kft
 8C:1F:64:CD:F0:00/36,CanwayTe Canway Technology GmbH
 8C:1F:64:CE:30:00/36,PixelDes Pixel Design & Manufacturing Sdn. Bhd.
+8C:1F:64:CE:40:00/36,"SlUsa Sl Usa, Llc"
 8C:1F:64:CE:B0:00/36,EurekaFo Eureka For Smart Properties Co. W.L.L
 8C:1F:64:CE:E0:00/36,Displax Displax S.A.
 8C:1F:64:CE:F0:00/36,"GoertekR Goertek Robotics Co.,Ltd."
 8C:1F:64:CF:10:00/36,"ROBOfibe ROBOfiber, Inc."
 8C:1F:64:CF:30:00/36,ABB ABB S.p.A.
 8C:1F:64:CF:40:00/36,Nt
 8C:1F:64:CF:70:00/36,BusPas
 8C:1F:64:CF:A0:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
 8C:1F:64:D0:20:00/36,Flextron Flextronics International Kft
 8C:1F:64:D0:80:00/36,"PowerEle Power Electronics Espana, S.L."
 8C:1F:64:D0:E0:00/36,Labforge Labforge Inc.
 8C:1F:64:D1:30:00/36,EYatskoI EYatsko Individual
 8C:1F:64:D2:00:00/36,NASEngin NAS Engineering PRO
+8C:1F:64:D2:10:00/36,AmetekCt Ametek Cts Gmbh
+8C:1F:64:D2:40:00/36,R3IoT R3 IoT Ltd.
 8C:1F:64:D2:90:00/36,SecureBi Secure Bits
 8C:1F:64:D2:A0:00/36,AnteusKf Anteus Kft.
 8C:1F:64:D3:A0:00/36,AppliedM Applied Materials
 8C:1F:64:D3:C0:00/36,"KIBEnerg ""KIB Energo"" LLC"
 8C:1F:64:D4:00:00/36,BreasMed Breas Medical AB
+8C:1F:64:D4:20:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
 8C:1F:64:D4:40:00/36,MonarchI Monarch Instrument
+8C:1F:64:D4:60:00/36,End2EndT End 2 End Technologies
 8C:1F:64:D4:A0:00/36,Caproc Caproc Oy
+8C:1F:64:D5:10:00/36,"ZIGENLig ZIGEN Lighting Solution co., ltd."
 8C:1F:64:D5:20:00/36,Critical Critical Software SA
 8C:1F:64:D5:30:00/36,Gridnt
 8C:1F:64:D5:40:00/36,GrupoEpe Grupo Epelsa S.L.
 8C:1F:64:D5:60:00/36,WisdomAu Wisdom Audio
 8C:1F:64:D5:B0:00/36,LocalSec Local Security
 8C:1F:64:D5:E0:00/36,Integerp Integer.pl S.A.
 8C:1F:64:D6:90:00/36,ADiCo ADiCo Corporation
+8C:1F:64:D6:C0:00/36,Packetal Packetalk LLC
+8C:1F:64:D7:30:00/36,BRSSiste BRS Sistemas Eletrônicos
+8C:1F:64:D7:40:00/36,TexCompu Tex Computer Srl
 8C:1F:64:D7:80:00/36,"HunanOus Hunan Oushi Electronic Technology Co.,Ltd"
 8C:1F:64:D7:C0:00/36,"QuercusT Quercus Technologies, S.L."
 8C:1F:64:D7:E0:00/36,ThalesBe Thales Belgium
+8C:1F:64:D7:F0:00/36,Fibersto Fiberstory communications Pvt Ltd
+8C:1F:64:D8:10:00/36,Mitsubis Mitsubishi Electric India Pvt. Ltd.
 8C:1F:64:D8:80:00/36,Universi University of Geneva - Department of Particle Physics
+8C:1F:64:D8:F0:00/36,DEUTA-WE DEUTA-WERKE GmbH
 8C:1F:64:D9:20:00/36,Mitsubis Mitsubishi Electric India Pvt. Ltd.
+8C:1F:64:D9:30:00/36,AlgodueE Algodue Elettronica Srl
+8C:1F:64:D9:80:00/36,Gnewtekp Gnewtek photoelectric technology Ltd.
 8C:1F:64:D9:A0:00/36,"BeijingR Beijing Redlink Information Technology Co., Ltd."
+8C:1F:64:D9:B0:00/36,GiSmbH GiS mbH
+8C:1F:64:D9:C0:00/36,"Relcom Relcom, Inc."
+8C:1F:64:DA:60:00/36,"PowerEle Power Electronics Espana, S.L."
 8C:1F:64:DA:A0:00/36,Davetech Davetech Limited
 8C:1F:64:DA:E0:00/36,Maincoau Mainco automotion s.l.
 8C:1F:64:DA:F0:00/36,"ZhuhaiLo Zhuhai Lonl electric Co.,Ltd"
 8C:1F:64:DB:50:00/36,victtron
 8C:1F:64:DB:70:00/36,Lambda Lambda Systems Inc.
 8C:1F:64:DB:90:00/36,ErmesEle Ermes Elettronica s.r.l.
 8C:1F:64:DB:D0:00/36,Giordano Giordano Controls Spa
 8C:1F:64:DC:00:00/36,PigsCanF Pigs Can Fly Labs LLC
+8C:1F:64:DC:20:00/36,ProconEl Procon Electronics Pty Ltd
 8C:1F:64:DC:90:00/36,PeterHub Peter Huber Kaeltemaschinenbau AG
 8C:1F:64:DC:A0:00/36,Porschee Porsche engineering
+8C:1F:64:DD:40:00/36,"Midlands Midlands Technical Co., Ltd."
 8C:1F:64:DD:50:00/36,Cardinal Cardinal Scales Manufacturing Co
 8C:1F:64:DD:70:00/36,KSTtechn KST technology
+8C:1F:64:DD:E0:00/36,JemacSwe Jemac Sweden AB
 8C:1F:64:DE:10:00/36,FrankeAq Franke Aquarotter GmbH
 8C:1F:64:DF:80:00/36,WittraNe Wittra Networks AB
+8C:1F:64:DF:A0:00/36,Atse Atse Llc
+8C:1F:64:DF:B0:00/36,Bobeesc Bobeesc Co.
+8C:1F:64:DF:C0:00/36,"MeikoEle Meiko Electronics Co.,Ltd."
 8C:1F:64:DF:E0:00/36,Nuvation Nuvation Energy
 8C:1F:64:E0:20:00/36,ITSTekni ITS Teknik A/S
 8C:1F:64:E0:E0:00/36,Nokeval Nokeval Oy
+8C:1F:64:E1:00:00/36,Scenario Scenario Automation
+8C:1F:64:E1:20:00/36,PixusTec Pixus Technologies Inc.
+8C:1F:64:E1:E0:00/36,Flextron Flextronics International Kft
 8C:1F:64:E2:10:00/36,LG-LHTAi LG-LHT Aircraft Solutions GmbH
+8C:1F:64:E2:30:00/36,ChemitoI Chemito Infotech PVT LTD
+8C:1F:64:E2:40:00/36,CometaSa Cometa Sas
 8C:1F:64:E2:D0:00/36,Private
 8C:1F:64:E3:00:00/36,VMuktiSo VMukti Solutions Private Limited
 8C:1F:64:E4:10:00/36,Grossenb Grossenbacher Systeme AG
 8C:1F:64:E4:30:00/36,Daedalea Daedalean AG
 8C:1F:64:E4:60:00/36,Nautel Nautel LTD
 8C:1F:64:E4:90:00/36,SamwellI Samwell International Inc
+8C:1F:64:E4:B0:00/36,Algazira Algazira Telecom Solutions
 8C:1F:64:E4:C0:00/36,"TTCTELEK TTC TELEKOMUNIKACE, s.r.o."
 8C:1F:64:E5:20:00/36,LcmVeloc LcmVeloci ApS
+8C:1F:64:E5:30:00/36,TProjeMu T Proje Muhendislik Dis Tic. Ltd. Sti.
 8C:1F:64:E5:C0:00/36,Scientif Scientific Lightning Solutions
 8C:1F:64:E5:D0:00/36,JinYuanI JinYuan International Corporation
 8C:1F:64:E5:E0:00/36,BRICKMAK BRICKMAKERS GmbH
 8C:1F:64:E6:10:00/36,StangeEl Stange Elektronik GmbH
 8C:1F:64:E6:20:00/36,Axcend
 8C:1F:64:E6:40:00/36,Indefac Indefac company
 8C:1F:64:E7:30:00/36,GTRIndus GTR Industries
+8C:1F:64:E7:40:00/36,Magosys Magosys Systems LTD
+8C:1F:64:E7:50:00/36,StercomP Stercom Power Soltions GmbH
 8C:1F:64:E7:70:00/36,Gy-FxSas Gy-Fx Sas
 8C:1F:64:E7:B0:00/36,Dongguan Dongguan Pengchen Earth Instrument CO. LT
 8C:1F:64:E7:C0:00/36,"AshinneT Ashinne Technology Co., Ltd"
 8C:1F:64:E8:60:00/36,ComVetia ComVetia AG
+8C:1F:64:E8:D0:00/36,Plura
+8C:1F:64:E8:F0:00/36,"JieChuan JieChuang HeYi(Beijing) Technology Co., Ltd."
 8C:1F:64:E9:00:00/36,MHEElect MHE Electronics
+8C:1F:64:E9:20:00/36,EAElektr EA Elektro-Automatik
 8C:1F:64:E9:40:00/36,ZinTechn Zin Technologies
 8C:1F:64:E9:80:00/36,Luxshare Luxshare Electronic Technology (Kunshan) LTD
 8C:1F:64:E9:90:00/36,Pantheru Pantherun Technologies Pvt Ltd
 8C:1F:64:EA:80:00/36,ZumbachE Zumbach Electronic AG
 8C:1F:64:EA:A0:00/36,"KBModul ""KB ""Modul"", LLC"
 8C:1F:64:EA:C0:00/36,"MiracleH Miracle Healthcare, Inc."
 8C:1F:64:EB:20:00/36,AquaBroa Aqua Broadcast Ltd
 8C:1F:64:EB:50:00/36,MeiryoDe Meiryo Denshi Corp.
 8C:1F:64:EB:70:00/36,DeltaSol Delta Solutions LLC
 8C:1F:64:EB:90:00/36,KxSTechn KxS Technologies Oy
 8C:1F:64:EB:F0:00/36,"STEAMIQ STEAMIQ, Inc."
 8C:1F:64:EC:10:00/36,Actronik Actronika SAS
+8C:1F:64:EC:C0:00/36,BaldwinJ Baldwin Jimek AB
+8C:1F:64:EC:F0:00/36,Monnit Monnit Corporation
 8C:1F:64:ED:40:00/36,"Zhejiang Zhejiang Chitic-Safeway New Energy Technical Co.,Ltd."
 8C:1F:64:ED:90:00/36,NetgenHi Netgen Hitech Solutions Llp
+8C:1F:64:ED:A0:00/36,DEUTA-WE DEUTA-WERKE GmbH
 8C:1F:64:EE:00:00/36,Private
+8C:1F:64:EE:10:00/36,PuSund PuS GmbH und Co. KG
 8C:1F:64:EE:60:00/36,Lynkx
 8C:1F:64:EE:80:00/36,GlobalOr Global Organ Group B.V.
 8C:1F:64:EE:A0:00/36,Amess
 8C:1F:64:EE:F0:00/36,"AiUnion AiUnion Co.,Ltd"
 8C:1F:64:EF:10:00/36,BiotageG Biotage Gb Ltd
+8C:1F:64:EF:50:00/36,SigmaDef Sigma Defense Systems LLC
 8C:1F:64:EF:80:00/36,Northwes Northwest Central Indiana Community Partnerships Inc dba Wabash Heartland Innovation Network (WHIN)
 8C:1F:64:EF:B0:00/36,"Warecube Warecube,Inc"
 8C:1F:64:F0:40:00/36,"IoTSecur IoTSecure, LLC"
 8C:1F:64:F0:90:00/36,TexiAS Texi AS
 8C:1F:64:F1:00:00/36,GSPSprac GSP Sprachtechnologie GmbH
 8C:1F:64:F1:20:00/36,CAITRON CAITRON GmbH
 8C:1F:64:F2:20:00/36,VoyageAu Voyage Audio LLC
 8C:1F:64:F2:30:00/36,IDEXIndi IDEX India Pvt Ltd
+8C:1F:64:F2:40:00/36,Albotron Albotronic
 8C:1F:64:F2:50:00/36,"MisakaNe Misaka Network, Inc."
 8C:1F:64:F2:70:00/36,Tesat-Sp Tesat-Spacecom GmbH & Co. KG
 8C:1F:64:F2:C0:00/36,Tunstall Tunstall A/S
 8C:1F:64:F2:D0:00/36,HUERNERS HUERNER Schweisstechnik GmbH
 8C:1F:64:F2:F0:00/36,QuantumT Quantum Technologies Inc
 8C:1F:64:F3:10:00/36,Internat International Water Treatment Maritime AS
 8C:1F:64:F3:20:00/36,"Shenzhen Shenzhen INVT Electric Co.,Ltd"
 8C:1F:64:F3:90:00/36,"WeinanWi Weinan Wins Future Technology Co.,Ltd"
-8C:1F:64:F3:B0:00/36,???????? ??????????
+8C:1F:64:F3:B0:00/36,"BeijingR Beijing REMANG Technology Co., Ltd."
 8C:1F:64:F3:C0:00/36,Microlyn Microlynx Systems Ltd
 8C:1F:64:F3:D0:00/36,ByteLabG Byte Lab Grupa d.o.o.
 8C:1F:64:F3:F0:00/36,"Industri Industrial Laser Machines, LLC"
 8C:1F:64:F4:10:00/36,Automati Automatizacion Y Conectividad Sa De Cv
 8C:1F:64:F4:30:00/36,wtec wtec GmbH
 8C:1F:64:F4:50:00/36,Jbf
+8C:1F:64:F4:C0:00/36,inomatic inomatic GmbH
 8C:1F:64:F4:E0:00/36,ADAMCZEW ADAMCZEWSKI elektronische Messtechnik GmbH
+8C:1F:64:F5:00:00/36,VigorEle Vigor Electric Corp.
 8C:1F:64:F5:20:00/36,AMFMedic AMF Medical SA
+8C:1F:64:F5:30:00/36,BeckmanC Beckman Coulter Inc
 8C:1F:64:F5:60:00/36,KC5Inter KC5 International Sdn Bhd
 8C:1F:64:F5:70:00/36,EAElektr EA Elektro-Automatik
 8C:1F:64:F5:90:00/36,Inovonic Inovonics Inc.
 8C:1F:64:F5:A0:00/36,TelcoAnt Telco Antennas Pty Ltd
 8C:1F:64:F5:B0:00/36,"SemaConn SemaConnect, Inc"
 8C:1F:64:F5:C0:00/36,Flextron Flextronics International Kft
+8C:1F:64:F5:F0:00/36,TR7Siber TR7 Siber Savunma A.S.
+8C:1F:64:F6:30:00/36,QuantumM Quantum Media Systems
 8C:1F:64:F6:50:00/36,Talleres Talleres de Escoriaza SA
 8C:1F:64:F7:00:00/36,VisionSa Vision Systems Safety Tech
 8C:1F:64:F7:20:00/36,Contrade Contrader
 8C:1F:64:F7:40:00/36,GEAVICCi GE AVIC Civil Avionics Systems Company Limited
 8C:1F:64:F7:80:00/36,TernaryR Ternary Research Corporation
+8C:1F:64:F7:90:00/36,"YUYAMAMF YUYAMA MFG Co.,Ltd"
 8C:1F:64:F7:A0:00/36,"SiEngine SiEngine Technology Co., Ltd."
+8C:1F:64:F8:40:00/36,KSTtechn KST technology
 8C:1F:64:F8:60:00/36,"INFOSTEC INFOSTECH Co., Ltd."
 8C:1F:64:F9:40:00/36,EAElektr EA Elektroautomatik GmbH & Co. KG
 8C:1F:64:F9:60:00/36,SACOCont SACO Controls Inc.
 8C:1F:64:F9:E0:00/36,"DREAMSWE DREAMSWELL Technology CO.,Ltd"
 8C:1F:64:FA:20:00/36,"AZDPraha AZD Praha s.r.o., ZOZ Olomouc"
+8C:1F:64:FA:40:00/36,"ChinaInf China Information Technology Designing &Consulting Institute Co.,Ltd."
 8C:1F:64:FA:80:00/36,Unitron Unitron Systems b.v.
 8C:1F:64:FA:A0:00/36,MassarNe Massar Networks
 8C:1F:64:FB:00:00/36,MARIAN MARIAN GmbH
 8C:1F:64:FB:10:00/36,Abb
 8C:1F:64:FB:40:00/36,ThalesNe Thales Nederland BV
 8C:1F:64:FB:50:00/36,BavariaD Bavaria Digital Technik GmbH
 8C:1F:64:FB:70:00/36,GraceDes Grace Design/Lunatec LLC
@@ -36196,16 +37246,21 @@
 8C:1F:64:FB:D0:00/36,"SAN-AIEl SAN-AI Electronic Industries Co.,Ltd."
 8C:1F:64:FC:20:00/36,IOContro I/O Controls
 8C:1F:64:FC:C0:00/36,Gredmann Gredmann Taiwan Ltd.
 8C:1F:64:FC:D0:00/36,elbit-EW elbit systems - EW and sigint - Elisra
 8C:1F:64:FD:10:00/36,Edgeware Edgeware AB
 8C:1F:64:FD:30:00/36,"SmilicsT Smilics Technologies, S.L."
 8C:1F:64:FD:40:00/36,EmbsysSi Embsys Sistemas Embarcados
+8C:1F:64:FD:50:00/36,"WHYHOWDO THE WHY HOW DO COMPANY, Inc."
+8C:1F:64:FD:70:00/36,"BeijingY Beijing Yahong Century Technology Co., Ltd"
+8C:1F:64:FD:C0:00/36,Nuphoton Nuphoton Technologies
 8C:1F:64:FE:00:00/36,PotterEl Potter Electric Signal Company
+8C:1F:64:FE:20:00/36,"VUVAnaly VUV Analytics, Inc."
 8C:1F:64:FE:30:00/36,"PowerEle Power Electronics Espana, S.L."
+8C:1F:64:FE:90:00/36,AlzajelM Alzajel Modern Telecommunication
 8C:1F:64:FE:D0:00/36,GSPSprac GSP Sprachtechnologie GmbH
 8C:1F:64:FF:40:00/36,SMSgroup SMS group GmbH
 8C:1F:64:FF:60:00/36,AsconTec Ascon Tecnologic S.r.l.
 8C:1F:64:FF:C0:00/36,Invendis Invendis Technologies India Pvt Ltd
 8C:1F:94,RFSurgic RF Surgical System Inc.
 8C:21:0A,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 8C:25:05,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -36226,14 +37281,15 @@
 8C:35:79,QDIQOSp QDIQO Sp. z o.o.
 8C:35:92,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 8C:36:7A,PaloAlto Palo Alto Networks
 8C:39:5C,Bit4id Bit4id Srl
 8C:3A:7E,"Universa Universal Electronics, Inc."
 8C:3A:E3,LGElectr LG Electronics (Mobile Communications)
 8C:3B:32,Microfan Microfan B.V.
+8C:3B:4A,"Universa Universal Global Scientific Industrial Co., Ltd."
 8C:3B:AD,Netgear
 8C:3C:07,"SkivaTec Skiva Technologies, Inc."
 8C:3C:4A,NAKAYO NAKAYO Inc
 8C:3D:B1,"BeijingH Beijing H-IoT Technology Co., Ltd."
 8C:41:F2,RDATechn RDA Technologies Ltd.
 8C:41:F4,IPmotion IPmotion GmbH
 8C:42:6D,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -36245,15 +37301,15 @@
 8C:47:6E:00:00:00/28,Chipsafe Chipsafer Pte. Ltd.
 8C:47:6E:10:00:00/28,TelWare TelWare Corporation
 8C:47:6E:20:00:00/28,"HuiZhouM HuiZhou MIKI Communication Equipment Co.,LTD"
 8C:47:6E:30:00:00/28,"Shanghai Shanghai Satellite Communication Technology Co.,Ltd"
 8C:47:6E:40:00:00/28,"Shenzhen Shenzhen Juding Electronics Co., Ltd."
 8C:47:6E:50:00:00/28,Square Square Inc.
 8C:47:6E:60:00:00/28,OxfordNa Oxford Nanopore Technologies Ltd.
-8C:47:6E:70:00:00/28,Private
+8C:47:6E:70:00:00/28,"Syng Syng, Inc."
 8C:47:6E:80:00:00/28,IntelliV IntelliVIX Co. Ltd.
 8C:47:6E:90:00:00/28,Xertifie Xertified AB
 8C:47:6E:A0:00:00/28,AUOptron AU Optronics Corporation
 8C:47:6E:B0:00:00/28,FaravidC Faravid Communication&Data Analysis
 8C:47:6E:C0:00:00/28,EdgeNetw Edge Networks Inc
 8C:47:6E:D0:00:00/28,innolect innolectric AG
 8C:47:6E:E0:00:00/28,Annapurn Annapurna labs
@@ -36285,14 +37341,15 @@
 8C:51:09:B0:00:00/28,"BeijingS Beijing Superhexa Century Technology Co., Ltd."
 8C:51:09:C0:00:00/28,SpotterR SpotterRF LLC
 8C:51:09:D0:00:00/28,"Surpedia Surpedia Technologies Co., Ltd."
 8C:51:09:E0:00:00/28,IROOTELL IROOTELLUCKY Corp.
 8C:52:19,SHARP SHARP Corporation
 8C:53:C3,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 8C:53:D2,"ChinaMob China Mobile Group Device Co.,Ltd."
+8C:53:E6,WistronN Wistron Neweb Corporation
 8C:53:F7,"A&DEngin A&D Engineering Co., Ltd."
 8C:54:1D,Lge
 8C:55:4A,IntelCor Intel Corporate
 8C:55:BB,"SongwooI Songwoo Information & Technology Co., Ltd"
 8C:56:46,LGElectr LG Electronics
 8C:56:9D,ImagingS Imaging Solutions Group
 8C:56:C5,"Nintendo Nintendo Co., Ltd."
@@ -36322,14 +37379,30 @@
 8C:5A:25,"ARRISGro ARRIS Group, Inc."
 8C:5A:C1,"HuaweiDe Huawei Device Co., Ltd."
 8C:5A:F0,Exeltech Exeltech Solar Products
 8C:5A:F8,"BeijingX Beijing Xiaomi Electronics Co., Ltd."
 8C:5B:F0,"ARRISGro ARRIS Group, Inc."
 8C:5C:A1,"d-broad d-broad,INC"
 8C:5D:60,"UCI UCI Corporation Co.,Ltd."
+8C:5D:B2,IEEERegi IEEE Registration Authority
+8C:5D:B2:00:00:00/28,NppNtt Npp Ntt Llc
+8C:5D:B2:10:00:00/28,Dayouplu Dayouplus
+8C:5D:B2:20:00:00/28,F+Networ F+ Networks
+8C:5D:B2:30:00:00/28,"YuzhouZh Yuzhou Zhongnan lnformation Technology Co.,Ltd"
+8C:5D:B2:40:00:00/28,CoreTigo
+8C:5D:B2:50:00:00/28,UniteAud Unite Audio
+8C:5D:B2:60:00:00/28,SmartMor SmartMore Corporation Limited
+8C:5D:B2:70:00:00/28,Cleartex Cleartex s.r.o.
+8C:5D:B2:80:00:00/28,"Guangzho Guangzhou Phimax Electronic Technology Co.,Ltd"
+8C:5D:B2:90:00:00/28,Issendor Issendorff Kg
+8C:5D:B2:A0:00:00/28,"BeijingS Beijing Scistor Technologies Co., Ltd"
+8C:5D:B2:B0:00:00/28,Naddod
+8C:5D:B2:C0:00:00/28,"HEXINTec HEXIN Technologies Co., Ltd."
+8C:5D:B2:D0:00:00/28,"Guandong Guandong Yuhang Automation Technology Co.,Ltd"
+8C:5D:B2:E0:00:00/28,SurbhiSa Surbhi Satcom Pvt Ltd
 8C:5E:BD,"HuaweiDe Huawei Device Co., Ltd."
 8C:5F:48,Continen Continental Intelligent Transportation Systems LLC
 8C:5F:AD,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 8C:5F:DF,BeijingR Beijing Railway Signal Factory
 8C:60:4F,"Cisco Cisco Systems, Inc"
 8C:60:78,Swissbit Swissbit AG
 8C:60:E7,"Mpgio Mpgio Co.,Ltd"
@@ -36340,32 +37413,35 @@
 8C:64:A2,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 8C:64:D4,"HyecoSma Hyeco Smart Tech Co.,Ltd"
 8C:67:94,"vivoMobi vivo Mobile Communication Co., Ltd."
 8C:68:3A,"HuaweiTe Huawei Technologies Co.,Ltd"
 8C:68:78,Nortek-A Nortek-AS
 8C:68:C8,zte zte corporation
 8C:6A:3B,"SamsungE Samsung Electronics Co.,Ltd"
-8C:6A:8D,Technico Technicolor CH USA Inc.
+8C:6A:8D,VantivaU Vantiva USA LLC
 8C:6A:E4,Viogem Viogem Limited
 8C:6B:DB,"HuaweiDe Huawei Device Co., Ltd."
 8C:6D:50,Shenzhen Shenzhen Mtc Co Ltd
 8C:6D:77,"HuaweiTe Huawei Technologies Co.,Ltd"
 8C:6D:C4,Megapixe Megapixel VR
+8C:6F:B9,SiliconL Silicon Laboratories
 8C:70:5A,IntelCor Intel Corporate
 8C:70:86,Gesellsc Gesellschaft für Sonder-EDV-Anlagen mbH
 8C:71:F8,"SamsungE Samsung Electronics Co.,Ltd"
 8C:73:6E,Fujitsu Fujitsu Limited
 8C:73:A0,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 8C:76:3F,"ARRISGro ARRIS Group, Inc."
 8C:76:C1,GodenTec Goden Tech Limited
 8C:77:12,"SamsungE Samsung Electronics Co.,Ltd"
 8C:77:16,Longchee Longcheer Telecommunication Limited
 8C:78:D7,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
+8C:79:09,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 8C:79:67,zte zte corporation
 8C:79:F5,"SamsungE Samsung Electronics Co.,Ltd"
+8C:7A:00,Nokia
 8C:7A:15,RuckusWi Ruckus Wireless
 8C:7A:3D,XiaomiCo Xiaomi Communications Co Ltd
 8C:7A:AA,"Apple Apple, Inc."
 8C:7B:9D,"Apple Apple, Inc."
 8C:7B:F0,XufengDe Xufeng Development Limited
 8C:7C:92,"Apple Apple, Inc."
 8C:7C:B5,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
@@ -36449,20 +37525,21 @@
 8C:B0:E9,"SamsungE Samsung Electronics.,LTD"
 8C:B6:4F,"Cisco Cisco Systems, Inc"
 8C:B7:F7,"Shenzhen Shenzhen UniStrong Science & Technology Co., Ltd"
 8C:B8:2C,IPitomyC IPitomy Communications
 8C:B8:4A,SamsungE Samsung Electro-Mechanics(Thailand)
 8C:B8:64,AcSiPTec AcSiP Technology Corp.
 8C:B8:7E,IntelCor Intel Corporate
-8C:BA:25,"Unionman Unionman Technology Co.,Ltd"
+8C:BA:25,"UnionMan Union Man Technology Co.,Ltd"
 8C:BE:24,"TashangS Tashang Semiconductor(Shanghai) Co., Ltd."
 8C:BE:BE,XiaomiCo Xiaomi Communications Co Ltd
 8C:BF:9D,Shanghai Shanghai Xinyou Information Technology Ltd. Co.
 8C:BF:A6,"SamsungE Samsung Electronics Co.,Ltd"
 8C:C1:21,Panasoni Panasonic Corporation AVC Networks Company
+8C:C5:8C,"ShenZhen ShenZhen Elsky Technology Co.,LTD"
 8C:C5:B4,Sagemcom Sagemcom Broadband SAS
 8C:C5:E1,"ShenZhen ShenZhen Konka Telecommunication Technology Co.,Ltd"
 8C:C6:61,"Currentp Current, powered by GE"
 8C:C6:81,IntelCor Intel Corporate
 8C:C7:AA,RadinetC Radinet Communications Inc.
 8C:C7:C3,NetlinkI Netlink Ict
 8C:C7:D0,"zhejiang zhejiang ebang communication co.,ltd"
@@ -36480,40 +37557,45 @@
 8C:C8:F4:80:00:00/28,Strongby Strongbyte Solutions Limited
 8C:C8:F4:90:00:00/28,SwiftNav Swift Navigation Inc
 8C:C8:F4:A0:00:00/28,TriluxGr Trilux Group Management GmbH
 8C:C8:F4:B0:00:00/28,"PTYPE PTYPE Co., LTD."
 8C:C8:F4:C0:00:00/28,"Shenzhen Shenzhen KSTAR Science and Technology Co., Ltd"
 8C:C8:F4:D0:00:00/28,"BeijingX Beijing Xinxunxintong Eletronics Co.,Ltd"
 8C:C8:F4:E0:00:00/28,Evaporco Evaporcool Solutions
+8C:CB:14,TBS TBS GmbH
 8C:CB:DF,FoxconnI Foxconn Interconnect Technology
 8C:CD:A2,"ACTP ACTP, Inc."
 8C:CD:E8,"Nintendo Nintendo Co., Ltd."
 8C:CD:FE,"AMPAKTec AMPAK Technology,Inc."
 8C:CE:4E,Espressi Espressif Inc.
 8C:CE:FD,"Shenzhen Shenzhen zhouhai technology co.,LTD"
 8C:CF:09,DellEMC Dell EMC
 8C:CF:5C,BEFEGA BEFEGA GmbH
 8C:CF:8F,ITC ITC Systems
+8C:D0:8B,"WuXiRigo WuXi Rigosys Technology Co.,LTD"
 8C:D0:B2,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 8C:D1:7B,CGMobile CG Mobile
 8C:D2:E9,"YokoteSe Yokote Seiko Co., Ltd."
 8C:D3:A2,VisSimAS VisSim AS
 8C:D4:8E,ItelMobi Itel Mobile Limited
+8C:D5:4A,"TaiyoYud Taiyo Yuden Co.,Ltd"
 8C:D6:28,IkorMete Ikor Metering
 8C:D6:7F,EMMicroe EM Microelectronic
 8C:D9:D6,XiaomiCo Xiaomi Communications Co Ltd
 8C:DB:25,ESGSolut ESG Solutions
 8C:DC:02,zte zte corporation
 8C:DC:D4,HewlettP Hewlett Packard
 8C:DD:8D,Wifly-Ci Wifly-City System Inc.
 8C:DE:52,ISSCTech ISSC Technologies Corp.
 8C:DE:99,Comlab Comlab Inc.
 8C:DE:E6,"SamsungE Samsung Electronics Co.,Ltd"
 8C:DE:F9,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
+8C:DF:2C,"vivoMobi vivo Mobile Communication Co., Ltd."
 8C:DF:9D,NEC NEC Corporation
+8C:E0:42,"vivoMobi vivo Mobile Communication Co., Ltd."
 8C:E0:81,zte zte corporation
 8C:E1:17,zte zte corporation
 8C:E2:DA,CircleMe Circle Media Inc
 8C:E3:8E,Kioxia Kioxia Corporation
 8C:E4:68,"Guangzho Guangzhou Sageran Technology Co., Ltd."
 8C:E5:C0,"SamsungE Samsung Electronics Co.,Ltd"
 8C:E5:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -36524,17 +37606,19 @@
 8C:EA:12,"Shenzhen Shenzhen MiaoMing Intelligent Technology Co.,Ltd"
 8C:EA:1B,Edgecore Edgecore Networks Corporation
 8C:EA:48,"SamsungE Samsung Electronics Co.,Ltd"
 8C:EB:C6,"HuaweiTe Huawei Technologies Co.,Ltd"
 8C:EC:4B,Dell Dell Inc.
 8C:EC:7B,"Apple Apple, Inc."
 8C:EE:C6,Precepsc Precepscion Pty. Ltd.
+8C:EE:FD,zte zte corporation
 8C:F1:12,"Motorola Motorola Mobility LLC, a Lenovo Company"
 8C:F2:28,"MercuryC Mercury Communication Technologies Co.,Ltd."
 8C:F3:19,"SiemensI Siemens Industrial Automation Products Ltd., Chengdu"
+8C:F3:E7,solidote solidotech
 8C:F5:A3,SamsungE Samsung Electro-Mechanics(Thailand)
 8C:F6:81,SiliconL Silicon Laboratories
 8C:F7:10,"AMPAKTec AMPAK Technology, Inc."
 8C:F7:73,Nokia
 8C:F8:13,OrangePo Orange Polska
 8C:F8:C5,IntelCor Intel Corporate
 8C:F9:45,PowerAut Power Automation pte Ltd
@@ -36558,14 +37642,15 @@
 90:02:7A,"Shenzhen Shenzhen Sworix Techonlogy Co., Ltd"
 90:02:8A,"Shenzhen Shenzhen Shidean Legrand Electronic Products Co.,Ltd"
 90:02:A9,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 90:03:25,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:03:72,LongnanJ Longnan Junya Digital Technology Co. Ltd.
 90:03:B7,Parrot Parrot Sa
 90:06:28,"SamsungE Samsung Electronics Co.,Ltd"
+90:06:F2,TexasIns Texas Instruments
 90:09:17,Far-sigh Far-sighted mobile
 90:09:D0,Synology Synology Incorporated
 90:09:DF,IntelCor Intel Corporate
 90:0A:1A,TaicangT Taicang T&W Electronics
 90:0A:39,"Wiio Wiio, Inc."
 90:0A:3A,PSGPlast PSG Plastic Service GmbH
 90:0A:62,Inventus Inventus Power Eletronica do Brasil LTDA
@@ -36607,34 +37692,38 @@
 90:23:B4,"NewH3CTe New H3C Technologies Co., Ltd"
 90:23:EC,"Availink Availink, Inc."
 90:25:F2,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:27:2B,Algorab Algorab S.r.l.
 90:27:59,"NanjingJ Nanjing Jiahao Technology Co., Ltd."
 90:27:78,OpenInfr Open Infrastructure
 90:27:E4,"Apple Apple, Inc."
+90:2A:EE,XiaomiCo Xiaomi Communications Co Ltd
 90:2B:34,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 90:2B:D2,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:2C:C7,C-MAXAsi C-MAX Asia Limited
 90:2C:FB,"CanTops CanTops Co,.Ltd."
 90:2E:16,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 90:2E:1C,IntelCor Intel Corporate
 90:2E:87,LabJack
+90:31:4B,AltoBeam AltoBeam Inc.
 90:31:CD,OnyxHeal Onyx Healthcare Inc.
 90:32:4B,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 90:34:2B,"Gatekeep Gatekeeper Systems, Inc."
 90:34:FC,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 90:35:6E,Vodafone Vodafone Omnitel N.V.
 90:35:EA,SiliconL Silicon Laboratories
 90:38:09,Ericsson Ericsson AB
 90:38:0C,Espressi Espressif Inc.
 90:38:DF,Changzho Changzhou Tiannengbo System Co. Ltd.
 90:39:5E,SiliconL Silicon Laboratories
+90:39:5F,AmazonTe Amazon Technologies Inc.
 90:3A:72,RuckusWi Ruckus Wireless
 90:3A:A0,Nokia
 90:3A:E6,Parrot Parrot Sa
+90:3C:1D,"HisenseV Hisense Visual Technology Co.,Ltd"
 90:3C:92,"Apple Apple, Inc."
 90:3C:AE,"YunnanKS Yunnan KSEC Digital Technology Co.,Ltd."
 90:3C:B3,Edgecore Edgecore Networks Corporation
 90:3D:5A,Shenzhen Shenzhen Wision Technology Holding Limited
 90:3D:68,"G-Printe G-Printec, Inc."
 90:3D:6B,ZiconTec Zicon Technology Corp.
 90:3D:BD,SecureMe Secure Meters Limited
@@ -36673,51 +37762,57 @@
 90:4E:91:C0:00:00/28,Showtacl Showtacle s.r.o.
 90:4E:91:D0:00:00/28,SKODAELE SKODA ELECTRIC a.s.
 90:4E:91:E0:00:00/28,"Shenzhen Shenzhen Cloudynamo Internet Technologies Co.,LTD."
 90:50:5A,"unGlue unGlue, Inc"
 90:50:7B,Advanced Advanced PANMOBIL Systems GmbH & Co. KG
 90:50:CA,HitronTe Hitron Technologies. Inc
 90:51:3F,Elettron Elettronica Santerno SpA
+90:52:BF,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 90:54:46,TesElect Tes Electronic Solutions
 90:55:AE,"Ericsson Ericsson, EAB/RWI/K"
 90:55:DE,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
+90:56:07,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 90:56:82,Lenbrook Lenbrook Industries Limited
 90:56:92,Autotalk Autotalks Ltd.
 90:56:FC,TecnoMob Tecno Mobile Limited
-90:58:51,Technico Technicolor CH USA Inc.
+90:58:51,VantivaU Vantiva USA LLC
 90:59:3C,Az-Techn Az-Technology Sdn Bhd
 90:59:AF,TexasIns Texas Instruments
+90:5A:08,"SuperMic Super Micro Computer, Inc."
 90:5C:34,SiriusEl Sirius Electronic Systems Srl
 90:5C:44,"CompalBr Compal Broadband Networks, Inc."
 90:5D:7C,"NewH3CTe New H3C Technologies Co., Ltd"
 90:5E:44,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:5F:2E,TCTmobil TCT mobile ltd
 90:5F:8D,modas modas GmbH
 90:60:F1,"Apple Apple, Inc."
 90:61:0C,FidaInte Fida International (S) Pte Ltd
 90:61:AE,IntelCor Intel Corporate
 90:63:3B,"SamsungE Samsung Electronics Co.,Ltd"
+90:64:AD,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:65:60,EMMicroe EM Microelectronic
 90:65:84,IntelCor Intel Corporate
 90:67:17,AlphionI Alphion India Private Limited
 90:67:1C,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:67:B5,Alcatel- Alcatel-Lucent
 90:67:F3,AlcatelL Alcatel Lucent
 90:68:C3,"Motorola Motorola Mobility LLC, a Lenovo Company"
 90:69:76,Withrobo Withrobot Inc.
 90:6A:94,"hangzhou hangzhou huacheng network technology co., ltd"
 90:6A:EB,Microsof Microsoft Corporation
 90:6C:AC,"Fortinet Fortinet, Inc."
 90:6D:05,"BxbElect Bxb Electronics Co., Ltd"
+90:6D:62,CambiumN Cambium Networks Limited
 90:6D:C8,DLGAutom DLG Automação Industrial Ltda
 90:6E:BB,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 90:6F:18,Private
 90:6F:A9,"NanjingP Nanjing Putian Telecommunications Technology Co.,Ltd."
 90:70:25,"GareaMic Garea Microsys Co.,Ltd."
 90:70:65,TexasIns Texas Instruments
+90:70:D3,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 90:72:40,"Apple Apple, Inc."
 90:72:82,Sagemcom Sagemcom Broadband SAS
 90:73:5A,"Motorola Motorola Mobility LLC, a Lenovo Company"
 90:74:9D,"IRayTech IRay Technology Co., Ltd."
 90:75:BC,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 90:76:9F,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 90:77:EE,"Cisco Cisco Systems, Inc"
@@ -36728,29 +37823,32 @@
 90:79:CF,zte zte corporation
 90:7A:0A,GebrBode Gebr. Bode GmbH & Co KG
 90:7A:28,BeijingM Beijing Morncloud Information And Technology Co. Ltd.
 90:7A:58,Zegna-Da Zegna-Daidong Limited
 90:7A:F1,Wally
 90:7B:C6,TexasIns Texas Instruments
 90:7E:30,Lars
+90:7E:43,zte zte corporation
 90:7E:BA,"UtekTech Utek Technology (Shenzhen) Co.,Ltd"
 90:7F:61,"ChiconyE Chicony Electronics Co., Ltd."
 90:80:60,Nilfisk Nilfisk A/S
 90:80:8F,"HuaweiDe Huawei Device Co., Ltd."
 90:81:2A,"Apple Apple, Inc."
 90:81:58,"Apple Apple, Inc."
 90:81:75,"SamsungE Samsung Electronics Co.,Ltd"
 90:82:60,IEEE1904 IEEE 1904.1 Working Group
 90:83:4B,"BeijingY Beijing Yunyi Times Technology Co,.Ltd"
 90:83:7A,GeneralE General Electric Water & Process Technologies
+90:83:7E,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 90:84:0D,"Apple Apple, Inc."
 90:84:2B,LEGOSyst LEGO System A/S
 90:84:8B,"HDR10+Te HDR10+ Technologies, LLC"
 90:86:74,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 90:86:9B,zte zte corporation
+90:88:55,"Cisco Cisco Systems, Inc"
 90:88:A2,IonicsTe Ionics Technology Me Ltda
 90:89:5F,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 90:8C:09,TotalPha Total Phase
 90:8C:43,"Apple Apple, Inc."
 90:8C:44,"HKZongmu H.K Zongmu Technology Co., Ltd."
 90:8C:63,"GZWeedon GZ Weedong Networks Technology Co. , Ltd"
 90:8D:1D,GHTechno GH Technologies
@@ -36771,14 +37869,15 @@
 90:97:F3,"SamsungE Samsung Electronics Co.,Ltd"
 90:98:38,"HuaweiDe Huawei Device Co., Ltd."
 90:98:64,Impex-Sa Impex-Sat GmbH&Co KG
 90:98:77,VestelEl Vestel Elektronik San ve Tic. A.S.
 90:99:16,ELVEESNe ELVEES NeoTek OJSC
 90:9A:4A,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 90:9A:77,TexasIns Texas Instruments
+90:9B:6F,"Apple Apple, Inc."
 90:9C:4A,"Apple Apple, Inc."
 90:9D:7D,"ARRISGro ARRIS Group, Inc."
 90:9D:E0,NewlandD Newland Design + Assoc. Inc.
 90:9F:33,EFMNetwo EFM Networks
 90:9F:43,Accutron Accutron Instruments Inc.
 90:A1:37,"BeijingS Beijing Splendidtel Communication Technology Co,. Ltd"
 90:A2:10,UnitedTe United Telecoms Ltd
@@ -36787,14 +37886,15 @@
 90:A3:65,HMDGloba HMD Global Oy
 90:A4:6A,"Sisnet Sisnet Co., Ltd"
 90:A4:DE,WistronN Wistron Neweb Corporation
 90:A5:AF,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:A6:2F,Naver
 90:A6:BF,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 90:A7:83,JswPacif Jsw Pacific Corporation
+90:A7:BF,EMMicroe EM Microelectronic
 90:A7:C1,PakedgeD Pakedge Device and Software Inc.
 90:A8:22,AmazonTe Amazon Technologies Inc.
 90:A9:35,JWEntert JWEntertainment
 90:AA:C3,HitronTe Hitron Technologies. Inc
 90:AB:96,SiliconL Silicon Laboratories
 90:AC:3F,BrightSi BrightSign LLC
 90:AD:F7,"vivoMobi vivo Mobile Communication Co., Ltd."
@@ -36803,15 +37903,15 @@
 90:AF:D1,"netKTI netKTI Co., Ltd"
 90:B0:ED,"Apple Apple, Inc."
 90:B1:1C,Dell Dell Inc.
 90:B1:34,"ARRISGro ARRIS Group, Inc."
 90:B1:44,"SamsungE Samsung Electronics Co.,Ltd"
 90:B1:E0,"BeijingN Beijing Nebula Link Technology Co., Ltd"
 90:B2:1F,"Apple Apple, Inc."
-90:B4:DD,ZptR&D Zpt R&D
+90:B4:DD,Private
 90:B5:7F,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 90:B6:22,"SamsungE Samsung Electronics Co.,Ltd"
 90:B6:7A,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 90:B6:86,"MurataMa Murata Manufacturing Co., Ltd."
 90:B8:32,"ExtremeN Extreme Networks, Inc."
 90:B8:D0,"Joyent Joyent, Inc."
 90:B8:E0,"Shenzhen Shenzhen Yanray Technology Co.,Ltd"
@@ -36841,22 +37941,26 @@
 90:C6:82:E0:00:00/28,"Shanghai Shanghai HuRong Communication Technology Development Co., Ltd."
 90:C6:82:F0:00:00/28,Private
 90:C7:92,"ARRISGro ARRIS Group, Inc."
 90:C7:D8,zte zte corporation
 90:C9:9B,Tesorion Tesorion Nederland B.V.
 90:CA:FA,"Google Google, Inc."
 90:CC:24,"Synaptic Synaptics, Inc"
+90:CC:7A,"HuaweiDe Huawei Device Co., Ltd."
 90:CC:DF,IntelCor Intel Corporate
 90:CD:1F,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 90:CD:B6,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+90:CE:B8,TexasIns Texas Instruments
 90:CF:15,Nokia Nokia Corporation
 90:CF:6F,Dlogixs Dlogixs Co Ltd
 90:CF:7D,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
+90:D0:92,"HUMAX HUMAX Co., Ltd."
 90:D1:1B,PalomarM Palomar Medical Technologies
 90:D4:73,"vivoMobi vivo Mobile Communication Co., Ltd."
+90:D6:89,"HuahaoFa Huahao Fangzhou Technology Co.,Ltd"
 90:D7:4F,Bookeen
 90:D7:BE,WavelabG Wavelab Global Inc.
 90:D7:EB,TexasIns Texas Instruments
 90:D8:52,"Comtec Comtec Co., Ltd."
 90:D8:F3,zte zte corporation
 90:D9:2C,Hug-Wits Hug-Witschi Ag
 90:DA:4E,Avanu
@@ -36869,56 +37973,77 @@
 90:DF:B7,smssmart s.m.s smart microwave sensors GmbH
 90:DF:FB,Homeride Homerider Systems
 90:E0:F0,IEEE1722 IEEE 1722a Working Group
 90:E1:7B,"Apple Apple, Inc."
 90:E2:02,TexasIns Texas Instruments
 90:E2:BA,IntelCor Intel Corporate
 90:E2:FC,IEEERegi IEEE Registration Authority
-90:E2:FC:00:00:00/28,ParsErte Pars Ertebat Afzar Co.
+90:E2:FC:00:00:00/28,PEADBT-T PEA (DBT-Technology)
 90:E2:FC:10:00:00/28,Yitetech Yite technology
 90:E2:FC:20:00:00/28,"ShenZhen ShenZhen Temwey Innovation Technology Co.,Ltd."
 90:E2:FC:30:00:00/28,"Shenzhen Shenzhen Hisource Technology Development CO.,Ltd."
 90:E2:FC:40:00:00/28,Dongguan Dongguan Kangyong electronics technology Co. Ltd
 90:E2:FC:50:00:00/28,"Totalone Totalone Technology Co., Ltd."
 90:E2:FC:60:00:00/28,"SindohTe Sindoh Techno Co., Ltd."
 90:E2:FC:70:00:00/28,FairWind Fair Winds Digital srl
 90:E2:FC:80:00:00/28,bitsensi bitsensing Inc.
 90:E2:FC:90:00:00/28,HuddlyAS Huddly AS
 90:E2:FC:A0:00:00/28,"PowerEng Power Engineering & Manufacturing, Inc."
 90:E2:FC:B0:00:00/28,"Shenzhen Shenzhen Dingsheng Intelligent Technology Co., Ltd"
 90:E2:FC:C0:00:00/28,StanleyS Stanley Security
 90:E2:FC:D0:00:00/28,"BeijingL Beijing Lanxum Computer Technology CO.,LTD."
 90:E2:FC:E0:00:00/28,DevComsp DevCom spol. s r.o.
+90:E4:68,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 90:E6:BA,ASUSTekC ASUSTek COMPUTER INC.
 90:E7:10,"NewH3CTe New H3C Technologies Co., Ltd"
 90:E7:C4,HTC HTC Corporation
 90:E8:68,AzureWav AzureWave Technology Inc.
+90:E9:5E,"Cisco Cisco Systems, Inc"
 90:EA:60,SPILaser SPI Lasers Ltd
 90:EB:48,"Shanghai Shanghai XinMiaoLink Technology Co., Ltd"
+90:EB:50,"Cisco Cisco Systems, Inc"
 90:EC:50,COBO C.O.B.O. Spa
 90:EC:77,silicom
+90:EC:E3,Nokia
+90:EC:EA,"Apple Apple, Inc."
 90:EE:C7,"SamsungE Samsung Electronics Co.,Ltd"
 90:EE:D9,"Universa Universal De Desarrollos Electrónicos, Sa"
 90:EF:68,ZyxelCom Zyxel Communications Corporation
 90:F0:52,"MEIZUTec MEIZU Technology Co., Ltd."
 90:F1:57,GarminIn Garmin International
 90:F1:AA,"SamsungE Samsung Electronics Co.,Ltd"
 90:F1:B0,"Hangzhou Hangzhou Anheng Info&Tech CO.,LTD"
 90:F2:60,"Shenzhen Shenzhen Honesty Electronics Co.,Ltd."
 90:F2:78,RadiusGa Radius Gateway
 90:F3:05,"HUMAX HUMAX Co., Ltd."
 90:F3:B7,"KirisunC Kirisun Communications Co., Ltd."
 90:F3:B8,"ChinaMob China Mobile Group Device Co.,Ltd."
+90:F4:21,IEEERegi IEEE Registration Authority
+90:F4:21:00:00:00/28,Gemstone Gemstone Lights
+90:F4:21:10:00:00/28,BeEnergy BeEnergy SG GmbH
+90:F4:21:20:00:00/28,Catvisio Catvision Ltd.
+90:F4:21:30:00:00/28,"SinpengG Sinpeng(Guangzhou)Technology Co.,Ltd"
+90:F4:21:40:00:00/28,SansapTe Sansap Technology Pvt. Ltd.
+90:F4:21:50:00:00/28,DESKO DESKO GmbH
+90:F4:21:60:00:00/28,"WuxiSunn Wuxi Sunning Smart Devices Co.,Ltd"
+90:F4:21:70:00:00/28,Senstar Senstar Corporation
+90:F4:21:80:00:00/28,Mi-JackP Mi-Jack Products
+90:F4:21:90:00:00/28,"Twunicom Twunicom Life Tech. Co., Ltd."
+90:F4:21:A0:00:00/28,Proquali Proqualit Telecom LTDA
+90:F4:21:B0:00:00/28,"JiangsuM Jiangsu MSInfo Technology Co.,Ltd."
+90:F4:21:C0:00:00/28,Acoba
+90:F4:21:D0:00:00/28,"Taichite Taichitel Technology Shanghai Co.,Ltd."
+90:F4:21:E0:00:00/28,VelanStu Velan Studios Inc.
 90:F4:C1,RandMcNa Rand McNally
 90:F6:44,"HuaweiDe Huawei Device Co., Ltd."
 90:F6:52,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 90:F7:2F,"Phillips Phillips Machine & Welding Co., Inc."
 90:F7:B2,"NewH3CTe New H3C Technologies Co., Ltd"
 90:F8:2E,AmazonTe Amazon Technologies Inc.
-90:F8:91,"Kaonmedi Kaonmedia CO., LTD."
+90:F8:91,"KaonGrou Kaon Group Co., Ltd."
 90:F9:70,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:F9:B7,"HuaweiTe Huawei Technologies Co.,Ltd"
 90:FB:5B,Avaya Avaya Inc
 90:FB:A6,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 90:FD:61,"Apple Apple, Inc."
 90:FD:73,zte zte corporation
 90:FD:9F,SiliconL Silicon Laboratories
@@ -36929,14 +38054,15 @@
 94:00:B0,"HuaweiTe Huawei Technologies Co.,Ltd"
 94:01:49,AutoHotB AutoHotBox
 94:01:AC,"WuhanQia Wuhan Qianyang Iotian Technology Co., Ltd"
 94:01:C2,"SamsungE Samsung Electronics Co.,Ltd"
 94:02:30,Logitech
 94:02:6B,"Optictim Optictimes Co.,Ltd"
 94:04:9C,"HuaweiTe Huawei Technologies Co.,Ltd"
+94:04:E3,VantivaU Vantiva USA LLC
 94:05:B6,LilingFu Liling FullRiver Electronics & Technology Ltd
 94:05:BB,IEEERegi IEEE Registration Authority
 94:05:BB:00:00:00/28,"QingdaoM Qingdao Maotran Electronics co., ltd"
 94:05:BB:10:00:00/28,"Dongguan Dongguan Kingtron Electronics Tech Co., Ltd"
 94:05:BB:20:00:00/28,"Dongguan Dongguan CXWE Technology Co.,Ltd."
 94:05:BB:30:00:00/28,Neutrik Neutrik AG
 94:05:BB:40:00:00/28,"Shenzhen Shenzhen Baolijie Technology Co., Ltd."
@@ -36987,15 +38113,15 @@
 94:28:2E,"NewH3CTe New H3C Technologies Co., Ltd"
 94:28:6F,zte zte corporation
 94:29:0C,"Shenyang Shenyang wisdom Foundation Technology Development Co., Ltd."
 94:29:2F,"NewH3CTe New H3C Technologies Co., Ltd"
 94:29:57,"AirpoNet Airpo Networks Technology Co.,Ltd."
 94:29:8D,"Shanghai Shanghai AdaptComm Technology Co., Ltd."
 94:2A:3F,Diversey Diversey Inc
-94:2A:6F,Ubiquiti Ubiquiti Networks Inc.
+94:2A:6F,Ubiquiti Ubiquiti Inc
 94:2C:B3,"HUMAX HUMAX Co., Ltd."
 94:2D:DC,"SamsungE Samsung Electronics Co.,Ltd"
 94:2E:17,Schneide Schneider Electric Canada Inc
 94:2E:63,Finsécur
 94:31:9B,Alphatro Alphatronics BV
 94:31:CB,"vivoMobi vivo Mobile Communication Co., Ltd."
 94:33:DD,Taco Taco Inc
@@ -37003,27 +38129,30 @@
 94:35:0A,"SamsungE Samsung Electronics Co.,Ltd"
 94:36:E0,"SichuanB Sichuan Bihong Broadcast & Television New Technologies Co.,Ltd"
 94:37:F7,"HuaweiDe Huawei Device Co., Ltd."
 94:39:E5,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 94:3A:91,AmazonTe Amazon Technologies Inc.
 94:3A:F0,Nokia Nokia Corporation
 94:3B:B0,"NewH3CTe New H3C Technologies Co., Ltd"
-94:3B:B1,"Kaonmedi Kaonmedia CO., LTD."
+94:3B:B1,"KaonGrou Kaon Group Co., Ltd."
 94:3C:96,Sagemcom Sagemcom Broadband SAS
 94:3C:C6,Espressi Espressif Inc.
 94:3D:C9,"AsahiNet Asahi Net, Inc."
+94:3E:E4,WiSATech WiSA Technologies Inc
 94:3F:BB,RPCIstok JSC RPC Istok named after Shokin
 94:3F:C2,HewlettP Hewlett Packard Enterprise
+94:3F:D6,"Apple Apple, Inc."
 94:40:A2,"AnywaveC Anywave Communication Technologies, Inc."
 94:40:C9,HewlettP Hewlett Packard Enterprise
 94:41:C1,Mini-Cam Mini-Cam Limited
 94:43:4D,Ciena Ciena Corporation
 94:44:44,LGInnote LG Innotek
 94:44:52,BelkinIn Belkin International Inc.
 94:46:96,BaudTec BaudTec Corporation
+94:47:88,"HuaweiTe Huawei Technologies Co.,Ltd"
 94:47:B0,"BeijingE Beijing Eswin Computing Technology Co., Ltd"
 94:49:96,WiSilica WiSilica Inc
 94:4A:09,BitWiseC BitWise Controls
 94:4A:0C,Sercomm Sercomm Corporation.
 94:4E:5B,"UbeeInte Ubee Interactive Co., Limited"
 94:4F:4C,SoundUni Sound United LLC
 94:50:47,Rechnerb Rechnerbetriebsgruppe
@@ -37053,24 +38182,25 @@
 94:63:72,"vivoMobi vivo Mobile Communication Co., Ltd."
 94:63:D1,"SamsungE Samsung Electronics Co.,Ltd"
 94:64:24,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 94:65:2D,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 94:65:9C,IntelCor Intel Corporate
 94:66:E7,WOMEngin WOM Engineering
 94:67:7E,BeldenIn Belden India Private Limited
-94:6A:77,Technico Technicolor CH USA Inc.
+94:6A:77,VantivaU Vantiva USA LLC
 94:6A:B0,Arcadyan Arcadyan Corporation
 94:6D:AE,"Mellanox Mellanox Technologies, Inc."
 94:70:D2,WinfirmT Winfirm Technology
 94:71:AC,TCTmobil TCT mobile ltd
 94:72:0F,"Guangdon Guangdong Nanguang Photo&Video Systems Co., Ltd."
 94:75:6E,QinetiQN QinetiQ North America
 94:76:B7,"SamsungE Samsung Electronics Co.,Ltd"
 94:77:2B,"HuaweiTe Huawei Technologies Co.,Ltd"
 94:78:06,"NingboSu Ningbo Sunvot Technology Co.,Ltd"
+94:79:18,ItelMobi Itel Mobile Limited
 94:7B:AE,XiaomiCo Xiaomi Communications Co Ltd
 94:7B:BE,Ubicquia Ubicquia LLC
 94:7B:E7,"SamsungE Samsung Electronics Co.,Ltd"
 94:7C:3E,Polewall Polewall Norge AS
 94:7D:77,"HuaweiTe Huawei Technologies Co.,Ltd"
 94:7E:B9,National National Narrowband Network Communications Pty Ltd
 94:7F:1D,"Shenzhen Shenzhen Fastrain Technology Co., Ltd."
@@ -37098,15 +38228,17 @@
 94:90:34,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 94:91:7F,AskeyCom Askey Computer Corp
 94:92:BC,SyntechH Syntech(Hk) Technology Limited
 94:92:D2,"KCFTechn KCF Technologies, Inc."
 94:94:26,"Apple Apple, Inc."
 94:94:4A,Particle Particle Industries Inc.
 94:95:A0,"Google Google, Inc."
+94:97:AE,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 94:98:69,zte zte corporation
+94:98:8F,Sagemcom Sagemcom Broadband SAS
 94:98:A2,Shanghai Shanghai LISTEN TECH.LTD
 94:99:01,"Shenzhen Shenzhen YITOA Digital Appliance CO.,LTD"
 94:99:90,VTCTelec VTC Telecommunications
 94:9A:A9,Microsof Microsoft Corporation
 94:9B:2C,"ExtremeN Extreme Networks, Inc."
 94:9B:FD,"TransNew Trans New Technology, Inc."
 94:9C:55,AltaData Alta Data Technologies
@@ -37175,21 +38307,22 @@
 94:C9:B7:20:00:00/28,Annapurn Annapurna labs
 94:C9:B7:30:00:00/28,Sitronic Sitronics JSC
 94:C9:B7:40:00:00/28,"Zhejiang Zhejiang Hengjie Communication Technology Co,. Ltd."
 94:C9:B7:50:00:00/28,"BeijingA Beijing Anyunshiji Technology Co., Ltd."
 94:C9:B7:60:00:00/28,"Realtime Realtimes Beijing Technology Co., Ltd."
 94:C9:B7:70:00:00/28,"Mammotht Mammothtek Cloud(Dong Guan)Technology Co., Ltd"
 94:C9:B7:80:00:00/28,OSOMProd OSOM Products Inc
-94:C9:B7:90:00:00/28,Private
+94:C9:B7:90:00:00/28,"Titanium Titanium union(shenzhen)technology co.,ltd"
 94:C9:B7:A0:00:00/28,"ShenZhen ShenZhen Beide Technology Co.,LTD"
 94:C9:B7:B0:00:00/28,"3DBiomed 3D Biomedicine Science & Technology Co., Limited"
 94:C9:B7:C0:00:00/28,"JinjinTe Jinjin Technology (Shenzhen) Co., Ltd"
 94:C9:B7:D0:00:00/28,DspreadT Dspread Technology (Beijing) Inc.
 94:C9:B7:E0:00:00/28,"shenzhen shenzhen UDD Technologies,co.,Ltd"
 94:CA:0F,Honeywel Honeywell Analytics
+94:CB:CD,zte zte corporation
 94:CC:04,IEEERegi IEEE Registration Authority
 94:CC:04:00:00:00/28,"Hangzhou Hangzhou Yongkong Technology Co., Ltd."
 94:CC:04:10:00:00/28,"Gocoax Gocoax, Inc"
 94:CC:04:20:00:00/28,NanjingY Nanjing Yacer Communication Technology Co. Ltd.
 94:CC:04:30:00:00/28,"Shenzhen Shenzhen Link technology Co.,Ltd"
 94:CC:04:40:00:00/28,"ProConne ProConnections, Inc."
 94:CC:04:50:00:00/28,"Shenzhen Shenzhen Sanray Technology Co.,Ltd"
@@ -37231,14 +38364,15 @@
 94:DB:DA,"HuaweiTe Huawei Technologies Co.,Ltd"
 94:DC:4E,"AEVspols AEV, spol. s r. o."
 94:DD:3F,"A+VLinkT A+V Link Technologies, Corp."
 94:DD:F8,"BrotherI Brother Industries, LTD."
 94:DE:0E,SmartOpt SmartOptics AS
 94:DE:80,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 94:DE:B8,SiliconL Silicon Laboratories
+94:DF:34,"HuaweiTe Huawei Technologies Co.,Ltd"
 94:DF:4E,"WistronI Wistron InfoComm(Kunshan)Co.,Ltd."
 94:DF:58,"IJElectr IJ Electron CO.,Ltd."
 94:E0:D0,HealthSt HealthStream Taiwan Inc.
 94:E0:D6,ChinaDra China Dragon Technology Limited
 94:E1:29,"SamsungE Samsung Electronics Co.,Ltd"
 94:E1:AC,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 94:E2:26,"DORtizCo D. ORtiz Consulting, LLC"
@@ -37264,22 +38398,24 @@
 94:EB:CD,BlackBer BlackBerry RTS
 94:EE:9F,HMDGloba HMD Global Oy
 94:F1:28,HewlettP Hewlett Packard Enterprise
 94:F1:9E,"HuizhouM Huizhou Maorong Intelligent Technology Co.,Ltd"
 94:F2:78,ElmaElec Elma Electronic
 94:F2:BB,ValeoVis Valeo Vision Systems
 94:F3:92,"Fortinet Fortinet, Inc."
+94:F5:24,ChengduB Chengdu BeiZhongWangXin Technology Co.Ltd
 94:F5:51,CadiScie Cadi Scientific Pte Ltd
 94:F6:65,RuckusWi Ruckus Wireless
 94:F6:92,"Geminico Geminico co.,Ltd."
 94:F6:A3,"Apple Apple, Inc."
 94:F6:D6,"Apple Apple, Inc."
 94:F7:20,"TianjinD Tianjin Deviser Electronics Instrument Co., Ltd"
 94:F7:AD,JuniperN Juniper Networks
 94:F8:27,Shanghai Shanghai Imilab Technology Co.Ltd
+94:F9:29,"MetaPlat Meta Platforms Technologies, LLC"
 94:FA:E8,"Shenzhen Shenzhen Eycom Technology Co., Ltd"
 94:FB:29,ZebraTec Zebra Technologies Inc.
 94:FB:A7,IEEERegi IEEE Registration Authority
 94:FB:A7:00:00:00/28,Reichert Reichert Inc.
 94:FB:A7:10:00:00/28,InaxsysS Inaxsys Security Systems inc.
 94:FB:A7:20:00:00/28,"BeijingL Beijing Leja Tech co., Ltd."
 94:FB:A7:30:00:00/28,"GuangDon Guang Dong Takstar Electronic Co.,Ltd."
@@ -37321,14 +38457,15 @@
 98:02:D8:90:00:00/28,"NavroomB Navroom Beijing, China"
 98:02:D8:A0:00:00/28,HySecuri HySecurity
 98:02:D8:B0:00:00/28,"HanshinM Hanshin Medical Co., Ltd."
 98:02:D8:C0:00:00/28,AGV AGV spa
 98:02:D8:D0:00:00/28,Promicon Promicon Elektronik GmbH + Co.KG
 98:02:D8:E0:00:00/28,Private
 98:02:D8:F0:00:00/28,Private
+98:03:8A,TexasIns Texas Instruments
 98:03:9B,"Mellanox Mellanox Technologies, Inc."
 98:03:A0,ABBPower ABB n.v. Power Quality Products
 98:03:D8,"Apple Apple, Inc."
 98:06:37,IEEERegi IEEE Registration Authority
 98:06:37:00:00:00/28,Zoleo Zoleo Inc.
 98:06:37:10:00:00/28,EPSchlum E. P. Schlumberger
 98:06:37:20:00:00/28,Summa Summa nv
@@ -37344,28 +38481,31 @@
 98:06:37:C0:00:00/28,HwaCom HwaCom Systems Inc.
 98:06:37:D0:00:00/28,VRTechno VR Technology(Shenzhen) Limited
 98:06:37:E0:00:00/28,Shanghai Shanghai Jinnian information technology Co. Ltd
 98:06:3A,HomeCont Home Control Singapore Pte Ltd
 98:06:3C,"SamsungE Samsung Electronics Co.,Ltd"
 98:07:2D,TexasIns Texas Instruments
 98:09:CF,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
+98:0C:33,SiliconL Silicon Laboratories
 98:0C:82,"SamsungE Samsung Electro Mechanics Co., Ltd."
 98:0C:A5,"Motorola Motorola (Wuhan) Mobility Technologies Communication Co., Ltd."
 98:0D:2E,HTC HTC Corporation
 98:0D:51,"HuaweiDe Huawei Device Co., Ltd."
 98:0D:67,ZyxelCom Zyxel Communications Corporation
 98:0D:6F,"SamsungE Samsung Electronics Co.,Ltd"
+98:0D:AF,"Apple Apple, Inc."
 98:0E:24,"PhytiumT Phytium Technology Co.,Ltd."
 98:0E:E4,Private
 98:10:82,"Nsolutio Nsolution Co., Ltd."
 98:10:94,"Shenzhen Shenzhen Vsun communication technology Co.,ltd"
 98:10:E8,"Apple Apple, Inc."
 98:13:33,zte zte corporation
 98:14:D2,Avonic
 98:16:EC,ICIntrac IC Intracom
+98:17:F1,zte zte corporation
 98:18:88,CiscoMer Cisco Meraki
 98:19:2C,Edgecore Edgecore Networks Corporation
 98:1A:35,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:1B:B5,"ASSAABLO ASSA ABLOY Korea Co., Ltd iRevo"
 98:1D:FA,"SamsungE Samsung Electronics Co.,Ltd"
 98:1E:0F,JeelanSh Jeelan (Shanghai Jeelan Technology Information Inc
 98:1E:19,Sagemcom Sagemcom Broadband SAS
@@ -37410,14 +38550,15 @@
 98:34:9D,KraussMa Krauss Maffei Technologies GmbH
 98:35:71,Sub10 Sub10 Systems Ltd
 98:35:B8,Assemble Assembled Products Corporation
 98:35:ED,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:37:13,PTNavico PT.Navicom Indonesia
 98:38:7D,"ItronicT Itronic Technology Co. , Ltd."
 98:39:8E,"SamsungE Samsung Electronics Co.,Ltd"
+98:39:C0,Flextron Flextronics
 98:3B:16,"AMPAKTec AMPAK Technology, Inc."
 98:3B:67,DWnetTec DWnet Technologies(Suzhou) Corporation
 98:3B:8F,IntelCor Intel Corporate
 98:3F:60,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:3F:66,"WuhanFun Wuhan Funshion Online Technologies Co.,Ltd"
 98:3F:9F,ChinaSSJ China SSJ (Suzhou) Network Technology Inc.
 98:40:BB,Dell Dell Inc.
@@ -37427,30 +38568,33 @@
 98:43:DA,Intertec Intertech
 98:43:FA,IntelCor Intel Corporate
 98:44:B6,Infranor Infranor Sas
 98:44:CE,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:45:62,"Shanghai Shanghai Baud Data Communication Co.,Ltd."
 98:46:0A,"Apple Apple, Inc."
 98:47:3C,"Shanghai Shanghai Sunmon Communication Technogy Co.,Ltd"
+98:47:44,Shenzhen Shenzhen Boomtech Industrial Corporation
 98:48:27,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 98:48:74,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:49:14,WistronN Wistron Neweb Corporation
+98:49:25,JuniperN Juniper Networks
 98:49:9F,DomoTact Domo Tactical Communications
 98:49:E1,BoeingDe Boeing Defence Australia
 98:4A:47,CHGHospi CHG Hospital Beds
+98:4B:06,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:4B:4A,"ARRISGro ARRIS Group, Inc."
 98:4B:E1,HewlettP Hewlett Packard
 98:4C:04,Zhangzho Zhangzhou Keneng Electrical Equipment Co Ltd
 98:4C:D3,MantisDe Mantis Deposition
 98:4E:97,Starligh Starlight Marketing (H. K.) Ltd.
 98:4F:EE,IntelCor Intel Corporate
 98:50:2E,"Apple Apple, Inc."
 98:50:A3,Signalte Signaltek Jsc
 98:52:3D,"SunitecE Sunitec Enterprise Co.,Ltd"
-98:52:4A,Technico Technicolor CH USA Inc.
+98:52:4A,VantivaU Vantiva USA LLC
 98:52:B1,"SamsungE Samsung Electronics Co.,Ltd"
 98:54:1B,IntelCor Intel Corporate
 98:57:D3,"HonHai-C Hon Hai-Ccpbg Precision Ind.Co.,Ltd."
 98:58:8A,SYSGRATI SYSGRATION Ltd.
 98:59:45,TexasIns Texas Instruments
 98:59:49,Luxottic Luxottica Group S.P.A.
 98:59:7A,IntelCor Intel Corporate
@@ -37510,15 +38654,15 @@
 98:73:C4,SageElec Sage Electronic Engineering LLC
 98:74:3D,Shenzhen Shenzhen Jun Kai Hengye Technology Co. Ltd
 98:74:DA,Infinixm Infinix mobility limited
 98:75:1A,"HuaweiDe Huawei Device Co., Ltd."
 98:76:B6,Adafruit
 98:77:70,"PepDigit Pep Digital Technology (Guangzhou) Co., Ltd"
 98:77:CB,VorteksE Vorteks ED
-98:77:E7,"Kaonmedi Kaonmedia CO., LTD."
+98:77:E7,"KaonGrou Kaon Group Co., Ltd."
 98:7A:10,Ericsson Ericsson AB
 98:7A:14,Microsof Microsoft Corporation
 98:7B:F3,TexasIns Texas Instruments
 98:7D:DD,"ChinaMob China Mobile Group Device Co.,Ltd."
 98:7E:46,EmizonNe Emizon Networks Limited
 98:7E:CA,Inventus Inventus Power Eletronica do Brasil LTDA
 98:7E:E3,"vivoMobi vivo Mobile Communication Co., Ltd."
@@ -37540,28 +38684,31 @@
 98:80:BB:E0:00:00/28,DMedTech D.Med Technical Products GmbH
 98:80:EE,"SamsungE Samsung Electronics Co.,Ltd"
 98:81:8A,"HuaweiDe Huawei Device Co., Ltd."
 98:82:17,Disrupti Disruptive Ltd
 98:83:89,"SamsungE Samsung Electronics Co.,Ltd"
 98:84:E3,TexasIns Texas Instruments
 98:86:5D,"NokiaSha Nokia Shanghai Bell Co., Ltd."
+98:86:8B,JuniperN Juniper Networks
 98:86:B1,Flyaudio Flyaudio corporation (China)
 98:87:44,"WuxiHong Wuxi Hongda Science and Technology Co.,LTD"
 98:89:24,TexasIns Texas Instruments
 98:89:ED,AnademIn Anadem Information Inc.
 98:8B:0A,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 98:8B:5D,Sagemcom Sagemcom Broadband SAS
 98:8B:69,"Shenzhen Shenzhen hylitech Co.,LTD"
 98:8B:AD,Corintec Corintech Ltd.
+98:8C:B3,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 98:8D:46,IntelCor Intel Corporate
 98:8E:34,"Zhejiang Zhejiang Boxsam Electronic Co.,Ltd"
 98:8E:4A,"NoxusBei Noxus(Beijing) Technology Co.,Ltd"
 98:8E:79,"Qudelix Qudelix, Inc."
 98:8E:D4,ItelMobi Itel Mobile Limited
 98:8E:DD,TEConnec TE Connectivity Limerick
+98:8F:00,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 98:8F:E0,IEEERegi IEEE Registration Authority
 98:8F:E0:00:00:00/28,Valinso Valinso B.V.
 98:8F:E0:10:00:00/28,"Guangzho Guangzhou Herystorm Technology Co.,Ltd."
 98:8F:E0:20:00:00/28,vhfelekt vhf elektronik GmbH
 98:8F:E0:30:00:00/28,Empowerm Empowerment Technologies Inc.
 98:8F:E0:40:00:00/28,"Schmiden Schmid AG, energy solutions"
 98:8F:E0:50:00:00/28,"KuaiZhuS KuaiZhu SmartTechnology?Suzhou?CO.,Ltd"
@@ -37579,17 +38726,18 @@
 98:93:CC,LgElectr Lg Electronics Inc
 98:94:49,Skyworth Skyworth Wireless Technology Ltd.
 98:97:CC,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 98:97:D1,MitraSta MitraStar Technology Corp.
 98:9A:B9,zte zte corporation
 98:9B:CB,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 98:9C:57,"HuaweiTe Huawei Technologies Co.,Ltd"
-98:9D:5D,Technico Technicolor CH USA Inc.
+98:9D:5D,VantivaU Vantiva USA LLC
 98:9D:E5,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 98:9E:63,"Apple Apple, Inc."
+98:9F:1E,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:A2:C0,"Cisco Cisco Systems, Inc"
 98:A4:04,Ericsson Ericsson AB
 98:A4:0E,"Snap Snap, Inc."
 98:A5:F9,"Apple Apple, Inc."
 98:A7:B0,Mcst Mcst Zao
 98:A9:2D,"NewH3CTe New H3C Technologies Co., Ltd"
 98:A9:42,"Guangzho Guangzhou Tozed Kangwei Intelligent Technology Co., LTD"
@@ -37607,21 +38755,23 @@
 98:AA:FC:80:00:00/28,BeijingT Beijing Tiandi-Marco Electro-Hydraulic Control System Company Ltd.
 98:AA:FC:90:00:00/28,BEAMAuth BEAM Authentic
 98:AA:FC:A0:00:00/28,"SENKO SENKO Co.,Ltd."
 98:AA:FC:B0:00:00/28,Resonant Resonant Systems Inc.
 98:AA:FC:C0:00:00/28,dots dots Inc.
 98:AA:FC:D0:00:00/28,MCSMicro MCS Micronic Computer Systeme GmbH
 98:AA:FC:E0:00:00/28,Comarch Comarch S.A.
+98:AB:15,"FujianYo Fujian Youyike Technology Co.,Ltd"
 98:AC:EF,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 98:AD:1D,"HuaweiDe Huawei Device Co., Ltd."
 98:AE:71,VVDNTech VVDN Technologies Pvt Ltd
 98:AF:65,IntelCor Intel Corporate
 98:B0:39,Nokia
 98:B0:8B,"SamsungE Samsung Electronics Co.,Ltd"
 98:B1:77,Landis+G Landis + Gyr
+98:B3:79,"Apple Apple, Inc."
 98:B3:EF,"HuaweiDe Huawei Device Co., Ltd."
 98:B6:E9,"Nintendo Nintendo Co.,Ltd"
 98:B7:85,"Shenzhen Shenzhen 10Gtek Transceivers Co., Limited"
 98:B8:BA,LGElectr LG Electronics (Mobile Communications)
 98:B8:BC,"SamsungE Samsung Electronics Co.,Ltd"
 98:B8:E3,"Apple Apple, Inc."
 98:BA:39,Doro Doro AB
@@ -37634,30 +38784,32 @@
 98:BF:F4,"MARKIN MARKIN co., Ltd."
 98:C0:EB,GlobalRe Global Regency Ltd
 98:C3:D2,"NingboSa Ningbo Sanxing Medical Electric Co.,Ltd"
 98:C5:DB,Ericsson Ericsson AB
 98:C7:A4,"Shenzhen Shenzhen HS Fiber Communication Equipment CO., LTD"
 98:C8:1C,Baytec Baytec Limited
 98:C8:45,PacketAc PacketAccess
-98:C8:54,"ChiunMai Chiun MaiCommunication System, Inc"
+98:C8:54,"ChiunMai Chiun Mai Communication System, Inc"
 98:C8:B8,"vivoMobi vivo Mobile Communication Co., Ltd."
 98:C9:7C,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 98:CA:20,Shanghai Shanghai SIMCOM Ltd.
 98:CA:33,"Apple Apple, Inc."
 98:CB:27,GaloreNe Galore Networks Pvt. Ltd.
 98:CB:A4,Benchmar Benchmark Electronics
 98:CC:4D,"Shenzhen Shenzhen mantunsci co., LTD"
 98:CC:D9,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 98:CC:E4,"Shenzhen Shenzhen Mindray Animal Medical Technology Co.,LTD"
+98:CC:F3,AmazonTe Amazon Technologies Inc.
 98:CD:AC,Espressi Espressif Inc.
 98:CD:B4,"Virident Virident Systems, Inc."
 98:CF:53,"BbkEduca Bbk Educational Electronics Corp.,Ltd."
 98:D2:93,"Google Google, Inc."
 98:D3:31,"Shenzhen Shenzhen Bolutek Technology Co.,Ltd."
 98:D3:D2,MEKRALan MEKRA Lang GmbH & Co. KG
+98:D3:D7,"HuaweiTe Huawei Technologies Co.,Ltd"
 98:D3:E7,NetafimL Netafim L
 98:D6:86,"ChyiLeei Chyi Lee industry Co., ltd."
 98:D6:BB,"Apple Apple, Inc."
 98:D6:F7,LGElectr LG Electronics (Mobile Communications)
 98:D7:42,"SamsungE Samsung Electronics Co.,Ltd"
 98:D8:63,"Shanghai Shanghai High-Flying Electronics Technology Co., Ltd"
 98:D8:8C,NortelNe Nortel Networks
@@ -37715,18 +38867,20 @@
 98:F9:C7:80:00:00/28,Renalsen Renalsense
 98:F9:C7:90:00:00/28,"KoalaTec Koala Technology CO., LTD."
 98:F9:C7:A0:00:00/28,MSBElekt MSB Elektronik und Gerätebau GmbH
 98:F9:C7:B0:00:00/28,HIROIACo HIROIA Communications Pte. Ltd. Taiwan Branch
 98:F9:C7:C0:00:00/28,"ShenZhen ShenZhen Chuangwei Electronic Appliance Co.,Ltd"
 98:F9:C7:D0:00:00/28,hangzhou hangzhou soar security technologies limited liability company
 98:F9:C7:E0:00:00/28,"NC-LINKT NC-LINK Technology Co., Ltd."
+98:F9:CC,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 98:FA:9B,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 98:FA:A7,Innonet
 98:FA:E3,XiaomiCo Xiaomi Communications Co Ltd
 98:FB:12,GrandEle Grand Electronics (HK) Ltd
+98:FB:F5,Atraltec Atraltech
 98:FC:11,"Cisco-Li Cisco-Linksys, LLC"
 98:FC:84,IEEERegi IEEE Registration Authority
 98:FC:84:00:00:00/28,"Leia Leia, Inc"
 98:FC:84:10:00:00/28,go-e go-e GmbH
 98:FC:84:20:00:00/28,"Juketek Juketek Co., Ltd."
 98:FC:84:30:00:00/28,"ZeXinSha ZeXin (Shanghai) Information Technologies Co.,Ltd"
 98:FC:84:40:00:00/28,Sferrum Sferrum GmbH
@@ -37755,16 +38909,18 @@
 9C:01:11,"Shenzhen Shenzhen Newabel Electronic Co., Ltd."
 9C:02:98,"SamsungE Samsung Electronics Co.,Ltd"
 9C:03:9E,"BeijingW Beijing Winchannel Software Technology Co., Ltd"
 9C:04:73,Tecmobil Tecmobile (International) Ltd.
 9C:04:EB,"Apple Apple, Inc."
 9C:05:67,"HonorDev Honor Device Co., Ltd."
 9C:05:91,"Mellanox Mellanox Technologies, Inc."
+9C:05:D6,Ubiquiti Ubiquiti Inc
 9C:06:1B,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 9C:06:6E,HyteraCo Hytera Communications Corporation Limited
+9C:09:71,"NewH3CTe New H3C Technologies Co., Ltd"
 9C:0B:05,eero eero inc.
 9C:0C:35,Shenzhen Shenzhenshi Xinzhongxin Technology Co.Ltd
 9C:0C:DF,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 9C:0D:AC,Tymphany Tymphany HK Limited
 9C:0E:4A,"Shenzhen Shenzhen Vastking Electronic Co.,Ltd."
 9C:13:AB,"ChansonW Chanson Water Co., Ltd."
 9C:14:63,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
@@ -37774,14 +38930,15 @@
 9C:1C:12,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 9C:1C:37,AltoBeam AltoBeam (China) Inc.
 9C:1C:6D,"HefeiDat Hefei Datang Storage Technology Co.,Ltd"
 9C:1D:36,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:1D:58,TexasIns Texas Instruments
 9C:1E:95,"Actionte Actiontec Electronics, Inc"
 9C:1E:A4,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
+9C:1E:CF,ValeoTel Valeo Telematik und Akustik GmbH
 9C:1F:CA,"Hangzhou Hangzhou AlmightyDigit Technology Co., Ltd"
 9C:1F:DD,Accupix Accupix Inc.
 9C:20:7B,"Apple Apple, Inc."
 9C:21:6A,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 9C:21:83,Broadcom Broadcom Limited
 9C:22:0E,TASCAN TASCAN Systems GmbH
 9C:25:95,"SamsungE Samsung Electronics Co.,Ltd"
@@ -37792,15 +38949,15 @@
 9C:28:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:28:F7,XiaomiCo Xiaomi Communications Co Ltd
 9C:29:3F,"Apple Apple, Inc."
 9C:29:76,IntelCor Intel Corporate
 9C:2A:70,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 9C:2A:83,"SamsungE Samsung Electronics Co.,Ltd"
 9C:2B:A6,"RuijieNe Ruijie Networks Co.,LTD"
-9C:2D:CD,"LCFCHefe LCFC(Hefei) Electronics Technology Co., Ltd"
+9C:2D:CD,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 9C:2D:CF,"ShishiTo Shishi Tongyun Technology(Chengdu)Co.,Ltd."
 9C:2E:7A,"SamsungE Samsung Electronics Co.,Ltd"
 9C:2E:A1,XiaomiCo Xiaomi Communications Co Ltd
 9C:2F:4E,zte zte corporation
 9C:2F:73,"Universa Universal Tiancheng Technology (Beijing) Co., Ltd."
 9C:2F:9D,LiteonTe Liteon Technology Corporation
 9C:30:5B,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
@@ -37853,14 +39010,15 @@
 9C:4F:CF,TCTmobil TCT mobile ltd
 9C:4F:DA,"Apple Apple, Inc."
 9C:50:D1,"MurataMa Murata Manufacturing Co., Ltd."
 9C:50:EE,"Cambridg Cambridge Industries(Group) Co.,Ltd."
 9C:52:F8,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:53:22,TP-Link TP-Link Corporation Limited
 9C:53:CD,ENGICAM ENGICAM s.r.l.
+9C:54:16,"Cisco Cisco Systems, Inc"
 9C:54:1C,"Shenzhen Shenzhen My-power Technology Co.,Ltd"
 9C:54:40,ChengDuT ChengDu TD Tech
 9C:54:67,Nokia
 9C:54:C2,"NewH3CTe New H3C Technologies Co., Ltd"
 9C:54:CA,"Zhengzho Zhengzhou VCOM Science and Technology Co.,Ltd"
 9C:54:DA,SkyBellT SkyBell Technologies Inc.
 9C:55:8F,"LockinTe Lockin Technology(Beijing) Co.,Ltd."
@@ -37885,16 +39043,17 @@
 9C:61:21,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 9C:62:AB,"Sumavisi Sumavision Technologies Co.,Ltd"
 9C:63:5B,zte zte corporation
 9C:63:ED,zte zte corporation
 9C:64:5E,HarmanCo Harman Consumer Group
 9C:64:8B,"Apple Apple, Inc."
 9C:65:B0,"SamsungE Samsung Electronics Co.,Ltd"
-9C:65:EE,DASANNet DASAN Network Solutions
+9C:65:EE,DZS DZS Inc.
 9C:65:F9,AcSiPTec AcSiP Technology Corp.
+9C:65:FA,AcSiP
 9C:66:50,"GlodioTe Glodio Technolies Co.,Ltd Tianjin Branch"
 9C:68:5B,Octonion Octonion SA
 9C:68:65,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 9C:69:37,QorvoInt Qorvo International Pte. Ltd.
 9C:69:B4,IEEERegi IEEE Registration Authority
 9C:69:B4:00:00:00/28,"SuzhouFi Suzhou Fitcan Technology Co.,LTD"
 9C:69:B4:10:00:00/28,EATechno EA Technology Ltd
@@ -37909,21 +39068,24 @@
 9C:69:B4:A0:00:00/28,"BeijingP Beijing Picohood Technology Co.,Ltd"
 9C:69:B4:B0:00:00/28,Toughdog Toughdog Security Systems
 9C:69:B4:C0:00:00/28,"Guangdon Guangdong Hanwei intergration Co.,Ltd"
 9C:69:B4:D0:00:00/28,"Intellec ""Intellect module"" LLC"
 9C:69:B4:E0:00:00/28,"NingboSh Ningbo Shen Link Communication Technology Co., Ltd"
 9C:69:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:6A:BE,QEESApS QEES ApS.
+9C:6B:00,ASRockIn ASRock Incorporation
 9C:6B:37,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 9C:6B:72,RealmeCh Realme Chongqing MobileTelecommunications Corp Ltd
 9C:6B:F0,"Shenzhen Shenzhen Yipingfang Network Technology Co., Ltd."
 9C:6C:15,Microsof Microsoft Corporation
 9C:6F:52,zte zte corporation
 9C:71:3A,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:73:70,"HuaweiTe Huawei Technologies Co.,Ltd"
+9C:73:B1,"SamsungE Samsung Electronics Co.,Ltd"
+9C:74:03,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 9C:74:1A,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:74:6F,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:75:14,Wildix Wildix srl
 9C:75:6E,AjaxDMCC Ajax Systems DMCC
 9C:76:0E,"Apple Apple, Inc."
 9C:76:13,Ring Ring LLC
 9C:77:AA,Nadasnv
@@ -37936,14 +39098,15 @@
 9C:7F:81,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
 9C:80:7D,SYSCABLE SYSCABLE Korea Inc.
 9C:80:DF,Arcadyan Arcadyan Technology Corporation
 9C:82:3F,"HuaweiDe Huawei Device Co., Ltd."
 9C:82:75,"YichipMi Yichip Microelectronics (Hangzhou) Co.,Ltd"
 9C:82:81,"vivoMobi vivo Mobile Communication Co., Ltd."
 9C:83:BF,"PRO-VISI PRO-VISION, Inc."
+9C:84:B6,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 9C:84:BF,"Apple Apple, Inc."
 9C:85:66,"Wingtech Wingtech Mobile Communications Co.,Ltd."
 9C:86:DA,PhoenixG Phoenix Geophysics Ltd.
 9C:88:24,PetroClo PetroCloud LLC
 9C:88:88,SimacTec Simac Techniek NV
 9C:88:AD,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 9C:8A:CB,JuniperN Juniper Networks
@@ -37978,14 +39141,15 @@
 9C:9C:40,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 9C:9D:5D,Raden Raden Inc
 9C:9D:7E,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 9C:9E:71,"HuaweiDe Huawei Device Co., Ltd."
 9C:A1:0A,ScleSfe Scle Sfe
 9C:A1:34,"Nike Nike, Inc."
 9C:A2:F4,TP-Link TP-Link Corporation Limited
+9C:A3:89,Nokia
 9C:A3:A9,"Guangzho Guangzhou Juan Optical and Electronical Tech Joint Stock Co., Ltd"
 9C:A3:BA,SAKURAIn SAKURA Internet Inc.
 9C:A5:13,"SamsungE Samsung Electronics Co.,Ltd"
 9C:A5:25,Shandong Shandong USR IOT Technology Limited
 9C:A5:70,eero eero inc.
 9C:A5:77,OsornoEn Osorno Enterprises Inc.
 9C:A5:C0,"vivoMobi vivo Mobile Communication Co., Ltd."
@@ -38009,43 +39173,47 @@
 9C:B7:93,Creatcom Creatcomm Technology Inc.
 9C:B8:B4,"AMPAKTec AMPAK Technology,Inc."
 9C:BB:98,"ShenZhen Shen Zhen RND Electronic Co.,LTD"
 9C:BC:F0,XiaomiCo Xiaomi Communications Co Ltd
 9C:BD:6E,"DERA DERA Co., Ltd"
 9C:BD:9D,"SkyDisk SkyDisk, Inc."
 9C:BE:E0,"Biosound Biosoundlab Co., Ltd."
+9C:BF:0D,Framewor Framework Computer LLC
 9C:BF:CD,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:C0:77,"PrintCou PrintCounts, LLC"
 9C:C0:D2,Conducti Conductix-Wampfler GmbH
 9C:C1:2D,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 9C:C1:72,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:C2:C4,"InspurEl Inspur Electronic Information Industry Co.,Ltd."
 9C:C7:A6,AVM AVM GmbH
 9C:C7:D1,SHARP SHARP Corporation
 9C:C8:93,JuniperN Juniper Networks
 9C:C8:AE,"BectonDi Becton, Dickinson and Company"
 9C:C8:FC,"ARRISGro ARRIS Group, Inc."
 9C:C9:50,Baumer Baumer Holding
 9C:C9:EB,Netgear
 9C:CA:D9,Nokia Nokia Corporation
+9C:CB:F7,"CloudSta Cloud Star Technology Co., Ltd."
 9C:CC:83,JuniperN Juniper Networks
 9C:CD:82,"ChengUei Cheng Uei Precision Industry Co.,Ltd"
+9C:D1:D0,"Guangzho Guangzhou Ronsuo Electronic Technology Co.,Ltd"
 9C:D2:1E,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 9C:D2:4B,zte zte corporation
 9C:D3:32,Technolo PLC Technology Ltd
 9C:D3:5B,"SamsungE Samsung Electronics Co.,Ltd"
 9C:D3:6D,Netgear
 9C:D4:8B,InnoluxT Innolux Technology Europe BV
 9C:D5:7D,"Cisco Cisco Systems, Inc"
 9C:D6:43,D-LinkIn D-Link International
 9C:D8:E3,"WuhanHua Wuhan Huazhong Numerical Control Co., Ltd"
 9C:D9:17,"Motorola Motorola Mobility LLC, a Lenovo Company"
 9C:D9:CB,LesiraMa Lesira Manufacturing Pty Ltd
 9C:DA:3E,IntelCor Intel Corporate
 9C:DB:07,Yellowte Yellowtec GmbH
+9C:DB:AF,"HuaweiTe Huawei Technologies Co.,Ltd"
 9C:DB:CB,"WuhanFun Wuhan Funshion Online Technologies Co.,Ltd"
 9C:DC:71,HewlettP Hewlett Packard Enterprise
 9C:DD:1F,"Intellig Intelligent Steward Co.,Ltd"
 9C:DE:4D,"MLvision ML vision Co.,LTD"
 9C:DF:03,HarmanBe Harman/Becker Automotive Systems GmbH
 9C:DF:B1,"Shenzhen Shenzhen Crave Communication Co., LTD"
 9C:E0:41,Nokia
@@ -38088,40 +39256,45 @@
 9C:F6:DD:80:00:00/28,Savari Savari Inc
 9C:F6:DD:90:00:00/28,CAMA（Luo CAMA（Luoyang）Electronics Co.，Ltd
 9C:F6:DD:A0:00:00/28,AVI AVI Pty Ltd
 9C:F6:DD:B0:00:00/28,"Guangzho Guangzhou LANGO Electronics Technology Co., Ltd."
 9C:F6:DD:C0:00:00/28,"Lighting Lighting New Energy Technology Co., Ltd."
 9C:F6:DD:D0:00:00/28,"FoshanSy Foshan Synwit Technology Co.,Ltd."
 9C:F6:DD:E0:00:00/28,ShanxiZh Shanxi ZhuoZhi fei High Electronic Technology Co. Ltd.
+9C:F8:6B,AgiTechD AgiTech Distribution Limited - Linki
 9C:F8:DB,"shenzhen shenzhen eyunmei technology co,.ltd"
 9C:F9:38,AREVANP AREVA NP GmbH
 9C:FA:3C,Daeyoung Daeyoung Electronics
+9C:FB:77,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 9C:FB:D5,"vivoMobi vivo Mobile Communication Co., Ltd."
 9C:FB:F1,MESOMATI MESOMATIC GmbH & Co.KG
 9C:FC:01,"Apple Apple, Inc."
 9C:FC:28,"Apple Apple, Inc."
 9C:FC:D1,"Aetheris Aetheris Technology (Shanghai) Co., Ltd."
 9C:FC:E8,IntelCor Intel Corporate
 9C:FE:A1,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 9C:FF:BE,OTSL OTSL Inc.
 9C:FF:C2,AVI AVI Systems GmbH
+A0:02:4A,IEEERegi IEEE Registration Authority
 A0:02:4A:00:00:00/28,"Zhejiang Zhejiang Hechuan Technology Co.,Ltd"
 A0:02:4A:10:00:00/28,VitecIma Vitec Imaging Solutions Spa
 A0:02:4A:20:00:00/28,Danriver Danriver Technologies Corp.
 A0:02:4A:30:00:00/28,SomaDete SomaDetect Inc
 A0:02:4A:40:00:00/28,ArgosSol Argos Solutions AS
 A0:02:4A:50:00:00/28,"Dongguan Dongguan Amsamotion Automation Technology Co., Ltd"
 A0:02:4A:60:00:00/28,"XiaojieT Xiaojie Technology (Shenzhen) Co., Ltd"
+A0:02:4A:70:00:00/28,EnnebiEl Ennebi Elettronica Srl
 A0:02:4A:80:00:00/28,"BeijingL Beijing Lyratone Technology Co., Ltd"
 A0:02:4A:90:00:00/28,KontaktM Kontakt Micro-Location Sp z o.o.
 A0:02:4A:A0:00:00/28,Guangdon Guangdong Jinpeng Technology Co. LTD
 A0:02:4A:B0:00:00/28,"XianYing Xi'an Yingsheng Electric Technology Co.,Ltd."
 A0:02:4A:C0:00:00/28,Encroute Encroute AB
 A0:02:4A:D0:00:00/28,bitbee bitbee Inc
 A0:02:4A:E0:00:00/28,IoTecha IoTecha Corp
+A0:02:A5,IntelCor Intel Corporate
 A0:02:DC,AmazonTe Amazon Technologies Inc.
 A0:03:63,RobertBo Robert Bosch Healthcare GmbH
 A0:04:3E,ParkerHa Parker Hannifin Manufacturing Germany GmbH & Co. KG
 A0:04:60,Netgear
 A0:06:27,NEXPASys NEXPA System
 A0:07:98,"SamsungE Samsung Electronics Co.,Ltd"
 A0:07:B6,"Advanced Advanced Technical Support, Inc."
@@ -38129,14 +39302,15 @@
 A0:09:2E,zte zte corporation
 A0:09:4C,CenturyL CenturyLink
 A0:09:ED,Avaya Avaya Inc
 A0:0A:BF,"WiesonTe Wieson Technologies Co., Ltd."
 A0:0B:BA,"SamsungE Samsung Electro Mechanics Co., Ltd."
 A0:0C:A1,SKTBSKiT SKTB SKiT
 A0:0F:37,"Cisco Cisco Systems, Inc"
+A0:10:77,zte zte corporation
 A0:10:81,"SamsungE Samsung Electronics Co.,Ltd"
 A0:12:90,Avaya Avaya Inc
 A0:12:DB,"TabuchiE Tabuchi Electric Co.,Ltd"
 A0:13:3B,"HiTiDigi HiTi Digital, Inc."
 A0:13:CB,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 A0:14:3D,Parrot Parrot Sa
 A0:16:5C,Triteka Triteka LTD
@@ -38159,25 +39333,25 @@
 A0:19:B2:A0:00:00/28,Adomi
 A0:19:B2:B0:00:00/28,"HangZhou HangZhou iMagic Technology Co., Ltd"
 A0:19:B2:C0:00:00/28,LDATechn LDA Technologies
 A0:19:B2:D0:00:00/28,"RYDElect RYD Electronic Technology Co.,Ltd."
 A0:19:B2:E0:00:00/28,AhgoraSi Ahgora Sistemas SA
 A0:1B:29,Sagemcom Sagemcom Broadband SAS
 A0:1C:05,"NimaxTel Nimax Telecom Co.,Ltd."
-A0:1C:87,"Unionman Unionman Technology Co.,Ltd"
+A0:1C:87,"UnionMan Union Man Technology Co.,Ltd"
 A0:1C:8D,"HuaweiTe Huawei Technologies Co.,Ltd"
 A0:1D:48,HewlettP Hewlett Packard
 A0:1E:0B,MINIXTec MINIX Technology Limited
 A0:20:A6,Espressi Espressif Inc.
 A0:21:8B,"ACEAnten ACE Antenna Co., ltd"
 A0:21:95,"SamsungE Samsung Electronics Co.,Ltd"
 A0:21:B7,Netgear
 A0:22:4E,IEEERegi IEEE Registration Authority
 A0:22:4E:00:00:00/28,KyungInE Kyung In Electronics
-A0:22:4E:10:00:00/28,rNETCont rNET Controls
+A0:22:4E:10:00:00/28,PoETexas PoE Texas
 A0:22:4E:20:00:00/28,"ClosedJo Closed Joint-Stock Company ""NORSI-TRANS"""
 A0:22:4E:30:00:00/28,ProPhoto ProPhotonix
 A0:22:4E:40:00:00/28,"TMGcore TMGcore, Inc."
 A0:22:4E:50:00:00/28,"ZhuhaiCh Zhuhai Cheer Technology Co., LTD."
 A0:22:4E:60:00:00/28,"MESITasd MESIT asd, s.r.o."
 A0:22:4E:70:00:00/28,"AppliedI Applied Information, Inc."
 A0:22:4E:80:00:00/28,EISSTInt EISST International Ltd
@@ -38187,14 +39361,15 @@
 A0:22:4E:C0:00:00/28,"Standart Standartoptic, Limited Liability Company"
 A0:22:4E:D0:00:00/28,Digifocu Digifocus Technology Inc.
 A0:22:4E:E0:00:00/28,"HunanYou Hunan Youmei Science&Technology Development Co.,Ltd."
 A0:22:DE,"vivoMobi vivo Mobile Communication Co., Ltd."
 A0:23:1B,TeleComp TeleComp R&D Corp.
 A0:23:9F,"Cisco Cisco Systems, Inc"
 A0:24:F9,"ChengduI Chengdu InnovaTest Technology Co., Ltd"
+A0:25:D7,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 A0:27:B6,"SamsungE Samsung Electronics Co.,Ltd"
 A0:28:33,IEEERegi IEEE Registration Authority
 A0:28:33:00:00:00/28,GERSYS GERSYS GmbH
 A0:28:33:10:00:00/28,Ordercub Ordercube GmbH
 A0:28:33:20:00:00/28,"Shanghai Shanghai Nohmi Secom Fire Protection Equipment Co.,Ltd."
 A0:28:33:30:00:00/28,"Shanghai Shanghai Xuntai Information Technology Co.,Ltd."
 A0:28:33:40:00:00/28,FirmINFO Firm INFORMTEST Ltd.
@@ -38214,21 +39389,23 @@
 A0:29:BD,TeamGrou Team Group Inc
 A0:2B:B8,HewlettP Hewlett Packard
 A0:2C:36,Fn-LinkT Fn-Link Technology Limited
 A0:2D:13,AirTiesW AirTies Wireless Networks
 A0:2E:F3,"UnitedIn United Integrated Services Co., Led."
 A0:31:31,Procenne Procenne Digital Security
 A0:31:DB,"HuaweiTe Huawei Technologies Co.,Ltd"
+A0:31:EB,Semikron Semikron Elektronik GmbH & Co. KG
 A0:32:99,"LenovoBe Lenovo (Beijing) Co., Ltd."
 A0:34:1B,Adero Adero Inc
 A0:36:79,"HuaweiTe Huawei Technologies Co.,Ltd"
 A0:36:9F,IntelCor Intel Corporate
 A0:36:BC,ASUSTekC ASUSTek COMPUTER INC.
 A0:36:F0,Comprehe Comprehensive Power
 A0:36:FA,EttusRes Ettus Research LLC
+A0:37:68,"Shenzhen Shenzhen E-Life Intelligence Technology Co.,Ltd."
 A0:38:F8,OURAHeal OURA Health Oy
 A0:39:75,LeoBodna Leo Bodnar Electronics Ltd
 A0:39:EE,Sagemcom Sagemcom Broadband SAS
 A0:39:F7,LGElectr LG Electronics (Mobile Communications)
 A0:3A:75,PSSBelgi PSS Belgium N.V.
 A0:3B:01,KyungInE Kyung In Electronics
 A0:3B:1B,InspireT Inspire Tech
@@ -38293,21 +39470,23 @@
 A0:59:3A,VDSVideo V.D.S. Video Display Systems srl
 A0:59:50,IntelCor Intel Corporate
 A0:5A:A4,"GrandPro Grand Products Nevada, Inc."
 A0:5B:21,ENVINET ENVINET GmbH
 A0:5D:C1,"TMCT TMCT Co., LTD."
 A0:5D:E7,"DIRECTV DIRECTV, Inc."
 A0:5E:6B,"MELPER MELPER Co., Ltd."
+A0:60:32,AmcrestT Amcrest Technologies
 A0:60:90,"SamsungE Samsung Electronics Co.,Ltd"
 A0:62:60,Private
 A0:62:FB,"HisenseV Hisense Visual Technology Co.,Ltd"
 A0:63:91,Netgear
 A0:64:8F,AskeyCom Askey Computer Corp
 A0:65:18,VnptTech Vnpt Technology
 A0:66:10,Fujitsu Fujitsu Limited
+A0:66:36,Intracom Intracom SA Telecom Solutions
 A0:67:20,ChinaDra China Dragon Technology Limited
 A0:67:BE,Sicon Sicon srl
 A0:68:1C,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 A0:68:7E,"ARRISGro ARRIS Group, Inc."
 A0:69:74,"HonorDev Honor Device Co., Ltd."
 A0:69:86,WellavTe Wellav Technologies Ltd
 A0:69:D9,"NewH3CTe New H3C Technologies Co., Ltd"
@@ -38326,38 +39505,42 @@
 A0:73:32,Cashmast Cashmaster International Limited
 A0:73:FC,RancoreT Rancore Technologies Private Limited
 A0:75:91,"SamsungE Samsung Electronics Co.,Ltd"
 A0:75:EA,"BoxLock BoxLock, Inc."
 A0:76:4E,Espressi Espressif Inc.
 A0:77:51,ASMediaT ASMedia Technology Inc.
 A0:77:71,Vialis Vialis BV
+A0:77:9E,ChipseaT Chipsea Technologies (Shenzhen) Corp.
 A0:78:17,"Apple Apple, Inc."
 A0:78:BA,"Pantech Pantech Co., Ltd."
+A0:7F:8A,Sagemcom Sagemcom Broadband SAS
 A0:80:69,IntelCor Intel Corporate
 A0:82:1F,"SamsungE Samsung Electronics Co.,Ltd"
 A0:82:22,"QingdaoH Qingdao Haier Technology Co.,Ltd"
 A0:82:AC,LinearDM Linear DMS Solutions Sdn. Bhd.
 A0:82:C7,"PTI P.T.I Co.,LTD"
 A0:83:B4,HeNet HeNet B.V.
 A0:84:CB,"SonicSen SonicSensory,Inc."
 A0:85:FC,Microsof Microsoft Corporation
 A0:86:1D,"ChengduF Chengdu Fuhuaxin Technology co.,Ltd"
 A0:86:C6,XiaomiCo Xiaomi Communications Co Ltd
 A0:86:EC,"SAEHANHI SAEHAN HITEC Co., Ltd"
 A0:88:69,IntelCor Intel Corporate
 A0:88:9D,"HuaweiDe Huawei Device Co., Ltd."
 A0:88:B4,IntelCor Intel Corporate
+A0:88:C2,"Mellanox Mellanox Technologies, Inc."
 A0:89:E4,"Skyworth Skyworth Digital Technology(Shenzhen) Co.,Ltd"
 A0:8A:87,"HuiZhouK HuiZhou KaiYue Electronic Co.,Ltd"
 A0:8C:15,GerhardD Gerhard D. Wempe KG
 A0:8C:9B,XtremeTe Xtreme Technologies Corp
 A0:8C:F2,"Yinuolin Yinuolink Co.,Ltd"
 A0:8C:F8,"HuaweiTe Huawei Technologies Co.,Ltd"
 A0:8C:FD,HewlettP Hewlett Packard
 A0:8D:16,"HuaweiTe Huawei Technologies Co.,Ltd"
+A0:8E:24,eero eero inc.
 A0:8E:78,Sagemcom Sagemcom Broadband SAS
 A0:90:DE,"Veedims Veedims,Llc"
 A0:91:69,LGElectr LG Electronics (Mobile Communications)
 A0:91:A2,"OnePlusE OnePlus Electronics (Shenzhen) Co., Ltd."
 A0:91:C8,zte zte corporation
 A0:92:08,TuyaSmar Tuya Smart Inc.
 A0:93:47,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -38381,30 +39564,33 @@
 A0:9F:7A,D-LinkMi D-Link Middle East FZCO
 A0:A0:01,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 A0:A0:DC,"HuaweiDe Huawei Device Co., Ltd."
 A0:A1:30,DLITaiwa DLI Taiwan Branch office
 A0:A2:3C,Gpms
 A0:A3:09,"Apple Apple, Inc."
 A0:A3:3B,"HuaweiTe Huawei Technologies Co.,Ltd"
+A0:A3:B3,Espressi Espressif Inc.
 A0:A3:B8,Wiscloud
 A0:A3:E2,"Actionte Actiontec Electronics, Inc"
 A0:A3:F0,D-LinkIn D-Link International
 A0:A4:C5,IntelCor Intel Corporate
 A0:A6:5C,Supercom Supercomputing Systems AG
 A0:A7:63,Polytron Polytron Vertrieb GmbH
 A0:A8:CD,IntelCor Intel Corporate
 A0:AA:FD,EraThink EraThink Technologies Corp.
 A0:AB:1B,D-LinkIn D-Link International
 A0:AB:51,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 A0:AC:69,"SamsungE Samsung Electronics Co.,Ltd"
 A0:AD:A1,"JMRElect JMR Electronics, Inc"
+A0:AF:12,"HuaweiTe Huawei Technologies Co.,Ltd"
 A0:AF:BD,IntelCor Intel Corporate
 A0:B0:45,HalongMi Halong Mining
 A0:B0:86,Hirschma Hirschmann Automation and Control GmbH
 A0:B1:00,"ShenZhen ShenZhen Cando Electronics Co.,Ltd"
+A0:B3:39,IntelCor Intel Corporate
 A0:B3:CC,HewlettP Hewlett Packard
 A0:B4:37,GDMissio GD Mission Systems
 A0:B4:39,"Cisco Cisco Systems, Inc"
 A0:B4:A5,"SamsungE Samsung Electronics Co.,Ltd"
 A0:B4:BF,InfiNet InfiNet LLC
 A0:B5:3C,Technico Technicolor Delivery Technologies Belgium NV
 A0:B5:49,Arcadyan Arcadyan Corporation
@@ -38431,14 +39617,15 @@
 A0:BB:3E:D0:00:00/28,Shenzhen Shenzhen Talent Technology company limited
 A0:BB:3E:E0:00:00/28,Messtech Messtechnik Sachs GmbH
 A0:BB:3E:F0:00:00/28,Private
 A0:BD:1D,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 A0:BD:CD,SkyUk Sky Uk Limited
 A0:BF:50,SCAdd-Pr S.C. Add-Production S.R.L.
 A0:BF:A5,Coresys
+A0:C2:0D,"HuaweiDe Huawei Device Co., Ltd."
 A0:C2:DE,CostarVi Costar Video Systems
 A0:C3:DE,TritonEl Triton Electronic Systems Ltd.
 A0:C4:A5,SygnHous Sygn House Inc.
 A0:C5:62,"ARRISGro ARRIS Group, Inc."
 A0:C5:89,IntelCor Intel Corporate
 A0:C5:F2,IEEERegi IEEE Registration Authority
 A0:C5:F2:00:00:00/28,"Quantlab Quantlab Financial, LLC"
@@ -38523,15 +39710,15 @@
 A0:FB:83,"HonorDev Honor Device Co., Ltd."
 A0:FB:C5,"Apple Apple, Inc."
 A0:FC:6E,Telegraf Telegrafia a.s.
 A0:FE:61,VivintWi Vivint Wireless Inc.
 A0:FE:91,AVATAuto AVAT Automation GmbH
 A0:FF:0C,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 A0:FF:22,"Shenzhen Shenzhen Apical Technology Co., Ltd"
-A0:FF:70,Technico Technicolor CH USA Inc.
+A0:FF:70,VantivaU Vantiva USA LLC
 A4:00:E2,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:01:30,"ABIsyste ABIsystems Co., LTD"
 A4:02:B9,IntelCor Intel Corporate
 A4:04:50,nForeTec nFore Technology Inc.
 A4:05:6E,Tiinlab Tiinlab Corporation
 A4:05:9E,STAInfin STA Infinity LLP
 A4:05:D6,"ARRISGro ARRIS Group, Inc."
@@ -38570,14 +39757,15 @@
 A4:11:BB,"Cisco Cisco Systems, Inc"
 A4:12:32,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 A4:12:42,"NECPlatf NEC Platforms, Ltd."
 A4:13:4E,Luxul
 A4:14:37,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 A4:15:66,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 A4:15:88,"ARRISGro ARRIS Group, Inc."
+A4:16:C0,"Apple Apple, Inc."
 A4:16:E7,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:17:31,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 A4:17:52,HifocusE Hifocus Electronics India Private Limited
 A4:17:8B,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:17:91,"Shenzhen Shenzhen Decnta Technology Co.,LTD."
 A4:18:75,"Cisco Cisco Systems, Inc"
 A4:18:94,BoschSec Bosch Security Systems B.V.
@@ -38585,14 +39773,15 @@
 A4:1A:3A,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 A4:1B:34,"ChinaMob China Mobile Group Device Co.,Ltd."
 A4:1B:C0,FastecIm Fastec Imaging Corporation
 A4:1C:B4,DFI DFI Inc
 A4:1E:E1,TaicangT Taicang T&W Electronics
 A4:1F:72,Dell Dell Inc.
 A4:21:8A,NortelNe Nortel Networks
+A4:22:49,Sagemcom Sagemcom Broadband SAS
 A4:23:05,OpenNetw Open Networking Laboratory
 A4:24:B3,FlatFrog FlatFrog Laboratories AB
 A4:24:DD,Cambrion Cambrionix Ltd
 A4:25:1B,Avaya Avaya Inc
 A4:26:18,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 A4:26:55,"LTIMotio LTI Motion (Shanghai) Co., Ltd."
 A4:28:B7,"YangtzeM Yangtze Memory Technologies Co., Ltd."
@@ -38693,22 +39882,24 @@
 A4:53:EE:30:00:00/28,Larvaio Larva.io OÜ
 A4:53:EE:40:00:00/28,Williams Williamson Corporation
 A4:53:EE:50:00:00/28,"FoshanYi Foshan Yisihang Electrical Technology Co., Ltd."
 A4:53:EE:60:00:00/28,"Shenzhen Shenzhen Xunqi Interconnet Technology Co., Ltd"
 A4:53:EE:70:00:00/28,"BeijingL Beijing Lanke Science and Technology Co.,LTd."
 A4:53:EE:80:00:00/28,"T-Touchi T-Touching Co., Ltd."
 A4:53:EE:90:00:00/28,"Dongguan Dongguan HuaFuu industrial co., LTD"
+A4:53:EE:A0:00:00/28,shanggon shanggong technology Ltd
 A4:53:EE:B0:00:00/28,"ViperDes Viper Design, LLC"
 A4:53:EE:C0:00:00/28,"SOSLAB SOS LAB Co., Ltd."
 A4:53:EE:D0:00:00/28,Ssk Ssk Corporation
+A4:53:EE:E0:00:00/28,Megacoun Megacount
 A4:55:90,XiaomiCo Xiaomi Communications Co Ltd
 A4:56:02,"fenglian fenglian Technology Co.,Ltd."
 A4:56:1B,MCOT MCOT Corporation
 A4:56:30,"Cisco Cisco Systems, Inc"
-A4:56:CC,Technico Technicolor CH USA Inc.
+A4:56:CC,VantivaU Vantiva USA LLC
 A4:58:02,Shin-IlT Shin-Il Tech
 A4:58:0F,IEEERegi IEEE Registration Authority
 A4:58:0F:00:00:00/28,Innopro
 A4:58:0F:10:00:00/28,"StoneLoc Stone Lock Global, Inc."
 A4:58:0F:20:00:00/28,BLOKS BLOKS. GmbH
 A4:58:0F:30:00:00/28,Engineer Engineered SA
 A4:58:0F:40:00:00/28,"Shenzhen Shenzhen City billion Leiden science and Technology Co., Ltd."
@@ -38740,14 +39931,15 @@
 A4:68:BC,Oakley Oakley Inc.
 A4:6B:B6,IntelCor Intel Corporate
 A4:6C:24,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:6C:2A,"Cisco Cisco Systems, Inc"
 A4:6C:C1,LTiREEne LTi REEnergy GmbH
 A4:6C:F1,"SamsungE Samsung Electronics Co.,Ltd"
 A4:6D:A4,"HuaweiTe Huawei Technologies Co.,Ltd"
+A4:6D:D4,SiliconL Silicon Laboratories
 A4:6E:79,DFTSyste DFT System Co.Ltd
 A4:70:D6,"Motorola Motorola Mobility LLC, a Lenovo Company"
 A4:71:74,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:75:B9,"SamsungE Samsung Electronics Co.,Ltd"
 A4:77:33,"Google Google, Inc."
 A4:77:58,"NingboFr Ningbo Freewings Technologies Co.,Ltd"
 A4:77:60,Nokia Nokia Corporation
@@ -38811,14 +40003,15 @@
 A4:9F:89,Shanghai Shanghai Rui Rui Communication Technology Co.Ltd.
 A4:A1:79,Nanjingd Nanjing dianyan electric power automation co. LTD
 A4:A1:C2,Ericsson Ericsson AB
 A4:A1:E4,"Innotube Innotube, Inc."
 A4:A2:4A,CiscoSPV Cisco SPVTG
 A4:A4:6B,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:A4:D3,Bluebank Bluebank Communication Technology Co.Ltd
+A4:A5:28,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 A4:A6:A9,Private
 A4:A8:0F,"Shenzhen Shenzhen Coship Electronics Co., Ltd."
 A4:AA:FE,"HuaweiDe Huawei Device Co., Ltd."
 A4:AC:0F,"HuaweiDe Huawei Device Co., Ltd."
 A4:AD:00,Ragsdale Ragsdale Technology
 A4:AD:B8,"VitecGro Vitec Group, Camera Dynamics Ltd"
 A4:AE:11,"HonHaiPr Hon Hai Precision Industry Co., Ltd."
@@ -38838,21 +40031,23 @@
 A4:B8:05,"Apple Apple, Inc."
 A4:B8:18,PENTAGes PENTA Gesellschaft für elektronische Industriedatenverarbeitung mbH
 A4:B9:80,ParkingB Parking BOXX Inc.
 A4:BA:76,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:BA:DB,Dell Dell Inc.
 A4:BB:6D,Dell Dell Inc.
 A4:BB:AF,LimeInst Lime Instruments
+A4:BD:7E,HMDGloba HMD Global Oy
 A4:BD:C4,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:BE:2B,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:BE:61,"EutroVis EutroVision System, Inc."
 A4:BF:01,IntelCor Intel Corporate
 A4:C0:C7,ShenZhen ShenZhen Hitom Communication Technology Co..LTD
 A4:C0:E1,"Nintendo Nintendo Co., Ltd."
 A4:C1:38,TelinkSe Telink Semiconductor (Taipei) Co. Ltd.
+A4:C2:3E,"HuizhouS Huizhou Speed Wireless Technology Co.,Ltd"
 A4:C2:AB,"Hangzhou Hangzhou LEAD-IT Information & Technology Co.,Ltd"
 A4:C3:37,"Apple Apple, Inc."
 A4:C3:61,"Apple Apple, Inc."
 A4:C3:F0,IntelCor Intel Corporate
 A4:C4:94,IntelCor Intel Corporate
 A4:C5:4E,"HuaweiDe Huawei Device Co., Ltd."
 A4:C6:4F,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -38860,28 +40055,31 @@
 A4:C6:F0,"Apple Apple, Inc."
 A4:C7:4B,"HuaweiDe Huawei Device Co., Ltd."
 A4:C7:DE,"Cambridg Cambridge Industries(Group) Co.,Ltd."
 A4:C7:F6,"ExtremeN Extreme Networks, Inc."
 A4:C9:39,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 A4:CA:A0,"HuaweiTe Huawei Technologies Co.,Ltd"
 A4:CC:32,"Inficomm Inficomm Co., Ltd"
+A4:CC:B3,XiaomiCo Xiaomi Communications Co Ltd
 A4:CC:B9,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 A4:CD:23,"Shenzhen Shenzhenshi Xinzhongxin Co., Ltd"
 A4:CE:DA,Arcadyan Arcadyan Corporation
 A4:CF:12,Espressi Espressif Inc.
 A4:CF:99,"Apple Apple, Inc."
 A4:CF:D2,"UbeeInte Ubee Interactive Co., Limited"
 A4:D0:94,Vivavis Vivavis Ag
 A4:D1:8C,"Apple Apple, Inc."
 A4:D1:8F,Shenzhen Shenzhen Skyee Optical Fiber Communication Technology Ltd.
 A4:D1:D1,ECOtalit ECOtality North America
 A4:D1:D2,"Apple Apple, Inc."
+A4:D2:3E,"Apple Apple, Inc."
 A4:D3:B5,"GLITELSt GLITEL Stropkov, s.r.o."
 A4:D4:B2,"Shenzhen Shenzhen MeiG Smart Technology Co.,Ltd"
 A4:D5:78,TexasIns Texas Instruments
+A4:D5:C2,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 A4:D7:3C,SeikoEps Seiko Epson Corporation
 A4:D7:95,"Wingtech Wingtech Mobile Communications Co.,Ltd"
 A4:D8:56,"Gimbal Gimbal, Inc"
 A4:D8:CA,HongKong Hong Kong Water World Technology Co. Limited
 A4:D9:31,"Apple Apple, Inc."
 A4:D9:90,"SamsungE Samsung Electronics Co.,Ltd"
 A4:D9:A4,neXusIDS neXus ID Solutions AB
@@ -38958,17 +40156,19 @@
 A4:F4:C2,VnptTech Vnpt Technology
 A4:F5:22,"ChofuSei Chofu Seisakusho Co.,Ltd"
 A4:F7:D0,"LANAcces LAN Accessories Co., Ltd."
 A4:F9:33,IntelCor Intel Corporate
 A4:F9:E4,"AirVineS AirVine Scientific, Inc."
 A4:FA:76,"NewH3CTe New H3C Technologies Co., Ltd"
 A4:FB:8D,Hangzhou Hangzhou Dunchong Technology Co.Ltd
+A4:FC:14,"Apple Apple, Inc."
 A4:FC:77,MegaWell Mega Well Limited
 A4:FC:CE,Security Security Expert Ltd.
 A4:FF:95,Nokia
+A8:00:E3,StarkeyL Starkey Labs Inc.
 A8:01:6D,Aiwa Aiwa Corporation
 A8:01:80,IMAGOTec IMAGO Technologies GmbH
 A8:02:DB,zte zte corporation
 A8:03:2A,Espressi Espressif Inc.
 A8:05:77,"Netlist Netlist, Inc."
 A8:06:00,"SamsungE Samsung Electronics Co.,Ltd"
 A8:0C:03,Florawis Florawise
@@ -38983,14 +40183,15 @@
 A8:15:59,"Breathom Breathometer, Inc."
 A8:15:D6,"Shenzhen Shenzhen Meione Technology CO., LTD"
 A8:16:9D,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 A8:16:B2,LGElectr LG Electronics (Mobile Communications)
 A8:16:D0,"SamsungE Samsung Electronics Co.,Ltd"
 A8:17:10,"Bouffalo Bouffalo Lab (Nanjing) Co., Ltd."
 A8:17:58,Elektron Elektronik System i Umeå AB
+A8:1A:F1,"Apple Apple, Inc."
 A8:1B:18,Xts Xts Corp
 A8:1B:5A,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 A8:1B:5D,FoxtelMa Foxtel Management Pty Ltd
 A8:1B:6A,TexasIns Texas Instruments
 A8:1D:16,AzureWav AzureWave Technology Inc.
 A8:1E:84,QuantaCo Quanta Computer Inc.
 A8:1F:AF,KryptonP Krypton Polska
@@ -38998,32 +40199,36 @@
 A8:23:16,Nokia
 A8:23:FE,LGElectr LG Electronics
 A8:24:B8,Nokia
 A8:24:EB,NPOIntro ZAO NPO Introtest
 A8:25:EB,"Cambridg Cambridge Industries(Group) Co.,Ltd."
 A8:26:D9,HTC HTC Corporation
 A8:29:4C,"Precisio Precision Optical Transceivers, Inc."
+A8:2A:D6,Arthrex Arthrex Inc.
 A8:2B:B5,Edgecore Edgecore Networks Corporation
 A8:2B:B9,"SamsungE Samsung Electronics Co.,Ltd"
 A8:2B:CD,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:2B:D6,"ShinaSys Shina System Co., Ltd"
+A8:2C:3E,"Shenzhen Shenzhen Cultraview Digital Technology Co., Ltd"
 A8:30:1C,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
 A8:30:AD,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 A8:30:BC,"SamsungE Samsung Electronics Co.,Ltd"
 A8:32:9A,DigicomF Digicom Futuristic Technologies Ltd.
 A8:34:6A,"SamsungE Samsung Electronics Co.,Ltd"
 A8:35:12,"HuaweiDe Huawei Device Co., Ltd."
 A8:36:7A,frogblue frogblue TECHNOLOGY GmbH
 A8:37:59,"HuaweiDe Huawei Device Co., Ltd."
 A8:39:44,"Actionte Actiontec Electronics, Inc"
 A8:3A:48,UbiqcomI Ubiqcom India Pvt Ltd
+A8:3A:79,"Mist Mist Systems, Inc."
 A8:3B:5C,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:3B:76,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 A8:3C:CB,Rossma
 A8:3E:0E,HMDGloba HMD Global Oy
+A8:3E:D3,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:3F:A1,IEEERegi IEEE Registration Authority
 A8:3F:A1:00:00:00/28,ImeconEn Imecon Engineering SrL
 A8:3F:A1:10:00:00/28,GTDevice GTDevice LLC
 A8:3F:A1:20:00:00/28,"Medcapta Medcaptain Medical Technology Co., Ltd."
 A8:3F:A1:30:00:00/28,"Guangzho Guangzhou Tupu Internet Technology Co., Ltd."
 A8:3F:A1:40:00:00/28,"Zhejiang Zhejiang Wellsun Intelligent Technology Co.,Ltd."
 A8:3F:A1:50:00:00/28,Sercomm Sercomm Corporation.
@@ -39057,20 +40262,22 @@
 A8:4B:4D,"SamsungE Samsung Electronics Co.,Ltd"
 A8:4D:4A,Audiowis Audiowise Technology Inc.
 A8:4E:3F,HitronTe Hitron Technologies. Inc
 A8:4F:B1,"Cisco Cisco Systems, Inc"
 A8:50:81,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:51:5B,"SamsungE Samsung Electronics Co.,Ltd"
 A8:51:AB,"Apple Apple, Inc."
+A8:52:D4,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 A8:53:7D,"Mist Mist Systems, Inc."
 A8:54:A2,Heimgard Heimgard Technologies AS
 A8:54:B2,WistronN Wistron Neweb Corporation
 A8:55:6A,3SSystem 3S System Technology Inc.
 A8:57:4E,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 A8:58:40,"Cambridg Cambridge Industries(Group) Co.,Ltd."
+A8:58:4E,PkVega Pk Vega
 A8:58:7C,Shoogee Shoogee GmbH & Co. KG
 A8:5A:E0,"HuaweiDe Huawei Device Co., Ltd."
 A8:5A:F3,"Shanghai Shanghai Siflower Communication Technology Co., Ltd"
 A8:5B:36,IEEERegi IEEE Registration Authority
 A8:5B:36:00:00:00/28,"BluesooT Bluesoo Tech (HongKong) Co.,Limited"
 A8:5B:36:10:00:00/28,Parma Parma Llc
 A8:5B:36:20:00:00/28,Loomanet Loomanet Inc.
@@ -39115,14 +40322,15 @@
 A8:6B:7C,"Shenzhen Shenzhen Fenglian Technology Co., Ltd."
 A8:6B:AD,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 A8:6D:5F,"Raisecom Raisecom Technology CO., LTD"
 A8:6D:AA,IntelCor Intel Corporate
 A8:6E:4E,"HuaweiDe Huawei Device Co., Ltd."
 A8:70:5D,"ARRISGro ARRIS Group, Inc."
 A8:70:A5,UniComm UniComm Inc.
+A8:71:16,EardaTec Earda Technologies co Ltd
 A8:72:7E,WISDRIwu WISDRI (wuhan) Automation Company Limited
 A8:72:85,"Idt Idt, Inc."
 A8:74:1D,PHOENIXC PHOENIX CONTACT Electronics GmbH
 A8:74:84,zte zte corporation
 A8:75:D6,"FreeTekI FreeTek International Co., Ltd."
 A8:75:E2,"Aventura Aventura Technologies, Inc."
 A8:76:50,"SamsungE Samsung Electronics Co.,Ltd"
@@ -39132,51 +40340,57 @@
 A8:7B:39,Nokia Nokia Corporation
 A8:7C:01,"SamsungE Samsung Electronics Co.,Ltd"
 A8:7C:F8,"Apple Apple, Inc."
 A8:7D:12,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:7E:33,NokiaDan Nokia Danmark A/S
 A8:7E:EA,IntelCor Intel Corporate
 A8:80:38,"ShenZhen ShenZhen MovingComm Technology Co., Limited"
+A8:80:55,TuyaSmar Tuya Smart Inc.
 A8:81:7E,"Apple Apple, Inc."
 A8:81:95,"SamsungE Samsung Electronics Co.,Ltd"
 A8:81:F1,Bmeye Bmeye B.V.
 A8:82:00,"HisenseE Hisense Electric Co.,Ltd"
 A8:82:7F,"CIBNOrie CIBN Oriental Network(Beijing) CO.,Ltd"
 A8:85:D7,SangforT Sangfor Technologies Inc.
 A8:86:DD,"Apple Apple, Inc."
 A8:87:92,Broadban Broadband Antenna Tracking Systems
 A8:87:B3,"SamsungE Samsung Electronics Co.,Ltd"
 A8:87:ED,ARCWirel ARC Wireless LLC
 A8:88:08,"Apple Apple, Inc."
+A8:88:1F,Serverco Servercom (India) Private Limited
 A8:89:40,"HuaweiDe Huawei Device Co., Ltd."
+A8:8B:28,"Shenzhen Shenzhen Diyang Smart Technology Co.,Ltd."
 A8:8C:3E,Microsof Microsoft Corporation
 A8:8C:EE,MicroMad MicroMade Galka i Drozdz sp.j.
 A8:8D:7B,SunDroid SunDroid Global limited.
 A8:8E:24,"Apple Apple, Inc."
 A8:8F:D9,"Apple Apple, Inc."
 A8:90:08,BeijingY Beijing Yuecheng Technology Co. Ltd.
 A8:90:42,"BeijingW Beijing Wanwei Intelligent Technology Co., Ltd."
 A8:91:3D,"Apple Apple, Inc."
+A8:91:62,Sophos Sophos Ltd
 A8:92:2C,LGElectr LG Electronics (Mobile Communications)
 A8:93:4A,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 A8:93:52,"Shanghai Shanghai Zhongmi Communication Technology Co.,Ltd"
 A8:93:E6,"JiangxiJ Jiangxi Jinggangshan Cking Communication Technology Co.,Ltd"
 A8:95:B0,AkerSubs Aker Subsea Ltd
 A8:96:75,"Motorola Motorola Mobility LLC, a Lenovo Company"
 A8:96:8A,"Apple Apple, Inc."
 A8:97:CD,"ARRISGro ARRIS Group, Inc."
 A8:97:DC,Ibm
 A8:98:92,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 A8:98:C6,"Shinbo Shinbo Co., Ltd."
 A8:99:5C,aizo aizo ag
 A8:99:69,Dell Dell Inc.
+A8:99:AD,"ChaoyueT Chaoyue Technology Co., Ltd."
 A8:99:DC,"i-TOPDES i-TOP DESING TECHNOLOGY CO.,LTD"
 A8:9A:93,Sagemcom Sagemcom Broadband SAS
 A8:9A:D7,Nokia
 A8:9B:10,inMotion inMotion Ltd.
+A8:9C:78,"Apple Apple, Inc."
 A8:9C:A4,Furrion Furrion Limited
 A8:9C:ED,XiaomiCo Xiaomi Communications Co Ltd
 A8:9D:21,"Cisco Cisco Systems, Inc"
 A8:9D:D2,"Shanghai Shanghai DareGlobal Technologies Co.,Ltd"
 A8:9F:BA,"SamsungE Samsung Electronics Co.,Ltd"
 A8:9F:EC,"ARRISGro ARRIS Group, Inc."
 A8:A0:89,Tactical Tactical Communications
@@ -39187,14 +40401,15 @@
 A8:A5:E2,MSF-Vath MSF-Vathauer Antriebstechnik GmbH & Co KG
 A8:A6:48,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
 A8:A6:68,zte zte corporation
 A8:A7:95,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 A8:AA:7C,"HuaweiDe Huawei Device Co., Ltd."
 A8:AB:B5,"Apple Apple, Inc."
 A8:AD:3D,"Alcatel- Alcatel-Lucent Shanghai Bell Co., Ltd"
+A8:B0:28,CubePilo CubePilot Pty Ltd
 A8:B0:88,eero eero inc.
 A8:B0:AE,BizLinkS BizLink Special Cables Germany GmbH
 A8:B1:3B,HP HP Inc.
 A8:B1:D4,"Cisco Cisco Systems, Inc"
 A8:B2:71,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:B2:DA,Fujitsu Fujitsu Limited
 A8:B4:56,"Cisco Cisco Systems, Inc"
@@ -39202,22 +40417,24 @@
 A8:B8:6E,LGElectr LG Electronics (Mobile Communications)
 A8:B9:B3,Essys
 A8:BB:50,WiZIoT WiZ IoT Company Limited
 A8:BB:CF,"Apple Apple, Inc."
 A8:BC:9C,CloudLig Cloud Light Technology Limited
 A8:BD:1A,HoneyBee Honey Bee (Hong Kong) Limited
 A8:BD:27,HewlettP Hewlett Packard Enterprise
-A8:BD:3A,"Unionman Unionman Technology Co.,Ltd"
+A8:BD:3A,"UnionMan Union Man Technology Co.,Ltd"
 A8:BE:27,"Apple Apple, Inc."
 A8:BF:3C,HDVPhoel HDV Phoelectron Technology Limited
 A8:C0:92,"HuaweiDe Huawei Device Co., Ltd."
 A8:C0:EA,Pepwave Pepwave Limited
 A8:C2:22,TM-Resea TM-Research Inc.
 A8:C2:52,"HuaweiDe Huawei Device Co., Ltd."
 A8:C2:66,"HUMAX HUMAX Co., Ltd."
+A8:C5:6F,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+A8:C6:47,"ExtremeN Extreme Networks, Inc."
 A8:C8:3A,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:C8:7F,"Roqos Roqos, Inc."
 A8:C9:8A,"NewH3CTe New H3C Technologies Co., Ltd"
 A8:CA:7B,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:CA:B9,"SamsungE Samsung Electro Mechanics Co., Ltd."
 A8:CB:95,"EastBest East Best Co., Ltd."
 A8:CC:6F,HMDGloba HMD Global Oy
@@ -39241,15 +40458,15 @@
 A8:DC:5A,DigitalW Digital Watchdog
 A8:DE:68,"BeijingW Beijing Wide Technology Co.,Ltd"
 A8:E0:18,Nokia Nokia Corporation
 A8:E2:07,GOIPGlob GOIP Global Services Pvt. Ltd.
 A8:E2:C1,TexasIns Texas Instruments
 A8:E2:C3,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 A8:E3:EE,SonyInte Sony Interactive Entertainment Inc.
-A8:E5:39,"Moimston Moimstone Co.,Ltd"
+A8:E5:39,"Nurivoic Nurivoice Co., Ltd"
 A8:E5:44,"HuaweiTe Huawei Technologies Co.,Ltd"
 A8:E5:52,JUWELAqu JUWEL Aquarium AG & Co. KG
 A8:E6:21,AmazonTe Amazon Technologies Inc.
 A8:E7:05,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 A8:E7:7D,TexasIns Texas Instruments
 A8:E8:1E,"AtwTechn Atw Technology, Inc."
 A8:E8:24,InimElec Inim Electronics S.R.L.
@@ -39266,14 +40483,15 @@
 A8:F5:DD,"ARRISGro ARRIS Group, Inc."
 A8:F7:66,ITETech ITE Tech Inc
 A8:F7:D9,"Mist Mist Systems, Inc."
 A8:F7:E0,PLANETTe PLANET Technology Corporation
 A8:F8:C9,NXPSemic NXP Semiconductor (Tianjin) LTD.
 A8:F9:4B,EltexEnt Eltex Enterprise Ltd.
 A8:FA:D8,"Apple Apple, Inc."
+A8:FB:40,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 A8:FB:70,WiseSecL WiseSec L.t.d
 A8:FC:B7,Consolid Consolidated Resource Imaging
 A8:FE:9D,"Apple Apple, Inc."
 A8:FF:BA,"HuaweiTe Huawei Technologies Co.,Ltd"
 AA:00:00,DecObsol DEC
 AA:00:01,DecObsol DEC
 AA:00:02,DecObsol DEC
@@ -39284,14 +40502,15 @@
 AA:34:D4,CDVIWire CDVI Wireless SpA
 AA:38:C7,Kaloom Kaloom inc
 AA:54:8B,Tintri
 AA:DC:47,"Cachengo Cachengo, Inc."
 AA:F0:19,Transfer TransferJet Consortium Incorporated Association
 AC:00:7A,"Apple Apple, Inc."
 AC:00:D0,zte zte corporation
+AC:00:F9,BizLinkT BizLink Technology (S.E.A) Sdn. Bhd.
 AC:01:42,UrielTec Uriel Technologies SIA
 AC:02:CA,"HISoluti HI Solutions, Inc."
 AC:02:CF,RWTecnol RW Tecnologia Industria e Comercio Ltda
 AC:02:EF,Comsis
 AC:04:0B,"PelotonI Peloton Interactive, Inc"
 AC:04:25,ball-b ball-b GmbH Co KG
 AC:04:81,"JiangsuH Jiangsu Huaxing Electronics Co., Ltd."
@@ -39301,27 +40520,30 @@
 AC:0A:61,Labor Labor S.r.L.
 AC:0B:FB,Espressi Espressif Inc.
 AC:0D:1B,LGElectr LG Electronics (Mobile Communications)
 AC:0D:FE,Ekon-myG Ekon GmbH - myGEKKO
 AC:11:D3,SuzhouHO Suzhou HOTEK Video Technology Co. Ltd
 AC:12:03,IntelCor Intel Corporate
 AC:12:2F,Fantasia Fantasia Trading LLC
+AC:12:8E,"Shanghai Shanghai Baud Data Communication Co.,Ltd."
 AC:13:9C,Adtran Adtran Inc
 AC:14:61,"ATAW ATAW Co., Ltd."
 AC:14:D2,"wi-daq wi-daq, inc."
 AC:15:85,silergy silergy corp
 AC:15:A2,TP-Link TP-Link Corporation Limited
 AC:15:F4,"Apple Apple, Inc."
 AC:16:15,"Apple Apple, Inc."
 AC:16:2D,HewlettP Hewlett Packard
 AC:17:02,FibarGro Fibar Group sp. z o.o.
+AC:17:54,tikoEner tiko Energy Solutions AG
 AC:17:C8,CiscoMer Cisco Meraki
 AC:18:26,SeikoEps Seiko Epson Corporation
 AC:19:8E,IntelCor Intel Corporate
 AC:19:9F,"SungrowP Sungrow Power Supply Co.,Ltd."
+AC:1A:3D,Dell Dell Inc.
 AC:1D:06,"Apple Apple, Inc."
 AC:1D:DF,IEEERegi IEEE Registration Authority
 AC:1D:DF:00:00:00/28,PiOctave PiOctave Solutions Pvt Ltd
 AC:1D:DF:10:00:00/28,"HellaSto HellaStorm, Inc."
 AC:1D:DF:20:00:00/28,ConectaI ConectaIP Tecnologia S.L.
 AC:1D:DF:30:00:00/28,Crde
 AC:1D:DF:40:00:00/28,Motec Motec Pty Ltd
@@ -39331,15 +40553,15 @@
 AC:1D:DF:80:00:00/28,"SichuanO Sichuan Odot Automation System Co.,Ltd."
 AC:1D:DF:90:00:00/28,SolareDa Solare Datensysteme GmbH
 AC:1D:DF:A0:00:00/28,WescoInt Wesco Integrated Supply
 AC:1D:DF:B0:00:00/28,FINEpowe FINEpowerX INC
 AC:1D:DF:C0:00:00/28,"BeijingC Beijing Chunhong Technology Co., Ltd."
 AC:1D:DF:D0:00:00/28,Elekon Elekon AG
 AC:1D:DF:E0:00:00/28,Duravit Duravit AG
-AC:1E:92,"SamsungE Samsung Electronics Co.,LTD"
+AC:1E:92,"SamsungE Samsung Electronics Co.,Ltd"
 AC:1E:9E,XiaomiCo Xiaomi Communications Co Ltd
 AC:1E:D0,TemicAut Temic Automotive Philippines Inc.
 AC:1F:09,"shenzhen shenzhen RAKwireless technology Co.,Ltd"
 AC:1F:0F,TexasIns Texas Instruments
 AC:1F:6B,"SuperMic Super Micro Computer, Inc."
 AC:1F:74,"Apple Apple, Inc."
 AC:1F:D7,"RealVisi Real Vision Technology Co.,Ltd."
@@ -39370,49 +40592,53 @@
 AC:37:28,TaicangT Taicang T&W Electronics
 AC:37:43,HTC HTC Corporation
 AC:37:C9,RAID RAID Incorporated
 AC:38:70,LenovoMo Lenovo Mobile Communication Technology Ltd.
 AC:3A:67,"Cisco Cisco Systems, Inc"
 AC:3A:7A,"Roku Roku, Inc."
 AC:3B:77,Sagemcom Sagemcom Broadband SAS
+AC:3B:96,NXPSemic NXP Semiconductor (Tianjin) LTD.
 AC:3C:0B,"Apple Apple, Inc."
 AC:3C:8E,"Flextron Flextronics Computing(Suzhou)Co.,Ltd."
 AC:3C:B4,Nilan Nilan A/S
 AC:3D:05,Instores Instorescreen Aisa
 AC:3D:75,"Hangzhou Hangzhou Zhiway Technologies Co.,Ltd."
+AC:3D:94,AristaNe Arista Networks
 AC:3E:B1,"Google Google, Inc."
 AC:3F:A4,"TaiyoYud Taiyo Yuden Co.,Ltd"
 AC:40:EA,C&TSolut C&T Solution Inc.
 AC:41:22,EclipseE Eclipse Electronic Systems Inc.
+AC:41:6A,AmazonTe Amazon Technologies Inc.
 AC:42:28,PartaNet Parta Networks
 AC:43:30,VersaNet Versa Networks
 AC:44:F2,Yamaha Yamaha Corporation
 AC:45:00,"Apple Apple, Inc."
 AC:47:1B,"HuaweiDe Huawei Device Co., Ltd."
 AC:47:23,Genelec
 AC:48:2D,"RalinwiN Ralinwi Nanjing Electronic Technology Co., Ltd."
 AC:49:DB,"Apple Apple, Inc."
 AC:4A:56,"Cisco Cisco Systems, Inc"
 AC:4A:67,"Cisco Cisco Systems, Inc"
 AC:4A:FE,"HisenseB Hisense Broadband Multimedia Technology Co.,Ltd."
 AC:4B:1E,Integri- Integri-Sys.Com LLC
 AC:4B:C8,JuniperN Juniper Networks
-AC:4C:A5,Technico Technicolor CH USA Inc.
+AC:4C:A5,VantivaU Vantiva USA LLC
 AC:4D:16,TexasIns Texas Instruments
+AC:4D:D9,"ExtremeN Extreme Networks, Inc."
 AC:4E:2E,Shenzhen Shenzhen JingHanDa Electronics Co.Ltd
 AC:4E:65,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 AC:4E:91,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:4F:FC,SVS-VIST SVS-VISTEK GmbH
 AC:50:36,Pi-Coral Pi-Coral Inc
 AC:50:93,MagnaEle Magna Electronics Europe GmbH & Co. OHG
 AC:50:DE,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 AC:51:2C,Infinixm Infinix mobility limited
 AC:51:35,MpiTech Mpi Tech
 AC:51:AB,"HuaweiTe Huawei Technologies Co.,Ltd"
-AC:51:EE,Cambridg Cambridge Communication Systems Ltd
+AC:51:EE,Adtran Adtran Inc
 AC:54:74,ChinaMob China Mobile IOT Company Limited
 AC:54:EC,IEEEP182 IEEE P1823 Standards Working Group
 AC:56:2C,LavaInte Lava International(H.K) Limited
 AC:56:7B,SunnovoI Sunnovo International Limited
 AC:57:75,HMDGloba HMD Global Oy
 AC:58:3B,"HumanAss Human Assembler, Inc."
 AC:58:7B,JCTHealt JCT Healthcare
@@ -39480,45 +40706,53 @@
 AC:76:4C,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 AC:77:13,"Honeywel Honeywell Safety Products (Shanghai) Co.,Ltd"
 AC:77:B9,"NanjingY Nanjing Yufei Intelligent Control Technology Co.,LTD"
 AC:78:D1,JuniperN Juniper Networks
 AC:7A:42,iConnect iConnectivity
 AC:7A:4D,"Alpsalpi Alpsalpine Co,.Ltd"
 AC:7A:56,"Cisco Cisco Systems, Inc"
+AC:7A:94,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 AC:7B:A1,IntelCor Intel Corporate
 AC:7E:01,"HuaweiDe Huawei Device Co., Ltd."
 AC:7E:8A,"Cisco Cisco Systems, Inc"
 AC:7F:3E,"Apple Apple, Inc."
+AC:80:0A,Sony Sony Corporation
 AC:80:AE,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 AC:80:D6,Hexatron Hexatronic AB
+AC:80:FB,"SamsungE Samsung Electronics Co.,Ltd"
 AC:81:12,"GemtekTe Gemtek Technology Co., Ltd."
 AC:81:F3,Nokia Nokia Corporation
 AC:82:26,"QingdaoH Qingdao Haier Technology Co.,Ltd"
 AC:82:47,IntelCor Intel Corporate
 AC:83:17,"Shenzhen Shenzhen Furtunetel Communication Co., Ltd"
 AC:83:E9,"BeijingZ Beijing Zile Technology Co., Ltd"
 AC:83:F0,CobaltDi Cobalt Digital Inc.
 AC:83:F3,"AMPAKTec AMPAK Technology, Inc."
 AC:84:C6,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 AC:84:C9,Sagemcom Sagemcom Broadband SAS
 AC:85:3D,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:86:74,"OpenMesh Open Mesh, Inc."
 AC:86:7E,CreateNe Create New Technology (HK) Limited Company
+AC:86:A3,"Apple Apple, Inc."
 AC:87:A3,"Apple Apple, Inc."
 AC:88:FD,"Apple Apple, Inc."
 AC:89:95,AzureWav AzureWave Technology Inc.
+AC:89:D2,Ciena Ciena Corporation
 AC:8A:CD,"ROGERDWe ROGER D.Wensker, G.Wensker sp.j."
 AC:8B:6A,ChinaMob China Mobile IOT Company Limited
 AC:8B:9C,"PrimeraT Primera Technology, Inc."
-AC:8B:A9,Ubiquiti Ubiquiti Networks Inc.
+AC:8B:A9,Ubiquiti Ubiquiti Inc
 AC:8D:14,Smartrov Smartrove Inc
 AC:8D:34,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:8F:A9,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 AC:8F:F8,Nokia
+AC:90:73,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:90:85,"Apple Apple, Inc."
+AC:91:9B,WistronN Wistron Neweb Corporation
+AC:91:A1,Dell Dell Inc.
 AC:92:32,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:93:2F,Nokia Nokia Corporation
 AC:93:6A,"HuaweiDe Huawei Device Co., Ltd."
 AC:93:C4,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 AC:94:03,Envision Envision Peripherals Inc
 AC:95:72,"Jovision Jovision Technology Co., Ltd."
 AC:96:5B,LucidMot Lucid Motors
@@ -39563,14 +40797,15 @@
 AC:BC:B5,"Apple Apple, Inc."
 AC:BC:D9,"Cisco Cisco Systems, Inc"
 AC:BD:0B,Leimac Leimac Ltd.
 AC:BD:70,"HuaweiDe Huawei Device Co., Ltd."
 AC:BE:75,"UfineTec Ufine Technologies Co.,Ltd."
 AC:BE:B6,"Visualed Visualedge Technology Co., Ltd."
 AC:BF:71,Bose Bose Corporation
+AC:C0:48,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 AC:C1:EE,XiaomiCo Xiaomi Communications Co Ltd
 AC:C2:5D,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 AC:C2:EC,CltIntLI Clt Int'L Ind. Corp.
 AC:C3:3A,"SamsungE Samsung Electronics Co.,Ltd"
 AC:C3:58,Continen Continental Automotive Czech Republic s.r.o.
 AC:C4:A9,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 AC:C4:BD,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -39599,24 +40834,27 @@
 AC:D1:80,"Crexendo Crexendo Business Solutions, Inc."
 AC:D1:B8,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 AC:D3:1D,CiscoMer Cisco Meraki
 AC:D3:64,"AbbAbbSa Abb Spa, Abb Sace Div."
 AC:D5:64,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 AC:D6:18,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 AC:D6:57,"ShaanxiG Shaanxi GuoLian Digital TV Technology Co.,Ltd."
+AC:D7:5B,Sagemcom Sagemcom Broadband SAS
 AC:D8:29,"Bouffalo Bouffalo Lab (Nanjing) Co., Ltd."
+AC:D8:A7,BELLDESI BELLDESIGN Inc.
 AC:D9:D6,tci tci GmbH
 AC:DB:48,"ARRISGro ARRIS Group, Inc."
 AC:DB:DA,"Shenzhen Shenzhen Geniatech Inc, Ltd"
 AC:DC:CA,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:DC:E5,ProcterG Procter & Gamble Company
 AC:DE:48,Private
 AC:DF:9F,Arcadyan Arcadyan Corporation
 AC:E0:10,LiteonTe Liteon Technology Corporation
 AC:E0:69,ISAACIns ISAAC Instruments
+AC:E0:D6,koreabts
 AC:E1:4F,"Autonomi Autonomic Controls, Inc."
 AC:E2:15,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:E2:D3,HewlettP Hewlett Packard
 AC:E3:42,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:E3:48,"MadgeTec MadgeTech, Inc"
 AC:E4:03,"Shenzhen Shenzhen Visteng Technology CO.,LTD"
 AC:E4:2E,SKhynix SK hynix
@@ -39628,14 +40866,15 @@
 AC:E8:7E,Bytemark Bytemark Computer Consulting Ltd
 AC:E9:7F,IoTTech IoT Tech Limited
 AC:E9:AA,Hay Hay Systems Ltd
 AC:EA:6A,"GenixInf Genix Infocomm Co., Ltd."
 AC:EB:51,"Universa Universal Electronics, Inc."
 AC:EC:80,"ARRISGro ARRIS Group, Inc."
 AC:EC:85,eero eero inc.
+AC:ED:32,"ExtremeN Extreme Networks, Inc."
 AC:ED:5C,IntelCor Intel Corporate
 AC:EE:3B,6harmoni 6harmonics Inc
 AC:EE:64,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 AC:EE:70,FontemVe Fontem Ventures BV
 AC:EE:9E,"SamsungE Samsung Electronics Co.,Ltd"
 AC:F0:B2,BeckerEl Becker Electronics Taiwan Ltd.
 AC:F1:08,LGInnote LG Innotek
@@ -39645,18 +40884,20 @@
 AC:F6:F7,LGElectr LG Electronics (Mobile Communications)
 AC:F7:F3,XiaomiCo Xiaomi Communications Co Ltd
 AC:F8:5C,"ChengduH Chengdu Higon Integrated Circuit Design Co,. Ltd."
 AC:F8:CC,"ARRISGro ARRIS Group, Inc."
 AC:F9:70,"HuaweiTe Huawei Technologies Co.,Ltd"
 AC:F9:7E,Elesys Elesys Inc.
 AC:FA:A5,digitron
+AC:FC:82,Shenzhen Shenzhen Sundray Technologies Company Limited
 AC:FD:93,"WeifangG Weifang Goertek Electronics Co.,Ltd"
 AC:FD:CE,IntelCor Intel Corporate
 AC:FD:EC,"Apple Apple, Inc."
 AC:FE:05,ItelMobi Itel Mobile Limited
+AC:FF:6B,"HuaweiTe Huawei Technologies Co.,Ltd"
 B0:00:73,WistronN Wistron Neweb Corporation
 B0:00:B4,"Cisco Cisco Systems, Inc"
 B0:02:47,"AMPAKTec AMPAK Technology, Inc."
 B0:02:7E,MullerSe Muller Services
 B0:05:94,LiteonTe Liteon Technology Corporation
 B0:08:75,"HuaweiTe Huawei Technologies Co.,Ltd"
 B0:08:BF,"VitalCon Vital Connect, Inc."
@@ -39667,15 +40908,15 @@
 B0:10:41,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 B0:10:A0,TexasIns Texas Instruments
 B0:12:03,Dynamics Dynamics Hong Kong Limited
 B0:12:66,Futaba-K Futaba-Kikaku
 B0:14:08,Lightspe Lightspeed International Co.
 B0:16:56,"HuaweiTe Huawei Technologies Co.,Ltd"
 B0:17:43,EdisonGl Edison Global Circuits Llc
-B0:18:86,SmarDTV
+B0:18:86,SmarDTV SmarDTV Corporation
 B0:19:C6,"Apple Apple, Inc."
 B0:1B:4B,Invisibl Invisible Fun Studio Limited
 B0:1B:7C,Ontrol Ontrol A.S.
 B0:1B:D2,LeShiZhi Le Shi Zhi Xin Electronic Technology (Tianjin) Limited
 B0:1C:0C,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 B0:1C:91,Elim Elim Co
 B0:1F:29,Helvetia Helvetia INC.
@@ -39694,14 +40935,15 @@
 B0:1F:81:A0:00:00/28,Steffens Steffens Systems GmbH
 B0:1F:81:B0:00:00/28,Rademach Rademacher Geraete-Elektronik GmbH
 B0:1F:81:C0:00:00/28,AccessDe Access Device Integrated Communications Corp.
 B0:1F:81:D0:00:00/28,"TAIWANAn TAIWAN Anjie Electronics Co.,Ltd."
 B0:1F:81:E0:00:00/28,Advanced Advanced & Wise Technology Corp.
 B0:1F:81:F0:00:00/28,Private
 B0:1F:8C,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
+B0:21:6F,"HuaweiTe Huawei Technologies Co.,Ltd"
 B0:22:7A,HP HP Inc.
 B0:23:47,Shenzhen Shenzhen Giant Microelectronics Company Limited
 B0:24:91,"HuaweiDe Huawei Device Co., Ltd."
 B0:24:F3,Progeny Progeny Systems
 B0:25:AA,Private
 B0:26:28,Broadcom Broadcom Limited
 B0:26:80,"Cisco Cisco Systems, Inc"
@@ -39717,29 +40959,30 @@
 B0:35:0B,"Mobiwire Mobiwire Mobiles (Ningbo) Co.,Ltd"
 B0:35:8D,Nokia Nokia Corporation
 B0:35:9F,IntelCor Intel Corporate
 B0:35:B5,"Apple Apple, Inc."
 B0:37:95,LGElectr LG Electronics
 B0:38:29,"Siliconw Siliconware Precision Industries Co., Ltd."
 B0:38:50,"NanjingC Nanjing CAS-ZDC IOT SYSTEM CO.,LTD"
-B0:38:93,OndaTLC Onda TLC GmbH
+B0:38:93,OndaTLCI Onda TLC Italia S.r.l.
 B0:38:E2,WananHon Wanan Hongsheng Electronic Co.Ltd
 B0:39:56,Netgear
 B0:3A:CE,"HuaweiDe Huawei Device Co., Ltd."
 B0:3C:DC,IntelCor Intel Corporate
 B0:3D:96,VisionVa Vision Valley FZ LLC
 B0:3D:C2,"Wasparti Wasp artificial intelligence(Shenzhen) Co.,ltd"
 B0:3E:51,SkyUk Sky Uk Limited
 B0:3E:B0,MICRODIA MICRODIA Ltd.
 B0:3F:64,"Apple Apple, Inc."
 B0:40:89,Senient Senient Systems LTD
 B0:41:1D,ITTIMTec ITTIM Technologies
 B0:41:6F,"Shenzhen Shenzhen Maxtang Computer Co.,Ltd"
 B0:43:5D,"NuLEDs NuLEDs, Inc."
 B0:44:14,"NewH3CTe New H3C Technologies Co., Ltd"
+B0:44:9C,AssaAblo Assa Abloy AB - Yale
 B0:45:02,"HuaweiDe Huawei Device Co., Ltd."
 B0:45:15,"mirafitn mira fitness,LLC."
 B0:45:19,TCTmobil TCT mobile ltd
 B0:45:30,SkyUk Sky Uk Limited
 B0:45:45,YACOUBAu YACOUB Automation GmbH
 B0:46:92,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 B0:46:FC,MitraSta MitraStar Technology Corp.
@@ -39750,14 +40993,15 @@
 B0:4A:39,"BeijingR Beijing Roborock Technology Co., Ltd."
 B0:4A:6A,"SamsungE Samsung Electronics Co.,Ltd"
 B0:4B:68,NAKAYO NAKAYO Inc
 B0:4B:BF,PtHanSun Pt Han Sung Electoronics Indonesia
 B0:4C:05,Freseniu Fresenius Medical Care Deutschland GmbH
 B0:4E:26,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 B0:4F:13,Dell Dell Inc.
+B0:4F:A6,DongGuan DongGuan Ramaxel Memory Technology
 B0:4F:C3,"Shenzhen Shenzhen NVC Cloud Technology Co., Ltd."
 B0:50:BC,"Shenzhen Shenzhen Basicom Electronic Co.,Ltd."
 B0:51:8E,Holltech Holl technology CO.Ltd.
 B0:52:16,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 B0:53:65,ChinaMob China Mobile IOT Company Limited
 B0:55:08,"HuaweiTe Huawei Technologies Co.,Ltd"
 B0:57:06,Vallox Vallox Oy
@@ -39831,45 +41075,50 @@
 B0:91:22,TexasIns Texas Instruments
 B0:91:34,Taleo
 B0:91:37,"ISisImag ISis ImageStream Internet Solutions, Inc"
 B0:93:5B,"ARRISGro ARRIS Group, Inc."
 B0:95:75,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 B0:95:8E,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 B0:96:6C,Lanbowan Lanbowan Technology Ltd.
+B0:96:EA,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
+B0:97:38,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 B0:97:3A,E-Fuel E-Fuel Corporation
 B0:98:2B,Sagemcom Sagemcom Broadband SAS
 B0:98:9F,LgCns Lg Cns
 B0:98:BC,"HuaweiDe Huawei Device Co., Ltd."
 B0:99:28,Fujitsu Fujitsu Limited
 B0:99:D7,"SamsungE Samsung Electronics Co.,Ltd"
 B0:9A:E2,STEMMERI STEMMER IMAGING GmbH
 B0:9B:D4,GNHSoftw GNH Software India Private Limited
 B0:9F:BA,"Apple Apple, Inc."
 B0:A1:0A,Pivotal Pivotal Systems Corporation
 B0:A2:E7,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 B0:A3:7E,"QingDaoH Qing Dao Haier Telecom Co.,Ltd."
+B0:A3:F2,HuaqinTe Huaqin Technology Co. LTD
 B0:A4:54,Tripwire Tripwire Inc.
 B0:A4:60,IntelCor Intel Corporate
 B0:A4:F0,"HuaweiTe Huawei Technologies Co.,Ltd"
 B0:A6:51,"Cisco Cisco Systems, Inc"
 B0:A6:F5,"Xaptum Xaptum, Inc."
 B0:A7:2A,"Ensemble Ensemble Designs, Inc."
+B0:A7:32,Espressi Espressif Inc.
 B0:A7:37,"Roku Roku, Inc."
 B0:A7:B9,TP-Link TP-Link Corporation Limited
 B0:A8:6E,JuniperN Juniper Networks
 B0:AA:36,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 B0:AA:77,"Cisco Cisco Systems, Inc"
 B0:AA:D2,"Sichuant Sichuan tianyi kanghe communications co., LTD"
 B0:AC:D2,zte zte corporation
 B0:AC:FA,Fujitsu Fujitsu Limited
 B0:AD:AA,Avaya Avaya Inc
 B0:AE:25,Varikore Varikorea
 B0:AF:F7,"Shenzhen Shenzhen Yipingfang Network Technology Co., Ltd."
 B0:B1:13,TexasIns Texas Instruments
 B0:B1:94,zte zte corporation
+B0:B2:1C,Espressi Espressif Inc.
 B0:B2:8F,Sagemcom Sagemcom Broadband SAS
 B0:B2:DC,ZyxelCom Zyxel Communications Corporation
 B0:B3:2B,SlicanSp Slican Sp. z o.o.
 B0:B3:53,IEEERegi IEEE Registration Authority
 B0:B3:53:00:00:00/28,BlakeUK Blake UK
 B0:B3:53:10:00:00/28,"Sprocomm Sprocomm Technologies CO.,LTD."
 B0:B3:53:20:00:00/28,"RizhaoSU Rizhao SUNWAM International Co., Ltd."
@@ -39901,15 +41150,15 @@
 B0:BE:76,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 B0:BE:83,"Apple Apple, Inc."
 B0:BF:99,Wizitdon Wizitdongdo
 B0:C0:90,"ChiconyE Chicony Electronics Co., Ltd."
 B0:C1:28,AdlerELR Adler ELREHA GmbH
 B0:C1:9E,zte zte corporation
 B0:C2:05,Bionime
-B0:C2:87,Technico Technicolor CH USA Inc.
+B0:C2:87,VantivaU Vantiva USA LLC
 B0:C3:87,"GOEFER GOEFER, Inc."
 B0:C4:6C,Senseit
 B0:C4:E7,"SamsungE Samsung Electronics Co.,Ltd"
 B0:C5:3C,"Cisco Cisco Systems, Inc"
 B0:C5:54,D-LinkIn D-Link International
 B0:C5:59,"SamsungE Samsung Electronics Co.,Ltd"
 B0:C5:CA,IEEERegi IEEE Registration Authority
@@ -39928,31 +41177,33 @@
 B0:C5:CA:C0:00:00/28,XMetrics
 B0:C5:CA:D0:00:00/28,Private
 B0:C5:CA:E0:00:00/28,AudioEle Audio Elektronik İthalat İhracat San ve Tic A.Ş.
 B0:C5:CA:F0:00:00/28,Private
 B0:C6:9A,JuniperN Juniper Networks
 B0:C7:45,Buffalo Buffalo.Inc
 B0:C7:87,"HuaweiTe Huawei Technologies Co.,Ltd"
+B0:C7:DE,SiliconL Silicon Laboratories
 B0:C8:3F,"JiangsuC Jiangsu Cynray IOT Co., Ltd."
 B0:C8:AD,PeoplePo People Power Company
 B0:C9:52,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 B0:C9:5B,"BeijingS Beijing Symtech CO.,LTD"
 B0:CA:68,"Apple Apple, Inc."
 B0:CC:FE,"HuaweiDe Huawei Device Co., Ltd."
 B0:CE:18,"Zhejiang Zhejiang shenghui lighting co.,Ltd"
 B0:CF:4D,MI-ZoneT MI-Zone Technology Ireland
+B0:CF:CB,AmazonTe Amazon Technologies Inc.
 B0:D0:9C,"SamsungE Samsung Electronics Co.,Ltd"
 B0:D2:78,TexasIns Texas Instruments
 B0:D2:F5,"Vello Vello Systems, Inc."
 B0:D5:68,"Shenzhen Shenzhen Cultraview Digital Technology Co., Ltd"
 B0:D5:9D,"Shenzhen Shenzhen Zowee Technology Co., Ltd"
 B0:D5:CC,TexasIns Texas Instruments
 B0:D7:C5,Logipix Logipix Ltd
 B0:D7:CC,Tridonic Tridonic GmbH & Co KG
-B0:D8:88,Panasoni Panasonic Corporation Automotive
+B0:D8:88,"Panasoni Panasonic Automotive Systems Co.,Ltd"
 B0:DA:00,CeraElec Cera Electronique
 B0:DA:F9,"ARRISGro ARRIS Group, Inc."
 B0:DC:EF,IntelCor Intel Corporate
 B0:DD:74,Heimgard Heimgard Technologies AS
 B0:DE:28,"Apple Apple, Inc."
 B0:DF:3A,"SamsungE Samsung Electronics Co.,Ltd"
 B0:DF:C1,"TendaTec Tenda Technology Co.,Ltd.Dongguan branch"
@@ -39978,24 +41229,26 @@
 B0:EB:7F,JuniperN Juniper Networks
 B0:EC:71,"SamsungE Samsung Electronics Co.,Ltd"
 B0:EC:8F,GmxSas Gmx Sas
 B0:EC:DD,"HuaweiTe Huawei Technologies Co.,Ltd"
 B0:EC:E1,Private
 B0:EE:45,AzureWav AzureWave Technology Inc.
 B0:EE:7B,"Roku Roku, Inc"
+B0:F0:0C,"Dongguan Dongguan Wecxw CO.,Ltd."
 B0:F1:A3,"FengfanB Fengfan (BeiJing) Technology Co., Ltd."
 B0:F1:BC,DhemaxIn Dhemax Ingenieros Ltda
 B0:F1:D8,"Apple Apple, Inc."
 B0:F1:EC,"AMPAKTec AMPAK Technology, Inc."
 B0:F2:08,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 B0:F5:30,HitronTe Hitron Technologies. Inc
 B0:F7:C4,AmazonTe Amazon Technologies Inc.
 B0:F8:93,"Shanghai Shanghai MXCHIP Information Technology Co., Ltd."
 B0:F9:63,"Hangzhou Hangzhou H3C Technologies Co., Limited"
 B0:FA:EB,"Cisco Cisco Systems, Inc"
+B0:FB:15,LairdCon Laird Connectivity
 B0:FB:DD,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 B0:FC:0D,AmazonTe Amazon Technologies Inc.
 B0:FC:36,CyberTAN CyberTAN Technology Inc.
 B0:FC:88,Sagemcom Sagemcom Broadband SAS
 B0:FD:0B,IEEERegi IEEE Registration Authority
 B0:FD:0B:00:00:00/28,"TAEHYUNG TAE HYUNG Industrial Electronics Co., Ltd."
 B0:FD:0B:10:00:00/28,IDspire IDspire Corporation Ltd.
@@ -40010,26 +41263,44 @@
 B0:FD:0B:A0:00:00/28,"TemcoJap Temco Japan Co., Ltd."
 B0:FD:0B:B0:00:00/28,"MartinLo MartinLogan, Ltd."
 B0:FD:0B:C0:00:00/28,HaltianP Haltian Products Oy
 B0:FD:0B:D0:00:00/28,HabanaLa Habana Labs LTD
 B0:FD:0B:E0:00:00/28,"Shenzhen Shenzhen FEIBIT Electronic Technology Co.,LTD"
 B0:FE:BD,Private
 B0:FE:E5,"HuaweiDe Huawei Device Co., Ltd."
+B0:FF:72,IEEERegi IEEE Registration Authority
+B0:FF:72:00:00:00/28,"ShenYang ShenYang LeShun Technology Co.,Ltd"
+B0:FF:72:10:00:00/28,"Guangzho Guangzhou Senguang Communication Technology Co., Ltd"
+B0:FF:72:20:00:00/28,MVTElekt MVT Elektrik Sanayi ve Ticaret Limited Sirketi
+B0:FF:72:30:00:00/28,Hammerhe Hammerhead Navigation Inc.
+B0:FF:72:40:00:00/28,"JiangxiX Jiangxi Xingchi Electronic Technology Co.,Ltd."
+B0:FF:72:50:00:00/28,"Shenzhen Shenzhen Ruilian Electronic Technology Co.,Ltd"
+B0:FF:72:60:00:00/28,TachyonE Tachyon Energy
+B0:FF:72:70:00:00/28,BLInnova BL Innovare
+B0:FF:72:80:00:00/28,ERARFTec ERA RF Technologies
+B0:FF:72:90:00:00/28,"JIUYEE?s JIUYEE?shenzhen) Medical Technology Co.,Ltd"
+B0:FF:72:A0:00:00/28,SimpleTh Simple Things
+B0:FF:72:B0:00:00/28,"LaunchTe Launch Tech Co., Ltd."
+B0:FF:72:C0:00:00/28,"Hopewhee Hopewheel info.Co.,Ltd."
+B0:FF:72:D0:00:00/28,TBBRenew TBB Renewable (Xiamen) Co Ltd
+B0:FF:72:E0:00:00/28,HANNINGK HANNING & KAHL GmbH & Co. KG
 B4:00:16,Ingenico Ingenico Terminals Sas
 B4:00:9C,CableWor CableWorld Ltd.
 B4:01:42,"GCIScien GCI Science & Technology Co.,LTD"
 B4:02:16,"Cisco Cisco Systems, Inc"
 B4:04:18,Smartchi Smartchip Integrated Inc.
 B4:04:21,zte zte corporation
 B4:05:5D,"InspurEl Inspur Electronic Information Industry Co.,Ltd."
 B4:05:66,"SPBest SP Best Corporation Co., LTD."
 B4:07:F9,"SamsungE Samsung Electro Mechanics Co., Ltd."
 B4:08:32,TCCommun TC Communications
 B4:09:31,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:0A:C6,DEXON DEXON Systems Ltd.
+B4:0A:D8,SonyInte Sony Interactive Entertainment Inc.
+B4:0B:1D,"SamsungE Samsung Electronics Co.,Ltd"
 B4:0B:44,"Smartisa Smartisan Technology Co., Ltd."
 B4:0B:78,BrusaEle Brusa Elektronik AG
 B4:0B:7A,BrusaEle Brusa Elektronik AG
 B4:0C:25,PaloAlto Palo Alto Networks
 B4:0E:96,Heran
 B4:0E:CF,"Bouffalo Bouffalo Lab (Nanjing) Co., Ltd."
 B4:0E:DC,"LG-Erics LG-Ericsson Co.,Ltd."
@@ -40038,15 +41309,15 @@
 B4:0F:B3,"vivoMobi vivo Mobile Communication Co., Ltd."
 B4:10:7B,TexasIns Texas Instruments
 B4:14:89,"Cisco Cisco Systems, Inc"
 B4:14:E6,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:15:13,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:15:7E,Celona Celona Inc.
 B4:17:80,DTIGroup DTI Group Ltd
-B4:17:A8,"Facebook Facebook Technologies, LLC"
+B4:17:A8,"MetaPlat Meta Platforms Technologies, LLC"
 B4:18:D1,"Apple Apple, Inc."
 B4:19:74,"Apple Apple, Inc."
 B4:1A:1D,"SamsungE Samsung Electronics Co.,Ltd"
 B4:1B:B0,"Apple Apple, Inc."
 B4:1C:30,zte zte corporation
 B4:1C:AB,"ICR ICR, inc."
 B4:1D:2B,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
@@ -40058,15 +41329,15 @@
 B4:22:00,"BrotherI Brother Industries, LTD."
 B4:23:30,Itron Itron Inc
 B4:24:E7,"CodetekT Codetek Technology Co.,Ltd"
 B4:26:5D,TaicangT Taicang T&W Electronics
 B4:28:75,FutechoS Futecho Solutions Private Limited
 B4:28:F1,"E-Prime E-Prime Co., Ltd."
 B4:29:3D,"Shenzhen Shenzhen Urovo Technology Co.,Ltd."
-B4:2A:0E,Technico Technicolor CH USA Inc.
+B4:2A:0E,VantivaU Vantiva USA LLC
 B4:2A:39,"ORBITMER ORBIT MERRET, spol. s r. o."
 B4:2C:92,"Zhejiang Zhejiang Weirong Electronic Co., Ltd"
 B4:2C:BE,DirectPa Direct Payment Solutions Limited
 B4:2D:56,"ExtremeN Extreme Networks, Inc."
 B4:2E:99,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 B4:2E:F8,ElineTec Eline Technology co.Ltd
 B4:30:52,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -40105,14 +41376,15 @@
 B4:3A:28,"SamsungE Samsung Electronics Co.,Ltd"
 B4:3A:31,SiliconL Silicon Laboratories
 B4:3A:E2,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:3D:08,GXIntern GX International BV
 B4:3D:B2,Degreane Degreane Horizon
 B4:3E:3B,"Viablewa Viableware, Inc"
 B4:40:A4,"Apple Apple, Inc."
+B4:40:DC,"SamsungE Samsung Electronics Co.,Ltd"
 B4:41:7A,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 B4:43:0D,Broadlin Broadlink Pty Ltd
 B4:43:26,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:45:06,Dell Dell Inc.
 B4:46:6B,Realtime Realtimeid As
 B4:47:5E,Avaya Avaya Inc
 B4:47:F5,EardaTec Earda Technologies co Ltd
@@ -40131,38 +41403,57 @@
 B4:4B:D6:A0:00:00/28,"Shenzhen Shenzhen Huabai Intelligent Technology Co., Ltd."
 B4:4B:D6:B0:00:00/28,DongYoun DongYoung media
 B4:4B:D6:C0:00:00/28,Impakt Impakt S.A.
 B4:4B:D6:D0:00:00/28,ElletaSo Elleta Solutions Ltd
 B4:4B:D6:E0:00:00/28,"Chunghsi Chunghsin International Electronics Co.,Ltd."
 B4:4C:3B,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 B4:4C:C2,"NrElectr Nr Electric Co., Ltd"
+B4:4D:43,IEEERegi IEEE Registration Authority
+B4:4D:43:00:00:00/28,Mihoyo
+B4:4D:43:10:00:00/28,iLineMic iLine Microsystems S.L. (B20956751)
+B4:4D:43:20:00:00/28,RgSoluti Rg Solutions Ltd
+B4:4D:43:30:00:00/28,"ETSMETec ETSME Technologies C0., Ltd."
+B4:4D:43:40:00:00/28,ALLSPACE ALL.SPACE Networks Ltd
+B4:4D:43:50:00:00/28,halstrup halstrup-walcher GmbH
+B4:4D:43:60:00:00/28,"SpotAI Spot AI, Inc."
+B4:4D:43:70:00:00/28,SernetSu Sernet (Suzhou) Technologies Corporation
+B4:4D:43:80:00:00/28,"ShenZhen ShenZhen Launch-Wonder Technology co., LTD"
+B4:4D:43:90:00:00/28,AdHocDev Ad Hoc Developments S.L
+B4:4D:43:A0:00:00/28,UAVNavig UAV Navigation
+B4:4D:43:B0:00:00/28,Paulmann Paulmann Licht GmbH
+B4:4D:43:C0:00:00/28,"Shenzhen Shenzhen Kosky Technology Co.,Ltd."
+B4:4D:43:D0:00:00/28,"Shenzhen Shenzhen CreatLentem Technology Co.,Ltd"
+B4:4D:43:E0:00:00/28,GearUPPo GearUP Portal Pte. Ltd.
 B4:4F:96,"Zhejiang Zhejiang Xinzailing Technology co., ltd"
 B4:50:62,EmBestor EmBestor Technology Inc.
 B4:51:F9,NBSoftwa NB Software
 B4:52:53,SeagateT Seagate Technology
 B4:52:7D,Sony Sony Corporation
 B4:52:7E,Sony Sony Corporation
 B4:52:A9,TexasIns Texas Instruments
 B4:54:59,"ChinaMob China Mobile (Hangzhou) Information Technology Co., Ltd."
 B4:55:70,Borea
 B4:56:B9,"Teraspek Teraspek Technologies Co.,Ltd"
 B4:56:E3,"Apple Apple, Inc."
+B4:56:FA,IOPSYSSo IOPSYS Software Solutions
 B4:57:E6,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 B4:58:61,"CRemote CRemote, LLC"
 B4:5C:A4,Thing-ta Thing-talk Wireless Communication Technologies Corporation Limited
 B4:5D:50,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 B4:5F:84,zte zte corporation
 B4:60:77,SichuanC Sichuan Changhong Electric Ltd.
 B4:60:8C,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 B4:60:ED,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 B4:61:42,"HuaweiTe Huawei Technologies Co.,Ltd"
+B4:61:E9,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 B4:61:FF,Lumigon Lumigon A/S
 B4:62:38,Exablox
 B4:62:93,"SamsungE Samsung Electronics Co.,Ltd"
 B4:62:AD,ElysiaGe Elysia Germany GmbH
+B4:63:6F,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 B4:66:98,Zealabs Zealabs srl
 B4:67:E9,"QingdaoG Qingdao GoerTek Technology Co., Ltd."
 B4:69:21,IntelCor Intel Corporate
 B4:69:5F,TCTmobil TCT mobile ltd
 B4:6B:FC,IntelCor Intel Corporate
 B4:6C:47,Panasoni Panasonic Appliances Company
 B4:6D:35,DalianSe Dalian Seasky Automation Co;Ltd
@@ -40202,14 +41493,15 @@
 B4:8A:0A,Espressi Espressif Inc.
 B4:8A:5F,JuniperN Juniper Networks
 B4:8B:19,"Apple Apple, Inc."
 B4:8C:9D,AzureWav AzureWave Technology Inc.
 B4:94:4E,"WeTeleco WeTelecom Co., Ltd."
 B4:96:91,IntelCor Intel Corporate
 B4:98:42,zte zte corporation
+B4:98:82,BrusaHyP Brusa HyPower AG
 B4:99:4C,TexasIns Texas Instruments
 B4:99:BA,HewlettP Hewlett Packard
 B4:9A:95,Shenzhen Shenzhen Boomtech Industrial Corporation
 B4:9C:DF,"Apple Apple, Inc."
 B4:9D:02,"SamsungE Samsung Electronics Co.,Ltd"
 B4:9D:0B,Bq
 B4:9D:B4,AxionTec Axion Technologies Inc.
@@ -40252,17 +41544,19 @@
 B4:A9:5A,Avaya Avaya Inc
 B4:A9:84,Symantec Symantec Corporation
 B4:A9:FC,QuantaCo Quanta Computer Inc.
 B4:A9:FE,GHIATech GHIA Technology (Shenzhen) LTD
 B4:AA:4D,"Ensequen Ensequence, Inc."
 B4:AB:2C,MtMTechn MtM Technology Corporation
 B4:AC:8C,BernUniv Bern University of Applied Sciences
+B4:AC:9D,TexasIns Texas Instruments
 B4:AD:A3,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 B4:AE:2B,Microsof Microsoft
 B4:AE:6F,"CircleRe Circle Reliance, Inc DBA Cranberry Networks"
+B4:AE:C1,"Apple Apple, Inc."
 B4:B0:17,Avaya Avaya Inc
 B4:B0:24,TP-Link TP-Link Corporation Limited
 B4:B0:55,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:B1:5A,SiemensE Siemens AG Energy Management Division
 B4:B2:65,DaehoI&T Daeho I&T
 B4:B2:91,LGElectr LG Electronics
 B4:B3:62,zte zte corporation
@@ -40272,33 +41566,35 @@
 B4:B5:AF,MinsungE Minsung Electronics
 B4:B5:B6,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 B4:B6:76,IntelCor Intel Corporate
 B4:B6:86,HewlettP Hewlett Packard
 B4:B7:42,AmazonTe Amazon Technologies Inc.
 B4:B8:59,Texa Texa Spa
 B4:B8:8D,Thuh Thuh Company
+B4:B9:E6,eero eero inc.
 B4:BA:02,Agatel Agatel Ltd
 B4:BA:12,"ChinaMob China Mobile (Hangzhou) Information Technology Co.,Ltd."
 B4:BA:9D,SkyUk Sky Uk Limited
 B4:BC:7C,TexasIns Texas Instruments
 B4:BF:F6,"SamsungE Samsung Electronics Co.,Ltd"
 B4:C0:F5,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 B4:C1:70,"YichipMi Yi chip Microelectronics (Hangzhou) Co., Ltd"
 B4:C2:6A,GarminIn Garmin International
+B4:C2:E0,"Bouffalo Bouffalo Lab (Nanjing) Co., Ltd."
 B4:C2:F7,"HuaweiDe Huawei Device Co., Ltd."
 B4:C4:4E,VXLeTech VXL eTech Pvt Ltd
 B4:C4:76,WuhanMar Wuhan Maritime Communication Research Institute
 B4:C4:FC,XiaomiCo Xiaomi Communications Co Ltd
 B4:C6:2E,MolexCMS Molex CMS
 B4:C6:F8,Axilspot Axilspot Communication
 B4:C7:99,"ExtremeN Extreme Networks, Inc."
 B4:C8:10,Umpi Umpi srl
 B4:C9:B9,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 B4:CB:57,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
-B4:CB:B8,Universa Universal Electronics
+B4:CB:B8,"Universa Universal Electronics, Inc."
 B4:CC:04,Piranti
 B4:CC:E9,Prosyst
 B4:CD:27,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:CD:F5,CubElecp Cub Elecparts Inc.
 B4:CE:40,"SamsungE Samsung Electronics Co.,Ltd"
 B4:CE:F6,HTC HTC Corporation
 B4:CE:FE,JamesCze James Czekaj
@@ -40311,39 +41607,42 @@
 B4:D6:4E,Caldero Caldero Limited
 B4:D8:A9,BetterBo BetterBots
 B4:D8:DE,"iotaComp iota Computing, Inc."
 B4:DB:91,Celestic Celestica Inc.
 B4:DC:09,"Guangzho Guangzhou Dawei Communication Co.,Ltd"
 B4:DD:15,ControlT ControlThings Oy Ab
 B4:DD:D0,Continen Continental Automotive Hungary Kft
+B4:DD:E0,"Shanghai Shanghai Amphenol Airwave Communication Electronics Co.,Ltd."
 B4:DE:31,"Cisco Cisco Systems, Inc"
 B4:DE:DF,zte zte corporation
 B4:DF:3B,Chromlec Chromlech
 B4:DF:FA,LitemaxE Litemax Electronics Inc.
 B4:E0:1D,Concepti Conception Electronique
 B4:E0:CD,"Fusion-i Fusion-io, Inc"
 B4:E1:0F,Dell Dell Inc.
 B4:E1:C4,Microsof Microsoft Mobile Oy
 B4:E1:EB,Private
 B4:E2:65,"Shenzhen Shenzhen SDMC Technology CO.,Ltd."
 B4:E3:F9,SiliconL Silicon Laboratories
 B4:E4:54,AmazonTe Amazon Technologies Inc.
 B4:E4:6B,ChinaMob China Mobile IOT Company Limited
+B4:E5:4C,"Elektra LLC ""Elektra"""
 B4:E6:2A,LGInnote LG Innotek
 B4:E6:2D,Espressi Espressif Inc.
 B4:E7:82,Vivalnk
 B4:E8:42,HongKong Hong Kong Bouffalo Lab Limited
 B4:E8:C9,XADATech XADA Technologies
 B4:E9:A3,portindu port industrial automation GmbH
 B4:E9:B0,"Cisco Cisco Systems, Inc"
 B4:EC:02,"Alpsalpi Alpsalpine Co,.Ltd"
 B4:EC:F2,"Shanghai Shanghai Listent Medical Tech Co., Ltd."
 B4:EC:FF,"WuhanIPG Wuhan IPG Technologies Co., Ltd."
 B4:ED:19,"PieDigit Pie Digital, Inc."
 B4:ED:54,WohlerTe Wohler Technologies
+B4:ED:D5,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 B4:EE:25,"Shenzhen Shenzhen Belon Technology CO.,LTD"
 B4:EE:B4,AskeyCom Askey Computer Corp
 B4:EE:D4,TexasIns Texas Instruments
 B4:EF:04,"DAIHANSc DAIHAN Scientific Co., Ltd."
 B4:EF:1C,360AITec 360 AI Technology Co.Ltd
 B4:EF:39,"SamsungE Samsung Electronics Co.,Ltd"
 B4:EF:FA,"Lemobile Lemobile Information Technology (Beijing) Co., Ltd."
@@ -40356,15 +41655,15 @@
 B4:F5:8E,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:F6:1C,"Apple Apple, Inc."
 B4:F7:A1,LGElectr LG Electronics (Mobile Communications)
 B4:F8:1E,Kinova
 B4:F9:49,optilink optilink networks pvt ltd
 B4:FA:48,"Apple Apple, Inc."
 B4:FB:E3,AltoBeam AltoBeam (China) Inc.
-B4:FB:E4,Ubiquiti Ubiquiti Networks Inc.
+B4:FB:E4,Ubiquiti Ubiquiti Inc
 B4:FB:F9,"HuaweiTe Huawei Technologies Co.,Ltd"
 B4:FC:75,"SEMAElec SEMA Electronics(HK) CO.,LTD"
 B4:FE:8C,CentroSi Centro Sicurezza Italia SpA
 B4:FF:98,"HuaweiTe Huawei Technologies Co.,Ltd"
 B8:00:18,Htel
 B8:02:A4,"Aeonsemi Aeonsemi, Inc."
 B8:03:05,IntelCor Intel Corporate
@@ -40389,14 +41688,15 @@
 B8:16:5F,LGInnote LG Innotek
 B8:16:DB,"ChantSin Chant Sincere Co.,Ltd"
 B8:17:C2,"Apple Apple, Inc."
 B8:18:6F,"Oriental Oriental Motor Co., Ltd."
 B8:19:04,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 B8:19:99,Nesys
 B8:1D:AA,LGElectr LG Electronics (Mobile Communications)
+B8:1E:A4,LiteonTe Liteon Technology Corporation
 B8:1F:5E,ApptionL Apption Labs Limited
 B8:20:8E,"Panasoni Panasonic Connect Co., Ltd."
 B8:20:E7,Guangzho Guangzhou Horizontal Information & Network Integration Co. Ltd
 B8:21:1C,"Apple Apple, Inc."
 B8:22:4F,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 B8:24:10,MagnetiM Magneti Marelli Slovakia s.r.o.
 B8:24:1A,SwedaInf Sweda Informatica Ltda
@@ -40418,23 +41718,26 @@
 B8:2F:CB,CMSElect CMS Electracom
 B8:30:A8,Road-Tra Road-Track Telematics Development
 B8:31:B5,Microsof Microsoft Corporation
 B8:32:41,"WuhanTia Wuhan Tianyu Information Industry Co., Ltd."
 B8:36:D8,Videoswi Videoswitch
 B8:37:4A,"Apple Apple, Inc."
 B8:37:65,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+B8:37:B2,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 B8:38:61,"Cisco Cisco Systems, Inc"
 B8:38:CA,"KyokkoTs Kyokko Tsushin System CO.,LTD"
+B8:38:EF,ADVAOpti ADVA Optical Networking Ltd.
 B8:3A:08,"TendaTec Tenda Technology Co.,Ltd.Dongguan branch"
 B8:3A:5A,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 B8:3A:7B,Worldpla Worldplay (Canada) Inc.
 B8:3A:9D,Alarmcom Alarm.com
 B8:3B:CC,XiaomiCo Xiaomi Communications Co Ltd
 B8:3C:28,"Apple Apple, Inc."
 B8:3D:4E,"Shenzhen Shenzhen Cultraview Digital Technology Co.,Ltd Shanghai Branch"
+B8:3D:F6,TexasIns Texas Instruments
 B8:3D:FB,"Bouffalo Bouffalo Lab (Nanjing) Co., Ltd."
 B8:3E:59,"Roku Roku, Inc."
 B8:3F:D2,"Mellanox Mellanox Technologies, Inc."
 B8:41:5F,Asp Asp Ag
 B8:41:A4,"Apple Apple, Inc."
 B8:43:E4,Vlatacom
 B8:44:AE,TCTmobil TCT mobile ltd
@@ -40445,60 +41748,66 @@
 B8:48:AA,EMMicroe EM Microelectronic
 B8:49:6D,"Apple Apple, Inc."
 B8:4D:43,HunanFn- Hunan Fn-Link Technology Limited
 B8:4D:EE,"Hisenseb Hisense broadband multimedia technology Co.,Ltd"
 B8:4F:D5,Microsof Microsoft Corporation
 B8:50:01,"ExtremeN Extreme Networks, Inc."
 B8:50:D8,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
+B8:51:A9,Nokia
 B8:53:AC,"Apple Apple, Inc."
 B8:55:10,ZioncomE Zioncom Electronics (Shenzhen) Ltd.
 B8:56:00,"HuaweiTe Huawei Technologies Co.,Ltd"
 B8:56:BD,Itt Itt Llc
 B8:57:76,lignex1
 B8:57:D8,"SamsungE Samsung Electronics Co.,Ltd"
 B8:58:10,"Numera Numera, Inc."
 B8:59:9F,"Mellanox Mellanox Technologies, Inc."
 B8:59:C8,"70mai 70mai Co.,Ltd."
 B8:59:CE,EardaTec Earda Technologies co Ltd
 B8:5A:73,"SamsungE Samsung Electronics Co.,Ltd"
 B8:5A:F7,"Ouya Ouya, Inc"
 B8:5A:FE,"HandaerC Handaer Communication Technology (Beijing) Co., Ltd"
+B8:5C:EE,"BaiduOnl Baidu Online Network Technology (Beijing) Co., Ltd"
 B8:5D:0A,"Apple Apple, Inc."
 B8:5D:C3,"HuaweiTe Huawei Technologies Co.,Ltd"
-B8:5E:71,Technico Technicolor CH USA Inc.
+B8:5E:71,VantivaU Vantiva USA LLC
 B8:5E:7B,"SamsungE Samsung Electronics Co.,Ltd"
 B8:5F:98,AmazonTe Amazon Technologies Inc.
 B8:5F:B0,"HuaweiTe Huawei Technologies Co.,Ltd"
+B8:60:61,"ChinaMob China Mobile Group Device Co.,Ltd."
 B8:60:91,OnnetTec Onnet Technologies and Innovations LLC
 B8:61:42,"BeijingT Beijing Tricolor Technology Co., Ltd"
 B8:61:6F,AcctonTe Accton Technology Corp
 B8:62:1F,"Cisco Cisco Systems, Inc"
 B8:63:4D,"Apple Apple, Inc."
 B8:63:92,"Guangdon Guangdong Genius Technology Co., Ltd."
 B8:63:BC,"ROBOTIS ROBOTIS, Co, Ltd"
 B8:64:91,CKTeleco CK Telecom Ltd
 B8:65:3B,"Bolymin Bolymin, Inc."
 B8:66:85,Sagemcom Sagemcom Broadband SAS
 B8:69:C2,"SunitecE Sunitec Enterprise Co., Ltd."
 B8:69:F4,Routerbo Routerboard.com
 B8:6A:97,Edgecore Edgecore Networks Corporation
+B8:6A:F1,Sagemcom Sagemcom Broadband SAS
 B8:6B:23,Toshiba
+B8:6C:E0,HewlettP Hewlett Packard Enterprise
 B8:6C:E8,"SamsungE Samsung Electronics Co.,Ltd"
 B8:70:F4,"CompalIn Compal Information (Kunshan) Co., Ltd."
 B8:74:24,Viessman Viessmann Elektronik GmbH
 B8:74:47,Converge Convergence Technologies
 B8:75:C0,"PayPal PayPal, Inc."
 B8:76:3F,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 B8:77:C3,METERGro METER Group
 B8:78:26,"Nintendo Nintendo Co.,Ltd"
 B8:78:2E,"Apple Apple, Inc."
 B8:78:79,RocheDia Roche Diagnostics GmbH
 B8:79:7E,SecureMe Secure Meters (UK) Limited
 B8:7A:C9,Siemens Siemens Ltd.
 B8:7B:C5,"Apple Apple, Inc."
+B8:7B:D4,"Google Google, Inc."
 B8:7C:6F,NXPChina NXP (China) Management Ltd.
 B8:7C:D0,"HuaweiDe Huawei Device Co., Ltd."
 B8:7C:F2,"ExtremeN Extreme Networks, Inc."
 B8:7E:E5,Intelbra Intelbras
 B8:80:35,Shenzhen Shenzhen Qihu Intelligent Technology Company Limited
 B8:80:4F,TexasIns Texas Instruments
 B8:81:98,IntelCor Intel Corporate
@@ -40529,14 +41838,15 @@
 B8:8F:B4,JabilCir Jabil Circuit Italia S.R.L
 B8:90:47,"Apple Apple, Inc."
 B8:91:C9,Handream Handreamnet
 B8:92:1D,BgT&A Bg T&A
 B8:94:36,"HuaweiTe Huawei Technologies Co.,Ltd"
 B8:94:70,Calix Calix Inc.
 B8:94:D2,RetailIn Retail Innovation HTT AB
+B8:94:D9,TexasIns Texas Instruments
 B8:94:E7,XiaomiCo Xiaomi Communications Co Ltd
 B8:96:74,AllDSP AllDSP GmbH & Co. KG
 B8:97:5A,BIOSTARM BIOSTAR Microtech Int'l Corp.
 B8:98:AD,"Motorola Motorola Mobility LLC, a Lenovo Company"
 B8:98:B0,Atlona Atlona Inc.
 B8:98:F7,"GioneeCo Gionee Communication Equipment Co,Ltd.ShenZhen"
 B8:99:19,"7signalS 7signal Solutions, Inc"
@@ -40553,16 +41863,19 @@
 B8:9F:CC,"HuaweiTe Huawei Technologies Co.,Ltd"
 B8:A1:4A,"Raisecom Raisecom Technology CO.,LTD"
 B8:A1:75,"Roku Roku, Inc."
 B8:A3:77,"Cisco Cisco Systems, Inc"
 B8:A3:86,D-LinkIn D-Link International
 B8:A3:E0,"BenRuiTe BenRui Technology Co.,Ltd"
 B8:A4:4F,AxisComm Axis Communications AB
+B8:A5:35,VantivaU Vantiva USA LLC
 B8:A5:8D,AxeGroup Axe Group Holdings Limited
+B8:A7:5E,"WuxiXinj Wuxi Xinjie Electric Co.,Ltd"
 B8:A8:AF,Logic Logic S.p.A.
+B8:AB:61,CiscoMer Cisco Meraki
 B8:AB:62,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 B8:AC:6F,Dell Dell Inc.
 B8:AD:3E,Bluecom
 B8:AE:1C,"SmartCub Smart Cube., Ltd"
 B8:AE:1D,"Guangzho Guangzhou Xingyi Electronic Technology Co.,Ltd"
 B8:AE:6E,"Nintendo Nintendo Co., Ltd."
 B8:AE:ED,"Elitegro Elitegroup Computer Systems Co.,Ltd."
@@ -40572,28 +41885,30 @@
 B8:B2:F7,Drimaes Drimaes Inc.
 B8:B2:F8,"Apple Apple, Inc."
 B8:B3:DC,DerekSha Derek (Shaoguan) Limited
 B8:B4:09,"SamsungE Samsung Electronics Co.,Ltd"
 B8:B4:2E,"GioneeCo Gionee Communication Equipment Co,Ltd.ShenZhen"
 B8:B7:7D,"Guangdon Guangdong Transtek Medical Electronics CO.,Ltd"
 B8:B7:D7,2GIGTech 2GIG Technologies
+B8:B7:DB,GOIPGlob GOIP Global Services Pvt. Ltd.
 B8:B7:F1,WistronN Wistron Neweb Corporation
 B8:B8:1E,IntelCor Intel Corporate
 B8:B9:4E,"Shenzhen Shenzhen iBaby Labs, Inc."
 B8:BA:68,"XianJizh Xi'an Jizhong Digital Communication Co.,Ltd"
 B8:BA:72,Cynove
 B8:BB:23,"Guangdon Guangdong Nufront CSC Co., Ltd"
 B8:BB:6D,"ENERES ENERES Co.,Ltd."
 B8:BB:AF,"SamsungE Samsung Electronics Co.,Ltd"
 B8:BC:1B,"HuaweiTe Huawei Technologies Co.,Ltd"
 B8:BC:5B,"SamsungE Samsung Electronics Co.,Ltd"
 B8:BD:79,TrendPoi TrendPoint Systems
 B8:BE:BF,"Cisco Cisco Systems, Inc"
 B8:BE:F4,devolo devolo AG
 B8:BF:83,IntelCor Intel Corporate
+B8:C0:65,"Universa Universal Electronics, Inc."
 B8:C1:11,"Apple Apple, Inc."
 B8:C1:A2,"DragonPa Dragon Path Technologies Co., Limited"
 B8:C2:27,PSTec
 B8:C2:53,JuniperN Juniper Networks
 B8:C3:85,"HuaweiTe Huawei Technologies Co.,Ltd"
 B8:C3:BF,HenanChe Henan Chengshi NetWork Technology Co.，Ltd
 B8:C4:6F,Primmcon Primmcon Industries Inc
@@ -40655,14 +41970,15 @@
 B8:E3:EE,"Universa Universal Electronics, Inc."
 B8:E5:89,Payter Payter BV
 B8:E6:0C,"Apple Apple, Inc."
 B8:E6:25,2Wire 2Wire Inc
 B8:E7:79,9Solutio 9Solutions Oy
 B8:E8:56,"Apple Apple, Inc."
 B8:E9:37,"Sonos Sonos, Inc."
+B8:EA:98,XiaomiCo Xiaomi Communications Co Ltd
 B8:EA:AA,"ICGNETWO ICG NETWORKS CO.,ltd"
 B8:EC:A3,ZyxelCom Zyxel Communications Corporation
 B8:EE:0E,Sagemcom Sagemcom Broadband SAS
 B8:EE:65,LiteonTe Liteon Technology Corporation
 B8:EE:79,"YWireTec YWire Technologies, Inc."
 B8:EF:8B,"Shenzhen Shenzhen Cannice Technology Co.,Ltd"
 B8:F0:09,Espressi Espressif Inc.
@@ -40680,14 +41996,15 @@
 B8:F7:4A,Rcntec
 B8:F8:28,Changshu Changshu Gaoshida Optoelectronic Technology Co. Ltd.
 B8:F8:53,Arcadyan Arcadyan Corporation
 B8:F8:83,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 B8:F8:BE,Bluecom
 B8:F9:34,Sony Sony Corporation
 B8:FB:AF,"XiamenIP Xiamen IPRT Technology CO.,LTD"
+B8:FC:28,ValeoVis Valeo Vision Systems
 B8:FC:9A,LeShiZhi Le Shi Zhi Xin Electronic Technology (Tianjin) Limited
 B8:FD:32,Zhejiang Zhejiang ROICX Microelectronics
 B8:FF:61,"Apple Apple, Inc."
 B8:FF:6F,Shanghai Shanghai Typrotech Technology Co.Ltd
 B8:FF:B3,MitraSta MitraStar Technology Corp.
 B8:FF:FE,TexasIns Texas Instruments
 BA:07:DA,Infinixm Infinix mobility limited
@@ -40711,14 +42028,15 @@
 BC:09:1B,IntelCor Intel Corporate
 BC:09:63,"Apple Apple, Inc."
 BC:0D:A5,TexasIns Texas Instruments
 BC:0F:2B,"FortuneT Fortune Techgroup Co.,Ltd"
 BC:0F:64,IntelCor Intel Corporate
 BC:0F:9A,D-LinkIn D-Link International
 BC:0F:A7,Ouster
+BC:0F:F3,HP HP Inc.
 BC:10:7B,"SamsungE Samsung Electronics Co.,Ltd"
 BC:12:5E,BeijingW Beijing WisVideo INC.
 BC:13:A8,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 BC:14:01,HitronTe Hitron Technologies. Inc
 BC:14:85,"SamsungE Samsung Electronics Co.,Ltd"
 BC:14:EF,ITONTech ITON Technology Limited
 BC:15:41,Nokia
@@ -40757,16 +42075,34 @@
 BC:2E:48,"ARRISGro ARRIS Group, Inc."
 BC:2E:F6,"HuaweiDe Huawei Device Co., Ltd."
 BC:2F:3D,"vivoMobi vivo Mobile Communication Co., Ltd."
 BC:30:5B,Dell Dell Inc.
 BC:30:7D,WistronN Wistron Neweb Corporation
 BC:30:7E,WistronN Wistron Neweb Corporation
 BC:30:D9,Arcadyan Arcadyan Corporation
+BC:31:98,IEEERegi IEEE Registration Authority
+BC:31:98:00:00:00/28,"Thinkcar Thinkcar Tech Co.,Ltd."
+BC:31:98:10:00:00/28,swiss-so swiss-sonic Ultraschall AG
+BC:31:98:20:00:00/28,Megapoli JSC Megapolis-telecom region
+BC:31:98:30:00:00/28,"Shenzhen Shenzhen Qichang Intelligent Technology Co., Ltd."
+BC:31:98:40:00:00/28,"Chongqin Chongqing e-skybest ELECT CO.,LIMITED"
+BC:31:98:50:00:00/28,"HunanGuk Hunan Gukam Railway Equipment Co.,Ltd"
+BC:31:98:60:00:00/28,ntcmekha ntc mekhanotronnika
+BC:31:98:70:00:00/28,"Zhejiang Zhejiang Delixi Electric Appliance Co., Ltd"
+BC:31:98:80:00:00/28,"Temposon Temposonics,LLC"
+BC:31:98:90:00:00/28,"Baisstar Baisstar (Shenzhen) Intelligence Co., Ltd."
+BC:31:98:A0:00:00/28,FujitsuC Fujitsu Component Limied
+BC:31:98:B0:00:00/28,"SuzhouAn Suzhou Anchi Control system.,Co.Ltd"
+BC:31:98:C0:00:00/28,"Innoflig Innoflight, Inc."
+BC:31:98:D0:00:00/28,"Shanghai Shanghai Sigen New Energy Technology Co., Ltd"
+BC:31:98:E0:00:00/28,Radar
 BC:32:5F,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
+BC:32:B2,"SamsungE Samsung Electronics Co.,Ltd"
 BC:33:29,SonyInte Sony Interactive Entertainment Inc.
+BC:33:40,CiscoMer Cisco Meraki
 BC:33:AC,SiliconL Silicon Laboratories
 BC:34:00,IEEERegi IEEE Registration Authority
 BC:34:00:00:00:00/28,Redvisio Redvision CCTV
 BC:34:00:10:00:00/28,IPLINKTe IPLINK Technology Corp
 BC:34:00:20:00:00/28,LifeSmar LifeSmart
 BC:34:00:30:00:00/28,Altronix Altronix Corporation
 BC:34:00:40:00:00/28,DexcelDe Dexcel Design Pvt Ltd
@@ -40802,14 +42138,15 @@
 BC:44:86,"SamsungE Samsung Electronics Co.,Ltd"
 BC:44:B0,Elastifi Elastifile
 BC:45:2E,Knowledg Knowledge Development for POF S.L.
 BC:45:5B,"SamsungE Samsung Electronics Co.,Ltd"
 BC:45:8C,"Shenzhen Shenzhen Topwise Communication Co.,Ltd"
 BC:46:99,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 BC:47:60,"SamsungE Samsung Electronics Co.,Ltd"
+BC:49:B2,"Shenzhen Shenzhen Along Communication Tech Co., Ltd"
 BC:4A:56,"Cisco Cisco Systems, Inc"
 BC:4B:79,SensingT SensingTek
 BC:4C:A0,"HuaweiTe Huawei Technologies Co.,Ltd"
 BC:4C:C4,"Apple Apple, Inc."
 BC:4D:FB,HitronTe Hitron Technologies. Inc
 BC:4E:3C,"CoreStaf Core Staff Co., Ltd."
 BC:4E:5D,"ZhongMia ZhongMiao Technology Co., Ltd."
@@ -40821,14 +42158,15 @@
 BC:54:36,"Apple Apple, Inc."
 BC:54:51,"SamsungE Samsung Electronics Co.,Ltd"
 BC:54:F9,"DrogooTe Drogoo Technology Co., Ltd."
 BC:54:FC,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 BC:57:29,"Shenzhen Shenzhen KKM Co., Ltd"
 BC:5A:56,"Cisco Cisco Systems, Inc"
 BC:5B:D5,"ARRISGro ARRIS Group, Inc."
+BC:5C:17,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
 BC:5C:4C,"Elecom Elecom Co.,Ltd."
 BC:5D:A3,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 BC:5E:33,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 BC:5E:A1,"PsiKick PsiKick, Inc."
 BC:5F:F4,ASRockIn ASRock Incorporation
 BC:5F:F6,"MercuryC Mercury Communication Technologies Co.,Ltd."
 BC:60:10,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
@@ -40874,14 +42212,15 @@
 BC:6D:05,"DusunEle Dusun Electron Co.,Ltd."
 BC:6E:64,Sony Sony Corporation
 BC:6E:6D,EMMicroe EM Microelectronic
 BC:6E:76,GreenEne Green Energy Options Ltd
 BC:6E:E2,IntelCor Intel Corporate
 BC:71:C1,"XTrillio XTrillion, Inc."
 BC:72:B1,"SamsungE Samsung Electronics Co.,Ltd"
+BC:73:A4,AndaTele Anda Telecom Pvt Ltd
 BC:74:D7,"HangZhou HangZhou JuRu Technology CO.,LTD"
 BC:75:36,"Alpsalpi Alpsalpine Co,.Ltd"
 BC:75:74,"HuaweiTe Huawei Technologies Co.,Ltd"
 BC:75:96,"BeijingB Beijing Broadwit Technology Co., Ltd."
 BC:76:4E,"Rackspac Rackspace US, Inc."
 BC:76:5E,"SamsungE Samsung Electronics Co.,Ltd"
 BC:76:70,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -40897,26 +42236,29 @@
 BC:7F:A4,XiaomiCo Xiaomi Communications Co Ltd
 BC:81:1F,Ingate Ingate Systems
 BC:81:99,"BASIC BASIC Co.,Ltd."
 BC:82:5D,"MitsumiE Mitsumi Electric Co.,Ltd."
 BC:83:85,Microsof Microsoft Corporation
 BC:83:A7,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 BC:85:1F,"SamsungE Samsung Electronics Co.,Ltd"
+BC:85:29,"JiangxiR Jiangxi Remote lntelligence Technology Co.,Ltd"
 BC:85:56,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+BC:87:FA,Bose Bose Corporation
 BC:88:93,VILLBAU VILLBAU Ltd.
 BC:88:C3,"NingboDo Ningbo Dooya Mechanic & Electronic Technology Co., Ltd"
 BC:89:A7,"Apple Apple, Inc."
 BC:8A:A3,NHNEnter NHN Entertainment
 BC:8A:E8,"QingDaoH Qing Dao Haier Telecom Co.,Ltd."
 BC:8B:55,NPPELIKS NPP ELIKS America Inc. DBA T&M Atlantic
 BC:8C:CD,SamsungE Samsung Electro-Mechanics(Thailand)
 BC:8D:0E,Nokia
 BC:90:3A,RobertBo Robert Bosch GmbH
 BC:91:B5,Infinixm Infinix mobility limited
 BC:92:6B,"Apple Apple, Inc."
+BC:93:07,"SamsungE Samsung Electronics Co.,Ltd"
 BC:93:25,"NingboJo Ningbo Joyson Preh Car Connect Co.,Ltd."
 BC:96:80,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 BC:97:40,IEEERegi IEEE Registration Authority
 BC:97:40:00:00:00/28,"AlphaESS Alpha ESS Co., Ltd."
 BC:97:40:10:00:00/28,comtac comtac AG
 BC:97:40:20:00:00/28,LattecIS Lattec I/S
 BC:97:40:30:00:00/28,Precisio Precision Galaxy Pvt. Ltd
@@ -40936,19 +42278,20 @@
 BC:98:89,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 BC:98:DF,"Motorola Motorola Mobility LLC, a Lenovo Company"
 BC:99:11,ZyxelCom Zyxel Communications Corporation
 BC:99:30,"HuaweiTe Huawei Technologies Co.,Ltd"
 BC:99:BC,FonSeeTe FonSee Technology Inc.
 BC:9A:53,"HuaweiDe Huawei Device Co., Ltd."
 BC:9B:5E,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
-BC:9B:68,Technico Technicolor CH USA Inc.
+BC:9B:68,VantivaU Vantiva USA LLC
 BC:9C:31,"HuaweiTe Huawei Technologies Co.,Ltd"
 BC:9C:C5,"BeijingH Beijing Huafei Technology Co., Ltd."
 BC:9D:42,"Shenzhen Shenzhen Rf-Link Technology Co.,Ltd."
 BC:9D:A5,DASCOMEu DASCOM Europe GmbH
+BC:9E:2C,"ChinaMob China Mobile Group Device Co.,Ltd."
 BC:9E:BB,"Nintendo Nintendo Co.,Ltd"
 BC:9F:E4,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 BC:9F:EF,"Apple Apple, Inc."
 BC:A0:42,"Shanghai Shanghai Flyco Electrical Appliance Co.,Ltd"
 BC:A1:3A,SES-imag SES-imagotag
 BC:A3:7F,Rail-Mil Rail-Mil Sp. z o.o. Sp. K.
 BC:A4:E1,Nabto
@@ -40957,20 +42300,22 @@
 BC:A5:A9,"Apple Apple, Inc."
 BC:A8:A6,IntelCor Intel Corporate
 BC:A9:20,"Apple Apple, Inc."
 BC:A9:93,CambiumN Cambium Networks Limited
 BC:A9:D6,"Cyber-Ra Cyber-Rain, Inc."
 BC:AB:7C,TRnPKORE TRnP KOREA Co Ltd
 BC:AD:28,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
+BC:AD:90,KymetaPu Kymeta Purchasing
 BC:AD:AB,Avaya Avaya Inc
 BC:AE:C5,ASUSTekC ASUSTek COMPUTER INC.
 BC:AF:87,"smartACc smartAC.com, Inc."
 BC:AF:91,TEConnec TE Connectivity Sensor Solutions
 BC:B0:E7,"HuaweiTe Huawei Technologies Co.,Ltd"
 BC:B1:81,Sharp Sharp Corporation
+BC:B1:D3,CiscoMer Cisco Meraki
 BC:B1:F3,"SamsungE Samsung Electronics Co.,Ltd"
 BC:B2:2B,EM-Tech
 BC:B3:08,"Hongkong Hongkong Ragentek Communication Technology Co.,Limited"
 BC:B8:52,"Cybera Cybera, Inc."
 BC:B8:63,"Apple Apple, Inc."
 BC:B9:23,AltaNetw Alta Networks
 BC:BA:C2,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
@@ -40980,14 +42325,15 @@
 BC:BD:84,zte zte corporation
 BC:BD:9E,ItelMobi Itel Mobile Limited
 BC:C0:0F,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 BC:C1:68,DinBoxSv DinBox Sverige AB
 BC:C2:3A,ThomsonV Thomson Video Networks
 BC:C3:1B,KygoLife Kygo Life A
 BC:C3:42,"Panasoni Panasonic Communications Co., Ltd."
+BC:C4:27,"HuaweiTe Huawei Technologies Co.,Ltd"
 BC:C4:93,"Cisco Cisco Systems, Inc"
 BC:C6:1A,SpectraE Spectra Embedded Systems
 BC:C6:DB,Nokia Nokia Corporation
 BC:C7:46,"HonHaiPr Hon Hai Precision IND.CO.,LTD"
 BC:C7:DA,EardaTec Earda Technologies co Ltd
 BC:C8:10,CiscoSPV Cisco SPVTG
 BC:CA:B5,"ARRISGro ARRIS Group, Inc."
@@ -41035,18 +42381,20 @@
 BC:EE:7B,ASUSTekC ASUSTek COMPUTER INC.
 BC:F1:71,IntelCor Intel Corporate
 BC:F1:F2,"Cisco Cisco Systems, Inc"
 BC:F2:92,"Plantron Plantronics, Inc."
 BC:F2:AF,devolo devolo AG
 BC:F3:10,"ExtremeN Extreme Networks, Inc."
 BC:F4:5F,zte zte corporation
+BC:F4:99,Rockwell Rockwell Automation
 BC:F4:D4,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 BC:F5:AC,LGElectr LG Electronics (Mobile Communications)
 BC:F6:1C,Geomodel Geomodeling Wuxi Technology Co. Ltd.
 BC:F6:85,D-LinkIn D-Link International
+BC:F7:30,"SamsungE Samsung Electronics Co.,Ltd"
 BC:F8:11,"XiamenDN Xiamen DNAKE Technology Co.,Ltd"
 BC:F8:8B,zte zte corporation
 BC:F9:F2,Teko
 BC:FA:B8,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 BC:FA:EB,"Cisco Cisco Systems, Inc"
 BC:FE:8C,"Altronic Altronic, LLC"
 BC:FE:D9,"Apple Apple, Inc."
@@ -41068,14 +42416,15 @@
 C0:12:42,AlphaSec Alpha Security Products
 C0:13:2B,SichuanC Sichuan Changhong Electric Ltd.
 C0:14:3D,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 C0:14:B8,Nokia
 C0:14:FE,"Cisco Cisco Systems, Inc"
 C0:16:92,"ChinaMob China Mobile Group Device Co.,Ltd."
 C0:17:4D,"SamsungE Samsung Electronics Co.,Ltd"
+C0:17:54,"Apple Apple, Inc."
 C0:18:03,HP HP Inc.
 C0:18:50,QuantaCo Quanta Computer Inc.
 C0:18:85,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 C0:1A:DA,"Apple Apple, Inc."
 C0:1B:23,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 C0:1C:30,"Shenzhen Shenzhen WIFI-3L Technology Co.,Ltd"
 C0:1E:9B,PixaviAS Pixavi AS
@@ -41092,14 +42441,15 @@
 C0:27:B9,"BeijingN Beijing National Railway Research & Design Institute of Signal & Communication Co., Ltd."
 C0:28:0B,"HonorDev Honor Device Co., Ltd."
 C0:28:8D,"Logitech Logitech, Inc"
 C0:29:73,Audyssey Audyssey Laboratories Inc.
 C0:29:F3,XySystem
 C0:2B:31,"PhytiumT Phytium Technology Co.,Ltd."
 C0:2B:FC,iNESappl iNES. applied informatics GmbH
+C0:2C:17,"Cisco Cisco Systems, Inc"
 C0:2C:5C,"Apple Apple, Inc."
 C0:2C:7A,"Shenzhen Shenzhen Horn Audio Co.,Ltd."
 C0:2D:EE,Cuff
 C0:2E:25,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 C0:2E:26,"iRhythmT iRhythm Technologies, Inc."
 C0:2F:F1,VoltaNet Volta Networks
 C0:33:5E,Microsof Microsoft
@@ -41131,34 +42481,39 @@
 C0:41:21,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 C0:41:F6,LgElectr Lg Electronics Inc
 C0:42:D0,JuniperN Juniper Networks
 C0:43:01,Epec Epec Oy
 C0:44:42,"Apple Apple, Inc."
 C0:44:E3,"Shenzhen Shenzhen Sinkna Electronics Co., LTD"
 C0:47:54,"vivoMobi vivo Mobile Communication Co., Ltd."
+C0:48:84,SigmaBil Sigma Bilisim Sist. Tekn. Elk. Enj. ve San. D??. Tic. Ltd. ?ti.
 C0:48:E6,"SamsungE Samsung Electronics Co.,Ltd"
 C0:48:FB,Shenzhen Shenzhen JingHanDa Electronics Co.Ltd
 C0:49:3D,Maitrise Maitrise Technologique
+C0:49:43,zte zte corporation
 C0:49:EF,Espressi Espressif Inc.
 C0:4A:00,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 C0:4A:09,"Zhejiang Zhejiang Everbright Communication Equip. Co,. Ltd"
 C0:4B:13,"WonderSo WonderSound Technology Co., Ltd"
 C0:4D:F7,Serelec
 C0:4E:30,Espressi Espressif Inc.
 C0:4E:8A,"HuaweiTe Huawei Technologies Co.,Ltd"
+C0:50:64,"ShennanC Shennan Circuits Co.,Ltd"
 C0:51:5C,zte zte corporation
 C0:51:7E,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 C0:53:36,BeijingN Beijing National Railway Research & Design Institute of Signal & Communication Group Co..Ltd.
 C0:56:27,BelkinIn Belkin International Inc.
 C0:56:E3,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 C0:57:BC,Avaya Avaya Inc
 C0:58:A7,"Pico Pico Systems Co., Ltd."
+C0:5B:44,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 C0:5E:6F,"VStonkau V. Stonkaus firma ""Kodinis Raktas"""
 C0:5E:79,"Shenzhen Shenzhen Huaxun Ark Technologies Co.,Ltd"
 C0:61:18,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
+C0:61:3D,"BioIntel BioIntelliSense, Inc."
 C0:61:9A,IEEERegi IEEE Registration Authority
 C0:61:9A:00:00:00/28,ParagonR Paragon Robotics LLC
 C0:61:9A:10:00:00/28,KidKraft
 C0:61:9A:20:00:00/28,GrupArge Grup Arge Enerji ve Kontrol Sistemleri
 C0:61:9A:30:00:00/28,"LyandAco Lyand Acoustic Technology Co.,Ltd."
 C0:61:9A:40:00:00/28,Stello
 C0:61:9A:50:00:00/28,"NanjingB Nanjing Balance Network Technology Co., Ltd"
@@ -41174,28 +42529,30 @@
 C0:62:6B,"Cisco Cisco Systems, Inc"
 C0:63:69,BinxinTe Binxin Technology(Zhejiang) Ltd.
 C0:63:94,"Apple Apple, Inc."
 C0:64:C6,Nokia Nokia Corporation
 C0:64:E4,"Cisco Cisco Systems, Inc"
 C0:65:99,"SamsungE Samsung Electronics Co.,Ltd"
 C0:67:AF,"Cisco Cisco Systems, Inc"
+C0:68:CC,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 C0:69:11,AristaNe Arista Networks
 C0:6B:55,"Motorola Motorola Mobility LLC, a Lenovo Company"
 C0:6C:0F,DobbsSta Dobbs Stanford
 C0:6C:6D,"MagneMot MagneMotion, Inc."
 C0:6D:1A,"TianjinH Tianjin Henxinhuifeng Technology Co.,Ltd."
 C0:6D:ED,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 C0:70:09,"HuaweiTe Huawei Technologies Co.,Ltd"
 C0:71:AA,"ShenZhen ShenZhen OnMicro Electronics Co.,Ltd."
 C0:74:2B,"Shenzhen Shenzhen Xunlong Software Co.,Limited"
 C0:74:AD,"Grandstr Grandstream Networks, Inc."
 C0:78:31,"HuaweiDe Huawei Device Co., Ltd."
 C0:78:78,"Flextron Flextronics Manufacturing(Zhuhai)Co.,Ltd."
 C0:79:82,"TCLKingE TCL King Electrical Appliances(Huizhou)Co.,Ltd"
 C0:7B:BC,"Cisco Cisco Systems, Inc"
+C0:7C:90,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 C0:7C:D1,Pegatron Pegatron Corporation
 C0:7E:40,"Shenzhen Shenzhen Xdk Communication Equipment Co.,Ltd"
 C0:81:35,"NingboFo Ningbo Forfan technology Co., LTD"
 C0:81:70,EffigisG Effigis GeoSolutions
 C0:83:0A,2Wire 2Wire Inc
 C0:83:59,IEEERegi IEEE Registration Authority
 C0:83:59:00:00:00/28,Chongqin Chongqing Jiuyu Smart Technology Co.Ltd.
@@ -41224,26 +42581,28 @@
 C0:88:5B,"SnDTech SnD Tech Co., Ltd."
 C0:88:6D,Securosy Securosys SA
 C0:89:97,"SamsungE Samsung Electronics Co.,Ltd"
 C0:89:AB,"ARRISGro ARRIS Group, Inc."
 C0:8A:CD,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 C0:8A:DE,RuckusWi Ruckus Wireless
 C0:8B:05,"HuaweiTe Huawei Technologies Co.,Ltd"
+C0:8B:2A,"Cisco Cisco Systems, Inc"
 C0:8B:6F,SISistem S I Sistemas Inteligentes Eletrônicos Ltda
 C0:8C:60,"Cisco Cisco Systems, Inc"
 C0:8C:71,"Motorola Motorola Mobility LLC, a Lenovo Company"
 C0:8D:51,AmazonTe Amazon Technologies Inc.
 C0:8F:20,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 C0:91:32,PatriotM Patriot Memory
 C0:91:34,ProCurve ProCurve Networking by HP
 C0:91:B9,AmazonTe Amazon Technologies Inc.
 C0:92:96,zte zte corporation
 C0:94:35,"ARRISGro ARRIS Group, Inc."
 C0:94:AD,zte zte corporation
 C0:95:6D,"Apple Apple, Inc."
+C0:95:73,AIxLink
 C0:95:DA,NXPIndia NXP India Private Limited
 C0:97:27,SamsungE Samsung Electro-Mechanics(Thailand)
 C0:98:79,Acer Acer Inc.
 C0:98:DA,ChinaMob China Mobile IOT Company Limited
 C0:98:E5,Universi University of Michigan
 C0:9A:71,XiamenMe Xiamen Meitu Mobile Technology Co.Ltd
 C0:9A:D0,"Apple Apple, Inc."
@@ -41290,14 +42649,15 @@
 C0:AA:68,OSASITec OSASI Technos Inc.
 C0:AC:54,Sagemcom Sagemcom Broadband SAS
 C0:AD:97,TecnoMob Tecno Mobile Limited
 C0:AE:FD,"Shenzhen Shenzhen HC-WLAN Technology Co.,Ltd"
 C0:B1:01,zte zte corporation
 C0:B3:39,Comigo Comigo Ltd.
 C0:B3:57,YoshikiE Yoshiki Electronics Industry Ltd.
+C0:B3:C8,"NTCRotek LLC ""NTC Rotek"""
 C0:B4:7D,"HuaweiDe Huawei Device Co., Ltd."
 C0:B5:CD,"HuaweiDe Huawei Device Co., Ltd."
 C0:B5:D7,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 C0:B6:58,"Apple Apple, Inc."
 C0:B6:F9,IntelCor Intel Corporate
 C0:B7:13,BeijingX Beijing Xiaoyuer Technology Co. Ltd.
 C0:B8:83,IntelCor Intel Corporate
@@ -41310,18 +42670,20 @@
 C0:BD:D1,SamsungE Samsung Electro-Mechanics(Thailand)
 C0:BF:A7,JuniperN Juniper Networks
 C0:BF:AC,"HuaweiDe Huawei Device Co., Ltd."
 C0:BF:C0,"HuaweiTe Huawei Technologies Co.,Ltd"
 C0:C1:70,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 C0:C1:C0,"Cisco-Li Cisco-Linksys, LLC"
 C0:C3:B6,Automati Automatic Systems
+C0:C4:F9,Qisda Qisda Corporation
 C0:C5:20,RuckusWi Ruckus Wireless
 C0:C5:22,"ARRISGro ARRIS Group, Inc."
 C0:C5:69,"Shanghai Shanghai Lynuc Cnc Technology Co.,Ltd"
 C0:C6:87,CiscoSPV Cisco SPVTG
+C0:C7:0A,RuckusWi Ruckus Wireless
 C0:C9:46,MitsuyaL Mitsuya Laboratories Inc.
 C0:C9:76,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 C0:C9:E3,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 C0:CB:38,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 C0:CB:F1,"Mobiwire Mobiwire Mobiles (NingBo) Co., LTD"
 C0:CC:42,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 C0:CC:F8,"Apple Apple, Inc."
@@ -41358,28 +42720,44 @@
 C0:D8:34,xvtec xvtec ltd
 C0:D9:62,AskeyCom Askey Computer Corp
 C0:D9:F7,"ShanDong ShanDong Domor Intelligent S&T CO.,Ltd"
 C0:DA:74,"Hangzhou Hangzhou Sunyard Technology Co., Ltd."
 C0:DC:6A,"QingdaoE Qingdao Eastsoft Communication Technology Co.,LTD"
 C0:DC:D7,"HuaweiDe Huawei Device Co., Ltd."
 C0:DC:DA,"SamsungE Samsung Electronics Co.,Ltd"
-C0:DD:8A,"Facebook Facebook Technologies, LLC"
+C0:DD:8A,"MetaPlat Meta Platforms Technologies, LLC"
 C0:DF:77,ConradEl Conrad Electronic SE
 C0:E0:18,"HuaweiTe Huawei Technologies Co.,Ltd"
 C0:E0:1C,"IoTSecur IoT Security Group, SL"
 C0:E1:BE,"HuaweiTe Huawei Technologies Co.,Ltd"
 C0:E3:A0,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 C0:E3:FB,"HuaweiTe Huawei Technologies Co.,Ltd"
 C0:E4:22,TexasIns Texas Instruments
 C0:E4:2D,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 C0:E4:34,AzureWav AzureWave Technology Inc.
 C0:E5:4E,ARIESEmb ARIES Embedded GmbH
 C0:E7:BF,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 C0:E8:62,"Apple Apple, Inc."
-C0:E9:11,Private
+C0:E9:11,RealNetw RealNetworks
+C0:EA:C3,IEEERegi IEEE Registration Authority
+C0:EA:C3:00:00:00/28,"AnhuiShe Anhui Shengjiaruiduo Electronic Technology Co., Ltd."
+C0:EA:C3:10:00:00/28,"Dongguan Dongguan Wecxw CO.,Ltd."
+C0:EA:C3:20:00:00/28,NEXSEC NEXSEC Incorporated
+C0:EA:C3:30:00:00/28,"Hangzhou Hangzhou Qixun Technology Co., Ltd"
+C0:EA:C3:40:00:00/28,Tokoz Tokoz a.s.
+C0:EA:C3:50:00:00/28,TechemEn Techem Energy Services GmbH
+C0:EA:C3:60:00:00/28,Worldpas Worldpass industrial Company Limited
+C0:EA:C3:70:00:00/28,Annapurn Annapurna labs
+C0:EA:C3:80:00:00/28,CDSTech
+C0:EA:C3:90:00:00/28,Oledcomm
+C0:EA:C3:A0:00:00/28,VoltEqui Volt Equipamentos Eletronicos Ltda
+C0:EA:C3:B0:00:00/28,SeongHoI SeongHo Information and Communication Corp.
+C0:EA:C3:C0:00:00/28,Trumeter
+C0:EA:C3:D0:00:00/28,KontronA Kontron Asia Technology Inc.
+C0:EA:C3:E0:00:00/28,BeijingZ Beijing Zhongyuanyishang Technology Co Ltd
 C0:EA:E4,Sonicwal Sonicwall
 C0:ED:E5,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 C0:EE:40,LairdCon Laird Connectivity
 C0:EE:B5,EniceNet Enice Network.
 C0:EE:FB,OnePlusT OnePlus Tech (Shenzhen) Ltd
 C0:F1:C4,Pacidal Pacidal Corporation Ltd.
 C0:F2:FB,"Apple Apple, Inc."
@@ -41467,15 +42845,15 @@
 C4:23:7A,WhizNets WhizNets Inc.
 C4:23:A2,PTEmsoni PT. Emsonic Indonesia
 C4:24:2E,Galvanic Galvanic Applied Sciences Inc
 C4:24:56,PaloAlto Palo Alto Networks
 C4:26:28,AiroWire Airo Wireless
 C4:27:28,zte zte corporation
 C4:27:8C,"HuaweiDe Huawei Device Co., Ltd."
-C4:27:95,Technico Technicolor CH USA Inc.
+C4:27:95,VantivaU Vantiva USA LLC
 C4:28:2D,Embedded Embedded Intellect Pty Ltd
 C4:29:1D,KlemsanE Klemsan Elektrik Elektronik San.Ve Tic.As.
 C4:29:96,Signify Signify B.V.
 C4:2A:D0,"Apple Apple, Inc."
 C4:2B:44,"HuaweiDe Huawei Device Co., Ltd."
 C4:2C:03,"Apple Apple, Inc."
 C4:2C:4F,"QingdaoH Qingdao Hisense Mobile Communication Technology Co,Ltd"
@@ -41526,14 +42904,15 @@
 C4:4D:84,"Cisco Cisco Systems, Inc"
 C4:4E:1F,BlueN
 C4:4E:AC,"Shenzhen Shenzhen Shiningworth Technology Co., Ltd."
 C4:4F:33,Espressi Espressif Inc.
 C4:4F:96,AlpsAlpi Alps Alpine
 C4:50:06,"SamsungE Samsung Electronics Co.,Ltd"
 C4:51:8D,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
+C4:52:4F,"Apple Apple, Inc."
 C4:53:79,Micronvi Micronview Limited Liability Company
 C4:54:44,QuantaCo Quanta Computer Inc.
 C4:55:A6,CadacHol Cadac Holdings Ltd
 C4:55:C2,Bach-Sim Bach-Simpson
 C4:56:00,GalleonE Galleon Embedded Computing
 C4:56:FE,LavaInte Lava International Ltd.
 C4:57:1F,JuneLife June Life Inc
@@ -41543,27 +42922,29 @@
 C4:5A:86,"HuaweiDe Huawei Device Co., Ltd."
 C4:5A:B1,Dell Dell Inc.
 C4:5B:BE,Espressi Espressif Inc.
 C4:5B:F7,ants
 C4:5D:83,"SamsungE Samsung Electronics Co.,Ltd"
 C4:5D:D8,HDMIForu HDMI Forum
 C4:5E:5C,"HuaweiTe Huawei Technologies Co.,Ltd"
+C4:60:26,SkyUk Sky Uk Limited
 C4:60:44,EverexEl Everex Electronics Limited
 C4:61:8B,"Apple Apple, Inc."
 C4:61:C7,Microsof Microsoft Corporation
 C4:62:6B,ZPTVigan ZPT Vigantice
 C4:62:EA,"SamsungE Samsung Electronics Co.,Ltd"
 C4:63:54,"U-Raku U-Raku, Inc."
 C4:63:FB,Neatfram Neatframe AS
 C4:64:13,"Cisco Cisco Systems, Inc"
 C4:64:B7,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 C4:64:E3,TexasIns Texas Instruments
 C4:64:F2,Infinixm Infinix mobility limited
 C4:65:16,HewlettP Hewlett Packard
 C4:66:99,"vivoMobi vivo Mobile Communication Co., Ltd."
+C4:67:8B,Alphabet Alphabet Capital Sdn Bhd
 C4:67:B5,Libraton Libratone A/S
 C4:67:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:68:D0,VTechTel VTech Telecommunications Ltd.
 C4:69:3E,Turbulen Turbulence Design Inc.
 C4:69:F0,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:6A:B7,XiaomiCo Xiaomi Communications Co Ltd
 C4:6B:B4,myIDkey
@@ -41583,14 +42964,15 @@
 C4:74:F8,"HotPeppe Hot Pepper, Inc."
 C4:75:AB,IntelCor Intel Corporate
 C4:75:EA,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:77:AB,"BeijingA Beijing ASU Tech Co.,Ltd"
 C4:77:AF,Advanced Advanced Digital Broadcast SA
 C4:78:A2,"HuaweiDe Huawei Device Co., Ltd."
 C4:79:05,"Zhejiang Zhejiang Uniview Technologies Co.,Ltd."
+C4:79:9F,"Haiguang Haiguang Smart Device Co.,Ltd."
 C4:7B:2F,BeijingJ Beijing JoinHope Image Technology Ltd.
 C4:7B:80,"Protempi Protempis, LLC"
 C4:7B:A3,NAVIS NAVIS Inc.
 C4:7C:8D,IEEERegi IEEE Registration Authority
 C4:7C:8D:00:00:00/28,Ati
 C4:7C:8D:10:00:00/28,LynxInno Lynx Innovation Litimed
 C4:7C:8D:20:00:00/28,"Star2Sta Star2Star Communications, LLC"
@@ -41607,19 +42989,21 @@
 C4:7C:8D:D0:00:00/28,"AnhuiGua Anhui GuangXing Linked-Video Communication Technology Co, Ltd."
 C4:7C:8D:E0:00:00/28,LaborStr Labor Strauss Sicherungsanlagenbau GmbH
 C4:7D:46,Fujitsu Fujitsu Limited
 C4:7D:4F,"Cisco Cisco Systems, Inc"
 C4:7D:9F,"SamsungE Samsung Electronics Co.,Ltd"
 C4:7D:CC,ZebraTec Zebra Technologies Inc
 C4:7D:FE,ANSoluti A.N. Solutions GmbH
+C4:7E:E0,"Cisco Cisco Systems, Inc"
 C4:7F:51,Inventek Inventek Systems
 C4:80:25,"HuaweiDe Huawei Device Co., Ltd."
 C4:80:8A,CloudDia Cloud Diagnostics Canada ULC
 C4:82:3F,"FujianNe Fujian Newland Auto-ID Tech. Co,.Ltd."
 C4:82:4E,"Changzho Changzhou Uchip Electronics Co., LTD."
+C4:82:E1,TuyaSmar Tuya Smart Inc.
 C4:83:6F,Ciena Ciena Corporation
 C4:83:72,IEEERegi IEEE Registration Authority
 C4:83:72:00:00:00/28,Compumed Compumedics Germany GmbH
 C4:83:72:10:00:00/28,"Shenzhen Shenzhen King Will Technology Co., LTD"
 C4:83:72:20:00:00/28,Ai-Rider Ai-Rider Corporation
 C4:83:72:30:00:00/28,NextSili NextSilicon
 C4:83:72:40:00:00/28,Transact Transact Technologies Inc
@@ -41687,14 +43071,15 @@
 C4:98:94:90:00:00/28,"Shenzhen Shenzhen Hexin Automation Technology Co.,Ltd."
 C4:98:94:A0:00:00/28,NeronInf Neron Informatics Pvt Ltd
 C4:98:94:B0:00:00/28,"Shanghai Shanghai YVR Technology Co., Ltd."
 C4:98:94:C0:00:00/28,"Zhejiang Zhejiang Rexense loT Technology Co., Ltd"
 C4:98:94:D0:00:00/28,"JiangsuA Jiangsu AIDriving Co.,Ltd."
 C4:98:94:E0:00:00/28,HansSass Hans Sasserath GmbH & Co. KG
 C4:9A:02,LGElectr LG Electronics (Mobile Communications)
+C4:9D:08,"HuaweiDe Huawei Device Co., Ltd."
 C4:9D:ED,Microsof Microsoft Corporation
 C4:9E:41,G24Power G24 Power Limited
 C4:9F:4C,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:9F:F3,"MciaoTec Mciao Technologies, Inc."
 C4:A0:52,"Motorola Motorola Mobility LLC, a Lenovo Company"
 C4:A1:0E,IEEERegi IEEE Registration Authority
 C4:A1:0E:00:00:00/28,HYOSUNGH HYOSUNG Heavy Industries Corporation
@@ -41709,28 +43094,36 @@
 C4:A1:0E:90:00:00/28,"XiAnYepT Xi'An Yep Telecom Technology Co.,Ltd"
 C4:A1:0E:A0:00:00/28,"JiangsuP Jiangsu Perceive World Technology Co.,Ltd."
 C4:A1:0E:B0:00:00/28,ClintonE Clinton Electronics Corporation
 C4:A1:0E:C0:00:00/28,Focus-on
 C4:A1:0E:D0:00:00/28,Connectl Connectlab SRL
 C4:A1:0E:E0:00:00/28,"Alio Alio, Inc"
 C4:A1:51,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
+C4:A1:AE,"HuaweiDe Huawei Device Co., Ltd."
 C4:A3:66,zte zte corporation
 C4:A4:02,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:A5:59,IEEERegi IEEE Registration Authority
+C4:A5:59:00:00:00/28,"Archermi Archermind Japan Co.,Ltd."
 C4:A5:59:10:00:00/28,"MotiveTe Motive Technologies, Inc."
+C4:A5:59:20:00:00/28,"Shenzhen Shenzhen Orfa Tech Co., Ltd"
+C4:A5:59:30:00:00/28,"X-speedl X-speed lnformation Technology Co.,Ltd"
+C4:A5:59:40:00:00/28,Private
 C4:A5:59:50:00:00/28,Moultrie Moultrie Mobile
 C4:A5:59:60:00:00/28,Annapurn Annapurna labs
 C4:A5:59:70:00:00/28,AvironIn Aviron Interactive Inc.
 C4:A5:59:80:00:00/28,Metics
 C4:A5:59:90:00:00/28,"Shenzhen Shenzhen Meishifu Technology Co.,Ltd."
 C4:A5:59:A0:00:00/28,"HebeiFar Hebei Far-East Communication System Engineerning Co.,Ltd."
 C4:A5:59:B0:00:00/28,SMHTechn SMH Technologies SRL
 C4:A5:59:C0:00:00/28,AltamSl Altam Systems Sl
 C4:A5:59:D0:00:00/28,MinoltaS Minolta Security
+C4:A5:59:E0:00:00/28,SernetSu Sernet (Suzhou) Technologies Corporation
+C4:A6:4E,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 C4:A7:2B,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
+C4:A8:16,eero eero inc.
 C4:A8:1D,D-LinkIn D-Link International
 C4:AA:A1,"SUMMITDE SUMMIT DEVELOPMENT, spol.s r.o."
 C4:AA:C4,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 C4:AB:B2,"vivoMobi vivo Mobile Communication Co., Ltd."
 C4:AC:59,"MurataMa Murata Manufacturing Co., Ltd."
 C4:AC:AA,"Apple Apple, Inc."
 C4:AD:21,MEDIAEDG MEDIAEDGE Corporation
@@ -41774,14 +43167,15 @@
 C4:D0:E3,IntelCor Intel Corporate
 C4:D1:97,VentiaUt Ventia Utility Services
 C4:D3:6A,TexasIns Texas Instruments
 C4:D4:38,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:D4:89,"JiangSuJ JiangSu Joyque Information Industry Co.,Ltd"
 C4:D4:96,"Shenzhen Shenzhen Excelsecu Data Technology Co.,Ltd"
 C4:D6:55,"Tercelte Tercel technology co.,ltd"
+C4:D6:66,CiscoMer Cisco Meraki
 C4:D7:38,"HuaweiDe Huawei Device Co., Ltd."
 C4:D7:FD,"Bouffalo Bouffalo Lab (Nanjing) Co., Ltd."
 C4:D8:F3,iZotope
 C4:D9:87,IntelCor Intel Corporate
 C4:DA:26,Noblex Noblex Sa
 C4:DA:7D,IviumTec Ivium Technologies B.V.
 C4:DB:04,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -41805,14 +43199,15 @@
 C4:E9:84,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 C4:EA:1D,Technico Technicolor Delivery Technologies Belgium NV
 C4:EB:39,Sagemcom Sagemcom Broadband SAS
 C4:EB:41,Sagemcom Sagemcom Broadband SAS
 C4:EB:42,Sagemcom Sagemcom Broadband SAS
 C4:EB:43,Sagemcom Sagemcom Broadband SAS
 C4:EB:E3,RrcnSas Rrcn Sas
+C4:EB:FF,zte zte corporation
 C4:ED:BA,TexasIns Texas Instruments
 C4:EE:AE,VSSMonit VSS Monitoring
 C4:EE:F5,II-VI II-VI Incorporated
 C4:EF:70,HomeSkin Home Skinovations
 C4:EF:DA,Honeywel Honeywell
 C4:F0:81,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:F0:EC,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
@@ -41823,14 +43218,15 @@
 C4:F4:64,Spicaint Spica international
 C4:F5:7C,BrocadeC Brocade Communications Systems LLC
 C4:F5:A5,"Kumalift Kumalift Co., Ltd."
 C4:F7:D5,"Cisco Cisco Systems, Inc"
 C4:F8:39,ActiaAut Actia Automotive
 C4:FB:AA,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:FB:C8,"Shenzhen Shenzhen Candour Co., Ltd."
+C4:FC:22,"YealinkX Yealink(Xiamen) Network Technology Co.,Ltd."
 C4:FC:E4,DishTVNZ DishTV NZ Ltd
 C4:FC:EF,"SambaNov SambaNova Systems, Inc."
 C4:FD:E6,Drtech
 C4:FE:5B,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 C4:FE:E2,AMICCOME AMICCOM Electronics Corporation
 C4:FF:1F,"HuaweiTe Huawei Technologies Co.,Ltd"
 C4:FF:22,"HuaweiDe Huawei Device Co., Ltd."
@@ -41867,18 +43263,20 @@
 C8:0C:C8,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:0D:32,Holoplot Holoplot GmbH
 C8:0E:14,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 C8:0E:77,LeShiZhi Le Shi Zhi Xin Electronic Technology (Tianjin) Limited
 C8:0E:95,OmniLync OmniLync Inc.
 C8:10:73,"CenturyO Century Opticomm Co.,Ltd"
 C8:12:0B,"SamsungE Samsung Electronics Co.,Ltd"
+C8:13:37,JuniperN Juniper Networks
 C8:13:8B,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 C8:14:51,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:14:79,"SamsungE Samsung Electronics Co.,Ltd"
 C8:14:B4,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
+C8:15:4E,IntelCor Intel Corporate
 C8:16:A5,Masimo Masimo Corporation
 C8:16:BD,"QingdaoH Qingdao Hisense Communications Co.,Ltd."
 C8:16:DA,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 C8:17:39,ItelMobi Itel Mobile Limited
 C8:19:F7,"SamsungE Samsung Electronics Co.,Ltd"
 C8:1A:FE,DLOGIC DLOGIC GmbH
 C8:1B:5C,BCTech
@@ -41898,14 +43296,15 @@
 C8:28:32,"BeijingX Beijing Xiaomi Electronics Co., Ltd."
 C8:28:E5,"Cisco Cisco Systems, Inc"
 C8:29:2A,BarunEle Barun Electronics
 C8:29:C8,PaloAlto Palo Alto Networks
 C8:2A:14,"Apple Apple, Inc."
 C8:2A:DD,"Google Google, Inc."
 C8:2A:F1,TCTmobil TCT mobile ltd
+C8:2B:6B,"shenzhen shenzhen worldelite electronics co., LTD"
 C8:2B:96,Espressi Espressif Inc.
 C8:2C:2B,IEEERegi IEEE Registration Authority
 C8:2C:2B:00:00:00/28,"Fungible Fungible, Inc."
 C8:2C:2B:10:00:00/28,Galgus
 C8:2C:2B:20:00:00/28,ReppHeal Repp Health
 C8:2C:2B:30:00:00/28,RFEngine RF Engineering and Energy Resource
 C8:2C:2B:40:00:00/28,iWaveTec iWave Systems Tech Pvt Ltd
@@ -41923,14 +43322,15 @@
 C8:2E:94,"HalfaEnt Halfa Enterprise Co., Ltd."
 C8:31:68,eZEX eZEX corporation
 C8:32:32,HuntingI Hunting Innova
 C8:33:4B,"Apple Apple, Inc."
 C8:33:E5,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:34:8E,IntelCor Intel Corporate
 C8:35:B8,"Ericsson Ericsson, EAB/RWI/K"
+C8:36:A3,GertecBr Gertec Brasil Ltda
 C8:38:70,"SamsungE Samsung Electronics Co.,Ltd"
 C8:39:AC,"HuaweiDe Huawei Device Co., Ltd."
 C8:3A:1B,ToshibaT Toshiba TEC Corporation Inc
 C8:3A:35,"TendaTec Tenda Technology Co., Ltd."
 C8:3A:6B,"Roku Roku, Inc"
 C8:3B:45,Jri
 C8:3C:85,"Apple Apple, Inc."
@@ -41951,22 +43351,24 @@
 C8:45:8F,Wyler Wyler AG
 C8:47:82,AresonTe Areson Technology Corp.
 C8:47:8C,Beken Beken Corporation
 C8:48:F5,"MEDISONX MEDISON Xray Co., Ltd"
 C8:4A:A0,SonyInte Sony Interactive Entertainment Inc.
 C8:4B:D6,Dell Dell Inc.
 C8:4C:75,"Cisco Cisco Systems, Inc"
+C8:4C:78,zte zte corporation
 C8:4D:34,LIONSTai LIONS Taiwan Technology Inc.
 C8:4D:44,"Shenzhen Shenzhen Jiapeng Huaxiang Technology Co.,Ltd"
 C8:4F:0E,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 C8:4F:86,Sophos Sophos Ltd
 C8:50:CE,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:50:E9,"Raisecom Raisecom Technology CO., LTD"
 C8:51:42,"SamsungE Samsung Electronics Co.,Ltd"
 C8:51:95,"HuaweiTe Huawei Technologies Co.,Ltd"
+C8:51:FB,"ExtremeN Extreme Networks, Inc."
 C8:52:61,"ARRISGro ARRIS Group, Inc."
 C8:53:E1,"BeijingB Beijing Bytedance Network Technology Co., Ltd"
 C8:54:4B,ZyxelCom Zyxel Communications Corporation
 C8:54:A4,Infinixm Infinix mobility limited
 C8:56:45,Intermas Intermas France
 C8:56:63,SunflexE Sunflex Europe GmbH
 C8:58:95,"Motorola Motorola Mobility LLC, a Lenovo Company"
@@ -41999,28 +43401,46 @@
 C8:63:FC,"ARRISGro ARRIS Group, Inc."
 C8:64:C7,zte zte corporation
 C8:66:2C,"BeijingH Beijing Haitai Fangyuan High Technology Co,.Ltd."
 C8:66:5D,"ExtremeN Extreme Networks, Inc."
 C8:67:5E,"ExtremeN Extreme Networks, Inc."
 C8:68:DE,"HuaweiDe Huawei Device Co., Ltd."
 C8:69:CD,"Apple Apple, Inc."
+C8:6B:BC,IEEERegi IEEE Registration Authority
+C8:6B:BC:00:00:00/28,SafelyYo SafelyYou
+C8:6B:BC:10:00:00/28,"WeLinkSo WeLink Solutions, Inc."
+C8:6B:BC:20:00:00/28,Vipaks+ Vipaks + Ltd
+C8:6B:BC:30:00:00/28,AnteviaN Antevia Networks
+C8:6B:BC:40:00:00/28,"LiuzhouZ Liuzhou Zuo You Trade Co., Ltd."
+C8:6B:BC:50:00:00/28,"Shenzhen Shenzhen Hebang Electronic Co., Ltd"
+C8:6B:BC:60:00:00/28,DrowsyDi Drowsy Digital Inc
+C8:6B:BC:70:00:00/28,"Shenzhen Shenzhen smart-core technology co.,ltd."
+C8:6B:BC:80:00:00/28,"Sinsegye Sinsegye Beijing Technology Co., Ltd"
+C8:6B:BC:90:00:00/28,OseeTech Osee Technology LTD.
+C8:6B:BC:A0:00:00/28,AlphaBri Alpha Bridge Technologies Private Limited
+C8:6B:BC:B0:00:00/28,"HAIROBOT HAI ROBOTICS Co.,Ltd."
+C8:6B:BC:C0:00:00/28,Zeus
+C8:6B:BC:D0:00:00/28,"Scantech Scantech(Hangzhou)Co.,Ltd"
+C8:6B:BC:E0:00:00/28,Waterkot Waterkotte GmbH
 C8:6C:1E,Display Display Systems Ltd
 C8:6C:20,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 C8:6C:3D,AmazonTe Amazon Technologies Inc.
 C8:6C:87,ZyxelCom Zyxel Communications Corporation
 C8:6C:B6,"Optcom Optcom Co., Ltd."
 C8:6F:1D,"Apple Apple, Inc."
+C8:70:23,AlticeLa Altice Labs S.A.
 C8:70:D4,"IBOTechn IBO Technology Co,Ltd"
 C8:71:25,JohnsonO Johnson Outdoors Marine Electronics d/b/a Minnkota
 C8:72:48,Aplicom Aplicom Oy
 C8:72:7E,Nokia
 C8:73:24,SowCheng Sow Cheng Technology Co. Ltd.
 C8:75:5B,Quantify Quantify Technology Pty. Ltd.
 C8:77:65,Tiesse Tiesse SpA
 C8:77:8B,"Mercury– Mercury Systems – Trusted Mission Solutions, Inc."
+C8:78:7D,D-Link D-Link Corporation
 C8:7B:23,Bose Bose Corporation
 C8:7B:5B,zte zte corporation
 C8:7C:BC,"Valink Valink Co., Ltd."
 C8:7D:77,"Shenzhen Shenzhen Kingtech Communication Equipment Co.,Ltd"
 C8:7E:75,"SamsungE Samsung Electronics Co.,Ltd"
 C8:7E:A1,TCLMOKAI TCL MOKA International Limited
 C8:7F:54,ASUSTekC ASUSTek COMPUTER INC.
@@ -42032,14 +43452,15 @@
 C8:84:CF,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:85:50,"Apple Apple, Inc."
 C8:86:29,"Shenzhen Shenzhen Duubee Intelligent Technologies Co.,LTD."
 C8:87:22,Lumenpul Lumenpulse
 C8:87:3B,NetOptic Net Optics
 C8:89:F3,"Apple Apple, Inc."
 C8:8A:83,"Dongguan Dongguan HuaHong Electronics Co.,Ltd"
+C8:8A:9A,IntelCor Intel Corporate
 C8:8B:47,Nolangro Nolangroup S.P.A con Socio Unico
 C8:8B:E8,Masimo Masimo Corporation
 C8:8D:83,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:8E:D1,IEEERegi IEEE Registration Authority
 C8:8E:D1:00:00:00/28,Aisworld Aisworld Private Limited
 C8:8E:D1:10:00:00/28,GermanPi German Pipe GmbH
 C8:8E:D1:20:00:00/28,Rotronic Rotronic Ag
@@ -42064,14 +43485,15 @@
 C8:93:83,"Embedded Embedded Automation, Inc."
 C8:94:02,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 C8:94:BB,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:94:D2,"JiangsuD Jiangsu Datang Electronic Products Co., Ltd"
 C8:96:5A,SkyUk Sky Uk Limited
 C8:96:65,Microsof Microsoft Corporation
 C8:97:9F,Nokia Nokia Corporation
+C8:98:28,zte zte corporation
 C8:99:B2,Arcadyan Arcadyan Corporation
 C8:9B:AD,"HonorDev Honor Device Co., Ltd."
 C8:9B:D7,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 C8:9C:13,Inspirem Inspiremobile
 C8:9C:1D,"Cisco Cisco Systems, Inc"
 C8:9C:DC,"Elitegro Elitegroup Computer Systems Co.,Ltd."
 C8:9D:18,"HuaweiDe Huawei Device Co., Ltd."
@@ -42080,16 +43502,19 @@
 C8:9F:1A,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:9F:1D,"Shenzhen Shenzhen Communication Technologies Co.,Ltd"
 C8:9F:42,VDIIInno VDII Innovation AB
 C8:A0:30,TexasIns Texas Instruments
 C8:A1:B6,"Shenzhen Shenzhen Longway Technologies Co., Ltd"
 C8:A1:BA,Neul Neul Ltd
 C8:A2:CE,OasisMed Oasis Media Systems LLC
+C8:A3:62,ASIXElec ASIX Electronics Corporation
 C8:A4:0D,CoolerMa Cooler Master Technology Inc
+C8:A6:08,RuckusWi Ruckus Wireless
 C8:A6:20,"Nebula Nebula, Inc"
+C8:A6:EF,"SamsungE Samsung Electronics Co.,Ltd"
 C8:A7:0A,VerizonB Verizon Business
 C8:A7:29,"SYStroni SYStronics Co., Ltd."
 C8:A7:76,"HuaweiTe Huawei Technologies Co.,Ltd"
 C8:A8:23,"SamsungE Samsung Electronics Co.,Ltd"
 C8:A9:FC,GoyooNet Goyoo Networks Inc.
 C8:AA:21,"ARRISGro ARRIS Group, Inc."
 C8:AA:55,"HunanCom Hunan Comtom Electronic Incorporated Co.,Ltd"
@@ -42102,14 +43527,15 @@
 C8:B2:1E,ChipseaT Chipsea Technologies (Shenzhen) Corp.
 C8:B2:9B,IntelCor Intel Corporate
 C8:B3:73,"Cisco-Li Cisco-Linksys, LLC"
 C8:B4:22,AskeyCom Askey Computer Corp
 C8:B5:AD,HewlettP Hewlett Packard Enterprise
 C8:B5:B7,"Apple Apple, Inc."
 C8:B6:D3,"HuaweiTe Huawei Technologies Co.,Ltd"
+C8:B6:FE,"Fitbit Fitbit, Inc."
 C8:B8:2F,eero eero inc.
 C8:BA:94,SamsungE Samsung Electro-Mechanics(Thailand)
 C8:BA:E9,Qdis
 C8:BB:81,"HuaweiDe Huawei Device Co., Ltd."
 C8:BB:D3,Embrane
 C8:BC:9C,"HuaweiDe Huawei Device Co., Ltd."
 C8:BC:C8,"Apple Apple, Inc."
@@ -42178,31 +43604,32 @@
 C8:ED:FC,"Shenzhen Shenzhen Ideaform Industrial Product Design Co., Ltd"
 C8:EE:08,"TangtopT Tangtop Technology Co.,Ltd"
 C8:EE:75,PishionI Pishion International Co. Ltd
 C8:EE:A6,"Shenzhen Shenzhen SHX Technology Co., Ltd"
 C8:EF:2E,"BeijingG Beijing Gefei Tech. Co., Ltd"
 C8:EF:BC,"InspurCo Inspur Communication Technology Co.,Ltd."
 C8:F0:9E,Espressi Espressif Inc.
+C8:F2:25,EMMicroe EM Microelectronic
 C8:F2:30,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 C8:F2:B4,"GuizhouH Guizhou Huaxin Information Technology Co., Ltd."
 C8:F3:19,LGElectr LG Electronics (Mobile Communications)
 C8:F3:6B,"YamatoSc Yamato Scale Co.,Ltd."
 C8:F3:86,"Shenzhen Shenzhen Xiaoniao Technology Co.,Ltd"
 C8:F4:06,Avaya Avaya Inc
 C8:F5:D6,IEEERegi IEEE Registration Authority
 C8:F5:D6:00:00:00/28,MeiryoTe Meiryo Technica Corporation
 C8:F5:D6:10:00:00/28,"ValeoInt Valeo Interior Controls (Shenzhen) Co.,Ltd"
 C8:F5:D6:20:00:00/28,"QbicTech Qbic Technology Co., Ltd"
-C8:F5:D6:30:00:00/28,BBPOSInt BBPOS International Limited
+C8:F5:D6:30:00:00/28,BBPOS BBPOS Limited
 C8:F5:D6:40:00:00/28,Evotor Evotor Llc
 C8:F5:D6:50:00:00/28,Pinmicro Pinmicro K K
 C8:F5:D6:60:00:00/28,Jabil
 C8:F5:D6:70:00:00/28,OscarsPr Oscars Pro
 C8:F5:D6:80:00:00/28,"YarwardE Yarward Electronics Co., Ltd."
-C8:F5:D6:90:00:00/28,"Shanghai Shanghai Mo xiang Network Technology CO.,Ltd"
+C8:F5:D6:90:00:00/28,"Shanghai Shanghai Mo xiang Network Technology CO.,ltd"
 C8:F5:D6:A0:00:00/28,"HENANFOX HENAN FOXSTAR DIGITAL DISPLAY Co.,Ltd."
 C8:F5:D6:B0:00:00/28,UnitedBa United Barcode Systems
 C8:F5:D6:C0:00:00/28,Eltako Eltako GmbH
 C8:F5:D6:D0:00:00/28,Volansys Volansys technologies pvt ltd
 C8:F5:D6:E0:00:00/28,Heitec Heitec Ag
 C8:F6:50,"Apple Apple, Inc."
 C8:F6:8D,SETechno S.E.Technologies Limited
@@ -42226,47 +43653,51 @@
 C8:FF:77,Dyson Dyson Limited
 CA:04:5A,Ossia Ossia Inc
 CA:12:5C,Microsof Microsoft Corporation
 CA:1E:45,ASMediaT ASMedia Technology Inc.
 CA:2B:5E,"SuzhouMo Suzhou Motor-comm Electronic Technology Co.,Ltd"
 CA:30:BF,IEEE8021 IEEE 802.1 Chair
 CA:37:82,"Storbyte Storbyte, Inc."
+CA:3E:A6,"Syng Syng, Inc."
 CA:44:6C,"CypressC Cypress Computer Systems, Inc."
 CA:7D:DD,"EmOneTha EmOne (Thailand) Co.,Ltd."
 CA:8F:A5,"Advanced Advanced TS Migrations, Co"
+CA:C2:76,SaabSeae Saab Seaeye Ltd
 CA:C8:7E,AllenOrg Allen Organ Company
 CA:E5:05,Mobiliti Mobilitie
 CA:F2:5B,"LexarEle Lexar Electronics(Shenzhen) Co.,Ltd."
 CC:00:80,Bettini Bettini Srl
 CC:00:F1,Sagemcom Sagemcom Broadband SAS
 CC:03:7B,TexasIns Texas Instruments
 CC:03:D9,CiscoMer Cisco Meraki
-CC:03:FA,Technico Technicolor CH USA Inc.
+CC:03:FA,VantivaU Vantiva USA LLC
 CC:04:7C,G-WAYMic G-WAY Microwave
 CC:04:B4,SelectCo Select Comfort
 CC:05:1B,"SamsungE Samsung Electronics Co.,Ltd"
 CC:05:77,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:06:77,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 CC:07:AB,"SamsungE Samsung Electronics Co.,Ltd"
 CC:07:E4,LenovoMo Lenovo Mobile Communication Technology Ltd.
 CC:08:7B,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:08:8D,"Apple Apple, Inc."
 CC:08:E0,"Apple Apple, Inc."
+CC:08:FA,"Apple Apple, Inc."
 CC:08:FB,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 CC:09:C8,Imaqliq Imaqliq Ltd
 CC:0C:DA,Miljovak Miljovakt AS
 CC:0D:E7,BMeters B Meters S.R.L.
 CC:0D:EC,CiscoSPV Cisco SPVTG
 CC:0D:F2,"Motorola Motorola Mobility LLC, a Lenovo Company"
 CC:10:A3,"BeijingN Beijing Nan Bao Technology Co., Ltd."
 CC:14:A6,"YichunMy Yichun MyEnergy Domain, Inc"
 CC:15:31,IntelCor Intel Corporate
 CC:16:7E,"Cisco Cisco Systems, Inc"
 CC:18:7B,"Manzanit Manzanita Systems, Inc."
 CC:19:A8,PTInovaç PT Inovação e Sistemas SA
+CC:1A:A3,AristaNe Arista Networks
 CC:1A:FA,zte zte corporation
 CC:1B:E0,IEEERegi IEEE Registration Authority
 CC:1B:E0:00:00:00/28,"Microtec Microtech System,Inc"
 CC:1B:E0:10:00:00/28,BeijingD Beijing Daotongtianxia Co.Ltd.
 CC:1B:E0:20:00:00/28,"i-Trinet i-Trinetech Co.,Ltd."
 CC:1B:E0:30:00:00/28,"Shenzhen Shenzhen Vanstor Technology Co.,Ltd"
 CC:1B:E0:40:00:00/28,Laserwor Laserworld (Switzerland) AG
@@ -42323,15 +43754,15 @@
 CC:31:2A,"HuizhouT Huizhou Tcl Communication Electron Co.,Ltd"
 CC:32:96,"HuaweiDe Huawei Device Co., Ltd."
 CC:32:E5,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 CC:33:31,TexasIns Texas Instruments
 CC:33:BB,Sagemcom Sagemcom Broadband SAS
 CC:34:29,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 CC:34:D7,Gewiss Gewiss S.P.A.
-CC:35:40,Technico Technicolor CH USA Inc.
+CC:35:40,VantivaU Vantiva USA LLC
 CC:35:5A,SecuGen SecuGen Corporation
 CC:37:AB,Edgecore Edgecore Networks Corporation
 CC:39:8C,Shiningt Shiningtek
 CC:3A:61,"SamsungE Samsung Electro Mechanics Co., Ltd."
 CC:3A:DF,NeptuneT Neptune Technology Group Inc.
 CC:3B:27,TecnoMob Tecno Mobile Limited
 CC:3B:3E,LesterEl Lester Electrical
@@ -42340,32 +43771,37 @@
 CC:3D:82,IntelCor Intel Corporate
 CC:3D:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:3E:5F,HewlettP Hewlett Packard
 CC:3E:79,"ARRISGro ARRIS Group, Inc."
 CC:3F:1D,HMSIndus HMS Industrial Networks SLU
 CC:3F:8A,Komatsu Komatsu Ltd.
 CC:3F:EA,"BAE BAE Systems, Inc"
+CC:40:85,WiZ
 CC:40:D0,Netgear
 CC:41:8E,MSAInnov MSA Innovation
+CC:42:10,XiaomiCo Xiaomi Communications Co Ltd
 CC:43:E3,Trump Trump s.a.
 CC:44:63,"Apple Apple, Inc."
 CC:46:39,"WAAV WAAV, Inc."
 CC:46:4E,"SamsungE Samsung Electronics Co.,Ltd"
 CC:46:D6,"Cisco Cisco Systems, Inc"
 CC:47:03,"Intercon Intercon Systems Co., Ltd."
+CC:47:40,AzureWav AzureWave Technology Inc.
 CC:47:92,ASIXElec ASIX Electronics Corporation
 CC:47:BD,Rhombus Rhombus Systems
 CC:48:3A,Dell Dell Inc.
 CC:4A:E1,fourtec- fourtec -Fourier Technologies
 CC:4B:73,"AMPAKTec AMPAK Technology, Inc."
 CC:4B:FB,Hellberg Hellberg Safety AB
 CC:4D:38,Carnegie Carnegie Technologies
+CC:4D:74,"FujianNe Fujian Newland Payment Technology Co., Ltd."
 CC:4E:24,BrocadeC Brocade Communications Systems LLC
 CC:4E:EC,"HUMAX HUMAX Co., Ltd."
 CC:4F:5C,IEEERegi IEEE Registration Authority
+CC:4F:5C:00:00:00/28,"ChengduR Chengdu Ren Heng Mei Guang Technology Co.,Ltd."
 CC:4F:5C:10:00:00/28,lesswire lesswire GmbH
 CC:4F:5C:20:00:00/28,MatchX MatchX GmbH
 CC:4F:5C:30:00:00/28,"Shanghai Shanghai Zenchant Electornics Co.,LTD"
 CC:4F:5C:40:00:00/28,SparkBio Spark Biomedical
 CC:4F:5C:50:00:00/28,Kymati Kymati GmbH
 CC:4F:5C:60:00:00/28,Watertec Watertech S.p.A.
 CC:4F:5C:70:00:00/28,SmithsUS Smiths US Innovation LLC
@@ -42382,28 +43818,31 @@
 CC:50:E3,Espressi Espressif Inc.
 CC:51:B4,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 CC:52:89,"Shenzhen Shenzhen Optfocus Technology.,Ltd"
 CC:52:AF,"Universa Universal Global Scientific Industrial Co., Ltd."
 CC:53:B5,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:54:59,OnTimeNe OnTime Networks AS
 CC:55:AD,Rim
+CC:57:63,"Panasoni Panasonic Automotive Systems Co.,Ltd"
+CC:58:30,Sagemcom Sagemcom Broadband SAS
 CC:59:3E,SensiumH Sensium Healthcare Limited
 CC:5A:53,"Cisco Cisco Systems, Inc"
 CC:5B:31,"Nintendo Nintendo Co.,Ltd"
 CC:5C:61,"HuaweiDe Huawei Device Co., Ltd."
 CC:5C:75,Weightec Weightech Com. Imp. Exp. Equip. Pesagem Ltda
 CC:5C:DE,"ChinaMob China Mobile Group Device Co.,Ltd."
 CC:5D:4E,ZyxelCom Zyxel Communications Corporation
 CC:5D:57,"Informat Information System Research Institute,Inc."
 CC:5D:78,JTDConsu JTD Consulting
 CC:5E:F8,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 CC:5F:BF,"Topwise3 Topwise 3G Communication Co., Ltd."
 CC:60:BB,EmpowerR Empower RF Systems
 CC:60:C8,Microsof Microsoft Corporation
 CC:61:E5,"Motorola Motorola Mobility LLC, a Lenovo Company"
+CC:62:FE,"UnionMan Union Man Technology Co.,Ltd"
 CC:64:A6,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:65:AD,"ARRISGro ARRIS Group, Inc."
 CC:66:0A,"Apple Apple, Inc."
 CC:66:18,Adtran Adtran Inc
 CC:66:B2,Nokia
 CC:68:B6,TP-Link TP-Link Corporation Limited
 CC:69:B0,"GlobalTr Global Traffic Technologies, LLC"
@@ -42454,15 +43893,15 @@
 CC:8C:E3,TexasIns Texas Instruments
 CC:8D:B5,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 CC:8E:71,"Cisco Cisco Systems, Inc"
 CC:90:70,"Cisco Cisco Systems, Inc"
 CC:90:93,HansongT Hansong Tehnologies
 CC:90:E8,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 CC:91:2B,TEConnec TE Connectivity Touch Solutions
-CC:93:4A,SierraWi Sierra Wireless
+CC:93:4A,"SierraWi Sierra Wireless, ULC"
 CC:94:4A,Pfeiffer Pfeiffer Vacuum GmbH
 CC:94:70,"Kinestra Kinestral Technologies, Inc."
 CC:95:D7,"Vizio Vizio, Inc"
 CC:96:35,"LVS LVS Co.,Ltd."
 CC:96:A0,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:96:E5,Dell Dell Inc.
 CC:98:8B,SONYVisu SONY Visual Products Inc.
@@ -42470,39 +43909,43 @@
 CC:99:16,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 CC:9C:3E,CiscoMer Cisco Meraki
 CC:9D:A2,EltexEnt Eltex Enterprise Ltd.
 CC:9E:00,"Nintendo Nintendo Co., Ltd."
 CC:9E:A2,AmazonTe Amazon Technologies Inc.
 CC:9E:CA,HMDGloba HMD Global Oy
 CC:9F:35,Transbit Transbit Sp. z o.o.
-CC:9F:7A,"ChiunMai Chiun Mai Communication Systems, Inc"
+CC:9F:7A,"ChiunMai Chiun Mai Communication System, Inc"
 CC:A0:E5,DZGMeter DZG Metering GmbH
 CC:A1:2B,"TCLKingE TCL King Electrical Appliances (Huizhou) Co., Ltd"
-CC:A1:74,"Facebook Facebook Technologies, LLC"
+CC:A1:74,"MetaPlat Meta Platforms Technologies, LLC"
 CC:A2:19,"Shenzhen Shenzhen Along Investment Co.,Ltd"
 CC:A2:23,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:A2:60,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 CC:A3:74,Guangdon Guangdong Guanglian Electronic Technology Co.Ltd
 CC:A3:BD,ItelMobi Itel Mobile Limited
 CC:A4:62,"ARRISGro ARRIS Group, Inc."
 CC:A4:AF,"Shenzhen Shenzhen Sowell Technology Co., LTD"
 CC:A6:14,AifaTech Aifa Technology Corp.
 CC:A7:C1,"Google Google, Inc."
 CC:AB:2C,"HUMAX HUMAX Co., Ltd."
+CC:AC:FE,"TelinkSe Telink Semiconductor (Shanghai) Co., Ltd."
 CC:AF:78,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+CC:B0:71,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 CC:B0:A8,"HuaweiDe Huawei Device Co., Ltd."
 CC:B0:DA,LiteonTe Liteon Technology Corporation
 CC:B1:1A,"SamsungE Samsung Electronics Co.,Ltd"
 CC:B1:82,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:B2:55,D-LinkIn D-Link International
 CC:B3:AB,"shenzhen shenzhen Biocare Bio-Medical Equipment Co.,Ltd."
 CC:B3:F8,FujitsuI Fujitsu Isotec Limited
+CC:B5:4C,TexasIns Texas Instruments
 CC:B5:5A,Fraunhof Fraunhofer ITWM
 CC:B5:D1,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 CC:B6:91,NECMagnu NECMagnusCommunications
+CC:B6:C8,"Cisco Cisco Systems, Inc"
 CC:B7:C4,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:B8:88,AnBSecur AnB Securite s.a.
 CC:B8:A8,"AMPAKTec AMPAK Technology, Inc."
 CC:B8:F1,EagleKin Eagle Kingdom Technologies Limited
 CC:BA:6F,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:BB:FE,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:BC:E3,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -42517,14 +43960,15 @@
 CC:C2:61:10:00:00/28,NWL NWL Inc.
 CC:C2:61:20:00:00/28,Tecnoide Tecnoideal Srl
 CC:C2:61:30:00:00/28,"Netradyn Netradyne, Inc."
 CC:C2:61:40:00:00/28,EDAGEngi EDAG Engineering GmbH
 CC:C2:61:50:00:00/28,"ViperDes Viper Design, LLC"
 CC:C2:61:60:00:00/28,Guardiar Guardiar USA
 CC:C2:61:70:00:00/28,"AbilityE Ability Enterprise Co., Ltd"
+CC:C2:61:80:00:00/28,RoomMate RoomMate AS
 CC:C2:61:90:00:00/28,Byterg Byterg Llc
 CC:C2:61:A0:00:00/28,"Shenzhen Shenzhen Uyesee Technology Co.,Ltd"
 CC:C2:61:B0:00:00/28,Winterth Winterthur Gas & Diesel Ltd.
 CC:C2:61:C0:00:00/28,NortekSe Nortek Security & Control
 CC:C2:61:D0:00:00/28,DspreadT Dspread Technology (Beijing) Inc.
 CC:C2:61:E0:00:00/28,ToongInE Toong In Electronic Corp.
 CC:C2:E0,"Raisecom Raisecom Technology CO., LTD"
@@ -42540,25 +43984,26 @@
 CC:CC:4E,SunFount Sun Fountainhead USA. Corp
 CC:CC:77,ZaramTec Zaram Technology. Inc.
 CC:CC:81,"HuaweiTe Huawei Technologies Co.,Ltd"
 CC:CC:CC,SiliconL Silicon Laboratories
 CC:CD:64,SM-Elect SM-Electronic GmbH
 CC:CE:1E,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 CC:CE:40,Janteq Janteq Corp
+CC:CF:83,CigShang Cig Shanghai Co Ltd
 CC:D0:83,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 CC:D2:81,"Apple Apple, Inc."
 CC:D2:9B,"Shenzhen Shenzhen Bopengfa Elec&Technology CO.,Ltd"
 CC:D3:1E,IEEERegi IEEE Registration Authority
 CC:D3:1E:00:00:00/28,SAMIM SAMIM Co
 CC:D3:1E:10:00:00/28,RondoBur Rondo Burgdorf AG
 CC:D3:1E:20:00:00/28,Neptune Neptune Systems
 CC:D3:1E:30:00:00/28,Ken Ken A/S
 CC:D3:1E:40:00:00/28,PJGSyste PJG Systementwicklung GmbH
 CC:D3:1E:50:00:00/28,"NTmore NTmore.Co.,Ltd"
-CC:D3:1E:60:00:00/28,BBPOSInt BBPOS International Limited
+CC:D3:1E:60:00:00/28,BBPOS BBPOS Limited
 CC:D3:1E:70:00:00/28,"Shenzhen Shenzhen Decnta Technology Co.,LTD."
 CC:D3:1E:80:00:00/28,inoage inoage GmbH
 CC:D3:1E:90:00:00/28,"SiemensM Siemens AG, MO MLT BG"
 CC:D3:1E:A0:00:00/28,HaishuTe Haishu Technology LIMITED
 CC:D3:1E:B0:00:00/28,ElkProdu Elk Products
 CC:D3:1E:C0:00:00/28,NantEner NantEnergy
 CC:D3:1E:D0:00:00/28,Cujo Cujo Llc
@@ -42604,29 +44049,32 @@
 CC:E2:36,Hangzhou Hangzhou Yaguan Technology Co. LTD
 CC:E6:86,"SamsungE Samsung Electronics Co.,Ltd"
 CC:E7:98,MySocial My Social Stuff
 CC:E7:DF,"American American Magnetics, Inc."
 CC:E8:AC,"SOYEATec SOYEA Technology Co.,Ltd."
 CC:EA:1C,"DCONWORK DCONWORKS Co., Ltd"
 CC:EB:18,"Tss Ooo ""Tss"""
+CC:EB:5E,XiaomiCo Xiaomi Communications Co Ltd
 CC:ED:21,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 CC:ED:4D,"Cisco Cisco Systems, Inc"
 CC:ED:DC,MitraSta MitraStar Technology Corp.
 CC:EE:D9,VAHLEAut VAHLE Automation GmbH
 CC:EF:03,"HunanKey Hunan Keyshare Communication Technology Co., Ltd."
 CC:EF:48,"Cisco Cisco Systems, Inc"
 CC:F0:FD,"ChinaMob China Mobile (Hangzhou) Information Technology Co., Ltd."
 CC:F3:05,"Shenzhen Shenzhen Tian Xing Chuang Zhan Electronic Co.,Ltd"
 CC:F3:A5,"ChiMeiCo Chi Mei Communication Systems, Inc"
+CC:F3:C8,VantivaU Vantiva USA LLC
 CC:F4:07,EukreaEl Eukrea Electromatique Sarl
 CC:F4:11,"Google Google, Inc."
 CC:F5:38,3isysnet 3isysnetworks
 CC:F5:5F,EFocusIn E Focus Instruments India Private Limited
 CC:F6:7A,AyeckaCo Ayecka Communication Systems LTD
 CC:F7:35,AmazonTe Amazon Technologies Inc.
+CC:F8:26,"SamsungE Samsung Electronics Co.,Ltd"
 CC:F8:41,Lumewave
 CC:F8:F0,"XianHISU Xi'an HISU Multimedia Technology Co.,Ltd."
 CC:F9:54,Avaya Avaya Inc
 CC:F9:57,u-blox u-blox AG
 CC:F9:E4,IntelCor Intel Corporate
 CC:F9:E8,"SamsungE Samsung Electronics Co.,Ltd"
 CC:FA:00,LGElectr LG Electronics (Mobile Communications)
@@ -42660,39 +44108,68 @@
 D0:13:FD,LGElectr LG Electronics (Mobile Communications)
 D0:14:11,IEEERegi IEEE Registration Authority
 D0:14:11:00:00:00/28,EkkoSens EkkoSense Ltd
 D0:14:11:10:00:00/28,Private
 D0:14:11:20:00:00/28,"EvocoLab Evoco Labs CO., LTD"
 D0:14:11:30:00:00/28,iLOQ iLOQ Oy
 D0:14:11:40:00:00/28,powerall
+D0:14:11:50:00:00/28,Superlea Superlead
 D0:14:11:60:00:00/28,Ahnnet
 D0:14:11:70:00:00/28,Realwave Realwave Inc.
 D0:14:11:80:00:00/28,"VideoSec Video Security, Inc."
 D0:14:11:90:00:00/28,Airthing Airthings
 D0:14:11:A0:00:00/28,AbbEvi Abb Evi Spa
 D0:14:11:B0:00:00/28,CYLTek CYLTek Limited
 D0:14:11:C0:00:00/28,"ShenZhen Shen Zhen HaiHe Hi-Tech Co., Ltd"
 D0:14:11:D0:00:00/28,"Guangdon Guangdong Shiqi Manufacture Co., Ltd."
 D0:14:11:E0:00:00/28,Tecnosof Tecnosoft srl
 D0:15:4A,zte zte corporation
 D0:15:A6,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
+D0:15:BB,IEEERegi IEEE Registration Authority
+D0:15:BB:20:00:00/28,"BeijingG Beijing Guangshu Zhiying Technology Development Co., Ltd."
+D0:15:BB:30:00:00/28,TePSEG TePS'EG
+D0:15:BB:50:00:00/28,ListenTe Listen Technologies
+D0:15:BB:60:00:00/28,"ShenZhen ShenZhen Zhongke GuanJie Data Technology Co.,Ltd."
+D0:15:BB:70:00:00/28,NewTechI New Tech IoT
+D0:15:BB:80:00:00/28,Alekto Alekto-Systems Ltd
+D0:15:BB:90:00:00/28,StellarB Stellar Blu Solutions
+D0:15:BB:A0:00:00/28,HongKong Hong Kong Cohonest Technology Limited
+D0:15:BB:C0:00:00/28,Shenzhen Shenzhen Waystar Communication Technology Co. Ltd.
+D0:15:BB:D0:00:00/28,Lampuga Lampuga GmbH
 D0:16:7C,eero eero inc.
 D0:16:B4,"HuaweiTe Huawei Technologies Co.,Ltd"
+D0:16:F0,IEEERegi IEEE Registration Authority
+D0:16:F0:00:00:00/28,"Shenzhen Shenzhen Lesingle Technology CO., LTD."
+D0:16:F0:10:00:00/28,QbicComm Qbic Communications Dmcc
+D0:16:F0:20:00:00/28,RYSE RYSE Inc.
+D0:16:F0:30:00:00/28,Sofinet Sofinet LLC
+D0:16:F0:40:00:00/28,"BeijingX Beijing Xiaoyuan Wenhua Culture Communication Co., Ltd."
+D0:16:F0:50:00:00/28,wuxihigh wuxi high information Security Technolog
+D0:16:F0:60:00:00/28,TornadoM Tornado Modular Systems
+D0:16:F0:70:00:00/28,HydacEle Hydac Electronic
+D0:16:F0:80:00:00/28,"Shenzhen Shenzhen DOOGEE Hengtong Technology CO.,LTD"
+D0:16:F0:90:00:00/28,CrystalA Crystal Alarm AB
+D0:16:F0:A0:00:00/28,Optitera Optitera Global Networks Private Limited
+D0:16:F0:B0:00:00/28,worldcns worldcns inc.
+D0:16:F0:C0:00:00/28,PeralexE Peralex Electronics (Pty) Ltd
+D0:16:F0:D0:00:00/28,TopGuard Top Guard Technologies
+D0:16:F0:E0:00:00/28,BBPOS BBPOS Limited
 D0:17:69,"MurataMa Murata Manufacturing Co., Ltd."
 D0:17:6A,"SamsungE Samsung Electronics Co.,Ltd"
 D0:17:C2,ASUSTekC ASUSTek COMPUTER INC.
 D0:19:6A,Ciena Ciena Corporation
+D0:19:D3,ItelMobi Itel Mobile Limited
 D0:1A:A7,UniPrint
 D0:1B:1F,Ohsung
 D0:1B:49,"SamsungE Samsung Electronics Co.,Ltd"
 D0:1C:3C,TecnoMob Tecno Mobile Limited
 D0:1C:BB,"BeijingC Beijing Ctimes Digital Technology Co., Ltd."
 D0:1E:1D,SaiNXTTe SaiNXT Technologies LLP
 D0:21:AC,Yohana
-D0:21:F9,Ubiquiti Ubiquiti Networks Inc.
+D0:21:F9,Ubiquiti Ubiquiti Inc
 D0:22:12,IEEERegi IEEE Registration Authority
 D0:22:12:00:00:00/28,SpiritIT Spirit IT B.V.
 D0:22:12:10:00:00/28,Aim
 D0:22:12:20:00:00/28,RHENAC RHENAC Systems GmbH
 D0:22:12:40:00:00/28,Viatron Viatron GmbH
 D0:22:12:50:00:00/28,"Shanghai Shanghai Routech Co., Ltd"
 D0:22:12:60:00:00/28,UranoInd Urano Industria De Balancas E Equipamentos Ltda
@@ -42723,27 +44200,29 @@
 D0:37:42,"YulongCo Yulong Computer Telecommunication Scientific (Shenzhen) Co.,Ltd"
 D0:37:45,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 D0:37:61,TexasIns Texas Instruments
 D0:39:57,LiteonTe Liteon Technology Corporation
 D0:39:72,TexasIns Texas Instruments
 D0:39:B3,"ARRISGro ARRIS Group, Inc."
 D0:39:EA,NetApp
+D0:39:FA,"SamsungE Samsung Electronics Co.,Ltd"
 D0:3C:1F,IntelCor Intel Corporate
 D0:3D:52,AvaSecur Ava Security Limited
 D0:3D:C3,AQ AQ Corporation
 D0:3E:5C,"HuaweiTe Huawei Technologies Co.,Ltd"
 D0:3E:7D,ChipseaT Chipsea Technologies (Shenzhen) Corp.
 D0:3F:27,WyzeLabs Wyze Labs Inc
 D0:3F:AA,"Apple Apple, Inc."
 D0:40:BE,NpoRps Npo Rps Llc
 D0:40:EF,"MurataMa Murata Manufacturing Co., Ltd."
 D0:41:C9,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 D0:43:1E,Dell Dell Inc.
 D0:46:DC,Southwes Southwest Research Institute
 D0:47:C1,ElmaElec Elma Electronic AG
+D0:48:4F,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
 D0:48:F3,DATTUS DATTUS Inc
 D0:49:7C,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 D0:49:8B,ZoomServ Zoom Server
 D0:4C:C1,SINTRONE SINTRONES Technology Corp.
 D0:4D:2C,"Roku Roku, Inc."
 D0:4D:C6,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 D0:4E:50,"Mobiwire Mobiwire Mobiles (NingBo) Co., LTD"
@@ -42762,22 +44241,23 @@
 D0:56:BF,Amosense
 D0:57:4C,"Cisco Cisco Systems, Inc"
 D0:57:7B,IntelCor Intel Corporate
 D0:57:85,"Pantech Pantech Co., Ltd."
 D0:57:94,Sagemcom Sagemcom Broadband SAS
 D0:57:A1,WermaSig Werma Signaltechnik GmbH & Co. KG
 D0:58:75,ActiveCo Active Control Technology Inc.
+D0:58:A5,"Apple Apple, Inc."
 D0:58:A8,zte zte corporation
 D0:58:C0,QingdaoH Qingdao Haier Multimedia Limited.
 D0:58:FC,SkyUk Sky Uk Limited
 D0:59:19,zte zte corporation
 D0:59:95,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 D0:59:C3,CeraMicr CeraMicro Technology Corporation
 D0:59:E4,"SamsungE Samsung Electronics Co.,Ltd"
-D0:5A:00,Technico Technicolor CH USA Inc.
+D0:5A:00,VantivaU Vantiva USA LLC
 D0:5A:0F,"I-BtDigi I-Bt Digital Co.,Ltd"
 D0:5A:F1,"Shenzhen Shenzhen Pulier Tech CO.,Ltd"
 D0:5A:FD,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 D0:5B:A8,zte zte corporation
 D0:5C:7A,Sarturad Sartura d.o.o.
 D0:5F:64,IEEERegi IEEE Registration Authority
 D0:5F:64:00:00:00/28,Decathlo Decathlon SA
@@ -42794,14 +44274,16 @@
 D0:5F:64:B0:00:00/28,"NorthAme North American Blue Tiger Company, LLC"
 D0:5F:64:C0:00:00/28,"NanjingH Nanjing Huamai Technology Co.,Ltd"
 D0:5F:64:D0:00:00/28,"Shenzhen Shenzhen Canzone Technology Co.,Ltd."
 D0:5F:64:E0:00:00/28,Montblan Montblanc-Simplo GmbH
 D0:5F:B8,TexasIns Texas Instruments
 D0:5F:CE,HitachiD Hitachi Data Systems
 D0:60:8C,zte zte corporation
+D0:61:58,"HuaweiTe Huawei Technologies Co.,Ltd"
+D0:62:2C,"XianYipu Xi'an Yipu Telecom Technology Co.,Ltd."
 D0:62:A0,"ChinaEss China Essence Technology (Zhumadian) Co., Ltd."
 D0:63:4D,MeikoMas Meiko Maschinenbau GmbH & Co. KG
 D0:63:B4,SolidRun SolidRun Ltd.
 D0:65:44,"Apple Apple, Inc."
 D0:65:CA,"HuaweiTe Huawei Technologies Co.,Ltd"
 D0:66:6D,"Shenzhen Shenzhen Bus-Lan Technology Co., Ltd."
 D0:66:7B,"SamsungE Samsung Electronics Co.,Ltd"
@@ -42836,40 +44318,60 @@
 D0:76:50:C0:00:00/28,Electro- Electro-Motive Diesel
 D0:76:50:D0:00:00/28,tecnotro tecnotron elekronik gmbh
 D0:76:50:E0:00:00/28,Revox Revox Inc.
 D0:76:50:F0:00:00/28,Private
 D0:76:8F,Calix Calix Inc.
 D0:76:E7,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 D0:77:14,"Motorola Motorola Mobility LLC, a Lenovo Company"
+D0:77:CE,Edgecore Edgecore Networks Corporation
 D0:78:80,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 D0:7A:B5,"HuaweiTe Huawei Technologies Co.,Ltd"
+D0:7B:6F,"ZhuhaiYu Zhuhai Yunmai Technology Co.,Ltd"
 D0:7C:2D,"LeieIOTt Leie IOT technology Co., Ltd"
+D0:7C:B2,Sigmasta Sigmastar Technology Ltd.
 D0:7D:33,"HuaweiDe Huawei Device Co., Ltd."
 D0:7D:E5,"ForwardP Forward Pay Systems, Inc."
 D0:7E:01,"HuaweiDe Huawei Device Co., Ltd."
 D0:7E:28,HewlettP Hewlett Packard
 D0:7E:35,IntelCor Intel Corporate
 D0:7F:A0,"SamsungE Samsung Electronics Co.,Ltd"
 D0:7F:C4,OuWeiTec Ou Wei Technology Co.，Ltd. of Shenzhen City
 D0:81:7A,"Apple Apple, Inc."
+D0:81:C5,JuniperN Juniper Networks
 D0:83:D4,XtelWire Xtel Wireless ApS
 D0:84:B0,Sagemcom Sagemcom Broadband SAS
 D0:87:E2,"SamsungE Samsung Electronics Co.,Ltd"
 D0:88:0C,"Apple Apple, Inc."
 D0:89:99,"APCON APCON, Inc."
 D0:8A:55,Skullcan Skullcandy
-D0:8A:91,Technico Technicolor CH USA Inc.
+D0:8A:91,VantivaU Vantiva USA LLC
 D0:8B:7E,PassifSe Passif Semiconductor
 D0:8C:B5,TexasIns Texas Instruments
 D0:8C:FF,Upwis Upwis Ab
 D0:8E:79,Dell Dell Inc.
 D0:92:00,FiRaCons FiRa Consortium
 D0:92:9E,Microsof Microsoft Corporation
 D0:92:FA,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 D0:93:80,DucereTe Ducere Technologies Pvt. Ltd.
+D0:93:95,IEEERegi IEEE Registration Authority
+D0:93:95:00:00:00/28,Zhejiang Zhejiang Ruiyi lntelligent Technology Co. Ltd
+D0:93:95:10:00:00/28,"HefeiSiq Hefei Siqiang Electronic Technology Co.,Ltd"
+D0:93:95:20:00:00/28,At&T
+D0:93:95:30:00:00/28,Nesecure Nesecure Telecom Pvt Ltd
+D0:93:95:40:00:00/28,DaesungC Daesung Celtic Enersys
+D0:93:95:50:00:00/28,"FungHwai FungHwa i-Link Technology CO., LTD"
+D0:93:95:60:00:00/28,Annapurn Annapurna labs
+D0:93:95:70:00:00/28,"iSolutio iSolution Technologies Co.,Ltd."
+D0:93:95:80:00:00/28,Annapurn Annapurna labs
+D0:93:95:90:00:00/28,"NingboSu Ningbo Sunny Opotech Co.,Ltd"
+D0:93:95:A0:00:00/28,Automati Automatic Devices
+D0:93:95:B0:00:00/28,Invendis Invendis Technologies India Pvt Ltd
+D0:93:95:C0:00:00/28,BRICK4U BRICK4U GmbH
+D0:93:95:D0:00:00/28,T-Com T-Com Llc
+D0:93:95:E0:00:00/28,"Shenzhen Shenzhen Hotack Technology Co.,Ltd"
 D0:93:F8,Stonestr Stonestreet One LLC
 D0:94:66,Dell Dell Inc.
 D0:95:C7,"Pantech Pantech Co., Ltd."
 D0:96:86,IEEERegi IEEE Registration Authority
 D0:96:86:00:00:00/28,SernetSu Sernet (Suzhou) Technologies Corporation
 D0:96:86:10:00:00/28,Provcom Provcom Ltd
 D0:96:86:20:00:00/28,"TMLakeTe TMLake Technology Ltd.,"
@@ -42881,29 +44383,29 @@
 D0:96:86:80:00:00/28,Energiek Energiekonzepte Deutschland GmbH
 D0:96:86:90:00:00/28,Camfil
 D0:96:86:A0:00:00/28,HeroHeal Hero Health Inc.
 D0:96:86:B0:00:00/28,"Changsha Changsha keruijie lnformation Technology Co.,Ltd"
 D0:96:86:C0:00:00/28,ECS ECS s.r.l.
 D0:96:86:D0:00:00/28,"CertusNe CertusNet Information Technology Co.,LTD"
 D0:96:86:E0:00:00/28,withnetw withnetworks
-D0:96:FB,DASANNet DASAN Network Solutions
+D0:96:FB,DZS DZS Inc.
 D0:97:FE,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 D0:98:9C,ConMet
 D0:99:D5,Alcatel- Alcatel-Lucent
 D0:9B:05,Emtronix
 D0:9C:30,"FosterEl Foster Electric Company, Limited"
 D0:9C:7A,XiaomiCo Xiaomi Communications Co Ltd
 D0:9C:AE,"vivoMobi vivo Mobile Communication Co., Ltd."
 D0:9D:0A,Linkcom
 D0:9D:AB,TCTmobil TCT mobile ltd
 D0:9F:D9,IEEERegi IEEE Registration Authority
 D0:9F:D9:00:00:00/28,"LemeiInt Lemei Intelligent IOT (Shenzhen) Co., Ltd"
 D0:9F:D9:10:00:00/28,elecgato elecgator bvba
 D0:9F:D9:20:00:00/28,WestarDi Westar Display Technologies
-D0:9F:D9:30:00:00/28,"GSYuasaI GS Yuasa Infrastructure Systems Co.,Ltd."
+D0:9F:D9:30:00:00/28,GSYuasaI GS Yuasa International Ltd.
 D0:9F:D9:40:00:00/28,"PotenSha Poten (Shanghai) Technology Co.,Ltd."
 D0:9F:D9:50:00:00/28,CarbonMo Carbon Mobile GmbH
 D0:9F:D9:60:00:00/28,"ElevocTe Elevoc Technology Co., Ltd."
 D0:9F:D9:70:00:00/28,RaymaxTe Raymax Technology Ltd.
 D0:9F:D9:80:00:00/28,"Queclink Queclink Wireless Solutions Co., Ltd."
 D0:9F:D9:90:00:00/28,ENTTEC ENTTEC Pty Ltd.
 D0:9F:D9:A0:00:00/28,Eurolan Eurolan Ltd
@@ -42913,21 +44415,22 @@
 D0:9F:D9:E0:00:00/28,Minibems Minibems Ltd
 D0:A0:D6,ChengDuT ChengDu TD Tech
 D0:A3:11,Neuberge Neuberger Gebäudeautomation GmbH
 D0:A4:6F,ChinaDra China Dragon Technology Limited
 D0:A4:B1,Sonifex Sonifex Ltd.
 D0:A5:A6,"Cisco Cisco Systems, Inc"
 D0:A6:37,"Apple Apple, Inc."
+D0:A9:D3,EMMicroe EM Microelectronic
 D0:AB:D5,IntelCor Intel Corporate
 D0:AE:EC,AlphaNet Alpha Networks Inc.
 D0:AF:B6,"LinktopT Linktop Technology Co., LTD"
 D0:B0:CD,Moen
 D0:B1:28,"SamsungE Samsung Electronics Co.,Ltd"
 D0:B2:14,PoeWit PoeWit Inc
-D0:B2:C4,Technico Technicolor CH USA Inc.
+D0:B2:C4,VantivaU Vantiva USA LLC
 D0:B3:3F,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 D0:B4:5D,"HuaweiDe Huawei Device Co., Ltd."
 D0:B4:98,RobertBo Robert Bosch LLC Automotive Electronics
 D0:B5:23,Bestcare Bestcare Cloucal Corp.
 D0:B5:3D,SeproRob Sepro Robotique
 D0:B5:C2,TexasIns Texas Instruments
 D0:B6:0A,XingluoT Xingluo Technology Company Limited
@@ -42967,18 +44470,19 @@
 D0:C8:57:90:00:00/28,Shenzhen Shenzhen xiaosha Intelligence Technology Co. Ltd
 D0:C8:57:A0:00:00/28,shenzhen shenzhen cnsun
 D0:C8:57:B0:00:00/28,"Chunghsi Chunghsin International Electronics Co.,Ltd."
 D0:C8:57:C0:00:00/28,DanteSec Dante Security Inc.
 D0:C8:57:D0:00:00/28,"Iflytek Iflytek Co.,Ltd."
 D0:C8:57:E0:00:00/28,E-T-AEle E-T-A Elektrotechnische Apparate GmbH
 D0:CD:E1,Scientec Scientech Electronics
+D0:CE:C9,HanChang Han Chang
 D0:CF:0E,Sagemcom Sagemcom Broadband SAS
 D0:CF:5E,EnergyMi Energy Micro AS
 D0:CF:D8,"HuizhouB Huizhou Boshijie Technology Co.,Ltd"
-D0:D0:03,"SamsungE Samsung Electronics Co.,LTD"
+D0:D0:03,"SamsungE Samsung Electronics Co.,Ltd"
 D0:D0:4B,"HuaweiTe Huawei Technologies Co.,Ltd"
 D0:D0:FD,"Cisco Cisco Systems, Inc"
 D0:D2:12,"K2NET K2NET Co.,Ltd."
 D0:D2:3C,"Apple Apple, Inc."
 D0:D2:86,BeckmanC Beckman Coulter K.K.
 D0:D2:B0,"Apple Apple, Inc."
 D0:D3:E0,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
@@ -43003,14 +44507,15 @@
 D0:D9:4F:C0:00:00/28,Arrowave Arrowave Technologies Limited
 D0:D9:4F:D0:00:00/28,"Duksanme Duksanmecasys Co., Ltd."
 D0:D9:4F:E0:00:00/28,"Appotron Appotronics Co., Ltd"
 D0:DA:D7,"Apple Apple, Inc."
 D0:DB:32,Nokia Nokia Corporation
 D0:DB:B7,Casa Casa Systems
 D0:DD:49,JuniperN Juniper Networks
+D0:DD:7C,zte zte corporation
 D0:DF:9A,LiteonTe Liteon Technology Corporation
 D0:DF:B2,GenieNet Genie Networks Limited
 D0:DF:C7,"SamsungE Samsung Electronics Co.,Ltd"
 D0:E0:42,"Cisco Cisco Systems, Inc"
 D0:E1:40,"Apple Apple, Inc."
 D0:E3:47,Yoga
 D0:E4:0B,Wearable Wearable Inc.
@@ -43028,33 +44533,37 @@
 D0:F2:7F,"SteadySe SteadyServ Technoligies, LLC"
 D0:F3:F5,"HuaweiDe Huawei Device Co., Ltd."
 D0:F4:F7,"HuaweiDe Huawei Device Co., Ltd."
 D0:F5:20,KYOCERA KYOCERA Corporation
 D0:F7:3B,HelmutMa Helmut Mauell GmbH Werk Weida
 D0:F8:65,ItelMobi Itel Mobile Limited
 D0:F8:8C,"Motorola Motorola (Wuhan) Mobility Technologies Communication Co., Ltd."
+D0:F9:28,zte zte corporation
 D0:F9:9B,zte zte corporation
 D0:FA:1D,"Qihoo360 Qihoo 360 Technology Co.,Ltd"
 D0:FC:CC,"SamsungE Samsung Electronics Co.,Ltd"
 D0:FC:D0,"HUMAX HUMAX Co., Ltd."
 D0:FF:50,TexasIns Texas Instruments
 D0:FF:98,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:00:0D,"PhoenixB Phoenix Broadband Technologies, LLC."
 D4:00:57,MCTechno MC Technologies GmbH
 D4:01:29,Broadcom
+D4:01:45,"AtwTechn Atw Technology, Inc."
 D4:01:6D,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 D4:02:4A,Delphian Delphian Systems LLC
 D4:04:CD,"ARRISGro ARRIS Group, Inc."
+D4:04:E6,Broadcom Broadcom Limited
 D4:04:FF,JuniperN Juniper Networks
 D4:05:98,"ARRISGro ARRIS Group, Inc."
 D4:05:DE,eero eero inc.
 D4:08:68,"BeijingL Beijing Lanxum Computer Technology CO.,LTD."
 D4:0A:A9,"ARRISGro ARRIS Group, Inc."
 D4:0B:1A,HTC HTC Corporation
 D4:0B:B9,SolidSem Solid Semecs bv.
+D4:0F:9E,"Apple Apple, Inc."
 D4:0F:B2,AppliedM Applied Micro Electronics AME bv
 D4:10:90,iNFORM iNFORM Systems AG
 D4:10:CF,"Huanshun Huanshun Network Science and Technology Co., Ltd."
 D4:11:A3,"SamsungE Samsung Electronics Co.,Ltd"
 D4:11:D6,"ShotSpot ShotSpotter, Inc."
 D4:12:43,"AMPAKTec AMPAK Technology, Inc."
 D4:12:96,AnobitTe Anobit Technologies Ltd.
@@ -43076,14 +44585,16 @@
 D4:20:00:20:00:00/28,"Shenzhen Shenzhen AI Develop & Manufacture Co.,LTD."
 D4:20:00:30:00:00/28,ArbeRobo Arbe Robotics Ltd.
 D4:20:00:40:00:00/28,"EVOCVINT EVOC VIN Technology Co.,Ltd"
 D4:20:00:50:00:00/28,"Monolith Monolith Electric?Changzhou?Co.,Ltd."
 D4:20:00:60:00:00/28,"HiARInfo HiAR Information Technology Co.,Ltd"
 D4:20:00:70:00:00/28,Annapurn Annapurna labs
 D4:20:00:80:00:00/28,"DalianBa Dalian Baishengyuan Technology Co.,Ltd"
+D4:20:00:90:00:00/28,"Weathex Weathex Co., Ltd."
+D4:20:00:A0:00:00/28,BirdDogA BirdDog Australia
 D4:20:00:B0:00:00/28,"Shenzhen Shenzhen Volt IoT technology co.,ltd."
 D4:20:00:C0:00:00/28,Gentec Gentec Systems Co.
 D4:20:00:D0:00:00/28,Zuum
 D4:20:00:E0:00:00/28,"RPUSICom RPUSI Communication Technology Co.,Ltd."
 D4:20:6D,HTC HTC Corporation
 D4:20:B0,"Mist Mist Systems, Inc."
 D4:21:22,Sercomm Sercomm Corporation.
@@ -43105,43 +44616,49 @@
 D4:25:CC:90:00:00/28,TakumiJa Takumi Japan Ltd
 D4:25:CC:A0:00:00/28,E-MetroT E-MetroTel
 D4:25:CC:B0:00:00/28,Veea
 D4:25:CC:C0:00:00/28,POSNETPo POSNET Polska S.A.
 D4:25:CC:D0:00:00/28,Combined Combined Energy Technologies Pty Ltd
 D4:25:CC:E0:00:00/28,Coperion
 D4:27:51,"Infopia Infopia Co., Ltd"
+D4:27:87,"Shanghai Shanghai High-Flying Electronics Technology Co., Ltd"
 D4:28:B2,"ioBridge ioBridge, Inc."
 D4:28:D5,TCTmobil TCT mobile ltd
 D4:29:EA,Zimory Zimory GmbH
 D4:2C:0F,"ARRISGro ARRIS Group, Inc."
 D4:2C:3D,SkyLight Sky Light Digital Limited
 D4:2C:44,"Cisco Cisco Systems, Inc"
 D4:2C:46,Buffalo Buffalo.Inc
 D4:2D:C5,"i-PRO i-PRO Co., Ltd."
 D4:2F:23,AkenoriP Akenori PTE Ltd
+D4:2F:CA,"Apple Apple, Inc."
+D4:31:27,"RuijieNe Ruijie Networks Co.,LTD"
 D4:31:9D,Sinwatec
 D4:32:60,GoPro
 D4:32:66,Fike Fike Corporation
 D4:35:1D,Technico Technicolor Delivery Technologies Belgium NV
 D4:35:38,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 D4:35:4A,ALAXALAN ALAXALA Networks Corporation
 D4:36:39,TexasIns Texas Instruments
 D4:36:DB,"JiangsuT Jiangsu Toppower Automotive Electronics Co., Ltd"
 D4:37:D7,zte zte corporation
+D4:38:44,"UnionMan Union Man Technology Co.,Ltd"
 D4:38:9C,Sony Sony Corporation
 D4:39:B8,Ciena Ciena Corporation
 D4:3A:2C,"Google Google, Inc."
 D4:3A:2E,Shenzhen Shenzhen Mtc Co Ltd
+D4:3A:2F,Shenzhen Shenzhen Mtc Co Ltd
 D4:3A:65,IGRSEngi IGRS Engineering Lab Ltd.
 D4:3A:E9,"DONGGUAN DONGGUAN ipt INDUSTRIAL CO., LTD"
 D4:3B:04,IntelCor Intel Corporate
 D4:3D:39,DialogSe Dialog Semiconductor
 D4:3D:67,CarmaInd Carma Industries Inc.
 D4:3D:7E,"Micro-St Micro-Star Int'l Co, Ltd"
 D4:3D:F3,ZyxelCom Zyxel Communications Corporation
+D4:3F:32,eero eero inc.
 D4:3F:CB,"ARRISGro ARRIS Group, Inc."
 D4:40:D0,"OCOSMOS OCOSMOS Co., LTD"
 D4:40:F0,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:41:65,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 D4:43:0E,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 D4:43:A8,"Changzho Changzhou Haojie Electric Co., Ltd."
 D4:45:E8,"JiangxiH Jiangxi Hongpai Technology Co., Ltd."
@@ -43160,15 +44677,17 @@
 D4:4F:68,EideticC Eidetic Communications Inc
 D4:4F:80,KemperDi Kemper Digital GmbH
 D4:50:3F,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 D4:50:7A,"CEIVALog CEIVA Logic, Inc"
 D4:52:2A,TangoWiF TangoWiFi.com
 D4:52:51,IBTIngen IBT Ingenieurbureau Broennimann Thun
 D4:52:97,"nSTREAMS nSTREAMS Technologies, Inc."
+D4:52:C7,"BeijingL Beijing L&S Lancom Platform Tech. Co., Ltd."
 D4:52:EE,SkyUk Sky Uk Limited
+D4:53:47,"Merytron Merytronic 2012, S.L."
 D4:53:83,"MurataMa Murata Manufacturing Co., Ltd."
 D4:53:AF,VIGOSyst VIGO System S.A.
 D4:54:8B,IntelCor Intel Corporate
 D4:55:56,FiberMou Fiber Mountain Inc.
 D4:55:BE,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
 D4:57:63,"Apple Apple, Inc."
 D4:58:00,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
@@ -43268,14 +44787,15 @@
 D4:7C:44:E0:00:00/28,Shenzhen Shenzhen Anysec Technology Co. Ltd
 D4:7D:FC,TecnoMob Tecno Mobile Limited
 D4:7E:E4,ChinaMob China Mobile IOT Company Limited
 D4:81:CA,"iDevices iDevices, LLC"
 D4:81:D7,Dell Dell Inc.
 D4:82:3E,"ArgosyTe Argosy Technologies, Ltd."
 D4:83:04,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
+D4:84:09,"Shenzhen Shenzhen Mercury Communication Technologies Co.,Ltd."
 D4:84:57,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 D4:85:64,HewlettP Hewlett Packard
 D4:86:60,Arcadyan Arcadyan Corporation
 D4:87:D8,"SamsungE Samsung Electronics Co.,Ltd"
 D4:88:3F,"Hdpro Hdpro Co., Ltd."
 D4:88:66,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:88:90,"SamsungE Samsung Electronics Co.,Ltd"
@@ -43300,14 +44820,15 @@
 D4:94:5A,"Cosmo Cosmo Co., Ltd"
 D4:94:A1,TexasIns Texas Instruments
 D4:94:E8,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:94:FB,Continen Continental Automotive Systems Inc.
 D4:95:24,"CloverNe Clover Network, Inc."
 D4:96:DF,"SungjinC Sungjin C&T Co.,Ltd"
 D4:97:0B,XiaomiCo Xiaomi Communications Co Ltd
+D4:99:6C,JuniperN Juniper Networks
 D4:9A:20,"Apple Apple, Inc."
 D4:9A:A0,VnptTech Vnpt Technology
 D4:9A:F6,AzureWav AzureWave Technology Inc.
 D4:9B:5C,"Chongqin Chongqing Miedu Technology Co., Ltd."
 D4:9B:74,KineticT Kinetic Technologies
 D4:9C:28,JayBird JayBird LLC
 D4:9C:8E,Universi University of FUKUI
@@ -43338,19 +44859,20 @@
 D4:AE:05,"SamsungE Samsung Electronics Co.,Ltd"
 D4:AE:52,Dell Dell Inc.
 D4:AF:F7,AristaNe Arista Networks
 D4:B1:10,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:B1:69,LeShiZhi Le Shi Zhi Xin Electronic Technology (Tianjin) Limited
 D4:B2:7A,"ARRISGro ARRIS Group, Inc."
 D4:B4:3E,Messcomp Messcomp Datentechnik GmbH
+D4:B6:80,"Shanghai Shanghai Linkyum Microeletronics Co.,Ltd"
 D4:B7:09,zte zte corporation
 D4:B7:61,"SichuanA Sichuan AI-Link Technology Co., Ltd."
 D4:B7:D0,Ciena Ciena Corporation
 D4:B8:FF,HomeCont Home Control Singapore Pte Ltd
-D4:B9:2F,Technico Technicolor CH USA Inc.
+D4:B9:2F,VantivaU Vantiva USA LLC
 D4:BA:BA,IEEERegi IEEE Registration Authority
 D4:BA:BA:00:00:00/28,"Shenzhen Shenzhen Action Technologies Co., Ltd."
 D4:BA:BA:10:00:00/28,Annapurn Annapurna labs
 D4:BA:BA:20:00:00/28,"GuangZho GuangZhou Ostec Electronic Technology Co.,Limited"
 D4:BA:BA:30:00:00/28,Shenzhen Shenzhen Pu Ying Innovation Technology Corporation Limited
 D4:BA:BA:40:00:00/28,"BeijingY Beijing Yuanxin Junsheng Technology Co.,ltd"
 D4:BA:BA:50:00:00/28,ReeR ReeR SpA
@@ -43359,14 +44881,15 @@
 D4:BA:BA:80:00:00/28,"ChengduB Chengdu Ba SAN SI YI Information Technology Co., LTD"
 D4:BA:BA:90:00:00/28,"Shenzhen Shenzhen Chuangyou Acoustic Technology Co., Ltd."
 D4:BA:BA:A0:00:00/28,Actionte Actiontec Electronics Inc.
 D4:BA:BA:B0:00:00/28,"QingdaoV Qingdao Vzense Technology Co., Ltd."
 D4:BA:BA:C0:00:00/28,"RusatomA Rusatom Automated Control Systems, Joint-Stock Company"
 D4:BA:BA:D0:00:00/28,AADONACo AADONA Communication Pvt Ltd
 D4:BA:BA:E0:00:00/28,CamozziA Camozzi Automation SpA
+D4:BA:FA,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 D4:BB:C8,"vivoMobi vivo Mobile Communication Co., Ltd."
 D4:BB:E6,"HuaweiDe Huawei Device Co., Ltd."
 D4:BD:1E,"5VTTechn 5VT Technologies,Taiwan LTd."
 D4:BD:4F,RuckusWi Ruckus Wireless
 D4:BE:D9,Dell Dell Inc.
 D4:BF:2D,SEContro SE Controls Asia Pacific Ltd
 D4:BF:7F,Upvel
@@ -43394,32 +44917,34 @@
 D4:D4:DA,Espressi Espressif Inc.
 D4:D5:0D,"Southwes Southwest Microwave, Inc"
 D4:D5:1B,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:D7:48,"Cisco Cisco Systems, Inc"
 D4:D7:A9,Shanghai Shanghai Kaixiang Info Tech LTD
 D4:D7:CF,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 D4:D8:53,IntelCor Intel Corporate
+D4:D8:92,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:D8:98,"KoreaCNO Korea CNO Tech Co., Ltd"
 D4:D9:19,GoPro
 D4:DA:21,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 D4:DA:CD,SkyUk Sky Uk Limited
 D4:DC:09,"Mist Mist Systems, Inc."
 D4:DC:CD,"Apple Apple, Inc."
 D4:DF:57,Alpinion Alpinion Medical Systems
 D4:E0:53,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 D4:E0:8E,ValueHD ValueHD Corporation
 D4:E2:2F,"Roku Roku, Inc"
-D4:E2:CB,Technico Technicolor CH USA Inc.
+D4:E2:CB,VantivaU Vantiva USA LLC
 D4:E3:2C,SSiedleS S. Siedle & Sohne
 D4:E3:3F,Nokia
 D4:E6:B7,"SamsungE Samsung Electronics Co.,Ltd"
 D4:E8:53,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 D4:E8:80,"Cisco Cisco Systems, Inc"
 D4:E8:B2,"SamsungE Samsung Electronics Co.,Ltd"
 D4:E9:0B,"Cvt Cvt Co.,Ltd"
+D4:E9:5E,TexasIns Texas Instruments
 D4:E9:8A,IntelCor Intel Corporate
 D4:EA:0E,Avaya Avaya Inc
 D4:EB:68,"Cisco Cisco Systems, Inc"
 D4:EC:0C,Harley-D Harley-Davidson Motor Company
 D4:EC:86,"LinkedHo LinkedHope Intelligent Technologies Co., Ltd"
 D4:EC:AB,"vivoMobi vivo Mobile Communication Co., Ltd."
 D4:EE:07,"HIWIFI HIWIFI Co., Ltd."
@@ -43446,22 +44971,25 @@
 D4:F9:8D,Espressi Espressif Inc.
 D4:F9:A1,"HuaweiTe Huawei Technologies Co.,Ltd"
 D4:FB:8E,"Apple Apple, Inc."
 D4:FC:13,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 D8:00:4D,"Apple Apple, Inc."
 D8:00:93,Aurender Aurender Inc.
 D8:02:8A,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
+D8:03:1A,LairdCon Laird Connectivity
 D8:05:2E,Skyviia Skyviia Corporation
 D8:06:D1,"Honeywel Honeywell Fire System (Shanghai) Co,. Ltd."
 D8:07:B6,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 D8:08:31,"SamsungE Samsung Electronics Co.,Ltd"
 D8:08:F5,ArcadiaN Arcadia Networks Co. Ltd.
+D8:09:7F,zte zte corporation
 D8:09:C3,Cercacor Cercacor Labs
 D8:09:D6,"Zexelon Zexelon Co., Ltd."
 D8:0A:60,"HuaweiTe Huawei Technologies Co.,Ltd"
+D8:0A:E6,zte zte corporation
 D8:0B:9A,"SamsungE Samsung Electronics Co.,Ltd"
 D8:0B:CB,"TelinkSe Telink Semiconductor (Shanghai) Co., Ltd."
 D8:0C:CF,CGVS C.G.V. S.A.S.
 D8:0D:17,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 D8:0D:E3,FxiTechn Fxi Technologies As
 D8:0E:29,"vivoMobi vivo Mobile Communication Co., Ltd."
 D8:0F:99,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
@@ -43475,26 +45003,29 @@
 D8:15:0D,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 D8:16:0A,NipponEl Nippon Electro-Sensory Devices
 D8:16:C1,DewavHkE Dewav (Hk) Electronics Limited
 D8:18:2B,ContiTem Conti Temic Microelectronic GmbH
 D8:18:D3,JuniperN Juniper Networks
 D8:19:7A,Nuheara Nuheara Ltd
 D8:19:CE,Telesqua Telesquare
+D8:1B:B5,"HuaweiTe Huawei Technologies Co.,Ltd"
 D8:1B:FE,Twinlinx Twinlinx Corporation
 D8:1C:14,"Compacta Compacta International, Ltd."
 D8:1C:79,"Apple Apple, Inc."
 D8:1D:72,"Apple Apple, Inc."
 D8:1E:DD,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 D8:1E:DE,B&WGroup B&W Group Ltd
 D8:1F:12,TuyaSmar Tuya Smart Inc.
 D8:1F:CC,BrocadeC Brocade Communications Systems LLC
 D8:20:9F,CubroAcr Cubro Acronet GesmbH
+D8:21:DA,SernetSu Sernet (Suzhou) Technologies Corporation
 D8:22:F4,AvnetSil Avnet Silica
 D8:24:77,Universa Universal Electric Corporation
 D8:24:BD,"Cisco Cisco Systems, Inc"
+D8:24:EC,Plenom Plenom A/S
 D8:25:22,"ARRISGro ARRIS Group, Inc."
 D8:25:B0,"Rockeete Rockeetech Systems Co.,Ltd."
 D8:26:B9,"Guangdon Guangdong Coagent Electronics S&T Co.,Ltd."
 D8:27:0C,"MaxTroni MaxTronic International Co., Ltd."
 D8:28:C9,GeneralE General Electric Consumer and Industrial
 D8:29:16,AscentCo Ascent Communication Technology
 D8:29:18,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -43509,56 +45040,62 @@
 D8:31:34,"Roku Roku, Inc"
 D8:31:CF,"SamsungE Samsung Electronics Co.,Ltd"
 D8:32:14,"TendaTec Tenda Technology Co.,Ltd.Dongguan branch"
 D8:32:5A,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 D8:32:E3,XiaomiCo Xiaomi Communications Co Ltd
 D8:33:7F,"OfficeFA Office FA.com Co.,Ltd."
 D8:33:B7,Sagemcom Sagemcom Broadband SAS
+D8:34:1C,"GDMideaA GD Midea Air-Conditioning Equipment Co.,Ltd."
 D8:34:D1,"Shenzhen Shenzhen Orange Digital Technology Co.,Ltd"
 D8:34:EE,Shure Shure Incorporated
 D8:36:5F,Intelbra Intelbras
 D8:37:3B,"Shenzhen Shenzhen Jingxun Software Telecommunication Technology Co.,Ltd"
 D8:37:BE,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 D8:38:0D,"SHENZHEN SHENZHEN IP-COM Network Co.,Ltd"
 D8:38:FC,RuckusWi Ruckus Wireless
+D8:3A:DD,Raspberr Raspberry Pi Trading Ltd
 D8:3A:F5,Wideband Wideband Labs LLC
 D8:3B:BF,IntelCor Intel Corporate
 D8:3C:69,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 D8:3D:CC,"shenzhen shenzhen UDD Technologies,co.,Ltd"
 D8:40:08,"HuaweiTe Huawei Technologies Co.,Ltd"
 D8:42:AC,"Shanghai Shanghai Feixun Communication Co.,Ltd."
 D8:42:E2,"CanaryCo Canary Connect, Inc."
 D8:43:ED,Suzuken
 D8:44:5C,DEVTecno DEV Tecnologia Ind Com Man Eq LTDA
 D8:45:2B,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 D8:46:06,SiliconV Silicon Valley Global Marketing
 D8:47:10,SichuanC Sichuan Changhong Electric Ltd.
 D8:47:32,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
+D8:47:8F,Microchi Microchip Technology Inc.
 D8:47:BB,"HuaweiDe Huawei Device Co., Ltd."
 D8:48:EE,"Hangzhou Hangzhou Xueji Technology Co., Ltd."
 D8:49:0B,"HuaweiTe Huawei Technologies Co.,Ltd"
 D8:49:2F,Canon Canon Inc.
 D8:4A:2B,zte zte corporation
 D8:4A:87,"OiElectr Oi Electric Co.,Ltd"
 D8:4B:2A,"Cognitas Cognitas Technologies, Inc."
 D8:4C:90,"Apple Apple, Inc."
 D8:4D:B9,"WuQiTech Wu Qi Technologies,Inc."
 D8:4F:37,"Proxissp Proxis, spol. s r.o."
 D8:4F:B8,LgElectr Lg Electronics
 D8:50:A1,"HunanDan Hunan Danuo Technology Co.,LTD"
 D8:50:E6,ASUSTekC ASUSTek COMPUTER INC.
 D8:53:9A,JuniperN Juniper Networks
+D8:53:BC,"LenovoIn Lenovo Information Products (Shenzhen)Co.,Ltd"
 D8:54:3A,TexasIns Texas Instruments
 D8:54:82,"Oxit Oxit, LLC"
 D8:54:A2,"ExtremeN Extreme Networks, Inc."
 D8:55:75,"SamsungE Samsung Electronics Co.,Ltd"
 D8:55:A3,zte zte corporation
 D8:57:EF,"SamsungE Samsung Electronics Co.,Ltd"
+D8:58:C6,KatchAss Katch Asset Tracking Pty Limited
 D8:58:D7,"CZNICzsp CZ.NIC, z.s.p.o."
 D8:59:82,"HuaweiTe Huawei Technologies Co.,Ltd"
+D8:5B:22,"Shenzhen Shenzhen Hohunet Technology Co., Ltd"
 D8:5B:2A,"SamsungE Samsung Electronics Co.,Ltd"
 D8:5D:4C,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 D8:5D:84,CAxsoft CAx soft GmbH
 D8:5D:E2,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 D8:5D:EF,Busch-Ja Busch-Jaeger Elektro GmbH
 D8:5D:FB,Private
 D8:5E:D3,"Giga-Byt Giga-Byte Technology Co.,Ltd."
@@ -43566,14 +45103,15 @@
 D8:60:B0,bioMérie bioMérieux Italia S.p.A.
 D8:60:B3,Guangdon Guangdong Global Electronic Technology CO.，LTD
 D8:61:62,WistronN Wistron Neweb Corporation
 D8:61:94,Objetivo Objetivos y Sevicios de Valor Añadido
 D8:62:DB,Eno Eno Inc.
 D8:63:0D,"Motorola Motorola (Wuhan) Mobility Technologies Communication Co., Ltd."
 D8:63:75,XiaomiCo Xiaomi Communications Co Ltd
+D8:63:8C,"Shenzhen Shenzhen Dttek Technology Co., Ltd."
 D8:65:95,ToysMyth Toy's Myth Inc.
 D8:66:C6,"Shenzhen Shenzhen Daystar Technology Co.,ltd"
 D8:66:EE,"BoxinCom Boxin Communication Co.,Ltd."
 D8:67:D3,"HuaweiDe Huawei Device Co., Ltd."
 D8:67:D9,"Cisco Cisco Systems, Inc"
 D8:68:52,"HuaweiTe Huawei Technologies Co.,Ltd"
 D8:68:A0,"SamsungE Samsung Electronics Co.,Ltd"
@@ -43587,18 +45125,20 @@
 D8:6D:17,"HuaweiTe Huawei Technologies Co.,Ltd"
 D8:71:4D,TexasIns Texas Instruments
 D8:71:57,LenovoMo Lenovo Mobile Communication Technology Ltd.
 D8:74:95,zte zte corporation
 D8:75:33,Nokia Nokia Corporation
 D8:76:0A,"Escort Escort, Inc."
 D8:76:AE,"HuaweiTe Huawei Technologies Co.,Ltd"
+D8:77:66,"Nurivoic Nurivoice Co., Ltd"
 D8:77:8B,Intelbra Intelbras
 D8:78:7F,"UbeeInte Ubee Interactive Co., Limited"
 D8:78:E5,Kuhn Kuhn Sa
 D8:79:88,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+D8:7A:3B,SiliconL Silicon Laboratories
 D8:7C:DD,Sanix Sanix Incorporated
 D8:7D:7F,Sagemcom Sagemcom Broadband SAS
 D8:7E:6F,Cascinat Cascination Ag
 D8:7E:76,ItelMobi Itel Mobile Limited
 D8:7E:B1,"xoware x.o.ware, inc."
 D8:80:39,Microchi Microchip Technology Inc.
 D8:80:3C,AnhuiHua Anhui Huami Information Technology Company Limited
@@ -43629,14 +45169,15 @@
 D8:8A:3B,Unit-Em
 D8:8A:DC,"HuaweiDe Huawei Device Co., Ltd."
 D8:8B:4C,KingTing KingTing Tech.
 D8:8C:73,zte zte corporation
 D8:8C:79,"Google Google, Inc."
 D8:8D:5C,Elentec
 D8:8D:C8,"AtilTech Atil Technology Co., LTD"
+D8:8E:D4,eero eero inc.
 D8:8F:76,"Apple Apple, Inc."
 D8:90:E8,"SamsungE Samsung Electronics Co.,Ltd"
 D8:91:2A,ZyxelCom Zyxel Communications Corporation
 D8:91:36,DoverFue Dover Fueling Solutions
 D8:93:41,GeneralE General Electric Global Research
 D8:94:03,HewlettP Hewlett Packard Enterprise
 D8:95:2F,TexasIns Texas Instruments
@@ -43675,31 +45216,34 @@
 D8:A9:8B,TexasIns Texas Instruments
 D8:AA:59,TonlyTec Tonly Technology Co. Ltd
 D8:AD:49,"HonorDev Honor Device Co., Ltd."
 D8:AD:DD,"Sonavati Sonavation, Inc."
 D8:AE:90,ItibiaTe Itibia Technologies
 D8:AE:D0,"Shanghai Shanghai Engineering Science & Technology Co.,LTD CGNPC"
 D8:AF:3B,"Hangzhou Hangzhou Bigbright Integrated communications system Co.,Ltd"
-D8:AF:81,"AONPKRoT AO ""NPK RoTeK"""
+D8:AF:81,Ao
 D8:AF:F1,Panasoni Panasonic Appliances Company
 D8:B0:2E,"Guangzho Guangzhou Zonerich Business Machine Co., LTD."
 D8:B0:4C,"JinanUSR Jinan USR IOT Technology Co., Ltd."
 D8:B0:53,XiaomiCo Xiaomi Communications Co Ltd
 D8:B1:22,JuniperN Juniper Networks
 D8:B1:2A,"Panasoni Panasonic Mobile Communications Co.,Ltd."
 D8:B1:90,"Cisco Cisco Systems, Inc"
+D8:B2:49,"HuaweiDe Huawei Device Co., Ltd."
+D8:B3:70,Ubiquiti Ubiquiti Inc
 D8:B3:77,HTC HTC Corporation
 D8:B6:73,TexasIns Texas Instruments
 D8:B6:B7,Comtrend Comtrend Corporation
 D8:B6:C1,"NetworkA NetworkAccountant, Inc."
 D8:B6:D6,BluTethe Blu Tether Limited
 D8:B8:F6,Nantwork Nantworks
 D8:B9:0E,"TripleDo Triple Domain Vision Co.,Ltd."
 D8:BB:2C,"Apple Apple, Inc."
 D8:BB:C1,"Micro-St Micro-Star INTL CO., LTD."
+D8:BC:38,Espressi Espressif Inc.
 D8:BC:59,"Shenzhen Shenzhen DAPU Microelectronics Co., Ltd"
 D8:BE:1F,"Apple Apple, Inc."
 D8:BE:65,AmazonTe Amazon Technologies Inc.
 D8:BF:4C,VictoryC Victory Concept Electronics Limited
 D8:BF:C0,Espressi Espressif Inc.
 D8:C0:68,"Netgenet Netgenetech.co.,ltd."
 D8:C0:6A,"Hunantvc Hunantv.com Interactive Entertainment Media Co.,Ltd."
@@ -43724,34 +45268,37 @@
 D8:CF:9C,"Apple Apple, Inc."
 D8:CF:BF,"Motorola Motorola Mobility LLC, a Lenovo Company"
 D8:D0:90,Dell Dell Inc.
 D8:D1:CB,"Apple Apple, Inc."
 D8:D2:7C,"JemaEner Jema Energy, Sa"
 D8:D3:85,HewlettP Hewlett Packard
 D8:D4:3C,Sony Sony Corporation
+D8:D4:5D,OrbicNor Orbic North America
 D8:D4:E6,"HytecInt Hytec Inter Co., Ltd."
 D8:D5:B9,"Rainfore Rainforest Automation, Inc."
 D8:D6:7E,"GskCncEq Gsk Cnc Equipment Co.,Ltd"
 D8:D6:F3,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 D8:D7:23,"IDS IDS, Inc"
 D8:D7:75,Sagemcom Sagemcom Broadband SAS
 D8:D8:66,"Shenzhen Shenzhen Tozed Technologies Co.,Ltd."
 D8:DA:52,Apator Apator S.A.
+D8:DA:F1,"HuaweiTe Huawei Technologies Co.,Ltd"
 D8:DC:40,"Apple Apple, Inc."
 D8:DC:E9,"KunshanE Kunshan Erlab ductless filtration system Co.,Ltd"
 D8:DD:5F,BALMUDA BALMUDA Inc.
 D8:DD:FD,TexasIns Texas Instruments
 D8:DE:3A,"Apple Apple, Inc."
 D8:DE:CE,"Isung Isung Co.,Ltd"
 D8:DF:0D,beroNet beroNet GmbH
 D8:DF:7A,"QuestSof Quest Software, Inc."
 D8:E0:04,VodiaNet Vodia Networks Inc
 D8:E0:B8,Bulat Bulat Llc
 D8:E0:E1,"SamsungE Samsung Electronics Co.,Ltd"
 D8:E2:DF,Microsof Microsoft Corporation
+D8:E3:5E,LGInnote LG Innotek
 D8:E3:AE,CirtecMe Cirtec Medical Systems
 D8:E5:6D,TCTmobil TCT mobile ltd
 D8:E7:2B,Netscout Netscout Systems Inc
 D8:E7:43,"Wush Wush, Inc"
 D8:E8:44,zte zte corporation
 D8:E9:52,Keopsys
 D8:EB:46,"Google Google, Inc."
@@ -43778,24 +45325,26 @@
 D8:FB:D6,AmazonTe Amazon Technologies Inc.
 D8:FC:38,GiantecS Giantec Semiconductor Inc
 D8:FC:93,IntelCor Intel Corporate
 D8:FE:8F,"IDFone IDFone Co., Ltd."
 D8:FE:E3,D-LinkIn D-Link International
 D8:FF:C3,Shenzhen Shenzhen 3SNIC information technology company Limited
 DA:0D:38,"Farpoint Farpointe Data, Inc."
+DA:19:B3,LGUplus LG Uplus
 DA:1C:21,Sesam Sesam GmbH
 DA:1E:56,OSNexus
 DA:28:EC,HGGenuin HG Genuine
 DA:2B:DD,"AT&T AT&T, Inc."
 DA:41:62,Xperi Xperi Corporation
 DA:7D:2E,DeltaCom Delta Computers LLC.
 DA:9D:49,Calix Calix Inc.
 DA:A1:19,"Google Google, Inc."
 DA:C4:51,Takarato Takaratomy
 DA:C8:7D,SEDevelo SE Development AB
+DA:E6:D7,"NVMExpre NVM Express, Inc."
 DA:FF:6B,TeamPrec Team Precision Public Company Limited
 DC:00:77,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 DC:00:B0,FreeboxS Freebox Sas
 DC:02:65,Meditech Meditech Kft
 DC:02:8E,zte zte corporation
 DC:03:98,LGInnote LG Innotek
 DC:05:2F,National National Products Inc.
@@ -43831,37 +45380,40 @@
 DC:1D:D4,Microste Microstep-MIS spol. s r.o.
 DC:1E:A3,Accensus Accensus LLC
 DC:20:08,ASDElect ASD Electronics Ltd
 DC:21:48,IntelCor Intel Corporate
 DC:21:5C,IntelCor Intel Corporate
 DC:21:B9,Sentec Sentec Co.Ltd
 DC:21:E2,"HuaweiTe Huawei Technologies Co.,Ltd"
+DC:23:3B,"ExtremeN Extreme Networks, Inc."
 DC:27:27,"HuaweiDe Huawei Device Co., Ltd."
 DC:28:34,HAKKO HAKKO Corporation
 DC:29:19,"AltoBeam AltoBeam (Xiamen) Technology Ltd, Co."
 DC:29:3A,"Shenzhen Shenzhen Nuoshi Technology Co., LTD."
 DC:2A:14,Shanghai Shanghai Longjing Technology Co.
 DC:2A:A1,MedHab MedHab LLC
 DC:2B:2A,"Apple Apple, Inc."
 DC:2B:61,"Apple Apple, Inc."
 DC:2B:66,InfoBLOC InfoBLOCK S.A. de C.V.
 DC:2B:CA,Zera Zera GmbH
 DC:2C:26,ItonTech Iton Technology Limited
 DC:2C:6E,Routerbo Routerboard.com
 DC:2D:3C,"HuaweiDe Huawei Device Co., Ltd."
 DC:2D:CB,"BeijingU Beijing Unis HengYue Technology Co., Ltd."
+DC:2D:DE,Ledworks Ledworks SRL
 DC:2E:6A,"HCT HCT. Co., Ltd."
 DC:2F:03,"Stepforw Step forward Group Co., Ltd."
 DC:30:9C,Heyrex Heyrex Limited
 DC:31:D1,"vivoMobi vivo Mobile Communication Co., Ltd."
 DC:33:0D,"QingDaoH Qing Dao Haier Telecom Co.,Ltd."
 DC:33:3D,"HuaweiDe Huawei Device Co., Ltd."
 DC:33:50,TechSAT TechSAT GmbH
 DC:35:F1,Positivo Positivo Tecnologia S.A.
 DC:36:0C,HitronTe Hitron Technologies. Inc
+DC:36:42,zte zte corporation
 DC:36:43,IEEERegi IEEE Registration Authority
 DC:36:43:00:00:00/28,MeierTob Meier Tobler AG
 DC:36:43:10:00:00/28,Dongguan Dongguan Pengchen Earth Instrument CO. LT
 DC:36:43:20:00:00/28,"WuhanLin Wuhan Linptech Co. ,Ltd."
 DC:36:43:30:00:00/28,WISNetwo WIS Networks
 DC:36:43:40:00:00/28,"Freseniu Fresenius Medical Care R&D (Shanghai) Co.,Ltd."
 DC:36:43:50:00:00/28,"Hangzhou Hangzhou Chingan Tech Co., Ltd."
@@ -43906,14 +45458,15 @@
 DC:44:27:C0:00:00/28,PyrexxTe Pyrexx Technologies GmbH
 DC:44:27:D0:00:00/28,Rohde&Sc Rohde&Schwarz Topex SA
 DC:44:27:E0:00:00/28,VerifEye VerifEye Technologies
 DC:44:27:F0:00:00/28,Private
 DC:44:6D,"Allwinne Allwinner Technology Co., Ltd"
 DC:44:B6,"SamsungE Samsung Electronics Co.,Ltd"
 DC:45:17,"ARRISGro ARRIS Group, Inc."
+DC:45:B8,"Apple Apple, Inc."
 DC:46:28,IntelCor Intel Corporate
 DC:48:B2,Baraja Baraja Pty. Ltd.
 DC:49:C9,CascoSig Casco Signal Ltd
 DC:4A:3E,HewlettP Hewlett Packard
 DC:4A:9E,IEEERegi IEEE Registration Authority
 DC:4A:9E:00:00:00/28,"Dongguan Dongguan Huili electroacoustic Industrial Co.,ltd"
 DC:4A:9E:10:00:00/28,Advanced Advanced Electronics Ltd
@@ -43956,31 +45509,34 @@
 DC:64:7C,CRSiiMot C.R.S. iiMotion GmbH
 DC:64:B8,Shenzhen Shenzhen JingHanDa Electronics Co.Ltd
 DC:66:3A,ApacerTe Apacer Technology Inc.
 DC:66:72,"SamsungE Samsung Electronics Co.,Ltd"
 DC:67:23,baroxKom barox Kommunikation GmbH
 DC:68:0C,HewlettP Hewlett Packard Enterprise
 DC:68:EB,"Nintendo Nintendo Co.,Ltd"
+DC:69:E2,"SamsungE Samsung Electronics Co.,Ltd"
 DC:6A:E7,XiaomiCo Xiaomi Communications Co Ltd
 DC:6A:EA,Infinixm Infinix mobility limited
 DC:6B:12,worldcns worldcns inc.
 DC:6B:1B,"HuaweiDe Huawei Device Co., Ltd."
+DC:6D:BC,"Apple Apple, Inc."
 DC:6D:CD,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 DC:6F:00,"Livescri Livescribe, Inc."
 DC:6F:08,BayStora Bay Storage Technology
 DC:70:14,Private
 DC:71:37,zte zte corporation
 DC:71:44,"SamsungE Samsung Electro Mechanics Co., Ltd."
 DC:71:96,IntelCor Intel Corporate
 DC:71:DD,AXTechno AX Technologies
 DC:72:23,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 DC:72:9B,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:73:85,"HuaweiDe Huawei Device Co., Ltd."
 DC:74:A8,"SamsungE Samsung Electronics Co.,Ltd"
 DC:77:4C,"Cisco Cisco Systems, Inc"
+DC:77:94,"HuaweiDe Huawei Device Co., Ltd."
 DC:78:34,Logicom Logicom Sa
 DC:7B:94,"Cisco Cisco Systems, Inc"
 DC:7F:A4,2Wire 2Wire Inc
 DC:80:84,"Apple Apple, Inc."
 DC:82:5B,"JANUSspo JANUS, spol. s r.o."
 DC:82:F6,iPort
 DC:84:E9,"Shenzhen Shenzhen Qihoo Intelligent Technology Co.,Ltd"
@@ -43988,37 +45544,41 @@
 DC:86:D8,"Apple Apple, Inc."
 DC:87:CB,"Perfectk        Beijing Perfectek Technologies Co., Ltd."
 DC:89:83,"SamsungE Samsung Electronics Co.,Ltd"
 DC:8B:28,IntelCor Intel Corporate
 DC:8C:1B,"vivoMobi vivo Mobile Communication Co., Ltd."
 DC:8C:37,"Cisco Cisco Systems, Inc"
 DC:8D:8A,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
+DC:8D:91,Infinixm Infinix mobility limited
 DC:8D:B7,"AtwTechn Atw Technology, Inc."
 DC:8E:95,SiliconL Silicon Laboratories
 DC:90:20,RuruTekP Ruru Tek Private Limited
 DC:90:88,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:91:66,"HuaweiDe Huawei Device Co., Ltd."
 DC:91:BF,AmazonTe Amazon Technologies Inc.
 DC:96:2C,NSTAudio NST Audio Ltd
 DC:97:3A,VeranaNe Verana Networks
 DC:97:58,"SichuanA Sichuan AI-Link Technology Co., Ltd."
+DC:97:E6,Sagemcom Sagemcom Broadband SAS
 DC:98:40,Microsof Microsoft Corporation
 DC:99:14,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:99:FE,Armatura Armatura LLC
 DC:9A:7D,"HisenseV Hisense Visual Technology Co.,Ltd"
 DC:9A:8E,"NanjingC Nanjing Cocomm electronics co., LTD"
 DC:9B:1E,"Intercom Intercom, Inc."
 DC:9B:9C,"Apple Apple, Inc."
 DC:9B:D6,TCTmobil TCT mobile ltd
 DC:9C:52,Sapphire Sapphire Technology Limited.
 DC:9C:9F,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
+DC:9E:AB,"Chongqin Chongqing Yipingfang Technology Co., Ltd."
 DC:9F:A4,Nokia Nokia Corporation
-DC:9F:DB,Ubiquiti Ubiquiti Networks Inc.
+DC:9F:DB,Ubiquiti Ubiquiti Inc
 DC:A1:20,Nokia
 DC:A2:66,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
+DC:A3:13,"Shenzhen Shenzhen Changjin Communication Technology Co.,Ltd"
 DC:A3:33,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 DC:A3:A2,"FengmiBe Feng mi(Beijing)technology co., LTD"
 DC:A3:AC,RBcloudt RBcloudtech
 DC:A4:CA,"Apple Apple, Inc."
 DC:A5:F4,"Cisco Cisco Systems, Inc"
 DC:A6:32,Raspberr Raspberry Pi Trading Ltd
 DC:A6:33,"ARRISGro ARRIS Group, Inc."
@@ -44039,45 +45599,51 @@
 DC:B0:58,BürkertW Bürkert Werke GmbH
 DC:B0:82,Nokia
 DC:B1:31,"Shenzhen Shenzhen Huaruian Technology Co.,Ltd"
 DC:B3:47,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
 DC:B3:B4,"Honeywel Honeywell Environmental & Combustion Controls (Tianjin) Co., Ltd."
 DC:B4:AC,"Flextron Flextronics Manufacturing(Zhuhai)Co.,Ltd."
 DC:B4:C4,Microsof Microsoft XCG
+DC:B4:CA,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 DC:B5:4F,"Apple Apple, Inc."
 DC:B7:2E,XiaomiCo Xiaomi Communications Co Ltd
 DC:B7:AC,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 DC:B7:FC,AlpsElec Alps Electric (Ireland) Ltd
 DC:B8:08,"ExtremeN Extreme Networks, Inc."
 DC:BB:96,FullSolu Full Solution Telecom
 DC:BD:7A,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
+DC:BD:CC,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 DC:BE:49,ItelMobi Itel Mobile Limited
 DC:BE:7A,Zhejiang Zhejiang Nurotron Biotechnology Co.
 DC:BF:90,"HuizhouQ Huizhou Qiaoxing Telecommunication Industry Co.,Ltd."
 DC:BF:E9,"Motorola Motorola Mobility LLC, a Lenovo Company"
 DC:C0:DB,"Shenzhen Shenzhen Kaiboer Technology Co., Ltd."
 DC:C0:EB,AssaAblo Assa Abloy Côte Picarde
 DC:C1:01,"SOLiDTec SOLiD Technologies, Inc."
+DC:C2:C9,Canon Canon Inc.
 DC:C4:22,Systemba Systembase Limited
 DC:C6:22,BuheungS Buheung System
 DC:C6:4B,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:C7:93,Nokia Nokia Corporation
 DC:C8:F5,"Shanghai Shanghai UMEinfo CO.,LTD."
 DC:CB:A8,ExploraT Explora Technologies Inc
 DC:CC:8D,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 DC:CC:E6,"SamsungE Samsung Electronics Co.,Ltd"
+DC:CD:18,"Nintendo Nintendo Co.,Ltd"
 DC:CD:2F,SeikoEps Seiko Epson Corporation
+DC:CD:66,NXPSemic NXP Semiconductor (Tianjin) LTD.
 DC:CD:74,"JapanEMS Japan E.M.Solutions Co., Ltd."
 DC:CE:41,FeGlobal Fe Global Hong Kong Limited
 DC:CE:BC,"Shenzhen Shenzhen JSR Technology Co.,Ltd."
 DC:CE:C1,"Cisco Cisco Systems, Inc"
 DC:CF:94,"BeijingR Beijing Rongcheng Hutong Technology Co., Ltd."
 DC:CF:96,"SamsungE Samsung Electronics Co.,Ltd"
 DC:D0:F7,Bentek Bentek Systems Ltd.
 DC:D2:55,"KinpoEle Kinpo Electronics, Inc."
+DC:D2:6A,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 DC:D2:FC,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:D2:FD,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:D3:21,"HUMAX HUMAX Co., Ltd."
 DC:D3:A2,"Apple Apple, Inc."
 DC:D4:44,"HuaweiDe Huawei Device Co., Ltd."
 DC:D5:2A,SunnyHea Sunny Heart Limited
 DC:D7:A0,"HuaweiDe Huawei Device Co., Ltd."
@@ -44096,15 +45662,15 @@
 DC:DE:4F,GioneeCo Gionee Communication Equipment Co Ltd
 DC:DE:CA,Akyllor
 DC:DF:D6,zte zte corporation
 DC:E0:26,"PatrolTa Patrol Tag, Inc"
 DC:E0:EB,NanjingA Nanjing Aozheng Information Technology Co.Ltd
 DC:E1:AD,"Shenzhen Shenzhen Wintop Photoelectric Technology Co., Ltd"
 DC:E2:AC,LumensDi Lumens Digital Optics Inc.
-DC:E3:05,"AONPKRoT AO ""NPK RoTeK"""
+DC:E3:05,Ao
 DC:E5:33,IEEERegi IEEE Registration Authority
 DC:E5:33:00:00:00/28,FLYHTAer FLYHT Aerospace
 DC:E5:33:10:00:00/28,AmbiLabs Ambi Labs Limited
 DC:E5:33:20:00:00/28,Remko Remko GmbH & Co. KG
 DC:E5:33:30:00:00/28,ShenZhen ShenZhen C&D Electronics CO.Ltd.
 DC:E5:33:40:00:00/28,"shenzhen shenzhen bangying electronics co,.ltd"
 DC:E5:33:50:00:00/28,Controls Controls Inc
@@ -44120,17 +45686,18 @@
 DC:E5:5B,"Google Google, Inc."
 DC:E5:78,Experime Experimental Factory of Scientific Engineering and Special Design Department
 DC:E6:50,"ExtremeN Extreme Networks, Inc."
 DC:E7:1C,AUGElekt AUG Elektronik GmbH
 DC:E8:38,CKTeleco CK Telecom (Shenzhen) Limited
 DC:E9:94,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 DC:EB:53,"WuhanQia Wuhan QianXiao Elecronic Technology CO.,LTD"
-DC:EB:69,Technico Technicolor CH USA Inc.
+DC:EB:69,VantivaU Vantiva USA LLC
 DC:EB:94,"Cisco Cisco Systems, Inc"
 DC:EC:06,"HeimiNet Heimi Network Technology Co., Ltd."
+DC:EC:E3,LyotechL Lyotech Labs Llc
 DC:ED:83,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 DC:ED:84,Haverfor Haverford Systems Inc
 DC:EE:06,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:EF:09,Netgear
 DC:EF:80,"HuaweiTe Huawei Technologies Co.,Ltd"
 DC:EF:CA,"MurataMa Murata Manufacturing Co., Ltd."
 DC:F0:5D,LettaTek Letta Teknoloji
@@ -44188,16 +45755,19 @@
 E0:1C:EE,"BravoTec Bravo Tech, Inc."
 E0:1C:FC,D-LinkIn D-Link International
 E0:1D:38,"BeijingH Beijing HuaqinWorld Technology Co.,Ltd"
 E0:1D:3B,"Cambridg Cambridge Industries(Group) Co.,Ltd."
 E0:1E:07,AniteTel Anite Telecoms US. Inc
 E0:1F:0A,XslentEn Xslent Energy Technologies. LLC
 E0:1F:2B,NokiaSol Nokia Solutions and Networks GmbH & Co. KG
+E0:1F:6A,"HuaweiDe Huawei Device Co., Ltd."
 E0:1F:88,XiaomiCo Xiaomi Communications Co Ltd
 E0:1F:ED,"NokiaSha Nokia Shanghai Bell Co., Ltd."
+E0:1F:FC,"Motorola Motorola (Wuhan) Mobility Technologies Communication Co., Ltd."
+E0:21:FE,"RicherLi Richer Link Technologies CO.,LTD"
 E0:22:02,"ARRISGro ARRIS Group, Inc."
 E0:23:D7,SleepNum Sleep Number
 E0:23:FF,"Fortinet Fortinet, Inc."
 E0:24:7F,"HuaweiTe Huawei Technologies Co.,Ltd"
 E0:24:81,"HuaweiTe Huawei Technologies Co.,Ltd"
 E0:25:38,TitanPet Titan Pet Products
 E0:26:30,"Intrigue Intrigue Technologies, Inc."
@@ -44223,15 +45793,15 @@
 E0:31:9E,Valve Valve Corporation
 E0:31:D0,"SZTelsta SZ Telstar CO., LTD"
 E0:33:8E,"Apple Apple, Inc."
 E0:34:E4,"FeitElec Feit Electric Company, Inc."
 E0:35:60,"Challeng Challenger Supply Holdings, LLC"
 E0:36:76,"HuaweiTe Huawei Technologies Co.,Ltd"
 E0:36:E3,"StageOne Stage One International Co., Ltd."
-E0:37:17,Technico Technicolor CH USA Inc.
+E0:37:17,VantivaU Vantiva USA LLC
 E0:37:BF,WistronN Wistron Neweb Corporation
 E0:38:2D,IEEERegi IEEE Registration Authority
 E0:38:2D:00:00:00/28,"BeijingC Beijing Cgprintech Technology Co.,Ltd"
 E0:38:2D:10:00:00/28,Annapurn Annapurna labs
 E0:38:2D:20:00:00/28,"XianXian Xi'an Xiangxun Technology Co., Ltd."
 E0:38:2D:30:00:00/28,Annapurn Annapurna labs
 E0:38:2D:40:00:00/28,"QingdaoU Qingdao Unovo Technologies Co., Ltd"
@@ -44243,14 +45813,30 @@
 E0:38:2D:A0:00:00/28,4DPhoton 4D Photonics GmbH
 E0:38:2D:B0:00:00/28,SercommP Sercomm Philippines Inc
 E0:38:2D:C0:00:00/28,"SiLANDCh SiLAND Chengdu Technology Co., Ltd"
 E0:38:2D:D0:00:00/28,KeplerCo Kepler Communications Inc.
 E0:38:2D:E0:00:00/28,Anysafe
 E0:38:3F,zte zte corporation
 E0:39:D7,"Plexxi Plexxi, Inc."
+E0:3C:1C,IEEERegi IEEE Registration Authority
+E0:3C:1C:00:00:00/28,Scangrip
+E0:3C:1C:10:00:00/28,"ShikinoH Shikino High-Tech Co., Ltd."
+E0:3C:1C:20:00:00/28,"HopliteI Hoplite Industries, Inc."
+E0:3C:1C:30:00:00/28,Dewetron Dewetron GmbH
+E0:3C:1C:40:00:00/28,Earable Earable Inc.
+E0:3C:1C:50:00:00/28,Semic Semic Inc.
+E0:3C:1C:60:00:00/28,"GhinFDig GhinF Digital information technology (hangzhou) Co., Ltd"
+E0:3C:1C:70:00:00/28,"TapHomes Tap Home, s.r.o."
+E0:3C:1C:80:00:00/28,"JiangsuR Jiangsu Riying Electronics Co.,Ltd."
+E0:3C:1C:90:00:00/28,"OcamarTe Ocamar Technologies (Shanghai) Co.,Ltd."
+E0:3C:1C:A0:00:00/28,MELAGMed MELAG Medizintechnik GmbH & Co. KG
+E0:3C:1C:B0:00:00/28,"Hangzhou Hangzhou Uni-Ubi Co.,Ltd."
+E0:3C:1C:C0:00:00/28,"MeferiTe Meferi Technologies Co.,Ltd."
+E0:3C:1C:D0:00:00/28,Sprintsh Sprintshield d.o.o.
+E0:3C:1C:E0:00:00/28,Annapurn Annapurna labs
 E0:3C:5B,"Shenzhen Shenzhen Jiaxinjie Electron Co.,Ltd"
 E0:3E:44,Broadcom
 E0:3E:4A,Cavanagh Cavanagh Group International
 E0:3E:7D,data-com data-complex GmbH
 E0:3F:49,ASUSTekC ASUSTek COMPUTER INC.
 E0:40:07,"HuaweiDe Huawei Device Co., Ltd."
 E0:41:02,zte zte corporation
@@ -44272,14 +45858,16 @@
 E0:4F:BD,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 E0:50:8B,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 E0:51:24,NXPSemic NXP Semiconductors
 E0:51:63,Arcadyan Arcadyan Corporation
 E0:51:D8,ChinaDra China Dragon Technology Limited
 E0:55:3D,CiscoMer Cisco Meraki
 E0:55:97,Emergent Emergent Vision Technologies Inc.
+E0:56:89,LootomTe Lootom Telcovideo Network (Wuxi) Co Ltd
+E0:56:94,Yunhight Yunhight Microelectronics
 E0:56:F4,AxesNetw AxesNetwork Solutions inc.
 E0:58:9E,LaerdalM Laerdal Medical
 E0:5A:1B,Espressi Espressif Inc.
 E0:5A:9F,IEEERegi IEEE Registration Authority
 E0:5A:9F:00:00:00/28,Annapurn Annapurna labs
 E0:5A:9F:10:00:00/28,"AitecSys Aitec System Co., Ltd."
 E0:5A:9F:20:00:00/28,"ChengduS Chengdu Song Yuan Electronic Technology Co.,Ltd"
@@ -44302,34 +45890,36 @@
 E0:5F:B9,"Cisco Cisco Systems, Inc"
 E0:60:66,Sercomm Sercomm Corporation.
 E0:60:89,"Cloudlea Cloudleaf, Inc."
 E0:61:B2,"Hangzhou Hangzhou Zenointel Technology Co., Ltd"
 E0:62:34,TexasIns Texas Instruments
 E0:62:67,XiaomiCo Xiaomi Communications Co Ltd
 E0:62:90,"JinanJov Jinan Jovision Science & Technology Co., Ltd."
-E0:63:DA,Ubiquiti Ubiquiti Networks Inc.
+E0:63:DA,Ubiquiti Ubiquiti Inc
 E0:63:E5,Sony Sony Corporation
 E0:64:BB,DigiView DigiView S.r.l.
 E0:66:78,"Apple Apple, Inc."
 E0:67:81,"Dongguan Dongguan Liesheng Electronic Co., Ltd."
 E0:67:B3,"Shenzhen Shenzhen C-Data Technology Co., Ltd"
 E0:68:6D,Raybased Raybased AB
+E0:68:EE,PhyplusM Phyplus Microelectronics Limited
 E0:69:3A,Innophas Innophase Inc.
 E0:69:95,Pegatron Pegatron Corporation
 E0:69:BA,"Cisco Cisco Systems, Inc"
 E0:6A:05,"Shenzhen Shenzhen YOUHUA Technology Co., Ltd"
 E0:6C:4E,Shenzhen Shenzhen TINNO Mobile Technology Corp.
 E0:6C:A6,Creotech Creotech Instruments S.A.
 E0:6C:C5,"HuaweiDe Huawei Device Co., Ltd."
 E0:6C:F6,ESSENCOR ESSENCORE limited
 E0:6D:17,"Apple Apple, Inc."
 E0:6D:18,Pioneerc Pioneercorporation
 E0:70:EA,HP HP Inc.
 E0:72:0A,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 E0:73:5F,Nucom
+E0:73:E7,HP HP Inc.
 E0:75:0A,"Alpsalpi Alpsalpine Co,.Ltd"
 E0:75:26,ChinaDra China Dragon Technology Limited
 E0:75:7D,"Motorola Motorola Mobility LLC, a Lenovo Company"
 E0:75:AA,"BeijingJ Beijing Jingling Information System Technology Co., Ltd."
 E0:76:D0,"AMPAKTec AMPAK Technology, Inc."
 E0:77:26,"HuaweiDe Huawei Device Co., Ltd."
 E0:78:A3,"Shanghai Shanghai Winner Information Technology Co.,Inc"
@@ -44344,15 +45934,15 @@
 E0:7F:88,EVIDENCE EVIDENCE Network SIA
 E0:80:6B,XiaomiCo Xiaomi Communications Co Ltd
 E0:81:77,"GreenByt GreenBytes, Inc."
 E0:84:F3,HighGrad High Grade Controls Corporation
 E0:85:9A,"Shenzhen Shenzhen Rf-Link Technology Co.,Ltd."
 E0:86:14,"NovatelW Novatel Wireless Solutions, Inc."
 E0:87:B1,Nata-Inf Nata-Info Ltd.
-E0:88:5D,Technico Technicolor CH USA Inc.
+E0:88:5D,VantivaU Vantiva USA LLC
 E0:89:7E,"Apple Apple, Inc."
 E0:89:9D,"Cisco Cisco Systems, Inc"
 E0:8A:7E,Exponent
 E0:8E:3C,AztechEl Aztech Electronics Pte Ltd
 E0:8F:EC,"Repotec Repotec Co., Ltd."
 E0:91:3C,"Kyeungin Kyeungin CNS Co., Ltd."
 E0:91:53,XAViTech XAVi Technologies Corp.
@@ -44363,20 +45953,22 @@
 E0:94:67,IntelCor Intel Corporate
 E0:95:79,"ORTHOsof ORTHOsoft inc, d/b/a Zimmer CAS"
 E0:97:96,"HuaweiTe Huawei Technologies Co.,Ltd"
 E0:97:F2,Atomax Atomax Inc.
 E0:98:06,Espressi Espressif Inc.
 E0:98:61,"Motorola Motorola Mobility LLC, a Lenovo Company"
 E0:99:71,"SamsungE Samsung Electronics Co.,Ltd"
+E0:9B:27,Ciena Ciena Corporation
 E0:9C:8D,"Seakeepe Seakeeper, Inc."
 E0:9D:13,"SamsungE Samsung Electronics Co.,Ltd"
 E0:9D:31,IntelCor Intel Corporate
 E0:9D:B8,PlanexCo Planex Communications Inc.
 E0:9D:FA,WananHon Wanan Hongsheng Electronic Co.Ltd
 E0:9F:2A,ItonTech Iton Technology Corp.
+E0:A1:29,"ExtremeN Extreme Networks, Inc."
 E0:A1:98,NOJAPowe NOJA Power Switchgear Pty Ltd
 E0:A1:CE,zte zte corporation
 E0:A1:D7,Sfr
 E0:A2:58,"WanbangD Wanbang Digital Energy Co.,Ltd"
 E0:A2:5A,"Shanghai Shanghai Mo xiang Network Technology CO.,ltd"
 E0:A3:0F,Pevco
 E0:A3:AC,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -44446,14 +46038,15 @@
 E0:C7:9D,TexasIns Texas Instruments
 E0:C8:6A,"SHENZHEN SHENZHEN TW-SCIE Co., Ltd"
 E0:C9:22,"JirehEne Jireh Energy Tech., Ltd."
 E0:C9:7A,"Apple Apple, Inc."
 E0:CA:3C,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 E0:CA:4D,"Shenzhen Shenzhen Unistar Communication Co.,LTD"
 E0:CA:94,AskeyCom Askey Computer Corp
+E0:CB:19,Nokia
 E0:CB:1D,AmazonTe Amazon Technologies Inc.
 E0:CB:4E,ASUSTekC ASUSTek COMPUTER INC.
 E0:CB:56,"Shenzhen Shenzhen iComm Semiconductor CO.,LTD"
 E0:CB:BC,CiscoMer Cisco Meraki
 E0:CB:EE,"SamsungE Samsung Electronics Co.,Ltd"
 E0:CC:7A,"HuaweiTe Huawei Technologies Co.,Ltd"
 E0:CC:F8,XiaomiCo Xiaomi Communications Co Ltd
@@ -44469,25 +46062,27 @@
 E0:D4:62,"HuaweiDe Huawei Device Co., Ltd."
 E0:D4:64,IntelCor Intel Corporate
 E0:D4:E8,IntelCor Intel Corporate
 E0:D5:5E,"Giga-Byt Giga-Byte Technology Co.,Ltd."
 E0:D7:38,WireStar WireStar Networks
 E0:D7:BA,TexasIns Texas Instruments
 E0:D8:48,Dell Dell Inc.
+E0:D8:C4,"QingdaoI Qingdao Intelligent&Precise Electronics Co.,Ltd."
 E0:D9:A2,Hippihap Hippih aps
 E0:D9:E3,EltexEnt Eltex Enterprise Ltd.
 E0:DA:90,"HuaweiTe Huawei Technologies Co.,Ltd"
 E0:DA:DC,JVCKENWO JVC KENWOOD Corporation
 E0:DB:10,"SamsungE Samsung Electronics Co.,Ltd"
 E0:DB:55,Dell Dell Inc.
 E0:DB:88,OpenStan Open Standard Digital-IF Interface for SATCOM Systems
-E0:DB:D1,Technico Technicolor CH USA Inc.
-E0:DC:A0,SiemensI Siemens Industrial Automation Products Ltd Chengdu
+E0:DB:D1,VantivaU Vantiva USA LLC
+E0:DC:A0,"SiemensI Siemens Industrial Automation Products Ltd., Chengdu"
 E0:DC:FF,XiaomiCo Xiaomi Communications Co Ltd
 E0:DD:C0,"vivoMobi vivo Mobile Communication Co., Ltd."
+E0:DF:13,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 E0:E0:C2,"ChinaMob China Mobile Group Device Co.,Ltd."
 E0:E0:FC,"HuaweiDe Huawei Device Co., Ltd."
 E0:E1:A9,"Shenzhen Shenzhen Four Seas Global Link Network Technology Co., Ltd."
 E0:E2:E6,Espressi Espressif Inc.
 E0:E3:7C,"HuaweiDe Huawei Device Co., Ltd."
 E0:E5:CF,TexasIns Texas Instruments
 E0:E6:2E,TCTmobil TCT mobile ltd
@@ -44524,23 +46119,25 @@
 E4:02:9B,IntelCor Intel Corporate
 E4:04:39,TomTomSo TomTom Software Ltd
 E4:05:F8,Bytedanc Bytedance
 E4:07:2B,"HuaweiDe Huawei Device Co., Ltd."
 E4:08:E7,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 E4:0C:FD,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 E4:0D:36,IntelCor Intel Corporate
+E4:0D:3B,Ericsson Ericsson AB
 E4:0E:EE,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:11:5B,HewlettP Hewlett Packard
 E4:12:18,"ShenZhen ShenZhen Rapoo Technology Co., Ltd."
 E4:12:1D,"SamsungE Samsung Electronics Co.,Ltd"
-E4:12:89,topsyste topsystem Systemhaus GmbH
+E4:12:89,topsyste topsystem GmbH
 E4:15:F6,TexasIns Texas Instruments
 E4:17:D8,8BitdoTe 8Bitdo Technology Hk Limited
 E4:18:6B,ZyxelCom Zyxel Communications Corporation
 E4:19:C1,"HuaweiTe Huawei Technologies Co.,Ltd"
+E4:1A:1D,NoveaEne Novea Energies
 E4:1A:2C,"ZPE ZPE Systems, Inc."
 E4:1C:4B,"V2Techno V2 Technology, Inc."
 E4:1D:2D,"Mellanox Mellanox Technologies, Inc."
 E4:1E:0A,IEEERegi IEEE Registration Authority
 E4:1E:0A:00:00:00/28,Zavod№42 Zavod № 423
 E4:1E:0A:10:00:00/28,Connecte Connected Cars A/S
 E4:1E:0A:20:00:00/28,IDvacoPr IDvaco Private Limited
@@ -44555,14 +46152,15 @@
 E4:1E:0A:B0:00:00/28,"SafetyVi Safety Vision, LLC"
 E4:1E:0A:C0:00:00/28,Teletask Teletask Belgium
 E4:1E:0A:D0:00:00/28,ROMOWind ROMO Wind A/S
 E4:1E:0A:E0:00:00/28,"Shanghai Shanghai LeXiang Technology Co., Ltd"
 E4:1F:13,IBM IBM Corp
 E4:1F:7B,"Cisco Cisco Systems, Inc"
 E4:1F:E9,Dunkermo Dunkermotoren GmbH
+E4:21:50,"Shanghai Shanghai Chint low voltage electrical technology Co.,Ltd."
 E4:22:A5,"Plantron Plantronics, Inc."
 E4:23:3C,JuniperN Juniper Networks
 E4:23:54,"Shenzhen Shenzhen Fuzhi Software Technology Co.,Ltd"
 E4:24:6C,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 E4:25:E7,"Apple Apple, Inc."
 E4:25:E9,Color-Ch Color-Chip
 E4:26:86,DWnetTec DWnet Technologies(Suzhou) Corporation
@@ -44587,33 +46185,36 @@
 E4:32:CB,"SamsungE Samsung Electronics Co.,Ltd"
 E4:33:AE,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 E4:34:93,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:35:93,Hangzhou Hangzhou GoTo technology Co.Ltd
 E4:35:C8,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:35:FB,SabreTec Sabre Technology (Hull) Ltd
 E4:37:D7,HenriDep Henri Depaepe S.A.S.
+E4:38:19,"Shenzhen Shenzhen Hi-Link Electronic CO.,Ltd."
 E4:38:7E,"Cisco Cisco Systems, Inc"
-E4:38:83,Ubiquiti Ubiquiti Networks Inc.
+E4:38:83,Ubiquiti Ubiquiti Inc
 E4:38:8C,DigitalP Digital Products Limited
 E4:38:F2,Advantag Advantage Controls
 E4:3A:65,MofiNetw MofiNetwork Inc
 E4:3A:6E,"Shenzhen Shenzhen Zeroone Technology CO.,LTD"
 E4:3B:C9,"HisenseV Hisense Visual Technology Co.,Ltd"
 E4:3C:80,Universi University of Oklahoma
 E4:3D:1A,Broadcom Broadcom Limited
 E4:3E:C6,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:3E:D7,Arcadyan Arcadyan Corporation
 E4:3F:A2,WuxiDSPT Wuxi DSP Technologies Inc.
+E4:40:97,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 E4:40:E2,"SamsungE Samsung Electronics Co.,Ltd"
 E4:41:22,"OnePlusT OnePlus Technology (Shenzhen) Co., Ltd"
 E4:41:64,Nokia
 E4:41:E6,OttecTec Ottec Technology GmbH
 E4:42:A6,IntelCor Intel Corporate
 E4:43:4B,Dell Dell Inc.
 E4:44:E5,"ExtremeN Extreme Networks, Inc."
+E4:45:19,"BeijingX Beijing Xiaomi Electronics Co.,Ltd"
 E4:46:B0,FujitsuC Fujitsu Client Computing Limited
 E4:46:BD,"C&CTechn C&C Technic Taiwan Co., Ltd."
 E4:46:DA,XiaomiCo Xiaomi Communications Co Ltd
 E4:47:90,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 E4:47:91,"IrisID Iris ID Systems, Inc."
 E4:47:B3,zte zte corporation
 E4:48:C7,CiscoSPV Cisco SPVTG
@@ -44705,14 +46306,15 @@
 E4:85:01,GeberitI Geberit International AG
 E4:8A:D5,"RfWindow Rf Window Co., Ltd."
 E4:8B:7F,"Apple Apple, Inc."
 E4:8C:0F,Discover Discovery Insure
 E4:8C:73,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 E4:8D:8C,Routerbo Routerboard.com
 E4:8E:10,CigShang Cig Shanghai Co Ltd
+E4:8E:BB,Rockwell Rockwell Automation
 E4:8F:1D,"HuaweiDe Huawei Device Co., Ltd."
 E4:8F:34,Vodafone Vodafone Italia S.p.A.
 E4:8F:65,"YelatmaI Yelatma Instrument Making Enterprise, JSC"
 E4:90:2A,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:90:69,Rockwell Rockwell Automation
 E4:90:7E,"Motorola Motorola Mobility LLC, a Lenovo Company"
 E4:90:FD,"Apple Apple, Inc."
@@ -44747,14 +46349,15 @@
 E4:9C:67,"Apple Apple, Inc."
 E4:9D:73,Edgecore Edgecore Networks Corporation
 E4:9E:12,FreeboxS Freebox Sas
 E4:9F:1E,"ARRISGro ARRIS Group, Inc."
 E4:A1:E6,"Alcatel- Alcatel-Lucent Shanghai Bell Co., Ltd"
 E4:A3:2F,"Shanghai Shanghai Artimen Technology Co., Ltd."
 E4:A3:87,ControlS Control Solutions LLC
+E4:A4:1C,"Cisco Cisco Systems, Inc"
 E4:A4:71,IntelCor Intel Corporate
 E4:A5:EF,"TronLink Tron Link Electronics Co., Ltd."
 E4:A6:34,"Universa Universal Electronics, Inc."
 E4:A7:49,PaloAlto Palo Alto Networks
 E4:A7:A0,IntelCor Intel Corporate
 E4:A7:C5,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:A7:FD,CellcoPa Cellco Partnership
@@ -44765,24 +46368,28 @@
 E4:AA:EC,"TianjinH Tianjin Hualai Technology Co., Ltd"
 E4:AB:46,UABSelte UAB Selteka
 E4:AB:89,MitraSta MitraStar Technology Corp.
 E4:AD:7D,SCLEleme SCL Elements
 E4:AF:A1,Hes-So
 E4:B0:05,"BeijingI Beijing IQIYI Science & Technology Co., Ltd."
 E4:B0:21,"SamsungE Samsung Electronics Co.,Ltd"
+E4:B2:24,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:B2:FB,"Apple Apple, Inc."
 E4:B3:18,IntelCor Intel Corporate
 E4:B5:03,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 E4:B5:55,"HuaweiDe Huawei Device Co., Ltd."
 E4:B6:33,"WuxiStar Wuxi Stars Microsystem Technology Co., Ltd"
 E4:B9:7A,Dell Dell Inc.
 E4:BA:D9,360Fly 360 Fly Inc.
+E4:BC:96,Dap Dap B.V.
+E4:BC:AA,XiaomiCo Xiaomi Communications Co Ltd
 E4:BD:4B,zte zte corporation
 E4:BE:ED,NetcoreT Netcore Technology Inc.
-E4:BF:FA,Technico Technicolor CH USA Inc.
+E4:BE:FB,"HuaweiTe Huawei Technologies Co.,Ltd"
+E4:BF:FA,VantivaU Vantiva USA LLC
 E4:C0:CC,"ChinaMob China Mobile Group Device Co.,Ltd."
 E4:C0:E2,Sagemcom Sagemcom Broadband SAS
 E4:C1:46,Objetivo Objetivos y Servicios de Valor A
 E4:C1:F1,"SHENZHEN SHENZHEN SPOTMAU INFORMATION TECHNOLIGY CO., Ltd"
 E4:C2:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:C3:2A,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 E4:C4:83,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
@@ -44809,14 +46416,15 @@
 E4:DA:DF,TaicangT Taicang T&W Electronics
 E4:DB:6D,"BeijingX Beijing Xiaomi Electronics Co., Ltd."
 E4:DB:AE,"ExtremeN Extreme Networks, Inc."
 E4:DC:43,"HuaweiDe Huawei Device Co., Ltd."
 E4:DC:5F,"Cofracta Cofractal, Inc."
 E4:DC:CC,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:DD:79,"En-Visio En-Vision America, Inc."
+E4:DE:40,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 E4:E0:A6,"Apple Apple, Inc."
 E4:E0:C5,"SamsungE Samsung Electronics Co.,Ltd"
 E4:E1:12,TexasIns Texas Instruments
 E4:E1:30,TCTmobil TCT mobile ltd
 E4:E4:09,Leifheit Leifheit Ag
 E4:E4:AB,"Apple Apple, Inc."
 E4:E7:49,HewlettP Hewlett Packard
@@ -44837,14 +46445,15 @@
 E4:F4:C6,Netgear
 E4:F7:5B,"ARRISGro ARRIS Group, Inc."
 E4:F7:A1,Datafox Datafox GmbH
 E4:F8:9C,IntelCor Intel Corporate
 E4:F8:EF,"SamsungE Samsung Electronics Co.,Ltd"
 E4:F9:39,MinxonHo Minxon Hotel Technology INC.
 E4:FA:1D,PADPerip PAD Peripheral Advanced Design Inc.
+E4:FA:C4,BigField Big Field Global PTE. Ltd.
 E4:FA:ED,"SamsungE Samsung Electronics Co.,Ltd"
 E4:FA:FD,IntelCor Intel Corporate
 E4:FB:5D,"HuaweiTe Huawei Technologies Co.,Ltd"
 E4:FB:8F,"Mobiwire Mobiwire Mobiles (Ningbo) Co.,Ltd"
 E4:FC:82,JuniperN Juniper Networks
 E4:FD:45,IntelCor Intel Corporate
 E4:FD:A1,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -44868,14 +46477,15 @@
 E8:09:59,"Guoguang Guoguang Electric Co.,Ltd"
 E8:0A:EC,"JiangsuH Jiangsu Hengtong Optic-Electric Co., LTD"
 E8:0B:13,"AkibTaiw Akib Systems Taiwan, INC"
 E8:0C:38,"Daeyoung Daeyoung Information System Co., Ltd"
 E8:0C:75,"Syncbak Syncbak, Inc."
 E8:0F:C8,"Universa Universal Electronics, Inc."
 E8:10:2E,"ReallySi Really Simple Software, Inc"
+E8:10:98,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 E8:11:32,"SamsungE Samsung Electronics Co.,Ltd"
 E8:11:CA,"Shandong Shandong Kaer Electric.Co.,Ltd"
 E8:13:24,"GuangZho GuangZhou Bonsoninfo System CO.,LTD"
 E8:13:63,"Comstock Comstock RD, Inc."
 E8:13:67,AIRSOUND AIRSOUND Inc.
 E8:13:6E,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:15:0E,Nokia Nokia Corporation
@@ -44903,14 +46513,16 @@
 E8:1B:4B,amnimo amnimo Inc.
 E8:1B:69,Sercomm Sercomm Corporation.
 E8:1C:BA,"Fortinet Fortinet, Inc."
 E8:1C:D8,"Apple Apple, Inc."
 E8:1D:A8,RuckusWi Ruckus Wireless
 E8:1E:92,"HuaweiDe Huawei Device Co., Ltd."
 E8:20:E2,"HUMAX HUMAX Co., Ltd."
+E8:24:04,"QuectelW Quectel Wireless Solutions Co.,Ltd."
+E8:24:A6,JuniperN Juniper Networks
 E8:26:89,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 E8:26:8D,"Shenzhen Shenzhen SuperElectron Technology Co.,Ltd."
 E8:26:B6,Companie Companies House to GlucoRx Technologies Ltd.
 E8:28:77,"TMY TMY Co., Ltd."
 E8:28:C1,EltexEnt Eltex Enterprise Ltd.
 E8:28:D5,CotsTech Cots Technology
 E8:2A:44,LiteonTe Liteon Technology Corporation
@@ -44941,14 +46553,15 @@
 E8:43:B6,"QNAP QNAP Systems, Inc."
 E8:44:7E,Bitdefen Bitdefender SRL
 E8:47:27,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 E8:47:3A,"HonHaiPr Hon Hai Precision Industry Co.,LTD"
 E8:48:1F,Advanced Advanced Automotive Antennas
 E8:48:B8,TP-Link TP-Link Corporation Limited
 E8:49:43,YUGEInfo YUGE Information technology Co. Ltd
+E8:4C:4A,AmazonTe Amazon Technologies Inc.
 E8:4C:56,Intercep Intercept Services Limited
 E8:4D:74,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:4D:D0,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:4D:EC,Xerox Xerox Corporation
 E8:4E:06,"EdupInte Edup International (Hk) Co., Ltd"
 E8:4E:84,"SamsungE Samsung Electronics Co.,Ltd"
 E8:4E:CE,"Nintendo Nintendo Co., Ltd."
@@ -45005,21 +46618,24 @@
 E8:6C:DA,Supercom Supercomputers and Neurocomputers Research Center
 E8:6D:52,"ARRISGro ARRIS Group, Inc."
 E8:6D:54,DigitMob Digit Mobile Inc
 E8:6D:65,AUDIOMOB AUDIO MOBIL Elektronik GmbH
 E8:6D:6E,voestalp voestalpine Signaling UK Ltd.
 E8:6D:CB,"SamsungE Samsung Electronics Co.,Ltd"
 E8:6D:E9,"HuaweiTe Huawei Technologies Co.,Ltd"
+E8:6E:3A,SonyInte Sony Interactive Entertainment Inc.
 E8:6E:44,zte zte corporation
 E8:6F:38,"Chongqin Chongqing Fugui Electronics Co.,Ltd."
 E8:6F:F2,"Actionte Actiontec Electronics, Inc"
+E8:70:72,"Hangzhou Hangzhou BroadLink Technology Co.,Ltd"
 E8:71:8D,ElsysEqu Elsys Equipamentos Eletronicos Ltda
 E8:74:C7,Sentinhe Sentinhealth
 E8:74:E6,ADBBroad ADB Broadband Italia
 E8:75:7F,"FIRSTech FIRS Technologies(Shenzhen) Co., Ltd"
+E8:76:40,SkyUk Sky Uk Limited
 E8:78:29,IEEERegi IEEE Registration Authority
 E8:78:29:00:00:00/28,TanzSecu Tanz Security Technology Ltd.
 E8:78:29:10:00:00/28,"Shenzhen Shenzhen Jointelli Technologies Co.,Ltd"
 E8:78:29:20:00:00/28,Galcon
 E8:78:29:30:00:00/28,"Electron Electronic Controlled Systems, Inc."
 E8:78:29:40:00:00/28,Annapurn Annapurna labs
 E8:78:29:50:00:00/28,"ShenZhen Shen Zhen Skysi Wisdom Technology Co.,Ltd."
@@ -45030,53 +46646,58 @@
 E8:78:29:A0:00:00/28,METZCONN METZ CONNECT GmbH
 E8:78:29:B0:00:00/28,Ampner Ampner Ltd
 E8:78:29:C0:00:00/28,FairPhon FairPhone B.V.
 E8:78:29:D0:00:00/28,BerndWal Bernd Walter Computer Technology
 E8:78:29:E0:00:00/28,SolosTec Solos Technology Limited
 E8:78:65,"Apple Apple, Inc."
 E8:78:A1,BeoviewI Beoview Intercom Doo
+E8:78:EE,"NewH3CTe New H3C Technologies Co., Ltd"
 E8:7A:F3,S5Tech S5 Tech S.r.l.
 E8:7F:6B,"SamsungE Samsung Electronics Co.,Ltd"
 E8:7F:95,"Apple Apple, Inc."
 E8:80:2E,"Apple Apple, Inc."
-E8:80:88,"LCFCHefe LCFC(Hefei) Electronics Technology Co., Ltd"
+E8:80:88,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 E8:80:D8,"GNTEKEle GNTEK Electronics Co.,Ltd."
 E8:81:52,"Apple Apple, Inc."
 E8:81:75,zte zte corporation
 E8:81:AB,"BeijingS Beijing Sankuai Online Technology Co.,Ltd"
 E8:82:5B,"ARRISGro ARRIS Group, Inc."
 E8:84:A5,IntelCor Intel Corporate
 E8:84:C6,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:85:4B,"Apple Apple, Inc."
 E8:86:CF,Nokia
 E8:87:A3,LoxleyPu Loxley Public Company Limited
+E8:88:43,XiaomiCo Xiaomi Communications Co Ltd
 E8:88:6C,"Shenzhen Shenzhen SC Technologies Co.,LTD"
 E8:89:2C,"ARRISGro ARRIS Group, Inc."
 E8:8D:28,"Apple Apple, Inc."
 E8:8D:F5,"ZNYXNetw ZNYX Networks, Inc."
 E8:8E:60,NSD NSD Corporation
 E8:8F:6F,TCTmobil TCT mobile ltd
+E8:8F:C4,"Mobiwire Mobiwire Mobiles(Ningbo) Co.,Ltd"
 E8:91:0F,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 E8:91:20,"Motorola Motorola Mobility LLC, a Lenovo Company"
 E8:92:18,Arcontia Arcontia International AB
 E8:92:A4,LGElectr LG Electronics (Mobile Communications)
 E8:93:09,"SamsungE Samsung Electronics Co.,Ltd"
 E8:93:63,Nokia
 E8:93:F3,Graphian Graphiant Inc
 E8:94:4C,CogentHe Cogent Healthcare Systems Ltd
 E8:94:F6,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 E8:95:26,"Luxshare Luxshare Precision Industry CO., LTD."
 E8:96:06,"testoIns testo Instruments (Shenzhen) Co., Ltd."
 E8:97:9A,"QuectelW Quectel Wireless Solutions Co.,Ltd."
+E8:97:B8,"ChiunMai Chiun Mai Communication System, Inc"
 E8:98:6D,PaloAlto Palo Alto Networks
 E8:98:C2,ZETLAB ZETLAB Company
 E8:99:5A,"PiiGABPr PiiGAB, Processinformation i Goteborg AB"
 E8:99:C4,HTC HTC Corporation
 E8:9A:8F,QuantaCo Quanta Computer Inc.
 E8:9A:FF,"FujianLA Fujian LANDI Commercial Equipment Co.,Ltd"
+E8:9C:25,ASUSTekC ASUSTek COMPUTER INC.
 E8:9D:87,Toshiba
 E8:9E:0C,Max8UsaD Max8Usa Distributors Inc.
 E8:9E:B4,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 E8:9F:39,Nokia
 E8:9F:6D,Espressi Espressif Inc.
 E8:9F:80,BelkinIn Belkin International Inc.
 E8:9F:EC,"ChengduK Chengdu Kt Electronic Hi-Tech Co.,Ltd"
@@ -45158,15 +46779,17 @@
 E8:D0:FA,MKSInstr MKS Instruments Deutschland GmbH
 E8:D0:FC,LiteonTe Liteon Technology Corporation
 E8:D1:1B,AskeyCom Askey Computer Corp
 E8:D2:FF,Sagemcom Sagemcom Broadband SAS
 E8:D3:22,"Cisco Cisco Systems, Inc"
 E8:D4:83,ULTIMATE ULTIMATE Europe Transportation Equipment GmbH
 E8:D4:E0,"BeijingB Beijing BenyWave Technology Co., Ltd."
+E8:D5:2B,"Google Google, Inc."
 E8:D7:65,"HuaweiTe Huawei Technologies Co.,Ltd"
+E8:D7:75,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:D8:19,AzureWav AzureWave Technology Inc.
 E8:D8:7E,AmazonTe Amazon Technologies Inc.
 E8:D8:D1,HP HP Inc.
 E8:DA:00,"KivoTech Kivo Technology, Inc."
 E8:DA:20,"Nintendo Nintendo Co.,Ltd"
 E8:DA:96,"ZhuhaiTi Zhuhai Tianrui Electrical Power Tech. Co., Ltd."
 E8:DA:AA,VideoHom VideoHome Technology Corp.
@@ -45175,14 +46798,15 @@
 E8:DE:00,"ChongQin ChongQing GuanFang Technology Co.,LTD"
 E8:DE:27,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 E8:DE:8E,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
 E8:DE:D6,"Intrisin Intrising Networks, Inc."
 E8:DE:FB,MesoticS Mesotic Sas
 E8:DF:70,AVMAudio AVM Audiovisuelles Marketing und Computersysteme GmbH
 E8:DF:F2,"PRF PRF Co., Ltd."
+E8:E0:7E,SiliconL Silicon Laboratories
 E8:E0:8F,Gravotec Gravotech Marking Sas
 E8:E0:B7,Toshiba
 E8:E1:E1,"GemtekTe Gemtek Technology Co., Ltd."
 E8:E1:E2,Energote Energotest
 E8:E5:D6,"SamsungE Samsung Electronics Co.,Ltd"
 E8:E7:32,Alcatel- Alcatel-Lucent Enterprise
 E8:E7:70,"Warp9Tec Warp9 Tech Design, Inc."
@@ -45193,14 +46817,15 @@
 E8:EA:4D,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:EA:6A,StarTech StarTech.com
 E8:EA:DA,DenkoviA Denkovi Assembly Electronics LTD
 E8:EB:11,TexasIns Texas Instruments
 E8:EB:1B,Microchi Microchip Technology Inc.
 E8:EB:34,"Cisco Cisco Systems, Inc"
 E8:EB:D3,"Mellanox Mellanox Technologies, Inc."
+E8:EB:DD,"Guangzho Guangzhou Qingying Acoustics Technology Co., Ltd"
 E8:EC:A3,Dongguan Dongguan Liesheng Electronic Co.Ltd
 E8:ED:05,"ARRISGro ARRIS Group, Inc."
 E8:ED:D6,"Fortinet Fortinet, Inc."
 E8:ED:F3,"Cisco Cisco Systems, Inc"
 E8:EE:CC,Fantasia Fantasia Trading LLC
 E8:EF:05,MindTech Mind Tech International Limited
 E8:EF:22,"SiemensN Siemens Numerical Control Ltd., Nanjing"
@@ -45210,14 +46835,15 @@
 E8:F2:E2,LGInnote LG Innotek
 E8:F2:E3,"StarcorB Starcor Beijing Co.,Limited"
 E8:F3:75,Nokia
 E8:F4:08,IntelCor Intel Corporate
 E8:F6:54,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:F7:24,HewlettP Hewlett Packard Enterprise
 E8:F7:91,XiaomiCo Xiaomi Communications Co Ltd
+E8:F8:D0,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 E8:F9:28,Rftech Rftech Srl
 E8:F9:D4,"HuaweiTe Huawei Technologies Co.,Ltd"
 E8:FA:23,"HuaweiDe Huawei Device Co., Ltd."
 E8:FA:F7,"Guangdon Guangdong Uniteddata Holding Group Co., Ltd."
 E8:FB:1C,AzureWav AzureWave Technology Inc.
 E8:FB:E9,"Apple Apple, Inc."
 E8:FC:60,ELCOMInn ELCOM Innovations Private Limited
@@ -45244,14 +46870,15 @@
 EC:01:E2,FoxconnI Foxconn Interconnect Technology
 EC:01:EE,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 EC:02:73,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 EC:04:41,"ShenZhen ShenZhen TIGO Semiconductor Co., Ltd."
 EC:08:6B,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 EC:08:E5,"Motorola Motorola Mobility LLC, a Lenovo Company"
 EC:0B:AE,"Hangzhou Hangzhou BroadLink Technology Co.,Ltd"
+EC:0C:96,Nokia
 EC:0D:9A,"Mellanox Mellanox Technologies, Inc."
 EC:0D:E4,AmazonTe Amazon Technologies Inc.
 EC:0E:C4,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 EC:0E:D6,ItechIns Itech Instruments Sas
 EC:10:00,"EnanceSo Enance Source Co., Ltd."
 EC:10:7B,"SamsungE Samsung Electronics Co.,Ltd"
 EC:11:20,FloDesig FloDesign Wind Turbine Corporation
@@ -45267,14 +46894,15 @@
 EC:1B:BD,SiliconL Silicon Laboratories
 EC:1C:5D,Siemens Siemens AG
 EC:1D:7F,zte zte corporation
 EC:1D:8B,"Cisco Cisco Systems, Inc"
 EC:1D:9E,"QuectelW Quectel Wireless Solutions Co.,Ltd."
 EC:1F:72,SamsungE Samsung Electro-Mechanics(Thailand)
 EC:21:25,Toshiba Toshiba Corp.
+EC:21:50,"vivoMobi vivo Mobile Communication Co., Ltd."
 EC:21:9F,VidaBox VidaBox LLC
 EC:21:E5,Toshiba
 EC:22:57,"JiangSuN JiangSu NanJing University Electronic Information Technology Co.,Ltd"
 EC:22:80,D-LinkIn D-Link International
 EC:23:3D,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:23:68,"IntelliV IntelliVoice Co.,Ltd."
 EC:23:7B,zte zte corporation
@@ -45283,15 +46911,16 @@
 EC:26:CA,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 EC:26:FB,"Tecc Tecc Co.,Ltd."
 EC:28:D3,"Apple Apple, Inc."
 EC:2A:72,Dell Dell Inc.
 EC:2A:F0,Ypsomed Ypsomed AG
 EC:2B:EB,AmazonTe Amazon Technologies Inc.
 EC:2C:11,CwdInnov Cwd Innovation Limited
-EC:2C:49,Universi University of Tokyo
+EC:2C:49,"NakaoLab NakaoLab, The University of Tokyo"
+EC:2C:73,"Apple Apple, Inc."
 EC:2C:E2,"Apple Apple, Inc."
 EC:2E:4E,Hitachi- Hitachi-Lg Data Storage Inc
 EC:2E:98,AzureWav AzureWave Technology Inc.
 EC:30:91,"Cisco Cisco Systems, Inc"
 EC:30:B3,XiaomiCo Xiaomi Communications Co Ltd
 EC:31:6D,Hansgroh Hansgrohe
 EC:35:4D,"Wingtech Wingtech Mobile Communications Co.,Ltd"
@@ -45306,14 +46935,15 @@
 EC:3C:BB,"HuaweiDe Huawei Device Co., Ltd."
 EC:3D:FD,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 EC:3E:09,"Performa Performance Designed Products, Llc"
 EC:3E:B3,ZyxelCom Zyxel Communications Corporation
 EC:3E:F7,JuniperN Juniper Networks
 EC:3F:05,"Institut Institute 706, The Second Academy China Aerospace Science & Industry Corp"
 EC:41:18,"XIAOMIEl XIAOMI Electronics,CO.,LTD"
+EC:41:CA,"Shenzhen Shenzhen TecAnswer Technology co.,ltd"
 EC:42:69,HMDGloba HMD Global Oy
 EC:42:B4,ADC ADC Corporation
 EC:42:CC,"Apple Apple, Inc."
 EC:42:F0,"ADLEmbed ADL Embedded Solutions, Inc."
 EC:43:8B,Yaptv
 EC:43:E6,AWCER AWCER Ltd.
 EC:43:F6,ZyxelCom Zyxel Communications Corporation
@@ -45325,14 +46955,15 @@
 EC:4C:4D,NPKRoTeK ZAO NPK RoTeK
 EC:4D:3E,"BeijingX Beijing Xiaomi Mobile Software Co., Ltd"
 EC:4D:47,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:4F:82,Calix Calix Inc.
 EC:50:AA,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 EC:51:BC,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 EC:52:DC,WORLDMED WORLD MEDIA AND TECHNOLOGY Corp.
+EC:53:82,"HonorDev Honor Device Co., Ltd."
 EC:54:2E,Shanghai Shanghai XiMei Electronic Technology Co. Ltd
 EC:55:1C,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:55:F9,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 EC:56:23,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:57:0D,AFE AFE Inc.
 EC:58:EA,RuckusWi Ruckus Wireless
 EC:59:E7,Microsof Microsoft Corporation
@@ -45350,14 +46981,15 @@
 EC:63:E5,ePBoardD ePBoard Design LLC
 EC:63:ED,HyundaiA Hyundai Autoever Corp.
 EC:64:88,"HonorDev Honor Device Co., Ltd."
 EC:64:E7,MOCACARE MOCACARE Corporation
 EC:65:6E,ThingsIn The Things Industries B.V.
 EC:65:CC,Panasoni Panasonic Automotive Systems Company of America
 EC:66:D1,B&WGroup B&W Group LTD
+EC:67:94,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 EC:68:81,PaloAlto Palo Alto Networks
 EC:6C:9A,Arcadyan Arcadyan Corporation
 EC:6C:9F,"ChengduV Chengdu Volans Technology CO.,LTD"
 EC:6C:B5,zte zte corporation
 EC:6F:0B,"FADU FADU, Inc."
 EC:70:97,"ARRISGro ARRIS Group, Inc."
 EC:71:DB,ReolinkI Reolink Innovation Limited
@@ -45374,39 +47006,41 @@
 EC:7C:74,"JustoneT Justone Technologies Co., Ltd."
 EC:7C:B6,"SamsungE Samsung Electronics Co.,Ltd"
 EC:7D:11,"vivoMobi vivo Mobile Communication Co., Ltd."
 EC:7D:9D,Cpi
 EC:7E:91,ItelMobi Itel Mobile Limited
 EC:7F:C6,EccelSas Eccel Corporation Sas
 EC:80:09,NovaSpar NovaSparks
+EC:81:50,"Apple Apple, Inc."
 EC:81:93,"Logitech Logitech, Inc"
 EC:81:9C,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:82:63,zte zte corporation
 EC:83:50,Microsof Microsoft Corporation
 EC:83:6C,"RMTech RM Tech Co., Ltd."
 EC:83:B7,PuwellCl Puwell Cloud Tech Limited
 EC:83:D5,GIRD GIRD Systems Inc
 EC:84:B4,CigShang Cig Shanghai Co Ltd
 EC:85:2F,"Apple Apple, Inc."
 EC:88:8F,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 EC:88:92,"Motorola Motorola Mobility LLC, a Lenovo Company"
 EC:89:14,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:89:F5,LenovoMo Lenovo Mobile Communication Technology Ltd.
+EC:8A:48,AristaNe Arista Networks
 EC:8A:4C,zte zte corporation
 EC:8A:C4,AmazonTe Amazon Technologies Inc.
 EC:8A:C7,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 EC:8C:9A,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:8C:A2,RuckusWi Ruckus Wireless
 EC:8E:AD,Dlx
 EC:8E:AE,Nagravis Nagravision SA
 EC:8E:B5,HewlettP Hewlett Packard
 EC:92:33,EddyfiND Eddyfi NDT Inc
 EC:93:27,MEMMERT+ MEMMERT GmbH + Co. KG
 EC:93:65,"Mapperai Mapper.ai, Inc."
-EC:93:7D,Technico Technicolor CH USA Inc.
+EC:93:7D,VantivaU Vantiva USA LLC
 EC:93:ED,DDoS-Gua DDoS-Guard LTD
 EC:94:68,MetaSyst Meta System Spa
 EC:94:CB,Espressi Espressif Inc.
 EC:94:D5,JuniperN Juniper Networks
 EC:96:81,2276427O 2276427 Ontario Inc
 EC:96:BF,eSystems eSystems MTG GmbH
 EC:97:B2,"SUMECMac SUMEC Machinery & Electric Co.,Ltd."
@@ -45435,27 +47069,30 @@
 EC:9F:0D:B0:00:00/28,"CrrcQing Crrc Qingdao Sifang Rolling Stock Research Institute Co.,Ltd"
 EC:9F:0D:C0:00:00/28,Sarcos Sarcos Corp
 EC:9F:0D:D0:00:00/28,SKSContr SKS Control Oy
 EC:9F:0D:E0:00:00/28,MAXTechn MAX Technologies
 EC:A1:38,AmazonTe Amazon Technologies Inc.
 EC:A1:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:A2:9B,Kemppi Kemppi Oy
+EC:A2:A0,TaicangT Taicang T&W Electronics
 EC:A5:DE,ONYXWIFI ONYX WIFI Inc
 EC:A6:2F,"HuaweiTe Huawei Technologies Co.,Ltd"
-EC:A8:1F,Technico Technicolor CH USA Inc.
+EC:A7:AD,"BarrotTe Barrot Technology Co.,Ltd."
+EC:A8:1F,VantivaU Vantiva USA LLC
 EC:A8:6B,"Elitegro Elitegroup Computer Systems Co.,Ltd."
 EC:A9:07,"Apple Apple, Inc."
 EC:A9:40,"ARRISGro ARRIS Group, Inc."
 EC:A9:FA,"Guangdon Guangdong Genius Technology Co., Ltd."
 EC:AA:25,"SamsungE Samsung Electronics Co.,Ltd"
 EC:AA:8F,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:AA:A0,Pegatron Pegatron Corporation
 EC:AD:B8,"Apple Apple, Inc."
 EC:AD:E0,D-LinkIn D-Link International
 EC:AF:97,Git
+EC:AF:F9,HailoTec Hailo Technologies Ltd.
 EC:B0:E1,Ciena Ciena Corporation
 EC:B1:06,"AcuroNet Acuro Networks, Inc"
 EC:B1:D7,HewlettP Hewlett Packard
 EC:B3:13,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 EC:B4:E8,WistronM Wistron Mexico SA de CV
 EC:B5:41,SHINANOE SHINANO E and E Co.Ltd.
 EC:B5:FA,PhilipsL Philips Lighting BV
@@ -45464,14 +47101,15 @@
 EC:B9:70,"RuijieNe Ruijie Networks Co.,LTD"
 EC:BA:FE,Giroptic
 EC:BB:AE,Digivoic Digivoice Tecnologia em Eletronica Ltda
 EC:BD:09,FUSIONEl FUSION Electronics Ltd
 EC:BD:1D,"Cisco Cisco Systems, Inc"
 EC:BE:5F,VestelEl Vestel Elektronik San ve Tic. A.S.
 EC:BE:DD,Sagemcom Sagemcom Broadband SAS
+EC:C0:18,"Cisco Cisco Systems, Inc"
 EC:C0:1B,"HuaweiTe Huawei Technologies Co.,Ltd"
 EC:C0:6A,PowerCho PowerChord Group Limited
 EC:C0:7A,LairdCon Laird Connectivity
 EC:C1:AB,Guangzho Guangzhou Shiyuan Electronic Technology Company Limited
 EC:C3:02,"HUMAX HUMAX Co., Ltd."
 EC:C3:8A,Accuener Accuenergy (CANADA) Inc
 EC:C3:B0,zte zte corporation
@@ -45509,15 +47147,17 @@
 EC:E7:44,Omntecmf Omntec mfg. inc
 EC:E7:A7,IntelCor Intel Corporate
 EC:E9:0B,SistemaS Sistema Solucoes Eletronicas Ltda - Easytech
 EC:E9:15,STI STI Ltd
 EC:E9:F8,"GuangZho Guang Zhou TRI-SUN Electronics Technology Co., Ltd"
 EC:EA:03,DarfonLi Darfon Lighting Corp
 EC:EB:B8,HewlettP Hewlett Packard Enterprise
+EC:ED:73,"Motorola Motorola Mobility LLC, a Lenovo Company"
 EC:EE:D8,"ZTLXNetw ZTLX Network Technology Co.,Ltd"
+EC:EF:17,"SunplusT Sunplus Technology Co., Ltd."
 EC:F0:0E,AboCom
 EC:F0:FE,zte zte corporation
 EC:F2:2B,TecnoMob Tecno Mobile Limited
 EC:F2:36,Neomonta Neomontana Electronics
 EC:F3:42,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 EC:F3:5B,Nokia Nokia Corporation
 EC:F4:0C,"Cisco Cisco Systems, Inc"
@@ -45561,14 +47201,16 @@
 F0:1C:13,LGElectr LG Electronics (Mobile Communications)
 F0:1C:2D,JuniperN Juniper Networks
 F0:1D:2D,"Cisco Cisco Systems, Inc"
 F0:1D:BC,Microsof Microsoft Corporation
 F0:1E:34,"ORICOTec ORICO Technologies Co., Ltd"
 F0:1F:AF,Dell Dell Inc.
 F0:1F:C7,"Apple Apple, Inc."
+F0:20:FF,IntelCor Intel Corporate
+F0:21:78,"Unionman Unionman Technology Co.,Ltd"
 F0:21:9D,Cal-Comp Cal-Comp Electronics & Communications Company Ltd.
 F0:21:E0,eero eero inc.
 F0:22:1D,IEEERegi IEEE Registration Authority
 F0:22:1D:00:00:00/28,Thanhbin Thanhbinh Company - E111 Factory
 F0:22:1D:10:00:00/28,DrEberlM Dr. Eberl MBE Komponenten GmbH
 F0:22:1D:20:00:00/28,"ChonelIn Chonel Industry?shanghai?Co., Ltd."
 F0:22:1D:30:00:00/28,ShenZhen ShenZhen Shizao Electronic Technology
@@ -45722,25 +47364,27 @@
 F0:6E:32,Microtel Microtel Innovation S.R.L.
 F0:6F:46,Ubiik
 F0:70:4F,"SamsungE Samsung Electronics Co.,Ltd"
 F0:72:8C,"SamsungE Samsung Electronics Co.,Ltd"
 F0:72:EA,"Google Google, Inc."
 F0:73:AE,PEAK-Sys PEAK-System Technik
 F0:74:85,"NGD NGD Systems, Inc."
+F0:74:8D,"RuijieNe Ruijie Networks Co.,LTD"
 F0:74:E4,"Thunderc Thundercomm Technology Co., Ltd"
 F0:76:1C,"CompalIn Compal Information (Kunshan) Co., Ltd."
 F0:76:6F,"Apple Apple, Inc."
 F0:77:65,"Sourcefi Sourcefire, Inc"
 F0:77:C3,IntelCor Intel Corporate
 F0:77:D0,Xcellen
 F0:78:07,"Apple Apple, Inc."
 F0:78:16,"Cisco Cisco Systems, Inc"
 F0:79:59,ASUSTekC ASUSTek COMPUTER INC.
 F0:79:60,"Apple Apple, Inc."
 F0:79:E8,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
+F0:7B:65,Sagemcom Sagemcom Broadband SAS
 F0:7B:CB,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 F0:7C:C7,JuniperN Juniper Networks
 F0:7D:68,D-Link D-Link Corporation
 F0:7F:06,"Cisco Cisco Systems, Inc"
 F0:7F:0C,LeopoldK Leopold Kostal GmbH &Co. KG
 F0:81:73,AmazonTe Amazon Technologies Inc.
 F0:81:75,Sagemcom Sagemcom Broadband SAS
@@ -45754,14 +47398,15 @@
 F0:87:56,ZyxelCom Zyxel Communications Corporation
 F0:87:7F,"Magnetar Magnetar Technology Shenzhen Co., LTD."
 F0:8A:28,"JIANGSUH JIANGSU HENGSION ELECTRONIC S and T CO.,LTD"
 F0:8A:76,"SamsungE Samsung Electronics Co.,Ltd"
 F0:8B:FE,"Costel Costel.,Co.Ltd"
 F0:8C:FB,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 F0:8E:DB,VeloClou VeloCloud Networks
+F0:90:08,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 F0:92:1C,HewlettP Hewlett Packard
 F0:92:B4,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 F0:93:3A,NxtConec NxtConect
 F0:93:C5,GarlandT Garland Technology
 F0:95:F1,CarlZeis Carl Zeiss AG
 F0:97:E5,"Tamio Tamio, Inc"
 F0:98:38,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -45772,16 +47417,17 @@
 F0:9A:51,Shanghai Shanghai Viroyal Electronic Technology Company Limited
 F0:9B:B8,"HuaweiTe Huawei Technologies Co.,Ltd"
 F0:9C:BB,RaonThin RaonThink Inc.
 F0:9C:D7,"Guangzho Guangzhou Blue Cheetah Intelligent Technology Co., Ltd."
 F0:9C:E9,"ExtremeN Extreme Networks, Inc."
 F0:9E:4A,IntelCor Intel Corporate
 F0:9E:63,"Cisco Cisco Systems, Inc"
-F0:9F:C2,Ubiquiti Ubiquiti Networks Inc.
+F0:9F:C2,Ubiquiti Ubiquiti Inc
 F0:9F:FC,SHARP SHARP Corporation
+F0:A0:B1,"HuaweiTe Huawei Technologies Co.,Ltd"
 F0:A2:25,AmazonTe Amazon Technologies Inc.
 F0:A3:5A,"Apple Apple, Inc."
 F0:A3:B2,"HuiZhouG Hui Zhou Gaoshengda Technology Co.,LTD"
 F0:A6:54,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 F0:A7:64,"GST GST Co., Ltd."
 F0:A7:B2,Futaba Futaba Corporation
 F0:A9:51,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -45840,14 +47486,15 @@
 F0:C1:CE,"GoodWeTe GoodWe Technologies CO., Ltd"
 F0:C1:F1,"Apple Apple, Inc."
 F0:C2:4C,"Zhejiang Zhejiang FeiYue Digital Technology Co., Ltd"
 F0:C2:7C,"Mianyang Mianyang Netop Telecom Equipment Co.,Ltd."
 F0:C3:71,"Apple Apple, Inc."
 F0:C4:2F,"HuaweiDe Huawei Device Co., Ltd."
 F0:C4:78,"HuaweiTe Huawei Technologies Co.,Ltd"
+F0:C5:58,UDElectr U.D.Electronic Corp.
 F0:C7:25,"Apple Apple, Inc."
 F0:C7:45,TecnoMob Tecno Mobile Limited
 F0:C7:7F,TexasIns Texas Instruments
 F0:C8:14,Shenzhen Shenzhen Bilian Electronic Co.，Ltd
 F0:C8:50,"HuaweiTe Huawei Technologies Co.,Ltd"
 F0:C8:8C,LeddarTe LeddarTech Inc.
 F0:C8:B5,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -45856,14 +47503,15 @@
 F0:CC:E0,"Shenzhen Shenzhen All-Smartlink Technology Co.,Ltd."
 F0:CD:31,"SamsungE Samsung Electronics Co.,Ltd"
 F0:D0:8C,TCTmobil TCT mobile ltd
 F0:D1:4F,Linear Linear Llc
 F0:D1:A9,"Apple Apple, Inc."
 F0:D1:B8,Ledvance
 F0:D2:F1,AmazonTe Amazon Technologies Inc.
+F0:D3:1F,"Apple Apple, Inc."
 F0:D3:A7,"CobaltRa CobaltRay Co., Ltd"
 F0:D3:E7,Sensomet Sensometrix SA
 F0:D4:15,IntelCor Intel Corporate
 F0:D4:E2,Dell Dell Inc.
 F0:D4:F6,LarsThra Lars Thrane A/S
 F0:D4:F7,varramsy varram system
 F0:D5:BF,IntelCor Intel Corporate
@@ -45903,14 +47551,15 @@
 F0:E7:7E,"SamsungE Samsung Electronics Co.,Ltd"
 F0:EB:D0,"Shanghai Shanghai Feixun Communication Co.,Ltd."
 F0:EC:39,Essec
 F0:ED:1E,BilkonBi Bilkon Bilgisayar Kontrollu Cih. Im.Ltd.
 F0:ED:B8,Serverco Servercom (India) Private Limited
 F0:EE:10,"SamsungE Samsung Electronics Co.,Ltd"
 F0:EE:58,PACETele PACE Telematics GmbH
+F0:EE:7A,"Apple Apple, Inc."
 F0:EE:BB,VIPAR VIPAR GmbH
 F0:EF:86,"Google Google, Inc."
 F0:EF:D2,"TfPaymen Tf Payment Service Co., Ltd"
 F0:F0:02,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 F0:F0:8F,NextekSo Nextek Solutions Pte Ltd
 F0:F0:A4,AmazonTe Amazon Technologies Inc.
 F0:F2:49,HitronTe Hitron Technologies. Inc
@@ -45930,14 +47579,15 @@
 F0:F8:F2,TexasIns Texas Instruments
 F0:F9:F7,IES IES GmbH & Co. KG
 F0:FA:C7,"HuaweiDe Huawei Device Co., Ltd."
 F0:FC:C8,"ARRISGro ARRIS Group, Inc."
 F0:FD:A0,AcurixNe Acurix Networks Pty Ltd
 F0:FE:6B,"Shanghai Shanghai High-Flying Electronics Technology Co., Ltd"
 F0:FE:E7,"HuaweiDe Huawei Device Co., Ltd."
+F4:00:46,ONSemico ON Semiconductor
 F4:02:23,PAXCompu PAX Computer Technology(Shenzhen) Ltd.
 F4:02:28,SamsungE Samsung Electro-Mechanics(Thailand)
 F4:02:70,Dell Dell Inc.
 F4:03:04,"Google Google, Inc."
 F4:03:21,BeNeXt BeNeXt B.V.
 F4:03:2A,AmazonTe Amazon Technologies Inc.
 F4:03:2F,Reduxio Reduxio Systems
@@ -45971,14 +47621,15 @@
 F4:0E:11:E0:00:00/28,Elektron Elektronika Naglic d.o.o.
 F4:0E:11:F0:00:00/28,Private
 F4:0E:22,"SamsungE Samsung Electronics Co.,Ltd"
 F4:0E:83,"ARRISGro ARRIS Group, Inc."
 F4:0F:1B,"Cisco Cisco Systems, Inc"
 F4:0F:24,"Apple Apple, Inc."
 F4:0F:9B,Wavelink
+F4:12:DA,zte zte corporation
 F4:12:FA,Espressi Espressif Inc.
 F4:13:99,"Aerospac Aerospace new generation communications Co.,Ltd"
 F4:15:32,"PETAiONa PETAiO (NanJing), Inc."
 F4:15:35,"SPONComm SPON Communication Technology Co.,Ltd"
 F4:15:63,"F5Networ F5 Networks, Inc."
 F4:15:FD,"Shanghai Shanghai Pateo Electronic Equipment Manufacturing Co., Ltd."
 F4:17:B8,AirTiesW AirTies Wireless Networks
@@ -45995,38 +47646,44 @@
 F4:1F:88,zte zte corporation
 F4:1F:C2,"Cisco Cisco Systems, Inc"
 F4:20:12,Cucinial Cuciniale GmbH
 F4:21:AE,Shanghai Shanghai Xiaodu Technology Limited
 F4:21:CA,"Apple Apple, Inc."
 F4:22:7A,"Guangdon Guangdong Seneasy Intelligent Technology Co., Ltd."
 F4:23:9C,SernetSu Sernet (Suzhou) Technologies Corporation
+F4:24:62,"SelcomEl Selcom Electronics (Shanghai) Co., Ltd"
 F4:26:79,IntelCor Intel Corporate
+F4:27:56,DASANNew DASAN Newtork Solutions
 F4:28:33,MMPC MMPC Inc.
 F4:28:53,ZioncomE Zioncom Electronics (Shenzhen) Ltd.
 F4:28:96,SpectoPa Specto Paineis Eletronicos Ltda
 F4:29:81,"vivoMobi vivo Mobile Communication Co., Ltd."
 F4:2A:7D,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 F4:2B:48,Ubiqam
 F4:2B:7D,"Chipsgui Chipsguide technology CO.,LTD."
+F4:2B:8C,"SamsungE Samsung Electronics Co.,Ltd"
 F4:2C:56,SenorTec Senor Tech Co Ltd
 F4:2D:06,zte zte corporation
+F4:2E:48,zte zte corporation
 F4:2E:7F,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 F4:30:8B,XiaomiCo Xiaomi Communications Co Ltd
 F4:30:B9,HewlettP Hewlett Packard
 F4:31:C3,"Apple Apple, Inc."
 F4:32:3D,"Sichuant Sichuan tianyi kanghe communications co., LTD"
 F4:33:1C,"Toast Toast, Inc."
 F4:33:28,CIMCONLi CIMCON Lighting Inc.
 F4:34:F0,"Apple Apple, Inc."
 F4:36:E1,Abilis Abilis Systems SARL
 F4:37:B7,"Apple Apple, Inc."
 F4:38:14,"Shanghai Shanghai Howell Electronic Co.,Ltd"
 F4:38:C1,"HuaweiDe Huawei Device Co., Ltd."
 F4:39:09,HewlettP Hewlett Packard
+F4:3A:7B,zte zte corporation
 F4:3B:D8,IntelCor Intel Corporate
+F4:3C:3B,HunanFn- Hunan Fn-Link Technology Limited
 F4:3D:80,FAGIndus FAG Industrial Services GmbH
 F4:3E:61,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 F4:3E:66,BeeCompu Bee Computing (HK) Limited
 F4:3E:9D,"BenuNetw Benu Networks, Inc."
 F4:41:56,Arrikto Arrikto Inc.
 F4:41:9E,"HuaweiDe Huawei Device Co., Ltd."
 F4:42:27,SSResear S & S Research Inc.
@@ -46072,27 +47729,29 @@
 F4:60:77,TexasIns Texas Instruments
 F4:60:E2,XiaomiCo Xiaomi Communications Co Ltd
 F4:62:D0,"NotforRa Not for Radio, LLC"
 F4:63:1F,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:63:49,Diffon Diffon Corporation
 F4:63:E7,"NanjingM Nanjing Maxon O.E. Tech. Co., LTD"
 F4:63:FC,"vivoMobi vivo Mobile Communication Co., Ltd."
+F4:64:12,SonyInte Sony Interactive Entertainment Inc.
 F4:64:5D,Toshiba
 F4:65:A6,"Apple Apple, Inc."
 F4:67:2D,ShenZhen ShenZhen Topstar Technology Company
 F4:69:42,AskeyCom Askey Computer Corp
 F4:69:D5,IEEERegi IEEE Registration Authority
 F4:69:D5:00:00:00/28,Mossman Mossman Limited
 F4:69:D5:10:00:00/28,"Junchuan Junchuang (Xiamen) Automation Technology Co.,Ltd"
 F4:69:D5:20:00:00/28,PulsarEn Pulsar Engineering srl
 F4:69:D5:30:00:00/28,"ITS ITS Co., Ltd."
 F4:69:D5:40:00:00/28,StypeCSd Stype CS d.o.o.
 F4:69:D5:50:00:00/28,"HefeiSTA Hefei STAROT Technology Co.,Ltd"
 F4:69:D5:60:00:00/28,"TianJinK TianJin KCHT Information Technology Co., Ltd."
 F4:69:D5:70:00:00/28,"Rosco Rosco, Inc"
+F4:69:D5:80:00:00/28,WiFiNati WiFi Nation Ltd
 F4:69:D5:90:00:00/28,"Terminus Terminus (Shanghai) Technology Co.,Ltd."
 F4:69:D5:A0:00:00/28,"ShenZhen ShenZhenShi EVADA technology Co.,Ltd"
 F4:69:D5:B0:00:00/28,Konntek Konntek Inc
 F4:69:D5:C0:00:00/28,"HuaqinTe Huaqin Telecom Technology Co.,Ltd."
 F4:69:D5:D0:00:00/28,"NantongZ Nantong ZYDZ Electronic.,Co.Ltd"
 F4:69:D5:E0:00:00/28,"ORtekTec ORtek Technology, Inc."
 F4:6A:92,"Shenzhen Shenzhen Fast Technologies Co.,Ltd"
@@ -46169,28 +47828,30 @@
 F4:90:CB:A0:00:00/28,Fend Fend Incorporated
 F4:90:CB:B0:00:00/28,A-dec A-dec Inc.
 F4:90:CB:C0:00:00/28,CheetahM Cheetah Medical
 F4:90:CB:D0:00:00/28,Simavita Simavita (Aust) Pty Ltd
 F4:90:CB:E0:00:00/28,RSAELabs RSAE Labs Inc
 F4:90:EA,Deciso Deciso B.V.
 F4:91:1E,ZhuhaiEw Zhuhai Ewpe Information Technology Inc
-F4:92:BF,Ubiquiti Ubiquiti Networks Inc.
+F4:92:BF,Ubiquiti Ubiquiti Inc
 F4:93:1C,"Universa Universal Electronics, Inc."
 F4:93:9F,"HonHaiPr Hon Hai Precision Industry Co., Ltd."
 F4:94:61,NexGenSt NexGen Storage
 F4:94:66,"CountMax CountMax, ltd"
 F4:95:1B,"HefeiRad Hefei Radio Communication Technology Co., Ltd"
 F4:96:34,IntelCor Intel Corporate
 F4:96:51,NAKAYO NAKAYO Inc
 F4:97:C2,Nebulon Nebulon Inc
 F4:99:AC,WEBERSch WEBER Schraubautomaten GmbH
 F4:9C:12,Structab Structab AB
+F4:9D:A7,Private
 F4:9E:EF,TaicangT Taicang T&W Electronics
 F4:9F:54,"SamsungE Samsung Electronics Co.,Ltd"
 F4:9F:F3,"HuaweiTe Huawei Technologies Co.,Ltd"
+F4:A1:7F,Marquard Marquardt Electronics Technology (Shanghai) Co.Ltd
 F4:A2:94,"EagleWor Eagle World Development Co., Limited"
 F4:A4:54,IEEERegi IEEE Registration Authority
 F4:A4:54:00:00:00/28,NKTPhoto NKT Photonics A/S
 F4:A4:54:10:00:00/28,PTTelkom PT Telkom Indonesia
 F4:A4:54:20:00:00/28,TriWorks Tri Works
 F4:A4:54:30:00:00/28,"Chongqin Chongqing Hengxun Liansheng Industrial Co.,Ltd"
 F4:A4:54:40:00:00/28,Earshots
@@ -46207,28 +47868,30 @@
 F4:A4:75,IntelCor Intel Corporate
 F4:A4:D6,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:A5:2A,HawaTech Hawa Technologies Inc
 F4:A5:9D,"HuaweiDe Huawei Device Co., Ltd."
 F4:A7:39,JuniperN Juniper Networks
 F4:A8:0D,"WistronI Wistron InfoComm(Kunshan)Co.,Ltd."
 F4:A9:97,Canon Canon Inc.
+F4:AA:D0,Ohsung
 F4:AC:C1,"Cisco Cisco Systems, Inc"
 F4:AF:E7,"Apple Apple, Inc."
 F4:B1:64,Lightnin Lightning Telecommunications Technology Co. Ltd
 F4:B1:9C,AltoBeam AltoBeam (China) Inc.
 F4:B1:C2,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 F4:B3:01,IntelCor Intel Corporate
 F4:B3:81,WindowMa WindowMaster A/S
 F4:B3:B1,SiliconL Silicon Laboratories
 F4:B5:20,BiostarM Biostar Microtech international corp.
 F4:B5:2F,JuniperN Juniper Networks
 F4:B5:49,"XiamenYe Xiamen Yeastar Information Technology Co., Ltd."
 F4:B5:AA,zte zte corporation
 F4:B5:BB,CeragonN Ceragon Networks
 F4:B6:88,"Plantron Plantronics, Inc."
+F4:B6:C6,IndraHee Indra Heera Technology LLP
 F4:B6:E5,"TerraSem TerraSem Co.,Ltd"
 F4:B7:2A,TimeInte Time Interconnect Ltd
 F4:B7:8D,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:B7:B3,"vivoMobi vivo Mobile Communication Co., Ltd."
 F4:B7:E2,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 F4:B8:5E,TexasIns Texas Instruments
 F4:B8:98,TexasIns Texas Instruments
@@ -46237,59 +47900,62 @@
 F4:BC:97,"Shenzhen Shenzhen Crave Communication Co., LTD"
 F4:BC:DA,"Shenzhen Shenzhen Jingxun Software Telecommunication Technology Co.,Ltd"
 F4:BD:7C,"Chengduj Chengdu jinshi communication Co., LTD"
 F4:BD:9E,"Cisco Cisco Systems, Inc"
 F4:BE:EC,"Apple Apple, Inc."
 F4:BF:80,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:BF:A8,JuniperN Juniper Networks
+F4:BF:BB,"ChinaMob China Mobile Group Device Co.,Ltd."
 F4:C0:2F,BlueBite
-F4:C1:14,Technico Technicolor CH USA Inc.
+F4:C1:14,VantivaU Vantiva USA LLC
 F4:C2:48,"SamsungE Samsung Electronics Co.,Ltd"
 F4:C4:47,CoagentI Coagent International Enterprise Limited
 F4:C4:D6,"Shenzhen Shenzhen Xinfa Electronic Co.,ltd"
 F4:C6:13,"Alcatel- Alcatel-Lucent Shanghai Bell Co., Ltd"
 F4:C6:D7,blackned blackned GmbH
 F4:C7:14,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:C7:95,WEYTechn WEY Technology AG
 F4:C7:AA,MarvellS Marvell Semiconductors
 F4:C7:C8,Kelvin Kelvin Inc.
 F4:C8:8A,IntelCor Intel Corporate
 F4:CA:24,"FreeBit FreeBit Co., Ltd."
 F4:CA:E5,FreeboxS Freebox Sas
+F4:CA:E7,Arcadyan Arcadyan Corporation
 F4:CB:52,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:CC:55,JuniperN Juniper Networks
 F4:CD:90,Vispiron Vispiron Rotec GmbH
 F4:CE:23,IntelCor Intel Corporate
 F4:CE:36,NordicSe Nordic Semiconductor ASA
 F4:CE:46,HewlettP Hewlett Packard
 F4:CE:48,"ExtremeN Extreme Networks, Inc."
 F4:CF:A2,Espressi Espressif Inc.
 F4:CF:E2,"Cisco Cisco Systems, Inc"
 F4:D0:32,"YunnanId Yunnan Ideal Information&Technology.,Ltd"
 F4:D1:08,IntelCor Intel Corporate
 F4:D2:61,"SEMOCON SEMOCON Co., Ltd"
 F4:D4:88,"Apple Apple, Inc."
+F4:D5:80,Yamaha Yamaha Corporation
 F4:D6:20,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 F4:D7:B2,"LGSInnov LGS Innovations, LLC"
-F4:D9:C6,"Unionman Unionman Technology Co.,Ltd"
+F4:D9:C6,"UnionMan Union Man Technology Co.,Ltd"
 F4:D9:FB,"SamsungE Samsung Electronics Co.,Ltd"
 F4:DB:E3,"Apple Apple, Inc."
 F4:DB:E6,"Cisco Cisco Systems, Inc"
 F4:DC:41,Youngzon Youngzone Culture (Shanghai) Corp
 F4:DC:4D,"BeijingC Beijing CCD Digital Technology Co., Ltd"
 F4:DC:A5,DawonDns Dawon Dns
 F4:DC:DA,"ZhuhaiJi Zhuhai Jiahe Communication Technology Co., limited"
 F4:DC:F9,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:DD:9E,GoPro
 F4:DE:0C,ESPOD ESPOD Ltd.
 F4:DE:AF,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:E1:1E,TexasIns Texas Instruments
 F4:E1:42,DeltaEle Delta Elektronika BV
 F4:E2:04,CoyoteSy Coyote System
-F4:E2:C6,Ubiquiti Ubiquiti Networks Inc.
+F4:E2:C6,Ubiquiti Ubiquiti Inc
 F4:E3:FB,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:E4:51,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:E4:AD,zte zte corporation
 F4:E4:D7,"FujianSt Fujian Star-Net Communication Co.,Ltd"
 F4:E5:78,"Proizvod LLC Proizvodstvennaya Kompania ""TransService"""
 F4:E5:F2,"HuaweiTe Huawei Technologies Co.,Ltd"
 F4:E6:D7,"SolarPow Solar Power Technologies, Inc."
@@ -46301,14 +47967,15 @@
 F4:EA:B5,"ExtremeN Extreme Networks, Inc."
 F4:EB:38,Sagemcom Sagemcom Broadband SAS
 F4:EB:9F,Ellu2019 Ellu Company 2019 SL
 F4:EC:38,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 F4:ED:5F,Shenzhen Shenzhen Ktc Technology Group
 F4:EE:08,Dell Dell Inc.
 F4:EE:14,"MercuryC Mercury Communication Technologies Co.,Ltd."
+F4:EE:31,"Cisco Cisco Systems, Inc"
 F4:EF:9E,SgsgScie Sgsg Science & Technology Co. Ltd
 F4:F1:5A,"Apple Apple, Inc."
 F4:F1:97,EMTAKE EMTAKE Inc
 F4:F1:9E,WistronI Wistron InforComm (Zhongshan) Corporation
 F4:F1:E1,"Motorola Motorola Mobility LLC, a Lenovo Company"
 F4:F2:6D,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 F4:F3:09,"SamsungE Samsung Electronics Co.,Ltd"
@@ -46356,26 +48023,27 @@
 F8:0B:BE,"ARRISGro ARRIS Group, Inc."
 F8:0B:CB,"Cisco Cisco Systems, Inc"
 F8:0B:D0,"DatangTe Datang Telecom communication terminal (Tianjin) Co., Ltd."
 F8:0C:58,TaicangT Taicang T&W Electronics
 F8:0C:F3,LGElectr LG Electronics (Mobile Communications)
 F8:0D:43,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 F8:0D:60,Canon Canon Inc.
+F8:0D:A9,ZyxelCom Zyxel Communications Corporation
 F8:0D:AC,HP HP Inc.
 F8:0D:EA,ZyCastTe ZyCast Technology Inc.
 F8:0D:F0,zte zte corporation
 F8:0D:F1,Sontex Sontex SA
 F8:0F:41,WistronI Wistron Infocomm (Zhongshan) Corporation
 F8:0F:6F,"Cisco Cisco Systems, Inc"
 F8:0F:84,NaturalS Natural Security SAS
 F8:0F:F9,"Google Google, Inc."
 F8:10:37,"AtopiaLP Atopia Systems, LP"
 F8:10:93,"Apple Apple, Inc."
 F8:13:08,Nokia
-F8:14:FE,"Unionman Unionman Technology Co.,Ltd"
+F8:14:FE,"UnionMan Union Man Technology Co.,Ltd"
 F8:15:47,Avaya Avaya Inc
 F8:16:54,IntelCor Intel Corporate
 F8:18:97,2Wire 2Wire Inc
 F8:1A:2B,"Google Google, Inc."
 F8:1A:67,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 F8:1B:04,ZhongSha Zhong Shan City Richsound Electronic Industrial Ltd
 F8:1C:E5,Telefonb Telefonbau Behnke GmbH
@@ -46404,26 +48072,28 @@
 F8:20:55,GreenInf Green Information System
 F8:20:A9,"HuaweiDe Huawei Device Co., Ltd."
 F8:22:29,"NokiaSha Nokia Shanghai Bell Co., Ltd."
 F8:22:85,"CypressT Cypress Technology CO., LTD."
 F8:23:87,"Shenzhen Shenzhen Horn Audio Co.,Ltd."
 F8:23:B2,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:24:41,Yeelink
+F8:24:DB,"EntryPoi EntryPoint Networks, Inc"
 F8:24:E4,"Beyonics Beyonics Technology Electronic (Changshu) Co., Ltd"
 F8:25:51,SeikoEps Seiko Epson Corporation
 F8:27:2E,Mercku
 F8:27:93,"Apple Apple, Inc."
 F8:28:19,LiteonTe Liteon Technology Corporation
 F8:28:C9,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:29:C0,"Availink Availink, Inc."
 F8:2B:7F,"HuaweiDe Huawei Device Co., Ltd."
 F8:2B:C8,"JiangsuS Jiangsu Switter Co., Ltd"
 F8:2C:18,2Wire 2Wire Inc
 F8:2D:7C,"Apple Apple, Inc."
 F8:2D:C0,"ARRISGro ARRIS Group, Inc."
+F8:2E:0C,TexasIns Texas Instruments
 F8:2E:3F,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:2E:8E,"NanjingK Nanjing Kechen Electric Co., Ltd."
 F8:2E:DB,RTW RTW GmbH & Co. KG
 F8:2F:08,MolexCMS Molex CMS
 F8:2F:5B,eGauge eGauge Systems LLC
 F8:2F:65,"HuaweiDe Huawei Device Co., Ltd."
 F8:2F:6A,ItelMobi Itel Mobile Limited
@@ -46431,22 +48101,24 @@
 F8:30:02,TexasIns Texas Instruments
 F8:30:94,Alcatel- Alcatel-Lucent Telecom Limited
 F8:31:3E,endeavou endeavour GmbH
 F8:32:E4,ASUSTekC ASUSTek COMPUTER INC.
 F8:33:31,TexasIns Texas Instruments
 F8:33:76,"GoodMind Good Mind Innovation Co., Ltd."
 F8:34:41,IntelCor Intel Corporate
+F8:34:51,Comcast Comcast-SRL
 F8:34:5A,HitronTe Hitron Technologies. Inc
 F8:35:53,MagentaR Magenta Research Ltd.
 F8:35:DD,"GemtekTe Gemtek Technology Co., Ltd."
 F8:36:9B,TexasIns Texas Instruments
 F8:38:69,LGElectr LG Electronics
 F8:38:80,"Apple Apple, Inc."
-F8:3B:1D,Technico Technicolor CH USA Inc.
+F8:3B:1D,VantivaU Vantiva USA LLC
 F8:3B:7E,"HuaweiDe Huawei Device Co., Ltd."
+F8:3C:80,"MitsumiE Mitsumi Electric Co.,Ltd."
 F8:3C:BF,BotatoEl Botato Electronics Sdn Bhd
 F8:3D:4E,"Softlink Softlink Automation System Co., Ltd"
 F8:3D:FF,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:3E:95,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:3F:51,"SamsungE Samsung Electronics Co.,Ltd"
 F8:42:FB,"YasudaJo Yasuda Joho Co.,ltd."
 F8:44:E3,TaicangT Taicang T&W Electronics
@@ -46473,14 +48145,15 @@
 F8:50:63,Verathon
 F8:51:28,SimpliSa SimpliSafe
 F8:51:6D,DenwaTec Denwa Technology Corp.
 F8:52:DF,VNLEurop VNL Europe AB
 F8:53:29,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:54:AF,ECITelec ECI Telecom Ltd.
 F8:54:B8,AmazonTe Amazon Technologies Inc.
+F8:54:F6,AzureWav AzureWave Technology Inc.
 F8:55:48,TexasIns Texas Instruments
 F8:55:CD,Visteon Visteon Corporation
 F8:56:C3,zte zte corporation
 F8:57:2E,"CoreBran Core Brands, LLC"
 F8:59:71,IntelCor Intel Corporate
 F8:5A:00,SanfordL Sanford LP
 F8:5B:3B,AskeyCom Askey Computer Corp
@@ -46490,49 +48163,52 @@
 F8:5B:C9,M-Cube M-Cube Spa
 F8:5C:45,ICNexus IC Nexus Co. Ltd.
 F8:5C:4D,Nokia
 F8:5C:7D,"Shenzhen Shenzhen Honesty Electronics Co.,Ltd."
 F8:5C:7E,"Shenzhen Shenzhen Honesty Electronics Co.,Ltd."
 F8:5E:0B,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 F8:5E:3C,"Shenzhen Shenzhen Zhibotong Electronics Co.,Ltd"
-F8:5E:42,Technico Technicolor CH USA Inc.
+F8:5E:42,VantivaU Vantiva USA LLC
 F8:5E:A0,IntelCor Intel Corporate
 F8:5F:2A,Nokia Nokia Corporation
 F8:60:F0,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 F8:62:14,"Apple Apple, Inc."
 F8:62:AA,xn xn systems
 F8:63:3F,IntelCor Intel Corporate
 F8:63:D9,"ARRISGro ARRIS Group, Inc."
 F8:64:65,"AnovaApp Anova Applied Electronics, Inc."
 F8:64:B8,zte zte corporation
 F8:66:01,"SuzhouCh Suzhou Chi-tek information technology Co., Ltd"
 F8:66:5A,"Apple Apple, Inc."
+F8:66:91,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 F8:66:D1,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 F8:66:F2,"Cisco Cisco Systems, Inc"
 F8:69:71,"SeibuEle Seibu Electric Co.,"
 F8:6B:14,"BarrotTe Barrot Technology Co.,LTD"
 F8:6B:D9,"Cisco Cisco Systems, Inc"
 F8:6C:03,"Shenzhen Shenzhen Teleone Technology Co., Ltd"
 F8:6C:E1,TaicangT Taicang T&W Electronics
 F8:6D:73,"Zengge Zengge Co., Limited"
 F8:6E:CF,Arcx Arcx Inc
 F8:6E:EE,"HuaweiTe Huawei Technologies Co.,Ltd"
+F8:6F:B0,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
 F8:6F:C1,"Apple Apple, Inc."
 F8:6F:DE,"Shenzhen Shenzhen Goodix Technology Co.,Ltd."
 F8:71:0C,XiaomiCo Xiaomi Communications Co Ltd
 F8:71:FE,"GoldmanS The Goldman Sachs Group, Inc."
 F8:72:EA,"Cisco Cisco Systems, Inc"
 F8:73:94,Netgear
 F8:73:A2,Avaya Avaya Inc
 F8:75:88,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:75:A4,"LCFCHeFe LCFC(HeFei) Electronics Technology co., ltd"
 F8:76:9B,"Neopis Neopis Co., Ltd."
 F8:77:B8,"SamsungE Samsung Electronics Co.,Ltd"
 F8:79:07,"HuaweiDe Huawei Device Co., Ltd."
 F8:79:0A,"ARRISGro ARRIS Group, Inc."
+F8:79:28,zte zte corporation
 F8:79:99,"Guangdon Guangdong Jiuzhi Technology Co.,Ltd"
 F8:7A:41,"Cisco Cisco Systems, Inc"
 F8:7A:EF,"RosonixT Rosonix Technology, Inc."
 F8:7B:20,"Cisco Cisco Systems, Inc"
 F8:7B:62,"FASTWELI FASTWEL INTERNATIONAL CO., LTD. Taiwan Branch"
 F8:7B:7A,"ARRISGro ARRIS Group, Inc."
 F8:7B:8C,AmpedWir Amped Wireless
@@ -46577,14 +48253,15 @@
 F8:91:73,AedleSas Aedle Sas
 F8:93:F3,Volans
 F8:94:C2,IntelCor Intel Corporate
 F8:95:22,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:95:50,ProtonPr Proton Products Chengdu Ltd
 F8:95:C7,LGElectr LG Electronics (Mobile Communications)
 F8:95:EA,"Apple Apple, Inc."
+F8:97:25,"OppleLig Opple Lighting Co., Ltd"
 F8:97:53,"HuaweiDe Huawei Device Co., Ltd."
 F8:97:A9,Ericsson Ericsson AB
 F8:97:CF,"Daeshin- Daeshin-Information Technology Co., Ltd."
 F8:98:3A,LeemanIn Leeman International (HongKong) Limited
 F8:98:B9,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:98:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:99:10,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
@@ -46667,33 +48344,35 @@
 F8:C1:20,"XianLink Xi'an Link-Science Technology Co.,Ltd"
 F8:C2:49,AmpereCo Ampere Computing Llc
 F8:C2:88,"Cisco Cisco Systems, Inc"
 F8:C3:72,TsuzukiD Tsuzuki Denki
 F8:C3:97,NZXT NZXT Corp. Ltd.
 F8:C3:9E,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:C3:CC,"Apple Apple, Inc."
+F8:C4:AE,"Guangdon Guangdong Oppo Mobile Telecommunications Corp.,Ltd"
 F8:C4:F3,"Shanghai Shanghai Infinity Wireless Technologies Co.,Ltd."
 F8:C6:78,Carefusi Carefusion
 F8:C9:6C,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 F8:CA:59,NetCommW NetComm Wireless
 F8:CA:85,NEC NEC Corporation
 F8:CA:B8,Dell Dell Inc.
 F8:CC:6E,DEPOElec DEPO Electronics Ltd
 F8:CD:C8,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 F8:CE:72,Wistron Wistron Corporation
 F8:CF:C5,"Motorola Motorola Mobility LLC, a Lenovo Company"
 F8:D0:27,SeikoEps Seiko Epson Corporation
 F8:D0:AC,SonyInte Sony Interactive Entertainment Inc.
 F8:D0:BD,"SamsungE Samsung Electronics Co.,Ltd"
 F8:D1:11,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
-F8:D2:AC,Technico Technicolor CH USA Inc.
+F8:D2:AC,VantivaU Vantiva USA LLC
 F8:D3:A9,AXANNetw AXAN Networks
 F8:D4:62,Pumatron Pumatronix Equipamentos Eletronicos Ltda.
 F8:D4:78,Flextron Flextronics Tech.(Ind) Pvt Ltd
 F8:D7:56,SimmTron Simm Tronic Limited
+F8:D7:58,Veratron Veratron AG
 F8:D7:BF,REVRitte REV Ritter GmbH
 F8:D9:B8,"OpenMesh Open Mesh, Inc."
 F8:DA:0C,"HonHaiPr Hon Hai Precision Ind. Co.,Ltd."
 F8:DA:DF,"EcoTech EcoTech, Inc."
 F8:DA:E2,NDCTechn NDC Technologies
 F8:DA:F4,"TaishanO Taishan Online Technology Co., Ltd."
 F8:DB:4C,"PNYTechn PNY Technologies, INC."
@@ -46707,27 +48386,29 @@
 F8:E0:79,"Motorola Motorola Mobility LLC, a Lenovo Company"
 F8:E4:3B,ASIXElec ASIX Electronics Corporation
 F8:E4:4E,Mcot Mcot Inc.
 F8:E4:A4,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
 F8:E4:E3,IntelCor Intel Corporate
 F8:E4:FB,"Actionte Actiontec Electronics, Inc"
 F8:E5:7E,"Cisco Cisco Systems, Inc"
+F8:E5:CE,"Apple Apple, Inc."
 F8:E5:CF,CgiItUk Cgi It Uk Limited
 F8:E6:1A,"SamsungE Samsung Electronics Co.,Ltd"
 F8:E7:1E,RuckusWi Ruckus Wireless
 F8:E7:A0,"vivoMobi vivo Mobile Communication Co., Ltd."
 F8:E7:B5,µTechTec µTech Tecnologia LTDA
 F8:E8:11,"HuaweiTe Huawei Technologies Co.,Ltd"
 F8:E8:77,HarmanBe Harman/Becker Automotive Systems GmbH
 F8:E9:03,D-LinkIn D-Link International
 F8:E9:4E,"Apple Apple, Inc."
 F8:E9:4F,"Cisco Cisco Systems, Inc"
 F8:E9:68,EgkerKft Egker Kft.
 F8:EA:0A,Dipl-Mat Dipl.-Math. Michael Rauch
 F8:ED:A5,"ARRISGro ARRIS Group, Inc."
+F8:ED:AE,"Mobiwire Mobiwire Mobiles(Ningbo) Co.,Ltd"
 F8:F0:05,NewportM Newport Media Inc.
 F8:F0:14,RackWare RackWare Inc.
 F8:F0:82,Nagtech Nagtech Llc
 F8:F0:C5,"SuzhouKu Suzhou Kuhan Information Technologies Co.,Ltd."
 F8:F1:B6,"Motorola Motorola Mobility LLC, a Lenovo Company"
 F8:F1:E6,"SamsungE Samsung Electronics Co.,Ltd"
 F8:F2:1E,IntelCor Intel Corporate
@@ -46741,15 +48422,15 @@
 F8:FC:E1,AmazonTe Amazon Technologies Inc.
 F8:FE:5C,Reciproc Reciprocal Labs Corp
 F8:FE:A8,Technico Technico Japan Corporation
 F8:FF:0B,Electron Electronic Technology Inc.
 F8:FF:5F,"Shenzhen Shenzhen Communication Technology Co.,Ltd"
 F8:FF:C2,"Apple Apple, Inc."
 FA:07:3E,NBASE-TA NBASE-T Alliance
-FA:0B:BC,Asd-Stan
+FA:0B:BC,Cen
 FA:14:66,Allegion Allegion PLC
 FA:16:19,trendyte trendytech
 FA:2E:E9,"OCAAllia OCA Alliance, Inc."
 FA:4C:77,Occitali Occitaline
 FA:55:6F,Symbolic SymbolicIO
 FA:61:0E,"Laborato Laboratory for Computational Sensing and Robotics, Johns Hopkins University"
 FA:63:E1,SamsungE Samsung Electronics (UK) Ltd
@@ -46802,14 +48483,15 @@
 FC:19:99,XiaomiCo Xiaomi Communications Co Ltd
 FC:19:D0,"CloudVis Cloud Vision Networks Technology Co.,Ltd."
 FC:1A:11,"vivoMobi vivo Mobile Communication Co., Ltd."
 FC:1B:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:1B:FF,V-Zug V-Zug Ag
 FC:1C:A1,Nokia
 FC:1D:2A,"vivoMobi vivo Mobile Communication Co., Ltd."
+FC:1D:3A,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:1D:43,"Apple Apple, Inc."
 FC:1D:59,ISmartCi I Smart Cities HK Ltd
 FC:1D:84,Autobase
 FC:1E:16,IPEVO IPEVO corp
 FC:1F:19,"SamsungE Samsung Electro Mechanics Co., Ltd."
 FC:1F:C0,Eurecam
 FC:22:9C,"HanKyung Han Kyung I Net Co.,Ltd."
@@ -46820,29 +48502,30 @@
 FC:27:A2,"TransEle Trans Electric Co., Ltd."
 FC:29:E3,Infinixm Infinix mobility limited
 FC:29:F3,"McPay McPay Co.,LTD."
 FC:2A:46,"RealmeCh Realme Chongqing Mobile Telecommunications Corp.,Ltd."
 FC:2A:54,"Connecte Connected Data, Inc."
 FC:2A:9C,"Apple Apple, Inc."
 FC:2B:B2,"Actionte Actiontec Electronics, Inc"
+FC:2C:FD,dormakab dormakaba Canada Inc. - Keyscan
 FC:2D:5E,zte zte corporation
 FC:2E:19,"ChinaMob China Mobile Group Device Co.,Ltd."
 FC:2E:2D,LoromInd Lorom Industrial Co.LTD.
 FC:2F:40,"Calxeda Calxeda, Inc."
 FC:2F:6B,"Everspin Everspin Technologies, Inc."
 FC:2F:AA,Nokia
 FC:2F:EF,"UTTTechn UTT Technologies Co., Ltd."
 FC:31:5D,"Apple Apple, Inc."
 FC:32:88,"CELOTWir CELOT Wireless Co., Ltd"
 FC:33:42,JuniperN Juniper Networks
 FC:33:57,"KAGAFEI KAGA FEI Co., Ltd."
 FC:33:5F,Polyera
 FC:34:97,ASUSTekC ASUSTek COMPUTER INC.
 FC:35:98,Favite Favite Inc.
-FC:35:E6,Visteon Visteon corp
+FC:35:E6,Visteon Visteon Corporation
 FC:37:2B,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 FC:38:C4,"ChinaGra China Grand Communications Co.,Ltd."
 FC:39:64,ItelMobi Itel Mobile Limited
 FC:3C:E9,"Tsington Tsingtong Technologies Co, Ltd."
 FC:3D:93,Longchee Longcheer Telecommunication Limited
 FC:3D:A5,Arcadyan Arcadyan Corporation
 FC:3F:7C,"HuaweiTe Huawei Technologies Co.,Ltd"
@@ -46856,45 +48539,48 @@
 FC:44:82,IntelCor Intel Corporate
 FC:44:99,SwarcoLE Swarco LEA d.o.o.
 FC:44:9F,zte zte corporation
 FC:45:5F,"JiangxiS Jiangxi Shanshui Optoelectronic Technology Co.,Ltd"
 FC:45:96,"CompalIn Compal Information (Kunshan) Co., Ltd."
 FC:45:C3,TexasIns Texas Instruments
 FC:47:D8,"Apple Apple, Inc."
+FC:48:C9,YobiiqIn Yobiiq Intelligence B.V.
 FC:48:EF,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:49:2D,AmazonTe Amazon Technologies Inc.
 FC:4A:E9,Castlene Castlenet Technology Inc.
 FC:4B:1C,Intersen Intersensor S.R.L.
 FC:4B:57,Peerless Peerless Instrument Division of Curtiss-Wright
 FC:4B:BC,"SunplusT Sunplus Technology Co., Ltd."
 FC:4D:8C,"Shenzhen Shenzhen Pante Electronics Technology Co., Ltd"
 FC:4D:A6,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:4D:D4,"Universa Universal Global Scientific Industrial Co., Ltd."
 FC:4E:A4,"Apple Apple, Inc."
 FC:50:90,SIMEXSp SIMEX Sp. z o.o.
 FC:51:A4,"ARRISGro ARRIS Group, Inc."
-FC:52:8D,Technico Technicolor CH USA Inc.
+FC:52:8D,VantivaU Vantiva USA LLC
 FC:52:CE,Controli Control iD
 FC:53:9E,"Shanghai Shanghai Wind Technologies Co.,Ltd"
 FC:55:DC,BalticLa Baltic Latvian Universal Electronics LLC
+FC:57:03,"Hisenseb Hisense broadband multimedia technology Co.,Ltd"
 FC:58:4A,"xiamensh xiamenshi c-chip technology co., ltd"
 FC:58:9A,"Cisco Cisco Systems, Inc"
 FC:58:DF,Interpho Interphone Service
 FC:58:FA,"ShenZhen Shen Zhen Shi Xin Zhong Xin Technology Co.,Ltd."
+FC:59:C0,AristaNe Arista Networks
 FC:5A:1D,HitronTe Hitron Technologies. Inc
 FC:5B:24,WeibelSc Weibel Scientific A/S
 FC:5B:26,MikroBit MikroBits
 FC:5B:39,"Cisco Cisco Systems, Inc"
 FC:5C:45,RuckusWi Ruckus Wireless
 FC:5F:49,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 FC:60:18,"Zhejiang Zhejiang Kangtai Electric Co., Ltd."
 FC:60:9B,"NewH3CTe New H3C Technologies Co., Ltd"
 FC:61:79,IEEERegi IEEE Registration Authority
 FC:61:79:00:00:00/28,"ZhuhaiAn Zhuhai Anjubao Electronics Technology Co., Ltd."
-FC:61:79:10:00:00/28,"Signalin Signalinks Communication Technology Co.,Ltd"
+FC:61:79:10:00:00/28,"Signalin Signalinks Communication Technology Co., Ltd"
 FC:61:79:20:00:00/28,"Shenzhen Shenzhen Shenshui Electronic Commerce Co.,Ltd"
 FC:61:79:30:00:00/28,EchoStar EchoStar Mobile
 FC:61:79:40:00:00/28,Choeunen Choeuneng
 FC:61:79:50:00:00/28,Qisda Qisda Corporation
 FC:61:79:60:00:00/28,"Hangzhou Hangzhou LiDe Communication Co.,Ltd"
 FC:61:79:70:00:00/28,Kvalitet Kvaliteta Systems and Solutions Private Limited
 FC:61:79:80:00:00/28,Annapurn Annapurna labs
@@ -46913,69 +48599,75 @@
 FC:65:B3,"HuaweiDe Huawei Device Co., Ltd."
 FC:65:DE,AmazonTe Amazon Technologies Inc.
 FC:66:CF,"Apple Apple, Inc."
 FC:67:1F,TuyaSmar Tuya Smart Inc.
 FC:68:3E,"Directed Directed Perception, Inc"
 FC:69:47,TexasIns Texas Instruments
 FC:69:8C,ANDREASS ANDREAS STIHL AG & Co. KG
+FC:6A:1C,"Mellanox Mellanox Technologies, Inc."
 FC:6B:F0,TopwellI Topwell International Holdinds Limited
 FC:6C:31,LXinstru LXinstruments GmbH
 FC:6D:C0,Bme Bme Corporation
 FC:6D:D1,"APRESIA APRESIA Systems, Ltd."
 FC:6F:B7,"ARRISGro ARRIS Group, Inc."
 FC:71:FA,TraneTec Trane Technologies
 FC:73:FB,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:75:16,D-LinkIn D-Link International
 FC:75:E6,Handream Handreamnet
 FC:76:92,"Semptian Semptian Co.,Ltd."
 FC:77:74,IntelCor Intel Corporate
 FC:77:7B,HitronTe Hitron Technologies. Inc
 FC:79:0B,"HitachiH Hitachi High Technologies America, Inc."
+FC:7A:58,"Shenzhen Shenzhen Skyworth Digital Technology CO., Ltd"
 FC:7C:02,"PhicommS Phicomm (Shanghai) Co., Ltd."
 FC:7C:E7,FciUsa Fci Usa Llc
 FC:7D:6C,"HYESUNGT HYESUNG TECHWIN Co., Ltd"
 FC:7F:56,CoSystCo CoSyst Control Systems GmbH
 FC:7F:F1,"ArubaaHe Aruba, a Hewlett Packard Enterprise Company"
 FC:83:29,Treitech Trei technics
 FC:83:99,Avaya Avaya Inc
 FC:83:C6,"N-RadioT N-Radio Technologies Co., Ltd."
 FC:84:17,"HonorDev Honor Device Co., Ltd."
+FC:84:A7,"MurataMa Murata Manufacturing Co., Ltd."
 FC:85:96,Axonne Axonne Inc.
 FC:86:2A,"HuaweiDe Huawei Device Co., Ltd."
 FC:87:43,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:8A:3D,zte zte corporation
 FC:8B:97,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 FC:8D:3D,Leapfive Leapfive Tech. Ltd.
 FC:8E:5B,ChinaMob China Mobile Iot Limited company
 FC:8E:6E,"StreamCC StreamCCTV, LLC"
 FC:8E:7E,"ARRISGro ARRIS Group, Inc."
 FC:8F:7D,"Shenzhen Shenzhen Gongjin Electronics Co.,Lt"
 FC:8F:90,"SamsungE Samsung Electronics Co.,Ltd"
 FC:8F:C4,Intellig Intelligent Technology Inc.
 FC:90:FA,Independ Independent Technologies
-FC:91:14,Technico Technicolor CH USA Inc.
+FC:91:14,VantivaU Vantiva USA LLC
 FC:91:89,"SichuanT Sichuan Tianyi Comheart Telecom Co.,LTD"
 FC:92:3B,Nokia Nokia Corporation
 FC:92:57,RenesasE Renesas Electronics (Penang) Sdn. Bhd.
 FC:94:35,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:94:6C,Ubivelox
 FC:94:CE,zte zte corporation
-FC:94:E3,Technico Technicolor CH USA Inc.
+FC:94:E3,VantivaU Vantiva USA LLC
 FC:95:6A,Octagon Octagon Systems Corp.
 FC:96:43,JuniperN Juniper Networks
+FC:97:A8,Cricut Cricut Inc.
 FC:99:47,"Cisco Cisco Systems, Inc"
 FC:9A:FA,MotusGlo Motus Global Inc.
 FC:9B:C6,"Sumavisi Sumavision Technologies Co.,Ltd"
 FC:9B:D4,EdgeQ
 FC:9C:98,ArloTech Arlo Technology
+FC:9C:A7,"Apple Apple, Inc."
 FC:9D:D8,BeijingT Beijing TongTongYiLian Science and Technology Ltd.
 FC:9F:AE,Fidus Fidus Systems Inc
 FC:9F:E1,CONWINTe CONWIN.Tech. Ltd
 FC:9F:FD,"Hangzhou Hangzhou Hikvision Digital Technology Co.,Ltd."
 FC:A0:5A,"Oraycom Oray.com co., LTD."
+FC:A0:F3,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:A1:3E,"SamsungE Samsung Electronics Co.,Ltd"
 FC:A1:83,AmazonTe Amazon Technologies Inc.
 FC:A2:2A,PTCallys PT. Callysta Multi Engineering
 FC:A3:86,"Shenzhen Shenzhen Chuangwei-Rgb Electronics Co.,Ltd"
 FC:A4:7A,IEEERegi IEEE Registration Authority
 FC:A4:7A:00:00:00/28,Broadcom Broadcom Inc.
 FC:A4:7A:10:00:00/28,"Shenzhen Shenzhen VMAX New Energy Co., Ltd."
@@ -47011,23 +48703,26 @@
 FC:AE:34,"ARRISGro ARRIS Group, Inc."
 FC:AF:6A,Qulsar Qulsar Inc
 FC:AF:AC,Socionex Socionext Inc.
 FC:AF:BE,TireChec TireCheck GmbH
 FC:B0:C4,"Shanghai Shanghai DareGlobal Technologies Co.,Ltd"
 FC:B0:DE,CloudNet Cloud Network Technology Singapore Pte. Ltd.
 FC:B1:0D,"Shenzhen Shenzhen Tian Kun Technology Co.,LTD."
+FC:B2:D6,CigShang Cig Shanghai Co Ltd
 FC:B3:BC,IntelCor Intel Corporate
+FC:B4:67,Espressi Espressif Inc.
 FC:B4:E6,AskeyCom Askey Computer Corp
 FC:B5:8A,Wapice Wapice Ltd.
 FC:B6:62,ICHoldin IC Holdings LLC
 FC:B6:98,"Cambridg Cambridge Industries(Group) Co.,Ltd."
 FC:B6:9D,"Zhejiang Zhejiang Dahua Technology Co., Ltd."
 FC:B6:D8,"Apple Apple, Inc."
 FC:B7:F0,IdahoNat Idaho National Laboratory
 FC:B9:7E,GEApplia GE Appliances
+FC:B9:DF,"Motorola Motorola Mobility LLC, a Lenovo Company"
 FC:BB:A1,"Shenzhen Shenzhen Minicreate Technology Co.,Ltd"
 FC:BC:0E,"Zhejiang Zhejiang Cainiao Supply Chain Management Co., Ltd"
 FC:BC:9C,Vimar Vimar Spa
 FC:BC:D1,"HuaweiTe Huawei Technologies Co.,Ltd"
 FC:BD:67,AristaNe Arista Networks
 FC:BE:7B,"vivoMobi vivo Mobile Communication Co., Ltd."
 FC:C2:33,ASUSTekC ASUSTek COMPUTER INC.
@@ -47074,14 +48769,15 @@
 FC:D2:B6:E0:00:00/28,Univer Univer S.p.A.
 FC:D4:36,"Motorola Motorola Mobility LLC, a Lenovo Company"
 FC:D4:F2,CocaCola The Coca Cola Company
 FC:D4:F6,MessanaA Messana Air.Ray Conditioning s.r.l.
 FC:D5:D9,"Shenzhen Shenzhen SDMC Technology CO.,Ltd."
 FC:D6:BD,RobertBo Robert Bosch GmbH
 FC:D7:33,"Tp-LinkT Tp-Link Technologies Co.,Ltd."
+FC:D7:49,AmazonTe Amazon Technologies Inc.
 FC:D8:17,BeijingH Beijing Hesun Technologies Co.Ltd.
 FC:D8:48,"Apple Apple, Inc."
 FC:D9:08,XiaomiCo Xiaomi Communications Co Ltd
 FC:DB:21,SamsaraN Samsara Networks Inc
 FC:DB:96,"Enervall Enervalley Co., Ltd"
 FC:DB:B3,"MurataMa Murata Manufacturing Co., Ltd."
 FC:DC:4A,G-Wearab G-Wearables Corp.
@@ -47099,26 +48795,28 @@
 FC:E5:57,Nokia Nokia Corporation
 FC:E6:6A,Industri Industrial Software Co
 FC:E8:06,EdifierI Edifier International
 FC:E8:92,"Hangzhou Hangzhou Lancable Technology Co.,Ltd"
 FC:E9:98,"Apple Apple, Inc."
 FC:E9:D8,AmazonTe Amazon Technologies Inc.
 FC:EA:50,Integrat Integrated Device Technology (Malaysia) Sdn. Bhd.
-FC:EC:DA,Ubiquiti Ubiquiti Networks Inc.
+FC:EC:DA,Ubiquiti Ubiquiti Inc
 FC:ED:B9,Arrayent
 FC:EE:E6,"FormikeE Formike Electronic Co., Ltd"
 FC:F1:36,"SamsungE Samsung Electronics Co.,Ltd"
 FC:F1:52,Sony Sony Corporation
 FC:F1:CD,"Optex-Fa Optex-Fa Co.,Ltd."
 FC:F2:9F,ChinaMob China Mobile Iot Limited company
 FC:F5:28,ZyxelCom Zyxel Communications Corporation
 FC:F5:C4,Espressi Espressif Inc.
 FC:F6:47,"Fiberhom Fiberhome Telecommunication Technologies Co.,LTD"
+FC:F7:63,"KunGaoMi KunGao Micro (JiangSu) Co., LTd"
 FC:F7:7B,"HuaweiDe Huawei Device Co., Ltd."
 FC:F8:AE,IntelCor Intel Corporate
 FC:F8:B7,TRONTEQE TRONTEQ Electronic
+FC:FA:21,zte zte corporation
 FC:FA:F7,"Shanghai Shanghai Baud Data Communication Co.,Ltd."
 FC:FB:FB,"Cisco Cisco Systems, Inc"
 FC:FC:48,"Apple Apple, Inc."
 FC:FE:77,"HitachiR Hitachi Reftechno, Inc."
 FC:FE:C2,Invensys Invensys Controls UK Limited
 FC:FF:AA,IEEERegi IEEE Registration Authority
```

### Comparing `MacToManufacturer-0.1.0/src/MacToManufacturer/main.py` & `MacToManufacturer-0.2.0/src/MacToManufacturer/main.py`

 * *Files identical despite different names*

