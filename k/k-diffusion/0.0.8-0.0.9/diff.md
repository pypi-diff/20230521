# Comparing `tmp/k-diffusion-0.0.8.tar.gz` & `tmp/k-diffusion-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-diffusion-0.0.8.tar", last modified: Sat Oct  1 09:07:03 2022, max compression
+gzip compressed data, was "k-diffusion-0.0.9.tar", last modified: Wed Oct  5 12:52:06 2022, max compression
```

## Comparing `k-diffusion-0.0.8.tar` & `k-diffusion-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 09:07:03.979699 k-diffusion-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-10-01 09:07:03.979699 k-diffusion-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 09:07:03.975699 k-diffusion-0.0.8/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4258 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (121)     9151 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 09:07:03.979699 k-diffusion-0.0.8/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8037 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    18727 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)    12930 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 09:07:03.979699 k-diffusion-0.0.8/k_diffusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-10-01 09:07:03.000000 k-diffusion-0.0.8/k_diffusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-01 09:07:03.000000 k-diffusion-0.0.8/k_diffusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-01 09:07:03.000000 k-diffusion-0.0.8/k_diffusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-01 09:07:03.000000 k-diffusion-0.0.8/k_diffusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-01 09:07:03.000000 k-diffusion-0.0.8/k_diffusion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-10-01 09:07:03.979699 k-diffusion-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-01 09:06:43.000000 k-diffusion-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 12:52:06.563614 k-diffusion-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-10-05 12:52:06.563614 k-diffusion-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 12:52:06.559615 k-diffusion-0.0.9/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4258 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5247 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9151 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 12:52:06.563614 k-diffusion-0.0.9/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8037 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18986 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12930 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 12:52:06.563614 k-diffusion-0.0.9/k_diffusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-10-05 12:52:06.000000 k-diffusion-0.0.9/k_diffusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-05 12:52:06.000000 k-diffusion-0.0.9/k_diffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 12:52:06.000000 k-diffusion-0.0.9/k_diffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-05 12:52:06.000000 k-diffusion-0.0.9/k_diffusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-05 12:52:06.000000 k-diffusion-0.0.9/k_diffusion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-10-05 12:52:06.563614 k-diffusion-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 12:51:52.000000 k-diffusion-0.0.9/setup.py
```

### Comparing `k-diffusion-0.0.8/LICENSE` & `k-diffusion-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/PKG-INFO` & `k-diffusion-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-diffusion
-Version: 0.0.8
+Version: 0.0.9
 Summary: Karras et al. (2022) diffusion models for PyTorch
 Home-page: https://github.com/crowsonkb/k-diffusion
 Author: Katherine Crowson
 Author-email: crowsonkb@gmail.com
 License: MIT
 Description: # k-diffusion
```

### Comparing `k-diffusion-0.0.8/README.md` & `k-diffusion-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion/augmentation.py` & `k-diffusion-0.0.9/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion/config.py` & `k-diffusion-0.0.9/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion/evaluation.py` & `k-diffusion-0.0.9/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion/external.py` & `k-diffusion-0.0.9/k_diffusion/external.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,39 +41,51 @@
 class DiscreteSchedule(nn.Module):
     """A mapping between continuous noise levels (sigmas) and a list of discrete noise
     levels."""
 
     def __init__(self, sigmas, quantize):
         super().__init__()
         self.register_buffer('sigmas', sigmas)
+        self.register_buffer('log_sigmas', sigmas.log())
         self.quantize = quantize
 
+    @property
+    def sigma_min(self):
+        return self.sigmas[0]
+
+    @property
+    def sigma_max(self):
+        return self.sigmas[-1]
+
     def get_sigmas(self, n=None):
         if n is None:
             return sampling.append_zero(self.sigmas.flip(0))
         t_max = len(self.sigmas) - 1
         t = torch.linspace(t_max, 0, n, device=self.sigmas.device)
         return sampling.append_zero(self.t_to_sigma(t))
 
     def sigma_to_t(self, sigma, quantize=None):
         quantize = self.quantize if quantize is None else quantize
-        dists = torch.abs(sigma - self.sigmas[:, None])
+        log_sigma = sigma.log()
+        dists = log_sigma - self.log_sigmas[:, None]
         if quantize:
-            return torch.argmin(dists, dim=0).view(sigma.shape)
-        low_idx, high_idx = torch.sort(torch.topk(dists, dim=0, k=2, largest=False).indices, dim=0)[0]
-        low, high = self.sigmas[low_idx], self.sigmas[high_idx]
-        w = (low - sigma) / (low - high)
+            return dists.abs().argmin(dim=0).view(sigma.shape)
+        low_idx = dists.ge(0).cumsum(dim=0).argmax(dim=0).clamp(max=self.log_sigmas.shape[0] - 2)
+        high_idx = low_idx + 1
+        low, high = self.log_sigmas[low_idx], self.log_sigmas[high_idx]
+        w = (low - log_sigma) / (low - high)
         w = w.clamp(0, 1)
         t = (1 - w) * low_idx + w * high_idx
         return t.view(sigma.shape)
 
     def t_to_sigma(self, t):
         t = t.float()
         low_idx, high_idx, w = t.floor().long(), t.ceil().long(), t.frac()
-        return (1 - w) * self.sigmas[low_idx] + w * self.sigmas[high_idx]
+        log_sigma = (1 - w) * self.log_sigmas[low_idx] + w * self.log_sigmas[high_idx]
+        return log_sigma.exp()
 
 
 class DiscreteEpsDDPMDenoiser(DiscreteSchedule):
     """A wrapper for discrete schedule DDPM models that output eps (the predicted
     noise)."""
 
     def __init__(self, model, alphas_cumprod, quantize):
```

### Comparing `k-diffusion-0.0.8/k_diffusion/gns.py` & `k-diffusion-0.0.9/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion/layers.py` & `k-diffusion-0.0.9/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion/models/image_v1.py` & `k-diffusion-0.0.9/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion/sampling.py` & `k-diffusion-0.0.9/k_diffusion/sampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     """Converts a denoiser output to a Karras ODE derivative."""
     return (x - denoised) / utils.append_dims(sigma, x.ndim)
 
 
 def get_ancestral_step(sigma_from, sigma_to, eta=1.):
     """Calculates the noise level (sigma_down) to step down to and the amount
     of noise to add (sigma_up) when doing an ancestral sampling step."""
+    if not eta:
+        return sigma_to, 0.
     sigma_up = min(sigma_to, eta * (sigma_to ** 2 * (sigma_from ** 2 - sigma_to ** 2) / sigma_from ** 2) ** 0.5)
     sigma_down = (sigma_to ** 2 - sigma_up ** 2) ** 0.5
     return sigma_down, sigma_up
 
 
 @torch.no_grad()
 def sample_euler(model, x, sigmas, extra_args=None, callback=None, disable=None, s_churn=0., s_tmin=0., s_tmax=float('inf'), s_noise=1.):
@@ -313,95 +315,100 @@
         eps_r1, eps_cache = self.eps(eps_cache, 'eps_r1', u1, s1)
         u2 = x - self.sigma(s2) * (r2 * h).expm1() * eps - self.sigma(s2) * (r2 / r1) * ((r2 * h).expm1() / (r2 * h) - 1) * (eps_r1 - eps)
         eps_r2, eps_cache = self.eps(eps_cache, 'eps_r2', u2, s2)
         x_3 = x - self.sigma(t_next) * h.expm1() * eps - self.sigma(t_next) / r2 * (h.expm1() / h - 1) * (eps_r2 - eps)
         return x_3, eps_cache
 
     def dpm_solver_fast(self, x, t_start, t_end, nfe, eta=0., s_noise=1.):
+        if not t_end > t_start and eta:
+            raise ValueError('eta must be 0 for reverse sampling')
+
         m = math.floor(nfe / 3) + 1
         ts = torch.linspace(t_start, t_end, m + 1, device=x.device)
 
         if nfe % 3 == 0:
             orders = [3] * (m - 2) + [2, 1]
         else:
             orders = [3] * (m - 1) + [nfe % 3]
 
         for i in range(len(orders)):
             eps_cache = {}
             t, t_next = ts[i], ts[i + 1]
-            gamma = eta * torch.sqrt(2 * (t_next - t).abs())
-            t = torch.maximum(torch.minimum(t_start, t_end), t - gamma.log1p())
-            noise = torch.randn_like(x) * s_noise
-            if t < ts[i]:
-                x = x + noise * (self.sigma(t) ** 2 - self.sigma(ts[i]) ** 2).sqrt()
+            if eta:
+                sd, su = get_ancestral_step(self.sigma(t), self.sigma(t_next), eta)
+                t_next_ = torch.minimum(t_end, self.t(sd))
+                su = (self.sigma(t_next) ** 2 - self.sigma(t_next_) ** 2) ** 0.5
+            else:
+                t_next_, su = t_next, 0.
 
             eps, eps_cache = self.eps(eps_cache, 'eps', x, t)
             denoised = x - self.sigma(t) * eps
             if self.info_callback is not None:
                 self.info_callback({'x': x, 'i': i, 't': ts[i], 't_up': t, 'denoised': denoised})
 
             if orders[i] == 1:
-                x, eps_cache = self.dpm_solver_1_step(x, t, t_next, eps_cache=eps_cache)
+                x, eps_cache = self.dpm_solver_1_step(x, t, t_next_, eps_cache=eps_cache)
             elif orders[i] == 2:
-                x, eps_cache = self.dpm_solver_2_step(x, t, t_next, eps_cache=eps_cache)
+                x, eps_cache = self.dpm_solver_2_step(x, t, t_next_, eps_cache=eps_cache)
             else:
-                x, eps_cache = self.dpm_solver_3_step(x, t, t_next, eps_cache=eps_cache)
+                x, eps_cache = self.dpm_solver_3_step(x, t, t_next_, eps_cache=eps_cache)
+
+            x = x + su * s_noise * torch.randn_like(x)
 
         return x
 
     def dpm_solver_adaptive(self, x, t_start, t_end, order=3, rtol=0.05, atol=0.0078, h_init=0.05, pcoeff=0., icoeff=1., dcoeff=0., accept_safety=0.81, eta=0., s_noise=1.):
         if order not in {2, 3}:
             raise ValueError('order should be 2 or 3')
         forward = t_end > t_start
+        if not forward and eta:
+            raise ValueError('eta must be 0 for reverse sampling')
         h_init = abs(h_init) * (1 if forward else -1)
         atol = torch.tensor(atol)
         rtol = torch.tensor(rtol)
         s = t_start
         x_prev = x
         accept = True
-        pid = PIDStepSizeController(h_init, pcoeff, icoeff, dcoeff, order, accept_safety)
+        pid = PIDStepSizeController(h_init, pcoeff, icoeff, dcoeff, 1.5 if eta else order, accept_safety)
         info = {'steps': 0, 'nfe': 0, 'n_accept': 0, 'n_reject': 0}
 
         while s < t_end - 1e-5 if forward else s > t_end + 1e-5:
             eps_cache = {}
             t = torch.minimum(t_end, s + pid.h) if forward else torch.maximum(t_end, s + pid.h)
+            if eta:
+                sd, su = get_ancestral_step(self.sigma(s), self.sigma(t), eta)
+                t_ = torch.minimum(t_end, self.t(sd))
+                su = (self.sigma(t) ** 2 - self.sigma(t_) ** 2) ** 0.5
+            else:
+                t_, su = t, 0.
 
-            gamma = eta * torch.sqrt(2 * (t - s).abs())
-            s_ = torch.maximum(torch.minimum(t_start, t_end), s - gamma.log1p())
-            x_pre_noise = x
-            if accept:
-                noise = torch.randn_like(x) * s_noise
-            if s_ < s:
-                x = x + noise * (self.sigma(s_) ** 2 - self.sigma(s) ** 2).sqrt()
-
-            eps, eps_cache = self.eps(eps_cache, 'eps', x, s_)
-            denoised = x - self.sigma(s_) * eps
+            eps, eps_cache = self.eps(eps_cache, 'eps', x, s)
+            denoised = x - self.sigma(s) * eps
 
             if order == 2:
-                x_low, eps_cache = self.dpm_solver_1_step(x, s_, t, eps_cache=eps_cache)
-                x_high, eps_cache = self.dpm_solver_2_step(x, s_, t, eps_cache=eps_cache)
+                x_low, eps_cache = self.dpm_solver_1_step(x, s, t_, eps_cache=eps_cache)
+                x_high, eps_cache = self.dpm_solver_2_step(x, s, t_, eps_cache=eps_cache)
             else:
-                x_low, eps_cache = self.dpm_solver_2_step(x, s_, t, r1=1 / 3, eps_cache=eps_cache)
-                x_high, eps_cache = self.dpm_solver_3_step(x, s_, t, eps_cache=eps_cache)
+                x_low, eps_cache = self.dpm_solver_2_step(x, s, t_, r1=1 / 3, eps_cache=eps_cache)
+                x_high, eps_cache = self.dpm_solver_3_step(x, s, t_, eps_cache=eps_cache)
             delta = torch.maximum(atol, rtol * torch.maximum(x_low.abs(), x_prev.abs()))
             error = torch.linalg.norm((x_low - x_high) / delta) / x.numel() ** 0.5
             accept = pid.propose_step(error)
             if accept:
                 x_prev = x_low
-                x = x_high
+                x = x_high + su * s_noise * torch.randn_like(x_high)
                 s = t
                 info['n_accept'] += 1
             else:
-                x = x_pre_noise
                 info['n_reject'] += 1
             info['nfe'] += order
             info['steps'] += 1
 
             if self.info_callback is not None:
-                self.info_callback({'x': x, 'i': info['steps'] - 1, 't': s, 't_up': s_, 'denoised': denoised, 'error': error, 'h': pid.h, **info})
+                self.info_callback({'x': x, 'i': info['steps'] - 1, 't': s, 't_up': s, 'denoised': denoised, 'error': error, 'h': pid.h, **info})
 
         return x, info
 
 
 @torch.no_grad()
 def sample_dpm_fast(model, x, sigma_min, sigma_max, n, extra_args=None, callback=None, disable=None, eta=0., s_noise=1.):
     """DPM-Solver-Fast (fixed step size). See https://arxiv.org/abs/2206.00927."""
```

### Comparing `k-diffusion-0.0.8/k_diffusion/utils.py` & `k-diffusion-0.0.9/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `k-diffusion-0.0.8/k_diffusion.egg-info/PKG-INFO` & `k-diffusion-0.0.9/k_diffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-diffusion
-Version: 0.0.8
+Version: 0.0.9
 Summary: Karras et al. (2022) diffusion models for PyTorch
 Home-page: https://github.com/crowsonkb/k-diffusion
 Author: Katherine Crowson
 Author-email: crowsonkb@gmail.com
 License: MIT
 Description: # k-diffusion
```

### Comparing `k-diffusion-0.0.8/setup.cfg` & `k-diffusion-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = k-diffusion
-version = 0.0.8
+version = 0.0.9
 author = Katherine Crowson
 author_email = crowsonkb@gmail.com
 url = https://github.com/crowsonkb/k-diffusion
 description = Karras et al. (2022) diffusion models for PyTorch
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

