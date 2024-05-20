# Comparing `tmp/alphafold3_pytorch-0.0.3.tar.gz` & `tmp/alphafold3_pytorch-0.0.4.tar.gz`

## Comparing `alphafold3_pytorch-0.0.3.tar` & `alphafold3_pytorch-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/.env.sample
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/alphafold3.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0    69445 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/tests/test_readme.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/LICENSE
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/.env.sample
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/alphafold3.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0    69585 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/tests/test_readme.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.4/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.0.3/alphafold3.png` & `alphafold3_pytorch-0.0.4/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/.github/workflows/publish.yml` & `alphafold3_pytorch-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.0.4/alphafold3_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.0.4/alphafold3_pytorch/alphafold3.py`

 * *Files 1% similar despite different names*

```diff
@@ -2191,14 +2191,15 @@
         atom_mask: Bool['b m'],
         atompair_feats: Float['b m m dap'],
         additional_residue_feats: Float['b n rf'],
         msa: Float['b s n d'],
         templates: Float['b t n n dt'],
         template_mask: Bool['b t'],
         num_recycling_steps: int = 1,
+        residue_atom_indices: Int['b n'] | None = None,
         num_sample_steps: int | None = None,
         atom_pos: Float['b m 3'] | None = None,
         distance_labels: Int['b n n'] | None = None,
         pae_labels: Int['b n n'] | None = None,
         pde_labels: Int['b n n'] | None = None,
         plddt_labels: Int['b n'] | None = None,
         resolved_labels: Int['b n'] | None = None,
@@ -2314,47 +2315,48 @@
         )
 
         # if neither atom positions or any labels are passed in, sample a structure and return
 
         if not return_loss:
             return self.edm.sample(num_sample_steps = num_sample_steps, **diffusion_cond)
 
-        # otherwise, noise and make it learn to denoise
+        # losses default to 0
+
+        distogram_loss = diffusion_loss = confidence_loss = pae_loss = pde_loss = plddt_loss = resolved_loss = self.zero
 
-        diffusion_loss = self.zero
+        # otherwise, noise and make it learn to denoise
 
         if exists(atom_pos):
             diffusion_loss, denoised_atom_pos = self.edm(atom_pos, return_denoised_pos = True, **diffusion_cond)
 
         # calculate all logits and losses
 
         ignore = self.ignore_index
 
         # distogram head
 
-        distogram_loss = self.zero
-
         if exists(distance_labels):
             distance_labels = torch.where(pairwise_mask, distance_labels, ignore)
             distogram_logits = self.distogram_head(pairwise)
             distogram_loss = F.cross_entropy(distogram_logits, distance_labels, ignore_index = ignore)
 
         # confidence head
 
         should_call_confidence_head = any([*map(exists, confidence_head_labels)])
         return_pae_logits = exists(pae_labels)
 
-        confidence_loss = pae_loss = pde_loss = plddt_loss = resolved_loss = self.zero
 
         if should_call_confidence_head:
             assert exists(atom_pos), 'diffusion module needs to have been called'
 
-            # fix this to accept representative atom indices for each residue
+            assert exists(residue_atom_indices)
+
+            windowed_denoised_atom_pos = rearrange(denoised_atom_pos, 'b (n w) c -> b n w c', w = w)
 
-            pred_atom_pos = rearrange(denoised_atom_pos, 'b (n w) d -> b n w d', w = w)[..., 0, :]
+            pred_atom_pos = einx.get_at('b n [w] c, b n -> b n c', windowed_denoised_atom_pos, residue_atom_indices)
 
             logits = self.confidence_head(
                 single_repr = single,
                 single_inputs_repr = single_inputs,
                 pairwise_repr = pairwise,
                 pred_atom_pos = pred_atom_pos,
                 mask = mask,
```

### Comparing `alphafold3_pytorch-0.0.3/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.0.4/alphafold3_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.0.4/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.0.4/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/tests/test_readme.py` & `alphafold3_pytorch-0.0.4/tests/test_readme.py`

 * *Files 5% similar despite different names*

```diff
@@ -253,14 +253,15 @@
 
     template_feats = torch.randn(2, 2, seq_len, seq_len, 44)
     template_mask = torch.ones((2, 2)).bool()
 
     msa = torch.randn(2, 7, seq_len, 64)
 
     atom_pos = torch.randn(2, atom_seq_len, 3)
+    residue_atom_indices = torch.randint(0, 27, (2, seq_len))
 
     distance_labels = torch.randint(0, 38, (2, seq_len, seq_len))
     pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
     pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
     plddt_labels = torch.randint(0, 50, (2, seq_len))
     resolved_labels = torch.randint(0, 2, (2, seq_len))
 
@@ -277,14 +278,15 @@
         atom_mask = atom_mask,
         atompair_feats = atompair_feats,
         additional_residue_feats = additional_residue_feats,
         msa = msa,
         templates = template_feats,
         template_mask = template_mask,
         atom_pos = atom_pos,
+        residue_atom_indices = residue_atom_indices,
         distance_labels = distance_labels,
         pae_labels = pae_labels,
         pde_labels = pde_labels,
         plddt_labels = plddt_labels,
         resolved_labels = resolved_labels
     )
```

### Comparing `alphafold3_pytorch-0.0.3/.gitignore` & `alphafold3_pytorch-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/LICENSE` & `alphafold3_pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.3/README.md` & `alphafold3_pytorch-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -42,29 +42,40 @@
 template_mask = torch.ones((2, 2)).bool()
 
 msa = torch.randn(2, 7, seq_len, 64)
 
 # required for training, but omitted on inference
 
 atom_pos = torch.randn(2, atom_seq_len, 3)
+residue_atom_indices = torch.randint(0, 27, (2, seq_len))
+
 distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
+pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+plddt_labels = torch.randint(0, 50, (2, seq_len))
+resolved_labels = torch.randint(0, 2, (2, seq_len))
 
 # train
 
 loss = alphafold3(
     num_recycling_steps = 2,
     atom_inputs = atom_inputs,
     atom_mask = atom_mask,
     atompair_feats = atompair_feats,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
     templates = template_feats,
     template_mask = template_mask,
     atom_pos = atom_pos,
-    distance_labels = distance_labels
+    residue_atom_indices = residue_atom_indices,
+    distance_labels = distance_labels,
+    pae_labels = pae_labels,
+    pde_labels = pde_labels,
+    plddt_labels = plddt_labels,
+    resolved_labels = resolved_labels
 )
 
 loss.backward()
 
 # after much training ...
 
 sampled_atom_pos = alphafold3(
```

#### html2text {}

```diff
@@ -7,33 +7,40 @@
 33, dim_template_feats = 44 ) # mock inputs seq_len = 16 atom_seq_len = seq_len
 * 27 atom_inputs = torch.randn(2, atom_seq_len, 77) atom_mask = torch.ones((2,
 atom_seq_len)).bool() atompair_feats = torch.randn(2, atom_seq_len,
 atom_seq_len, 16) additional_residue_feats = torch.randn(2, seq_len, 33)
 template_feats = torch.randn(2, 2, seq_len, seq_len, 44) template_mask =
 torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) # required for
 training, but omitted on inference atom_pos = torch.randn(2, atom_seq_len, 3)
-distance_labels = torch.randint(0, 37, (2, seq_len, seq_len)) # train loss =
-alphafold3( num_recycling_steps = 2, atom_inputs = atom_inputs, atom_mask =
-atom_mask, atompair_feats = atompair_feats, additional_residue_feats =
+residue_atom_indices = torch.randint(0, 27, (2, seq_len)) distance_labels =
+torch.randint(0, 37, (2, seq_len, seq_len)) pae_labels = torch.randint(0, 64,
+(2, seq_len, seq_len)) pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+plddt_labels = torch.randint(0, 50, (2, seq_len)) resolved_labels =
+torch.randint(0, 2, (2, seq_len)) # train loss = alphafold3
+( num_recycling_steps = 2, atom_inputs = atom_inputs, atom_mask = atom_mask,
+atompair_feats = atompair_feats, additional_residue_feats =
 additional_residue_feats, msa = msa, templates = template_feats, template_mask
-= template_mask, atom_pos = atom_pos, distance_labels = distance_labels )
-loss.backward() # after much training ... sampled_atom_pos = alphafold3
-( num_recycling_steps = 4, num_sample_steps = 16, atom_inputs = atom_inputs,
-atom_mask = atom_mask, atompair_feats = atompair_feats,
-additional_residue_feats = additional_residue_feats, msa = msa, templates =
-template_feats, template_mask = template_mask ) sampled_atom_pos.shape # (2, 16
-* 27, 3) ``` ## Citations ```bibtex @article{Abramson2024-fj, title = "Accurate
-structure prediction of biomolecular interactions with {AlphaFold} 3", author =
-"Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans, Richard and Green,
-Tim and Pritzel, Alexander and Ronneberger, Olaf and Willmore, Lindsay and
-Ballard, Andrew J and Bambrick, Joshua and Bodenstein, Sebastian W and Evans,
-David A and Hung, Chia-Chun and O'Neill, Michael and Reiman, David and
-Tunyasuvunakool, Kathryn and Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and
-Arvaniti, Eirini and Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex
-and Cherepanov, Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and
-Cowie, Andrew and Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and
-Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and
-Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and
-Thillaisundaram, Ashok and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen
-D and Zielinski, Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and
-Kohli, Pushmeet and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
-journal = "Nature", month = "May", year = 2024 } ```
+= template_mask, atom_pos = atom_pos, residue_atom_indices =
+residue_atom_indices, distance_labels = distance_labels, pae_labels =
+pae_labels, pde_labels = pde_labels, plddt_labels = plddt_labels,
+resolved_labels = resolved_labels ) loss.backward() # after much training ...
+sampled_atom_pos = alphafold3( num_recycling_steps = 4, num_sample_steps = 16,
+atom_inputs = atom_inputs, atom_mask = atom_mask, atompair_feats =
+atompair_feats, additional_residue_feats = additional_residue_feats, msa = msa,
+templates = template_feats, template_mask = template_mask )
+sampled_atom_pos.shape # (2, 16 * 27, 3) ``` ## Citations ```bibtex @article
+{Abramson2024-fj, title = "Accurate structure prediction of biomolecular
+interactions with {AlphaFold} 3", author = "Abramson, Josh and Adler, Jonas and
+Dunger, Jack and Evans, Richard and Green, Tim and Pritzel, Alexander and
+Ronneberger, Olaf and Willmore, Lindsay and Ballard, Andrew J and Bambrick,
+Joshua and Bodenstein, Sebastian W and Evans, David A and Hung, Chia-Chun and
+O'Neill, Michael and Reiman, David and Tunyasuvunakool, Kathryn and Wu, Zachary
+and {\v Z}emgulyt{\.e}, Akvil{\.e} and Arvaniti, Eirini and Beattie, Charles
+and Bertolli, Ottavia and Bridgland, Alex and Cherepanov, Alexey and Congreve,
+Miles and Cowen-Rivers, Alexander I and Cowie, Andrew and Figurnov, Michael and
+Fuchs, Fabian B and Gladman, Hannah and Jain, Rishub and Khan, Yousuf A and
+Low, Caroline M R and Perlin, Kuba and Potapenko, Anna and Savy, Pascal and
+Singh, Sukhdeep and Stecula, Adrian and Thillaisundaram, Ashok and Tong,
+Catherine and Yakneen, Sergei and Zhong, Ellen D and Zielinski, Michal and {\v
+Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet and Jaderberg, Max
+and Hassabis, Demis and Jumper, John M", journal = "Nature", month = "May",
+year = 2024 } ```
```

### Comparing `alphafold3_pytorch-0.0.3/pyproject.toml` & `alphafold3_pytorch-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.0.3"
+version = "0.0.4"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
```

### Comparing `alphafold3_pytorch-0.0.3/PKG-INFO` & `alphafold3_pytorch-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
@@ -90,29 +90,40 @@
 template_mask = torch.ones((2, 2)).bool()
 
 msa = torch.randn(2, 7, seq_len, 64)
 
 # required for training, but omitted on inference
 
 atom_pos = torch.randn(2, atom_seq_len, 3)
+residue_atom_indices = torch.randint(0, 27, (2, seq_len))
+
 distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
+pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+plddt_labels = torch.randint(0, 50, (2, seq_len))
+resolved_labels = torch.randint(0, 2, (2, seq_len))
 
 # train
 
 loss = alphafold3(
     num_recycling_steps = 2,
     atom_inputs = atom_inputs,
     atom_mask = atom_mask,
     atompair_feats = atompair_feats,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
     templates = template_feats,
     template_mask = template_mask,
     atom_pos = atom_pos,
-    distance_labels = distance_labels
+    residue_atom_indices = residue_atom_indices,
+    distance_labels = distance_labels,
+    pae_labels = pae_labels,
+    pde_labels = pde_labels,
+    plddt_labels = plddt_labels,
+    resolved_labels = resolved_labels
 )
 
 loss.backward()
 
 # after much training ...
 
 sampled_atom_pos = alphafold3(
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.3 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.4 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -34,34 +34,40 @@
 77, dim_additional_residue_feats = 33, dim_template_feats = 44 ) # mock inputs
 seq_len = 16 atom_seq_len = seq_len * 27 atom_inputs = torch.randn(2,
 atom_seq_len, 77) atom_mask = torch.ones((2, atom_seq_len)).bool()
 atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
 additional_residue_feats = torch.randn(2, seq_len, 33) template_feats =
 torch.randn(2, 2, seq_len, seq_len, 44) template_mask = torch.ones((2, 2)).bool
 () msa = torch.randn(2, 7, seq_len, 64) # required for training, but omitted on
-inference atom_pos = torch.randn(2, atom_seq_len, 3) distance_labels =
-torch.randint(0, 37, (2, seq_len, seq_len)) # train loss = alphafold3
-( num_recycling_steps = 2, atom_inputs = atom_inputs, atom_mask = atom_mask,
-atompair_feats = atompair_feats, additional_residue_feats =
-additional_residue_feats, msa = msa, templates = template_feats, template_mask
-= template_mask, atom_pos = atom_pos, distance_labels = distance_labels )
-loss.backward() # after much training ... sampled_atom_pos = alphafold3
-( num_recycling_steps = 4, num_sample_steps = 16, atom_inputs = atom_inputs,
-atom_mask = atom_mask, atompair_feats = atompair_feats,
+inference atom_pos = torch.randn(2, atom_seq_len, 3) residue_atom_indices =
+torch.randint(0, 27, (2, seq_len)) distance_labels = torch.randint(0, 37, (2,
+seq_len, seq_len)) pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+pde_labels = torch.randint(0, 64, (2, seq_len, seq_len)) plddt_labels =
+torch.randint(0, 50, (2, seq_len)) resolved_labels = torch.randint(0, 2, (2,
+seq_len)) # train loss = alphafold3( num_recycling_steps = 2, atom_inputs =
+atom_inputs, atom_mask = atom_mask, atompair_feats = atompair_feats,
 additional_residue_feats = additional_residue_feats, msa = msa, templates =
-template_feats, template_mask = template_mask ) sampled_atom_pos.shape # (2, 16
-* 27, 3) ``` ## Citations ```bibtex @article{Abramson2024-fj, title = "Accurate
-structure prediction of biomolecular interactions with {AlphaFold} 3", author =
-"Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans, Richard and Green,
-Tim and Pritzel, Alexander and Ronneberger, Olaf and Willmore, Lindsay and
-Ballard, Andrew J and Bambrick, Joshua and Bodenstein, Sebastian W and Evans,
-David A and Hung, Chia-Chun and O'Neill, Michael and Reiman, David and
-Tunyasuvunakool, Kathryn and Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and
-Arvaniti, Eirini and Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex
-and Cherepanov, Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and
-Cowie, Andrew and Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and
-Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and
-Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and
-Thillaisundaram, Ashok and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen
-D and Zielinski, Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and
-Kohli, Pushmeet and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
-journal = "Nature", month = "May", year = 2024 } ```
+template_feats, template_mask = template_mask, atom_pos = atom_pos,
+residue_atom_indices = residue_atom_indices, distance_labels = distance_labels,
+pae_labels = pae_labels, pde_labels = pde_labels, plddt_labels = plddt_labels,
+resolved_labels = resolved_labels ) loss.backward() # after much training ...
+sampled_atom_pos = alphafold3( num_recycling_steps = 4, num_sample_steps = 16,
+atom_inputs = atom_inputs, atom_mask = atom_mask, atompair_feats =
+atompair_feats, additional_residue_feats = additional_residue_feats, msa = msa,
+templates = template_feats, template_mask = template_mask )
+sampled_atom_pos.shape # (2, 16 * 27, 3) ``` ## Citations ```bibtex @article
+{Abramson2024-fj, title = "Accurate structure prediction of biomolecular
+interactions with {AlphaFold} 3", author = "Abramson, Josh and Adler, Jonas and
+Dunger, Jack and Evans, Richard and Green, Tim and Pritzel, Alexander and
+Ronneberger, Olaf and Willmore, Lindsay and Ballard, Andrew J and Bambrick,
+Joshua and Bodenstein, Sebastian W and Evans, David A and Hung, Chia-Chun and
+O'Neill, Michael and Reiman, David and Tunyasuvunakool, Kathryn and Wu, Zachary
+and {\v Z}emgulyt{\.e}, Akvil{\.e} and Arvaniti, Eirini and Beattie, Charles
+and Bertolli, Ottavia and Bridgland, Alex and Cherepanov, Alexey and Congreve,
+Miles and Cowen-Rivers, Alexander I and Cowie, Andrew and Figurnov, Michael and
+Fuchs, Fabian B and Gladman, Hannah and Jain, Rishub and Khan, Yousuf A and
+Low, Caroline M R and Perlin, Kuba and Potapenko, Anna and Savy, Pascal and
+Singh, Sukhdeep and Stecula, Adrian and Thillaisundaram, Ashok and Tong,
+Catherine and Yakneen, Sergei and Zhong, Ellen D and Zielinski, Michal and {\v
+Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet and Jaderberg, Max
+and Hassabis, Demis and Jumper, John M", journal = "Nature", month = "May",
+year = 2024 } ```
```

