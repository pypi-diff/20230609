# Comparing `tmp/fad_pytorch-0.0.5.tar.gz` & `tmp/fad_pytorch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fad_pytorch-0.0.5.tar", last modified: Mon Jun  5 19:29:14 2023, max compression
+gzip compressed data, was "fad_pytorch-0.0.6.tar", last modified: Fri Jun  9 17:09:51 2023, max compression
```

## Comparing `fad_pytorch-0.0.5.tar` & `fad_pytorch-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-05 19:29:14.420126 fad_pytorch-0.0.5/
--rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/LICENSE
--rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/MANIFEST.in
--rw-r--r--   0 shawley    (501) staff       (20)     4690 2023-06-05 19:29:14.419998 fad_pytorch-0.0.5/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)     3888 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/README.md
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-05 19:29:14.418918 fad_pytorch-0.0.5/fad_pytorch/
--rw-r--r--   0 shawley    (501) staff       (20)       22 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/fad_pytorch/__init__.py
--rw-r--r--   0 shawley    (501) staff       (20)    31274 2023-06-01 23:44:14.000000 fad_pytorch-0.0.5/fad_pytorch/_modidx.py
--rw-r--r--   0 shawley    (501) staff       (20)      142 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/fad_pytorch/core.py
--rw-r--r--   0 shawley    (501) staff       (20)    18465 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/fad_pytorch/fad_embed.py
--rw-r--r--   0 shawley    (501) staff       (20)     4423 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/fad_gen.py
--rw-r--r--   0 shawley    (501) staff       (20)     3773 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/fad_score.py
--rw-r--r--   0 shawley    (501) staff       (20)   123697 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/pann.py
--rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.5/fad_pytorch/pann_pytorch_utils.py
--rw-r--r--   0 shawley    (501) staff       (20)     8474 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/sqrtm.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-05 19:29:14.419853 fad_pytorch-0.0.5/fad_pytorch.egg-info/
--rw-r--r--   0 shawley    (501) staff       (20)     4690 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      512 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 shawley    (501) staff       (20)      176 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/not-zip-safe
--rw-r--r--   0 shawley    (501) staff       (20)       93 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/requires.txt
--rw-r--r--   0 shawley    (501) staff       (20)       12 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/top_level.txt
--rw-r--r--   0 shawley    (501) staff       (20)     1274 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/settings.ini
--rw-r--r--   0 shawley    (501) staff       (20)       38 2023-06-05 19:29:14.420159 fad_pytorch-0.0.5/setup.cfg
--rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/setup.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-09 17:09:51.193726 fad_pytorch-0.0.6/
+-rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.6/LICENSE
+-rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.6/MANIFEST.in
+-rw-r--r--   0 shawley    (501) staff       (20)     5606 2023-06-09 17:09:51.193586 fad_pytorch-0.0.6/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)     4804 2023-06-09 17:09:36.000000 fad_pytorch-0.0.6/README.md
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-09 17:09:51.192445 fad_pytorch-0.0.6/fad_pytorch/
+-rw-r--r--   0 shawley    (501) staff       (20)       22 2023-06-09 17:09:36.000000 fad_pytorch-0.0.6/fad_pytorch/__init__.py
+-rw-r--r--   0 shawley    (501) staff       (20)    31174 2023-06-06 19:52:11.000000 fad_pytorch-0.0.6/fad_pytorch/_modidx.py
+-rw-r--r--   0 shawley    (501) staff       (20)    18465 2023-06-06 19:52:10.000000 fad_pytorch-0.0.6/fad_pytorch/fad_embed.py
+-rw-r--r--   0 shawley    (501) staff       (20)     5083 2023-06-09 17:09:36.000000 fad_pytorch-0.0.6/fad_pytorch/fad_gen.py
+-rw-r--r--   0 shawley    (501) staff       (20)     3773 2023-06-06 19:52:10.000000 fad_pytorch-0.0.6/fad_pytorch/fad_score.py
+-rw-r--r--   0 shawley    (501) staff       (20)   123697 2023-05-31 21:21:07.000000 fad_pytorch-0.0.6/fad_pytorch/pann.py
+-rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.6/fad_pytorch/pann_pytorch_utils.py
+-rw-r--r--   0 shawley    (501) staff       (20)     8474 2023-06-06 19:52:10.000000 fad_pytorch-0.0.6/fad_pytorch/sqrtm.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-09 17:09:51.193430 fad_pytorch-0.0.6/fad_pytorch.egg-info/
+-rw-r--r--   0 shawley    (501) staff       (20)     5606 2023-06-09 17:09:51.000000 fad_pytorch-0.0.6/fad_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      492 2023-06-09 17:09:51.000000 fad_pytorch-0.0.6/fad_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-06-09 17:09:51.000000 fad_pytorch-0.0.6/fad_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 shawley    (501) staff       (20)      176 2023-06-09 17:09:51.000000 fad_pytorch-0.0.6/fad_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.6/fad_pytorch.egg-info/not-zip-safe
+-rw-r--r--   0 shawley    (501) staff       (20)       93 2023-06-09 17:09:51.000000 fad_pytorch-0.0.6/fad_pytorch.egg-info/requires.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       12 2023-06-09 17:09:51.000000 fad_pytorch-0.0.6/fad_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 shawley    (501) staff       (20)     1274 2023-06-09 17:09:36.000000 fad_pytorch-0.0.6/settings.ini
+-rw-r--r--   0 shawley    (501) staff       (20)       38 2023-06-09 17:09:51.193762 fad_pytorch-0.0.6/setup.cfg
+-rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.6/setup.py
```

### Comparing `fad_pytorch-0.0.5/LICENSE` & `fad_pytorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.5/PKG-INFO` & `fad_pytorch-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,57 @@
-Metadata-Version: 2.1
-Name: fad_pytorch
-Version: 0.0.5
-Summary: Frechet Audio Distance evaluation in PyTorch
-Home-page: https://github.com/drscotthawley/fad_pytorch
-Author: Scott H. Hawley
-Author-email: scott.hawley@belmont.edu
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 fad_pytorch
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 [Original FAD paper (PDF)](https://arxiv.org/pdf/1812.08466.pdf)
 
 ## Install
 
 ``` sh
 pip install fad_pytorch
 ```
 
-## About
-
-Features:
+## Features:
 
 - runs in parallel on multiple processors and multiple GPUs (via
   `accelerate`)
 - supports multiple embedding methods:
   - VGGish and PANN, both mono @ 16kHz
   - OpenL3 and (LAION-)CLAP, stereo @ 48kHz
+- uses publicly-available pretrained checkpoints for music (+other
+  sources) for those models. (if you want Speech, submit a PR or an
+  Issue; I don’t do speech.)
 - favors ops in PyTorch rather than numpy (or tensorflow)
-- `fad_gen` supports WebDataset (audio data stored in S3 buckets)
+- `fad_gen` supports local data read or WebDataset (audio data stored in
+  S3 buckets)
 - runs on CPU, CUDA, or MPS
 
+## Instructions:
+
 This is designed to be run as 3 command-line scripts in succession. The
 latter 2 (`fad_embed` and `fad_score`) are probably what most people
 will want:
 
-1.  `fad_gen`: produces directories of real & fake audio. See
-    `fad_gen docs` for calling sequence.
+1.  `fad_gen`: produces directories of real & fake audio (given real
+    data). See `fad_gen`
+    [documentation](https://drscotthawley.github.io/fad_pytorch/fad_gen.html)
+    for calling sequence.
 2.  `fad_embed [options] <real_audio_dir> <fake_audio_dir>`: produces
     directories of *embeddings* of real & fake audio
-3.  `fad_score [optoions] <real_emb_dir> <fake_emb_dir>`: reads the
+3.  `fad_score [options] <real_emb_dir> <fake_emb_dir>`: reads the
     embeddings & generates FAD score, for real (“$r$”) and fake (“$f$”):
 
 $$ FAD = || \mu_r - \mu_f ||^2 + tr\left(\Sigma_r + \Sigma_f - 2 \sqrt{\Sigma_r \Sigma_f}\right)$$
 
+## Documentation
+
+See the [Documentation
+Website](https://drscotthawley.github.io/fad_pytorch/).
+
 ## Comments / FAQ / Troubleshooting
 
 - “`RuntimeError: CUDA error: invalid device ordinal`”: This happens
   when you have a “bad node” on an AWS cluster. [Haven’t yet figured out
   what causes it or how to fix
   it](https://discuss.huggingface.co/t/solved-accelerate-accelerator-cuda-error-invalid-device-ordinal/21509/1).
   Workaround: Just add the current node to your SLURM `--exclude` list,
@@ -77,36 +66,49 @@
   …Yea. There seems to be an uncertainty of around +/- 0.008. I’d say,
   don’t quote any numbers past the first decimal point.
 
 ## Contributing
 
 This repo is still fairly “bare bones” and will benefit from more
 documentation and features as time goes on. Note that it is written
-using [nbdev](https://nbdev.fast.ai/), so the things to are:
+using [nbdev](https://nbdev.fast.ai/), so the things to do are:
 
-1.  fork this repo
-2.  clone your fork to your (local) machine
+1.  Fork this repo
+2.  Clone your fork to your (local) machine
 3.  Install nbdev: `python3 -m pip install -U nbdev`
 4.  Make changes by editing the notebooks in `nbs/`, not the `.py` files
     in `fad_pytorch/`.
 5.  Run `nbdev_export` to export notebook changes to `.py` files
 6.  For good measure, run `nbdev_install_hooks` and `nbdev_clean` -
     especially if you’ve *added* any notebooks.
 7.  Do a `git status` to see all the `.ipynb` and `.py` files that need
     to be added & committed
 8.  `git add` those files and then `git commit`, and then `git push`
-9.  Take a look in your GitHub Actions tab, and see if the “test” and
-    “deploy” CI runs finish properly (green light) or fail (red light)
-10. One you get green lights, send in a Pull Request!
+9.  Take a look in your fork’s GitHub Actions tab, and see if the “test”
+    and “deploy” CI runs finish properly (green light) or fail (red
+    light)
+10. Once you get green lights, send in a Pull Request!
 
 *Feel free to ask me for tips with nbdev, it has quite a learning curve.
 You can also ask on [fast.ai forums](https://forums.fast.ai/) and/or
 [fast.ai
 Discord](https://discord.com/channels/689892369998676007/887694559952400424)*
 
+## Citations / Blame / Disclaimer
+
+This repo is 2 weeks old. I’m not ready for this to be cited in your
+papers. I’d hate for there to be some mistake I haven’t found yet.
+Perhaps a later version will have citation info. For now, instead,
+there’s:
+
+**Disclaimer:** Results from this repo are still a work in progress.
+While every effort has been made to test model outputs, the author takes
+no responsbility for mistakes. If you want to double-check via another
+source, see “Related Repos” below.
+
 ## Related Repos
 
 There are \[several\] others, but this one is mine. These repos didn’t
 have all the features I wanted, but I used them for inspiration:
 
 - https://github.com/gudgud96/frechet-audio-distance
 - https://github.com/google-research/google-research/tree/master/frechet_audio_distance:
```

### Comparing `fad_pytorch-0.0.5/fad_pytorch/_modidx.py` & `fad_pytorch-0.0.6/fad_pytorch/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/fad_pytorch',
                 'doc_host': 'https://drscotthawley.github.io',
                 'git_url': 'https://github.com/drscotthawley/fad_pytorch',
                 'lib_path': 'fad_pytorch'},
-  'syms': { 'fad_pytorch.core': {'fad_pytorch.core.foo': ('core.html#foo', 'fad_pytorch/core.py')},
-            'fad_pytorch.fad_embed': { 'fad_pytorch.fad_embed.download_file': ('fad_embed.html#download_file', 'fad_pytorch/fad_embed.py'),
+  'syms': { 'fad_pytorch.fad_embed': { 'fad_pytorch.fad_embed.download_file': ('fad_embed.html#download_file', 'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.download_if_needed': ( 'fad_embed.html#download_if_needed',
                                                                                      'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.embed': ('fad_embed.html#embed', 'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.get_ckpt': ('fad_embed.html#get_ckpt', 'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.main': ('fad_embed.html#main', 'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.setup_embedder': ( 'fad_embed.html#setup_embedder',
                                                                                  'fad_pytorch/fad_embed.py')},
```

### Comparing `fad_pytorch-0.0.5/fad_pytorch/fad_embed.py` & `fad_pytorch-0.0.6/fad_pytorch/fad_embed.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.5/fad_pytorch/fad_gen.py` & `fad_pytorch-0.0.6/fad_pytorch/fad_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import argparse
 from accelerate import Accelerator
 import warnings
 import torch
 
 from aeiou.core import get_device, load_audio, get_audio_filenames, makedir
-from aeiou.datasets import get_wds_loader
+from aeiou.datasets import get_wds_loader, AudioDataset
 from aeiou.hpc import HostPrinter
 from pathlib import Path
 #from audio_algebra.given_models import StackedDiffAEWrapper
 import ast
 import torchaudio
 from tqdm.auto import tqdm
 import math
@@ -32,31 +32,39 @@
     device = accelerator.device  # get_device()
     hprint(f"gen: args = {args}")
     hprint(f'{ddps} Using device: {device}')
     
     
     model_ckpt, data_sources, profiles, n = args.model_ckpt, args.data_sources, args.profiles,  args.n
     names = data_sources.split(' ')
-    hprint(f"names = {names}")
-    profiles = ast.literal_eval(profiles)
-    hprint(f"profiles = {profiles}")
-    
-    dl = get_wds_loader(
-        batch_size=args.batch_size,
-        s3_url_prefix=None,
-        sample_size=args.sample_size,
-        names=names,
-        sample_rate=args.sample_rate,
-        num_workers=args.num_workers,
-        recursive=True,
-        random_crop=True,
-        epoch_steps=10000,
-        profiles=profiles,
-    )
-    
+    #hprint(f"names = {names}")
+    local_data = False
+    if 's3://' in data_sources: 
+        hprint("Data sources are on S3")
+        profiles = ast.literal_eval(profiles)
+        hprint(f"profiles = {profiles}")
+
+        dl = get_wds_loader(
+            batch_size=args.batch_size,
+            s3_url_prefix=None,
+            sample_size=args.sample_size,
+            names=names,
+            sample_rate=args.sample_rate,
+            num_workers=args.num_workers,
+            recursive=True,
+            random_crop=True,
+            epoch_steps=10000,
+            profiles=profiles,
+        )
+    else:
+        hprint("Data sources are local")
+        dataset = AudioDataset(names, sample_rate=args.sample_rate, sample_size=args.sample_size)
+        dl = torch.utils.data.DataLoader(dataset, batch_size=args.batch_size, num_workers=args.num_workers)
+        local_data = True
+        
     print(f"loading {model_ckpt}....")
     if model_ckpt.endswith('.ts'):
         model = torch.jit.load(model_ckpt)
     #else:  # default is stacked diffae
     #    model = StackedDiffAEWrapper(ckpt_info={'ckpt_path':model_ckpt})
     try:
         model.setup()  # if it needs setup call
@@ -71,40 +79,41 @@
     reals_path, fakes_path = f"{args.name}_reals", f"{args.name}_fakes"
     makedir(reals_path)
     makedir(fakes_path)
 
     progress_bar = tqdm(range(math.ceil(args.n/args.batch_size)), disable=not accelerator.is_local_main_process)
 
     for i, data in enumerate(dl):
-        reals = data[0][0]
-        #hprint(f"{ddps} i = {i}, reals.shape = {reals.shape}")
+        reals = data if local_data else data[0][0]
+        if args.debug: hprint(f"{ddps} i = {i}, reals.shape = {reals.shape}")
         
         with torch.no_grad():
             fakes = accelerator.unwrap_model(model).forward(reals.to(device)).cpu()
         #hprint(f"fakes.shape = {fakes.shape}")
         
         for b in range(reals.shape[0]):
             waveform = reals[b]
-            torchaudio.save(f"{reals_path}/{i}_{b}.wav", waveform, args.sample_rate)
+            torchaudio.save(f"{reals_path}/{i}_{b}.wav", waveform.cpu(), args.sample_rate)
             waveform = fakes[b]
-            torchaudio.save(f"{fakes_path}/{i}_{b}.wav", waveform, args.sample_rate)
+            torchaudio.save(f"{fakes_path}/{i}_{b}.wav", waveform.cpu(), args.sample_rate)
             
         progress_bar.update(1)
         if (i+1)*args.batch_size > args.n:
             hprint(f"\nGot all the data we needed: {i*args.batch_size}. Stopping")
             break
     
     hprint("Success!")
 
 # %% ../nbs/01_fad_gen.ipynb 8
 def main(): 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('name', help='Name prefix for output directories: <name>_reals/ & <name>_fakes/')
     parser.add_argument('model_ckpt', help='TorchScript (.ts) (Generative) Model checkpoint file')
-    parser.add_argument('data_sources', help='Space-separated string listing S3 resources for data')
+    parser.add_argument('data_sources', help='Space-separated string listing either S3 resources or local directories (but not a mix of both!) for real data')
+    parser.add_argument('-d','--debug', action="store_true", help='Enable extra debugging messages')
     parser.add_argument('-b',"--batch_size", default=2, help='batch size')
     parser.add_argument('--n', type=int, default=256, help='Number of real/fake samples to grab/generate, respectively')
     parser.add_argument('--num_workers', type=int, default=12, help='Number of pytorch workers to use in DataLoader')
     parser.add_argument('-p',"--profiles", default='', help='String representation of dict {resource:profile} of AWS credentials')
     parser.add_argument('--sample_rate', type=int, default=48000, help='sample rate (will resample inputs at this rate)')
     parser.add_argument('-s','--sample_size', type=int, default=2**18, help='Number of samples per clip')
     args = parser.parse_args()
```

### Comparing `fad_pytorch-0.0.5/fad_pytorch/fad_score.py` & `fad_pytorch-0.0.6/fad_pytorch/fad_score.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.5/fad_pytorch/pann.py` & `fad_pytorch-0.0.6/fad_pytorch/pann.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.5/fad_pytorch/pann_pytorch_utils.py` & `fad_pytorch-0.0.6/fad_pytorch/pann_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.5/fad_pytorch/sqrtm.py` & `fad_pytorch-0.0.6/fad_pytorch/sqrtm.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.5/fad_pytorch.egg-info/PKG-INFO` & `fad_pytorch-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fad-pytorch
-Version: 0.0.5
+Name: fad_pytorch
+Version: 0.0.6
 Summary: Frechet Audio Distance evaluation in PyTorch
 Home-page: https://github.com/drscotthawley/fad_pytorch
 Author: Scott H. Hawley
 Author-email: scott.hawley@belmont.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -29,40 +29,51 @@
 
 ## Install
 
 ``` sh
 pip install fad_pytorch
 ```
 
-## About
-
-Features:
+## Features:
 
 - runs in parallel on multiple processors and multiple GPUs (via
   `accelerate`)
 - supports multiple embedding methods:
   - VGGish and PANN, both mono @ 16kHz
   - OpenL3 and (LAION-)CLAP, stereo @ 48kHz
+- uses publicly-available pretrained checkpoints for music (+other
+  sources) for those models. (if you want Speech, submit a PR or an
+  Issue; I don’t do speech.)
 - favors ops in PyTorch rather than numpy (or tensorflow)
-- `fad_gen` supports WebDataset (audio data stored in S3 buckets)
+- `fad_gen` supports local data read or WebDataset (audio data stored in
+  S3 buckets)
 - runs on CPU, CUDA, or MPS
 
+## Instructions:
+
 This is designed to be run as 3 command-line scripts in succession. The
 latter 2 (`fad_embed` and `fad_score`) are probably what most people
 will want:
 
-1.  `fad_gen`: produces directories of real & fake audio. See
-    `fad_gen docs` for calling sequence.
+1.  `fad_gen`: produces directories of real & fake audio (given real
+    data). See `fad_gen`
+    [documentation](https://drscotthawley.github.io/fad_pytorch/fad_gen.html)
+    for calling sequence.
 2.  `fad_embed [options] <real_audio_dir> <fake_audio_dir>`: produces
     directories of *embeddings* of real & fake audio
-3.  `fad_score [optoions] <real_emb_dir> <fake_emb_dir>`: reads the
+3.  `fad_score [options] <real_emb_dir> <fake_emb_dir>`: reads the
     embeddings & generates FAD score, for real (“$r$”) and fake (“$f$”):
 
 $$ FAD = || \mu_r - \mu_f ||^2 + tr\left(\Sigma_r + \Sigma_f - 2 \sqrt{\Sigma_r \Sigma_f}\right)$$
 
+## Documentation
+
+See the [Documentation
+Website](https://drscotthawley.github.io/fad_pytorch/).
+
 ## Comments / FAQ / Troubleshooting
 
 - “`RuntimeError: CUDA error: invalid device ordinal`”: This happens
   when you have a “bad node” on an AWS cluster. [Haven’t yet figured out
   what causes it or how to fix
   it](https://discuss.huggingface.co/t/solved-accelerate-accelerator-cuda-error-invalid-device-ordinal/21509/1).
   Workaround: Just add the current node to your SLURM `--exclude` list,
@@ -77,36 +88,49 @@
   …Yea. There seems to be an uncertainty of around +/- 0.008. I’d say,
   don’t quote any numbers past the first decimal point.
 
 ## Contributing
 
 This repo is still fairly “bare bones” and will benefit from more
 documentation and features as time goes on. Note that it is written
-using [nbdev](https://nbdev.fast.ai/), so the things to are:
+using [nbdev](https://nbdev.fast.ai/), so the things to do are:
 
-1.  fork this repo
-2.  clone your fork to your (local) machine
+1.  Fork this repo
+2.  Clone your fork to your (local) machine
 3.  Install nbdev: `python3 -m pip install -U nbdev`
 4.  Make changes by editing the notebooks in `nbs/`, not the `.py` files
     in `fad_pytorch/`.
 5.  Run `nbdev_export` to export notebook changes to `.py` files
 6.  For good measure, run `nbdev_install_hooks` and `nbdev_clean` -
     especially if you’ve *added* any notebooks.
 7.  Do a `git status` to see all the `.ipynb` and `.py` files that need
     to be added & committed
 8.  `git add` those files and then `git commit`, and then `git push`
-9.  Take a look in your GitHub Actions tab, and see if the “test” and
-    “deploy” CI runs finish properly (green light) or fail (red light)
-10. One you get green lights, send in a Pull Request!
+9.  Take a look in your fork’s GitHub Actions tab, and see if the “test”
+    and “deploy” CI runs finish properly (green light) or fail (red
+    light)
+10. Once you get green lights, send in a Pull Request!
 
 *Feel free to ask me for tips with nbdev, it has quite a learning curve.
 You can also ask on [fast.ai forums](https://forums.fast.ai/) and/or
 [fast.ai
 Discord](https://discord.com/channels/689892369998676007/887694559952400424)*
 
+## Citations / Blame / Disclaimer
+
+This repo is 2 weeks old. I’m not ready for this to be cited in your
+papers. I’d hate for there to be some mistake I haven’t found yet.
+Perhaps a later version will have citation info. For now, instead,
+there’s:
+
+**Disclaimer:** Results from this repo are still a work in progress.
+While every effort has been made to test model outputs, the author takes
+no responsbility for mistakes. If you want to double-check via another
+source, see “Related Repos” below.
+
 ## Related Repos
 
 There are \[several\] others, but this one is mine. These repos didn’t
 have all the features I wanted, but I used them for inspiration:
 
 - https://github.com/gudgud96/frechet-audio-distance
 - https://github.com/google-research/google-research/tree/master/frechet_audio_distance:
```

### Comparing `fad_pytorch-0.0.5/settings.ini` & `fad_pytorch-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fad_pytorch
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fad_pytorch
```

### Comparing `fad_pytorch-0.0.5/setup.py` & `fad_pytorch-0.0.6/setup.py`

 * *Files identical despite different names*

