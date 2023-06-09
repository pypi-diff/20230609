# Comparing `tmp/vocex-0.1.4.tar.gz` & `tmp/vocex-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocex-0.1.4.tar", last modified: Wed May 31 10:00:00 2023, max compression
+gzip compressed data, was "vocex-0.1.5.tar", last modified: Fri Jun  9 06:17:40 2023, max compression
```

## Comparing `vocex-0.1.4.tar` & `vocex-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0        8 2023-05-08 02:42:27.826184 vocex-0.1.4/README.md
--rw-r--r--   0        0        0      398 2023-05-31 10:00:00.864400 vocex-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      507 2023-05-29 13:47:25.541785 vocex-0.1.4/vocex/__init__.py
--rw-r--r--   0        0        0     2025 2023-05-07 15:53:39.423391 vocex-0.1.4/vocex/conformer_layer.py
--rw-r--r--   0        0        0     8759 2023-05-31 09:59:22.905727 vocex-0.1.4/vocex/conformer_model.py
--rw-r--r--   0        0        0     4208 2023-05-27 22:17:11.509445 vocex-0.1.4/vocex/scaler.py
--rw-r--r--   0        0        0     3830 2023-05-24 18:47:16.895683 vocex-0.1.4/vocex/softdtw.py
--rw-r--r--   0        0        0     2460 2023-05-07 15:45:50.981971 vocex-0.1.4/vocex/transformer.py
--rw-r--r--   0        0        0     1756 2023-05-09 04:48:57.299991 vocex-0.1.4/vocex/utils.py
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 vocex-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        8 2023-06-08 08:33:20.634384 vocex-0.1.5/README.md
+-rw-r--r--   0        0        0      398 2023-06-09 06:17:40.167695 vocex-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-06-08 17:35:48.983019 vocex-0.1.5/test/__init__.py
+-rw-r--r--   0        0        0     9229 2023-06-09 06:14:29.212202 vocex-0.1.5/test/test.py
+-rw-r--r--   0        0        0     3033 2023-06-08 17:34:50.826301 vocex-0.1.5/test/wada_snr.py
+-rw-r--r--   0        0        0    11843 2023-06-09 06:10:57.279008 vocex-0.1.5/vocex/__init__.py
+-rw-r--r--   0        0        0     3250 2023-06-08 11:03:36.601864 vocex-0.1.5/vocex/conformer_layer.py
+-rw-r--r--   0        0        0    10299 2023-06-08 16:45:34.410508 vocex-0.1.5/vocex/conformer_model.py
+-rw-r--r--   0        0        0     4208 2023-06-08 08:33:21.154426 vocex-0.1.5/vocex/scaler.py
+-rw-r--r--   0        0        0     3830 2023-06-08 08:33:21.154426 vocex-0.1.5/vocex/softdtw.py
+-rw-r--r--   0        0        0     3377 2023-06-08 11:05:02.020794 vocex-0.1.5/vocex/transformer.py
+-rw-r--r--   0        0        0     1756 2023-06-08 08:33:21.154426 vocex-0.1.5/vocex/utils.py
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 vocex-0.1.5/PKG-INFO
```

### Comparing `vocex-0.1.4/vocex/conformer_layer.py` & `vocex-0.1.5/vocex/conformer_layer.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,22 +32,55 @@
             self.conv2 = nn.Conv1d(
                 kwargs["conv_filter_size"],
                 kwargs["conv_in"],
                 kernel_size=kwargs["conv_kernel"][1],
                 padding=(kwargs["conv_kernel"][1] - 1) // 2,
             )
 
-    def forward(self, src, src_mask=None, src_key_padding_mask=None):
+    def forward(self, src, src_mask=None, src_key_padding_mask=None, need_weights=False):
         x = src
         if self.norm_first:
-            x = x + self._sa_block(self.norm1(x), src_mask, src_key_padding_mask)
+            if not need_weights:
+                attn = self._sa_block(self.norm1(x), src_mask, src_key_padding_mask)
+            else:
+                attn, weights = self._sa_block(self.norm1(x), src_mask, src_key_padding_mask, need_weights=need_weights)
+            x = x + attn
             x = x + self._ff_block(self.norm2(x))
         else:
-            x = self.norm1(x + self._sa_block(x, src_mask, src_key_padding_mask))
+            if not need_weights:
+                attn = self._sa_block(x, src_mask, src_key_padding_mask)
+            else:
+                attn, weights = self._sa_block(x, src_mask, src_key_padding_mask, need_weights=need_weights)
+            x = self.norm1(x + attn)
             x = self.norm2(x + self._ff_block(x))
-        return x
+        if need_weights:
+            return x, weights
+        else:
+            return x
 
     def _ff_block(self, x):
         x = self.conv2(
             self.dropout(self.activation(self.conv1(x.transpose(1, 2))))
         ).transpose(1, 2)
-        return self.dropout2(x)
+        return self.dropout2(x)
+
+    def _sa_block(
+            self, 
+            x,
+            attn_mask,
+            key_padding_mask=None,
+            need_weights=False,
+        ):
+        if not need_weights:
+            x = self.self_attn(x, x, x,
+                            attn_mask=attn_mask,
+                            key_padding_mask=key_padding_mask,
+                            need_weights=need_weights)[0]
+        else:
+            x, weights = self.self_attn(x, x, x,
+                            attn_mask=attn_mask,
+                            key_padding_mask=key_padding_mask,
+                            need_weights=need_weights)
+        if need_weights:
+            return self.dropout1(x), weights
+        else:
+            return self.dropout1(x)
```

### Comparing `vocex-0.1.4/vocex/conformer_model.py` & `vocex-0.1.5/vocex/conformer_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -100,14 +100,30 @@
         if self.use_softdtw:
             self.softdtw = SoftDTW(gamma=softdtw_gamma)
 
         self.verbose = False
 
         self.apply(self._init_weights)
 
+        # save hparams
+        self.hparams = {
+            "measures": measures,
+            "in_channels": in_channels,
+            "filter_size": filter_size,
+            "kernel_size": kernel_size,
+            "dropout": dropout,
+            "depthwise": depthwise,
+            "measure_nlayers": measure_nlayers,
+            "dvector_dim": dvector_dim,
+            "dvector_nlayers": dvector_nlayers,
+            "noise_factor": noise_factor,
+            "use_softdtw": use_softdtw,
+            "softdtw_gamma": softdtw_gamma,
+        }
+
     @property
     def scalers(self):
         return self.scaler_dict
 
     def _init_weights(self, module):
         if isinstance(module, nn.Linear):
             module.weight.data.normal_(mean=0.0, std=0.02)
@@ -128,34 +144,48 @@
                     self.scalers[k].partial_fit(batch["measures"][k])
             self.scalers["dvector"].partial_fit(batch["dvector"])
             if i >= n_batches:
                 break
         for k in self.scalers:
             self.scalers[k].is_fit = True
 
-    def forward(self, mel, dvector=None, measures=None, inference=False):
+    def forward(self, mel, dvector=None, measures=None, inference=False, return_activations=False, return_attention=False):
         mel_padding_mask = mel.sum(dim=-1) != 0
         mel_padding_mask = mel_padding_mask.to(torch.float32)
+
+        if return_activations:
+            self.layers.return_additional_layers = list(range(self.hparams["measure_nlayers"]))
+
         if not self.scalers["mel"].is_fit:
             self.scalers["mel"].partial_fit(mel)
         x = self.scalers["mel"].transform(mel)
         x = x + (torch.randn_like(x) * x.std() + x.mean()) * self.noise_factor
         out = self.in_layer(x)
         if self.verbose:
             print(out.mean(), "1")
         out = self.positional_encoding(out)
         if self.verbose:
             print(out.mean(), "2")
-        out_conv = self.layers(out, src_key_padding_mask=mel_padding_mask)
+        res = self.layers(out, src_key_padding_mask=mel_padding_mask, need_weights=return_attention)
+        if return_activations:
+            activations = res["activations"]
+            out_conv = res["output"]
+            self.layers.return_additional_layers = None
+        if return_attention:
+            attention = res["attention"]
+            out_conv = res["output"]
+        if not return_activations and not return_attention:
+            out_conv = res
         if self.verbose:
             print(out_conv.mean(), "3")
         out = self.linear(out_conv)
         if self.verbose:
             print(out.mean(), "4")
         out = out.transpose(1, 2)
+
         measure_results = {}
         measure_true = {}
         loss_dict = {}
         for i, measure in enumerate(self.measures):
             measure_out = out[:, i]
             if not measure.endswith("_binary") and not self.scalers[measure].is_fit:
                 self.scalers[measure].partial_fit(measures[measure])
@@ -211,14 +241,18 @@
             else:
                 loss = dvector_loss
         if not inference:
             results = {
                 "loss": loss,
                 "compound_losses": loss_dict,
             }
+            if return_activations:
+                results["activations"] = [a.detach() for a in activations]
+            if return_attention:
+                results["attention"] = [a.detach() for a in attention]
             return results
         else:
             # transform back to original scale
             for measure in self.measures:
                 if not measure.endswith("_binary"):
                     measure_results[measure] = self.scalers[measure].inverse_transform(
                         measure_results[measure]
@@ -228,8 +262,12 @@
             dvector_pred = self.scalers["dvector"].inverse_transform(dvector_pred)
             results = {
                 "loss": loss,
                 "compound_losses": loss_dict,
                 "measures": measure_results,
                 "dvector": dvector_pred,
             }
+            if return_activations:
+                results["activations"] = [a.detach() for a in activations]
+            if return_attention:
+                results["attention"] = [a.detach() for a in attention]
             return results
```

### Comparing `vocex-0.1.4/vocex/scaler.py` & `vocex-0.1.5/vocex/scaler.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.4/vocex/softdtw.py` & `vocex-0.1.5/vocex/softdtw.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.4/vocex/transformer.py` & `vocex-0.1.5/vocex/transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,40 +26,63 @@
 # from https://pytorch.org/docs/1.13/_modules/torch/nn/modules/transformer.html#TransformerEncoder
 class TransformerEncoder(nn.Module):
     def __init__(
         self,
         encoder_layer,
         num_layers,
         norm=None,
-        return_additional_layer=None,
+        return_additional_layers=None,
     ):
         super(TransformerEncoder, self).__init__()
         self.layers = nn.ModuleList([copy.deepcopy(encoder_layer) for i in range(num_layers)])
         self.num_layers = num_layers
         self.norm = norm
-        self.return_additional_layer = return_additional_layer
+        self.return_additional_layers = return_additional_layers
 
-    def forward(self, src, mask=None, src_key_padding_mask=None, condition=None):
+    def forward(self, src, mask=None, src_key_padding_mask=None, condition=None, need_weights=False):
             if src_key_padding_mask is not None:
                 _skpm_dtype = src_key_padding_mask.dtype
                 if _skpm_dtype != torch.bool and not torch.is_floating_point(src_key_padding_mask):
                     raise AssertionError("only bool and floating types of key_padding_mask are supported")
             
             output = src
             src_key_padding_mask_for_layers = src_key_padding_mask
 
-            output_for_return = None
+            output_for_return = []
+
+            if need_weights:
+                weight_list = []
 
             for i, mod in enumerate(self.layers):
                 if condition is not None:
                     output = output + condition
-                output = mod(output, src_mask=mask, src_key_padding_mask=src_key_padding_mask_for_layers)
-                if self.return_additional_layer is not None and i == self.return_additional_layer:
-                    output_for_return = output
+                if need_weights:
+                    output, weights = mod(output, src_mask=mask, src_key_padding_mask=src_key_padding_mask_for_layers, need_weights=need_weights)
+                    weight_list.append(weights)
+                else:
+                    output = mod(output, src_mask=mask, src_key_padding_mask=src_key_padding_mask_for_layers)
+                if self.return_additional_layers is not None and i in self.return_additional_layers:
+                    output_for_return.append(output)
 
             if self.norm is not None:
                 output = self.norm(output)
 
-            if output_for_return is not None:
-                return output, output_for_return
+            if self.return_additional_layers is not None:
+                if need_weights:
+                    return {
+                        "output": output,
+                        "activations": output_for_return,
+                        "attention": weight_list,
+                    }
+                else:
+                    return {
+                        "output": output,
+                        "activations": output_for_return,
+                    }
             else:
-                return output
+                if need_weights:
+                    return {
+                        "output": output,
+                        "attention": weight_list,
+                    }
+                else:
+                    return output
```

### Comparing `vocex-0.1.4/vocex/utils.py` & `vocex-0.1.5/vocex/utils.py`

 * *Files identical despite different names*

