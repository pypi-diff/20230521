# Comparing `tmp/dprox-0.0.2.tar.gz` & `tmp/dprox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/OpenProx/dist/.tmp-e2sch1_z/dprox-0.0.2.tar", last modified: Fri Feb 24 04:16:23 2023, max compression
+gzip compressed data, was "dprox-0.1.0.tar", last modified: Sun May 21 15:40:01 2023, max compression
```

## Comparing `dprox-0.0.2.tar` & `dprox-0.1.0.tar`

### file list

```diff
@@ -1,141 +1,165 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1067 2021-12-28 08:47:07.000000 dprox-0.0.2/LICENSE
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      133 2023-02-24 04:16:23.000000 dprox-0.0.2/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1175 2023-01-04 11:33:26.000000 dprox-0.0.2/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       62 2023-02-22 12:21:36.000000 dprox-0.0.2/dprox/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/algo/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      276 2023-02-22 12:09:37.000000 dprox-0.0.2/dprox/algo/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3558 2023-02-22 12:57:41.000000 dprox-0.0.2/dprox/algo/admm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5747 2023-02-22 14:07:44.000000 dprox-0.0.2/dprox/algo/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      483 2023-01-15 04:55:40.000000 dprox-0.0.2/dprox/algo/hqs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      679 2023-01-07 01:54:52.000000 dprox-0.0.2/dprox/algo/invert.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/algo/opt/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 03:34:32.000000 dprox-0.0.2/dprox/algo/opt/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1212 2023-01-05 14:16:13.000000 dprox-0.0.2/dprox/algo/opt/absorb.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-01-04 15:10:13.000000 dprox-0.0.2/dprox/algo/opt/equil.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2239 2023-01-04 15:10:13.000000 dprox-0.0.2/dprox/algo/opt/merge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1047 2023-02-17 16:09:23.000000 dprox-0.0.2/dprox/algo/pc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-01-15 04:55:51.000000 dprox-0.0.2/dprox/algo/pgd.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2093 2023-02-22 13:01:44.000000 dprox-0.0.2/dprox/algo/problem.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/algo/special/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       72 2023-02-13 15:28:40.000000 dprox-0.0.2/dprox/algo/special/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6857 2023-02-22 14:30:28.000000 dprox-0.0.2/dprox/algo/special/deq.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/algo/special/deq_utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 03:34:36.000000 dprox-0.0.2/dprox/algo/special/deq_utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-01-14 04:16:49.000000 dprox-0.0.2/dprox/algo/special/deq_utils/jacobian.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-01-14 04:16:49.000000 dprox-0.0.2/dprox/algo/special/deq_utils/layer_utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-01-14 04:16:49.000000 dprox-0.0.2/dprox/algo/special/deq_utils/optimizations.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-01-14 04:16:50.000000 dprox-0.0.2/dprox/algo/special/deq_utils/radam.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    14116 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/algo/special/deq_utils/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-02-22 14:00:39.000000 dprox-0.0.2/dprox/algo/special/unroll.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/algo/tune/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       23 2023-01-06 14:08:11.000000 dprox-0.0.2/dprox/algo/tune/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12895 2023-02-22 13:28:02.000000 dprox-0.0.2/dprox/algo/tune/autotune.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1850 2023-01-04 11:33:27.000000 dprox-0.0.2/dprox/algo/tune/dpir.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-01-04 11:33:27.000000 dprox-0.0.2/dprox/algo/tune/learnable.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/linop/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      650 2023-02-22 15:12:52.000000 dprox-0.0.2/dprox/linop/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2128 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/linop/blackbox.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13023 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/linop/comp_graph.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-01-06 06:46:09.000000 dprox-0.0.2/dprox/linop/constant.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7046 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/linop/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      328 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/linop/edge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1242 2023-01-09 07:41:54.000000 dprox-0.0.2/dprox/linop/grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5504 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/linop/lin_op.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      339 2023-01-24 15:42:43.000000 dprox-0.0.2/dprox/linop/placeholder.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1847 2023-01-05 09:46:05.000000 dprox-0.0.2/dprox/linop/scale.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2630 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/linop/subsample.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2953 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/linop/sum.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1779 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/linop/variable.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2739 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/linop/vstack.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-01-05 15:08:40.000000 dprox-0.0.2/dprox/proxfn/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2689 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/proxfn/base.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/fast/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/fast/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-01-09 07:42:34.000000 dprox-0.0.2/dprox/proxfn/fast/cs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      922 2023-02-13 15:28:40.000000 dprox-0.0.2/dprox/proxfn/fast/csmri.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-01-09 07:43:00.000000 dprox-0.0.2/dprox/proxfn/fast/pr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-01-09 07:43:08.000000 dprox-0.0.2/dprox/proxfn/fast/spi.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3915 2023-01-09 07:41:54.000000 dprox-0.0.2/dprox/proxfn/fast/sr.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/linear_solve/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      432 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/proxfn/linear_solve/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3955 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/proxfn/linear_solve/cg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3202 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/proxfn/linear_solve/custom.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4441 2023-01-20 05:44:49.000000 dprox-0.0.2/dprox/proxfn/linear_solve/torchcg.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/nlm/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/nlm/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/nlm/nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/nlm/patch_nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/nonneg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/norm.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/pnp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3307 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/composite.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 03:33:57.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/network_unet.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/unet/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-01-16 01:08:46.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-02-13 15:28:40.000000 dprox-0.0.2/dprox/proxfn/pnp/denoisers/wrapper.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2913 2023-02-13 15:31:25.000000 dprox-0.0.2/dprox/proxfn/pnp/prior.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5898 2023-02-17 15:10:40.000000 dprox-0.0.2/dprox/proxfn/sum_square.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/proxfn/unrolling/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/proxfn/unrolling/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/proxfn/unrolling/dgu.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      482 2023-02-13 15:26:39.000000 dprox-0.0.2/dprox/proxfn/unrolling/prior.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      164 2023-02-22 12:33:34.000000 dprox-0.0.2/dprox/utils/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/utils/examples/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       50 2023-02-22 12:34:09.000000 dprox-0.0.2/dprox/utils/examples/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/utils/examples/csmri/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       57 2023-02-22 13:22:17.000000 dprox-0.0.2/dprox/utils/examples/csmri/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3011 2023-02-22 12:49:49.000000 dprox-0.0.2/dprox/utils/examples/csmri/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4146 2023-02-22 12:34:50.000000 dprox-0.0.2/dprox/utils/examples/csmri/dataset.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2089 2023-02-22 12:16:32.000000 dprox-0.0.2/dprox/utils/examples/csmri/misc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1659 2023-02-24 04:11:33.000000 dprox-0.0.2/dprox/utils/examples/misc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      891 2023-01-14 14:28:10.000000 dprox-0.0.2/dprox/utils/examples/mosaic.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/utils/examples/optic/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       46 2023-02-23 12:56:17.000000 dprox-0.0.2/dprox/utils/examples/optic/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5211 2023-02-23 12:59:05.000000 dprox-0.0.2/dprox/utils/examples/optic/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13167 2023-02-22 14:58:27.000000 dprox-0.0.2/dprox/utils/examples/optic/doe_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3063 2023-02-23 13:37:21.000000 dprox-0.0.2/dprox/utils/examples/optic/unet.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox/utils/init/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 03:34:11.000000 dprox-0.0.2/dprox/utils/init/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4704 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/utils/init/mosaic.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      755 2023-01-04 11:33:26.000000 dprox-0.0.2/dprox/utils/init/sr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1106 2023-02-17 13:31:17.000000 dprox-0.0.2/dprox/utils/io.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2442 2023-01-05 13:07:07.000000 dprox-0.0.2/dprox/utils/metrics.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1436 2023-01-06 16:01:13.000000 dprox-0.0.2/dprox/utils/misc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2289 2023-01-20 07:25:19.000000 dprox-0.0.2/dprox/utils/psf2otf.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      133 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3599 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-02-24 04:16:23.000000 dprox-0.0.2/dprox.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-02-24 04:16:23.000000 dprox-0.0.2/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      236 2023-02-24 04:16:02.000000 dprox-0.0.2/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-02-24 04:16:23.000000 dprox-0.0.2/test/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5680 2023-02-13 15:26:39.000000 dprox-0.0.2/test/test_dpir.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      310 2023-05-21 15:40:01.413618 dprox-0.1.0/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3156 2023-05-10 07:07:21.000000 dprox-0.1.0/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.401618 dprox-0.1.0/dprox/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      105 2023-05-12 08:43:00.000000 dprox-0.1.0/dprox/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      276 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3612 2023-05-20 09:01:13.000000 dprox-0.1.0/dprox/algo/admm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5833 2023-05-20 09:14:46.000000 dprox-0.1.0/dprox/algo/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/hqs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      679 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/invert.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/lp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2355 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/linear_solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13377 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6017 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/utils.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/opt/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/opt/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.1.0/dprox/algo/opt/absorb.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/opt/equil.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2239 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/opt/merge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/pc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/pgd.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4576 2023-05-20 09:37:39.000000 dprox-0.1.0/dprox/algo/problem.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/special/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       72 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6866 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/special/deq_utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/jacobian.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/layer_utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/optimizations.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/radam.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/unroll.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/tune/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       23 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12895 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/autotune.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1850 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/dpir.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/learnable.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/linop/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-10 14:07:17.000000 dprox-0.1.0/dprox/linop/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7440 2023-05-20 03:13:06.000000 dprox-0.1.0/dprox/linop/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2126 2023-05-10 14:07:18.000000 dprox-0.1.0/dprox/linop/blackbox.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15084 2023-05-20 09:13:41.000000 dprox-0.1.0/dprox/linop/comp_graph.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.1.0/dprox/linop/constaints.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2862 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/constant.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5036 2023-05-12 06:37:57.000000 dprox-0.1.0/dprox/linop/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/edge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/linop/grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      339 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/linop/placeholder.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2560 2023-05-12 06:38:28.000000 dprox-0.1.0/dprox/linop/scale.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3439 2023-05-12 06:38:59.000000 dprox-0.1.0/dprox/linop/subsample.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2991 2023-05-20 03:13:06.000000 dprox-0.1.0/dprox/linop/sum.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2968 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/variable.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3657 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/vstack.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      306 2023-05-10 08:01:32.000000 dprox-0.1.0/dprox/proxfn/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2693 2023-05-20 01:26:10.000000 dprox-0.1.0/dprox/proxfn/base.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/fast/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/cs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      884 2023-05-20 03:23:29.000000 dprox-0.1.0/dprox/proxfn/fast/csmri.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/pr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/spi.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.1.0/dprox/proxfn/fast/sr.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/linalg/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-10 08:37:58.000000 dprox-0.1.0/dprox/proxfn/linalg/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1782 2023-05-11 03:05:00.000000 dprox-0.1.0/dprox/proxfn/linalg/custom.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/linalg/solve/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      271 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5069 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/bicgstab.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1134 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/broyden.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6317 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/cg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6501 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/gmres.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1631 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/plss.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/nlm/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nlm/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nlm/nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nlm/patch_nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nonneg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/norm.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/composite.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_unet.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/wrapper.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2902 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/pnp/prior.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6025 2023-05-20 09:35:06.000000 dprox-0.1.0/dprox/proxfn/sum_square.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/proxfn/unrolling/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/unrolling/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/unrolling/dgu.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      482 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/unrolling/prior.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      164 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      107 2023-05-12 09:12:18.000000 dprox-0.1.0/dprox/utils/containar.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-05-13 14:43:30.000000 dprox-0.1.0/dprox/utils/examples/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/csmri/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       82 2023-05-13 14:45:34.000000 dprox-0.1.0/dprox/utils/examples/csmri/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3011 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/csmri/common.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4146 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/csmri/dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1993 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/utils/examples/csmri/misc.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/derain/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       40 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/derain/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2564 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/derain/custom_linop.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/energy_system/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      947 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/utils/examples/energy_system/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/optic/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       46 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5211 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/common.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13167 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/doe_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3063 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2488 2023-05-14 13:57:57.000000 dprox-0.1.0/dprox/utils/examples/restoration.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/init/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/init/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4704 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/init/mosaic.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      755 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/init/sr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2130 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/utils/io.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2442 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/metrics.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1709 2023-05-20 08:50:17.000000 dprox-0.1.0/dprox/utils/misc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2289 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/psf2otf.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.401618 dprox-0.1.0/dprox.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      310 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4251 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-21 15:40:01.413618 dprox-0.1.0/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      662 2023-05-21 15:39:51.000000 dprox-0.1.0/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/tests/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2715 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_algorithms.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      316 2023-05-20 03:14:24.000000 dprox-0.1.0/tests/test_energy_system.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1101 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_inverse_problems.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2119 2023-05-21 14:42:14.000000 dprox-0.1.0/tests/test_linear_solver.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3272 2023-05-12 08:09:14.000000 dprox-0.1.0/tests/test_linear_solver_grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5780 2023-05-20 03:12:27.000000 dprox-0.1.0/tests/test_linear_solver_torch.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2692 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_linop.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_linop_primitive.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1196 2023-05-20 09:38:13.000000 dprox-0.1.0/tests/test_ml_problems.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dprox-0.0.2/dprox/algo/admm.py` & `dprox-0.1.0/dprox/algo/admm.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,24 +45,25 @@
         self.least_square = get_least_square_solver(psi_fns, omega_fns, try_diagonalize, try_freq_diagonalize, lin_solver_kwargs)
 
     def _iter(self, state, rho, lam):
         x, v, u = state
         b = [v[i] - u[i] for i in range(len(self.psi_fns))]
         x = self.least_square.solve(b, rho)
 
-        Kx = self.K.forward([x])  # cache Kx
+        Kx = self.K.forward(x, return_list=True)  # cache Kx
         for i, fn in enumerate(self.psi_fns):
             v[i] = fn.prox(Kx[i] + u[i], lam=lam[fn])
             u[i] = u[i] + Kx[i] - v[i]
 
         return x, v, u
 
     def initialize(self, x0):
         x = x0
-        v = self.K.forward([x])
+        v = self.K.forward(x, return_list=True)
+        if v is None: v = []  # in case there is no psi fns
         u = [torch.zeros_like(e) for e in v]
         return x, v, u
 
     @property
     def nparams(self):
         return len(self.psi_fns) + 1
 
@@ -77,39 +78,40 @@
 
         # solve x problem using least square
         b = []
         for i, fn in enumerate(self.psi_fns):
             # coeff = expand(rho/lam[fn])
             # we empircally find ignore the coefficient works better.
             coeff = 1
-            tmp = eval(fn.linop, [x])[0] - v[i] + u[i]
-            tmp = adjoint(fn.linop, [tmp])[0]
+            tmp = eval(fn.linop, x) - v[i] + u[i]
+            tmp = adjoint(fn.linop, tmp)
             b += [x - coeff * tmp]
 
         x = self.least_square.solve(b, rho)
 
         # solve proximal fns
-        Kx = self.K.forward([x])  # cache Kx
+        Kx = self.K.forward(x)  # cache Kx
         for i, fn in enumerate(self.psi_fns):
             v[i] = fn.prox(Kx[i] + u[i], lam=lam[fn])
             u[i] = u[i] + Kx[i] - v[i]
 
         return x, v, u
 
 
 class ADMM_vxu(ADMM):
     """ update x,v,u in v,x,u order
     """
+
     def _iter(self, state, rho, lam):
         z, x, u = state
 
-        Kz = self.K.forward([z])  # cache Kx
+        Kz = self.K.forward(z)  # cache Kx
         for i, fn in enumerate(self.psi_fns):
             x[i] = fn.prox(Kz[i] - u[i], lam=lam[fn])
-            
+
         b = [x[i] + u[i] for i in range(len(self.psi_fns))]
         z = self.least_square.solve(b, rho)
-        
+
         for i, fn in enumerate(self.psi_fns):
             u[i] = u[i] + x[i] - z
 
-        return x[0], [z], u
+        return z, x, u
```

### Comparing `dprox-0.0.2/dprox/algo/base.py` & `dprox-0.1.0/dprox/algo/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     # instance method
 
     def __init__(self, psi_fns: List[ProxFn], omega_fns: List[ProxFn]):
         super().__init__()
         self.psi_fns = nn.ModuleList(psi_fns)
         self.omega_fns = nn.ModuleList(omega_fns)
         self.K = CompGraph(vstack([fn.linop for fn in psi_fns]))
+        self.Kall = CompGraph(vstack([fn.linop for fn in psi_fns + omega_fns]))
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     @auto_convert_to_tensor(['x0', 'rhos', 'lams'], batchify=['x0'])
     def solve(self, x0=None, rhos=None, lams=None, max_iter=24, pbar=False):
@@ -103,17 +104,17 @@
 
         for op in [fn.linop for fn in self.psi_fns]:
             recursive_set_step(op, step)
         for op in [fn.linop for fn in self.omega_fns]:
             recursive_set_step(op, step)
 
     def iter(self, state, rho, lam):
-        self.K.update_vars([state[0]])
+        self.Kall.update_vars([state[0]])
         state = self._iter(state, rho, lam)
-        self.K.update_vars([state[0]])
+        self.Kall.update_vars([state[0]])
         return state
 
     @abc.abstractmethod
     def _iter(self, state, rho, lam):
         return NotImplementedError
 
     def _notify_all_op_current_step(self, step):
```

### Comparing `dprox-0.0.2/dprox/algo/invert.py` & `dprox-0.1.0/dprox/algo/invert.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/opt/absorb.py` & `dprox-0.1.0/dprox/algo/opt/absorb.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 def absorb_linop(prox_fn):
     """If possible moves the top level lin op argument
        into the prox operator.
 
        For example, elementwise multiplication can be folded into
        a separable function's prox.
     """
-    if isinstance(prox_fn.linop, mosaic):
-        new_fn = weighted_sum_squares(prox_fn.linop.input_nodes[0], prox_fn.linop)
-
-        # Fold scalar into the function.
+    if isinstance(prox_fn.linop, mosaic) and isinstance(prox_fn, sum_squares):
+        new_fn = weighted_sum_squares(prox_fn.linop.input_nodes[0], prox_fn.linop, prox_fn.offset)
+        return [new_fn]
+    
+    # Fold scalar into the function.
     if isinstance(prox_fn.linop, scale):
         scalar = prox_fn.linop.scalar
         prox_fn.linop = prox_fn.linop.input_nodes[0]
         prox_fn.beta = prox_fn.beta * scalar
         return [prox_fn]
     # No change.
     return [prox_fn]
```

### Comparing `dprox-0.0.2/dprox/algo/opt/equil.py` & `dprox-0.1.0/dprox/algo/opt/equil.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/opt/merge.py` & `dprox-0.1.0/dprox/algo/opt/merge.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/pc.py` & `dprox-0.1.0/dprox/algo/pc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
+from ..linop import adjoint
 from .admm import ADMM
 from .base import expand
-from ..linop import adjoint
 
 
 class PockChambolle(ADMM):
     def initialize(self, x0):
         x = x0
         xbar = x.clone()
-        z = self.K.forward([x])
+        z = self.K.forward(x, return_list=True)
         return x, z, xbar
 
     def _iter(self, state, rho, lam):
         x, z, xbar = state
 
         # update z
-        Kxbar = self.K.forward([xbar])
+        Kxbar = self.K.forward(xbar, return_list=True)
         for i, fn in enumerate(self.psi_fns):
             r = expand(lam[fn])
             z[i] = z[i] + r * Kxbar[i]
             z[i] = z[i] - r * fn.prox(z[i], lam=r)
 
         # update x
         # Ktz = self.K.adjoint(z)
-        Ktz = [adjoint(fn.linop, [z[i]])[0] for i, fn in enumerate(self.psi_fns)]
+        Ktz = [adjoint(fn.linop, z[i]) for i, fn in enumerate(self.psi_fns)]
         x_next = [x - Ktz[i] for i in range(len(Ktz))]
         if len(self.omega_fns) > 0:
             x_next = self.least_square.solve(x_next, rho)
         else:
             x_next = sum(x_next)
 
         # update xbar
```

### Comparing `dprox-0.0.2/dprox/algo/pgd.py` & `dprox-0.1.0/dprox/algo/pgd.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/special/deq.py` & `dprox-0.1.0/dprox/algo/special/deq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 from pathlib import Path
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.data import DataLoader
-from torch.utils.tensorboard import SummaryWriter
-from tqdm import tqdm
+
 
 from dprox.algo.base import Algorithm
 from dprox.utils import to_torch_tensor
 
 from .deq_utils.jacobian import jac_loss_estimate
 from .deq_utils.solvers import anderson, broyden
 
@@ -99,14 +98,16 @@
     def load(self, state_dict, strict=True):
         self.load_state_dict(state_dict['solver'], strict=strict)
         self.rhos = state_dict.get('rhos')
         self.lams = state_dict.get('lams')
         
     
 def train_deq(args, dataset, solver, step_fn, on_epoch_end=None):
+    from torch.utils.tensorboard import SummaryWriter
+    from tqdm import tqdm
     import torchlight as tl
     from torchlight.nn.utils import adjust_learning_rate
     loader = DataLoader(dataset, batch_size=args.bs, num_workers=8, shuffle=True)
     device = torch.device('cuda')
 
     optimizer = torch.optim.AdamW(solver.parameters(), lr=1e-4, weight_decay=1e-4)
```

### Comparing `dprox-0.0.2/dprox/algo/special/deq_utils/jacobian.py` & `dprox-0.1.0/dprox/algo/special/deq_utils/jacobian.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/special/deq_utils/layer_utils.py` & `dprox-0.1.0/dprox/algo/special/deq_utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/special/deq_utils/optimizations.py` & `dprox-0.1.0/dprox/algo/special/deq_utils/optimizations.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/special/deq_utils/radam.py` & `dprox-0.1.0/dprox/algo/special/deq_utils/radam.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/special/deq_utils/solvers.py` & `dprox-0.1.0/dprox/algo/special/deq_utils/solvers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 # Modified based on the DEQ repo.
 
 import torch
-from torch import nn
-import torch.nn.functional as functional
-from torch.autograd import Function
 import numpy as np 
 import pickle
-import sys
-import os
-from scipy.optimize import root
-import time
-from termcolor import colored
 
 
 def _safe_norm(v):
     if not torch.isfinite(v).all():
         return np.inf
     return torch.norm(v)
 
@@ -325,14 +317,16 @@
     X = F = None
     return out
 
 def analyze_broyden(res_info, err=None, judge=True, name='forward', training=True, save_err=True):
     """
     For debugging use only :-)
     """
+    from termcolor import colored
+    
     res_est = res_info['result']
     nstep = res_info['nstep']
     diff = res_info['diff']
     diff_detail = res_info['diff_detail']
     prot_break = res_info['prot_break']
     trace = res_info['trace']
     eps = res_info['eps']
```

### Comparing `dprox-0.0.2/dprox/algo/special/unroll.py` & `dprox-0.1.0/dprox/algo/special/unroll.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/tune/autotune.py` & `dprox-0.1.0/dprox/algo/tune/autotune.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/algo/tune/dpir.py` & `dprox-0.1.0/dprox/algo/tune/dpir.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/linop/__init__.py` & `dprox-0.1.0/dprox/linop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .conv import conv, conv_doe
 from .constant import Constant
 from .comp_graph import CompGraph, est_CompGraph_norm, eval, adjoint, gram
 from .scale import scale
 from .subsample import mosaic
 from .sum import sum, copy
 from .variable import Variable
-from .lin_op import LinOp
+from .base import LinOp
 from .vstack import vstack, split
 from .placeholder import Placeholder
 from .grad import grad
 # from .conv_nofft import conv_nofft
 # from .mul_elemwise import mul_elemwise
 # from .hstack import hstack
 # from .warp import warp
```

### Comparing `dprox-0.0.2/dprox/linop/blackbox.py` & `dprox-0.1.0/dprox/linop/blackbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .lin_op import LinOp
+from .base import LinOp
 
 
 def LinOpFactory(forward, adjoint, diag=None, norm_bound=None):
     """Returns a function to generate a custom LinOp.
 
     Parameters
     ----------
```

### Comparing `dprox-0.0.2/dprox/linop/comp_graph.py` & `dprox-0.1.0/dprox/linop/comp_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from .sum import copy
-from .edge import Edge
-from .variable import Variable
-from .constant import Constant
-from .vstack import split
-from .vstack import vstack
 import copy as cp
 from collections import defaultdict
+
 import numpy as np
-from scipy.sparse.linalg import LinearOperator, eigs
 import torch
+from scipy.sparse.linalg import LinearOperator, eigs
+
+from .constant import Constant
+from .edge import Edge
+from .sum import copy
+from .variable import Variable
+from .vstack import split, vstack
+from .base import LinOp
 
 
 class CompGraph:
     """A computation graph representing a composite lin op.
     """
 
     instanceCnt = 0
@@ -82,36 +84,45 @@
                     ready.append(node)
 
             self.edges += input_edges
             self.input_edges[curr] = input_edges
 
         # replace the split nodes with copy nodes
         for n in self.split_nodes.keys():
+            # find out the outputs by traverse the outputs of original node
             outedges = self.output_edges[n]
             outnodes = [e.end for e in outedges]
             copy_node = copy(n)
-            copy_node.input_nodes += [n]  # we actually can have more than two input nodes
+
+            # link split(copy) node with its original node, link in two direction, forward and adjoint
             self.output_edges[n] = [Edge(n, copy_node)]
             self.input_edges[copy_node] = self.output_edges[n]
+
+            # ---- link the output of copy node to its outputs. ---- #
             self.output_edges[copy_node] = []
+            # modify the input edge of the outputs node
             self.nodes.append(copy_node)
             for ns in outnodes:
                 inedges = self.input_edges[ns]
                 newinedges = []
                 for e in inedges:
+                    # if input edges's start is original node, replace it with the new copy node.
                     if e.start is n:
                         e = Edge(copy_node, e.end)
                         newinedges.append(e)
                         self.output_edges[copy_node].append(e)
                     else:
                         newinedges.append(e)
                 self.input_edges[ns] = newinedges
 
+            # we actually can have more than two input nodes
+            copy_node.input_nodes += [n] * (len(self.output_edges[copy_node]) - 1)
+
         # Make copy node for each variable.
-        old_vars = self.end.variables()
+        old_vars = self.end.variables
         id2copy = {}
         copy_nodes = []
         self.var_info = {}
         offset = 0
         for var in old_vars:
             copy_node = copy(var)
             copy_node.orig_node = None
@@ -167,55 +178,73 @@
         """Returns the output data for a node.
         """
         return [e.data for e in self.output_edges[node]]
 
     def write_outputs(self, node, outputs):
         """Returns the output data for a node.
         """
+        if not isinstance(outputs, LinOp.MultOutput):
+            outputs = [outputs]
         for e, output in zip(self.output_edges[node], outputs):
             e.data = output
 
     def write_inputs(self, node, inputs):
         """Returns the input data for a node.
         """
+        if not isinstance(inputs, LinOp.MultOutput):
+            inputs = [inputs]
         for e, input in zip(self.input_edges[node], inputs):
             e.data = input
 
-    def forward(self, x):
+    def forward(self, *values, return_list=False):
         """Evaluates the forward composition.
         """
         global y
         y = None
 
         def forward_eval(node):
-            if node == self.start: inputs = x
+            if node == self.start: inputs = list(values)
             else: inputs = self.get_inputs(node)
-            outputs = node.forward(inputs)
+            if len(inputs) > 1:
+                outputs = node.forward(*inputs)
+            elif len(inputs) == 1:
+                outputs = node.forward(inputs[0])
+            else:
+                outputs = node.forward()
             if node == self.end: global y; y = outputs
             else: self.write_outputs(node, outputs)
 
         self.traverse_graph(forward_eval, forward=True)
 
+        if return_list and y is not None and not isinstance(y, LinOp.MultOutput):
+            y = [y]
         return y
 
-    def adjoint(self, x):
+    def adjoint(self, *values, return_list=False):
         """Evaluates the adjoint composition.
         """
         global y
         y = None
 
         def adjoint_eval(node):
-            if node == self.end: outputs = x
+            if node == self.end: outputs = list(values)
             else: outputs = self.get_outputs(node)
-            inputs = node.adjoint(outputs)
+            if len(outputs) > 1:
+                inputs = node.adjoint(*outputs)
+            elif len(outputs) == 1:
+                inputs = node.adjoint(outputs[0])
+            else:
+                inputs = node.adjoint()
             if node == self.start: global y; y = inputs
             else: self.write_inputs(node, inputs)
 
         self.traverse_graph(adjoint_eval, forward=False)
 
+        if return_list and y is not None and not isinstance(y, LinOp.MultOutput):
+            y = [y]
         return y
 
     def traverse_graph(self, node_fn, forward):
         """Traverse the graph and apply the given function at each node.
 
            forward: Traverse in standard or reverse order?
            node_fn: Function to evaluate on each node.
@@ -280,16 +309,17 @@
                     e.mag = output_mag
 
         self.traverse_graph(node_norm_bound, True)
 
     def visualize(self, save_path=None):
         """ Visualize the graph with graphviz
         """
-        import graphviz
         import queue
+
+        import graphviz
         from IPython.display import display
         dot = graphviz.Digraph()
         nodes = {}
 
         def node_name(obj):
             if not obj in nodes:
                 nodes[obj] = 'N%d' % len(nodes)
@@ -300,45 +330,59 @@
             node = Q.get()
             if node not in nodes:
                 dot.node(node_name(node), str(node))
             for e in self.input_edges.get(node, []):
                 Q.put(e.start)
         for node in nodes.keys():
             for e in self.input_edges.get(node, []):
-                dot.edge(node_name(e.end), node_name(e.start))
+                dot.edge(node_name(e.start), node_name(e.end))
 
         if save_path is None:
             display(dot)
 
     def sanity_check(self, eps=1e-5):
         """ Perform dot product test to check the sanity of this linear operator
         """
         from scipy.misc import face
-        import torch
         m = torch.from_numpy(face().copy()).float().cuda() / 255
         m = m.permute(2, 0, 1).unsqueeze(0)
-        d = self.forward([m])[0]
-        d2 = torch.rand_like(d)
-        m2 = self.adjoint([d2])[0]
-        diff = torch.abs(torch.sum(m * m2) - torch.sum(d * d2))
-        rel_diff = torch.abs((torch.sum(m * m2) - torch.sum(d * d2)) / torch.sum(m * m2))
+        d = self.forward(m)
+
+        if isinstance(d, LinOp.MultOutput):
+            d2 = [torch.rand_like(e) for e in d]
+            m2 = self.adjoint(*d2)
+            sum_m = torch.sum(m * m2)
+            sum_d = sum([torch.sum(e1 * e2) for e1, e2 in zip(d, d2)])
+            diff = torch.abs(sum_m - sum_d)
+            rel_diff = torch.abs((sum_m - sum_d) / sum_m)
+        else:
+            d2 = torch.rand_like(d)
+            m2 = self.adjoint(d2)
+
+            sum_m = torch.sum(m * m2)
+            sum_d = torch.sum(d * d2)
+            diff = torch.abs(sum_m - sum_d)
+            rel_diff = torch.abs((sum_m - sum_d) / sum_m)
+
         if rel_diff < eps:
             print(f'Sanity check passed, diff={diff} rel_diff={rel_diff}')
+            return True
         else:
             print(f'Sanity check failed, diff={diff} rel_diff={rel_diff}')
+            return False
 
     def update_vars(self, val):
         """Map sections of val to variables.
         """
-        for i, var in enumerate(self.end.variables()):
+        for i, var in enumerate(self.end.variables):
             var.value = val[i]
 
     def x0(self):
         res = []
-        for var in self.end.variables():
+        for var in self.end.variables:
             res += [torch.zeros(var.shape)]
         return res
 
     def __str__(self):
         return self.__class__.__name__
 
 
@@ -375,18 +419,33 @@
     A = LinearOperator((K.input_size, K.input_size),
                        KtK, KtK)
 
     Knorm = np.sqrt(eigs(A, k=1, M=None, sigma=None, which='LM', tol=tol)[0].real)
     return np.float(Knorm)
 
 
-def eval(linop, inputs, zero_out_constant=True):
-    return CompGraph(linop, zero_out_constant).forward(inputs)
-
-
-def adjoint(linop, inputs, zero_out_constant=True):
-    return CompGraph(linop, zero_out_constant).adjoint(inputs)
+def eval(linop, *inputs, zero_out_constant=True):
+    G = CompGraph(linop, zero_out_constant)
+    if len(inputs) > 1:
+        return G.forward(*inputs)
+    elif len(inputs) == 1:
+        return G.forward(inputs[0])
+    else:
+        return G.forward()
+
+
+def adjoint(linop, *inputs, zero_out_constant=True):
+    G = CompGraph(linop, zero_out_constant)
+    if len(inputs) > 1:
+        return G.adjoint(*inputs)
+    elif len(inputs) == 1:
+        return G.adjoint(inputs[0])
+    else:
+        return G.adjoint()
 
 
-def gram(linop, inputs, zero_out_constant=True):
+def gram(linop, *inputs, zero_out_constant=True):
     K = CompGraph(linop, zero_out_constant)
-    return K.adjoint(K.forward(inputs))
+    outputs = K.forward(*inputs)
+    if isinstance(outputs, LinOp.MultOutput):
+        return K.adjoint(*outputs)
+    return K.adjoint(outputs)
```

### Comparing `dprox-0.0.2/dprox/linop/constant.py` & `dprox-0.1.0/dprox/linop/scale.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,80 @@
-from .lin_op import LinOp
 import numpy as np
 import torch
 
-class Constant(LinOp):
-    """A constant.
-    """
+from .base import LinOp
 
-    def __init__(self, value):
-        super(Constant, self).__init__([])
-        if np.isscalar(value):
-            value = torch.tensor(value)
-        self._value = value
 
-    def variables(self):
-        return []
+class scale(LinOp):
+    """Multiplication scale*X with a fixed scalar.
+    """
 
-    def constants(self):
-        return [self]
+    def __init__(self, scalar, arg):
+        assert np.isscalar(scalar)
+        self.scalar = scalar
+        super(scale, self).__init__([arg])
+
+    # ---------------------------------------------------------------------------- #
+    #                                  Computation                                 #
+    # ---------------------------------------------------------------------------- #
 
-    def forward(self, inputs):
+    def forward(self, input):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
-        return [self.value]
+        return input * self.scalar
 
-    def adjoint(self, inputs):
+    def adjoint(self, input):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
-        return [self.value*0]
-    
-    @property
-    def value(self):
-        return self._value.to(self.device)
+        return self.forward(input)
+
+    # ---------------------------------------------------------------------------- #
+    #                                   Diagonal                                   #
+    # ---------------------------------------------------------------------------- #
+
+    def is_gram_diag(self, freq=False):
+        """Is the lin  Gram diagonal (in the frequency domain)?
+        """
+        return self.input_nodes[0].is_gram_diag(freq)
 
     def is_diag(self, freq=False):
         """Is the lin op diagonal (in the frequency domain)?
         """
-        return True
+        return self.input_nodes[0].is_diag(freq)
 
-    def get_diag(self, freq=False):
+    def get_diag(self, ref, freq=False):
         """Returns the diagonal representation (A^TA)^(1/2).
 
         Parameters
         ----------
         freq : bool
             Is the diagonal representation in the frequency domain?
         Returns
         -------
         dict of variable to ndarray
             The diagonal operator acting on each variable.
         """
-        return {}
+        var_diags = self.input_nodes[0].get_diag(ref, freq) * self.scalar
+        return var_diags * torch.conj(var_diags)
+
+    # ---------------------------------------------------------------------------- #
+    #                                   Property                                   #
+    # ---------------------------------------------------------------------------- #
 
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
             List of magnitudes of inputs.
 
         Returns
         -------
         float
             Magnitude of outputs.
         """
-        return 0.0
+        return abs(self.scalar) * input_mags[0]
```

### Comparing `dprox-0.0.2/dprox/linop/grad.py` & `dprox-0.1.0/dprox/linop/grad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from .lin_op import LinOp
 import numpy as np
-from .conv import conv
+
 from dprox.utils.misc import to_torch_tensor
 
+from .conv import conv
+
+
 class grad(conv):
     """
     gradient operation. can be defined for different dimensions.
     default is n-d gradient.
     """
 
     def __init__(self, arg, dim=1):
```

### Comparing `dprox-0.0.2/dprox/linop/lin_op.py` & `dprox-0.1.0/dprox/linop/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,191 @@
 import abc
+import copy
+
 import numpy as np
 import torch
 import torch.nn as nn
+
 from dprox.utils import to_torch_tensor
 
 
 def cast_to_const(expr):
     """Converts a non-LinOp to a Constant.
     """
     from .constant import Constant
     return expr if isinstance(expr, LinOp) else Constant(expr)
 
 
 class LinOp(nn.Module):
     """Represents a linear operator.
     """
-    __metaclass__ = abc.ABCMeta
+
+    class MultOutput(list): pass
 
     instanceCnt = 0
 
-    def __init__(self, input_nodes):
+    def __init__(self, input_nodes=[]):
         super(LinOp, self).__init__()
         self.input_nodes = nn.ModuleList([cast_to_const(node) for node in input_nodes])
+
+        # count id
         self.linop_id = LinOp.instanceCnt
         LinOp.instanceCnt += 1
+
+        # create a dummy parameter to automatically infer device
         self.dummy = torch.nn.parameter.Parameter(torch.tensor(0), requires_grad=False)
 
         # will be set later by proximal algorithm to indicate current iteration step
         self.step = 0
 
+    # ---------------------------------------------------------------------------- #
+    #                                  Computation                                 #
+    # ---------------------------------------------------------------------------- #
+
+    @abc.abstractmethod
+    def forward(self, inputs):
+        """The forward operator. Compute x -> Kx
+        """
+        return NotImplemented
+
+    @abc.abstractmethod
+    def adjoint(self, inputs):
+        """The adjoint operator. Compute x -> K^Tx
+        """
+        return NotImplemented
+
+    # ---------------------------------------------------------------------------- #
+    #                                   Diagonal                                   #
+    # ---------------------------------------------------------------------------- #
+
+    def is_gram_diag(self, freq=False):
+        """Is the lin op's Gram matrix K^TK diagonal (in the frequency domain)?
+        """
+        return self.is_diag(freq)
+
+    def is_diag(self, freq=False):
+        """Is the lin op K diagonal (in the frequency domain)?
+        """
+        return False
+
+    def get_diag(self, freq=False):
+        """Returns the diagonal representation (K^TK)^(1/2).
+
+        Parameters
+        ----------
+        freq : bool
+            Is the diagonal representation in the frequency domain?
+
+        Returns
+        -------
+        dict of variable to ndarray
+            The diagonal operator acting on each variable.
+        """
+        return NotImplemented
+
+    # ---------------------------------------------------------------------------- #
+    #                                   Property                                   #
+    # ---------------------------------------------------------------------------- #
+
     @property
     def device(self):
         return self.dummy.device
 
-    def unwrap(self, value):
-        from .placeholder import Placeholder
-        if isinstance(value, Placeholder):
-            return value.value
-        return to_torch_tensor(value, batch=True)
-
-    def params(self):
-        params = []
-        for node in self.input_nodes:
-            params += node.params()
-        return params
-    
+    @property
     def variables(self):
         """Return the list of variables used in the LinOp.
         """
         vars_ = []
         for arg in self.input_nodes:
-            vars_ += arg.variables()
+            vars_ += arg.variables
         unordered = list(set(vars_))  # Make unique, order by uuid.
         return sorted(unordered, key=lambda x: x.uuid)
 
+    @property
     def constants(self):
         """Returns a list of constants in the LinOp.
         """
         consts = []
         for arg in self.input_nodes:
-            consts += arg.constants()
+            consts += arg.constants
         return consts
 
     def is_constant(self):
         """Is the LinOp constant?
         """
         return len(self.variables()) == 0
 
-    @abc.abstractmethod
-    def forward(self, inputs, outputs):
-        """The forward operator.
-
-        Reads from inputs and writes to outputs.
-        """
-        return NotImplemented
-
-    @abc.abstractmethod
-    def adjoint(self, inputs, outputs):
-        """The adjoint operator.
-
-        Reads from inputs and writes to outputs.
-        """
-        return NotImplemented
-
-    def is_gram_diag(self, freq=False):
-        """Is the lin op's Gram matrix diagonal (in the frequency domain)?
-        """
-        return self.is_diag(freq)
+    @property
+    def value(self):
+        inputs = []
+        for node in self.input_nodes:
+            inputs.append(node.value)
+        output = self.forward(*inputs)
+        return output
 
-    def is_diag(self, freq=False):
-        """Is the lin op diagonal (in the frequency domain)?
+    @property
+    def offset(self):
+        """Get the constant offset.
         """
-        return False
+        old_vals = {}
+        for var in self.variables:
+            old_vals[var] = var.value
+            var.value = torch.zeros_like(var.value)
+        offset = self.value
+        # Restore old variable values.
+        for var in self.variables:
+            var.value = old_vals[var]
+        return offset
 
-    def get_diag(self, freq=False):
-        """Returns the diagonal representation (A^TA)^(1/2).
+    def norm_bound(self, input_mags):
+        """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
-        freq : bool
-            Is the diagonal representation in the frequency domain?
+        input_mags : list
+            List of magnitudes of inputs.
+
         Returns
         -------
-        dict of variable to ndarray
-            The diagonal operator acting on each variable.
+        float
+            Magnitude of outputs.
         """
         return NotImplemented
 
+    # ---------------------------------------------------------------------------- #
+    #                                     Util                                     #
+    # ---------------------------------------------------------------------------- #
+
+    @property
+    def T(self):
+        op = self.clone()
+        op.forward, op.adjoint = op.adjoint, op.forward
+        return op
+
+    @property
+    def gram(self):
+        op = self.clone()
+        forward, adjoint = op.forward, op.adjoint
+        op.forward = lambda inputs: adjoint(forward(inputs))
+        op.adjoint = lambda inputs: forward(adjoint(inputs))
+        return op
+
+    def clone(self):
+        return copy.deepcopy(self)
+
+    def unwrap(self, value):
+        from .placeholder import Placeholder
+        if isinstance(value, Placeholder):
+            return value.value
+        return to_torch_tensor(value, batch=True)
+
+    # ---------------------------------------------------------------------------- #
+    #                                 Python Magic                                 #
+    # ---------------------------------------------------------------------------- #
+
     def __add__(self, other):
         """Lin Op + Lin Op.
         """
         other = cast_to_const(other)
         from .sum import sum
         args = []
         for elem in [self, other]:
@@ -120,14 +195,15 @@
                 args += [elem]
         return sum(args)
 
     def __mul__(self, other):
         """Lin Op * Number.
         """
         from .scale import scale
+
         # Can only divide by scalar constants.
         if np.isscalar(other):
             return scale(other, self)
         else:
             raise TypeError("Can only multiply by a scalar constant.")
 
     def __rmul__(self, other):
@@ -140,14 +216,15 @@
         """
         return self.__div__(other)
 
     def __div__(self, other):
         """Lin Op / Number.
         """
         from .scale import scale
+
         # Can only divide by scalar constants.
         if np.isscalar(other):
             return scale(1. / other, self)
         else:
             raise TypeError("Can only divide by a scalar constant.")
 
     def __sub__(self, other):
@@ -160,48 +237,22 @@
         """
         return -self + other
 
     def __neg__(self):
         """The negation of the Lin Op.
         """
         return -1 * self
-
+    
+    def __rmatmul__(self, other):
+        # other @ self
+        from .constaints import matmul
+        from .variable import Variable
+        if not isinstance(self, Variable):
+            print('only support variable')
+        return matmul(self, other)
+    
     def __str__(self):
         """Default to string is name of class.
         """
         return self.__class__.__name__
-
-    @property
-    def value(self):
-        inputs = []
-        for node in self.input_nodes:
-            inputs.append(node.value)
-        output = self.forward(inputs)[0]
-        return output
-
-    def get_offset(self):
-        """Get the constant offset.
-        """
-        old_vals = {}
-        for var in self.variables():
-            old_vals[var] = var.value
-            var.value = torch.zeros_like(var.value)
-        offset = self.value
-        # Restore old variable values.
-        for var in self.variables():
-            var.value = old_vals[var]
-        return offset
-
-    def norm_bound(self, input_mags):
-        """Gives an upper bound on the magnitudes of the outputs given inputs.
-
-        Parameters
-        ----------
-        input_mags : list
-            List of magnitudes of inputs.
-
-        Returns
-        -------
-        float
-            Magnitude of outputs.
-        """
-        return NotImplemented
+    
+    __array_priority__ = 10000
```

### Comparing `dprox-0.0.2/dprox/linop/scale.py` & `dprox-0.1.0/dprox/linop/sum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,109 @@
-from .lin_op import LinOp
 import torch
-import numpy as np
 
-class scale(LinOp):
-    """Multiplication scale*X with a fixed scalar.
-    """
-
-    def __init__(self, scalar, arg):
-        assert np.isscalar(scalar)
-        self.scalar = scalar
-        super(scale, self).__init__([arg])
+from .base import LinOp
 
-    def forward(self, inputs):
-        """The forward operator.
 
-        Reads from inputs and writes to outputs.
-        """
-        return [inputs[0]* self.scalar]
+class sum(LinOp):
+    """Sums its inputs.
+    """
 
-    def adjoint(self, inputs):
-        """The adjoint operator.
+    def __init__(self, input_nodes):
+        super(sum, self).__init__(input_nodes)
 
-        Reads from inputs and writes to outputs.
+    def forward(self, *inputs):
+        """ Just sum all the inputs, all inputs should have the same shape
         """
-        return self.forward(inputs)
-
-    def is_gram_diag(self, freq=False):
-        """Is the lin  Gram diagonal (in the frequency domain)?
+        output = torch.zeros_like(inputs[0])
+        for input in inputs:
+            output += input.to(output.device)
+        return output
+
+    def adjoint(self, input):
+        """ The adjoint of sum spread of the input to all its child
+        """
+        outputs = LinOp.MultOutput()
+        for _ in self.input_nodes:
+            outputs.append(input)
+        if len(outputs) > 1:
+            return outputs
+        return outputs[0]
+    
+    def is_diag(self, freq=False):
+        """Is the lin op diagonal (in the frequency domain)?
         """
-        return self.input_nodes[0].is_gram_diag(freq)
+        return all([arg.is_diag(freq) for arg in self.input_nodes])
 
-    def is_diag(self, freq=False):
+    def is_gram_diag(self, freq=False):
         """Is the lin op diagonal (in the frequency domain)?
         """
-        return self.input_nodes[0].is_diag(freq)
+        return all([arg.is_gram_diag(freq) for arg in self.input_nodes])
 
-    def get_diag(self, freq=False):
+    def get_diag(self, ref, freq=False):
         """Returns the diagonal representation (A^TA)^(1/2).
 
         Parameters
         ----------
         freq : bool
             Is the diagonal representation in the frequency domain?
         Returns
         -------
         dict of variable to ndarray
             The diagonal operator acting on each variable.
         """
-        var_diags = self.input_nodes[0].get_diag(freq)
-        for var in var_diags.keys():
-            var_diags[var] = var_diags[var] * self.scalar
-        return var_diags
+        # var_diags = {var: torch.zeros(var.size) for var in self.variables()}
+        # for arg in self.input_nodes:
+        #     arg_diags = arg.get_diag(shape, freq)
+        #     for var, diag in arg_diags.items():
+        #         var_diags[var] = var_diags[var] + diag
+        # return var_diags.values()[0]
+        return self.input_nodes[0].get_diag(ref, freq)
+
+    def norm_bound(self, input_mags):
+        """Gives an upper bound on the magnitudes of the outputs given inputs.
+
+        Parameters
+        ----------
+        input_mags : list
+            List of magnitudes of inputs.
+
+        Returns
+        -------
+        float
+            Magnitude of outputs.
+        """
+        return torch.sum(input_mags)
+
+
+class copy(sum):
+
+    def __init__(self, arg):
+        super(copy, self).__init__([arg])
+
+    def forward(self, inputs):
+        """The forward operator.
+
+        Reads from inputs and writes to outputs.
+        """
+        return super(copy, self).adjoint(inputs)
+
+    def adjoint(self, *inputs):
+        """The adjoint operator.
+
+        Reads from inputs and writes to outputs.
+        """
+        return super(copy, self).forward(*inputs)
 
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
             List of magnitudes of inputs.
 
         Returns
         -------
         float
             Magnitude of outputs.
         """
-        return abs(self.scalar) * input_mags[0]
+        return input_mags[0]
```

### Comparing `dprox-0.0.2/dprox/linop/subsample.py` & `dprox-0.1.0/dprox/linop/subsample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-from .lin_op import LinOp
 import numpy as np
+
 from dprox.utils.misc import to_nn_parameter, to_torch_tensor
 
+from .base import LinOp
+
 
 class mosaic(LinOp):
 
     def __init__(self, arg):
         super(mosaic, self).__init__([arg])
         self.cache = {}
-    
+
+    # ---------------------------------------------------------------------------- #
+    #                                  Computation                                 #
+    # ---------------------------------------------------------------------------- #
+
+    def forward(self, input):
+        """The forward operator.
+
+        Reads from inputs and writes to outputs.
+        """
+        mask = self._mask(input.shape).to(input.device)
+        return mask * input
+
+    def adjoint(self, input):
+        """The adjoint operator.
+
+        Reads from inputs and writes to outputs.
+        """
+        return self.forward(input)
+
     @staticmethod
     def masks_CFA_Bayer(shape):
         pattern = 'RGGB'
         channels = dict((channel, np.zeros(shape)) for channel in 'RGB')
         for channel, (y, x) in zip(pattern, [(0, 0), (0, 1), (1, 0), (1, 1)]):
             channels[channel][y::2, x::2] = 1
         return tuple(channels[c].astype(bool) for c in 'RGB')
-    
+
     def _mask(self, shape):
         if shape not in self.cache:
             shape = shape[-2:]
             R_m, G_m, B_m = self.masks_CFA_Bayer(shape)
             mask = np.concatenate((R_m[..., None], G_m[..., None], B_m[..., None]), axis=-1)
             self.cache[shape] = to_nn_parameter(to_torch_tensor(mask.astype('float32'), batch=True))
         return self.cache[shape]
 
-    def forward(self, inputs):
-        """The forward operator.
-
-        Reads from inputs and writes to outputs.
-        """
-        input = inputs[0]
-        mask = self._mask(input.shape).to(input.device)
-        return [mask * input]
-
-    def adjoint(self, inputs):
-        """The adjoint operator.
-
-        Reads from inputs and writes to outputs.
-        """
-        return self.forward(inputs)
+    # ---------------------------------------------------------------------------- #
+    #                                   Diagonal                                   #
+    # ---------------------------------------------------------------------------- #
 
     def is_gram_diag(self, freq=False):
         """Is the lin op's Gram matrix diagonal (in the frequency domain)?
         """
-        return not freq and self.input_nodes[0].is_diag(freq)
+        return self.is_self_diag(freq) and self.input_nodes[0].is_diag(freq)
+
+    def is_self_diag(self, freq=False):
+        return not freq
 
     def get_diag(self, x, freq=False):
         """Returns the diagonal representation (A^TA)^(1/2).
 
         Parameters
         ----------
         freq : bool
@@ -63,14 +75,18 @@
         # selection = self.get_selection()
         # self_diag = np.zeros(self.input_nodes[0].shape)
         # self_diag[selection] = 1
         # for var in var_diags.keys():
         #     var_diags[var] = var_diags[var] * self_diag.ravel()
         return self._mask(x.shape).to(self.device)
 
+    # ---------------------------------------------------------------------------- #
+    #                                   Property                                   #
+    # ---------------------------------------------------------------------------- #
+
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
             List of magnitudes of inputs.
```

### Comparing `dprox-0.0.2/dprox/linop/sum.py` & `dprox-0.1.0/dprox/linop/vstack.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,112 @@
-import torch
-from .lin_op import LinOp
+import numpy as np
 
+from .base import LinOp
 
-class sum(LinOp):
-    """Sums its inputs.
+
+class vstack(LinOp):
+    """Vectorizes and stacks inputs.
     """
 
     def __init__(self, input_nodes):
-        super(sum, self).__init__(input_nodes)
+        super(vstack, self).__init__(input_nodes)
 
-    def forward(self, inputs):
-        """ Just sum all the inputs, all inputs should have the same shape
-        """
-        output = torch.zeros_like(inputs[0])
-        for input in inputs:
-            output += input.to(output.device)
-        return [output]
+    # ---------------------------------------------------------------------------- #
+    #                                  Computation                                 #
+    # ---------------------------------------------------------------------------- #
+
+    def forward(self, *inputs):
+        """The forward operator.
 
-    def adjoint(self, inputs):
-        """ The adjoint of sum spread of the input to all its child
+        Reads from inputs and writes to outputs.
         """
-        assert len(inputs) == 1
-        outputs = []
-        for _ in self.input_nodes:
-            outputs.append(inputs[0])
-        return outputs
+        if len(inputs) > 1:
+            return LinOp.MultOutput(inputs)
+        return inputs[0]
+
+    def adjoint(self, *inputs):
+        """The adjoint operator.
 
-    def is_diag(self, freq=False):
-        """Is the lin op diagonal (in the frequency domain)?
+        Reads from inputs and writes to outputs.
         """
-        return all([arg.is_diag(freq) for arg in self.input_nodes])
+        if len(inputs) > 1:
+            return LinOp.MultOutput(inputs)
+        return inputs[0]
+    
+    # ---------------------------------------------------------------------------- #
+    #                                   Diagonal                                   #
+    # ---------------------------------------------------------------------------- #
 
     def is_gram_diag(self, freq=False):
-        """Is the lin op diagonal (in the frequency domain)?
+        """Is the lin op's Gram matrix diagonal (in the frequency domain)?
         """
         return all([arg.is_gram_diag(freq) for arg in self.input_nodes])
 
-    def get_diag(self, shape, freq=False):
+    def get_diag(self, freq=False):
         """Returns the diagonal representation (A^TA)^(1/2).
 
         Parameters
         ----------
         freq : bool
             Is the diagonal representation in the frequency domain?
         Returns
         -------
         dict of variable to ndarray
             The diagonal operator acting on each variable.
         """
-        # var_diags = {var: torch.zeros(var.size) for var in self.variables()}
-        # for arg in self.input_nodes:
-        #     arg_diags = arg.get_diag(shape, freq)
-        #     for var, diag in arg_diags.items():
-        #         var_diags[var] = var_diags[var] + diag
-        # return var_diags.values()[0]
-        return self.input_nodes[0].get_diag(shape, freq)
+        var_diags = {var: np.zeros(var.size) for var in self.variables()}
+        for arg in self.input_nodes:
+            arg_diags = arg.get_diag(freq)
+            for var, diag in arg_diags.items():
+                var_diags[var] = var_diags[var] + diag * np.conj(diag)
+        # Get (A^TA)^{1/2}
+        for var in self.variables():
+            var_diags[var] = np.sqrt(var_diags[var])
+        return var_diags
+    
+    # ---------------------------------------------------------------------------- #
+    #                                   Property                                   #
+    # ---------------------------------------------------------------------------- #
 
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
             List of magnitudes of inputs.
 
         Returns
         -------
         float
             Magnitude of outputs.
         """
-        return torch.sum(input_mags)
+        return np.linalg.norm(input_mags, 2)
 
 
-class copy(sum):
+class split(vstack):
 
-    def __init__(self, arg):
-        super(copy, self).__init__([arg])
+    def __init__(self, output_nodes):
+        self.output_nodes = output_nodes
+        self.input_nodes = []
+        super(split, self).__init__(output_nodes)
 
-    def forward(self, inputs):
+    def forward(self, *inputs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
-        return super(copy, self).adjoint(inputs)
+        return super(split, self).adjoint(*inputs)
 
-    def adjoint(self, inputs):
+    def adjoint(self, *inputs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
-        return super(copy, self).forward(inputs)
+        return super(split, self).forward(*inputs)
 
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
```

### Comparing `dprox-0.0.2/dprox/linop/variable.py` & `dprox-0.1.0/dprox/linop/variable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-from .lin_op import LinOp
-import numpy as np
 import uuid
+
 import torch
 
+from .base import LinOp
+
 
 class Variable(LinOp):
     """A variable.
     """
 
-    def __init__(self, shape=None, name=None):
+    def __init__(self, shape=None, value=None, name=None):
         super(Variable, self).__init__([])
         self.uuid = uuid.uuid1()
-        self._value = None
+        self._value = value
         self.shape = shape
         self.varname = name
         self.initval = None
 
+    # ---------------------------------------------------------------------------- #
+    #                                  Computation                                 #
+    # ---------------------------------------------------------------------------- #
+    
     def forward(self, inputs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
         return inputs
 
     def adjoint(self, inputs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
         return inputs
 
-    def variables(self):
-        return [self]
+    # ---------------------------------------------------------------------------- #
+    #                                   Diagonal                                   #
+    # ---------------------------------------------------------------------------- #
 
     def is_diag(self, freq=False):
         """Is the lin op diagonal (in the frequency domain)?
         """
         return True
 
     def get_diag(self, ref, freq=False):
@@ -48,14 +54,24 @@
         Returns
         -------
         dict of variable to ndarray
             The diagonal operator acting on each variable.
         """
         return torch.ones(ref.shape)
 
+
+    # ---------------------------------------------------------------------------- #
+    #                                   Property                                   #
+    # ---------------------------------------------------------------------------- #
+
+
+    @property
+    def variables(self):
+        return [self]
+    
     @property
     def value(self):
         return self._value.to(self.device)
 
     @value.setter
     def value(self, val):
         """Assign a value to the variable.
@@ -72,7 +88,14 @@
 
         Returns
         -------
         float
             Magnitude of outputs.
         """
         return 1.0
+
+    # ---------------------------------------------------------------------------- #
+    #                                 Python Magic                                 #
+    # ---------------------------------------------------------------------------- #
+    
+    def __repr__(self):
+        return f'Variable(id={self.uuid}, shape={self.shape}, value={"None" if self._value is None else "somevalue"})'
```

### Comparing `dprox-0.0.2/dprox/proxfn/base.py` & `dprox-0.1.0/dprox/proxfn/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         self.linop = linop
         self.alpha = alpha
         self.beta = beta
         self.step = 0
         self.dag = CompGraph(linop, zero_out_constant=True)
 
     @property
-    def b(self):
-        return -self.linop.get_offset()
+    def offset(self):
+        return -self.linop.offset
 
     def unwrap(self, value):
         if isinstance(value, Placeholder):
             return value.value
         return to_torch_tensor(value, batch=True).to(self.linop.device)
 
     def eval(self, v):
@@ -56,15 +56,15 @@
         """ v: [B,C,H,W], lam: [B]
         """
         if len(lam.shape) == 1: lam = lam.view(lam.shape[0], 1, 1, 1)
 
         fn = self._prox
         fn = prox_scaled(fn, self.alpha)
         fn = prox_affine(fn, self.beta)
-        fn = prox_translated(fn, self.b)
+        fn = prox_translated(fn, self.offset)
         return fn(v, lam)
 
     def convex_conjugate_prox(self, v, lam):
         # use Moreau’s identity
         return v - self.prox(v / lam, lam)
 
     def _prox(self, v, lam):
```

### Comparing `dprox-0.0.2/dprox/proxfn/fast/cs.py` & `dprox-0.1.0/dprox/proxfn/fast/cs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/fast/csmri.py` & `dprox-0.1.0/dprox/proxfn/fast/csmri.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,15 @@
         self.mask = mask
         self.y = y
 
     def _prox(self, v, lam, num_psi):
         if len(lam.shape) == 1:
             lam = lam.view(lam.shape[0], 1, 1, 1)
         y = self.unwrap(self.y)
-        mask = self.unwrap(self.mask)
-        
-        mask = mask.expand(v.shape)
+        mask = self.unwrap(self.mask).bool()
 
         z = fft2(v)
         temp = ((lam * z.clone()) + y) / (1 + lam * num_psi)
         z[mask] = temp[mask]
         z = ifft2(z)
 
         return z
```

### Comparing `dprox-0.0.2/dprox/proxfn/fast/pr.py` & `dprox-0.1.0/dprox/proxfn/fast/pr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/fast/spi.py` & `dprox-0.1.0/dprox/proxfn/fast/spi.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/fast/sr.py` & `dprox-0.1.0/dprox/proxfn/fast/sr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from ..sum_square import ext_sum_squares
 from dprox.utils.misc import to_nn_parameter, to_torch_tensor
 
 
 class misr(ext_sum_squares):
     def __init__(self, linop, b, srf, eps=1e-7):
         super().__init__(linop, b, eps)
-        self.b = self.to_parameter(b)
+        self.offset = self.to_parameter(b)
         self.srf = srf
 
     def _reload(self, shape):
-        b = self.b.value
+        b = self.offset.value
         srf = self.srf
 
         srf = to_torch_tensor(srf).float()  # C*3
         b = to_torch_tensor(b, batch=True).float().cpu()
         N, C, H, W = b.shape
         z = b.reshape(N, C, H * W)  # N,3,H*W
```

### Comparing `dprox-0.0.2/dprox/proxfn/nlm/nlm.py` & `dprox-0.1.0/dprox/proxfn/nlm/nlm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/norm.py` & `dprox-0.1.0/dprox/proxfn/norm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/base.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/composite.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import cvxpy as cp
 import torch
 import torch.nn as nn
 
 
 class Augment(nn.Module):
     def __init__(self, base_denoiser):
         super().__init__()
@@ -53,14 +52,15 @@
                  deep_hypara_list=[40., 20., 10., 5.], tv_hypara_list=[10, 0.01]):
         self.deep_hypara_list = deep_hypara_list
         self.tv_hypara_list = tv_hypara_list
         self.tv_denoising = tv_denoising
         self.deep_denoise = deep_denoise
 
     def denoise(self, x):
+        import cvxpy as cp
         # x: 1,31,512,512
         deep_num = len(self.deep_hypara_list)
         tv_num = len(self.tv_hypara_list)
         deep_list = [self.deep_denoise(x, torch.tensor(level/255.).to(x.device)) for level in self.deep_hypara_list]
         deep_list = [tmp.squeeze().permute(1, 2, 0) for tmp in deep_list]
 
         tv_list = [self.tv_denoising(x.squeeze().permute(1, 2, 0), level, 5).clamp(0, 1) for level in self.tv_hypara_list]
```

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/TV_denoising.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/basicblock.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_dncnn.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/network_unet.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/pnp/denoisers/wrapper.py` & `dprox-0.1.0/dprox/proxfn/pnp/denoisers/wrapper.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/proxfn/sum_square.py` & `dprox-0.1.0/dprox/proxfn/sum_square.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 from typing import List
 
 import torch
-import torch.nn as nn
-import numpy as np
 
-from dprox.linop import LinOp, vstack, eval, adjoint, gram, CompGraph
-from dprox.utils import to_torch_tensor
-from .linear_solve import LINEAR_SOLVER
+from dprox.linop import LinOp, vstack, eval, adjoint
+# from .linalg import LINEAR_SOLVER
 
 from . import ProxFn
 
 
 class sum_squares(ProxFn):
     """ |x|_2^2 
     """
 
     def __init__(self, linop, b=None, eps=1e-7):
         super().__init__(linop)
         self.eps = eps
         self._b = b
 
     @property
-    def b(self):
+    def offset(self):
         if self._b is not None:
             return self.unwrap(self._b)
-        return super().b
+        return super().offset
 
     def _prox(self, v, lam):
         return v / (1 + 2 * lam)
 
     def grad(self, x):
-        tmp = eval(self.linop, [x])[0] - self.b
-        out = adjoint(self.linop, [tmp])[0]
+        tmp = eval(self.linop, x) - self.offset
+        out = adjoint(self.linop, tmp)
         return out
 
 
 class ext_sum_squares(sum_squares):
     def __init__(self, linop, eps=1e-7):
         super().__init__(linop, eps=eps)
 
@@ -54,24 +51,24 @@
     """ |Ax-b|_2^2 
         (AtA + I)^-1(Atb + v)
     """
 
     def __init__(self, linop, weight: LinOp, b, eps=0):
         super().__init__(linop, b, eps)
         self.weight = weight
-        if self.weight.is_gram_diag():
+        if self.weight.is_self_diag():
             self._prox_fn = self._prox
-        elif self.weight.is_gram_diag(freq=True):
+        elif self.weight.is_self_diag(freq=True):
             self._prox_fn = self._prox_freq
         else:
-            raise ValueError('weight must be diagonalizable')
+            raise ValueError('weight {} must be diagonalizable'.format(weight))
 
     @property
     def Ktb(self):
-        return adjoint(self.weight, [self.unwrap(self._b)])[0]
+        return adjoint(self.weight, self.unwrap(self._b))
 
     def prox(self, v, lam):
         return self._prox_fn(v, lam)
 
     def _prox(self, v, lam):
         if len(lam.shape) == 1:
             lam = lam.view(lam.shape[0], 1, 1, 1)
@@ -121,32 +118,37 @@
         else:
             return self.solve_cg(b, rho, v, **self.lin_solver_kwargs)
 
     def solve_direct(self, b, rho, v=None, eps=1e-7):
         device = rho.device
         Ktb = 0
         for fn in self.quad_fns:
-            Ktb += fn.dag.adjoint([fn.b])[0]
+            # TODO: ideally, we should rewrite the dag to remove offset, 
+            # then we don't need to specially process sum's adjoint.
+            out = fn.dag.adjoint(fn.offset)
+            if isinstance(out, LinOp.MultOutput):
+                out = out[0]
+            Ktb += out
         for i, fn in enumerate(self.other_fns):
-            Ktb += rho * fn.dag.adjoint([b[i]])[0]
+            Ktb += rho * fn.dag.adjoint(b[i])
         if v is not None:
             Ktb += rho * v
-        
+
         def get_diag(fn: ProxFn):
             # TODO: hack for derain, don't forgot change it back, Ktb -> Ktb.shape
             return fn.linop.get_diag(Ktb, freq=self.freq_diagonalizable)
 
         diag = 0
         for fn in self.quad_fns:
             diag = diag + get_diag(fn).to(device)
         for fn in self.other_fns:
             diag = diag + rho * get_diag(fn).to(device)
         if v is not None:
             diag = diag + rho
-        
+
         if self.freq_diagonalizable:
             Ktb = torch.fft.fftn(Ktb, dim=[-2, -1])
             out = torch.real(torch.fft.ifftn((Ktb + eps) / (diag + eps), dim=[-2, -1]))
         else:
             out = Ktb / (diag + eps)
 
         return out.float()
@@ -167,15 +169,15 @@
         Ktb = 0
         for fn in self.quad_fns:
             Ktb += fn.dag.adjoint([fn.b])[0]
         for i, fn in enumerate(self.other_fns):
             Ktb += rho * fn.dag.adjoint([b[i]])[0]
         if v is not None:
             Ktb += rho * v
-            
+
         init_with_last_pred = kwargs.pop('init_with_last_pred', False)
         lin_solver_type = kwargs.pop('lin_solver_type', 'cg2')
         lin_solver = LINEAR_SOLVER[lin_solver_type]
         if init_with_last_pred:
             x_init = self.last_x_pred if hasattr(self, 'last_x_pred') else None
             x_pred = lin_solver(KtK, Ktb, x_init=x_init, **kwargs)
             self.last_x_pred = x_pred
```

### Comparing `dprox-0.0.2/dprox/proxfn/unrolling/dgu.py` & `dprox-0.1.0/dprox/proxfn/unrolling/dgu.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/examples/csmri/common.py` & `dprox-0.1.0/dprox/utils/examples/csmri/common.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/examples/csmri/dataset.py` & `dprox-0.1.0/dprox/utils/examples/csmri/dataset.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/examples/csmri/misc.py` & `dprox-0.1.0/dprox/utils/examples/csmri/misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 import torch
 import torch.fft
 from PIL import Image
 from scipy.io import loadmat
 from torchlight.data import SingleImageDataset
 
 from dprox.utils import to_torch_tensor
-
-
-CURRENT_DIR = os.path.dirname(os.path.abspath(__file__))
+from dprox.utils.io import get_path
 
 
 def fft2(x):
     x = torch.fft.ifftshift(x, dim=(-2, -1))
     x = torch.fft.fft2(x, norm='ortho')
     x = torch.fft.fftshift(x, dim=(-2, -1))
     return x
@@ -25,20 +23,18 @@
     x = torch.fft.ifftshift(x, dim=(-2, -1))
     x = torch.fft.ifft2(x, norm='ortho')
     x = torch.fft.fftshift(x, dim=(-2, -1))
     return x
 
 
 def sample(name='Bust.jpg'):
-    base_dir = Path(os.path.join(CURRENT_DIR, 'data'))
-
-    mask = loadmat(base_dir / 'masks/radial_128_2.mat').get('mask')
+    mask = loadmat(get_path('data/csmri/masks/radial_128_2.mat')).get('mask')
     mask = mask.astype('bool')
 
-    imgpath = base_dir / 'Medical_128' / name
+    imgpath = get_path(os.path.join('data/csmri/Medical_128', name))
     target = Image.open(imgpath).convert('L')
     target = np.array(target, dtype=np.float32) / 255.0
 
     target = target[None]
     target = torch.from_numpy(target)
     mask = torch.from_numpy(mask)
 
@@ -56,17 +52,15 @@
     mask = to_torch_tensor(mask, batch=True)
     return Aty0.real, y0, target, mask
 
 
 class Dataset(SingleImageDataset):
     def __init__(self, root):
         super().__init__(root, mode='gray')
-        base_dir = Path(os.path.join(CURRENT_DIR, 'data'))
-
-        mask = loadmat(base_dir / 'masks/radial_128_2.mat').get('mask')
+        mask = loadmat(get_path('data/csmri/masks/radial_128_2.mat')).get('mask')
         mask = mask.astype('bool')
 
         self.mask = mask
 
     def __getitem__(self, index):
         target, path = super().__getitem__(index)
         target = torch.from_numpy(target)
```

### Comparing `dprox-0.0.2/dprox/utils/examples/optic/common.py` & `dprox-0.1.0/dprox/utils/examples/optic/common.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/examples/optic/doe_model.py` & `dprox-0.1.0/dprox/utils/examples/optic/doe_model.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/examples/optic/unet.py` & `dprox-0.1.0/dprox/utils/examples/optic/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/init/mosaic.py` & `dprox-0.1.0/dprox/utils/init/mosaic.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/init/sr.py` & `dprox-0.1.0/dprox/utils/init/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/metrics.py` & `dprox-0.1.0/dprox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox/utils/psf2otf.py` & `dprox-0.1.0/dprox/utils/psf2otf.py`

 * *Files identical despite different names*

### Comparing `dprox-0.0.2/dprox.egg-info/SOURCES.txt` & `dprox-0.1.0/dprox.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-LICENSE
 README.md
 setup.py
 dprox/__init__.py
 dprox.egg-info/PKG-INFO
 dprox.egg-info/SOURCES.txt
 dprox.egg-info/dependency_links.txt
+dprox.egg-info/requires.txt
 dprox.egg-info/top_level.txt
 dprox/algo/__init__.py
 dprox/algo/admm.py
 dprox/algo/base.py
 dprox/algo/hqs.py
 dprox/algo/invert.py
 dprox/algo/pc.py
 dprox/algo/pgd.py
 dprox/algo/problem.py
+dprox/algo/lp/__init__.py
+dprox/algo/lp/linear_solvers.py
+dprox/algo/lp/solvers.py
+dprox/algo/lp/utils.py
 dprox/algo/opt/__init__.py
 dprox/algo/opt/absorb.py
 dprox/algo/opt/equil.py
 dprox/algo/opt/merge.py
 dprox/algo/special/__init__.py
 dprox/algo/special/deq.py
 dprox/algo/special/unroll.py
@@ -28,21 +32,22 @@
 dprox/algo/special/deq_utils/radam.py
 dprox/algo/special/deq_utils/solvers.py
 dprox/algo/tune/__init__.py
 dprox/algo/tune/autotune.py
 dprox/algo/tune/dpir.py
 dprox/algo/tune/learnable.py
 dprox/linop/__init__.py
+dprox/linop/base.py
 dprox/linop/blackbox.py
 dprox/linop/comp_graph.py
+dprox/linop/constaints.py
 dprox/linop/constant.py
 dprox/linop/conv.py
 dprox/linop/edge.py
 dprox/linop/grad.py
-dprox/linop/lin_op.py
 dprox/linop/placeholder.py
 dprox/linop/scale.py
 dprox/linop/subsample.py
 dprox/linop/sum.py
 dprox/linop/variable.py
 dprox/linop/vstack.py
 dprox/proxfn/__init__.py
@@ -52,18 +57,22 @@
 dprox/proxfn/sum_square.py
 dprox/proxfn/fast/__init__.py
 dprox/proxfn/fast/cs.py
 dprox/proxfn/fast/csmri.py
 dprox/proxfn/fast/pr.py
 dprox/proxfn/fast/spi.py
 dprox/proxfn/fast/sr.py
-dprox/proxfn/linear_solve/__init__.py
-dprox/proxfn/linear_solve/cg.py
-dprox/proxfn/linear_solve/custom.py
-dprox/proxfn/linear_solve/torchcg.py
+dprox/proxfn/linalg/__init__.py
+dprox/proxfn/linalg/custom.py
+dprox/proxfn/linalg/solve/__init__.py
+dprox/proxfn/linalg/solve/bicgstab.py
+dprox/proxfn/linalg/solve/broyden.py
+dprox/proxfn/linalg/solve/cg.py
+dprox/proxfn/linalg/solve/gmres.py
+dprox/proxfn/linalg/solve/plss.py
 dprox/proxfn/nlm/__init__.py
 dprox/proxfn/nlm/nlm.py
 dprox/proxfn/nlm/patch_nlm.py
 dprox/proxfn/pnp/__init__.py
 dprox/proxfn/pnp/prior.py
 dprox/proxfn/pnp/denoisers/__init__.py
 dprox/proxfn/pnp/denoisers/base.py
@@ -88,26 +97,37 @@
 dprox/proxfn/pnp/denoisers/models/unet/__init__.py
 dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
 dprox/proxfn/pnp/denoisers/models/unet/unet.py
 dprox/proxfn/unrolling/__init__.py
 dprox/proxfn/unrolling/dgu.py
 dprox/proxfn/unrolling/prior.py
 dprox/utils/__init__.py
+dprox/utils/containar.py
 dprox/utils/io.py
 dprox/utils/metrics.py
 dprox/utils/misc.py
 dprox/utils/psf2otf.py
 dprox/utils/examples/__init__.py
-dprox/utils/examples/misc.py
-dprox/utils/examples/mosaic.py
+dprox/utils/examples/restoration.py
 dprox/utils/examples/csmri/__init__.py
 dprox/utils/examples/csmri/common.py
 dprox/utils/examples/csmri/dataset.py
 dprox/utils/examples/csmri/misc.py
+dprox/utils/examples/derain/__init__.py
+dprox/utils/examples/derain/custom_linop.py
+dprox/utils/examples/energy_system/__init__.py
 dprox/utils/examples/optic/__init__.py
 dprox/utils/examples/optic/common.py
 dprox/utils/examples/optic/doe_model.py
 dprox/utils/examples/optic/unet.py
 dprox/utils/init/__init__.py
 dprox/utils/init/mosaic.py
 dprox/utils/init/sr.py
-test/test_dpir.py
+tests/test_algorithms.py
+tests/test_energy_system.py
+tests/test_inverse_problems.py
+tests/test_linear_solver.py
+tests/test_linear_solver_grad.py
+tests/test_linear_solver_torch.py
+tests/test_linop.py
+tests/test_linop_primitive.py
+tests/test_ml_problems.py
```

