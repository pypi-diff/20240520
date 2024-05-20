# Comparing `tmp/alphafold3_pytorch-0.0.1.tar.gz` & `tmp/alphafold3_pytorch-0.0.2.tar.gz`

## Comparing `alphafold3_pytorch-0.0.1.tar` & `alphafold3_pytorch-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/.env.sample
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/alphafold3.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0    60360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/tests/test_readme.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/LICENSE
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/.env.sample
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/alphafold3.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0    67235 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/tests/test_readme.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.2/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.0.1/alphafold3.png` & `alphafold3_pytorch-0.0.2/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.1/.github/workflows/publish.yml` & `alphafold3_pytorch-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.1/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.0.2/alphafold3_pytorch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from alphafold3_pytorch.attention import (
     Attention,
     Attend
 )
 
 from alphafold3_pytorch.alphafold3 import (
+    RelativePositionEncoding,
     TemplateEmbedder,
     PreLayerNorm,
     AdaptiveLayerNorm,
     ConditionWrapper,
     OuterProductMean,
     MSAPairWeightedAveraging,
     TriangleMultiplication,
@@ -24,14 +25,15 @@
     DistogramHead,
     Alphafold3
 )
 
 __all__ = [
     Attention,
     Attend,
+    RelativePositionEncoding,
     TemplateEmbedder,
     PreLayerNorm,
     AdaptiveLayerNorm,
     ConditionWrapper,
     OuterProductMean,
     MSAPairWeightedAveraging,
     TriangleMultiplication,
```

### Comparing `alphafold3_pytorch-0.0.1/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.0.2/alphafold3_pytorch/alphafold3.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 b - batch
 h - heads
 n - residue sequence length
 i - residue sequence length (source)
 j - residue sequence length (target)
 m - atom sequence length
-c - coordinates (3 for spatial)
 d - feature dimension
 ds - feature dimension (single)
 dp - feature dimension (pairwise)
 dap - feature dimension (atompair)
-da - feature dimensino (atom)
+da - feature dimension (atom)
 t - templates
-m - msa
+s - msa
 """
 
 from __future__ import annotations
 
 from math import pi, sqrt
 from functools import partial
 from collections import namedtuple
@@ -819,14 +818,107 @@
             single_repr = pair_bias_attn(single_repr, pairwise_repr = pairwise_repr, mask = mask) + single_repr
             single_repr = single_transition(single_repr) + single_repr
 
         return single_repr, pairwise_repr
 
 # embedding related
 
+"""
+additional_residue_feats: [*, rf]:
+    0: residue_index
+    1: token_index
+    2: asym_id
+    3: entity_id
+    4: sym_id 
+    5: restype (must be one hot encoded to 32)
+    6: is_protein
+    7: is_rna
+    8: is_dna
+    9: is_ligand
+"""
+
+class RelativePositionEncoding(Module):
+    """ Algorithm 3 """
+    
+    def __init__(
+        self,
+        *,
+        r_max = 32,
+        s_max = 2,
+        dim_out = 128
+    ):
+        super().__init__()
+        self.r_max = r_max
+        self.s_max = s_max
+        
+        dim_input = (2*r_max+2) + (2*r_max+2) + 1 + (2*s_max+2)
+        self.out_embedder = LinearNoBias(dim_input, dim_out)
+
+    @typecheck
+    def forward(
+        self,
+        *,
+        additional_residue_feats: Float['b n rf']
+    ) -> Float['b n n dp']:
+
+        device = additional_residue_feats.device
+        assert additional_residue_feats.shape[-1] >= 5
+
+        res_idx, token_idx, asym_id, entity_id, sym_id = additional_residue_feats[..., :5].unbind(dim = -1)
+        
+        diff_res_idx = einx.subtract('b i, b j -> b i j', res_idx, res_idx)
+        diff_token_idx = einx.subtract('b i, b j -> b i j', token_idx, token_idx)
+        diff_sym_id = einx.subtract('b i, b j -> b i j', sym_id, sym_id)
+
+        mask_same_chain = einx.subtract('b i, b j -> b i j', asym_id, asym_id) == 0
+        mask_same_res = diff_res_idx == 0
+        mask_same_entity = einx.subtract('b i, b j -> b i j 1', entity_id, entity_id) == 0
+        
+        d_res = torch.where(
+            mask_same_chain, 
+            torch.clip(diff_res_idx + self.r_max, 0, 2*self.r_max),
+            2*self.r_max + 1
+        )
+
+        d_token = torch.where(
+            mask_same_chain * mask_same_res, 
+            torch.clip(diff_token_idx + self.r_max, 0, 2*self.r_max),
+            2*self.r_max + 1
+        )
+
+        d_chain = torch.where(
+            ~mask_same_chain, 
+            torch.clip(diff_sym_id + self.s_max, 0, 2*self.s_max),
+            2*self.s_max + 1
+        )
+        
+        def onehot(x, bins):
+            x, packed_shape = pack_one(x, '*')
+            dist_from_bins = einx.subtract('i, j -> i j', x, bins)
+            indexes = dist_from_bins.abs().min(dim = 1, keepdim = True).indices
+            indexes = rearrange(indexes.long(), 'i j -> (i j) 1')
+            one_hots = torch.zeros(indexes.shape[0], len(bins)).scatter_(1, indexes, 1)
+            return unpack_one(one_hots, packed_shape, '* d')
+
+        r_arange = torch.arange(2*self.r_max + 2, device = device)
+        s_arange = torch.arange(2*self.s_max + 2, device = device)
+
+        a_rel_pos = onehot(d_res, r_arange)
+        a_rel_token = onehot(d_token, r_arange)
+        a_rel_chain = onehot(d_chain, s_arange)
+
+        out, _ = pack((
+            a_rel_pos,
+            a_rel_token,
+            mask_same_entity,
+            a_rel_chain
+        ), 'b i j *')
+
+        return self.out_embedder(out)
+
 class TemplateEmbedder(Module):
     """ Algorithm 16 """
 
     def __init__(
         self,
         *,
         dim_template_feats,
@@ -1288,15 +1380,15 @@
             nn.LayerNorm(dim_atom),
             LinearNoBias(dim_atom, 3)
         )
 
     @typecheck
     def forward(
         self,
-        noised_atom_pos: Float['b m c'],
+        noised_atom_pos: Float['b m 3'],
         *,
         atom_feats: Float['b m da'],
         atompair_feats: Float['b m m dap'],
         atom_mask: Bool['b m'],
         times: Float[' b'],
         mask: Bool['b n'],
         single_trunk_repr: Float['b n dst'],
@@ -1461,15 +1553,15 @@
 
     # preconditioned network output
     # equation (7) in the paper
 
     @typecheck
     def preconditioned_network_forward(
         self,
-        noised_atom_pos: Float['b m c'],
+        noised_atom_pos: Float['b m 3'],
         sigma: Float[' b'] | Float[' '] | float,
         network_condition_kwargs: dict,
         clamp = False,
     ):
         batch, device = noised_atom_pos.shape[0], noised_atom_pos.device
 
         if isinstance(sigma, float):
@@ -1811,15 +1903,15 @@
     @typecheck
     def forward(
         self,
         *,
         single_inputs_repr: Float['b n dsi'],
         single_repr: Float['b n ds'],
         pairwise_repr: Float['b n n dp'],
-        pred_atom_pos: Float['b n c'],
+        pred_atom_pos: Float['b n 3'],
         mask: Bool['b n'] | None = None,
         return_pae_logits = True
 
     ) -> ConfidenceHeadLogits[
         Float['b pae n n'] | None,
         Float['b pde n n'],
         Float['b plddt n'],
@@ -1886,20 +1978,22 @@
         dim_template_model = 64,
         atoms_per_window = 27,
         dim_atom = 128,
         dim_atompair = 16,
         dim_input_embedder_token = 384,
         dim_single = 384,
         dim_pairwise = 128,
+        dim_token = 768,
         atompair_dist_bins: Float[' dist_bins'] = torch.linspace(3, 20, 37),
         ignore_index = -1,
         num_dist_bins = 38,
         num_plddt_bins = 50,
         num_pde_bins = 64,
         num_pae_bins = 64,
+        sigma_data = 16,
         loss_confidence_weight = 1e-4,
         loss_distogram_weight = 1e-2,
         loss_diffusion_weight = 4.,
         input_embedder_kwargs: dict = dict(
             atom_transformer_blocks = 3,
             atom_transformer_heads = 4,
             atom_transformer_kwargs = dict()
@@ -1923,14 +2017,44 @@
         ),
         pairformer_stack: dict = dict(
             depth = 48,
             pair_bias_attn_dim_head = 64,
             pair_bias_attn_heads = 16,
             dropout_row_prob = 0.25,
             pairwise_block_kwargs = dict()
+        ),
+        relative_position_encoding_kwargs: dict = dict(
+            r_max = 32,
+            s_max = 2,
+        ),
+        diffusion_module_kwargs: dict = dict(
+            single_cond_kwargs = dict(
+                num_transitions = 2,
+                transition_expansion_factor = 2,
+            ),
+            pairwise_cond_kwargs = dict(
+                num_transitions = 2
+            ),
+            atom_encoder_depth = 3,
+            atom_encoder_heads = 4,
+            token_transformer_depth = 24,
+            token_transformer_heads = 16,
+            atom_decoder_depth = 3,
+            atom_decoder_heads = 4
+        ),
+        edm_kwargs: dict = dict(
+            sigma_min = 0.002,
+            sigma_max = 80,
+            rho = 7,
+            P_mean = -1.2,
+            P_std = 1.2,
+            S_churn = 80,
+            S_tmin = 0.05,
+            S_tmax = 50,
+            S_noise = 1.003,
         )
     ):
         super().__init__()
 
         self.atoms_per_window = atoms_per_window
 
         # input feature embedder
@@ -1945,14 +2069,23 @@
             dim_single = dim_single,
             dim_pairwise = dim_pairwise,
             **input_embedder_kwargs
         )
 
         dim_single_inputs = dim_input_embedder_token + dim_additional_residue_feats
 
+        # relative positional encoding
+        # used by pairwise in main alphafold2 trunk
+        # and also in the diffusion module separately from alphafold3
+
+        self.relative_position_encoding = RelativePositionEncoding(
+            dim_out = dim_pairwise,
+            **relative_position_encoding_kwargs
+        )
+
         # templates
 
         self.template_embedder = TemplateEmbedder(
             dim_template_feats = dim_template_feats,
             dim = dim_template_model,
             dim_pairwise = dim_pairwise,
             **template_embedder_kwargs
@@ -1982,14 +2115,35 @@
         )
 
         self.recycle_pairwise = nn.Sequential(
             nn.LayerNorm(dim_pairwise),
             LinearNoBias(dim_pairwise, dim_pairwise)
         )
 
+        # diffusion
+
+        self.diffusion_module = DiffusionModule(
+            dim_pairwise_trunk = dim_pairwise,
+            dim_pairwise_rel_pos_feats = dim_pairwise,
+            atoms_per_window = atoms_per_window,
+            dim_pairwise = dim_pairwise,
+            sigma_data = sigma_data,
+            dim_atom = dim_atom,
+            dim_atompair = dim_atompair,
+            dim_token = dim_token,
+            dim_single = dim_single + dim_single_inputs,
+            **diffusion_module_kwargs
+        )
+
+        self.edm = ElucidatedAtomDiffusion(
+            self.diffusion_module,
+            sigma_data = sigma_data,
+            **edm_kwargs
+        )
+
         # logit heads
 
         self.distogram_head = DistogramHead(
             dim_pairwise = dim_pairwise,
             num_dist_bins = num_dist_bins
         )
 
@@ -2007,32 +2161,42 @@
         # loss related
 
         self.ignore_index = ignore_index
         self.loss_distogram_weight = loss_distogram_weight
         self.loss_confidence_weight = loss_confidence_weight
         self.loss_diffusion_weight = loss_diffusion_weight
 
+        self.register_buffer('zero', torch.tensor(0.), persistent = False)
+
+    @property
+    def device(self):
+        return self.zero.device
+
     @typecheck
     def forward(
         self,
         *,
         atom_inputs: Float['b m dai'],
         atom_mask: Bool['b m'],
         atompair_feats: Float['b m m dap'],
         additional_residue_feats: Float['b n rf'],
         msa: Float['b s n d'],
         templates: Float['b t n n dt'],
         template_mask: Bool['b t'],
         num_recycling_steps: int = 1,
+        num_sample_steps: int | None = None,
+        atom_pos: Float['b m 3'] | None = None,
         distance_labels: Int['b n n'] | None = None,
         pae_labels: Int['b n n'] | None = None,
         pde_labels: Int['b n n'] | None = None,
         plddt_labels: Int['b n'] | None = None,
         resolved_labels: Int['b n'] | None = None,
-    ) -> Float['b m c'] | Float['']:
+    ) -> Float['b m 3'] | Float['']:
+
+        w = self.atoms_per_window
 
         # embed inputs
 
         (
             single_inputs,
             single_init,
             pairwise_init,
@@ -2041,17 +2205,26 @@
         ) = self.input_embedder(
             atom_inputs = atom_inputs,
             atom_mask = atom_mask,
             atompair_feats = atompair_feats,
             additional_residue_feats = additional_residue_feats
         )
 
-        w = self.atoms_per_window
+        # relative positional encoding
+
+        relative_position_encoding = self.relative_position_encoding(
+            additional_residue_feats = additional_residue_feats
+        )
+
+        pairwise_init = pairwise_init + relative_position_encoding
+
+        # pairwise mask
 
         mask = reduce(atom_mask, 'b (n w) -> b n', w = w, reduction = 'any')
+        pairwise_mask = einx.logical_and('b i, b j -> b i j', mask, mask)
 
         # init recycled single and pairwise
 
         recycled_pairwise = recycled_single = None
         single = pairwise = None
 
         # for each recycling step
@@ -2102,11 +2275,56 @@
                 pairwise_repr = pairwise,
                 mask = mask
             )
 
         # determine whether to return loss if any labels were to be passed in
         # otherwise will sample the atomic coordinates
 
+        atom_pos_given = exists(atom_pos)
+
         labels = (distance_labels, pae_labels, pde_labels, plddt_labels, resolved_labels)
-        return_loss = any([*filter(exists, labels)])
+        has_labels = any([*map(exists, labels)])
+
+        return_loss = atom_pos_given or has_labels
+
+        # setup all the data necessary for conditioning the diffusion module
+
+        diffusion_cond = dict(
+            atom_feats = atom_feats,
+            atompair_feats = atompair_feats,
+            atom_mask = atom_mask,
+            mask = mask,
+            single_trunk_repr = single,
+            single_inputs_repr = single_inputs,
+            pairwise_trunk = pairwise,
+            pairwise_rel_pos_feats = relative_position_encoding
+        )
+
+        # if neither atom positions or any labels are passed in, sample a structure and return
+
+        if not return_loss:
+            return self.edm.sample(num_sample_steps = num_sample_steps, **diffusion_cond)
+
+        # otherwise, noise and make it learn to denoise
+
+        diffusion_loss = self.zero
+
+        if exists(atom_pos):
+            diffusion_loss = self.edm(atom_pos, **diffusion_cond)
+
+        # calculate all logits and losses
+
+        ignore = self.ignore_index
+
+        distogram_loss = self.zero
+
+        if exists(distance_labels):
+            distance_labels = torch.where(pairwise_mask, distance_labels, ignore)
+            distogram_logits = self.distogram_head(pairwise)
+            distogram_loss = F.cross_entropy(distogram_logits, distance_labels, ignore_index = ignore)
+
+        loss = (
+            distogram_loss * self.loss_distogram_weight +
+            diffusion_loss * self.loss_diffusion_weight
+        )
 
-        return torch.tensor(0.)
+        return loss
```

### Comparing `alphafold3_pytorch-0.0.1/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.0.2/alphafold3_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.1/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.0.2/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.1/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.0.2/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.1/tests/test_readme.py` & `alphafold3_pytorch-0.0.2/tests/test_readme.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 
 from alphafold3_pytorch import (
     PairformerStack,
     MSAModule,
     DiffusionTransformer,
     DiffusionModule,
     ElucidatedAtomDiffusion,
+    RelativePositionEncoding,
     TemplateEmbedder,
     Attention,
     InputFeatureEmbedder,
     ConfidenceHead,
     DistogramHead,
-    Alphafold3
+    Alphafold3,
 )
 
 def test_pairformer():
     single = torch.randn(2, 16, 384)
     pairwise = torch.randn(2, 16, 16, 128)
     mask = torch.randint(0, 2, (2, 16)).bool()
 
@@ -158,14 +159,23 @@
         single_trunk_repr = single_trunk_repr,
         single_inputs_repr = single_inputs_repr,
         pairwise_trunk = pairwise_trunk,
         pairwise_rel_pos_feats = pairwise_rel_pos_feats
     )
 
     assert sampled_atom_pos.shape == noised_atom_pos.shape
+    
+def test_relative_position_encoding():
+    additional_residue_feats = torch.randn(8, 100, 10)
+
+    embedder = RelativePositionEncoding()
+
+    rpe_embed = embedder(
+        additional_residue_feats = additional_residue_feats
+    )
 
 def test_template_embed():
     template_feats = torch.randn(2, 2, 16, 16, 77)
     template_mask = torch.ones((2, 2)).bool()
 
     pairwise_repr = torch.randn(2, 16, 16, 128)
     mask = torch.ones((2, 16)).bool()
@@ -242,25 +252,44 @@
     additional_residue_feats = torch.randn(2, seq_len, 33)
 
     template_feats = torch.randn(2, 2, seq_len, seq_len, 44)
     template_mask = torch.ones((2, 2)).bool()
 
     msa = torch.randn(2, 7, seq_len, 64)
 
+    atom_pos = torch.randn(2, atom_seq_len, 3)
+    distance_labels = torch.randint(0, 38, (2, seq_len, seq_len))
+
     alphafold3 = Alphafold3(
         dim_atom_inputs = 77,
         dim_additional_residue_feats = 33,
-        dim_template_feats = 44
+        dim_template_feats = 44,
+        num_dist_bins = 38
     )
 
     loss = alphafold3(
         num_recycling_steps = 2,
         atom_inputs = atom_inputs,
         atom_mask = atom_mask,
         atompair_feats = atompair_feats,
         additional_residue_feats = additional_residue_feats,
         msa = msa,
         templates = template_feats,
-        template_mask = template_mask
+        template_mask = template_mask,
+        atom_pos = atom_pos,
+        distance_labels = distance_labels
+    )
+
+    loss.backward()
+
+    sampled_atom_pos = alphafold3(
+        num_sample_steps = 16,
+        atom_inputs = atom_inputs,
+        atom_mask = atom_mask,
+        atompair_feats = atompair_feats,
+        additional_residue_feats = additional_residue_feats,
+        msa = msa,
+        templates = template_feats,
+        template_mask = template_mask,
     )
 
-    print(loss)
+    assert sampled_atom_pos.ndim == 3
```

### Comparing `alphafold3_pytorch-0.0.1/.gitignore` & `alphafold3_pytorch-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.1/LICENSE` & `alphafold3_pytorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.1/README.md` & `alphafold3_pytorch-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 ## Alphafold 3 - Pytorch (wip)
 
 Implementation of <a href="https://www.nature.com/articles/s41586-024-07487-w">Alphafold 3</a> in Pytorch
 
 Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
+## Appreciation
+
+- <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the relative positional encoding module!
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
@@ -35,29 +39,51 @@
 additional_residue_feats = torch.randn(2, seq_len, 33)
 
 template_feats = torch.randn(2, 2, seq_len, seq_len, 44)
 template_mask = torch.ones((2, 2)).bool()
 
 msa = torch.randn(2, 7, seq_len, 64)
 
+# required for training, but omitted on inference
+
+atom_pos = torch.randn(2, atom_seq_len, 3)
+distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
+
 # train
 
 loss = alphafold3(
     num_recycling_steps = 2,
     atom_inputs = atom_inputs,
     atom_mask = atom_mask,
     atompair_feats = atompair_feats,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
     templates = template_feats,
-    template_mask = template_mask
+    template_mask = template_mask,
+    atom_pos = atom_pos,
+    distance_labels = distance_labels
 )
 
 loss.backward()
 
+# after much training ...
+
+sampled_atom_pos = alphafold3(
+    num_recycling_steps = 4,
+    num_sample_steps = 16,
+    atom_inputs = atom_inputs,
+    atom_mask = atom_mask,
+    atompair_feats = atompair_feats,
+    additional_residue_feats = additional_residue_feats,
+    msa = msa,
+    templates = template_feats,
+    template_mask = template_mask
+)
+
+sampled_atom_pos.shape # (2, 16 * 27, 3)
 ```
 
 ## Citations
 
 ```bibtex
 @article{Abramson2024-fj,
   title    = "Accurate structure prediction of biomolecular interactions with
@@ -75,11 +101,11 @@
               Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin,
               Kuba and Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and
               Stecula, Adrian and Thillaisundaram, Ashok and Tong, Catherine
               and Yakneen, Sergei and Zhong, Ellen D and Zielinski, Michal and
               {\v Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet
               and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
   journal  = "Nature",
-  month    =  may,
+  month    = "May",
   year     =  2024
 }
 ```
```

#### html2text {}

```diff
@@ -1,31 +1,39 @@
 [./alphafold3.png]## Alphafold 3 - Pytorch (wip) Implementation of _A_l_p_h_a_f_o_l_d_ _3
 in Pytorch Getting a fair number of emails. You can chat with me about this
-work _h_e_r_e ## Install ```bash $ pip install alphafold3-pytorch ``` ## Usage
-```python import torch from alphafold3_pytorch import Alphafold3 alphafold3 =
-Alphafold3( dim_atom_inputs = 77, dim_additional_residue_feats = 33,
-dim_template_feats = 44 ) # mock inputs seq_len = 16 atom_seq_len = seq_len *
-27 atom_inputs = torch.randn(2, atom_seq_len, 77) atom_mask = torch.ones((2,
+work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for contributing the relative positional
+encoding module! ## Install ```bash $ pip install alphafold3-pytorch ``` ##
+Usage ```python import torch from alphafold3_pytorch import Alphafold3
+alphafold3 = Alphafold3( dim_atom_inputs = 77, dim_additional_residue_feats =
+33, dim_template_feats = 44 ) # mock inputs seq_len = 16 atom_seq_len = seq_len
+* 27 atom_inputs = torch.randn(2, atom_seq_len, 77) atom_mask = torch.ones((2,
 atom_seq_len)).bool() atompair_feats = torch.randn(2, atom_seq_len,
 atom_seq_len, 16) additional_residue_feats = torch.randn(2, seq_len, 33)
 template_feats = torch.randn(2, 2, seq_len, seq_len, 44) template_mask =
-torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) # train loss =
+torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) # required for
+training, but omitted on inference atom_pos = torch.randn(2, atom_seq_len, 3)
+distance_labels = torch.randint(0, 37, (2, seq_len, seq_len)) # train loss =
 alphafold3( num_recycling_steps = 2, atom_inputs = atom_inputs, atom_mask =
 atom_mask, atompair_feats = atompair_feats, additional_residue_feats =
 additional_residue_feats, msa = msa, templates = template_feats, template_mask
-= template_mask ) loss.backward() ``` ## Citations ```bibtex @article
-{Abramson2024-fj, title = "Accurate structure prediction of biomolecular
-interactions with {AlphaFold} 3", author = "Abramson, Josh and Adler, Jonas and
-Dunger, Jack and Evans, Richard and Green, Tim and Pritzel, Alexander and
-Ronneberger, Olaf and Willmore, Lindsay and Ballard, Andrew J and Bambrick,
-Joshua and Bodenstein, Sebastian W and Evans, David A and Hung, Chia-Chun and
-O'Neill, Michael and Reiman, David and Tunyasuvunakool, Kathryn and Wu, Zachary
-and {\v Z}emgulyt{\.e}, Akvil{\.e} and Arvaniti, Eirini and Beattie, Charles
-and Bertolli, Ottavia and Bridgland, Alex and Cherepanov, Alexey and Congreve,
-Miles and Cowen-Rivers, Alexander I and Cowie, Andrew and Figurnov, Michael and
-Fuchs, Fabian B and Gladman, Hannah and Jain, Rishub and Khan, Yousuf A and
-Low, Caroline M R and Perlin, Kuba and Potapenko, Anna and Savy, Pascal and
-Singh, Sukhdeep and Stecula, Adrian and Thillaisundaram, Ashok and Tong,
-Catherine and Yakneen, Sergei and Zhong, Ellen D and Zielinski, Michal and {\v
-Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet and Jaderberg, Max
-and Hassabis, Demis and Jumper, John M", journal = "Nature", month = may, year
-= 2024 } ```
+= template_mask, atom_pos = atom_pos, distance_labels = distance_labels )
+loss.backward() # after much training ... sampled_atom_pos = alphafold3
+( num_recycling_steps = 4, num_sample_steps = 16, atom_inputs = atom_inputs,
+atom_mask = atom_mask, atompair_feats = atompair_feats,
+additional_residue_feats = additional_residue_feats, msa = msa, templates =
+template_feats, template_mask = template_mask ) sampled_atom_pos.shape # (2, 16
+* 27, 3) ``` ## Citations ```bibtex @article{Abramson2024-fj, title = "Accurate
+structure prediction of biomolecular interactions with {AlphaFold} 3", author =
+"Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans, Richard and Green,
+Tim and Pritzel, Alexander and Ronneberger, Olaf and Willmore, Lindsay and
+Ballard, Andrew J and Bambrick, Joshua and Bodenstein, Sebastian W and Evans,
+David A and Hung, Chia-Chun and O'Neill, Michael and Reiman, David and
+Tunyasuvunakool, Kathryn and Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and
+Arvaniti, Eirini and Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex
+and Cherepanov, Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and
+Cowie, Andrew and Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and
+Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and
+Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and
+Thillaisundaram, Ashok and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen
+D and Zielinski, Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and
+Kohli, Pushmeet and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
+journal = "Nature", month = "May", year = 2024 } ```
```

### Comparing `alphafold3_pytorch-0.0.1/pyproject.toml` & `alphafold3_pytorch-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.0.1"
+version = "0.0.2"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
```

### Comparing `alphafold3_pytorch-0.0.1/PKG-INFO` & `alphafold3_pytorch-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
@@ -50,14 +50,18 @@
 
 ## Alphafold 3 - Pytorch (wip)
 
 Implementation of <a href="https://www.nature.com/articles/s41586-024-07487-w">Alphafold 3</a> in Pytorch
 
 Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
+## Appreciation
+
+- <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the relative positional encoding module!
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
@@ -83,29 +87,51 @@
 additional_residue_feats = torch.randn(2, seq_len, 33)
 
 template_feats = torch.randn(2, 2, seq_len, seq_len, 44)
 template_mask = torch.ones((2, 2)).bool()
 
 msa = torch.randn(2, 7, seq_len, 64)
 
+# required for training, but omitted on inference
+
+atom_pos = torch.randn(2, atom_seq_len, 3)
+distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
+
 # train
 
 loss = alphafold3(
     num_recycling_steps = 2,
     atom_inputs = atom_inputs,
     atom_mask = atom_mask,
     atompair_feats = atompair_feats,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
     templates = template_feats,
-    template_mask = template_mask
+    template_mask = template_mask,
+    atom_pos = atom_pos,
+    distance_labels = distance_labels
 )
 
 loss.backward()
 
+# after much training ...
+
+sampled_atom_pos = alphafold3(
+    num_recycling_steps = 4,
+    num_sample_steps = 16,
+    atom_inputs = atom_inputs,
+    atom_mask = atom_mask,
+    atompair_feats = atompair_feats,
+    additional_residue_feats = additional_residue_feats,
+    msa = msa,
+    templates = template_feats,
+    template_mask = template_mask
+)
+
+sampled_atom_pos.shape # (2, 16 * 27, 3)
 ```
 
 ## Citations
 
 ```bibtex
 @article{Abramson2024-fj,
   title    = "Accurate structure prediction of biomolecular interactions with
@@ -123,11 +149,11 @@
               Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin,
               Kuba and Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and
               Stecula, Adrian and Thillaisundaram, Ashok and Tong, Catherine
               and Yakneen, Sergei and Zhong, Ellen D and Zielinski, Michal and
               {\v Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet
               and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
   journal  = "Nature",
-  month    =  may,
+  month    = "May",
   year     =  2024
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.1 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.2 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -23,37 +23,45 @@
 Python :: 3.8 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8 Requires-Dist: beartype Requires-Dist:
 einops>=0.8.0 Requires-Dist: einx>=0.2.2 Requires-Dist: environs Requires-Dist:
 jaxtyping>=0.2.28 Requires-Dist: torch>=2.1 Requires-Dist: tqdm Provides-Extra:
 examples Provides-Extra: test Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown [./alphafold3.png]## Alphafold 3 -
 Pytorch (wip) Implementation of _A_l_p_h_a_f_o_l_d_ _3 in Pytorch Getting a fair number of
-emails. You can chat with me about this work _h_e_r_e ## Install ```bash $ pip
+emails. You can chat with me about this work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for
+contributing the relative positional encoding module! ## Install ```bash $ pip
 install alphafold3-pytorch ``` ## Usage ```python import torch from
 alphafold3_pytorch import Alphafold3 alphafold3 = Alphafold3( dim_atom_inputs =
 77, dim_additional_residue_feats = 33, dim_template_feats = 44 ) # mock inputs
 seq_len = 16 atom_seq_len = seq_len * 27 atom_inputs = torch.randn(2,
 atom_seq_len, 77) atom_mask = torch.ones((2, atom_seq_len)).bool()
 atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
 additional_residue_feats = torch.randn(2, seq_len, 33) template_feats =
 torch.randn(2, 2, seq_len, seq_len, 44) template_mask = torch.ones((2, 2)).bool
-() msa = torch.randn(2, 7, seq_len, 64) # train loss = alphafold3
+() msa = torch.randn(2, 7, seq_len, 64) # required for training, but omitted on
+inference atom_pos = torch.randn(2, atom_seq_len, 3) distance_labels =
+torch.randint(0, 37, (2, seq_len, seq_len)) # train loss = alphafold3
 ( num_recycling_steps = 2, atom_inputs = atom_inputs, atom_mask = atom_mask,
 atompair_feats = atompair_feats, additional_residue_feats =
 additional_residue_feats, msa = msa, templates = template_feats, template_mask
-= template_mask ) loss.backward() ``` ## Citations ```bibtex @article
-{Abramson2024-fj, title = "Accurate structure prediction of biomolecular
-interactions with {AlphaFold} 3", author = "Abramson, Josh and Adler, Jonas and
-Dunger, Jack and Evans, Richard and Green, Tim and Pritzel, Alexander and
-Ronneberger, Olaf and Willmore, Lindsay and Ballard, Andrew J and Bambrick,
-Joshua and Bodenstein, Sebastian W and Evans, David A and Hung, Chia-Chun and
-O'Neill, Michael and Reiman, David and Tunyasuvunakool, Kathryn and Wu, Zachary
-and {\v Z}emgulyt{\.e}, Akvil{\.e} and Arvaniti, Eirini and Beattie, Charles
-and Bertolli, Ottavia and Bridgland, Alex and Cherepanov, Alexey and Congreve,
-Miles and Cowen-Rivers, Alexander I and Cowie, Andrew and Figurnov, Michael and
-Fuchs, Fabian B and Gladman, Hannah and Jain, Rishub and Khan, Yousuf A and
-Low, Caroline M R and Perlin, Kuba and Potapenko, Anna and Savy, Pascal and
-Singh, Sukhdeep and Stecula, Adrian and Thillaisundaram, Ashok and Tong,
-Catherine and Yakneen, Sergei and Zhong, Ellen D and Zielinski, Michal and {\v
-Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet and Jaderberg, Max
-and Hassabis, Demis and Jumper, John M", journal = "Nature", month = may, year
-= 2024 } ```
+= template_mask, atom_pos = atom_pos, distance_labels = distance_labels )
+loss.backward() # after much training ... sampled_atom_pos = alphafold3
+( num_recycling_steps = 4, num_sample_steps = 16, atom_inputs = atom_inputs,
+atom_mask = atom_mask, atompair_feats = atompair_feats,
+additional_residue_feats = additional_residue_feats, msa = msa, templates =
+template_feats, template_mask = template_mask ) sampled_atom_pos.shape # (2, 16
+* 27, 3) ``` ## Citations ```bibtex @article{Abramson2024-fj, title = "Accurate
+structure prediction of biomolecular interactions with {AlphaFold} 3", author =
+"Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans, Richard and Green,
+Tim and Pritzel, Alexander and Ronneberger, Olaf and Willmore, Lindsay and
+Ballard, Andrew J and Bambrick, Joshua and Bodenstein, Sebastian W and Evans,
+David A and Hung, Chia-Chun and O'Neill, Michael and Reiman, David and
+Tunyasuvunakool, Kathryn and Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and
+Arvaniti, Eirini and Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex
+and Cherepanov, Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and
+Cowie, Andrew and Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and
+Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and
+Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and
+Thillaisundaram, Ashok and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen
+D and Zielinski, Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and
+Kohli, Pushmeet and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
+journal = "Nature", month = "May", year = 2024 } ```
```

