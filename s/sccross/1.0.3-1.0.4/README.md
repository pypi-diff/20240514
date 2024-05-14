# Comparing `tmp/sccross-1.0.3.tar.gz` & `tmp/sccross-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccross-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sccross-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sccross-1.0.3.tar` & `sccross-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2023-10-28 18:30:45.294486 sccross-1.0.3/LICENSE
--rw-r--r--   0        0        0     2351 2023-10-29 07:00:16.407759 sccross-1.0.3/README.md
--rw-r--r--   0        0        0     1937 2023-11-05 21:41:58.530486 sccross-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      629 2023-10-28 18:30:45.455335 sccross-1.0.3/sccross/__init__.py
--rw-r--r--   0        0        0    17811 2023-10-28 18:30:45.456327 sccross-1.0.3/sccross/data.py
--rw-r--r--   0        0        0     8859 2023-10-28 18:30:45.457323 sccross-1.0.3/sccross/metrics.py
--rw-r--r--   0        0        0     3014 2023-10-28 18:30:45.457323 sccross-1.0.3/sccross/models/__init__.py
--rw-r--r--   0        0        0    11735 2023-10-28 18:30:45.458320 sccross-1.0.3/sccross/models/data.py
--rw-r--r--   0        0        0    21125 2023-10-28 18:30:45.459324 sccross-1.0.3/sccross/models/layers.py
--rw-r--r--   0        0        0    76582 2023-11-05 20:54:30.796803 sccross-1.0.3/sccross/models/sccross.py
--rw-r--r--   0        0        0    25980 2023-10-28 18:30:45.461102 sccross-1.0.3/sccross/models/utils.py
--rw-r--r--   0        0        0    29842 2023-10-28 18:30:45.462102 sccross-1.0.3/sccross/utils.py
--rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 sccross-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-10-28 18:30:45.294486 sccross-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2426 2023-11-30 11:28:02.743664 sccross-1.0.4/README.md
+-rw-r--r--   0        0        0     1937 2024-05-14 07:00:30.528885 sccross-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-10-28 18:30:45.455335 sccross-1.0.4/sccross/__init__.py
+-rw-r--r--   0        0        0    17811 2023-10-28 18:30:45.456327 sccross-1.0.4/sccross/data.py
+-rw-r--r--   0        0        0     8859 2023-10-28 18:30:45.457323 sccross-1.0.4/sccross/metrics.py
+-rw-r--r--   0        0        0     3014 2023-10-28 18:30:45.457323 sccross-1.0.4/sccross/models/__init__.py
+-rw-r--r--   0        0        0    11735 2023-10-28 18:30:45.458320 sccross-1.0.4/sccross/models/data.py
+-rw-r--r--   0        0        0    17422 2024-04-08 20:25:48.188384 sccross-1.0.4/sccross/models/layers.py
+-rw-r--r--   0        0        0    76422 2024-05-14 06:53:55.596888 sccross-1.0.4/sccross/models/sccross.py
+-rw-r--r--   0        0        0    25980 2023-10-28 18:30:45.461102 sccross-1.0.4/sccross/models/utils.py
+-rw-r--r--   0        0        0    29842 2023-10-28 18:30:45.462102 sccross-1.0.4/sccross/utils.py
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 sccross-1.0.4/PKG-INFO
```

### Comparing `sccross-1.0.3/LICENSE` & `sccross-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/README.md` & `sccross-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # scCross
-A Deep Learning-Based Model for the integration, cross-dataset cross-modality generation, self enhancing and matched multi-omics simulation of single-cell multi-omics data. Our model excels at maintaining in-silico perturbations during cross-modality generation and harnessing these perturbations to identify key genes.
+A Deep Learning-Based Model for the integration, cross-dataset cross-modality generation, self augmentation and matched multi-omics simulation of single-cell multi-omics data. Our model excels at maintaining in-silico perturbations during cross-modality generation and harnessing these perturbations to identify key genes.
 
 For detailed instructions, comprehensive documentation, and helpful tutorials, please visit:
   
 * [https://sccross.readthedocs.io](https://sccross.readthedocs.io/en/latest/)
 
 
 ## Overview
 <img title="Model Overview" alt="Alt text" src="/figures/main.png">
 Single-cell multi-omics provides deep biological insights, but data scarcity and modality integration remain significant challenges. We introduce scCross, harnessing variational autoencoder and generative adversarial network (VAE-GAN) principles, meticulously designed to integrate diverse single-cell multi-omics data. Incorporating biological priors, scCross adeptly aligns modalities with enhanced relevance. Its standout feature is generating cross-modality single-cell data and in-silico perturbations, enabling deeper cellular state examinations and drug explorations. Applied to dual and triple-omics datasets, scCross maps data into a unified latent space, surpassing existing methods. By addressing data limitations and offering novel biological insights, scCross promises to advance single-cell research and therapeutic discovery.
 
 ## Key Capabilities
 
 1. Combine more than three single-cell multi-omics datasets, whether they are matched or unmatched, into a unified latent space. This space can be used for downstream analysis, even when dealing with over 4 million cells of varying types.
 
-2. Generate cross-compatible single-cell data between two different types in the training set.
+2. Generate cross-compatible single-cell data between two or more different omics. Trained and tested on independent referenced multi-omics datasets is also feasible.
 
 3. Augment single-cell omics data through self-improvement techniques.
 
 4. Simulate single-cell multi-omics data that match a specific cellular state, irrespective of the type and quantity of omics data involved.
 
 5. Accurately identify key genes by comparing two different cell clusters using in-silico perturbation methods.
```

### Comparing `sccross-1.0.3/pyproject.toml` & `sccross-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sccross"
-version = "1.0.3"
+version = "1.0.4"
 description = "Single cell multi-omics cross modal generation, multi-omics simulation and perturbation"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 
 keywords = ["bioinformatics", "deep-learning", "single-cell", "single-cell-multiomics"]
 classifiers = [
```

### Comparing `sccross-1.0.3/sccross/__init__.py` & `sccross-1.0.4/sccross/__init__.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/sccross/data.py` & `sccross-1.0.4/sccross/data.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/sccross/metrics.py` & `sccross-1.0.4/sccross/metrics.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/sccross/models/__init__.py` & `sccross-1.0.4/sccross/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/sccross/models/data.py` & `sccross-1.0.4/sccross/models/data.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/sccross/models/layers.py` & `sccross-1.0.4/sccross/models/layers.py`

 * *Files 20% similar despite different names*

```diff
@@ -367,99 +367,17 @@
         -------
         recon
             Data reconstruction distribution
         """
         raise NotImplementedError  # pragma: no cover
 
 
-class NormalDataDecoder(DataDecoder):
 
-    r"""
-    Normal data decoder
-
-    Parameters
-    ----------
-    out_features
-        Output dimensionality
-    n_batches
-        Number of batches
-    """
-
-    def __init__(self, out_features: int, n_batches: int = 1) -> None:
-        super().__init__(out_features, n_batches=n_batches)
-        self.scale_lin = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-        self.bias = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-        self.std_lin = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-
-    def forward(
-            self, u: torch.Tensor, v: torch.Tensor,
-            b: torch.Tensor, l: Optional[torch.Tensor]
-    ) -> D.Normal:
-        scale = F.softplus(self.scale_lin[b])
-        loc = scale * (u @ v.t()) + self.bias[b]
-        std = F.softplus(self.std_lin[b]) + EPS
-        return D.Normal(loc, std)
-
-
-class ZINDataDecoder(NormalDataDecoder):
 
-    r"""
-    Zero-inflated normal data decoder
-
-    Parameters
-    ----------
-    out_features
-        Output dimensionality
-    n_batches
-        Number of batches
-    """
-
-    def __init__(self, out_features: int, n_batches: int = 1) -> None:
-        super().__init__(out_features, n_batches=n_batches)
-        self.zi_logits = torch.nn.Parameter(torch.zeros(n_batches, out_features))
 
-    def forward(
-            self, u: torch.Tensor, v: torch.Tensor,
-            b: torch.Tensor, l: Optional[torch.Tensor]
-    ) -> ZIN:
-        scale = F.softplus(self.scale_lin[b])
-        loc = scale * (u @ v.t()) + self.bias[b]
-        std = F.softplus(self.std_lin[b]) + EPS
-        return ZIN(self.zi_logits[b].expand_as(loc), loc, std)
-
-
-class ZILNDataDecoder1(DataDecoder):
-
-    r"""
-    Zero-inflated log-normal data decoder
-
-    Parameters
-    ----------
-    out_features
-        Output dimensionality
-    n_batches
-        Number of batches
-    """
-
-    def __init__(self, out_features: int, n_batches: int = 1) -> None:
-        super().__init__(out_features, n_batches=n_batches)
-        self.scale_lin = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-        self.bias = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-        self.zi_logits = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-        self.std_lin = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-
-
-    def forward(
-            self, u: torch.Tensor, v: torch.Tensor,
-            b: torch.Tensor, l: Optional[torch.Tensor]
-    ) -> ZILN:
-        scale = F.softplus(self.scale_lin[b])
-        loc = scale * (u @ v.t()) + self.bias[b]
-        std = F.softplus(self.std_lin[b]) + EPS
-        return ZILN(self.zi_logits[b].expand_as(loc), loc, std)
 
 class ZILNDataDecoder(DataDecoder):
 
     r"""
     Zero-inflated log-normal data decoder
 
     Parameters
@@ -542,44 +460,15 @@
             log_theta.exp(),
             logits=(mu + EPS).log()
         )
 
 
 
 
-class ZINBDataDecoder(NBDataDecoder):
-
-    r"""
-    Zero-inflated negative binomial data decoder
-
-    Parameters
-    ----------
-    out_features
-        Output dimensionality
-    n_batches
-        Number of batches
-    """
 
-    def __init__(self, out_features: int, n_batches: int = 1) -> None:
-        super().__init__(out_features, n_batches=n_batches)
-        self.zi_logits = torch.nn.Parameter(torch.zeros(n_batches, out_features))
-
-    def forward(
-            self, u: torch.Tensor, v: torch.Tensor,
-            b: torch.Tensor, l: Optional[torch.Tensor]
-    ) -> ZINB:
-        scale = F.softplus(self.scale_lin[b])
-        logit_mu = scale * (u @ v.t()) + self.bias[b]
-        mu = F.softmax(logit_mu, dim=1) * l
-        log_theta = self.log_theta[b]
-        return ZINB(
-            self.zi_logits[b].expand_as(mu),
-            log_theta.exp(),
-            logits=(mu + EPS).log() - log_theta
-        )
 
 
 class Discriminator(torch.nn.Sequential, torch.nn.Module):
 
     r"""
     Domain discriminator
```

### Comparing `sccross-1.0.3/sccross/models/sccross.py` & `sccross-1.0.4/sccross/models/sccross.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,24 +140,21 @@
         Data probabilistic model
 
     Return
     ------
     decoder
         Decoder type
     """
-    if prob_model == "Normal":
-        return layers.NormalDataDecoder
-    if prob_model == "ZIN":
-        return layers.ZINDataDecoder
+
+
     if prob_model == "ZILN":
         return layers.ZILNDataDecoder
     if prob_model == "NB":
         return layers.NBDataDecoder
-    if prob_model == "ZINB":
-        return layers.ZINBDataDecoder
+
     raise ValueError("Invalid `prob_model`!")
 
 
 @logged
 class AnnDataset(Dataset):
 
     r"""
@@ -2165,15 +2162,15 @@
             temp.append(gene)
             adata_u = adata_perturb.copy()
             if isinstance(adata_u.X, scipy.sparse._csr.csr_matrix):
                 adata_u.X = np.array(adata_u.X.todense())
 
 
 
-            adata_u[:, gene].X += 1
+            adata_u[:, gene].X += 0.5*adata_u[:, gene].X
             sc.pp.normalize_total(adata_u)
             sc.pp.log1p(adata_u)
             sc.pp.scale(adata_u)
             sc.tl.pca(adata_u, n_comps=use_rep_dim, svd_solver="auto")
             adata_u.obsm[use_rep] = np.concatenate((adata_u.obsm[use_rep], adata_perturb.obsm[use_rep][:,use_rep_dim:use_rep_dim+5]), axis=1)
 
             data_u_t = AnnDataset(
@@ -2215,16 +2212,16 @@
 
             temp.append(cos_o - cos_u.mean())
 
             adata_d = adata_perturb.copy()
             if isinstance(adata_d.X, scipy.sparse._csr.csr_matrix):
                 adata_d.X = np.array(adata_d.X.todense())
 
-            adata_d[:, gene].X -= 1
-            adata_d.X[np.where(adata_d.X < 0.0)] = 0
+            adata_d[:, gene].X -= 0.5*adata_d[:, gene].X
+            #adata_d.X[np.where(adata_d.X < 0.0)] = 0
             sc.pp.normalize_total(adata_d)
             sc.pp.log1p(adata_d)
             sc.pp.scale(adata_d)
             sc.tl.pca(adata_d, n_comps=use_rep_dim, svd_solver="auto")
             adata_d.obsm[use_rep] = np.concatenate((adata_d.obsm[use_rep], adata_perturb.obsm[use_rep][:, use_rep_dim:use_rep_dim+5]),axis=1)
 
             data_d_t = AnnDataset(
```

### Comparing `sccross-1.0.3/sccross/models/utils.py` & `sccross-1.0.4/sccross/models/utils.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/sccross/utils.py` & `sccross-1.0.4/sccross/utils.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.3/PKG-INFO` & `sccross-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sccross
-Version: 1.0.3
+Version: 1.0.4
 Summary: Single cell multi-omics cross modal generation, multi-omics simulation and perturbation
 Keywords: bioinformatics,deep-learning,single-cell,single-cell-multiomics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -51,30 +51,30 @@
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Github, https://github.com/Xiuhui-Yang/scCross
 Provides-Extra: doc
 Provides-Extra: test
 
 # scCross
-A Deep Learning-Based Model for the integration, cross-dataset cross-modality generation, self enhancing and matched multi-omics simulation of single-cell multi-omics data. Our model excels at maintaining in-silico perturbations during cross-modality generation and harnessing these perturbations to identify key genes.
+A Deep Learning-Based Model for the integration, cross-dataset cross-modality generation, self augmentation and matched multi-omics simulation of single-cell multi-omics data. Our model excels at maintaining in-silico perturbations during cross-modality generation and harnessing these perturbations to identify key genes.
 
 For detailed instructions, comprehensive documentation, and helpful tutorials, please visit:
   
 * [https://sccross.readthedocs.io](https://sccross.readthedocs.io/en/latest/)
 
 
 ## Overview
 <img title="Model Overview" alt="Alt text" src="/figures/main.png">
 Single-cell multi-omics provides deep biological insights, but data scarcity and modality integration remain significant challenges. We introduce scCross, harnessing variational autoencoder and generative adversarial network (VAE-GAN) principles, meticulously designed to integrate diverse single-cell multi-omics data. Incorporating biological priors, scCross adeptly aligns modalities with enhanced relevance. Its standout feature is generating cross-modality single-cell data and in-silico perturbations, enabling deeper cellular state examinations and drug explorations. Applied to dual and triple-omics datasets, scCross maps data into a unified latent space, surpassing existing methods. By addressing data limitations and offering novel biological insights, scCross promises to advance single-cell research and therapeutic discovery.
 
 ## Key Capabilities
 
 1. Combine more than three single-cell multi-omics datasets, whether they are matched or unmatched, into a unified latent space. This space can be used for downstream analysis, even when dealing with over 4 million cells of varying types.
 
-2. Generate cross-compatible single-cell data between two different types in the training set.
+2. Generate cross-compatible single-cell data between two or more different omics. Trained and tested on independent referenced multi-omics datasets is also feasible.
 
 3. Augment single-cell omics data through self-improvement techniques.
 
 4. Simulate single-cell multi-omics data that match a specific cellular state, irrespective of the type and quantity of omics data involved.
 
 5. Accurately identify key genes by comparing two different cell clusters using in-silico perturbation methods.
```

