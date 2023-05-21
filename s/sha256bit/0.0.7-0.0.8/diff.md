# Comparing `tmp/sha256bit-0.0.7.tar.gz` & `tmp/sha256bit-0.0.8.tar.gz`

## Comparing `sha256bit-0.0.7.tar` & `sha256bit-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sha256bit-0.0.7/publish_to_pypi
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sha256bit-0.0.7/requirements.txt
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.github/workflows/build.yml
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 sha256bit-0.0.7/sha256bit/__init__.py
--rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/SHA256LongMsg.rsp
--rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/SHA256ShortMsg.rsp
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/__init__.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_api.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_cavp.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_hardcoded.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_vs_hashlib.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.7/LICENSE
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 sha256bit-0.0.7/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 sha256bit-0.0.7/hatch.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 sha256bit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 sha256bit-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sha256bit-0.0.8/publish_to_pypi
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sha256bit-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6929 2020-02-02 00:00:00.000000 sha256bit-0.0.8/sha256bit/__init__.py
+-rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/SHA256LongMsg.rsp
+-rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/SHA256ShortMsg.rsp
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/__init__.py
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_api.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_cavp.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_hardcoded.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sha256bit-0.0.8/test/test_vs_hashlib.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 sha256bit-0.0.8/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 sha256bit-0.0.8/hatch.toml
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 sha256bit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 sha256bit-0.0.8/PKG-INFO
```

### Comparing `sha256bit-0.0.7/.github/workflows/build.yml` & `sha256bit-0.0.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/.github/workflows/python-package.yml` & `sha256bit-0.0.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/.github/workflows/test.yml` & `sha256bit-0.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/sha256bit/__init__.py` & `sha256bit-0.0.8/sha256bit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import binascii
 import copy
 import struct
-import binascii
 
 
-class sha256bit(object):
+class sha256bit:
     F32 = 0xFFFFFFFF
 
     _k = [
         0x428A2F98,
         0x71374491,
         0xB5C0FBCF,
         0xE9B5DBA5,
@@ -115,45 +115,37 @@
     def export_state(self):
         if self._digest is None:
             h = self._h
             c = self._cache
         else:
             h = self._digest
             c = None
-        return {"h": h, "cnt": self._counter, "cache": c}
+        return {'h': h, 'cnt': self._counter, 'cache': c}
 
     @staticmethod
     def import_state(state):
         o = sha256bit()
-        o._counter = state["cnt"]
+        o._counter = state['cnt']
         if 0 != (o._counter % 8):
             o._has_bitlen = True
-        if state["cache"] is None:
-            o._digest = state["h"]
+        if state['cache'] is None:
+            o._digest = state['h']
             o._h = None
             o._cache = None
         else:
-            o._h = state["h"]
-            o._cache = bytearray(state["cache"])
+            o._h = state['h']
+            o._cache = bytearray(state['cache'])
         return o
 
     def _compress(self, c):
         w = [0] * 64
-        w[0:16] = struct.unpack("!16L", c)
+        w[0:16] = struct.unpack('!16L', c)
         for i in range(16, 64):
-            s0 = (
-                sha256bit._rotr(w[i - 15], 7)
-                ^ sha256bit._rotr(w[i - 15], 18)
-                ^ (w[i - 15] >> 3)
-            )
-            s1 = (
-                sha256bit._rotr(w[i - 2], 17)
-                ^ sha256bit._rotr(w[i - 2], 19)
-                ^ (w[i - 2] >> 10)
-            )
+            s0 = sha256bit._rotr(w[i - 15], 7) ^ sha256bit._rotr(w[i - 15], 18) ^ (w[i - 15] >> 3)
+            s1 = sha256bit._rotr(w[i - 2], 17) ^ sha256bit._rotr(w[i - 2], 19) ^ (w[i - 2] >> 10)
             w[i] = (w[i - 16] + s0 + w[i - 7] + s1) & sha256bit.F32
 
         a, b, c, d, e, f, g, h = self._h
 
         for i in range(64):
             s0 = sha256bit._rotr(a, 2) ^ sha256bit._rotr(a, 13) ^ sha256bit._rotr(a, 22)
             t2 = s0 + sha256bit._maj(a, b, c)
@@ -175,20 +167,20 @@
     def update(self, m, *, bitlen=None):
         """Update the hash object with the bytes in data. Repeated calls
         are equivalent to a single call with the concatenation of all
         the arguments.
         """
         if not m:
             return
-        assert not self._has_bitlen, "we support bitlen only for last call"
+        assert not self._has_bitlen, 'we support bitlen only for last call'
         if bitlen is not None:
             if 0 != (bitlen % 8):
                 self._has_bitlen = True
             else:
-                assert bitlen == len(m) * 8, "bitLen=%d, len(m)*8=%d" % (
+                assert bitlen == len(m) * 8, 'bitLen=%d, len(m)*8=%d' % (
                     bitlen,
                     len(m) * 8,
                 )
             self._counter += bitlen
         else:
             self._counter += len(m) * 8
 
@@ -217,37 +209,37 @@
             print(lastBlockBitLen, lastBlockFullBytesCnt, padlen, len(self._cache))
 
         shift = self._counter % 8
         if shift > 0 and (len(self._cache) > 0):
             mask = 0xFF << (8 - shift)
             self._cache[-1] = (self._cache[-1] & mask) | (0x80 >> shift)
         else:
-            self._cache += b"\x80"
-        self._cache += (b"\x00" * padlen) + self._counter.to_bytes(8, byteorder="big")
+            self._cache += b'\x80'
+        self._cache += (b'\x00' * padlen) + self._counter.to_bytes(8, byteorder='big')
         if False:
             from pysatl import Utils
 
-            print("counter=%d (0x%x)" % (self._counter, self._counter))
+            print('counter=%d (0x%x)' % (self._counter, self._counter))
             print(Utils.hexstr(self._cache))
-        assert len(self._cache) in [64, 128], "len(self._cache)=%d" % len(self._cache)
+        assert len(self._cache) in [64, 128], 'len(self._cache)=%d' % len(self._cache)
 
     def digest(self):
         """Return the digest of the bytes passed to the update() method
         so far as a bytes object.
         """
         if self._digest is not None:
             return self._digest
         self._pad()
         blocks = [self._cache[i : i + 64] for i in range(0, len(self._cache), 64)]
         for b in blocks:
             self._compress(b)
-        data = [struct.pack("!L", i) for i in self._h[: self._output_size]]
-        self._digest = b"".join(data)
+        data = [struct.pack('!L', i) for i in self._h[: self._output_size]]
+        self._digest = b''.join(data)
         self._cache = None
         self._h = None
         return self._digest
 
     def hexdigest(self):
         """Like digest() except the digest is returned as a string
         of double length, containing only hexadecimal digits.
         """
-        return binascii.hexlify(self.digest()).decode("ascii")
+        return binascii.hexlify(self.digest()).decode('ascii')
```

### Comparing `sha256bit-0.0.7/test/SHA256LongMsg.rsp` & `sha256bit-0.0.8/test/SHA256LongMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/test/SHA256ShortMsg.rsp` & `sha256bit-0.0.8/test/SHA256ShortMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/test/test.py` & `sha256bit-0.0.8/test/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import hashlib
-from pysatl import Utils
 import re
+
+from pysatl import Utils
+
 from sha256bit import sha256bit
 
 
 def block_generator(seed, msg_bitlen):
     l2block = hashlib.sha256(seed).digest()
     l2block += hashlib.sha256(l2block).digest()
     blockBitLen = len(l2block) * 8
@@ -31,17 +33,17 @@
     o = bytearray()
     for b in block_generator(seed, msg_bitlen):
         o += b
     return o
 
 
 def check_against_hashlib(n_seeds=3, max_length=1024 * 4):
-    print("check against hashlib")
+    print('check against hashlib')
 
-    assert hashlib.sha256("abc".encode()).digest() == sha256bit("abc".encode()).digest()
+    assert hashlib.sha256(b'abc').digest() == sha256bit(b'abc').digest()
 
     def check_against_hashlib(seed, msg_bitlen):
         expected = hashlib.sha256()
         dut = sha256bit()
         for block in block_generator(seed, msg_bitlen):
             # print(Utils.hexstr(block))
             expected.update(block)
@@ -53,89 +55,88 @@
             seed = bytearray([seedByte])
             check_against_hashlib(seed, msgBitLen)
 
 
 def check(msg, bitlen, sig):
     m = sha256bit()
     if isinstance(msg, str):
-        msg = msg.encode("ascii")
-    descr = "msg      = " + Utils.hexstr(msg) + "\n"
-    descr += "bitlen   = %d\n" % bitlen
-    descr += "expected = " + sig + "\n"
+        msg = msg.encode('ascii')
+    descr = 'msg      = ' + Utils.hexstr(msg) + '\n'
+    descr += 'bitlen   = %d\n' % bitlen
+    descr += 'expected = ' + sig + '\n'
     try:
         m.update(msg, bitlen=bitlen)
         digest = m.hexdigest()
     except Exception as e:
         print(descr)
         raise e
-    errMsg = "\n"
+    errMsg = '\n'
     errMsg += descr
-    errMsg += "digest   = " + digest + "\n"
+    errMsg += 'digest   = ' + digest + '\n'
     assert digest == sig, errMsg
 
 
 def check_hardcoded_test_vectors():
-    print("check few minimal hardcoded test vectors")
+    print('check few minimal hardcoded test vectors')
 
     tests = [
         {
-            "msg": "",
-            "bitlen": 0,
-            "digest": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+            'msg': '',
+            'bitlen': 0,
+            'digest': 'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855',
         },
         {
-            "msg": "a",
-            "bitlen": 8,
-            "digest": "ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb",
+            'msg': 'a',
+            'bitlen': 8,
+            'digest': 'ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb',
         },
         {
-            "msg": Utils.ba("00"),
-            "bitlen": 1,
-            "digest": "bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375",
+            'msg': Utils.ba('00'),
+            'bitlen': 1,
+            'digest': 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375',
         },
         {
-            "msg": Utils.ba("80"),
-            "bitlen": 2,
-            "digest": "18f331f626210ff9bad6995d8cff6e891adba50eb2fdbddcaa921221cdc333ae",
+            'msg': Utils.ba('80'),
+            'bitlen': 2,
+            'digest': '18f331f626210ff9bad6995d8cff6e891adba50eb2fdbddcaa921221cdc333ae',
         },
     ]
 
     for test in tests:
-        check(test["msg"], test["bitlen"], test["digest"])
+        check(test['msg'], test['bitlen'], test['digest'])
 
     assert (
-        sha256bit(b"\x00", bitlen=1).hexdigest()
-        == "bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375"
+        sha256bit(b'\x00', bitlen=1).hexdigest() == 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
     )
 
 
 def check_against_nist_cavp():
     print("check against 'short' and 'long' bit oriented test vectors from NIST CAVP")
     # (https://csrc.nist.gov/CSRC/media/Projects/Cryptographic-Algorithm-Validation-Program/documents/shs/shabittestvectors.zip)
 
     from pathlib import Path
 
     resource_path = Path(__file__).parent
-    for tvFile in ["SHA256ShortMsg.rsp", "SHA256LongMsg.rsp"]:
+    for tvFile in ['SHA256ShortMsg.rsp', 'SHA256LongMsg.rsp']:
         tvPath = resource_path.joinpath(tvFile)
         with open(tvPath) as f:
             for line in f:
-                if line.startswith("Len"):
-                    bitlen = int(re.search(r"Len = (.+)", line).group(1))
-                if line.startswith("Msg"):
-                    msg = Utils.ba(re.search(r"Msg = (.+)", line).group(1))
+                if line.startswith('Len'):
+                    bitlen = int(re.search(r'Len = (.+)', line).group(1))
+                if line.startswith('Msg'):
+                    msg = Utils.ba(re.search(r'Msg = (.+)', line).group(1))
                     if bitlen == 0:
                         msg = bytes(0)
-                if line.startswith("MD"):
-                    MD = re.search(r"MD = (.+)", line).group(1)
+                if line.startswith('MD'):
+                    MD = re.search(r'MD = (.+)', line).group(1)
                     check(msg, bitlen, MD)
 
 
 def check_api():
-    print("check API")
+    print('check API')
     msg = msg_generator(bytes(0), 300 * 8)
     expected = hashlib.sha256(msg).digest()
     # print(Utils.hexstr(msg))
     # print(Utils.hexstr(expected))
     assert expected == sha256bit(msg).digest()
     for len1 in range(0, len(msg) * 8):
         dut1 = sha256bit()
@@ -153,15 +154,19 @@
             dut.update(chunk, bitlen=len(chunk) * 8)
             p += len1
             remaining -= len1
         assert expected == dut.digest()
         state = dut.export_state()
         dut2 = sha256bit.import_state(state)
         assert expected == dut2.digest()
+    dut = sha256bit(b'\x00', bitlen=1)
+    state = dut.export_state()
+    dut2 = sha256bit.import_state(state)
+    assert dut2.hexdigest() == 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     check_api()
     check_hardcoded_test_vectors()
     check_against_nist_cavp()
     check_against_hashlib(n_seeds=3, max_length=1024 * 4)
-    print("All test PASS")
+    print('All test PASS')
```

### Comparing `sha256bit-0.0.7/.gitignore` & `sha256bit-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/LICENSE` & `sha256bit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/README.md` & `sha256bit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.7/hatch.toml` & `sha256bit-0.0.8/hatch.toml`

 * *Files identical despite different names*

