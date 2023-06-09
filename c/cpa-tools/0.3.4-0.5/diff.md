# Comparing `tmp/cpa-tools-0.3.4.tar.gz` & `tmp/cpa-tools-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpa-tools-0.3.4.tar", max compression
+gzip compressed data, was "cpa-tools-0.5.tar", max compression
```

## Comparing `cpa-tools-0.3.4.tar` & `cpa-tools-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1517 2022-04-01 23:55:03.874861 cpa-tools-0.3.4/LICENSE
--rw-r--r--   0        0        0     1250 2022-04-02 00:17:06.103882 cpa-tools-0.3.4/README.md
--rw-r--r--   0        0        0      414 2022-07-29 12:08:20.495796 cpa-tools-0.3.4/cpa/__init__.py
--rw-r--r--   0        0        0    43639 2022-08-11 03:26:43.524454 cpa-tools-0.3.4/cpa/_api.py
--rw-r--r--   0        0        0     2229 2022-08-20 01:22:22.061574 cpa-tools-0.3.4/cpa/_data.py
--rw-r--r--   0        0        0     2691 2022-08-20 06:10:47.643977 cpa-tools-0.3.4/cpa/_metrics.py
--rw-r--r--   0        0        0    19914 2022-08-20 01:17:08.158404 cpa-tools-0.3.4/cpa/_model.py
--rw-r--r--   0        0        0    34643 2022-08-19 21:49:34.579313 cpa-tools-0.3.4/cpa/_module.py
--rw-r--r--   0        0        0    42293 2022-04-02 00:05:11.287541 cpa-tools-0.3.4/cpa/_plotting.py
--rw-r--r--   0        0        0    14322 2022-08-19 20:50:00.904851 cpa-tools-0.3.4/cpa/_task.py
--rw-r--r--   0        0        0     7965 2022-08-18 11:20:58.645313 cpa-tools-0.3.4/cpa/_utils.py
--rw-r--r--   0        0        0     3161 2022-08-20 05:52:47.774840 cpa-tools-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3044 2022-08-20 06:13:59.501964 cpa-tools-0.3.4/setup.py
--rw-r--r--   0        0        0     3946 2022-08-20 06:13:59.502563 cpa-tools-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1517 2022-04-01 23:55:03.874861 cpa-tools-0.5/LICENSE
+-rw-r--r--   0        0        0     1079 2023-03-02 23:38:15.247636 cpa-tools-0.5/README.md
+-rw-r--r--   0        0        0      414 2022-07-29 12:08:20.495796 cpa-tools-0.5/cpa/__init__.py
+-rw-r--r--   0        0        0    43624 2023-03-06 06:00:03.914642 cpa-tools-0.5/cpa/_api.py
+-rw-r--r--   0        0        0     2296 2023-03-07 03:47:44.190154 cpa-tools-0.5/cpa/_data.py
+-rw-r--r--   0        0        0     2691 2022-08-20 06:10:47.643977 cpa-tools-0.5/cpa/_metrics.py
+-rw-r--r--   0        0        0    22493 2023-06-09 04:27:08.479657 cpa-tools-0.5/cpa/_model.py
+-rw-r--r--   0        0        0    16496 2023-06-09 04:28:57.055398 cpa-tools-0.5/cpa/_module.py
+-rw-r--r--   0        0        0    42293 2022-04-02 00:05:11.287541 cpa-tools-0.5/cpa/_plotting.py
+-rw-r--r--   0        0        0    24812 2023-06-09 05:04:15.310286 cpa-tools-0.5/cpa/_task.py
+-rw-r--r--   0        0        0     7572 2023-06-09 04:29:36.955303 cpa-tools-0.5/cpa/_utils.py
+-rw-r--r--   0        0        0     3159 2023-06-09 05:28:19.574753 cpa-tools-0.5/pyproject.toml
+-rw-r--r--   0        0        0     2866 2023-06-09 05:30:27.929135 cpa-tools-0.5/setup.py
+-rw-r--r--   0        0        0     3773 2023-06-09 05:30:27.929622 cpa-tools-0.5/PKG-INFO
```

### Comparing `cpa-tools-0.3.4/LICENSE` & `cpa-tools-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpa-tools-0.3.4/README.md` & `cpa-tools-0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,12 +17,7 @@
 -------------------------------
 See [here](https://cpa-tools.readthedocs.io/en/latest/index.html) for documentation and tutorials.
 
 Support and contribute
 -------------------------------
 If you have a question or new architecture or a model that could be integrated into our pipeline, you can
 post an [issue](https://github.com/theislab/cpa/issues/new)
-
-
-###### Acknowledgment
-This code is inspired by an early implementatiom by [Pierre Boyeau](https://github.com/PierreBoyeau) using [scvi-tools](https://scvi-tools.org/).
-
```

### Comparing `cpa-tools-0.3.4/cpa/_api.py` & `cpa-tools-0.5/cpa/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
             self.de_genes = None
 
         self.split_key = model.split_key
         data_types = list(np.unique(adata.obs[self.split_key])) + ['all']
 
         self.unique_perts = list(model.drug_encoder.keys())
         self.unique_covars = {}
-        for covar in model.cat_covars_encoders.keys():
-            self.unique_covars[covar] = list(model.cat_covars_encoders[covar].keys())
+        for covar in model.covars_encoder.keys():
+            self.unique_covars[covar] = list(model.covars_encoder[covar].keys())
 
         self.num_drugs = len(model.drug_encoder)
 
         self.perts_dict = model.drug_encoder.copy()
-        self.covars_dict = model.cat_covars_encoders.copy()
+        self.covars_dict = model.covars_encoder.copy()
 
         self.emb_covars = None
         self.emb_perts = None
         self.seen_covars_perts = None
         self.comb_emb = None
         self.control_cat = None
 
@@ -243,18 +243,18 @@
 
         df = pd.DataFrame(columns=[self.perturbation_key, self.dose_key, 'response'])
 
         for drug in perturbations:
             d = self.perts_dict[drug]
             this_drug = torch.Tensor(dose).to(self.model.device).view(-1, 1)
             if self.model.module.doser_type == 'mlp':
-                response = (self.model.module.drug_network.dosers[d](this_drug).sigmoid() * this_drug.gt(
+                response = (self.model.module.pert_network.dosers[d](this_drug).sigmoid() * this_drug.gt(
                     0)).cpu().clone().detach().numpy().reshape(-1)
             else:
-                response = self.model.module.drug_network.dosers.one_drug(this_drug.view(-1),
+                response = self.model.module.pert_network.dosers.one_drug(this_drug.view(-1),
                                                                           d).cpu().clone().detach().numpy().reshape(-1)
 
             df_drug = pd.DataFrame(list(zip([drug] * n_points, dose, list(response))),
                                    columns=[self.perturbation_key, self.dose_key, 'response'])
             df = pd.concat([df, df_drug], ignore_index=True)
 
         return df
@@ -291,18 +291,18 @@
         df = pd.DataFrame(columns=perturbations + ['response'])
         response = {}
 
         for drug in perturbations:
             d = self.perts_dict[drug]
             this_drug = torch.Tensor(dose).to(self.model.device).view(-1, 1)
             if self.model.module.doser_type == 'mlp':
-                response[drug] = (self.model.module.drug_network.dosers[d](this_drug).sigmoid() * this_drug.gt(
+                response[drug] = (self.model.module.pert_network.dosers[d](this_drug).sigmoid() * this_drug.gt(
                     0)).cpu().clone().detach().numpy().reshape(-1)
             else:
-                response[drug] = self.model.module.drug_network.dosers.one_drug(this_drug.view(-1),
+                response[drug] = self.model.module.pert_network.dosers.one_drug(this_drug.view(-1),
                                                                                 d).cpu().clone().detach().numpy().reshape(
                     -1)
 
         l = 0
         for i in range(len(dose)):
             for j in range(len(dose)):
                 df.loc[l] = [dose[i], dose[j], response[perturbations[0]][i] + response[perturbations[1]][j]]
```

### Comparing `cpa-tools-0.3.4/cpa/_data.py` & `cpa-tools-0.5/cpa/_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,21 @@
         self.data_loader_kwargs = kwargs
         self.use_gpu = use_gpu
         self.train_idx = train_indices
         self.val_idx = valid_indices
         self.test_idx = test_indices
 
     def setup(self, stage: Optional[str] = None):
-        gpus, self.device = parse_use_gpu_arg(self.use_gpu, return_device=True)
+        accelerator, _, self.device = parse_use_gpu_arg(
+            self.use_gpu, return_device=True
+        )
         self.pin_memory = (
-            True if (settings.dl_pin_memory_gpu_training and gpus != 0) else False
+            True
+            if (settings.dl_pin_memory_gpu_training and accelerator == "gpu")
+            else False
         )
 
     def train_dataloader(self):
         if len(self.train_idx) > 0:
             return AnnDataLoader(
                 self.adata_manager,
                 indices=self.train_idx,
```

### Comparing `cpa-tools-0.3.4/cpa/_metrics.py` & `cpa-tools-0.5/cpa/_metrics.py`

 * *Files identical despite different names*

### Comparing `cpa-tools-0.3.4/cpa/_model.py` & `cpa-tools-0.5/cpa/_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from scvi.data import AnnDataManager
 from scvi.dataloaders import DataSplitter
 from torch.nn import functional as F
 from scvi.data.fields import (
     LayerField,
     CategoricalObsField,
     NumericalObsField,
-    NumericalJointObsField,
     ObsmField,
 )
 
 from anndata import AnnData
 from scvi.model.base import BaseModelClass
 from scvi.train import TrainRunner
 from scvi.train._callbacks import SaveBestState
@@ -41,15 +40,15 @@
         ----------
         adata : Anndata
             Registered Annotation Dataset
 
         n_latent: int
             Number of latent dimensions used for drug and Autoencoder
 
-        loss_ae: str
+        recon_loss: str
             Either `gauss` or `NB`. Autoencoder loss function.
 
         doser_type: str
             Type of doser network. Either `sigm`, `logsigm` or `mlp`.
 
         split_key : str, optional
             Key used to split the data between train test and validation.
@@ -62,71 +61,63 @@
 
         Examples
         --------
         >>> import cpa
         >>> import scanpy as sc
         >>> adata = sc.read('dataset.h5ad')
         >>> adata = cpa.CPA.setup_anndata(adata,
-                                          drug_key='condition',
-                                          dose_key='dose_val',
+                                          perturbation_keys={'perturbation': 'condition',  'dosage': 'dose_val'},
                                           categorical_covariate_keys=['cell_type'],
                                           control_key='control'
                                           )
         >>> hyperparams = {'autoencoder_depth': 3, 'autoencoder_width': 256}
         >>> model = cpa.CPA(adata,
                             n_latent=256,
                             loss_ae='gauss',
                             doser_type='logsigm',
                             split_key='split',
                             )
     """
-    cat_covars_encoders: dict = None
-    drug_encoder: dict = None
-    cont_covars: list = None
+    covars_encoder: dict = None
+    pert_encoder: dict = None
 
     def __init__(
             self,
             adata: AnnData,
-            n_latent: int = 128,
-            loss_ae: str = 'gauss',
-            doser_type: str = 'logsigm',
             split_key: str = None,
-            train_split: str = 'train',
-            valid_split: str = 'test',
-            test_split: str = 'ood',
+            train_split: Union[str, List[str]] = 'train',
+            valid_split: Union[str, List[str]] = 'test',
+            test_split: Union[str, List[str]] = 'ood',
             **hyper_params,
     ):
         super().__init__(adata)
-        self.drug_encoder = CPA.drug_encoder
-        self.cat_covars_encoders = CPA.cat_covars_encoders
 
-        self.n_genes = adata.n_vars
-        self.n_drugs = len(self.drug_encoder)
         self.split_key = split_key
 
-        self.drugs = list(self.drug_encoder.keys())
+        self.drugs = list(self.pert_encoder.keys())
         self.covars = {
-            covar: list(self.cat_covars_encoders[covar].keys()) for covar in self.cat_covars_encoders.keys()
+            covar: list(self.covars_encoder[covar].keys()) for covar in self.covars_encoder.keys()
         }
 
         self.module = CPAModule(
-            n_genes=self.n_genes,
-            n_drugs=self.n_drugs,
-            cat_covars_encoder=self.cat_covars_encoders,
-            n_latent=n_latent,
-            loss_ae=loss_ae,
-            doser_type=doser_type,
+            n_genes=adata.n_vars,
+            n_perts=len(self.pert_encoder),
+            covars_encoder=self.covars_encoder,
             **hyper_params,
         ).float()
 
         train_indices, valid_indices, test_indices = None, None, None
         if split_key is not None:
-            train_indices = np.where(adata.obs.loc[:, split_key] == train_split)[0]
-            valid_indices = np.where(adata.obs.loc[:, split_key] == valid_split)[0]
-            test_indices = np.where(adata.obs.loc[:, split_key] == test_split)[0]
+            train_split = train_split if isinstance(train_split, list) else [train_split]
+            valid_split = valid_split if isinstance(valid_split, list) else [valid_split]
+            test_split = test_split if isinstance(test_split, list) else [test_split]
+
+            train_indices = np.where(adata.obs.loc[:, split_key].isin(train_split))[0]
+            valid_indices = np.where(adata.obs.loc[:, split_key].isin(valid_split))[0]
+            test_indices = np.where(adata.obs.loc[:, split_key].isin(test_split))[0]
 
         self.train_indices = train_indices
         self.valid_indices = valid_indices
         self.test_indices = test_indices
 
         self._model_summary_string = f"Compositional Perturbation Autoencoder"
 
@@ -135,111 +126,167 @@
         self.epoch_history = None
 
     @classmethod
     @setup_anndata_dsp.dedent
     def setup_anndata(
             cls,
             adata: AnnData,
-            perturbation_keys: Dict[str, str],
-            use_counts: Optional[bool] = False,
-            categorical_covariate_keys: Optional[List[str]] = [],
-            continuous_covariate_keys: Optional[List[str]] = [],
-            control_key: Optional[str] = None,
+            perturbation_key: str,
+            control_group: str,
+            dosage_key: str,
+            batch_key: Optional[str] = None,
+            layer: Optional[str] = None,
+            is_count_data: Optional[bool] = False,
+            categorical_covariate_keys: Optional[List[str]] = None,
             deg_uns_key: Optional[str] = None,
+            deg_uns_cat_key: Optional[str] = None,
+            verbose: bool = False,
+            max_comb_len: int = 2,
             **kwargs,
     ):
         """
         Annotation Data setup function
 
         Parameters
         ----------
         adata
 
         categorical_covariate_keys
 
         continuous_covariate_keys
 
         """
-        CPA_REGISTRY_KEYS.PERTURBATION_KEYS = perturbation_keys
+        CPA_REGISTRY_KEYS.PERTURBATION_KEY = perturbation_key
+        CPA_REGISTRY_KEYS.DOSAGE_KEY = dosage_key
         CPA_REGISTRY_KEYS.CAT_COV_KEYS = categorical_covariate_keys
-        CPA_REGISTRY_KEYS.CONT_COV_KEYS = continuous_covariate_keys
+        CPA_REGISTRY_KEYS.MAX_COMB_LENGTH = max_comb_len
+        CPA_REGISTRY_KEYS.BATCH_KEY = batch_key
 
-        drug_key = perturbation_keys['perturbation']
-        dose_key = perturbation_keys['dosage']
+        perturbations = adata.obs[perturbation_key].astype(str).values
+        dosages = adata.obs[dosage_key].astype(str).values
 
-        drugs = adata.obs[drug_key]
-        dosages = adata.obs[dose_key].astype(str)
+        category_key = f'{cls.__name__}_cat'
+        keys = categorical_covariate_keys + [perturbation_key]
 
-        # get unique drugs
-        drugs_names_unique = set()
-        for d in np.unique(drugs):
-            [drugs_names_unique.add(i) for i in d.split("+")]
-        drugs_names_unique = sorted(list(np.array(list(drugs_names_unique))))
-
-        drugs_obsm = np.zeros((adata.n_obs, len(drugs_names_unique)))
-        for i in tqdm(range(adata.n_obs)):
-            cell_drugs = np.isin(drugs_names_unique, drugs[i].split('+'))
-            cell_doses = np.array(dosages[i].split("+")).astype(np.float32)
-            drugs_obsm[i, cell_drugs] = cell_doses
+        adata.obs[category_key] = adata.obs[keys].apply(lambda x: '_'.join(x), axis=1)
+        CPA_REGISTRY_KEYS.CATEGORY_KEY = category_key
+
+        if cls.pert_encoder is None:
+            # get unique drugs
+            perts_names_unique = set()
+            for d in np.unique(perturbations):
+                [perts_names_unique.add(i) for i in d.split("+") if i != control_group]
+            perts_names_unique = ['<PAD>', control_group] + sorted(list(perts_names_unique))
+            CPA_REGISTRY_KEYS.PADDING_IDX = 0
 
-        adata.obsm['drugs_doses'] = np.array(drugs_obsm)
+            pert_encoder = {pert: i for i, pert in
+                            enumerate(perts_names_unique)}
 
-        drug_encoder = {drug: i for i, drug in
-                        enumerate(drugs_names_unique)}
+        else:
+            pert_encoder = cls.pert_encoder
+            perts_names_unique = list(pert_encoder.keys())
+
+        pert_map = {}
+        for condition in tqdm(perts_names_unique):
+            perts_list = np.where(np.isin(perts_names_unique, condition.split('+')))[0]
+            pert_map[condition] = list(perts_list) + [CPA_REGISTRY_KEYS.PADDING_IDX for _ in
+                                                      range(max_comb_len - len(perts_list))]
+
+        dose_map = {}
+        for dosage_str in tqdm(dosages):
+            dosages_list = [float(i) for i in dosage_str.split('+')]
+            dose_map[dosage_str] = list(dosages_list) + [0.0 for _ in range(max_comb_len - len(dosages_list))]
+
+        data_perts = np.vstack(np.vectorize(lambda x: pert_map[x], otypes=[np.ndarray])(perturbations)).astype(int)
+        adata.obsm[CPA_REGISTRY_KEYS.PERTURBATIONS] = data_perts
+
+        data_perts_dosages = np.vstack(np.vectorize(lambda x: dose_map[x], otypes=[np.ndarray])(dosages)).astype(float)
+        adata.obsm[CPA_REGISTRY_KEYS.PERTURBATIONS_DOSAGES] = data_perts_dosages
+
+        # setup control column
+        control_key = f"{cls.__name__}_{control_group}"
+        CPA_REGISTRY_KEYS.CONTROL_KEY = control_key
+        adata.obs[control_key] = (adata.obs[perturbation_key] == control_group).astype(int)
 
         setup_method_args = cls._get_setup_method_args(**locals())
         anndata_fields = \
             [
-                LayerField(registry_key=CPA_REGISTRY_KEYS.X_KEY, layer='counts' if use_counts else None,
-                           is_count_data=True if use_counts else False),
-                ObsmField('drugs_doses', 'drugs_doses', is_count_data=False, correct_data_format=True)
+                LayerField(registry_key=CPA_REGISTRY_KEYS.X_KEY,
+                           layer=layer,
+                           is_count_data=is_count_data),
+                ObsmField(CPA_REGISTRY_KEYS.PERTURBATIONS, CPA_REGISTRY_KEYS.PERTURBATIONS,
+                          is_count_data=True, correct_data_format=True),
+                ObsmField(CPA_REGISTRY_KEYS.PERTURBATIONS_DOSAGES, CPA_REGISTRY_KEYS.PERTURBATIONS_DOSAGES,
+                          is_count_data=False, correct_data_format=True),
+                CategoricalObsField(registry_key=CPA_REGISTRY_KEYS.PERTURBATION_KEY, attr_key=perturbation_key),
             ] + \
-            [CategoricalObsField(registry_key=covar, obs_key=covar) for covar in categorical_covariate_keys] + \
-            [NumericalObsField(registry_key=covar, obs_key=covar) for covar in continuous_covariate_keys]
+            [CategoricalObsField(registry_key=covar, attr_key=covar) for covar in categorical_covariate_keys]
 
-        if control_key:
-            anndata_fields.append(NumericalObsField(registry_key='control', obs_key=control_key))
+        anndata_fields.append(NumericalObsField(registry_key=control_key, attr_key=control_key))
+        anndata_fields.append(CategoricalObsField(registry_key=category_key, attr_key=category_key))
 
         if deg_uns_key:
-            mask = np.zeros((adata.n_obs, adata.n_vars))
-            for i, cov_drug in tqdm(enumerate(adata.obs['cov_drug'].values)):
-                if cov_drug in adata.uns[deg_uns_key].keys():
-                    mask[i] = adata.var.index.isin(adata.uns[deg_uns_key][cov_drug]).astype(np.int)
-                else:
-                    mask[i] = 1
+            n_deg_r2 = kwargs.pop('n_deg_r2', 10)
 
-            adata.obsm['deg_mask'] = np.array(mask)
+            cov_cond_unique = np.unique(adata.obs[deg_uns_cat_key].astype(str).values)
 
-            anndata_fields.append(ObsmField("deg_mask", "deg_mask", is_count_data=False, correct_data_format=True))
+            cov_cond_map = {}
+            cov_cond_map_r2 = {}
+            for cov_cond in tqdm(cov_cond_unique):
+                if cov_cond in adata.uns[deg_uns_key].keys():
+                    mask_hvg = adata.var_names.isin(adata.uns[deg_uns_key][cov_cond]).astype(np.int)
+                    mask_hvg_r2 = adata.var_names.isin(adata.uns[deg_uns_key][cov_cond][:n_deg_r2]).astype(np.int)
+                    cov_cond_map[cov_cond] = list(mask_hvg)
+                    cov_cond_map_r2[cov_cond] = list(mask_hvg_r2)
+                else:
+                    no_mask = list(np.ones(shape=(adata.n_vars,)))
+                    cov_cond_map[cov_cond] = no_mask
+                    cov_cond_map_r2[cov_cond] = no_mask
+
+            mask = np.vstack(np.vectorize(lambda x: cov_cond_map[x], otypes=[np.ndarray])(
+                adata.obs[deg_uns_cat_key].astype(str).values))
+            mask_r2 = np.vstack(np.vectorize(lambda x: cov_cond_map[x], otypes=[np.ndarray])(
+                adata.obs[deg_uns_cat_key].astype(str).values))
+
+            CPA_REGISTRY_KEYS.DEG_MASK = 'deg_mask'
+            CPA_REGISTRY_KEYS.DEG_MASK_R2 = 'deg_mask_r2'
+            adata.obsm[CPA_REGISTRY_KEYS.DEG_MASK] = np.array(mask)
+            adata.obsm[CPA_REGISTRY_KEYS.DEG_MASK_R2] = np.array(mask_r2)
+
+            anndata_fields.append(ObsmField(CPA_REGISTRY_KEYS.DEG_MASK, CPA_REGISTRY_KEYS.DEG_MASK,
+                                            is_count_data=True, correct_data_format=True))
+            anndata_fields.append(ObsmField(CPA_REGISTRY_KEYS.DEG_MASK_R2, CPA_REGISTRY_KEYS.DEG_MASK_R2,
+                                            is_count_data=True, correct_data_format=True))
 
         adata_manager = AnnDataManager(
             fields=anndata_fields, setup_method_args=setup_method_args
         )
         adata_manager.register_fields(adata, **kwargs)
         cls.register_manager(adata_manager)
 
-        cat_covar_encoders = {}
+        covars_encoder = {}
         for covar in categorical_covariate_keys:
-            cat_covar_encoders[covar] = {c: i for i, c in enumerate(
+            covars_encoder[covar] = {c: i for i, c in enumerate(
                 adata_manager.registry['field_registries'][covar]['state_registry']['categorical_mapping'])}
 
-        CPA.cat_covars_encoders = cat_covar_encoders
-        CPA.drug_encoder = drug_encoder
-        CPA.cont_covars = continuous_covariate_keys
+        if cls.covars_encoder is None:
+            cls.covars_encoder = covars_encoder
+
+        if cls.pert_encoder is None:
+            cls.pert_encoder = pert_encoder
 
     def train(
             self,
             max_epochs: Optional[int] = None,
             use_gpu: Optional[Union[str, int, bool]] = None,
             train_size: float = 0.9,
             validation_size: Optional[float] = None,
             batch_size: int = 128,
             early_stopping: bool = False,
             plan_kwargs: Optional[dict] = None,
-            hyperopt: bool = False,
             save_path: Optional[str] = None,
             **trainer_kwargs,
     ):
         """
         Trains CPA on the given dataset
 
         Parameters
@@ -287,18 +334,30 @@
                 self.adata_manager,
                 train_size=train_size,
                 validation_size=validation_size,
                 batch_size=batch_size,
                 use_gpu=use_gpu,
             )
 
-        self.training_plan = CPATrainingPlan(self.module, self.cat_covars_encoders, **plan_kwargs)
+        perturbation_key = CPA_REGISTRY_KEYS.PERTURBATION_KEY
+        pert_adv_encoder = {c: i for i, c in enumerate(
+            self.adata_manager.registry['field_registries'][perturbation_key]['state_registry'][
+                'categorical_mapping'])}
+
+        drug_weights = []
+        n_adv_perts = len(self.adata.obs[perturbation_key].unique())
+        for condition in tqdm(list(pert_adv_encoder.keys())):
+            n_positive = len(self.adata[self.adata.obs[perturbation_key] == condition])
+            drug_weights.append((self.adata.n_obs / n_positive) - 1.0)
+
+        self.training_plan = CPATrainingPlan(self.module, self.covars_encoder,
+                                             n_adv_perts=n_adv_perts, **plan_kwargs,
+                                             drug_weights=drug_weights)
         trainer_kwargs["early_stopping"] = False
-        trainer_kwargs.update({'weights_summary': 'top'})
-        trainer_kwargs['check_val_every_n_epoch'] = trainer_kwargs.get('check_val_every_n_epoch', 20)
+        trainer_kwargs['check_val_every_n_epoch'] = trainer_kwargs.get('check_val_every_n_epoch', 10)
 
         es_callback = EarlyStopping(monitor='cpa_metric',
                                     patience=trainer_kwargs['early_stopping_patience'],
                                     check_on_train_epoch_end=False,
                                     verbose=False,
                                     mode='max',
                                     )
@@ -307,41 +366,40 @@
             trainer_kwargs['callbacks'] += [es_callback]
         else:
             trainer_kwargs['callbacks'] = [es_callback]
 
         if save_path is None:
             save_path = './'
 
-        checkpoint = SaveBestState(monitor='cpa_metric', mode='max', period=20, verbose=False)
+        checkpoint = SaveBestState(monitor='cpa_metric', mode='max', period=1, verbose=False)
         trainer_kwargs['callbacks'].append(checkpoint)
 
-        runner = TrainRunner(
+        self.runner = TrainRunner(
             self,
             training_plan=self.training_plan,
             data_splitter=data_splitter,
             max_epochs=max_epochs,
             use_gpu=use_gpu,
             early_stopping_monitor="cpa_metric",
             early_stopping_mode='max',
-            checkpoint_callback=True,
             **trainer_kwargs,
         )
-        runner()
+        self.runner()
 
         self.epoch_history = pd.DataFrame().from_dict(self.training_plan.epoch_history)
-        if save_path is not None:
+        if save_path is not False:
             self.save(save_path, overwrite=True)
 
     @torch.no_grad()
     def get_latent_representation(
             self,
             adata: Optional[AnnData] = None,
             indices: Optional[Sequence[int]] = None,
             batch_size: Optional[int] = 32,
-    ) -> np.ndarray:
+    ):
         """Returns the basal latent variable
 
         Parameters
         ----------
         adata : Optional[AnnData], optional
             [description], by default None
         indices : Optional[Sequence[int]], optional
@@ -359,18 +417,19 @@
         scdl = self._make_data_loader(
             adata=adata, indices=indices, batch_size=batch_size, shuffle=False
         )
 
         latent_basal = []
         latent = []
         for tensors in scdl:
+            tensors, _ = self.module.mixup_data(tensors, alpha=0.0)
             inference_inputs = self.module._get_inference_input(tensors)
             outputs = self.module.inference(**inference_inputs)
-            latent_basal += [outputs["latent_basal"].cpu().numpy()]
-            latent += [outputs['latent'].cpu().numpy()]
+            latent_basal += [outputs["z_basal"].cpu().numpy()]
+            latent += [outputs['z'].cpu().numpy()]
 
         latent_basal_adata = AnnData(X=np.concatenate(latent_basal, axis=0), obs=adata.obs.copy())
         latent_basal_adata.obs_names = adata.obs_names
 
         latent_adata = AnnData(X=np.concatenate(latent, axis=0), obs=adata.obs.copy())
         latent_adata.obs_names = adata.obs_names
 
@@ -378,52 +437,51 @@
 
     @torch.no_grad()
     def predict(
             self,
             adata: Optional[AnnData] = None,
             indices: Optional[Sequence[int]] = None,
             batch_size: Optional[int] = 32,
+            n_samples: int = 20,
+            return_mean: bool = True,
     ):
         """Counterfactual-friendly gene expression prediction
         # TODO: See if another signature makes more sense for better usability
 
         To produce counterfactuals,
 
         Returns
         -------
         Tuple
             Gene expression means and standard variations
         """
-        assert self.module.loss_ae in ["gauss", 'mse']
+        assert self.module.recon_loss in ["gauss", 'nb', 'zinb']
         self.module.eval()
 
-        # adata = self.adata if adata is None else adata
         adata = self._validate_anndata(adata)
         if indices is None:
             indices = np.arange(adata.n_obs)
         scdl = self._make_data_loader(
             adata=adata, indices=indices, batch_size=batch_size, shuffle=False
         )
-        mus = []
-        stds = []
-        for tensors in scdl:
-            _mus, _stds = self.module.get_expression(tensors)
-            mus.append(_mus.detach().cpu().numpy())
-            stds.append(_stds.detach().cpu().numpy())
-
-        pred_adata_mean = AnnData(X=np.concatenate(mus, axis=0), obs=adata.obs.copy())
-        pred_adata_var = AnnData(X=np.concatenate(stds, axis=0), obs=adata.obs.copy())
-
-        pred_adata_mean.obs_names = adata.obs_names
-        pred_adata_var.obs_names = adata.obs_names
+        xs = []
+        for tensors in tqdm(scdl):
+            x_pred = self.module.get_expression(tensors, n_samples=n_samples).detach().cpu().numpy()
+            xs.append(x_pred)
+
+        if n_samples > 1 and self.module.variational:
+            # The -2 axis correspond to cells.
+            x_pred = np.concatenate(xs, axis=1)
+        else:
+            x_pred = np.concatenate(xs, axis=0)
 
-        pred_adata_mean.var_names = adata.var_names
-        pred_adata_var.var_names = adata.var_names
+        if self.module.variational and n_samples > 1 and return_mean:
+            x_pred = x_pred.mean(0)
 
-        return pred_adata_mean, pred_adata_var
+        adata.obsm[f'{self.__class__.__name__}_pred'] = x_pred
 
     @torch.no_grad()
     def get_drug_embeddings(self, doses=1.0, drug: Optional[str] = None):
         """Computes all drug drug
 
         Parameters
         ----------
@@ -434,22 +492,22 @@
 
         """
         self.module.eval()
         if isinstance(doses, float):
             if drug is None:
                 treatments = doses * torch.eye(self.n_drugs, device=self.device)
             else:
-                treatments = doses * F.one_hot(torch.LongTensor([self.drug_encoder[drug]]).to(self.device),
+                treatments = doses * F.one_hot(torch.LongTensor([self.pert_encoder[drug]]).to(self.device),
                                                self.n_drugs)
         elif isinstance(doses, np.ndarray):
             treatments = torch.tensor(doses).to(self.device).float()
         else:
             treatments = doses
 
-        embeds = self.module.drug_network(treatments).detach().cpu().numpy()
+        embeds = self.module.pert_network(treatments).detach().cpu().numpy()
 
         return embeds
 
     @torch.no_grad()
     def get_covar_embeddings(self, covariate: str, covariate_value: str = None):
         """Computes Covariate drug
 
@@ -458,29 +516,29 @@
         covariate : str
             covariate to be computed
         covariate_value: str, Optional
             Covariate specific value for embedding computation
 
         """
         if covariate_value is None:
-            covar_ids = torch.arange(len(self.cat_covars_encoders[covariate]), device=self.device)
+            covar_ids = torch.arange(len(self.covars_encoder[covariate]), device=self.device)
         else:
-            covar_ids = torch.LongTensor([self.cat_covars_encoders[covariate][covariate_value]]).to(self.device)
-        embeddings = self.module.cat_covars_embeddings[covariate](covar_ids).detach().cpu().numpy()
+            covar_ids = torch.LongTensor([self.covars_encoder[covariate][covariate_value]]).to(self.device)
+        embeddings = self.module.covars_embeddings[covariate](covar_ids).detach().cpu().numpy()
 
         return embeddings
 
     def save(self, dir_path: str, overwrite: bool = False, save_anndata: bool = False, **anndata_write_kwargs):
         os.makedirs(dir_path, exist_ok=True)
 
         # save public dictionaries
         total_dict = {
-            'drug_encoder': self.drug_encoder,
-            'cat_covars_encoder': self.cat_covars_encoders,
-            'cont_covars': self.cont_covars,
+            'pert_encoder': self.pert_encoder,
+            # 'pert_adv_encoder': self.pert_adv_encoder,
+            'covars_encoder': self.covars_encoder,
         }
 
         json_dict = json.dumps(total_dict)
         with open(os.path.join(dir_path, 'CPA_dicts.json'), 'w') as f:
             f.write(json_dict)
 
         if isinstance(self.epoch_history, dict):
@@ -497,39 +555,19 @@
              deg_uns_key: Optional[str] = None, ):
         assert (adata and perturbation_keys) or (adata is None)
 
         # load public dictionaries
         with open(os.path.join(dir_path, 'CPA_dicts.json')) as f:
             total_dict = json.load(f)
 
-            cls.drug_encoder = total_dict['drug_encoder']
-            cls.cat_covars_encoder = total_dict['cat_covars_encoder']
-            cls.cont_covars = total_dict['cont_covars']
+            cls.pert_encoder = total_dict['pert_encoder']
+            # cls.pert_adv_encoder = total_dict['pert_adv_encoder']
+            cls.covars_encoder = total_dict['covars_encoder']
 
         model = super().load(dir_path, adata, use_gpu)
 
-        drug_key = perturbation_keys['perturbation']
-        dosage_key = perturbation_keys['dosage']
-
-        if adata is not None and 'drugs_doses' not in adata.obsm:
-            drugs_obsm = np.zeros((adata.n_obs, len(CPA.drug_encoder)))
-            drugs, dosages = adata.obs[drug_key], adata.obs[dosage_key].astype(str)
-            for i in tqdm(range(adata.n_obs)):
-                cell_drugs = np.isin(list(CPA.drug_encoder.keys()), drugs[i].split('+'))
-                cell_doses = np.array(dosages[i].split("+")).astype(np.float32)
-                drugs_obsm[i, cell_drugs] = cell_doses
-
-            adata.obsm['drugs_doses'] = drugs_obsm
-
-            if deg_uns_key:
-                mask = np.zeros((adata.n_obs, adata.n_vars))
-                for i, cov_drug in tqdm(enumerate(adata.obs['cov_drug'].values)):
-                    mask[i] = adata.var.index.isin(adata.uns[deg_uns_key][cov_drug]).astype(np.int)
-
-                adata.obsm['deg_mask'] = np.array(mask)
-
         try:
             model.epoch_history = pd.read_csv(os.path.join(dir_path, 'history.csv'))
         except:
             print('WARNING: The history was not found.')
 
         return model
```

### Comparing `cpa-tools-0.3.4/cpa/_plotting.py` & `cpa-tools-0.5/cpa/_plotting.py`

 * *Files identical despite different names*

### Comparing `cpa-tools-0.3.4/cpa/_utils.py` & `cpa-tools-0.5/cpa/_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,32 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from scvi.distributions import NegativeBinomial
 
 from scvi.nn import FCLayers
 from torch.distributions import Normal
+from typing import Optional
 
 
 class _REGISTRY_KEYS:
     X_KEY: str = "X"
-    PERTURBATIONS: str = "drugs_doses"
-    INDICES_KEY: str = "ind_x"
+    X_CTRL_KEY: str = None
+    BATCH_KEY: str = "cpa_batch"
+    CATEGORY_KEY: str = "cpa_category"
+    PERTURBATION_KEY: str = None
+    PERTURBATIONS: str = "perts"
+    PERTURBATIONS_DOSAGES: str = "perts_doses"
     SIZE_FACTOR_KEY: str = "size_factor"
-    PERTURBATION_KEYS: Dict[str, str] = None
     CAT_COV_KEYS: List[str] = []
-    CONT_COV_KEYS: List[str] = []
+    MAX_COMB_LENGTH: int = 2
+    CONTROL_KEY: str = None
+    DEG_MASK: str = None
+    DEG_MASK_R2: str = None
+    PADDING_IDX: int = 0
 
 
 CPA_REGISTRY_KEYS = _REGISTRY_KEYS()
 
 
 class VanillaEncoder(nn.Module):
     def __init__(
@@ -54,91 +62,14 @@
         self.z = nn.Linear(n_hidden, n_output)
 
     def forward(self, inputs, *cat_list):
         z = self.z(self.network(inputs, *cat_list))
         return z
 
 
-class DecoderNormal(nn.Module):
-    def __init__(
-            self,
-            n_input,
-            n_output,
-            n_hidden,
-            n_layers,
-            n_cat_list,
-            use_layer_norm=True,
-            use_batch_norm=False,
-            output_activation: str = 'linear',
-            dropout_rate: float = 0.1,
-    ):
-        super().__init__()
-        self.n_output = n_output
-        self.output_activation = output_activation
-
-        self.network = FCLayers(
-            n_in=n_input,
-            n_out=n_hidden,
-            n_cat_list=n_cat_list,
-            n_layers=n_layers,
-            n_hidden=n_hidden,
-            use_layer_norm=use_layer_norm,
-            use_batch_norm=use_batch_norm,
-            dropout_rate=dropout_rate,
-            activation_fn=nn.ReLU,
-        )
-        self.mean = nn.Linear(n_hidden, n_output)
-        self.var = nn.Linear(n_hidden, n_output, bias=False)
-
-    def forward(self, inputs, *cat_list):
-        x = self.network(inputs, *cat_list)
-        locs = self.mean(x)
-        var_ = self.var(x)
-        if self.output_activation == 'relu':
-            locs = F.relu(locs)
-        elif self.output_activation == 'leaky_relu':
-            locs = F.leaky_relu(locs)
-
-        variances = var_.exp().add(1).log().add(1e-3)
-        return Normal(loc=locs, scale=variances.sqrt())
-
-
-class DecoderNB(nn.Module):
-    def __init__(
-            self,
-            n_input,
-            n_output,
-            n_hidden,
-            n_layers,
-            use_layer_norm=True,
-            use_batch_norm=False,
-            output_activation: str = 'linear',
-            dropout_rate: float = 0.0,
-    ):
-        super().__init__()
-        self.hidden = nn.Sequential(
-            FCLayers(
-                n_in=n_input,
-                n_out=n_output,
-                n_layers=n_layers,
-                n_hidden=n_hidden,
-                use_layer_norm=use_layer_norm,
-                use_batch_norm=use_batch_norm,
-                dropout_rate=dropout_rate,
-                activation_fn=nn.ReLU,
-            ),
-            nn.Softmax(-1),
-        )
-
-    def forward(self, inputs, library, px_r):
-        px_scale = self.hidden(inputs)
-        px_rate = library.exp() * px_scale
-        return NegativeBinomial(mu=px_rate, theta=px_r.exp())
-
-
 class GeneralizedSigmoid(nn.Module):
     """
     Sigmoid, log-sigmoid or linear functions for encoding dose-response for
     drug perurbations.
     """
 
     def __init__(self, n_drugs, non_linearity='sigmoid'):
@@ -158,95 +89,147 @@
         self.bias = torch.nn.Parameter(
             torch.zeros(1, n_drugs),
             requires_grad=True
         )
 
         self.vmap = None
 
-    def forward(self, x, y=None):
+    def forward(self, x, y):
         """
             Parameters
             ----------
-            x: (batch_size, n_drugs) or (batch_size, )
-                Doses matrix
-            y: (batch_size, )
+            x: (batch_size, max_comb_len)
+            y: (batch_size, max_comb_len)
         """
+        y = y.long()
         if self.non_linearity == 'logsigm':
-            if y is None:
-                c0 = self.bias.sigmoid()
-                return (torch.log1p(x) * self.beta + self.bias).sigmoid() - c0
-            else:
-                bias = self.bias[0][y]
-                beta = self.beta[0][y]
-                c0 = bias.sigmoid()
-                return (torch.log1p(x) * beta + bias).sigmoid() - c0
+            bias = self.bias[0][y]
+            beta = self.beta[0][y]
+            c0 = bias.sigmoid()
+            return (torch.log1p(x) * beta + bias).sigmoid() - c0
         elif self.non_linearity == 'sigm':
-            if y is None:
-                c0 = self.bias.sigmoid()
-                return (x * self.beta + self.bias).sigmoid() - c0
-            else:
-                bias = self.bias[0][y]
-                beta = self.beta[0][y]
-                c0 = bias.sigmoid()
-                return (x * beta + bias).sigmoid() - c0
+            bias = self.bias[0][y]
+            beta = self.beta[0][y]
+            c0 = bias.sigmoid()
+            return (x * beta + bias).sigmoid() - c0
         else:
             return x
 
     def one_drug(self, x, i):
         if self.non_linearity == 'logsigm':
             c0 = self.bias[0][i].sigmoid()
             return (torch.log1p(x) * self.beta[0][i] + self.bias[0][i]).sigmoid() - c0
         elif self.non_linearity == 'sigm':
             c0 = self.bias[0][i].sigmoid()
             return (x * self.beta[0][i] + self.bias[0][i]).sigmoid() - c0
         else:
             return x
 
 
-class DrugNetwork(nn.Module):
-    def __init__(self, n_drugs,
+class PerturbationNetwork(nn.Module):
+    def __init__(self,
+                 n_perts,
                  n_latent,
                  doser_type='logsigm',
                  n_hidden=None,
                  n_layers=None,
-                 dropout_rate: float = 0.1):
+                 dropout_rate: float = 0.0):
         super().__init__()
         self.n_latent = n_latent
-        self.drug_embedding = nn.Embedding(n_drugs, n_latent)
+        self.pert_embedding = nn.Embedding(n_perts + 1, n_latent, padding_idx=CPA_REGISTRY_KEYS.PADDING_IDX)
         self.doser_type = doser_type
         if self.doser_type == 'mlp':
             self.dosers = nn.ModuleList()
-            for _ in range(n_drugs):
+            for _ in range(n_perts):
                 self.dosers.append(
                     FCLayers(
                         n_in=1,
                         n_out=1,
                         n_hidden=n_hidden,
                         n_layers=n_layers,
                         use_batch_norm=False,
-                        use_layer_norm=False,
+                        use_layer_norm=True,
                         dropout_rate=dropout_rate
                     )
                 )
         else:
-            self.dosers = GeneralizedSigmoid(n_drugs, non_linearity=self.doser_type)
+            self.dosers = GeneralizedSigmoid(n_perts, non_linearity=self.doser_type)
 
-    def forward(self, drugs, doses=None):
+    def forward(self, perts, dosages):
         """
-            drugs: (batch_size, n_drugs) if combinatorial else (batch_size, )
-                OneHot multiplied by doses if combinatorial is True
+            perts: (batch_size, max_comb_len)
+            dosages: (batch_size, max_comb_len)
         """
-        if self.doser_type == 'mlp':
-            doses = []
-            for d in range(drugs.size(1)):
-                this_drug = drugs[:, d].view(-1, 1)
-                doses.append(self.dosers[d](this_drug).sigmoid() * this_drug.gt(0))
-            return torch.cat(doses, 1) @ self.drug_embedding.weight
-        else:
-            if doses is not None:
-                drugs = drugs.long().view(-1, )
-                doses = doses.float().view(-1, )
-                scaled_dosages = self.dosers(doses, drugs)
-                drug_embeddings = self.drug_embedding(drugs)
-                return torch.einsum('b,be->be', [scaled_dosages, drug_embeddings])
-            else:
-                return self.dosers(drugs) @ self.drug_embedding.weight
+        perts = perts.long()
+        scaled_dosages = self.dosers(dosages, perts)  # (batch_size, max_comb_len)
+        drug_embeddings = self.pert_embedding(perts)  # (batch_size, max_comb_len, n_latent)
+
+        z_drugs = torch.einsum('bm,bme->bme', [scaled_dosages, drug_embeddings])  # (batch_size, n_latent)
+
+        z_drugs = torch.einsum('bmn,bm->bmn', z_drugs, (perts > 0).int()).sum(dim=1)  # mask single perts
+
+        return z_drugs
+
+class FocalLoss(nn.Module):
+    """ Inspired by https://github.com/AdeelH/pytorch-multi-class-focal-loss/blob/master/focal_loss.py
+
+    Focal Loss, as described in https://arxiv.org/abs/1708.02002.
+    It is essentially an enhancement to cross entropy loss and is
+    useful for classification tasks when there is a large class imbalance.
+    x is expected to contain raw, unnormalized scores for each class.
+    y is expected to contain class labels.
+    Shape:
+        - x: (batch_size, C) or (batch_size, C, d1, d2, ..., dK), K > 0.
+        - y: (batch_size,) or (batch_size, d1, d2, ..., dK), K > 0.
+    """
+
+    def __init__(self,
+                 alpha: Optional[torch.Tensor] = None,
+                 gamma: float = 2.,
+                 reduction: str = 'mean',
+                 ):
+        """
+        Args:
+            alpha (Tensor, optional): Weights for each class. Defaults to None.
+            gamma (float, optional): A constant, as described in the paper.
+                Defaults to 0.
+            reduction (str, optional): 'mean', 'sum' or 'none'.
+                Defaults to 'mean'.
+        """
+        if reduction not in ('mean', 'sum', 'none'):
+            raise ValueError(
+                'Reduction must be one of: "mean", "sum", "none".')
+
+        super().__init__()
+        self.alpha = alpha
+        self.gamma = gamma
+        self.reduction = reduction
+
+        self.nll_loss = nn.NLLLoss(
+            weight=alpha, reduction='none')
+
+    def forward(self, y_pred: torch.Tensor, y_true: torch.Tensor) -> torch.Tensor:
+        if len(y_true) == 0:
+            return torch.tensor(0.)
+
+        # compute weighted cross entropy term: -alpha * log(pt)
+        # (alpha is already part of self.nll_loss)
+        log_p = F.log_softmax(y_pred, dim=-1)
+        ce = self.nll_loss(log_p, y_true)
+
+        # get true class column from each row
+        all_rows = torch.arange(len(y_pred))
+        log_pt = log_p[all_rows, y_true]
+
+        # compute focal term: (1 - pt)^gamma
+        pt = log_pt.exp()
+        focal_term = (1 - pt) ** self.gamma
+
+        # the full loss: -alpha * ((1 - pt)^gamma) * log(pt)
+        loss = focal_term * ce
+
+        if self.reduction == 'mean':
+            loss = loss.mean()
+        elif self.reduction == 'sum':
+            loss = loss.sum()
+
+        return loss
```

### Comparing `cpa-tools-0.3.4/pyproject.toml` & `cpa-tools-0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 homepage = "https://github.com/theislab/cpa/"
 license = "BSD-3-Clause"
 name = "cpa-tools"
 packages = [
     { include = "cpa" },
 ]
 readme = "README.md"
-version = "0.3.4"
+version = "0.5"
 
 [tool.poetry.dependencies]
 adjustText = { version = "*", optional = true }
 anndata = ">=0.7.5"
 black = { version = ">=20.8b1", optional = true }
 codecov = { version = ">=2.0.8", optional = true }
 flake8 = { version = ">=3.7.7", optional = true }
```

### Comparing `cpa-tools-0.3.4/setup.py` & `cpa-tools-0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,17 +42,17 @@
  'tutorials': ['leidenalg',
                'loompy>=3.0.6',
                'python-igraph',
                'scikit-misc>=0.1.3']}
 
 setup_kwargs = {
     'name': 'cpa-tools',
-    'version': '0.3.4',
+    'version': '0.5',
     'description': 'Compositional Perturbation Autoencoder (CPA)',
-    'long_description': '# CPA - Compositional Perturbation Autoencoder\n\n\n## What is CPA?\n\n![Alt text](https://user-images.githubusercontent.com/33202701/156530222-c61e5982-d063-461c-b66e-c4591d2d0de4.png?raw=true "Title")\n\n`CPA` is a framework to learn effects of perturbations at the single-cell level. CPA encodes and learns phenotypic drug response across different cell types, doses and drug combinations. CPA allows:\n\n* Out-of-distribution predictions of unseen drug combinations at various doses and among different cell types.\n* Learn interpretable drug and cell type latent spaces.\n* Estimate dose response curve for each perturbation and their combinations.\n* Access the uncertainty of the estimations of the model.\n\n\nUsage and installation\n-------------------------------\nSee [here](https://cpa-tools.readthedocs.io/en/latest/index.html) for documentation and tutorials.\n\nSupport and contribute\n-------------------------------\nIf you have a question or new architecture or a model that could be integrated into our pipeline, you can\npost an [issue](https://github.com/theislab/cpa/issues/new)\n\n\n###### Acknowledgment\nThis code is inspired by an early implementatiom by [Pierre Boyeau](https://github.com/PierreBoyeau) using [scvi-tools](https://scvi-tools.org/).\n\n',
+    'long_description': '# CPA - Compositional Perturbation Autoencoder\n\n\n## What is CPA?\n\n![Alt text](https://user-images.githubusercontent.com/33202701/156530222-c61e5982-d063-461c-b66e-c4591d2d0de4.png?raw=true "Title")\n\n`CPA` is a framework to learn effects of perturbations at the single-cell level. CPA encodes and learns phenotypic drug response across different cell types, doses and drug combinations. CPA allows:\n\n* Out-of-distribution predictions of unseen drug combinations at various doses and among different cell types.\n* Learn interpretable drug and cell type latent spaces.\n* Estimate dose response curve for each perturbation and their combinations.\n* Access the uncertainty of the estimations of the model.\n\n\nUsage and installation\n-------------------------------\nSee [here](https://cpa-tools.readthedocs.io/en/latest/index.html) for documentation and tutorials.\n\nSupport and contribute\n-------------------------------\nIf you have a question or new architecture or a model that could be integrated into our pipeline, you can\npost an [issue](https://github.com/theislab/cpa/issues/new)\n',
     'author': 'Mohsen Naghipourfar',
     'author_email': 'naghipourfar@berkeley.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/theislab/cpa/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cpa-tools-0.3.4/PKG-INFO` & `cpa-tools-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpa-tools
-Version: 0.3.4
+Version: 0.5
 Summary: Compositional Perturbation Autoencoder (CPA)
 Home-page: https://github.com/theislab/cpa/
 License: BSD-3-Clause
 Author: Mohsen Naghipourfar
 Author-email: naghipourfar@berkeley.edu
 Requires-Python: >=3.7.2,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -78,12 +78,7 @@
 See [here](https://cpa-tools.readthedocs.io/en/latest/index.html) for documentation and tutorials.
 
 Support and contribute
 -------------------------------
 If you have a question or new architecture or a model that could be integrated into our pipeline, you can
 post an [issue](https://github.com/theislab/cpa/issues/new)
 
-
-###### Acknowledgment
-This code is inspired by an early implementatiom by [Pierre Boyeau](https://github.com/PierreBoyeau) using [scvi-tools](https://scvi-tools.org/).
-
-
```

