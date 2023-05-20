# Comparing `tmp/sha256bit-0.0.6.tar.gz` & `tmp/sha256bit-0.0.7.tar.gz`

## Comparing `sha256bit-0.0.6.tar` & `sha256bit-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sha256bit-0.0.6/publish_to_pypi
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 sha256bit-0.0.6/sha256bit/__init__.py
--rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.6/test/SHA256LongMsg.rsp
--rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.6/test/SHA256ShortMsg.rsp
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sha256bit-0.0.6/test/__init__.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 sha256bit-0.0.6/test/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.6/LICENSE
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 sha256bit-0.0.6/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 sha256bit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 sha256bit-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sha256bit-0.0.7/publish_to_pypi
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sha256bit-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 sha256bit-0.0.7/sha256bit/__init__.py
+-rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/SHA256LongMsg.rsp
+-rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/SHA256ShortMsg.rsp
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/__init__.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_api.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_cavp.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_hardcoded.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sha256bit-0.0.7/test/test_vs_hashlib.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 sha256bit-0.0.7/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 sha256bit-0.0.7/hatch.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 sha256bit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 sha256bit-0.0.7/PKG-INFO
```

### Comparing `sha256bit-0.0.6/sha256bit/__init__.py` & `sha256bit-0.0.7/sha256bit/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,160 @@
 import copy
 import struct
 import binascii
 
-class sha256bit(object):
 
+class sha256bit(object):
     F32 = 0xFFFFFFFF
 
-    _k = [0x428a2f98, 0x71374491, 0xb5c0fbcf, 0xe9b5dba5,
-        0x3956c25b, 0x59f111f1, 0x923f82a4, 0xab1c5ed5,
-        0xd807aa98, 0x12835b01, 0x243185be, 0x550c7dc3,
-        0x72be5d74, 0x80deb1fe, 0x9bdc06a7, 0xc19bf174,
-        0xe49b69c1, 0xefbe4786, 0x0fc19dc6, 0x240ca1cc,
-        0x2de92c6f, 0x4a7484aa, 0x5cb0a9dc, 0x76f988da,
-        0x983e5152, 0xa831c66d, 0xb00327c8, 0xbf597fc7,
-        0xc6e00bf3, 0xd5a79147, 0x06ca6351, 0x14292967,
-        0x27b70a85, 0x2e1b2138, 0x4d2c6dfc, 0x53380d13,
-        0x650a7354, 0x766a0abb, 0x81c2c92e, 0x92722c85,
-        0xa2bfe8a1, 0xa81a664b, 0xc24b8b70, 0xc76c51a3,
-        0xd192e819, 0xd6990624, 0xf40e3585, 0x106aa070,
-        0x19a4c116, 0x1e376c08, 0x2748774c, 0x34b0bcb5,
-        0x391c0cb3, 0x4ed8aa4a, 0x5b9cca4f, 0x682e6ff3,
-        0x748f82ee, 0x78a5636f, 0x84c87814, 0x8cc70208,
-        0x90befffa, 0xa4506ceb, 0xbef9a3f7, 0xc67178f2]
-
-    _h_init = [0x6a09e667, 0xbb67ae85, 0x3c6ef372, 0xa54ff53a,
-        0x510e527f, 0x9b05688c, 0x1f83d9ab, 0x5be0cd19]
+    _k = [
+        0x428A2F98,
+        0x71374491,
+        0xB5C0FBCF,
+        0xE9B5DBA5,
+        0x3956C25B,
+        0x59F111F1,
+        0x923F82A4,
+        0xAB1C5ED5,
+        0xD807AA98,
+        0x12835B01,
+        0x243185BE,
+        0x550C7DC3,
+        0x72BE5D74,
+        0x80DEB1FE,
+        0x9BDC06A7,
+        0xC19BF174,
+        0xE49B69C1,
+        0xEFBE4786,
+        0x0FC19DC6,
+        0x240CA1CC,
+        0x2DE92C6F,
+        0x4A7484AA,
+        0x5CB0A9DC,
+        0x76F988DA,
+        0x983E5152,
+        0xA831C66D,
+        0xB00327C8,
+        0xBF597FC7,
+        0xC6E00BF3,
+        0xD5A79147,
+        0x06CA6351,
+        0x14292967,
+        0x27B70A85,
+        0x2E1B2138,
+        0x4D2C6DFC,
+        0x53380D13,
+        0x650A7354,
+        0x766A0ABB,
+        0x81C2C92E,
+        0x92722C85,
+        0xA2BFE8A1,
+        0xA81A664B,
+        0xC24B8B70,
+        0xC76C51A3,
+        0xD192E819,
+        0xD6990624,
+        0xF40E3585,
+        0x106AA070,
+        0x19A4C116,
+        0x1E376C08,
+        0x2748774C,
+        0x34B0BCB5,
+        0x391C0CB3,
+        0x4ED8AA4A,
+        0x5B9CCA4F,
+        0x682E6FF3,
+        0x748F82EE,
+        0x78A5636F,
+        0x84C87814,
+        0x8CC70208,
+        0x90BEFFFA,
+        0xA4506CEB,
+        0xBEF9A3F7,
+        0xC67178F2,
+    ]
+
+    _h_init = [
+        0x6A09E667,
+        0xBB67AE85,
+        0x3C6EF372,
+        0xA54FF53A,
+        0x510E527F,
+        0x9B05688C,
+        0x1F83D9AB,
+        0x5BE0CD19,
+    ]
 
     @staticmethod
     def _rotr(x, y):
         return ((x >> y) | (x << (32 - y))) & sha256bit.F32
 
-
     @staticmethod
     def _maj(x, y, z):
         return (x & y) ^ (x & z) ^ (y & z)
 
-
     @staticmethod
     def _ch(x, y, z):
         return (x & y) ^ ((~x) & z)
-    
+
     _output_size = 8
     blocksize = 1
     block_size = 64
     digest_size = 32
 
     def __init__(self, m=None, *, bitlen=None):
-        """ SHA-256 implementation supporting bit granularity for message input length.
-            API is the same as hashlib.
+        """SHA-256 implementation supporting bit granularity for message input length.
+        API is the same as hashlib.
         """
         self._counter = 0
         self._cache = bytearray()
         self._h = copy.deepcopy(sha256bit._h_init)
-        self._has_bitlen = False 
+        self._has_bitlen = False
         self._digest = None
-        self.update(m,bitlen=bitlen)
+        self.update(m, bitlen=bitlen)
 
     def export_state(self):
         if self._digest is None:
             h = self._h
             c = self._cache
         else:
             h = self._digest
             c = None
-        return {"h":h, "cnt":self._counter, "cache":c}
+        return {"h": h, "cnt": self._counter, "cache": c}
 
     @staticmethod
     def import_state(state):
-        o=sha256bit()
+        o = sha256bit()
         o._counter = state["cnt"]
         if 0 != (o._counter % 8):
             o._has_bitlen = True
         if state["cache"] is None:
             o._digest = state["h"]
             o._h = None
             o._cache = None
         else:
             o._h = state["h"]
             o._cache = bytearray(state["cache"])
         return o
 
     def _compress(self, c):
         w = [0] * 64
-        w[0:16] = struct.unpack('!16L', c)
+        w[0:16] = struct.unpack("!16L", c)
         for i in range(16, 64):
-            s0 = sha256bit._rotr(w[i-15], 7) ^ sha256bit._rotr(w[i-15], 18) ^ (w[i-15] >> 3)
-            s1 = sha256bit._rotr(w[i-2], 17) ^ sha256bit._rotr(w[i-2], 19) ^ (w[i-2] >> 10)
-            w[i] = (w[i-16] + s0 + w[i-7] + s1) & sha256bit.F32
+            s0 = (
+                sha256bit._rotr(w[i - 15], 7)
+                ^ sha256bit._rotr(w[i - 15], 18)
+                ^ (w[i - 15] >> 3)
+            )
+            s1 = (
+                sha256bit._rotr(w[i - 2], 17)
+                ^ sha256bit._rotr(w[i - 2], 19)
+                ^ (w[i - 2] >> 10)
+            )
+            w[i] = (w[i - 16] + s0 + w[i - 7] + s1) & sha256bit.F32
 
         a, b, c, d, e, f, g, h = self._h
 
         for i in range(64):
             s0 = sha256bit._rotr(a, 2) ^ sha256bit._rotr(a, 13) ^ sha256bit._rotr(a, 22)
             t2 = s0 + sha256bit._maj(a, b, c)
             s1 = sha256bit._rotr(e, 6) ^ sha256bit._rotr(e, 11) ^ sha256bit._rotr(e, 25)
@@ -105,82 +169,85 @@
             b = a
             a = (t1 + t2) & sha256bit.F32
 
         for i, (x, y) in enumerate(zip(self._h, [a, b, c, d, e, f, g, h])):
             self._h[i] = (x + y) & sha256bit.F32
 
     def update(self, m, *, bitlen=None):
-        """ Update the hash object with the bytes in data. Repeated calls
-            are equivalent to a single call with the concatenation of all
-            the arguments.
+        """Update the hash object with the bytes in data. Repeated calls
+        are equivalent to a single call with the concatenation of all
+        the arguments.
         """
         if not m:
             return
         assert not self._has_bitlen, "we support bitlen only for last call"
         if bitlen is not None:
-            if 0 != (bitlen%8):
+            if 0 != (bitlen % 8):
                 self._has_bitlen = True
             else:
-                assert bitlen == len(m)*8, "bitLen=%d, len(m)*8=%d"%(bitlen,len(m)*8)
+                assert bitlen == len(m) * 8, "bitLen=%d, len(m)*8=%d" % (
+                    bitlen,
+                    len(m) * 8,
+                )
             self._counter += bitlen
         else:
-            self._counter += len(m)*8
-        
+            self._counter += len(m) * 8
+
         self._cache += m
-        
+
         while len(self._cache) > 64:
             self._compress(self._cache[:64])
             self._cache = self._cache[64:]
 
         if len(self._cache) == 64:
             if 0 != (self._counter % 8):
                 assert self._has_bitlen
                 # at least one bit is issing to form a full block, nothing to do
             else:
                 self._compress(self._cache[:64])
                 self._cache = self._cache[64:]
 
     def _pad(self):
         lastBlockBitLen = self._counter % 512
-        lastBlockFullBytesCnt = lastBlockBitLen//8
+        lastBlockFullBytesCnt = lastBlockBitLen // 8
         if lastBlockBitLen < 448:
             padlen = 55 - lastBlockFullBytesCnt
         else:
             padlen = 119 - lastBlockFullBytesCnt
         if False:
-            print(lastBlockBitLen,lastBlockFullBytesCnt,padlen, len(self._cache))
-        
+            print(lastBlockBitLen, lastBlockFullBytesCnt, padlen, len(self._cache))
+
         shift = self._counter % 8
-        if shift>0 and (len(self._cache)>0):
-            mask = 0xFF << (8-shift)
+        if shift > 0 and (len(self._cache) > 0):
+            mask = 0xFF << (8 - shift)
             self._cache[-1] = (self._cache[-1] & mask) | (0x80 >> shift)
         else:
-            self._cache += b'\x80'
-        self._cache += (b'\x00' * padlen) + self._counter.to_bytes(8,byteorder='big')
+            self._cache += b"\x80"
+        self._cache += (b"\x00" * padlen) + self._counter.to_bytes(8, byteorder="big")
         if False:
             from pysatl import Utils
-            print("counter=%d (0x%x)"%(self._counter,self._counter))
+
+            print("counter=%d (0x%x)" % (self._counter, self._counter))
             print(Utils.hexstr(self._cache))
-        assert len(self._cache) in [64,128], "len(self._cache)=%d"%len(self._cache)
-    
+        assert len(self._cache) in [64, 128], "len(self._cache)=%d" % len(self._cache)
+
     def digest(self):
-        """ Return the digest of the bytes passed to the update() method
-            so far as a bytes object.
+        """Return the digest of the bytes passed to the update() method
+        so far as a bytes object.
         """
         if self._digest is not None:
             return self._digest
         self._pad()
-        blocks = [self._cache[i:i+64] for i in range(0, len(self._cache), 64)]
+        blocks = [self._cache[i : i + 64] for i in range(0, len(self._cache), 64)]
         for b in blocks:
             self._compress(b)
-        data = [struct.pack('!L', i) for i in self._h[:self._output_size]]
-        self._digest = b''.join(data)
+        data = [struct.pack("!L", i) for i in self._h[: self._output_size]]
+        self._digest = b"".join(data)
         self._cache = None
         self._h = None
         return self._digest
 
     def hexdigest(self):
-        """ Like digest() except the digest is returned as a string
-            of double length, containing only hexadecimal digits.
+        """Like digest() except the digest is returned as a string
+        of double length, containing only hexadecimal digits.
         """
-        return binascii.hexlify(self.digest()).decode('ascii')
-    
+        return binascii.hexlify(self.digest()).decode("ascii")
```

### Comparing `sha256bit-0.0.6/test/SHA256LongMsg.rsp` & `sha256bit-0.0.7/test/SHA256LongMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.6/test/SHA256ShortMsg.rsp` & `sha256bit-0.0.7/test/SHA256ShortMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.6/test/test.py` & `sha256bit-0.0.7/test/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,145 +1,167 @@
 import hashlib
 from pysatl import Utils
 import re
 from sha256bit import sha256bit
 
 
-def block_generator(seed,msg_bitlen):
+def block_generator(seed, msg_bitlen):
     l2block = hashlib.sha256(seed).digest()
     l2block += hashlib.sha256(l2block).digest()
-    blockBitLen = len(l2block)*8
-    assert blockBitLen == 64*8
-    bitlen=0
-    while(bitlen+blockBitLen<msg_bitlen):
+    blockBitLen = len(l2block) * 8
+    assert blockBitLen == 64 * 8
+    bitlen = 0
+    while bitlen + blockBitLen < msg_bitlen:
         yield l2block
         bitlen += blockBitLen
         l2block = hashlib.sha256(l2block).digest()
         l2block += hashlib.sha256(l2block).digest()
     # last block
     lastBlockBitLen = msg_bitlen % 512
     if 0 != lastBlockBitLen:
-        lastBlockFullByteLen = (lastBlockBitLen+7)//8
+        lastBlockFullByteLen = (lastBlockBitLen + 7) // 8
         l2block = bytearray(l2block[0:lastBlockFullByteLen])
         assert len(l2block) == lastBlockFullByteLen
-        mask = 0xFF & (0xFF << (8-(msg_bitlen % 8)))
+        mask = 0xFF & (0xFF << (8 - (msg_bitlen % 8)))
         if 0 != mask:
-            l2block[-1] &= mask 
+            l2block[-1] &= mask
     yield l2block
 
+
 def msg_generator(seed, msg_bitlen):
     o = bytearray()
-    for b in block_generator(seed,msg_bitlen):
-        o += b 
+    for b in block_generator(seed, msg_bitlen):
+        o += b
     return o
 
-def check_against_hashlib(n_seeds=3,max_length=1024*4):
+
+def check_against_hashlib(n_seeds=3, max_length=1024 * 4):
     print("check against hashlib")
 
     assert hashlib.sha256("abc".encode()).digest() == sha256bit("abc".encode()).digest()
 
-    def check_against_hashlib(seed,msg_bitlen):
+    def check_against_hashlib(seed, msg_bitlen):
         expected = hashlib.sha256()
         dut = sha256bit()
-        for block in block_generator(seed,msg_bitlen):
-            #print(Utils.hexstr(block))
+        for block in block_generator(seed, msg_bitlen):
+            # print(Utils.hexstr(block))
             expected.update(block)
             dut.update(block)
         assert expected.digest() == dut.digest()
 
     for seedByte in range(0, n_seeds):
-        for msgBitLen in range(0,max_length, 8):
+        for msgBitLen in range(0, max_length, 8):
             seed = bytearray([seedByte])
-            check_against_hashlib(seed,msgBitLen)
+            check_against_hashlib(seed, msgBitLen)
+
 
 def check(msg, bitlen, sig):
-        m = sha256bit()
-        if isinstance(msg,str):
-            msg=msg.encode('ascii')
-        descr = "msg      = "+Utils.hexstr(msg)+"\n"
-        descr+= "bitlen   = %d\n"%bitlen
-        descr+= "expected = "+sig+"\n"
-        try:
-            
-            m.update(msg, bitlen=bitlen)
-            digest = m.hexdigest()
-        except Exception as e:
-            print(descr)
-            raise e
-        errMsg ='\n'
-        errMsg+= descr
-        errMsg+= "digest   = "+digest+"\n"
-        assert digest == sig, errMsg
+    m = sha256bit()
+    if isinstance(msg, str):
+        msg = msg.encode("ascii")
+    descr = "msg      = " + Utils.hexstr(msg) + "\n"
+    descr += "bitlen   = %d\n" % bitlen
+    descr += "expected = " + sig + "\n"
+    try:
+        m.update(msg, bitlen=bitlen)
+        digest = m.hexdigest()
+    except Exception as e:
+        print(descr)
+        raise e
+    errMsg = "\n"
+    errMsg += descr
+    errMsg += "digest   = " + digest + "\n"
+    assert digest == sig, errMsg
+
 
 def check_hardcoded_test_vectors():
     print("check few minimal hardcoded test vectors")
-    
+
     tests = [
-        {"msg":"","bitlen":0,"digest":'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'},
-        {"msg":"a","bitlen":8,"digest":'ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb'},
-        {"msg":Utils.ba("00"),"bitlen":1,"digest":'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'},
-        {"msg":Utils.ba("80"),"bitlen":2,"digest":'18f331f626210ff9bad6995d8cff6e891adba50eb2fdbddcaa921221cdc333ae'},
+        {
+            "msg": "",
+            "bitlen": 0,
+            "digest": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+        },
+        {
+            "msg": "a",
+            "bitlen": 8,
+            "digest": "ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb",
+        },
+        {
+            "msg": Utils.ba("00"),
+            "bitlen": 1,
+            "digest": "bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375",
+        },
+        {
+            "msg": Utils.ba("80"),
+            "bitlen": 2,
+            "digest": "18f331f626210ff9bad6995d8cff6e891adba50eb2fdbddcaa921221cdc333ae",
+        },
     ]
 
     for test in tests:
-        check(test["msg"],test["bitlen"],test["digest"])
+        check(test["msg"], test["bitlen"], test["digest"])
 
-    assert sha256bit(b'\x00',bitlen=1).hexdigest() == 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
+    assert (
+        sha256bit(b"\x00", bitlen=1).hexdigest()
+        == "bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375"
+    )
 
 
 def check_against_nist_cavp():
     print("check against 'short' and 'long' bit oriented test vectors from NIST CAVP")
     # (https://csrc.nist.gov/CSRC/media/Projects/Cryptographic-Algorithm-Validation-Program/documents/shs/shabittestvectors.zip)
 
     from pathlib import Path
-    resource_path = Path(__file__).parent 
-    for tvFile in ["SHA256ShortMsg.rsp","SHA256LongMsg.rsp"]:
+
+    resource_path = Path(__file__).parent
+    for tvFile in ["SHA256ShortMsg.rsp", "SHA256LongMsg.rsp"]:
         tvPath = resource_path.joinpath(tvFile)
         with open(tvPath) as f:
-            for l in f:
-                if l.startswith("Len"):
-                    bitlen = int(re.search(r"Len = (.+)",l).group(1))
-                if l.startswith("Msg"):
-                    msg = Utils.ba(re.search(r"Msg = (.+)",l).group(1))
-                    if bitlen==0:
-                        msg=bytes(0)
-                if l.startswith("MD"):
-                    MD = re.search(r"MD = (.+)",l).group(1)
-                    check(msg,bitlen,MD)
+            for line in f:
+                if line.startswith("Len"):
+                    bitlen = int(re.search(r"Len = (.+)", line).group(1))
+                if line.startswith("Msg"):
+                    msg = Utils.ba(re.search(r"Msg = (.+)", line).group(1))
+                    if bitlen == 0:
+                        msg = bytes(0)
+                if line.startswith("MD"):
+                    MD = re.search(r"MD = (.+)", line).group(1)
+                    check(msg, bitlen, MD)
+
 
 def check_api():
     print("check API")
-    msg = msg_generator(bytes(0),300*8)
+    msg = msg_generator(bytes(0), 300 * 8)
     expected = hashlib.sha256(msg).digest()
-    #print(Utils.hexstr(msg))
-    #print(Utils.hexstr(expected))
+    # print(Utils.hexstr(msg))
+    # print(Utils.hexstr(expected))
     assert expected == sha256bit(msg).digest()
-    for len1 in range(0,len(msg)*8):
+    for len1 in range(0, len(msg) * 8):
         dut1 = sha256bit()
         dut1.update(msg[:len1])
         state = dut1.export_state()
         dut2 = sha256bit.import_state(state)
         dut2.update(msg[len1:])
         assert expected == dut2.digest()
-    for len1 in range(1,len(msg)*8):
+    for len1 in range(1, len(msg) * 8):
         dut = sha256bit()
         remaining = len(msg)
         p = 0
-        while remaining>0:
-            chunk = msg[p:p+len1]
-            dut.update(chunk, bitlen=len(chunk)*8)
+        while remaining > 0:
+            chunk = msg[p : p + len1]
+            dut.update(chunk, bitlen=len(chunk) * 8)
             p += len1
             remaining -= len1
         assert expected == dut.digest()
         state = dut.export_state()
         dut2 = sha256bit.import_state(state)
         assert expected == dut2.digest()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     check_api()
     check_hardcoded_test_vectors()
     check_against_nist_cavp()
-    check_against_hashlib(n_seeds=3,max_length=1024*4)
+    check_against_hashlib(n_seeds=3, max_length=1024 * 4)
     print("All test PASS")
-                
-            
-
```

### Comparing `sha256bit-0.0.6/.gitignore` & `sha256bit-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.6/LICENSE` & `sha256bit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.6/pyproject.toml` & `sha256bit-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.6/PKG-INFO` & `sha256bit-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-Metadata-Version: 2.1
-Name: sha256bit
-Version: 0.0.6
-Summary: SHA256 with bit granularity for message input length
-Project-URL: Homepage, https://github.com/sebastien-riou/sha256bit
-Project-URL: Bug Tracker, https://github.com/sebastien-riou/sha256bit/issues
-Author: Sebastien Riou
-License-File: LICENSE
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # sha256bit
+
+
+| | |
+| --- | --- |
+| CI/CD | [![CI - Test](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml) [![CD - Build](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/sha256bit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/sha256bits/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hsha256bit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/sha256bit/) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) |
+
+
 Pure python implementation of SHA256 with features which are often lacking:
 - bit granularity for message input length
 - import/export API to "persist" the state in the middle of a hash computation
 
 ## Installation
 
     python3 -m pip install sha256bit
@@ -41,17 +36,32 @@
     >>> h1 = sha256bit("a".encode())
     >>> state = h1.export_state()
     >>> h2 = sha256bit.import_state(state)
     >>> h2.update("bc".encode())
     >>> h2.hexdigest()
     'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
 
-## Build the package
-````
-python3 -m build
-````
+## Test with `pytest`
 
-## Test
+    pytest-3
+
+## Test without `pytest`
 Tests can run without creating/installing the package:
-````
-python3 -m test.test
-````
+
+    python3 -m test.test
+
+
+you can also run each test separately:
+
+    python3 -m test.test_api
+    python3 -m test.test_cavp
+    python3 -m test.test_hardcoded
+    python3 -m test.test_vs_hashlib
+
+## Build the package
+Build is done using `hatchling`
+
+    python3 -m build
+
+
+## Create a new version
+Version is managed by `hatch-vcs`, you just need to create a tag in github.
```

