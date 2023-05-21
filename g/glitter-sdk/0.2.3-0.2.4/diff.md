# Comparing `tmp/glitter_sdk-0.2.3.tar.gz` & `tmp/glitter_sdk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glitter_sdk-0.2.3.tar", max compression
+gzip compressed data, was "glitter_sdk-0.2.4.tar", max compression
```

## Comparing `glitter_sdk-0.2.3.tar` & `glitter_sdk-0.2.4.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0     1073 2023-03-05 15:04:49.729817 glitter_sdk-0.2.3/LICENSE
--rw-r--r--   0        0        0     1912 2023-04-01 03:19:53.336155 glitter_sdk-0.2.3/README.md
--rw-r--r--   0        0        0       13 2023-03-13 11:08:58.347247 glitter_sdk-0.2.3/glitter_sdk/.gitignore
--rw-r--r--   0        0        0      163 2023-03-13 11:08:58.347884 glitter_sdk-0.2.3/glitter_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 11:08:58.347981 glitter_sdk-0.2.3/glitter_sdk/client/__init__.py
--rw-r--r--   0        0        0      196 2023-04-01 03:19:53.341248 glitter_sdk-0.2.3/glitter_sdk/client/lcd/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 11:08:58.348980 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/__init__.py
--rw-r--r--   0        0        0      812 2023-03-13 11:08:58.349462 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/_base.py
--rw-r--r--   0        0        0     1491 2023-03-26 07:42:53.767656 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/auth.py
--rw-r--r--   0        0        0     3436 2023-03-13 11:08:58.350610 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/authz.py
--rw-r--r--   0        0        0     2471 2023-04-28 15:30:57.343890 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/bank.py
--rw-r--r--   0        0        0     4394 2023-03-13 11:08:58.351558 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/distribution.py
--rw-r--r--   0        0        0     3632 2023-03-13 11:08:58.352180 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/feegrant.py
--rw-r--r--   0        0        0    10274 2023-03-13 11:08:58.352841 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/gov.py
--rw-r--r--   0        0        0      587 2023-03-13 11:08:58.353005 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/ibc.py
--rw-r--r--   0        0        0      762 2023-03-13 11:08:58.353409 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/ibc_transfer.py
--rw-r--r--   0        0        0     2330 2023-03-13 11:08:58.353973 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/mint.py
--rw-r--r--   0        0        0     3776 2023-03-13 11:08:58.354544 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/slashing.py
--rw-r--r--   0        0        0    13196 2023-03-13 11:08:58.355132 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/staking.py
--rw-r--r--   0        0        0     3065 2023-03-13 11:08:58.355281 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/tendermint.py
--rw-r--r--   0        0        0    14761 2023-04-01 03:49:21.407472 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/tx.py
--rw-r--r--   0        0        0     5011 2023-03-13 11:08:58.356484 glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/wasm.py
--rw-r--r--   0        0        0      878 2023-03-13 11:08:58.357495 glitter_sdk-0.2.3/glitter_sdk/client/lcd/constants/CLIENT.py
--rw-r--r--   0        0        0        0 2023-03-13 11:08:58.357577 glitter_sdk-0.2.3/glitter_sdk/client/lcd/constants/__init__.py
--rw-r--r--   0        0        0    14293 2023-05-01 08:56:31.893244 glitter_sdk-0.2.3/glitter_sdk/client/lcd/db.py
--rw-r--r--   0        0        0    11243 2023-04-28 15:29:59.244706 glitter_sdk-0.2.3/glitter_sdk/client/lcd/lcdclient.py
--rw-r--r--   0        0        0     1803 2023-03-13 11:08:58.358639 glitter_sdk-0.2.3/glitter_sdk/client/lcd/lcdutils.py
--rw-r--r--   0        0        0     2394 2023-03-13 11:08:58.359148 glitter_sdk-0.2.3/glitter_sdk/client/lcd/params.py
--rw-r--r--   0        0        0      949 2023-03-27 15:23:06.688797 glitter_sdk-0.2.3/glitter_sdk/core/__init__.py
--rw-r--r--   0        0        0      661 2023-03-26 07:20:19.533891 glitter_sdk-0.2.3/glitter_sdk/core/auth/__init__.py
--rw-r--r--   0        0        0      656 2023-03-26 07:19:34.210859 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/__init__.py
--rw-r--r--   0        0        0     1835 2023-03-26 07:18:28.803583 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/account.py
--rw-r--r--   0        0        0     2953 2023-03-13 11:08:58.362249 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/base_account.py
--rw-r--r--   0        0        0     3965 2023-03-13 11:08:58.362787 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/base_vesting_account.py
--rw-r--r--   0        0        0     2731 2023-03-13 11:08:58.363597 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/continuous_vesting_account.py
--rw-r--r--   0        0        0     2498 2023-03-13 11:08:58.364171 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/delayed_vesting_account.py
--rw-r--r--   0        0        0     2340 2023-03-26 07:47:19.134258 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/eth_account.py
--rw-r--r--   0        0        0     4441 2023-03-13 11:08:58.364906 glitter_sdk-0.2.3/glitter_sdk/core/auth/data/periodic_vesting_account.py
--rw-r--r--   0        0        0      331 2023-03-13 11:08:58.365065 glitter_sdk-0.2.3/glitter_sdk/core/auth/msgs/__init__.py
--rw-r--r--   0        0        0     2921 2023-03-13 11:08:58.365643 glitter_sdk-0.2.3/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py
--rw-r--r--   0        0        0     2838 2023-03-13 11:08:58.366178 glitter_sdk-0.2.3/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py
--rw-r--r--   0        0        0     1620 2023-03-13 11:08:58.366670 glitter_sdk-0.2.3/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py
--rw-r--r--   0        0        0      446 2023-03-13 11:08:58.366825 glitter_sdk-0.2.3/glitter_sdk/core/authz/__init__.py
--rw-r--r--   0        0        0     9613 2023-03-13 11:08:58.367344 glitter_sdk-0.2.3/glitter_sdk/core/authz/data.py
--rw-r--r--   0        0        0     6109 2023-03-13 11:08:58.367944 glitter_sdk-0.2.3/glitter_sdk/core/authz/msgs.py
--rw-r--r--   0        0        0      149 2023-03-13 11:08:58.368579 glitter_sdk-0.2.3/glitter_sdk/core/bank/__init__.py
--rw-r--r--   0        0        0     7099 2023-03-13 11:08:58.369139 glitter_sdk-0.2.3/glitter_sdk/core/bank/msgs.py
--rw-r--r--   0        0        0     5009 2023-03-13 11:08:58.369678 glitter_sdk-0.2.3/glitter_sdk/core/bech32.py
--rw-r--r--   0        0        0     1616 2023-03-13 11:08:58.369822 glitter_sdk-0.2.3/glitter_sdk/core/block.py
--rw-r--r--   0        0        0     2724 2023-03-13 11:08:58.370319 glitter_sdk-0.2.3/glitter_sdk/core/broadcast.py
--rw-r--r--   0        0        0     7746 2023-03-13 11:08:58.370786 glitter_sdk-0.2.3/glitter_sdk/core/coin.py
--rw-r--r--   0        0        0     8360 2023-03-13 11:08:58.371350 glitter_sdk-0.2.3/glitter_sdk/core/coins.py
--rw-r--r--   0        0        0     2707 2023-03-13 11:08:58.371947 glitter_sdk-0.2.3/glitter_sdk/core/compact_bit_array.py
--rw-r--r--   0        0        0       71 2023-03-13 11:08:58.372138 glitter_sdk-0.2.3/glitter_sdk/core/crisis/__init__.py
--rw-r--r--   0        0        0     2069 2023-03-13 11:08:58.372665 glitter_sdk-0.2.3/glitter_sdk/core/crisis/msgs.py
--rw-r--r--   0        0        0     1085 2023-03-13 11:08:58.373096 glitter_sdk-0.2.3/glitter_sdk/core/deposit.py
--rw-r--r--   0        0        0      371 2023-03-13 11:08:58.373255 glitter_sdk-0.2.3/glitter_sdk/core/distribution/__init__.py
--rw-r--r--   0        0        0     6940 2023-03-13 11:08:58.373671 glitter_sdk-0.2.3/glitter_sdk/core/distribution/msgs.py
--rw-r--r--   0        0        0     2692 2023-03-13 11:08:58.374225 glitter_sdk-0.2.3/glitter_sdk/core/distribution/proposals.py
--rw-r--r--   0        0        0     2008 2023-03-13 11:08:58.374552 glitter_sdk-0.2.3/glitter_sdk/core/fee.py
--rw-r--r--   0        0        0      297 2023-03-13 11:08:58.374699 glitter_sdk-0.2.3/glitter_sdk/core/feegrant/__init__.py
--rw-r--r--   0        0        0     9141 2023-03-13 11:08:58.375006 glitter_sdk-0.2.3/glitter_sdk/core/feegrant/data.py
--rw-r--r--   0        0        0     3178 2023-03-13 11:08:58.375537 glitter_sdk-0.2.3/glitter_sdk/core/feegrant/msgs.py
--rw-r--r--   0        0        0      412 2023-03-13 11:08:58.376076 glitter_sdk-0.2.3/glitter_sdk/core/gov/__init__.py
--rw-r--r--   0        0        0     6154 2023-03-13 11:08:58.376639 glitter_sdk-0.2.3/glitter_sdk/core/gov/data.py
--rw-r--r--   0        0        0     6516 2023-03-13 11:08:58.377173 glitter_sdk-0.2.3/glitter_sdk/core/gov/msgs.py
--rw-r--r--   0        0        0     1695 2023-03-13 11:08:58.377677 glitter_sdk-0.2.3/glitter_sdk/core/gov/proposals.py
--rw-r--r--   0        0        0       47 2023-03-13 11:08:58.377816 glitter_sdk-0.2.3/glitter_sdk/core/ibc/__init__.py
--rw-r--r--   0        0        0      492 2023-03-13 11:08:58.377946 glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/__init__.py
--rw-r--r--   0        0        0     4811 2023-03-13 11:08:58.378397 glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/channel.py
--rw-r--r--   0        0        0     5323 2023-03-13 11:08:58.378944 glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/client.py
--rw-r--r--   0        0        0     1407 2023-03-13 11:08:58.379538 glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/commitment.py
--rw-r--r--   0        0        0     1947 2023-03-13 11:08:58.380124 glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/connection.py
--rw-r--r--   0        0        0      944 2023-03-13 11:08:58.380315 glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/__init__.py
--rw-r--r--   0        0        0    14728 2023-03-13 11:08:58.380848 glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/channel.py
--rw-r--r--   0        0        0     5942 2023-03-13 11:08:58.381430 glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/client.py
--rw-r--r--   0        0        0     9941 2023-03-13 11:08:58.381746 glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/connection.py
--rw-r--r--   0        0        0       80 2023-03-13 11:08:58.381885 glitter_sdk-0.2.3/glitter_sdk/core/ibc/proposals/__init__.py
--rw-r--r--   0        0        0     2205 2023-03-13 11:08:58.382371 glitter_sdk-0.2.3/glitter_sdk/core/ibc/proposals/proposals.py
--rw-r--r--   0        0        0      100 2023-03-13 11:08:58.382853 glitter_sdk-0.2.3/glitter_sdk/core/ibc_transfer/__init__.py
--rw-r--r--   0        0        0      703 2023-03-13 11:08:58.383309 glitter_sdk-0.2.3/glitter_sdk/core/ibc_transfer/data.py
--rw-r--r--   0        0        0     3369 2023-03-13 11:08:58.383789 glitter_sdk-0.2.3/glitter_sdk/core/ibc_transfer/msgs.py
--rw-r--r--   0        0        0     3334 2023-03-13 11:08:58.384170 glitter_sdk-0.2.3/glitter_sdk/core/mode_info.py
--rw-r--r--   0        0        0      805 2023-03-13 11:08:58.384582 glitter_sdk-0.2.3/glitter_sdk/core/msg.py
--rw-r--r--   0        0        0      188 2023-03-13 11:08:58.385068 glitter_sdk-0.2.3/glitter_sdk/core/msgs/__init__.py
--rw-r--r--   0        0        0     1033 2023-03-13 11:08:58.385519 glitter_sdk-0.2.3/glitter_sdk/core/msgs/argument.py
--rw-r--r--   0        0        0     3793 2023-03-13 11:08:58.385939 glitter_sdk-0.2.3/glitter_sdk/core/msgs/arguments.py
--rw-r--r--   0        0        0     2993 2023-03-13 11:08:58.386453 glitter_sdk-0.2.3/glitter_sdk/core/msgs/msgs.py
--rw-r--r--   0        0        0     2394 2023-03-13 11:08:58.386999 glitter_sdk-0.2.3/glitter_sdk/core/multisig.py
--rw-r--r--   0        0        0    11366 2023-03-13 11:08:58.387613 glitter_sdk-0.2.3/glitter_sdk/core/numeric.py
--rw-r--r--   0        0        0      114 2023-03-13 11:08:58.387760 glitter_sdk-0.2.3/glitter_sdk/core/params/__init__.py
--rw-r--r--   0        0        0     3325 2023-03-13 11:08:58.388287 glitter_sdk-0.2.3/glitter_sdk/core/params/proposals.py
--rw-r--r--   0        0        0    12728 2023-04-01 02:49:01.061356 glitter_sdk-0.2.3/glitter_sdk/core/public_key.py
--rw-r--r--   0        0        0     2621 2023-03-28 05:25:40.105427 glitter_sdk-0.2.3/glitter_sdk/core/sign_doc.py
--rw-r--r--   0        0        0     3550 2023-03-13 11:08:58.389976 glitter_sdk-0.2.3/glitter_sdk/core/signature_v2.py
--rw-r--r--   0        0        0       53 2023-03-13 11:08:58.390162 glitter_sdk-0.2.3/glitter_sdk/core/slashing/__init__.py
--rw-r--r--   0        0        0     1103 2023-03-13 11:08:58.390660 glitter_sdk-0.2.3/glitter_sdk/core/slashing/msgs.py
--rw-r--r--   0        0        0      661 2023-03-13 11:08:58.390909 glitter_sdk-0.2.3/glitter_sdk/core/staking/__init__.py
--rw-r--r--   0        0        0      429 2023-03-13 11:08:58.391064 glitter_sdk-0.2.3/glitter_sdk/core/staking/data/__init__.py
--rw-r--r--   0        0        0    11301 2023-03-13 11:08:58.391674 glitter_sdk-0.2.3/glitter_sdk/core/staking/data/delegation.py
--rw-r--r--   0        0        0     9625 2023-03-13 11:08:58.392264 glitter_sdk-0.2.3/glitter_sdk/core/staking/data/validator.py
--rw-r--r--   0        0        0    11092 2023-03-13 11:08:58.392899 glitter_sdk-0.2.3/glitter_sdk/core/staking/msgs.py
--rw-r--r--   0        0        0    15136 2023-03-28 05:26:03.502060 glitter_sdk-0.2.3/glitter_sdk/core/tx.py
--rw-r--r--   0        0        0      176 2023-03-13 11:08:58.393573 glitter_sdk-0.2.3/glitter_sdk/core/upgrade/__init__.py
--rw-r--r--   0        0        0      149 2023-03-13 11:08:58.393699 glitter_sdk-0.2.3/glitter_sdk/core/upgrade/data/__init__.py
--rw-r--r--   0        0        0     3330 2023-03-13 11:08:58.394221 glitter_sdk-0.2.3/glitter_sdk/core/upgrade/data/proposal.py
--rw-r--r--   0        0        0     2191 2023-03-13 11:08:58.394592 glitter_sdk-0.2.3/glitter_sdk/core/upgrade/plan.py
--rw-r--r--   0        0        0      315 2023-03-13 11:08:58.394733 glitter_sdk-0.2.3/glitter_sdk/core/wasm/__init__.py
--rw-r--r--   0        0        0     9320 2023-03-13 11:08:58.395189 glitter_sdk-0.2.3/glitter_sdk/core/wasm/data.py
--rw-r--r--   0        0        0    11303 2023-03-13 11:08:58.395703 glitter_sdk-0.2.3/glitter_sdk/core/wasm/msgs.py
--rw-r--r--   0        0        0    24195 2023-03-13 11:08:58.396188 glitter_sdk-0.2.3/glitter_sdk/core/wasm/proposals.py
--rw-r--r--   0        0        0      968 2023-04-09 13:57:19.944409 glitter_sdk-0.2.3/glitter_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-13 11:08:58.396859 glitter_sdk-0.2.3/glitter_sdk/key/__init__.py
--rw-r--r--   0        0        0     8381 2023-04-02 10:34:15.503189 glitter_sdk-0.2.3/glitter_sdk/key/key.py
--rw-r--r--   0        0        0     2365 2023-05-20 09:44:19.176923 glitter_sdk-0.2.3/glitter_sdk/key/mnemonic.py
--rw-r--r--   0        0        0     1846 2023-04-02 15:21:54.394109 glitter_sdk-0.2.3/glitter_sdk/key/raw.py
--rw-r--r--   0        0        0     3623 2023-03-26 02:18:44.107996 glitter_sdk-0.2.3/glitter_sdk/key/topub.py
--rw-r--r--   0        0        0        0 2023-03-13 11:08:58.398493 glitter_sdk-0.2.3/glitter_sdk/util/__init__.py
--rw-r--r--   0        0        0     1678 2023-03-13 11:08:58.398629 glitter_sdk-0.2.3/glitter_sdk/util/base.py
--rw-r--r--   0        0        0      878 2023-03-13 11:08:58.398824 glitter_sdk-0.2.3/glitter_sdk/util/constants/CLIENT.py
--rw-r--r--   0        0        0      679 2023-03-13 11:08:58.399255 glitter_sdk-0.2.3/glitter_sdk/util/constants/COMMAND.py
--rw-r--r--   0        0        0     1927 2023-03-13 11:08:58.399786 glitter_sdk-0.2.3/glitter_sdk/util/constants/CR.py
--rw-r--r--   0        0        0    12296 2023-03-13 11:08:58.400320 glitter_sdk-0.2.3/glitter_sdk/util/constants/ER.py
--rw-r--r--   0        0        0      370 2023-03-13 11:08:58.400832 glitter_sdk-0.2.3/glitter_sdk/util/constants/FIELD_TYPE.py
--rw-r--r--   0        0        0      214 2023-03-13 11:08:58.401339 glitter_sdk-0.2.3/glitter_sdk/util/constants/FLAG.py
--rw-r--r--   0        0        0      333 2023-03-13 11:08:58.401638 glitter_sdk-0.2.3/glitter_sdk/util/constants/SERVER_STATUS.py
--rw-r--r--   0        0        0        0 2023-03-13 11:08:58.401707 glitter_sdk-0.2.3/glitter_sdk/util/constants/__init__.py
--rw-r--r--   0        0        0     3253 2023-03-13 11:08:58.402210 glitter_sdk-0.2.3/glitter_sdk/util/contract.py
--rw-r--r--   0        0        0      199 2023-03-13 11:08:58.402331 glitter_sdk-0.2.3/glitter_sdk/util/converter.py
--rw-r--r--   0        0        0     1325 2023-04-06 08:22:21.253664 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/__init__.py
--rw-r--r--   0        0        0     1386 2023-04-06 03:28:40.834754 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/converter/__init__.py
--rw-r--r--   0        0        0     5017 2023-04-01 02:40:55.205070 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/converter/bech32.py
--rw-r--r--   0        0        0      230 2023-04-01 02:49:31.013058 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/__init__.py
--rw-r--r--   0        0        0      270 2023-04-01 02:49:31.022589 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/ecdsa.py
--rw-r--r--   0        0        0     6072 2023-04-01 02:40:55.205900 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/ecdsa_base.py
--rw-r--r--   0        0        0    14377 2023-04-01 02:40:55.206225 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py
--rw-r--r--   0        0        0    24914 2023-04-01 02:49:31.016470 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/ecdsa_python.py
--rw-r--r--   0        0        0    17376 2023-04-01 02:40:55.207175 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/openssl.py
--rw-r--r--   0        0        0     8962 2023-04-01 02:40:55.207492 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/utils.py
--rw-r--r--   0        0        0        0 2023-04-01 02:40:55.207660 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/eth/__init__.py
--rw-r--r--   0        0        0    55432 2023-04-01 02:49:31.019972 glitter_sdk-0.2.3/glitter_sdk/util/encrypt/eth/ethereum.py
--rw-r--r--   0        0        0      211 2023-03-13 11:08:58.402439 glitter_sdk-0.2.3/glitter_sdk/util/hash.py
--rw-r--r--   0        0        0      377 2023-04-30 02:03:55.614570 glitter_sdk-0.2.3/glitter_sdk/util/highlight.py
--rw-r--r--   0        0        0     1696 2023-03-13 11:08:58.403849 glitter_sdk-0.2.3/glitter_sdk/util/json.py
--rw-r--r--   0        0        0     1045 2023-03-13 11:08:58.404376 glitter_sdk-0.2.3/glitter_sdk/util/parse_authorization.py
--rw-r--r--   0        0        0     2550 2023-03-13 11:08:58.404831 glitter_sdk-0.2.3/glitter_sdk/util/parse_content.py
--rw-r--r--   0        0        0     3887 2023-03-13 11:08:58.405152 glitter_sdk-0.2.3/glitter_sdk/util/parse_msg.py
--rw-r--r--   0        0        0      732 2023-03-13 11:08:58.405653 glitter_sdk-0.2.3/glitter_sdk/util/parse_proto.py
--rw-r--r--   0        0        0     2837 2023-04-29 05:25:05.534669 glitter_sdk-0.2.3/glitter_sdk/util/parse_query_str.py
--rw-r--r--   0        0        0    10425 2023-04-29 05:25:05.535860 glitter_sdk-0.2.3/glitter_sdk/util/parse_sql.py
--rw-r--r--   0        0        0      294 2023-03-13 11:08:58.406577 glitter_sdk-0.2.3/glitter_sdk/util/remove_none.py
--rw-r--r--   0        0        0      133 2023-03-13 11:08:58.406694 glitter_sdk-0.2.3/glitter_sdk/util/url.py
--rw-r--r--   0        0        0      765 2023-05-20 10:05:46.187671 glitter_sdk-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 glitter_sdk-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-05 15:04:49.729817 glitter_sdk-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1912 2023-04-01 03:19:53.336155 glitter_sdk-0.2.4/README.md
+-rw-r--r--   0        0        0       13 2023-03-13 11:08:58.347247 glitter_sdk-0.2.4/glitter_sdk/.gitignore
+-rw-r--r--   0        0        0      163 2023-03-13 11:08:58.347884 glitter_sdk-0.2.4/glitter_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.347981 glitter_sdk-0.2.4/glitter_sdk/client/__init__.py
+-rw-r--r--   0        0        0      196 2023-04-01 03:19:53.341248 glitter_sdk-0.2.4/glitter_sdk/client/lcd/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.348980 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/__init__.py
+-rw-r--r--   0        0        0      812 2023-03-13 11:08:58.349462 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/_base.py
+-rw-r--r--   0        0        0     1491 2023-03-26 07:42:53.767656 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/auth.py
+-rw-r--r--   0        0        0     3436 2023-03-13 11:08:58.350610 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/authz.py
+-rw-r--r--   0        0        0     2471 2023-04-28 15:30:57.343890 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/bank.py
+-rw-r--r--   0        0        0     4394 2023-03-13 11:08:58.351558 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/distribution.py
+-rw-r--r--   0        0        0     3632 2023-03-13 11:08:58.352180 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/feegrant.py
+-rw-r--r--   0        0        0    10274 2023-03-13 11:08:58.352841 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/gov.py
+-rw-r--r--   0        0        0      587 2023-03-13 11:08:58.353005 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/ibc.py
+-rw-r--r--   0        0        0      762 2023-03-13 11:08:58.353409 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/ibc_transfer.py
+-rw-r--r--   0        0        0     2330 2023-03-13 11:08:58.353973 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/mint.py
+-rw-r--r--   0        0        0     3776 2023-03-13 11:08:58.354544 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/slashing.py
+-rw-r--r--   0        0        0    13196 2023-03-13 11:08:58.355132 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/staking.py
+-rw-r--r--   0        0        0     3065 2023-03-13 11:08:58.355281 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/tendermint.py
+-rw-r--r--   0        0        0    14761 2023-04-01 03:49:21.407472 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/tx.py
+-rw-r--r--   0        0        0     5011 2023-03-13 11:08:58.356484 glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/wasm.py
+-rw-r--r--   0        0        0      878 2023-03-13 11:08:58.357495 glitter_sdk-0.2.4/glitter_sdk/client/lcd/constants/CLIENT.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.357577 glitter_sdk-0.2.4/glitter_sdk/client/lcd/constants/__init__.py
+-rw-r--r--   0        0        0    14293 2023-05-01 08:56:31.893244 glitter_sdk-0.2.4/glitter_sdk/client/lcd/db.py
+-rw-r--r--   0        0        0    11250 2023-05-20 12:00:58.833798 glitter_sdk-0.2.4/glitter_sdk/client/lcd/lcdclient.py
+-rw-r--r--   0        0        0     1803 2023-03-13 11:08:58.358639 glitter_sdk-0.2.4/glitter_sdk/client/lcd/lcdutils.py
+-rw-r--r--   0        0        0     2394 2023-03-13 11:08:58.359148 glitter_sdk-0.2.4/glitter_sdk/client/lcd/params.py
+-rw-r--r--   0        0        0      949 2023-03-27 15:23:06.688797 glitter_sdk-0.2.4/glitter_sdk/core/__init__.py
+-rw-r--r--   0        0        0      661 2023-03-26 07:20:19.533891 glitter_sdk-0.2.4/glitter_sdk/core/auth/__init__.py
+-rw-r--r--   0        0        0      656 2023-03-26 07:19:34.210859 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/__init__.py
+-rw-r--r--   0        0        0     1835 2023-03-26 07:18:28.803583 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/account.py
+-rw-r--r--   0        0        0     2953 2023-03-13 11:08:58.362249 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/base_account.py
+-rw-r--r--   0        0        0     3965 2023-03-13 11:08:58.362787 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/base_vesting_account.py
+-rw-r--r--   0        0        0     2731 2023-03-13 11:08:58.363597 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/continuous_vesting_account.py
+-rw-r--r--   0        0        0     2498 2023-03-13 11:08:58.364171 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/delayed_vesting_account.py
+-rw-r--r--   0        0        0     2340 2023-03-26 07:47:19.134258 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/eth_account.py
+-rw-r--r--   0        0        0     4441 2023-03-13 11:08:58.364906 glitter_sdk-0.2.4/glitter_sdk/core/auth/data/periodic_vesting_account.py
+-rw-r--r--   0        0        0      331 2023-03-13 11:08:58.365065 glitter_sdk-0.2.4/glitter_sdk/core/auth/msgs/__init__.py
+-rw-r--r--   0        0        0     2921 2023-03-13 11:08:58.365643 glitter_sdk-0.2.4/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py
+-rw-r--r--   0        0        0     2838 2023-03-13 11:08:58.366178 glitter_sdk-0.2.4/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py
+-rw-r--r--   0        0        0     1620 2023-03-13 11:08:58.366670 glitter_sdk-0.2.4/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py
+-rw-r--r--   0        0        0      446 2023-03-13 11:08:58.366825 glitter_sdk-0.2.4/glitter_sdk/core/authz/__init__.py
+-rw-r--r--   0        0        0     9613 2023-03-13 11:08:58.367344 glitter_sdk-0.2.4/glitter_sdk/core/authz/data.py
+-rw-r--r--   0        0        0     6109 2023-03-13 11:08:58.367944 glitter_sdk-0.2.4/glitter_sdk/core/authz/msgs.py
+-rw-r--r--   0        0        0      149 2023-03-13 11:08:58.368579 glitter_sdk-0.2.4/glitter_sdk/core/bank/__init__.py
+-rw-r--r--   0        0        0     7099 2023-03-13 11:08:58.369139 glitter_sdk-0.2.4/glitter_sdk/core/bank/msgs.py
+-rw-r--r--   0        0        0     5009 2023-03-13 11:08:58.369678 glitter_sdk-0.2.4/glitter_sdk/core/bech32.py
+-rw-r--r--   0        0        0     1616 2023-03-13 11:08:58.369822 glitter_sdk-0.2.4/glitter_sdk/core/block.py
+-rw-r--r--   0        0        0     2724 2023-03-13 11:08:58.370319 glitter_sdk-0.2.4/glitter_sdk/core/broadcast.py
+-rw-r--r--   0        0        0     7746 2023-03-13 11:08:58.370786 glitter_sdk-0.2.4/glitter_sdk/core/coin.py
+-rw-r--r--   0        0        0     8360 2023-03-13 11:08:58.371350 glitter_sdk-0.2.4/glitter_sdk/core/coins.py
+-rw-r--r--   0        0        0     2707 2023-03-13 11:08:58.371947 glitter_sdk-0.2.4/glitter_sdk/core/compact_bit_array.py
+-rw-r--r--   0        0        0       71 2023-03-13 11:08:58.372138 glitter_sdk-0.2.4/glitter_sdk/core/crisis/__init__.py
+-rw-r--r--   0        0        0     2069 2023-03-13 11:08:58.372665 glitter_sdk-0.2.4/glitter_sdk/core/crisis/msgs.py
+-rw-r--r--   0        0        0     1085 2023-03-13 11:08:58.373096 glitter_sdk-0.2.4/glitter_sdk/core/deposit.py
+-rw-r--r--   0        0        0      371 2023-03-13 11:08:58.373255 glitter_sdk-0.2.4/glitter_sdk/core/distribution/__init__.py
+-rw-r--r--   0        0        0     6940 2023-03-13 11:08:58.373671 glitter_sdk-0.2.4/glitter_sdk/core/distribution/msgs.py
+-rw-r--r--   0        0        0     2692 2023-03-13 11:08:58.374225 glitter_sdk-0.2.4/glitter_sdk/core/distribution/proposals.py
+-rw-r--r--   0        0        0     2008 2023-03-13 11:08:58.374552 glitter_sdk-0.2.4/glitter_sdk/core/fee.py
+-rw-r--r--   0        0        0      297 2023-03-13 11:08:58.374699 glitter_sdk-0.2.4/glitter_sdk/core/feegrant/__init__.py
+-rw-r--r--   0        0        0     9141 2023-03-13 11:08:58.375006 glitter_sdk-0.2.4/glitter_sdk/core/feegrant/data.py
+-rw-r--r--   0        0        0     3178 2023-03-13 11:08:58.375537 glitter_sdk-0.2.4/glitter_sdk/core/feegrant/msgs.py
+-rw-r--r--   0        0        0      412 2023-03-13 11:08:58.376076 glitter_sdk-0.2.4/glitter_sdk/core/gov/__init__.py
+-rw-r--r--   0        0        0     6154 2023-03-13 11:08:58.376639 glitter_sdk-0.2.4/glitter_sdk/core/gov/data.py
+-rw-r--r--   0        0        0     6516 2023-03-13 11:08:58.377173 glitter_sdk-0.2.4/glitter_sdk/core/gov/msgs.py
+-rw-r--r--   0        0        0     1695 2023-03-13 11:08:58.377677 glitter_sdk-0.2.4/glitter_sdk/core/gov/proposals.py
+-rw-r--r--   0        0        0       47 2023-03-13 11:08:58.377816 glitter_sdk-0.2.4/glitter_sdk/core/ibc/__init__.py
+-rw-r--r--   0        0        0      492 2023-03-13 11:08:58.377946 glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/__init__.py
+-rw-r--r--   0        0        0     4811 2023-03-13 11:08:58.378397 glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/channel.py
+-rw-r--r--   0        0        0     5323 2023-03-13 11:08:58.378944 glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/client.py
+-rw-r--r--   0        0        0     1407 2023-03-13 11:08:58.379538 glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/commitment.py
+-rw-r--r--   0        0        0     1947 2023-03-13 11:08:58.380124 glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/connection.py
+-rw-r--r--   0        0        0      944 2023-03-13 11:08:58.380315 glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/__init__.py
+-rw-r--r--   0        0        0    14728 2023-03-13 11:08:58.380848 glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/channel.py
+-rw-r--r--   0        0        0     5942 2023-03-13 11:08:58.381430 glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/client.py
+-rw-r--r--   0        0        0     9941 2023-03-13 11:08:58.381746 glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/connection.py
+-rw-r--r--   0        0        0       80 2023-03-13 11:08:58.381885 glitter_sdk-0.2.4/glitter_sdk/core/ibc/proposals/__init__.py
+-rw-r--r--   0        0        0     2205 2023-03-13 11:08:58.382371 glitter_sdk-0.2.4/glitter_sdk/core/ibc/proposals/proposals.py
+-rw-r--r--   0        0        0      100 2023-03-13 11:08:58.382853 glitter_sdk-0.2.4/glitter_sdk/core/ibc_transfer/__init__.py
+-rw-r--r--   0        0        0      703 2023-03-13 11:08:58.383309 glitter_sdk-0.2.4/glitter_sdk/core/ibc_transfer/data.py
+-rw-r--r--   0        0        0     3369 2023-03-13 11:08:58.383789 glitter_sdk-0.2.4/glitter_sdk/core/ibc_transfer/msgs.py
+-rw-r--r--   0        0        0     3334 2023-03-13 11:08:58.384170 glitter_sdk-0.2.4/glitter_sdk/core/mode_info.py
+-rw-r--r--   0        0        0      805 2023-03-13 11:08:58.384582 glitter_sdk-0.2.4/glitter_sdk/core/msg.py
+-rw-r--r--   0        0        0      188 2023-03-13 11:08:58.385068 glitter_sdk-0.2.4/glitter_sdk/core/msgs/__init__.py
+-rw-r--r--   0        0        0     1033 2023-03-13 11:08:58.385519 glitter_sdk-0.2.4/glitter_sdk/core/msgs/argument.py
+-rw-r--r--   0        0        0     3793 2023-03-13 11:08:58.385939 glitter_sdk-0.2.4/glitter_sdk/core/msgs/arguments.py
+-rw-r--r--   0        0        0     2993 2023-03-13 11:08:58.386453 glitter_sdk-0.2.4/glitter_sdk/core/msgs/msgs.py
+-rw-r--r--   0        0        0     2394 2023-03-13 11:08:58.386999 glitter_sdk-0.2.4/glitter_sdk/core/multisig.py
+-rw-r--r--   0        0        0    11366 2023-03-13 11:08:58.387613 glitter_sdk-0.2.4/glitter_sdk/core/numeric.py
+-rw-r--r--   0        0        0      114 2023-03-13 11:08:58.387760 glitter_sdk-0.2.4/glitter_sdk/core/params/__init__.py
+-rw-r--r--   0        0        0     3325 2023-03-13 11:08:58.388287 glitter_sdk-0.2.4/glitter_sdk/core/params/proposals.py
+-rw-r--r--   0        0        0    12728 2023-04-01 02:49:01.061356 glitter_sdk-0.2.4/glitter_sdk/core/public_key.py
+-rw-r--r--   0        0        0     2621 2023-03-28 05:25:40.105427 glitter_sdk-0.2.4/glitter_sdk/core/sign_doc.py
+-rw-r--r--   0        0        0     3550 2023-03-13 11:08:58.389976 glitter_sdk-0.2.4/glitter_sdk/core/signature_v2.py
+-rw-r--r--   0        0        0       53 2023-03-13 11:08:58.390162 glitter_sdk-0.2.4/glitter_sdk/core/slashing/__init__.py
+-rw-r--r--   0        0        0     1103 2023-03-13 11:08:58.390660 glitter_sdk-0.2.4/glitter_sdk/core/slashing/msgs.py
+-rw-r--r--   0        0        0      661 2023-03-13 11:08:58.390909 glitter_sdk-0.2.4/glitter_sdk/core/staking/__init__.py
+-rw-r--r--   0        0        0      429 2023-03-13 11:08:58.391064 glitter_sdk-0.2.4/glitter_sdk/core/staking/data/__init__.py
+-rw-r--r--   0        0        0    11301 2023-03-13 11:08:58.391674 glitter_sdk-0.2.4/glitter_sdk/core/staking/data/delegation.py
+-rw-r--r--   0        0        0     9625 2023-03-13 11:08:58.392264 glitter_sdk-0.2.4/glitter_sdk/core/staking/data/validator.py
+-rw-r--r--   0        0        0    11092 2023-03-13 11:08:58.392899 glitter_sdk-0.2.4/glitter_sdk/core/staking/msgs.py
+-rw-r--r--   0        0        0    15136 2023-03-28 05:26:03.502060 glitter_sdk-0.2.4/glitter_sdk/core/tx.py
+-rw-r--r--   0        0        0      176 2023-03-13 11:08:58.393573 glitter_sdk-0.2.4/glitter_sdk/core/upgrade/__init__.py
+-rw-r--r--   0        0        0      149 2023-03-13 11:08:58.393699 glitter_sdk-0.2.4/glitter_sdk/core/upgrade/data/__init__.py
+-rw-r--r--   0        0        0     3330 2023-03-13 11:08:58.394221 glitter_sdk-0.2.4/glitter_sdk/core/upgrade/data/proposal.py
+-rw-r--r--   0        0        0     2191 2023-03-13 11:08:58.394592 glitter_sdk-0.2.4/glitter_sdk/core/upgrade/plan.py
+-rw-r--r--   0        0        0      315 2023-03-13 11:08:58.394733 glitter_sdk-0.2.4/glitter_sdk/core/wasm/__init__.py
+-rw-r--r--   0        0        0     9320 2023-03-13 11:08:58.395189 glitter_sdk-0.2.4/glitter_sdk/core/wasm/data.py
+-rw-r--r--   0        0        0    11303 2023-03-13 11:08:58.395703 glitter_sdk-0.2.4/glitter_sdk/core/wasm/msgs.py
+-rw-r--r--   0        0        0    24195 2023-03-13 11:08:58.396188 glitter_sdk-0.2.4/glitter_sdk/core/wasm/proposals.py
+-rw-r--r--   0        0        0      968 2023-04-09 13:57:19.944409 glitter_sdk-0.2.4/glitter_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.396859 glitter_sdk-0.2.4/glitter_sdk/key/__init__.py
+-rw-r--r--   0        0        0     8381 2023-04-02 10:34:15.503189 glitter_sdk-0.2.4/glitter_sdk/key/key.py
+-rw-r--r--   0        0        0     2371 2023-05-21 02:50:58.868900 glitter_sdk-0.2.4/glitter_sdk/key/mnemonic.py
+-rw-r--r--   0        0        0     1846 2023-04-02 15:21:54.394109 glitter_sdk-0.2.4/glitter_sdk/key/raw.py
+-rw-r--r--   0        0        0     3623 2023-03-26 02:18:44.107996 glitter_sdk-0.2.4/glitter_sdk/key/topub.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.398493 glitter_sdk-0.2.4/glitter_sdk/util/__init__.py
+-rw-r--r--   0        0        0     1678 2023-03-13 11:08:58.398629 glitter_sdk-0.2.4/glitter_sdk/util/base.py
+-rw-r--r--   0        0        0      878 2023-03-13 11:08:58.398824 glitter_sdk-0.2.4/glitter_sdk/util/constants/CLIENT.py
+-rw-r--r--   0        0        0      679 2023-03-13 11:08:58.399255 glitter_sdk-0.2.4/glitter_sdk/util/constants/COMMAND.py
+-rw-r--r--   0        0        0     1927 2023-03-13 11:08:58.399786 glitter_sdk-0.2.4/glitter_sdk/util/constants/CR.py
+-rw-r--r--   0        0        0    12296 2023-03-13 11:08:58.400320 glitter_sdk-0.2.4/glitter_sdk/util/constants/ER.py
+-rw-r--r--   0        0        0      370 2023-03-13 11:08:58.400832 glitter_sdk-0.2.4/glitter_sdk/util/constants/FIELD_TYPE.py
+-rw-r--r--   0        0        0      214 2023-03-13 11:08:58.401339 glitter_sdk-0.2.4/glitter_sdk/util/constants/FLAG.py
+-rw-r--r--   0        0        0      333 2023-03-13 11:08:58.401638 glitter_sdk-0.2.4/glitter_sdk/util/constants/SERVER_STATUS.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:08:58.401707 glitter_sdk-0.2.4/glitter_sdk/util/constants/__init__.py
+-rw-r--r--   0        0        0     3253 2023-03-13 11:08:58.402210 glitter_sdk-0.2.4/glitter_sdk/util/contract.py
+-rw-r--r--   0        0        0      199 2023-03-13 11:08:58.402331 glitter_sdk-0.2.4/glitter_sdk/util/converter.py
+-rw-r--r--   0        0        0     1325 2023-04-06 08:22:21.253664 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/__init__.py
+-rw-r--r--   0        0        0     1386 2023-04-06 03:28:40.834754 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/converter/__init__.py
+-rw-r--r--   0        0        0     5017 2023-04-01 02:40:55.205070 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/converter/bech32.py
+-rw-r--r--   0        0        0      230 2023-04-01 02:49:31.013058 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-01 02:49:31.022589 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/ecdsa.py
+-rw-r--r--   0        0        0     6072 2023-04-01 02:40:55.205900 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/ecdsa_base.py
+-rw-r--r--   0        0        0    14377 2023-04-01 02:40:55.206225 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py
+-rw-r--r--   0        0        0    24914 2023-04-01 02:49:31.016470 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/ecdsa_python.py
+-rw-r--r--   0        0        0    17376 2023-04-01 02:40:55.207175 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/openssl.py
+-rw-r--r--   0        0        0     8962 2023-04-01 02:40:55.207492 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/utils.py
+-rw-r--r--   0        0        0        0 2023-04-01 02:40:55.207660 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/eth/__init__.py
+-rw-r--r--   0        0        0    55432 2023-04-01 02:49:31.019972 glitter_sdk-0.2.4/glitter_sdk/util/encrypt/eth/ethereum.py
+-rw-r--r--   0        0        0      211 2023-03-13 11:08:58.402439 glitter_sdk-0.2.4/glitter_sdk/util/hash.py
+-rw-r--r--   0        0        0      377 2023-04-30 02:03:55.614570 glitter_sdk-0.2.4/glitter_sdk/util/highlight.py
+-rw-r--r--   0        0        0     1696 2023-03-13 11:08:58.403849 glitter_sdk-0.2.4/glitter_sdk/util/json.py
+-rw-r--r--   0        0        0     1045 2023-03-13 11:08:58.404376 glitter_sdk-0.2.4/glitter_sdk/util/parse_authorization.py
+-rw-r--r--   0        0        0     2550 2023-03-13 11:08:58.404831 glitter_sdk-0.2.4/glitter_sdk/util/parse_content.py
+-rw-r--r--   0        0        0     3887 2023-03-13 11:08:58.405152 glitter_sdk-0.2.4/glitter_sdk/util/parse_msg.py
+-rw-r--r--   0        0        0      732 2023-03-13 11:08:58.405653 glitter_sdk-0.2.4/glitter_sdk/util/parse_proto.py
+-rw-r--r--   0        0        0     2837 2023-04-29 05:25:05.534669 glitter_sdk-0.2.4/glitter_sdk/util/parse_query_str.py
+-rw-r--r--   0        0        0    10425 2023-04-29 05:25:05.535860 glitter_sdk-0.2.4/glitter_sdk/util/parse_sql.py
+-rw-r--r--   0        0        0      294 2023-03-13 11:08:58.406577 glitter_sdk-0.2.4/glitter_sdk/util/remove_none.py
+-rw-r--r--   0        0        0      133 2023-03-13 11:08:58.406694 glitter_sdk-0.2.4/glitter_sdk/util/url.py
+-rw-r--r--   0        0        0      765 2023-05-20 12:01:21.280689 glitter_sdk-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 glitter_sdk-0.2.4/PKG-INFO
```

### Comparing `glitter_sdk-0.2.3/LICENSE` & `glitter_sdk-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/README.md` & `glitter_sdk-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/_base.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/_base.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/auth.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/auth.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/authz.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/authz.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/bank.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/bank.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/distribution.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/distribution.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/feegrant.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/feegrant.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/gov.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/gov.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/ibc.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/ibc.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/ibc_transfer.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/ibc_transfer.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/mint.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/mint.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/slashing.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/slashing.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/staking.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/staking.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/tendermint.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/tendermint.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/tx.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/tx.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/api/wasm.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/api/wasm.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/constants/CLIENT.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/db.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/db.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/lcdclient.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/lcdclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from .api.wasm import AsyncWasmAPI, WasmAPI
 from .lcdutils import AsyncLCDUtils, LCDUtils
 from .params import APIParams
 from .db import AsyncDB, DB
 
 
 def get_default(chain_id: str) -> [Coins, Numeric]:
-    if chain_id == "glitter_12000-1":
+    if chain_id.startswith("glitter_12000"):
         return [Coins.from_str("0.15agli"), Numeric.parse(1.75)]
 
     raise ValueError("chain_id is invalid")
 
 
 class AsyncLCDClient:
     def __init__(
```

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/lcdutils.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/lcdutils.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/client/lcd/params.py` & `glitter_sdk-0.2.4/glitter_sdk/client/lcd/params.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/__init__.py` & `glitter_sdk-0.2.4/glitter_sdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/__init__.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/__init__.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/base_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/base_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/base_vesting_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/base_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/continuous_vesting_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/continuous_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/delayed_vesting_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/delayed_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/eth_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/eth_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/data/periodic_vesting_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/data/periodic_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/msgs/msg_create_vesting_account.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py` & `glitter_sdk-0.2.4/glitter_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/authz/data.py` & `glitter_sdk-0.2.4/glitter_sdk/core/authz/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/authz/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/authz/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/bank/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/bank/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/bech32.py` & `glitter_sdk-0.2.4/glitter_sdk/core/bech32.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/block.py` & `glitter_sdk-0.2.4/glitter_sdk/core/block.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/broadcast.py` & `glitter_sdk-0.2.4/glitter_sdk/core/broadcast.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/coin.py` & `glitter_sdk-0.2.4/glitter_sdk/core/coin.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/coins.py` & `glitter_sdk-0.2.4/glitter_sdk/core/coins.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/compact_bit_array.py` & `glitter_sdk-0.2.4/glitter_sdk/core/compact_bit_array.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/crisis/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/crisis/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/deposit.py` & `glitter_sdk-0.2.4/glitter_sdk/core/deposit.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/distribution/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/distribution/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/distribution/proposals.py` & `glitter_sdk-0.2.4/glitter_sdk/core/distribution/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/fee.py` & `glitter_sdk-0.2.4/glitter_sdk/core/fee.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/feegrant/data.py` & `glitter_sdk-0.2.4/glitter_sdk/core/feegrant/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/feegrant/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/feegrant/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/gov/data.py` & `glitter_sdk-0.2.4/glitter_sdk/core/gov/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/gov/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/gov/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/gov/proposals.py` & `glitter_sdk-0.2.4/glitter_sdk/core/gov/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/channel.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/channel.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/client.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/client.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/commitment.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/commitment.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/data/connection.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/data/connection.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/__init__.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/channel.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/channel.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/client.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/client.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/msgs/connection.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/msgs/connection.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc/proposals/proposals.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc/proposals/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc_transfer/data.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc_transfer/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/ibc_transfer/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/ibc_transfer/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/mode_info.py` & `glitter_sdk-0.2.4/glitter_sdk/core/mode_info.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/msg.py` & `glitter_sdk-0.2.4/glitter_sdk/core/msg.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/msgs/argument.py` & `glitter_sdk-0.2.4/glitter_sdk/core/msgs/argument.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/msgs/arguments.py` & `glitter_sdk-0.2.4/glitter_sdk/core/msgs/arguments.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/msgs/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/msgs/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/multisig.py` & `glitter_sdk-0.2.4/glitter_sdk/core/multisig.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/numeric.py` & `glitter_sdk-0.2.4/glitter_sdk/core/numeric.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/params/proposals.py` & `glitter_sdk-0.2.4/glitter_sdk/core/params/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/public_key.py` & `glitter_sdk-0.2.4/glitter_sdk/core/public_key.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/sign_doc.py` & `glitter_sdk-0.2.4/glitter_sdk/core/sign_doc.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/signature_v2.py` & `glitter_sdk-0.2.4/glitter_sdk/core/signature_v2.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/slashing/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/slashing/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/staking/__init__.py` & `glitter_sdk-0.2.4/glitter_sdk/core/staking/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/staking/data/delegation.py` & `glitter_sdk-0.2.4/glitter_sdk/core/staking/data/delegation.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/staking/data/validator.py` & `glitter_sdk-0.2.4/glitter_sdk/core/staking/data/validator.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/staking/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/staking/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/tx.py` & `glitter_sdk-0.2.4/glitter_sdk/core/tx.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/upgrade/data/proposal.py` & `glitter_sdk-0.2.4/glitter_sdk/core/upgrade/data/proposal.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/upgrade/plan.py` & `glitter_sdk-0.2.4/glitter_sdk/core/upgrade/plan.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/wasm/data.py` & `glitter_sdk-0.2.4/glitter_sdk/core/wasm/data.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/wasm/msgs.py` & `glitter_sdk-0.2.4/glitter_sdk/core/wasm/msgs.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/core/wasm/proposals.py` & `glitter_sdk-0.2.4/glitter_sdk/core/wasm/proposals.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/exceptions.py` & `glitter_sdk-0.2.4/glitter_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/key/key.py` & `glitter_sdk-0.2.4/glitter_sdk/key/key.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/key/mnemonic.py` & `glitter_sdk-0.2.4/glitter_sdk/key/mnemonic.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,18 +53,18 @@
         coin_type: int = GLITTER_COIN_TYPE,
     ):
         self.coin_type = coin_type
         self.account = account
         self.index = index
 
         master_key = HDPrivateKey.master_key_from_mnemonic(mnemonic)
-        root_keys = HDKey.from_path(master_key, self.hd_path)
+        root_keys = HDKey.from_path(master_key, "m/44'/60'/0'")
         acct_priv_key = root_keys[-1]
         acct_pub_key = HDKey.from_b58check(acct_priv_key.to_b58check())
-        keys = HDKey.from_path(acct_pub_key, f'{0}/{0}')
+        keys = HDKey.from_path(acct_pub_key, f'{0}/{index}')
 
         # eth_address = keys[-1].public_key.address()
         # self.private_key = bytes.fromhex(keys[-1]._key.to_hex())
         # self.evmos_address = eth_to_evmos(eth_address)
         # self.public_key = keys[-1].public_key.compressed_bytes
         super().__init__(keys[-1])
```

### Comparing `glitter_sdk-0.2.3/glitter_sdk/key/raw.py` & `glitter_sdk-0.2.4/glitter_sdk/key/raw.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/key/topub.py` & `glitter_sdk-0.2.4/glitter_sdk/key/topub.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/base.py` & `glitter_sdk-0.2.4/glitter_sdk/util/base.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/constants/CLIENT.py` & `glitter_sdk-0.2.4/glitter_sdk/util/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/constants/COMMAND.py` & `glitter_sdk-0.2.4/glitter_sdk/util/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/constants/CR.py` & `glitter_sdk-0.2.4/glitter_sdk/util/constants/CR.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/constants/ER.py` & `glitter_sdk-0.2.4/glitter_sdk/util/constants/ER.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/contract.py` & `glitter_sdk-0.2.4/glitter_sdk/util/contract.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/__init__.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/converter/__init__.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/converter/bech32.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/converter/bech32.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/ecdsa_base.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/ecdsa_base.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/ecdsa_openssl.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/ecdsa_python.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/ecdsa_python.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/openssl.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/openssl.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/crypto/utils.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/crypto/utils.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/encrypt/eth/ethereum.py` & `glitter_sdk-0.2.4/glitter_sdk/util/encrypt/eth/ethereum.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/json.py` & `glitter_sdk-0.2.4/glitter_sdk/util/json.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/parse_authorization.py` & `glitter_sdk-0.2.4/glitter_sdk/util/parse_authorization.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/parse_content.py` & `glitter_sdk-0.2.4/glitter_sdk/util/parse_content.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/parse_msg.py` & `glitter_sdk-0.2.4/glitter_sdk/util/parse_msg.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/parse_proto.py` & `glitter_sdk-0.2.4/glitter_sdk/util/parse_proto.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/parse_query_str.py` & `glitter_sdk-0.2.4/glitter_sdk/util/parse_query_str.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/glitter_sdk/util/parse_sql.py` & `glitter_sdk-0.2.4/glitter_sdk/util/parse_sql.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk-0.2.3/pyproject.toml` & `glitter_sdk-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glitter-sdk"
-version = "0.2.3"
+version = "0.2.4"
 description='Glitter Protocol is a blockchain based database and index engine for developing and hosting web3 applications in decentralized storage networks.'
 authors = ["Glitter Protocol <ted@glitterprotocol.io>"]
 readme = "README.md"
 packages = [{include = "glitter_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `glitter_sdk-0.2.3/PKG-INFO` & `glitter_sdk-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glitter-sdk
-Version: 0.2.3
+Version: 0.2.4
 Summary: Glitter Protocol is a blockchain based database and index engine for developing and hosting web3 applications in decentralized storage networks.
 Author: Glitter Protocol
 Author-email: ted@glitterprotocol.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glitter-sdk Version: 0.2.3 Summary: Glitter
+Metadata-Version: 2.1 Name: glitter-sdk Version: 0.2.4 Summary: Glitter
 Protocol is a blockchain based database and index engine for developing and
 hosting web3 applications in decentralized storage networks. Author: Glitter
 Protocol Author-email: ted@glitterprotocol.io Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

